# Comparing `tmp/NikeCA-0.2.2rc0.tar.gz` & `tmp/NikeCA-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.2.2rc0.tar", last modified: Wed May 10 19:56:07 2023, max compression
+gzip compressed data, was "NikeCA-0.2.3.tar", last modified: Wed May 10 20:33:01 2023, max compression
```

## Comparing `NikeCA-0.2.2rc0.tar` & `NikeCA-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.070460 NikeCA-0.2.2rc0/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.2rc0/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18014 2023-05-10 19:56:07.070051 NikeCA-0.2.2rc0/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.2rc0/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 19:56:07.070587 NikeCA-0.2.2rc0/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2487 2023-05-10 19:55:46.000000 NikeCA-0.2.2rc0/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.061057 NikeCA-0.2.2rc0/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.062524 NikeCA-0.2.2rc0/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.2rc0/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.064377 NikeCA-0.2.2rc0/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.2rc0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       27 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.066670 NikeCA-0.2.2rc0/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.2rc0/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.2rc0/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       39 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       44 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:56:07.069408 NikeCA-0.2.2rc0/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18014 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 19:56:06.000000 NikeCA-0.2.2rc0/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      339 2023-05-10 19:50:52.000000 NikeCA-0.2.2rc0/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19225 2023-05-10 19:50:52.000000 NikeCA-0.2.2rc0/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14091 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.2rc0/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)       45 2023-05-10 19:46:50.000000 NikeCA-0.2.2rc0/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:33:01.497192 NikeCA-0.2.3/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.3/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 20:33:01.496763 NikeCA-0.2.3/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.3/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 20:33:01.497317 NikeCA-0.2.3/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2486 2023-05-10 20:31:31.000000 NikeCA-0.2.3/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:33:01.486739 NikeCA-0.2.3/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:33:01.488887 NikeCA-0.2.3/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4244 2023-05-10 19:45:47.000000 NikeCA-0.2.3/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:33:01.491201 NikeCA-0.2.3/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    10886 2023-05-10 19:45:47.000000 NikeCA-0.2.3/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       27 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:33:01.493509 NikeCA-0.2.3/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6967 2023-05-10 19:41:44.000000 NikeCA-0.2.3/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7325 2023-05-10 19:45:47.000000 NikeCA-0.2.3/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       39 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       44 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 20:33:01.496124 NikeCA-0.2.3/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 20:33:01.000000 NikeCA-0.2.3/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 20:33:01.000000 NikeCA-0.2.3/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 20:33:01.000000 NikeCA-0.2.3/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 20:33:01.000000 NikeCA-0.2.3/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      351 2023-05-10 20:33:01.000000 NikeCA-0.2.3/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      344 2023-05-10 20:27:42.000000 NikeCA-0.2.3/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19225 2023-05-10 19:50:52.000000 NikeCA-0.2.3/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14091 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7154 2023-05-10 19:40:28.000000 NikeCA-0.2.3/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)       49 2023-05-10 20:27:42.000000 NikeCA-0.2.3/src/__init__.py
```

### Comparing `NikeCA-0.2.2rc0/LICENSE` & `NikeCA-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/PKG-INFO` & `NikeCA-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.2rc0
+Version: 0.2.3
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.2rc0/README.md` & `NikeCA-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/setup.py` & `NikeCA-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.2.2c',
+	version='0.2.3',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"_BuildSearchQuery",
 		"_GitHub",
 		"_SearchFiles",
 		"_SnowflakeData",
```

### Comparing `NikeCA-0.2.2rc0/src/Dashboards/Dashboards.py` & `NikeCA-0.2.3/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.2.3/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.2.3/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.2.3/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.2.3/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.2rc0
+Version: 0.2.3
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.2rc0/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.2.3/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.2.3/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/NikeQA.py` & `NikeCA-0.2.3/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/NikeSF.py` & `NikeCA-0.2.3/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/_BuildSearchQuery.py` & `NikeCA-0.2.3/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/_GitHub.py` & `NikeCA-0.2.3/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/_QA.py` & `NikeCA-0.2.3/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/_SearchFiles.py` & `NikeCA-0.2.3/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/_SnowflakeData.py` & `NikeCA-0.2.3/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/_SnowflakeDependencies.py` & `NikeCA-0.2.3/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2rc0/src/_SnowflakePull.py` & `NikeCA-0.2.3/src/_SnowflakePull.py`

 * *Files identical despite different names*

