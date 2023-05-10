# Comparing `tmp/stac-fastapi.api-2.4.5.tar.gz` & `tmp/stac-fastapi.api-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.api-2.4.5.tar", last modified: Wed Apr  5 14:03:47 2023, max compression
+gzip compressed data, was "stac-fastapi.api-2.4.6.tar", last modified: Wed May 10 15:53:13 2023, max compression
```

## Comparing `stac-fastapi.api-2.4.5.tar` & `stac-fastapi.api-2.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:47.168946 stac-fastapi.api-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-05 14:03:47.168946 stac-fastapi.api-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-05 14:03:47.172946 stac-fastapi.api-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:47.168946 stac-fastapi.api-2.4.5/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:47.168946 stac-fastapi.api-2.4.5/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-05 14:03:26.000000 stac-fastapi.api-2.4.5/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:03:47.168946 stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-05 14:03:47.000000 stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-05 14:03:47.000000 stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:03:47.000000 stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:03:47.000000 stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-05 14:03:47.000000 stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-05 14:03:47.000000 stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:13.574463 stac-fastapi.api-2.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-10 15:53:13.574463 stac-fastapi.api-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 15:53:13.574463 stac-fastapi.api-2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:13.570464 stac-fastapi.api-2.4.6/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:13.574463 stac-fastapi.api-2.4.6/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 15:52:48.000000 stac-fastapi.api-2.4.6/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:53:13.570464 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:53:13.000000 stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/top_level.txt
```

### Comparing `stac-fastapi.api-2.4.5/PKG-INFO` & `stac-fastapi.api-2.4.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
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

### Comparing `stac-fastapi.api-2.4.5/setup.py` & `stac-fastapi.api-2.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "stac_pydantic==2.0.*",
     "brotli_asgi",
     "stac-fastapi.types",
 ]
 
 extra_reqs = {
     "dev": [
+        "httpx",
         "pytest",
         "pytest-cov",
         "pytest-asyncio",
         "pre-commit",
         "requests",
         "pystac[validation]==1.*",
     ],
```

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi/api/app.py` & `stac-fastapi.api-2.4.6/stac_fastapi/api/app.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi/api/config.py` & `stac-fastapi.api-2.4.6/stac_fastapi/api/config.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi/api/errors.py` & `stac-fastapi.api-2.4.6/stac_fastapi/api/errors.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi/api/middleware.py` & `stac-fastapi.api-2.4.6/stac_fastapi/api/middleware.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi/api/models.py` & `stac-fastapi.api-2.4.6/stac_fastapi/api/models.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi/api/openapi.py` & `stac-fastapi.api-2.4.6/stac_fastapi/api/openapi.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi/api/routes.py` & `stac-fastapi.api-2.4.6/stac_fastapi/api/routes.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/PKG-INFO` & `stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
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

### Comparing `stac-fastapi.api-2.4.5/stac_fastapi.api.egg-info/SOURCES.txt` & `stac-fastapi.api-2.4.6/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

