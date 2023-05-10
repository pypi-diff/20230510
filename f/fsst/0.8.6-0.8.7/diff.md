# Comparing `tmp/fsst-0.8.6.tar.gz` & `tmp/fsst-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsst-0.8.6.tar", last modified: Tue May  9 23:08:15 2023, max compression
+gzip compressed data, was "fsst-0.8.7.tar", last modified: Wed May 10 11:14:26 2023, max compression
```

## Comparing `fsst-0.8.6.tar` & `fsst-0.8.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 23:08:15.484519 fsst-0.8.6/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 23:08:15.484519 fsst-0.8.6/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.6/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 23:08:15.484519 fsst-0.8.6/fsst.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 23:08:14.000000 fsst-0.8.6/fsst.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.6/fsst.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/top_level.txt
--rwxrwxr-x   0 rob       (1000) rob       (1000)   116659 2023-05-09 23:07:16.000000 fsst-0.8.6/fsst.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 23:08:15.484519 fsst-0.8.6/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1170 2023-05-09 23:06:55.000000 fsst-0.8.6/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 11:14:26.467332 fsst-0.8.7/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-10 11:14:26.467332 fsst-0.8.7/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.7/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 11:14:26.467332 fsst-0.8.7/fsst.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-10 11:14:25.000000 fsst-0.8.7/fsst.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-10 11:14:26.000000 fsst-0.8.7/fsst.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-10 11:14:26.000000 fsst-0.8.7/fsst.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-10 11:14:26.000000 fsst-0.8.7/fsst.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.7/fsst.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-10 11:14:26.000000 fsst-0.8.7/fsst.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-10 11:14:26.000000 fsst-0.8.7/fsst.egg-info/top_level.txt
+-rwxrwxr-x   0 rob       (1000) rob       (1000)   116783 2023-05-10 11:14:06.000000 fsst-0.8.7/fsst.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-10 11:14:26.467332 fsst-0.8.7/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1195 2023-05-10 11:13:44.000000 fsst-0.8.7/setup.py
```

### Comparing `fsst-0.8.6/PKG-INFO` & `fsst-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.6
+Version: 0.8.7
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.6/README.md` & `fsst-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `fsst-0.8.6/fsst.egg-info/PKG-INFO` & `fsst-0.8.7/fsst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.6
+Version: 0.8.7
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.6/fsst.py` & `fsst-0.8.7/fsst.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import argparse
 import json
 import time
 import asyncio
 import itertools
 import importlib.util
 import requests
-VERSION = "0.8.6"
+VERSION = "0.8.7"
 CRYPTO_OK = True
 DOCKER_OK = True
 try:
     import aioflureedb
 except ModuleNotFoundError:
     print("WARNING: - aioflureedb python lib not found.")
     CRYPTO_OK = False
@@ -840,15 +840,15 @@
                                   keys=tnokeys)
     # Run cleanup transactions
     await process_fluree_testfile(database,
                                   fdb,
                                   os.path.join(testdir, "cleanup.json"))
 
 
-async def domainapi_test(host, port, dbase, key, tests, transactions, api_dir, api_modules):
+async def domainapi_test(host, port, dbase, key, tests, transactions, api_dir, api_modules, run=0):
     # pylint: disable=too-many-statements, too-many-branches
     """Create a test database, initialize database with transactions up to stage and run all
        domain-API tests for stage.
 
     Parameters
     ----------
     host: string
@@ -875,14 +875,16 @@
         await flureeclient.health.ready()
         for test_index, current_test in enumerate(tests):
             print(" ###", current_test["test"], "test_index =", test_index, "###")
             print(" ###", current_test["doc"], "###")
             coverage_treshold = current_test["coverage"]
             coverage = 0
             dbase_name = dbase if test_index == 0 else dbase + "-" + str(test_index) # pylint: disable=compare-to-zero
+            if run:
+                dbase_name += "-" + str(run)
             # Create the new database for our tests
             await flureeclient.new_ledger(ledger_id=dbase_name)
             fdb = await flureeclient[dbase_name]
             # Database context
             async with fdb(key) as database:
                 await database.ready()
                 full_public_api_root = aioflureedb.domain_api.FlureeDomainAPI(api_dir, database, bigint_patch=False, debug_print=True)
@@ -1160,26 +1162,26 @@
     # Fluree host context, using priviledged (root role) default key.
     async with aioflureedb.FlureeClient(masterkey=key, host=host,
                                         port=port) as flureeclient:
         print("Client created")
         await flureeclient.health.ready()
         print("Server ready, creating database", dbase)
         # Create the new database for our tests
-        if run == 0:
+        if not run:
             await flureeclient.new_ledger(ledger_id=dbase)
         print("Database created")
         fdb = await flureeclient[dbase]
         print("Database handle fetched")
         # Database context
         async with fdb(key) as database:
             print("Database handle context opened")
             await database.ready()
             print("Database ready")
             # Run all the transactions in preparation to the tests
-            if run == 0:
+            if not run:
                 print(" - processing schema transaction sub-set")
                 for transaction in transactions:
                     try:
                         await database.command.transaction(transaction)
                     except aioflureedb.FlureeException as exp:
                         print("Exception while processing schema transaction")
                         print(json.dumps(transaction, indent=4, sort_keys=True))
@@ -1557,15 +1559,16 @@
                             await domainapi_test(host,
                                                  port,
                                                  database,
                                                  createkey,
                                                  test_list,
                                                  expanded2,
                                                  api,
-                                                 apimap_modules)
+                                                 apimap_modules,
+                                                 run)
                         else:
                             print("WARNING: Skipping apimap tests because apimap dir is missing or",
                                   "incomplete:", api)
                 maxstage += 1
         hooks.after()
         if output:
             # Write the expanded transaction list for all stages combined to a single artifact.
```

### Comparing `fsst-0.8.6/setup.py` & `fsst-0.8.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup
+from fsst import VERSION
 
 setup(
     name='fsst',
-    version="0.8.6",
+    version=VERSION,
     description="Fluree Schema Scenario Tool",
     long_description="Testing tool for schema and smart function unit tests for FlureeDB",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/fluree-schema-scenario-tool',
     license='BSD',
     py_modules=['fsst'],
```

