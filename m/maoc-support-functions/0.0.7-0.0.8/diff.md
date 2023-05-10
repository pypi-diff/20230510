# Comparing `tmp/maoc_support_functions-0.0.7.tar.gz` & `tmp/maoc_support_functions-0.0.8.tar.gz`

## Comparing `maoc_support_functions-0.0.7.tar` & `maoc_support_functions-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/Untitled.ipynb
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/src/maoc_support_functions/__init__.py
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/src/maoc_support_functions/representation.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/src/maoc_support_functions/supporting_functions.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/README.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/Untitled.ipynb
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/src/maoc_support_functions/__init__.py
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/src/maoc_support_functions/representation.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/src/maoc_support_functions/supporting_functions.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/README.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.8/PKG-INFO
```

### Comparing `maoc_support_functions-0.0.7/src/maoc_support_functions/representation.py` & `maoc_support_functions-0.0.8/src/maoc_support_functions/representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 # In[ ]:
 
 
 #The code that generates the MAOC representation
-def MAOC(PATH=None, basis_set='sto-3g',charge=0,nr_pca=None,spin=None,pre_orth_AO='ANO',pca_explanation=True):
+def MAOC(PATH=None, basis_set='sto-3g',charge=0,nr_pca=None,spin=None,pre_orth_AO='ANO',pca_explanation=False):
     from pyscf import scf,gto,lo
     import glob
     import pandas as pd
     import re
     import numpy as np
     from maoc_support_functions.supporting_functions import MAOC_atom_extraction
     from maoc_support_functions.supporting_functions import MAOC_min_ch_max_ch
```

### Comparing `maoc_support_functions-0.0.7/src/maoc_support_functions/supporting_functions.py` & `maoc_support_functions-0.0.8/src/maoc_support_functions/supporting_functions.py`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.7/LICENSE` & `maoc_support_functions-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.7/pyproject.toml` & `maoc_support_functions-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maoc_support_functions"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Stiv Llenga", email="stiv.llenga@h-its.org" },
 ]
 description = "Functions for generating the MAOC representation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `maoc_support_functions-0.0.7/PKG-INFO` & `maoc_support_functions-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maoc_support_functions
-Version: 0.0.7
+Version: 0.0.8
 Summary: Functions for generating the MAOC representation.
 Project-URL: Homepage, https://github.com/hits-ccc/MAOC
 Author-email: Stiv Llenga <stiv.llenga@h-its.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

