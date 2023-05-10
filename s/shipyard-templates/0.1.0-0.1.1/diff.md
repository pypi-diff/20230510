# Comparing `tmp/shipyard_templates-0.1.0.tar.gz` & `tmp/shipyard_templates-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_templates-0.1.0.tar", max compression
+gzip compressed data, was "shipyard_templates-0.1.1.tar", max compression
```

## Comparing `shipyard_templates-0.1.0.tar` & `shipyard_templates-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-04-07 13:46:34.140116 shipyard_templates-0.1.0/README.md
--rw-r--r--   0        0        0      342 2023-04-11 13:08:42.728720 shipyard_templates-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      292 2023-04-07 13:46:34.140699 shipyard_templates-0.1.0/shipyard_templates/__init__.py
--rw-r--r--   0        0        0      552 2023-04-07 13:46:34.140873 shipyard_templates-0.1.0/shipyard_templates/cloudstorage.py
--rw-r--r--   0        0        0     1965 2023-04-07 13:46:34.141099 shipyard_templates-0.1.0/shipyard_templates/database.py
--rw-r--r--   0        0        0      267 2023-04-07 13:46:34.141270 shipyard_templates-0.1.0/shipyard_templates/datavisualization.py
--rw-r--r--   0        0        0     1093 2023-04-10 03:43:07.250794 shipyard_templates-0.1.0/shipyard_templates/etl.py
--rw-r--r--   0        0        0      245 2023-04-07 13:46:34.141569 shipyard_templates-0.1.0/shipyard_templates/messaging.py
--rw-r--r--   0        0        0      235 2023-04-07 13:46:34.141711 shipyard_templates-0.1.0/shipyard_templates/notebooks.py
--rw-r--r--   0        0        0      532 2023-04-07 13:46:34.141852 shipyard_templates-0.1.0/shipyard_templates/shipyard_logger.py
--rw-r--r--   0        0        0      280 2023-04-07 13:46:34.141996 shipyard_templates-0.1.0/shipyard_templates/spreadsheets.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 shipyard_templates-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 15:33:24.335210 shipyard_templates-0.1.1/README.md
+-rw-r--r--   0        0        0      342 2023-05-10 14:49:14.274212 shipyard_templates-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-05-10 14:28:46.511020 shipyard_templates-0.1.1/shipyard_templates/__init__.py
+-rw-r--r--   0        0        0      552 2023-04-18 15:33:24.336079 shipyard_templates-0.1.1/shipyard_templates/cloudstorage.py
+-rw-r--r--   0        0        0     1965 2023-04-18 15:33:24.336218 shipyard_templates-0.1.1/shipyard_templates/database.py
+-rw-r--r--   0        0        0      267 2023-04-18 15:33:24.336346 shipyard_templates-0.1.1/shipyard_templates/datavisualization.py
+-rw-r--r--   0        0        0     1093 2023-04-18 15:33:24.336748 shipyard_templates-0.1.1/shipyard_templates/etl.py
+-rw-r--r--   0        0        0      245 2023-04-18 15:33:24.336885 shipyard_templates-0.1.1/shipyard_templates/messaging.py
+-rw-r--r--   0        0        0      235 2023-04-18 15:33:24.337013 shipyard_templates-0.1.1/shipyard_templates/notebooks.py
+-rw-r--r--   0        0        0      532 2023-04-18 15:33:24.337263 shipyard_templates-0.1.1/shipyard_templates/shipyard_logger.py
+-rw-r--r--   0        0        0      280 2023-04-18 15:33:24.337469 shipyard_templates-0.1.1/shipyard_templates/spreadsheets.py
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 shipyard_templates-0.1.1/PKG-INFO
```

### Comparing `shipyard_templates-0.1.0/shipyard_templates/cloudstorage.py` & `shipyard_templates-0.1.1/shipyard_templates/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.0/shipyard_templates/database.py` & `shipyard_templates-0.1.1/shipyard_templates/database.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.0/shipyard_templates/etl.py` & `shipyard_templates-0.1.1/shipyard_templates/etl.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.0/shipyard_templates/shipyard_logger.py` & `shipyard_templates-0.1.1/shipyard_templates/shipyard_logger.py`

 * *Files identical despite different names*

### Comparing `shipyard_templates-0.1.0/PKG-INFO` & `shipyard_templates-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-templates
-Version: 0.1.0
+Version: 0.1.1
 Summary: Super classes for blueprint development
 License: Apache-2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

