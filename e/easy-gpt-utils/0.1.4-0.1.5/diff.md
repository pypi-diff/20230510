# Comparing `tmp/easy_gpt_utils-0.1.4.tar.gz` & `tmp/easy_gpt_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gpt_utils-0.1.4.tar", last modified: Mon May  8 02:23:13 2023, max compression
+gzip compressed data, was "easy_gpt_utils-0.1.5.tar", last modified: Wed May 10 01:37:35 2023, max compression
```

## Comparing `easy_gpt_utils-0.1.4.tar` & `easy_gpt_utils-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-08 02:23:13.907361 easy_gpt_utils-0.1.4/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)    11357 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.4/LICENSE
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-08 02:23:13.907361 easy_gpt_utils-0.1.4/PKG-INFO
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      156 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.4/README.md
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-08 02:23:13.894361 easy_gpt_utils-0.1.4/easy_gpt_utils/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       53 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.4/easy_gpt_utils/__init__.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)     3880 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.4/easy_gpt_utils/embedding.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)    40471 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.4/easy_gpt_utils/gpt.py
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-08 02:23:13.906361 easy_gpt_utils-0.1.4/easy_gpt_utils.egg-info/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-08 02:23:13.000000 easy_gpt_utils-0.1.4/easy_gpt_utils.egg-info/PKG-INFO
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      292 2023-05-08 02:23:13.000000 easy_gpt_utils-0.1.4/easy_gpt_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)        1 2023-05-08 02:23:13.000000 easy_gpt_utils-0.1.4/easy_gpt_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       22 2023-05-08 02:23:13.000000 easy_gpt_utils-0.1.4/easy_gpt_utils.egg-info/requires.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       15 2023-05-08 02:23:13.000000 easy_gpt_utils-0.1.4/easy_gpt_utils.egg-info/top_level.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       38 2023-05-08 02:23:13.908361 easy_gpt_utils-0.1.4/setup.cfg
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      803 2023-05-08 02:22:57.000000 easy_gpt_utils-0.1.4/setup.py
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 01:37:35.312805 easy_gpt_utils-0.1.5/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)    11357 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.5/LICENSE
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 01:37:35.312805 easy_gpt_utils-0.1.5/PKG-INFO
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      156 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.5/README.md
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 01:37:35.304805 easy_gpt_utils-0.1.5/easy_gpt_utils/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       53 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.5/easy_gpt_utils/__init__.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)     4061 2023-05-09 03:39:40.000000 easy_gpt_utils-0.1.5/easy_gpt_utils/embedding.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)    40471 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.5/easy_gpt_utils/gpt.py
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)     4993 2023-05-09 09:03:55.000000 easy_gpt_utils-0.1.5/easy_gpt_utils/vector_database.py
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 01:37:35.311805 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      326 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)        1 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       22 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/requires.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       15 2023-05-10 01:37:35.000000 easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/top_level.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       38 2023-05-10 01:37:35.313805 easy_gpt_utils-0.1.5/setup.cfg
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      803 2023-05-10 01:36:25.000000 easy_gpt_utils-0.1.5/setup.py
```

### Comparing `easy_gpt_utils-0.1.4/LICENSE` & `easy_gpt_utils-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.4/PKG-INFO` & `easy_gpt_utils-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_gpt_utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy GPT utils include 1. chat completion 2. embedding and 3. vector database
 Home-page: https://github.com/ark338/easy_gpt_utils
 Author: Hou Wei
 Author-email: messenger929@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `easy_gpt_utils-0.1.4/easy_gpt_utils/embedding.py` & `easy_gpt_utils-0.1.5/easy_gpt_utils/embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     def get_embedding(self, input_text_list):
         # if input_text_list is not a list throw an exception
         if not isinstance(input_text_list, list):
             raise TypeError("input_text_list should be a list")
 
         embedding = openai.Embedding.create(model=self.model, input=input_text_list)
         return [(text, data.embedding) for text, data in zip(input_text_list, embedding.data)], embedding.usage.total_tokens
+
+    def get_raw_embedding(self, raw_text: str):
+        embedding = openai.Embedding.create(model=self.model, input=raw_text)
+        return list(embedding.data[0].embedding)
     
     def create_embeddings(self, input_text_list):
         # if input_text_list is not a list throw an exception
         if not isinstance(input_text_list, list):
             raise TypeError("input_text_list should be a list")
 
         result = []
@@ -51,15 +55,15 @@
 
         if query_len > 0:
             ebd, tk = self.get_embedding(input_text_list[start_index:])
             tokens += tk
             result.extend(ebd)
         return result, tokens
 
-    def create_embeddings_from_text(self, text):
+    def create_embeddings_from_text(self, text: str):
         # if text is not a string throw an exception
         if not isinstance(text, str):
             raise TypeError("text should be a string")
 
         return self.create_embeddings([text.strip() for text in text.splitlines() if text.strip()])
 
     def create_embedding_from_file(self, input_file, output_file= None):
```

### Comparing `easy_gpt_utils-0.1.4/easy_gpt_utils/gpt.py` & `easy_gpt_utils-0.1.5/easy_gpt_utils/gpt.py`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.4/easy_gpt_utils.egg-info/PKG-INFO` & `easy_gpt_utils-0.1.5/easy_gpt_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-gpt-utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy GPT utils include 1. chat completion 2. embedding and 3. vector database
 Home-page: https://github.com/ark338/easy_gpt_utils
 Author: Hou Wei
 Author-email: messenger929@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `easy_gpt_utils-0.1.4/setup.py` & `easy_gpt_utils-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="easy_gpt_utils",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         "openai",
         "tiktoken",
         "numpy"
     ],
     author="Hou Wei",
```

