# Comparing `tmp/metaquantus-0.0.3.tar.gz` & `tmp/metaquantus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaquantus-0.0.3.tar", last modified: Sat Apr  1 15:48:45 2023, max compression
+gzip compressed data, was "metaquantus-0.0.4.tar", last modified: Wed May 10 08:55:01 2023, max compression
```

## Comparing `metaquantus-0.0.3.tar` & `metaquantus-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 15:48:45.736227 metaquantus-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-01 15:48:33.000000 metaquantus-0.0.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-01 15:48:33.000000 metaquantus-0.0.3/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-01 15:48:45.736227 metaquantus-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-04-01 15:48:33.000000 metaquantus-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 15:48:45.732227 metaquantus-0.0.3/metaquantus/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/benchmarking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 15:48:45.732227 metaquantus-0.0.3/metaquantus/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/helpers/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    61736 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/helpers/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/helpers/sanity_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28260 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32511 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/meta_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 15:48:45.736227 metaquantus-0.0.3/metaquantus/perturbation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/perturbation_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/perturbation_tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/perturbation_tests/ipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-01 15:48:33.000000 metaquantus-0.0.3/metaquantus/perturbation_tests/mpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 15:48:45.732227 metaquantus-0.0.3/metaquantus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-01 15:48:45.000000 metaquantus-0.0.3/metaquantus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-01 15:48:45.000000 metaquantus-0.0.3/metaquantus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 15:48:45.000000 metaquantus-0.0.3/metaquantus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 15:48:45.000000 metaquantus-0.0.3/metaquantus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-01 15:48:45.000000 metaquantus-0.0.3/metaquantus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-01 15:48:45.000000 metaquantus-0.0.3/metaquantus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 15:48:45.736227 metaquantus-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-01 15:48:33.000000 metaquantus-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 15:48:45.736227 metaquantus-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 15:48:33.000000 metaquantus-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-01 15:48:33.000000 metaquantus-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-01 15:48:33.000000 metaquantus-0.0.3/tests/test_benchmarking.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-04-01 15:48:33.000000 metaquantus-0.0.3/tests/test_meta_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:55:01.445043 metaquantus-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 08:54:50.000000 metaquantus-0.0.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-10 08:54:50.000000 metaquantus-0.0.4/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 08:54:50.000000 metaquantus-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-05-10 08:55:01.445043 metaquantus-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-10 08:54:50.000000 metaquantus-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:55:01.441043 metaquantus-0.0.4/metaquantus/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/benchmarking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:55:01.441043 metaquantus-0.0.4/metaquantus/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31086 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/helpers/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61764 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/helpers/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/helpers/sanity_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28260 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32517 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/meta_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:55:01.445043 metaquantus-0.0.4/metaquantus/perturbation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/perturbation_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/perturbation_tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/perturbation_tests/ipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-10 08:54:50.000000 metaquantus-0.0.4/metaquantus/perturbation_tests/mpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:55:01.441043 metaquantus-0.0.4/metaquantus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-05-10 08:55:01.000000 metaquantus-0.0.4/metaquantus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-10 08:55:01.000000 metaquantus-0.0.4/metaquantus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:55:01.000000 metaquantus-0.0.4/metaquantus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:55:01.000000 metaquantus-0.0.4/metaquantus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 08:55:01.000000 metaquantus-0.0.4/metaquantus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 08:55:01.000000 metaquantus-0.0.4/metaquantus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 08:54:50.000000 metaquantus-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 08:54:50.000000 metaquantus-0.0.4/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:55:01.445043 metaquantus-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-10 08:54:50.000000 metaquantus-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:55:01.445043 metaquantus-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:54:50.000000 metaquantus-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-10 08:54:50.000000 metaquantus-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-10 08:54:50.000000 metaquantus-0.0.4/tests/test_benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-10 08:54:50.000000 metaquantus-0.0.4/tests/test_meta_evaluation.py
```

### Comparing `metaquantus-0.0.3/COPYING` & `metaquantus-0.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/COPYING.LESSER` & `metaquantus-0.0.4/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/PKG-INFO` & `metaquantus-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: metaquantus
-Version: 0.0.3
+Version: 0.0.4
 Summary: MetaQuantus is a XAI performance tool for identifying reliable metrics.
 Home-page: https://github.com/annahedstroem/MetaQuantus
 Author: Anna Hedstrom
 Author-email: hedstroem.anna@gmail.com
 License: GNU LESSER GENERAL PUBLIC LICENSE VERSION 3
 Keywords: explainable ai,evaluation,xai,machine learning,deep learning
-Requires-Python: >=3.7.1
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 
 <br/><br/>
 <p align="center">
   <img width="450" src="https://raw.githubusercontent.com/annahedstroem/MetaQuantus/main/logo.png">
@@ -19,15 +19,15 @@
 <h3 align="center"><b>An XAI performance tool for the identification of reliable metrics</b></h3>
 <p align="center">
   PyTorch
   
 This repository contains the code and experimental results for the paper **[The Meta-Evaluation Problem in Explainable AI: Identifying Reliable Estimators with MetaQuantus](https://arxiv.org/abs/2302.07265)** by Hedström et al., 2023.
 
 [![Getting started!](https://colab.research.google.com/assets/colab-badge.svg)](anonymous)
-![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/metaquantus.svg)](https://badge.fury.io/py/metaquantus)
 [![Python package](https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)](https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)
 <!--[![Launch Tutorials](https://mybinder.org/badge_logo.svg)](anonymous)-->
 
 _MetaQuantus is currently under active development. Carefully note the release version to ensure reproducibility of your work._
```

#### html2text {}

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 2.1 Name: metaquantus Version: 0.0.3 Summary: MetaQuantus is
+Metadata-Version: 2.1 Name: metaquantus Version: 0.0.4 Summary: MetaQuantus is
 a XAI performance tool for identifying reliable metrics. Home-page: https://
 github.com/annahedstroem/MetaQuantus Author: Anna Hedstrom Author-email:
 hedstroem.anna@gmail.com License: GNU LESSER GENERAL PUBLIC LICENSE VERSION 3
 Keywords: explainable ai,evaluation,xai,machine learning,deep learning
-Requires-Python: >=3.7.1 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 COPYING License-File: COPYING.LESSER
 
   [https://raw.githubusercontent.com/annahedstroem/MetaQuantus/main/logo.png]
  **** An XAI performance tool for the identification of reliable metrics ****
   PyTorch This repository contains the code and experimental results for the
  paper **[The Meta-Evaluation Problem in Explainable AI: Identifying Reliable
  Estimators with MetaQuantus](https://arxiv.org/abs/2302.07265)** by HedstrÃ¶m
  et al., 2023. [![Getting started!](https://colab.research.google.com/assets/
  colab-badge.svg)](anonymous) ![Python version](https://img.shields.io/badge/
-  python-3.7%20%7C%203.8%20%7C%203.9-blue.svg) [![Code style: black](https://
- img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-  black) [![PyPI version](https://badge.fury.io/py/metaquantus.svg)](https://
-     badge.fury.io/py/metaquantus) [![Python package](https://github.com/
-  annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)]
+python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg) [![Code
+  style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+   (https://github.com/psf/black) [![PyPI version](https://badge.fury.io/py/
+  metaquantus.svg)](https://badge.fury.io/py/metaquantus) [![Python package]
     (https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-
-  publish.yml/badge.svg)  _MetaQuantus is currently under active development.
-Carefully note the release version to ensure reproducibility of your work._ ##
-Citation If you find this toolkit or its companion paper interesting or useful
-  in your research, use the following Bibtex annotation to cite us: ```bibtex
-@article{hedstrom2023metaquantus, author = {HedstrÃ¶m, Anna and Bommer, Philine
-and WickstrÃ¸m, Kristoffer K. and Samek, Wojciech and Lapuschkin, Sebastian and
-HÃ¶hne, Marina M. -C.}, title = {The Meta-Evaluation Problem in Explainable AI:
-      Identifying Reliable Estimators with MetaQuantus}, doi = {10.48550/
-   ARXIV.2302.07265}, url = {https://arxiv.org/abs/2302.07265}, publisher =
-{arXiv}, year = {2023}, } ``` ## Table of Contents 1. [Motivation](#motivation)
- 2. [Library](#library) 3. [Installation](#installation) 4. [Getting started]
- (#getting-started) 5. [MetaQuantus methodology](#metaquantus-methodology) 6.
-  [Reproduce the experiments](#reproduce-the-experiments) ## Motivation **The
- Evaluation Disagreement Problem.** In Explainable AI (XAI), the need of meta-
-evaluation (i.e., the process of evaluating the evaluation method) arises as we
-   select and quantitatively compare explanation methods for a given model,
- dataset and task---where the use of multiple metrics or evaluation techniques
-  oftentimes lead to conflicting results. For example, scores from different
-    metrics vary, both in range and direction, with lower or higher scores
- indicating higher quality explanations, making it difficult for practitioners
-to interpret the scores and select the best explanation method. As illustrated
- in the Figure below, the two metrics, Faithfulness Correlation (FC) (Bhatt_et
-     al.,_2020) and Pixel-Flipping (PF) (Bach_et_al.,_2015) rank the same
- explanation methods differently. For example, the Gradient method (MÃ¸rch_et
-  al.,_1995) (Baehrens_et_al.,_2010) is both ranked the highest (R=1) and the
+ publish.yml/badge.svg)](https://github.com/annahedstroem/MetaQuantus/actions/
+workflows/python-publish.yml/badge.svg)  _MetaQuantus is currently under active
+ development. Carefully note the release version to ensure reproducibility of
+    your work._ ## Citation If you find this toolkit or its companion paper
+interesting or useful in your research, use the following Bibtex annotation to
+cite us: ```bibtex @article{hedstrom2023metaquantus, author = {HedstrÃ¶m, Anna
+   and Bommer, Philine and WickstrÃ¸m, Kristoffer K. and Samek, Wojciech and
+Lapuschkin, Sebastian and HÃ¶hne, Marina M. -C.}, title = {The Meta-Evaluation
+ Problem in Explainable AI: Identifying Reliable Estimators with MetaQuantus},
+ doi = {10.48550/ARXIV.2302.07265}, url = {https://arxiv.org/abs/2302.07265},
+publisher = {arXiv}, year = {2023}, } ``` ## Table of Contents 1. [Motivation]
+   (#motivation) 2. [Library](#library) 3. [Installation](#installation) 4.
+[Getting started](#getting-started) 5. [MetaQuantus methodology](#metaquantus-
+  methodology) 6. [Reproduce the experiments](#reproduce-the-experiments) ##
+ Motivation **The Evaluation Disagreement Problem.** In Explainable AI (XAI),
+  the need of meta-evaluation (i.e., the process of evaluating the evaluation
+method) arises as we select and quantitatively compare explanation methods for
+    a given model, dataset and task---where the use of multiple metrics or
+  evaluation techniques oftentimes lead to conflicting results. For example,
+scores from different metrics vary, both in range and direction, with lower or
+ higher scores indicating higher quality explanations, making it difficult for
+ practitioners to interpret the scores and select the best explanation method.
+As illustrated in the Figure below, the two metrics, Faithfulness Correlation
+(FC) (Bhatt_et_al.,_2020) and Pixel-Flipping (PF) (Bach_et_al.,_2015) rank the
+same explanation methods differently. For example, the Gradient method (MÃ¸rch
+et_al.,_1995) (Baehrens_et_al.,_2010) is both ranked the highest (R=1) and the
  lowest (R=3) depending on the metric used. From a practitioner's perspective,
                             this causes confusion.
     [https://raw.githubusercontent.com/annahedstroem/MetaQuantus/main/fig1-
                                   cmnist.png]
 **Our Meta-Evaluation Approach.** With [MetaQuantus](https://github.com/
 annahedstroem/MetaQuantus), we address the problem of meta-evaluation by
 providing a simple yet comprehensive framework that evaluates metrics against
```

### Comparing `metaquantus-0.0.3/README.md` & `metaquantus-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 <h3 align="center"><b>An XAI performance tool for the identification of reliable metrics</b></h3>
 <p align="center">
   PyTorch
   
 This repository contains the code and experimental results for the paper **[The Meta-Evaluation Problem in Explainable AI: Identifying Reliable Estimators with MetaQuantus](https://arxiv.org/abs/2302.07265)** by Hedström et al., 2023.
 
 [![Getting started!](https://colab.research.google.com/assets/colab-badge.svg)](anonymous)
-![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/metaquantus.svg)](https://badge.fury.io/py/metaquantus)
 [![Python package](https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)](https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)
 <!--[![Launch Tutorials](https://mybinder.org/badge_logo.svg)](anonymous)-->
 
 _MetaQuantus is currently under active development. Carefully note the release version to ensure reproducibility of your work._
```

#### html2text {}

```diff
@@ -3,45 +3,45 @@
   [https://raw.githubusercontent.com/annahedstroem/MetaQuantus/main/logo.png]
  **** An XAI performance tool for the identification of reliable metrics ****
   PyTorch This repository contains the code and experimental results for the
  paper **[The Meta-Evaluation Problem in Explainable AI: Identifying Reliable
  Estimators with MetaQuantus](https://arxiv.org/abs/2302.07265)** by HedstrÃ¶m
  et al., 2023. [![Getting started!](https://colab.research.google.com/assets/
  colab-badge.svg)](anonymous) ![Python version](https://img.shields.io/badge/
-  python-3.7%20%7C%203.8%20%7C%203.9-blue.svg) [![Code style: black](https://
- img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-  black) [![PyPI version](https://badge.fury.io/py/metaquantus.svg)](https://
-     badge.fury.io/py/metaquantus) [![Python package](https://github.com/
-  annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)]
+python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg) [![Code
+  style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+   (https://github.com/psf/black) [![PyPI version](https://badge.fury.io/py/
+  metaquantus.svg)](https://badge.fury.io/py/metaquantus) [![Python package]
     (https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-
-  publish.yml/badge.svg)  _MetaQuantus is currently under active development.
-Carefully note the release version to ensure reproducibility of your work._ ##
-Citation If you find this toolkit or its companion paper interesting or useful
-  in your research, use the following Bibtex annotation to cite us: ```bibtex
-@article{hedstrom2023metaquantus, author = {HedstrÃ¶m, Anna and Bommer, Philine
-and WickstrÃ¸m, Kristoffer K. and Samek, Wojciech and Lapuschkin, Sebastian and
-HÃ¶hne, Marina M. -C.}, title = {The Meta-Evaluation Problem in Explainable AI:
-      Identifying Reliable Estimators with MetaQuantus}, doi = {10.48550/
-   ARXIV.2302.07265}, url = {https://arxiv.org/abs/2302.07265}, publisher =
-{arXiv}, year = {2023}, } ``` ## Table of Contents 1. [Motivation](#motivation)
- 2. [Library](#library) 3. [Installation](#installation) 4. [Getting started]
- (#getting-started) 5. [MetaQuantus methodology](#metaquantus-methodology) 6.
-  [Reproduce the experiments](#reproduce-the-experiments) ## Motivation **The
- Evaluation Disagreement Problem.** In Explainable AI (XAI), the need of meta-
-evaluation (i.e., the process of evaluating the evaluation method) arises as we
-   select and quantitatively compare explanation methods for a given model,
- dataset and task---where the use of multiple metrics or evaluation techniques
-  oftentimes lead to conflicting results. For example, scores from different
-    metrics vary, both in range and direction, with lower or higher scores
- indicating higher quality explanations, making it difficult for practitioners
-to interpret the scores and select the best explanation method. As illustrated
- in the Figure below, the two metrics, Faithfulness Correlation (FC) (Bhatt_et
-     al.,_2020) and Pixel-Flipping (PF) (Bach_et_al.,_2015) rank the same
- explanation methods differently. For example, the Gradient method (MÃ¸rch_et
-  al.,_1995) (Baehrens_et_al.,_2010) is both ranked the highest (R=1) and the
+ publish.yml/badge.svg)](https://github.com/annahedstroem/MetaQuantus/actions/
+workflows/python-publish.yml/badge.svg)  _MetaQuantus is currently under active
+ development. Carefully note the release version to ensure reproducibility of
+    your work._ ## Citation If you find this toolkit or its companion paper
+interesting or useful in your research, use the following Bibtex annotation to
+cite us: ```bibtex @article{hedstrom2023metaquantus, author = {HedstrÃ¶m, Anna
+   and Bommer, Philine and WickstrÃ¸m, Kristoffer K. and Samek, Wojciech and
+Lapuschkin, Sebastian and HÃ¶hne, Marina M. -C.}, title = {The Meta-Evaluation
+ Problem in Explainable AI: Identifying Reliable Estimators with MetaQuantus},
+ doi = {10.48550/ARXIV.2302.07265}, url = {https://arxiv.org/abs/2302.07265},
+publisher = {arXiv}, year = {2023}, } ``` ## Table of Contents 1. [Motivation]
+   (#motivation) 2. [Library](#library) 3. [Installation](#installation) 4.
+[Getting started](#getting-started) 5. [MetaQuantus methodology](#metaquantus-
+  methodology) 6. [Reproduce the experiments](#reproduce-the-experiments) ##
+ Motivation **The Evaluation Disagreement Problem.** In Explainable AI (XAI),
+  the need of meta-evaluation (i.e., the process of evaluating the evaluation
+method) arises as we select and quantitatively compare explanation methods for
+    a given model, dataset and task---where the use of multiple metrics or
+  evaluation techniques oftentimes lead to conflicting results. For example,
+scores from different metrics vary, both in range and direction, with lower or
+ higher scores indicating higher quality explanations, making it difficult for
+ practitioners to interpret the scores and select the best explanation method.
+As illustrated in the Figure below, the two metrics, Faithfulness Correlation
+(FC) (Bhatt_et_al.,_2020) and Pixel-Flipping (PF) (Bach_et_al.,_2015) rank the
+same explanation methods differently. For example, the Gradient method (MÃ¸rch
+et_al.,_1995) (Baehrens_et_al.,_2010) is both ranked the highest (R=1) and the
  lowest (R=3) depending on the metric used. From a practitioner's perspective,
                             this causes confusion.
     [https://raw.githubusercontent.com/annahedstroem/MetaQuantus/main/fig1-
                                   cmnist.png]
 **Our Meta-Evaluation Approach.** With [MetaQuantus](https://github.com/
 annahedstroem/MetaQuantus), we address the problem of meta-evaluation by
 providing a simple yet comprehensive framework that evaluates metrics against
```

### Comparing `metaquantus-0.0.3/metaquantus/__init__.py` & `metaquantus-0.0.4/metaquantus/__init__.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/benchmarking.py` & `metaquantus-0.0.4/metaquantus/benchmarking.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 
                         self.results[dataset_name][model_name][estimator_category][
                             estimator_name
                         ] = {}
 
                         # Update attributes of master, make sure to save every run of master.
                         self.master.fname = f"{dataset_name}_{model_name}_{estimator_category}_{estimator_name}_{self.name}"
+                        self.master.return_aggregate = False
                         self.master.write_to_file = self.write_to_file
                         self.master.uid = uid
                         self.master.path = self.path + f"{dataset_name}/"
 
                         # Run full analysis.
                         self.master(
                             estimator=estimator[0],
```

### Comparing `metaquantus-0.0.3/metaquantus/helpers/__init__.py` & `metaquantus-0.0.4/metaquantus/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/helpers/configs.py` & `metaquantus-0.0.4/metaquantus/helpers/configs.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/helpers/models.py` & `metaquantus-0.0.4/metaquantus/helpers/models.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/helpers/plotting.py` & `metaquantus-0.0.4/metaquantus/helpers/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -862,18 +862,27 @@
 
     plt.tight_layout()
     if save:
         plt.savefig(
             path + "plots/" + f"benchmarking_scatter_bar_plots_combined.png", dpi=500
         )
     plt.show()
+
+
 from typing import Dict
 
+
 def plot_average_meta_evaluation_categories(
-    datasets: list, means: list, stds: list, metrics: list, colours: Dict, save: bool, path: str
+    datasets: list,
+    means: list,
+    stds: list,
+    metrics: list,
+    colours: Dict,
+    save: bool,
+    path: str,
 ) -> None:
     """
     Plot average MC scores for the different categoriees.
 
     Parameters
     ----------
     datasets: list
```

### Comparing `metaquantus-0.0.3/metaquantus/helpers/sanity_checks.py` & `metaquantus-0.0.4/metaquantus/helpers/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/helpers/utils.py` & `metaquantus-0.0.4/metaquantus/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/meta_evaluation.py` & `metaquantus-0.0.4/metaquantus/meta_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
                     else:
                         U.append(0)
                 else:
                     if q_star > q_hat:
                         U.append(1)
                     else:
                         U.append(0)
-        return float(np.mean(U))
+        return float(np.nanmean(U))
 
     @staticmethod
     def compute_iec_resilience(
         Q_star: np.array, Q_hat: np.array, indices: np.array
     ) -> float:
         """
         Return the mean of the agreement ranking matrix U \in [0, 1] to specify if the ranking condition is met.
@@ -828,15 +828,15 @@
             else:
                 for q_star, q_hat in zip(row_star, row_hat):
                     if q_star == q_hat:
                         U.append(1)
                     else:
                         U.append(0)
 
-        return float(np.mean(U))
+        return float(np.nanmean(U))
 
     """Getters."""
 
     def get_results_eval_scores(self):
         return self.results_eval_scores
 
     def get_results_eval_scores_perturbed(self):
```

### Comparing `metaquantus-0.0.3/metaquantus/perturbation_tests/__init__.py` & `metaquantus-0.0.4/metaquantus/perturbation_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/perturbation_tests/base.py` & `metaquantus-0.0.4/metaquantus/perturbation_tests/base.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/perturbation_tests/ipt.py` & `metaquantus-0.0.4/metaquantus/perturbation_tests/ipt.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus/perturbation_tests/mpt.py` & `metaquantus-0.0.4/metaquantus/perturbation_tests/mpt.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/metaquantus.egg-info/PKG-INFO` & `metaquantus-0.0.4/metaquantus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: metaquantus
-Version: 0.0.3
+Version: 0.0.4
 Summary: MetaQuantus is a XAI performance tool for identifying reliable metrics.
 Home-page: https://github.com/annahedstroem/MetaQuantus
 Author: Anna Hedstrom
 Author-email: hedstroem.anna@gmail.com
 License: GNU LESSER GENERAL PUBLIC LICENSE VERSION 3
 Keywords: explainable ai,evaluation,xai,machine learning,deep learning
-Requires-Python: >=3.7.1
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
 License-File: COPYING.LESSER
 
 <br/><br/>
 <p align="center">
   <img width="450" src="https://raw.githubusercontent.com/annahedstroem/MetaQuantus/main/logo.png">
@@ -19,15 +19,15 @@
 <h3 align="center"><b>An XAI performance tool for the identification of reliable metrics</b></h3>
 <p align="center">
   PyTorch
   
 This repository contains the code and experimental results for the paper **[The Meta-Evaluation Problem in Explainable AI: Identifying Reliable Estimators with MetaQuantus](https://arxiv.org/abs/2302.07265)** by Hedström et al., 2023.
 
 [![Getting started!](https://colab.research.google.com/assets/colab-badge.svg)](anonymous)
-![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9-blue.svg)
+![Python version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/metaquantus.svg)](https://badge.fury.io/py/metaquantus)
 [![Python package](https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)](https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)
 <!--[![Launch Tutorials](https://mybinder.org/badge_logo.svg)](anonymous)-->
 
 _MetaQuantus is currently under active development. Carefully note the release version to ensure reproducibility of your work._
```

#### html2text {}

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 2.1 Name: metaquantus Version: 0.0.3 Summary: MetaQuantus is
+Metadata-Version: 2.1 Name: metaquantus Version: 0.0.4 Summary: MetaQuantus is
 a XAI performance tool for identifying reliable metrics. Home-page: https://
 github.com/annahedstroem/MetaQuantus Author: Anna Hedstrom Author-email:
 hedstroem.anna@gmail.com License: GNU LESSER GENERAL PUBLIC LICENSE VERSION 3
 Keywords: explainable ai,evaluation,xai,machine learning,deep learning
-Requires-Python: >=3.7.1 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 COPYING License-File: COPYING.LESSER
 
   [https://raw.githubusercontent.com/annahedstroem/MetaQuantus/main/logo.png]
  **** An XAI performance tool for the identification of reliable metrics ****
   PyTorch This repository contains the code and experimental results for the
  paper **[The Meta-Evaluation Problem in Explainable AI: Identifying Reliable
  Estimators with MetaQuantus](https://arxiv.org/abs/2302.07265)** by HedstrÃ¶m
  et al., 2023. [![Getting started!](https://colab.research.google.com/assets/
  colab-badge.svg)](anonymous) ![Python version](https://img.shields.io/badge/
-  python-3.7%20%7C%203.8%20%7C%203.9-blue.svg) [![Code style: black](https://
- img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-  black) [![PyPI version](https://badge.fury.io/py/metaquantus.svg)](https://
-     badge.fury.io/py/metaquantus) [![Python package](https://github.com/
-  annahedstroem/MetaQuantus/actions/workflows/python-publish.yml/badge.svg)]
+python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg) [![Code
+  style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+   (https://github.com/psf/black) [![PyPI version](https://badge.fury.io/py/
+  metaquantus.svg)](https://badge.fury.io/py/metaquantus) [![Python package]
     (https://github.com/annahedstroem/MetaQuantus/actions/workflows/python-
-  publish.yml/badge.svg)  _MetaQuantus is currently under active development.
-Carefully note the release version to ensure reproducibility of your work._ ##
-Citation If you find this toolkit or its companion paper interesting or useful
-  in your research, use the following Bibtex annotation to cite us: ```bibtex
-@article{hedstrom2023metaquantus, author = {HedstrÃ¶m, Anna and Bommer, Philine
-and WickstrÃ¸m, Kristoffer K. and Samek, Wojciech and Lapuschkin, Sebastian and
-HÃ¶hne, Marina M. -C.}, title = {The Meta-Evaluation Problem in Explainable AI:
-      Identifying Reliable Estimators with MetaQuantus}, doi = {10.48550/
-   ARXIV.2302.07265}, url = {https://arxiv.org/abs/2302.07265}, publisher =
-{arXiv}, year = {2023}, } ``` ## Table of Contents 1. [Motivation](#motivation)
- 2. [Library](#library) 3. [Installation](#installation) 4. [Getting started]
- (#getting-started) 5. [MetaQuantus methodology](#metaquantus-methodology) 6.
-  [Reproduce the experiments](#reproduce-the-experiments) ## Motivation **The
- Evaluation Disagreement Problem.** In Explainable AI (XAI), the need of meta-
-evaluation (i.e., the process of evaluating the evaluation method) arises as we
-   select and quantitatively compare explanation methods for a given model,
- dataset and task---where the use of multiple metrics or evaluation techniques
-  oftentimes lead to conflicting results. For example, scores from different
-    metrics vary, both in range and direction, with lower or higher scores
- indicating higher quality explanations, making it difficult for practitioners
-to interpret the scores and select the best explanation method. As illustrated
- in the Figure below, the two metrics, Faithfulness Correlation (FC) (Bhatt_et
-     al.,_2020) and Pixel-Flipping (PF) (Bach_et_al.,_2015) rank the same
- explanation methods differently. For example, the Gradient method (MÃ¸rch_et
-  al.,_1995) (Baehrens_et_al.,_2010) is both ranked the highest (R=1) and the
+ publish.yml/badge.svg)](https://github.com/annahedstroem/MetaQuantus/actions/
+workflows/python-publish.yml/badge.svg)  _MetaQuantus is currently under active
+ development. Carefully note the release version to ensure reproducibility of
+    your work._ ## Citation If you find this toolkit or its companion paper
+interesting or useful in your research, use the following Bibtex annotation to
+cite us: ```bibtex @article{hedstrom2023metaquantus, author = {HedstrÃ¶m, Anna
+   and Bommer, Philine and WickstrÃ¸m, Kristoffer K. and Samek, Wojciech and
+Lapuschkin, Sebastian and HÃ¶hne, Marina M. -C.}, title = {The Meta-Evaluation
+ Problem in Explainable AI: Identifying Reliable Estimators with MetaQuantus},
+ doi = {10.48550/ARXIV.2302.07265}, url = {https://arxiv.org/abs/2302.07265},
+publisher = {arXiv}, year = {2023}, } ``` ## Table of Contents 1. [Motivation]
+   (#motivation) 2. [Library](#library) 3. [Installation](#installation) 4.
+[Getting started](#getting-started) 5. [MetaQuantus methodology](#metaquantus-
+  methodology) 6. [Reproduce the experiments](#reproduce-the-experiments) ##
+ Motivation **The Evaluation Disagreement Problem.** In Explainable AI (XAI),
+  the need of meta-evaluation (i.e., the process of evaluating the evaluation
+method) arises as we select and quantitatively compare explanation methods for
+    a given model, dataset and task---where the use of multiple metrics or
+  evaluation techniques oftentimes lead to conflicting results. For example,
+scores from different metrics vary, both in range and direction, with lower or
+ higher scores indicating higher quality explanations, making it difficult for
+ practitioners to interpret the scores and select the best explanation method.
+As illustrated in the Figure below, the two metrics, Faithfulness Correlation
+(FC) (Bhatt_et_al.,_2020) and Pixel-Flipping (PF) (Bach_et_al.,_2015) rank the
+same explanation methods differently. For example, the Gradient method (MÃ¸rch
+et_al.,_1995) (Baehrens_et_al.,_2010) is both ranked the highest (R=1) and the
  lowest (R=3) depending on the metric used. From a practitioner's perspective,
                             this causes confusion.
     [https://raw.githubusercontent.com/annahedstroem/MetaQuantus/main/fig1-
                                   cmnist.png]
 **Our Meta-Evaluation Approach.** With [MetaQuantus](https://github.com/
 annahedstroem/MetaQuantus), we address the problem of meta-evaluation by
 providing a simple yet comprehensive framework that evaluates metrics against
```

### Comparing `metaquantus-0.0.3/metaquantus.egg-info/SOURCES.txt` & `metaquantus-0.0.4/metaquantus.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 COPYING
 COPYING.LESSER
+MANIFEST.in
 README.md
+requirements.txt
+requirements_test.txt
 setup.py
 metaquantus/__init__.py
 metaquantus/benchmarking.py
 metaquantus/meta_evaluation.py
 metaquantus.egg-info/PKG-INFO
 metaquantus.egg-info/SOURCES.txt
 metaquantus.egg-info/dependency_links.txt
```

### Comparing `metaquantus-0.0.3/setup.py` & `metaquantus-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,34 @@
 # This file is part of MetaQuantus.
 # MetaQuantus is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 # MetaQuantus is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details.
 # You should have received a copy of the GNU Lesser General Public License along with MetaQuantus. If not, see <https://www.gnu.org/licenses/>.
 
-import importlib
 from setuptools import setup, find_packages
-from sys import version_info
-from importlib import util
 
-# Interpret the version of a package depending on if python>=3.8 vs python<3.8:
-# Read: https://stackoverflow.com/questions/20180543/how-to-check-version-of-python-modules?rq=1.
-if version_info[1] <= 7:
-    import pkg_resources
-
-    def version(s: str):
-        return pkg_resources.get_distribution(s).version
-
-else:
-    from importlib.metadata import version
+with open('requirements.txt') as f:
+    required = f.read().splitlines()
 
 # Define setup.
 setup(
     name="metaquantus",
-    version="0.0.3",
+    version="0.0.4",
     description="MetaQuantus is a XAI performance tool for identifying reliable metrics.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
-    install_requires=[
-        "quantus>=0.3.4",
-        "captum>=0.4.1",
-        "timm>=0.6.12",
-        "torch>=1.10.1",
-        "torchvision>=0.11.2",
-        "pandas>=1.3.5",
-    ],
-    # extras_require=EXTRAS,
+    install_requires=required,
     url="https://github.com/annahedstroem/MetaQuantus",
     author="Anna Hedstrom",
     author_email="hedstroem.anna@gmail.com",
     keywords=[
         "explainable ai",
         "evaluation",
         "xai",
         "machine learning",
         "deep learning",
     ],
     license="GNU LESSER GENERAL PUBLIC LICENSE VERSION 3",
     packages=find_packages(),
     zip_safe=False,
-    python_requires=">=3.7.1",
+    python_requires=">=3.8",
     include_package_data=True,
 )
```

### Comparing `metaquantus-0.0.3/tests/conftest.py` & `metaquantus-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/tests/test_benchmarking.py` & `metaquantus-0.0.4/tests/test_benchmarking.py`

 * *Files identical despite different names*

### Comparing `metaquantus-0.0.3/tests/test_meta_evaluation.py` & `metaquantus-0.0.4/tests/test_meta_evaluation.py`

 * *Files identical despite different names*

