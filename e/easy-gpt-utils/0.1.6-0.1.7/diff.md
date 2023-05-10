# Comparing `tmp/easy_gpt_utils-0.1.6.tar.gz` & `tmp/easy_gpt_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gpt_utils-0.1.6.tar", last modified: Wed May 10 03:19:20 2023, max compression
+gzip compressed data, was "easy_gpt_utils-0.1.7.tar", last modified: Wed May 10 03:33:05 2023, max compression
```

## Comparing `easy_gpt_utils-0.1.6.tar` & `easy_gpt_utils-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:19:20.319657 easy_gpt_utils-0.1.6/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)    11357 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.6/LICENSE
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 03:19:20.318657 easy_gpt_utils-0.1.6/PKG-INFO
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      156 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.6/README.md
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:19:20.311657 easy_gpt_utils-0.1.6/easy_gpt_utils/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      130 2023-05-10 03:18:02.000000 easy_gpt_utils-0.1.6/easy_gpt_utils/__init__.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)     4061 2023-05-09 03:39:40.000000 easy_gpt_utils-0.1.6/easy_gpt_utils/embedding.py
--rw-r--r--   0 houwei    (1001) houwei    (1001)    40471 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.6/easy_gpt_utils/gpt.py
--rw-rw-r--   0 houwei    (1001) houwei    (1001)     4993 2023-05-09 09:03:55.000000 easy_gpt_utils-0.1.6/easy_gpt_utils/vector_database.py
-drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:19:20.317657 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/PKG-INFO
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      326 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)        1 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       22 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/requires.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       15 2023-05-10 03:19:20.000000 easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/top_level.txt
--rw-rw-r--   0 houwei    (1001) houwei    (1001)       38 2023-05-10 03:19:20.319657 easy_gpt_utils-0.1.6/setup.cfg
--rw-rw-r--   0 houwei    (1001) houwei    (1001)      803 2023-05-10 03:19:05.000000 easy_gpt_utils-0.1.6/setup.py
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:33:05.128967 easy_gpt_utils-0.1.7/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)    11357 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.7/LICENSE
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 03:33:05.128967 easy_gpt_utils-0.1.7/PKG-INFO
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      156 2023-05-08 01:56:20.000000 easy_gpt_utils-0.1.7/README.md
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:33:05.118967 easy_gpt_utils-0.1.7/easy_gpt_utils/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      130 2023-05-10 03:18:02.000000 easy_gpt_utils-0.1.7/easy_gpt_utils/__init__.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)     4061 2023-05-09 03:39:40.000000 easy_gpt_utils-0.1.7/easy_gpt_utils/embedding.py
+-rw-r--r--   0 houwei    (1001) houwei    (1001)    40471 2023-05-08 01:57:00.000000 easy_gpt_utils-0.1.7/easy_gpt_utils/gpt.py
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)     5309 2023-05-10 03:32:16.000000 easy_gpt_utils-0.1.7/easy_gpt_utils/vector_database.py
+drwxrwxr-x   0 houwei    (1001) houwei    (1001)        0 2023-05-10 03:33:05.127967 easy_gpt_utils-0.1.7/easy_gpt_utils.egg-info/
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      761 2023-05-10 03:33:04.000000 easy_gpt_utils-0.1.7/easy_gpt_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      326 2023-05-10 03:33:04.000000 easy_gpt_utils-0.1.7/easy_gpt_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)        1 2023-05-10 03:33:04.000000 easy_gpt_utils-0.1.7/easy_gpt_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       22 2023-05-10 03:33:04.000000 easy_gpt_utils-0.1.7/easy_gpt_utils.egg-info/requires.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       15 2023-05-10 03:33:04.000000 easy_gpt_utils-0.1.7/easy_gpt_utils.egg-info/top_level.txt
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)       38 2023-05-10 03:33:05.128967 easy_gpt_utils-0.1.7/setup.cfg
+-rw-rw-r--   0 houwei    (1001) houwei    (1001)      803 2023-05-10 03:32:29.000000 easy_gpt_utils-0.1.7/setup.py
```

### Comparing `easy_gpt_utils-0.1.6/LICENSE` & `easy_gpt_utils-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.6/PKG-INFO` & `easy_gpt_utils-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_gpt_utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easy GPT utils include 1. chat completion 2. embedding and 3. vector database
 Home-page: https://github.com/ark338/easy_gpt_utils
 Author: Hou Wei
 Author-email: messenger929@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `easy_gpt_utils-0.1.6/easy_gpt_utils/embedding.py` & `easy_gpt_utils-0.1.7/easy_gpt_utils/embedding.py`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.6/easy_gpt_utils/gpt.py` & `easy_gpt_utils-0.1.7/easy_gpt_utils/gpt.py`

 * *Files identical despite different names*

### Comparing `easy_gpt_utils-0.1.6/easy_gpt_utils/vector_database.py` & `easy_gpt_utils-0.1.7/easy_gpt_utils/vector_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pinecone
-from embedding import Embedding
 import uuid
 from enum import Enum
 from typing import Union, List, Tuple, Optional, Dict, Any
 
 # namespaces
 class NamesSpaces(Enum):
     Glossary = 'Glossary'
@@ -82,33 +81,41 @@
               vector: Optional[List[float]] = None, 
               id: Optional[str] = None,
               filter: Optional[Dict[str, Union[str, float, int, bool, List, dict]]] = None):
         return [{'score':result['score'], 'metadata': result['metadata']} for result in 
             self.index.query(namespace = namespace, top_k = top_k, vector=vector, id=id, filter=filter, include_metadata=True)['matches'] if result['score'] > threshold]
 
 
-testcase = [
-'withstand voltage	耐压',
-'fingerprint U-lock	指纹U型锁',
-'No rider detected	未触发站人模式'
-]
-
-embedding_instance = Embedding()
-
-my_pinecone = Pinecone(index = 'segway-knowledge-base', environment='asia-southeast1-gcp')
-#print ("delete", my_pinecone.delete(namespace = NamesSpaces.Glossary.value, ids = ['id0']))
-#print ("my_pinecone: ", my_pinecone.fetch(namespace = NamesSpaces.Glossary.value, ids = ['id0', 'id1']))
-#print ("update test", my_pinecone.update(namespace = NamesSpaces.Glossary.value, id = 'id0', metadata = {'category': 'nihkao'}))
-#print ("delete all", my_pinecone.delete(namespace = NamesSpaces.Glossary.value, deleteAll = 'true'))
-
-if False:
-    vectors = [vector for vector in [embedding_instance.get_raw_embedding(item) for item in testcase]]
-    metas = [create_meta("Glossary", item, url = "https://www.segway.com.cn/", label = ["Glossary"]) for item in testcase]
-    ids = [str('id' + str(id)) for id in range(len(testcase))]
+# TODO: test code should move to unit test
+define_test = False
+if define_test:
+    try:
+        from .embedding import Embedding  # for when the module is imported
+    except ImportError:
+        from embedding import Embedding  # for when the module is run directly
+
+    testcase = [
+    'withstand voltage	耐压',
+    'fingerprint U-lock	指纹U型锁',
+    'No rider detected	未触发站人模式'
+    ]
+
+    embedding_instance = Embedding()
+
+    my_pinecone = Pinecone(index = 'segway-knowledge-base', environment='asia-southeast1-gcp')
+    #print ("delete", my_pinecone.delete(namespace = NamesSpaces.Glossary.value, ids = ['id0']))
+    #print ("my_pinecone: ", my_pinecone.fetch(namespace = NamesSpaces.Glossary.value, ids = ['id0', 'id1']))
+    #print ("update test", my_pinecone.update(namespace = NamesSpaces.Glossary.value, id = 'id0', metadata = {'category': 'nihkao'}))
+    #print ("delete all", my_pinecone.delete(namespace = NamesSpaces.Glossary.value, deleteAll = 'true'))
+
+    if False:
+        vectors = [vector for vector in [embedding_instance.get_raw_embedding(item) for item in testcase]]
+        metas = [create_meta("Glossary", item, url = "https://www.segway.com.cn/", label = ["Glossary"]) for item in testcase]
+        ids = [str('id' + str(id)) for id in range(len(testcase))]
 
-    to_upsert = list(zip(ids, vectors, metas))
+        to_upsert = list(zip(ids, vectors, metas))
 
-    my_pinecone.upsert(namespace = NamesSpaces.Glossary.value, items = to_upsert)
-    print ("my_pinecone: ", my_pinecone.fetch(namespace = NamesSpaces.Glossary.value, ids = ['id0', 'id1']))
+        my_pinecone.upsert(namespace = NamesSpaces.Glossary.value, items = to_upsert)
+        print ("my_pinecone: ", my_pinecone.fetch(namespace = NamesSpaces.Glossary.value, ids = ['id0', 'id1']))
 
-embe = embedding_instance.get_raw_embedding("withstand voltage")
-print ("querytest: ", my_pinecone.query_meta(namespace = NamesSpaces.Glossary.value, threshold = 0.8, vector = embe, top_k = 5))
+    embe = embedding_instance.get_raw_embedding("withstand voltage")
+    print ("querytest: ", my_pinecone.query_meta(namespace = NamesSpaces.Glossary.value, threshold = 0.8, vector = embe, top_k = 5))
```

### Comparing `easy_gpt_utils-0.1.6/easy_gpt_utils.egg-info/PKG-INFO` & `easy_gpt_utils-0.1.7/easy_gpt_utils.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-gpt-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easy GPT utils include 1. chat completion 2. embedding and 3. vector database
 Home-page: https://github.com/ark338/easy_gpt_utils
 Author: Hou Wei
 Author-email: messenger929@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `easy_gpt_utils-0.1.6/setup.py` & `easy_gpt_utils-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="easy_gpt_utils",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=[
         "openai",
         "tiktoken",
         "numpy"
     ],
     author="Hou Wei",
```

