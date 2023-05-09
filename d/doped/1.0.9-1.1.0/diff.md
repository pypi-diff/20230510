# Comparing `tmp/doped-1.0.9.tar.gz` & `tmp/doped-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doped-1.0.9.tar", last modified: Fri Apr  7 11:48:49 2023, max compression
+gzip compressed data, was "doped-1.1.0.tar", last modified: Tue May  9 22:29:43 2023, max compression
```

## Comparing `doped-1.0.9.tar` & `doped-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.756421 doped-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-07 11:34:11.000000 doped-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-07 11:48:49.756421 doped-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-07 11:34:11.000000 doped-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.752421 doped-1.0.9/doped/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-07 11:34:11.000000 doped-1.0.9/doped/DefectSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-07 11:34:11.000000 doped-1.0.9/doped/HSE06_RelaxSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-07 11:34:11.000000 doped-1.0.9/doped/PBEsol_ConvergenceSet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-07 11:34:11.000000 doped-1.0.9/doped/PotcarSet.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2173 2023-04-07 11:34:11.000000 doped-1.0.9/doped/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-07 11:34:11.000000 doped-1.0.9/doped/aide_murphy_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-04-07 11:34:11.000000 doped-1.0.9/doped/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    69785 2023-04-07 11:34:11.000000 doped-1.0.9/doped/chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    35319 2023-04-07 11:34:11.000000 doped-1.0.9/doped/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.752421 doped-1.0.9/doped/pycdt/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.752421 doped-1.0.9/doped/pycdt/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46022 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/core/_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/core/defects_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    43509 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/core/defectsmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.756421 doped-1.0.9/doped/pycdt/core/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16095 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/core/tests/test_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/core/tests/test_defects_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/core/tests/test_defectsmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.756421 doped-1.0.9/doped/pycdt/corrections/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/finite_size_charge_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/freysoldt_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/ldau_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/sxdefect_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.756421 doped-1.0.9/doped/pycdt/corrections/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/tests/test_finite_size_charge_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/tests/test_ldau_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/corrections/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.756421 doped-1.0.9/doped/pycdt/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/log_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    65571 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/parse_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.756421 doped-1.0.9/doped/pycdt/utils/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/tests/test_log_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/tests/test_parse_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/tests/test_vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    22709 2023-04-07 11:34:11.000000 doped-1.0.9/doped/pycdt/utils/vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)    40678 2023-04-07 11:34:11.000000 doped-1.0.9/doped/vasp_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.752421 doped-1.0.9/doped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-04-07 11:48:49.000000 doped-1.0.9/doped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-07 11:48:49.000000 doped-1.0.9/doped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 11:48:49.000000 doped-1.0.9/doped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-07 11:48:49.000000 doped-1.0.9/doped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 11:48:49.000000 doped-1.0.9/doped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-07 11:34:13.000000 doped-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 11:48:49.756421 doped-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:48:49.756421 doped-1.0.9/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)    25523 2023-04-07 11:34:13.000000 doped-1.0.9/tests/test_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    22093 2023-04-07 11:34:13.000000 doped-1.0.9/tests/test_parse_calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-07 11:34:13.000000 doped-1.0.9/tests/test_vasp_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.388530 doped-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 21:54:35.000000 doped-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-09 22:29:43.388530 doped-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-09 21:54:35.000000 doped-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.380529 doped-1.1.0/doped/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-09 21:54:35.000000 doped-1.1.0/doped/DefectSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-09 21:54:35.000000 doped-1.1.0/doped/HSE06_RelaxSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-09 21:54:35.000000 doped-1.1.0/doped/PBEsol_ConvergenceSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 21:54:35.000000 doped-1.1.0/doped/PotcarSet.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2476 2023-05-09 21:54:35.000000 doped-1.1.0/doped/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    41977 2023-05-09 21:54:35.000000 doped-1.1.0/doped/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71417 2023-05-09 21:54:35.000000 doped-1.1.0/doped/chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-05-09 21:54:35.000000 doped-1.1.0/doped/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35271 2023-05-09 21:54:35.000000 doped-1.1.0/doped/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.380529 doped-1.1.0/doped/pycdt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.384529 doped-1.1.0/doped/pycdt/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47141 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43829 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/defectsmaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.384529 doped-1.1.0/doped/pycdt/core/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/tests/test_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/core/tests/test_defectsmaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.384529 doped-1.1.0/doped/pycdt/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53328 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/parse_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.384529 doped-1.1.0/doped/pycdt/utils/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/tests/test_parse_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/tests/test_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-09 21:54:35.000000 doped-1.1.0/doped/pycdt/utils/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40542 2023-05-09 21:54:35.000000 doped-1.1.0/doped/vasp_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.380529 doped-1.1.0/doped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 22:29:43.000000 doped-1.1.0/doped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-09 21:54:37.000000 doped-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:29:43.388530 doped-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:29:43.388530 doped-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-05-09 21:54:37.000000 doped-1.1.0/tests/test_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25523 2023-05-09 21:54:37.000000 doped-1.1.0/tests/test_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-09 21:54:37.000000 doped-1.1.0/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-09 21:54:37.000000 doped-1.1.0/tests/test_vasp_input.py
```

### Comparing `doped-1.0.9/LICENSE` & `doped-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doped-1.0.9/PKG-INFO` & `doped-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <sean.kavanagh.19@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # **D**efect **O**riented **P**ython **E**nvironment **D**istribution (`doped`)
 This is a (mid-development) Python package for managing solid-state defect calculations,
 geared toward VASP. Much of it is a modified version of the excellent [PyCDT](https://bitbucket.org/mbkumar/pycdt).  
@@ -62,26 +62,30 @@
 - Because of breaking changes made to the `pymatgen` defects code in version `2022.8.23`, `doped` requires 
 `pymatgen<2022.8.23`, which is installed automatically when installing `doped`. 
 However, as discussed briefly below and in the example notebooks, the 
 [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach is highly recommended when calculating 
 defects in solids, and this package has been updated to be compatible with the latest version of `pymatgen`.
 As such, it is recommended to install `doped` in a virtual python environment as follows:
 
-1. 
+1. Create virtual environment and install: 
 ```bash
-conda create -n doped  # create conda environment named doped
+conda create -n doped python=3.10  # create conda environment named doped
 conda activate doped  # activate doped conda environment
-pip install doped  # install doped package and dependencies
+pip install doped  # install doped and dependencies, can also  
+pip install numpy --upgrade # upgrade numpy to avoid binary incompatibility
 ```
 And then use this environment whenever using `doped`.
-Instead of `conda` you can also use `venv` to setup virtual environments, 
-see [here](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/) for more.
+Alternatively if desired, `doped` can also be installed from `conda` with:
+
+```bash
+  conda install -c conda-forge doped
+```
 
 If you want to use the [example files](examples), 
-you should clone the repository and install with `pip install -e .` from the `doped` directory.
+you should clone the repository and install with `pip install -e .` from the `doped` directory, but still make sure to `pip install numpy --upgrade`.
 
 2. (If not set) Set the VASP pseudopotential directory and your Materials Project API key in `$HOME/.pmgrc.yaml` 
 (`pymatgen` config file) as follows:
 ```bash
   PMG_VASP_PSP_DIR: <Path to VASP pseudopotential top directory>
   PMG_MAPI_KEY: <Your MP API key obtained from https://legacy.materialsproject.org/open>
 ```
@@ -99,24 +103,26 @@
 pmg config -p temp_potcars psp_resources  # configure the psp_resources pymatgen POTCAR directory
 pmg config --add PMG_VASP_PSP_DIR "${PWD}/psp_resources"  # add the POTCAR directory to pymatgen's config file (`$HOME/.pmgrc.yaml`)
 rm -r temp_potcars  # remove the temporary POTCAR directory
 ```
 If this has been successful, you should be able to run `pmg potcar -s Na_pv`, and `grep PBE POTCAR` should show 
 `PAW_PBE Na_pv {date}` (you can ignore any `pymatgen` warnings about recognising the `POTCAR`). 
 
+If it does not work check that the `PMG_DEFAULT_FUNCTIONAL` is set to whatever your functionals are (e.g. `PBE` or `PBE_54`)
+
 This is necessary to generate `POTCAR` input files, and auto-determine `INCAR` settings such as `NELECT` for charged 
 defects.
 
 The Materials Project API key is required for determining the necessary competing phases to calculate in order to 
 determine the chemical potential limits (required for defect formation energies). This should correspond to the legacy 
 MP API, with your unique key available at: https://legacy.materialsproject.org/open.
 
 
 ## `ShakeNBreak`
-As shown in the example notebook, it is highly recommended to use the [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects in solids, to ensure you have identified the groundstate structures of your defects. As detailed in the [theory paper](https://arxiv.org/abs/2207.09862), skipping this step can result in drastically incorrect formation energies, transition levels, carrier capture (basically any property associated with defects). This approach is followed in the [doped example notebook](https://github.com/SMTG-UCL/doped/blob/master/dope_Example_Notebook.ipynb), with a more in-depth explanation and tutorial given on the [ShakeNBreak](https://shakenbreak.readthedocs.io/en/latest/) website.
+As shown in the example notebook, it is highly recommended to use the [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects in solids, to ensure you have identified the groundstate structures of your defects. As detailed in the [theory paper](https://arxiv.org/abs/2207.09862), skipping this step can result in drastically incorrect formation energies, transition levels, carrier capture (basically any property associated with defects). This approach is followed in the [doped example notebook](https://github.com/SMTG-UCL/doped/blob/master/dope_workflow_example.ipynb), with a more in-depth explanation and tutorial given on the [ShakeNBreak](https://shakenbreak.readthedocs.io/en/latest/) website.
 
 Summary GIF:
 ![ShakeNBreak Summary](files/SnB_Supercell_Schematic_PES_2sec_Compressed.gif)
 
 `SnB` CLI Usage:
 ![ShakeNBreak CLI](files/SnB_CLI.gif)
```

### Comparing `doped-1.0.9/README.md` & `doped-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,30 @@
 - Because of breaking changes made to the `pymatgen` defects code in version `2022.8.23`, `doped` requires 
 `pymatgen<2022.8.23`, which is installed automatically when installing `doped`. 
 However, as discussed briefly below and in the example notebooks, the 
 [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach is highly recommended when calculating 
 defects in solids, and this package has been updated to be compatible with the latest version of `pymatgen`.
 As such, it is recommended to install `doped` in a virtual python environment as follows:
 
-1. 
+1. Create virtual environment and install: 
 ```bash
-conda create -n doped  # create conda environment named doped
+conda create -n doped python=3.10  # create conda environment named doped
 conda activate doped  # activate doped conda environment
-pip install doped  # install doped package and dependencies
+pip install doped  # install doped and dependencies, can also  
+pip install numpy --upgrade # upgrade numpy to avoid binary incompatibility
 ```
 And then use this environment whenever using `doped`.
-Instead of `conda` you can also use `venv` to setup virtual environments, 
-see [here](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/) for more.
+Alternatively if desired, `doped` can also be installed from `conda` with:
+
+```bash
+  conda install -c conda-forge doped
+```
 
 If you want to use the [example files](examples), 
-you should clone the repository and install with `pip install -e .` from the `doped` directory.
+you should clone the repository and install with `pip install -e .` from the `doped` directory, but still make sure to `pip install numpy --upgrade`.
 
 2. (If not set) Set the VASP pseudopotential directory and your Materials Project API key in `$HOME/.pmgrc.yaml` 
 (`pymatgen` config file) as follows:
 ```bash
   PMG_VASP_PSP_DIR: <Path to VASP pseudopotential top directory>
   PMG_MAPI_KEY: <Your MP API key obtained from https://legacy.materialsproject.org/open>
 ```
@@ -57,24 +61,26 @@
 pmg config -p temp_potcars psp_resources  # configure the psp_resources pymatgen POTCAR directory
 pmg config --add PMG_VASP_PSP_DIR "${PWD}/psp_resources"  # add the POTCAR directory to pymatgen's config file (`$HOME/.pmgrc.yaml`)
 rm -r temp_potcars  # remove the temporary POTCAR directory
 ```
 If this has been successful, you should be able to run `pmg potcar -s Na_pv`, and `grep PBE POTCAR` should show 
 `PAW_PBE Na_pv {date}` (you can ignore any `pymatgen` warnings about recognising the `POTCAR`). 
 
+If it does not work check that the `PMG_DEFAULT_FUNCTIONAL` is set to whatever your functionals are (e.g. `PBE` or `PBE_54`)
+
 This is necessary to generate `POTCAR` input files, and auto-determine `INCAR` settings such as `NELECT` for charged 
 defects.
 
 The Materials Project API key is required for determining the necessary competing phases to calculate in order to 
 determine the chemical potential limits (required for defect formation energies). This should correspond to the legacy 
 MP API, with your unique key available at: https://legacy.materialsproject.org/open.
 
 
 ## `ShakeNBreak`
-As shown in the example notebook, it is highly recommended to use the [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects in solids, to ensure you have identified the groundstate structures of your defects. As detailed in the [theory paper](https://arxiv.org/abs/2207.09862), skipping this step can result in drastically incorrect formation energies, transition levels, carrier capture (basically any property associated with defects). This approach is followed in the [doped example notebook](https://github.com/SMTG-UCL/doped/blob/master/dope_Example_Notebook.ipynb), with a more in-depth explanation and tutorial given on the [ShakeNBreak](https://shakenbreak.readthedocs.io/en/latest/) website.
+As shown in the example notebook, it is highly recommended to use the [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects in solids, to ensure you have identified the groundstate structures of your defects. As detailed in the [theory paper](https://arxiv.org/abs/2207.09862), skipping this step can result in drastically incorrect formation energies, transition levels, carrier capture (basically any property associated with defects). This approach is followed in the [doped example notebook](https://github.com/SMTG-UCL/doped/blob/master/dope_workflow_example.ipynb), with a more in-depth explanation and tutorial given on the [ShakeNBreak](https://shakenbreak.readthedocs.io/en/latest/) website.
 
 Summary GIF:
 ![ShakeNBreak Summary](files/SnB_Supercell_Schematic_PES_2sec_Compressed.gif)
 
 `SnB` CLI Usage:
 ![ShakeNBreak CLI](files/SnB_CLI.gif)
```

### Comparing `doped-1.0.9/doped/PotcarSet.yaml` & `doped-1.1.0/doped/PotcarSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-1.0.9/doped/__init__.py` & `doped-1.1.0/doped/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import warnings
 from datetime import date
 from importlib.metadata import PackageNotFoundError, version
+from packaging.version import parse
 
 from pymatgen.io.vasp.inputs import UnknownPotcarWarning
+from pymatgen.io.vasp.sets import BadInputSetWarning
 
 if date.today().weekday() in [5, 6]:
     print("""Working on the weekend, like usual...\n""")
 if date.today().weekday() == 5:
     print("Seriously though, everyone knows Saturday's for the boys/girls...\n")
 
 
@@ -24,33 +26,42 @@
     if v_pmg_def:
         raise TypeError(
             "You have the `pymatgen-analysis-defects` package installed, which is currently "
             "incompatible with `doped`. Please uninstall `pymatgen-analysis-defects` (with `pip "
             "uninstall pymatgen-analysis-defects`) and restart the kernel."
         )
 
-    if v_pmg > "2022.7.25":
+    if parse(v_pmg) > parse("2022.7.25"):
         raise TypeError(
             f"You have the version {v_pmg} of `pymatgen` installed, which is currently "
             f"incompatible with `doped`. Please revert this package (with `pip install "
             f"pymatgen==2022.7.25`) and restart the kernel."
         )
 
 
 _check_pmg_compatibility()
 
-# globally ignore these POTCAR warnings
-warnings.filterwarnings("ignore", category=UnknownPotcarWarning)
-warnings.filterwarnings("ignore", message="No POTCAR file with matching TITEL fields")
-warnings.filterwarnings("ignore", message="Ignoring unknown variable type")
-warnings.filterwarnings(
+
+def _ignore_pmg_warnings():
+    # globally ignore these POTCAR warnings
+    warnings.filterwarnings("ignore", category=UnknownPotcarWarning)
+    warnings.filterwarnings("ignore", category=BadInputSetWarning)
+    warnings.filterwarnings(
+        "ignore", message="No POTCAR file with matching TITEL fields"
+    )
+    warnings.filterwarnings("ignore", message="Ignoring unknown variable type")
+    warnings.filterwarnings(
         "ignore", message="POTCAR data with symbol"
     )  # Ignore POTCAR warnings because Pymatgen incorrectly detecting POTCAR types
-# Ignore because comment after 'ALGO = Normal' causes this unnecessary warning:
-warnings.filterwarnings("ignore", message="Hybrid functionals only support")
+    # Ignore because comment after 'ALGO = Normal' causes this unnecessary warning:
+    warnings.filterwarnings("ignore", message="Hybrid functionals only support")
+
+    # until updated from pymatgen==2022.7.25 :
+    warnings.filterwarnings(
+        "ignore", message="Using `tqdm.autonotebook.tqdm` in notebook mode"
+    )
+    warnings.filterwarnings(
+        "ignore", message="`np.int` is a deprecated alias for the builtin `int`"
+    )
+    warnings.filterwarnings("ignore", message="Use get_magnetic_symmetry()")
 
-# until updated from pymatgen==2022.7.25 :
-warnings.filterwarnings(
-    "ignore", message="Using `tqdm.autonotebook.tqdm` in notebook mode"
-)
-warnings.filterwarnings("ignore", message="`np.int` is a deprecated alias for the builtin `int`")
-warnings.filterwarnings("ignore", message="Use get_magnetic_symmetry()")
+_ignore_pmg_warnings()
```

### Comparing `doped-1.0.9/doped/chemical_potentials.py` & `doped-1.1.0/doped/chemical_potentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pymatgen.core import Composition, Element, Structure
 from pymatgen.entries.computed_entries import ComputedStructureEntry
 from pymatgen.ext.matproj import MPRester
 from pymatgen.io.vasp.inputs import Kpoints, UnknownPotcarWarning
 from pymatgen.io.vasp.outputs import Vasprun
 from pymatgen.io.vasp.sets import BadInputSetWarning, DictSet
 
-from doped.pycdt.utils.parse_calculations import get_vasprun
+from doped.pycdt.utils.parse_calculations import _get_output_files_and_check_if_multiple
 
 MODULE_DIR = os.path.dirname(os.path.abspath(__file__))
 default_potcar_dict = loadfn(os.path.join(MODULE_DIR, "PotcarSet.yaml"))
 
 # globally ignore:
 warnings.filterwarnings("ignore", category=BadInputSetWarning)
 warnings.filterwarnings("ignore", category=UnknownPotcarWarning)
@@ -31,15 +31,16 @@
 )  # currently rely on this so shouldn't show warning
 warnings.filterwarnings("ignore", message="Ignoring unknown variable type")
 
 
 # TODO: Check default error when user attempts `CompetingPhases()` with no API key setup; if not
 #  sufficiently informative, add try except catch to give more informative error message for this.
 # TODO: Need to recheck all functionality from old `_chemical_potentials.py` is now present here.
-# TODO: Add chemical potential diagram plotting functionality that we had before with `plot_cplap_ternary`.
+# TODO: Add chemical potential diagram plotting functionality that we had before
+#  with `plot_cplap_ternary`.
 
 
 def make_molecule_in_a_box(element):
     # (but do try to fix it so that the nupdown is the same as magnetisation
     # so that it makes that assignment easier later on when making files)
     # the bond distances are taken from various sources and *not* thoroughly vetted
     lattice = [[30, 0, 0], [0, 30, 0], [0, 0, 30]]
@@ -621,14 +622,15 @@
         for e in self.molecules:  # gamma-only for molecules
             if user_incar_settings is not None:
                 uis = copy.deepcopy(user_incar_settings)
             else:
                 uis = {}
 
             uis["ISIF"] = 2  # can't change the volume
+            uis["KPAR"] = 1  # can't use k-point parallelization, gamma only
 
             if e.data["total_magnetization"] > 0.1:  # account for magnetic moment
                 if "ISPIN" not in uis:
                     uis["ISPIN"] = 2
                 if "NUPDOWN" not in uis and int(e.data["total_magnetization"]) > 0:
                     uis["NUPDOWN"] = int(e.data["total_magnetization"])
 
@@ -1050,19 +1052,21 @@
             self.elemental.append(extrinsic_species)
 
     def from_vaspruns(self, path="competing_phases", folder="vasp_std", csv_fname=None):
         """
         Reads in vaspruns, collates energies to csv.
 
         Args:
-            path (list, str, pathlib Path): Either a list of strings or Paths to vasprun.xml(.gz)
-            files, or a path to the base folder in which you have your
-            formula_EaH_/vasp_std/vasprun.xml
-            folder (str): The folder in which vasprun is, only use if you set base path
-            (i.e. change to vasp_ncl or if vaspruns are in the formula_EaH folder).
+            path (list, str, pathlib Path): Either a path to the base folder in which you have your
+                competing phase calculation outputs (e.g. formula_EaH_X/vasp_std/vasprun.xml(
+                .gz), or formula_EaH_X/vasprun.xml(.gz)), or a list of strings or Paths to
+                vasprun.xml(.gz) files.
+            folder (str): The subfolder in which your vasprun.xml output files are located (e.g.
+                a file-structure like: formula_EaH_X/{folder}/vasprun.xml(.gz)). Default is to
+                search for `vasp_std` subfolders, or directly in the `formula_EaH_X` folder.
             csv_fname (str): If set will save to csv with this name
         Returns:
             None, sets self.data and self.elemental_energies
         """
         # TODO: Change this to just recursively search for vaspruns within the specified path
         # TODO: Add check for matching INCAR and POTCARs from these calcs, as we also want with
         #  defect parsing
@@ -1085,36 +1089,52 @@
                     )
 
         # if path provided points to the doped created directories
         elif isinstance(path, (PurePath, str)):
             path = Path(path)
             for p in path.iterdir():
                 if p.glob("EaH"):
-                    vp = p / folder / "vasprun.xml"
-                    try:
-                        vr, vr_path = get_vasprun(vp)
+                    # add bulk simple properties
+                    vr_path, multiple = _get_output_files_and_check_if_multiple(
+                        "vasprun.xml", p / folder
+                    )
+                    if multiple:
+                        warnings.warn(
+                            f"Multiple `vasprun.xml` files found in directory: {p/folder}. Using "
+                            f"{vr_path} to parse the calculation energy and metadata."
+                        )
+
+                    if os.path.exists(vr_path):
                         self.vasprun_paths.append(vr_path)
 
-                    except FileNotFoundError:
-                        try:
-                            vp = p / "vasprun.xml"
-                            vr, vr_path = get_vasprun(vp)
+                    else:
+                        vr_path, multiple = _get_output_files_and_check_if_multiple(
+                            "vasprun.xml", p
+                        )
+                        if multiple:
+                            warnings.warn(
+                                f"Multiple `vasprun.xml` files found in directory: {p}. Using "
+                                f"{vr_path} to parse the calculation energy and metadata."
+                            )
+
+                        if os.path.exists(vr_path):
                             self.vasprun_paths.append(vr_path)
 
-                        except FileNotFoundError:
-                            print(
-                                f"Can't find a vasprun.xml(.gz) file in {p} or {p/folder}, "
+                        else:
+                            warnings.warn(
+                                f"Can't find a vasprun.xml file in {p} or {p/folder}, "
                                 f"proceed with caution"
                             )
                             continue
 
                 else:
                     raise FileNotFoundError(
                         "Folders are not in the correct structure, provide them as a list of "
-                        "paths (or strings)"
+                        "paths (or strings). Competing phase folders should have `EaH` in the "
+                        "folder name."
                     )
 
         else:
             raise ValueError(
                 "Path should either be a list of paths, a string or a pathlib Path object"
             )
 
@@ -1224,32 +1244,38 @@
         """
 
         intrinsic_phase_diagram_entries = []
         extrinsic_formation_energies = []
         bulk_pde_list = []
         for d in self.data:
             e = PDEntry(d["formula"], d["energy_per_fu"])
-            # presumably checks if the phase is intrinsic
+            # checks if the phase is intrinsic
             if set(Composition(d["formula"]).elements).issubset(
                 self.bulk_composition.elements
             ):
                 intrinsic_phase_diagram_entries.append(e)
                 if e.composition == self.bulk_composition:  # bulk phase
                     bulk_pde_list.append(e)
             else:
                 extrinsic_formation_energies.append(
                     {"formula": d["formula"], "formation_energy": d["formation_energy"]}
                 )
 
         if len(bulk_pde_list) == 0:
+            if len(intrinsic_phase_diagram_entries) == 0:
+                intrinsic_phase_diagram_compositions = None
+            else:
+                intrinsic_phase_diagram_compositions = {
+                    e.composition.reduced_formula
+                    for e in intrinsic_phase_diagram_entries
+                }
             raise ValueError(
                 f"Could not find bulk phase for "
                 f"{self.bulk_composition.reduced_formula} in the supplied data. "
-                f"Found phases: "
-                f"{ {e.composition.reduced_formula for e in intrinsic_phase_diagram_entries} }"
+                f"Found phases: {intrinsic_phase_diagram_entries}"
             )
         if len(bulk_pde_list) > 0:
             # lowest energy bulk phase
             self.bulk_pde = sorted(bulk_pde_list, key=lambda x: x.energy_per_atom)[0]
 
         self._intrinsic_phase_diagram = PhaseDiagram(
             intrinsic_phase_diagram_entries,
@@ -1316,14 +1342,15 @@
                     e[el] = Composition(e["formula"]).as_dict()[el]
 
             # gets the df into a slightly more convenient dict
             cpd = df.to_dict(orient="records")
             mins = []
             mins_formulas = []
             df3 = pd.DataFrame(extrinsic_formation_energies)
+            print(f"df3: {df3}")
             for i, c in enumerate(cpd):
                 name = f"mu_{self.extrinsic_species}_{i}"
                 df3[name] = df3["formation_energy"]
                 for k, v in c.items():
                     df3[name] -= df3[k] * v
                 df3[name] /= df3[self.extrinsic_species]
                 # find min at that chempot
@@ -1351,26 +1378,30 @@
             # reverse engineer chem lims for extrinsic
             df4 = df.copy().to_dict(orient="records")
             cl2 = {
                 "elemental_refs": self.elemental_energies,
                 "facets_wrt_el_refs": {},
                 "facets": {},
             }
+            print(f"df4: {df4}")
 
             for i, d in enumerate(df4):
                 key = (
                     list(self._intrinsic_chem_limits["facets_wrt_el_refs"].keys())[i]
                     + "-"
                     + d[col_name]
                 )
+                print(f"key: {key}")  # TODO: Remove any unnecessary print statements when this
+                # has been fixed
                 new_vals = list(
                     self._intrinsic_chem_limits["facets_wrt_el_refs"].values()
                 )[i]
                 new_vals[f"{self.extrinsic_species}"] = d[f"{self.extrinsic_species}"]
                 cl2["facets_wrt_el_refs"][key] = new_vals
+            print(f"cl2: {cl2}")
 
             # relate the facets to the elemental
             # energies but in reverse this time
             for facet, chempot_dict in cl2["facets_wrt_el_refs"].items():
                 relative_chempot_dict = copy.deepcopy(chempot_dict)
                 for e in relative_chempot_dict.keys():
                     relative_chempot_dict[e] += cl2["elemental_refs"][e]
```

### Comparing `doped-1.0.9/doped/plotting.py` & `doped-1.1.0/doped/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Jackson and Alex Ganose), alongside substantial modification, in the efforts of making an
 efficient, user-friendly package for managing and analysing defect calculations,
 with publication-quality outputs
 """
 
 import warnings
 
-from matplotlib import cm, ticker, rc
+from matplotlib import cm, ticker, rc, colormaps
 import matplotlib.pyplot as plt
 import numpy as np
 from pymatgen.util.string import latexify
 
 default_fonts = [
     "Whitney Book Extended",
     "Whitney Pro",
@@ -25,19 +25,19 @@
     "Andale Sans",
 ]
 
 
 # TODO: Lean out the options for this function (inherited from AIDE)(particularly those that can
 #  just be edited by the user with the returned Matplotlib object – show example of this in
 #  notebooks maybe?)
+# TOOD: Add option to only plot defect states that are stable at some point in the bandgap
 def formation_energy_plot(
     defect_phase_diagram,
     chempot_limits: dict = None,
     elt_refs: dict = None,
-    ax=None,
     fonts=None,
     xlim=None,
     ylim=None,
     ax_fontsize=1.0,
     lg_fontsize=1.0,
     lg_position=None,
     fermi_level=None,
@@ -114,15 +114,14 @@
             else:
                 plot_filename = plot_title + "_" + facet + ".pdf"
 
             plot = _aide_pmg_plot(
                 defect_phase_diagram,
                 mu_elts=mu_elts,
                 elt_refs=elt_refs,
-                ax=ax,
                 fonts=fonts,
                 xlim=xlim,
                 ylim=ylim,
                 ax_fontsize=ax_fontsize,
                 lg_fontsize=lg_fontsize,
                 lg_position=lg_position,
                 fermi_level=fermi_level,
@@ -139,15 +138,14 @@
         return plot
 
     # Else if you only want to give {Elt: Energy} dict for chempot_limits, or no chempot_limits
     return _aide_pmg_plot(
         defect_phase_diagram,
         mu_elts=chempot_limits,
         elt_refs=elt_refs,
-        ax=ax,
         fonts=fonts,
         xlim=xlim,
         ylim=ylim,
         ax_fontsize=ax_fontsize,
         lg_fontsize=lg_fontsize,
         lg_position=lg_position,
         fermi_level=fermi_level,
@@ -162,15 +160,14 @@
     )
 
 
 def _aide_pmg_plot(
     defect_phase_diagram,
     mu_elts=None,
     elt_refs=None,
-    ax=None,
     fonts=None,
     xlim=None,
     ylim=None,
     ax_fontsize=1.0,
     lg_fontsize=1.0,
     lg_position=None,
     fermi_level=None,
@@ -295,28 +292,28 @@
             for x_window in xlim:
                 y_range_vals.append(
                     chg_ent.formation_energy(
                         chemical_potentials=mu_elts, fermi_level=x_window
                     )
                 )
 
-    cmap = cm.get_cmap(colormap)
+    cmap = colormaps[colormap]
     colors = cmap(np.linspace(0, 1, len(xy)))
     if colormap == "Dark2" and len(xy) >= 8:
         warnings.warn(
             f"""
 The chosen colormap is Dark2, which only has 8 colours, yet you have {len(xy)} defect species (so
 some defects will have the same line colour). Recommended to change/set colormap to 'tab10' or
 'tab20' (10 and 20 colours each)."""
         )
     plt.figure(dpi=600, figsize=(2.6, 1.95))  # Gives a final figure width of c. 3.5
     # inches, the standard single column width for publication (which is what we're about)
     plt.clf()
     width = 9
-    ax = pretty_axis(ax=ax, fonts=fonts)
+    ax = pretty_axis(fonts=fonts)
     # plot formation energy lines
     for_legend = []
     for cnt, defnom in enumerate(xy.keys()):
         ax.plot(
             xy[defnom][0],
             xy[defnom][1],
             color=colors[cnt],
@@ -616,15 +613,14 @@
     return ax
 
 
 def all_lines_formation_energy_plot(
     defect_phase_diagram,
     chempot_limits=None,
     elt_refs: dict = None,
-    ax=None,
     fonts=None,
     xlim=None,
     ylim=None,
     ax_fontsize=1.0,
     lg_fontsize=1.0,
     lg_position=None,
     fermi_level=None,
@@ -701,15 +697,14 @@
             else:
                 plot_title = facet
 
             return _all_lines_aide_pmg_plot(
                 defect_phase_diagram,
                 mu_elts=mu_elts,
                 elt_refs=elt_refs,
-                ax=ax,
                 fonts=fonts,
                 xlim=xlim,
                 ylim=ylim,
                 ax_fontsize=ax_fontsize,
                 lg_fontsize=lg_fontsize,
                 lg_position=lg_position,
                 fermi_level=fermi_level,
@@ -722,15 +717,14 @@
                 filename=plot_filename,
             )
     else:  # If you only want to give {Elt: Energy} dict for chempot_limits, or no chempot_limits
         return _all_lines_aide_pmg_plot(
             defect_phase_diagram,
             mu_elts=chempot_limits,
             elt_refs=elt_refs,
-            ax=ax,
             fonts=fonts,
             xlim=xlim,
             ylim=ylim,
             ax_fontsize=ax_fontsize,
             lg_fontsize=lg_fontsize,
             lg_position=lg_position,
             fermi_level=fermi_level,
@@ -744,15 +738,14 @@
         )
 
 
 def _all_lines_aide_pmg_plot(
     defect_phase_diagram,
     mu_elts=None,
     elt_refs=None,
-    ax=None,
     fonts=None,
     xlim=None,
     ylim=None,
     ax_fontsize=1.0,
     lg_fontsize=1.0,
     lg_position=None,
     fermi_level=None,
@@ -844,28 +837,28 @@
         for x_window in xlim:
             y_range_vals.append(
                 chg_ent.formation_energy(
                     chemical_potentials=mu_elts, fermi_level=x_window
                 )
             )
 
-    cmap = cm.get_cmap(colormap)
+    cmap = colormaps[colormap]
     colors = cmap(np.linspace(0, 1, len(xy)))
     if colormap == "Dark2" and len(xy) >= 8:
         warnings.warn(
             f"""
 The chosen colormap is Dark2, which only has 8 colours, yet you have {len(xy)} defect species (so
 some defects will have the same line colour). Recommended to change/set colormap to 'tab10' or
 'tab20' (10 and 20 colours each)."""
         )
     plt.figure(dpi=600, figsize=(2.6, 1.95))  # Gives a final figure width of c. 3.5
     # inches, the standard single column width for publication (which is what we're about)
     plt.clf()
     width = 9
-    ax = pretty_axis(ax=ax, fonts=fonts)
+    ax = pretty_axis(fonts=fonts)
     # plot formation energy lines
 
     for cnt, def_name in enumerate(xy.keys()):
         ax.plot(
             xy[def_name][0],
             xy[def_name][1],
             color=colors[cnt],
```

### Comparing `doped-1.0.9/doped/pycdt/core/_chemical_potentials.py` & `doped-1.1.0/doped/pycdt/core/_chemical_potentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 """
 A class for performing analysis of chemical potentials with the grand
 canonical linear programming approach
 """
 from __future__ import division
 
 import copy
-import logging
 import os
+import warnings
 
 from pymatgen.analysis.phase_diagram import PDEntry, PhaseDiagram
-from pymatgen.core.structure import Element, Structure
+from pymatgen.core.structure import Element, Structure, Composition
 from pymatgen.entries.computed_entries import ComputedStructureEntry
 from pymatgen.ext.matproj import MPRester
 
 
 def get_mp_chempots_from_dpd(dpd):
     """
     Grab Materials Project chemical potentials from a pymatgen DefectPhaseDiagram object
@@ -68,22 +68,19 @@
         Args:
             bulk_ce: Pymatgen ComputedStructureEntry object for
                 bulk entry / supercell
         """
         self.bulk_ce = kwargs.get("bulk_ce", None)
 
     def get_chempots_from_pd(self, pd):
-        logger = logging.getLogger(__name__)
-
         if not self.bulk_ce:
             msg = (
                 "No bulk entry supplied. "
                 "Cannot compute atomic chempots without knowing the bulk entry of interest."
             )
-            logger.warning(msg)
             raise ValueError(msg)
 
         bulk_composition = self.bulk_ce.composition
         redcomp = bulk_composition.reduced_composition
         # append bulk_ce to phase diagram, if not present
         entries = pd.all_entries
         if not any(
@@ -113,15 +110,16 @@
         # which may include a substitutional element...
         # face_list is an array of phases in a facet
         # sub_el is the element to look out for within the face_list array
         blk = []
         sub_spcs = []
         for face in face_list:
             if sub_el:
-                if sub_el in face:
+                face_comp = Composition(face)
+                if Element(sub_el) in face_comp.elements:
                     sub_spcs.append(face)
                 else:
                     blk.append(face)
             else:
                 blk.append(face)
         blk.sort()
         sub_spcs.sort()
@@ -163,23 +161,24 @@
         """
         super(self.__class__, self).__init__(**kwargs)
         self.sub_species = kwargs.get("sub_species", set())
         self.entries = kwargs.get("entries", {})
         self.mpid = kwargs.get("mpid", None)
         self.mapi_key = kwargs.get("mapi_key", None)
 
-    def analyze_GGA_chempots(self, full_sub_approach=False):
+    def analyze_GGA_chempots(self, full_sub_approach=False, verbose=False):
         """
         For calculating GGA-PBE atomic chemical potentials by using
             Materials Project pre-computed data
 
         Args:
             full_sub_approach: generate chemical potentials by looking at
                 full phase diagram (setting to True is NOT recommended
                 if subs_species set has more than one element in it...)
+            verbose: print out debug notes
 
         This code retrieves atomic chempots from Materials
         Project (MP) entries by making use of the pymatgen
         phase diagram (PD) object and computed entries from the MP
         database. There are debug notes that are made based on the stability of
         the structure of interest with respect to the phase diagram generated from MP
 
@@ -192,15 +191,14 @@
             This default approach speeds up analysis when analyzing several substitutional
             species at the same time.
 
             If you prefer to consider the full phase diagram (not recommended
             when you have more than 2 substitutional defects), then set
             full_sub_approach to True.
         """
-        logger = logging.getLogger(__name__)
 
         # gather entries
         self.get_mp_entries(full_sub_approach=full_sub_approach)
 
         # figure out how system should be treated for chemical potentials
         # based on phase diagram
         entry_list = self.entries["bulk_derived"]
@@ -212,51 +210,56 @@
 
         stable_composition_exists = False
         for i in pd.stable_entries:
             if i.composition.reduced_composition == self.redcomp:
                 stable_composition_exists = True
 
         if (decomp_en <= 0) and stable_composition_exists:
-            logger.debug(
-                "Bulk Computed Entry found to be stable with respect "
-                "to MP Phase Diagram (e_above_hull = {} eV/atom).".format(decomp_en)
-            )
+            if verbose:
+                print(
+                    "Bulk Computed Entry found to be stable with respect "
+                    "to MP Phase Diagram (e_above_hull = {} eV/atom).".format(decomp_en)
+                )
         elif (decomp_en <= 0) and not stable_composition_exists:
-            logger.info(
-                "Bulk Computed Entry found to be stable with respect "
-                "to MP Phase Diagram (e_above_hull = {} eV/atom).\n"
-                "However, no stable entry with this composition exists "
-                "in the MP database!\nPlease consider submitting the "
-                "POSCAR to the MP xtaltoolkit, so future users will "
-                "know about this structure:"
-                " https://materialsproject.org/#apps/xtaltoolkit\n"
-                "Manually inserting structure into phase diagram and "
-                "proceeding as normal.".format(decomp_en)
-            )
+            if verbose:
+                print(
+                    "Bulk Computed Entry found to be stable with respect "
+                    "to MP Phase Diagram (e_above_hull = {} eV/atom).\n"
+                    "However, no stable entry with this composition exists "
+                    "in the MP database!\nPlease consider submitting the "
+                    "POSCAR to the MP xtaltoolkit, so future users will "
+                    "know about this structure:"
+                    " https://materialsproject.org/#apps/xtaltoolkit\n"
+                    "Manually inserting structure into phase diagram and "
+                    "proceeding as normal.".format(decomp_en)
+                )
             entry_list.append(self.bulk_ce)
         elif stable_composition_exists:
-            logger.warning(
-                "Bulk Computed Entry not stable with respect to MP "
-                "Phase Diagram (e_above_hull = {} eV/atom), but found "
-                "stable MP composition to exist.\nProducing chemical "
-                "potentials with respect to stable phase.".format(decomp_en)
-            )
+            if verbose:
+                print(
+                    "Bulk Computed Entry not stable with respect to MP "
+                    "Phase Diagram (e_above_hull = {} eV/atom), but found "
+                    "stable MP composition to exist.\nProducing chemical "
+                    "potentials with respect to stable phase.".format(decomp_en)
+                )
         else:
-            logger.warning(
-                "Bulk Computed Entry not stable with respect to MP "
-                "Phase Diagram (e_above_hull = {} eV/atom) and no "
-                "stable structure with this composition exists in the "
-                "MP database.\nProceeding with atomic chemical "
-                "potentials according to composition position within "
-                "phase diagram.".format(decomp_en)
-            )
+            if verbose:
+                print(
+                    "Bulk Computed Entry not stable with respect to MP "
+                    "Phase Diagram (e_above_hull = {} eV/atom) and no "
+                    "stable structure with this composition exists in the "
+                    "MP database.\nProceeding with atomic chemical "
+                    "potentials according to composition position within "
+                    "phase diagram.".format(decomp_en)
+                )
 
         pd = PhaseDiagram(entry_list)
         chem_lims = self.get_chempots_from_pd(pd)
-        logger.debug("Bulk Chemical potential facets: {}".format(chem_lims.keys()))
+        if verbose:
+            print("Bulk Chemical potential facets: {}".format(chem_lims.keys()))
 
         if not full_sub_approach:
             # NOTE if full_sub_approach was True, then all the sub_entries
             # would be ported into the bulk_derived list
             finchem_lims = {}  # this will be final chem_lims dictionary
             for key in chem_lims.keys():
                 face_list = key.split("-")
@@ -308,27 +311,28 @@
                 cp_key_num = (
                     (len(cps.keys()) - 1) if "name-append" in cps else len(cps.keys())
                 )
                 if cp_key_num != (
                     len(self.bulk_species_symbol) + len(self.sub_species)
                 ):
                     facets_to_delete.append(facet_name)
-                    logger.info(
-                        "Not using facet {} because insufficient number of bulk facets for "
-                        "bulk set {} with sub_species set {}. (only dependent on {})."
-                        "".format(
-                            facet_name,
-                            self.bulk_species_symbol,
-                            self.sub_species,
-                            cps.get("name-append"),
+                    if verbose:
+                        print(
+                            "Not using facet {} because insufficient number of bulk facets for "
+                            "bulk set {} with sub_species set {}. (only dependent on {})."
+                            "".format(
+                                facet_name,
+                                self.bulk_species_symbol,
+                                self.sub_species,
+                                cps.get("name-append"),
+                            )
                         )
-                    )
             if len(facets_to_delete) == len(finchem_lims):
                 overdependent_chempot = True
-                logger.warning(
+                warnings.warn(
                     "Determined chemical potentials to be over dependent"
                     " on a substitutional specie. Needing to revert to full_sub_approach. If "
                     "multiple sub species exist this could take a while/break the code..."
                 )
             else:
                 finchem_lims = {
                     k: v for k, v in finchem_lims.items() if k not in facets_to_delete
@@ -368,15 +372,14 @@
             bulk_composition : Composition of bulk as a pymatgen Composition
                 object. This and mapi_key are only actual required input for
                 generating set of chemical potentials from Materials Project
                 database
             full_sub_approach : Include sub_species in query, sub entries can
                 be found in self.entries['subs_set']
         """
-        logger = logging.getLogger(__name__)
 
         redcomp = bulk_composition.reduced_composition
         self.bulk_species_symbol = [s.symbol for s in redcomp.elements]
 
         if not self.entries:
             if (
                 full_sub_approach
@@ -413,15 +416,14 @@
         input bulk and sub elements of interest
 
         Args:
             mpid (str): Structure id of the system in the MP databse.
             mapi_key (str): Materials API key to access database
                 (if not in ~/.pmgrc.yaml already)
         """
-        logger = logging.getLogger(__name__)
 
         if self.bulk_ce:
             self.bulk_species_symbol = [
                 s.symbol for s in self.bulk_ce.composition.elements
             ]
             self.redcomp = self.bulk_ce.composition.reduced_composition
             bce_override = True
@@ -434,15 +436,14 @@
             self.redcomp = self.bulk_ce.composition.reduced_composition
             bce_override = False
         else:
             msg = (
                 "No bulk entry OR mpid supplied. "
                 "Cannot compute atomic chempots without know the bulk entry of interest."
             )
-            logger.warning(msg)
             raise ValueError(msg)
 
         if full_sub_approach:  # this can be time consuming if several sub species exist
             species_symbols = self.bulk_species_symbol[:]
             for sub_el in self.sub_species:
                 species_symbols.append(sub_el)
 
@@ -466,30 +467,28 @@
                 if self.mpid and bce_override:  # overriding bulk_ce if mp-id is given.
                     self.bulk_ce = mp.get_entry_by_material_id(self.mpid)
             if not self.entries:
                 msg = (
                     "Could not fetch bulk entries for atomic chempots!"
                     "MPRester query error."
                 )
-                logger.warning(msg)
                 raise ValueError(msg)
 
             # now compile substitution entries
             self.entries["subs_set"] = dict()
             bulk_entry_set = [entry.entry_id for entry in self.entries["bulk_derived"]]
             for sub_el in self.sub_species:
                 els = self.bulk_species_symbol + [sub_el]
                 with MPRester(api_key=self.mapi_key) as mp:
                     sub_entry_set = mp.get_entries_in_chemsys(els)
                 if not sub_entry_set:
                     msg = (
                         "Could not fetch sub entries for {} atomic chempots! "
                         "Encountered MPRester query error".format(sub_el)
                     )
-                    logger.warning(msg)
                     raise ValueError(msg)
 
                 fin_sub_entry_set = []
                 for entry in sub_entry_set:
                     if entry.entry_id not in bulk_entry_set:
                         fin_sub_entry_set.append(entry)
                 # All entries apart from the bulk entry set
@@ -547,86 +546,94 @@
 
             include_mp_entries: if set to True, extra entries from
                 Materials Project will be added to phase diagram
                 according to phases that are stable in the Materials
                 Project database
 
         """
-        pdfile = os.path.join(self.path_base, "PhaseDiagram")
-        if not os.path.exists(pdfile):
-            print("Phase diagram file does not exist at ", pdfile)
-            return
+        from doped.pycdt.utils.parse_calculations import (
+            get_vasprun,
+            _get_output_files_and_check_if_multiple,
+        )
+
+        pd_folder = os.path.join(self.path_base, "PhaseDiagram")
+        if not os.path.exists(pd_folder):
+            raise FileNotFoundError(f"Phase diagram folder does not exist at {pd_folder}!")
 
         # this is where we read computed entries into a list for parsing...
         # NOTE TO USER: If not running with VASP need to use another
         # pymatgen functionality for importing computed entries below...
         personal_entry_list = []
-        for structfile in os.listdir(pdfile):
-            if os.path.exists(
-                os.path.join(pdfile, structfile, "vasprun.xml")
-            ) or os.path.exists(os.path.join(pdfile, structfile, "vasprun.xml.gz")):
-                try:
-                    print("loading ", structfile)
-                    from doped.pycdt.utils.parse_calculations import get_vasprun
-
-                    vr, vr_path = get_vasprun(
-                        os.path.join(pdfile, structfile, "vasprun.xml")
-                    )
-                    vr_entry = vr.get_computed_entry()
-                    pdentry = PDEntry(
-                        vr_entry.composition, vr_entry.energy, attribute=structfile
-                    )
-                    personal_entry_list.append(pdentry)
-                except:
-                    print("Could not load ", structfile)
-
-            else:
-                print("No vasprun.xml(.gz) found in ", structfile)
+        for structfile in os.listdir(pd_folder):
+            try:
+                print("loading ", structfile)
+                vr_path, multiple = _get_output_files_and_check_if_multiple(
+                    "vasprun.xml", os.path.join(pd_folder, structfile),
+                )
+                if multiple:
+                    warnings.warn(
+                        f"Multiple `vasprun.xml` files found in directory: "
+                        f"{os.path.join(pd_folder, structfile)}. Using {vr_path} to parse the "
+                        f"calculation energy and metadata."
+                    )
+                vr = get_vasprun(vr_path)
+                vr_entry = vr.get_computed_entry()
+                pdentry = PDEntry(
+                    vr_entry.composition, vr_entry.energy, attribute=structfile
+                )
+                personal_entry_list.append(pdentry)
+            except:
+                print("Could not load a vasprun.xml file for", structfile)
 
         # add bulk computed entry to phase diagram, and see if it is stable
         if not self.bulk_ce:
-            vr_path = os.path.join(self.path_base, "bulk", "vasprun.xml")
-            if os.path.exists(vr_path):
+            try:
+                bulk_vr_path, multiple = _get_output_files_and_check_if_multiple(
+                    "vasprun.xml", os.path.join(self.path_base, "bulk")
+                )
+                if multiple:
+                    warnings.warn(
+                        f"Multiple `vasprun.xml` files found in directory: "
+                        f"{os.path.join(self.path_base, 'bulk')}. Using {bulk_vr_path} to parse "
+                        f"the "
+                        f"calculation energy and metadata."
+                    )
+                bulk_vr = get_vasprun(bulk_vr_path)
                 print("loading bulk computed entry")
-                from doped.pycdt.utils.parse_calculations import get_vasprun
-
-                bulkvr, bulkvr_path = get_vasprun(vr_path)
-                bulkvr_entry = bulkvr.get_computed_entry()
+                bulk_vr_entry = bulk_vr.get_computed_entry()
                 self.bulk_ce = PDEntry(
-                    bulkvr_entry.composition, bulkvr_entry.energy, attribute=bulkvr_path
-                )
-            else:
-                print(
-                    "No bulk entry given locally. Phase diagram "
-                    + "calculations cannot be set up without this"
-                )
-                return
+                    bulk_vr_entry.composition,
+                    bulk_vr_entry.energy,
+                    attribute=bulk_vr_path,
+                )
+            except Exception as e:
+                raise FileNotFoundError(
+                    "No bulk entry (`bulk_ce`) provided, and no vasprun.xml file found in {"
+                    "os.path.join(self.path_base, 'bulk')}. Required for parsing competing phase "
+                    "calculations!"
+                ) from e
 
         self.bulk_composition = self.bulk_ce.composition
         self.redcomp = self.bulk_composition.reduced_composition
         self.bulk_species_symbol = [s.symbol for s in self.bulk_ce.composition.elements]
 
         # Supplement entries to phase diagram with those from MP database
         if include_mp_entries:
             mpcpa = MPChemPotAnalyzer(
                 bulk_ce=self.bulk_ce,
                 sub_species=self.sub_species,
                 mapi_key=self.mapi_key,
             )
-            tempcl = mpcpa.analyze_GGA_chempots(
-                full_sub_approach=full_sub_approach
-            )  # Use MPentries
-
-            curr_pd = PhaseDiagram(
-                list(
-                    set().union(
-                        mpcpa.entries["bulk_derived"], mpcpa.entries["subs_set"]
-                    )
-                )
-            )
+            mpcpa.get_mp_entries(full_sub_approach=full_sub_approach)  # Use MP entries
+
+            full_entries = mpcpa.entries["bulk_derived"]
+            for entry_set in mpcpa.entries["subs_set"].values():
+                full_entries.extend(entry_set)
+            curr_pd = PhaseDiagram(full_entries)
+
             stable_idlist = {
                 i.composition.reduced_composition: [i.energy_per_atom, i.entry_id, i]
                 for i in curr_pd.stable_entries
             }
             for mpcomp, mplist in stable_idlist.items():
                 matched = False
                 for pe in personal_entry_list:
@@ -642,19 +649,21 @@
                         "Adding entry from MP-database:",
                         mpcomp,
                         "(entry-id:",
                         mplist[1],
                     )
                     personal_entry_list.append(mplist[2])
         else:
-            # personal_entry_list.append(self.bulk_ce)
-            # if you dont have entries for elemental corners of phase diagram then code breaks
-            # manually inserting entries with energies of zero for competeness...USER DO NOT USE
+            # if you don't have entries for elemental corners of phase diagram then code breaks
+            # manually inserting entries with energies of zero for completeness... USER DO NOT USE
             # THIS
-            eltcount = {elt: 0 for elt in set(self.bulk_ce.composition.elements)}
+            eltcount = {elt: 0 for elt in self.bulk_ce.composition.elements}
+            for elt_sym in self.sub_species:
+                eltcount[Element(elt_sym)] = 0
+
             for pentry in personal_entry_list:
                 if (
                     pentry.is_element
                     and pentry.composition.elements[0] in eltcount.keys()
                 ):
                     eltcount[pentry.composition.elements[0]] += 1
             for elt, eltnum in eltcount.items():
@@ -719,34 +728,40 @@
             # Now consider adding single elements to extend the phase diagram,
             # adding new additions to chemical potentials ONLY for the cases
             # where the phases in equilibria are those from the bulk phase
             # diagram. This is essentially the assumption that the majority of
             # the elements in the total composition will be from the native
             # species present rather than the sub species (a good approximation)
             for sub_el in self.sub_species:
+                sub_el = Element(sub_el)
                 sub_specie_entries = entry_list[:]
                 for entry in sub_associated_entry_list:
-                    if sub_el in entry.composition.elements:
+                    if Element(sub_el) in entry.composition.elements:
                         sub_specie_entries.append(entry)
 
                 pd = PhaseDiagram(sub_specie_entries)
                 chem_lims = self.get_chempots_from_pd(pd)
 
                 for key in chem_lims.keys():
                     face_list = key.split("-")
                     blk, blknom, subnom = self.diff_bulk_sub_phases(
-                        face_list, sub_el=sub_el
+                        face_list, sub_el=sub_el.symbol
                     )
                     # if one less than number of bulk species then can be
                     # grouped with rest of structures
-                    if len(blk) == len(self.bulk_species_symbol):
+                    bulk_species_symbol = [
+                        s.symbol for s in self.bulk_composition.elements
+                    ]
+                    if len(blk) == len(bulk_species_symbol):
                         if blknom not in finchem_lims.keys():
                             finchem_lims[blknom] = chem_lims[key]
                         else:
-                            finchem_lims[blknom][sub_el] = chem_lims[key][sub_el]
+                            finchem_lims[blknom][sub_el] = chem_lims[key][
+                                Element(sub_el)
+                            ]
                         if "name-append" not in finchem_lims[blknom].keys():
                             finchem_lims[blknom]["name-append"] = subnom
                         else:
                             finchem_lims[blknom]["name-append"] += "-" + subnom
                     else:
                         # if chem pots determined by two (or more) sub-specie
                         # containing phases, skip this facet!
@@ -755,14 +770,15 @@
             # run a check to make sure all facets dominantly defined by bulk species
             overdependent_chempot = False
             facets_to_delete = []
             for facet_name, cps in finchem_lims.items():
                 cp_key_num = (
                     (len(cps.keys()) - 1) if "name-append" in cps else len(cps.keys())
                 )
+                bulk_species_symbol = [s.symbol for s in self.bulk_composition.elements]
                 if cp_key_num != (
                     len(self.bulk_species_symbol) + len(self.sub_species)
                 ):
                     facets_to_delete.append(facet_name)
                     print(
                         "Not using facet {} because insufficient number of bulk facets for "
                         "bulk set {} with sub_species set {}. (only dependent on {})."
@@ -815,15 +831,15 @@
                 for elt, ent in self.phase_diagram.el_refs.items()
             },
             "facets_wrt_elt_refs": {},
         }
         for facet, chempot_dict in chem_lims["facets"].items():
             rel_chempot_dict = copy.deepcopy(chempot_dict)
             for elt, chempot_energy in rel_chempot_dict.items():
-                rel_chempot_dict[elt] -= chem_lims["elemental_refs"][elt]
+                rel_chempot_dict[elt] -= chem_lims["elemental_refs"][Element(elt)]
             chem_lims["facets_wrt_elt_refs"].update({facet: rel_chempot_dict})
         return chem_lims
 
 
 class UserChemPotInputGenerator(object):
     """
     For setting up phase diagram for user, based on structures that exist in the MP database
```

### Comparing `doped-1.0.9/doped/pycdt/core/defects_analyzer.py` & `doped-1.1.0/doped/corrections.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,672 +1,547 @@
-#!/usr/bin/env python
+"""
+Code to compute finite-size charge corrections for charged defects in periodic systems.
+These functions are built from a combination of useful modules from pymatgen, pycdt and AIDE (by
+Adam Jackson and Alex Ganose), alongside substantial modification, in the efforts of making an
+efficient, user-friendly package for managing and analysing defect calculations,
+with publication-quality outputs.
+
+The charge-correction methods implemented are:
+1) Freysoldt correction for isotropic systems. Includes:
+       a) PC energy
+       b) potential alignment by planar averaging.
+2) Extended Freysoldt or Kumagai correction for anistropic systems. Includes:
+       a) anisotropic PC energy
+       b) potential alignment by atomic site averaging outside Wigner Seitz radius
+
+If you use the corrections implemented in this module, cite
+   Freysoldt, Neugebauer, and Van de Walle,
+    Phys. Status Solidi B. 248, 1067-1076 (2011) for isotropic correction
+   Kumagai and Oba, Phys. Rev. B. 89, 195205 (2014) for anisotropic correction
+"""
 
-
-import os
 import warnings
-from collections import defaultdict
-from itertools import combinations
-from math import exp, pi, sqrt
+import itertools
+import copy
+from math import erfc, exp
 
 import numpy as np
-from pymatgen.core import Element
-from pymatgen.core.structure import PeriodicSite, Structure
-from pymatgen.entries.computed_entries import ComputedStructureEntry
-from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
-
-from doped.pycdt.corrections.finite_size_charge_correction import (
-    get_correction_freysoldt,
-    get_correction_kumagai,
-)
+from monty.json import MontyDecoder
+from pymatgen.analysis.defects.corrections import FreysoldtCorrection, KumagaiCorrection
+
 from doped.pycdt.utils.parse_calculations import SingleDefectParser
-from doped.pycdt.utils.units import conv, hbar, kb
+from doped.analysis import _convert_dielectric_to_tensor
 
 warnings.simplefilter("default")
-warnings.filterwarnings("ignore", message="`np.int` is a deprecated alias for the builtin `int`")
+warnings.filterwarnings(
+    "ignore", message="`np.int` is a deprecated alias for the builtin `int`"
+)
 warnings.filterwarnings("ignore", message="Use get_magnetic_symmetry()")
 
 
+def _monty_decode_nested_dicts(d):
+    """
+    Recursively find any dictionaries in defect_entry.parameters, which may be nested in dicts or in
+    lists of dicts and decode them:
+    """
+    for key, value in d.items():
+        if isinstance(value, dict) and not any(
+            k in value for k in ["@module", "@class"]
+        ):
+            _monty_decode_nested_dicts(value)
+        elif isinstance(value, list):
+            if all(isinstance(i, dict) for i in value) and all(
+                k in i for k in ["@module", "@class"] for i in value
+            ):
+                try:
+                    d[key] = [MontyDecoder().process_decoded(i) for i in value]
+                except Exception as exc:
+                    print(f"Failed to decode {key} with error {exc}")
+                    pass
+
+        if isinstance(value, dict) and all(k in value for k in ["@module", "@class"]):
+            try:
+                d[key] = MontyDecoder().process_decoded(value)
+            except Exception as exc:
+                print(f"Failed to decode {key} with error {exc}")
+                pass
+
+
+def get_correction_freysoldt(
+    defect_entry,
+    dielectric,
+    plot: bool = False,
+    filename: str = None,
+    partflag="All",
+    axis=None,
+):
+    """
+    Function to compute the isotropic Freysoldt correction for each defect.
+    If this correction is used, please reference Freysoldt's original paper.
+    doi: 10.1103/PhysRevLett.102.016402
+    Args:
+        defect_entry: DefectEntry object with the following
+            keys stored in defect.parameters:
+                required:
+                    axis_grid (3 x NGX where NGX is the length of the NGX grid
+                    in the x,y and z axis directions. Same length as planar
+                    average lists):
+                        A list of 3 numpy arrays which contain the cartesian axis
+                        values (in angstroms) that correspond to each planar avg
+                        potential supplied.
+
+                    bulk_planar_averages (3 x NGX where NGX is the length of
+                    the NGX grid in the x,y and z axis directions.):
+                        A list of 3 numpy arrays which contain the planar averaged
+                        electrostatic potential for the bulk supercell.
+
+                    defect_planar_averages (3 x NGX where NGX is the length of
+                    the NGX grid in the x,y and z axis directions.):
+                        A list of 3 numpy arrays which contain the planar averaged
+                        electrostatic potential for the defective supercell.
+
+                    bulk_sc_structure (Structure) bulk structure corresponding to
+                        defect supercell structure (uses Lattice for charge correction)
+
+                    defect_frac_sc_coords (3 x 1 array) Fracitional co-ordinates of
+                        defect location in supercell structure
+                optional:
+                    'encut' : energy cutoff desired for Freysoldt correction
+                    'madetol' : madelung tolerance for Freysoldt correction
+                    'q_model' : Charge Model for Freysoldt correction
+                    'q_model' : Charge Model for Freysoldt correction
+        dielectric (float or int or 3x1 matrix or 3x3 matrix):
+            ionic + static contributions to dielectric constant
+        plot (bool): decides whether to plot electrostatic potential plots or not.
+        filename (str): if None, plots are not saved, if a string,
+            then the plot will be saved as '{filename}_{axis}.pdf'
+        partflag: four options for correction output:
+               'pc' for just point charge correction, or
+               'potalign' for just potalign correction, or
+               'All' for both (added together), or
+               'AllSplit' for individual parts split up (form is [PC, potterm, full])
+        axis (int or None): if integer, then freysoldt correction is performed on the single axis.
+            If it is None, then averaging of the corrections for the three axes is used for the
+            correction.
+
+    Returns Correction
+    """
+    # ensure parameters are decoded in case defect_dict was reloaded from json
+    _monty_decode_nested_dicts(defect_entry.parameters)
+
+    dielectric = _convert_dielectric_to_tensor(dielectric)
+
+    if partflag not in ["All", "AllSplit", "pc", "potalign"]:
+        print(
+            '{} is incorrect potalign type. Must be "All", "AllSplit", "pc", or '
+            '"potalign".'.format(partflag)
+        )
+        return
+
+    q_model = defect_entry.parameters.get("q_model", None)
+    encut = defect_entry.parameters.get("encut", 520)
+    madetol = defect_entry.parameters.get("madetol", 0.0001)
+
+    if not defect_entry.charge:
+        print("Charge is zero so charge correction is zero.")
+        return 0.0
+
+    template_defect = copy.deepcopy(defect_entry)
+    corr_class = FreysoldtCorrection(
+        dielectric, q_model=q_model, energy_cutoff=encut, madetol=madetol, axis=axis
+    )
+    f_corr_summ = corr_class.get_correction(template_defect)
+
+    if plot:
+        if axis is None:
+            ax_list = [
+                [k, "axis" + str(k)]
+                for k in corr_class.metadata["pot_plot_data"].keys()
+            ]
+        else:
+            ax_list = [[axis, "axis" + str(axis + 1)]]
+
+        for ax_key, ax_title in ax_list:
+            p = corr_class.plot(ax_key, title=ax_title, saved=False)
+            if filename:
+                p.savefig(filename + "_" + ax_title + ".pdf", bbox_inches="tight")
+
+    if partflag in ["AllSplit", "All"]:
+        freyval = np.sum(list(f_corr_summ.values()))
+    elif partflag == "pc":
+        freyval = f_corr_summ["freysoldt_electrostatic"]
+    elif partflag == "potalign":
+        freyval = f_corr_summ["freysoldt_potential_alignment"]
+
+    print(f"Final Freysoldt correction is {freyval:.3f} eV")
+
+    if partflag == "AllSplit":
+        freyval = [
+            f_corr_summ["freysoldt_electrostatic"],
+            f_corr_summ["freysoldt_potential_alignment"],
+            freyval,
+        ]
+
+    return freyval
+
+
+def get_correction_kumagai(
+    defect_entry, dielectric, plot: bool = False, filename: str = None, partflag="All"
+):
+    """
+    Function to compute the Kumagai correction for each defect (modified freysoldt for
+    anisotropic dielectric).
+    NOTE that bulk_init class must be pre-instantiated to use this function
+    Args:
+        defect_entry: DefectEntry object with the following
+            keys stored in defect.parameters:
+                required:
+                    bulk_atomic_site_averages (list):  list of bulk structure"s atomic site
+                    averaged ESPs * charge, in same order as indices of bulk structure note this
+                    is list given by VASP's OUTCAR (so it is multiplied by a test charge of -1)
+
+                    defect_atomic_site_averages (list):  list of defect structure"s atomic site
+                    averaged ESPs * charge, in same order as indices of defect structure note
+                    this is list given by VASP's OUTCAR (so it is multiplied by a test charge of -1)
+
+                    site_matching_indices (list):  list of corresponding site index values for
+                    bulk and defect site structures EXCLUDING the defect site itself (ex. [[bulk
+                    structure site index, defect structure"s corresponding site index], ... ]
+
+                    initial_defect_structure (Structure): Pymatgen Structure object representing
+                    un-relaxed defect structure
+
+                    defect_frac_sc_coords (array): Defect Position in fractional coordinates of
+                    the supercell given in bulk_structure
+                optional:
+                    gamma (float): Ewald parameter, Default is to determine it based on
+                        convergence of brute summation tolerance
+                    sampling_radius (float): radius (in Angstrom) which sites must be outside of
+                        to be included in the correction. Publication by Kumagai advises to use
+                        Wigner-Seitz radius of defect supercell, so this is default value.
+        dielectric (float or int or 3x1 matrix or 3x3 matrix):
+            ionic + static contributions to dielectric constant
+        plot (bool): decides whether to plot electrostatic potential plots or not.
+        filename (str): if None, plots are not saved, if a string, then the plot will be saved as
+            '{filename}.pdf'
+        partflag: four options for correction output:
+               'pc' for just point charge correction, or
+               'potalign' for just potalign correction, or
+               'All' for both (added together), or
+               'AllSplit' for individual parts split up (form is [PC, potterm, full])
+    """
+    # ensure parameters are decoded in case defect_dict was reloaded from json
+    _monty_decode_nested_dicts(defect_entry.parameters)
+
+    dielectric = _convert_dielectric_to_tensor(dielectric)
+
+    if partflag not in ["All", "AllSplit", "pc", "potalign"]:
+        print(
+            '{} is incorrect potalign type. Must be "All", "AllSplit", "pc", or '
+            '"potalign".'.format(partflag)
+        )
+        return
+
+    sampling_radius = defect_entry.parameters.get("sampling_radius", None)
+    gamma = defect_entry.parameters.get("gamma", None)
+
+    if not defect_entry.charge:
+        print("Charge is zero so charge correction is zero.")
+        return 0.0
+
+    template_defect = copy.deepcopy(defect_entry)
+    corr_class = KumagaiCorrection(
+        dielectric, sampling_radius=sampling_radius, gamma=gamma
+    )
+    k_corr_summ = corr_class.get_correction(template_defect)
+
+    if plot:
+        p = corr_class.plot(title="Kumagai", saved=False)
+        if filename:
+            p.savefig(f"{filename}.pdf", bbox_inches="tight")
+
+    if partflag in ["AllSplit", "All"]:
+        kumagai_val = np.sum(list(k_corr_summ.values()))
+    elif partflag == "pc":
+        kumagai_val = k_corr_summ["kumagai_electrostatic"]
+    elif partflag == "potalign":
+        kumagai_val = k_corr_summ["kumagai_potential_alignment"]
+
+    print(f"\nFinal Kumagai correction is {kumagai_val:.3f} eV")
+
+    if partflag == "AllSplit":
+        kumagai_val = [
+            k_corr_summ["kumagai_electrostatic"],
+            k_corr_summ["kumagai_potential_alignment"],
+            kumagai_val,
+        ]
+    return kumagai_val
+
+
 def freysoldt_correction_from_paths(
-    defect_file_path, bulk_file_path, dielectric, defect_charge, plot=False
+    defect_file_path,
+    bulk_file_path,
+    dielectric,
+    defect_charge,
+    plot=False,
+    filename=None,
 ):
     """
     A function for performing the Freysoldt correction with a set of file paths.
     If this correction is used, please reference Freysoldt's original paper.
     doi: 10.1103/PhysRevLett.102.016402
 
-    Does not require transformation.json file to exist in file path.
-
     :param defect_file_path (str): file path to defect folder of interest
     :param bulk_file_path (str): file path to bulk folder of interest
-    :param dielectric (float or 3x3 matrix): Dielectric constant (or tensor) for the structure
-    :param defect_charge (int): charge of defect structure of interest
-    :param plot (bool): allow for plotting electrostatic potential
+    :param dielectric (float or int or 3x1 matrix or 3x3 matrix):
+            ionic + static contributions to dielectric constant
+    :param charge (int): charge of defect structure of interest
+    :param plot (bool): decides whether to plot electrostatic potential plots or not.
+    :param filename (str): if None, plots are not saved, if a string,
+            then the plot will be saved as '{filename}_{axis}.pdf'
     :return:
         Dictionary of Freysoldt Correction for defect
     """
     sdp = SingleDefectParser.from_paths(
         defect_file_path, bulk_file_path, dielectric, defect_charge
     )
     _ = sdp.freysoldt_loader()
     if plot:
         print(f"{sdp.defect_entry.name}, charge = {defect_charge}")
-    correction = get_correction_freysoldt(sdp.defect_entry, dielectric, plot=plot)
+    correction = get_correction_freysoldt(
+        sdp.defect_entry, dielectric, plot=plot, filename=filename
+    )
 
     return correction
 
 
 def kumagai_correction_from_paths(
-    defect_file_path, bulk_file_path, dielectric, defect_charge, plot=False
+    defect_file_path,
+    bulk_file_path,
+    dielectric,
+    defect_charge,
+    plot=False,
+    filename=None,
 ):
     """
     A function for performing the Kumagai correction with a set of file paths.
     If this correction is used, please reference Kumagai and Oba's original paper
     (doi: 10.1103/PhysRevB.89.195205) as well as Freysoldt's original
     paper (doi: 10.1103/PhysRevLett.102.016402
 
-    Does not require transformation.json file to exist in file path.
-
     :param defect_file_path (str): file path to defect folder of interest
     :param bulk_file_path (str): file path to bulk folder of interest
-    :param dielectric (float or 3x3 matrix): Dielectric constant (or tensor) for the structure
-    :param defect_charge (int): charge of defect structure of interest
-    :param plot (bool): allow for plotting electrostatic potential
+    :param dielectric (float or int or 3x1 matrix or 3x3 matrix):
+            ionic + static contributions to dielectric constant
+    :param charge (int): charge of defect structure of interest
+    :param plot (bool): decides whether to plot electrostatic potential plots or not.
+    :param filename (str): if None, plots are not saved, if a string, then the plot will be saved as
+        '{filename}.pdf'
     :return:
         Dictionary of Kumagai Correction for defect
     """
     sdp = SingleDefectParser.from_paths(
         defect_file_path, bulk_file_path, dielectric, defect_charge
     )
     _ = sdp.kumagai_loader()
-    plt_title = (
-        os.path.join(
-            defect_file_path, "{}_chg_{}".format(sdp.defect_entry.name, defect_charge)
-        )
-        if plot
-        else None
+    if plot:
+        print(f"{sdp.defect_entry.name}, charge = {defect_charge}")
+    correction = get_correction_kumagai(
+        sdp.defect_entry, dielectric, plot=plot, filename=filename
     )
-    correction = get_correction_kumagai(sdp.defect_entry, dielectric, title=plt_title)
 
     return correction
 
 
-class ComputedDefect(object):
-    """
-    Holds all the info concerning a defect computation:
-    composition+structure, energy, correction on energy and name
-    """
-
-    def __init__(
-        self,
-        entry_defect,
-        site_in_bulk,
-        multiplicity=None,
-        supercell_size=(1, 1, 1),
-        charge=0.0,
-        charge_correction=0.0,
-        other_correction=0.0,
-        name=None,
-    ):
-        """
-        Args:
-            entry_defect:
-                An ComputedStructureEntry object corresponding to the
-                defect supercell
-            site_in_bulk:
-                Site of the defect in bulk supercell. Defect positions
-                are often required to perform posteriori corrections
-            multiplicity:
-                Multiplicity of defect site in a cell. Useful to
-                evaluate defect concentrations
-            supercell_size:
-                Size of the defect supercell in terms of unit cell
-            charge:
-                The charge of the defect
-            charge_correction:
-                Correction to the energy due to charge
-            other_correction:
-                Correction to the energy due to other factors
-            name:
-                The name of the defect
-        """
-
-        self.entry = entry_defect
-        self.site = site_in_bulk
-        self.multiplicity = multiplicity
-        self.supercell_size = supercell_size
-        self.charge = charge
-        self.charge_correction = charge_correction  # Can be added after initialization
-        self.other_correction = other_correction
-        self.name = name
-        if self.name:
-            self.full_name = self.name + "_" + str(charge)
-        else:
-            self.full_name = "defect_" + str(charge)
-        warnings.warn(
-            "Replaced PyCDT usage of ComputedDefect objects with "
-            "DefectEntry objects from pymatgen.analysis.defects.core\n"
-            "Will remove ComputedDefect with Version 2.5 of PyCDT.",
-            DeprecationWarning,
-        )
-
-    def as_dict(self):
-        return {
-            "entry": self.entry.as_dict(),
-            "site": self.site.as_dict(),
-            "multiplicity": self.multiplicity,
-            "supercell_size": self.supercell_size,
-            "charge": self.charge,
-            "charge_correction": self.charge_correction,
-            "other_correction": self.other_correction,
-            "name": self.name,
-            "full_name": self.full_name,
-            "@module": self.__class__.__module__,
-            "@class": self.__class__.__name__,
-        }
-
-    @classmethod
-    def from_dict(cls, d):
-        return cls(
-            ComputedStructureEntry.from_dict(d["entry"]),
-            PeriodicSite.from_dict(d["site"]),
-            multiplicity=d.get("multiplicity", None),
-            supercell_size=d.get("supercell_size", [1, 1, 1]),
-            charge=d.get("charge", 0.0),
-            charge_correction=d.get("charge_correction", 0.0),
-            other_correction=d.get("other_correction", 0.0),
-            name=d.get("name", None),
-        )
-
-
-class DefectsAnalyzer(object):
-    """
-    a class aimed at performing standard analysis of defects
-    """
+# The following functions are taken from the deprecated AIDE package developed by the dynamic duo
+# Adam Jackson and Alex Ganose (https://github.com/SMTG-UCL/aide)
 
-    def __init__(self, entry_bulk, e_vbm, mu_elts, band_gap):
-        """
-        Args:
-            entry_bulk:
-                the bulk data as an Entry
-            e_vbm:
-                the energy of the vbm (in eV)
-            mu_elts:
-                a dictionnary of {Element:value} giving the chemical
-                potential of each element
-            band_gap:
-                the band gap (in eV)
-        """
-        self._entry_bulk = entry_bulk
-        self._e_vbm = e_vbm
-        self._mu_elts = mu_elts
-        self._band_gap = band_gap
-        self._defects = []
-        self._formation_energies = []
-        warnings.warn(
-            "Replaced PyCDT usage of DefectsAnalyzer objects with "
-            "DefectPhaseDiagram objects from pymatgen.analysis.defects.thermodynamics\n"
-            "Will remove DefectsAnalyzer with Version 2.5 of PyCDT.",
-            DeprecationWarning,
-        )
 
-    def as_dict(self):
-        d = {
-            "entry_bulk": self._entry_bulk.as_dict(),
-            "e_vbm": self._e_vbm,
-            "mu_elts": {k.symbol: v for k, v in self._mu_elts.items()},
-            "band_gap": self._band_gap,
-            "defects": [d.as_dict() for d in self._defects],
-            "formation_energies": self._formation_energies,
-            "@module": self.__class__.__module__,
-            "@class": self.__class__.__name__,
-        }
-        return d
-
-    @classmethod
-    def from_dict(cls, d):
-        struct = d["entry_bulk"]["structure"]
-        struct = (
-            struct if isinstance(struct, Structure) else Structure.from_dict(struct)
-        )
-        entry_bulk = ComputedStructureEntry(struct, d["entry_bulk"]["energy"])
-        analyzer = DefectsAnalyzer(
-            entry_bulk,
-            d["e_vbm"],
-            {Element(el): d["mu_elts"][el] for el in d["mu_elts"]},
-            d["band_gap"],
-        )
-        for ddict in d["defects"]:
-            analyzer.add_computed_defect(ComputedDefect.from_dict(ddict))
-        return analyzer
-
-    def add_computed_defect(self, defect):
-        """
-        add a parsed defect to the analyzer
-        Args:
-            defect:
-                a ComputedDefect object
-        """
-        self._defects.append(defect)
-        self._compute_form_en()
-
-    def change_charge_correction(self, i, correction):
-        """
-        Change the charge correction for defect at index i
-        Args:
-            i:
-                Index of defects
-            correction:
-                New correction to be applied for defect
-        """
-        self._defects[i].charge_correction = correction
-        self._compute_form_en()
-
-    def change_other_correction(self, i, correction):
-        """
-        Change the charge correction for defect at index i
-        Args:
-            i:
-                Index of defects
-            correction:
-                New correction to be applied for defect
-        """
-        self._defects[i].other_correction = correction
-        self._compute_form_en()
-
-    def _get_all_defect_types(self):
-        to_return = []
-        for d in self._defects:
-            if d.name not in to_return:
-                to_return.append(d.name)
-        return to_return
-
-    def _compute_form_en(self):
-        """
-        compute the formation energies for all defects in the analyzer
-        """
-        self._formation_energies = []
-        for d in self._defects:
-            # compensate each element in defect with the chemical potential
-            mu_needed_coeffs = {}
-            for elt in d.entry.composition.elements:
-                el_def_comp = d.entry.composition[elt]
-                el_blk_comp = self._entry_bulk.composition[elt]
-                mu_needed_coeffs[Element(elt)] = el_blk_comp - el_def_comp
-
-            sum_mus = 0.0
-            for elt in mu_needed_coeffs:
-                sum_mus += mu_needed_coeffs[elt] * self._mu_elts[elt]
-
-            self._formation_energies.append(
-                d.entry.energy
-                - self._entry_bulk.energy
-                + sum_mus
-                + d.charge * self._e_vbm
-                + d.charge_correction
-                + d.other_correction
-            )
+def get_murphy_image_charge_correction(
+    lattice,
+    dielectric_matrix,
+    conv=0.3,
+    factor=30,
+    verbose=False,
+):
+    """Calculates the anisotropic image charge correction by Sam Murphy in eV.
 
-    def correct_bg_simple(self, vbm_correct, cbm_correct):
-        """
-        correct the band gap in the analyzer.
-        We assume the defects level remain the same when moving the
-        band edges
-        Args:
-            vbm_correct:
-                The correction on the vbm as a positive number. e.g.,
-                if the VBM goes 0.1 eV down vbm_correct=0.1
-            cbm_correct:
-                The correction on the cbm as a positive number. e.g.,
-                if the CBM goes 0.1 eV up cbm_correct=0.1
-
-        """
-        self._band_gap = self._band_gap + cbm_correct + vbm_correct
-        self._e_vbm = self._e_vbm - vbm_correct
-        self._compute_form_en()
-
-    def get_transition_levels(self):
-        """
-        Charge transition levels are computed
-        :return: Transition levels for each pair of the defects.
-        If any pair is missing, the transition level for that pair is
-        not within the band gap.
-        """
-        xlim = (-0.5, self._band_gap + 1.5)
-        nb_steps = 1000
-        x = np.arange(xlim[0], xlim[1], (xlim[1] - xlim[0]) / nb_steps)
-
-        y = defaultdict(defaultdict)
-        for i, dfct in enumerate(self._defects):
-            yval = self._formation_energies[i] + dfct.charge * x
-            y[dfct.name][dfct.charge] = yval
-
-        transit_levels = defaultdict(defaultdict)
-        for dfct_name in y:
-            q_ys = y[dfct_name]
-            for qpair in combinations(q_ys.keys(), 2):
-                qpair_s = tuple(sorted(list(qpair)))
-                y_absdiff = abs(q_ys[qpair_s[1]] - q_ys[qpair_s[0]])
-                if y_absdiff.min() < 0.4:
-                    transit_levels[dfct_name][qpair_s] = x[np.argmin(y_absdiff)]
-        return transit_levels
-
-    def _get_form_energy(self, ef, i):
-        return self._formation_energies[i] + self._defects[i].charge * ef
-
-    def get_formation_energies(self, ef=0.0):
-        """
-        Get the defect formation energies for a given Fermi level
-        Args:
-            ef:
-                the fermi level in eV (with respect to the VBM)
-        Returns:
-            a list of dict of {'name': defect name, 'charge': defect charge
-                               'energy': defect formation energy in eV}
-        """
-        energies = []
-        i = 0
-        for i, d in enumerate(self._defects):
-            energies.append(
-                {
-                    "name": d.name,
-                    "charge": d.charge,
-                    "energy": self._get_form_energy(ef, i),
-                }
-            )
-        return energies
+    This a rewrite of the code 'madelung.pl' written by Sam Murphy (see [1]).
+    The default convergence parameter of conv = 0.3 seems to work perfectly
+    well. However, it may be worth testing convergence of defect energies with
+    respect to the factor (i.e. cut-off radius).
+
+    References:
+        [1] S. T. Murphy and N. D. H. Hine, Phys. Rev. B 87, 094111 (2013).
+
+    Args:
+        lattice (list): The defect cell lattice as a 3x3 matrix.
+        dielectric_matrix (list): The dielectric tensor as 3x3 matrix.
+        conv (float): A value between 0.1 and 0.9 which adjusts how much real
+                      space vs reciprocal space contribution there is.
+        factor: The cut-off radius, defined as a multiple of the longest cell
+            parameter.
+        verbose (bool): If True details of the correction will be printed.
 
-    def get_defects_concentration(self, temp=300, ef=0.0):
-        """
-        Get the defect concentration for a temperature and Fermi level.
-        Note: This method has an approximation and can fail
-        [Ref: PRB 86, 144109 (2012)]
-        Args:
-            temp:
-                the temperature in K
-            Ef:
-                the fermi level in eV (with respect to the VBM)
-        Returns:
-            A list of dict of {'name': defect name, 'charge': defect charge
-                               'conc': defects concentration in m-3}
-        """
-        conc = []
-        struct = self._entry_bulk.structure
-        for i, d in enumerate(self._defects):
-            cell_multiplier = np.prod(d.supercell_size)
-            n = d.multiplicity * cell_multiplier * 1e30 / struct.volume
-            conc.append(
-                {
-                    "name": d.name,
-                    "charge": d.charge,
-                    "conc": n * exp(-self._get_form_energy(ef, i) / (kb * temp)),
-                }
-            )
+    Returns:
 
-        return conc
+        The image charge correction as {charge: correction}
+    """
+    inv_diel = np.linalg.inv(dielectric_matrix)
+    det_diel = np.linalg.det(dielectric_matrix)
+    latt = np.sqrt(np.sum(lattice**2, axis=1))
+
+    # calc real space cutoff
+    longest = max(latt)
+    r_c = factor * longest
+
+    # Estimate the number of boxes required in each direction to ensure
+    # r_c is contained (the tens are added to ensure the number of cells
+    # contains r_c). This defines the size of the supercell in which
+    # the real space section is performed, however only atoms within rc
+    # will be conunted.
+    axis = np.array([int(r_c / a + 10) for a in latt])
+
+    # Calculate supercell parallelpiped and dimensions
+    sup_latt = np.dot(np.diag(axis), lattice)
+
+    # Determine which of the lattice parameters is the largest and determine
+    # reciprocal space supercell
+    recip_axis = np.array([int(x) for x in factor * max(latt) / latt])
+    recip_volume = abs(np.dot(np.cross(lattice[0], lattice[1]), lattice[2]))
+
+    # Calculatate the reciprocal lattice vectors (need factor of 2 pi)
+    recip_latt = np.linalg.inv(lattice).T * 2 * np.pi
+
+    real_space = _get_real_space(conv, inv_diel, det_diel, r_c, axis, sup_latt)
+    reciprocal = _get_recip(
+        conv,
+        recip_axis,
+        recip_volume,
+        recip_latt,
+        dielectric_matrix,
+    )
 
-    def get_defects_concentration_old(self, temp=300, ef=0.0):
-        """
-        get the defect concentration for a temperature and Fermi level
-        Written when the site multiplicity is not supplied with ComputedDefect
-        Args:
-            temp:
-                the temperature in K
-            Ef:
-                the fermi level in eV (with respect to the VBM)
-        Returns:
-            a list of dict of {'name': defect name, 'charge': defect charge
-                               'conc': defects concentration in m-3}
-        """
-        conc = []
-        spga = SpacegroupAnalyzer(self._entry_bulk.structure, symprec=1e-1)
-        struct = spga.get_symmetrized_structure()
-        i = 0
-        for d in self._defects:
-            df_coords = d.site.frac_coords
-            target_site = None
-            for s in struct.sites:
-                sf_coords = s.frac_coords
-                if (
-                    abs(s.frac_coords[0] - df_coords[0]) < 0.1
-                    and abs(s.frac_coords[1] - df_coords[1]) < 0.1
-                    and abs(s.frac_coords[2] - df_coords[2]) < 0.1
-                ):
-                    target_site = s
-                    break
-            equiv_site_no = len(struct.find_equivalent_sites(target_site))
-            n = equiv_site_no * 1e30 / struct.volume
-            conc.append(
-                {
-                    "name": d.name,
-                    "charge": d.charge,
-                    "conc": n * exp(-self._get_form_energy(ef, i) / (kb * temp)),
-                }
+    # calculate the other terms and the final Madelung potential
+    third_term = -2 * conv / np.sqrt(np.pi * det_diel)
+    fourth_term = -3.141592654 / (recip_volume * conv**2)
+    madelung = -(real_space + reciprocal + third_term + fourth_term)
+
+    # convert to atomic units
+    conversion = 14.39942
+    real_ev = real_space * conversion / 2
+    recip_ev = reciprocal * conversion / 2
+    third_ev = third_term * conversion / 2
+    fourth_ev = fourth_term * conversion / 2
+    madelung_ev = madelung * conversion / 2
+
+    correction = {}
+    for q in range(1, 8):
+        makov = 0.5 * madelung * q**2 * conversion
+        lany = 0.65 * makov
+        correction[q] = makov
+
+    if verbose:
+        print(
+            """
+    Results                      v_M^scr    dE(q=1) /eV
+    -----------------------------------------------------
+    Real space contribution    =  {:.6f}     {:.6f}
+    Reciprocal space component =  {:.6f}     {:.6f}
+    Third term                 = {:.6f}    {:.6f}
+    Neutralising background    = {:.6f}    {:.6f}
+    -----------------------------------------------------
+    Final Madelung potential   = {:.6f}     {:.6f}
+    -----------------------------------------------------""".format(
+                real_space,
+                real_ev,
+                reciprocal,
+                recip_ev,
+                third_term,
+                third_ev,
+                fourth_term,
+                fourth_ev,
+                madelung,
+                madelung_ev,
             )
-            i += 1
-        return conc
+        )
 
-    def _get_dos(self, e, m1, m2, m3, e_ext):
-        return sqrt(2) / (pi**2 * hbar**3) * sqrt(m1 * m2 * m3) * sqrt(e - e_ext)
+        print(
+            """
+    Here are your final corrections:
+    +--------+------------------+-----------------+
+    | Charge | Point charge /eV | Lany-Zunger /eV |
+    +--------+------------------+-----------------+"""
+        )
+        for q in range(1, 8):
+            makov = 0.5 * madelung * q**2 * conversion
+            lany = 0.65 * makov
+            correction[q] = makov
+            print("|   {}    |     {:10f}   |    {:10f}   |".format(q, makov, lany))
+        print("+--------+------------------+-----------------+")
+    return correction
 
-    def _get_dos_fd_elec(self, e, ef, t, m1, m2, m3):
-        return (
-            conv
-            * (2.0 / (exp((e - ef) / (kb * t)) + 1))
-            * (sqrt(2) / (pi**2))
-            * sqrt(m1 * m2 * m3)
-            * sqrt(e - self._band_gap)
-        )
 
-    def _get_dos_fd_hole(self, e, ef, t, m1, m2, m3):
-        return (
-            conv
-            * (exp((e - ef) / (kb * t)) / (exp((e - ef) / (kb * t)) + 1))
-            * (2.0 * sqrt(2) / (pi**2))
-            * sqrt(m1 * m2 * m3)
-            * sqrt(-e)
-        )
+def _get_real_space(conv, inv_diel, det_diel, r_c, axis, sup_latt):
+    # Calculate real space component
+    real_space = 0.0
+    axis_ranges = [range(-a, a) for a in axis]
+
+    # Pre-compute square of cutoff distance for cheaper comparison than
+    # separation < r_c
+    r_c_sq = r_c**2
+
+    def _real_loop_function(mno):
+        # Calculate the defect's fractional position in extended supercell
+        d_super = np.array(mno, dtype=float) / axis
+        d_super_cart = np.dot(d_super, sup_latt)
+
+        # Test if the new atom coordinates fall within r_c, then solve
+        separation_sq = np.sum(np.square(d_super_cart))
+        # Take all cases within r_c except m,n,o != 0,0,0
+        if separation_sq < r_c_sq and any(mno):
+            mod = np.dot(d_super_cart, inv_diel)
+            dot_prod = np.dot(mod, d_super_cart)
+            N = np.sqrt(dot_prod)
+            contribution = 1 / np.sqrt(det_diel) * erfc(conv * N) / N
+            return contribution
+        else:
+            return 0.0
 
-    def _get_qd(self, ef, t):
-        summation = 0.0
-        for d in self.get_defects_concentration(t, ef):
-            summation += d["charge"] * d["conc"]
-        return summation
+    real_space = sum(
+        _real_loop_function(mno) for mno in itertools.product(*axis_ranges)
+    )
+    return real_space
 
-    def get_qi(self, ef, t, m_elec, m_hole):
-        from scipy import integrate as intgrl
 
-        elec_den_fn = lambda e: self._get_dos_fd_elec(
-            e, ef, t, m_elec[0], m_elec[1], m_elec[2]
-        )
-        hole_den_fn = lambda e: self._get_dos_fd_hole(
-            e, ef, t, m_hole[0], m_hole[1], m_hole[2]
-        )
+def _get_recip(
+    conv,
+    recip_axis,
+    recip_volume,
+    recip_latt,
+    dielectric_matrix,
+):
+    # convert factional motif to reciprocal space and
+    # calculate reciprocal space supercell parallelpiped
+    recip_sup_latt = np.dot(np.diag(recip_axis), recip_latt)
+
+    # Calculate reciprocal space component
+    axis_ranges = [range(-a, a) for a in recip_axis]
+
+    def _recip_loop_function(mno):
+        # Calculate the defect's fractional position in extended supercell
+        d_super = np.array(mno, dtype=float) / recip_axis
+        d_super_cart = np.dot(d_super, recip_sup_latt)
+
+        if any(mno):
+            mod = np.dot(d_super_cart, dielectric_matrix)
+            dot_prod = np.dot(mod, d_super_cart)
+            contribution = exp(-dot_prod / (4 * conv**2)) / dot_prod
+            return contribution
+        else:
+            return 0.0
 
-        bg = self._band_gap
-        elec_count = -intgrl.quad(elec_den_fn, bg, bg + 5)[0]
-        hole_count = intgrl.quad(hole_den_fn, -5, 0.0)[0]
-
-        return elec_count + hole_count
-
-    def _get_qtot(self, ef, t, m_elec, m_hole):
-        return self._get_qd(ef, t) + self.get_qi(ef, t, m_elec, m_hole)
-
-    def get_eq_ef(self, t, m_elec, m_hole):
-        """
-        access to equilibrium values of Fermi level and concentrations
-        in defects and carriers obtained by self-consistent solution of
-        charge balance + defect and carriers concentrations
-        Args:
-            t: temperature in K
-            m_elec: electron effective mass as a 3 value list
-                    (3 eigenvalues for the tensor)
-            m_hole:: hole effective mass as a 3 value list
-                    (3 eigenvalues for the tensor)
-        Returns:
-            a dict with {
-                'ef':eq fermi level,
-                'Qi': the concentration of carriers
-                      (positive for holes, negative for e-) in m^-3,
-                'conc': the concentration of defects as a list of dicts
-                }
-        """
-        from scipy.optimize import bisect
-
-        e_vbm = self._e_vbm
-        e_cbm = self._e_vbm + self._band_gap
-        ef = bisect(lambda e: self._get_qtot(e, t, m_elec, m_hole), 0, self._band_gap)
-        return {
-            "ef": ef,
-            "Qi": self.get_qi(ef, t, m_elec, m_hole),
-            "QD": self._get_qd(ef, t),
-            "conc": self.get_defects_concentration(t, ef),
-        }
-
-    def get_non_eq_ef(self, tsyn, teq, m_elec, m_hole):
-        """
-        access to the non-equilibrium values of Fermi level and
-        concentrations in defects and carriers obtained by
-        self-consistent solution of charge balance + defect and
-        carriers concentrations
-
-        Implemented following Sun, R., Chan, M. K. Y., Kang, S.,
-        and Ceder, G. (2011). doi:10.1103/PhysRevB.84.035212
-
-        Args:
-            tsyn: the synthesis temperature in K
-            teq: the temperature of use in K
-            m_elec: electron effective mass as a 3 value list
-                    (3 eigenvalues for the tensor)
-            m_hole: hole effective mass as a 3 value list
-                    (3 eigenvalues for the tensor)
-        Returns:
-            a dict with {
-                'ef':eq fermi level,
-                'Qi': the concentration of carriers
-                      (positive for holes, negative for e-) in m^-3,
-                'conc': the concentration of defects as a list of dict
-                }
-        """
-        from scipy.optimize import bisect
-
-        eqsyn = self.get_eq_ef(tsyn, m_elec, m_hole)
-        cd = {}
-        for c in eqsyn["conc"]:
-            if c["name"] in cd:
-                cd[c["name"]] += c["conc"]
-            else:
-                cd[c["name"]] = c["conc"]
-        ef = bisect(
-            lambda e: self._get_non_eq_qtot(cd, e, teq, m_elec, m_hole),
-            -1.0,
-            self._band_gap + 1.0,
-        )
-        return {
-            "ef": ef,
-            "Qi": self.get_qi(ef, teq, m_elec, m_hole),
-            "conc_syn": eqsyn["conc"],
-            "conc": self._get_non_eq_conc(cd, ef, teq),
-        }
-
-    def _get_non_eq_qd(self, cd, ef, t):
-        sum_tot = 0.0
-        for n in cd:
-            sum_d = 0.0
-            sum_q = 0.0
-            i = 0
-            for d in self._defects:
-                if d.name == n:
-                    sum_d += exp(-self._get_form_energy(ef, i) / (kb * t))
-                    sum_q += d.charge * exp(-self._get_form_energy(ef, i) / (kb * t))
-                i += 1
-            sum_tot += cd[n] * sum_q / sum_d
-        return sum_tot
-
-    def _get_non_eq_conc(self, cd, ef, t):
-        sum_tot = 0.0
-        res = []
-        for n in cd:
-            sum_tot = 0
-            i = 0
-            for d in self._defects:
-                if d.name == n:
-                    sum_tot += exp(-self._get_form_energy(ef, i) / (kb * t))
-                i += 1
-            i = 0
-            for d in self._defects:
-                if d.name == n:
-                    res.append(
-                        {
-                            "name": d.name,
-                            "charge": d.charge,
-                            "conc": cd[n]
-                            * exp(-self._get_form_energy(ef, i) / (kb * t))
-                            / sum_tot,
-                        }
-                    )
-                i += 1
-        return res
-
-    def _get_non_eq_qtot(self, cd, ef, t, m_elec, m_hole):
-        return self._get_non_eq_qd(cd, ef, t) + self.get_qi(ef, t, m_elec, m_hole)
-
-    def correct_bg(self, dict_levels, vbm_correct, cbm_correct):
-        """
-        NOTE from developers: This code uses deprecated concepts and
-            will not be used or maintained going forward (as of 12/15/2017).
-            However, we are keeping function here to allow for
-            current users to make use of it...
-
-        correct the band gap in the analyzer and make sure the levels move
-        accordingly.
-        There are two types of defects vbm_like and cbm_like and we need
-        to provide a formal oxidation state
-        The vbm-like will follow the vbm and the cbm_like the cbm. If nothing
-        is specified the defect transition level does not move
-        Args:
-            dict_levels: a dictionary of type {defect_name:
-            {'type':type_of_defect,'q*':formal_ox_state}}
-            Where type_of_defect is a string: 'vbm_like' or 'cbm_like'
-        """
-        self._band_gap = self._band_gap + cbm_correct + vbm_correct
-        self._e_vbm = self._e_vbm - vbm_correct
-        self._compute_form_en()
-        for i in range(len(self._defects)):
-            name = self._defects[i].name
-            if not name in dict_levels:
-                continue
-
-            if dict_levels[name]["type"] == "vbm_like":
-                z = self._defects[i].charge - dict_levels[name]["q*"]
-                self._formation_energies[i] += z * vbm_correct
-            if dict_levels[name]["type"] == "cbm_like":
-                z = dict_levels[name]["q*"] - self._defects[i].charge
-                self._formation_energies[i] += z * cbm_correct
-
-    def get_defect_occupancies(self):
-        """
-        NOTE from developers: This code uses deprecated concepts and
-            will not be used or maintained going forward (as of 12/15/2017).
-            However, we are keeping function here to allow for
-            current users to make use of it...
-
-        Defect occupancies with respect to defect chargest.
-        The assumption is that the highest charge of defect numerically
-        has zero occupancy:
-        Ex: In Cr2O3, V_O has 0 occupancy for +2 q and 2 occupancy for 0 q.
-            V_{Cr} has 0 occupancy for 0 q and 3 occupancy for -3 q
-        Caution: Didn't check for semiconductor with large # of defect q's.
-        Returns:
-            Defect occupancies as a nested dict
-        """
-        charges = defaultdict(list)
-        for dfct in self._defects:
-            charges[dfct.name].append(dfct.charge)
-
-        occupancies = defaultdict(lambda: defaultdict(int))
-        for dfct_name in charges:
-            for i, q in enumerate(sorted(charges[dfct_name], reverse=True)):
-                occupancies[dfct_name][q] = i
-            occupancies[dfct_name]["0_occupancy"] = sorted(
-                charges[dfct_name], reverse=True
-            )[0]
-        return occupancies
+    reciprocal = sum(
+        _recip_loop_function(mno) for mno in itertools.product(*axis_ranges)
+    )
+    scale_factor = 4 * np.pi / recip_volume
+    return reciprocal * scale_factor
```

### Comparing `doped-1.0.9/doped/pycdt/core/defectsmaker.py` & `doped-1.1.0/doped/pycdt/core/defectsmaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 
 """
 Code to generate charged defects structure files.
 """
 
 
 import abc
-import re
 from tabulate import tabulate
 
 from monty.serialization import dumpfn
 from pymatgen.analysis.defects.core import Interstitial
 from pymatgen.analysis.defects.generators import (
-    InterstitialGenerator,
     SimpleChargeGenerator,
     SubstitutionGenerator,
     VacancyGenerator,
     VoronoiInterstitialGenerator,
 )
 from pymatgen.analysis.local_env import ValenceIonicRadiusEvaluator as VIRE
 from pymatgen.core.periodic_table import Element, Specie, get_el_sp
@@ -377,15 +375,14 @@
                 return [-1, 0, 1]
             else:
                 minval = min(-vac_oxi_state, 0)
                 maxval = max(-vac_oxi_state, 0)
                 return [c for c in range(minval - 1, maxval + 2)]
 
         elif defect_type in ["antisite", "substitution"]:
-            # TODO: may cause some weird states for substitutions. Worth updating in future.
             vac_symbol = get_el_sp(site_specie).symbol
             vac_oxi_state = self.oxi_states[vac_symbol]
             as_symbol = get_el_sp(sub_specie).symbol
             as_oxi_state = self.oxi_states[as_symbol]
             expected_oxi = as_oxi_state - vac_oxi_state
             if expected_oxi == 0:
                 return [-1, 0, 1]
@@ -746,15 +743,15 @@
                         as_defs.append(
                             {
                                 "name": f"as_{i+1}_{as_symbol}_on_{vac_symbol}",
                                 "unique_site": as_site,
                                 "bulk_supercell_site": as_sc_site,
                                 "defect_type": "antisite",
                                 "site_specie": vac_symbol,
-                                "substituting_specie": as_symbol,
+                                "substitution_specie": as_symbol,
                                 "site_multiplicity": sub.multiplicity,
                                 "supercell": {"size": sc_scale, "structure": as_sc},
                                 "charges": charges_as,
                                 "Possible_KV_Charge": c.charge,
                             }
                         )
 
@@ -834,60 +831,69 @@
             if len(inter_elems) == 0:
                 raise RuntimeError("empty element list for interstitials")
 
             if intersites:
                 print("Setting up interstitials from intersites")
                 # manual specification of interstitials
                 for i, intersite in enumerate(intersites):
-                    elt = intersite.specie
-                    name = f"inter_{i+1}_{elt}"
+                    for elt in inter_elems:
+                        name = f"inter_{i+1}_{elt}"
 
-                    if intersite.lattice != self.struct.lattice:
-                        err_msg = "Lattice matching error occurs between provided interstitial and the bulk structure."
-                        if standardized:
-                            err_msg += (
-                                "\nLikely because the standardized flag was used. Turn this flag off or reset "
-                                "your interstitial PeriodicSite to match the standardized form of the bulk structure."
+                        if intersite.lattice != self.struct.lattice:
+                            err_msg = (
+                                "Lattice matching error occurs between provided "
+                                "interstitial and the bulk structure."
                             )
-                        raise ValueError(err_msg)
-                    else:
-                        intersite_object = Interstitial(self.struct, intersite)
+                            if standardized:
+                                err_msg += (
+                                    "\nLikely because the standardized flag was used. "
+                                    "Turn this flag off or reset "
+                                    "your interstitial PeriodicSite to match the "
+                                    "standardized form of the bulk structure."
+                                )
+                            raise ValueError(err_msg)
+                        else:
+                            intersite_object = Interstitial(self.struct, intersite)
 
-                    # create a trivial defect structure to find where supercell transformation
-                    # moves the defect site
-                    struct_for_defect_site = Structure(
-                        intersite_object.bulk_structure.copy().lattice,
-                        [intersite_object.site.specie],
-                        [intersite_object.site.frac_coords],
-                        to_unit_cell=True,
-                        coords_are_cartesian=False,
-                    )
-                    struct_for_defect_site.make_supercell(sc_scale)
-                    site_sc = struct_for_defect_site[0]
-
-                    sc_with_inter = intersite_object.generate_defect_structure(sc_scale)
-                    charges_inter = self.defect_charger.get_charges("interstitial", elt)
+                        # create a trivial defect structure to find where supercell transformation
+                        # moves the defect site
+                        struct_for_defect_site = Structure(
+                            intersite_object.bulk_structure.copy().lattice,
+                            [intersite_object.site.specie],
+                            [intersite_object.site.frac_coords],
+                            to_unit_cell=True,
+                            coords_are_cartesian=False,
+                        )
+                        struct_for_defect_site.make_supercell(sc_scale)
+                        site_sc = struct_for_defect_site[0]
 
-                    for c in SimpleChargeGenerator(intersite_object):
-                        interstitials.append(
-                            {
-                                "name": name,
-                                "unique_site": intersite_object.site,
-                                "bulk_supercell_site": site_sc,
-                                "defect_type": "interstitial",
-                                "site_specie": intersite_object.site.specie.symbol,
-                                "site_multiplicity": intersite_object.multiplicity,
-                                "supercell": {
-                                    "size": sc_scale,
-                                    "structure": sc_with_inter,
-                                },
-                                "charges": charges_inter,
-                                "Possible_KV_Charge": c.charge,
-                            }
+                        sc_with_inter = intersite_object.generate_defect_structure(
+                            sc_scale
                         )
+                        charges_inter = self.defect_charger.get_charges(
+                            "interstitial", elt
+                        )
+
+                        for c in SimpleChargeGenerator(intersite_object):
+                            interstitials.append(
+                                {
+                                    "name": name,
+                                    "unique_site": intersite_object.site,
+                                    "bulk_supercell_site": site_sc,
+                                    "defect_type": "interstitial",
+                                    "site_specie": intersite_object.site.specie.symbol,
+                                    "site_multiplicity": intersite_object.multiplicity,
+                                    "supercell": {
+                                        "size": sc_scale,
+                                        "structure": sc_with_inter,
+                                    },
+                                    "charges": charges_inter,
+                                    "Possible_KV_Charge": c.charge,
+                                }
+                            )
 
             else:
                 print(
                     "Searching for Voronoi interstitial sites (this can take a little while)"
                 )
                 # the use of O here is completely arbitrary
                 IG = VoronoiInterstitialGenerator(self.struct, "O")
```

### Comparing `doped-1.0.9/doped/pycdt/core/tests/test_defectsmaker.py` & `doped-1.1.0/doped/pycdt/core/tests/test_defectsmaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pymatgen.core import PeriodicSite
 from pymatgen.core.structure import Structure
 from pymatgen.util.testing import PymatgenTest
 
 from doped.pycdt.core.defectsmaker import *
 
-file_loc = os.path.abspath(os.path.join(__file__, "..", "..", "..", "..", "test_files"))
+file_loc = os.path.abspath(os.path.join(__file__, "..", "..", "..", "test_files"))
 
 
 class GetOptimizedScScaleTest(PymatgenTest):
     def setUp(self):
         self.gaas_prim_struct = Structure.from_file(
             os.path.join(file_loc, "POSCAR_GaAs")
         )
@@ -178,19 +178,18 @@
         self.assertEqual(self.ga_site, check_subs["sub_1_In_on_Ga"])
         self.assertEqual(self.as_site, check_subs["sub_2_Sb_on_As"])
 
         # Test automatic interstitial finding.
         CDS = ChargedDefectsStructures(
             self.gaas_struct, include_interstitials=True, interstitial_elements=["Mn"]
         )
-        self.assertEqual(CDS.get_n_defects_of_type("interstitials"), 2)
+        self.assertEqual(CDS.get_n_defects_of_type("interstitials"), 3)
         fnames = [
             i["name"][i["name"].index("M") :] for i in CDS.defects["interstitials"]
         ]
-        self.assertEqual(sorted(fnames), sorted(["Mn_InFiT1_mult6", "Mn_InFiT2_mult6"]))
         nsites = len(CDS.defects["interstitials"][0]["supercell"]["structure"].sites)
         self.assertEqual(
             len(CDS.get_ith_supercell_of_defect_type(0, "interstitials").sites), nsites
         )
         self.assertEqual(
             CDS.defects["interstitials"][0]["charges"], [0, 1, 2, 3, 4, 5, 6, 7]
         )
```

### Comparing `doped-1.0.9/doped/pycdt/utils/parse_calculations.py` & `doped-1.1.0/doped/pycdt/utils/parse_calculations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,185 +1,126 @@
 # coding: utf-8
 """
 Parses the computed data from VASP defect calculations.
 """
-# from __future__ import unicode_literals
-from __future__ import division
 
 import glob
-import logging
 import os
 import warnings
 
 import numpy as np
 from monty.json import MontyDecoder
 from monty.serialization import dumpfn, loadfn
 from pymatgen.analysis.defects.core import (
     DefectEntry,
     Interstitial,
     Substitution,
     Vacancy,
 )
 from pymatgen.analysis.defects.defect_compatibility import DefectCompatibility
-from pymatgen.analysis.defects.utils import TopographyAnalyzer
 from pymatgen.analysis.structure_matcher import StructureMatcher
 from pymatgen.core import PeriodicSite, Structure
 from pymatgen.entries.computed_entries import ComputedStructureEntry
 from pymatgen.ext.matproj import MPRester
 from pymatgen.io.vasp.inputs import Potcar, UnknownPotcarWarning
 from pymatgen.io.vasp.outputs import Locpot, Outcar, Poscar, Vasprun
 from pymatgen.util.coord import pbc_diff
 
 from doped.pycdt.core import _chemical_potentials
+from doped import _ignore_pmg_warnings
 
-_ANGSTROM = "\u212B"  # unicode symbol for angstrom to print in strings
+_ignore_pmg_warnings()
 
-# globally ignore these POTCAR warnings
-warnings.filterwarnings("ignore", category=UnknownPotcarWarning)
-warnings.filterwarnings("ignore", message="No POTCAR file with matching TITEL fields")
-warnings.filterwarnings("ignore", message="Ignoring unknown variable type")
-
-# until updated from pymatgen==2022.7.25 :
-warnings.filterwarnings(
-    "ignore", message="Using `tqdm.autonotebook.tqdm` in notebook mode"
-)
-warnings.filterwarnings(
-    "ignore", message="`np.int` is a deprecated alias for the builtin `int`"
-)
-warnings.filterwarnings("ignore", message="Use get_magnetic_symmetry()")
 
-
-def custom_formatwarning(msg, *args, **kwargs):
+def _custom_formatwarning(msg, *args, **kwargs):
     """Reformat warnings to just print the warning message"""
     return f"{msg}\n"
 
 
-warnings.formatwarning = custom_formatwarning
-
-
-def convert_cd_to_de(cd, b_cse):
-    """
-    As of pymatgen v2.0, ComputedDefect objects were deprecated in favor
-    of DefectEntry objects in pymatgen.analysis.defects.core
-    This function takes a ComputedDefect (either as a dict or object) and
-    converts it into a DefectEntry object in order to handle legacy
-    PyCDT creation within the current paradigm of PyCDT.
-
-    :param cd (dict or ComputedDefect object): ComputedDefect as an object or as a dictionary
-    :params b_cse (dict or ComputedStructureEntry object): ComputedStructureEntry of bulk entry
-        associated with the ComputedDefect.
-    :return: de (DefectEntry): Resulting DefectEntry object
-    """
-    if isinstance(cd, dict):
-        cd = cd.as_dict()
-    if isinstance(b_cse, dict):
-        b_cse = b_cse.as_dict()
-
-    bulk_sc_structure = Structure.from_dict(b_cse["structure"])
-
-    # modify defect_site as required for Defect object, confirming site exists in bulk structure
-    site_cls = cd["site"]
-    defect_site = PeriodicSite.from_dict(site_cls)
-    def_nom = cd["name"].lower()
-    if "sub_" in def_nom or "as_" in def_nom:
-        # modify site object for substitution site of Defect object
-        site_cls["species"][0]["element"] = cd["name"].split("_")[2]
-        defect_site = PeriodicSite.from_dict(site_cls)
-
-    poss_deflist = sorted(
-        bulk_sc_structure.get_sites_in_sphere(
-            defect_site.coords, 0.2, include_index=True
-        ),
-        key=lambda x: x[1],
-    )
-    if len(poss_deflist) != 1:
-        raise ValueError(
-            "ComputedDefect to DefectEntry conversion failed. "
-            "Could not determine periodic site position in bulk supercell."
-        )
-
-    # create defect object
-    if "vac_" in def_nom:
-        defect_obj = Vacancy(bulk_sc_structure, defect_site, charge=cd["charge"])
-    elif "as_" in def_nom or "sub_" in def_nom:
-        defect_obj = Substitution(bulk_sc_structure, defect_site, charge=cd["charge"])
-    elif "int_" in def_nom:
-        defect_obj = Interstitial(bulk_sc_structure, defect_site, charge=cd["charge"])
-    else:
-        raise ValueError(f"Could not recognize defect type for {cd['name']}")
-
-    # assign proper energy and parameter metadata
-    uncorrected_energy = cd["entry"]["energy"] - b_cse["energy"]
-    def_path = os.path.split(cd["entry"]["data"]["locpot_path"])[0]
-    bulk_path = os.path.split(b_cse["data"]["locpot_path"])[0]
-    p = {
-        "defect_path": def_path,
-        "bulk_path": bulk_path,
-        "encut": cd["entry"]["data"]["encut"],
-    }
-
-    de = DefectEntry(defect_obj, uncorrected_energy, parameters=p)
-
-    return de
+warnings.formatwarning = _custom_formatwarning
 
 
 def get_vasprun(vasprun_path, **kwargs):
     """Read the vasprun.xml(.gz) file as a pymatgen Vasprun object"""
     vasprun_path = str(vasprun_path)  # convert to string if Path object
     warnings.filterwarnings(
         "ignore", category=UnknownPotcarWarning
     )  # Ignore POTCAR warnings when loading vasprun.xml
     # pymatgen assumes the default PBE with no way of changing this within get_vasprun())
     warnings.filterwarnings(
         "ignore", message="No POTCAR file with matching TITEL fields"
     )
-    if os.path.exists(vasprun_path):
-        vasprun = Vasprun(vasprun_path)
-        read_vasprun_path = vasprun_path
-    elif os.path.exists(vasprun_path + ".gz", **kwargs):
-        vasprun = Vasprun(vasprun_path + ".gz", **kwargs)
-        read_vasprun_path = vasprun_path + ".gz"
+    if os.path.exists(vasprun_path) and os.path.isfile(vasprun_path):
+        vasprun = Vasprun(vasprun_path, **kwargs)
     else:
         raise FileNotFoundError(
-            f"""vasprun.xml(.gz) not found at {vasprun_path}(.gz). Needed for parsing defect 
-            calculations."""
+            f"vasprun.xml file not found at {vasprun_path}. Needed for parsing calculation output."
         )
-    return vasprun, read_vasprun_path
+    return vasprun
 
 
 def get_locpot(locpot_path):
     """Read the LOCPOT(.gz) file as a pymatgen Locpot object"""
     locpot_path = str(locpot_path)  # convert to string if Path object
-    if os.path.exists(locpot_path):
+    if os.path.exists(locpot_path) and os.path.isfile(locpot_path):
         locpot = Locpot.from_file(locpot_path)
-    elif os.path.exists(locpot_path + ".gz"):
-        locpot = Locpot.from_file(locpot_path + ".gz")
     else:
         raise FileNotFoundError(
-            f"""LOCPOT(.gz) not found at {locpot_path}(.gz). Needed for calculating the 
-            Freysoldt (FNV) image charge corrections."""
+            f"LOCPOT file not found at {locpot_path}. Needed for calculating the Freysoldt (FNV) "
+            f"image charge correction."
         )
     return locpot
 
 
 def get_outcar(outcar_path):
     """Read the OUTCAR(.gz) file as a pymatgen Outcar object"""
     outcar_path = str(outcar_path)  # convert to string if Path object
-    if os.path.exists(outcar_path):
+    if os.path.exists(outcar_path) and os.path.isfile(outcar_path):
         outcar = Outcar(outcar_path)
-    elif os.path.exists(outcar_path + ".gz"):
-        outcar = Outcar(outcar_path + ".gz")
     else:
         raise FileNotFoundError(
-            f"""OUTCAR(.gz) not found at {outcar_path}(.gz). Needed for calculating the Kumagai (
-            eFNV) image charge corrections."""
+            f"OUTCAR file not found at {outcar_path}. Needed for calculating the Kumagai (eFNV) "
+            f"image charge correction."
         )
     return outcar
 
 
+def _get_output_files_and_check_if_multiple(output_file="vasprun.xml", path="."):
+    """
+    Search for all files with filenames matching `output_file`, case-insensitive.
+
+    Returns (output file path, Multiple?) where Multiple is True if multiple matching files are
+    found.
+    """
+    files = os.listdir(path)
+    output_files = [
+        filename for filename in files if output_file.lower() in filename.lower()
+    ]
+    # sort by, direct match to output_file, direct match to output_file with .gz extension,
+    # then alphabetically:
+    output_files = sorted(
+        output_files,
+        key=lambda x: (
+            x == output_file,
+            x == output_file + ".gz",
+            x,
+        ),
+        reverse=True,
+    )
+    if output_files:
+        output_path = os.path.join(path, output_files[0])
+        if len(output_files) > 1:
+            return output_path, True
+        else:
+            return output_path, False
+    else:
+        return path, False  # so when `get_X()` is called, it will raise an
+        # informative FileNotFoundError
+
+
 def get_defect_type_and_composition_diff(bulk, defect):
     """Get the difference in composition between a bulk structure and a defect structure.
     Contributed by Dr. Alex Ganose (@ Imperial Chemistry) and refactored for extrinsic species
     """
     bulk_comp = bulk.composition.get_el_amt_dict()
     defect_comp = defect.composition.get_el_amt_dict()
 
@@ -377,35 +318,74 @@
     return (
         bulk_site_idx,
         defect_site_idx,
         unrelaxed_defect_structure,
     )
 
 
-class SingleDefectParser:
-    # TODO: Given this is our recommended workflow, should streamline this similar to in
-    #  `vasp_input.py`, where it tries to run the freysoldt/kumagai loader (chosen by an
-    #  optional imput parameter, if not set check if OUTCAR/LOCPOT present), throw warning if not
-    #  successful, then `get_stdrd_metadata()`, `get_bulk_gap_data()` and `run_compatibility()` (
-    #  again throwing warnings for any of these that don't work) – so replacing 4+ function calls
-    #  with just one.
-    # TODO: Should also add check the bulk and defect KPOINTS/INCAR/POTCAR/POSCAR (size) settings
-    #  are compatible, and throw warning if not.
-    # TODO: Add `check_defects_compatibility()` function that checks the bulk and defect
-    #  KPOINTS/INCAR/POTCAR/POSCAR (size) settings for all defects in the supplied defect_dict
-    #  are compatible, if not throw warnings and say what the differences are. Should recommend
-    #  using this in the example notebook if a user has parsed the defects individually (rather
-    #  than with the single looping function described below):
-    # TODO: Add a function that loops over all the defects in a directory (with `defect_dir = .`,
-    #  and `subfolder = vasp_ncl` options) and parses them all, returning a dictionary of defect
-    #  entries, with the defect name as the key. (i.e. doing the loop in the example notebook).
-    #  Show both this function and the individual function calls in the example notebook. Benefit
-    #  of this one is that we can then auto-run `check_defects_compatibility()` at the end of
-    #  parsing the full defects dict.
+def get_site_mapping_indices(
+    structure_a: Structure, structure_b: Structure, threshold=2.0
+):
+    """
+    Reset the position of a partially relaxed structure to its unrelaxed positions.
+    The template structure may have a different species ordering to the `input_structure`.
+    """
+
+    ## Generate a site matching table between the input and the template
+    input_fcoords = [site.frac_coords for site in structure_a]
+    template_fcoords = [site.frac_coords for site in structure_b]
+
+    dmat = structure_a.lattice.get_all_distances(input_fcoords, template_fcoords)
+    min_dist_with_index = []
+    for index in range(len(input_fcoords)):
+        dists = dmat[index]
+        template_index = dists.argmin()
+        current_dist = dists.min()
+        min_dist_with_index.append(
+            [
+                current_dist,
+                index,
+                template_index,
+            ]
+        )
+
+        if current_dist > threshold:
+            sitea = structure_a[index]
+            siteb = structure_b[template_index]
+            warnings.warn(
+                f"Large site displacement {current_dist:.4f} detected when matching atomic sites:"
+                f" {sitea}-> {siteb}."
+            )
+    return min_dist_with_index
+
 
+def reorder_unrelaxed_structure(
+    unrelaxed_structure: Structure, initial_relax_structure: Structure, threshold=2.0
+):
+    """
+    Reset the position of a partially relaxed structure to its unrelaxed positions.
+    The template structure may have a different species ordering to the `input_structure`.
+    """
+
+    # Obtain site mapping between the initial_relax_structure and the unrelaxed structure
+    mapping = get_site_mapping_indices(
+        initial_relax_structure, unrelaxed_structure, threshold=threshold
+    )
+
+    # Reorder the unrelaxed_structure so it matches the ordering of the initial_relax_structure (
+    # from the actual calculation)
+    reordered_sites = [unrelaxed_structure[tmp[2]] for tmp in mapping]
+    new_structure = Structure.from_sites(reordered_sites)
+
+    assert len(new_structure) == len(unrelaxed_structure)
+
+    return new_structure
+
+
+class SingleDefectParser:
     _delocalization_warning_printed = False  # class variable
     # ensures the verbose delocalization analysis warning is only printed once. Needs to be done
     # this way because the current workflow is to create a `SingleDefectParser` object for each
     # defect, and then warning originates from the `run_compatibility()` method of different
     # `SingleDefectParser` instances, so warnings detects each instance as a different source and
     # prints the warning multiple times. When we move to a single function call for all defects
     # (as described above), this can be removed.
@@ -442,298 +422,61 @@
 
         """
         self.defect_entry = defect_entry
         self.compatibility = compatibility
         self.defect_vr = defect_vr
         self.bulk_vr = bulk_vr
 
-    @staticmethod
+    @classmethod
     def from_paths(
-        path_to_defect,
-        path_to_bulk,
+        self,
+        defect_path,
+        bulk_path,
         dielectric,
-        defect_charge,
-        mpid=None,
-        compatibility=DefectCompatibility(
-            plnr_avg_var_tol=0.01,
-            plnr_avg_minmax_tol=0.3,
-            atomic_site_var_tol=0.025,
-            atomic_site_minmax_tol=0.3,
-            tot_relax_tol=5.0,
-            defect_tot_relax_tol=5.0,
-            use_bandfilling=False,  # don't include bandfilling by default
-            use_bandedgeshift=False,  # don't include band edge shift by default
-        ),
+        charge=None,
         initial_defect_structure=None,
+        skip_corrections=False,
+        bulk_bandgap_path=None,
+        **kwargs,
     ):
         """
-        Identify defect object based on file paths. Minimal parsing performing for
-        instantiating the SingleDefectParser class.
+        Parse the defect calculation outputs in `defect_path` and return the parsed `DefectEntry`
+        object.
 
         Args:
-        path_to_defect (str): path to defect folder of interest (with vasprun.xml(.gz))
-        path_to_bulk (str): path to bulk folder of interest (with vasprun.xml(.gz))
+        defect_path (str): path to defect folder of interest (with vasprun.xml(.gz))
+        bulk_path (str): path to bulk folder of interest (with vasprun.xml(.gz))
         dielectric (float or int or 3x1 matrix or 3x3 matrix):
             ionic + static contributions to dielectric constant
-        defect_charge (int):  charge of defect
-        mpid (str):  Materials Project ID of bulk structure
-        compatibility (DefectCompatibility): Compatibility class instance for
-            performing charge correction compatibility analysis on defect entry.
+        charge (int): charge of defect. If not provided, will be automatically determined
+            from the defect calculation outputs (requires POTCARs to be set up with `pymatgen`).
         initial_defect_structure (str):  Path to the unrelaxed defect structure,
             if structure matching with the relaxed defect structure(s) fails.
+        skip_corrections (bool): Whether to skip the calculation and application of finite-size
+            charge corrections to the defect energy.
+        bulk_bandgap_path (str): Path to bulk OUTCAR file for determining the band gap. If the
+            VBM/CBM occur at reciprocal space points not included in the bulk supercell calculation,
+            you should use this tag to point to a bulk bandstructure calculation instead. If None,
+            will use self.defect_entry.parameters["bulk_path"].
 
         Return:
-            Instance of the SingleDefectParser class.
+            Parsed `DefectEntry` object.
         """
-        # check if dielectric in required 3x3 matrix format
-        if not isinstance(dielectric, (float, int)):
-            dielectric = np.array(dielectric)
-            if dielectric.shape == (3,):
-                dielectric = np.diag(dielectric)
-            elif dielectric.shape != (3, 3):
-                raise ValueError(
-                    f"Dielectric constant must be a float/int or a 3x1 matrix or 3x3 matrix, "
-                    f"got type {type(dielectric)} and shape {dielectric.shape}"
-                )
-
-        parameters = {
-            "bulk_path": path_to_bulk,
-            "defect_path": path_to_defect,
-            "dielectric": dielectric,
-            "mpid": mpid,
-        }
-
-        # add bulk simple properties
-        bulk_vr, bulk_vr_path = get_vasprun(os.path.join(path_to_bulk, "vasprun.xml"))
-        bulk_energy = bulk_vr.final_energy
-        bulk_sc_structure = bulk_vr.initial_structure.copy()
-
-        # add defect simple properties
-        defect_vr, defect_vr_path = get_vasprun(
-            os.path.join(path_to_defect, "vasprun.xml")
-        )
-        defect_energy = defect_vr.final_energy
-        # Can specify initial defect structure (to help PyCDT find the defect site if
-        # multiple relaxations were required, else use from defect relaxation OUTCAR:
-        if initial_defect_structure:
-            initial_defect_structure = Poscar.from_file(
-                initial_defect_structure
-            ).structure.copy()
-        else:
-            initial_defect_structure = defect_vr.initial_structure.copy()
-
-        # Add initial defect structure to parameters, so it can be pulled later on
-        # (eg. for Kumagai loader)
-        parameters["initial_defect_structure"] = initial_defect_structure
-
-        # identify defect site, structural information, and create defect object
-        try:
-            def_type, comp_diff = get_defect_type_and_composition_diff(
-                bulk_sc_structure, initial_defect_structure
-            )
-        except RuntimeError as exc:
-            raise ValueError(
-                "Could not identify defect type from number of sites in structure: "
-                f"{len(bulk_sc_structure)} in bulk vs. {len(initial_defect_structure)} in defect?"
-            ) from exc
-
-        bulk_site_idx = None
-        defect_site_idx = None
-        unrelaxed_defect_structure = None
-        # Try automatic defect site detection - this gives us the "unrelaxed" defect structure
-        try:
-            (
-                bulk_site_idx,
-                defect_site_idx,
-                unrelaxed_defect_structure,
-            ) = get_defect_site_idxs_and_unrelaxed_structure(
-                bulk_sc_structure, initial_defect_structure, def_type, comp_diff
-            )
-        except RuntimeError as exc:
-            # if auto site-matching failed, try use transformation.json
-            # The goal is to find the `defect_site_idx` or `defect_site_idx` based on the
-            # tranformation.
-            transformation_path = os.path.join(path_to_defect, "transformation.json")
-            if not os.path.exists(transformation_path):  # try next folder up
-                orig_transformation_path = transformation_path
-                transformation_path = os.path.join(
-                    os.path.dirname(os.path.normpath(path_to_defect)),
-                    "transformation.json",
-                )
-                if os.path.exists(transformation_path):
-                    print(
-                        f"No transformation file found at {orig_transformation_path}, but found "
-                        f"one at {transformation_path}. Using this for defect parsing."
-                    )
-
-            if os.path.exists(transformation_path):
-                tf = loadfn(transformation_path)
-                site = tf["defect_supercell_site"]
-                if def_type == "vacancy":
-                    poss_deflist = sorted(
-                        bulk_sc_structure.get_sites_in_sphere(
-                            site.coords, 0.2, include_index=True
-                        ),
-                        key=lambda x: x[1],
-                    )
-                    searched = "bulk_supercell"
-                    if poss_deflist:
-                        bulk_site_idx = poss_deflist[0][2]
-                else:
-                    poss_deflist = sorted(
-                        initial_defect_structure.get_sites_in_sphere(
-                            site.coords, 2.5, include_index=True
-                        ),
-                        key=lambda x: x[1],
-                    )
-                    searched = "initial_defect_structure"
-                    if poss_deflist:
-                        defect_site_idx = poss_deflist[0][2]
-                if not poss_deflist:
-                    raise ValueError(
-                        f"{transformation_path} specified defect site {site}, but could not find "
-                        f"it in {searched}. Abandoning parsing."
-                    ) from exc
-                if poss_deflist[0][1] > 1:
-                    site_matched_defect = poss_deflist[0]  # pymatgen Neighbor object
-                    offsite_warning = (
-                        f"Site-matching has determined {site_matched_defect.species} at "
-                        f"{site_matched_defect.coords} as the defect site, located "
-                        f"{site_matched_defect.nn_distance:.2f} {_ANGSTROM} from its initial "
-                        f"position. This may incur small errors in the charge correction."
-                    )
-                    warnings.warn(message=offsite_warning)
-
-            else:
-                raise RuntimeError(
-                    f"Could not identify {def_type} defect site in defect structure. "
-                    f"Try supplying the initial defect structure to "
-                    f"SingleDefectParser.from_paths(), or making sure the doped "
-                    f"transformation.json files are in the defect directory."
-                ) from exc
-
-        if def_type == "vacancy":
-            defect_site = bulk_sc_structure[bulk_site_idx]
-        else:
-            if unrelaxed_defect_structure:
-                defect_site = unrelaxed_defect_structure[defect_site_idx]
-            else:
-                defect_site = initial_defect_structure[defect_site_idx]
-
-        if unrelaxed_defect_structure:
-            if def_type == "interstitial":
-                # get closest Voronoi site in bulk supercell to final interstitial site as this is
-                # likely to be the initial interstitial site
-                try:
-                    struc_and_node_dict = loadfn("./bulk_voronoi_nodes.json")
-                    if not StructureMatcher(
-                        stol=0.05,
-                        primitive_cell=False,
-                        scale=False,
-                        attempt_supercell=False,
-                        allow_subset=False,
-                    ).fit(struc_and_node_dict["bulk_supercell"], bulk_sc_structure):
-                        warnings.warn(
-                            "Previous bulk_voronoi_nodes.json detected, but does not "
-                            "match current bulk supercell. Recalculating Voronoi nodes."
-                        )
-                        raise FileNotFoundError
-
-                    voronoi_frac_coords = struc_and_node_dict["Voronoi nodes"]
-
-                except FileNotFoundError:  # first time parsing
-                    topography = TopographyAnalyzer(
-                        bulk_sc_structure,
-                        bulk_sc_structure.symbol_set,
-                        [],
-                        check_volume=False,
-                    )
-                    topography.cluster_nodes()
-                    topography.remove_collisions()
-                    voronoi_frac_coords = [
-                        site.frac_coords for site in topography.vnodes
-                    ]
-                    struc_and_node_dict = {
-                        "bulk_supercell": bulk_sc_structure,
-                        "Voronoi nodes": voronoi_frac_coords,
-                    }
-                    dumpfn(
-                        struc_and_node_dict, "./bulk_voronoi_nodes.json"
-                    )  # for efficient
-                    # parsing of multiple defects at once
-                    print(
-                        "Saving parsed Voronoi sites (for interstitial site-matching) to "
-                        "bulk_voronoi_sites.json to speed up future parsing."
-                    )
+        from doped.analysis import defect_entry_from_paths
 
-                closest_node_frac_coords = min(
-                    voronoi_frac_coords,
-                    key=lambda node: defect_site.distance_and_image_from_frac_coords(
-                        node
-                    )[0],
-                )
-                int_site = unrelaxed_defect_structure[defect_site_idx]
-                unrelaxed_defect_structure.remove_sites([defect_site_idx])
-                unrelaxed_defect_structure.insert(
-                    defect_site_idx,  # Place defect at same position as in DFT calculation
-                    int_site.species_string,
-                    closest_node_frac_coords,
-                    coords_are_cartesian=False,
-                    validate_proximity=True,
-                )
-                defect_site = unrelaxed_defect_structure[defect_site_idx]
-
-            # Use the unrelaxed_defect_structure to fix the initial defect structure
-            initial_defect_structure = reorder_unrelaxed_structure(
-                unrelaxed_defect_structure, initial_defect_structure
-            )
-            parameters["initial_defect_structure"] = initial_defect_structure
-            parameters["unrelaxed_defect_structure"] = unrelaxed_defect_structure
-        else:
-            warnings.warn(
-                "Cannot determine the unrelaxed `initial_defect_structure`. Please ensure the "
-                "`initial_defect_structure` is indeed unrelaxed."
-            )
-
-        for_monty_defect = {
-            "@module": "pymatgen.analysis.defects.core",
-            "@class": def_type.capitalize(),
-            "charge": defect_charge,
-            "structure": bulk_sc_structure,
-            "defect_site": defect_site,
-        }
-        defect = MontyDecoder().process_decoded(for_monty_defect)
-
-        if unrelaxed_defect_structure:
-            # only do StructureMatcher test if unrelaxed structure exists
-            test_defect_structure = defect.generate_defect_structure()
-            if not StructureMatcher(
-                stol=0.25,
-                primitive_cell=False,
-                scale=False,
-                attempt_supercell=False,
-                allow_subset=False,
-            ).fit(test_defect_structure, unrelaxed_defect_structure):
-                # NOTE: this does not insure that cartesian coordinates or indexing are identical
-                raise ValueError(
-                    "Error in defect object matching! Unrelaxed structure (1st below) "
-                    "does not match pymatgen defect.generate_defect_structure() "
-                    f"(2nd below):\n{unrelaxed_defect_structure}"
-                    f"\n{test_defect_structure}"
-                )
-
-        defect_entry = DefectEntry(
-            defect, defect_energy - bulk_energy, corrections={}, parameters=parameters
-        )
-
-        return SingleDefectParser(
-            defect_entry,
-            compatibility=compatibility,
-            defect_vr=defect_vr,
-            bulk_vr=bulk_vr,
+        kwargs.update({"return SingleDefectParser": True})
+        return defect_entry_from_paths(
+            defect_path,
+            bulk_path,
+            dielectric,
+            charge=charge,
+            initial_defect_structure=initial_defect_structure,
+            skip_corrections=skip_corrections,
+            bulk_bandgap_path=bulk_bandgap_path,
+            **kwargs,
         )
 
     def freysoldt_loader(self, bulk_locpot=None):
         """
         Load metadata required for performing Freysoldt correction
         requires "bulk_path" and "defect_path" to be loaded to DefectEntry parameters dict.
         Can read gunzipped "LOCPOT.gz" files as well.
@@ -745,28 +488,42 @@
             bulk_locpot object for reuse by another defect entry (for expedited parsing)
         """
         if not self.defect_entry.charge:
             # dont need to load locpots if charge is zero
             return None
 
         if not bulk_locpot:
-            bulk_locpot_path = os.path.join(
-                self.defect_entry.parameters["bulk_path"], "LOCPOT"
+            bulk_locpot_path, multiple = _get_output_files_and_check_if_multiple(
+                "LOCPOT", self.defect_entry.parameters["bulk_path"]
             )
+            if multiple:
+                warnings.warn(
+                    f"Multiple `LOCPOT` files found in bulk directory: "
+                    f"{self.defect_entry.parameters['bulk_path']}. Using {bulk_locpot_path} to "
+                    f"parse the electrostatic potential and compute the Freysoldt (FNV) charge "
+                    f"correction."
+                )
             bulk_locpot = get_locpot(bulk_locpot_path)
 
-        def_locpot_path = os.path.join(
-            self.defect_entry.parameters["defect_path"], "LOCPOT"
+        defect_locpot_path, multiple = _get_output_files_and_check_if_multiple(
+            "LOCPOT", self.defect_entry.parameters["defect_path"]
         )
-        def_locpot = get_locpot(def_locpot_path)
+        if multiple:
+            warnings.warn(
+                f"Multiple `LOCPOT` files found in defect directory: "
+                f"{self.defect_entry.parameters['defect_path']}. Using {defect_locpot_path} to "
+                f"parse the electrostatic potential and compute the Freysoldt (FNV) charge "
+                f"correction."
+            )
+        defect_locpot = get_locpot(defect_locpot_path)
 
-        axis_grid = [def_locpot.get_axis_grid(i) for i in range(3)]
+        axis_grid = [defect_locpot.get_axis_grid(i) for i in range(3)]
         bulk_planar_averages = [bulk_locpot.get_average_along_axis(i) for i in range(3)]
         defect_planar_averages = [
-            def_locpot.get_average_along_axis(i) for i in range(3)
+            defect_locpot.get_average_along_axis(i) for i in range(3)
         ]
 
         self.defect_entry.parameters.update(
             {
                 "axis_grid": axis_grid,
                 "bulk_planar_averages": bulk_planar_averages,
                 "defect_planar_averages": defect_planar_averages,
@@ -778,17 +535,14 @@
                 {
                     "initial_defect_structure": self.defect_entry.parameters[
                         "unrelaxed_defect_structure"
                     ],
                 }
             )
 
-        return bulk_locpot
-
-    # noinspection DuplicatedCode
     def kumagai_loader(self, bulk_outcar=None):
         """
         Load metadata required for performing Kumagai correction
         requires "bulk_path" and "defect_path" to be loaded to DefectEntry parameters dict.
 
         Args:
             bulk_outcar (Outcar): Add bulk Outcar object for expedited parsing.
@@ -797,44 +551,54 @@
             bulk_outcar object for reuse by another defect entry (for expedited parsing)
         """
         if not self.defect_entry.charge:
             # dont need to load outcars if charge is zero
             return None
 
         if not bulk_outcar:
-            bulk_outcar_path = os.path.join(
-                self.defect_entry.parameters["bulk_path"], "OUTCAR"
+            bulk_outcar_path, multiple = _get_output_files_and_check_if_multiple(
+                "OUTCAR", self.defect_entry.parameters["bulk_path"]
             )
+            if multiple:
+                warnings.warn(
+                    f"Multiple `OUTCAR` files found in bulk directory: "
+                    f"{self.defect_entry.parameters['bulk_path']}. Using {bulk_outcar_path} to "
+                    f"parse core levels and compute the Kumagai (eFNV) image charge correction."
+                )
             bulk_outcar = get_outcar(bulk_outcar_path)
         else:
-            bulk_outcar_path = "`bulk_outcar`"
+            bulk_outcar_path = bulk_outcar.filename
 
-        def_outcar_path = os.path.join(
-            self.defect_entry.parameters["defect_path"], "OUTCAR"
+        defect_outcar_path, multiple = _get_output_files_and_check_if_multiple(
+            "OUTCAR", self.defect_entry.parameters["defect_path"]
         )
-        def_outcar = get_outcar(def_outcar_path)
+        if multiple:
+            warnings.warn(
+                f"Multiple `OUTCAR` files found in defect directory: "
+                f"{self.defect_entry.parameters['defect_path']}. Using {defect_outcar_path} to "
+                f"parse core levels and compute the Kumagai (eFNV) image charge correction."
+            )
+        defect_outcar = get_outcar(defect_outcar_path)
 
         bulk_atomic_site_averages = bulk_outcar.electrostatic_potential
-        defect_atomic_site_averages = def_outcar.electrostatic_potential
+        defect_atomic_site_averages = defect_outcar.electrostatic_potential
         if not bulk_atomic_site_averages:
             raise ValueError(
                 f"Unable to parse atomic core potentials from bulk `OUTCAR` at "
-                f"{bulk_outcar_path}. This can happen if `ICORELEVEL` was not set "
-                f"to 0 (= default) in the `INCAR`, or if the calculation was "
-                f"finished prematurely with a `STOPCAR`. The Kumagai charge "
-                f"correction cannot be computed without this data!"
+                f"{bulk_outcar_path}. This can happen if `ICORELEVEL` was not set to 0 (= "
+                f"default) in the `INCAR`, or if the calculation was finished prematurely with a "
+                f"`STOPCAR`. The Kumagai charge correction cannot be computed without this data!"
             )
 
         if not defect_atomic_site_averages:
             raise ValueError(
                 f"Unable to parse atomic core potentials from defect `OUTCAR` at "
-                f"{def_outcar_path}. This can happen if `ICORELEVEL` was not set "
-                f"to 0 (= default) in the `INCAR`, or if the calculation was "
-                f"finished prematurely with a `STOPCAR`. The Kumagai charge "
-                f"correction cannot be computed without this data!"
+                f"{defect_outcar_path}. This can happen if `ICORELEVEL` was not set to 0 (= "
+                f"default) in the `INCAR`, or if the calculation was finished prematurely with a "
+                f"`STOPCAR`. The Kumagai charge correction cannot be computed without this data!"
             )
 
         bulk_structure = self.defect_entry.bulk_structure
         bulksites = [site.frac_coords for site in bulk_structure]
 
         defect_structure = self.defect_entry.parameters["initial_defect_structure"]
         initsites = [site.frac_coords for site in defect_structure]
@@ -871,28 +635,38 @@
                 "bulk_atomic_site_averages": bulk_atomic_site_averages,
                 "defect_atomic_site_averages": defect_atomic_site_averages,
                 "site_matching_indices": site_matching_indices,
                 "defect_frac_sc_coords": self.defect_entry.site.frac_coords,
             }
         )
 
-        return bulk_outcar
-
     def get_stdrd_metadata(self):
         if not self.bulk_vr:
-            path_to_bulk = self.defect_entry.parameters["bulk_path"]
-            self.bulk_vr, bulk_vr_path = get_vasprun(
-                os.path.join(path_to_bulk, "vasprun.xml")
+            bulk_vr_path, multiple = _get_output_files_and_check_if_multiple(
+                "vasprun.xml", self.defect_entry.parameters["bulk_path"]
             )
+            if multiple:
+                warnings.warn(
+                    f"Multiple `vasprun.xml` files found in bulk directory: "
+                    f"{self.defect_entry.parameters['bulk_path']}. Using {bulk_vr_path} to "
+                    f"parse the calculation energy and metadata."
+                )
+            self.bulk_vr = get_vasprun(bulk_vr_path)
 
         if not self.defect_vr:
-            path_to_defect = self.defect_entry.parameters["defect_path"]
-            self.defect_vr, defect_vr_path = get_vasprun(
-                os.path.join(path_to_defect, "vasprun.xml")
+            defect_vr_path, multiple = _get_output_files_and_check_if_multiple(
+                "vasprun.xml", self.defect_entry.parameters["defect_path"]
             )
+            if multiple:
+                warnings.warn(
+                    f"Multiple `vasprun.xml` files found in defect directory: "
+                    f"{self.defect_entry.parameters['defect_path']}. Using {defect_vr_path} to "
+                    f"parse the calculation energy and metadata."
+                )
+            self.defect_vr = get_vasprun(defect_vr_path)
 
         # standard bulk metadata
         bulk_energy = self.bulk_vr.final_energy
         bulk_sc_structure = self.bulk_vr.initial_structure
         self.defect_entry.parameters.update(
             {"bulk_energy": bulk_energy, "bulk_sc_structure": bulk_sc_structure}
         )
@@ -952,36 +726,56 @@
             for spincls, eigdict in self.defect_vr.eigenvalues.items()
         }
         kpoint_weights = self.defect_vr.actual_kpoints_weights[:]
         self.defect_entry.parameters.update(
             {"eigenvalues": eigenvalues, "kpoint_weights": kpoint_weights}
         )
 
-    def get_bulk_gap_data(self, no_MP=True, actual_bulk_path=None):
-        """Get bulk gap data from Materials Project or from local OUTCAR file.
+    def get_bulk_gap_data(
+        self, bulk_bandgap_path=None, use_MP=False, mpid=None, api_key=None
+    ):
+        """Get bulk gap data from bulk OUTCAR file, or OUTCAR located at `actual_bulk_path`.
+
+        Alternatively, one can specify query the Materials Project (MP) database for the bulk gap
+        data, using `use_MP = True`, in which case the MP entry with the lowest number ID and
+        composition matching the bulk will be used, or  the MP ID (mpid) of the bulk material to
+        use can be specified. This is not recommended as it will correspond to a
+        severely-underestimated GGA DFT bandgap!
 
         Args:
-            no_MP (bool): If True, will not query MP for bulk gap data. (Default: True)
-            actual_bulk_path (str): Path to bulk OUTCAR file for determining the band gap. If
+            bulk_bandgap_path (str): Path to bulk OUTCAR file for determining the band gap. If
                 the VBM/CBM occur at reciprocal space points not included in the bulk supercell
                 calculation, you should use this tag to point to a bulk bandstructure calculation
                 instead. If None, will use self.defect_entry.parameters["bulk_path"].
+            use_MP (bool): If True, will query the Materials Project database for the bulk gap
+                data.
+            mpid (str): If provided, will query the Materials Project database for the bulk gap
+                data, using this Materials Project ID.
+            api_key (str): Materials API key to access database.
         """
         if not self.bulk_vr:
-            path_to_bulk = self.defect_entry.parameters["bulk_path"]
-            self.bulk_vr, bulk_vr_path = get_vasprun(
-                os.path.join(path_to_bulk, "vasprun.xml")
+            bulk_vr_path, multiple = _get_output_files_and_check_if_multiple(
+                "vasprun.xml", self.defect_entry.parameters["bulk_path"]
             )
+            if multiple:
+                warnings.warn(
+                    f"Multiple `vasprun.xml` files found in bulk directory: "
+                    f"{self.defect_entry.parameters['bulk_path']}. Using {bulk_vr_path} to "
+                    f"parse the calculation energy and metadata."
+                )
+            self.bulk_vr = get_vasprun(bulk_vr_path)
 
         bulk_sc_structure = self.bulk_vr.initial_structure
-        mpid = self.defect_entry.parameters["mpid"]
 
-        if not mpid and not no_MP:
+        vbm, cbm, bandgap = None, None, None
+        gap_parameters = {}
+
+        if use_MP and mpid is None:
             try:
-                with MPRester() as mp:
+                with MPRester(api_key=api_key) as mp:
                     tmp_mplist = mp.get_entries_in_chemsys(
                         list(bulk_sc_structure.symbol_set)
                     )
                 mplist = [
                     ment.entry_id
                     for ment in tmp_mplist
                     if ment.composition.reduced_composition
@@ -991,15 +785,15 @@
                 raise ValueError(
                     f"Error with querying MPRester for"
                     f" {bulk_sc_structure.composition.reduced_formula}:"
                 ) from exc
 
             mpid_fit_list = []
             for trial_mpid in mplist:
-                with MPRester() as mp:
+                with MPRester(api_key=api_key) as mp:
                     mpstruct = mp.get_structure_by_material_id(trial_mpid)
                 if StructureMatcher(
                     primitive_cell=True,
                     scale=False,
                     attempt_supercell=True,
                     allow_subset=False,
                 ).fit(bulk_sc_structure, mpstruct):
@@ -1009,67 +803,61 @@
                 mpid = mpid_fit_list[0]
                 print(f"Single mp-id found for bulk structure:{mpid}.")
             elif len(mpid_fit_list) > 1:
                 num_mpid_list = [int(mp.split("" - "")[1]) for mp in mpid_fit_list]
                 num_mpid_list.sort()
                 mpid = "mp-" + str(num_mpid_list[0])
                 print(
-                    f"Multiple mp-ids found for bulk structure:{mpid_fit_list}\nWill use lowest "
+                    f"Multiple mp-ids found for bulk structure:{mpid_fit_list}. Will use lowest "
                     f"number mpid for bulk band structure = {mpid}."
                 )
             else:
                 print(
                     "Could not find bulk structure in MP database after tying the following "
                     f"list:\n{mplist}"
                 )
                 mpid = None
 
-        vbm, cbm, bandgap = None, None, None
-        gap_parameters = {}
-        if mpid is not None and not no_MP:
+        if mpid is not None:
             print(f"Using user-provided mp-id for bulk structure: {mpid}.")
-            with MPRester() as mp:
+            with MPRester(api_key=api_key) as mp:
                 bs = mp.get_bandstructure_by_material_id(mpid)
             if bs:
                 cbm = bs.get_cbm()["energy"]
                 vbm = bs.get_vbm()["energy"]
                 bandgap = bs.get_band_gap()["energy"]
                 gap_parameters.update(
                     {"MP_gga_BScalc_data": bs.get_band_gap().copy()}
                 )  # contains gap kpt transition
 
-        if (
-            vbm is None
-            or bandgap is None
-            or cbm is None
-            or no_MP
-            or not actual_bulk_path
-        ):
+        if vbm is None or bandgap is None or cbm is None or not bulk_bandgap_path:
             if mpid and bandgap is None:
                 print(
                     f"WARNING: Mpid {mpid} was provided, but no bandstructure entry currently "
                     "exists for it. \nReverting to use of bulk supercell calculation for band "
                     "edge extrema."
                 )
-            if mpid and no_MP:
-                print(
-                    f"Mpid {mpid} was provided, but `no_MP` flag was set to True. \n"
-                    "Reverting to use of bulk supercell calculation for band edge extrema."
-                )
 
             gap_parameters.update(
                 {"MP_gga_BScalc_data": None}
             )  # to signal no MP BS is used
             bandgap, cbm, vbm, _ = self.bulk_vr.eigenvalue_band_properties
 
-        if actual_bulk_path:
-            print(f"Using actual bulk path: {actual_bulk_path}")
-            actual_bulk_vr, actual_bulk_vr_path = get_vasprun(
-                os.path.join(actual_bulk_path, "vasprun.xml")
+        if bulk_bandgap_path:
+            print(f"Using actual bulk path: {bulk_bandgap_path}")
+            actual_bulk_vr_path, multiple = _get_output_files_and_check_if_multiple(
+                "vasprun.xml", bulk_bandgap_path
             )
+            if multiple:
+                warnings.warn(
+                    f"Multiple `vasprun.xml` files found in specified directory: "
+                    f"{bulk_bandgap_path}. Using {actual_bulk_vr_path} to  parse the calculation "
+                    f"energy and metadata."
+                )
+            actual_bulk_vr = get_vasprun(actual_bulk_vr_path)
             bandgap, cbm, vbm, _ = actual_bulk_vr.eigenvalue_band_properties
 
         gap_parameters.update({"mpid": mpid, "cbm": cbm, "vbm": vbm, "gap": bandgap})
         self.defect_entry.parameters.update(gap_parameters)
 
     def run_compatibility(self):
         # Set potalign so pymatgen can calculate bandfilling for 'neutral' defects
@@ -1087,22 +875,24 @@
             if (
                 "plnr_avg" in delocalization_meta
                 and not delocalization_meta["plnr_avg"]["is_compatible"]
             ) or (
                 "atomic_site" in delocalization_meta
                 and not delocalization_meta["atomic_site"]["is_compatible"]
             ):
-                specific_delocalized_warning = f"""
-Delocalization analysis has indicated that {self.defect_entry.name}
-with charge {self.defect_entry.charge} may not be compatible with the chosen charge correction."""
+                specific_delocalized_warning = (
+                    f"Delocalization analysis has indicated that {self.defect_entry.name} with "
+                    f"charge {self.defect_entry.charge:+} may not be compatible with the chosen "
+                    f"charge correction."
+                )
                 general_delocalization_warning = """
 Note: Defects throwing a "delocalization analysis" warning may require a larger supercell for
 accurate total energies. Recommended to look at the correction plots (i.e. run 
 `get_correction_freysoldt(DefectEntry,...,plot=True)` from
-`doped.pycdt.corrections.finite_size_charge_correction`) to visually determine if the charge 
+`doped.corrections`) to visually determine if the charge 
 correction scheme is still appropriate (replace 'freysoldt' with 'kumagai' if using anisotropic 
 correction). You can also change the DefectCompatibility() tolerance settings via the 
 `compatibility` parameter in `SingleDefectParser.from_paths()`."""
                 warnings.warn(message=specific_delocalized_warning)
                 if not self._delocalization_warning_printed:
                     warnings.warn(
                         message=general_delocalization_warning
@@ -1120,17 +910,17 @@
                 < self.defect_entry.parameters["num_elec_cbm"]
             ):
                 num_holes = self.defect_entry.parameters["num_hole_vbm"]
                 num_electrons = self.defect_entry.parameters["num_elec_cbm"]
                 warnings.warn(
                     f"Eigenvalue analysis has determined that `num_hole_vbm` (= {num_holes}) or "
                     f"`num_elec_cbm` (= {num_electrons}) is significant (>2.1) for "
-                    f"{self.defect_entry.name} with charge {self.defect_entry.charge}, indicating "
-                    f"that there are many free charges in this defect supercell calculation and "
-                    f"so the defect charge correction is unlikely to be accurate."
+                    f"{self.defect_entry.name} with charge {self.defect_entry.charge}:+, "
+                    f"indicating that there are many free charges in this defect supercell "
+                    f"calculation and so the defect charge correction is unlikely to be accurate."
                 )
                 if "freysoldt_meta" in self.defect_entry.parameters:
                     frey_meta = self.defect_entry.parameters["freysoldt_meta"]
                     frey_corr = (
                         frey_meta["freysoldt_electrostatic"]
                         + frey_meta["freysoldt_potential_alignment_correction"]
                     )
@@ -1149,15 +939,15 @@
 
         if (
             self.defect_entry.charge != 0
             and self.defect_entry.corrections.get("charge_correction", None) is None
         ):
             warnings.warn(
                 f"No charge correction computed for {self.defect_entry.name} with "
-                f"charge {self.defect_entry.charge}, indicating problems with the "
+                f"charge {self.defect_entry.charge:+}, indicating problems with the "
                 f"required data for the charge correction (i.e. dielectric constant, "
                 f"LOCPOT files for Freysoldt correction, OUTCAR (with ICORELEVEL = 0) "
                 f"for Kumagai correction etc)."
             )
 
 
 class PostProcess:
@@ -1181,81 +971,78 @@
 
     def parse_defect_calculations(self):
         """
         Parses the defect calculations as DefectEntry objects,
         from a PyCDT root_fldr file structure.
         Charge correction is missing in the first run.
         """
-        logger = logging.getLogger(__name__)
         parsed_defects = []
         subfolders = glob.glob(os.path.join(self._root_fldr, "vac_*"))
         subfolders += glob.glob(os.path.join(self._root_fldr, "as_*"))
         subfolders += glob.glob(os.path.join(self._root_fldr, "sub_*"))
         subfolders += glob.glob(os.path.join(self._root_fldr, "inter_*"))
 
         def get_vr_and_check_locpot(fldr):
             vr_file = os.path.join(fldr, "vasprun.xml")
             if not (os.path.exists(vr_file) or os.path.exists(vr_file + ".gz")):
-                logger.warning("{} doesn't exit".format(vr_file))
+                warnings.warn("{} doesn't exit".format(vr_file))
                 error_msg = ": Failure, vasprun.xml doesn't exist."
                 return (None, error_msg)  # Further processing is not useful
 
             try:
-                vr, vr_path = get_vasprun(vr_file, parse_potcar_file=False)
+                vr = get_vasprun(vr_file, parse_potcar_file=False)
             except:
-                logger.warning("Couldn't parse {}".format(vr_file))
+                warnings.warn("Couldn't parse {}".format(vr_file))
                 error_msg = ": Failure, couldn't parse vasprun.xml file."
                 return (None, error_msg)
 
             if not vr.converged:
-                logger.warning("Vasp calculation at {} not converged".format(fldr))
+                warnings.warn("Vasp calculation at {} not converged".format(fldr))
                 error_msg = ": Failure, Vasp calculation not converged."
                 return (None, error_msg)  # Further processing is not useful
 
             # Check if locpot exists
             locpot_file = os.path.join(fldr, "LOCPOT")
             if not (os.path.exists(locpot_file) or os.path.exists(locpot_file + ".gz")):
-                logger.warning("{} doesn't exit".format(locpot_file))
+                warnings.warn("{} doesn't exit".format(locpot_file))
                 error_msg = ": Failure, LOCPOT doesn't exist"
                 return (None, error_msg)  # Further processing is not useful
 
             return (vr, None)
 
         def get_encut_from_potcar(fldr):
             potcar_file = os.path.join(fldr, "POTCAR")
             if not os.path.exists(potcar_file):
-                logger.warning("Not POTCAR in {} to parse ENCUT".format(fldr))
+                warnings.warn("Not POTCAR in {} to parse ENCUT".format(fldr))
                 error_msg = ": Failure, No POTCAR file."
                 return (None, error_msg)  # Further processing is not useful
 
             try:
                 potcar = Potcar.from_file(potcar_file)
             except:
-                logger.warning("Couldn't parse {}".format(potcar_file))
+                warnings.warn("Couldn't parse {}".format(potcar_file))
                 error_msg = ": Failure, couldn't read POTCAR file."
                 return (None, error_msg)
 
             encut = max(ptcr_sngl.enmax for ptcr_sngl in potcar)
             return (encut, None)
 
         # get bulk entry information first
         fldr = os.path.join(self._root_fldr, "bulk")
         vr, error_msg = get_vr_and_check_locpot(fldr)
         if error_msg:
-            logger.error("Abandoning parsing of the calculations")
-            return {}
+            raise ValueError(f"Abandoning parsing of the calculations: {error_msg}")
         bulk_energy = vr.final_energy
         bulk_sc_struct = vr.final_structure
         try:
             encut = vr.incar["ENCUT"]
         except:  # ENCUT not specified in INCAR. Read from POTCAR
             encut, error_msg = get_encut_from_potcar(fldr)
             if error_msg:
-                logger.error("Abandoning parsing of the calculations")
-                return {}
+                raise ValueError(f"Abandoning parsing of the calculations: {error_msg}")
 
         trans_dict = loadfn(os.path.join(fldr, "transformation.json"), cls=MontyDecoder)
         supercell_size = trans_dict["supercell"]
 
         bulk_file_path = fldr
         bulk_entry = ComputedStructureEntry(
             bulk_sc_struct,
@@ -1274,15 +1061,15 @@
             for chrg_fldr in chrg_fldrs:
                 trans_dict = loadfn(
                     os.path.join(chrg_fldr, "transformation.json"), cls=MontyDecoder
                 )
                 chrg = trans_dict["charge"]
                 vr, error_msg = get_vr_and_check_locpot(chrg_fldr)
                 if error_msg:
-                    logger.warning("Parsing the rest of the calculations")
+                    warnings.warn("Parsing the rest of the calculations")
                     continue
                 if (
                     "substitution_specie" in trans_dict
                     and trans_dict["substitution_specie"]
                     not in bulk_sc_struct.symbol_set
                 ):
                     self._substitution_species.add(trans_dict["substitution_specie"])
@@ -1303,18 +1090,18 @@
                 defect_type = trans_dict.get("defect_type", None)
                 energy = vr.final_energy
                 try:
                     encut = vr.incar["ENCUT"]
                 except:  # ENCUT not specified in INCAR. Read from POTCAR
                     encut, error_msg = get_encut_from_potcar(chrg_fldr)
                     if error_msg:
-                        logger.warning(
+                        warnings.warn(
                             "Not able to determine ENCUT " "in {}".format(fldr_name)
                         )
-                        logger.warning("Parsing the rest of the " "calculations")
+                        warnings.warn("Parsing the rest of the " "calculations")
                         continue
 
                 comp_data = {
                     "bulk_path": bulk_file_path,
                     "defect_path": chrg_fldr,
                     "encut": encut,
                     "fldr_name": fldr_name,
@@ -1367,40 +1154,39 @@
         Returns the valence band maximum (float) of the structure with
         MP-ID mpid.
 
         Args:
             mpid (str): MP-ID for which the valence band maximum is to
                 be fetched from the Materials Project database
         """
-        logger = logging.getLogger(__name__)
         vbm, bandgap = None, None
 
         if self._mpid is not None:
             with MPRester(api_key=self._mapi_key) as mp:
                 bs = mp.get_bandstructure_by_material_id(self._mpid)
             if bs:
                 vbm = bs.get_vbm()["energy"]
                 bandgap = bs.get_band_gap()["energy"]
 
         if vbm is None or bandgap is None:
             if self._mpid:
-                logger.warning(
+                warnings.warn(
                     "Mpid {} was provided, but no bandstructure entry currently exists for it. "
                     "Reverting to use of bulk calculation.".format(self._mpid)
                 )
             else:
-                logger.warning(
+                warnings.warn(
                     "No mp-id provided, will fetch CBM/VBM details from the "
                     "bulk calculation."
                 )
-            logger.warning(
+            warnings.warn(
                 "This may not be appropriate if the VBM/CBM occur at reciprocal points "
                 "not included in the bulk calculation."
             )
-            vr, vr_path = get_vasprun(
+            vr = get_vasprun(
                 os.path.join(self._root_fldr, "bulk", "vasprun.xml"),
                 parse_potcar_file=False,
             )
             bandgap = vr.eigenvalue_band_properties[0]
             vbm = vr.eigenvalue_band_properties[2]
 
         return (vbm, bandgap)
@@ -1411,30 +1197,29 @@
         the materials project database. This is abstractly handled in the
         ChemPotAnalyzer
 
         Note to user: If personal phase diagram desired,
             option exists in the pycdt.core.chemical_potentials to setup,
             run and parse personal phase diagrams for purposes of chemical potentials
         """
-        logger = logging.getLogger(__name__)
 
         if self._mpid:
             cpa = _chemical_potentials.MPChemPotAnalyzer(
                 mpid=self._mpid,
                 sub_species=self._substitution_species,
                 mapi_key=self._mapi_key,
             )
         else:
-            bulkvr, bulkvr_path = get_vasprun(
+            bulkvr = get_vasprun(
                 os.path.join(self._root_fldr, "bulk", "vasprun.xml"),
                 parse_potcar_file=False,
             )
             if not bulkvr:
                 msg = "Could not fetch computed entry for atomic chempots!"
-                logger.warning(msg)
+                warnings.warn(msg)
                 raise ValueError(msg)
             cpa = _chemical_potentials.MPChemPotAnalyzer(
                 bulk_ce=bulkvr.get_computed_entry(),
                 sub_species=self._substitution_species,
                 mapi_key=self._mapi_key,
             )
 
@@ -1453,20 +1238,20 @@
                 root directory where subdirectory "dielectric" is expected
         Returns:
             eps (float):
                 average of the trace of the dielectric tensor
         """
 
         try:
-            vr, vr_path = get_vasprun(
+            vr = get_vasprun(
                 os.path.join(self._root_fldr, "dielectric", "vasprun.xml"),
                 parse_potcar_file=False,
             )
         except:
-            logging.getLogger(__name__).warning("Parsing Dielectric calculation failed")
+            warnings.warn("Parsing Dielectric calculation failed")
             return None
 
         eps_ion = vr.epsilon_ionic
         eps_stat = vr.epsilon_static
 
         eps = []
         for i in range(len(eps_ion)):
@@ -1486,66 +1271,7 @@
         output["epsilon"] = self.parse_dielectric_calculation()
         output["mu_range"] = self.get_chempot_limits()
         vbm, gap = self.get_vbm_bandgap()
         output["vbm"] = vbm
         output["gap"] = gap
 
         return output
-
-
-def get_site_mapping_indices(
-    structure_a: Structure, structure_b: Structure, threshold=2.0
-):
-    """
-    Reset the position of a partially relaxed structure to its unrelaxed positions.
-    The template structure may have a different species ordering to the `input_structure`.
-    """
-
-    ## Generate a site matching table between the input and the template
-    input_fcoords = [site.frac_coords for site in structure_a]
-    template_fcoords = [site.frac_coords for site in structure_b]
-
-    dmat = structure_a.lattice.get_all_distances(input_fcoords, template_fcoords)
-    min_dist_with_index = []
-    for index in range(len(input_fcoords)):
-        dists = dmat[index]
-        template_index = dists.argmin()
-        current_dist = dists.min()
-        min_dist_with_index.append(
-            [
-                current_dist,
-                index,
-                template_index,
-            ]
-        )
-
-        if current_dist > threshold:
-            sitea = structure_a[index]
-            siteb = structure_b[template_index]
-            warnings.warn(
-                f"Large site displacement {current_dist:.4f} detected when matching atomic sites:"
-                f" {sitea}-> {siteb}."
-            )
-    return min_dist_with_index
-
-
-def reorder_unrelaxed_structure(
-    unrelaxed_structure: Structure, initial_relax_structure: Structure, threshold=2.0
-):
-    """
-    Reset the position of a partially relaxed structure to its unrelaxed positions.
-    The template structure may have a different species ordering to the `input_structure`.
-    """
-
-    # Obtain site mapping between the initial_relax_structure and the unrelaxed structure
-    mapping = get_site_mapping_indices(
-        initial_relax_structure, unrelaxed_structure, threshold=threshold
-    )
-
-    # Reorder the unrelaxed_structure so it matches the ordering of the initial_relax_structure (
-    # from the actual calculation)
-    reordered_sites = [unrelaxed_structure[tmp[2]] for tmp in mapping]
-    new_structure = Structure.from_sites(reordered_sites)
-
-    assert len(new_structure) == len(unrelaxed_structure)
-
-    return new_structure
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `doped-1.0.9/doped/vasp_input.py` & `doped-1.1.0/doped/vasp_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,42 +11,34 @@
 from typing import TYPE_CHECKING, Optional, Union
 
 from monty.io import zopen
 from monty.serialization import dumpfn, loadfn
 from pymatgen.io.vasp.inputs import (
     BadIncarWarning,
     incar_params,
-    UnknownPotcarWarning,
     Incar,
     Kpoints,
     Poscar,
 )
 from pymatgen.io.vasp.sets import DictSet
 
 from doped.pycdt.utils.vasp import DefectRelaxSet, _check_psp_dir
+from doped import _ignore_pmg_warnings
 
 if TYPE_CHECKING:
     import pymatgen.core.periodic_table
     import pymatgen.core.structure
 
 MODULE_DIR = os.path.dirname(os.path.abspath(__file__))
 default_potcar_dict = loadfn(os.path.join(MODULE_DIR, "PotcarSet.yaml"))
 default_relax_set = loadfn(os.path.join(MODULE_DIR, "HSE06_RelaxSet.yaml"))
 default_defect_set = loadfn(os.path.join(MODULE_DIR, "DefectSet.yaml"))
 default_relax_set["INCAR"].update(default_defect_set["INCAR"])
 
-# globally ignore these POTCAR warnings
-warnings.filterwarnings("ignore", category=UnknownPotcarWarning)
-warnings.filterwarnings("ignore", message="No POTCAR file with matching TITEL fields")
-warnings.filterwarnings("ignore", message="Ignoring unknown variable type")
-warnings.filterwarnings(
-    "ignore", message="POTCAR data with symbol"
-)  # Ignore POTCAR warnings because Pymatgen incorrectly detecting POTCAR types
-# Ignore because comment after 'ALGO = Normal' causes this unnecessary warning:
-warnings.filterwarnings("ignore", message="Hybrid functionals only support")
+_ignore_pmg_warnings()
 
 # until updated from pymatgen==2022.7.25 :
 warnings.filterwarnings(
     "ignore", message="Using `tqdm.autonotebook.tqdm` in notebook mode"
 )
 
 
@@ -84,15 +76,17 @@
                 "charge": charge,
                 "supercell": supercell["size"],
             }
             if "substitution_specie" in defect:
                 dict_transf["substitution_specie"] = defect["substitution_specie"]
 
             frac_coords = defect["unique_site"].frac_coords
-            approx_coords = f"~[{frac_coords[0]:.4f},{frac_coords[1]:.4f},{frac_coords[2]:.4f}]"
+            approx_coords = (
+                f"~[{frac_coords[0]:.4f},{frac_coords[1]:.4f},{frac_coords[2]:.4f}]"
+            )
             # Note this gets truncated to 40 characters in the CONTCAR: (this should be less than
             # 40 chars in all cases):
             poscar_comment = f"{defect['name']} {approx_coords} {charge}"
             defect_species = defect["name"] + f"_{charge}"
 
             defect_input_dict[defect_species] = {
                 "Defect Structure": defect["supercell"]["structure"],
@@ -123,15 +117,17 @@
         single_defect_dict["POSCAR Comment"]
         if "POSCAR Comment" in single_defect_dict
         else None
     )
     transf_dict = single_defect_dict["Transformation Dict"]
 
     if subfolder is None:
-        vaspinputdir = output_dir  # output_dir here = {orig output_dir}/{defect_species}
+        vaspinputdir = (
+            output_dir  # output_dir here = {orig output_dir}/{defect_species}
+        )
     else:
         vaspinputdir = f"{output_dir}/{subfolder}"
 
     if not os.path.exists(vaspinputdir) and write_files:
         os.makedirs(vaspinputdir)
 
     if unperturbed_poscar and write_files:
@@ -214,15 +210,17 @@
 
     defect_relax_set = DefectRelaxSet(
         supercell,
         config_dict=relax_set,
         user_kpoints_settings=user_kpoints_settings,  # accepts Kpoints obj, so we can set comment
         charge=transf_dict["charge"],
     )
-    defect_relax_set.output_dir = vaspinputdir  # assign attribute to later use in write_input()
+    defect_relax_set.output_dir = (
+        vaspinputdir  # assign attribute to later use in write_input()
+    )
 
     return defect_relax_set
 
 
 def vasp_gam_files(
     defect_dict: dict,
     output_dir: str = ".",
@@ -303,16 +301,20 @@
                 else None
             )
             if poscar_comment is not None:
                 poscar = Poscar(single_defect_dict["Defect Structure"])
                 poscar.comment = poscar_comment
                 poscar.write_file(defect_relax_set.output_dir + "/POSCAR")
 
-            dumpfn(single_defect_dict["Transformation Dict"],  # write transformation.json file
-                   f"{defect_relax_set.output_dir}/transformation.json")
+            dumpfn(
+                single_defect_dict[
+                    "Transformation Dict"
+                ],  # write transformation.json file
+                f"{defect_relax_set.output_dir}/transformation.json",
+            )
 
         defect_relax_set_dict[defect_species] = defect_relax_set
 
     return defect_relax_set_dict
 
 
 def vasp_std_files(
@@ -406,20 +408,28 @@
             unperturbed_poscar=unperturbed_poscar,
             write_files=write_files,
         )
 
         if write_files:
             # then use `write_file()`s rather than `write_input()` to avoid writing POSCARs
             defect_relax_set.incar.write_file(defect_relax_set.output_dir + "/INCAR")
-            defect_relax_set.kpoints.write_file(defect_relax_set.output_dir + "/KPOINTS")
+            defect_relax_set.kpoints.write_file(
+                defect_relax_set.output_dir + "/KPOINTS"
+            )
             if user_potcar_functional is not None:  # for GH Actions testing
-                defect_relax_set.potcar.write_file(defect_relax_set.output_dir + "/POTCAR")
+                defect_relax_set.potcar.write_file(
+                    defect_relax_set.output_dir + "/POTCAR"
+                )
 
-            dumpfn(single_defect_dict["Transformation Dict"],  # write transformation.json file
-                   f"{defect_relax_set.output_dir}/transformation.json")
+            dumpfn(
+                single_defect_dict[
+                    "Transformation Dict"
+                ],  # write transformation.json file
+                f"{defect_relax_set.output_dir}/transformation.json",
+            )
 
         defect_relax_set_dict[defect_species] = defect_relax_set
 
     return defect_relax_set_dict
 
 
 def vasp_ncl_files(
@@ -519,20 +529,28 @@
             unperturbed_poscar=unperturbed_poscar,
             write_files=write_files,
         )
 
         if write_files:  # write INCAR, KPOINTS and POTCAR files
             # then use `write_file()`s rather than `write_input()` to avoid writing POSCARs
             defect_relax_set.incar.write_file(defect_relax_set.output_dir + "/INCAR")
-            defect_relax_set.kpoints.write_file(defect_relax_set.output_dir + "/KPOINTS")
+            defect_relax_set.kpoints.write_file(
+                defect_relax_set.output_dir + "/KPOINTS"
+            )
             if user_potcar_functional is not None:  # for GH Actions testing
-                defect_relax_set.potcar.write_file(defect_relax_set.output_dir + "/POTCAR")
+                defect_relax_set.potcar.write_file(
+                    defect_relax_set.output_dir + "/POTCAR"
+                )
 
-            dumpfn(single_defect_dict["Transformation Dict"],  # write transformation.json file
-                   f"{defect_relax_set.output_dir}/transformation.json")
+            dumpfn(
+                single_defect_dict[
+                    "Transformation Dict"
+                ],  # write transformation.json file
+                f"{defect_relax_set.output_dir}/transformation.json",
+            )
 
         defect_relax_set_dict[defect_species] = defect_relax_set
 
     return defect_relax_set_dict
 
 
 # TODO: Remove these functions once confirming all functionality is in `chemical_potentials.py`;
```

### Comparing `doped-1.0.9/doped.egg-info/PKG-INFO` & `doped-1.1.0/doped.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <sean.kavanagh.19@ucl.ac.uk>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,15 +31,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # **D**efect **O**riented **P**ython **E**nvironment **D**istribution (`doped`)
 This is a (mid-development) Python package for managing solid-state defect calculations,
 geared toward VASP. Much of it is a modified version of the excellent [PyCDT](https://bitbucket.org/mbkumar/pycdt).  
@@ -62,26 +62,30 @@
 - Because of breaking changes made to the `pymatgen` defects code in version `2022.8.23`, `doped` requires 
 `pymatgen<2022.8.23`, which is installed automatically when installing `doped`. 
 However, as discussed briefly below and in the example notebooks, the 
 [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach is highly recommended when calculating 
 defects in solids, and this package has been updated to be compatible with the latest version of `pymatgen`.
 As such, it is recommended to install `doped` in a virtual python environment as follows:
 
-1. 
+1. Create virtual environment and install: 
 ```bash
-conda create -n doped  # create conda environment named doped
+conda create -n doped python=3.10  # create conda environment named doped
 conda activate doped  # activate doped conda environment
-pip install doped  # install doped package and dependencies
+pip install doped  # install doped and dependencies, can also  
+pip install numpy --upgrade # upgrade numpy to avoid binary incompatibility
 ```
 And then use this environment whenever using `doped`.
-Instead of `conda` you can also use `venv` to setup virtual environments, 
-see [here](https://www.freecodecamp.org/news/how-to-setup-virtual-environments-in-python/) for more.
+Alternatively if desired, `doped` can also be installed from `conda` with:
+
+```bash
+  conda install -c conda-forge doped
+```
 
 If you want to use the [example files](examples), 
-you should clone the repository and install with `pip install -e .` from the `doped` directory.
+you should clone the repository and install with `pip install -e .` from the `doped` directory, but still make sure to `pip install numpy --upgrade`.
 
 2. (If not set) Set the VASP pseudopotential directory and your Materials Project API key in `$HOME/.pmgrc.yaml` 
 (`pymatgen` config file) as follows:
 ```bash
   PMG_VASP_PSP_DIR: <Path to VASP pseudopotential top directory>
   PMG_MAPI_KEY: <Your MP API key obtained from https://legacy.materialsproject.org/open>
 ```
@@ -99,24 +103,26 @@
 pmg config -p temp_potcars psp_resources  # configure the psp_resources pymatgen POTCAR directory
 pmg config --add PMG_VASP_PSP_DIR "${PWD}/psp_resources"  # add the POTCAR directory to pymatgen's config file (`$HOME/.pmgrc.yaml`)
 rm -r temp_potcars  # remove the temporary POTCAR directory
 ```
 If this has been successful, you should be able to run `pmg potcar -s Na_pv`, and `grep PBE POTCAR` should show 
 `PAW_PBE Na_pv {date}` (you can ignore any `pymatgen` warnings about recognising the `POTCAR`). 
 
+If it does not work check that the `PMG_DEFAULT_FUNCTIONAL` is set to whatever your functionals are (e.g. `PBE` or `PBE_54`)
+
 This is necessary to generate `POTCAR` input files, and auto-determine `INCAR` settings such as `NELECT` for charged 
 defects.
 
 The Materials Project API key is required for determining the necessary competing phases to calculate in order to 
 determine the chemical potential limits (required for defect formation energies). This should correspond to the legacy 
 MP API, with your unique key available at: https://legacy.materialsproject.org/open.
 
 
 ## `ShakeNBreak`
-As shown in the example notebook, it is highly recommended to use the [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects in solids, to ensure you have identified the groundstate structures of your defects. As detailed in the [theory paper](https://arxiv.org/abs/2207.09862), skipping this step can result in drastically incorrect formation energies, transition levels, carrier capture (basically any property associated with defects). This approach is followed in the [doped example notebook](https://github.com/SMTG-UCL/doped/blob/master/dope_Example_Notebook.ipynb), with a more in-depth explanation and tutorial given on the [ShakeNBreak](https://shakenbreak.readthedocs.io/en/latest/) website.
+As shown in the example notebook, it is highly recommended to use the [`ShakeNBreak`](https://shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects in solids, to ensure you have identified the groundstate structures of your defects. As detailed in the [theory paper](https://arxiv.org/abs/2207.09862), skipping this step can result in drastically incorrect formation energies, transition levels, carrier capture (basically any property associated with defects). This approach is followed in the [doped example notebook](https://github.com/SMTG-UCL/doped/blob/master/dope_workflow_example.ipynb), with a more in-depth explanation and tutorial given on the [ShakeNBreak](https://shakenbreak.readthedocs.io/en/latest/) website.
 
 Summary GIF:
 ![ShakeNBreak Summary](files/SnB_Supercell_Schematic_PES_2sec_Compressed.gif)
 
 `SnB` CLI Usage:
 ![ShakeNBreak CLI](files/SnB_CLI.gif)
```

### Comparing `doped-1.0.9/pyproject.toml` & `doped-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "doped"
-version = "1.0.9"
+version = "1.1.0"
 description = "Python package to setup, process and analyse solid-state defect calculations with VASP"
 authors = [{name = "Seán Kavanagh", email = "sean.kavanagh.19@ucl.ac.uk"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -12,15 +12,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Software Development :: Libraries :: Python Modules",
     ]
-requires-python = ">=3.7"
+requires-python = ">=3.7, <3.11"  # current pymatgen version <2022.8.23 incompatible with python 3.11
 dependencies = [
     "ase",
     "tabulate",
     "matplotlib",
     "numpy>=1.21.0",
     "pymatgen<2022.8.23",
     "shakenbreak==22.11.1",
```

### Comparing `doped-1.0.9/tests/test_chemical_potentials.py` & `doped-1.1.0/tests/test_chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-1.0.9/tests/test_vasp_input.py` & `doped-1.1.0/tests/test_vasp_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,21 +135,20 @@
             self.assertIn(contents[1], ["Te_sv_GW", "Te_sv_GW\n"])
 
         # test no files written with write_files=False
         self.tearDown()
         vasp_input.vasp_gam_files(
             self.cdte_generated_defect_dict,
             user_potcar_functional=None,
-            write_files=False
+            write_files=False,
         )
         for folder in os.listdir(self.CDTE_DATA_DIR):
             if os.path.isdir(f"{self.CDTE_DATA_DIR}/{folder}"):
                 self.assertFalse(os.path.exists(f"./{folder}"))
 
-
     def test_vasp_gam_files_single_defect_dict(self):
         single_defect_dict = self.cdte_generated_defect_dict["vacancies"][0]  # V_Cd
         vasp_input.vasp_gam_files(
             single_defect_dict,
             user_incar_settings={"ENCUT": 350},
             potcar_spec=True,
             user_potcar_functional=None,
@@ -178,17 +177,15 @@
             contents = file.readlines()
             self.assertIn(contents[0], ["Cd_sv_GW", "Cd_sv_GW\n"])
             self.assertIn(contents[1], ["Te_sv_GW", "Te_sv_GW\n"])
 
         # test no files written with write_files=False
         self.tearDown()
         vasp_input.vasp_gam_files(
-            vac_Te_dict,
-            user_potcar_functional=None,
-            write_files=False
+            vac_Te_dict, user_potcar_functional=None, write_files=False
         )
         self.assertFalse(os.path.exists(f"vac_2_Te_0"))
 
     def test_vasp_std_files(self):
         vasp_input.vasp_std_files(
             self.cdte_generated_defect_dict,
             user_incar_settings={
@@ -217,15 +214,15 @@
         self.check_generated_vasp_inputs(vasp_type="vasp_std", check_poscar=True)
 
         # test no files written with write_files=False
         self.tearDown()
         vasp_input.vasp_std_files(
             self.cdte_generated_defect_dict,
             user_potcar_functional=None,
-            write_files=False
+            write_files=False,
         )
         for folder in os.listdir(self.CDTE_DATA_DIR):
             if os.path.isdir(f"{self.CDTE_DATA_DIR}/{folder}"):
                 self.assertFalse(os.path.exists(f"./{folder}"))
 
     def test_vasp_std_files_single_defect_dict(self):
         # test interstitials this time:
@@ -274,17 +271,15 @@
                 check_poscar=True,
                 single_defect_dir=True,
             )
 
         # test no files written with write_files=False
         self.tearDown()
         vasp_input.vasp_gam_files(
-            single_defect_dict,
-            user_potcar_functional=None,
-            write_files=False
+            single_defect_dict, user_potcar_functional=None, write_files=False
         )
         self.assertFalse(os.path.exists(f"inter_1_Cd_0"))
         self.assertFalse(os.path.exists(f"inter_1_Cd_1"))
         self.assertFalse(os.path.exists(f"inter_1_Cd_2"))
 
     def test_vasp_ncl_files(self):
         vasp_input.vasp_ncl_files(
@@ -305,15 +300,15 @@
         self.check_generated_vasp_inputs(vasp_type="vasp_ncl", check_poscar=True)
 
         # test no files written with write_files=False
         self.tearDown()
         vasp_input.vasp_ncl_files(
             self.cdte_generated_defect_dict,
             user_potcar_functional=None,
-            write_files=False
+            write_files=False,
         )
         for folder in os.listdir(self.CDTE_DATA_DIR):
             if os.path.isdir(f"{self.CDTE_DATA_DIR}/{folder}"):
                 self.assertFalse(os.path.exists(f"./{folder}"))
 
     def test_vasp_ncl_files_single_defect_dict(self):
         # test substitutions this time:
@@ -352,17 +347,15 @@
                 check_poscar=True,
                 single_defect_dir=True,
             )
 
         # test no files written with write_files=False
         self.tearDown()
         vasp_input.vasp_ncl_files(
-            single_defect_dict,
-            user_potcar_functional=None,
-            write_files=False
+            single_defect_dict, user_potcar_functional=None, write_files=False
         )
         for charge in range(-1, 6):
             self.assertFalse(os.path.exists(f"sub_2_Se_on_Te_{charge}"))
 
 
 if __name__ == "__main__":
     unittest.main()
```

