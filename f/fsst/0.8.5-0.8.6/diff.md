# Comparing `tmp/fsst-0.8.5.tar.gz` & `tmp/fsst-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsst-0.8.5.tar", last modified: Tue May  9 22:44:15 2023, max compression
+gzip compressed data, was "fsst-0.8.6.tar", last modified: Tue May  9 23:08:15 2023, max compression
```

## Comparing `fsst-0.8.5.tar` & `fsst-0.8.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 22:44:15.879866 fsst-0.8.5/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 22:44:15.879866 fsst-0.8.5/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.5/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 22:44:15.879866 fsst-0.8.5/fsst.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.5/fsst.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/top_level.txt
--rwxrwxr-x   0 rob       (1000) rob       (1000)   116361 2023-05-09 22:43:35.000000 fsst-0.8.5/fsst.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 22:44:15.879866 fsst-0.8.5/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1170 2023-05-09 22:43:49.000000 fsst-0.8.5/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 23:08:15.484519 fsst-0.8.6/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 23:08:15.484519 fsst-0.8.6/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.6/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 23:08:15.484519 fsst-0.8.6/fsst.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 23:08:14.000000 fsst-0.8.6/fsst.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.6/fsst.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 23:08:15.000000 fsst-0.8.6/fsst.egg-info/top_level.txt
+-rwxrwxr-x   0 rob       (1000) rob       (1000)   116659 2023-05-09 23:07:16.000000 fsst-0.8.6/fsst.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 23:08:15.484519 fsst-0.8.6/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1170 2023-05-09 23:06:55.000000 fsst-0.8.6/setup.py
```

### Comparing `fsst-0.8.5/PKG-INFO` & `fsst-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.5
+Version: 0.8.6
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.5/README.md` & `fsst-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `fsst-0.8.5/fsst.egg-info/PKG-INFO` & `fsst-0.8.6/fsst.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.5
+Version: 0.8.6
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.5/fsst.py` & `fsst-0.8.6/fsst.py`

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
-VERSION = "0.8.1"
+VERSION = "0.8.6"
 CRYPTO_OK = True
 DOCKER_OK = True
 try:
     import aioflureedb
 except ModuleNotFoundError:
     print("WARNING: - aioflureedb python lib not found.")
     CRYPTO_OK = False
@@ -1124,15 +1124,15 @@
                                            str(test_index) + " : " + str(coverage_treshold) +
                                            " > " + str(coverage))
                 else:
                     raise RuntimeError("No domain-API python testing module loaded for " +
                                        current_test["test"])
 
 
-async def smartfunction_test(host, port, dbase, key, subdir, transactions, fluree_parts):
+async def smartfunction_test(host, port, dbase, key, subdir, transactions, fluree_parts, run=0):
     """Create a test database, initialize database with transactions up to stage and run all
        tests for stage.
 
     Parameters
     ----------
     host: string
         The FlureeDB host
@@ -1160,34 +1160,36 @@
     # Fluree host context, using priviledged (root role) default key.
     async with aioflureedb.FlureeClient(masterkey=key, host=host,
                                         port=port) as flureeclient:
         print("Client created")
         await flureeclient.health.ready()
         print("Server ready, creating database", dbase)
         # Create the new database for our tests
-        await flureeclient.new_ledger(ledger_id=dbase)
+        if run == 0:
+            await flureeclient.new_ledger(ledger_id=dbase)
         print("Database created")
         fdb = await flureeclient[dbase]
         print("Database handle fetched")
         # Database context
         async with fdb(key) as database:
             print("Database handle context opened")
             await database.ready()
             print("Database ready")
             # Run all the transactions in preparation to the tests
-            print(" - processing schema transaction sub-set")
-            for transaction in transactions:
-                try:
-                    await database.command.transaction(transaction)
-                except aioflureedb.FlureeException as exp:
-                    print("Exception while processing schema transaction")
-                    print(json.dumps(transaction, indent=4, sort_keys=True))
-                    print()
-                    raise exp
-            print(" - ok, completed", len(transactions), "transactions on", dbase)
+            if run == 0:
+                print(" - processing schema transaction sub-set")
+                for transaction in transactions:
+                    try:
+                        await database.command.transaction(transaction)
+                    except aioflureedb.FlureeException as exp:
+                        print("Exception while processing schema transaction")
+                        print(json.dumps(transaction, indent=4, sort_keys=True))
+                        print()
+                        raise exp
+                print(" - ok, completed", len(transactions), "transactions on", dbase)
             # Read the test scenario config file for this stage.
             with open(os.path.join(fluree_parts, subdir, "test.json")) as testscenariosfile:
                 testscenarios = json.load(testscenariosfile)
             print(" - running test scenarios")
             # Run all test scenarios.
             for scenario in testscenarios:
                 await run_test_scenario(database, subdir, fluree_parts, fdb, scenario)
@@ -1260,25 +1262,28 @@
         except FileNotFoundError:
             print("ERROR: No build.json in", fluree_parts, "dir.")
             print("       Use --dir option to specify alternative build dir")
             return
         hooks = Hooks()
         hooks.before()
         for run in range(0, runs):
-            if run > 0 and fluree_process is not None:
-                fluree_process.terminate()
-                wait_for_flureedb_to_terminate()
-                hooks.between()
-                command = ["/bin/bash", "/usr/src/fsst/fluree_start.sh", "-Dfdb-api-port=8090"]
-                if not verbosefluree:
-                    # pylint: disable=consider-using-with
-                    fluree_process = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+            if run > 0:
+                if fluree_process is None:
+                    print("ERROR: No fluree process to restart")
                 else:
-                    # pylint: disable=consider-using-with
-                    fluree_process = subprocess.Popen(command)
+                    fluree_process.terminate()
+                    wait_for_flureedb_to_terminate()
+                    hooks.between()
+                    command = ["/bin/bash", "/usr/src/fsst/fluree_start.sh", "-Dfdb-api-port=8090"]
+                    if not verbosefluree:
+                        # pylint: disable=consider-using-with
+                        fluree_process = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+                    else:
+                        # pylint: disable=consider-using-with
+                        fluree_process = subprocess.Popen(command)
             maxstage = 0
             # Outer loop for finding out where and how far to run the inner loop.
             # pylint: disable=too-many-nested-blocks
             testcount = 0
             for subdir in build:
                 if output or notest:
                     # If output or notest, we dont run any tests, we just fill the expanded list
@@ -1352,15 +1357,16 @@
                             print("Running smartfunction_test")
                             await smartfunction_test(host,
                                                      port,
                                                      database,
                                                      createkey,
                                                      build[maxstage],
                                                      expanded2,
-                                                     fluree_parts)
+                                                     fluree_parts,
+                                                     run=run)
                         else:
                             print("Skipping tests for", build[maxstage])
                     # If notest is false and the stage has a domain.json,
                     #  we run domain-API tests
                     testfile = os.path.join(fluree_parts, subdir, "domain.json")
                     if os.path.isfile(testfile) and not notest and (allstages or subdir in teststages):
                         expanded2 = []
```

### Comparing `fsst-0.8.5/setup.py` & `fsst-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fsst',
-    version="0.8.5",
+    version="0.8.6",
     description="Fluree Schema Scenario Tool",
     long_description="Testing tool for schema and smart function unit tests for FlureeDB",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/fluree-schema-scenario-tool',
     license='BSD',
     py_modules=['fsst'],
```

