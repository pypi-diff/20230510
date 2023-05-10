# Comparing `tmp/renderit-0.0.2.tar.gz` & `tmp/renderit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renderit-0.0.2.tar", last modified: Tue May  9 18:42:25 2023, max compression
+gzip compressed data, was "renderit-0.0.4.tar", last modified: Wed May 10 05:24:34 2023, max compression
```

## Comparing `renderit-0.0.2.tar` & `renderit-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:42:25.682861 renderit-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 18:41:32.000000 renderit-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-09 18:42:25.682861 renderit-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 18:41:32.000000 renderit-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-09 18:41:32.000000 renderit-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-09 18:42:25.682861 renderit-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-09 18:41:32.000000 renderit-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:42:25.678861 renderit-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:42:25.682861 renderit-0.0.2/src/renderit/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 18:41:32.000000 renderit-0.0.2/src/renderit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-09 18:41:32.000000 renderit-0.0.2/src/renderit/custom_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-09 18:41:32.000000 renderit-0.0.2/src/renderit/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-09 18:41:32.000000 renderit-0.0.2/src/renderit/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-09 18:41:32.000000 renderit-0.0.2/src/renderit/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:42:25.682861 renderit-0.0.2/src/renderit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-09 18:42:25.000000 renderit-0.0.2/src/renderit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-09 18:42:25.000000 renderit-0.0.2/src/renderit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:42:25.000000 renderit-0.0.2/src/renderit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 18:42:25.000000 renderit-0.0.2/src/renderit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 18:42:25.000000 renderit-0.0.2/src/renderit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:24:34.483631 renderit-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 05:23:45.000000 renderit-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-10 05:24:34.483631 renderit-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 05:23:45.000000 renderit-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-10 05:23:45.000000 renderit-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-10 05:24:34.483631 renderit-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-10 05:23:45.000000 renderit-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:24:34.479630 renderit-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:24:34.483631 renderit-0.0.4/src/renderit/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-10 05:23:45.000000 renderit-0.0.4/src/renderit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-10 05:23:45.000000 renderit-0.0.4/src/renderit/custom_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-10 05:23:45.000000 renderit-0.0.4/src/renderit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-10 05:23:45.000000 renderit-0.0.4/src/renderit/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-10 05:23:45.000000 renderit-0.0.4/src/renderit/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:24:34.483631 renderit-0.0.4/src/renderit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-10 05:24:34.000000 renderit-0.0.4/src/renderit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-10 05:24:34.000000 renderit-0.0.4/src/renderit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:24:34.000000 renderit-0.0.4/src/renderit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-10 05:24:34.000000 renderit-0.0.4/src/renderit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 05:24:34.000000 renderit-0.0.4/src/renderit.egg-info/top_level.txt
```

### Comparing `renderit-0.0.2/LICENSE` & `renderit-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `renderit-0.0.2/PKG-INFO` & `renderit-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renderit
-Version: 0.0.2
+Version: 0.0.4
 Summary: A small python package
 Home-page: https://github.com/Yashwanth1119/renderit
 Author: Yashwanth1119
 Author-email: yashwanthtvv@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Yashwanth1119/renderit/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `renderit-0.0.2/setup.cfg` & `renderit-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `renderit-0.0.2/setup.py` & `renderit-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
-__version__ = "0.0.2"
+__version__ = "0.0.4"
 
 REPO_NAME = "renderit"
 AUTHOR_USER_NAME = "Yashwanth1119"
 SRC_REPO = "renderit"
 AUTHOR_EMAIL = "yashwanthtvv@gmail.com"
 
 setuptools.setup(
```

### Comparing `renderit-0.0.2/src/renderit/site.py` & `renderit-0.0.4/src/renderit/site.py`

 * *Files identical despite different names*

### Comparing `renderit-0.0.2/src/renderit/youtube.py` & `renderit-0.0.4/src/renderit/youtube.py`

 * *Files identical despite different names*

### Comparing `renderit-0.0.2/src/renderit.egg-info/PKG-INFO` & `renderit-0.0.4/src/renderit.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renderit
-Version: 0.0.2
+Version: 0.0.4
 Summary: A small python package
 Home-page: https://github.com/Yashwanth1119/renderit
 Author: Yashwanth1119
 Author-email: yashwanthtvv@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Yashwanth1119/renderit/issues
 Classifier: Programming Language :: Python :: 3.7
```

