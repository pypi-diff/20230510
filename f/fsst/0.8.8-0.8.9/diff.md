# Comparing `tmp/fsst-0.8.8.tar.gz` & `tmp/fsst-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsst-0.8.8.tar", last modified: Wed May 10 12:02:18 2023, max compression
+gzip compressed data, was "fsst-0.8.9.tar", last modified: Wed May 10 12:39:17 2023, max compression
```

## Comparing `fsst-0.8.8.tar` & `fsst-0.8.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 12:02:18.247876 fsst-0.8.8/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-10 12:02:18.247876 fsst-0.8.8/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.8/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 12:02:18.247876 fsst-0.8.8/fsst.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-10 12:02:17.000000 fsst-0.8.8/fsst.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-10 12:02:18.000000 fsst-0.8.8/fsst.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-10 12:02:17.000000 fsst-0.8.8/fsst.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-10 12:02:17.000000 fsst-0.8.8/fsst.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.8/fsst.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-10 12:02:18.000000 fsst-0.8.8/fsst.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-10 12:02:18.000000 fsst-0.8.8/fsst.egg-info/top_level.txt
--rwxrwxr-x   0 rob       (1000) rob       (1000)   116747 2023-05-10 12:01:50.000000 fsst-0.8.8/fsst.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-10 12:02:18.247876 fsst-0.8.8/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1195 2023-05-10 11:13:44.000000 fsst-0.8.8/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 12:39:17.479915 fsst-0.8.9/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-10 12:39:17.479915 fsst-0.8.9/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.9/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 12:39:17.479915 fsst-0.8.9/fsst.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-10 12:39:16.000000 fsst-0.8.9/fsst.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-10 12:39:17.000000 fsst-0.8.9/fsst.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-10 12:39:17.000000 fsst-0.8.9/fsst.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-10 12:39:17.000000 fsst-0.8.9/fsst.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.9/fsst.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-10 12:39:17.000000 fsst-0.8.9/fsst.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-10 12:39:17.000000 fsst-0.8.9/fsst.egg-info/top_level.txt
+-rwxrwxr-x   0 rob       (1000) rob       (1000)   116907 2023-05-10 12:38:58.000000 fsst-0.8.9/fsst.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-10 12:39:17.479915 fsst-0.8.9/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1195 2023-05-10 11:13:44.000000 fsst-0.8.9/setup.py
```

### Comparing `fsst-0.8.8/PKG-INFO` & `fsst-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.8
+Version: 0.8.9
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.8/README.md` & `fsst-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `fsst-0.8.8/fsst.egg-info/PKG-INFO` & `fsst-0.8.9/fsst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.8
+Version: 0.8.9
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.8/fsst.py` & `fsst-0.8.9/fsst.py`

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
-VERSION = "0.8.8"
+VERSION = "0.8.9"
 CRYPTO_OK = True
 DOCKER_OK = True
 try:
     import aioflureedb
 except ModuleNotFoundError:
     print("WARNING: - aioflureedb python lib not found.")
     CRYPTO_OK = False
@@ -865,26 +865,28 @@
     transactions: list
         All transactions from the first till the current stage to run prior to test runs.
     api_modules: list
         List of dynamically loaded Domain-API modules
 
     """
     # pylint: disable=too-many-locals, too-many-arguments
+    print("domain API test, run =", run)
     # Fluree host context, using priviledged (root role) default key.
     async with aioflureedb.FlureeClient(masterkey=key, host=host,
                                         port=port) as flureeclient:
         await flureeclient.health.ready()
         for test_index, current_test in enumerate(tests):
             print(" ###", current_test["test"], "test_index =", test_index, "###")
             print(" ###", current_test["doc"], "###")
             coverage_treshold = current_test["coverage"]
             coverage = 0
             dbase_name = dbase if test_index == 0 else dbase + "-" + str(test_index) # pylint: disable=compare-to-zero
             if run:
                 dbase_name += "-" + str(run)
+            print("- dbase =", dbase_name)
             # Create the new database for our tests
             await flureeclient.new_ledger(ledger_id=dbase_name)
             fdb = await flureeclient[dbase_name]
             # Database context
             async with fdb(key) as database:
                 await database.ready()
                 full_public_api_root = aioflureedb.domain_api.FlureeDomainAPI(api_dir, database, bigint_patch=False, debug_print=True)
@@ -1264,14 +1266,15 @@
         except FileNotFoundError:
             print("ERROR: No build.json in", fluree_parts, "dir.")
             print("       Use --dir option to specify alternative build dir")
             return
         hooks = Hooks()
         hooks.before()
         for run in range(0, runs):
+            print("RUN:", run)
             if run > 0:
                 if fluree_process is None:
                     print("ERROR: No fluree process to restart")
                 else:
                     fluree_process.terminate()
                     wait_for_flureedb_to_terminate()
                     hooks.between()
@@ -1560,19 +1563,20 @@
                                                  port,
                                                  database,
                                                  createkey,
                                                  test_list,
                                                  expanded2,
                                                  api,
                                                  apimap_modules,
-                                                 run)
+                                                 run=run)
                         else:
                             print("WARNING: Skipping apimap tests because apimap dir is missing or",
                                   "incomplete:", api)
                 maxstage += 1
+            print("RUN completed:", run)
         hooks.after()
         if output:
             # Write the expanded transaction list for all stages combined to a single artifact.
             with open(output, "w") as opf:
                 opf.write(json.dumps(expanded, indent=4))
         elif notest:
             # If no output but notest specified, fill the database with the expanded tranactions
```

### Comparing `fsst-0.8.8/setup.py` & `fsst-0.8.9/setup.py`

 * *Files identical despite different names*

