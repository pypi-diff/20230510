# Comparing `tmp/robocorp_tasks-0.2.0.tar.gz` & `tmp/robocorp_tasks-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-0.2.0.tar", max compression
+gzip compressed data, was "robocorp_tasks-0.2.1.tar", max compression
```

## Comparing `robocorp_tasks-0.2.0.tar` & `robocorp_tasks-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     4922 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/README.md
--rw-r--r--   0        0        0     1265 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3113 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4495 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1457 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5120 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0     7689 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      182 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     1123 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     1367 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     5267 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0      461 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     3738 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5487 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0      809 2023-05-09 16:38:41.559194 robocorp_tasks-0.2.0/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 robocorp_tasks-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4922 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/README.md
+-rw-r--r--   0        0        0     1134 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1457 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5120 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0     7689 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1123 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     5267 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0      461 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     3738 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5487 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0      870 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:53:59.462590 robocorp_tasks-0.2.1/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 robocorp_tasks-0.2.1/PKG-INFO
```

### Comparing `robocorp_tasks-0.2.0/README.md` & `robocorp_tasks-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/pyproject.toml` & `robocorp_tasks-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "0.2.0"
+version = "0.2.1"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/tasks", from = "src"}]
 classifiers = [
@@ -13,16 +13,18 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "0.1.0"
-# robocorp-log = {path = "../log/", develop = true}
+robocorp-log = "0.1.1"
+
+[tool.poetry.group.dev.dependencies]
+robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.mypy]
 mypy_path = "src:tests"
 
 [[tool.mypy.overrides]]
 module = "setuptools.*"
 ignore_missing_imports = true
@@ -35,19 +37,10 @@
 module = "pytest_timeout.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "module_that_does_not_exist"
 ignore_missing_imports = true
 
-[tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
-ruff = "^0.0.255"
-mypy = "^1.1.1"
-pytest = "^7.2.2"
-pytest-xdist = "^3.2.1"
-pytest-regressions = "1.0.6"
-fire = "^0.5.0"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/__init__.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-"""
-robocorp-tasks: mark entry points with:
+"""Robocorp tasks helps in creating entry points for your automation project.
+
+To use:
+
+Mark entry points with:
 
 ```
+from robocorp.tasks import task
+
 @task
 def my_method():
     ...
 ```
 
-
 Running options:
 
 Runs all the tasks in a .py file:
 
   `python -m robocorp.tasks run <path_to_file>`
 
 Run all the tasks in files named *task*.py:
@@ -28,15 +32,15 @@
 automatically logged is not imported prior the the `cli.main` call.
 """
 from pathlib import Path
 from typing import Optional
 from ._protocols import ITask
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(func):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
 
@@ -65,14 +69,16 @@
     _hooks.on_task_func_found(func)
 
     return func
 
 
 def session_cache(func):
     """
+    Provides decorator which caches return and clears automatically when all tasks have been run.
+
     A decorator which automatically cache the result of the given function and
     will return it on any new invocation until robocorp-tasks finishes running
     all tasks.
 
     The function may be either a generator with a single yield (so, the first
     yielded value will be returned and when the cache is released the generator
     will be resumed) or a function returning some value.
@@ -84,14 +90,16 @@
     from ._lifecycle import _cache
 
     return _cache(after_all_tasks_run, func)
 
 
 def task_cache(func):
     """
+    Provides decorator which caches return and clears it automatically when the current task has been run.
+
     A decorator which automatically cache the result of the given function and
     will return it on any new invocation until robocorp-tasks finishes running
     the current task.
 
     The function may be either a generator with a single yield (so, the first
     yielded value will be returned and when the cache is released the generator
     will be resumed) or a function returning some value.
@@ -103,26 +111,27 @@
     from ._lifecycle import _cache
 
     return _cache(after_task_run, func)
 
 
 def get_output_dir() -> Optional[Path]:
     """
-    Provide the output directory being used for the run or None if there's
-    no output dir configured.
+    Provide the output directory being used for the run or None if there's no output dir configured.
     """
     from ._config import get_config
 
     config = get_config()
     if config is None:
         return None
     return config.output_dir
 
 
 def get_current_task() -> Optional[ITask]:
     """
-    Provides the task which is being currently run or None if not currently
-    running a task.
+    Provides the task which is being currently run or None if not currently running a task.
     """
     from . import _task
 
     return _task.get_current_task()
+
+
+__all__ = ["task", "session_cache", "task_cache", "get_output_dir", "get_current_task"]
```

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_callback.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_commands.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_commands.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_config.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/src/robocorp/tasks/_task.py` & `robocorp_tasks-0.2.1/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.2.0/PKG-INFO` & `robocorp_tasks-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 0.2.0
+Version: 0.2.1
 Summary: The automation framework for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (==0.1.0)
+Requires-Dist: robocorp-log (==0.1.1)
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework designed to simplify the development 
 of Python automations.
```

