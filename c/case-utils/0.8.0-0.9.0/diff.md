# Comparing `tmp/case_utils-0.8.0.tar.gz` & `tmp/case_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "case_utils-0.8.0.tar", last modified: Wed Nov 23 20:18:07 2022, max compression
+gzip compressed data, was "case_utils-0.9.0.tar", last modified: Thu Dec  8 22:59:21 2022, max compression
```

## Comparing `case_utils-0.8.0.tar` & `case_utils-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:18:07.222906 case_utils-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10173 2022-11-23 19:46:05.000000 case_utils-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-11-23 20:18:07.222906 case_utils-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8788 2022-11-23 19:46:05.000000 case_utils-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1955 2022-11-23 19:46:05.000000 case_utils-0.8.0/THIRD_PARTY_LICENSES.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:18:07.218906 case_utils-0.8.0/case_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:18:07.218906 case_utils-0.8.0/case_utils/case_file/
--rw-r--r--   0 runner    (1001) docker     (121)     9709 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/case_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:18:07.218906 case_utils-0.8.0/case_utils/case_sparql_construct/
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/case_sparql_construct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:18:07.218906 case_utils-0.8.0/case_utils/case_sparql_select/
--rw-r--r--   0 runner    (1001) docker     (121)     6083 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/case_sparql_select/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:18:07.218906 case_utils-0.8.0/case_utils/case_validate/
--rw-r--r--   0 runner    (1001) docker     (121)    12361 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/case_validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5901 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/local_uuid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2761 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:18:07.222906 case_utils-0.8.0/case_utils/ontology/
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    61806 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-0.5.0-subclasses.ttl
--rw-r--r--   0 runner    (1001) docker     (121)   475799 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-0.5.0.ttl
--rw-r--r--   0 runner    (1001) docker     (121)    62432 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-0.6.0-subclasses.ttl
--rw-r--r--   0 runner    (1001) docker     (121)   496903 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-0.6.0.ttl
--rw-r--r--   0 runner    (1001) docker     (121)    62275 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-0.7.0-subclasses.ttl
--rw-r--r--   0 runner    (1001) docker     (121)   491247 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-0.7.0.ttl
--rw-r--r--   0 runner    (1001) docker     (121)    62275 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-0.7.1-subclasses.ttl
--rw-r--r--   0 runner    (1001) docker     (121)   490226 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-0.7.1.ttl
--rw-r--r--   0 runner    (1001) docker     (121)    70411 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-1.0.0-subclasses.ttl
--rw-r--r--   0 runner    (1001) docker     (121)   549021 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/case-1.0.0.ttl
--rw-r--r--   0 runner    (1001) docker     (121)    71585 2022-11-23 19:46:36.000000 case_utils-0.8.0/case_utils/ontology/case-1.1.0-subclasses.ttl
--rw-r--r--   0 runner    (1001) docker     (121)   554982 2022-11-23 19:46:36.000000 case_utils-0.8.0/case_utils/ontology/case-1.1.0.ttl
--rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-11-23 19:46:52.000000 case_utils-0.8.0/case_utils/ontology/ontology_and_version_iris.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/ontology/version_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-11-23 19:46:05.000000 case_utils-0.8.0/case_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 20:18:07.218906 case_utils-0.8.0/case_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-11-23 20:18:07.000000 case_utils-0.8.0/case_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-11-23 20:18:07.000000 case_utils-0.8.0/case_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 20:18:07.000000 case_utils-0.8.0/case_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-11-23 20:18:07.000000 case_utils-0.8.0/case_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-23 20:18:07.000000 case_utils-0.8.0/case_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-23 20:18:07.000000 case_utils-0.8.0/case_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-11-23 20:18:07.226906 case_utils-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-11-23 19:46:05.000000 case_utils-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:21.196822 case_utils-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2022-12-08 22:26:53.000000 case_utils-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2022-12-08 22:59:21.196822 case_utils-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2022-12-08 22:26:53.000000 case_utils-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2022-12-08 22:26:53.000000 case_utils-0.9.0/THIRD_PARTY_LICENSES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:21.188822 case_utils-0.9.0/case_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:21.188822 case_utils-0.9.0/case_utils/case_file/
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/case_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:21.188822 case_utils-0.9.0/case_utils/case_sparql_construct/
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/case_sparql_construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:21.188822 case_utils-0.9.0/case_utils/case_sparql_select/
+-rw-r--r--   0 runner    (1001) docker     (123)    12114 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/case_sparql_select/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:21.188822 case_utils-0.9.0/case_utils/case_validate/
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/case_validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/local_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:21.196822 case_utils-0.9.0/case_utils/ontology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61806 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-0.5.0-subclasses.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)   475799 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-0.5.0.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    62432 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-0.6.0-subclasses.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)   496903 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-0.6.0.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    62275 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-0.7.0-subclasses.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)   491247 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-0.7.0.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    62275 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-0.7.1-subclasses.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)   490226 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-0.7.1.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    70411 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-1.0.0-subclasses.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)   549021 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/case-1.0.0.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)    71585 2022-12-08 22:27:20.000000 case_utils-0.9.0/case_utils/ontology/case-1.1.0-subclasses.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)   554982 2022-12-08 22:27:20.000000 case_utils-0.9.0/case_utils/ontology/case-1.1.0.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2022-12-08 22:27:35.000000 case_utils-0.9.0/case_utils/ontology/ontology_and_version_iris.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/ontology/version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2022-12-08 22:26:53.000000 case_utils-0.9.0/case_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 22:59:21.188822 case_utils-0.9.0/case_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2022-12-08 22:59:21.000000 case_utils-0.9.0/case_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2022-12-08 22:59:21.000000 case_utils-0.9.0/case_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 22:59:21.000000 case_utils-0.9.0/case_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-08 22:59:21.000000 case_utils-0.9.0/case_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-08 22:59:21.000000 case_utils-0.9.0/case_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-08 22:59:21.000000 case_utils-0.9.0/case_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2022-12-08 22:59:21.196822 case_utils-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2022-12-08 22:26:53.000000 case_utils-0.9.0/setup.py
```

### Comparing `case_utils-0.8.0/LICENSE` & `case_utils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/PKG-INFO` & `case_utils-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: case_utils
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python utilities for working with the CASE ontology
 Home-page: https://github.com/casework/CASE-Utilities-Python
 Author: Alex Nelson
 Author-email: alexander.nelson@nist.gov
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `case_utils-0.8.0/README.md` & `case_utils-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/THIRD_PARTY_LICENSES.md` & `case_utils-0.9.0/THIRD_PARTY_LICENSES.md`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/__init__.py` & `case_utils-0.9.0/case_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 # protection and is in the public domain. NIST assumes no
 # responsibility whatsoever for its use by other parties, and makes
 # no guarantees, expressed or implied, about its quality,
 # reliability, or any other characteristic.
 #
 # We would appreciate acknowledgement if the software is used.
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 from . import local_uuid  # noqa: F401
```

### Comparing `case_utils-0.8.0/case_utils/case_file/__init__.py` & `case_utils-0.9.0/case_utils/case_file/__init__.py`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/case_sparql_construct/__init__.py` & `case_utils-0.9.0/case_utils/case_sparql_construct/__init__.py`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/case_validate/__init__.py` & `case_utils-0.9.0/case_utils/case_validate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ontology and shape graphs).  More specifically to CASE, if no particular
 ontology or shapes graph is requested, the most recent version of CASE
 will be used.  (That most recent version is shipped with this package as
 a monolithic file; see case_utils.ontology if interested in further
 details.)
 """
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 import argparse
 import importlib.resources
 import logging
 import os
 import sys
 import typing
@@ -47,14 +47,15 @@
     CURRENT_CASE_VERSION,
     built_version_choices_list,
 )
 
 NS_OWL = rdflib.OWL
 NS_RDF = rdflib.RDF
 NS_RDFS = rdflib.RDFS
+NS_SH = rdflib.SH
 
 _logger = logging.getLogger(os.path.basename(__file__))
 
 
 class NonExistentCDOConceptWarning(UserWarning):
     """
     This class is used when a concept is encountered in the data graph that is not part of CDO ontologies, according to the --built-version flags and --ontology-graph flags.
@@ -185,14 +186,17 @@
 
     for n_structural_class in [
         NS_OWL.Class,
         NS_OWL.AnnotationProperty,
         NS_OWL.DatatypeProperty,
         NS_OWL.ObjectProperty,
         NS_RDFS.Datatype,
+        NS_SH.NodeShape,
+        NS_SH.PropertyShape,
+        NS_SH.Shape,
     ]:
         for ontology_triple in ontology_graph.triples(
             (None, NS_RDF.type, n_structural_class)
         ):
             if not isinstance(ontology_triple[0], rdflib.URIRef):
                 continue
             if concept_is_cdo_concept(ontology_triple[0]):
```

### Comparing `case_utils-0.8.0/case_utils/local_uuid.py` & `case_utils-0.9.0/case_utils/local_uuid.py`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/namespace.py` & `case_utils-0.9.0/case_utils/namespace.py`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/__init__.py` & `case_utils-0.9.0/case_utils/ontology/__init__.py`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-0.5.0-subclasses.ttl` & `case_utils-0.9.0/case_utils/ontology/case-0.5.0-subclasses.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-0.5.0.ttl` & `case_utils-0.9.0/case_utils/ontology/case-0.5.0.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-0.6.0-subclasses.ttl` & `case_utils-0.9.0/case_utils/ontology/case-0.6.0-subclasses.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-0.6.0.ttl` & `case_utils-0.9.0/case_utils/ontology/case-0.6.0.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-0.7.0-subclasses.ttl` & `case_utils-0.9.0/case_utils/ontology/case-0.7.0-subclasses.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-0.7.0.ttl` & `case_utils-0.9.0/case_utils/ontology/case-0.7.0.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-0.7.1-subclasses.ttl` & `case_utils-0.9.0/case_utils/ontology/case-0.7.1-subclasses.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-0.7.1.ttl` & `case_utils-0.9.0/case_utils/ontology/case-0.7.1.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-1.0.0-subclasses.ttl` & `case_utils-0.9.0/case_utils/ontology/case-1.0.0-subclasses.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-1.0.0.ttl` & `case_utils-0.9.0/case_utils/ontology/case-1.0.0.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-1.1.0-subclasses.ttl` & `case_utils-0.9.0/case_utils/ontology/case-1.1.0-subclasses.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/case-1.1.0.ttl` & `case_utils-0.9.0/case_utils/ontology/case-1.1.0.ttl`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/ontology_and_version_iris.txt` & `case_utils-0.9.0/case_utils/ontology/ontology_and_version_iris.txt`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/ontology/version_info.py` & `case_utils-0.9.0/case_utils/ontology/version_info.py`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils/py.typed` & `case_utils-0.9.0/case_utils/py.typed`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/case_utils.egg-info/PKG-INFO` & `case_utils-0.9.0/case_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: case-utils
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python utilities for working with the CASE ontology
 Home-page: https://github.com/casework/CASE-Utilities-Python
 Author: Alex Nelson
 Author-email: alexander.nelson@nist.gov
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `case_utils-0.8.0/case_utils.egg-info/SOURCES.txt` & `case_utils-0.9.0/case_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/setup.cfg` & `case_utils-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `case_utils-0.8.0/setup.py` & `case_utils-0.9.0/setup.py`

 * *Files identical despite different names*

