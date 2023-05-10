# Comparing `tmp/crdb-0.7.0.tar.gz` & `tmp/crdb-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crdb-0.7.0.tar", last modified: Tue May  9 09:28:48 2023, max compression
+gzip compressed data, was "crdb-0.8.0.tar", last modified: Wed May 10 16:56:07 2023, max compression
```

## Comparing `crdb-0.7.0.tar` & `crdb-0.8.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.842773 crdb-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-09 09:28:36.000000 crdb-0.7.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.834773 crdb-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.838773 crdb-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-09 09:28:36.000000 crdb-0.7.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-09 09:28:36.000000 crdb-0.7.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-09 09:28:36.000000 crdb-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-09 09:28:36.000000 crdb-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 09:28:36.000000 crdb-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-09 09:28:36.000000 crdb-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 09:28:36.000000 crdb-0.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-09 09:28:36.000000 crdb-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-09 09:28:36.000000 crdb-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 09:28:36.000000 crdb-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-09 09:28:48.842773 crdb-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-09 09:28:36.000000 crdb-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.838773 crdb-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/build.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 09:28:36.000000 crdb-0.7.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-09 09:28:36.000000 crdb-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-09 09:28:48.842773 crdb-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.834773 crdb-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.838773 crdb-0.7.0/src/crdb/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21678 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/crdb_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/mpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-09 09:28:36.000000 crdb-0.7.0/src/crdb/solarsystem_abundances2003.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.842773 crdb-0.7.0/src/crdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 09:28:48.000000 crdb-0.7.0/src/crdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:28:48.842773 crdb-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-09 09:28:36.000000 crdb-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-09 09:28:36.000000 crdb-0.7.0/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-09 09:28:36.000000 crdb-0.7.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-09 09:28:36.000000 crdb-0.7.0/tests/test_mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.855631 crdb-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-10 16:55:55.000000 crdb-0.8.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.847631 crdb-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.851631 crdb-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-10 16:55:55.000000 crdb-0.8.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-10 16:55:55.000000 crdb-0.8.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 16:55:55.000000 crdb-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-10 16:55:55.000000 crdb-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 16:55:55.000000 crdb-0.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 16:55:55.000000 crdb-0.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 16:55:55.000000 crdb-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-10 16:55:55.000000 crdb-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 16:55:55.000000 crdb-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 16:55:55.000000 crdb-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-10 16:56:07.855631 crdb-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-10 16:55:55.000000 crdb-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.851631 crdb-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 16:55:55.000000 crdb-0.8.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 16:55:55.000000 crdb-0.8.0/get_valid_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-10 16:55:55.000000 crdb-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 16:56:07.855631 crdb-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.847631 crdb-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.855631 crdb-0.8.0/src/crdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22743 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/crdb_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-10 16:55:55.000000 crdb-0.8.0/src/crdb/solarsystem_abundances2003.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.855631 crdb-0.8.0/src/crdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 16:56:07.000000 crdb-0.8.0/src/crdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:56:07.855631 crdb-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-10 16:55:55.000000 crdb-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-10 16:55:55.000000 crdb-0.8.0/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-10 16:55:55.000000 crdb-0.8.0/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-10 16:55:55.000000 crdb-0.8.0/tests/test_mpl.py
```

### Comparing `crdb-0.7.0/.github/workflows/publish.yml` & `crdb-0.8.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/.github/workflows/test.yml` & `crdb-0.8.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/.gitignore` & `crdb-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/.pre-commit-config.yaml` & `crdb-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/CONTRIBUTING.rst` & `crdb-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/LICENSE` & `crdb-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/PKG-INFO` & `crdb-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.7.0
+Version: 0.8.0
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `crdb-0.7.0/README.rst` & `crdb-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/docs/conf.py` & `crdb-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/pyproject.toml` & `crdb-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/src/crdb/__init__.py` & `crdb-0.8.0/src/crdb/__init__.py`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/src/crdb/cli.py` & `crdb-0.8.0/src/crdb/cli.py`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/src/crdb/core.py` & `crdb-0.8.0/src/crdb/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,292 +14,366 @@
 from typing import Tuple
 from typing import Union
 
 import cachier
 import numpy as np
 from numpy.typing import NDArray
 
-# from "Submit data" tab on CRDB website
+# generated from np.unqiue(crdb.all().quantity)
 VALID_NAMES = (
-    "H",
-    "He",
-    "Li",
-    "Be",
-    "B",
-    "C",
-    "N",
-    "O",
-    "F",
-    "Ne",
-    "Na",
-    "Mg",
-    "Al",
-    "Si",
-    "P",
-    "S",
-    "Cl",
-    "Ar",
-    "K",
-    "Ca",
-    "Sc",
-    "Ti",
-    "V",
-    "Cr",
-    "Mn",
-    "Fe",
-    "Co",
-    "Ni",
-    "Cu",
-    "Zn",
-    "Ga",
-    "Ge",
-    "As",
-    "Se",
-    "Br",
-    "Kr",
-    "Rb",
-    "Sr",
-    "Y",
-    "Zr",
-    "Nb",
-    "Mo",
-    "Tc",
-    "Ru",
-    "Rh",
-    "Pd",
-    "Ag",
-    "Cd",
-    "In",
-    "Sn",
-    "Sb",
-    "Te",
-    "I",
-    "Xe",
-    "Cs",
-    "Ba",
-    "La",
-    "Ce",
-    "Pr",
-    "Nd",
-    "Pm",
-    "Sm",
-    "Eu",
-    "Gd",
-    "Tb",
-    "Dy",
-    "Ho",
-    "Er",
-    "Tm",
-    "Yb",
-    "Lu",
-    "Hf",
-    "Ta",
-    "W",
-    "Re",
-    "Os",
-    "Ir",
-    "Pt",
-    "Au",
-    "Hg",
-    "Tl",
-    "Pb",
-    "Bi",
-    "Po",
-    "At",
-    "Rn",
-    "Fr",
-    "Ra",
-    "Ac",
-    "Th",
-    "Pa",
-    "U",
-    "Np",
-    "Pu",
-    "Am",
-    "Cm",
-    "Bk",
-    "Cf",
-    "Es",
-    "Zgeq1",
-    "Zgeq2",
-    "Zgeq3",
-    "Zgeq4",
-    "Zgeq5",
-    "Zgeq6",
-    "Zgeq7",
-    "Zgeq8",
-    "H-bar",
-    "He-bar",
-    "Li-bar",
-    "Be-bar",
-    "B-bar",
-    "C-bar",
-    "N-bar",
-    "O-bar",
-    "Zgeq1-bar",
-    "Zgeq2-bar",
-    "Zgeq3-bar",
-    "Zgeq4-bar",
-    "Zgeq5-bar",
-    "Zgeq6-bar",
-    "Zgeq7-bar",
-    "Zgeq8-bar",
-    "1H-bar",
-    "2H-bar",
-    "3He-bar",
-    "4He-bar",
-    "6Li-bar",
-    "9Be-bar",
-    "11B-bar",
-    "12C-bar",
-    "14N-bar",
-    "16O-bar",
-    "e-",
-    "e+",
-    "NU_E",
-    "NU_M",
-    "NU_T",
-    "GAMMA",
-    "e-+e+",
-    "SubFe",
-    "1H",
-    "2H",
-    "3He",
-    "4He",
-    "6Li",
-    "7Li",
-    "7Be",
-    "9Be",
-    "10B",
-    "10Be",
-    "11B",
-    "12C",
-    "13C",
-    "14N",
-    "14C",
-    "15N",
-    "16O",
-    "17O",
-    "18O",
-    "19F",
-    "20Ne",
-    "21Ne",
-    "22Ne",
-    "23Na",
-    "24Mg",
-    "25Mg",
-    "26Mg",
-    "26Al",
-    "27Al",
-    "28Si",
-    "29Si",
-    "30Si",
-    "31P",
-    "32S",
-    "33S",
-    "34S",
-    "35Cl",
-    "36S",
-    "36Ar",
-    "36Cl",
-    "37Cl",
-    "37Ar",
-    "38Ar",
-    "39K",
-    "40Ar",
-    "40Ca",
-    "40K",
-    "41K",
-    "41Ca",
-    "42Ca",
-    "43Ca",
-    "44Ca",
-    "44Ti",
-    "45Sc",
-    "46Ti",
-    "46Ca",
-    "47Ti",
-    "48Ti",
-    "48Ca",
-    "48Cr",
-    "49Ti",
-    "49V",
-    "50Ti",
-    "50Cr",
-    "50V",
-    "51V",
-    "51Cr",
-    "52Cr",
-    "53Cr",
-    "53Mn",
-    "54Cr",
-    "54Fe",
-    "54Mn",
-    "55Mn",
-    "55Fe",
-    "56Fe",
-    "56Ni",
-    "57Fe",
-    "57Co",
-    "58Fe",
-    "58Ni",
-    "59Co",
-    "59Ni",
-    "60Ni",
-    "60Fe",
-    "61Ni",
-    "62Ni",
-    "63Cu",
-    "64Ni",
-    "64Zn",
-    "65Cu",
-    "66Zn",
-    "67Zn",
-    "68Zn",
-    "70Zn",
-    "H-He-group",
-    "N-group",
-    "O-group",
-    "Al-group",
-    "Si-group",
-    "Fe-group",
-    "O-Fe-group",
-    "C-Fe-group",
-    "AllParticles",
-    "<LnA>",
-    "<X_max>",
-    "X_mu_max",
-    "<rho_mu_600>",
-    "<rho_mu_800>",
-    "<R_mu>",
-    "LS-group",
-    "HS-group",
-    "Pt-group",
-    "Pb-group",
-    "Subactinides",
-    "Actinides",
-    "Z_33-34",
-    "Z_35-36",
-    "Z_37-38",
-    "Z_39-40",
-    "Z_41-42",
-    "Z_43-44",
-    "Z_45-46",
-    "Z_47-48",
-    "Z_49-50",
-    "Z_51-52",
-    "Z_53-54",
-    "Z_55-56",
-    "Z_57-58",
-    "Z_59-60",
-    "Zgeq70",
-    "9Be+10Be",
+    '10B',
+    '10Be',
+    '11B',
+    '12C',
+    '13C',
+    '14N',
+    '15N',
+    '16O',
+    '17O',
+    '18O',
+    '19F',
+    '1H',
+    '1H-bar',
+    '20Ne',
+    '21Ne',
+    '22Ne',
+    '23Na',
+    '24Mg',
+    '25Mg',
+    '26Al',
+    '26Mg',
+    '27Al',
+    '28Si',
+    '29Si',
+    '2H',
+    '2H-bar',
+    '30Si',
+    '31P',
+    '32S',
+    '33S',
+    '34S',
+    '35Cl',
+    '36Ar',
+    '36Cl',
+    '36S',
+    '37Ar',
+    '37Cl',
+    '38Ar',
+    '39K',
+    '3He',
+    '40Ar',
+    '40Ca',
+    '40K',
+    '41Ca',
+    '41K',
+    '42Ca',
+    '43Ca',
+    '44Ca',
+    '44Ti',
+    '46Ca',
+    '46Ti',
+    '47Ti',
+    '48Ti',
+    '49Ti',
+    '49V',
+    '4He',
+    '50Cr',
+    '50Ti',
+    '50V',
+    '51Cr',
+    '51V',
+    '52Cr',
+    '53Cr',
+    '53Mn',
+    '54Cr',
+    '54Fe',
+    '54Mn',
+    '55Fe',
+    '55Mn',
+    '56Fe',
+    '56Ni',
+    '57Co',
+    '57Fe',
+    '58Fe',
+    '58Ni',
+    '59Co',
+    '59Ni',
+    '60Ni',
+    '61Ni',
+    '62Ni',
+    '63Cu',
+    '64Ni',
+    '64Zn',
+    '65Cu',
+    '66Zn',
+    '67Ga',
+    '67Zn',
+    '68Zn',
+    '69Ga',
+    '6Li',
+    '70Ge',
+    '70Zn',
+    '71Ga',
+    '71Ge',
+    '72Ge',
+    '73As',
+    '73Ge',
+    '74+75+76+77+78Se',
+    '74Ge',
+    '75As',
+    '76Ge',
+    '78+80+81+82Kr',
+    '79Br',
+    '7Be',
+    '7Li',
+    '80+82Se',
+    '81Br',
+    '83+84+86Kr',
+    '84+85+86Sr',
+    '87+88Sr',
+    '9Be',
+    '9Be+10Be',
+    'Ac',
+    'Al',
+    'AllParticles',
+    'Am',
+    'Ar',
+    'As',
+    'At',
+    'Au',
+    'B',
+    'Ba',
+    'Be',
+    'Bi',
+    'Bk',
+    'Br',
+    'C',
+    'C-Fe-group',
+    'C-bar',
+    'Ca',
+    'Cd',
+    'Ce',
+    'Cl',
+    'Cm',
+    'Co',
+    'Cr',
+    'Cs',
+    'Cu',
+    'DipoleAmplitude',
+    'DipolePhase',
+    'Dy',
+    'Er',
+    'Eu',
+    'F',
+    'Fe',
+    'Fe-group',
+    'Fr',
+    'Ga',
+    'Gd',
+    'Ge',
+    'H',
+    'H-He-group',
+    'He',
+    'He-bar',
+    'Hf',
+    'Hg',
+    'Ho',
+    'Ir',
+    'K',
+    'Kr',
+    'La',
+    'Li',
+    'Lu',
+    'Mg',
+    'Mn',
+    'Mo',
+    'N',
+    'N-group',
+    'Na',
+    'Nb',
+    'Nd',
+    'Ne',
+    'Ni',
+    'Np',
+    'O',
+    'O-group',
+    'Os',
+    'P',
+    'Pa',
+    'Pb',
+    'Pm',
+    'Po',
+    'Pr',
+    'Pt',
+    'Pu',
+    'Ra',
+    'Rb',
+    'Re',
+    'Rn',
+    'Ru',
+    'S',
+    'Sc',
+    'Se',
+    'Si',
+    'Sm',
+    'Sn',
+    'Sr',
+    'SubFe',
+    'Ta',
+    'Tb',
+    'Te',
+    'Th',
+    'Ti',
+    'Tl',
+    'Tm',
+    'U',
+    'V',
+    'W',
+    'Xe',
+    'Y',
+    'Yb',
+    'Z_33-34',
+    'Z_35-36',
+    'Z_37-38',
+    'Z_39-40',
+    'Z_41-42',
+    'Z_43-44',
+    'Z_45-46',
+    'Z_47-48',
+    'Z_49-50',
+    'Z_51-52',
+    'Z_53-54',
+    'Z_55-56',
+    'Z_57-58',
+    'Z_59-60',
+    'Z_62-69',
+    'Z_70-73',
+    'Z_74-80',
+    'Z_74-87',
+    'Z_81-87',
+    'Zgeq110',
+    'Zgeq2',
+    'Zgeq2-bar',
+    'Zgeq3',
+    'Zgeq3-bar',
+    'Zgeq55',
+    'Zgeq6',
+    'Zgeq6-bar',
+    'Zgeq65',
+    'Zgeq70',
+    'Zgeq88',
+    'Zgeq94',
+    'Zn',
+    'Zr',
+    'e+',
+    'e-',
+    'e-+e+',
 )
 
-ELEMENTS = {k: i + 1 for (i, k) in enumerate(VALID_NAMES[:99])}
+ELEMENTS = {
+    'H': 1,
+    'He': 2,
+    'Li': 3,
+    'Be': 4,
+    'B': 5,
+    'C': 6,
+    'N': 7,
+    'O': 8,
+    'F': 9,
+    'Ne': 10,
+    'Na': 11,
+    'Mg': 12,
+    'Al': 13,
+    'Si': 14,
+    'P': 15,
+    'S': 16,
+    'Cl': 17,
+    'Ar': 18,
+    'K': 19,
+    'Ca': 20,
+    'Sc': 21,
+    'Ti': 22,
+    'V': 23,
+    'Cr': 24,
+    'Mn': 25,
+    'Fe': 26,
+    'Co': 27,
+    'Ni': 28,
+    'Cu': 29,
+    'Zn': 30,
+    'Ga': 31,
+    'Ge': 32,
+    'As': 33,
+    'Se': 34,
+    'Br': 35,
+    'Kr': 36,
+    'Rb': 37,
+    'Sr': 38,
+    'Y': 39,
+    'Zr': 40,
+    'Nb': 41,
+    'Mo': 42,
+    'Tc': 43,
+    'Ru': 44,
+    'Rh': 45,
+    'Pd': 46,
+    'Ag': 47,
+    'Cd': 48,
+    'In': 49,
+    'Sn': 50,
+    'Sb': 51,
+    'Te': 52,
+    'I': 53,
+    'Xe': 54,
+    'Cs': 55,
+    'Ba': 56,
+    'La': 57,
+    'Ce': 58,
+    'Pr': 59,
+    'Nd': 60,
+    'Pm': 61,
+    'Sm': 62,
+    'Eu': 63,
+    'Gd': 64,
+    'Tb': 65,
+    'Dy': 66,
+    'Ho': 67,
+    'Er': 68,
+    'Tm': 69,
+    'Yb': 70,
+    'Lu': 71,
+    'Hf': 72,
+    'Ta': 73,
+    'W': 74,
+    'Re': 75,
+    'Os': 76,
+    'Ir': 77,
+    'Pt': 78,
+    'Au': 79,
+    'Hg': 80,
+    'Tl': 81,
+    'Pb': 82,
+    'Bi': 83,
+    'Po': 84,
+    'At': 85,
+    'Rn': 86,
+    'Fr': 87,
+    'Ra': 88,
+    'Ac': 89,
+    'Th': 90,
+    'Pa': 91,
+    'U': 92,
+    'Np': 93,
+    'Pu': 94,
+    'Am': 95,
+    'Cm': 96,
+    'Bk': 97,
+    'Cf': 98,
+    'Es': 99,
+}
 
 COMBINE = (
     "AESOP",
     "AMS01",
     "ATIC",
     "BESS",
     "BETS",
@@ -599,17 +673,18 @@
     if time_series:
         kwargs["time_series"] = time_series
     if format:
         kwargs["format"] = format
     if modulation:
         kwargs["modulation"] = modulation
 
-    return f"{server_url}/rest.php?" + "&".join(
+    url = f"{server_url}/rest.php?" + "&".join(
         ["{0}={1}".format(k, v) for (k, v) in kwargs.items()]
     )
+    return url
 
 
 @cachier.cachier(stale_after=timedelta(days=30))
 def _server_request(url: str, timeout: int) -> List[str]:
     # if there is a timeout error, we hide original long traceback from the internal
     # libs and instead show a simple traceback
     try:
@@ -752,14 +827,15 @@
     return result
 
 
 def clear_cache() -> None:
     """Delete the local CRDB cache."""
     _server_request.clear_cache()
     _all_request.clear_cache()
+    all.clear_cache()
 
 
 def reference_urls(table: np.recarray) -> List[str]:
     """Return list of URLs to entries in the ADSABS database for datasets in table."""
     result = []
     for key in sorted(np.unique(table.ads)):
         result.append(f"https://ui.adsabs.harvard.edu/abs/{key}")
@@ -826,14 +902,15 @@
 
     if not data:
         raise ValueError("empty server response")
 
     return data
 
 
+@cachier.cachier(stale_after=timedelta(days=30))
 def all() -> NDArray:
     """Return the full raw CRDB database as a table."""
     data = _all_request()
     return _convert_csv(data, _CSV_FIELDS)
 
 
 def solar_system_composition() -> Dict[str, List[Tuple[int, float]]]:
```

### Comparing `crdb-0.7.0/src/crdb/crdb_logo.png` & `crdb-0.8.0/src/crdb/crdb_logo.png`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/src/crdb/experimental.py` & `crdb-0.8.0/src/crdb/experimental.py`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/src/crdb/mpl.py` & `crdb-0.8.0/src/crdb/mpl.py`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/src/crdb/solarsystem_abundances2003.dat` & `crdb-0.8.0/src/crdb/solarsystem_abundances2003.dat`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/src/crdb.egg-info/PKG-INFO` & `crdb-0.8.0/src/crdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.7.0
+Version: 0.8.0
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `crdb-0.7.0/src/crdb.egg-info/SOURCES.txt` & `crdb-0.8.0/src/crdb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
+get_valid_names.py
 pyproject.toml
 setup.cfg
 .github/workflows/publish.yml
 .github/workflows/test.yml
 docs/authors.rst
 docs/build.py
 docs/changelog.rst
```

### Comparing `crdb-0.7.0/tests/test_experimental.py` & `crdb-0.8.0/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `crdb-0.7.0/tests/test_lib.py` & `crdb-0.8.0/tests/test_lib.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
-
+import numpy as np
 from crdb import ELEMENTS
+from crdb import VALID_NAMES
 from crdb import all
 from crdb import query
 from crdb import solar_system_composition
 
 
 @pytest.mark.parametrize("quantity", ("B/C", "H", "Li"))
 def test_all(quantity):
@@ -55,7 +56,18 @@
 
 def test_solar_system_composition():
     d = solar_system_composition()
     assert "H-bar" not in d
     assert d["H"] == [(1, 2.431e10), (2, 4.716e5)]
     assert d["Li"] == [(6, 4.21), (7, 51.26)]
     assert d["U"] == [(235, 0.000067), (238, 0.009238)]
+
+
+def test_VALID_NAMES():
+    tab = all()
+    valid = set()
+    for q in np.unique(tab.quantity):
+        num, *rest = q.split("/")
+        valid.add(num)
+        if rest:
+            valid.add(rest[0])
+    assert valid == set(VALID_NAMES)
```

### Comparing `crdb-0.7.0/tests/test_mpl.py` & `crdb-0.8.0/tests/test_mpl.py`

 * *Files identical despite different names*

