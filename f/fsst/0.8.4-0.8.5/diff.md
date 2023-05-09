# Comparing `tmp/fsst-0.8.4.tar.gz` & `tmp/fsst-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsst-0.8.4.tar", last modified: Tue May  9 21:14:18 2023, max compression
+gzip compressed data, was "fsst-0.8.5.tar", last modified: Tue May  9 22:44:15 2023, max compression
```

## Comparing `fsst-0.8.4.tar` & `fsst-0.8.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 21:14:18.677457 fsst-0.8.4/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 21:14:18.677457 fsst-0.8.4/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.4/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 21:14:18.677457 fsst-0.8.4/fsst.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.4/fsst.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/top_level.txt
--rwxrwxr-x   0 rob       (1000) rob       (1000)   116361 2023-05-09 21:14:03.000000 fsst-0.8.4/fsst.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 21:14:18.677457 fsst-0.8.4/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1170 2023-05-09 21:14:11.000000 fsst-0.8.4/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 22:44:15.879866 fsst-0.8.5/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 22:44:15.879866 fsst-0.8.5/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.5/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 22:44:15.879866 fsst-0.8.5/fsst.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.5/fsst.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 22:44:15.000000 fsst-0.8.5/fsst.egg-info/top_level.txt
+-rwxrwxr-x   0 rob       (1000) rob       (1000)   116361 2023-05-09 22:43:35.000000 fsst-0.8.5/fsst.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 22:44:15.879866 fsst-0.8.5/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1170 2023-05-09 22:43:49.000000 fsst-0.8.5/setup.py
```

### Comparing `fsst-0.8.4/PKG-INFO` & `fsst-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.4
+Version: 0.8.5
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.4/README.md` & `fsst-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `fsst-0.8.4/fsst.egg-info/PKG-INFO` & `fsst-0.8.5/fsst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.4
+Version: 0.8.5
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.4/fsst.py` & `fsst-0.8.5/fsst.py`

 * *Files 0% similar despite different names*

```diff
@@ -1260,15 +1260,15 @@
         except FileNotFoundError:
             print("ERROR: No build.json in", fluree_parts, "dir.")
             print("       Use --dir option to specify alternative build dir")
             return
         hooks = Hooks()
         hooks.before()
         for run in range(0, runs):
-            if run > 1 and fluree_process is not None:
+            if run > 0 and fluree_process is not None:
                 fluree_process.terminate()
                 wait_for_flureedb_to_terminate()
                 hooks.between()
                 command = ["/bin/bash", "/usr/src/fsst/fluree_start.sh", "-Dfdb-api-port=8090"]
                 if not verbosefluree:
                     # pylint: disable=consider-using-with
                     fluree_process = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```

### Comparing `fsst-0.8.4/setup.py` & `fsst-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fsst',
-    version="0.8.4",
+    version="0.8.5",
     description="Fluree Schema Scenario Tool",
     long_description="Testing tool for schema and smart function unit tests for FlureeDB",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/fluree-schema-scenario-tool',
     license='BSD',
     py_modules=['fsst'],
```

