# Comparing `tmp/procurement_bytetheory-1.0.2.tar.gz` & `tmp/procurement_bytetheory-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procurement_bytetheory-1.0.2.tar", last modified: Tue May  9 23:20:18 2023, max compression
+gzip compressed data, was "procurement_bytetheory-1.0.3.tar", last modified: Tue May  9 23:46:51 2023, max compression
```

## Comparing `procurement_bytetheory-1.0.2.tar` & `procurement_bytetheory-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.736373 procurement_bytetheory-1.0.2/
--rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-04-27 14:56:54.000000 procurement_bytetheory-1.0.2/LICENSE
--rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-09 23:20:18.736458 procurement_bytetheory-1.0.2/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 17:35:18.000000 procurement_bytetheory-1.0.2/README.md
--rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-04-27 14:58:37.000000 procurement_bytetheory-1.0.2/pyproject.toml
--rw-r--r--   0 robertblom   (501) staff       (20)      543 2023-05-09 23:20:18.736768 procurement_bytetheory-1.0.2/setup.cfg
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.729614 procurement_bytetheory-1.0.2/src/
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.730785 procurement_bytetheory-1.0.2/src/procurement_bytetheory/
--rw-r--r--   0 robertblom   (501) staff       (20)      295 2023-05-02 16:19:26.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.732469 procurement_bytetheory-1.0.2/src/procurement_bytetheory/controllers/
--rw-r--r--   0 robertblom   (501) staff       (20)      611 2023-04-28 20:46:41.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/controllers/CLIController.py
--rw-r--r--   0 robertblom   (501) staff       (20)       63 2023-05-02 14:53:25.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/controllers/Observer.py
--rw-r--r--   0 robertblom   (501) staff       (20)     1877 2023-05-09 23:19:12.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/controllers/UIController.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:35.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/controllers/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.732985 procurement_bytetheory-1.0.2/src/procurement_bytetheory/data/
--rw-r--r--   0 robertblom   (501) staff       (20)    86016 2023-05-09 23:20:15.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/data/ProcurementGame.db
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 15:08:49.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/data/__init__.py
--rw-r--r--   0 robertblom   (501) staff       (20)      397 2023-05-02 20:07:41.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/data/items.csv
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.733909 procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/
--rw-r--r--   0 robertblom   (501) staff       (20)     2440 2023-05-03 14:15:31.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     3510 2023-05-03 14:20:12.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/DatabaseHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2524 2023-05-03 19:02:03.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2387 2023-05-03 16:58:38.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/ItemDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2429 2023-05-03 19:02:11.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/MarketDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:07.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.735129 procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/
--rw-r--r--   0 robertblom   (501) staff       (20)     4427 2023-05-09 23:00:26.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Business.py
--rw-r--r--   0 robertblom   (501) staff       (20)     1556 2023-05-09 23:16:37.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Inventory.py
--rw-r--r--   0 robertblom   (501) staff       (20)     1610 2023-05-09 23:15:53.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Item.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2081 2023-05-09 23:16:37.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Market.py
--rw-r--r--   0 robertblom   (501) staff       (20)      374 2023-05-09 23:08:16.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Subject.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:02.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.735540 procurement_bytetheory-1.0.2/src/procurement_bytetheory/utils/
--rw-r--r--   0 robertblom   (501) staff       (20)      374 2023-04-27 21:42:06.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/utils/FloatValidator.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:56.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/utils/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.736260 procurement_bytetheory-1.0.2/src/procurement_bytetheory/views/
--rw-r--r--   0 robertblom   (501) staff       (20)     1448 2023-04-28 20:27:35.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/views/CLIProcurementGame.py
--rw-r--r--   0 robertblom   (501) staff       (20)     3057 2023-04-28 18:43:21.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/views/CLIProcurementSimulator.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:50.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory/views/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:20:18.731424 procurement_bytetheory-1.0.2/src/procurement_bytetheory.egg-info/
--rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-09 23:20:18.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory.egg-info/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)     1507 2023-05-09 23:20:18.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory.egg-info/SOURCES.txt
--rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-05-09 23:20:18.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory.egg-info/dependency_links.txt
--rw-r--r--   0 robertblom   (501) staff       (20)       23 2023-05-09 23:20:18.000000 procurement_bytetheory-1.0.2/src/procurement_bytetheory.egg-info/top_level.txt
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.478784 procurement_bytetheory-1.0.3/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-04-27 14:56:54.000000 procurement_bytetheory-1.0.3/LICENSE
+-rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-09 23:46:51.479019 procurement_bytetheory-1.0.3/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 17:35:18.000000 procurement_bytetheory-1.0.3/README.md
+-rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-04-27 14:58:37.000000 procurement_bytetheory-1.0.3/pyproject.toml
+-rw-r--r--   0 robertblom   (501) staff       (20)      543 2023-05-09 23:46:51.479624 procurement_bytetheory-1.0.3/setup.cfg
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.467127 procurement_bytetheory-1.0.3/src/
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.468292 procurement_bytetheory-1.0.3/src/procurement_bytetheory/
+-rw-r--r--   0 robertblom   (501) staff       (20)      295 2023-05-02 16:19:26.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.470839 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/
+-rw-r--r--   0 robertblom   (501) staff       (20)      611 2023-04-28 20:46:41.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/CLIController.py
+-rw-r--r--   0 robertblom   (501) staff       (20)       63 2023-05-02 14:53:25.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/Observer.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     1877 2023-05-09 23:44:08.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/UIController.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:35.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.471433 procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/
+-rw-r--r--   0 robertblom   (501) staff       (20)    86016 2023-05-09 23:46:47.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/ProcurementGame.db
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 15:08:49.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/__init__.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      397 2023-05-02 20:07:41.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/items.csv
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.473059 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/
+-rw-r--r--   0 robertblom   (501) staff       (20)     2440 2023-05-03 14:15:31.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     3510 2023-05-03 14:20:12.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/DatabaseHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2524 2023-05-03 19:02:03.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2387 2023-05-03 16:58:38.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/ItemDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2429 2023-05-03 19:02:11.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/MarketDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:07.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.473930 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/
+-rw-r--r--   0 robertblom   (501) staff       (20)     4485 2023-05-09 23:43:15.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Business.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     1590 2023-05-09 23:42:24.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Inventory.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     1610 2023-05-09 23:15:53.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Item.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2115 2023-05-09 23:41:33.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Market.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      371 2023-05-09 23:39:38.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Subject.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:02.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.476014 procurement_bytetheory-1.0.3/src/procurement_bytetheory/utils/
+-rw-r--r--   0 robertblom   (501) staff       (20)      374 2023-04-27 21:42:06.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/utils/FloatValidator.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:56.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/utils/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.478304 procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1448 2023-04-28 20:27:35.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/CLIProcurementGame.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     3057 2023-04-28 18:43:21.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/CLIProcurementSimulator.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:50.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.468882 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/
+-rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-09 23:46:51.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)     1507 2023-05-09 23:46:51.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-05-09 23:46:51.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)       23 2023-05-09 23:46:51.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/top_level.txt
```

### Comparing `procurement_bytetheory-1.0.2/LICENSE` & `procurement_bytetheory-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/setup.cfg` & `procurement_bytetheory-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = procurement_bytetheory
-version = 1.0.2
+version = 1.0.3
 author = Robbie Blom
 description = Provides helpers to procurement app.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/controllers/CLIController.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/CLIController.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/controllers/UIController.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/UIController.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/data/ProcurementGame.db` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/ProcurementGame.db`

 * *Format-specific differences are supported for SQLite databases but no file-specific differences were detected; falling back to a binary diff. file(1) reports: SQLite 3.x database, last written using SQLite version 3037000, file counter 7170, database pages 21, 1st free page 11, free pages 4, cookie 0xd0, schema 4, UTF-8, version-valid-for 7170*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5351 4c69 7465 2066 6f72 6d61 7420 3300  SQLite format 3.
-00000010: 1000 0101 0040 2020 0000 1c02 0000 0015  .....@  ........
-00000020: 0000 000b 0000 0004 0000 00d0 0000 0004  ................
+00000010: 1000 0101 0040 2020 0000 1d0e 0000 0015  .....@  ........
+00000020: 0000 000b 0000 0004 0000 0120 0000 0004  ........... ....
 00000030: 0000 0000 0000 0000 0000 0001 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0000 0000 0000 0000 0000 1c02  ................
+00000050: 0000 0000 0000 0000 0000 0000 0000 1d0e  ................
 00000060: 002e 5748 0d0f f800 100a 0000 0f1d 0fc7  ..WH............
 00000070: 0e29 0ee2 0d99 0dfc 0cf0 0d62 0c30 0cc7  .).........b.0..
 00000080: 0b57 0bfd 0ab8 0b24 0a00 0a7b 0979 0979  .W.....$...{.y.y
 00000090: 0979 0979 0000 0000 0000 0000 0000 0000  .y.y............
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/DatabaseHandler.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/DatabaseHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/ItemDbHandler.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/ItemDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/db_connectors/MarketDbHandler.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/MarketDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Business.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Business.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,25 @@
         self.inventory = inventory if inventory else Inventory("ACME Innovations Inventory")
         self.market = market if market else Market("USA")
         self.dbHandler = dbHandler if dbHandler else BusinessDbHandler()
 
     def save(self):
         self.dbHandler.saveBusiness(self)
     
-    def serializeToJson(self):
-        dictionaryRepresentation = {
+    def getDictionaryRepresentation(self):
+        return {
             "id": self.id,
             "name": self.name,
             "moneyAmount": self.money_amount,
-            "inventory": self.inventory.serializeToJson(),
-            "market": self.market.serializeToJson()
+            "inventory": self.inventory.getDictionaryRepresentation(),
+            "market": self.market.getDictionaryRepresentation()
         }
-        return json.dumps(dictionaryRepresentation)
+
+    def serializeToJson(self):
+        return json.dumps(self.getDictionaryRepresentation())
 
     def buyCheapest(self, itemName=None):
         """Buys the cheapest item with the specified itemName, and if no itemName is specified,
         buys one of the cheapest items in the market.
         """
         buyingCheapestOfSpecificItem = bool(itemName)
         if buyingCheapestOfSpecificItem:
```

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Inventory.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Inventory.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 
         self.items = items if items else []  # [item1, item2, ...]
         self.dbHandler = dbHandler if dbHandler else InventoryDbHandler()
 
     def save(self):
         self.dbHandler.saveInventory(self)
 
-    def serializeToJson(self):
-        dictionaryRepresentation = {
+    def getDictionaryRepresentation(self):
+        return {
             "id": self.id,
             "name": self.name,
             "items": [item.getDictionaryRepresentation() for item in self.items]
         }
-        return json.dumps(dictionaryRepresentation)
+
+    def serializeToJson(self):
+        return json.dumps(self.getDictionaryRepresentation())
 
     def addItem(self, item):
         self.items.append(item)
         item.setInventory(self)
 
     def removeItem(self, item):
         self.items.remove(item)
```

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Item.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Item.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/model/Market.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Market.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 
         self.items = items if items else [] # [item1, item2, ...]
         self.dbHandler = dbHandler if dbHandler else MarketDbHandler()
 
     def save(self):
         self.dbHandler.saveMarket(self)
 
-    def serializeToJson(self):
-        dictionaryRepresentation = {
+    def getDictionaryRepresentation(self):
+        return {
             "id": self.id,
             "name": self.name,
             "items": [item.getDictionaryRepresentation() for item in self.items]
         }
-        return json.dumps(dictionaryRepresentation)
+
+    def serializeToJson(self):
+        return json.dumps(self.getDictionaryRepresentation())
 
     def seedMarket(self):
         seedItems = self.getSeedItems()
         self.addItemsToMarket(seedItems)
 
     def getSeedItems(self):
         csvin = csv.reader(open(Market.seedFile))
```

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/views/CLIProcurementGame.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/CLIProcurementGame.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory/views/CLIProcurementSimulator.py` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/CLIProcurementSimulator.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.2/src/procurement_bytetheory.egg-info/SOURCES.txt` & `procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

