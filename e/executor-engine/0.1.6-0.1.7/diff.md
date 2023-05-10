# Comparing `tmp/executor-engine-0.1.6.tar.gz` & `tmp/executor-engine-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "executor-engine-0.1.6.tar", last modified: Sat Apr  8 09:15:50 2023, max compression
+gzip compressed data, was "executor-engine-0.1.7.tar", last modified: Wed May 10 01:29:56 2023, max compression
```

## Comparing `executor-engine-0.1.6.tar` & `executor-engine-0.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:50.952825 executor-engine-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-08 09:15:40.000000 executor-engine-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-08 09:15:50.952825 executor-engine-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-08 09:15:40.000000 executor-engine-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:50.948825 executor-engine-0.1.6/executor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:50.952825 executor-engine-0.1.6/executor/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:50.952825 executor-engine-0.1.6/executor/engine/job/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:50.952825 executor-engine-0.1.6/executor/engine/job/extend/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/extend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/extend/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/extend/webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:50.952825 executor-engine-0.1.6/executor/engine/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/launcher/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:50.952825 executor-engine-0.1.6/executor/engine/middle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/middle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/middle/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/middle/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-08 09:15:40.000000 executor-engine-0.1.6/executor/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 09:15:50.952825 executor-engine-0.1.6/executor_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-08 09:15:50.000000 executor-engine-0.1.6/executor_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-08 09:15:50.000000 executor-engine-0.1.6/executor_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 09:15:50.000000 executor-engine-0.1.6/executor_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 09:15:50.000000 executor-engine-0.1.6/executor_engine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-08 09:15:50.000000 executor-engine-0.1.6/executor_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 09:15:50.000000 executor-engine-0.1.6/executor_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 09:15:50.952825 executor-engine-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-08 09:15:40.000000 executor-engine-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:56.323624 executor-engine-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 01:29:42.000000 executor-engine-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-10 01:29:56.323624 executor-engine-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-10 01:29:42.000000 executor-engine-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:56.319624 executor-engine-0.1.7/executor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:56.319624 executor-engine-0.1.7/executor/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:56.319624 executor-engine-0.1.7/executor/engine/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:56.319624 executor-engine-0.1.7/executor/engine/job/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/extend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/extend/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/extend/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:56.323624 executor-engine-0.1.7/executor/engine/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/launcher/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:56.323624 executor-engine-0.1.7/executor/engine/middle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/middle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/middle/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/middle/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-10 01:29:42.000000 executor-engine-0.1.7/executor/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:29:56.323624 executor-engine-0.1.7/executor_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-10 01:29:56.000000 executor-engine-0.1.7/executor_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-10 01:29:56.000000 executor-engine-0.1.7/executor_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 01:29:56.000000 executor-engine-0.1.7/executor_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 01:29:56.000000 executor-engine-0.1.7/executor_engine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-10 01:29:56.000000 executor-engine-0.1.7/executor_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 01:29:56.000000 executor-engine-0.1.7/executor_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 01:29:56.323624 executor-engine-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-10 01:29:42.000000 executor-engine-0.1.7/setup.py
```

### Comparing `executor-engine-0.1.6/LICENSE` & `executor-engine-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/PKG-INFO` & `executor-engine-0.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: executor-engine
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package for manage job executions.
 Home-page: https://github.com/Nanguage/executor-engine
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT
 Keywords: Job Management
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `executor-engine-0.1.6/README.md` & `executor-engine-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/core.py` & `executor-engine-0.1.7/executor/engine/core.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/job/base.py` & `executor-engine-0.1.7/executor/engine/job/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import inspect
 import typing as T
 from datetime import datetime
 from pathlib import Path
 from copy import copy
 import itertools
 
 import cloudpickle
@@ -300,26 +301,32 @@
         self.release_resource()
 
     async def on_done(self, res):
         """Callback when the job is done."""
         logger.info(f"Job {self} done.")
         self.future.set_result(res)
         for callback in self.future.done_callbacks:
-            callback(res)
+            if inspect.iscoroutinefunction(callback):
+                await callback(res)
+            else:
+                callback(res)
         self._on_finish("done")
 
     async def on_failed(self, e: Exception):
         """Callback when the job is failed."""
         logger.error(f"Job {self} failed: {repr(e)}")
         assert self.engine is not None
         if self.engine.print_traceback:
             logger.exception(e)
         self.future.set_exception(e)
         for err_callback in self.future.error_callbacks:
-            err_callback(e)
+            if inspect.iscoroutinefunction(err_callback):
+                await err_callback(e)
+            else:
+                err_callback(e)
         if self.retry_remain > 0:
             self._on_finish("pending")
             self.retry_remain -= 1
             await asyncio.sleep(self.retry_time_delta)
             await self.rerun(check_status=False)
         else:
             self._on_finish("failed")
```

### Comparing `executor-engine-0.1.6/executor/engine/job/condition.py` & `executor-engine-0.1.7/executor/engine/job/condition.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/job/dask.py` & `executor-engine-0.1.7/executor/engine/job/dask.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/job/extend/subprocess.py` & `executor-engine-0.1.7/executor/engine/job/extend/subprocess.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/job/extend/webapp.py` & `executor-engine-0.1.7/executor/engine/job/extend/webapp.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/job/process.py` & `executor-engine-0.1.7/executor/engine/job/process.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/job/thread.py` & `executor-engine-0.1.7/executor/engine/job/thread.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/job/utils.py` & `executor-engine-0.1.7/executor/engine/job/utils.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/launcher/core.py` & `executor-engine-0.1.7/executor/engine/launcher/core.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/manager.py` & `executor-engine-0.1.7/executor/engine/manager.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/middle/capture.py` & `executor-engine-0.1.7/executor/engine/middle/capture.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor/engine/utils.py` & `executor-engine-0.1.7/executor/engine/utils.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/executor_engine.egg-info/PKG-INFO` & `executor-engine-0.1.7/executor_engine.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: executor-engine
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package for manage job executions.
 Home-page: https://github.com/Nanguage/executor-engine
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT
 Keywords: Job Management
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `executor-engine-0.1.6/executor_engine.egg-info/SOURCES.txt` & `executor-engine-0.1.7/executor_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `executor-engine-0.1.6/setup.py` & `executor-engine-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     return get_requirements_from_file('requirements.txt')
 
 
 def get_doc_requires():
     return get_requirements_from_file('docs/requirements.txt')
 
 
-requires_test = ['pytest', 'pytest-cov', 'flake8', 'mypy']
+requires_test = ['pytest', 'pytest-cov', 'pytest-asyncio', 'flake8', 'mypy']
 packages_for_dev = ["pip", "setuptools", "wheel", "twine", "ipdb"]
 
 requires_dev = packages_for_dev + requires_test + get_doc_requires()
 
 requires_dask = ['dask', 'distributed', 'nest_asyncio']
```

