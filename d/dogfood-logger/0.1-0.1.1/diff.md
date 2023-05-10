# Comparing `tmp/dogfood-logger-0.1.tar.gz` & `tmp/dogfood-logger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogfood-logger-0.1.tar", last modified: Wed May 10 03:09:48 2023, max compression
+gzip compressed data, was "dogfood-logger-0.1.1.tar", last modified: Wed May 10 03:29:01 2023, max compression
```

## Comparing `dogfood-logger-0.1.tar` & `dogfood-logger-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:09:48.529045 dogfood-logger-0.1/
--rw-r--r--   0 root         (0) root         (0)     1087 2023-05-10 02:17:04.000000 dogfood-logger-0.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 02:17:04.000000 dogfood-logger-0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      683 2023-05-10 03:09:48.529045 dogfood-logger-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-10 02:17:04.000000 dogfood-logger-0.1/README.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:09:48.529045 dogfood-logger-0.1/dogfood-logger/
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-10 02:17:04.000000 dogfood-logger-0.1/dogfood-logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-10 02:17:04.000000 dogfood-logger-0.1/dogfood-logger/somePython.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:09:48.529045 dogfood-logger-0.1/dogfood_logger.egg-info/
--rw-r--r--   0 root         (0) root         (0)      683 2023-05-10 03:09:48.000000 dogfood-logger-0.1/dogfood_logger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      317 2023-05-10 03:09:48.000000 dogfood-logger-0.1/dogfood_logger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 03:09:48.000000 dogfood-logger-0.1/dogfood_logger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-10 03:09:48.000000 dogfood-logger-0.1/dogfood_logger.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 03:09:48.000000 dogfood-logger-0.1/dogfood_logger.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-10 03:07:59.000000 dogfood-logger-0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 03:09:48.529045 dogfood-logger-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-10 02:18:46.000000 dogfood-logger-0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:09:48.529045 dogfood-logger-0.1/tests/
--rw-r--r--   0 root         (0) root         (0)      143 2023-05-10 02:20:45.000000 dogfood-logger-0.1/tests/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:29:01.767470 dogfood-logger-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-05-10 02:17:04.000000 dogfood-logger-0.1.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 02:17:04.000000 dogfood-logger-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-10 03:29:01.767470 dogfood-logger-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-10 02:17:04.000000 dogfood-logger-0.1.1/README.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:29:01.767470 dogfood-logger-0.1.1/dogfood-logger/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 03:18:57.000000 dogfood-logger-0.1.1/dogfood-logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-05-10 03:18:57.000000 dogfood-logger-0.1.1/dogfood-logger/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:29:01.767470 dogfood-logger-0.1.1/dogfood_logger.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-05-10 03:29:01.000000 dogfood-logger-0.1.1/dogfood_logger.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2023-05-10 03:29:01.000000 dogfood-logger-0.1.1/dogfood_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 03:29:01.000000 dogfood-logger-0.1.1/dogfood_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-10 03:29:01.000000 dogfood-logger-0.1.1/dogfood_logger.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 03:29:01.000000 dogfood-logger-0.1.1/dogfood_logger.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      339 2023-05-10 03:26:09.000000 dogfood-logger-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 03:29:01.767470 dogfood-logger-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      405 2023-05-10 03:28:52.000000 dogfood-logger-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:29:01.767470 dogfood-logger-0.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      143 2023-05-10 02:20:45.000000 dogfood-logger-0.1.1/tests/test.py
```

### Comparing `dogfood-logger-0.1/LICENSE.txt` & `dogfood-logger-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dogfood-logger-0.1/PKG-INFO` & `dogfood-logger-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogfood-logger
-Version: 0.1
+Version: 0.1.1
 Summary: Logger for Grafana
 Home-page: https://github.com/dogfoodhq/dogfood-logger
 Author: Matt Wong
 Author-email: nycmattw@gmail.com
 License: MIT
 License-File: LICENSE.txt
```

### Comparing `dogfood-logger-0.1/dogfood_logger.egg-info/PKG-INFO` & `dogfood-logger-0.1.1/dogfood_logger.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogfood-logger
-Version: 0.1
+Version: 0.1.1
 Summary: Logger for Grafana
 Home-page: https://github.com/dogfoodhq/dogfood-logger
 Author: Matt Wong
 Author-email: nycmattw@gmail.com
 License: MIT
 License-File: LICENSE.txt
```

