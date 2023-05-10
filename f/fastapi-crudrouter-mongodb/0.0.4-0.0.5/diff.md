# Comparing `tmp/fastapi-crudrouter-mongodb-0.0.4.tar.gz` & `tmp/fastapi-crudrouter-mongodb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-crudrouter-mongodb-0.0.4.tar", last modified: Mon Apr 10 12:03:58 2023, max compression
+gzip compressed data, was "fastapi-crudrouter-mongodb-0.0.5.tar", last modified: Wed May 10 21:32:19 2023, max compression
```

## Comparing `fastapi-crudrouter-mongodb-0.0.4.tar` & `fastapi-crudrouter-mongodb-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/
--rw-r--r--   0 pierro    (1000) pierro    (1000)     1070 2023-04-09 10:32:33.000000 fastapi-crudrouter-mongodb-0.0.4/LICENSE
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     4732 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/PKG-INFO
--rw-r--r--   0 pierro    (1000) pierro    (1000)     3370 2023-04-10 11:52:16.000000 fastapi-crudrouter-mongodb-0.0.4/README.md
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.895207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      279 2023-04-10 12:03:13.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      177 2023-04-09 11:15:45.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      134 2023-04-09 10:58:04.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/CRUDEmbed.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      384 2023-04-09 10:54:52.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/CRUDLookup.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      191 2023-04-09 11:09:33.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/__init__.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1145 2023-04-09 10:50:18.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/mongo_model.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      400 2023-04-09 10:50:03.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     6253 2023-04-09 19:39:43.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1464 2023-04-09 10:51:15.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1963 2023-04-09 19:40:02.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      220 2023-04-09 11:17:14.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     5101 2023-04-09 11:00:10.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1433 2023-04-09 10:59:36.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     3152 2023-04-09 19:57:13.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       82 2023-04-09 11:18:46.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     6480 2023-04-09 10:57:21.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1432 2023-04-09 19:40:37.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     3730 2023-04-09 10:57:30.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       86 2023-04-09 11:18:20.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     4732 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1398 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)        1 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       31 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/requires.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       27 2023-04-10 12:03:58.000000 fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/top_level.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       38 2023-04-10 12:03:58.899207 fastapi-crudrouter-mongodb-0.0.4/setup.cfg
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1720 2023-04-10 12:03:09.000000 fastapi-crudrouter-mongodb-0.0.4/setup.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     1070 2023-04-09 10:32:33.000000 fastapi-crudrouter-mongodb-0.0.5/LICENSE
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     5268 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/PKG-INFO
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     3906 2023-04-14 08:07:27.000000 fastapi-crudrouter-mongodb-0.0.5/README.md
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-05-10 21:32:19.331092 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      279 2023-05-10 20:43:01.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      177 2023-05-10 20:33:11.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/models/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      134 2023-04-09 10:58:04.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/models/CRUDEmbed.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      384 2023-04-09 10:54:52.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/models/CRUDLookup.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      191 2023-04-09 11:09:33.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/models/__init__.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1145 2023-04-09 10:50:18.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/models/mongo_model.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      400 2023-04-09 10:50:03.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     8580 2023-05-10 21:29:59.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1607 2023-05-10 20:54:22.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1963 2023-04-09 19:40:02.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      221 2023-05-10 20:33:17.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/embed/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     5101 2023-04-09 11:00:10.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1433 2023-04-09 10:59:36.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     3152 2023-04-09 19:57:13.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       82 2023-04-09 11:18:46.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/embed/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/lookup/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     6480 2023-04-09 10:57:21.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1432 2023-04-09 19:40:37.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     3730 2023-04-09 10:57:30.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       86 2023-04-09 11:18:20.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/lookup/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb.egg-info/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     5268 2023-05-10 21:32:19.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1398 2023-05-10 21:32:19.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)        1 2023-05-10 21:32:19.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       31 2023-05-10 21:32:19.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       27 2023-05-10 21:32:19.000000 fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb.egg-info/top_level.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       38 2023-05-10 21:32:19.335092 fastapi-crudrouter-mongodb-0.0.5/setup.cfg
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1720 2023-05-10 20:42:57.000000 fastapi-crudrouter-mongodb-0.0.5/setup.py
```

### Comparing `fastapi-crudrouter-mongodb-0.0.4/LICENSE` & `fastapi-crudrouter-mongodb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/PKG-INFO` & `fastapi-crudrouter-mongodb-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-crudrouter-mongodb
-Version: 0.0.4
+Version: 0.0.5
 Summary: A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models
 Home-page: https://github.com/pierrod/fastapi-crudrouter-mongodb
 Author: Pierre DUVEAU
 Author-email: 
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Internet
@@ -32,14 +32,19 @@
   <img src="./docs/assets/img/logo-long-color.png" height="200" />
 </p>
 <p align="center">
   <em>⚡ Create CRUD routes with lighting speed</em> ⚡</br>
   <sub>A dynamic FastAPI router that automatically creates CRUD routes for your Mongodb models</sub>
 </p>
 
+<div align="center">
+
+![Monthly Downloads Shield Badge](https://img.shields.io/pypi/dm/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Weekly Downloads Shield Badge](https://img.shields.io/pypi/dw/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Python Version](https://img.shields.io/pypi/v/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Python Version](https://img.shields.io/pypi/pyversions/fastapi-crudrouter-mongodb?color=3776AB&style=for-the-badge&logo=python&logoColor=white)
+
+</div>
 ---
 
 **Documentation**: [https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/)
 
 **Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
 **Credits** :
```

### Comparing `fastapi-crudrouter-mongodb-0.0.4/README.md` & `fastapi-crudrouter-mongodb-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,19 @@
   <img src="./docs/assets/img/logo-long-color.png" height="200" />
 </p>
 <p align="center">
   <em>⚡ Create CRUD routes with lighting speed</em> ⚡</br>
   <sub>A dynamic FastAPI router that automatically creates CRUD routes for your Mongodb models</sub>
 </p>
 
+<div align="center">
+
+![Monthly Downloads Shield Badge](https://img.shields.io/pypi/dm/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Weekly Downloads Shield Badge](https://img.shields.io/pypi/dw/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Python Version](https://img.shields.io/pypi/v/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Python Version](https://img.shields.io/pypi/pyversions/fastapi-crudrouter-mongodb?color=3776AB&style=for-the-badge&logo=python&logoColor=white)
+
+</div>
 ---
 
 **Documentation**: [https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/)
 
 **Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
 **Credits** :
```

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/models/mongo_model.py` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/models/mongo_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/PKG-INFO` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-crudrouter-mongodb
-Version: 0.0.4
+Version: 0.0.5
 Summary: A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models
 Home-page: https://github.com/pierrod/fastapi-crudrouter-mongodb
 Author: Pierre DUVEAU
 Author-email: 
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Internet
@@ -32,14 +32,19 @@
   <img src="./docs/assets/img/logo-long-color.png" height="200" />
 </p>
 <p align="center">
   <em>⚡ Create CRUD routes with lighting speed</em> ⚡</br>
   <sub>A dynamic FastAPI router that automatically creates CRUD routes for your Mongodb models</sub>
 </p>
 
+<div align="center">
+
+![Monthly Downloads Shield Badge](https://img.shields.io/pypi/dm/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Weekly Downloads Shield Badge](https://img.shields.io/pypi/dw/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Python Version](https://img.shields.io/pypi/v/fastapi-crudrouter-mongodb?color=50b052&style=for-the-badge) ![Python Version](https://img.shields.io/pypi/pyversions/fastapi-crudrouter-mongodb?color=3776AB&style=for-the-badge&logo=python&logoColor=white)
+
+</div>
 ---
 
 **Documentation**: [https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/](https://pierrod.github.io/fastapi-crudrouter-mongodb-doc/)
 
 **Source Code**: [https://github.com/pierrod/fastapi-crudrouter-mongodb](https://github.com/pierrod/fastapi-crudrouter-mongodb)
 
 **Credits** :
```

### Comparing `fastapi-crudrouter-mongodb-0.0.4/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt` & `fastapi-crudrouter-mongodb-0.0.5/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.4/setup.py` & `fastapi-crudrouter-mongodb-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fastapi-crudrouter-mongodb",
-    version="0.0.4",
+    version="0.0.5",
     author="Pierre DUVEAU",
     author_email="",
     description="A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pierrod/fastapi-crudrouter-mongodb",
     packages=find_packages(),
```

