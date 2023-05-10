# Comparing `tmp/sequence_modelling-0.1.0.tar.gz` & `tmp/sequence_modelling-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequence_modelling-0.1.0.tar", max compression
+gzip compressed data, was "sequence_modelling-0.1.1.tar", max compression
```

## Comparing `sequence_modelling-0.1.0.tar` & `sequence_modelling-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1500 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/LICENSE
--rw-r--r--   0        0        0     1662 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/README.md
--rw-r--r--   0        0        0      842 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9876 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/src/sequence_modelling/DiscreteOptim.py
--rw-r--r--   0        0        0        0 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/src/sequence_modelling/__init__.py
--rw-r--r--   0        0        0     5924 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/src/sequence_modelling/emissionplus.py
--rw-r--r--   0        0        0     5215 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/src/sequence_modelling/emmissions.py
--rw-r--r--   0        0        0    18463 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/src/sequence_modelling/hmm.py
--rw-r--r--   0        0        0     5939 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/src/sequence_modelling/hmmviz.py
--rw-r--r--   0        0        0    14746 2023-05-09 18:37:00.533197 sequence_modelling-0.1.0/src/sequence_modelling/qdhmm.py
--rw-r--r--   0        0        0    11882 2023-05-09 18:37:00.537197 sequence_modelling-0.1.0/src/sequence_modelling/qdhmm_logscaled.py
--rw-r--r--   0        0        0     1538 2023-05-09 18:37:00.537197 sequence_modelling-0.1.0/src/sequence_modelling/utils.py
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 sequence_modelling-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-05-09 19:09:21.749576 sequence_modelling-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1662 2023-05-09 19:09:21.749576 sequence_modelling-0.1.1/README.md
+-rw-r--r--   0        0        0      842 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9876 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/DiscreteOptim.py
+-rw-r--r--   0        0        0        0 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/__init__.py
+-rw-r--r--   0        0        0     5924 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/emissionplus.py
+-rw-r--r--   0        0        0     5215 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/emmissions.py
+-rw-r--r--   0        0        0    18463 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/hmm.py
+-rw-r--r--   0        0        0     5939 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/hmmviz.py
+-rw-r--r--   0        0        0    14746 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/qdhmm.py
+-rw-r--r--   0        0        0    11882 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/qdhmm_logscaled.py
+-rw-r--r--   0        0        0     1538 2023-05-09 19:09:21.753576 sequence_modelling-0.1.1/src/sequence_modelling/utils.py
+-rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 sequence_modelling-0.1.1/PKG-INFO
```

### Comparing `sequence_modelling-0.1.0/LICENSE` & `sequence_modelling-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/README.md` & `sequence_modelling-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/pyproject.toml` & `sequence_modelling-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequence_modelling"
-version = "0.1.0"
+version = "0.1.1"
 description = "sequence modelling using HMMs"
 authors = ["Nitin Bhushan <bhushan.nitin@posteo.net>"]
 readme = "README.md"
 license = "BSD-2-Clause"
 
 
 [tool.poetry.dependencies]
```

### Comparing `sequence_modelling-0.1.0/src/sequence_modelling/DiscreteOptim.py` & `sequence_modelling-0.1.1/src/sequence_modelling/DiscreteOptim.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/src/sequence_modelling/emissionplus.py` & `sequence_modelling-0.1.1/src/sequence_modelling/emissionplus.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/src/sequence_modelling/emmissions.py` & `sequence_modelling-0.1.1/src/sequence_modelling/emmissions.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/src/sequence_modelling/hmm.py` & `sequence_modelling-0.1.1/src/sequence_modelling/hmm.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/src/sequence_modelling/hmmviz.py` & `sequence_modelling-0.1.1/src/sequence_modelling/hmmviz.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/src/sequence_modelling/qdhmm.py` & `sequence_modelling-0.1.1/src/sequence_modelling/qdhmm.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/src/sequence_modelling/qdhmm_logscaled.py` & `sequence_modelling-0.1.1/src/sequence_modelling/qdhmm_logscaled.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/src/sequence_modelling/utils.py` & `sequence_modelling-0.1.1/src/sequence_modelling/utils.py`

 * *Files identical despite different names*

### Comparing `sequence_modelling-0.1.0/PKG-INFO` & `sequence_modelling-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequence-modelling
-Version: 0.1.0
+Version: 0.1.1
 Summary: sequence modelling using HMMs
 License: BSD-2-Clause
 Author: Nitin Bhushan
 Author-email: bhushan.nitin@posteo.net
 Requires-Python: >=3.9.0,<3.10.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

