# Comparing `tmp/intake_dataframe_catalog-0.0.6.tar.gz` & `tmp/intake_dataframe_catalog-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_dataframe_catalog-0.0.6.tar", last modified: Tue May  9 21:59:08 2023, max compression
+gzip compressed data, was "intake_dataframe_catalog-0.0.7.tar", last modified: Tue May  9 22:44:01 2023, max compression
```

## Comparing `intake_dataframe_catalog-0.0.6.tar` & `intake_dataframe_catalog-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:59:08.886654 intake_dataframe_catalog-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 21:59:08.886654 intake_dataframe_catalog-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 21:59:08.886654 intake_dataframe_catalog-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:59:08.882654 intake_dataframe_catalog-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:59:08.886654 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 21:59:08.886654 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:59:08.882654 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 21:59:08.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 21:59:08.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:59:08.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 21:59:08.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 21:59:08.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 21:59:08.000000 intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:59:08.886654 intake_dataframe_catalog-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-09 21:58:55.000000 intake_dataframe_catalog-0.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:01.246138 intake_dataframe_catalog-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-09 22:44:01.246138 intake_dataframe_catalog-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 22:44:01.246138 intake_dataframe_catalog-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:01.242138 intake_dataframe_catalog-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:01.246138 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 22:44:01.246138 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:01.246138 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-09 22:44:01.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 22:44:01.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:44:01.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 22:44:01.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 22:44:01.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 22:44:01.000000 intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:01.246138 intake_dataframe_catalog-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-09 22:43:40.000000 intake_dataframe_catalog-0.0.7/versioneer.py
```

### Comparing `intake_dataframe_catalog-0.0.6/LICENSE` & `intake_dataframe_catalog-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.6/README.rst` & `intake_dataframe_catalog-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.6/pyproject.toml` & `intake_dataframe_catalog-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "intake_dataframe_catalog"
 authors = [
     { name = "ACCESS-NRI" },
 ]
 description = "An intake driver for a searchable table of intake catalogs and associated metadata"
-readme = "README.md"
+readme = "README.rst"
 requires-python = ">=3.9"
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

### Comparing `intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog/_search.py` & `intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog/_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog/core.py` & `intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog/core.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.6/src/intake_dataframe_catalog.egg-info/SOURCES.txt` & `intake_dataframe_catalog-0.0.7/src/intake_dataframe_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.6/tests/test_core.py` & `intake_dataframe_catalog-0.0.7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.6/tests/test_search.py` & `intake_dataframe_catalog-0.0.7/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.6/versioneer.py` & `intake_dataframe_catalog-0.0.7/versioneer.py`

 * *Files identical despite different names*

