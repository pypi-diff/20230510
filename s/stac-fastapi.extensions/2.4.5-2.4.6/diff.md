# Comparing `tmp/stac-fastapi.extensions-2.4.5.tar.gz` & `tmp/stac-fastapi.extensions-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.extensions-2.4.5.tar", last modified: Wed Apr  5 14:03:42 2023, max compression
+gzip compressed data, was "stac-fastapi.extensions-2.4.6.tar", last modified: Wed May 10 15:53:08 2023, max compression
```

## Comparing `stac-fastapi.extensions-2.4.5.tar` & `stac-fastapi.extensions-2.4.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.372911 stac-fastapi.extensions-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-05 14:03:42.372911 stac-fastapi.extensions-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-05 14:03:42.372911 stac-fastapi.extensions-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.364911 stac-fastapi.extensions-2.4.5/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.368911 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.368911 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.368911 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/fields/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/fields/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.368911 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/filter/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.368911 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/pagination/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/pagination/token_pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.372911 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/query/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/query/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.372911 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/sort/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/sort/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/sort/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.372911 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/third_party/bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 14:03:26.000000 stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:42.368911 stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-05 14:03:42.000000 stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-05 14:03:42.000000 stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:03:42.000000 stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:03:42.000000 stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-05 14:03:42.000000 stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-05 14:03:42.000000 stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 15:53:08.086403 stac-fastapi.extensions-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 15:53:08.086403 stac-fastapi.extensions-2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/token_pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/third_party/bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 15:52:48.000000 stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:08.082404 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:53:08.000000 stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/top_level.txt
```

### Comparing `stac-fastapi.extensions-2.4.5/PKG-INFO` & `stac-fastapi.extensions-2.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 2.4.5
+Version: 2.4.6
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.extensions-2.4.5/setup.py` & `stac-fastapi.extensions-2.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/__init__.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/context.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/context.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/fields/fields.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/fields.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/fields/request.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/fields/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/filter/filter.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/filter.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/filter/request.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/filter/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/pagination/pagination.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/pagination/token_pagination.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/pagination/token_pagination.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/query/query.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/query/query.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/sort/request.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/sort/sort.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/sort/sort.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/core/transaction.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/core/transaction.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi/extensions/third_party/bulk_transactions.py` & `stac-fastapi.extensions-2.4.6/stac_fastapi/extensions/third_party/bulk_transactions.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/PKG-INFO` & `stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 2.4.5
+Version: 2.4.6
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.extensions-2.4.5/stac_fastapi.extensions.egg-info/SOURCES.txt` & `stac-fastapi.extensions-2.4.6/stac_fastapi.extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

