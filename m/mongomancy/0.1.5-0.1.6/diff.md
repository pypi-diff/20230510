# Comparing `tmp/mongomancy-0.1.5.tar.gz` & `tmp/mongomancy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.1.5.tar", last modified: Wed May 10 08:26:29 2023, max compression
+gzip compressed data, was "mongomancy-0.1.6.tar", last modified: Wed May 10 08:34:40 2023, max compression
```

## Comparing `mongomancy-0.1.5.tar` & `mongomancy-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:26:29.418511 mongomancy-0.1.5/
--rw-r--r--   0 trval     (1000) trval     (1000)     1866 2023-05-10 08:26:11.000000 mongomancy-0.1.5/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.5/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.5/LICENSE
--rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.5/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 08:26:29.418511 mongomancy-0.1.5/PKG-INFO
--rw-r--r--   0 trval     (1000) trval     (1000)     3675 2023-05-10 08:26:11.000000 mongomancy-0.1.5/README.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.5/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.5/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-10 08:26:29.418511 mongomancy-0.1.5/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:26:29.415177 mongomancy-0.1.5/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:26:29.415177 mongomancy-0.1.5/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-10 08:26:11.000000 mongomancy-0.1.5/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    13993 2023-05-10 08:26:11.000000 mongomancy-0.1.5/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.5/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.5/src/mongomancy/py.typed
--rw-r--r--   0 trval     (1000) trval     (1000)    15479 2023-05-10 08:26:11.000000 mongomancy-0.1.5/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     6194 2023-05-10 08:26:11.000000 mongomancy-0.1.5/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:26:29.418511 mongomancy-0.1.5/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 08:26:29.000000 mongomancy-0.1.5/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-10 08:26:29.000000 mongomancy-0.1.5/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-10 08:26:29.000000 mongomancy-0.1.5/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-10 08:26:29.000000 mongomancy-0.1.5/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-10 08:26:29.000000 mongomancy-0.1.5/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:34:40.132743 mongomancy-0.1.6/
+-rw-r--r--   0 trval     (1000) trval     (1000)     1947 2023-05-10 08:34:13.000000 mongomancy-0.1.6/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.6/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.6/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 08:34:40.132743 mongomancy-0.1.6/PKG-INFO
+-rw-r--r--   0 trval     (1000) trval     (1000)     3675 2023-05-10 08:26:11.000000 mongomancy-0.1.6/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.6/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.6/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-10 08:34:40.132743 mongomancy-0.1.6/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:34:40.129410 mongomancy-0.1.6/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:34:40.132743 mongomancy-0.1.6/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-10 08:34:13.000000 mongomancy-0.1.6/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    13993 2023-05-10 08:26:11.000000 mongomancy-0.1.6/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.6/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.6/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    15558 2023-05-10 08:31:22.000000 mongomancy-0.1.6/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     6194 2023-05-10 08:26:11.000000 mongomancy-0.1.6/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-10 08:34:40.132743 mongomancy-0.1.6/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4466 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-10 08:34:40.000000 mongomancy-0.1.6/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.1.5/CHANGELOG.md` & `mongomancy-0.1.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.1.5] - 2023-05-09
+## [0.1.6] - 2023-05-10
+
+### Fix
+
+- broken default data insert from last commit
+
+## [0.1.5] - 2023-05-10
 
 ### Fixed
 
 - reset references correctly after dispose
 - query repeat on fail - queries are now actually repeated on new collection instance instead of disconnected one
 
 ## [0.1.4] - 2023-05-09
```

### Comparing `mongomancy-0.1.5/CONTRIBUTING.md` & `mongomancy-0.1.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.5/LICENSE` & `mongomancy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.5/PKG-INFO` & `mongomancy-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.1.5/README.md` & `mongomancy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.5/pyproject.toml` & `mongomancy-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.5/src/mongomancy/engine.py` & `mongomancy-0.1.6/src/mongomancy/engine.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.5/src/mongomancy/mongo_errors.py` & `mongomancy-0.1.6/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.5/src/mongomancy/schema.py` & `mongomancy-0.1.6/src/mongomancy/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,18 @@
     def pymongo_collection(self, value: pymongo.collection.Collection) -> None:
         self.dialect_entity = value
 
     @property
     def name(self) -> str:
         return self.pymongo_collection.name
 
+    @property
+    def full_name(self) -> str:
+        return self.pymongo_collection.full_name
+
     def find_one(
         self,
         where: Optional[types.BsonDict],
         *args,
         **kwargs,
     ) -> Optional[DocumentType]:
         return self.engine.find_one(self, where, *args, **kwargs)
@@ -444,15 +448,15 @@
         Insert default data from definition into collection.
 
         :param docs: default docs
         :param collection: new collection to insert defaults into
         :return: docs created
         """
         new_docs_cnt = 0
-        coll_name = collection.mongo_collection.full_name
+        coll_name = collection.full_name
         for doc in docs:
             if not collection.find_one(doc.unique_key, {"_id": 1}):
                 self.logger.debug(f"{coll_name} - inserting default {doc!r}")
                 _ = collection.insert_one(doc.data)
                 new_docs_cnt += 1
                 self.logger.debug(f"{coll_name} - inserted new default {doc!r}")
                 self.logger.info(f"{coll_name} - inserted new default {doc.unique_key!r}")
```

### Comparing `mongomancy-0.1.5/src/mongomancy/types.py` & `mongomancy-0.1.6/src/mongomancy/types.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.5/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.1.6/src/mongomancy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

