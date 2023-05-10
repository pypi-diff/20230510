# Comparing `tmp/wolkenatlas-0.1.6.tar.gz` & `tmp/wolkenatlas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolkenatlas-0.1.6.tar", last modified: Mon Sep 12 12:35:07 2022, max compression
+gzip compressed data, was "wolkenatlas-0.2.0.tar", last modified: Wed May 10 09:51:37 2023, max compression
```

## Comparing `wolkenatlas-0.1.6.tar` & `wolkenatlas-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2022-09-12 12:35:07.009639 wolkenatlas-0.1.6/
--rw-r--r--   0 tkober     (502) staff       (20)     1063 2022-05-13 10:09:18.000000 wolkenatlas-0.1.6/LICENSE
--rw-r--r--   0 tkober     (502) staff       (20)       58 2022-07-15 11:38:43.000000 wolkenatlas-0.1.6/MANIFEST.in
--rw-r--r--   0 tkober     (502) staff       (20)     3229 2022-09-12 12:35:07.009382 wolkenatlas-0.1.6/PKG-INFO
--rw-r--r--   0 tkober     (502) staff       (20)     1113 2022-07-15 11:38:43.000000 wolkenatlas-0.1.6/Readme.md
--rw-r--r--   0 tkober     (502) staff       (20)      730 2022-09-12 12:33:45.000000 wolkenatlas-0.1.6/pyproject.toml
--rw-r--r--   0 tkober     (502) staff       (20)       38 2022-09-12 12:35:07.009696 wolkenatlas-0.1.6/setup.cfg
--rw-r--r--   0 tkober     (502) staff       (20)     3145 2022-09-12 12:33:45.000000 wolkenatlas-0.1.6/setup.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2022-09-12 12:35:07.005892 wolkenatlas-0.1.6/wolkenatlas/
--rw-r--r--   0 tkober     (502) staff       (20)       69 2022-05-13 10:09:18.000000 wolkenatlas-0.1.6/wolkenatlas/__init__.py
--rw-r--r--   0 tkober     (502) staff       (20)     1215 2022-09-08 14:46:14.000000 wolkenatlas-0.1.6/wolkenatlas/constants.py
--rw-r--r--   0 tkober     (502) staff       (20)     6332 2022-05-13 10:09:18.000000 wolkenatlas-0.1.6/wolkenatlas/download.py
--rw-r--r--   0 tkober     (502) staff       (20)     7117 2022-09-08 14:46:14.000000 wolkenatlas-0.1.6/wolkenatlas/embedding.py
--rw-r--r--   0 tkober     (502) staff       (20)     1849 2022-05-16 18:14:21.000000 wolkenatlas-0.1.6/wolkenatlas/encoder.py
--rw-r--r--   0 tkober     (502) staff       (20)     4682 2022-05-18 08:23:47.000000 wolkenatlas-0.1.6/wolkenatlas/preprocessing.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2022-09-12 12:35:07.008908 wolkenatlas-0.1.6/wolkenatlas/util/
--rw-r--r--   0 tkober     (502) staff       (20)        0 2022-05-13 10:09:18.000000 wolkenatlas-0.1.6/wolkenatlas/util/__init__.py
--rw-r--r--   0 tkober     (502) staff       (20)     6219 2022-09-08 14:46:14.000000 wolkenatlas-0.1.6/wolkenatlas/util/data_processing.py
--rw-r--r--   0 tkober     (502) staff       (20)     2249 2022-09-08 14:46:14.000000 wolkenatlas-0.1.6/wolkenatlas/util/file_processing.py
-drwxr-xr-x   0 tkober     (502) staff       (20)        0 2022-09-12 12:35:07.007895 wolkenatlas-0.1.6/wolkenatlas.egg-info/
--rw-r--r--   0 tkober     (502) staff       (20)     3229 2022-09-12 12:35:06.000000 wolkenatlas-0.1.6/wolkenatlas.egg-info/PKG-INFO
--rw-r--r--   0 tkober     (502) staff       (20)      516 2022-09-12 12:35:07.000000 wolkenatlas-0.1.6/wolkenatlas.egg-info/SOURCES.txt
--rw-r--r--   0 tkober     (502) staff       (20)        1 2022-09-12 12:35:06.000000 wolkenatlas-0.1.6/wolkenatlas.egg-info/dependency_links.txt
--rw-r--r--   0 tkober     (502) staff       (20)       39 2022-09-12 12:35:06.000000 wolkenatlas-0.1.6/wolkenatlas.egg-info/entry_points.txt
--rw-r--r--   0 tkober     (502) staff       (20)       53 2022-09-12 12:35:06.000000 wolkenatlas-0.1.6/wolkenatlas.egg-info/requires.txt
--rw-r--r--   0 tkober     (502) staff       (20)       12 2022-09-12 12:35:06.000000 wolkenatlas-0.1.6/wolkenatlas.egg-info/top_level.txt
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 09:51:37.827349 wolkenatlas-0.2.0/
+-rw-r--r--   0 tkober     (502) staff       (20)     1063 2022-05-13 10:09:18.000000 wolkenatlas-0.2.0/LICENSE
+-rw-r--r--   0 tkober     (502) staff       (20)       58 2022-07-15 11:38:43.000000 wolkenatlas-0.2.0/MANIFEST.in
+-rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-05-10 09:51:37.827122 wolkenatlas-0.2.0/PKG-INFO
+-rw-r--r--   0 tkober     (502) staff       (20)     1113 2022-07-15 11:38:43.000000 wolkenatlas-0.2.0/Readme.md
+-rw-r--r--   0 tkober     (502) staff       (20)      730 2023-05-10 09:42:53.000000 wolkenatlas-0.2.0/pyproject.toml
+-rw-r--r--   0 tkober     (502) staff       (20)       38 2023-05-10 09:51:37.827403 wolkenatlas-0.2.0/setup.cfg
+-rw-r--r--   0 tkober     (502) staff       (20)     3145 2023-05-10 09:42:53.000000 wolkenatlas-0.2.0/setup.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 09:51:37.821869 wolkenatlas-0.2.0/wolkenatlas/
+-rw-r--r--   0 tkober     (502) staff       (20)       69 2022-05-13 10:09:18.000000 wolkenatlas-0.2.0/wolkenatlas/__init__.py
+-rw-r--r--   0 tkober     (502) staff       (20)     1391 2023-05-10 09:45:02.000000 wolkenatlas-0.2.0/wolkenatlas/constants.py
+-rw-r--r--   0 tkober     (502) staff       (20)     6332 2022-05-13 10:09:18.000000 wolkenatlas-0.2.0/wolkenatlas/download.py
+-rw-r--r--   0 tkober     (502) staff       (20)     8835 2023-05-10 09:40:56.000000 wolkenatlas-0.2.0/wolkenatlas/embedding.py
+-rw-r--r--   0 tkober     (502) staff       (20)     1849 2022-05-16 18:14:21.000000 wolkenatlas-0.2.0/wolkenatlas/encoder.py
+-rw-r--r--   0 tkober     (502) staff       (20)     4682 2022-05-18 08:23:47.000000 wolkenatlas-0.2.0/wolkenatlas/preprocessing.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 09:51:37.826399 wolkenatlas-0.2.0/wolkenatlas/util/
+-rw-r--r--   0 tkober     (502) staff       (20)        0 2022-05-13 10:09:18.000000 wolkenatlas-0.2.0/wolkenatlas/util/__init__.py
+-rw-r--r--   0 tkober     (502) staff       (20)     6219 2023-05-10 09:45:18.000000 wolkenatlas-0.2.0/wolkenatlas/util/data_processing.py
+-rw-r--r--   0 tkober     (502) staff       (20)     2249 2022-09-08 14:46:14.000000 wolkenatlas-0.2.0/wolkenatlas/util/file_processing.py
+drwxr-xr-x   0 tkober     (502) staff       (20)        0 2023-05-10 09:51:37.824819 wolkenatlas-0.2.0/wolkenatlas.egg-info/
+-rw-r--r--   0 tkober     (502) staff       (20)     3229 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/PKG-INFO
+-rw-r--r--   0 tkober     (502) staff       (20)      516 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/SOURCES.txt
+-rw-r--r--   0 tkober     (502) staff       (20)        1 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/dependency_links.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       39 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/entry_points.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       53 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/requires.txt
+-rw-r--r--   0 tkober     (502) staff       (20)       12 2023-05-10 09:51:37.000000 wolkenatlas-0.2.0/wolkenatlas.egg-info/top_level.txt
```

### Comparing `wolkenatlas-0.1.6/LICENSE` & `wolkenatlas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.1.6/PKG-INFO` & `wolkenatlas-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolkenatlas
-Version: 0.1.6
+Version: 0.2.0
 Summary: NLP embedding wrapper
 Home-page: https://github.com/tttthomasssss/wolkenatlas
 Author: Thomas Kober
 Author-email: Thomas Kober <tttthomasssss@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Thomas
```

### Comparing `wolkenatlas-0.1.6/Readme.md` & `wolkenatlas-0.2.0/Readme.md`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.1.6/pyproject.toml` & `wolkenatlas-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wolkenatlas"
-version = "0.1.6"
+version = "0.2.0"
 authors = [
   { name="Thomas Kober", email="tttthomasssss@gmail.com" },
 ]
 description = "NLP embedding wrapper"
 readme = "Readme.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `wolkenatlas-0.1.6/setup.py` & `wolkenatlas-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
 	name='wolkenatlas',
 
 	# Versions should comply with PEP440.  For a discussion on single-sourcing
 	# the version across setup.py and the project code, see
 	# https://packaging.python.org/en/latest/single_source_version.html
-	version='0.1.6',
+	version='0.2.0',
 
 	description='NLP embedding wrapper',
 	long_description=long_description,
 
 	# The project's main homepage.
 	url='https://github.com/tttthomasssss/wolkenatlas',
```

### Comparing `wolkenatlas-0.1.6/wolkenatlas/constants.py` & `wolkenatlas-0.2.0/wolkenatlas/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,50 @@
-VECTORS_FILENAME_HDF = 'X.hdf'
-VECTORS_FILENAME_NPY = 'X.npy'
-INVERTED_INDEX_FILENAME = 'inverted_index.json'
+VECTORS_FILENAME_HDF = "X.hdf"
+VECTORS_FILENAME_NPY = "X.npy"
+INVERTED_INDEX_FILENAME = "inverted_index.json"
+
+INPUT_IDS_KEY = "input_ids"
+TOKEN_TYPE_IDS_KEY = "token_type_ids"
+ATTENTION_MASK_KEY = "attention_mask"
+
+INPUT_IDS_INDEX = 0
+TOKEN_TYPE_IDS_INDEX = 2
+ATTENTION_MASK_INDEX = 1
 
 FILE_TYPE_MAP = {
-    '.txt': 'text',
-    '.bin': 'binary',
-    '.tgz': 'archive',
-    '.tar.gz': 'archive',
-    '.gz': 'archive'
+    ".txt": "text",
+    ".bin": "binary",
+    ".tgz": "archive",
+    ".tar.gz": "archive",
+    ".gz": "archive"
 }
 
 COMPOSITION_FUNCTION_DIM_MULTIPLIER = {
-    'sum': 1,
-    'average': 1,
-    'max': 1,
-    'concatenate_average_max': 2,
-    'concatenate_sum_max': 2,
-    'concatenate_average_min': 2,
-    'concatenate_sum_min': 2,
-    'concatenate_min_max': 2
+    "sum": 1,
+    "average": 1,
+    "max": 1,
+    "concatenate_average_max": 2,
+    "concatenate_sum_max": 2,
+    "concatenate_average_min": 2,
+    "concatenate_sum_min": 2,
+    "concatenate_min_max": 2
 }
 
-FASTTEXT_CC_URL = 'https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/'
-FASTTEXT_WIKI_URL = 'https://dl.fbaipublicfiles.com/fasttext/vectors-wiki/'
-FASTTEXT_ALIGNED_URL = 'https://dl.fbaipublicfiles.com/fasttext/vectors-aligned/'
-
-FASTTEXT_CC_VECTOR_NAME_TEMPLATE = 'cc.{}.300.vec.gz'
-FASTTEXT_WIKI_VECTOR_NAME_TEMPLATE = 'wiki.{}.vec'
-FASTTEXT_ALIGNED_VECTOR_NAME_TEMPLATE = 'wiki.{}.align.vec'
+FASTTEXT_CC_URL = "https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/"
+FASTTEXT_WIKI_URL = "https://dl.fbaipublicfiles.com/fasttext/vectors-wiki/"
+FASTTEXT_ALIGNED_URL = "https://dl.fbaipublicfiles.com/fasttext/vectors-aligned/"
+
+FASTTEXT_CC_VECTOR_NAME_TEMPLATE = "cc.{}.300.vec.gz"
+FASTTEXT_WIKI_VECTOR_NAME_TEMPLATE = "wiki.{}.vec"
+FASTTEXT_ALIGNED_VECTOR_NAME_TEMPLATE = "wiki.{}.align.vec"
 
 FASTTEXT_TRAINING_CORPUS_URL_MAP = {
-    'cc': FASTTEXT_CC_URL,
-    'wiki': FASTTEXT_WIKI_URL,
-    'aligned': FASTTEXT_ALIGNED_URL
+    "cc": FASTTEXT_CC_URL,
+    "wiki": FASTTEXT_WIKI_URL,
+    "aligned": FASTTEXT_ALIGNED_URL
 }
 
 FASTTEXT_TRAINING_CORPUS_VECTOR_NAME_MAP = {
-    'cc': FASTTEXT_CC_VECTOR_NAME_TEMPLATE,
-    'wiki': FASTTEXT_WIKI_VECTOR_NAME_TEMPLATE,
-    'aligned': FASTTEXT_ALIGNED_VECTOR_NAME_TEMPLATE
+    "cc": FASTTEXT_CC_VECTOR_NAME_TEMPLATE,
+    "wiki": FASTTEXT_WIKI_VECTOR_NAME_TEMPLATE,
+    "aligned": FASTTEXT_ALIGNED_VECTOR_NAME_TEMPLATE
 }
```

### Comparing `wolkenatlas-0.1.6/wolkenatlas/download.py` & `wolkenatlas-0.2.0/wolkenatlas/download.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.1.6/wolkenatlas/embedding.py` & `wolkenatlas-0.2.0/wolkenatlas/embedding.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,33 @@
 
 from wolkenatlas import constants
 from wolkenatlas.util import data_processing
 from wolkenatlas.util import file_processing
 
 
 class Embedding:
-    def __init__(self, inverted_index: Dict[str, int], vector_space: np.ndarray, **kwargs: Any):
+    def __init__(
+            self,
+            inverted_index: Dict[str, int],
+            vector_space: Union[np.ndarray, Dict[str, np.ndarray]],
+            **kwargs: Any
+    ):
         self.inverted_index_ = inverted_index
-        self.vector_space_ = vector_space
+        if isinstance(vector_space, dict):
+            vector_stack = np.dstack((vector_space["input_ids"], vector_space["attention_mask"]))
+            if vector_stack.shape[-1] > 2:
+                vector_stack = np.dstack((vector_stack, vector_space["token_type_ids"]))
+            self.vector_space_ = vector_stack
+
+            self.fn_getitem_ = self._getitem_multi_embeddings
+        else:
+            self.vector_space_ = vector_space
+
+            self.fn_getitem_ = self._getitem_single_embedding
+
         self.index_ = None
         self.random_state_ = np.random.RandomState(kwargs.get("random_seed", 29306))
         self.character_embeddings_ = kwargs.pop("character_embeddings", False)
 
         if kwargs.pop('should_finalize', True):
             self._finalize(**kwargs)
 
@@ -65,14 +81,18 @@
     def _load_from_file(model_file: str, **kwargs: Any) -> "Embedding":
         emb = Embedding._empty()
 
         if data_processing.check_is_wolkenatlas(model_file):
             emb.inverted_index_ = file_processing.load_json(os.path.join(model_file,
                                                                          constants.INVERTED_INDEX_FILENAME))
             emb.vector_space_ = file_processing.load_vector_space(model_file)
+            if emb.vector_space_.ndim > 2:
+                emb.fn_getitem_ = emb._getitem_multi_embeddings
+            else:
+                emb.fn_getitem_ = emb._getitem_single_embedding
         else:
             file_type = kwargs.pop('file_type', None)
 
             if file_type is None:
                 ext = os.path.splitext(model_file)[1]
                 if ext not in ['.txt', '.bin', '.tgz', '.tar.gz', '.gz']:
                     raise ValueError(f'Need to specify "file_type" (e.g. "text" or "binary") if you are not '
@@ -123,21 +143,45 @@
     def __contains__(self, word):
         return word in self.inverted_index_
 
     def __index__(self, word):
         return self.inverted_index_[word]
 
     def __getitem__(self, word, default=None):
+        return self.fn_getitem_(word=word, default=default)
+
+    def _getitem_multi_embeddings(self, word, default=None):
+        default = default or self.oov_
+
+        if word not in self.inverted_index_:
+            d = {
+                constants.INPUT_IDS_KEY: default,
+                constants.ATTENTION_MASK_KEY: default
+            }
+            if self.vector_space_.shape[-1] == 3:
+                d[constants.TOKEN_TYPE_IDS_KEY] = default
+            return d
+
+        word_idx = self.inverted_index_[word]
+        d = {
+            constants.INPUT_IDS_KEY: self.vector_space_[word_idx, :, constants.INPUT_IDS_INDEX],
+            constants.ATTENTION_MASK_KEY: self.vector_space_[word_idx, :, constants.ATTENTION_MASK_INDEX]
+        }
+        if self.vector_space_.shape[-1] == 3:
+            d[constants.TOKEN_TYPE_IDS_KEY] = self.vector_space_[word_idx, :, constants.TOKEN_TYPE_IDS_INDEX]
+
+        return d
+
+    def _getitem_single_embedding(self, word, default=None):
         default = default or self.oov_
 
         if word not in self.inverted_index_:
             return default
 
         return self.vector_space_[self.inverted_index_[word]]
-
     @property
     def dimensionality(self):
         return self.dimensionality_
 
     @property
     def vocab_size(self):
         return self.vector_space_.shape[0]
```

### Comparing `wolkenatlas-0.1.6/wolkenatlas/encoder.py` & `wolkenatlas-0.2.0/wolkenatlas/encoder.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.1.6/wolkenatlas/preprocessing.py` & `wolkenatlas-0.2.0/wolkenatlas/preprocessing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.1.6/wolkenatlas/util/data_processing.py` & `wolkenatlas-0.2.0/wolkenatlas/util/data_processing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.1.6/wolkenatlas/util/file_processing.py` & `wolkenatlas-0.2.0/wolkenatlas/util/file_processing.py`

 * *Files identical despite different names*

### Comparing `wolkenatlas-0.1.6/wolkenatlas.egg-info/PKG-INFO` & `wolkenatlas-0.2.0/wolkenatlas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolkenatlas
-Version: 0.1.6
+Version: 0.2.0
 Summary: NLP embedding wrapper
 Home-page: https://github.com/tttthomasssss/wolkenatlas
 Author: Thomas Kober
 Author-email: Thomas Kober <tttthomasssss@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Thomas
```

### Comparing `wolkenatlas-0.1.6/wolkenatlas.egg-info/SOURCES.txt` & `wolkenatlas-0.2.0/wolkenatlas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

