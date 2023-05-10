# Comparing `tmp/diffcord-1.0.2.tar.gz` & `tmp/diffcord-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffcord-1.0.2.tar", last modified: Tue May  9 20:08:00 2023, max compression
+gzip compressed data, was "diffcord-1.0.3.tar", last modified: Wed May 10 01:17:32 2023, max compression
```

## Comparing `diffcord-1.0.2.tar` & `diffcord-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 20:08:00.342915 diffcord-1.0.2/
--rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2607 2023-05-09 20:08:00.341915 diffcord-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-08 22:12:05.000000 diffcord-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 20:08:00.326913 diffcord-1.0.2/diffcord/
--rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-1.0.2/diffcord/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-1.0.2/diffcord/api.py
--rw-rw-rw-   0        0        0     7224 2023-05-09 20:02:04.000000 diffcord-1.0.2/diffcord/client.py
--rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-1.0.2/diffcord/error.py
--rw-rw-rw-   0        0        0     3397 2023-05-08 22:11:45.000000 diffcord-1.0.2/diffcord/vote.py
-drwxrwxrwx   0        0        0        0 2023-05-09 20:08:00.335912 diffcord-1.0.2/diffcord.egg-info/
--rw-rw-rw-   0        0        0     2607 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 20:08:00.000000 diffcord-1.0.2/diffcord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 20:08:00.342915 diffcord-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-05-09 20:07:55.000000 diffcord-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 20:08:00.340915 diffcord-1.0.2/tests/
--rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-1.0.2/tests/test_client.py
--rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-1.0.2/tests/test_webhook_listener.py
--rw-rw-rw-   0        0        0      216 2023-05-09 20:03:08.000000 diffcord-1.0.2/tests/testing_main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:17:32.486456 diffcord-1.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-03-12 19:55:56.000000 diffcord-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2607 2023-05-10 01:17:32.486456 diffcord-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-08 22:12:05.000000 diffcord-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 01:17:32.435455 diffcord-1.0.3/diffcord/
+-rw-rw-rw-   0        0        0       86 2023-03-12 21:51:54.000000 diffcord-1.0.3/diffcord/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-05-07 20:08:24.000000 diffcord-1.0.3/diffcord/api.py
+-rw-rw-rw-   0        0        0     7214 2023-05-10 01:15:02.000000 diffcord-1.0.3/diffcord/client.py
+-rw-rw-rw-   0        0        0     2111 2023-03-20 16:51:23.000000 diffcord-1.0.3/diffcord/error.py
+-rw-rw-rw-   0        0        0     3397 2023-05-08 22:11:45.000000 diffcord-1.0.3/diffcord/vote.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:17:32.470455 diffcord-1.0.3/diffcord.egg-info/
+-rw-rw-rw-   0        0        0     2607 2023-05-10 01:17:32.000000 diffcord-1.0.3/diffcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-05-10 01:17:32.000000 diffcord-1.0.3/diffcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:17:32.000000 diffcord-1.0.3/diffcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 01:17:32.000000 diffcord-1.0.3/diffcord.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-05-10 01:17:32.000000 diffcord-1.0.3/diffcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 01:17:32.000000 diffcord-1.0.3/diffcord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 01:17:32.487457 diffcord-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-05-10 01:16:36.000000 diffcord-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:17:32.484455 diffcord-1.0.3/tests/
+-rw-rw-rw-   0        0        0      108 2023-03-20 14:33:45.000000 diffcord-1.0.3/tests/test_client.py
+-rw-rw-rw-   0        0        0     4232 2023-05-08 19:50:49.000000 diffcord-1.0.3/tests/test_webhook_listener.py
+-rw-rw-rw-   0        0        0      183 2023-05-10 01:15:55.000000 diffcord-1.0.3/tests/testing_main.py
```

### Comparing `diffcord-1.0.2/LICENSE` & `diffcord-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.2/PKG-INFO` & `diffcord-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `diffcord-1.0.2/README.md` & `diffcord-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.2/diffcord/api.py` & `diffcord-1.0.3/diffcord/api.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.2/diffcord/client.py` & `diffcord-1.0.3/diffcord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     def __init__(self, bot: Any, token: str, vote_listener: VoteWebhookListener, send_stats: bool = True,
                  send_stats_success: Callable[[], Awaitable[None]] = None,
                  send_stats_failure: Callable[[Exception], Awaitable[None]] = None,
                  base_url: str = None,
                  send_stats_interval: datetime.timedelta = None,
                  ) -> None:
-        super().__init__(token, "https://diffcord.com/api" if base_url is None else base_url)
+        super().__init__(token, "https://www.diffcord.com/api" if base_url is None else base_url)
 
         self.bot: Any = bot
         """ The bot object. """
 
         self.token: str = token
         """ The Diffcord API token. """
 
@@ -182,15 +182,15 @@
                 else:
                     if self.send_stats_success is not None:
                         await self.send_stats_success()
 
                 await asyncio.sleep(self.send_stats_interval.total_seconds())
 
     def start(self) -> Task:
-        """ Start the client synchronously.
+        """ Start the client.
         """
         return asyncio.ensure_future(self.__start())
 
     def __repr__(self):
         return f"<Client bot={self.bot} token={self.token}>"
 
     def __str__(self):
```

### Comparing `diffcord-1.0.2/diffcord/error.py` & `diffcord-1.0.3/diffcord/error.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.2/diffcord/vote.py` & `diffcord-1.0.3/diffcord/vote.py`

 * *Files identical despite different names*

### Comparing `diffcord-1.0.2/diffcord.egg-info/PKG-INFO` & `diffcord-1.0.3/diffcord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffcord
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python wrapper for the Diffcord API written in Python.
 Author: jadelasmar4@gmail.com
 Project-URL: Github, https://github.com/diff-cord/python-sdk
 Keywords: diffcord,diffcord-api,diffcord-api-wrapper,diffcord-api-python-wrapper,diffcord-api-python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `diffcord-1.0.2/setup.py` & `diffcord-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name='diffcord',
-    version='1.0.2',
+    version='1.0.3',
     description="A Python wrapper for the Diffcord API written in Python.",
     packages=find_packages(),
     author='jadelasmar4@gmail.com',
     zip_safe=False,
     install_requires=requirements,
     python_requires='>=3.7.0',
     long_description_content_type="text/markdown",
```

### Comparing `diffcord-1.0.2/tests/test_webhook_listener.py` & `diffcord-1.0.3/tests/test_webhook_listener.py`

 * *Files identical despite different names*

