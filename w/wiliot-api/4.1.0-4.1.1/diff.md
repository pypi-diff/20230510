# Comparing `tmp/wiliot-api-4.1.0.tar.gz` & `tmp/wiliot-api-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.1.0.tar", last modified: Mon Mar 20 00:39:59 2023, max compression
+gzip compressed data, was "wiliot-api-4.1.1.tar", last modified: Wed May 10 03:45:39 2023, max compression
```

## Comparing `wiliot-api-4.1.0.tar` & `wiliot-api-4.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.272695 wiliot-api-4.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3056 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7163 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-20 00:39:59.272695 wiliot-api-4.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11124 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13640 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14095 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    33288 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-03-20 00:39:45.000000 wiliot-api-4.1.0/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-20 00:39:59.000000 wiliot-api-4.1.0/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 00:39:59.268695 wiliot-api-4.1.0/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3056 2023-03-20 00:39:59.000000 wiliot-api-4.1.0/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-03-20 00:39:59.000000 wiliot-api-4.1.0/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-20 00:39:59.000000 wiliot-api-4.1.0/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-20 00:39:59.000000 wiliot-api-4.1.0/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-20 00:39:59.000000 wiliot-api-4.1.0/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-03-20 00:39:59.000000 wiliot-api-4.1.0/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11124 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13640 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    14095 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35636 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7223 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.265504 wiliot-api-4.1.1/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-10 03:45:20.000000 wiliot-api-4.1.1/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 03:45:39.261504 wiliot-api-4.1.1/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-10 03:45:39.000000 wiliot-api-4.1.1/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.1.0/LICENSE` & `wiliot-api-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/PKG-INFO` & `wiliot-api-4.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.1.0
+Version: 4.1.1
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,24 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.1.1:
+-----------------
+* Changed additional functions use the metadataFetch API to support larger returned data sets:
+    * Get Locations
+    * Get zones
+    * Get location associations
+    * Get zone associations
+* Added the ability to associate pixels to zones
+* Added the ability to associate bridges and gateways to locations
+
 Version 4.1.0:
 -----------------
 * Changed get_locations and get_categories to use the metadataFetch API endpoint to support:
     * Fetching more than the first 100 items
     * To return the underlying zones for each location when fetching locations
 * Added calls to get, create and delete asset labels
 * Changed get_asset function call to use the metdataFetch endpoint for compatibility with the get_assets call
```

### Comparing `wiliot-api-4.1.0/README.md` & `wiliot-api-4.1.1/wiliot_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: wiliot-api
+Version: 4.1.1
+Summary: A library for interacting with Wiliot's private Cloud API
+Home-page: UNKNOWN
+Author: Wiliot
+Author-email: support@wiliot.com
+License: MIT
+Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyWiliot: wiliot-api #
 
 wiliot-api is a python library for accessing Wiliot's cloud services from Python
 
 ## Public Library
 
 ### MAC Installation
@@ -40,14 +57,24 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.1.1:
+-----------------
+* Changed additional functions use the metadataFetch API to support larger returned data sets:
+    * Get Locations
+    * Get zones
+    * Get location associations
+    * Get zone associations
+* Added the ability to associate pixels to zones
+* Added the ability to associate bridges and gateways to locations
+
 Version 4.1.0:
 -----------------
 * Changed get_locations and get_categories to use the metadataFetch API endpoint to support:
     * Fetching more than the first 100 items
     * To return the underlying zones for each location when fetching locations
 * Added calls to get, create and delete asset labels
 * Changed get_asset function call to use the metdataFetch endpoint for compatibility with the get_assets call
@@ -67,7 +94,9 @@
 for more information please read 'wiliot' package's release notes
   
   
    
 
 
 
+
+
```

### Comparing `wiliot-api-4.1.0/bitbucket-pipelines.yml` & `wiliot-api-4.1.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/setup.py` & `wiliot-api-4.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/__init__.py` & `wiliot-api-4.1.1/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/api_client.py` & `wiliot-api-4.1.1/wiliot_api/api_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/edge/edge.py` & `wiliot-api-4.1.1/wiliot_api/edge/edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.1.1/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.1.1/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.1.1/wiliot_api/manufacturing/manufacturing.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.1.1/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/platform/platform.py` & `wiliot-api-4.1.1/wiliot_api/platform/platform.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,56 +96,21 @@
 class LocationType(Enum):
     SITE = 'SITE'
     TRANSPORTER = 'TRANSPORTER'
 
 
 class ZoneAssociationType(Enum):
     BRIDGE = 'bridge'
+    TAG = 'tag'
 
 
 class LocationAssociationType(Enum):
     BRIDGE = 'bridge'
 
 
-# class Tag(Type):
-#     tagId = String
-#
-#
-# class Category(Type):
-#     id = String
-#     name = String
-#
-#
-# class AssetNode(Type):
-#     id = String
-#     name = String
-#     tags = Field(Tag)
-#     createdAt = Int
-#     createdBy = String
-#     category = Field(Category)
-#
-#
-# class PageInfoNode(Type):
-#     cursor = String
-#     hasNext = Boolean
-#     totalPages = Int
-#
-#
-# class AssetConnection(Type):
-#     page = list_of(AssetNode)
-#     pageInfo = Field(PageInfoNode)
-#
-#
-# class Query(Type):
-#     assets = Field(AssetConnection, args={
-#         'pageSize': Int,
-#         'cursor': String
-#     })
-
-
 class PlatformClient(Client):
     def __init__(self, api_key, owner_id, env='', log_file=None, logger_=None):
         self.client_path = "traceability/owner/{owner_id}/".format(owner_id=owner_id)
         self.owner_id = owner_id
         super().__init__(api_key=api_key, env=env, log_file=log_file, logger_=logger_)
 
     # Tag calls
@@ -655,17 +620,40 @@
     # Associations
     def get_location_associations(self, location_id):
         """
         Get all associations for a given location
         :param location_id: String - Required - The location ID to return associations for
         :return: A list of associations
         """
-        path = f"/location/{location_id}/association"
-        res = self._get(path)
-        return res.get('data', [])
+        path = "/fetchMetadata"
+
+        has_next = True
+        cursor = None
+        poi_associations = []
+        from .platform_models import Query, Operation, StringFilter
+
+        while True:
+            query = Operation(Query)
+            if not has_next:
+                break
+            if cursor is not None:
+                query.poi_associations(poiId={'filterType': 'equalTo', 'value': location_id}, cursor=cursor)
+            else:
+                query.poi_associations(poiId={'filterType': 'equalTo', 'value': location_id})
+            query.poi_associations.page.__fields__()
+            query.poi_associations.pageInfo()
+            payload = {
+                "query": f"{{{query.poi_associations()}}}"
+            }
+            res = self._post(path, payload=payload)
+            has_next = res['data']['poiAssociations']['pageInfo']['hasNext']
+            cursor = res['data']['poiAssociations']['pageInfo']['cursor']
+            poi_associations += res["data"]["poiAssociations"]["page"]
+
+        return poi_associations
 
     def create_location_association(self, location_id, association_type, association_value):
         """
         Create a new association for a location
         :param location_id: String - Required - The ID of the location to create the association for
         :param association_type: LocationAssociationType - Required - The type of association
         :param association_value: String - Required - The value of the association (the bridge ID in case of a bridge
@@ -711,23 +699,47 @@
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete location associations")
             raise e
 
-    def get_zone_associations(self, location_id, zone_id):
+    def get_zone_associations(self, zone_id):
         """
         Get all associations for a given zone
         :param location_id: String - Required - The location ID the zone belongs to
+        :param zone_id: String - Required - The zone ID to query
         :return: A list of associations
         """
-        path = f"/location/{location_id}/zone/{zone_id}/association"
-        res = self._get(path)
-        return res.get('data', [])
+        path = "/fetchMetadata"
+
+        has_next = True
+        cursor = None
+        poi_associations = []
+        from .platform_models import Query, Operation, StringFilter
+
+        while True:
+            query = Operation(Query)
+            if not has_next:
+                break
+            if cursor is not None:
+                query.poi_associations(poiId={'filterType': 'equalTo', 'value': zone_id}, cursor=cursor)
+            else:
+                query.poi_associations(poiId={'filterType': 'equalTo', 'value': zone_id})
+            query.poi_associations.page.__fields__()
+            query.poi_associations.pageInfo()
+            payload = {
+                "query": f"{{{query.poi_associations()}}}"
+            }
+            res = self._post(path, payload=payload)
+            has_next = res['data']['poiAssociations']['pageInfo']['hasNext']
+            cursor = res['data']['poiAssociations']['pageInfo']['cursor']
+            poi_associations += res["data"]["poiAssociations"]["page"]
+
+        return poi_associations
 
     def create_zone_association(self, location_id, zone_id, association_type, association_value):
         """
         Create a new association for a location
         :param location_id: String - Required - The ID of the location to create the association for
         :param zone_id: String - Required -  The ID of the zone to create the association for
         :param association_type: ZoneAssociationType - Required - The type of association
@@ -774,23 +786,52 @@
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete zone associations")
 
     # Zones
-    def get_zones(self, location_id):
+    def get_zones(self, location_id=None):
         """
-        Get all zones under a location
+        Get all zones (can be filtered by location)
         :param location_id: The ID of the location to return zones belonging to
         :return: A list of zones
         """
-        path = f"/location/{location_id}/zone"
-        res = self._get(path)
-        return res.get('data', [])
+        path = "/fetchMetdata"
+
+        has_next = True
+        cursor = None
+        zones = []
+        from .platform_models import Query, Operation, StringFilter
+
+        while True:
+            query = Operation(Query)
+            if not has_next:
+                break
+            if cursor is not None:
+                if location_id is not None:
+                    query.zones(locationId={'value': location_id, 'filterType': 'equalTo'}, cursor=cursor)
+                else:
+                    query.zones(cursor=cursor)
+            else:
+                if location_id is not None:
+                    query.zones(locationId={'value': location_id, 'filterType': 'equalTo'})
+                else:
+                    query.zones()
+            query.zones.page.__fields__()
+            query.zones.pageInfo()
+            payload = {
+                "query": f"{{{query.zones()}}}"
+            }
+            res = self._post(path, payload=payload)
+            has_next = res['data']['zones']['pageInfo']['hasNext']
+            cursor = res['data']['zones']['pageInfo']['cursor']
+            zones += res["data"]["zones"]["page"]
+
+        return zones
 
     def get_zone(self, location_id, zone_id):
         """
         Get all zones under a location
         :param location_id: The ID of the location the zone belongs to
         :param zone_id: The ID of the zone to return
         :return: A list of zones
@@ -860,17 +901,17 @@
             raise e
 
     def query_metadata(self,  query):
         """
         Execute a query to get metadata
         :param query: String - Required - The query to send
         """
-        path = f"metadataFetch"
+        path = f"/metadataFetch"
         payload = {
             "query": query
         }
         try:
             res = self._post(path, payload)
             return res["data"]
         except WiliotCloudError as e:
-            print("Failed to update zone")
-            raise e
+            print("Failed to query metadata")
+            raise e
```

### Comparing `wiliot-api-4.1.0/wiliot_api/platform/platform_models.py` & `wiliot-api-4.1.1/wiliot_api/platform/platform_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,19 +86,35 @@
     ownerId = String
     locationType = String
     lastUpdatedBy = String
     lastUpdatedAt = String
     zones = Field(Zone)
 
 
+class PoiAssociation(Type):
+    associationType = String
+    poiId = String
+    associationValue = String
+
+
 class LocationConnection(Type):
     page = list_of(Location)
     pageInfo = Field(PageInfoNode)
 
 
+class ZoneConnection(Type):
+    page = list_of(Zone)
+    pageInfo = Field(PageInfoNode)
+
+
+class PoiAssociationConnection(Type):
+    page = list_of(PoiAssociation)
+    pageInfo = Field(PageInfoNode)
+
+
 class CategoryConnection(Type):
     page = list_of(Category)
     pageInfo = Field(PageInfoNode)
 
 
 class StringFilter(Type):
     filterType = String
@@ -117,11 +133,23 @@
     })
 
     locations = Field(LocationConnection, args={
         'pageSize': Int,
         'cursor': String
     })
 
+    zones = Field(ZoneConnection, args={
+        'pageSize': Int,
+        'cursor': String,
+        'locationId': StringFilter
+    })
+
+    poi_associations = Field(PoiAssociationConnection, args={
+        'pageSize': Int,
+        'cursor': String,
+        'poiId': StringFilter
+    })
+
     categories = Field(CategoryConnection, args={
         'pageSize': Int,
         'cursor': String
     })
```

### Comparing `wiliot-api-4.1.0/wiliot_api/security/security.py` & `wiliot-api-4.1.1/wiliot_api/security/security.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api/utils/get_version.py` & `wiliot-api-4.1.1/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.1.0/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: wiliot-api
-Version: 4.1.0
-Summary: A library for interacting with Wiliot's private Cloud API
-Home-page: UNKNOWN
-Author: Wiliot
-Author-email: support@wiliot.com
-License: MIT
-Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyWiliot: wiliot-api #
 
 wiliot-api is a python library for accessing Wiliot's cloud services from Python
 
 ## Public Library
 
 ### MAC Installation
@@ -57,14 +40,24 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.1.1:
+-----------------
+* Changed additional functions use the metadataFetch API to support larger returned data sets:
+    * Get Locations
+    * Get zones
+    * Get location associations
+    * Get zone associations
+* Added the ability to associate pixels to zones
+* Added the ability to associate bridges and gateways to locations
+
 Version 4.1.0:
 -----------------
 * Changed get_locations and get_categories to use the metadataFetch API endpoint to support:
     * Fetching more than the first 100 items
     * To return the underlying zones for each location when fetching locations
 * Added calls to get, create and delete asset labels
 * Changed get_asset function call to use the metdataFetch endpoint for compatibility with the get_assets call
@@ -84,9 +77,7 @@
 for more information please read 'wiliot' package's release notes
   
   
    
 
 
 
-
-
```

### Comparing `wiliot-api-4.1.0/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.1.1/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

