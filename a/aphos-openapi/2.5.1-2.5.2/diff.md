# Comparing `tmp/aphos_openapi-2.5.1.tar.gz` & `tmp/aphos_openapi-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aphos_openapi-2.5.1.tar", last modified: Tue May  9 21:33:44 2023, max compression
+gzip compressed data, was "aphos_openapi-2.5.2.tar", last modified: Tue May  9 22:08:13 2023, max compression
```

## Comparing `aphos_openapi-2.5.1.tar` & `aphos_openapi-2.5.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.112702 aphos_openapi-2.5.1/aphos_openapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/aphos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/aphos_openapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/catalog_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/flux_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/space_object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/aphos_openapi/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/aphos_openapi/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/comparison_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/flux_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/night.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/photo_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/space_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/space_object_with_fluxes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    82630 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/aphos_openapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/models/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/aphos_openapi/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:33:44.112702 aphos_openapi-2.5.1/aphos_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 21:33:44.000000 aphos_openapi-2.5.1/aphos_openapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:33:44.116702 aphos_openapi-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 21:33:32.000000 aphos_openapi-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:08:13.462980 aphos_openapi-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-05-09 22:08:13.462980 aphos_openapi-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:08:13.458980 aphos_openapi-2.5.2/aphos_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/aphos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:08:13.458980 aphos_openapi-2.5.2/aphos_openapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/api/catalog_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/api/flux_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25235 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/api/space_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:08:13.458980 aphos_openapi-2.5.2/aphos_openapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:08:13.458980 aphos_openapi-2.5.2/aphos_openapi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/comparison_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/flux_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/night.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/photo_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/space_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/space_object_with_fluxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82630 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:08:13.458980 aphos_openapi-2.5.2/aphos_openapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/models/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/aphos_openapi/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:08:13.458980 aphos_openapi-2.5.2/aphos_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-05-09 22:08:13.000000 aphos_openapi-2.5.2/aphos_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 22:08:13.000000 aphos_openapi-2.5.2/aphos_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:08:13.000000 aphos_openapi-2.5.2/aphos_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 22:08:13.000000 aphos_openapi-2.5.2/aphos_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 22:08:13.000000 aphos_openapi-2.5.2/aphos_openapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:08:13.462980 aphos_openapi-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 22:08:01.000000 aphos_openapi-2.5.2/setup.py
```

### Comparing `aphos_openapi-2.5.1/LICENSE` & `aphos_openapi-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/PKG-INFO` & `aphos_openapi-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: aphos_openapi
-Version: 2.5.1
+Version: 2.5.2
 Summary: APhoS Python library for data representation
 Author: Pavel Kinc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # APhoS client for retrieving data in Python
 
 This is Amateur Photometric Survey (APhoS) client for web application.  
 Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
 Server is accessible from: https://aphos.cerit-sc.cz/  
-Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html
+Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html  
 Openapi json or yaml file (documentation of api): https://aphos.cerit-sc.cz/openapi
 
 ## Installation
 ### Package: `aphos-openapi`
 
 Install: `pip install aphos-openapi`  
 Upgrade: `pip install aphos-openapi --upgrade`
```

### Comparing `aphos_openapi-2.5.1/README.md` & `aphos_openapi-2.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # APhoS client for retrieving data in Python
 
 This is Amateur Photometric Survey (APhoS) client for web application.  
 Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
 Server is accessible from: https://aphos.cerit-sc.cz/  
-Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html
+Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html  
 Openapi json or yaml file (documentation of api): https://aphos.cerit-sc.cz/openapi
 
 ## Installation
 ### Package: `aphos-openapi`
 
 Install: `pip install aphos-openapi`  
 Upgrade: `pip install aphos-openapi --upgrade`
```

### Comparing `aphos_openapi-2.5.1/aphos_openapi/__init__.py` & `aphos_openapi-2.5.2/aphos_openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/aphos.py` & `aphos_openapi-2.5.2/aphos_openapi/aphos.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/api/catalog_api.py` & `aphos_openapi-2.5.2/aphos_openapi/api/catalog_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/api/flux_api.py` & `aphos_openapi-2.5.2/aphos_openapi/api/flux_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/api/space_object_api.py` & `aphos_openapi-2.5.2/aphos_openapi/api/space_object_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/api/user_api.py` & `aphos_openapi-2.5.2/aphos_openapi/api/user_api.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/api_client.py` & `aphos_openapi-2.5.2/aphos_openapi/api_client.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/apis/__init__.py` & `aphos_openapi-2.5.2/aphos_openapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/configuration.py` & `aphos_openapi-2.5.2/aphos_openapi/configuration.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/exceptions.py` & `aphos_openapi-2.5.2/aphos_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/comparison_object.py` & `aphos_openapi-2.5.2/aphos_openapi/model/comparison_object.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/error_message.py` & `aphos_openapi-2.5.2/aphos_openapi/model/error_message.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/flux.py` & `aphos_openapi-2.5.2/aphos_openapi/model/flux.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/flux_data.py` & `aphos_openapi-2.5.2/aphos_openapi/model/flux_data.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/night.py` & `aphos_openapi-2.5.2/aphos_openapi/model/night.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/photo_properties.py` & `aphos_openapi-2.5.2/aphos_openapi/model/photo_properties.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/space_object.py` & `aphos_openapi-2.5.2/aphos_openapi/model/space_object.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/space_object_with_fluxes.py` & `aphos_openapi-2.5.2/aphos_openapi/model/space_object_with_fluxes.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model/user.py` & `aphos_openapi-2.5.2/aphos_openapi/model/user.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/model_utils.py` & `aphos_openapi-2.5.2/aphos_openapi/model_utils.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/models/__init__.py` & `aphos_openapi-2.5.2/aphos_openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/models/coordinates.py` & `aphos_openapi-2.5.2/aphos_openapi/models/coordinates.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/models/graph_data.py` & `aphos_openapi-2.5.2/aphos_openapi/models/graph_data.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi/rest.py` & `aphos_openapi-2.5.2/aphos_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/aphos_openapi.egg-info/PKG-INFO` & `aphos_openapi-2.5.2/aphos_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: aphos-openapi
-Version: 2.5.1
+Version: 2.5.2
 Summary: APhoS Python library for data representation
 Author: Pavel Kinc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # APhoS client for retrieving data in Python
 
 This is Amateur Photometric Survey (APhoS) client for web application.  
 Contains documentation about modules, models and functions for working with astronomical data from APhoS database.  
 Server is accessible from: https://aphos.cerit-sc.cz/  
-Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html
+Swagger UI (Interface for api of the server): https://aphos.cerit-sc.cz/swagger-ui/index.html  
 Openapi json or yaml file (documentation of api): https://aphos.cerit-sc.cz/openapi
 
 ## Installation
 ### Package: `aphos-openapi`
 
 Install: `pip install aphos-openapi`  
 Upgrade: `pip install aphos-openapi --upgrade`
```

### Comparing `aphos_openapi-2.5.1/aphos_openapi.egg-info/SOURCES.txt` & `aphos_openapi-2.5.2/aphos_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aphos_openapi-2.5.1/setup.py` & `aphos_openapi-2.5.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aphos_openapi",
-    version="2.5.1",
+    version="2.5.2",
     author="Pavel Kinc",
     description="APhoS Python library for data representation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license_files=('LICENSE',),
     classifiers=[
```

