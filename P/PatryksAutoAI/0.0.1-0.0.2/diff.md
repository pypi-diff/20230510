# Comparing `tmp/PatryksAutoAI-0.0.1.tar.gz` & `tmp/PatryksAutoAI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.0.1.tar", last modified: Wed May 10 15:10:29 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.0.2.tar", last modified: Wed May 10 15:41:45 2023, max compression
```

## Comparing `PatryksAutoAI-0.0.1.tar` & `PatryksAutoAI-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 15:10:29.611993 PatryksAutoAI-0.0.1/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 15:10:29.611993 PatryksAutoAI-0.0.1/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       95 2023-05-10 15:04:54.000000 PatryksAutoAI-0.0.1/Machine_Learning_Classes/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.0.1/Machine_Learning_Classes/helper_function.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      517 2023-05-10 15:10:29.611993 PatryksAutoAI-0.0.1/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 15:10:29.611993 PatryksAutoAI-0.0.1/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      517 2023-05-10 15:10:29.000000 PatryksAutoAI-0.0.1/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      237 2023-05-10 15:10:29.000000 PatryksAutoAI-0.0.1/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 15:10:29.000000 PatryksAutoAI-0.0.1/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 15:10:29.000000 PatryksAutoAI-0.0.1/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 15:10:29.611993 PatryksAutoAI-0.0.1/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      809 2023-05-10 15:10:23.000000 PatryksAutoAI-0.0.1/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 15:41:45.237884 PatryksAutoAI-0.0.2/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 15:41:45.233884 PatryksAutoAI-0.0.2/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       56 2023-05-10 15:24:32.000000 PatryksAutoAI-0.0.2/Machine_Learning_Classes/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.0.2/Machine_Learning_Classes/helper_function.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 15:41:45.237884 PatryksAutoAI-0.0.2/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 15:41:45.237884 PatryksAutoAI-0.0.2/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 15:41:45.000000 PatryksAutoAI-0.0.2/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      273 2023-05-10 15:41:45.000000 PatryksAutoAI-0.0.2/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 15:41:45.000000 PatryksAutoAI-0.0.2/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      157 2023-05-10 15:41:45.000000 PatryksAutoAI-0.0.2/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 15:41:45.000000 PatryksAutoAI-0.0.2/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 15:41:45.237884 PatryksAutoAI-0.0.2/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 15:40:20.000000 PatryksAutoAI-0.0.2/setup.py
```

### Comparing `PatryksAutoAI-0.0.1/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.0.2/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.0.1/PKG-INFO` & `PatryksAutoAI-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.0.1
+Version: 0.0.2
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
+Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 UNKNOWN
```

### Comparing `PatryksAutoAI-0.0.1/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.0.2/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.0.1
+Version: 0.0.2
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
+Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 UNKNOWN
```

### Comparing `PatryksAutoAI-0.0.1/setup.py` & `PatryksAutoAI-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Auto_AI_patryk'
-LONG_DESCRIPTION = 'Package contain helping functions for creating ML models'
+LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
+
+# Read the requirements from requirements.txt
+with open('./Machine_Learning_Classes/requirements.txt') as f:
+    requirements = f.read().splitlines()
 
 setup(
     name="PatryksAutoAI",
     version=VERSION,
     author="patryk",
+    author_email="lyczkopatryk1@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=[],
+    install_requires=requirements, 
     keywords=['python', 'machine_learning', 'auto'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX :: Linux",
     ]
 )
```

