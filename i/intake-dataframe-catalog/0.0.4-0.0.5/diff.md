# Comparing `tmp/intake_dataframe_catalog-0.0.4.tar.gz` & `tmp/intake_dataframe_catalog-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_dataframe_catalog-0.0.4.tar", last modified: Tue May  9 06:34:54 2023, max compression
+gzip compressed data, was "intake_dataframe_catalog-0.0.5.tar", last modified: Tue May  9 07:01:01 2023, max compression
```

## Comparing `intake_dataframe_catalog-0.0.4.tar` & `intake_dataframe_catalog-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.625875 intake_dataframe_catalog-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 06:34:54.000000 intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:34:54.629875 intake_dataframe_catalog-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-09 06:34:39.000000 intake_dataframe_catalog-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:01:01.045306 intake_dataframe_catalog-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 07:01:01.045306 intake_dataframe_catalog-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 07:01:01.045306 intake_dataframe_catalog-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:01:01.045306 intake_dataframe_catalog-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:01:01.045306 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 07:01:01.045306 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:01:01.045306 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-09 07:01:01.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 07:01:01.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:01:01.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 07:01:01.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 07:01:01.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 07:01:01.000000 intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:01:01.045306 intake_dataframe_catalog-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-09 07:00:46.000000 intake_dataframe_catalog-0.0.5/versioneer.py
```

### Comparing `intake_dataframe_catalog-0.0.4/LICENSE` & `intake_dataframe_catalog-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.4/README.rst` & `intake_dataframe_catalog-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.4/pyproject.toml` & `intake_dataframe_catalog-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/_search.py` & `intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog/_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog/core.py` & `intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog/core.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.4/src/intake_dataframe_catalog.egg-info/SOURCES.txt` & `intake_dataframe_catalog-0.0.5/src/intake_dataframe_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.4/tests/test_core.py` & `intake_dataframe_catalog-0.0.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.4/tests/test_search.py` & `intake_dataframe_catalog-0.0.5/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.4/versioneer.py` & `intake_dataframe_catalog-0.0.5/versioneer.py`

 * *Files identical despite different names*

