# Comparing `tmp/dogfood_logger-0.1.4.tar.gz` & `tmp/dogfood_logger-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogfood_logger-0.1.4.tar", max compression
+gzip compressed data, was "dogfood_logger-0.1.5.tar", max compression
```

## Comparing `dogfood_logger-0.1.4.tar` & `dogfood_logger-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1087 2023-05-10 02:17:04.332370 dogfood_logger-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0      464 2023-05-10 02:17:04.332370 dogfood_logger-0.1.4/README.md
--rw-r--r--   0        0        0       21 2023-05-10 03:18:57.202008 dogfood_logger-0.1.4/dogfood_logger/__init__.py
--rw-r--r--   0        0        0     3074 2023-05-10 03:18:57.202008 dogfood_logger-0.1.4/dogfood_logger/logger.py
--rw-r--r--   0        0        0       42 2023-05-10 02:17:04.332370 dogfood_logger-0.1.4/dogfood_logger/packageData/sampleData.dat
--rw-r--r--   0        0        0      370 2023-05-10 03:55:15.557701 dogfood_logger-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 dogfood_logger-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-10 02:17:04.332370 dogfood_logger-0.1.5/LICENSE.txt
+-rw-r--r--   0        0        0      464 2023-05-10 02:17:04.332370 dogfood_logger-0.1.5/README.md
+-rw-r--r--   0        0        0       21 2023-05-10 03:18:57.202008 dogfood_logger-0.1.5/dogfood_logger/__init__.py
+-rw-r--r--   0        0        0     3074 2023-05-10 03:18:57.202008 dogfood_logger-0.1.5/dogfood_logger/logger.py
+-rw-r--r--   0        0        0       42 2023-05-10 02:17:04.332370 dogfood_logger-0.1.5/dogfood_logger/packageData/sampleData.dat
+-rw-r--r--   0        0        0      370 2023-05-10 04:04:11.138571 dogfood_logger-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 dogfood_logger-0.1.5/PKG-INFO
```

### Comparing `dogfood_logger-0.1.4/LICENSE.txt` & `dogfood_logger-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dogfood_logger-0.1.4/dogfood_logger/logger.py` & `dogfood_logger-0.1.5/dogfood_logger/logger.py`

 * *Files identical despite different names*

### Comparing `dogfood_logger-0.1.4/PKG-INFO` & `dogfood_logger-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogfood-logger
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

