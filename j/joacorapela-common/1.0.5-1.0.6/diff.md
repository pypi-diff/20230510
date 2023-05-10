# Comparing `tmp/joacorapela_common-1.0.5.tar.gz` & `tmp/joacorapela_common-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joacorapela_common-1.0.5.tar", last modified: Wed May 10 13:54:57 2023, max compression
+gzip compressed data, was "joacorapela_common-1.0.6.tar", last modified: Wed May 10 14:05:47 2023, max compression
```

## Comparing `joacorapela_common-1.0.5.tar` & `joacorapela_common-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 13:54:57.943011 joacorapela_common-1.0.5/
--rw-rw-r--   0 rapela    (5397) rapela    (5397)      524 2023-05-10 13:54:57.944011 joacorapela_common-1.0.5/PKG-INFO
--rw-rw-r--   0 rapela    (5397) rapela    (5397)      116 2022-12-21 15:51:07.000000 joacorapela_common-1.0.5/README.md
--rw-rw-r--   0 rapela    (5397) rapela    (5397)       81 2023-05-10 08:19:50.000000 joacorapela_common-1.0.5/pyproject.toml
--rw-rw-r--   0 rapela    (5397) rapela    (5397)      595 2023-05-10 13:54:57.947018 joacorapela_common-1.0.5/setup.cfg
--rw-rw-r--   0 rapela    (5397) rapela    (5397)       37 2023-05-05 16:48:18.000000 joacorapela_common-1.0.5/setup.py
-drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 13:54:57.870014 joacorapela_common-1.0.5/src/
-drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 13:54:57.884010 joacorapela_common-1.0.5/src/joacorapela_common/
--rw-rw-r--   0 rapela    (5397) rapela    (5397)        2 2023-05-10 08:19:50.000000 joacorapela_common-1.0.5/src/joacorapela_common/__init__.py
-drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 13:54:57.940012 joacorapela_common-1.0.5/src/joacorapela_common/utils/
--rw-rw-r--   0 rapela    (5397) rapela    (5397)        2 2023-05-10 08:19:50.000000 joacorapela_common-1.0.5/src/joacorapela_common/utils/__init__.py
--rw-rw-r--   0 rapela    (5397) rapela    (5397)     1755 2022-12-21 15:51:07.000000 joacorapela_common-1.0.5/src/joacorapela_common/utils/geometry.py
--rw-rw-r--   0 rapela    (5397) rapela    (5397)      104 2023-05-10 08:19:50.000000 joacorapela_common-1.0.5/src/joacorapela_common/utils/numerical_methods.py
--rw-rw-r--   0 rapela    (5397) rapela    (5397)     1430 2022-12-21 15:51:07.000000 joacorapela_common-1.0.5/src/joacorapela_common/utils/probability.py
-drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 13:54:57.917011 joacorapela_common-1.0.5/src/joacorapela_common.egg-info/
--rw-rw-r--   0 rapela    (5397) rapela    (5397)      524 2023-05-10 13:54:57.000000 joacorapela_common-1.0.5/src/joacorapela_common.egg-info/PKG-INFO
--rw-rw-r--   0 rapela    (5397) rapela    (5397)      483 2023-05-10 13:54:57.000000 joacorapela_common-1.0.5/src/joacorapela_common.egg-info/SOURCES.txt
--rw-rw-r--   0 rapela    (5397) rapela    (5397)        1 2023-05-10 13:54:57.000000 joacorapela_common-1.0.5/src/joacorapela_common.egg-info/dependency_links.txt
--rw-rw-r--   0 rapela    (5397) rapela    (5397)       12 2023-05-10 13:54:57.000000 joacorapela_common-1.0.5/src/joacorapela_common.egg-info/requires.txt
--rw-rw-r--   0 rapela    (5397) rapela    (5397)       19 2023-05-10 13:54:57.000000 joacorapela_common-1.0.5/src/joacorapela_common.egg-info/top_level.txt
+drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 14:05:47.235761 joacorapela_common-1.0.6/
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)      524 2023-05-10 14:05:47.236763 joacorapela_common-1.0.6/PKG-INFO
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)      116 2022-12-21 15:51:07.000000 joacorapela_common-1.0.6/README.md
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)       81 2023-05-10 08:19:50.000000 joacorapela_common-1.0.6/pyproject.toml
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)      595 2023-05-10 14:05:47.240760 joacorapela_common-1.0.6/setup.cfg
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)       37 2023-05-05 16:48:18.000000 joacorapela_common-1.0.6/setup.py
+drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 14:05:46.800760 joacorapela_common-1.0.6/src/
+drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 14:05:46.836760 joacorapela_common-1.0.6/src/joacorapela_common/
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)        2 2023-05-10 08:19:50.000000 joacorapela_common-1.0.6/src/joacorapela_common/__init__.py
+drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 14:05:46.859761 joacorapela_common-1.0.6/src/joacorapela_common/stats/
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)        2 2023-05-10 14:02:59.000000 joacorapela_common-1.0.6/src/joacorapela_common/stats/__init__.py
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)     1069 2023-05-10 08:19:50.000000 joacorapela_common-1.0.6/src/joacorapela_common/stats/bayesianLinearRegression.py
+drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 14:05:47.231761 joacorapela_common-1.0.6/src/joacorapela_common/utils/
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)        2 2023-05-10 08:19:50.000000 joacorapela_common-1.0.6/src/joacorapela_common/utils/__init__.py
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)     1755 2022-12-21 15:51:07.000000 joacorapela_common-1.0.6/src/joacorapela_common/utils/geometry.py
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)      104 2023-05-10 08:19:50.000000 joacorapela_common-1.0.6/src/joacorapela_common/utils/numerical_methods.py
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)     1430 2022-12-21 15:51:07.000000 joacorapela_common-1.0.6/src/joacorapela_common/utils/probability.py
+drwxrwxr-x   0 rapela    (5397) rapela    (5397)        0 2023-05-10 14:05:46.852765 joacorapela_common-1.0.6/src/joacorapela_common.egg-info/
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)      524 2023-05-10 14:05:46.000000 joacorapela_common-1.0.6/src/joacorapela_common.egg-info/PKG-INFO
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)      581 2023-05-10 14:05:46.000000 joacorapela_common-1.0.6/src/joacorapela_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)        1 2023-05-10 14:05:46.000000 joacorapela_common-1.0.6/src/joacorapela_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)       12 2023-05-10 14:05:46.000000 joacorapela_common-1.0.6/src/joacorapela_common.egg-info/requires.txt
+-rw-rw-r--   0 rapela    (5397) rapela    (5397)       19 2023-05-10 14:05:46.000000 joacorapela_common-1.0.6/src/joacorapela_common.egg-info/top_level.txt
```

### Comparing `joacorapela_common-1.0.5/PKG-INFO` & `joacorapela_common-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joacorapela_common
-Version: 1.0.5
+Version: 1.0.6
 Summary: Repository of common functionality for joacorapela's codebase
 Home-page: https://github.com/joacorapela/joacorapela_common
 Author: Joaquin Rapela
 Author-email: joacorapela@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `joacorapela_common-1.0.5/setup.cfg` & `joacorapela_common-1.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = joacorapela_common
-version = 1.0.5
+version = 1.0.6
 description = Repository of common functionality for joacorapela's codebase
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/joacorapela/joacorapela_common
 author = Joaquin Rapela
 author_email = joacorapela@gmail.com
 license = MIT
```

### Comparing `joacorapela_common-1.0.5/src/joacorapela_common/utils/geometry.py` & `joacorapela_common-1.0.6/src/joacorapela_common/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `joacorapela_common-1.0.5/src/joacorapela_common/utils/probability.py` & `joacorapela_common-1.0.6/src/joacorapela_common/utils/probability.py`

 * *Files identical despite different names*

### Comparing `joacorapela_common-1.0.5/src/joacorapela_common.egg-info/PKG-INFO` & `joacorapela_common-1.0.6/src/joacorapela_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joacorapela-common
-Version: 1.0.5
+Version: 1.0.6
 Summary: Repository of common functionality for joacorapela's codebase
 Home-page: https://github.com/joacorapela/joacorapela_common
 Author: Joaquin Rapela
 Author-email: joacorapela@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

