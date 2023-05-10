# Comparing `tmp/netunicorn-executor-0.2.4.tar.gz` & `tmp/netunicorn-executor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netunicorn/netunicorn/netunicorn-executor/dist/.tmp-94s4lg_w/netunicorn-executor-0.2.4.tar", last modified: Wed Mar 15 07:15:46 2023, max compression
+gzip compressed data, was "/home/runner/work/netunicorn/netunicorn/netunicorn-executor/dist/.tmp-zldw1r7u/netunicorn-executor-0.3.0.tar", last modified: Wed May 10 07:50:15 2023, max compression
```

## Comparing `netunicorn-executor-0.2.4.tar` & `netunicorn-executor-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-15 07:15:36.000000 netunicorn-executor-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/netunicorn/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-15 07:15:36.000000 netunicorn-executor-0.2.4/src/netunicorn/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-15 07:15:36.000000 netunicorn-executor-0.2.4/src/netunicorn/executor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-03-15 07:15:36.000000 netunicorn-executor-0.2.4/src/netunicorn/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/netunicorn_executor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/netunicorn_executor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/netunicorn_executor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/netunicorn_executor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/netunicorn_executor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-15 07:15:46.000000 netunicorn-executor-0.2.4/src/netunicorn_executor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-10 07:50:00.000000 netunicorn-executor-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 07:50:00.000000 netunicorn-executor-0.3.0/src/netunicorn/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 07:50:00.000000 netunicorn-executor-0.3.0/src/netunicorn/executor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-05-10 07:50:00.000000 netunicorn-executor-0.3.0/src/netunicorn/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 07:50:15.000000 netunicorn-executor-0.3.0/src/netunicorn_executor.egg-info/top_level.txt
```

### Comparing `netunicorn-executor-0.2.4/pyproject.toml` & `netunicorn-executor-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [project]
 name = "netunicorn-executor"
-version = "0.2.4"
+version = "0.3.0"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn executor module"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = ["netunicorn"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "returns",
     "cloudpickle",
     "requests",
-    "netunicorn-base >= 0.2.0",
+    "netunicorn-base >= 0.3.0",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 ignore_missing_imports = true
 explicit_package_bases = true
 strict = true
 exclude = "tests"
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
```

### Comparing `netunicorn-executor-0.2.4/src/netunicorn/executor/executor.py` & `netunicorn-executor-0.3.0/src/netunicorn/executor/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         return logger
 
     def __call__(self) -> None:
         """
         This method is the main loop of the executor.
         :return: None
         """
-        # TODO: add keepalive in the background that will send current state
         while True:
             try:
                 if self.state == PipelineExecutorState.LOOKING_FOR_PIPELINE:
                     self.request_pipeline()
                 elif self.state == PipelineExecutorState.EXECUTING:
                     asyncio.run(self.execute())
                 elif self.state == PipelineExecutorState.REPORTING:
```

