# Comparing `tmp/NikeCA-0.2.0.tar.gz` & `tmp/NikeCA-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.2.0.tar", last modified: Sun May  7 22:14:24 2023, max compression
+gzip compressed data, was "NikeCA-0.2.1.tar", last modified: Wed May 10 17:50:52 2023, max compression
```

## Comparing `NikeCA-0.2.0.tar` & `NikeCA-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:14:24.470006 NikeCA-0.2.0/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.0/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-07 22:14:24.469648 NikeCA-0.2.0/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.0/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-07 22:14:24.470115 NikeCA-0.2.0/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2502 2023-05-07 22:14:14.000000 NikeCA-0.2.0/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:14:24.460036 NikeCA-0.2.0/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:14:24.461430 NikeCA-0.2.0/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4020 2023-05-07 22:07:42.000000 NikeCA-0.2.0/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:14:24.462688 NikeCA-0.2.0/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.2.0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:14:24.465005 NikeCA-0.2.0/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6138 2023-05-07 21:58:42.000000 NikeCA-0.2.0/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-07 22:14:24.468307 NikeCA-0.2.0/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-07 22:14:24.000000 NikeCA-0.2.0/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-07 22:14:24.000000 NikeCA-0.2.0/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-07 22:14:24.000000 NikeCA-0.2.0/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-07 22:14:24.000000 NikeCA-0.2.0/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-07 22:14:24.000000 NikeCA-0.2.0/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.2.0/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    23787 2023-05-07 21:48:03.000000 NikeCA-0.2.0/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.2.0/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.2.0/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.2.0/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.2.0/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.900535 NikeCA-0.2.1/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.1/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 17:50:52.900140 NikeCA-0.2.1/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.1/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 17:50:52.900655 NikeCA-0.2.1/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2502 2023-05-10 17:50:03.000000 NikeCA-0.2.1/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.892196 NikeCA-0.2.1/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.893756 NikeCA-0.2.1/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4020 2023-05-07 22:07:42.000000 NikeCA-0.2.1/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.894836 NikeCA-0.2.1/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.2.1/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.896470 NikeCA-0.2.1/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6140 2023-05-08 17:16:29.000000 NikeCA-0.2.1/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 17:50:52.899442 NikeCA-0.2.1/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-10 17:50:52.000000 NikeCA-0.2.1/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.2.1/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23793 2023-05-08 17:16:29.000000 NikeCA-0.2.1/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.2.1/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.2.1/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.2.1/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.2.1/src/__init__.py
```

### Comparing `NikeCA-0.2.0/LICENSE` & `NikeCA-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/PKG-INFO` & `NikeCA-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.0
+Version: 0.2.1
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.0/README.md` & `NikeCA-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/setup.py` & `NikeCA-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.2.0',
+	version='0.2.1',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
-		"NikeSF",
-		"_SnowflakeData",
 		"_BuildSearchQuery",
+		"_GitHub",
+		"_SearchFiles",
+		"_SnowflakeData",
+		"_SnowflakeDependencies",
+		"_SnowflakePull",
+		"_QA",
+		"Dashboards",
 		"Dashboards/__init__",
+		"Dashboards/Dashboards",
 		"Dashboards/InclusionExclusion/InclusionExclusion",
 		"Dashboards/InclusionExclusion/__init__",
 		"Dashboards/Telemetry/ProductUsage",
 		"Dashboards/Telemetry/Telemetry",
 		"Dashboards/Telemetry/__init__",
-		"Dashboards/Dashboards",
-		"Dashboards",
-		"_SearchFiles",
-		"_SnowflakeDependencies",
-		"_SnowflakePull",
-		"NikeQA",
-		"_QA",
-		"_GitHub",
-		"NikeCA"
+		"NikeCA",
+		"NikeSF",
+		"NikeQA"
 	],
 	package_dir={'': 'src'},
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"Programming Language :: Python :: 3.11",
 		"License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
 		"Operating System :: OS Independent",
```

### Comparing `NikeCA-0.2.0/src/Dashboards/Dashboards.py` & `NikeCA-0.2.1/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.2.1/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.2.1/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.2.1/src/Dashboards/Telemetry/Telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from .ProductUsage import ProductUsage
 
 
 class Telemetry(ProductUsage):
 
-    ProductUsage = ProductUsage
+    ProductUsage = ProductUsage()
 
     def telemetry_product_viewed(self
                        , username: str
                        , warehouse: str
                        , database: str
                        , role: str
                        , filters: list | None = None
```

### Comparing `NikeCA-0.2.0/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.2.1/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.0
+Version: 0.2.1
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.0/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.2.1/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.2.1/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/NikeQA.py` & `NikeCA-0.2.1/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/NikeSF.py` & `NikeCA-0.2.1/src/NikeSF.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from Dashboards.InclusionExclusion.InclusionExclusion import InclusionExclusion
 from Dashboards.Telemetry.Telemetry import Telemetry
 from Dashboards.Telemetry.ProductUsage import ProductUsage
 
 
 class Snowflake(SnowflakeData, Dashboards, SnowflakeDependencies, BuildSearchQuery):#, InclusionExclusion):
 
-    Dashboards = Dashboards
-    Telemetry = Telemetry
-    ProductUsage = ProductUsage
+    Dashboards = Dashboards()
+    Telemetry = Telemetry()
+    ProductUsage = ProductUsage()
 
     """
         A class for interacting with Snowflake databases and executing queries.
         Inherits from _SnowflakeData.SnowflakeData.
         """
 
     # Constructor
```

### Comparing `NikeCA-0.2.0/src/_BuildSearchQuery.py` & `NikeCA-0.2.1/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/_GitHub.py` & `NikeCA-0.2.1/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/_QA.py` & `NikeCA-0.2.1/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/_SearchFiles.py` & `NikeCA-0.2.1/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/_SnowflakeData.py` & `NikeCA-0.2.1/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/_SnowflakeDependencies.py` & `NikeCA-0.2.1/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.0/src/_SnowflakePull.py` & `NikeCA-0.2.1/src/_SnowflakePull.py`

 * *Files identical despite different names*

