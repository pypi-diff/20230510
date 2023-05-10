# Comparing `tmp/ikarus-0.0.2.tar.gz` & `tmp/ikarus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ikarus-0.0.2.tar", last modified: Fri Mar 11 17:31:50 2022, max compression
+gzip compressed data, was "ikarus-0.0.3.tar", last modified: Wed May 10 10:32:31 2023, max compression
```

## Comparing `ikarus-0.0.2.tar` & `ikarus-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2022-03-11 17:31:50.903338 ikarus-0.0.2/
--rw-r--r--   0 jona      (1000) jona      (1000)      131 2022-03-11 17:31:50.903338 ikarus-0.0.2/PKG-INFO
--rw-r--r--   0 jona      (1000) jona      (1000)     2702 2022-03-11 17:29:27.000000 ikarus-0.0.2/README.rst
-drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2022-03-11 17:31:50.903338 ikarus-0.0.2/ikarus/
--rw-r--r--   0 jona      (1000) jona      (1000)       88 2022-03-11 13:46:43.000000 ikarus-0.0.2/ikarus/__init__.py
--rw-r--r--   0 jona      (1000) jona      (1000)    22413 2022-03-11 13:46:43.000000 ikarus-0.0.2/ikarus/classifier.py
--rw-r--r--   0 jona      (1000) jona      (1000)     2404 2022-03-11 13:46:43.000000 ikarus-0.0.2/ikarus/data.py
--rw-r--r--   0 jona      (1000) jona      (1000)     6687 2022-03-11 13:46:43.000000 ikarus-0.0.2/ikarus/gene_list.py
--rw-r--r--   0 jona      (1000) jona      (1000)      159 2022-03-11 13:46:43.000000 ikarus-0.0.2/ikarus/utils.py
-drwxr-xr-x   0 jona      (1000) jona      (1000)        0 2022-03-11 17:31:50.903338 ikarus-0.0.2/ikarus.egg-info/
--rw-r--r--   0 jona      (1000) jona      (1000)      131 2022-03-11 17:31:50.000000 ikarus-0.0.2/ikarus.egg-info/PKG-INFO
--rw-r--r--   0 jona      (1000) jona      (1000)      259 2022-03-11 17:31:50.000000 ikarus-0.0.2/ikarus.egg-info/SOURCES.txt
--rw-r--r--   0 jona      (1000) jona      (1000)        1 2022-03-11 17:31:50.000000 ikarus-0.0.2/ikarus.egg-info/dependency_links.txt
--rw-r--r--   0 jona      (1000) jona      (1000)       43 2022-03-11 17:31:50.000000 ikarus-0.0.2/ikarus.egg-info/requires.txt
--rw-r--r--   0 jona      (1000) jona      (1000)        7 2022-03-11 17:31:50.000000 ikarus-0.0.2/ikarus.egg-info/top_level.txt
--rw-r--r--   0 jona      (1000) jona      (1000)       38 2022-03-11 17:31:50.903338 ikarus-0.0.2/setup.cfg
--rw-r--r--   0 jona      (1000) jona      (1000)      372 2022-03-11 17:31:36.000000 ikarus-0.0.2/setup.py
+drwxr-xr-x   0 jd         (501) staff       (20)        0 2023-05-10 10:32:31.483446 ikarus-0.0.3/
+-rw-r--r--   0 jd         (501) staff       (20)     1086 2023-05-10 10:17:49.000000 ikarus-0.0.3/LICENSE
+-rw-r--r--   0 jd         (501) staff       (20)       85 2023-05-10 10:32:31.483328 ikarus-0.0.3/PKG-INFO
+-rw-r--r--   0 jd         (501) staff       (20)     2908 2023-05-10 10:17:49.000000 ikarus-0.0.3/README.rst
+drwxr-xr-x   0 jd         (501) staff       (20)        0 2023-05-10 10:32:31.482551 ikarus-0.0.3/ikarus/
+-rw-r--r--   0 jd         (501) staff       (20)       88 2023-05-10 10:17:49.000000 ikarus-0.0.3/ikarus/__init__.py
+-rw-r--r--   0 jd         (501) staff       (20)    22412 2023-05-10 10:17:49.000000 ikarus-0.0.3/ikarus/classifier.py
+-rw-r--r--   0 jd         (501) staff       (20)     2404 2023-05-10 10:17:49.000000 ikarus-0.0.3/ikarus/data.py
+-rw-r--r--   0 jd         (501) staff       (20)     6687 2023-05-10 10:17:49.000000 ikarus-0.0.3/ikarus/gene_list.py
+-rw-r--r--   0 jd         (501) staff       (20)      159 2023-05-10 10:17:49.000000 ikarus-0.0.3/ikarus/utils.py
+drwxr-xr-x   0 jd         (501) staff       (20)        0 2023-05-10 10:32:31.483167 ikarus-0.0.3/ikarus.egg-info/
+-rw-r--r--   0 jd         (501) staff       (20)       85 2023-05-10 10:32:31.000000 ikarus-0.0.3/ikarus.egg-info/PKG-INFO
+-rw-r--r--   0 jd         (501) staff       (20)      267 2023-05-10 10:32:31.000000 ikarus-0.0.3/ikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 jd         (501) staff       (20)        1 2023-05-10 10:32:31.000000 ikarus-0.0.3/ikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 jd         (501) staff       (20)       51 2023-05-10 10:32:31.000000 ikarus-0.0.3/ikarus.egg-info/requires.txt
+-rw-r--r--   0 jd         (501) staff       (20)        7 2023-05-10 10:32:31.000000 ikarus-0.0.3/ikarus.egg-info/top_level.txt
+-rw-r--r--   0 jd         (501) staff       (20)       38 2023-05-10 10:32:31.483482 ikarus-0.0.3/setup.cfg
+-rw-r--r--   0 jd         (501) staff       (20)      410 2023-05-10 10:26:55.000000 ikarus-0.0.3/setup.py
```

### Comparing `ikarus-0.0.2/README.rst` & `ikarus-0.0.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-|3.8 badge| |3.9 badge| |3.10 badge| |PyPI version|
+|3.8 badge| |3.9 badge| |3.10 badge| |license badge| |PyPI version|
 
 ========
-Ikarus
+ikarus
 ========
 
-Ikarus is a stepwise machine learning pipeline that tries to cope with a task of distinguishing tumor cells from normal cells.
+ikarus is a stepwise machine learning pipeline that tries to cope with a task of distinguishing tumor cells from normal cells.
 Leveraging multiple annotated single cell datasets it can be used to define a gene set specific to tumor cells. 
 First, the latter gene set is used to rank cells and then to train a logistic classifier for the robust classification of tumor and normal cells.
 Finally, sensitivity is increased by propagating the cell labels based on a custom cell-cell network. 
-Ikarus is tested on multiple single cell datasets to ascertain that it achieves high sensitivity and specificity in multiple experimental contexts.
-Please find more information in `our preprint <https://doi.org/10.1101/2021.10.15.463909>`_.
+ikarus is tested on multiple single cell datasets to ascertain that it achieves high sensitivity and specificity in multiple experimental contexts.
+Please find more information in the corresponding `publication <https://genomebiology.biomedcentral.com/articles/10.1186/s13059-022-02683-1>`_.
 
 .. image:: ikarus_schema.svg
   :width: 600
   
   
 Installation
 ============
-Ikarus currently supports :code:`python 3.8`, and can be installed from PyPI:
+ikarus currently supports :code:`python>=3.8`, and can be installed from PyPI:
 
 ::
 
   pip install ikarus
  
 Alterantively, one can install ikarus' master branch directly from github:
  
@@ -49,16 +49,18 @@
 
 +----------------------------------------------------+
 | Example notebooks                                  |
 +====================================================+
 | `Data preparation and basic prediction`_           |
 +----------------------------------------------------+
 
-.. _`Data preparation and basic prediction`: https://github.com/BIMSBbioinfo/ikarus/blob/master/tutorial.ipynb
+.. _`Data preparation and basic prediction`: https://github.com/BIMSBbioinfo/ikarus/blob/master/tutorials/tutorial.ipynb
 .. |3.8 badge| image:: https://github.com/BIMSBbioinfo/ikarus/actions/workflows/python-package-3.8.yml/badge.svg
     :target: https://github.com/BIMSBbioinfo/ikarus/actions/workflows/python-package-3.8.yml
 .. |3.9 badge| image:: https://github.com/BIMSBbioinfo/ikarus/actions/workflows/python-package-3.9.yml/badge.svg
     :target: https://github.com/BIMSBbioinfo/ikarus/actions/workflows/python-package-3.9.yml
 .. |3.10 badge| image:: https://github.com/BIMSBbioinfo/ikarus/actions/workflows/python-package-3.10.yml/badge.svg
     :target: https://github.com/BIMSBbioinfo/ikarus/actions/workflows/python-package-3.10.yml
+.. |license badge| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+    :target: https://opensource.org/licenses/MIT
 .. |PyPI version| image:: https://badge.fury.io/py/ikarus.svg
     :target: https://pypi.org/project/ikarus/
```

### Comparing `ikarus-0.0.2/ikarus/classifier.py` & `ikarus-0.0.3/ikarus/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import pandas as pd
 import scanpy as sc
 from pathlib import Path
 from sklearn.linear_model import LogisticRegression
 from scipy.sparse import save_npz, load_npz
 from pyscenic.aucell import aucell, derive_auc_threshold
-from pyscenic.genesig import GeneSignature
+from ctxcore.genesig import GeneSignature
 
 
 def init_core_model(core_model_str):
     """Method to set the underlying core model.
     
     The core model is used to make first predictions 
     based on ranked scores.
```

### Comparing `ikarus-0.0.2/ikarus/data.py` & `ikarus-0.0.3/ikarus/data.py`

 * *Files identical despite different names*

### Comparing `ikarus-0.0.2/ikarus/gene_list.py` & `ikarus-0.0.3/ikarus/gene_list.py`

 * *Files identical despite different names*

