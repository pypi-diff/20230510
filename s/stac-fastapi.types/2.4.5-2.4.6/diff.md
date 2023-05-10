# Comparing `tmp/stac-fastapi.types-2.4.5.tar.gz` & `tmp/stac-fastapi.types-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.types-2.4.5.tar", last modified: Wed Apr  5 14:03:37 2023, max compression
+gzip compressed data, was "stac-fastapi.types-2.4.6.tar", last modified: Wed May 10 15:53:01 2023, max compression
```

## Comparing `stac-fastapi.types-2.4.5.tar` & `stac-fastapi.types-2.4.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:37.196875 stac-fastapi.types-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-05 14:03:37.196875 stac-fastapi.types-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-05 14:03:37.196875 stac-fastapi.types-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:37.192875 stac-fastapi.types-2.4.5/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:37.196875 stac-fastapi.types-2.4.5/stac_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/links.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 14:03:26.000000 stac-fastapi.types-2.4.5/stac_fastapi/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:37.192875 stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-05 14:03:37.000000 stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-05 14:03:37.000000 stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:03:37.000000 stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:03:37.000000 stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-05 14:03:37.000000 stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-05 14:03:37.000000 stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:01.438334 stac-fastapi.types-2.4.6/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/stac_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 15:52:48.000000 stac-fastapi.types-2.4.6/stac_fastapi/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:01.442334 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:53:01.000000 stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/top_level.txt
```

### Comparing `stac-fastapi.types-2.4.5/PKG-INFO` & `stac-fastapi.types-2.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
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

### Comparing `stac-fastapi.types-2.4.5/setup.py` & `stac-fastapi.types-2.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 install_requires = [
     "fastapi>=0.73.0",
     "attrs",
     "pydantic[dotenv]",
     "stac_pydantic==2.0.*",
     "pystac==1.*",
-    "iso8601~=1.0.2",
+    "iso8601>=1.0.2,<1.2.0",
 ]
 
 extra_reqs = {
     "dev": [
         "pytest",
         "pytest-cov",
         "pytest-asyncio",
```

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/config.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/config.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/conformance.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/conformance.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/core.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/core.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/errors.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/errors.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/extension.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/extension.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/links.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/links.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/rfc3339.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/rfc3339.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/search.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/search.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi/types/stac.py` & `stac-fastapi.types-2.4.6/stac_fastapi/types/stac.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/PKG-INFO` & `stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
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

### Comparing `stac-fastapi.types-2.4.5/stac_fastapi.types.egg-info/SOURCES.txt` & `stac-fastapi.types-2.4.6/stac_fastapi.types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

