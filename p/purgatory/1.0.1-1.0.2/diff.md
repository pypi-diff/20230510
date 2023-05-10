# Comparing `tmp/purgatory-1.0.1.tar.gz` & `tmp/purgatory-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purgatory-1.0.1.tar", max compression
+gzip compressed data, was "purgatory-1.0.2.tar", max compression
```

## Comparing `purgatory-1.0.1.tar` & `purgatory-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0     1523 2021-12-28 07:38:48.830707 purgatory-1.0.1/LICENSE
--rw-r--r--   0        0        0     3314 2022-01-04 12:22:12.260583 purgatory-1.0.1/README.rst
--rw-r--r--   0        0        0     1612 2022-05-28 13:41:12.616497 purgatory-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1199 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/__init__.py
--rw-r--r--   0        0        0        0 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/domain/__init__.py
--rw-r--r--   0        0        0       85 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/domain/messages/__init__.py
--rw-r--r--   0        0        0      304 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/domain/messages/base.py
--rw-r--r--   0        0        0      221 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/domain/messages/commands.py
--rw-r--r--   0        0        0      554 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/domain/messages/events.py
--rw-r--r--   0        0        0     7510 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/domain/model.py
--rw-r--r--   0        0        0        0 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/py.typed
--rw-r--r--   0        0        0        0 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/service/__init__.py
--rw-r--r--   0        0        0        0 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/service/_async/__init__.py
--rw-r--r--   0        0        0     5795 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/service/_async/circuitbreaker.py
--rw-r--r--   0        0        0     1633 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/service/_async/message_handlers.py
--rw-r--r--   0        0        0     3723 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/service/_async/messagebus.py
--rw-r--r--   0        0        0     4592 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/service/_async/repository.py
--rw-r--r--   0        0        0     1833 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/service/_async/unit_of_work.py
--rw-r--r--   0        0        0      269 2022-02-27 11:30:02.810013 purgatory-1.0.1/src/purgatory/service/_redis.py
--rw-r--r--   0        0        0        0 2022-05-28 13:41:07.606515 purgatory-1.0.1/src/purgatory/service/_sync/__init__.py
--rw-r--r--   0        0        0     5663 2022-05-28 13:41:07.613182 purgatory-1.0.1/src/purgatory/service/_sync/circuitbreaker.py
--rw-r--r--   0        0        0     1573 2022-05-28 13:41:08.206513 purgatory-1.0.1/src/purgatory/service/_sync/message_handlers.py
--rw-r--r--   0        0        0     3692 2022-05-28 13:41:07.616515 purgatory-1.0.1/src/purgatory/service/_sync/messagebus.py
--rw-r--r--   0        0        0     4405 2022-05-28 13:41:08.253180 purgatory-1.0.1/src/purgatory/service/_sync/repository.py
--rw-r--r--   0        0        0     1746 2022-05-28 13:41:07.619849 purgatory-1.0.1/src/purgatory/service/_sync/unit_of_work.py
--rw-r--r--   0        0        0      945 2022-02-27 11:30:02.813346 purgatory-1.0.1/src/purgatory/service/typing.py
--rw-r--r--   0        0        0      383 2022-02-27 11:30:02.813346 purgatory-1.0.1/src/purgatory/typing.py
--rw-r--r--   0        0        0     4333 2022-05-28 13:42:09.550686 purgatory-1.0.1/setup.py
--rw-r--r--   0        0        0     4366 2022-05-28 13:42:09.551024 purgatory-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1523 2021-12-28 07:38:48.830707 purgatory-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3314 2022-01-04 12:22:12.260583 purgatory-1.0.2/README.rst
+-rw-r--r--   0        0        0     1559 2023-05-10 11:38:05.322742 purgatory-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1199 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/__init__.py
+-rw-r--r--   0        0        0       85 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/messages/__init__.py
+-rw-r--r--   0        0        0      304 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/messages/base.py
+-rw-r--r--   0        0        0      221 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/messages/commands.py
+-rw-r--r--   0        0        0      554 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/messages/events.py
+-rw-r--r--   0        0        0     7510 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/domain/model.py
+-rw-r--r--   0        0        0        0 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/py.typed
+-rw-r--r--   0        0        0        0 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/__init__.py
+-rw-r--r--   0        0        0     5795 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/circuitbreaker.py
+-rw-r--r--   0        0        0     1633 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/message_handlers.py
+-rw-r--r--   0        0        0     3723 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/messagebus.py
+-rw-r--r--   0        0        0     4614 2023-05-10 11:37:55.332762 purgatory-1.0.2/src/purgatory/service/_async/repository.py
+-rw-r--r--   0        0        0     1833 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/_async/unit_of_work.py
+-rw-r--r--   0        0        0      274 2023-05-10 11:37:55.332762 purgatory-1.0.2/src/purgatory/service/_redis.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:38:00.232752 purgatory-1.0.2/src/purgatory/service/_sync/__init__.py
+-rw-r--r--   0        0        0     5663 2023-05-10 11:38:00.239419 purgatory-1.0.2/src/purgatory/service/_sync/circuitbreaker.py
+-rw-r--r--   0        0        0     1573 2023-05-10 11:38:00.866084 purgatory-1.0.2/src/purgatory/service/_sync/message_handlers.py
+-rw-r--r--   0        0        0     3692 2023-05-10 11:38:00.242752 purgatory-1.0.2/src/purgatory/service/_sync/messagebus.py
+-rw-r--r--   0        0        0     4433 2023-05-10 11:38:00.899418 purgatory-1.0.2/src/purgatory/service/_sync/repository.py
+-rw-r--r--   0        0        0     1746 2023-05-10 11:38:00.242752 purgatory-1.0.2/src/purgatory/service/_sync/unit_of_work.py
+-rw-r--r--   0        0        0      945 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/service/typing.py
+-rw-r--r--   0        0        0      383 2022-05-29 11:59:12.982727 purgatory-1.0.2/src/purgatory/typing.py
+-rw-r--r--   0        0        0     4379 1970-01-01 00:00:00.000000 purgatory-1.0.2/PKG-INFO
```

### Comparing `purgatory-1.0.1/LICENSE` & `purgatory-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/README.rst` & `purgatory-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/pyproject.toml` & `purgatory-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -12,52 +12,50 @@
 homepage = "https://github.com/mardiros/purgatory"
 license = "BSD-derived"
 name = "purgatory"
 packages = [
   {include = "purgatory", from = "src"},
 ]
 readme = "README.rst"
-version = "1.0.1"
+version = "1.0.2"
 
 [tool.pyright]
 include = ["src"]
 typeCheckingMode = "strict"
 
 [[tool.mypy.overrides]]
 module = "purgatory.*"
 disallow_untyped_defs = true
 disallow_any_generics = true
 
 [tool.poetry.dependencies]
 python = "^3.7"
-aioredis = {version = "^2.0.1", optional = true}
-redis = {version = "^4.1.0", optional = true}
+redis = {version = "^4.2.0", optional = true}
 
 [tool.poetry.extras]
-aioredis = ["aioredis"]
+aioredis = ["redis"]  # kept for compat
 redis = ["redis"]
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 coverage = {version = "^6.2", extras = ["toml"]}
-flake8 = "^4.0.1"
-isort = "^5.9.3"
-pytest = "^7.1.2"
-pytest-asyncio = "^0.18.3"
-pytest-cov = "^3.0.0"
-aioredis = "^2.0.1"
+flake8 = "^5.0.4"
+isort = "^5.10.1"
+pytest = "^7.1.3"
+pytest-asyncio = "^0.20.1"
+pytest-cov = "^4.0.0"
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
 tomlkit = "^0.11.0"
 unasync = "^0.5.0"
-redis = "^4.1.0"
-mypy = "^0.960"
-typing-extensions = "^4.0.1"
-types-redis = "^4.1.8"
-types-setuptools = "^57.4.7"
+redis = "^4.2.0"
+mypy = "^1.2"
+typing-extensions = "^4.4.0"
+types-redis = "^4.3.21"
+types-setuptools = "^65.5.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.coverage.report]
 exclude_lines = [
   "except ImportError:",
```

### Comparing `purgatory-1.0.1/src/purgatory/__init__.py` & `purgatory-1.0.2/src/purgatory/__init__.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/domain/messages/events.py` & `purgatory-1.0.2/src/purgatory/domain/messages/events.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/domain/model.py` & `purgatory-1.0.2/src/purgatory/domain/model.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/_async/circuitbreaker.py` & `purgatory-1.0.2/src/purgatory/service/_async/circuitbreaker.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/_async/message_handlers.py` & `purgatory-1.0.2/src/purgatory/service/_async/message_handlers.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/_async/messagebus.py` & `purgatory-1.0.2/src/purgatory/service/_async/messagebus.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/_async/repository.py` & `purgatory-1.0.2/src/purgatory/service/_async/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     async def reset_failure(self, name: str) -> None:
         """Reset the number of failure in the repository."""
 
 
 class AsyncRedisRepository(AsyncAbstractRepository):
     def __init__(self, url: str) -> None:
         try:
-            import aioredis
+            from redis import asyncio as aioredis
         except ImportError:
             raise ConfigurationError("redis extra dependencies not installed.")
         self.redis: AsyncRedis = aioredis.from_url(url)  # type: ignore
         self.messages = []
         self.prefix = "cbr::"
 
     async def initialize(self) -> None:
```

### Comparing `purgatory-1.0.1/src/purgatory/service/_async/unit_of_work.py` & `purgatory-1.0.2/src/purgatory/service/_async/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/_sync/circuitbreaker.py` & `purgatory-1.0.2/src/purgatory/service/_sync/circuitbreaker.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/_sync/message_handlers.py` & `purgatory-1.0.2/src/purgatory/service/_sync/message_handlers.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/_sync/messagebus.py` & `purgatory-1.0.2/src/purgatory/service/_sync/messagebus.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/_sync/repository.py` & `purgatory-1.0.2/src/purgatory/service/_sync/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,18 @@
     def reset_failure(self, name: str) -> None:
         """Reset the number of failure in the repository."""
 
 
 class SyncRedisRepository(SyncAbstractRepository):
     def __init__(self, url: str) -> None:
         try:
-            import redis
+            from redis import asyncio as aioredis
         except ImportError:
             raise ConfigurationError("redis extra dependencies not installed.")
-        self.redis: SyncRedis = redis.from_url(url)  # type: ignore
+        self.redis: SyncRedis = aioredis.from_url(url)  # type: ignore
         self.messages = []
         self.prefix = "cbr::"
 
     def initialize(self) -> None:
         self.redis.initialize()  # type: ignore
 
     def get(self, name: CircuitName) -> Optional[Context]:
```

### Comparing `purgatory-1.0.1/src/purgatory/service/_sync/unit_of_work.py` & `purgatory-1.0.2/src/purgatory/service/_sync/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/src/purgatory/service/typing.py` & `purgatory-1.0.2/src/purgatory/service/typing.py`

 * *Files identical despite different names*

### Comparing `purgatory-1.0.1/PKG-INFO` & `purgatory-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: purgatory
-Version: 1.0.1
+Version: 1.0.2
 Summary: A circuit breaker implementation for asyncio
 Home-page: https://github.com/mardiros/purgatory
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: aioredis
 Provides-Extra: redis
-Requires-Dist: aioredis (>=2.0.1,<3.0.0); extra == "aioredis"
-Requires-Dist: redis (>=4.1.0,<5.0.0); extra == "redis"
+Requires-Dist: redis (>=4.2.0,<5.0.0) ; extra == "aioredis" or extra == "redis"
 Description-Content-Type: text/x-rst
 
 Purgatory
 =========
 
 .. image:: https://readthedocs.org/projects/purgatory/badge/?version=latest
    :target: https://purgatory.readthedocs.io/en/latest/?badge=latest
```

