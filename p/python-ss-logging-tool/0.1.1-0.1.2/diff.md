# Comparing `tmp/python-ss-logging-tool-0.1.1.tar.gz` & `tmp/python-ss-logging-tool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ss-logging-tool-0.1.1.tar", last modified: Tue May  9 06:10:31 2023, max compression
+gzip compressed data, was "python-ss-logging-tool-0.1.2.tar", last modified: Wed May 10 08:14:24 2023, max compression
```

## Comparing `python-ss-logging-tool-0.1.1.tar` & `python-ss-logging-tool-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-09 06:10:31.759573 python-ss-logging-tool-0.1.1/
--rw-r--r--   0 jimmychui   (501) staff       (20)      714 2023-05-09 06:10:31.759161 python-ss-logging-tool-0.1.1/PKG-INFO
--rw-r--r--   0 jimmychui   (501) staff       (20)      187 2023-03-17 04:10:00.000000 python-ss-logging-tool-0.1.1/README.md
-drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-09 06:10:31.756984 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/
--rw-r--r--   0 jimmychui   (501) staff       (20)      714 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/PKG-INFO
--rw-r--r--   0 jimmychui   (501) staff       (20)      301 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/SOURCES.txt
--rw-r--r--   0 jimmychui   (501) staff       (20)        1 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/dependency_links.txt
--rw-r--r--   0 jimmychui   (501) staff       (20)       12 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/requires.txt
--rw-r--r--   0 jimmychui   (501) staff       (20)       16 2023-05-09 06:10:31.000000 python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/top_level.txt
--rw-r--r--   0 jimmychui   (501) staff       (20)       38 2023-05-09 06:10:31.759698 python-ss-logging-tool-0.1.1/setup.cfg
--rw-r--r--   0 jimmychui   (501) staff       (20)      817 2023-05-09 06:10:22.000000 python-ss-logging-tool-0.1.1/setup.py
-drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-09 06:10:31.758327 python-ss-logging-tool-0.1.1/ss_logging_tool/
--rw-r--r--   0 jimmychui   (501) staff       (20)       26 2023-03-17 04:04:53.000000 python-ss-logging-tool-0.1.1/ss_logging_tool/__init__.py
--rw-r--r--   0 jimmychui   (501) staff       (20)     1795 2023-05-09 06:09:25.000000 python-ss-logging-tool-0.1.1/ss_logging_tool/logger.py
+drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-10 08:14:24.368407 python-ss-logging-tool-0.1.2/
+-rw-r--r--   0 jimmychui   (501) staff       (20)      714 2023-05-10 08:14:24.367693 python-ss-logging-tool-0.1.2/PKG-INFO
+-rw-r--r--   0 jimmychui   (501) staff       (20)      187 2023-03-17 04:10:00.000000 python-ss-logging-tool-0.1.2/README.md
+drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-10 08:14:24.365281 python-ss-logging-tool-0.1.2/python_ss_logging_tool.egg-info/
+-rw-r--r--   0 jimmychui   (501) staff       (20)      714 2023-05-10 08:14:24.000000 python-ss-logging-tool-0.1.2/python_ss_logging_tool.egg-info/PKG-INFO
+-rw-r--r--   0 jimmychui   (501) staff       (20)      301 2023-05-10 08:14:24.000000 python-ss-logging-tool-0.1.2/python_ss_logging_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 jimmychui   (501) staff       (20)        1 2023-05-10 08:14:24.000000 python-ss-logging-tool-0.1.2/python_ss_logging_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 jimmychui   (501) staff       (20)       12 2023-05-10 08:14:24.000000 python-ss-logging-tool-0.1.2/python_ss_logging_tool.egg-info/requires.txt
+-rw-r--r--   0 jimmychui   (501) staff       (20)       16 2023-05-10 08:14:24.000000 python-ss-logging-tool-0.1.2/python_ss_logging_tool.egg-info/top_level.txt
+-rw-r--r--   0 jimmychui   (501) staff       (20)       38 2023-05-10 08:14:24.368583 python-ss-logging-tool-0.1.2/setup.cfg
+-rw-r--r--   0 jimmychui   (501) staff       (20)      817 2023-05-10 08:14:22.000000 python-ss-logging-tool-0.1.2/setup.py
+drwxr-xr-x   0 jimmychui   (501) staff       (20)        0 2023-05-10 08:14:24.366657 python-ss-logging-tool-0.1.2/ss_logging_tool/
+-rw-r--r--   0 jimmychui   (501) staff       (20)       26 2023-03-17 04:04:53.000000 python-ss-logging-tool-0.1.2/ss_logging_tool/__init__.py
+-rw-r--r--   0 jimmychui   (501) staff       (20)     1634 2023-05-10 08:13:50.000000 python-ss-logging-tool-0.1.2/ss_logging_tool/logger.py
```

### Comparing `python-ss-logging-tool-0.1.1/PKG-INFO` & `python-ss-logging-tool-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ss-logging-tool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple logger package
 Home-page: https://github.com/yourusername/mypackage
 Author: Jimmy
 Author-email: jimm@xxx.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-ss-logging-tool-0.1.1/python_ss_logging_tool.egg-info/PKG-INFO` & `python-ss-logging-tool-0.1.2/python_ss_logging_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ss-logging-tool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple logger package
 Home-page: https://github.com/yourusername/mypackage
 Author: Jimmy
 Author-email: jimm@xxx.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-ss-logging-tool-0.1.1/setup.py` & `python-ss-logging-tool-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name="python-ss-logging-tool",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
         "pino",
         "nanoid",
         # Add other dependencies if needed
     ],
     author="Jimmy",
```

### Comparing `python-ss-logging-tool-0.1.1/ss_logging_tool/logger.py` & `python-ss-logging-tool-0.1.2/ss_logging_tool/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,13 +47,7 @@
 
     def debug(self, *args, **kwargs):
         self._call(self.logger.debug, *args, **kwargs)
 
     def warn(self, *args, **kwargs):
         self._call(self.logger.warn, *args, **kwargs)
 
-
-logger = Logger.create("testing")
-# logger = pino(
-#     bindings={"apptype": 'testing', "metas": "main"},
-# )
-logger.info("莎士比亞是哪一年出生的")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

