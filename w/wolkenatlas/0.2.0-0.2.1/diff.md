# Comparing `tmp/wolkenatlas-0.2.0.tar.gz` & `tmp/wolkenatlas-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolkenatlas-0.2.0.tar", last modified: Wed May 10 09:51:37 2023, max compression
+gzip compressed data, was "wolkenatlas-0.2.1.tar", last modified: Wed May 10 13:10:20 2023, max compression
```

## Comparing `wolkenatlas-0.2.0.tar` & `wolkenatlas-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 09:51:37.827349 wolkenatlas-0.2.0/
--rw-r--r--   0 tkober     (502) staff       (20)     1063 2022-05-13 10:09:18.000000 wolkenatlas-0.2.0/LICENSE
--rw-r--r--   0 tkober     (502) staff       (20)       58 2022-07-15 11:38:43.000000 wolkenatlas-0.2.0/MANIFEST.in
--rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-05-10 09:51:37.827122 wolkenatlas-0.2.0/PKG-INFO
--rw-r--r--   0 tkober     (502) staff       (20)     1113 2022-07-15 11:38:43.000000 wolkenatlas-0.2.0/Readme.md
--rw-r--r--   0 tkober     (502) staff       (20)      730 2023-05-10 09:42:53.000000 wolkenatlas-0.2.0/pyproject.toml
--rw-r--r--   0 tkober     (502) staff       (20)       38 2023-05-10 09:51:37.827403 wolkenatlas-0.2.0/setup.cfg
--rw-r--r--   0 tkober     (502) staff       (20)     3145 2023-05-10 09:42:53.000000 wolkenatlas-0.2.0/setup.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 09:51:37.821869 wolkenatlas-0.2.0/wolkenatlas/
--rw-r--r--   0 tkober     (502) staff       (20)       69 2022-05-13 10:09:18.000000 wolkenatlas-0.2.0/wolkenatlas/__init__.py
--rw-r--r--   0 tkober     (502) staff       (20)     1391 2023-05-10 09:45:02.000000 wolkenatlas-0.2.0/wolkenatlas/constants.py
--rw-r--r--   0 tkober     (502) staff       (20)     6332 2022-05-13 10:09:18.000000 wolkenatlas-0.2.0/wolkenatlas/download.py
--rw-r--r--   0 tkober     (502) staff       (20)     8835 2023-05-10 09:40:56.000000 wolkenatlas-0.2.0/wolkenatlas/embedding.py
--rw-r--r--   0 tkober     (502) staff       (20)     1849 2022-05-16 18:14:21.000000 wolkenatlas-0.2.0/wolkenatlas/encoder.py
--rw-r--r--   0 tkober     (502) staff       (20)     4682 2022-05-18 08:23:47.000000 wolkenatlas-0.2.0/wolkenatlas/preprocessing.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 09:51:37.826399 wolkenatlas-0.2.0/wolkenatlas/util/
--rw-r--r--   0 tkober     (502) staff       (20)        0 2022-05-13 10:09:18.000000 wolkenatlas-0.2.0/wolkenatlas/util/__init__.py
--rw-r--r--   0 tkober     (502) staff       (20)     6219 2023-05-10 09:45:18.000000 wolkenatlas-0.2.0/wolkenatlas/util/data_processing.py
--rw-r--r--   0 tkober     (502) staff       (20)     2249 2022-09-08 14:46:14.000000 wolkenatlas-0.2.0/wolkenatlas/util/file_processing.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 09:51:37.824819 wolkenatlas-0.2.0/wolkenatlas.egg-info/
--rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/PKG-INFO
--rw-r--r--   0 tkober     (502) staff       (20)      516 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/SOURCES.txt
--rw-r--r--   0 tkober     (502) staff       (20)        1 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/dependency_links.txt
--rw-r--r--   0 tkober     (502) staff       (20)       39 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/entry_points.txt
--rw-r--r--   0 tkober     (502) staff       (20)       53 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/requires.txt
--rw-r--r--   0 tkober     (502) staff       (20)       12 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/top_level.txt
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 13:10:20.127932 wolkenatlas-0.2.1/
+-rw-r--r--   0 tkober     (502) staff       (20)     1063 2022-05-13 10:09:18.000000 wolkenatlas-0.2.1/LICENSE
+-rw-r--r--   0 tkober     (502) staff       (20)       58 2022-07-15 11:38:43.000000 wolkenatlas-0.2.1/MANIFEST.in
+-rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-05-10 13:10:20.127679 wolkenatlas-0.2.1/PKG-INFO
+-rw-r--r--   0 tkober     (502) staff       (20)     1113 2022-07-15 11:38:43.000000 wolkenatlas-0.2.1/Readme.md
+-rw-r--r--   0 tkober     (502) staff       (20)      730 2023-05-10 13:10:12.000000 wolkenatlas-0.2.1/pyproject.toml
+-rw-r--r--   0 tkober     (502) staff       (20)       38 2023-05-10 13:10:20.127987 wolkenatlas-0.2.1/setup.cfg
+-rw-r--r--   0 tkober     (502) staff       (20)     3145 2023-05-10 13:10:12.000000 wolkenatlas-0.2.1/setup.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 13:10:20.123055 wolkenatlas-0.2.1/wolkenatlas/
+-rw-r--r--   0 tkober     (502) staff       (20)       69 2022-05-13 10:09:18.000000 wolkenatlas-0.2.1/wolkenatlas/__init__.py
+-rw-r--r--   0 tkober     (502) staff       (20)     1391 2023-05-10 13:05:08.000000 wolkenatlas-0.2.1/wolkenatlas/constants.py
+-rw-r--r--   0 tkober     (502) staff       (20)     6332 2022-05-13 10:09:18.000000 wolkenatlas-0.2.1/wolkenatlas/download.py
+-rw-r--r--   0 tkober     (502) staff       (20)     9321 2023-05-10 13:10:12.000000 wolkenatlas-0.2.1/wolkenatlas/embedding.py
+-rw-r--r--   0 tkober     (502) staff       (20)     1849 2022-05-16 18:14:21.000000 wolkenatlas-0.2.1/wolkenatlas/encoder.py
+-rw-r--r--   0 tkober     (502) staff       (20)     4682 2022-05-18 08:23:47.000000 wolkenatlas-0.2.1/wolkenatlas/preprocessing.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 13:10:20.127023 wolkenatlas-0.2.1/wolkenatlas/util/
+-rw-r--r--   0 tkober     (502) staff       (20)        0 2022-05-13 10:09:18.000000 wolkenatlas-0.2.1/wolkenatlas/util/__init__.py
+-rw-r--r--   0 tkober     (502) staff       (20)     6219 2023-05-10 09:45:18.000000 wolkenatlas-0.2.1/wolkenatlas/util/data_processing.py
+-rw-r--r--   0 tkober     (502) staff       (20)     2249 2022-09-08 14:46:14.000000 wolkenatlas-0.2.1/wolkenatlas/util/file_processing.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 13:10:20.125640 wolkenatlas-0.2.1/wolkenatlas.egg-info/
+-rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-05-10 13:10:20.000000 wolkenatlas-0.2.1/wolkenatlas.egg-info/PKG-INFO
+-rw-r--r--   0 tkober     (502) staff       (20)      516 2023-05-10 13:10:20.000000 wolkenatlas-0.2.1/wolkenatlas.egg-info/SOURCES.txt
+-rw-r--r--   0 tkober     (502) staff       (20)        1 2023-05-10 13:10:20.000000 wolkenatlas-0.2.1/wolkenatlas.egg-info/dependency_links.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       39 2023-05-10 13:10:20.000000 wolkenatlas-0.2.1/wolkenatlas.egg-info/entry_points.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       53 2023-05-10 13:10:20.000000 wolkenatlas-0.2.1/wolkenatlas.egg-info/requires.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       12 2023-05-10 13:10:20.000000 wolkenatlas-0.2.1/wolkenatlas.egg-info/top_level.txt
```

### Comparing `wolkenatlas-0.2.0/LICENSE` & `wolkenatlas-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.0/PKG-INFO` & `wolkenatlas-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolkenatlas
-Version: 0.2.0
+Version: 0.2.1
 Summary: NLP embedding wrapper
 Home-page: https://github.com/tttthomasssss/wolkenatlas
 Author: Thomas Kober
 Author-email: Thomas Kober <tttthomasssss@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Thomas
```

### Comparing `wolkenatlas-0.2.0/Readme.md` & `wolkenatlas-0.2.1/Readme.md`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.0/pyproject.toml` & `wolkenatlas-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wolkenatlas"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Thomas Kober", email="tttthomasssss@gmail.com" },
 ]
 description = "NLP embedding wrapper"
 readme = "Readme.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `wolkenatlas-0.2.0/setup.py` & `wolkenatlas-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
 	name='wolkenatlas',
 
 	# Versions should comply with PEP440.  For a discussion on single-sourcing
 	# the version across setup.py and the project code, see
 	# https://packaging.python.org/en/latest/single_source_version.html
-	version='0.2.0',
+	version='0.2.1',
 
 	description='NLP embedding wrapper',
 	long_description=long_description,
 
 	# The project's main homepage.
 	url='https://github.com/tttthomasssss/wolkenatlas',
```

### Comparing `wolkenatlas-0.2.0/wolkenatlas/constants.py` & `wolkenatlas-0.2.1/wolkenatlas/constants.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.0/wolkenatlas/download.py` & `wolkenatlas-0.2.1/wolkenatlas/download.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.0/wolkenatlas/embedding.py` & `wolkenatlas-0.2.1/wolkenatlas/embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Any, Dict, List, Union
 import logging
+import operator
 import os
+from typing import Any, Dict, List, Union
 
 import numpy as np
 
 from wolkenatlas import constants
 from wolkenatlas.util import data_processing
 from wolkenatlas.util import file_processing
 
@@ -148,40 +149,53 @@
 
     def __getitem__(self, word, default=None):
         return self.fn_getitem_(word=word, default=default)
 
     def _getitem_multi_embeddings(self, word, default=None):
         default = default or self.oov_
 
-        if word not in self.inverted_index_:
-            d = {
+        multi_key_request = isinstance(word, tuple)
+        if not multi_key_request and word not in self.inverted_index_:
+            data = {
                 constants.INPUT_IDS_KEY: default,
                 constants.ATTENTION_MASK_KEY: default
             }
             if self.vector_space_.shape[-1] == 3:
-                d[constants.TOKEN_TYPE_IDS_KEY] = default
-            return d
+                data[constants.TOKEN_TYPE_IDS_KEY] = default
+            return data
+
+        if multi_key_request:
+            word_idx = np.array(operator.itemgetter(*word)(self.inverted_index_))
+        else:
+            word_idx = self.inverted_index_[word]
 
-        word_idx = self.inverted_index_[word]
-        d = {
+        data = {
             constants.INPUT_IDS_KEY: self.vector_space_[word_idx, :, constants.INPUT_IDS_INDEX],
             constants.ATTENTION_MASK_KEY: self.vector_space_[word_idx, :, constants.ATTENTION_MASK_INDEX]
         }
         if self.vector_space_.shape[-1] == 3:
-            d[constants.TOKEN_TYPE_IDS_KEY] = self.vector_space_[word_idx, :, constants.TOKEN_TYPE_IDS_INDEX]
+            data[constants.TOKEN_TYPE_IDS_KEY] = self.vector_space_[word_idx, :, constants.TOKEN_TYPE_IDS_INDEX]
 
-        return d
+        return data
 
     def _getitem_single_embedding(self, word, default=None):
         default = default or self.oov_
 
-        if word not in self.inverted_index_:
+        multi_key_request = isinstance(word, tuple)
+
+        if not multi_key_request and word not in self.inverted_index_:
             return default
 
-        return self.vector_space_[self.inverted_index_[word]]
+        if multi_key_request:
+            word_idx = np.array(operator.itemgetter(*word)(self.inverted_index_))
+        else:
+            word_idx = self.inverted_index_[word]
+
+        return self.vector_space_[word_idx]
+    
     @property
     def dimensionality(self):
         return self.dimensionality_
 
     @property
     def vocab_size(self):
         return self.vector_space_.shape[0]
```

### Comparing `wolkenatlas-0.2.0/wolkenatlas/encoder.py` & `wolkenatlas-0.2.1/wolkenatlas/encoder.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.0/wolkenatlas/preprocessing.py` & `wolkenatlas-0.2.1/wolkenatlas/preprocessing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.0/wolkenatlas/util/data_processing.py` & `wolkenatlas-0.2.1/wolkenatlas/util/data_processing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.0/wolkenatlas/util/file_processing.py` & `wolkenatlas-0.2.1/wolkenatlas/util/file_processing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.2.0/wolkenatlas.egg-info/PKG-INFO` & `wolkenatlas-0.2.1/wolkenatlas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolkenatlas
-Version: 0.2.0
+Version: 0.2.1
 Summary: NLP embedding wrapper
 Home-page: https://github.com/tttthomasssss/wolkenatlas
 Author: Thomas Kober
 Author-email: Thomas Kober <tttthomasssss@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Thomas
```

### Comparing `wolkenatlas-0.2.0/wolkenatlas.egg-info/SOURCES.txt` & `wolkenatlas-0.2.1/wolkenatlas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

