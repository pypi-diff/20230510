# Comparing `tmp/doped-1.1.0.tar.gz` & `tmp/doped-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doped-1.1.0.tar", last modified: Tue May  9 22:29:43 2023, max compression
+gzip compressed data, was "doped-1.1.1.tar", last modified: Tue May  9 23:32:05 2023, max compression
```

## Comparing `doped-1.1.0.tar` & `doped-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.388530 doped-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 21:54:35.000000 doped-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-09 22:29:43.388530 doped-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-09 21:54:35.000000 doped-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.380529 doped-1.1.0/doped/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-09 21:54:35.000000 doped-1.1.0/doped/DefectSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-09 21:54:35.000000 doped-1.1.0/doped/HSE06_RelaxSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 21:54:35.000000 doped-1.1.0/doped/PBEsol_ConvergenceSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 21:54:35.000000 doped-1.1.0/doped/PotcarSet.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-05-09 21:54:35.000000 doped-1.1.0/doped/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    41977 2023-05-09 21:54:35.000000 doped-1.1.0/doped/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    71417 2023-05-09 21:54:35.000000 doped-1.1.0/doped/chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-05-09 21:54:35.000000 doped-1.1.0/doped/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    35271 2023-05-09 21:54:35.000000 doped-1.1.0/doped/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.380529 doped-1.1.0/doped/pycdt/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.384529 doped-1.1.0/doped/pycdt/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47141 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    43829 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/defectsmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.384529 doped-1.1.0/doped/pycdt/core/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/tests/test_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/tests/test_defectsmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.384529 doped-1.1.0/doped/pycdt/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53328 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/parse_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.384529 doped-1.1.0/doped/pycdt/utils/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/tests/test_parse_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/tests/test_vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)    40542 2023-05-09 21:54:35.000000 doped-1.1.0/doped/vasp_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.380529 doped-1.1.0/doped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-09 21:54:37.000000 doped-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:29:43.388530 doped-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.388530 doped-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-05-09 21:54:37.000000 doped-1.1.0/tests/test_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25523 2023-05-09 21:54:37.000000 doped-1.1.0/tests/test_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-09 21:54:37.000000 doped-1.1.0/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-09 21:54:37.000000 doped-1.1.0/tests/test_vasp_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.483678 doped-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 22:47:19.000000 doped-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-05-09 23:32:05.483678 doped-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-05-09 22:47:19.000000 doped-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.471678 doped-1.1.1/doped/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-09 22:47:19.000000 doped-1.1.1/doped/DefectSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-09 22:47:19.000000 doped-1.1.1/doped/HSE06_RelaxSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 22:47:19.000000 doped-1.1.1/doped/PBEsol_ConvergenceSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 22:47:19.000000 doped-1.1.1/doped/PotcarSet.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-05-09 22:47:19.000000 doped-1.1.1/doped/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41977 2023-05-09 22:47:19.000000 doped-1.1.1/doped/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71417 2023-05-09 22:47:19.000000 doped-1.1.1/doped/chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-05-09 22:47:19.000000 doped-1.1.1/doped/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35271 2023-05-09 22:47:19.000000 doped-1.1.1/doped/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.471678 doped-1.1.1/doped/pycdt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.475678 doped-1.1.1/doped/pycdt/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47141 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43829 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/defectsmaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.475678 doped-1.1.1/doped/pycdt/core/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/tests/test_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/core/tests/test_defectsmaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.479678 doped-1.1.1/doped/pycdt/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53328 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/parse_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.479678 doped-1.1.1/doped/pycdt/utils/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/tests/test_parse_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/tests/test_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-09 22:47:19.000000 doped-1.1.1/doped/pycdt/utils/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40542 2023-05-09 22:47:19.000000 doped-1.1.1/doped/vasp_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.471678 doped-1.1.1/doped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 23:32:05.000000 doped-1.1.1/doped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-09 22:47:21.000000 doped-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 23:32:05.483678 doped-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:32:05.483678 doped-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-05-09 22:47:21.000000 doped-1.1.1/tests/test_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25523 2023-05-09 22:47:21.000000 doped-1.1.1/tests/test_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-09 22:47:21.000000 doped-1.1.1/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-09 22:47:21.000000 doped-1.1.1/tests/test_vasp_input.py
```

### Comparing `doped-1.1.0/LICENSE` & `doped-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/PKG-INFO` & `doped-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <sean.kavanagh.19@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,19 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
+[![Build status](https://github.com/SMTG-UCL/doped/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/SMTG-UCL/doped/actions)
+[![PyPI](https://img.shields.io/pypi/v/doped)](https://pypi.org/project/doped)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/doped.svg)](https://anaconda.org/conda-forge/doped)
+[![Downloads](https://img.shields.io/pypi/dm/doped)](https://shakenbreak.readthedocs.io/en/latest/)
+
 # **D**efect **O**riented **P**ython **E**nvironment **D**istribution (`doped`)
 This is a (mid-development) Python package for managing solid-state defect calculations,
 geared toward VASP. Much of it is a modified version of the excellent [PyCDT](https://bitbucket.org/mbkumar/pycdt).  
 See [this link](https://www.sciencedirect.com/science/article/pii/S0010465518300079) for the original PyCDT paper.
 
 Defect formation energy plots are templated from [AIDE](https://github.com/SMTG-UCL/aide) and follow the aesthetics
 philosopy of [sumo](https://smtg-ucl.github.io/sumo/), both developed by the dynamic duo Adam Jackson and Alex Ganose.
```

### Comparing `doped-1.1.0/README.md` & `doped-1.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[![Build status](https://github.com/SMTG-UCL/doped/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/SMTG-UCL/doped/actions)
+[![PyPI](https://img.shields.io/pypi/v/doped)](https://pypi.org/project/doped)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/doped.svg)](https://anaconda.org/conda-forge/doped)
+[![Downloads](https://img.shields.io/pypi/dm/doped)](https://shakenbreak.readthedocs.io/en/latest/)
+
 # **D**efect **O**riented **P**ython **E**nvironment **D**istribution (`doped`)
 This is a (mid-development) Python package for managing solid-state defect calculations,
 geared toward VASP. Much of it is a modified version of the excellent [PyCDT](https://bitbucket.org/mbkumar/pycdt).  
 See [this link](https://www.sciencedirect.com/science/article/pii/S0010465518300079) for the original PyCDT paper.
 
 Defect formation energy plots are templated from [AIDE](https://github.com/SMTG-UCL/aide) and follow the aesthetics
 philosopy of [sumo](https://smtg-ucl.github.io/sumo/), both developed by the dynamic duo Adam Jackson and Alex Ganose.
```

### Comparing `doped-1.1.0/doped/DefectSet.yaml` & `doped-1.1.1/doped/DefectSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/PotcarSet.yaml` & `doped-1.1.1/doped/PotcarSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/__init__.py` & `doped-1.1.1/doped/__init__.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/analysis.py` & `doped-1.1.1/doped/analysis.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/chemical_potentials.py` & `doped-1.1.1/doped/chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/corrections.py` & `doped-1.1.1/doped/corrections.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/plotting.py` & `doped-1.1.1/doped/plotting.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/core/_chemical_potentials.py` & `doped-1.1.1/doped/pycdt/core/_chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/core/defectsmaker.py` & `doped-1.1.1/doped/pycdt/core/defectsmaker.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/core/tests/test_chemical_potentials.py` & `doped-1.1.1/doped/pycdt/core/tests/test_chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/core/tests/test_defectsmaker.py` & `doped-1.1.1/doped/pycdt/core/tests/test_defectsmaker.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/utils/parse_calculations.py` & `doped-1.1.1/doped/pycdt/utils/parse_calculations.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/utils/plotter.py` & `doped-1.1.1/doped/pycdt/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/utils/tests/test_parse_calculations.py` & `doped-1.1.1/doped/pycdt/utils/tests/test_parse_calculations.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/utils/tests/test_vasp.py` & `doped-1.1.1/doped/pycdt/utils/tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/pycdt/utils/vasp.py` & `doped-1.1.1/doped/pycdt/utils/vasp.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped/vasp_input.py` & `doped-1.1.1/doped/vasp_input.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/doped.egg-info/PKG-INFO` & `doped-1.1.1/doped.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <sean.kavanagh.19@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,19 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
+[![Build status](https://github.com/SMTG-UCL/doped/actions/workflows/build_and_test.yml/badge.svg)](https://github.com/SMTG-UCL/doped/actions)
+[![PyPI](https://img.shields.io/pypi/v/doped)](https://pypi.org/project/doped)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/doped.svg)](https://anaconda.org/conda-forge/doped)
+[![Downloads](https://img.shields.io/pypi/dm/doped)](https://shakenbreak.readthedocs.io/en/latest/)
+
 # **D**efect **O**riented **P**ython **E**nvironment **D**istribution (`doped`)
 This is a (mid-development) Python package for managing solid-state defect calculations,
 geared toward VASP. Much of it is a modified version of the excellent [PyCDT](https://bitbucket.org/mbkumar/pycdt).  
 See [this link](https://www.sciencedirect.com/science/article/pii/S0010465518300079) for the original PyCDT paper.
 
 Defect formation energy plots are templated from [AIDE](https://github.com/SMTG-UCL/aide) and follow the aesthetics
 philosopy of [sumo](https://smtg-ucl.github.io/sumo/), both developed by the dynamic duo Adam Jackson and Alex Ganose.
```

### Comparing `doped-1.1.0/doped.egg-info/SOURCES.txt` & `doped-1.1.1/doped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/pyproject.toml` & `doped-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "doped"
-version = "1.1.0"
+version = "1.1.1"
 description = "Python package to setup, process and analyse solid-state defect calculations with VASP"
 authors = [{name = "Seán Kavanagh", email = "sean.kavanagh.19@ucl.ac.uk"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `doped-1.1.0/tests/test_analysis.py` & `doped-1.1.1/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/tests/test_chemical_potentials.py` & `doped-1.1.1/tests/test_chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/tests/test_corrections.py` & `doped-1.1.1/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `doped-1.1.0/tests/test_vasp_input.py` & `doped-1.1.1/tests/test_vasp_input.py`

 * *Files identical despite different names*

