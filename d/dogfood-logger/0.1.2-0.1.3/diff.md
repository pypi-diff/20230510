# Comparing `tmp/dogfood-logger-0.1.2.tar.gz` & `tmp/dogfood-logger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogfood-logger-0.1.2.tar", last modified: Wed May 10 03:37:23 2023, max compression
+gzip compressed data, was "dogfood-logger-0.1.3.tar", last modified: Wed May 10 03:44:24 2023, max compression
```

## Comparing `dogfood-logger-0.1.2.tar` & `dogfood-logger-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:37:23.047994 dogfood-logger-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1087 2023-05-10 02:17:04.000000 dogfood-logger-0.1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 02:17:04.000000 dogfood-logger-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-10 03:37:23.047994 dogfood-logger-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-10 02:17:04.000000 dogfood-logger-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:37:23.047994 dogfood-logger-0.1.2/dogfood-logger/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 03:18:57.000000 dogfood-logger-0.1.2/dogfood-logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-05-10 03:18:57.000000 dogfood-logger-0.1.2/dogfood-logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:37:23.047994 dogfood-logger-0.1.2/dogfood_logger.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-10 03:37:23.000000 dogfood-logger-0.1.2/dogfood_logger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-10 03:37:23.000000 dogfood-logger-0.1.2/dogfood_logger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 03:37:23.000000 dogfood-logger-0.1.2/dogfood_logger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-10 03:37:23.000000 dogfood-logger-0.1.2/dogfood_logger.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 03:37:23.000000 dogfood-logger-0.1.2/dogfood_logger.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      339 2023-05-10 03:26:09.000000 dogfood-logger-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 03:37:23.047994 dogfood-logger-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-10 03:37:21.000000 dogfood-logger-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:37:23.047994 dogfood-logger-0.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)      143 2023-05-10 02:20:45.000000 dogfood-logger-0.1.2/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-05-10 02:17:04.000000 dogfood-logger-0.1.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 02:17:04.000000 dogfood-logger-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-10 02:17:04.000000 dogfood-logger-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/dogfood_logger/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 03:18:57.000000 dogfood-logger-0.1.3/dogfood_logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-05-10 03:18:57.000000 dogfood-logger-0.1.3/dogfood_logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/dogfood_logger.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      339 2023-05-10 03:43:18.000000 dogfood-logger-0.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      404 2023-05-10 03:43:18.000000 dogfood-logger-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/tests/
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-10 02:20:45.000000 dogfood-logger-0.1.3/tests/test.py
```

### Comparing `dogfood-logger-0.1.2/LICENSE.txt` & `dogfood-logger-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dogfood-logger-0.1.2/PKG-INFO` & `dogfood-logger-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogfood-logger
-Version: 0.1.2
+Version: 0.1.3
 Summary: Logger for Grafana
 Home-page: https://github.com/dogfoodhq/dogfood-logger
 Author: Matt Wong
 Author-email: nycmattw@gmail.com
 License: MIT
 License-File: LICENSE.txt
```

### Comparing `dogfood-logger-0.1.2/dogfood-logger/logger.py` & `dogfood-logger-0.1.3/dogfood_logger/logger.py`

 * *Files identical despite different names*

### Comparing `dogfood-logger-0.1.2/dogfood_logger.egg-info/PKG-INFO` & `dogfood-logger-0.1.3/dogfood_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogfood-logger
-Version: 0.1.2
+Version: 0.1.3
 Summary: Logger for Grafana
 Home-page: https://github.com/dogfoodhq/dogfood-logger
 Author: Matt Wong
 Author-email: nycmattw@gmail.com
 License: MIT
 License-File: LICENSE.txt
```

