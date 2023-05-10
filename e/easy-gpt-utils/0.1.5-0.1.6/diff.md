# Comparing `tmp/easy_gpt_utils-0.1.5.tar.gz` & `tmp/easy_gpt_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gpt_utils-0.1.5.tar", last modified: Wed May 10 01:37:35 2023, max compression
+gzip compressed data, was "easy_gpt_utils-0.1.6.tar", last modified: Wed May 10 03:19:20 2023, max compression
```

## Comparing `easy_gpt_utils-0.1.5.tar` & `easy_gpt_utils-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 01:37:35.312805 easy_gpt_utils-0.1.5/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)    11357 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.5/LICENSE
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 01:37:35.312805 easy_gpt_utils-0.1.5/PKG-INFO
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      156 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.5/README.md
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 01:37:35.304805 easy_gpt_utils-0.1.5/easy_gpt_utils/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       53 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.5/easy_gpt_utils/__init__.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)     4061 2023-05-09 03:39:40.000000 easy_gpt_utils-0.1.5/easy_gpt_utils/embedding.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)    40471 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.5/easy_gpt_utils/gpt.py
--rw-rw-r--   0 houwei    (1001) houwei    (1001)     4993 2023-05-09 09:03:55.000000 easy_gpt_utils-0.1.5/easy_gpt_utils/vector_database.py
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 01:37:35.311805 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/PKG-INFO
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      326 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)        1 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       22 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/requires.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       15 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/top_level.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       38 2023-05-10 01:37:35.313805 easy_gpt_utils-0.1.5/setup.cfg
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      803 2023-05-10 01:36:25.000000 easy_gpt_utils-0.1.5/setup.py
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:19:20.319657 easy_gpt_utils-0.1.6/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)    11357 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.6/LICENSE
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 03:19:20.318657 easy_gpt_utils-0.1.6/PKG-INFO
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      156 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.6/README.md
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:19:20.311657 easy_gpt_utils-0.1.6/easy_gpt_utils/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      130 2023-05-10 03:18:02.000000 easy_gpt_utils-0.1.6/easy_gpt_utils/__init__.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)     4061 2023-05-09 03:39:40.000000 easy_gpt_utils-0.1.6/easy_gpt_utils/embedding.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)    40471 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.6/easy_gpt_utils/gpt.py
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)     4993 2023-05-09 09:03:55.000000 easy_gpt_utils-0.1.6/easy_gpt_utils/vector_database.py
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:19:20.317657 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      326 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)        1 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       22 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/requires.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       15 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/top_level.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       38 2023-05-10 03:19:20.319657 easy_gpt_utils-0.1.6/setup.cfg
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      803 2023-05-10 03:19:05.000000 easy_gpt_utils-0.1.6/setup.py
```

### Comparing `easy_gpt_utils-0.1.5/LICENSE` & `easy_gpt_utils-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.5/PKG-INFO` & `easy_gpt_utils-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_gpt_utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy GPT utils include 1. chat completion 2. embedding and 3. vector database
 Home-page: https://github.com/ark338/easy_gpt_utils
 Author: Hou Wei
 Author-email: messenger929@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `easy_gpt_utils-0.1.5/easy_gpt_utils/embedding.py` & `easy_gpt_utils-0.1.6/easy_gpt_utils/embedding.py`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.5/easy_gpt_utils/gpt.py` & `easy_gpt_utils-0.1.6/easy_gpt_utils/gpt.py`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.5/easy_gpt_utils/vector_database.py` & `easy_gpt_utils-0.1.6/easy_gpt_utils/vector_database.py`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/PKG-INFO` & `easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-gpt-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Easy GPT utils include 1. chat completion 2. embedding and 3. vector database
 Home-page: https://github.com/ark338/easy_gpt_utils
 Author: Hou Wei
 Author-email: messenger929@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `easy_gpt_utils-0.1.5/setup.py` & `easy_gpt_utils-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="easy_gpt_utils",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
         "openai",
         "tiktoken",
         "numpy"
     ],
     author="Hou Wei",
```

