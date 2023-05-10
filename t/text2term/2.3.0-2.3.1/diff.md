# Comparing `tmp/text2term-2.3.0.tar.gz` & `tmp/text2term-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2term-2.3.0.tar", last modified: Thu May  4 15:09:44 2023, max compression
+gzip compressed data, was "text2term-2.3.1.tar", last modified: Wed May 10 16:24:55 2023, max compression
```

## Comparing `text2term-2.3.0.tar` & `text2term-2.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-04 15:09:44.164136 text2term-2.3.0/
--rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.3.0/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-04 15:09:44.163948 text2term-2.3.0/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)    14156 2023-05-04 15:09:10.000000 text2term-2.3.0/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2023-05-04 15:09:44.164179 text2term-2.3.0/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.3.0/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-04 15:09:44.160366 text2term-2.3.0/test/
--rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-2.3.0/test/test-pypi.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-04 15:09:44.163001 text2term-2.3.0/text2term/
--rw-r--r--   0 jason      (501) staff       (20)      427 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-2.3.0/text2term/__main__.py
--rw-r--r--   0 jason      (501) staff       (20)     4416 2022-08-03 13:24:07.000000 text2term-2.3.0/text2term/bioportal_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)       17 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/config.py
--rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.3.0/text2term/mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     3649 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/onto_cache.py
--rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.3.0/text2term/onto_utils.py
--rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.3.0/text2term/preprocess.py
--rw-r--r--   0 jason      (501) staff       (20)     5403 2023-02-09 15:42:55.000000 text2term-2.3.0/text2term/syntactic_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)    12516 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/t2t.py
--rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.3.0/text2term/tagged_terms.py
--rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-2.3.0/text2term/term.py
--rw-r--r--   0 jason      (501) staff       (20)    17050 2023-05-04 15:09:10.000000 text2term-2.3.0/text2term/term_collector.py
--rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.3.0/text2term/term_graph.py
--rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.3.0/text2term/term_graph_generator.py
--rw-r--r--   0 jason      (501) staff       (20)     2158 2023-04-11 13:56:32.000000 text2term-2.3.0/text2term/term_mapping.py
--rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.3.0/text2term/tfidf_mapper.py
--rw-r--r--   0 jason      (501) staff       (20)     4098 2023-02-09 15:42:55.000000 text2term-2.3.0/text2term/zooma_mapper.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-04 15:09:44.163758 text2term-2.3.0/text2term.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      649 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)      248 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)       10 2023-05-04 15:09:44.000000 text2term-2.3.0/text2term.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-10 16:24:55.959643 text2term-2.3.1/
+-rw-r--r--   0 jason      (501) staff       (20)     1117 2022-08-03 13:24:07.000000 text2term-2.3.1/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-10 16:24:55.959439 text2term-2.3.1/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)    14156 2023-05-04 15:09:10.000000 text2term-2.3.1/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2023-05-10 16:24:55.959695 text2term-2.3.1/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1162 2023-03-27 17:45:54.000000 text2term-2.3.1/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-10 16:24:55.955062 text2term-2.3.1/test/
+-rw-r--r--   0 jason      (501) staff       (20)     1435 2023-04-25 18:43:12.000000 text2term-2.3.1/test/test-pypi.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-10 16:24:55.958185 text2term-2.3.1/text2term/
+-rw-r--r--   0 jason      (501) staff       (20)      427 2023-05-04 15:09:10.000000 text2term-2.3.1/text2term/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4540 2023-04-25 19:04:10.000000 text2term-2.3.1/text2term/__main__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4416 2023-05-10 15:07:50.000000 text2term-2.3.1/text2term/bioportal_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)       17 2023-05-10 16:24:04.000000 text2term-2.3.1/text2term/config.py
+-rw-r--r--   0 jason      (501) staff       (20)      469 2022-09-26 14:42:08.000000 text2term-2.3.1/text2term/mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     3735 2023-05-10 16:24:04.000000 text2term-2.3.1/text2term/onto_cache.py
+-rw-r--r--   0 jason      (501) staff       (20)     6692 2023-03-27 17:45:54.000000 text2term-2.3.1/text2term/onto_utils.py
+-rw-r--r--   0 jason      (501) staff       (20)     5540 2023-03-27 17:45:54.000000 text2term-2.3.1/text2term/preprocess.py
+-rw-r--r--   0 jason      (501) staff       (20)     5403 2023-05-10 15:07:50.000000 text2term-2.3.1/text2term/syntactic_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)    12516 2023-05-10 15:07:50.000000 text2term-2.3.1/text2term/t2t.py
+-rw-r--r--   0 jason      (501) staff       (20)      741 2023-02-24 16:05:08.000000 text2term-2.3.1/text2term/tagged_terms.py
+-rw-r--r--   0 jason      (501) staff       (20)     2479 2023-04-18 15:25:34.000000 text2term-2.3.1/text2term/term.py
+-rw-r--r--   0 jason      (501) staff       (20)    17050 2023-05-04 15:09:10.000000 text2term-2.3.1/text2term/term_collector.py
+-rw-r--r--   0 jason      (501) staff       (20)     2697 2022-08-03 13:24:07.000000 text2term-2.3.1/text2term/term_graph.py
+-rw-r--r--   0 jason      (501) staff       (20)     2991 2023-01-20 15:17:36.000000 text2term-2.3.1/text2term/term_graph_generator.py
+-rw-r--r--   0 jason      (501) staff       (20)     2158 2023-04-11 13:56:32.000000 text2term-2.3.1/text2term/term_mapping.py
+-rw-r--r--   0 jason      (501) staff       (20)     5108 2022-11-15 20:43:11.000000 text2term-2.3.1/text2term/tfidf_mapper.py
+-rw-r--r--   0 jason      (501) staff       (20)     4098 2023-05-10 15:07:50.000000 text2term-2.3.1/text2term/zooma_mapper.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2023-05-10 16:24:55.959219 text2term-2.3.1/text2term.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)    14914 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      649 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)      248 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)       10 2023-05-10 16:24:55.000000 text2term-2.3.1/text2term.egg-info/top_level.txt
```

### Comparing `text2term-2.3.0/LICENSE` & `text2term-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/PKG-INFO` & `text2term-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.3.0
+Version: 2.3.1
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2term-2.3.0/README.md` & `text2term-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/setup.py` & `text2term-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/test/test-pypi.py` & `text2term-2.3.1/test/test-pypi.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/__main__.py` & `text2term-2.3.1/text2term/__main__.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/bioportal_mapper.py` & `text2term-2.3.1/text2term/bioportal_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/onto_cache.py` & `text2term-2.3.1/text2term/onto_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import text2term
 from .mapper import Mapper
 import os
 from shutil import rmtree
 import sys
+import pandas as pd
+import owlready2
 
 """
 CACHING FUNCTIONS -- Public
 """
 # Caches many ontologies from a csv
 def cache_ontology_set(ontology_registry_path):
     registry = pd.read_csv(ontology_registry_path)
     cache_set = {}
     for index, row in registry.iterrows():
         try:
             cache = text2term.cache_ontology(row.url, row.acronym)
             cache_set.update({row.acronym : cache})
         except Exception as err:
-            sys.stderr.write("Could not cache ontology", row.acronym, "due to error:", err)
+            err_message = "Could not cache ontology " + row.acronym + " due to error: " + str(err)
+            sys.stderr.write(err_message)
         owlready2.default_world.ontologies.clear()
     return cache_set
 
 # Will check if an acronym exists in the cache
 def cache_exists(ontology_acronym=''):
     return os.path.exists("cache/" + ontology_acronym)
```

### Comparing `text2term-2.3.0/text2term/onto_utils.py` & `text2term-2.3.1/text2term/onto_utils.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/preprocess.py` & `text2term-2.3.1/text2term/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/syntactic_mapper.py` & `text2term-2.3.1/text2term/syntactic_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/t2t.py` & `text2term-2.3.1/text2term/t2t.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/tagged_terms.py` & `text2term-2.3.1/text2term/tagged_terms.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/term.py` & `text2term-2.3.1/text2term/term.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/term_collector.py` & `text2term-2.3.1/text2term/term_collector.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/term_graph.py` & `text2term-2.3.1/text2term/term_graph.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/term_graph_generator.py` & `text2term-2.3.1/text2term/term_graph_generator.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/term_mapping.py` & `text2term-2.3.1/text2term/term_mapping.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/tfidf_mapper.py` & `text2term-2.3.1/text2term/tfidf_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term/zooma_mapper.py` & `text2term-2.3.1/text2term/zooma_mapper.py`

 * *Files identical despite different names*

### Comparing `text2term-2.3.0/text2term.egg-info/PKG-INFO` & `text2term-2.3.1/text2term.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2term
-Version: 2.3.0
+Version: 2.3.1
 Summary: A tool for mapping free-text descriptions of (biomedical) entities to controlled terms in ontologies
 Home-page: https://github.com/ccb-hms/ontology-mapper
 Author: Center for Computational Biomedicine, Harvard Medical School
 Author-email: rafael_goncalves@hms.harvard.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2term-2.3.0/text2term.egg-info/SOURCES.txt` & `text2term-2.3.1/text2term.egg-info/SOURCES.txt`

 * *Files identical despite different names*

