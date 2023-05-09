# Comparing `tmp/ratelimitx-0.0.1.tar.gz` & `tmp/ratelimitx-0.1.0.tar.gz`

## Comparing `ratelimitx-0.0.1.tar` & `ratelimitx-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/ratelimitx/__about__.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/ratelimitx/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/tests/test_multiratelimiter.py
--rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/tests/test_ratelimiter.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/README.md
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 ratelimitx-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/ratelimitx/__about__.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/ratelimitx/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5527 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/tests/test_multiratelimiter.py
+-rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/tests/test_ratelimiter.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/README.md
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ratelimitx-0.1.0/PKG-INFO
```

### Comparing `ratelimitx-0.0.1/ratelimitx/__init__.py` & `ratelimitx-0.1.0/ratelimitx/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,161 @@
 import asyncio
 from dataclasses import dataclass
+from datetime import datetime
 import time
+from typing import Optional
 
 from redis.asyncio import Redis
 
 
+@dataclass(order=True)
+class RetryAfter:
+    date: datetime
+    seconds: float
+
+
 @dataclass
-class RateLimiter:
+class RateLimitError(Exception):
+    retry_after: RetryAfter
 
+
+@dataclass
+class RateLimiter:
     client: Redis
-    identifier: str
-    duration: int
+    window_length: int
     n: int
-    prefix: str = "ratelimitx"
+    prefix: Optional[str] = None
     delimiter: str = "|"
 
-    @property
-    def key(self) -> str:
-        """
-            Returns the key that will be used to store the data into Redis.
-        """
-        return self.delimiter.join([self.prefix, self.identifier, str(self.duration)])
+    def _build_key(self, identifier: str) -> str:
+        if self.prefix is None:
+            return self.delimiter.join([identifier, str(self.window_length)])
+        return self.delimiter.join([self.prefix, identifier, str(self.window_length)])
 
-    @property
-    def retry_after(self) -> int:
+    async def rate_limit(
+        self,
+        identifier: str,
+        timestamp: Optional[float] = None,
+        add_timestamp: bool = True,
+    ):
         """
-            Return the amount of time in seconds before a retry is allowed.
+        Raise a RateLimitError if rate limited.
         """
-        return getattr(self, '_retry_after', 0)
-
-    async def __call__(self, timestamp: float | None = None, add_timestamp: bool = True):
         if timestamp is None:
             timestamp = time.time()
 
-        count, least_recent_timestamp = await self.slide_window(timestamp)
-        if count < self.n:
-            self._retry_after = 0
-            if add_timestamp:
-                await self.add_timestamp(timestamp)
-            return True
-
-        self._retry_after = self.duration - (timestamp - least_recent_timestamp)
-        return False
-
-    async def slide_window(self, timestamp: float | None = None) -> tuple[int, float | None]:
-        """
-            Remove expired timestamps (slides the window).
-            Returns a tuple containing the number of unexpired timestamps
-            and the least recent timestamp if applicable or None.
+        count, least_recent_timestamp = await self.slide_window(identifier, timestamp)
+        if count >= self.n:
+            seconds = self.window_length - (timestamp - least_recent_timestamp)
+            date = datetime.fromtimestamp(timestamp + seconds)
+            retry_after = RetryAfter(date=date, seconds=seconds)
+            raise RateLimitError(retry_after)
+
+        if add_timestamp:
+            await self.add_timestamp(identifier, timestamp)
+
+    async def slide_window(
+        self, identifier: str, timestamp: Optional[float] = None
+    ) -> tuple[int, Optional[float]]:
+        """
+        Remove expired timestamps (slides the window).
+        Returns a tuple containing the number of unexpired timestamps
+        and the least recent timestamp if applicable or None.
         """
+        key = self._build_key(identifier)
         if timestamp is None:
             timestamp = time.time()
 
         pipeline = self.client.pipeline()
 
         # Remove expired timestamps.
-        pipeline.zremrangebyscore(self.key, min=0, max=timestamp - self.duration)
+        pipeline.zremrangebyscore(key, min=0, max=timestamp - self.window_length)
 
         # Count the amount of timestamps remaining.
-        pipeline.zcount(self.key, min=0, max=timestamp)
+        pipeline.zcount(key, min=0, max=timestamp)
 
         # Get the lowest ranked score. (least recent timestamp)
-        pipeline.zrange(self.key, start=0, end=0)
+        pipeline.zrange(key, start=0, end=0)
 
         _, count, scores = await pipeline.execute()
         return count, float(scores[0]) if scores else None
 
-    async def add_timestamp(self, timestamp: float | None = None):
+    async def add_timestamp(self, identifier: str, timestamp: Optional[float] = None):
         """
-            Adds a timestamp and updates the expiration.
+        Adds a timestamp and updates the expiration.
         """
+        key = self._build_key(identifier)
         if timestamp is None:
             timestamp = time.time()
 
         pipeline = self.client.pipeline()
-        pipeline.zadd(self.key, {timestamp: timestamp})
-        pipeline.expire(self.key, self.duration)
+        pipeline.zadd(key, {timestamp: timestamp})
+        pipeline.expire(key, self.window_length)
         await pipeline.execute()
 
 
 @dataclass
 class MultiRateLimiter:
     rate_limiters: list[RateLimiter]
 
     @classmethod
-    def from_mapping(cls, client: Redis, identifier: str, mapping: dict[int, int]):
+    def from_mapping(cls, client: Redis, mapping: dict[int, int]):
         """
-            Creates a new multi-ratelimiter by creating new rate limiter objects
-            from a mapping containing durations for keys and units for values.
+        Creates a new multi-ratelimiter by creating new rate limiter objects
+        from a mapping containing window lengths for keys and units for values.
         """
         rate_limiters = [
-            RateLimiter(client, identifier, duration, n) for duration, n in mapping.items()
+            RateLimiter(client, window_length, n)
+            for window_length, n in mapping.items()
         ]
         return cls(rate_limiters)
 
     @classmethod
     def new(
         cls,
         client: Redis,
-        identifier: str,
-        per_second: int | None = None,
-        per_minute: int | None = None,
-        per_hour: int | None = None,
-        per_day: int | None = None
+        per_second: Optional[int] = None,
+        per_minute: Optional[int] = None,
+        per_hour: Optional[int] = None,
+        per_day: Optional[int] = None,
     ):
         """
-            Creates a new multi-ratelimiter by specifying the number
-            of units for each unit of time.
+        Creates a new multi-ratelimiter by specifying the number
+        of units for each unit of time.
         """
         assert any([per_second, per_minute, per_hour, per_day])
         mapping = {}
         if per_second is not None:
             mapping[1] = per_second
 
         if per_minute is not None:
             mapping[60] = per_minute
 
         if per_hour is not None:
-            mapping[60*60] = per_hour
+            mapping[3600] = per_hour
 
         if per_day is not None:
-            mapping[24*60*60] = per_day
-
-        return cls.from_mapping(client, identifier, mapping)
-
-    @property
-    def retry_after(self) -> int:
-        return getattr(self, '_retry_after', None)
-
-    async def __call__(self, timestamp: float | None = None):
-        if timestamp is None:
-            timestamp = time.time()
-
-        coroutines = [rl(timestamp, add_timestamp=False) for rl in self.rate_limiters]
-        results = await asyncio.gather(*coroutines)
-        success = all(results)
-
-        if success:
-            self._retry_after = 0
-            await self.add_timstamps(timestamp)
+            mapping[86400] = per_day
 
-        self._retry_after = max([rl.retry_after for rl in self.rate_limiters])
-        return success
+        return cls.from_mapping(client, mapping)
 
-    async def add_timstamps(self, timestamp: float | None = None):
+    async def rate_limit(self, identifier: str, timestamp: Optional[float] = None):
         if timestamp is None:
             timestamp = time.time()
 
-        coroutines = [rl.add_timestamp(timestamp) for rl in self.rate_limiters]
+        # Perform rate-limiting on each rate limiter.
+        coroutines = [
+            rl.rate_limit(identifier, timestamp, add_timestamp=False) for rl in self.rate_limiters
+        ]
+        results = await asyncio.gather(*coroutines, return_exceptions=True)
+        errors = [result for result in results if isinstance(result, RateLimitError)]
+        if errors:
+            # If there are any errors then find the max retry after
+            # and raise a RateLimitError.
+            retry_after = max(error.retry_after for error in errors)
+            raise RateLimitError(retry_after)
+
+        # Add timestamps.
+        coroutines = [
+            rl.add_timestamp(identifier, timestamp) for rl in self.rate_limiters
+        ]
         await asyncio.gather(*coroutines)
```

### Comparing `ratelimitx-0.0.1/tests/test_ratelimiter.py` & `ratelimitx-0.1.0/tests/test_multiratelimiter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,207 +1,161 @@
+from collections.abc import Iterable
+from datetime import datetime
 import time
 
 import pytest
 import pytest_asyncio
 from redis.asyncio import Redis
 
-from ratelimitx import RateLimiter
+from ratelimitx import MultiRateLimiter, RateLimiter, RateLimitError
 
 
 @pytest_asyncio.fixture
 async def client():
     client = Redis()
     await client.flushdb()
     return client
 
 
-def test_ratelimiter_key(client):
-    # test default
-    limiter = RateLimiter(
-        client=client,
-        identifier="test",
-        duration=60,
-        n=5
+def test_from_mapping(client):
+    mapping = {1: 1, 60: 2, 3_600: 3, 86_400: 5}
+
+    multilimiter = MultiRateLimiter.from_mapping(
+        client=client, mapping=mapping
     )
 
-    assert limiter.key == "ratelimit|test|60"
+    assert len(multilimiter.rate_limiters) == 4
 
-    # Test custom prefix
-    limiter = RateLimiter(
-        client=client,
-        identifier="test",
-        duration=60,
-        n=5,
-        prefix="prefix"
-    )
+    limiter_one = RateLimiter(client=client, window_length=1, n=1)
+    assert multilimiter.rate_limiters[0] == limiter_one
 
-    assert limiter.key == "prefix|test|60"
+    limiter_two = RateLimiter(client=client, window_length=60, n=2)
+    assert multilimiter.rate_limiters[1] == limiter_two
 
-    # Test custom deilimiter.
-    limiter = RateLimiter(
-        client=client,
-        identifier="test",
-        duration=60,
-        n=5,
-        delimiter=":"
-    )
+    limiter_three = RateLimiter(client=client, window_length=3600, n=3)
+    assert multilimiter.rate_limiters[2] == limiter_three
 
-    assert limiter.key == "ratelimit:test:60"
+    limiter_four = RateLimiter(client=client, window_length=86_400, n=5)
+    assert multilimiter.rate_limiters[3] == limiter_four
 
 
-@pytest.mark.asyncio
-async def test_add_timestamp(client):
-    limiter = RateLimiter(
-        client=client, identifier="test", duration=60, n=5
+def test_new_one(client):
+    multilimiter = MultiRateLimiter.new(
+        client=client, per_second=1, per_minute=2
     )
 
-    await limiter.add_timestamp()
-    
-    # Confirm that the ttl was set.
-    assert await client.ttl(limiter.key) == limiter.duration
+    assert len(multilimiter.rate_limiters) == 2
 
-    # confirm that a single timestamp was added.
-    assert await client.zcount(limiter.key, min=0, max=time.time()) == 1
+    second_limiter = RateLimiter(client=client, window_length=1, n=1)
+    assert multilimiter.rate_limiters[0] == second_limiter
 
+    minute_limiter = RateLimiter(client=client, window_length=60, n=2)
+    assert multilimiter.rate_limiters[1] == minute_limiter
 
-@pytest.mark.asyncio
-async def test_slide_window_one(client):
-    limiter = RateLimiter(
-        client=client, identifier="test", duration=60, n=5
+
+def test_new_two(client):
+    multilimiter = MultiRateLimiter.new(
+        client=client, per_hour=3, per_day=5
     )
 
-    # Test running slide_window() without adding any timestamps.
-    ts = time.time()
-    count, least_recent_timestamp = await limiter.slide_window(ts)
-    assert count == 0
-    assert least_recent_timestamp is None
+    assert len(multilimiter.rate_limiters) == 2
 
+    hour_limiter = RateLimiter(client=client, window_length=3_600, n=3)
+    assert multilimiter.rate_limiters[0] == hour_limiter
 
-@pytest.mark.asyncio
-async def test_slide_window_two(client):
-    limiter = RateLimiter(
-        client=client, identifier="test", duration=60, n=5
+    day_limiter = RateLimiter(client=client, window_length=86_400, n=5)
+    assert multilimiter.rate_limiters[1] == day_limiter
+
+
+def test_new_four(client):
+    multilimiter = MultiRateLimiter.new(
+        client=client, per_second=1, per_minute=2, per_hour=3, per_day=5
     )
 
-    # test to make sure that a timestamp will show up in the window.
-    ts = time.time()
-    await limiter.add_timestamp(ts)
-
-    count, least_recent_timestamp = await limiter.slide_window(ts)
-    assert count == 1
-    assert least_recent_timestamp == ts
+    assert len(multilimiter.rate_limiters) == 4
 
+    second_limiter = RateLimiter(client=client, window_length=1, n=1)
+    assert multilimiter.rate_limiters[0] == second_limiter
+
+    minute_limiter = RateLimiter(client=client, window_length=60, n=2)
+    assert multilimiter.rate_limiters[1] == minute_limiter
+
+    hour_limiter = RateLimiter(client=client, window_length=3_600, n=3)
+    assert multilimiter.rate_limiters[2] == hour_limiter
+
+    day_limiter = RateLimiter(client=client, window_length=86_400, n=5)
+    assert multilimiter.rate_limiters[3] == day_limiter
 
-@pytest.mark.asyncio
-async def test_slide_window_three(client):
-    limiter = RateLimiter(
-        client=client, identifier="test", duration=60, n=5
-    )
 
-    # Test to make sure that a timestamp will slide out of the window
-    start = time.time()
-    await limiter.add_timestamp(start)
-
-    # 59 seconds later (one second before the window)
-    ts = start + 59
-
-    count, least_recent_timestamp = await limiter.slide_window(ts)
-    assert count == 1
-    assert least_recent_timestamp == start
-
-    # 60 seconds later, the timestamp is no longer in the window.
-    ts = start + 60
-    count, least_recent_timestamp = await limiter.slide_window(ts)
-    assert count == 0
-    assert least_recent_timestamp == None
+def timsim(duration_secs: int, step: float) -> Iterable[tuple[float, float]]:
+    """
+        Time Simulator (timsim)
+        A generator that simulates time.
+        duration_secs: The total duration to be simulated in seconds.
+        step: The amount of time that passes per iteration.
+        returns: A tuple containing the timestamp and the elapsed time.
+    """
+    elapsed_time = 0
+    start_time = time.time()
+    while elapsed_time <= duration_secs:
+        yield start_time + elapsed_time, elapsed_time
+        elapsed_time += step
 
 
 @pytest.mark.asyncio
-async def test_slide_window_four(client):
-    limiter = RateLimiter(
-        client=client, identifier="test", duration=60, n=5
+async def test_rate_limit(client):
+    multilimiter = MultiRateLimiter.new(
+        client=client, per_second=1, per_minute=6
     )
 
-    # make sure that the least recent timestamp is accurate over time.
+    # simulate every half second in the span of two minutes.
+    for ts, time_elapsed in timsim(120, .5):
 
-    start = time.time()
-    await limiter.add_timestamp(start)
+        # add some valid requests.
+        if time_elapsed in (0, 2, 4, 6, 8, 10, 60, 65, 70, 75, 80, 85):
+            await multilimiter.rate_limit("test", ts)
 
-    fifteen = start + 15
-    await limiter.add_timestamp(fifteen)
+        # ~~~ Test for specific scenarios that will be rate limited. ~~~
 
-    thirty = start + 30
-    await limiter.add_timestamp(thirty)
-
-    fourty_five = start + 45
-    await limiter.add_timestamp(fourty_five)
-
-    # check results of slide_window at the 45th second.
-    count, least_recent_timestamp = await limiter.slide_window(fourty_five)
-    assert count == 4
-    assert least_recent_timestamp == start
-
-    # Confirm that at the 60th second, the first ts is no longer in the window,
-    # thus making the count 3, and the least recent timestamp to be fifteen.
-    sixty = start + 60
-    count, least_recent_timestamp = await limiter.slide_window(sixty)
-    assert count == 3
-    assert least_recent_timestamp == fifteen
-
-    seventy_five = start + 75
-    count, least_recent_timestamp = await limiter.slide_window(seventy_five)
-    assert count == 2
-    assert least_recent_timestamp == thirty
-
-    ninety = start + 90
-    count, least_recent_timestamp = await limiter.slide_window(ninety)
-    assert count == 1
-    assert least_recent_timestamp == fourty_five
+        if time_elapsed == 0.5:
+            # Test seconds rate limiter
+            with pytest.raises(RateLimitError) as exc_info:
+                await multilimiter.rate_limit("test", ts)
+            
+            retry_after = exc_info.value.retry_after
+            assert retry_after.seconds == .5
+            assert retry_after.date == datetime.fromtimestamp(ts + .5)
 
+        if time_elapsed == 10.5:
+            # This will be stopped by both rate limiters.
+            # make sure that the retry after with the max date
+            # is returned.
+            with pytest.raises(RateLimitError) as exc_info:
+                await multilimiter.rate_limit("test", ts)
+            
+            retry_after = exc_info.value.retry_after
+            assert retry_after.seconds == 49.5
+            assert retry_after.date == datetime.fromtimestamp(ts + 49.5)
+        
+        if time_elapsed == 11:
+            with pytest.raises(RateLimitError) as exc_info:
+                await multilimiter.rate_limit("test", ts)
 
-@pytest.mark.asyncio
-async def test_ratelimit(client):
-    limiter = RateLimiter(
-        client=client, identifier="test", duration=60, n=3
-    )
+            retry_after = exc_info.value.retry_after
+            assert retry_after.seconds == 49
+            assert retry_after.date == datetime.fromtimestamp(ts + 49)
+
+        if time_elapsed == 60.5:
+            with pytest.raises(RateLimitError) as exc_info:
+                await multilimiter.rate_limit("test", ts)
+
+            retry_after = exc_info.value.retry_after
+            assert retry_after.seconds == 1.5
+            assert retry_after.date == datetime.fromtimestamp(ts + 1.5)
 
-    start = time.time()
+        if time_elapsed == 70.5:
+            with pytest.raises(RateLimitError) as exc_info:
+                await multilimiter.rate_limit("test", ts)
 
-    result = await limiter(start)
-    assert result == True
-    assert limiter.retry_after == 0
-
-    # 15 seconds later
-    fifteen = start + 15
-    result = await limiter(fifteen)
-    assert result == True
-    assert limiter.retry_after == 0
-
-    # 30 seconds later
-    thirty = start + 30
-    result = await limiter(thirty)
-    assert result == True
-    assert limiter.retry_after == 0
-
-    # 45 seconds later
-    forty_five = start + 45
-    result = await limiter(forty_five)
-    assert result == False
-    assert limiter.retry_after == 15
-
-    # 59 seconds later
-    fifty_nine = start + 59
-    result = await limiter(fifty_nine)
-    assert result == False
-    assert limiter.retry_after == 1
-
-    # 60 seconds later
-    sixty = start + 60
-    result = await limiter(sixty)
-    assert result == True
-    assert limiter.retry_after == 0
-
-    # 61 seconds later
-    sixty_one = start + 61
-    result = await limiter(sixty_one)
-    assert result == False
-    assert limiter.retry_after == 14
+            retry_after = exc_info.value.retry_after
+            assert retry_after.seconds == 0.5
+            assert retry_after.date == datetime.fromtimestamp(ts + 0.5)
```

### Comparing `ratelimitx-0.0.1/.gitignore` & `ratelimitx-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ratelimitx-0.0.1/LICENSE.txt` & `ratelimitx-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ratelimitx-0.0.1/PKG-INFO` & `ratelimitx-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: ratelimitx
-Version: 0.0.1
-Project-URL: Documentation, https://github.com/unknown/ratelimitx#readme
-Project-URL: Issues, https://github.com/unknown/ratelimitx/issues
-Project-URL: Source, https://github.com/unknown/ratelimitx
+Version: 0.1.0
+Project-URL: Documentation, https://github.com/rykroon/ratelimitx#readme
+Project-URL: Issues, https://github.com/rykroon/ratelimitx/issues
+Project-URL: Source, https://github.com/rykroon/ratelimitx
 Author-email: Ryan Kroon <rykroon.tech@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Requires-Dist: redis==4.5.*
+Requires-Python: >=3.9
+Requires-Dist: redis>=4.4
 Description-Content-Type: text/markdown
 
 # ratelimitx
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ratelimitx.svg)](https://pypi.org/project/ratelimitx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ratelimitx.svg)](https://pypi.org/project/ratelimitx)
```

