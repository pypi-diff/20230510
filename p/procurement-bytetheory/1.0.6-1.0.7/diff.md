# Comparing `tmp/procurement_bytetheory-1.0.6.tar.gz` & `tmp/procurement_bytetheory-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procurement_bytetheory-1.0.6.tar", last modified: Wed May 10 19:01:11 2023, max compression
+gzip compressed data, was "procurement_bytetheory-1.0.7.tar", last modified: Wed May 10 20:25:19 2023, max compression
```

## Comparing `procurement_bytetheory-1.0.6.tar` & `procurement_bytetheory-1.0.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.544686 procurement_bytetheory-1.0.6/
--rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-04-27 14:56:54.000000 procurement_bytetheory-1.0.6/LICENSE
--rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-10 19:01:11.544752 procurement_bytetheory-1.0.6/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 17:35:18.000000 procurement_bytetheory-1.0.6/README.md
--rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-04-27 14:58:37.000000 procurement_bytetheory-1.0.6/pyproject.toml
--rw-r--r--   0 robertblom   (501) staff       (20)      543 2023-05-10 19:01:11.545018 procurement_bytetheory-1.0.6/setup.cfg
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.539065 procurement_bytetheory-1.0.6/src/
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.540106 procurement_bytetheory-1.0.6/src/procurement_bytetheory/
--rw-r--r--   0 robertblom   (501) staff       (20)      295 2023-05-02 16:19:26.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.541624 procurement_bytetheory-1.0.6/src/procurement_bytetheory/controllers/
--rw-r--r--   0 robertblom   (501) staff       (20)      611 2023-04-28 20:46:41.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/controllers/CLIController.py
--rw-r--r--   0 robertblom   (501) staff       (20)       63 2023-05-02 14:53:25.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/controllers/Observer.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2364 2023-05-10 18:17:50.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/controllers/UIController.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:35.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/controllers/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.541998 procurement_bytetheory-1.0.6/src/procurement_bytetheory/data/
--rw-r--r--   0 robertblom   (501) staff       (20)    86016 2023-05-10 19:01:08.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/data/ProcurementGame.db
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 15:08:49.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/data/__init__.py
--rw-r--r--   0 robertblom   (501) staff       (20)      397 2023-05-02 20:07:41.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/data/items.csv
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.542769 procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/
--rw-r--r--   0 robertblom   (501) staff       (20)     2438 2023-05-10 16:05:26.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     3721 2023-05-10 15:24:35.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/DatabaseHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2524 2023-05-03 19:02:03.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2934 2023-05-10 17:06:27.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/ItemDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2429 2023-05-03 19:02:11.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/MarketDbHandler.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:07.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.543530 procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/
--rw-r--r--   0 robertblom   (501) staff       (20)     4476 2023-05-10 18:55:11.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/Business.py
--rw-r--r--   0 robertblom   (501) staff       (20)     1603 2023-05-10 18:55:27.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/Inventory.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2249 2023-05-10 13:06:56.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/Item.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2114 2023-05-10 15:36:21.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/Market.py
--rw-r--r--   0 robertblom   (501) staff       (20)      371 2023-05-09 23:39:38.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/Subject.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:02.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.543774 procurement_bytetheory-1.0.6/src/procurement_bytetheory/utils/
--rw-r--r--   0 robertblom   (501) staff       (20)      374 2023-04-27 21:42:06.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/utils/FloatValidator.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:56.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/utils/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.544147 procurement_bytetheory-1.0.6/src/procurement_bytetheory/views/
--rw-r--r--   0 robertblom   (501) staff       (20)     1448 2023-04-28 20:27:35.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/views/CLIProcurementGame.py
--rw-r--r--   0 robertblom   (501) staff       (20)     3057 2023-04-28 18:43:21.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/views/CLIProcurementSimulator.py
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:50.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory/views/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.540625 procurement_bytetheory-1.0.6/src/procurement_bytetheory.egg-info/
--rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-10 19:01:11.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory.egg-info/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)     1553 2023-05-10 19:01:11.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory.egg-info/SOURCES.txt
--rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-05-10 19:01:11.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory.egg-info/dependency_links.txt
--rw-r--r--   0 robertblom   (501) staff       (20)       23 2023-05-10 19:01:11.000000 procurement_bytetheory-1.0.6/src/procurement_bytetheory.egg-info/top_level.txt
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 19:01:11.544562 procurement_bytetheory-1.0.6/tests/
--rw-r--r--   0 robertblom   (501) staff       (20)      307 2023-05-10 17:14:41.000000 procurement_bytetheory-1.0.6/tests/test_Item.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2667 2023-05-10 18:59:15.000000 procurement_bytetheory-1.0.6/tests/test_UIController.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.055567 procurement_bytetheory-1.0.7/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-04-27 14:56:54.000000 procurement_bytetheory-1.0.7/LICENSE
+-rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-10 20:25:19.055658 procurement_bytetheory-1.0.7/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 17:35:18.000000 procurement_bytetheory-1.0.7/README.md
+-rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-04-27 14:58:37.000000 procurement_bytetheory-1.0.7/pyproject.toml
+-rw-r--r--   0 robertblom   (501) staff       (20)      543 2023-05-10 20:25:19.056111 procurement_bytetheory-1.0.7/setup.cfg
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.049655 procurement_bytetheory-1.0.7/src/
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.050703 procurement_bytetheory-1.0.7/src/procurement_bytetheory/
+-rw-r--r--   0 robertblom   (501) staff       (20)      295 2023-05-02 16:19:26.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.051955 procurement_bytetheory-1.0.7/src/procurement_bytetheory/controllers/
+-rw-r--r--   0 robertblom   (501) staff       (20)      611 2023-04-28 20:46:41.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/controllers/CLIController.py
+-rw-r--r--   0 robertblom   (501) staff       (20)       63 2023-05-02 14:53:25.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/controllers/Observer.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2364 2023-05-10 18:17:50.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/controllers/UIController.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:35.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/controllers/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.052402 procurement_bytetheory-1.0.7/src/procurement_bytetheory/data/
+-rw-r--r--   0 robertblom   (501) staff       (20)    86016 2023-05-10 20:25:16.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/data/ProcurementGame.db
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 15:08:49.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/data/__init__.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      397 2023-05-02 20:07:41.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/data/items.csv
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.053354 procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/
+-rw-r--r--   0 robertblom   (501) staff       (20)     2438 2023-05-10 16:05:26.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     3721 2023-05-10 15:24:35.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/DatabaseHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2524 2023-05-03 19:02:03.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2934 2023-05-10 17:06:27.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/ItemDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2429 2023-05-03 19:02:11.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/MarketDbHandler.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:07.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.054274 procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/
+-rw-r--r--   0 robertblom   (501) staff       (20)     5870 2023-05-10 20:21:21.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/Business.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     1603 2023-05-10 18:55:27.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/Inventory.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2249 2023-05-10 13:06:56.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/Item.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2114 2023-05-10 15:36:21.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/Market.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      371 2023-05-09 23:39:38.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/Subject.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:45:02.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.054502 procurement_bytetheory-1.0.7/src/procurement_bytetheory/utils/
+-rw-r--r--   0 robertblom   (501) staff       (20)      374 2023-04-27 21:42:06.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/utils/FloatValidator.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:56.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/utils/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.054888 procurement_bytetheory-1.0.7/src/procurement_bytetheory/views/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1448 2023-04-28 20:27:35.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/views/CLIProcurementGame.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     3057 2023-04-28 18:43:21.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/views/CLIProcurementSimulator.py
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-27 21:44:50.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory/views/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.051195 procurement_bytetheory-1.0.7/src/procurement_bytetheory.egg-info/
+-rw-r--r--   0 robertblom   (501) staff       (20)      363 2023-05-10 20:25:19.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory.egg-info/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)     1553 2023-05-10 20:25:19.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-05-10 20:25:19.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)       23 2023-05-10 20:25:19.000000 procurement_bytetheory-1.0.7/src/procurement_bytetheory.egg-info/top_level.txt
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-10 20:25:19.055308 procurement_bytetheory-1.0.7/tests/
+-rw-r--r--   0 robertblom   (501) staff       (20)      307 2023-05-10 17:14:41.000000 procurement_bytetheory-1.0.7/tests/test_Item.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2667 2023-05-10 18:59:15.000000 procurement_bytetheory-1.0.7/tests/test_UIController.py
```

### Comparing `procurement_bytetheory-1.0.6/LICENSE` & `procurement_bytetheory-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/setup.cfg` & `procurement_bytetheory-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = procurement_bytetheory
-version = 1.0.6
+version = 1.0.7
 author = Robbie Blom
 description = Provides helpers to procurement app.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/controllers/CLIController.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/controllers/CLIController.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/controllers/UIController.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/controllers/UIController.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/data/ProcurementGame.db` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/data/ProcurementGame.db`

 * *Format-specific differences are supported for SQLite databases but no file-specific differences were detected; falling back to a binary diff. file(1) reports: SQLite 3.x database, last written using SQLite version 3037000, file counter 22466, database pages 21, 1st free page 11, free pages 4, cookie 0x240, schema 4, UTF-8, version-valid-for 22466*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5351 4c69 7465 2066 6f72 6d61 7420 3300  SQLite format 3.
-00000010: 1000 0101 0040 2020 0000 57c2 0000 0015  .....@  ..W.....
-00000020: 0000 000b 0000 0004 0000 0240 0000 0004  ...........@....
+00000010: 1000 0101 0040 2020 0000 5880 0000 0015  .....@  ..X.....
+00000020: 0000 000b 0000 0004 0000 0270 0000 0004  ...........p....
 00000030: 0000 0000 0000 0000 0000 0001 0000 0000  ................
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0000 0000 0000 0000 0000 57c2  ..............W.
+00000050: 0000 0000 0000 0000 0000 0000 0000 5880  ..............X.
 00000060: 002e 5748 0d0f f800 100a 0000 0f1d 0fc7  ..WH............
 00000070: 0e29 0ee2 0d99 0dfc 0cf0 0d62 0c30 0cc7  .).........b.0..
 00000080: 0b57 0bfd 0ab8 0b24 0a00 0a7b 0979 0979  .W.....$...{.y.y
 00000090: 0979 0979 0000 0000 0000 0000 0000 0000  .y.y............
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/BusinessDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/DatabaseHandler.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/DatabaseHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/InventoryDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/ItemDbHandler.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/ItemDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/db_connectors/MarketDbHandler.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/db_connectors/MarketDbHandler.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/Inventory.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/Inventory.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/Item.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/Item.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/model/Market.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/model/Market.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/views/CLIProcurementGame.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/views/CLIProcurementGame.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory/views/CLIProcurementSimulator.py` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory/views/CLIProcurementSimulator.py`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/src/procurement_bytetheory.egg-info/SOURCES.txt` & `procurement_bytetheory-1.0.7/src/procurement_bytetheory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `procurement_bytetheory-1.0.6/tests/test_UIController.py` & `procurement_bytetheory-1.0.7/tests/test_UIController.py`

 * *Files identical despite different names*

