# Comparing `tmp/procurement_bytetheory-1.0.3.tar.gz` & `tmp/procurement_bytetheory-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procurement_bytetheory-1.0.3.tar", last modified: Tue May  9 23:46:51 2023, max compression
+gzip compressed data, was "procurement_bytetheory-1.0.4.tar", last modified: Wed May 10 17:19:03 2023, max compression
```

## Comparing `procurement_bytetheory-1.0.3.tar` & `procurement_bytetheory-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.478784 procurement_bytetheory-1.0.3/
--rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-04-27 14:56:54.000000 procurement_bytetheory-1.0.3/LICENSE
--rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-09 23:46:51.479019 procurement_bytetheory-1.0.3/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 17:35:18.000000 procurement_bytetheory-1.0.3/README.md
--rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-04-27 14:58:37.000000 procurement_bytetheory-1.0.3/pyproject.toml
--rw-r--r--   0 robertblom   (501) staff       (20)      543 2023-05-09 23:46:51.479624 procurement_bytetheory-1.0.3/setup.cfg
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.467127 procurement_bytetheory-1.0.3/src/
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.468292 procurement_bytetheory-1.0.3/src/procurement_bytetheory/
--rw-r--r--   0 robertblom   (501) staff       (20)      295 2023-05-02 16:19:26.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.470839 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/
--rw-r--r--   0 robertblom   (501) staff       (20)      611 2023-04-28 20:46:41.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/CLIController.py
--rw-r--r--   0 robertblom   (501) staff       (20)       63 2023-05-02 14:53:25.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/Observer.py
--rw-r--r--   0 robertblom   (501) staff       (20)     1877 2023-05-09 23:44:08.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/UIController.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:35.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.471433 procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/
--rw-r--r--   0 robertblom   (501) staff       (20)    86016 2023-05-09 23:46:47.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/ProcurementGame.db
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 15:08:49.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/__init__.py
--rw-r--r--   0 robertblom   (501) staff       (20)      397 2023-05-02 20:07:41.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/items.csv
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.473059 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/
--rw-r--r--   0 robertblom   (501) staff       (20)     2440 2023-05-03 14:15:31.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     3510 2023-05-03 14:20:12.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/DatabaseHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2524 2023-05-03 19:02:03.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2387 2023-05-03 16:58:38.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/ItemDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2429 2023-05-03 19:02:11.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/MarketDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:07.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.473930 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/
--rw-r--r--   0 robertblom   (501) staff       (20)     4485 2023-05-09 23:43:15.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Business.py
--rw-r--r--   0 robertblom   (501) staff       (20)     1590 2023-05-09 23:42:24.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Inventory.py
--rw-r--r--   0 robertblom   (501) staff       (20)     1610 2023-05-09 23:15:53.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Item.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2115 2023-05-09 23:41:33.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Market.py
--rw-r--r--   0 robertblom   (501) staff       (20)      371 2023-05-09 23:39:38.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Subject.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:02.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.476014 procurement_bytetheory-1.0.3/src/procurement_bytetheory/utils/
--rw-r--r--   0 robertblom   (501) staff       (20)      374 2023-04-27 21:42:06.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/utils/FloatValidator.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:56.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/utils/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.478304 procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/
--rw-r--r--   0 robertblom   (501) staff       (20)     1448 2023-04-28 20:27:35.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/CLIProcurementGame.py
--rw-r--r--   0 robertblom   (501) staff       (20)     3057 2023-04-28 18:43:21.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/CLIProcurementSimulator.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:50.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-09 23:46:51.468882 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/
--rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-09 23:46:51.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)     1507 2023-05-09 23:46:51.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/SOURCES.txt
--rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-05-09 23:46:51.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/dependency_links.txt
--rw-r--r--   0 robertblom   (501) staff       (20)       23 2023-05-09 23:46:51.000000 procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/top_level.txt
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.494657 procurement_bytetheory-1.0.4/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-04-27 14:56:54.000000 procurement_bytetheory-1.0.4/LICENSE
+-rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-10 17:19:03.494738 procurement_bytetheory-1.0.4/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 17:35:18.000000 procurement_bytetheory-1.0.4/README.md
+-rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-04-27 14:58:37.000000 procurement_bytetheory-1.0.4/pyproject.toml
+-rw-r--r--   0 robertblom   (501) staff       (20)      543 2023-05-10 17:19:03.495029 procurement_bytetheory-1.0.4/setup.cfg
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.488859 procurement_bytetheory-1.0.4/src/
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.489867 procurement_bytetheory-1.0.4/src/procurement_bytetheory/
+-rw-r--r--   0 robertblom   (501) staff       (20)      295 2023-05-02 16:19:26.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.490850 procurement_bytetheory-1.0.4/src/procurement_bytetheory/controllers/
+-rw-r--r--   0 robertblom   (501) staff       (20)      611 2023-04-28 20:46:41.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/controllers/CLIController.py
+-rw-r--r--   0 robertblom   (501) staff       (20)       63 2023-05-02 14:53:25.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/controllers/Observer.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2142 2023-05-10 15:28:29.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/controllers/UIController.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:35.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/controllers/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.491242 procurement_bytetheory-1.0.4/src/procurement_bytetheory/data/
+-rw-r--r--   0 robertblom   (501) staff       (20)    86016 2023-05-10 17:19:00.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/data/ProcurementGame.db
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 15:08:49.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/data/__init__.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      397 2023-05-02 20:07:41.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/data/items.csv
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.492379 procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/
+-rw-r--r--   0 robertblom   (501) staff       (20)     2438 2023-05-10 16:05:26.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     3721 2023-05-10 15:24:35.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/DatabaseHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2524 2023-05-03 19:02:03.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2934 2023-05-10 17:06:27.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/ItemDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2429 2023-05-03 19:02:11.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/MarketDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:07.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.493146 procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/
+-rw-r--r--   0 robertblom   (501) staff       (20)     4476 2023-05-10 16:05:26.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Business.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     1593 2023-05-10 12:34:19.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Inventory.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2249 2023-05-10 13:06:56.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Item.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2114 2023-05-10 15:36:21.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Market.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      371 2023-05-09 23:39:38.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Subject.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:02.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.493372 procurement_bytetheory-1.0.4/src/procurement_bytetheory/utils/
+-rw-r--r--   0 robertblom   (501) staff       (20)      374 2023-04-27 21:42:06.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/utils/FloatValidator.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:56.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/utils/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.493709 procurement_bytetheory-1.0.4/src/procurement_bytetheory/views/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1448 2023-04-28 20:27:35.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/views/CLIProcurementGame.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     3057 2023-04-28 18:43:21.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/views/CLIProcurementSimulator.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:50.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory/views/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.490339 procurement_bytetheory-1.0.4/src/procurement_bytetheory.egg-info/
+-rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-10 17:19:03.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory.egg-info/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)     1553 2023-05-10 17:19:03.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-05-10 17:19:03.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)       23 2023-05-10 17:19:03.000000 procurement_bytetheory-1.0.4/src/procurement_bytetheory.egg-info/top_level.txt
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 17:19:03.494311 procurement_bytetheory-1.0.4/tests/
+-rw-r--r--   0 robertblom   (501) staff       (20)      307 2023-05-10 17:14:41.000000 procurement_bytetheory-1.0.4/tests/test_Item.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     1317 2023-05-10 17:11:57.000000 procurement_bytetheory-1.0.4/tests/test_UIController.py
```

### Comparing `procurement_bytetheory-1.0.3/LICENSE` & `procurement_bytetheory-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.3/setup.cfg` & `procurement_bytetheory-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = procurement_bytetheory
-version = 1.0.3
+version = 1.0.4
 author = Robbie Blom
 description = Provides helpers to procurement app.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/CLIController.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/controllers/CLIController.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/controllers/UIController.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/controllers/UIController.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from procurement_bytetheory.controllers.Observer import Observer
 from procurement_bytetheory.model.Business import Business
-
+from procurement_bytetheory.model.Item import Item
 class UIController(Observer):
     def __init__(self):
         super().__init__()
         self.view = None
         self.business = None
 
     def setView(self, view):
@@ -24,14 +24,20 @@
         self.setBusiness(newBusiness)
 
     def seedMarket(self):
         self.business.market.seedMarket()
         self.business.market.save()
         self.business.notifyObservers("Market seeded", self.business.serializeToJson())
 
+    def buyItemById(self, id):
+        item = Item.getItemById(id)
+        self.business.buy(item)
+        self.business.save()
+        self.business.notifyObservers("Item bought", self.business.serializeToJson())
+
     def buyCheapest(self, itemName=None):
         self.business.buyCheapest(itemName)
         self.business.save()
         self.business.notifyObservers("Cheapest item bought", self.business.serializeToJson())
 
     def buyAsManyAsPossible(self, itemName=None):
         self.business.buyAsManyAsPossible(itemName)
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/data/ProcurementGame.db` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/data/ProcurementGame.db`

 * *Format-specific differences are supported for SQLite databases but no file-specific differences were detected; falling back to a binary diff. file(1) reports: SQLite 3.x database, last written using SQLite version 3037000, file counter 7438, database pages 21, 1st free page 11, free pages 4, cookie 0x120, schema 4, UTF-8, version-valid-for 7438*

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5351 4c69 7465 2066 6f72 6d61 7420 3300  SQLite format 3.
-00000010: 1000 0101 0040 2020 0000 1d0e 0000 0015  .....@  ........
-00000020: 0000 000b 0000 0004 0000 0120 0000 0004  ........... ....
+00000010: 1000 0101 0040 2020 0000 46c1 0000 0015  .....@  ..F.....
+00000020: 0000 000b 0000 0004 0000 01d0 0000 0004  ................
 00000030: 0000 0000 0000 0000 0000 0001 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0000 0000 0000 0000 0000 1d0e  ................
+00000050: 0000 0000 0000 0000 0000 0000 0000 46c1  ..............F.
 00000060: 002e 5748 0d0f f800 100a 0000 0f1d 0fc7  ..WH............
 00000070: 0e29 0ee2 0d99 0dfc 0cf0 0d62 0c30 0cc7  .).........b.0..
 00000080: 0b57 0bfd 0ab8 0b24 0a00 0a7b 0979 0979  .W.....$...{.y.y
 00000090: 0979 0979 0000 0000 0000 0000 0000 0000  .y.y............
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from procurement_bytetheory.db_connectors.DatabaseHandler import DatabaseHandler
 from procurement_bytetheory.db_connectors.MarketDbHandler import MarketDbHandler
 from procurement_bytetheory.db_connectors.InventoryDbHandler import InventoryDbHandler
-
 class BusinessDbHandler(DatabaseHandler):
 
     def __init__(self):
         super().__init__()
         self.marketDbHandler = MarketDbHandler()
         self.inventoryDbHandler = InventoryDbHandler()
 
@@ -18,26 +17,26 @@
         curs = self.db.cursor()
         try:
             print('Attempting to insert a new Business...')
             curs.execute(
                 """
                 INSERT INTO Business
                 VALUES ({id}, '{name}', {money_amount}, {marketId}, {inventoryId});
-                """.format(id=business.id, name=business.name, money_amount=business.money_amount, marketId=business.market.id if business.market else -1, inventoryId=business.inventory.id if business.inventory else -1)
+                """.format(id=business.id, name=business.name, money_amount=business.moneyAmount, marketId=business.market.id if business.market else -1, inventoryId=business.inventory.id if business.inventory else -1)
             )
             print('New business inserted.')
         except Exception as e:
             print(e)
             print('Record already exists.  Updating a Business...')
             curs.execute(
                 """
                 UPDATE Business
                 SET id={id}, name='{name}', money_amount={money_amount}, market_id={marketId}, inventory_id={inventoryId}
                 WHERE id={id};
-                """.format(id=business.id, name=business.name, money_amount=business.money_amount, marketId=business.market.id, inventoryId=business.inventory.id)
+                """.format(id=business.id, name=business.name, money_amount=business.moneyAmount, marketId=business.market.id, inventoryId=business.inventory.id)
             )
             print('Business updated')
         self.db.commit()
         curs.close()
 
     def getBusinessById(self, id):
         curs = self.db.cursor()
@@ -52,8 +51,8 @@
                 )
             )
             dbResponse = curs.fetchall()
             curs.close()
             return self.deserializer.deserializeBusiness(dbResponse[0])
         except Exception as e:
             print(e)
-            raise Exception("No business with id {} exists", id)
+            raise Exception("No business with id {} exists", id)
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/DatabaseHandler.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/DatabaseHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,21 @@
         self.db = sqlite3.connect(dbFile)
 
     @classmethod
     def truncateTables(cls):
         db = sqlite3.connect(cls.dbFile)
         curs = db.cursor()
         curs.execute("""DELETE FROM Business""")
+        curs.execute("""DELETE FROM Temp_Business""")
         curs.execute("""DELETE FROM Market""")
+        curs.execute("""DELETE FROM Temp_Market""")
         curs.execute("""DELETE FROM Inventory""")
+        curs.execute("""DELETE FROM Temp_Inventory""")
         curs.execute("""DELETE FROM Item""")
+        curs.execute("""DELETE FROM Temp_Item""")
         db.commit()
         curs.close()
         db.close()
 
     @classmethod
     def get_all_items(cls, item_name=None):
         db = sqlite3.connect("../data/ProcurementGame.db")
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/ItemDbHandler.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/ItemDbHandler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from procurement_bytetheory.db_connectors.DatabaseHandler import DatabaseHandler
-
 class ItemDbHandler(DatabaseHandler):
 
     def __init__(self):
         super().__init__()
 
     def saveItem(self, item):
         # Note: temp table not needed because we're just upserting
@@ -23,43 +22,61 @@
 
         for item in items:
             print('Inserting a new Item into temp table...')
             curs.execute(
                 """
                 INSERT INTO Temp_Item
                 VALUES ({id}, '{name}', {value}, {marketId}, {inventoryId})
-                """.format(id=item.id, name=item.name, value=item.value, marketId=item.market.id if item.market else -1, inventoryId=item.inventory.id if item.inventory else -1)
+                """.format(id=item.id, name=item.name, value=item.value, marketId=item.marketId if item.marketId else -1, inventoryId=item.inventoryId if item.inventoryId else -1)
             )
             print('New item inserted into temp table.')
         
         self.db.commit()
         curs.close()
 
     def upsertItem(self, item):
         curs = self.db.cursor()
         try:
             print('Attempting to insert a new Item...')
             curs.execute(
                 """
                 INSERT INTO Item
                 VALUES ({id}, '{name}', {value}, {marketId}, {inventoryId})
-                """.format(id=item.id, name=item.name, value=item.value, marketId=item.market.id if item.market else -1, inventoryId=item.inventory.id if item.inventory else -1)
+                """.format(id=item.id, name=item.name, value=item.value, marketId=item.marketId if item.marketId else -1, inventoryId=item.inventoryId if item.inventoryId else -1)
             )
             print('New item inserted.')
         except Exception as e:
             print(e)
             print('Record already exists.  Updating an Item...')
             curs.execute(
                 """
                 UPDATE Item
                 SET id={id}, name='{name}', value={value}, market_id={marketId}, inventory_id={inventoryId}
                 WHERE id={id};
-                """.format(id=item.id, name=item.name, value=item.value, marketId=item.market.id if item.market else -1, inventoryId=item.inventory.id if item.inventory else -1)
+                """.format(id=item.id, name=item.name, value=item.value, marketId=item.marketId if item.marketId else -1, inventoryId=item.inventoryId if item.inventoryId else -1)
             )
             print('Item updated')
         self.db.commit()
         curs.close()
 
     def upsertItems(self, items):
         for item in items:
             self.upsertItem(item)
-    
+    
+    def getItemById(self, id):
+        curs = self.db.cursor()
+        try:
+            curs.execute(
+                """
+                SELECT id, name, value, market_id, inventory_id
+                FROM Item
+                WHERE id = {}
+                """.format(
+                    id
+                )
+            )
+            dbResponse = curs.fetchall()
+            curs.close()
+            return dbResponse[0]
+        except Exception as e:
+            print(e)
+            raise Exception("No business with id {} exists", id)
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/db_connectors/MarketDbHandler.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/db_connectors/MarketDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Business.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Business.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from procurement_bytetheory.model.Subject import Subject
 from procurement_bytetheory.model.Inventory import Inventory
 import json
 
 class Business(Subject):
     numBusinesses = 0
 
-    def __init__(self, name, money_amount=400, id=None, inventory=None, market=None, dbHandler=None):
+    def __init__(self, name, moneyAmount=400, id=None, inventory=None, market=None, dbHandler=None):
         super().__init__()
 
         self.name = name
-        self.money_amount = money_amount
+        self.moneyAmount = moneyAmount
 
         self.id = id if id else Business.numBusinesses + 1
         Business.numBusinesses += 1
 
         self.inventory = inventory if inventory else Inventory("ACME Innovations Inventory")
         self.market = market if market else Market("USA")
         self.dbHandler = dbHandler if dbHandler else BusinessDbHandler()
@@ -23,15 +23,15 @@
     def save(self):
         self.dbHandler.saveBusiness(self)
     
     def getDictionaryRepresentation(self):
         return {
             "id": self.id,
             "name": self.name,
-            "moneyAmount": self.money_amount,
+            "moneyAmount": self.moneyAmount,
             "inventory": self.inventory.getDictionaryRepresentation(),
             "market": self.market.getDictionaryRepresentation()
         }
 
     def serializeToJson(self):
         return json.dumps(self.getDictionaryRepresentation())
 
@@ -60,21 +60,21 @@
                 self.buy(cheapestOfGivenItem)
                 self.buyAsManyAsPossible(cheapestOfGivenItem.name)
         else:
             itemToBuy = self.market.getCheapestItemInMarket()
             self.buyAsManyAsPossible(itemToBuy.name)
 
     def payPriceOfItem(self, price):
-        self.money_amount = self.money_amount - price
+        self.moneyAmount = self.moneyAmount - price
 
     def addItemToInventory(self, item):
         self.inventory.addItem(item)
 
     def canAfford(self, item):
-        if self.money_amount > item.getPurchasePrice():
+        if self.moneyAmount > item.getPurchasePrice():
             return True
         return False
 
     def buy(self, item):
         if self.canAfford(item):
             self.market.removeItemFromMarket(item)
             self.payPriceOfItem(item.getPurchasePrice())
@@ -98,21 +98,21 @@
 
     def liquidateInventory(self):
         for item in self.inventory.items:
             self.collectPaymentFromMarketCustomer(item.getFireSalePrice())
         self.clearInventory()
 
     def collectPaymentFromMarketCustomer(self, salesPrice):
-        self.money_amount += salesPrice
+        self.moneyAmount += salesPrice
 
     def removeItemFromInventory(self, item):
         self.inventory.removeItem(item)
 
     def clearInventory(self):
         self.inventory.clear()
 
     def executeSale(self, item):
         self.collectPaymentFromMarketCustomer(item.getSalesPrice())
         self.removeItemFromInventory(item)
 
     def getNetWorth(self):
-        return self.money_amount + self.inventory.getValue()
+        return self.moneyAmount + self.inventory.getValue()
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Inventory.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         }
 
     def serializeToJson(self):
         return json.dumps(self.getDictionaryRepresentation())
 
     def addItem(self, item):
         self.items.append(item)
-        item.setInventory(self)
+        item.setInventory(self.id)
 
     def removeItem(self, item):
         self.items.remove(item)
         item.setInventory(None)
 
     def clear(self):
         for item in self.items:
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Item.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Item.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,62 @@
 from procurement_bytetheory.db_connectors.ItemDbHandler import ItemDbHandler
 import json
 
 class Item:
     itemCount = 0
 
-    def __init__(self, name, value, id=None, market=None, inventory=None, dbHandler=None):
+    def __init__(self, name, value, id=None, marketId=None, inventoryId=None, dbHandler=None):
         self.name = name
         self.value = value
 
         self.id = id if id else Item.itemCount + 1
         Item.itemCount += 1
         
-        self.market = market
-        self.inventory = inventory
+        self.marketId = marketId
+        self.inventoryId = inventoryId
         self.dbHandler = dbHandler if dbHandler else ItemDbHandler()
 
     def save(self):
         self.dbHandler.saveItem(self)
 
-    def getDictionaryRepresentation(self):
-        return {
-            "id": self.id,
-            "name": self.name,
-            "value": self.value,
-            "marketId": self.market.id,
-        }
+    @staticmethod
+    def getItemById(id):
+        dbHandler = ItemDbHandler()
+        dbRecord = dbHandler.getItemById(id)
+        return Item.deserializeToObject(dbRecord)
+
+    @staticmethod
+    def deserializeToObject(dbRecord):
+        (id, name, value, market_id, inventory_id) = dbRecord
+        return Item(name, value, id=id, marketId=market_id, inventoryId=inventory_id)
 
+    def getDictionaryRepresentation(self):
+        try :
+            return {
+                "id": self.id,
+                "name": self.name,
+                "value": self.value,
+                "marketId": self.marketId,
+            }
+        except: 
+            return {
+                "id": self.id,
+                "name": self.name,
+                "value": self.value,
+                "marketId": None,
+            }
+        
     def serializeToJson(self):
         return json.dumps(self.getDictionaryRepresentation())
 
-    def setMarket(self, market):
-        self.market = market
+    def setMarket(self, marketId):
+        self.marketId = marketId
 
-    def setInventory(self, inventory):
-        self.inventory = inventory
+    def setInventory(self, inventoryId):
+        self.inventoryId = inventoryId
 
     def getPurchasePrice(self):
         return .95*self.value
 
     def getSalesPrice(self):
         return 1.05*self.value
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/model/Market.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/model/Market.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,18 +43,18 @@
             newItem = Item(name, value)
             seedItems.append(newItem)
         return seedItems
 
     def addItemsToMarket(self, items):
         for item in items:
             self.addItemToMarket(item)
-    
+
     def addItemToMarket(self, item):
         self.items.append(item)
-        item.setMarket(self)
+        item.setMarket(self.id)
 
     def removeItemFromMarket(self, item):
         self.items.remove(item)
         item.setMarket(None)
 
     def hasItem(self, itemName):
         return itemName in [item.name for item in self.items]
```

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/CLIProcurementGame.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/views/CLIProcurementGame.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory/views/CLIProcurementSimulator.py` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory/views/CLIProcurementSimulator.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.3/src/procurement_bytetheory.egg-info/SOURCES.txt` & `procurement_bytetheory-1.0.4/src/procurement_bytetheory.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -26,8 +26,10 @@
 src/procurement_bytetheory/model/Market.py
 src/procurement_bytetheory/model/Subject.py
 src/procurement_bytetheory/model/__init__.py
 src/procurement_bytetheory/utils/FloatValidator.py
 src/procurement_bytetheory/utils/__init__.py
 src/procurement_bytetheory/views/CLIProcurementGame.py
 src/procurement_bytetheory/views/CLIProcurementSimulator.py
-src/procurement_bytetheory/views/__init__.py
+src/procurement_bytetheory/views/__init__.py
+tests/test_Item.py
+tests/test_UIController.py
```

