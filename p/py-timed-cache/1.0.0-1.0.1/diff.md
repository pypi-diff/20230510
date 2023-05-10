# Comparing `tmp/py-timed-cache-1.0.0.tar.gz` & `tmp/py-timed-cache-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-timed-cache-1.0.0.tar", last modified: Wed May 10 14:42:59 2023, max compression
+gzip compressed data, was "py-timed-cache-1.0.1.tar", last modified: Wed May 10 14:44:19 2023, max compression
```

## Comparing `py-timed-cache-1.0.0.tar` & `py-timed-cache-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:42:59.136810 py-timed-cache-1.0.0/
--rw-r--r--   0 nadrian  (546264773) staff       (20)     1067 2023-05-10 13:54:04.000000 py-timed-cache-1.0.0/LICENSE
--rw-r--r--   0 nadrian  (546264773) staff       (20)     1279 2023-05-10 14:42:59.136665 py-timed-cache-1.0.0/PKG-INFO
--rw-r--r--   0 nadrian  (546264773) staff       (20)      958 2023-05-10 14:16:51.000000 py-timed-cache-1.0.0/README.md
-drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:42:59.135502 py-timed-cache-1.0.0/py_timed_cache.egg-info/
--rw-r--r--   0 nadrian  (546264773) staff       (20)     1279 2023-05-10 14:42:59.000000 py-timed-cache-1.0.0/py_timed_cache.egg-info/PKG-INFO
--rw-r--r--   0 nadrian  (546264773) staff       (20)      286 2023-05-10 14:42:59.000000 py-timed-cache-1.0.0/py_timed_cache.egg-info/SOURCES.txt
--rw-r--r--   0 nadrian  (546264773) staff       (20)        1 2023-05-10 14:42:59.000000 py-timed-cache-1.0.0/py_timed_cache.egg-info/dependency_links.txt
--rw-r--r--   0 nadrian  (546264773) staff       (20)       17 2023-05-10 14:42:59.000000 py-timed-cache-1.0.0/py_timed_cache.egg-info/top_level.txt
--rw-r--r--   0 nadrian  (546264773) staff       (20)       38 2023-05-10 14:42:59.136859 py-timed-cache-1.0.0/setup.cfg
--rw-r--r--   0 nadrian  (546264773) staff       (20)      532 2023-05-10 14:42:52.000000 py-timed-cache-1.0.0/setup.py
-drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:42:59.136109 py-timed-cache-1.0.0/tests/
--rw-r--r--   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:00:38.000000 py-timed-cache-1.0.0/tests/__init__.py
--rw-r--r--   0 nadrian  (546264773) staff       (20)      148 2023-05-10 14:19:10.000000 py-timed-cache-1.0.0/tests/context.py
--rw-r--r--   0 nadrian  (546264773) staff       (20)     1091 2023-05-10 14:35:21.000000 py-timed-cache-1.0.0/tests/test.timedcache.py
-drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:42:59.136467 py-timed-cache-1.0.0/timedcache/
--rw-r--r--   0 nadrian  (546264773) staff       (20)       59 2023-05-10 14:17:28.000000 py-timed-cache-1.0.0/timedcache/__init__.py
--rw-r--r--   0 nadrian  (546264773) staff       (20)     2230 2023-05-10 14:18:36.000000 py-timed-cache-1.0.0/timedcache/timedcache.py
+drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:44:19.453976 py-timed-cache-1.0.1/
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     1067 2023-05-10 13:54:04.000000 py-timed-cache-1.0.1/LICENSE
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     1283 2023-05-10 14:44:19.453818 py-timed-cache-1.0.1/PKG-INFO
+-rw-r--r--   0 nadrian  (546264773) staff       (20)      962 2023-05-10 14:43:21.000000 py-timed-cache-1.0.1/README.md
+drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:44:19.452480 py-timed-cache-1.0.1/py_timed_cache.egg-info/
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     1283 2023-05-10 14:44:19.000000 py-timed-cache-1.0.1/py_timed_cache.egg-info/PKG-INFO
+-rw-r--r--   0 nadrian  (546264773) staff       (20)      286 2023-05-10 14:44:19.000000 py-timed-cache-1.0.1/py_timed_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 nadrian  (546264773) staff       (20)        1 2023-05-10 14:44:19.000000 py-timed-cache-1.0.1/py_timed_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 nadrian  (546264773) staff       (20)       17 2023-05-10 14:44:19.000000 py-timed-cache-1.0.1/py_timed_cache.egg-info/top_level.txt
+-rw-r--r--   0 nadrian  (546264773) staff       (20)       38 2023-05-10 14:44:19.454024 py-timed-cache-1.0.1/setup.cfg
+-rw-r--r--   0 nadrian  (546264773) staff       (20)      532 2023-05-10 14:44:15.000000 py-timed-cache-1.0.1/setup.py
+drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:44:19.453082 py-timed-cache-1.0.1/tests/
+-rw-r--r--   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:00:38.000000 py-timed-cache-1.0.1/tests/__init__.py
+-rw-r--r--   0 nadrian  (546264773) staff       (20)      148 2023-05-10 14:19:10.000000 py-timed-cache-1.0.1/tests/context.py
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     1091 2023-05-10 14:35:21.000000 py-timed-cache-1.0.1/tests/test.timedcache.py
+drwxr-xr-x   0 nadrian  (546264773) staff       (20)        0 2023-05-10 14:44:19.453564 py-timed-cache-1.0.1/timedcache/
+-rw-r--r--   0 nadrian  (546264773) staff       (20)       59 2023-05-10 14:17:28.000000 py-timed-cache-1.0.1/timedcache/__init__.py
+-rw-r--r--   0 nadrian  (546264773) staff       (20)     2230 2023-05-10 14:18:36.000000 py-timed-cache-1.0.1/timedcache/timedcache.py
```

### Comparing `py-timed-cache-1.0.0/LICENSE` & `py-timed-cache-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-timed-cache-1.0.0/PKG-INFO` & `py-timed-cache-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-timed-cache
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pure Python timed-cache
 Home-page: https://github.com/NicoAdrian/timed-cache
 Author: Nicolas Adrian
 Author-email: nicolasadrian3@gmail.com
 License: MIT
 Keywords: cache,timed-cache,timedcache
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # timed-cache
 
 Pure Python timed-cache that behaves like a regular `dict`.
 Can also be used as a decorator to cache function calls (works for async functions as well).
 
 ## Installation
 
-`pip install timedcache`
+`pip install py-timed-cache`
 
 ## Example
 
 ```python
 from timedcache import TimedCache
 
 my_cache = TimedCache(1) # 1 second cache
```

### Comparing `py-timed-cache-1.0.0/README.md` & `py-timed-cache-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # timed-cache
 
 Pure Python timed-cache that behaves like a regular `dict`.
 Can also be used as a decorator to cache function calls (works for async functions as well).
 
 ## Installation
 
-`pip install timedcache`
+`pip install py-timed-cache`
 
 ## Example
 
 ```python
 from timedcache import TimedCache
 
 my_cache = TimedCache(1) # 1 second cache
```

### Comparing `py-timed-cache-1.0.0/py_timed_cache.egg-info/PKG-INFO` & `py-timed-cache-1.0.1/py_timed_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-timed-cache
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pure Python timed-cache
 Home-page: https://github.com/NicoAdrian/timed-cache
 Author: Nicolas Adrian
 Author-email: nicolasadrian3@gmail.com
 License: MIT
 Keywords: cache,timed-cache,timedcache
 Description-Content-Type: text/markdown
@@ -13,15 +13,15 @@
 # timed-cache
 
 Pure Python timed-cache that behaves like a regular `dict`.
 Can also be used as a decorator to cache function calls (works for async functions as well).
 
 ## Installation
 
-`pip install timedcache`
+`pip install py-timed-cache`
 
 ## Example
 
 ```python
 from timedcache import TimedCache
 
 my_cache = TimedCache(1) # 1 second cache
```

### Comparing `py-timed-cache-1.0.0/setup.py` & `py-timed-cache-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as fd:
     readme = fd.read()
 
 setup(
     name="py-timed-cache",
-    version="1.0.0",
+    version="1.0.1",
     description="Pure Python timed-cache",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Nicolas Adrian",
     author_email="nicolasadrian3@gmail.com",
     url="https://github.com/NicoAdrian/timed-cache",
     license="MIT",
```

### Comparing `py-timed-cache-1.0.0/tests/test.timedcache.py` & `py-timed-cache-1.0.1/tests/test.timedcache.py`

 * *Files identical despite different names*

### Comparing `py-timed-cache-1.0.0/timedcache/timedcache.py` & `py-timed-cache-1.0.1/timedcache/timedcache.py`

 * *Files identical despite different names*

