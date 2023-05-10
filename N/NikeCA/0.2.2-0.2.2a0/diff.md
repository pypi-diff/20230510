# Comparing `tmp/NikeCA-0.2.2.tar.gz` & `tmp/NikeCA-0.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.2.2.tar", last modified: Wed May 10 18:28:18 2023, max compression
+gzip compressed data, was "NikeCA-0.2.2a0.tar", last modified: Wed May 10 19:02:33 2023, max compression
```

## Comparing `NikeCA-0.2.2.tar` & `NikeCA-0.2.2a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.871101 NikeCA-0.2.2/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.2/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 18:28:18.870650 NikeCA-0.2.2/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.2/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 18:28:18.871221 NikeCA-0.2.2/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2502 2023-05-10 18:27:12.000000 NikeCA-0.2.2/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.861583 NikeCA-0.2.2/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.863152 NikeCA-0.2.2/src/Dashboards/
--rw-r--r--   0 WCheaq     (502) staff       (20)     4020 2023-05-07 22:07:42.000000 NikeCA-0.2.2/src/Dashboards/Dashboards.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.864641 NikeCA-0.2.2/src/Dashboards/InclusionExclusion/
--rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.2.2/src/Dashboards/InclusionExclusion/InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/Dashboards/InclusionExclusion/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.866826 NikeCA-0.2.2/src/Dashboards/Telemetry/
--rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/Dashboards/Telemetry/ProductUsage.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     6140 2023-05-08 17:16:29.000000 NikeCA-0.2.2/src/Dashboards/Telemetry/Telemetry.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/Dashboards/Telemetry/__init__.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/Dashboards/__init__.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 18:28:18.870016 NikeCA-0.2.2/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18011 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-10 18:28:18.000000 NikeCA-0.2.2/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.2.2/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    19181 2023-05-10 18:07:25.000000 NikeCA-0.2.2/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.2.2/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.2.2/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.2.2/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.2.2/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.371349 NikeCA-0.2.2a0/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-04-17 20:38:20.000000 NikeCA-0.2.2a0/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-10 19:02:33.370838 NikeCA-0.2.2a0/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-04-17 20:38:20.000000 NikeCA-0.2.2a0/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-05-10 19:02:33.371483 NikeCA-0.2.2a0/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2503 2023-05-10 19:02:23.000000 NikeCA-0.2.2a0/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.363345 NikeCA-0.2.2a0/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.364772 NikeCA-0.2.2a0/src/Dashboards/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4020 2023-05-07 22:07:42.000000 NikeCA-0.2.2a0/src/Dashboards/Dashboards.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.365745 NikeCA-0.2.2a0/src/Dashboards/InclusionExclusion/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9016 2023-05-07 20:33:10.000000 NikeCA-0.2.2a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/Dashboards/InclusionExclusion/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.367304 NikeCA-0.2.2a0/src/Dashboards/Telemetry/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     5902 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/Dashboards/Telemetry/ProductUsage.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     6140 2023-05-08 17:16:29.000000 NikeCA-0.2.2a0/src/Dashboards/Telemetry/Telemetry.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        2 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/Dashboards/Telemetry/__init__.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/Dashboards/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-05-10 19:02:33.370246 NikeCA-0.2.2a0/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18013 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      672 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1184 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      362 2023-05-10 19:02:33.000000 NikeCA-0.2.2a0/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      428 2023-05-07 22:01:04.000000 NikeCA-0.2.2a0/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    19181 2023-05-10 18:07:25.000000 NikeCA-0.2.2a0/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13609 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14112 2023-05-04 17:11:39.000000 NikeCA-0.2.2a0/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7068 2023-05-04 17:07:22.000000 NikeCA-0.2.2a0/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7134 2023-05-07 19:42:02.000000 NikeCA-0.2.2a0/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)      231 2023-05-03 02:40:56.000000 NikeCA-0.2.2a0/src/__init__.py
```

### Comparing `NikeCA-0.2.2/LICENSE` & `NikeCA-0.2.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/PKG-INFO` & `NikeCA-0.2.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.2
+Version: 0.2.2a0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.2/README.md` & `NikeCA-0.2.2a0/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/setup.py` & `NikeCA-0.2.2a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.2.2',
+	version='0.2.2a',
 	description='Standardize and Automate processes',
 	py_modules=[
 		"__init__",
 		"_BuildSearchQuery",
 		"_GitHub",
 		"_SearchFiles",
 		"_SnowflakeData",
```

### Comparing `NikeCA-0.2.2/src/Dashboards/Dashboards.py` & `NikeCA-0.2.2a0/src/Dashboards/Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/Dashboards/InclusionExclusion/InclusionExclusion.py` & `NikeCA-0.2.2a0/src/Dashboards/InclusionExclusion/InclusionExclusion.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/Dashboards/Telemetry/ProductUsage.py` & `NikeCA-0.2.2a0/src/Dashboards/Telemetry/ProductUsage.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/Dashboards/Telemetry/Telemetry.py` & `NikeCA-0.2.2a0/src/Dashboards/Telemetry/Telemetry.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.2.2a0/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.2.2
+Version: 0.2.2a0
 Summary: Standardize and Automate processes
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.2.2/src/NikeCA.egg-info/SOURCES.txt` & `NikeCA-0.2.2a0/src/NikeCA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.2.2a0/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/NikeQA.py` & `NikeCA-0.2.2a0/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/NikeSF.py` & `NikeCA-0.2.2a0/src/NikeSF.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/_BuildSearchQuery.py` & `NikeCA-0.2.2a0/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/_GitHub.py` & `NikeCA-0.2.2a0/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/_QA.py` & `NikeCA-0.2.2a0/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/_SearchFiles.py` & `NikeCA-0.2.2a0/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/_SnowflakeData.py` & `NikeCA-0.2.2a0/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/_SnowflakeDependencies.py` & `NikeCA-0.2.2a0/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.2.2/src/_SnowflakePull.py` & `NikeCA-0.2.2a0/src/_SnowflakePull.py`

 * *Files identical despite different names*

