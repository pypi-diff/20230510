# Comparing `tmp/azure-datalake-store-0.0.8.tar.gz` & `tmp/azure-datalake-store-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-datalake-store-0.0.8.tar", last modified: Mon May  1 16:50:51 2017, max compression
+gzip compressed data, was "dist/azure-datalake-store-0.0.9.tar", last modified: Thu May 11 18:27:55 2017, max compression
```

## Comparing `azure-datalake-store-0.0.8.tar` & `azure-datalake-store-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure/datalake/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure/datalake/store/
--rw-r--r--   0 travis    (1000) travis    (1000)      582 2017-05-01 16:50:08.000000 azure-datalake-store-0.0.8/azure/datalake/store/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    35273 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/azure/datalake/store/core.py
--rw-r--r--   0 travis    (1000) travis    (1000)      557 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/azure/datalake/store/enums.py
--rw-r--r--   0 travis    (1000) travis    (1000)      855 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/azure/datalake/store/exceptions.py
--rw-r--r--   0 travis    (1000) travis    (1000)    16177 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/azure/datalake/store/lib.py
--rw-r--r--   0 travis    (1000) travis    (1000)    20907 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/azure/datalake/store/multithread.py
--rw-r--r--   0 travis    (1000) travis    (1000)    20814 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/azure/datalake/store/transfer.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5211 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/azure/datalake/store/utils.py
--rw-r--r--   0 travis    (1000) travis    (1000)       56 2017-05-01 16:50:08.000000 azure-datalake-store-0.0.8/azure/datalake/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)       56 2017-05-01 16:50:08.000000 azure-datalake-store-0.0.8/azure/__init__.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure_datalake_store.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)    10549 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure_datalake_store.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      734 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure_datalake_store.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure_datalake_store.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-01 16:50:20.000000 azure-datalake-store-0.0.8/azure_datalake_store.egg-info/not-zip-safe
--rw-r--r--   0 travis    (1000) travis    (1000)       99 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure_datalake_store.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       14 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/azure_datalake_store.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/docs/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/docs/source/
--rw-r--r--   0 travis    (1000) travis    (1000)     1032 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/docs/source/api.rst
--rw-r--r--   0 travis    (1000) travis    (1000)     4104 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/docs/source/index.rst
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/samples/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/samples/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     8531 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/samples/benchmarks.py
--rw-r--r--   0 travis    (1000) travis    (1000)    16355 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/samples/cli.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2593 2017-05-01 16:50:08.000000 azure-datalake-store-0.0.8/HISTORY.rst
--rw-r--r--   0 travis    (1000) travis    (1000)      243 2017-05-01 16:50:08.000000 azure-datalake-store-0.0.8/MANIFEST.in
--rw-r--r--   0 travis    (1000) travis    (1000)     5458 2017-05-01 16:50:08.000000 azure-datalake-store-0.0.8/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)    21096 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/azure_bdist_wheel.py
--rw-r--r--   0 travis    (1000) travis    (1000)      105 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1995 2017-05-01 16:50:09.000000 azure-datalake-store-0.0.8/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10549 2017-05-01 16:50:51.000000 azure-datalake-store-0.0.8/PKG-INFO
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure/datalake/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure/datalake/store/
+-rw-r--r--   0 travis    (1000) travis    (1000)      582 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/store/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    35273 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/store/core.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      557 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/store/enums.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      855 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/store/exceptions.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    16837 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/store/lib.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    20907 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/store/multithread.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    20814 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/store/transfer.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     5211 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/store/utils.py
+-rw-r--r--   0 travis    (1000) travis    (1000)       56 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/datalake/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)       56 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure/__init__.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure_datalake_store.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)    10747 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure_datalake_store.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      734 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure_datalake_store.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure_datalake_store.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-11 18:27:27.000000 azure-datalake-store-0.0.9/azure_datalake_store.egg-info/not-zip-safe
+-rw-r--r--   0 travis    (1000) travis    (1000)       99 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure_datalake_store.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       14 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/azure_datalake_store.egg-info/top_level.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/docs/
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/docs/source/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1032 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/docs/source/api.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)     4104 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/docs/source/index.rst
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/samples/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/samples/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     8531 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/samples/benchmarks.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    16355 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/samples/cli.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     2759 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/HISTORY.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)      243 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/MANIFEST.in
+-rw-r--r--   0 travis    (1000) travis    (1000)     5458 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/README.rst
+-rw-r--r--   0 travis    (1000) travis    (1000)    21096 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/azure_bdist_wheel.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      105 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     1995 2017-05-11 18:27:16.000000 azure-datalake-store-0.0.9/setup.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    10747 2017-05-11 18:27:55.000000 azure-datalake-store-0.0.9/PKG-INFO
```

### Comparing `azure-datalake-store-0.0.8/azure/datalake/store/__init__.py` & `azure-datalake-store-0.0.9/azure/datalake/store/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 from .core import AzureDLFileSystem
 from .multithread import ADLDownloader
 
 # Set default logging handler
 import logging
 from logging import NullHandler
```

### Comparing `azure-datalake-store-0.0.8/azure/datalake/store/core.py` & `azure-datalake-store-0.0.9/azure/datalake/store/core.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/azure/datalake/store/enums.py` & `azure-datalake-store-0.0.9/azure/datalake/store/enums.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/azure/datalake/store/exceptions.py` & `azure-datalake-store-0.0.9/azure/datalake/store/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/azure/datalake/store/lib.py` & `azure-datalake-store-0.0.9/azure/datalake/store/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,29 @@
 import platform
 
 # 3rd party imports
 import adal
 import requests
 import requests.exceptions
 
+# this is required due to github issue, to ensure we don't lose perf from openPySSL: https://github.com/pyca/pyopenssl/issues/625
+enforce_no_py_open_ssl = None
+try:
+    from requests.packages.urllib3.contrib.pyopenssl import extract_from_urllib3 as enforce_no_py_open_ssl
+except ImportError:
+    # in the case of debian/ubuntu system packages, the import is slightly different
+    try:
+        from urllib3.contrib.pyopenssl import extract_from_urllib3 as enforce_no_py_open_ssl
+    except ImportError:
+        # if OpenSSL is unavailable in both cases then there is no need to "undo" it.
+        pass
+
+if enforce_no_py_open_ssl:
+    enforce_no_py_open_ssl()
+
 from msrest.authentication import Authentication
 from .exceptions import DatalakeBadOffsetException, DatalakeRESTException
 from .exceptions import FileNotFoundError, PermissionError
 from . import __version__
 
 logger = logging.getLogger(__name__)
```

### Comparing `azure-datalake-store-0.0.8/azure/datalake/store/multithread.py` & `azure-datalake-store-0.0.9/azure/datalake/store/multithread.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/azure/datalake/store/transfer.py` & `azure-datalake-store-0.0.9/azure/datalake/store/transfer.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/azure/datalake/store/utils.py` & `azure-datalake-store-0.0.9/azure/datalake/store/utils.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/azure_datalake_store.egg-info/PKG-INFO` & `azure-datalake-store-0.0.9/azure_datalake_store.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: azure-datalake-store
-Version: 0.0.8
+Version: 0.0.9
 Summary: Azure Data Lake Store Filesystem Client Library for Python
 Home-page: https://github.com/Azure/azure-data-lake-store-python
 Author: Microsoft Corporation
 Author-email: ptvshelp@microsoft.com
 License: MIT License
 Description: azure-datalake-store
         ====================
@@ -160,14 +160,18 @@
             >
         
         
         .. :changelog:
         
         Release History
         ===============
+        0.0.9 (2017-05-09)
+        ------------------
+        * Enforce basic SSL utilization to ensure performance due to `GitHub issue 625 <https://github.com/pyca/pyopenssl/issues/625>`
+        
         0.0.8 (2017-04-26)
         ------------------
         * Fix server-side throttling retry support. This is not a guarantee that if the server is throttling the upload (or download) it will eventually succeed, but there is now a back-off retry in place to make it more likely.
         
         0.0.7 (2017-04-19)
         ------------------
         * Update the build process to more efficiently handle multi-part namespaces for pip.
```

### Comparing `azure-datalake-store-0.0.8/azure_datalake_store.egg-info/SOURCES.txt` & `azure-datalake-store-0.0.9/azure_datalake_store.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/docs/source/api.rst` & `azure-datalake-store-0.0.9/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/docs/source/index.rst` & `azure-datalake-store-0.0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/samples/benchmarks.py` & `azure-datalake-store-0.0.9/samples/benchmarks.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/samples/cli.py` & `azure-datalake-store-0.0.9/samples/cli.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/HISTORY.rst` & `azure-datalake-store-0.0.9/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 .. :changelog:
 
 Release History
 ===============
+0.0.9 (2017-05-09)
+------------------
+* Enforce basic SSL utilization to ensure performance due to `GitHub issue 625 <https://github.com/pyca/pyopenssl/issues/625>`
+
 0.0.8 (2017-04-26)
 ------------------
 * Fix server-side throttling retry support. This is not a guarantee that if the server is throttling the upload (or download) it will eventually succeed, but there is now a back-off retry in place to make it more likely.
 
 0.0.7 (2017-04-19)
 ------------------
 * Update the build process to more efficiently handle multi-part namespaces for pip.
```

### Comparing `azure-datalake-store-0.0.8/README.rst` & `azure-datalake-store-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/azure_bdist_wheel.py` & `azure-datalake-store-0.0.9/azure_bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/setup.py` & `azure-datalake-store-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `azure-datalake-store-0.0.8/PKG-INFO` & `azure-datalake-store-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: azure-datalake-store
-Version: 0.0.8
+Version: 0.0.9
 Summary: Azure Data Lake Store Filesystem Client Library for Python
 Home-page: https://github.com/Azure/azure-data-lake-store-python
 Author: Microsoft Corporation
 Author-email: ptvshelp@microsoft.com
 License: MIT License
 Description: azure-datalake-store
         ====================
@@ -160,14 +160,18 @@
             >
         
         
         .. :changelog:
         
         Release History
         ===============
+        0.0.9 (2017-05-09)
+        ------------------
+        * Enforce basic SSL utilization to ensure performance due to `GitHub issue 625 <https://github.com/pyca/pyopenssl/issues/625>`
+        
         0.0.8 (2017-04-26)
         ------------------
         * Fix server-side throttling retry support. This is not a guarantee that if the server is throttling the upload (or download) it will eventually succeed, but there is now a back-off retry in place to make it more likely.
         
         0.0.7 (2017-04-19)
         ------------------
         * Update the build process to more efficiently handle multi-part namespaces for pip.
```

