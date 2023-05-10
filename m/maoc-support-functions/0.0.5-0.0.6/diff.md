# Comparing `tmp/maoc_support_functions-0.0.5.tar.gz` & `tmp/maoc_support_functions-0.0.6.tar.gz`

## Comparing `maoc_support_functions-0.0.5.tar` & `maoc_support_functions-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/src/maoc_support_functions/__init__.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/src/maoc_support_functions/representation.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/src/maoc_support_functions/supporting_functions.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/README.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.6/src/maoc_support_functions/__init__.py
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.6/src/maoc_support_functions/representation.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.6/src/maoc_support_functions/supporting_functions.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.6/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.6/README.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.6/PKG-INFO
```

### Comparing `maoc_support_functions-0.0.5/src/maoc_support_functions/representation.py` & `maoc_support_functions-0.0.6/src/maoc_support_functions/representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 #The code that generates the MAOC representation
 def MAOC(PATH=None, basis_set='sto-3g',charge=0,nr_pca=None,spin=None,pre_orth_AO='ANO',pca_explanation=True):
     from pyscf import scf,gto,lo
     import glob
     import pandas as pd
+    import re
     import numpy as np
     from maoc_support_functions.supporting_functions import MAOC_atom_extraction
     from maoc_support_functions.supporting_functions import MAOC_min_ch_max_ch
     from maoc_support_functions.supporting_functions import MAOC_partial_charges
     from maoc_support_functions.supporting_functions import MAOC_periodic_table
     from natsort import natsorted
     from sklearn.decomposition import PCA
```

### Comparing `maoc_support_functions-0.0.5/src/maoc_support_functions/supporting_functions.py` & `maoc_support_functions-0.0.6/src/maoc_support_functions/supporting_functions.py`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.5/LICENSE` & `maoc_support_functions-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.5/pyproject.toml` & `maoc_support_functions-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maoc_support_functions"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Stiv Llenga", email="stiv.llenga@h-its.org" },
 ]
 description = "Functions for generating the MAOC representation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `maoc_support_functions-0.0.5/PKG-INFO` & `maoc_support_functions-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maoc_support_functions
-Version: 0.0.5
+Version: 0.0.6
 Summary: Functions for generating the MAOC representation.
 Project-URL: Homepage, https://github.com/hits-ccc/MAOC
 Author-email: Stiv Llenga <stiv.llenga@h-its.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

