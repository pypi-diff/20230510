# Comparing `tmp/PatryksAutoAI-0.0.5.tar.gz` & `tmp/PatryksAutoAI-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.0.5.tar", last modified: Wed May 10 16:08:39 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.0.6.tar", last modified: Wed May 10 16:25:22 2023, max compression
```

## Comparing `PatryksAutoAI-0.0.5.tar` & `PatryksAutoAI-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:08:39.249589 PatryksAutoAI-0.0.5/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:08:39.249589 PatryksAutoAI-0.0.5/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       56 2023-05-10 15:24:32.000000 PatryksAutoAI-0.0.5/Machine_Learning_Classes/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.0.5/Machine_Learning_Classes/helper_function.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:08:39.249589 PatryksAutoAI-0.0.5/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:08:39.249589 PatryksAutoAI-0.0.5/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:08:39.000000 PatryksAutoAI-0.0.5/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      273 2023-05-10 16:08:39.000000 PatryksAutoAI-0.0.5/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 16:08:39.000000 PatryksAutoAI-0.0.5/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      164 2023-05-10 16:08:39.000000 PatryksAutoAI-0.0.5/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 16:08:39.000000 PatryksAutoAI-0.0.5/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 16:08:39.249589 PatryksAutoAI-0.0.5/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 16:08:28.000000 PatryksAutoAI-0.0.5/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:25:22.086462 PatryksAutoAI-0.0.6/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:25:22.086462 PatryksAutoAI-0.0.6/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       81 2023-05-10 16:24:53.000000 PatryksAutoAI-0.0.6/Machine_Learning_Classes/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.0.6/Machine_Learning_Classes/helper_function.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:25:22.086462 PatryksAutoAI-0.0.6/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:25:22.086462 PatryksAutoAI-0.0.6/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:25:22.000000 PatryksAutoAI-0.0.6/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      273 2023-05-10 16:25:22.000000 PatryksAutoAI-0.0.6/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 16:25:22.000000 PatryksAutoAI-0.0.6/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 16:25:22.000000 PatryksAutoAI-0.0.6/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 16:25:22.000000 PatryksAutoAI-0.0.6/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 16:25:22.086462 PatryksAutoAI-0.0.6/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 16:24:47.000000 PatryksAutoAI-0.0.6/setup.py
```

### Comparing `PatryksAutoAI-0.0.5/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.0.6/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.0.5/PKG-INFO` & `PatryksAutoAI-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.0.5/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.0.6/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.0.5
+Version: 0.0.6
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.0.5/setup.py` & `PatryksAutoAI-0.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./Machine_Learning_Classes/requirements.txt') as f:
     requirements = f.read().splitlines()
```

