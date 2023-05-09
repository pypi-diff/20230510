# Comparing `tmp/Hunabku_siiu-0.0.3.tar.gz` & `tmp/Hunabku_siiu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_siiu-0.0.3.tar", last modified: Sun May  7 18:37:12 2023, max compression
+gzip compressed data, was "Hunabku_siiu-0.0.4.tar", last modified: Tue May  9 22:54:38 2023, max compression
```

## Comparing `Hunabku_siiu-0.0.3.tar` & `Hunabku_siiu-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/hunabku_siiu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/hunabku_siiu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/hunabku_siiu/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/hunabku_siiu/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/hunabku_siiu/endpoints/SIIU.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 22:54:38.000000 Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/hunabku_siiu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/hunabku_siiu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/hunabku_siiu/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/hunabku_siiu/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/hunabku_siiu/endpoints/SIIU.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:54:38.182297 Hunabku_siiu-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-09 22:54:24.000000 Hunabku_siiu-0.0.4/setup.py
```

### Comparing `Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/PKG-INFO` & `Hunabku_siiu-0.0.4/Hunabku_siiu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-siiu
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_siiu-0.0.3/PKG-INFO` & `Hunabku_siiu-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_siiu
-Version: 0.0.3
+Version: 0.0.4
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_siiu-0.0.3/README.md` & `Hunabku_siiu-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_siiu-0.0.3/hunabku_siiu/endpoints/SIIU.py` & `Hunabku_siiu-0.0.4/hunabku_siiu/endpoints/SIIU.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from hunabku.HunabkuBase import HunabkuPluginBase, endpoint
 from hunabku.Config import Config, Param
 from pymongo import MongoClient
-from elasticsearch import Elasticsearch, helpers
+from elasticsearch import Elasticsearch, helpers, __version__ as es_version
 from elasticsearch_dsl import Search
 import time
 
 
 class SIIU(HunabkuPluginBase):
     config = Config()
     config += Param(mdb_uri="mongodb://localhost:27017/",
@@ -20,16 +20,19 @@
                     doc="Elastic Search password")
     config += Param(es_project_index="siiu_project",
                     doc="Elastic Search siiu project index name")
 
     def __init__(self, hunabku):
         super().__init__(hunabku)
         self.dbclient = MongoClient(self.config.mdb_uri)
-        basic_auth = (self.config.es_user, self.config.es_pass)
-        self.es = Elasticsearch(self.config.es_uri, basic_auth=basic_auth)
+        auth = (self.config.es_user, self.config.es_pass)
+        if es_version[0] < 8:
+            self.es = Elasticsearch(self.config.es_uri, http_auth=auth)
+        else:
+            self.es = Elasticsearch(self.config.es_uri, basic_auth=auth)
 
     @endpoint('/siiu/project', methods=['GET'])
     def siiu_project(self):
         """
         @api {get} /siiu/project Project
         @apiName Project
         @apiGroup SIIU
@@ -192,15 +195,15 @@
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
             # all the products for the user
             curl -i http://apis.colav.co/siiu/info?apikey=XXXX
         """
-        data = list(self.dbclient[self.config.db_name]
+        data = list(self.dbclient[self.config.mdb_name]
                     ["project"].find({}, {'_id': 0, 'CODIGO': 1}))
         response = self.app.response_class(
             response=self.json.dumps(data),
             status=200,
             mimetype='application/json'
         )
         return response
```

### Comparing `Hunabku_siiu-0.0.3/setup.py` & `Hunabku_siiu-0.0.4/setup.py`

 * *Files identical despite different names*

