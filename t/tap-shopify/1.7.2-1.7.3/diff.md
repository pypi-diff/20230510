# Comparing `tmp/tap-shopify-1.7.2.tar.gz` & `tmp/tap-shopify-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-shopify-1.7.2.tar", last modified: Wed May  3 15:40:15 2023, max compression
+gzip compressed data, was "tap-shopify-1.7.3.tar", last modified: Wed May 10 10:05:31 2023, max compression
```

## Comparing `tap-shopify-1.7.2.tar` & `tap-shopify-1.7.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-03 15:40:15.454698 tap-shopify-1.7.2/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    32387 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/LICENSE
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       84 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/MANIFEST.in
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      295 2023-05-03 15:40:15.458698 tap-shopify-1.7.2/PKG-INFO
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2548 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/README.md
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       79 2023-05-03 15:40:15.458698 tap-shopify-1.7.2/setup.cfg
--rwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)      840 2023-05-03 15:39:48.000000 tap-shopify-1.7.2/setup.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-03 15:40:15.450698 tap-shopify-1.7.2/tap_shopify/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     8700 2023-05-02 20:25:26.000000 tap-shopify-1.7.2/tap_shopify/__init__.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1321 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/context.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      143 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/exceptions.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-03 15:40:15.454698 tap-shopify-1.7.2/tap_shopify/schemas/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    10539 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/abandoned_checkouts.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      690 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/collects.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1518 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/custom_collections.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       43 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/customers.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    27088 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/definitions.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1147 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/events.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1577 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/inventory_items.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      394 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/inventory_levels.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       43 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/locations.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1160 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/metafields.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    20799 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/order_refunds.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    23571 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/orders.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     6059 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/products.json
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3294 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/schemas/transactions.json
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-03 15:40:15.454698 tap-shopify-1.7.2/tap_shopify/streams/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      513 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/__init__.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      277 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/abandoned_checkouts.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    12469 2023-05-03 15:39:48.000000 tap-shopify-1.7.2/tap_shopify/streams/base.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1873 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/collects.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      283 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/custom_collections.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      241 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/customers.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      575 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/events.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2037 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/inventory_items.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2486 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/inventory_levels.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1381 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/locations.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3810 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/metafields.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2583 2023-05-02 20:25:28.000000 tap-shopify-1.7.2/tap_shopify/streams/order_refunds.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      225 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/orders.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      272 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/products.py
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3513 2023-05-02 17:48:48.000000 tap-shopify-1.7.2/tap_shopify/streams/transactions.py
-drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-05-03 15:40:15.454698 tap-shopify-1.7.2/tap_shopify.egg-info/
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      295 2023-05-03 15:40:15.000000 tap-shopify-1.7.2/tap_shopify.egg-info/PKG-INFO
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1378 2023-05-03 15:40:15.000000 tap-shopify-1.7.2/tap_shopify.egg-info/SOURCES.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        1 2023-05-03 15:40:15.000000 tap-shopify-1.7.2/tap_shopify.egg-info/dependency_links.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       49 2023-05-03 15:40:15.000000 tap-shopify-1.7.2/tap_shopify.egg-info/entry_points.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       89 2023-05-03 15:40:15.000000 tap-shopify-1.7.2/tap_shopify.egg-info/requires.txt
--rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       12 2023-05-03 15:40:15.000000 tap-shopify-1.7.2/tap_shopify.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2548 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      840 2023-05-10 09:42:36.000000 tap-shopify-1.7.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.391802 tap-shopify-1.7.3/tap_shopify/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8700 2023-05-04 18:16:17.000000 tap-shopify-1.7.3/tap_shopify/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1321 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/context.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      143 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/tap_shopify/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10539 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/abandoned_checkouts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/collects.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1518 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/custom_collections.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/customers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27088 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/definitions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1147 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/inventory_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      394 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/inventory_levels.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       43 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/schemas/locations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1160 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/metafields.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20799 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/order_refunds.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23571 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/orders.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6059 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/products.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3294 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/schemas/transactions.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.395802 tap-shopify-1.7.3/tap_shopify/streams/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      513 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/abandoned_checkouts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13353 2023-05-10 09:42:36.000000 tap-shopify-1.7.3/tap_shopify/streams/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1873 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/collects.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      283 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/custom_collections.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/customers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/events.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2037 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/inventory_items.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/inventory_levels.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1381 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/locations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3810 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/streams/metafields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2583 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/streams/order_refunds.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/orders.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      272 2023-01-25 09:00:08.000000 tap-shopify-1.7.3/tap_shopify/streams/products.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-05-04 05:21:45.000000 tap-shopify-1.7.3/tap_shopify/streams/transactions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 10:05:31.391802 tap-shopify-1.7.3/tap_shopify.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1378 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       89 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-05-10 10:05:31.000000 tap-shopify-1.7.3/tap_shopify.egg-info/top_level.txt
```

### Comparing `tap-shopify-1.7.2/LICENSE` & `tap-shopify-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/README.md` & `tap-shopify-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/setup.py` & `tap-shopify-1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-shopify",
-    version="1.7.2",
+    version="1.7.3",
     description="Singer.io tap for extracting Shopify data",
     author="Stitch",
     url="http://github.com/singer-io/tap-shopify",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     python_requires='>=3.5.2',
     py_modules=["tap_shopify"],
     install_requires=[
```

### Comparing `tap-shopify-1.7.2/tap_shopify/__init__.py` & `tap-shopify-1.7.3/tap_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/context.py` & `tap-shopify-1.7.3/tap_shopify/context.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/abandoned_checkouts.json` & `tap-shopify-1.7.3/tap_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/collects.json` & `tap-shopify-1.7.3/tap_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/custom_collections.json` & `tap-shopify-1.7.3/tap_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/definitions.json` & `tap-shopify-1.7.3/tap_shopify/schemas/definitions.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/events.json` & `tap-shopify-1.7.3/tap_shopify/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/inventory_items.json` & `tap-shopify-1.7.3/tap_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/metafields.json` & `tap-shopify-1.7.3/tap_shopify/schemas/metafields.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/order_refunds.json` & `tap-shopify-1.7.3/tap_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/orders.json` & `tap-shopify-1.7.3/tap_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/products.json` & `tap-shopify-1.7.3/tap_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/schemas/transactions.json` & `tap-shopify-1.7.3/tap_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/__init__.py` & `tap-shopify-1.7.3/tap_shopify/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/base.py` & `tap-shopify-1.7.3/tap_shopify/streams/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,14 +179,18 @@
 
     def get_since_id(self):
         return singer.get_bookmark(Context.state,
                                    # name is overridden by some substreams
                                    self.name,
                                    'since_id')
 
+    def get_updated_at_max(self):
+        updated_at_max = Context.state.get('bookmarks', {}).get(self.name, {}).get('updated_at_max')
+        return utils.strptime_with_tz(updated_at_max) if updated_at_max else None
+
     def update_bookmark(self, bookmark_value, bookmark_key=None):
         # NOTE: Bookmarking can never be updated to not get the most
         # recent thing it saw the next time you run, because the querying
         # only allows greater than or equal semantics.
         singer.write_bookmark(
             Context.state,
             # name is overridden by some substreams
@@ -212,14 +216,15 @@
             "updated_at_min": updated_at_min,
             "updated_at_max": updated_at_max,
             "limit": self.results_per_page,
             status_key: "any"
         }
 
     def get_objects(self):
+        last_sync_interrupted_at = self.get_updated_at_max()
         updated_at_min = self.get_bookmark()
         max_bookmark = updated_at_min
 
         stop_time = singer.utils.now().replace(microsecond=0)
         date_window_size = float(Context.config.get("date_window_size", DATE_WINDOW_SIZE))
 
         # Page through till the end of the resultset
@@ -231,15 +236,22 @@
                 LOGGER.info("Resuming sync from since_id %d", since_id)
 
             # It's important that `updated_at_min` has microseconds
             # truncated. Why has been lost to the mists of time but we
             # think it has something to do with how the API treats
             # microseconds on its date windows. Maybe it's possible to
             # drop data due to rounding errors or something like that?
-            updated_at_max = updated_at_min + datetime.timedelta(days=date_window_size)
+            # If last sync was interrupted, set updated_at_max to
+            # updated_at_max bookmarked in the interrupted sync.
+            # This will make sure that records with lower id than since_id
+            # which got updated later won't be missed
+            updated_at_max = (last_sync_interrupted_at
+                              or updated_at_min + datetime.timedelta(days=date_window_size))
+            last_sync_interrupted_at = None
+
             if updated_at_max > stop_time:
                 updated_at_max = stop_time
             while True:
                 status_key = self.status_key or "status"
                 query_params = self.get_query_params(since_id,
                                                      status_key,
                                                      updated_at_min,
@@ -262,28 +274,31 @@
 
                 # You know you're at the end when the current page has
                 # less than the request size limits you set.
                 if len(objects) < self.results_per_page:
                     # Save the updated_at_max as our bookmark as we've synced all rows up in our
                     # window and can move forward. Also remove the since_id because we want to
                     # restart at 1.
-                    Context.state.get('bookmarks', {}).get(self.name, {}).pop('since_id', None)
+                    stream_bookmarks = Context.state.get('bookmarks', {}).get(self.name, {})
+                    stream_bookmarks.pop('since_id', None)
+                    stream_bookmarks.pop('updated_at_max', None)
                     self.update_bookmark(utils.strftime(updated_at_max))
                     break
 
                 if objects[-1].id != max([o.id for o in objects]):
                     # This verifies the api behavior expectation we have
                     # that all pages are internally ordered by the
                     # `since_id`.
                     raise OutOfOrderIdsError("{} is not the max id in objects ({})".format(
                         objects[-1].id, max([o.id for o in objects])))
                 since_id = objects[-1].id
 
-                # Put since_id into the state.
+                # Put since_id and updated_at_max into the state.
                 self.update_bookmark(since_id, bookmark_key='since_id')
+                self.update_bookmark(utils.strftime(updated_at_max), bookmark_key='updated_at_max')
 
             updated_at_min = updated_at_max
         bookmark = max(min(stop_time,
                            max_bookmark),
                        (stop_time - datetime.timedelta(days=date_window_size)))
         self.update_bookmark(utils.strftime(bookmark))
```

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/collects.py` & `tap-shopify-1.7.3/tap_shopify/streams/collects.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/events.py` & `tap-shopify-1.7.3/tap_shopify/streams/events.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/inventory_items.py` & `tap-shopify-1.7.3/tap_shopify/streams/inventory_items.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/inventory_levels.py` & `tap-shopify-1.7.3/tap_shopify/streams/inventory_levels.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/locations.py` & `tap-shopify-1.7.3/tap_shopify/streams/locations.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/metafields.py` & `tap-shopify-1.7.3/tap_shopify/streams/metafields.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/order_refunds.py` & `tap-shopify-1.7.3/tap_shopify/streams/order_refunds.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify/streams/transactions.py` & `tap-shopify-1.7.3/tap_shopify/streams/transactions.py`

 * *Files identical despite different names*

### Comparing `tap-shopify-1.7.2/tap_shopify.egg-info/SOURCES.txt` & `tap-shopify-1.7.3/tap_shopify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

