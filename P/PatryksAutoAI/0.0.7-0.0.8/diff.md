# Comparing `tmp/PatryksAutoAI-0.0.7.tar.gz` & `tmp/PatryksAutoAI-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.0.7.tar", last modified: Wed May 10 16:40:17 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.0.8.tar", last modified: Wed May 10 16:48:48 2023, max compression
```

## Comparing `PatryksAutoAI-0.0.7.tar` & `PatryksAutoAI-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:40:17.711372 PatryksAutoAI-0.0.7/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:40:17.711372 PatryksAutoAI-0.0.7/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-10 16:31:21.000000 PatryksAutoAI-0.0.7/Machine_Learning_Classes/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.0.7/Machine_Learning_Classes/helper_function.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:40:17.711372 PatryksAutoAI-0.0.7/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:40:17.711372 PatryksAutoAI-0.0.7/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:40:17.000000 PatryksAutoAI-0.0.7/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      273 2023-05-10 16:40:17.000000 PatryksAutoAI-0.0.7/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 16:40:17.000000 PatryksAutoAI-0.0.7/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 16:40:17.000000 PatryksAutoAI-0.0.7/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 16:40:17.000000 PatryksAutoAI-0.0.7/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 16:40:17.711372 PatryksAutoAI-0.0.7/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 16:31:25.000000 PatryksAutoAI-0.0.7/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       95 2023-05-10 16:48:00.000000 PatryksAutoAI-0.0.8/Machine_Learning_Classes/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.0.8/Machine_Learning_Classes/helper_function.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      273 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 16:48:48.000000 PatryksAutoAI-0.0.8/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 16:48:48.588164 PatryksAutoAI-0.0.8/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 16:48:38.000000 PatryksAutoAI-0.0.8/setup.py
```

### Comparing `PatryksAutoAI-0.0.7/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.0.8/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.0.7/setup.py` & `PatryksAutoAI-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./Machine_Learning_Classes/requirements.txt') as f:
     requirements = f.read().splitlines()
```

