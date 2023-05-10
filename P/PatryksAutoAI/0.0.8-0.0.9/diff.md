# Comparing `tmp/PatryksAutoAI-0.0.8.tar.gz` & `tmp/PatryksAutoAI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.0.8.tar", last modified: Wed May 10 16:48:48 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.0.9.tar", last modified: Wed May 10 16:55:34 2023, max compression
```

## Comparing `PatryksAutoAI-0.0.8.tar` & `PatryksAutoAI-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,22 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       95 2023-05-10 16:48:00.000000 PatryksAutoAI-0.0.8/Machine_Learning_Classes/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.0.8/Machine_Learning_Classes/helper_function.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      273 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 16:48:38.000000 PatryksAutoAI-0.0.8/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:55:34.755933 PatryksAutoAI-0.0.9/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:55:34.751933 PatryksAutoAI-0.0.9/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       95 2023-05-10 16:49:59.000000 PatryksAutoAI-0.0.9/Machine_Learning_Classes/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:55:34.751933 PatryksAutoAI-0.0.9/Machine_Learning_Classes/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:52:40.000000 PatryksAutoAI-0.0.9/Machine_Learning_Classes/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.0.9/Machine_Learning_Classes/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:55:34.755933 PatryksAutoAI-0.0.9/Machine_Learning_Classes/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:53:23.000000 PatryksAutoAI-0.0.9/Machine_Learning_Classes/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.0.9/Machine_Learning_Classes/model_data/metrics.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.0.9/Machine_Learning_Classes/model_data/metrics_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.0.9/Machine_Learning_Classes/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:55:34.755933 PatryksAutoAI-0.0.9/Machine_Learning_Classes/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:53:05.000000 PatryksAutoAI-0.0.9/Machine_Learning_Classes/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:55:34.755933 PatryksAutoAI-0.0.9/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:55:34.755933 PatryksAutoAI-0.0.9/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:55:34.000000 PatryksAutoAI-0.0.9/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      576 2023-05-10 16:55:34.000000 PatryksAutoAI-0.0.9/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 16:55:34.000000 PatryksAutoAI-0.0.9/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 16:55:34.000000 PatryksAutoAI-0.0.9/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 16:55:34.000000 PatryksAutoAI-0.0.9/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 16:55:34.755933 PatryksAutoAI-0.0.9/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 16:55:28.000000 PatryksAutoAI-0.0.9/setup.py
```

### Comparing `PatryksAutoAI-0.0.8/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.0.9/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.0.8/PKG-INFO` & `PatryksAutoAI-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.0.9/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.0.8/setup.py` & `PatryksAutoAI-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./Machine_Learning_Classes/requirements.txt') as f:
     requirements = f.read().splitlines()
```

