# Comparing `tmp/astro_ghost-0.2.3.tar.gz` & `tmp/astro_ghost-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-0.2.3.tar", last modified: Wed Mar  1 05:31:57 2023, max compression
+gzip compressed data, was "astro_ghost-0.2.4.tar", last modified: Tue May  9 06:01:47 2023, max compression
```

## Comparing `astro_ghost-0.2.3.tar` & `astro_ghost-0.2.4.tar`

### file list

```diff
@@ -1,57 +1,54 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-03-01 05:31:57.088329 astro_ghost-0.2.3/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-03-01 05:31:56.951791 astro_ghost-0.2.3/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-03-01 05:31:56.957596 astro_ghost-0.2.3/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      593 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3428 2023-03-01 05:31:57.088548 astro_ghost-0.2.3/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2827 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-03-01 05:31:57.077364 astro_ghost-0.2.3/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17721 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     5357 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    34065 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1047 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)   649501 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/Star_Galaxy_IdealModel.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)  3377881 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/Star_Galaxy_RealisticModel.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3394 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-03-01 01:53:33.000000 astro_ghost-0.2.3/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    22612 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/classifier.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    31268 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/dimensionalityReduction.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    34935 2023-03-01 01:50:13.000000 astro_ghost-0.2.3/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    30947 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2734 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17149 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9827 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17629 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4485 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/tonry_ps1_locus.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7106 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/transientHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3950 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1264 2023-02-17 00:45:54.000000 astro_ghost-0.2.3/astro_ghost/tutorial_databaseSearch.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-03-01 05:31:57.079984 astro_ghost-0.2.3/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3428 2023-03-01 05:31:56.000000 astro_ghost-0.2.3/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1273 2023-03-01 05:31:56.000000 astro_ghost-0.2.3/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-03-01 05:31:56.000000 astro_ghost-0.2.3/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-03-01 05:31:56.000000 astro_ghost-0.2.3/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      271 2023-03-01 05:31:56.000000 astro_ghost-0.2.3/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-03-01 05:31:56.000000 astro_ghost-0.2.3/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-03-01 05:31:57.084924 astro_ghost-0.2.3/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2323 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3908 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-03-01 05:31:57.086233 astro_ghost-0.2.3/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1568 2023-03-01 05:31:57.089599 astro_ghost-0.2.3/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1824 2023-03-01 01:53:26.000000 astro_ghost-0.2.3/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-03-01 05:31:57.087620 astro_ghost-0.2.3/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-0.2.3/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       58 2023-02-16 19:42:21.000000 astro_ghost-0.2.3/tests/test_basic.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2022-08-10 18:18:27.000000 astro_ghost-0.2.3/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.890842 astro_ghost-0.2.4/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.827431 astro_ghost-0.2.4/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.832830 astro_ghost-0.2.4/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      593 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3428 2023-05-09 06:01:47.891465 astro_ghost-0.2.4/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2827 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.879143 astro_ghost-0.2.4/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    14833 2023-05-08 20:39:24.000000 astro_ghost-0.2.4/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     6023 2023-05-08 20:39:46.000000 astro_ghost-0.2.4/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37406 2023-05-09 05:21:02.000000 astro_ghost-0.2.4/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1047 2023-02-17 00:45:54.000000 astro_ghost-0.2.4/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-0.2.4/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1496 2023-05-09 03:31:55.000000 astro_ghost-0.2.4/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-0.2.4/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-05-08 17:41:11.000000 astro_ghost-0.2.4/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-0.2.4/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37793 2023-05-09 04:36:12.000000 astro_ghost-0.2.4/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32155 2023-05-09 05:17:11.000000 astro_ghost-0.2.4/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2839 2023-05-09 05:55:39.000000 astro_ghost-0.2.4/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    16231 2023-05-09 05:36:08.000000 astro_ghost-0.2.4/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    10406 2023-05-09 05:55:34.000000 astro_ghost-0.2.4/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     6479 2023-05-09 03:37:31.000000 astro_ghost-0.2.4/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     5687 2023-05-08 21:51:30.000000 astro_ghost-0.2.4/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-0.2.4/astro_ghost/tonry_ps1_locus.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3817 2023-05-08 18:40:26.000000 astro_ghost-0.2.4/astro_ghost/tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1264 2023-02-17 00:45:54.000000 astro_ghost-0.2.4/astro_ghost/tutorial_databaseSearch.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.882704 astro_ghost-0.2.4/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3428 2023-05-09 06:01:47.000000 astro_ghost-0.2.4/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1105 2023-05-09 06:01:47.000000 astro_ghost-0.2.4/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-09 06:01:47.000000 astro_ghost-0.2.4/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-05-09 06:01:47.000000 astro_ghost-0.2.4/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      271 2023-05-09 06:01:47.000000 astro_ghost-0.2.4/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-05-09 06:01:47.000000 astro_ghost-0.2.4/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.883338 astro_ghost-0.2.4/database/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3288 2023-02-16 19:42:21.000000 astro_ghost-0.2.4/database/GHOST.csv
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.886192 astro_ghost-0.2.4/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2323 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3908 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.887849 astro_ghost-0.2.4/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1568 2023-05-09 06:01:47.892956 astro_ghost-0.2.4/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1824 2023-05-08 17:41:22.000000 astro_ghost-0.2.4/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-05-09 06:01:47.889692 astro_ghost-0.2.4/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-0.2.4/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       58 2023-02-16 19:42:21.000000 astro_ghost-0.2.4/tests/test_basic.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2022-08-10 18:18:27.000000 astro_ghost-0.2.4/tox.ini
```

### Comparing `astro_ghost-0.2.3/.github/workflows/tests.yml` & `astro_ghost-0.2.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/.gitignore` & `astro_ghost-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/PKG-INFO` & `astro_ghost-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-0.2.3/README.rst` & `astro_ghost-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-0.2.4/astro_ghost/NEDQueryFunctions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,30 @@
-import matplotlib
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astroquery.ned import Ned
-import warnings
-warnings.filterwarnings("ignore", category=UserWarning)
 import re
-import os
-import pandas as pd
 import numpy as np
-import seaborn as sns
-import matplotlib.pyplot as plt
 from astro_ghost.PS1QueryFunctions import find_all
 
-def getNEDSpectra(df, path, verbose=0):
+import warnings
+warnings.filterwarnings("ignore", category=UserWarning)
+
+def getNEDSpectra(df, path, verbose=False):
+    """Downloads NED spectra for the host galaxy, if it exists.
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+        Dataframe containing the associated transients and their host galaxies in PS1.
+    path : str
+        Filepath where NED spectra should be saved.
+    verbose : boolean
+        Whether to print relevant debugging information.
+
+    """
     hostNames = np.array(df.dropna(subset=['NED_name'])['NED_name'])
     transientNames = np.array(df.dropna(subset=['NED_name'])['TransientName'])
     for j in np.arange(len(hostNames)):
         try:
             spectra = Ned.get_spectra(hostNames[j])
         except:
             continue
@@ -30,18 +38,30 @@
                         print("Saving spectrum %i for %s, host of %s."%(i, hostNames[j], transientNames[j]))
                     try:
                         sp.writeto(path+"/%s_%.02i.fits"%(fn, i), output_verify='ignore')
                     except:
                         if verbose:
                             print("Error in saving host spectrum for %s." % transientNames[j])
                 elif verbose:
-#                    if verbose:
                     print("host spectrum for %s already downloaded!" % transientNames[j])
 
 def getNEDInfo(df):
+    """Gets galaxy information from NED, if it exists.
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+        Dataframe of the PS1 objects for which to query NED.
+
+    Returns
+    -------
+    df : Pandas DataFrame
+        The same dataframe as input, with NED info added.
+
+    """
     df.reset_index(inplace=True, drop=True)
 
     df['NED_name'] = ""
     df['NED_type'] = ""
     df["NED_vel"] = np.nan
     df["NED_redshift"] = np.nan
     df["NED_mag"] = np.nan
@@ -58,49 +78,52 @@
     sep = []
 
     missingCounter = 0
 
     for index, row in df.iterrows():
         tempRA = ra[index]
         tempDEC = dec[index]
+
         # create a sky coordinate to query NED
         c = SkyCoord(ra=tempRA*u.degree, dec=tempDEC*u.degree, frame='icrs')
+
         # execute query
         result_table = []
         tempName = ""
         tempType = ""
         tempRed = np.nan
         tempVel = np.nan
         tempMag = np.nan
 
         try:
+            #query NED with a 2'' radius.
             result_table = Ned.query_region(c, radius=(0.00055555)*u.deg, equinox='J2000.0')
-            #print(result_table)
+
             if len(result_table) > 0:
                 missingCounter = 0
         except:
             missingCounter += 1
-            #print(c)
         if len(result_table) > 0:
             result_table = result_table[result_table['Separation'] == np.min(result_table['Separation'])]
             result_table = result_table[result_table['Type'] != b'SN']
             result_table = result_table[result_table['Type'] != b'MCld']
             result_gal = result_table[result_table['Type'] == b'G']
             if len(result_gal) > 0:
                 result_table = result_gal
             if len(result_table) > 0:
+
+                # Subset for the objects with listed references and photometry, if more than one option.
                 result_table = result_table[result_table['Photometry Points'] == np.nanmax(result_table['Photometry Points'])]
                 result_table = result_table[result_table['References'] == np.nanmax(result_table['References'])]
-                #return result_table
+
                 # NED Info is presented as:
                 # No. ObjectName	RA	DEC	Type	Velocity	Redshift	Redshift Flag	Magnitude and Filter	Separation	References	Notes	Photometry Points	Positions	Redshift Points	Diameter Points	Associations
                 #Split NED info up - specifically, we want to pull the type, velocity, redshift, mag
                 tempNED = str(np.array(result_table)[0]).split(",")
                 if len(tempNED) > 2:
-                    #print("Found one!")
                     tempName = tempNED[1].strip().strip("b").strip("'")
                     if len(tempNED) > 20:
                         seps = [float(tempNED[9].strip()), float(tempNED[25].strip())]
                         if np.argmin(seps):
                             tempNED = tempNED[16:]
                     tempType =  tempNED[4].strip().strip("b").strip("''")
                     tempVel = tempNED[5].strip()
@@ -113,14 +136,16 @@
                         df.loc[index, 'NED_type'] = tempType
                     if tempVel:
                         df.loc[index, 'NED_vel'] = float(tempVel)
                     if tempRed:
                         df.loc[index, 'NED_redshift'] = float(tempRed)
                     if tempMag:
                         tempMag = re.findall(r"[-+]?\d*\.\d+|\d+", tempMag)[0]
-                        df.loc[index, 'NED_mag'] = float(tempMag) 
+                        df.loc[index, 'NED_mag'] = float(tempMag)
                     if tempRedFlag:
                         df.loc[index, 'NED_redshift_flag'] = str(tempRedFlag)
+                        
+        # if the method fails for many in a row, it's likely that too many queries have been made.
         if missingCounter > 5000:
             print("Locked out of NED, will have to try again later...")
             return df
     return df
```

### Comparing `astro_ghost-0.2.3/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-0.2.4/astro_ghost/PS1QueryFunctions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,162 +1,213 @@
-from __future__ import print_function
 import numpy as np
-from astropy.table import Table
 from PIL import Image
 from io import BytesIO
 import os
 import pandas as pd
-from astropy.io import fits
-from astropy.visualization import PercentileInterval, AsinhStretch
-from astropy.io import ascii
-from astropy.table import Table
 import sys
 import re
 import json
 import mastcasjobs
 import requests
 from datetime import datetime
-from astropy import units as u
-from astropy.coordinates import Angle
 try: # Python 3.x
     from urllib.parse import quote as urlencode
     from urllib.request import urlretrieve
+    import http.client as httplib
 except ImportError:  # Python 2.x
     from urllib import pathname2url as urlencode
     from urllib import urlretrieve
-try: # Python 3.x
-    import http.client as httplib
-except ImportError:  # Python 2.x
     import httplib
-# std lib
 from collections import OrderedDict
 from os import listdir
 from os.path import isfile, join
-# 3rd party
 from astropy import utils, io, convolution, wcs
-from astropy.visualization import make_lupton_rgb
-from astropy.coordinates import name_resolve
+from astropy import units as u
+from astropy.visualization import make_lupton_rgb,PercentileInterval, AsinhStretch
+from astropy.coordinates import name_resolve, Angle
+from astropy.io import fits, ascii
+from astropy.table import Table
 from pyvo.dal import sia
 import pickle
 from io import BytesIO
 
 from astropy.coordinates import SkyCoord
 from astroquery.vo_conesearch import ConeSearch
 from astroquery.vo_conesearch import vos_catalog
 vos_catalog.list_catalogs("conesearch_good")
 from warnings import simplefilter
 
-#could absolutely be more efficient, but filter for now 
+# could absolutely be more efficient, but filter out warnings for now
 simplefilter(action="ignore", category=pd.errors.PerformanceWarning)
 
-#set environmental variables
+# set a few environmental variables that we'll need to query PS2 for more accurate galaxy sizes.
 if "CASJOBS_USERID" not in os.environ:
     os.environ['CASJOBS_USERID'] = 'ghostbot'
     os.environ['CASJOBS_PW'] = 'ghostbot'
 
-def getAllPostageStamps(df, tempSize, path=".", verbose=0):
+def getAllPostageStamps(df, tempSize, path=".", verbose=False):
+    """Loops through a pandas dataframe and saves PS1 stacked color images of all
+       host galaxies.
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+        Description of parameter `df`.
+    tempSize : int
+        The downloaded image will be tempSize x tempSize pixels.
+    path : str
+        Filepath where images should be saved.
+    verbose : bool
+        If true, The progress of the image downloads is printed.
+
+    """
     for i in np.arange(len(df["raMean"])):
             tempRA = df.loc[i, 'raMean']
             tempDEC = df.loc[i, 'decMean']
             tempName = df.loc[i, 'TransientName']
             a = find_all(path+"/%s.png" % tempName, path)
             if not a:
                 try:
                     img = getcolorim(tempRA, tempDEC, size=tempSize, filters="grizy", format="png")
                     img.save(path+"/%s.png" % tempName)
                     if verbose:
                         print("Saving postage stamp for the host of %s."% tempName)
                 except:
                     continue
 
-def preview_image(i, ra, dec, rad, band, save=1):
-    a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, rad, band), ".")
-    hdul = fits.open(a[0])
-    image_file = get_pkg_data_filename(a[0])
-    image_data = fits.getdata(image_file, ext=0)
-    plt.figure()
-    plt.imshow(image_data,cmap='viridis')
-    plt.axis('off')
-    #plt.colorbar()
-    if save:
-        plt.savefig("PS1_%i_%s.png" % (i, band))
-
 def get_hosts(path, transient_fn, fn_Host, rad):
+    """Wrapper function for getting candidate host galaxies in PS1 for dec>-30 deg and
+       in Skymapper for dec<-30 deg.
+
+    Parameters
+    ----------
+    path : str
+        Filepath where csv of candidate hosts should be saved.
+    transient_fn : str
+        Filename of csv containing the transients to associate (and their coordinates).
+    fn_Host : str
+        Filename of csv containing candidate host galaxy properties.
+    rad : float
+        Search radius of the algorithm, in arcseconds.
+
+    Returns
+    -------
+    host_df : Pandas DataFrame
+        Dataframe of all candidate host galaxies.
+
+    """
     transient_df = pd.read_csv(path+"/"+transient_fn)
     now = datetime.now()
     dict_fn = fn_Host.replace(".csv", "") + ".p"
 
     tempDEC = Angle(transient_df['DEC'], unit=u.deg)
     tempDEC = tempDEC.deg
 
+    # distinguish between PS1 sources and Skymapper sources.
     df_North = transient_df[(tempDEC > -30)].reset_index()
     df_South = transient_df[(tempDEC <= -30)].reset_index()
-    #print("Number of southern sources = %i.\n" % len(df_South))
+
+    # get southern-hemisphere sources
     append=0
     if len(df_South) > 0:
         print("Finding southern sources with SkyMapper...")
         find_host_info_SH(df_South, fn_Host, dict_fn, path, rad)
         append=1
-    #print("Number of northern sources = %i.\n" % len(df_North))
+
+    # get northern-hemisphere sources
     if len(df_North) > 0:
         print("Finding northern sources with Pan-starrs...")
         find_host_info_PS1(df_North, fn_Host, dict_fn, path, rad, append=append)
+
+    # load the saved csv and remove duplicates, then return
     host_df = pd.read_csv(path+"/"+fn_Host)
     host_df = host_df.drop_duplicates()
     host_df.to_csv(path+"/"+fn_Host[:-4]+"_cleaned.csv", index=False)
     return host_df
 
 def find_all(name, path):
+    """Crawls through a directory and all its sub-directories looking for a file matching
+       'name'. If found, it is returned.
+
+    Parameters
+    ----------
+    name : str
+        The filename for which to search.
+    path : str
+        The directory to search.
+
+    Returns
+    -------
+    result : list
+        The list of absolute paths to all files called 'name' in 'path'.
+
+    """
     result = []
     for root, dirs, files in os.walk(path):
         if name in files:
             result.append(os.path.join(root, name))
     return result
 
 def getimages(ra,dec,size=240,filters="grizy", type='stack'):
+    """Query ps1filenames.py service to get a list of images.
 
-    """Query ps1filenames.py service to get a list of images
-
-    ra, dec = position in degrees
-    size = image size in pixels (0.25 arcsec/pixel)
-    filters = string with filters to include
-    Returns a table with the results
+    ra, dec : float
+        The position in degrees
+    size : int
+        The image size in pixels (0.25 arcsec/pixel)
+    filters : str
+        A string with the filters to include
+
+    Returns
+    -------
+    table : Astropy Table
+        The results of the search for relevant images.
     """
 
     service = "https://ps1images.stsci.edu/cgi-bin/ps1filenames.py"
     url = ("{service}?ra={ra}&dec={dec}&size={size}&format=fits"
            "&filters={filters}&type={type}").format(**locals())
     table = Table.read(url, format='ascii')
     return table
 
 
 def geturl(ra, dec, size=240, output_size=None, filters="grizy", format="jpg", color=False, type='stack'):
+    """Get the URL for images in the table.
 
-    """Get URL for images in the table
-
-    ra, dec = position in degrees
-    size = extracted image size in pixels (0.25 arcsec/pixel)
-    output_size = output (display) image size in pixels (default = size).
-                  output_size has no effect for fits format images.
-    filters = string with filters to include
-    format = data format (options are "jpg", "png" or "fits")
-    color = if True, creates a color image (only for jpg or png format).
-            Default is return a list of URLs for single-filter grayscale images.
-    Returns a string with the URL
+    ra, dec :
+        The position in degrees
+    size : int
+        The extracted image size in pixels (0.25 arcsec/pixel)
+    output_size : int
+        output (display) image size in pixels (default = size).
+        The output_size has no effect for fits format images.
+    filters : str
+        The string with filters to include.
+    format : str
+        The data format (options are "jpg", "png" or "fits").
+    color : bool
+        If True, creates a color image (only for jpg or png format).
+        If False, return a list of URLs for single-filter grayscale images.
+
+    Returns
+    -------
+    url : str
+        The url for the image to download.
     """
 
     if color and format == "fits":
         raise ValueError("color images are available only for jpg or png formats")
     if format not in ("jpg","png","fits"):
         raise ValueError("format must be one of jpg, png, fits")
     table = getimages(ra,dec,size=size,filters=filters, type=type)
     url = ("https://ps1images.stsci.edu/cgi-bin/fitscut.cgi?"
            "ra={ra}&dec={dec}&size={size}&format={format}").format(**locals())
     if output_size:
         url = url + "&output_size={}".format(output_size)
+
     # sort filters from red to blue
     flist = ["yzirg".find(x) for x in table['filter']]
     table = table[np.argsort(flist)]
     if color:
         if len(table) > 3:
             # pick 3 filters
             table = table[[0,len(table)//2,len(table)-1]]
@@ -167,119 +218,137 @@
         url = []
         for filename in table['filename']:
             url.append(urlbase+filename)
     return url
 
 
 def getcolorim(ra, dec, size=240, output_size=None, filters="grizy", format="jpg"):
+    """Get a PS1 color image at a sky position.
 
-    """Get color image at a sky position
-
-    ra, dec = position in degrees
-    size = extracted image size in pixels (0.25 arcsec/pixel)
-    output_size = output (display) image size in pixels (default = size).
-                  output_size has no effect for fits format images.
-    filters = string with filters to include
-    format = data format (options are "jpg", "png")
-    Returns the image
+    ra, dec : float
+        The position in degrees.
+    size : int
+        The extracted image size in pixels (0.25 arcsec/pixel).
+    output_size : int
+        The output (display) image size in pixels (default = size).
+        The output_size has no effect for fits format images.
+    filters : str
+        The string with filters to include.
+    format : str
+        The data format (options are "jpg", "png")
+    Returns
+    -------
+    im : PIL Image
+        The image.
     """
 
     if format not in ("jpg","png"):
         raise ValueError("format must be jpg or png")
     url = geturl(ra,dec,size=size,filters=filters,output_size=output_size,format=format,color=True, type='stack')
     r = requests.get(url)
     im = Image.open(BytesIO(r.content))
     return im
 
+def get_PS1_type(ra, dec, size, band, type):
+    """Download and save PS1 imaging data in a given band of a given type.
 
-def getgrayim(ra, dec, size=240, output_size=None, filter="g", format="jpg"):
-
-    """Get grayscale image at a sky position
+    Parameters
+    ----------
+    ra, dec : float
+        The position in degrees.
+    size : int
+        The size of the image in pixels.
+    band : str
+        The PS1 band.
+    type : str
+        The type of imaging data to obtain. Options are given below for the PS1 stack:
+            'stack.mask' images indicate which pixels in the stack are good and which are bad
+            'stack.wt' images are the stack variance images
+            'stack.num' images contain the number of warps with valid data which contributed to each pixel
+            'stack.exp' images contain the exposure time in seconds which contributed to each pixel
+            'stack.expwt' images are weighted exposure time maps
+        See more information at https://outerspace.stsci.edu/display/PANSTARRS/PS1+Stack+images.
 
-    ra, dec = position in degrees
-    size = extracted image size in pixels (0.25 arcsec/pixel)
-    output_size = output (display) image size in pixels (default = size).
-                  output_size has no effect for fits format images.
-    filter = string with filter to extract (one of grizy)
-    format = data format (options are "jpg", "png")
-    Returns the image
     """
-
-    if format not in ("jpg","png"):
-        raise ValueError("format must be jpg or png")
-    if filter not in list("grizy"):
-        raise ValueError("filter must be one of grizy")
-    url = geturl(ra,dec,size=size,filters=filter,output_size=output_size,format=format)
-    r = requests.get(url[0])
-    im = Image.open(BytesIO(r.content))
-    return im
-
-def get_PS1_type(ra, dec, rad, band, type):
-    fitsurl = geturl(ra, dec, size=rad, filters="{}".format(band), format="fits", type=type)
+    fitsurl = geturl(ra, dec, size=size, filters="{}".format(band), format="fits", type=type)
     fh = fits.open(fitsurl[0])
-    fh.writeto('PS1_ra={}_dec={}_{}arcsec_{}_{}.fits'.format(ra, dec, int(rad*0.25), band, type))
+    fh.writeto('PS1_ra={}_dec={}_{}arcsec_{}_{}.fits'.format(ra, dec, int(size*0.25), band, type))
 
-def get_PS1_wt(ra, dec, rad, band):
-    fitsurl = geturl(ra, dec, size=rad, filters="{}".format(band), format="fits", type='stack.wt')
-    fh = fits.open(fitsurl[0])
-    fh.writeto('PS1_ra={}_dec={}_{}arcsec_{}_wt.fits'.format(ra, dec, int(rad*0.25), band))
+def get_PS1_Pic(objID, ra, dec, size, band, safe=False):
+    """Downloads PS1 picture (in fits) at a given position.
 
-def get_PS1_mask(ra, dec, rad, band):
-    fitsurl = geturl(ra, dec, size=rad, filters="{}".format(band), format="fits", type='stack.mask')
-    fh = fits.open(fitsurl[0])
-    fh.writeto('PS1_ra={}_dec={}_{}arcsec_{}_mask.fits'.format(ra, dec, int(rad*0.25), band))
+    Parameters
+    ----------
+    objID : int
+        The PS1 objID of the object of interest (to save as filename).
+    ra, dec : float
+        The position in degrees.
+    size : int
+        The size of the of the image, in pixels (image is size x size).
+    band : str
+        The PS1 passband.
+    safe : bool
+        If True, include the objID of the object of interest in the filename
+        (useful when saving multiple files at comparable positions).
 
-def get_PS1_Pic(objID, ra, dec, rad, band, safe=False):
-    fitsurl = geturl(ra, dec, size=rad, filters="{}".format(band), format="fits")
+    """
+    fitsurl = geturl(ra, dec, size=size, filters="{}".format(band), format="fits")
     fh = fits.open(fitsurl[0])
     if safe==True:
-        fh.writeto('PS1_{}_{}arcsec_{}.fits'.format(objID, int(rad*0.25), band))
+        fh.writeto('PS1_{}_{}arcsec_{}.fits'.format(objID, int(size*0.25), band))
     else:
-        fh.writeto('PS1_ra={}_dec={}_{}arcsec_{}.fits'.format(ra, dec, int(rad*0.25), band))
-
-# Data Lab
-#from dl import queryClient as qc
-#from dl.helpers.utils import convert
+        fh.writeto('PS1_ra={}_dec={}_{}arcsec_{}.fits'.format(ra, dec, int(size*0.25), band))
 
-# set up Simple Image Access (SIA) service
-DEF_ACCESS_URL = "http://datalab.noao.edu/sia/des_dr1"
-svc = sia.SIAService(DEF_ACCESS_URL)
-
-##################### PS1 HELPER FUNCTIONS ############################################
 def ps1metadata(table="mean",release="dr1",baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs"):
-    """Return metadata for the specified catalog and table
+    """Return metadata for the specified catalog and table.
 
     Parameters
     ----------
-    table (string): mean, stack, or detection
-    release (string): dr1 or dr2
-    baseurl: base URL for the request
+    table : str
+        Table type. Can be 'mean', 'stack', or 'detection'
+    release: str
+        The Pan-STARRS data release. Can be 'dr1' or 'dr2'.
+    baseurl: str
+        The base URL for the request
+
+    Returns
+    -------
+    Astropy Table
+        The table containing the metadata, with columns name, type, and description.
 
-    Returns an astropy table with columns name, type, description
     """
 
     checklegal(table,release)
     url = "{baseurl}/{release}/{table}/metadata".format(**locals())
     r = requests.get(url)
     r.raise_for_status()
     v = r.json()
+
     # convert to astropy table
     tab = Table(rows=[(x['name'],x['type'],x['description']) for x in v],
                names=('name','type','description'))
     return tab
 
 
 def mastQuery(request):
     """Perform a MAST query.
 
-        Parameters
-        ----------
-        request (dictionary): The MAST request json object
+    Parameters
+    ----------
+    request : dictionary
+        The MAST request json object.
+
+    Returns
+    -------
+    head : HTTP header
+        The response HTTP headers.
+    content :
+        The data obtained.
 
-        Returns head,content where head is the response HTTP headers, and content is the returned data"""
+    """
 
     server='mast.stsci.edu'
 
     # Grab Python Version
     version = ".".join(map(str, sys.version_info[:3]))
 
     # Create Http Header Variables
@@ -304,66 +373,85 @@
 
     # Close the https connection
     conn.close()
 
     return head,content
 
 def resolve(name):
-    """Get the RA and Dec for an object using the MAST name resolver
+    """Get the RA and Dec for an object using the MAST name resolver.
 
     Parameters
     ----------
-    name (str): Name of object
+    name : str
+        Name of the object of interest.
 
-    Returns RA, Dec tuple with position"""
+    Returns
+    -------
+    (objRa, objDec) : tuple
+        Position of resolved object.
+
+    """
 
     resolverRequest = {'service':'Mast.Name.Lookup',
                        'params':{'input':name,
                                  'format':'json'
                                 },
                       }
     headers,resolvedObjectString = mastQuery(resolverRequest)
     resolvedObject = json.loads(resolvedObjectString)
+
     # The resolver returns a variety of information about the resolved object,
     # however for our purposes all we need are the RA and Dec
     try:
         objRa = resolvedObject['resolvedCoordinate'][0]['ra']
         objDec = resolvedObject['resolvedCoordinate'][0]['decl']
     except IndexError as e:
         raise ValueError("Unknown object '{}'".format(name))
     return (objRa, objDec)
 
 def checklegal(table,release):
-    """Checks if this combination of table and release is acceptable
+    """Checks if this combination of table and release is acceptable.
+       Raises a VelueError exception if there is problem.
 
-    Raises a VelueError exception if there is problem
     """
 
     releaselist = ("dr1", "dr2")
     if release not in ("dr1","dr2"):
         raise ValueError("Bad value for release (must be one of {})".format(', '.join(releaselist)))
     if release=="dr1":
         tablelist = ("mean", "stack")
     else:
         tablelist = ("mean", "stack", "detection")
     if table not in tablelist:
         raise ValueError("Bad value for table (for {} must be one of {})".format(release, ", ".join(tablelist)))
 
 def ps1search(table="mean",release="dr1",format="csv",columns=None,baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs", verbose=False,**kw):
-    """Do a general search of the PS1 catalog (possibly without ra/dec/radius)
+    """Do a general search of the PS1 catalog (possibly without ra/dec/radius).
 
     Parameters
     ----------
-    table (string): mean, stack, or detection
-    release (string): dr1 or dr2
-    format: csv, votable, json
-    columns: list of column names to include (None means use defaults)
-    baseurl: base URL for the request
-    verbose: print info about request
-    **kw: other parameters (e.g., 'nDetections.min':2).  Note this is required!
+    table: str
+        Can be 'mean', 'stack', or 'detection'.
+    release: str
+        PS1 data release. Can be 'dr1' or 'dr2'.
+    format: str
+        Can be 'csv', 'votable', or 'json'.
+    columns: list
+        Column names to include (None means use defaults).
+    baseurl: str
+        Base URL for the request.
+    verbose: bool
+        If true, print info about request.
+    **kw: dictionary
+        Other parameters (e.g., 'nDetections.min':2).  Note that this is required!
+
+    Returns
+    -------
+    r : 'format'
+        Result of PS1 query, in 'csv', 'votable', or 'json' format.
     """
 
     data = kw.copy()
     if not data:
         raise ValueError("You must specify some parameters for search")
     checklegal(table,release)
     if format not in ("csv","votable","json"):
@@ -378,174 +466,224 @@
         badcols = []
         for col in columns:
             if col.lower().strip() not in dcols:
                 badcols.append(col)
         if badcols:
             raise ValueError('Some columns not found in table: {}'.format(', '.join(badcols)))
         # two different ways to specify a list of column values in the API
-        # data['columns'] = columns
         data['columns'] = '[{}]'.format(','.join(columns))
 
-# either get or post works
-#    r = requests.post(url, data=data)
+    # either get or post works
     r = requests.get(url, params=data)
 
     if verbose:
         print(r.url)
     r.raise_for_status()
     if format == "json":
         return r.json()
     else:
         return r.text
 
 
 def ps1cone(ra,dec,radius,table="stack",release="dr1",format="csv",columns=None,baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs", verbose=False,**kw):
-    """Do a cone search of the PS1 catalog
+    """Do a cone search of the PS1 catalog. Note that this is just a thin wrapper for the function 'ps1search'.
 
     Parameters
     ----------
-    ra (float): (degrees) J2000 Right Ascension
-    dec (float): (degrees) J2000 Declination
-    radius (float): (degrees) Search radius (<= 0.5 degrees)
-    table (string): mean, stack, or detection
-    release (string): dr1 or dr2
-    format: csv, votable, json
-    columns: list of column names to include (None means use defaults)
-    baseurl: base URL for the request
-    verbose: print info about request
-    **kw: other parameters (e.g., 'nDetections.min':2)
+    ra, dec: float
+        Central coordinates for the cone search, in J2000 degrees.
+    radius : float
+        Search radius, in degrees (<= 0.5 degrees)
+    table: str
+        Can be 'mean', 'stack', or 'detection'.
+    release: str
+        PS1 data release. Can be 'dr1' or 'dr2'.
+    format: str
+        Can be 'csv', 'votable', or 'json'.
+    columns: list
+        Column names to include (None means use defaults).
+    baseurl: str
+        Base URL for the request.
+    verbose: bool
+        If true, print info about request.
+    **kw: dictionary
+        Other parameters (e.g., 'nDetections.min':2).
+
+    Returns
+    -------
+    r : 'format'
+        Result of PS1 query, in 'csv', 'votable', or 'json' format.
     """
 
     data = kw.copy()
     data['ra'] = ra
     data['dec'] = dec
     data['radius'] = radius
     return ps1search(table=table,release=release,format=format,columns=columns,
                     baseurl=baseurl, verbose=verbose, **data)
 
-#########################END PS1 HELPER FUNCTIONS##############################################
-
 def create_df(tns_loc):
-    """Combine all supernovae data into dataframe"""
+    """Combine all supernova data into a single dataframe.
+
+    Parameters
+    ----------
+    tns_loc : str
+        Filepath where files containing TNS data is stored.
+
+    Returns
+    -------
+    df : Pandas DataFrame
+        Dataframe of all TNS metadata.
+
+    """
     files = [f for f in listdir(tns_loc) if isfile(join(tns_loc, f))]
     arr = []
     for file in files:
         tempPD = pd.read_csv(tns_loc+file)
         arr.append(tempPD)
     df = pd.concat(arr)
     df = df.loc[df['RA'] != '00:00:00.000']
     df = df.drop_duplicates()
     df = df.replace({'Anon.': ''})
     df = df.replace({'2019-02-13.49': ''})
     df = df.apply(lambda x: x.str.strip() if x.dtype == "object" else x)
     return df
-    #df.to_csv('SNe_TNS_061019.csv')
 
-def query_ps1_noname(RA, DEC, rad):
-    #print("Querying PS1 for nearest host...")
-    return ps1cone(RA,DEC,rad/3600,table="stack",release="dr1",format="csv",columns=None,baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs", verbose=False)
-
-def query_ps1_name(name, rad):
-    #print("Querying PS1 with host name!")
-    [ra, dec] = resolve(name)
-    return ps1cone(ra,dec,rad/3600,table="stack",release="dr1",format="csv",columns=None,baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs", verbose=False)
-
-# stolen from the wonderful API at https://ps1images.stsci.edu/ps1_dr2_api.html
-def ps1metadata(table="mean",release="dr1",
-           baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs"):
-    """Return metadata for the specified catalog and table
+def ps1metadata(table="mean", release="dr1", baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs"):
+    """Return metadata for the specified catalog and table. Snagged from the
+       wonderful API at https://ps1images.stsci.edu/ps1_dr2_api.html.
 
     Parameters
     ----------
-    table (string): mean, stack, or detection
-    release (string): dr1 or dr2
-    baseurl: base URL for the request
+    table: str
+        Can be 'mean', 'stack', or 'detection'.
+    release: str
+        PS1 data release. Can be 'dr1' or 'dr2'.
+    baseurl: str
+        Base URL for the request.
+
+    Returns
+    -------
+    tab : Astropy Table
+        Table with columns name, type, description.
 
-    Returns an astropy table with columns name, type, description
     """
 
     checklegal(table,release)
     url = f"{baseurl}/{release}/{table}/metadata"
     r = requests.get(url)
     r.raise_for_status()
     v = r.json()
+
     # convert to astropy table
     tab = Table(rows=[(x['name'],x['type'],x['description']) for x in v],
                names=('name','type','description'))
     return tab
 
-# Queries PS1 to find host info for each transient
-# Input: df - a dataframe of all spectroscopically classified transients in TNS
-#        fn - the output data frame of all PS1 potential hosts
-#        dict_fn - the dictionary matching candidate hosts in PS1 and transients
-# Output: N/A
 def find_host_info_PS1(df, fn, dict_fn, path, rad, append=0):
+    """Querying PS1 for all objects within rad arcsec of each SN.
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+        Dataframe of transient information (name and coordinates).
+    fn : str
+        The output data frame of all PS1 potential hosts.
+    dict_fn : str
+        The filename of the dictionary to keep track of transient-candidate host matches.
+        Keys are transient names, values are lists containing objIDs of all host candidates.
+    path : str
+        The filepath where df will be saved.
+    rad : float
+        The search radius, in arcsec.
+    append : bool
+        If True, append results to fn. If False, create a new file.
+
+    """
     i = 0
-    """Querying PS1 for all objects within rad arcsec of SNe"""
-    #os.chdir()
-    # SN_Host_PS1 - the dictionary to map SN IDs to nearby obj IDs in PS1
-    # EDIT - We now know there are MANY SNe without IDs!! This is pretty problematic, so we're going to switch to
-    # keeping a dictionary between names and objIDs
+
+    # The dictionary to map SN names to nearby obj IDs in PS1
     SN_Host_PS1 = {}
-    # PS1_queries - an array of relevant PS1 obj info
+
+    #a running list of all PS1 results
     PS1_queries = []
     for j, row in enumerate(df.itertuples(), 1):
             if ":" in str(row.RA):
                 tempRA = Angle(row.RA, unit=u.hourangle)
             else:
                 tempRA = Angle(row.RA, unit=u.deg)
             tempDEC = Angle(row.DEC, unit=u.deg)
-            a = query_ps1_noname(tempRA.degree,tempDEC.degree, rad)
+            a = ps1cone(tempRA.degree,tempDEC.degree,rad/3600,table="stack",release="dr1",format="csv",columns=None,baseurl="https://catalogs.mast.stsci.edu/api/v0.1/panstarrs", verbose=False)
             if a:
                 a = ascii.read(a)
                 a = a.to_pandas()
                 PS1_queries.append(a)
                 SN_Host_PS1[row.Name] = np.array(a['objID'])
             else:
                 SN_Host_PS1[row.Name] = np.array([])
 
             # Print status messages every 10 lines
             if j%10 == 0:
                 print("Processed {} of {} lines!".format(j, len(df.Name)))
-                #print(SN_Host_PS1)
 
-            # Print every query to a file Note: this was done in order
+            # Print every query to a file. This was done in order
             # to prevent the code crashing after processing 99% of the data
-            # frame and losing everything. This allows for duplicates though,
-            # so they should be removed before the file is used again
+            # frame and losing everything. This allows for duplicates, though,
+            # so they should be removed before the file is used again.
             if (len(PS1_queries) > 0):
                 PS1_hosts = pd.concat(PS1_queries)
                 PS1_hosts = PS1_hosts.drop_duplicates()
+
+                #match up rows to skymapper cols to join into a single dataframe
                 newCols = np.array(['SkyMapper_StarClass', 'gelong','g_a','g_b','g_pa',
                 'relong','r_a','r_b','r_pa',
                 'ielong','i_a','i_b','i_pa',
                 'zelong','z_a','z_b','z_pa'])
                 for col in newCols:
-                    PS1_hosts[col] = np.nan #match up rows to skymapper cols to join in one dataframe
+                    PS1_hosts[col] = np.nan
                 PS1_queries = []
                 if not append:
                     PS1_hosts.to_csv(path+fn, header=True, index=False)
                     i = 1
                     append = True
                 else:
                     PS1_hosts.to_csv(path+"/"+fn, mode='a+', header=False, index=False)
             else:
                 print("No potential hosts found for this object...")
+
             # Save host info
             if not os.path.exists(path+ '/dictionaries/'):
             	os.makedirs(path+'/dictionaries/')
             option = "wb"
             if append:
                 option = "ab"
             with open(path+"/dictionaries/" + dict_fn, option) as fp:
                 pickle.dump(SN_Host_PS1, fp, protocol=pickle.HIGHEST_PROTOCOL)
 
 def find_host_info_SH(df, fn, dict_fn, path, rad):
+    """VO Cone Search for all objects within rad arcsec of SNe (for Southern-Hemisphere (SH) objects).
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+        Dataframe of transient information (name and coordinates).
+    fn : str
+        The output data frame of all PS1 potential hosts.
+    dict_fn : str
+        The filename of the dictionary to keep track of transient-candidate host matches.
+        Keys are transient names, values are lists containing objIDs of all host candidates.
+    path : str
+        The filepath where df will be saved.
+    rad : float
+        The search radius, in arcsec.
+    append : bool
+        If True, append results to fn. If False, create a new file.
+
+    """
     i = 0
-    """VO Cone Search for all objects within rad arcsec of SNe (for Southern-Hemisphere (SH) objects)"""
     SN_Host_SH = {}
     SH_queries = []
     pd.options.mode.chained_assignment = None
     for j, row in df.iterrows():
             if ":" in str(row.RA):
                 tempRA = Angle(row.RA, unit=u.hourangle)
             else:
@@ -558,15 +696,14 @@
                 SN_Host_SH[row.Name] = np.array(a['objID'])
             else:
                 SN_Host_SH[row.Name] = np.array([])
 
             # Print status messages every 10 lines
             if j%10 == 0:
                 print("Processed {} of {} lines!".format(j, len(df.Name)))
-                #print(SN_Host_PS1)
 
             # Print every query to a file Note: this was done in order
             # to prevent the code crashing after processing 99% of the data
             # frame and losing everything. This allows for duplicates though,
             # so they should be removed before the file is used again
             if (len(SH_queries) > 0):
                 SH_hosts = pd.concat(SH_queries)
@@ -575,41 +712,60 @@
                 if i == 0:
                     SH_hosts.to_csv(path+"/"+fn, header=True, index=False)
                     i = 1
                 else:
                     SH_hosts.to_csv(path+"/"+fn, mode='a+', header=False, index=False)
             else:
                 print("No potential hosts found for this object...")
+
             # Save host info
             if not os.path.exists(path+ '/dictionaries/'):
             	os.makedirs(path+'/dictionaries/')
             with open(path+"/dictionaries/" + dict_fn, 'wb') as fp:
                 pickle.dump(SN_Host_SH, fp, protocol=pickle.HIGHEST_PROTOCOL)
     pd.options.mode.chained_assignment = 'warn'
 
 def southernSearch(ra, dec, rad):
+    """Conducts a cone search for Skymapper objects at a given position.
+
+    Parameters
+    ----------
+    ra, dec : float
+        Search position, in degrees.
+    rad : float
+        Search radius, in degrees.
+
+    Returns
+    -------
+    fullDF : Pandas DataFrame
+        Dataframe of Skymapper objects formatted to be joined with PS1 sources.
+
+    """
     searchCoord = SkyCoord(ra*u.deg, dec*u.deg, frame='icrs')
     responseMain = requests.get("http://skymapper.anu.edu.au/sm-cone/public/query?CATALOG=dr2.master&RA=%.5f&DEC=%.5f&SR=%.5f&RESPONSEFORMAT=CSV&VERB=3" %(ra, dec, (rad/3600)))
     responsePhot = requests.get("http://skymapper.anu.edu.au/sm-cone/public/query?CATALOG=dr2.photometry&RA=%.5f&DEC=%.5f&SR=%.5f&RESPONSEFORMAT=CSV&VERB=3" %(ra, dec, (rad/3600)))
 
     dfMain = pd.read_csv(BytesIO(responseMain.content))
     dfPhot = pd.read_csv(BytesIO(responsePhot.content))
 
     filt_dfs = []
     for filter in 'griz':
+
         #add the photometry columns
         tempDF = dfPhot[dfPhot['filter']==filter]
         if len(tempDF) <1:
             tempDF.append(pd.Series(), ignore_index=True) #add dummy row for the sake of not crashing
         for col in tempDF.columns.values:
             if col != 'object_id':
                 tempDF[filter + col] = tempDF[col]
                 del tempDF[col]
-        #take the column with the smallest uncertainty in the measured semi-major axis - this is what we'll use to
-        #calculate DLR later!
+
+        # take the column with the smallest uncertainty in the measured semi-major axis -
+        # this is what we'll use to
+        # calculate DLR later!
         tempDF = tempDF.loc[tempDF.groupby("object_id")[filter + 'e_a'].idxmin()]
         filt_dfs.append(tempDF)
 
     test = filt_dfs[0]
 
     for i in np.arange(1, len(filt_dfs)):
         test = test.merge(filt_dfs[i], on='object_id', how='outer')
@@ -726,55 +882,90 @@
 
     for i in np.arange(len(df_cols)):
         if df_cols[i] == 'nan':
             fullDF[mapped_cols[i]] = np.nan
         else:
             fullDF[mapped_cols[i]] = fullDF[df_cols[i]]
 
-    fullDF['gPlateScale'] = 0.50 #''/px
-    fullDF['rPlateScale'] = 0.50 #''/px
-    fullDF['iPlateScale'] = 0.50 #''/px
-    fullDF['zPlateScale'] = 0.50 #''/px #plate scale of skymapper
-    fullDF['yPlateScale'] = 0.50
+    # save the plate scale of skymapper in each band
+    for band in 'grizy':
+        fullDF['%sPlateScale'%band] = 0.5
     fullDF['primaryDetection'] = 1
     fullDF['bestDetection'] = 1
-    fullDF['qualityFlag'] = 0 #dummy variable set so that no sources get cut by qualityFlag in PS1 (which isn't in SkyMapper)
-    fullDF['ny'] = 1 #dummy variable
+
+    #dummy variable set so that no sources get cut by qualityFlag in PS1 (which isn't in SkyMapper)
+    fullDF['qualityFlag'] = 0
+
+    #dummy variable
+    fullDF['ny'] = 1
     colSet = np.concatenate([list(flag_mapping.keys()), ['gPlateScale', 'rPlateScale',
         'iPlateScale', 'zPlateScale', 'yPlateScale', 'primaryDetection', 'bestDetection', 'qualityFlag', 'ny']])
 
     fullDF = fullDF[colSet]
 
     leftover = set(PS1_cols) - set(fullDF.columns.values)
     for col in leftover:
         fullDF[col] = np.nan
 
-    #fullDF = fullDF[PS1_cols] #arrange correctly
     fullDF.drop_duplicates(subset=['objID'], inplace=True)
     return fullDF
 
 def getDR2_petrosianSizes(ra_arr, dec_arr, rad):
+    """Retrieves petrosian radius information from DR2 for panstarrs sources.
+
+    Parameters
+    ----------
+    ra_arr : list
+        List of right ascension values, in degrees.
+    dec_arr : list
+        List of declination values, in degrees.
+    rad : float
+        The search radius, in arcseconds.
+
+    Returns
+    -------
+    df_petro_full : Pandas DataFrame
+        Dataframe containing dr2 petrosian radiuses.
+
+    """
     if len(ra_arr) < 1:
         return
-    
-    halfLightList = []
+
+    petroList = []
     for i in np.arange(len(ra_arr)):
         query = """select st.objID, st.primaryDetection, st.gpetR90, st.rpetR90, st.ipetR90, st.zpetR90, st.ypetR90
         from fGetNearbyObjEq(%.3f,%.3f,%.1f/60.0) nb
         inner join StackPetrosian st on st.objID=nb.objid where st.primaryDetection = 1""" %(ra_arr[i], dec_arr[i], rad)
 
         jobs = mastcasjobs.MastCasJobs(context="PanSTARRS_DR2")
-        tab = jobs.quick(query, task_name="halfLightSearch")
-        df_halfLight = tab.to_pandas()
-        halfLightList.append(df_halfLight)
+        tab = jobs.quick(query, task_name="PetrosianRadiusSearch")
+        df_petro = tab.to_pandas()
+        petroList.append(df_petro)
 
-    df_halfLight_full = pd.concat(halfLightList)
-    return df_halfLight_full
+    df_petro_full = pd.concat(petroList)
+    return df_petro_full
 
 def getDR2_halfLightSizes(ra_arr, dec_arr, rad):
+    """Retrieves half-light radius information from DR2 for panstarrs sources.
+
+    Parameters
+    ----------
+    ra_arr : list
+        List of right ascension values, in degrees.
+    dec_arr : list
+        List of declination values, in degrees.
+    rad : float
+        The search radius, in arcseconds.
+
+    Returns
+    -------
+    df_halfLight_full : Pandas DataFrame
+        Dataframe containing dr2 half-light radiuses.
+
+    """
     if len(ra_arr) < 1:
         return
 
     halfLightList = []
     for i in np.arange(len(ra_arr)):
         query = """select st.objID, st.primaryDetection, st.gHalfLightRad, st.rHalfLightRad, st.iHalfLightRad,
         st.zHalfLightRad, st.yHalfLightRad from fGetNearbyObjEq(%.3f,%.3f,%.1f/60.0) nb
```

### Comparing `astro_ghost-0.2.3/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-0.2.4/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-0.2.4/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/astro_ghost/conftest.py` & `astro_ghost-0.2.4/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-0.2.4/astro_ghost/ghostHelperFunctions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 import numpy as np
 from astropy.table import Table
-import requests
 from PIL import Image
 from io import BytesIO
 import pathlib
 import os
 import sys
 import pandas as pd
 import matplotlib.pyplot as plt
 from astropy.io import fits
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 import re
+import astro_ghost
 from astro_ghost.PS1QueryFunctions import *
 from astro_ghost.hostMatching import build_ML_df
 from astro_ghost.NEDQueryFunctions import getNEDInfo
 from astro_ghost.SimbadQueryFunctions import getSimbadInfo
 from astro_ghost.gradientAscent import gradientAscent
 from astro_ghost.starSeparation import separateStars_STRM, separateStars_South
 from astro_ghost.sourceCleaning import clean_dict, removePS1Duplicates, getColors, makeCuts
 from astro_ghost.stellarLocus import calc_7DCD
 from astro_ghost.DLR import chooseByDLR
 import requests
 import pickle
-import os
 import glob
 from datetime import datetime
-import astro_ghost
 from joblib import dump, load
 
 def getGHOST(real=False, verbose=False, installpath='', clobber=False):
+    """Downloads the GHOST database.
+
+    Parameters
+    ----------
+    real : bool
+        If True, download the GHOST database. If False, write an empty files with
+        relevant columns (so that every transient is manually associated).
+    verbose : bool
+        If True, print debugging info.
+    installpath : str
+        Filepath where GHOST database will be installed.
+    clobber : bool
+        If True, write new GHOST database even if it already exists at installpath.
+
+    """
     if not installpath:
         try:
             installpath = os.environ['GHOST_PATH']
         except:
             print("Couldn't find where you want to save GHOST. Setting location to package path...")
             installpath = astro_ghost.__file__
             installpath = installpath.split("/")[:-1]
@@ -122,75 +135,80 @@
             'host_logmass', 'host_logmass_min', 'host_logmass_max',
             'Hubble Residual', 'TransientName']
         df = pd.DataFrame(columns = colnames)
         df.to_csv(installpath + "/database/GHOST.csv",index=False)
         if verbose:
             print("Successfully created dummy database.\n")
 
-# Calculates the fraction of supernovae
-# in our dictionary that have at least
-# one candidate host associated with
-# them.
-# input: transient_dict, the dictionary
-#        of supernovae and their host
-#        galaxy candidate objIDs from PS1
-# output: the fraction of supernovae
-#         with candidate hosts
 def fracWithHosts(transient_dict):
+    """Calculates the fraction of supernovae
+       in our dictionary that have at least
+       one candidate host associated with
+       them.
+
+    Parameters
+    ----------
+    transient_dict : dictionary
+        The dictionary of supernovae and their host galaxy candidate objIDs from PS1.
+
+    Returns
+    -------
+    dictionary
+        the fraction of supernovae with at least one candidate host galaxy.
+
+    """
     count = 0
     for name, host in transient_dict.items():
         # only do matching if there's a found host
         if isinstance(host, list) or isinstance(host, np.ndarray):
             if len(host) > 0 and np.any(np.array(host == host)):
                 count += 1
-        #elif isinstance(host, np.ndarray):
-        #    if len(host) > 0 and np.any(np.array(host == host)):
-        #        count += 1
         else:
             if host == host:
                 count+=1
     return count/len(transient_dict.keys())
 
-# Removes the prefix from a string
-# input - text and prefix to remove from text
-# output - text without prefix
-# very useful for removing the 'SN' from
-# supernova names!
 def remove_prefix(text, prefix):
+    """Removes the prefix from a string. Very useful for removing the 'SN' from
+       supernova names!
+
+    Parameters
+    ----------
+    text : str
+        The full text.
+    prefix : str
+        The prefix to remove from the text.
+
+    Returns
+    -------
+    str
+        The input text, with prefix removed.
+
+    """
     return text[text.startswith(prefix) and len(prefix):]
 
-# Gets the host associated with a supernova in
-# the GHOST database, if it exists. If not,
-# this method runs through the pipeline to
-# find a host for a new event, and returns all
-# data for the transient host.
-# input - TransientCoord, the coordinates of
-#         a transient being queried
-# output - A data frame of the host
-#          associated with the transient
-#          being queried, with PS1 information.
-#          If the supernova is currently in the
-#          database, return the database object.
-#          If not, complete the pipeline for
-#          host association and return the database
-#          object.
-#          If no host is found, return None
-
-# Returns all data for a transient host
-# currently in the database based on its
-# coordinates.
-# input - TransientCoord, the coordinates of
-#         a new transient being queried
-# output - A data frame of the host
-#          associated with the transient
-#          being queried, with PS1 information.
-#          If the supernova is currently in the
-#          database, return the database object.
-#          If not found, return None
 def getDBHostFromTransientCoords(transientCoords, GHOSTpath=''):
+    """Gets the host associated with a supernova in
+       the GHOST database by the supernova's position, if it exists.
+
+    Parameters
+    ----------
+    transientCoords : array-like
+        A list of astropy SkyCoord coordinates of transients.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    Returns
+    -------
+    host_DF : pandas DataFrame
+        The PS1 objects associated with the queried transients in GHOST.
+    notFound : array-like
+        A list of the coordinates of transients not found in the database.
+
+    """
     fullTable = fullData(GHOSTpath)
     notFound = []
     host_DF = None
     hostList = []
 
     #a little wrapper so that this function can take lists of coords in addition to one coord
     for transientCoord in transientCoords:
@@ -203,63 +221,71 @@
         sep = np.array(transientCoord.separation(c2).arcsec)
         if np.nanmin(sep) <= 1:
             host_idx = np.where(sep == np.nanmin(sep))[0][0]
             host = smallTable.iloc[[host_idx]]
             hostList.append(host)
         else:
             notFound.append(transientCoord)
-        #    print("Sorry, that supernova was not found in our database! The closest supernova is %.2f arcsec away.\n" %np.nanmin(sep))
     if len(hostList) > 0:
         host_DF = pd.concat(hostList, ignore_index=True)
     return host_DF, notFound
 
-# Returns all data for transient host,
-# based on supernova name
-# input - TransientCoord, the coordinates of
-#         a new transient being queried
-# output - A data frame of the host
-#          associated with the transient
-#          being queried, with PS1 information.
-#          If the supernova is currently in the
-#          database, return the database object.
-#          If no host is found, return None
-def getDBHostFromTransientName(SNNames, GHOSTpath=''):
+def getDBHostFromTransientName(transientNames, GHOSTpath=''):
+    """Gets the host associated with a supernova in
+       the GHOST database by the supernova's name, if it exists.
+
+    Parameters
+    ----------
+    transientNames : array-like
+        A list of transient names.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    Returns
+    -------
+    host_DF : pandas DataFrame
+        The PS1 objects associated with the queried transients in GHOST.
+    notFound : array-like
+        A list of the coordinates of transients not found in the database.
+
+    """
     fullTable = fullData(GHOSTpath)
     allHosts = []
     notFound = []
     host_DF = None
-#    if isinstance(SNName, list) or isinstance(SNName, np.ndarray):
-#        SNNames = SNName
-#    else:
-#        SNNames = np.array([SNname])
-    for SNName in SNNames:
-        SNName = re.sub(r"\s+", "", str(SNName))
+    for transientName in transientNames:
+        transientName = re.sub(r"\s+", "", str(transientName))
         host = None
-        possibleNames = [SNName, SNName.upper(), SNName.lower(), "SN"+SNName]
+        possibleNames = [transientName, transientName.upper(), transientName.lower(), "SN"+transientName]
         for name in possibleNames:
             if len(fullTable[fullTable['TransientName'] == name])>0:
                 host = fullTable[fullTable['TransientName'] == name]
                 allHosts.append(host)
                 break
         if host is None:
-            notFound.append(SNName)
+            notFound.append(transientName)
     if len(allHosts) > 0:
         host_DF = pd.concat(allHosts, ignore_index=True)
     return host_DF, notFound
 
-# Returns all data for transient and host,
-# based on host name
-# input - hostName
-# output - A data frame of the host
-#          associated with the transient
-#          being queried, with PS1 information.
-#          If the supernova is currently in the
-#          database, return the database object.
-#          If no host is found, return None
 def getHostFromHostName(hostNames, GHOSTpath=''):
+    """Gets hosts in the GHOST database by name.
+
+    Parameters
+    ----------
+    hostNames : array-like
+        A list of host galaxy names.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    Returns
+    -------
+    host : pandas DataFrame
+        The host galaxies found in GHOST.
+    """
     fullTable = fullData(GHOSTpath)
     possibleNames = []
 
     for name in hostNames:
         possibleNames.append(name)
         possibleNames.append(name.upper())
         possibleNames.append(re.sub(r"\s+", "", str(name)))
@@ -267,14 +293,29 @@
 
     host = fullTable[fullTable['NED_name'].isin(possibleNames)]
     if host is None:
         print("Sorry, no hosts were found in our database!\n")
     return host
 
 def getHostFromHostCoords(hostCoords, GHOSTpath=''):
+    """Gets hosts in the GHOST database by coordinates.
+
+    Parameters
+    ----------
+    hostCoords : array-like
+        A list of astropy SkyCoord coordinates of host galaxies.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    Returns
+    -------
+    host : pandas DataFrame
+        The subset of discovered hosts.
+
+    """
     fullTable = fullData(GHOSTpath)
     c2 = SkyCoord(fullTable['raMean']*u.deg, fullTable['decMean']*u.deg, frame='icrs')
     host = []
     for hostCoord in hostCoords:
         sep = np.array(hostCoord.separation(c2).arcsec)
         if np.nanmin(sep) <= 1:
             host_idx = np.where(sep == np.nanmin(sep))[0][0]
@@ -282,23 +323,25 @@
 
     if len(host) < 1:
         print("Sorry, No hosts found in our database!\n")
     else:
         host = pd.concat(host, ignore_index=True)
     return host
 
-# Returns basic statistics for transient,
-# based on a query of the coordinates of
-# its host
-# inputs - the position of the host
-# outputs - A printout of name,
-#           discovery year and discovery mag
-#           for all transients associated
-#           with a host at that coordinates
 def getTransientStatsFromHostCoords(hostCoord):
+    """Prints basic statistics for transient,
+       based on a query of the coordinates of
+       its host.
+
+    Parameters
+    ----------
+    hostCoord : Astropy SkyCoord Object
+        The position of the host galaxy.
+
+    """
     host = getHostFromHostCoords(hostCoord)
     i = 0
     if len(host) > 0:
         print("Found info for host %s.\n"%host['NED_name'].values[0])
         print("Associated supernovae: ")
         for SN in np.array(host['TransientName'].values):
             SN_frame = host.loc[host['TransientName'] == SN]
@@ -306,53 +349,69 @@
             print("RA, DEC (J2000): %f, %f"%(SN_frame['TransientRA'].values[0], SN_frame['TransientDEC'].values[0]))
             print("Redshift: %f"%SN_frame['TransientRedshift'].values[0])
             print("Discovery Date: %s"%SN_frame['TransientDiscoveryDate'].values[0].split(" ")[0])
             print("Discovery Mag: %.2f"%SN_frame['TransientDiscoveryMag'].values[0])
             i+= 1
     return
 
-# Returns basic statistics for transient,
-# based on a query of the coordinates of
-# its host
-# inputs - the position of the host
-# outputs - A printout of name,
-#           discovery year and discovery mag
-#           for all transients associated
-#           with a host at that coordinates
 def getTransientStatsFromHostName(hostName):
+    """Returns basic statistics for transient,
+       based on a query of the name of
+       its host.
+
+    Parameters
+    ----------
+    hostName : str
+        The name of the host galaxy.
+
+    """
     host = getHostFromHostName(hostName)
     hostCoord = SkyCoord(np.unique(host['raMean'])*u.deg, np.unique(host['decMean'])*u.deg, frame='icrs')
     getTransientStatsFromHostCoords(hostCoord)
     return
 
-# Returns basic statistics for the most likely
-# host of a previously identified transient, using
-# the pipeline outlined above.
-# inputs - the coordinates of the transient to search
 def getHostStatsFromTransientCoords(transientCoordsList, GHOSTpath=''):
+    """ Returns basic statistics for the most likely
+        host of a previously identified transient, from the
+        transient's coordinates.
+
+    Parameters
+    ----------
+    transientCoordsList : array-like
+        A list of astropy SkyCoord coordinates of transients.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    """
     fullTable = fullData(GHOSTpath)
     names = []
     for transientCoords in transientCoordsList:
         c2 = SkyCoord(fullTable['TransientRA']*u.deg, fullTable['TransientDEC']*u.deg, frame='icrs')
         sep = np.array(transientCoords.separation(c2).arcsec)
         host = None
         if np.nanmin(sep) <= 1:
             host_idx = np.where(sep == np.nanmin(sep))[0][0]
             host = fullTable.iloc[[host_idx]]
             names.append(host['TransientName'].values[0])
     getHostStatsFromTransientName(names)
 
-# Returns basic statistics for the most likely
-# host of a previously identified transient, using
-# the pipeline outlined above.
-# inputs - the coordinates of the transient to search
-def getHostStatsFromTransientName(SNName, GHOSTpath=''):
-    SNName = np.array(SNName)
+def getHostStatsFromTransientName(transientName, GHOSTpath=''):
+    """Returns basic statistics for the most likely host of a previously identified transient.
+
+    Parameters
+    ----------
+    transientName : str
+        Array of transient names.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    """
+    transientName = np.array(transientName)
     fullTable = fullData(GHOSTpath)
-    host, notFound = getDBHostFromTransientName(SNName, GHOSTpath)
+    host, notFound = getDBHostFromTransientName(transientName, GHOSTpath)
     if host is not None:
         for idx, row in host.iterrows():
             if np.unique(row['NED_name']) != "":
                 print("Found host %s.\n"%row['NED_name'])
             else:
                 print("Found host with PS1 ID %s"%row['objID'])
             print("RA, DEC (J2000): %f, %f"%(row['raMean'], row['decMean']))
@@ -368,20 +427,32 @@
                 tempHost = fullTable[fullTable['objID'] == row['objID']]
             for SN in np.array(tempHost['TransientName'].values):
                 print(SN)
     else:
         print("No host info found!")
     return
 
-# Returns a postage stamp of the most likely
-# host in one of the PS1 bands - g,r,i,z,y - as a
-# fits file with radius rad, and plots the image.
-# inputs
-# outputs
-def getHostImage(transientName='', band="grizy", rad=60, save=0, GHOSTpath=''):
+def getHostImage(transientName='', band="grizy", rad=60, save=False, GHOSTpath=''):
+    """Returns a postage stamp of the most likely host in one of the PS1 bands - g,r,i,z,y - as a
+       fits file with radius rad, and plots the image.
+
+    Parameters
+    ----------
+    transientName : str
+        Name of queried transient.
+    band : str
+        Band for host-galaxy image.
+    rad : float
+        Size of the image, in arcsec.
+    save : bool
+        If True, save host image.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    """
     if transientName == '':
         print("Error! Please enter a supernova!\n")
         return
     fullTable = fullData(GHOSTpath)
     host, notFound = getDBHostFromTransientName(transientName, GHOSTpath)
     if host is not None:
         host.reset_index(drop=True, inplace=True)
@@ -398,168 +469,268 @@
         plt.imshow(img)
         if save:
             img.save("%s.png" % fn_save)
         return
     else:
         print("Transient host not found!")
 
-# description
-# inputs
-# outputs
-def getTransientSpectra(path, SNname):#
-    SNname = remove_prefix(SNname, 'SN')
-    files = glob.glob(path+"*%s*"%SNname)
+def getTransientSpectra(path, transientName):
+    """Retrieves all saved spectra associated with a transient.
+
+    Parameters
+    ----------
+    path : str
+        Filepath to spectra.
+    transientName : str
+        Name of transient to query.
+
+    Returns
+    -------
+    specFiles : list of Pandas DataFrames
+        Saved spectra.
+
+    """
+    transientName = remove_prefix(transientName, 'SN')
+    files = glob.glob(path+"*%s*"%transientName)
     specFiles = []
     if len(files) > 0:
         for file in files:
             if remove_prefix(file, path).startswith("osc_"):
                 spectra = pd.read_csv(file, header=None, names=['Wave(A)', 'I', 'Ierr'])
             else:
                 spectra = pd.read_csv(file, delim_whitespace=True, header=None, names=['x', 'y', 'z'])
-            #spectra = spectra.astype('float')
             specFiles.append(spectra)
     else:
         print("Sorry! No spectra found.")
     return specFiles
 
-# description
-# inputs
-# outputs
-def getHostSpectra(SNname, path):#
-    SNname = remove_prefix(SNname, 'SN')
-    files = glob.glob(path+"*%s_hostSpectra.csv*"%SNname)
+def getHostSpectra(transientName, path):
+    """Retrieves all saved spectra associated with a host galaxy.
+
+    Parameters
+    ----------
+    path : str
+        Filepath to spectra.
+    transientName : str
+        Name of transient to query.
+
+    Returns
+    -------
+    specFiles : list of Pandas DataFrames
+        Saved spectra.
+
+    """
+    transientName = remove_prefix(transientName, 'SN')
+    files = glob.glob(path+"*%s_hostSpectra.csv*"%transientName)
     specFiles = []
     if len(files) > 0:
         for file in files:
             spectra = pd.read_csv(file)
-            #spectra = spectra.astype('float')
             specFiles.append(spectra)
     else:
         print("Sorry! No spectra found.")
     return specFiles
 
-# A cone search for all transient-host pairs
-# within a certain radius, returned as a pandas dataframe
-# inputs location, in astropy coordinates, and radius in arcsec
-# outputs the data frame of all nearby pairs
 def coneSearchPairs(coord, radius, GHOSTpath=''):
+    """A cone search for all transient-host pairs within a certain radius, returned as a pandas dataframe.
+
+    Parameters
+    ----------
+    coord : Astropy SkyCoord
+        Position for cone search.
+    radius : float
+        Search radius, in arcsec.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    Returns
+    -------
+    hosts : Pandas DataFrame
+        GHOST galaxies within search radius.
+
+    """
     fullTable = fullData(GHOSTpath)
     c2 = SkyCoord(fullTable['TransientRA']*u.deg, fullTable['TransientDEC']*u.deg, frame='icrs')
     sep = np.array(coord.separation(c2).arcsec)
     hosts = None
     if np.nanmin(sep) < radius:
         host_idx = np.where(sep < radius)[0]
         hosts = fullTable.iloc[host_idx]
-        #hosts = pd.concat(hosts)
     return hosts
 
-# Returns the full table of data
-# inputs: none
-# outputs: the full GHOST database
 def fullData(GHOSTpath=''):
+    """Returns the full GHOST database.
+
+    Parameters
+    ----------
+    GHOSTpath : str
+        The path to the saved GHOST database.
+
+    Returns
+    -------
+    fullTable : Pandas DataFrame
+        GHOST database.
+
+    """
     if not GHOSTpath:
         GHOSTpath = os.getenv('GHOST_PATH')
         if not GHOSTpath:
             try:
                 GHOSTpath = astro_ghost.__file__
                 GHOSTpath = GHOSTpath.split("/")[:-1]
                 GHOSTpath = "/".join(GHOSTpath)
             except:
                 print("Error! I don't know where you installed GHOST -- set GHOST_PATH as an environmental variable or pass in the GHOSTpath parameter.")
     fullTable = pd.read_csv(GHOSTpath+"/database/GHOST.csv")
     return fullTable
 
-# The wrapper function for the
-# host association pipeline.
-# inputs: the location of the supernova
-#         as an astropy SkyCoord object
-# output: A pandas dataframe of
-#         the most likely host in PS1,
-#         with stats provided at
-#         printout
-def getTransientHosts(snName=[''], snCoord=[''], snClass=[''], verbose=0, starcut='normal', ascentMatch=False, px=800, savepath='./', GHOSTpath='', redo_search=True):
+def getTransientHosts(transientName=[''], snCoord=[''], snClass=[''], verbose=False, starcut='normal', ascentMatch=False, px=800, savepath='./', GHOSTpath='', redo_search=True):
+    """The wrapper function for the main host association pipeline. The function first
+       searches the pre-existing GHOST database by transient name, then by transient coordinates, and finally
+       associates the remaining transients not found.
+
+    Parameters
+    ----------
+    transientName : array-like
+        List of transients to associate.
+    snCoord : array-like
+        List of astropy SkyCoord transient positions.
+    snClass : array-like
+        List of transient classifications (if they exist).
+    verbose : bool
+        If True, print logging information.
+    starcut : str
+        Strings corresponding to the classification thresholds required to classify a star as such.
+        Options are 'gentle' (P>0.8), normal (P>0.5), and aggressive (P>0.3).
+    ascentMatch : bool
+        If True, run the gradient ascent algorithm for the transients not matched with the
+        Directional Light Radius algorithm.
+    px : int
+        Size of the image used in gradient ascent (ignored if ascentMatch=False).
+    savepath : str
+        Filepath where dataframe of associated hosts will be saved.
+    GHOSTpath : str
+        The path to the saved GHOST database.
+    redo_search : bool
+        If True, redo the search with 150'' cone search radius if hosts were not
+        found for any of the queried transients.
+
+    Returns
+    -------
+    hostDB : Pandas DataFrame
+        Final dataframe of associated transients and host galaxies.
+
+    """
 
     #if no names were passed in, add placeholder names for each transient in the search
-    if snName == ['']:
-        snName = []
+    if transientName == ['']:
+        transientName = []
         print("No transient names listed, adding placeholder names...")
         for i in np.arange(len(snCoord)):
-            snName.append("Transient_%i" % (i+1))
+            transientName.append("Transient_%i" % (i+1))
     hostDB = None
     tempHost1 = tempHost2 = tempHost3 = None
     found_by_name = found_by_coord = found_by_manual = 0
     if not isinstance(snCoord, list) and not isinstance(snCoord, np.ndarray):
         snCoord = [snCoord]
-        snName = [snName]
+        transientName = [transientName]
         snClass = [snClass]
-    if len(snClass) != len(snName):
-        snClass = ['']*len(snName)
+    if len(snClass) != len(transientName):
+        snClass = ['']*len(transientName)
 
-    snName = [x.replace(" ", "") for x in snName]
-    df_transients = pd.DataFrame({'Name':np.array(snName), 'snCoord':np.array(snCoord), 'snClass':np.array(snClass)})
+    transientName = [x.replace(" ", "") for x in transientName]
+    df_transients = pd.DataFrame({'Name':np.array(transientName), 'snCoord':np.array(snCoord), 'snClass':np.array(snClass)})
 
-    tempHost1, notFoundNames = getDBHostFromTransientName(snName, GHOSTpath)
-    found_by_name = len(snName) - len(notFoundNames)
+    tempHost1, notFoundNames = getDBHostFromTransientName(transientName, GHOSTpath)
+    found_by_name = len(transientName) - len(notFoundNames)
 
     if tempHost1 is None or len(notFoundNames) > 0:
         if verbose:
             print("%i transients not found in GHOST by name, trying a coordinate search..."%len(notFoundNames))
 
         df_transients_remaining = df_transients[df_transients['Name'].isin(notFoundNames)]
 
         snCoord_remaining =  df_transients_remaining['snCoord'].values
 
         tempHost2, notFoundCoords = getDBHostFromTransientCoords(snCoord_remaining, GHOSTpath);
-        found_by_coord = len(snName) - len(notFoundCoords) - found_by_name
+        found_by_coord = len(transientName) - len(notFoundCoords) - found_by_name
         if tempHost2 is None or len(notFoundCoords) > 0:
             if verbose:
                 print("%i transients not found in GHOST by name or coordinates, manually associating..."% len(notFoundCoords))
 
             df_transients_remaining = df_transients_remaining[df_transients_remaining['snCoord'].isin(notFoundCoords)]
 
-            snName_remaining =  df_transients_remaining['Name'].values
+            transientName_remaining =  df_transients_remaining['Name'].values
             snCoord_remaining = df_transients_remaining['snCoord'].values
             snClass_remaining = df_transients_remaining['snClass'].values
 
-            tempHost3 = findNewHosts(snName_remaining, snCoord_remaining, snClass_remaining, verbose, starcut, ascentMatch, px, savepath)
-            
-            if (len(snName_remaining) > 0) and (len(tempHost3)==0) and (redo_search):
-                 #bump up the search radius to 150 arcsec for reallyyy low-redshift hosts...
-                 if verbose: 
+            tempHost3 = findNewHosts(transientName_remaining, snCoord_remaining, snClass_remaining, verbose, starcut, ascentMatch, px, savepath)
+
+            if (len(transientName_remaining) > 0) and (len(tempHost3)==0) and (redo_search):
+                 #bump up the search radius to 150 arcsec for extremely low-redshift hosts...
+                 if verbose:
                      print("Couldn't find any hosts! Trying again with a search radius of 150''.")
-                 tempHost3 = findNewHosts(snName_remaining, snCoord_remaining, snClass_remaining, verbose, starcut, ascentMatch, px, savepath, 150)
+                 tempHost3 = findNewHosts(transientName_remaining, snCoord_remaining, snClass_remaining, verbose, starcut, ascentMatch, px, savepath, 150)
             found_by_manual = len(tempHost3)
     hostDB = pd.concat([tempHost1, tempHost2, tempHost3], ignore_index=True)
     hostDB.replace(-999.0, np.nan, inplace=True)
     if verbose:
         print("%i transients found by name, %i transients found by coordinates, %i transients manually associated."% (found_by_name, found_by_coord, found_by_manual))
     return hostDB
 
-# The wrapper function for the
-# host association pipeline.
 # inputs: the location of the supernova
 #         as an astropy SkyCoord object
 # output: A pandas dataframe of
 #         the most likely host in PS1,
 #         with stats provided at
 #         printout
-def findNewHosts(snName, snCoord, snClass, verbose=0, starcut='gentle', ascentMatch=False, px=800, savepath='./', rad=60):
-    if isinstance(snName, str):
-        snName = snName.replace(" ", "")
+def findNewHosts(transientName, snCoord, snClass, verbose=False, starcut='gentle', ascentMatch=False, px=800, savepath='./', rad=60):
+    """Associates hosts of transients not in the GHOST database.
+
+    Parameters
+    ----------
+    transientName : array-like
+        List of transients to associate.
+    snCoord : array-like
+        List of astropy SkyCoord transient positions.
+    snClass : array-like
+        List of transient classifications (if they exist).
+    verbose : bool
+        If True, print logging information.
+    starcut : str
+        Strings corresponding to the classification thresholds required to classify a star as such.
+        Options are 'gentle' (P>0.8), normal (P>0.5), and aggressive (P>0.3).
+    ascentMatch : bool
+        If True, run the gradient ascent algorithm for the transients not matched with the
+        Directional Light Radius algorithm.
+    px : int
+        Size of the image used in gradient ascent (ignored if ascentMatch=False).
+    savepath : str
+        Filepath where dataframe of associated hosts will be saved.
+    rad : float
+        The search radius around each transient position, in arcseconds.
+
+    Returns
+    -------
+    host_df : Pandas DataFrame
+        Final dataframe of associated transients and host galaxies.
+
+    """
+    if isinstance(transientName, str):
+        transientName = transientName.replace(" ", "")
         snRA = snCoord.ra.degree
         snDEC = snCoord.dec.degree
-    elif isinstance(snName, list) or isinstance(snName, np.ndarray):
-        snName = [x.replace(" ", "") for x in snName]
+    elif isinstance(transientName, list) or isinstance(transientName, np.ndarray):
+        transientName = [x.replace(" ", "") for x in transientName]
         snRA = [x.ra.degree for x in snCoord]
         snDEC = [x.dec.degree for x in snCoord]
     else:
         print("Error! Please pass in your transient name as either a string or a list/array of strings.\n")
-        #return None
 
-    snName_arr = np.array(snName)
+    transientName_arr = np.array(transientName)
     snRA_arr = np.array(snRA)
     snDEC_arr = np.array(snDEC)
     snClass_arr = np.array(snClass)
 
     dateStr = str(datetime.today()).replace("-", '').replace(".", '').replace(":", "").replace(" ", '')
 
     fn_Host = "SNe_TNS_%s_PS1Hosts_%iarcsec.csv" % (dateStr, rad)
@@ -567,34 +738,30 @@
     fn_Dict = fn_Host[:-4] + ".p"
     dir_name = fn_SN[:-4]
     if not os.path.exists(savepath):
         os.mkdir(savepath)
         os.chmod(savepath, 0o777)
     os.makedirs(savepath + dir_name)
     path = savepath+dir_name+'/'
-    #create temp dataframe with RA and DEC corresponding to the transient
 
-    snDF = pd.DataFrame({'Name':snName_arr, 'RA':snRA_arr, 'DEC':snDEC_arr, 'HostName':['']*len(snDEC_arr), 'Obj. Type':snClass_arr})
+    #create temp dataframe with RA and DEC corresponding to the transient
+    snDF = pd.DataFrame({'Name':transientName_arr, 'RA':snRA_arr, 'DEC':snDEC_arr, 'HostName':['']*len(snDEC_arr), 'Obj. Type':snClass_arr})
     snDF.to_csv(path+fn_SN, index=False)
 
     #begin doing the heavy lifting to associate transients with hosts
     host_DF = get_hosts(path, fn_SN, fn_Host, rad)
-    #halfLightSizes = getDR2_halfLightSizes(snRA_arr, snDEC_arr, rad)
     halfLightSizes = getDR2_petrosianSizes(snRA_arr, snDEC_arr, rad)
     host_DF_new = host_DF.merge(halfLightSizes, on='objID')
     host_DF = host_DF_new if not halfLightSizes.empty else host_DF
-    #host_DF = host_DF.merge(halfLightSizes, on='objID')
 
     if len(host_DF) < 1:
         print("ERROR: Found no hosts in cone search during manual association!")
         return None
 
-    #turn off all cuts now for debugging
     cuts = ["n", "quality", "coords", "duplicate"]
-    #cuts = []
 
     transient_dict =[]
     # this bit of trickery is required to combine northern-hemisphere and
     # southern-hemisphere source dictionaries
     f = open(path+'/dictionaries/'+fn_Dict, "rb")
     try:
         while True:
@@ -622,15 +789,14 @@
 
     hostFrac = fracWithHosts(cut_dict)*100
     if verbose:
         print("Associated fraction after quality cuts: %.2f%%."%hostFrac)
 
     #automatically add to host association for gradient ascent
     lost = np.array([k for k, v in cut_dict.items() if len(v) <1])
-    #lost = set(snName_arr) - set(cut_dict.keys())
 
     host_DF_north = getColors(host_DF_north)
     host_DF_north = removePS1Duplicates(host_DF_north)
     host_DF_north = calc_7DCD(host_DF_north)
 
     host_DF = pd.concat([host_DF_north, host_DF_south], ignore_index=True)
     host_DF = getSimbadInfo(host_DF)
@@ -653,75 +819,65 @@
     #plotLocus(host_gals_DF, color=1, save=1, type="Gals", timestamp=dateStr)
     #plotLocus(stars_DF, color=1, save=1, type="Stars", timestamp=dateStr)
 
     host_dict_nospace = {k.replace(' ', ''): v for k, v in cut_dict.items()}
 
     fn = "DLR.txt"
     transients = pd.read_csv(path+fn_SN)
-#    clean_dict(host_dict_nospace, host_gals_DF, [])
-#    fracWithHosts(host_dict_nospace)
-#    print(len(host_gals_DF[host_gals_DF['decMean'] < -30]))
 
     with open(path+"/dictionaries/checkpoint_preDLR.p", 'wb') as fp:
-           #pickle.dump(host_dict_nospace, fp, protocol=pickle.HIGHEST_PROTOCOL)
            dump(host_dict_nospace, fp)
 
-    host_DF, host_dict_nospace_postDLR, noHosts, GD_SN = chooseByDLR(path, host_gals_DF, transients, fn, host_dict_nospace, host_dict_nospace, todo="r")
+    host_DF, host_dict_nospace_postDLR, noHosts, GD_SN = chooseByDLR(path, host_gals_DF, transients, fn, host_dict_nospace, todo="r")
 
     #last-ditch effort -- for the ones with no found host, just pick the nearest NED galaxy.
     for transient in noHosts:
           tempDF = host_gals_DF[host_gals_DF['objID'].isin(desperate_dict[transient])]
           tempDF_gals = tempDF[tempDF['NED_type'].isin(['G', 'PofG', 'GPair', 'GGroup', 'GClstr'])].reset_index()
           if len(tempDF_gals) < 1:
              continue
           transientRA = transients.loc[transients['Name'] == transient, 'RA'].values[0]
           transientDEC = transients.loc[transients['Name'] == transient, 'DEC'].values[0]
           transientCoord = SkyCoord(transientRA*u.deg, transientDEC*u.deg, frame='icrs')
           tempHostCoords = SkyCoord(tempDF_gals['raMean'].values*u.deg, tempDF_gals['decMean'].values*u.deg, frame='icrs')
           sep = transientCoord.separation(tempHostCoords)
-          desperateMatch = tempDF_gals.iloc[[np.argmin(sep.arcsec)]]  
+          desperateMatch = tempDF_gals.iloc[[np.argmin(sep.arcsec)]]
           host_DF = pd.concat([host_DF, desperateMatch], ignore_index=True)
           host_dict_nospace_postDLR[transient] = desperateMatch['objID'].values[0]
           if verbose:
                print("Desperate match found for %s, %.2f arcsec away." % (transient, sep[np.argmin(sep.arcsec)].arcsec))
 
     if len(noHosts) > 0:
         with open(path+"/dictionaries/noHosts_fromDLR.p", 'wb') as fp:
-            #pickle.dump(noHosts, fp)
             dump(noHosts, fp)
 
     if len(GD_SN) > 0:
         with open(path+"/dictionaries/badInfo_fromDLR.p", 'wb') as fp:
-            #pickle.dump(GD_SN, fp)
              dump(GD_SN, fp)
 
     #gradient ascent algorithm for the SNe that didn't pass this stage
     SN_toReassociate = np.concatenate([np.array(noHosts), np.array(GD_SN), np.array(list(lost))])
-    #SN_toReassociate = np.concatenate([np.array(noHosts), np.array(list(lost))])
-    #SN_toReassociate = np.array(SN_toReassociate)
 
     if (len(SN_toReassociate) > 0) and (ascentMatch):
         if verbose:
             print("%i transients with no host found with DLR, %i transients with bad host data with DLR." %(len(noHosts), len(GD_SN)))
             print("Running gradient ascent for %i remaining transients."%len(SN_toReassociate))
             print("See GradientAscent.txt for more information.")
 
         fn_GD= path+'/GradientAscent.txt'
 
         host_dict_nospace_postDLR_GD, host_DF, unchanged = gradientAscent(path, transient_dict,  host_dict_nospace_postDLR, SN_toReassociate, host_DF, transients, fn_GD, plot=verbose, px=px)
 
         with open(path+"/dictionaries/gals_postGD.p", 'wb') as fp:
-            #pickle.dump(host_dict_nospace_postDLR_GD, fp, protocol=pickle.HIGHEST_PROTOCOL)
             dump(host_dict_nospace_postDLR_GD, fp)
 
         if verbose:
             print("Hosts not found for %i transients in gradient ascent. Storing names in GD_unchanged.txt" %(len(unchanged)))
 
         with open(path+"/GD_unchanged.txt", 'wb') as fp:
-            #pickle.dump(unchanged, fp)
             dump(unchanged, fp)
 
         hostFrac = fracWithHosts(host_dict_nospace_postDLR_GD)*100
 
         if verbose:
             print("Associated fraction after gradient ascent: %.2f%%."%hostFrac)
 
@@ -729,15 +885,14 @@
 
     else:
         final_dict = host_dict_nospace_postDLR.copy()
 
     host_DF = build_ML_df(final_dict, host_DF, transients)
 
     with open(path+"/dictionaries/" + "Final_Dictionary.p", 'wb') as fp:
-           #pickle.dump(final_dict, fp, protocol=pickle.HIGHEST_PROTOCOL)
            dump(final_dict, fp)
 
     #a few final cleaning steps
     host_DF.drop_duplicates(subset=['TransientName'], inplace=True)
     host_DF = host_DF[host_DF['TransientName'] != ""]
     host_DF.reset_index(inplace=True, drop=True)
     host_DF['TransientName'] = [x.replace(" ", "") for x in host_DF['TransientName']]
@@ -745,21 +900,17 @@
     matchFrac = len(host_DF)/len(transients)*100
     print("Found matches for %.1f%% of events."%matchFrac)
     if verbose:
         print("Saving table of hosts to %s."%(path+"tables/FinalAssociationTable.csv"))
 
     host_DF.to_csv(path+"FinalAssociationTable.csv", index=False)
 
-    #hSpecPath = path+"/hostSpectra/"
-    #tSpecPath = path+"/SNspectra/"
-    #psPath = path+"/hostPostageStamps/"
     tablePath = path+"/tables/"
     printoutPath = path+'/printouts/'
 
-    #paths = [hSpecPath, tSpecPath, psPath, tablePath, printoutPath]
     paths = [tablePath, printoutPath]
 
     for tempPath in paths:
         if not os.path.exists(tempPath):
             os.mkdir(tempPath)
 
     #move tables to the tables directory, and printouts to the printouts directory
@@ -775,8 +926,8 @@
             fn = remove_prefix(t, path)
             os.rename(t, tablePath+fn)
     #remove if there's an extra index column
     try:
         del host_DF['index']
     except:
         pass
-    return(host_DF)
+    return host_DF
```

### Comparing `astro_ghost-0.2.3/astro_ghost/gradientAscent.py` & `astro_ghost-0.2.4/astro_ghost/gradientAscent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,122 @@
 import os
+import cv2
+import time
+import pandas as pd
+import numpy as np
 from astro_ghost.PS1QueryFunctions import *
 from astro_ghost.NEDQueryFunctions import getNEDInfo
-from datetime import datetime
 from astropy import units as u
-from astropy.coordinates import SkyCoord
-import pandas as pd
-import numpy as np
-import pickle
-from astropy.io import ascii
-from collections import Counter
-import scipy
-from scipy import ndimage
-import numpy as np
-from matplotlib import pyplot as plt
-from astropy.table import Table
-from matplotlib.colors import LogNorm
+from astropy.io import fits, ascii
+from astropy.utils.exceptions import AstropyUserWarning,AstropyWarning
+from astropy.wcs import WCS
 from astropy.utils.data import get_pkg_data_filename
-#from astro_ghost import DLR as dlr
-from photutils import Background2D
-import numpy.ma as ma
-import cv2
-import time
-from astropy.io import fits
-import warnings
-from astropy.utils.exceptions import AstropyUserWarning
-from astropy.utils.exceptions import AstropyWarning
+from matplotlib import pyplot as plt
 from matplotlib import colors
-from scipy import interpolate
-from astropy.wcs import WCS
-from astropy.stats import mad_std
-from astropy.stats import sigma_clipped_stats
-from astropy.visualization.mpl_normalize import ImageNormalize
-from photutils import CircularAperture
-from astropy.visualization import SqrtStretch
-from photutils import DAOStarFinder
-from photutils import MedianBackground, MeanBackground
-from astropy.stats import SigmaClip
-import gc
+from photutils import Background2D
+from astropy.stats import sigma_clipped_stats, SigmaClip
+from photutils import CircularAperture, DAOStarFinder, MedianBackground, MeanBackground
 from joblib import dump, load
+import gc
+import warnings
 
-############# functions ####################################
 def updateStep(px, gradx, grady, step, point, size):
+    """ Determine direction of movement by image gradients.
+
+    Parameters
+    ----------
+    px : int
+        The maximum size of the image, in pixels.
+    gradx : float
+        The horizontal gradient of the image.
+    grady : float
+        The vertical gradient of the image.
+    step : float
+        The step size for updating the position.
+    point : array-like
+        The current position.
+    size : str
+        The predicted size of the true host. Can be "small", "medium", or "large".
+
+    Returns
+    -------
+    newPoint : array-like
+        The updated position.
+
+    """
     max_x = px
     max_y =  px
     grad = np.array([gradx[point[0], point[1]], grady[point[0], point[1]]])
-    #make sure we move at least one unit in grid spacing - so the grad must have len 1
-#    if grad[0] + grad[1] > 0:
     ds = step/np.sqrt(grad[0]**2 + grad[1]**2)
     ds = np.nanmin([ds, step])
-#    else:
-#        ds = step
-
     newPoint = [point[0] + ds*grad[0], point[1] + ds*grad[1]]
     newPoint = [int(newPoint[0]), int(newPoint[1])] #round to nearest index
     if (newPoint[0] >= max_x) or (newPoint[1] >= max_y) or (newPoint[0] < 0) or (newPoint[1] < 0):
         #if we're going to go out of bounds, don't move
         return point
-    elif ((newPoint == point) and (size == 'large')): #if we're stuck, perturb one pixel in a random direction:
+    #if we're stuck, perturb one pixel in a random direction:
+    elif ((newPoint == point) and (size == 'large')):
         a = np.random.choice([-1, 0, 1], 2)#
         newPoint = [newPoint[0] + a[0], newPoint[1] + a[1]]
     return newPoint
 
 
 def dist(p1, p2):
+    """Measure the euclidean distance between two points.
+
+    Parameters
+    ----------
+    p1 : array-like
+        The first point.
+    p2 : array-like
+        The second point.
+
+    Returns
+    -------
+    float
+        The euclidean distance.
+
+    """
     return np.sqrt((p1[0] - p2[0])**2 + (p1[1] - p2[1])**2)
 
-def plot_DLR_vectors_GD(size, path, transient, transient_df, host_dict_candidates, host_dict_final, host_df, R_dict, ra_dict, df = "TNS", dual_axes=0, scale=1, postCut=0):
+def plot_DLR_vectors_GD(size, path, transient, transient_df, host_dict_candidates, host_dict_final, host_df, R_dict, ra_dict, scale=1):
+    """Plots the DLR vectors associated with each candidate host in a transient's field.
+
+    Parameters
+    ----------
+    size : int
+        Size of the plotted image, in pixels.
+    path : str
+        Filepath where image will be saved.
+    transient : str
+        Name of transient.
+    transient_df : Pandas DataFrame
+        Description of parameter `transient_df`.
+    host_dict_candidates : dictionary
+        key,value pairs of transient name, list of PS1 objIDs of
+        candidate hosts. Dictionary is before gradient ascent is run.
+    host_dict_final : dictionary
+        key,value pairs of transient name, list of PS1 objIDs of
+        candidate hosts. Dictionary is after gradient ascent is run.
+    host_df : Pandas DataFrame
+        List of all candidate hosts in the field (before gradient ascent).
+    R_dict : dictionary
+        The r/DLR normalized distance metrics for all candidate hosts.
+    ra_dict : dictionary
+        The DLR values for all candidate hosts.
+    scale : float
+        An additional scale factor for the image size (to fully capture low-z hosts).
+
+    Returns
+    -------
+    ax_grads : figure axis
+        axes of the plotted image (to overlay a quiver map, or 2D field of gradient arrows).
+
+    """
     hostList = host_dict_candidates[str(transient)]
-    #os.chdir(path)
     if type(hostList) is np.ndarray:
         if len(hostList) > 1:
             chosen = host_dict_final[transient]
         else:
             chosen = hostList[0]
     else:
         chosen = hostList
@@ -87,33 +132,27 @@
     searchRA = transientRA
     searchDEC = transientDEC
 
     a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(searchRA, searchDEC, int(px*0.25), band), '.')
     if not a:
         get_PS1_Pic(searchRA, searchDEC, px, band)
         a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(searchRA, searchDEC, int(px*0.25), band), '.')
-    #a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(transientRA, transientDEC, int(px*0.25), band), '.')
-    #if not a:
-    #    get_PS1_Pic(transientRA, transientDEC, px, band)
-    #    a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(transientRA, transientDEC, int(px*0.25), band), '.')
     hdu = fits.open(a[0])[0]
     image_file = get_pkg_data_filename(a[0])
     image_data = fits.getdata(image_file, ext=0)
     wcs = WCS(hdu.header)
     fig = figure(num=None, figsize=(20,20), facecolor='w', edgecolor='k')
-    #ax = plt.subplot(projection=wcs)
     fig.add_axes(projection=wcs)
     axes_coords = [0, 0, 1, 1] # plotting full width and height
     ax = fig.add_axes(axes_coords, projection=wcs)
     axes_coords2 = [-0.045, -0.03, 1.06, 1.08]
     ax_grads = fig.add_axes(axes_coords2, projection=None)
     plt.axis('off')
     for host in hostList:
         hostDF = host_df[host_df['objID'] == host]
-
         band = choose_band_SNR(hostDF)
         XX = hostDF[band + 'momentXX'].values[0]
         YY = hostDF[band + 'momentYY'].values[0]
         XY = hostDF[band + 'momentXY'].values[0]
         U = np.float(XY)
         Q = np.float(XX) - np.float(YY)
         if (Q == 0):
@@ -135,42 +174,57 @@
         hostDLR = R_dict[host]
         c = '#666dc9'
         c2 = 'red'
         if (host == chosen):
             c = c2 = '#d308d0'
         hostDF['raMean'], hostDF['decMean']
         plot_ellipse(ax, px, hostDF, searchRA, searchDEC, c)
-        #plot_ellipse(ax, px, hostDF, transientRA, transientDEC, c)
 
         # in arcseconds
         dx = float(hostRA - transientRA)*3600
         dy = float(hostDEC - transientDEC)*3600
 
         dist = np.sqrt(dx**2 + dy**2)
         if hostDLR == 10000000000.0:
             hostDLR = 0.0
         else:
             hostDLR = dist/hostDLR
+
         #in arcseconds
         scale_factor = hostDLR/dist
 
         DLR_RA = float(hostRA) - dx*scale_factor/3600
         DLR_DEC = float(hostDEC) - dy*scale_factor/3600
 
         pointRA = [hostRA, DLR_RA]
         pointDEC = [hostDEC, DLR_DEC]
 
         ax.plot(pointRA, pointDEC, transform=ax.get_transform('fk5'), lw=6, color= c)
-#    ax.imshow(image_data, norm=colors.LogNorm(), cmap='gray_r')
     ax.imshow(image_data, norm=colors.PowerNorm(gamma = 0.5, vmin=1, vmax=1.e4), cmap='gray')
     plt.axis('off')
     return ax_grads
 
 
 def plot_ellipse(ax, px, s, ra, dec, color):
+    """Plots an ellipse on an image.
+
+    Parameters
+    ----------
+    ax : figure axis
+        Axis of figure for plotting.
+    px : int
+        Image size, in pixels.
+    s : Pandas DataFrame
+        PS1 source, with shape parameters (phi, r_a, and r_b)
+    ra, dec : float
+        Image position, in degrees.
+    color : str
+        Color of plotted ellipse.
+
+    """
     i=0
     size = px  #PS cutout image size, 240*sidelength in arcmin
     x0, y0 = ((ra-s['raMean'])*4*3600*np.cos(s['decMean']/180*np.pi)+(size/2)), (s['decMean']-dec)*4*3600+(size/2)
     i=i+1
 
     y, x = np.mgrid[0:size, 0:size]# 4 pixel for 1 arcsec for PS1, here image size is set to be 20"*20", depend on your cutout image size
     #make fitted image
@@ -254,23 +308,46 @@
 
         # don't forget to update iterator
         i += 1
 
     return u
 
 def get_clean_img(ra, dec, px, band):
+    """Takes PS1 images, removes bad pixels, and
+       estimates new pixel values through a 2D
+       interpolation.
+
+    Parameters
+    ----------
+    ra, dec : float
+        Image position, in degrees.
+    px : int
+        Image size, in pixels.
+    band : str
+        Passband of image.
+
+    Returns
+    -------
+    image_masked : 2D array
+        Image data, with bad pixels masked.
+    wcs : Astropy world coordinate system object
+        wcs of image fits file.
+    hdu : Fits header
+        header of image fits file.
+
+    """
     #first, mask the data
     if dec > -30:
         a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band), '.')
         if not a:
             get_PS1_Pic(0, ra, dec, px, band)
             a = find_all("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band), '.')
         b = find_all("PS1_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.25), band), '.')
         if not b:
-            get_PS1_mask(ra, dec, px, band)
+            get_PS1_type(ra, dec, px, band, 'stack.mask')
             b = find_all("PS1_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.25), band), '.')
         c = find_all("PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band), '.')
         if not c:
             get_PS1_type(ra, dec, px, band, 'stack.num')
             c = find_all("PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band), '.')
 
         image_data_mask = fits.open(b[0])[0].data
@@ -292,16 +369,16 @@
                             mask[i][j] = np.nan
                     elif len(str(int(bit[i][j]))) > 5:
                         if (tempBit[-6] == 1):
                             mask[i][j] = np.nan
 
         mask = ~np.isnan(image_data_mask)
         mask_num = image_data_num
-        image_masked = ma.masked_array(image_data, mask=mask)
-        image_masked_num = ma.masked_array(image_masked, mask=mask_num)
+        image_masked = np.ma.masked_array(image_data, mask=mask)
+        image_masked_num = np.ma.masked_array(image_masked, mask=mask_num)
 
     else:
         a = find_all("SkyMapper_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.5), band), '.')
         if not a:
             get_SkyMapper_Pic(0, ra, dec, px, band)
             a = find_all("SkyMapper_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.5), band), '.')
         b = find_all("SkyMapper_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.5), band), '.')
@@ -324,395 +401,434 @@
                     if len(str(int(bit[i][j]))) > 12:
                         if (tempBit[-6] == 1) or (tempBit[-13] == 1):
                             mask[i][j] = np.nan
                     elif len(str(int(bit[i][j]))) > 5:
                         if (tempBit[-6] == 1):
                             mask[i][j] = np.nan
         mask = ~np.isnan(image_data_mask)
-        image_masked = ma.masked_array(image_data, mask=mask)
-    #edited to PASS BACK THE MASKED ARRAY!!
+        image_masked = np.ma.masked_array(image_data, mask=mask)
+
     #then return the data
     return np.array(image_masked), wcs, hdu
 
-def getSteps(SN_dict, SN_names, hostDF):
+def getSteps(SN_dict, transientNames, hostDF):
+    """Calculates a scale factor for the gradient ascent step
+       based on the mean kron radius of the galaxies in the field.
+
+    Parameters
+    ----------
+    SN_dict : dictionary
+        Key,value pairs of transient names and lists of candidate
+        host galaxy objIDs in PS1.
+    transientNames : array-like
+        Names of transients to associate.
+    hostDF : type
+        Description of parameter `hostDF`.
+
+    Returns
+    -------
+    steps : array-like
+        List of calculated steps.
+
+    """
     steps = []
     hostDF.replace(-999, np.nan, inplace=True)
     hostDF.replace(-999, np.nan, inplace=True)
-    for name in SN_names:
+    for name in transientNames:
         hostList = SN_dict[name]
         if (type(hostList) is np.int64 or type(hostList) is float):
             hostList = [hostList]
         checkNan = [x == x for x in hostList]
         if np.sum(checkNan) > 0:
             hostRadii = hostDF.loc[hostDF['objID'].isin(hostList), 'rKronRad'].values
             mean = np.nanmean(hostRadii)
             if mean == mean:
                 mean = np.max([mean,2])
                 step = np.min([mean, 50])
-                steps.append(step) #find some proper scaling factor between the mean and the step size
+
+                #find some proper scaling factor between the mean and the step size
+                steps.append(step)
             else:
                 steps.append(5)
         else:
             steps.append(5)
     return steps
 
-############# end functions ####################################
-def gradientAscent(path, SN_dict, SN_dict_postDLR, SN_names, hostDF, transientDF, fn, plot=1, px=800):
+def gradientAscent(path, SN_dict, SN_dict_postDLR, transientNames, hostDF, transientDF, fn, plot=True, px=800):
+    """The gradient ascent algorithm for identifying a final host galaxy.
+
+    Parameters
+    ----------
+    path : str
+        Filepath to save the output log for the algorithm.
+    SN_dict : dictionary
+        Key, val pairs are transient name, list of PS1 objIDs of
+        potential hosts. Dictionary is before the DLR method.
+    SN_dict_postDLR : dictionary
+        Key, val pairs are transient name, list of PS1 objIDs of
+        potential hosts. Dictionary is after the DLR method (so
+        should have mostly one host per transient).
+    transientNames : array-like
+        List of transient names.
+    hostDF : Pandas DataFrame
+        PS1 info for candidate hosts.
+    transientDF : Pandas DataFrame
+        TNS info for associated transients.
+    fn : str
+        Filename for gradientAscent log.
+    plot : bool
+        If True, plot the associated transients, the background maps,
+        and the gradient fields associated with each transient.
+    px : int
+        Image size (in pixels).
+
+    Returns
+    -------
+    SN_dict_postDLR : dictionary
+        Dictionary of transient, host objID pairs after
+        gradient ascent.
+    hostDF : Pandas DataFrame
+        Description of returned object.
+    unchanged : array-like
+        List of transients for which gradient ascent failed.
+
+    """
     warnings.filterwarnings('ignore', category=AstropyUserWarning)
     warnings.filterwarnings('ignore', category=AstropyWarning)
-    step_sizes = getSteps(SN_dict, SN_names, hostDF)
+    step_sizes = getSteps(SN_dict, transientNames, hostDF)
     unchanged = []
     N_associated = 0
     totalDTime = 0.
     totalGATime = 0.
     startGATime = time.time()
     f = open(fn, 'w')
     print("Starting size of data frame: %i" % len(hostDF), file=f)
     if plot:
         try:
             os.makedirs('quiverMaps')
         except:
             print("Already have the folder quiverMaps!")
     for i in np.arange(len(step_sizes)):
-        #try:
-        if True:
-            #clear buffer memory
-            gc.collect()
+        #clear buffer memory
+        gc.collect()
 
-            transient_name = SN_names[i]
-            print("Transient: %s"% transient_name, file=f)
+        transient_name = transientNames[i]
+        print("Transient: %s"% transient_name, file=f)
 
-            ra = transientDF.loc[transientDF['Name'] == transient_name, 'RA'].values[0]
-            dec = transientDF.loc[transientDF['Name'] == transient_name, 'DEC'].values[0]
-            #px = 64 #switching from 800 to 64 to speed up computation time a ton (this will fail for local bright hosts)
-            startTime = time.time()
-            g_img, wcs, g_hdu  = get_clean_img(ra, dec, px, 'g')
-            g_mask = np.ma.masked_invalid(g_img).mask
-            r_img, wcs, r_hdu  = get_clean_img(ra, dec, px, 'r')
-            r_mask = np.ma.masked_invalid(r_img).mask
-            i_img, wcs, i_hdu  = get_clean_img(ra, dec, px, 'i')
-            i_mask = np.ma.masked_invalid(i_img).mask
-            endTime = time.time()
-            dTime = endTime - startTime
-            print("Download time: %.2f\n"%dTime, file=f)
-            totalDTime+=dTime
-
-            #cleanup - remove the fits files when we're done using them
-            for band in ['g', 'r', 'i']:
-                os.remove("PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band))
-                os.remove("PS1_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.25), band))
-                os.remove("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band))
-
-            #os.chdir(path)
-            #    if e.errno != errno.EEXIST:
-            #        raise
-            #os.chdir("./quiverMaps")
-            nancount = 0
-            obj_interp = []
-            print("Commencing DAOStarFinder:\n", file=f)
-            for obj in [g_img, r_img, i_img]:
-                data = obj
-                mean, median, std = sigma_clipped_stats(data, sigma=15.0)
-                daofind = DAOStarFinder(fwhm=3.0, threshold=15.*std)
-                sources = daofind(data - median)
-                try:
-                    xvals = np.array(sources['xcentroid'])
-                    yvals = np.array(sources['ycentroid'])
-                    for k in np.arange(len(xvals)):
-                        tempx = xvals[k]
-                        tempy = yvals[k]
-                        yleft = np.max([int(tempy) - 10, 0])
-                        yright = np.min([int(tempy) + 10, np.shape(data)[1]-1])
-                        xleft = np.max([int(tempx) - 10, 0])
-                        xright = np.min([int(tempx) + 10, np.shape(data)[1]-1])
-
-                        for r in np.arange(yleft,yright+1):
-                            for j in np.arange(xleft, xright+1):
-                                if dist([xvals[k], yvals[k]], [j, r]) < 7:
-                                    data[r, j] = np.nan
-                    nancount += np.sum(np.isnan(data))
-                    positions = np.transpose((sources['xcentroid'], sources['ycentroid']))
-                    apertures = CircularAperture(positions, r=7.)
-                    if plot:
-                        fig = plt.figure(figsize=(10,10))
-                        ax = fig.gca()
-                        ax.imshow(data)
-                        apertures.plot(color='blue', lw=1.5, alpha=0.5)
-                        plt.axis('off')
-                        plt.savefig("quiverMaps/detectedStars_%s.png"%transient_name, bbox_inches='tight')
-                        plt.close()
-                except:
-                    print("No stars here!", file=f)
-
-                #old way of interpolating the data
-                #backx = np.arange(0,data.shape[1])
-                #backy = np.arange(0, data.shape[0])
-                #backxx, backyy = np.meshgrid(backx, backy)
-                #mask invalid values
-                #array = np.ma.masked_invalid(data)
-                #x1 = backxx[~array.mask]
-                #y1 = backyy[~array.mask]
-                #newarr = array[~array.mask]
-                #data = interpolate.griddata((x1, y1), newarr.ravel(), (backxx, backyy), method='cubic')
-                #print(np.nanmin(data))
-                #print(np.nanmax(data))
-
-                #new way of interpolating the data
-                mask = np.isnan(data).astype(np.uint8)
-                data = cv2.inpaint(data.astype(np.float32), mask, 3, cv2.INPAINT_TELEA)
-
-                obj_interp.append(data)
-
-            gMax = np.nanmax(obj_interp[0])
-
-            g_ZP = g_hdu.header['ZPT_0001']
-            r_ZP = r_hdu.header['ZPT_0001']
-            i_ZP = i_hdu.header['ZPT_0001']
-
-            gmag = -2.5*np.log10(obj_interp[0]) + g_ZP
-            rmag = -2.5*np.log10(obj_interp[1]) + r_ZP
-            imag = -2.5*np.log10(obj_interp[2]) + i_ZP
-
-            #now the mean can be taken
-            mean_zp = (g_ZP + r_ZP + i_ZP)/3
-            meanMag = (gmag + rmag + imag)/3
-            meanImg = 10**((mean_zp-meanMag)/2.5) #convert back to flux
-
-            print("NanCount = %i"%nancount,file=f)
-            mean_center = meanImg[int(px/2),int(px/2)]
-            print("Mean_center = %f" % mean_center,file=f)
+        ra = transientDF.loc[transientDF['Name'] == transient_name, 'RA'].values[0]
+        dec = transientDF.loc[transientDF['Name'] == transient_name, 'DEC'].values[0]
 
-            if plot:
-                plt.figure(figsize=(10,7))
-                plt.hist(meanImg.flatten(), bins=np.logspace(0, 6))
-                plt.xscale("log")
-                plt.savefig("quiverMaps/countsHistogram_%s.png" % transient_name, bbox_inches='tight')
-                plt.close()
+        startTime = time.time()
+        g_img, wcs, g_hdu  = get_clean_img(ra, dec, px, 'g')
+        g_mask = np.ma.masked_invalid(g_img).mask
+        r_img, wcs, r_hdu  = get_clean_img(ra, dec, px, 'r')
+        r_mask = np.ma.masked_invalid(r_img).mask
+        i_img, wcs, i_hdu  = get_clean_img(ra, dec, px, 'i')
+        i_mask = np.ma.masked_invalid(i_img).mask
+        endTime = time.time()
+        dTime = endTime - startTime
+        print("Download time: %.2f\n"%dTime, file=f)
+        totalDTime+=dTime
+
+        # cleanup - remove the fits files when we're done using them
+        for band in ['g', 'r', 'i']:
+            os.remove("PS1_ra={}_dec={}_{}arcsec_{}_stack.num.fits".format(ra, dec, int(px*0.25), band))
+            os.remove("PS1_ra={}_dec={}_{}arcsec_{}_mask.fits".format(ra, dec, int(px*0.25), band))
+            os.remove("PS1_ra={}_dec={}_{}arcsec_{}.fits".format(ra, dec, int(px*0.25), band))
+
+        nancount = 0
+        obj_interp = []
+        print("Commencing DAOStarFinder:\n", file=f)
+        for obj in [g_img, r_img, i_img]:
+            data = obj
+            mean, median, std = sigma_clipped_stats(data, sigma=15.0)
+            daofind = DAOStarFinder(fwhm=3.0, threshold=15.*std)
+            sources = daofind(data - median)
+            try:
+                xvals = np.array(sources['xcentroid'])
+                yvals = np.array(sources['ycentroid'])
+                for k in np.arange(len(xvals)):
+                    tempx = xvals[k]
+                    tempy = yvals[k]
+                    yleft = np.max([int(tempy) - 10, 0])
+                    yright = np.min([int(tempy) + 10, np.shape(data)[1]-1])
+                    xleft = np.max([int(tempx) - 10, 0])
+                    xright = np.min([int(tempx) + 10, np.shape(data)[1]-1])
+
+                    for r in np.arange(yleft,yright+1):
+                        for j in np.arange(xleft, xright+1):
+                            if dist([xvals[k], yvals[k]], [j, r]) < 7:
+                                data[r, j] = np.nan
+                nancount += np.sum(np.isnan(data))
+                positions = np.transpose((sources['xcentroid'], sources['ycentroid']))
+                apertures = CircularAperture(positions, r=7.)
+                if plot:
+                    fig = plt.figure(figsize=(10,10))
+                    ax = fig.gca()
+                    ax.imshow(data)
+                    apertures.plot(color='blue', lw=1.5, alpha=0.5)
+                    plt.axis('off')
+                    plt.savefig("quiverMaps/detectedStars_%s.png"%transient_name, bbox_inches='tight')
+                    plt.close()
+            except:
+                print("No stars here!", file=f)
 
-            meanImg[meanImg != meanImg] = 1.e-30
-            mean, median, std = sigma_clipped_stats(meanImg, sigma=10.0)
-            print("mean image = %e"% mean, file=f)
-            aboveCount = np.sum(meanImg > 1.)
-            aboveCount2 = np.sum(meanImg[int(px/2)-100:int(px/2)+100, int(px/2)-100:int(px/2)+100] > 1.)
-            aboveFrac2= aboveCount2/40000
-            print("aboveCount = %f"% aboveCount,file=f)
-            print("aboveCount2 = %f "% aboveCount2, file=f)
-            totalPx = px**2
-            aboveFrac = aboveCount/totalPx
-            print("aboveFrac= %f" % aboveFrac, file=f)
-            print("aboveFrac2 = %f "% aboveFrac2, file=f)
-
-            if ((median <15) and (np.round(aboveFrac2, 2) < 0.70)) or ((mean_center > 1.e3) and (np.round(aboveFrac,2) < 0.60) and (np.round(aboveFrac2,2) < 0.75)):
-                bs = 10
-                fs = 1
-                if aboveFrac2 < 0.7:
-                    step_sizes[int(i)] = 2.
-                else:
-                    step_sizes[int(i)] = 10.
-                print("Small filter", file=f)
-                size = 'small'
-            elif ((mean_center > 40) and (median > 500) and (aboveFrac > 0.60)) or ((mean_center > 300) and (aboveFrac2 > 0.7)):
-                bs = 75 #the big sources
-                fs = 3
-                print("Large filter", file=f)
-                step_sizes[int(i)] = np.max([step_sizes[int(i)], 50])
-                size = 'large'
+            # new way of interpolating the data
+            mask = np.isnan(data).astype(np.uint8)
+            data = cv2.inpaint(data.astype(np.float32), mask, 3, cv2.INPAINT_TELEA)
+
+            obj_interp.append(data)
+
+        gMax = np.nanmax(obj_interp[0])
+
+        g_ZP = g_hdu.header['ZPT_0001']
+        r_ZP = r_hdu.header['ZPT_0001']
+        i_ZP = i_hdu.header['ZPT_0001']
+
+        gmag = -2.5*np.log10(obj_interp[0]) + g_ZP
+        rmag = -2.5*np.log10(obj_interp[1]) + r_ZP
+        imag = -2.5*np.log10(obj_interp[2]) + i_ZP
+
+        #now the mean can be taken
+        mean_zp = (g_ZP + r_ZP + i_ZP)/3
+        meanMag = (gmag + rmag + imag)/3
+        meanImg = 10**((mean_zp-meanMag)/2.5) #convert back to flux
+
+        print("NanCount = %i"%nancount,file=f)
+        mean_center = meanImg[int(px/2),int(px/2)]
+        print("Mean_center = %f" % mean_center,file=f)
+
+        if plot:
+            plt.figure(figsize=(10,7))
+            plt.hist(meanImg.flatten(), bins=np.logspace(0, 6))
+            plt.xscale("log")
+            plt.savefig("quiverMaps/countsHistogram_%s.png" % transient_name, bbox_inches='tight')
+            plt.close()
+
+        meanImg[meanImg != meanImg] = 1.e-30
+        mean, median, std = sigma_clipped_stats(meanImg, sigma=10.0)
+        print("mean image = %e"% mean, file=f)
+        aboveCount = np.sum(meanImg > 1.)
+        aboveCount2 = np.sum(meanImg[int(px/2)-100:int(px/2)+100, int(px/2)-100:int(px/2)+100] > 1.)
+        aboveFrac2= aboveCount2/40000
+        print("aboveCount = %f"% aboveCount,file=f)
+        print("aboveCount2 = %f "% aboveCount2, file=f)
+        totalPx = px**2
+        aboveFrac = aboveCount/totalPx
+        print("aboveFrac= %f" % aboveFrac, file=f)
+        print("aboveFrac2 = %f "% aboveFrac2, file=f)
+
+        if ((median <15) and (np.round(aboveFrac2, 2) < 0.70)) or ((mean_center > 1.e3) and (np.round(aboveFrac,2) < 0.60) and (np.round(aboveFrac2,2) < 0.75)):
+            bs = 10
+            fs = 1
+            if aboveFrac2 < 0.7:
+                step_sizes[int(i)] = 2.
             else:
-                bs = 40 #everything in between
-                fs = 3
-                print("Medium filter", file=f)
-                step_sizes[int(i)] = np.max([step_sizes[int(i)], 15])
-                size = 'medium'
-
-            sigma_clip = SigmaClip(sigma=15.)
-            bkg_estimator = MeanBackground()
-            bkg3_g = Background2D(g_img, box_size=bs, filter_size=fs,
-             sigma_clip=sigma_clip, bkg_estimator=bkg_estimator)
-            bkg3_r = Background2D(r_img, box_size=bs, filter_size=fs,
-             sigma_clip=sigma_clip, bkg_estimator=bkg_estimator)
-            bkg3_i = Background2D(i_img, box_size=bs, filter_size=fs,
-             sigma_clip=sigma_clip, bkg_estimator=bkg_estimator)
-
-            #Bkg is in counts so average in mags
-            bkg3_g.background[bkg3_g.background < 0] = 1.e-30
-            bkg3_r.background[bkg3_r.background < 0] = 1.e-30
-            bkg3_i.background[bkg3_i.background < 0] = 1.e-30
-
-            backmag_g = -2.5*np.log10(bkg3_g.background) + g_ZP
-            backmag_r = -2.5*np.log10(bkg3_r.background) + r_ZP
-            backmag_i = -2.5*np.log10(bkg3_i.background) + i_ZP
-
-            mean_zp = (g_ZP + r_ZP + i_ZP)/3.
-            backmag = 0.333*backmag_g + 0.333*backmag_r + 0.333*backmag_i
-            background = 10**(mean_zp-backmag/2.5)
-
-            if plot:
-                fig, axs = plt.subplots(1, 3, sharex=True, sharey=True,figsize=(20,10))
-                axs[0].imshow(bkg3_g.background)
-                axs[0].axis('off')
-                axs[1].imshow(bkg3_r.background)
-                axs[1].axis('off')
-                axs[2].imshow(bkg3_i.background)
-                axs[2].axis('off')
-                plt.savefig("quiverMaps/backgrounds_%s.png" % transient_name, bbox_inches='tight')
-                plt.close()
+                step_sizes[int(i)] = 10.
+            print("Small filter", file=f)
+            size = 'small'
+        elif ((mean_center > 40) and (median > 500) and (aboveFrac > 0.60)) or ((mean_center > 300) and (aboveFrac2 > 0.7)):
+            bs = 75 #the big sources
+            fs = 3
+            print("Large filter", file=f)
+            step_sizes[int(i)] = np.max([step_sizes[int(i)], 50])
+            size = 'large'
+        else:
+            bs = 40 #everything in between
+            fs = 3
+            print("Medium filter", file=f)
+            step_sizes[int(i)] = np.max([step_sizes[int(i)], 15])
+            size = 'medium'
+
+        sigma_clip = SigmaClip(sigma=15.)
+        bkg_estimator = MeanBackground()
+        bkg3_g = Background2D(g_img, box_size=bs, filter_size=fs,
+         sigma_clip=sigma_clip, bkg_estimator=bkg_estimator)
+        bkg3_r = Background2D(r_img, box_size=bs, filter_size=fs,
+         sigma_clip=sigma_clip, bkg_estimator=bkg_estimator)
+        bkg3_i = Background2D(i_img, box_size=bs, filter_size=fs,
+         sigma_clip=sigma_clip, bkg_estimator=bkg_estimator)
+
+        #Bkg is in counts so average in mags
+        bkg3_g.background[bkg3_g.background < 0] = 1.e-30
+        bkg3_r.background[bkg3_r.background < 0] = 1.e-30
+        bkg3_i.background[bkg3_i.background < 0] = 1.e-30
+
+        backmag_g = -2.5*np.log10(bkg3_g.background) + g_ZP
+        backmag_r = -2.5*np.log10(bkg3_r.background) + r_ZP
+        backmag_i = -2.5*np.log10(bkg3_i.background) + i_ZP
+
+        mean_zp = (g_ZP + r_ZP + i_ZP)/3.
+        backmag = 0.333*backmag_g + 0.333*backmag_r + 0.333*backmag_i
+        background = 10**(mean_zp-backmag/2.5)
+
+        if plot:
+            fig, axs = plt.subplots(1, 3, sharex=True, sharey=True,figsize=(20,10))
+            axs[0].imshow(bkg3_g.background)
+            axs[0].axis('off')
+            axs[1].imshow(bkg3_r.background)
+            axs[1].axis('off')
+            axs[2].imshow(bkg3_i.background)
+            axs[2].axis('off')
+            plt.savefig("quiverMaps/backgrounds_%s.png" % transient_name, bbox_inches='tight')
+            plt.close()
+
+        mean, median, std = sigma_clipped_stats(meanImg, sigma=1.0)
+        meanImg[meanImg <= (mean)] = 1.e-30
+        meanImg[meanImg < 0] = 1.e-30
+
+        if plot:
+            fig = plt.figure(figsize=(10,10))
+            ax = fig.gca()
+            ax.imshow((meanImg)/np.nanmax(meanImg))
+            plt.axis('off')
+            plt.savefig("quiverMaps/normalizedMeanImage_%s.png" % transient_name, bbox_inches='tight')
+            plt.close()
+
+            fig = plt.figure(figsize=(10,10))
+            ax = fig.gca()
+            ax.imshow(background/np.nanmax(background))
+            plt.axis('off')
+            plt.savefig("quiverMaps/normalizedMeanBackground_%s.png" % transient_name, bbox_inches='tight')
+            plt.close()
+
+        if nancount > 1.e5:
+            imgWeight = 0
+        elif (mean_center > 1.e4):
+            imgWeight = 0.75
+        elif size == 'medium':
+            imgWeight = 0.33
+        else:
+            imgWeight = 0.10
 
-            mean, median, std = sigma_clipped_stats(meanImg, sigma=1.0)
-            meanImg[meanImg <= (mean)] = 1.e-30
-            meanImg[meanImg < 0] = 1.e-30
+        print("imgWeight= %f"%imgWeight, file=f)
+        fullbackground = ((1-imgWeight)*background/np.nanmax(background) + imgWeight*meanImg/np.nanmax(meanImg))*np.nanmax(background)
 
-            if plot:
-                fig = plt.figure(figsize=(10,10))
-                ax = fig.gca()
-                ax.imshow((meanImg)/np.nanmax(meanImg))
-                plt.axis('off')
-                plt.savefig("quiverMaps/normalizedMeanImage_%s.png" % transient_name, bbox_inches='tight')
-                plt.close()
+        n = px
+        X, Y = np.mgrid[0:n, 0:n]
+        dx, dy = np.gradient(fullbackground.T)
 
-                fig = plt.figure(figsize=(10,10))
-                ax = fig.gca()
-                ax.imshow(background/np.nanmax(background))
-                plt.axis('off')
-                plt.savefig("quiverMaps/normalizedMeanBackground_%s.png" % transient_name, bbox_inches='tight')
-                plt.close()
+        n_plot = 10
 
-            if nancount > 1.e5:
-                imgWeight = 0
-            elif (mean_center > 1.e4):
-                imgWeight = 0.75
-            elif size == 'medium':
-                imgWeight = 0.33
-            else:
-                imgWeight = 0.10
-            print("imgWeight= %f"%imgWeight, file=f)
-            fullbackground = ((1-imgWeight)*background/np.nanmax(background) + imgWeight*meanImg/np.nanmax(meanImg))*np.nanmax(background)
+        dx_small = dx[::n_plot, ::n_plot]
+        dy_small = dy[::n_plot, ::n_plot]
+        print("step = %f"%  step_sizes[int(i)], file=f)
 
-            n = px
-            X, Y = np.mgrid[0:n, 0:n]
-            dx, dy = np.gradient(fullbackground.T)
+        # the center of the grid
+        start = [[int(px/2),int(px/2)]]
 
-            n_plot = 10
+        if True:
+            start.append(updateStep(px, dx, dy, step_sizes[int(i)], start[-1], size))
+            for j in np.arange(1.e3):
+                start.append(updateStep(px, dx, dy, step_sizes[int(i)], start[-1], size))
+            it_array = np.array(start)
+            endPoint = start[-1]
 
-            dx_small = dx[::n_plot, ::n_plot]
-            dy_small = dy[::n_plot, ::n_plot]
-            print("step = %f"%  step_sizes[int(i)], file=f)
+            if plot:
+                fig  = plt.figure(figsize=(10,10))
+                ax = fig.gca()
+                ax.imshow(fullbackground)
+                plt.axis("off")
+                plt.savefig("quiverMaps/fullBackground_%s.png"%transient_name, bbox_inches='tight')
+                plt.close()
 
-            start = [[int(px/2),int(px/2)]] #the center of the grid
+            coords = wcs.wcs_pix2world(endPoint[0], endPoint[1], 0., ra_dec_order = True) # Note the third argument, set to 0, which indicates whether the pixel coordinates should be treated as starting from (1, 1) (as FITS files do) or from (0, 0)
+            print("Final ra, dec after GD : %f %f"% (coords[0], coords[1]), file=f)
 
-            if True:
-                start.append(updateStep(px, dx, dy, step_sizes[int(i)], start[-1], size))
-                for j in np.arange(1.e3):
-                    start.append(updateStep(px, dx, dy, step_sizes[int(i)], start[-1], size))
-                it_array = np.array(start)
-                endPoint = start[-1]
+            col = '#D34E24'
+            col2 = '#B54A24'
 
-                if plot:
-                    fig  = plt.figure(figsize=(10,10))
-                    ax = fig.gca()
-                    ax.imshow(fullbackground)
-                    plt.axis("off")
-                    plt.savefig("quiverMaps/fullBackground_%s.png"%transient_name, bbox_inches='tight')
-                    plt.close()
+            #lookup by ra, dec
+            try:
+                if size == 'large':
+                    a = query_ps1_noname(float(coords[0]), float(coords[1]), 20)
+                else:
+                    a = query_ps1_noname(float(coords[0]), float(coords[1]), 5)
+            except TypeError:
+                 continue
+            if a:
+                print("Found a host here!", file=f)
+                a = ascii.read(a)
+                a = a.to_pandas()
+                a.sort_values(by=['distance'], inplace=True)
+
+                a = a[a['nDetections'] > 1]
+                smallType = ['AbLS', 'EmLS' , 'EmObj', 'G', 'GammaS', 'GClstr', 'GGroup', 'GPair', 'GTrpl', 'G_Lens', 'IrS', 'PofG', 'RadioS', 'UvES', 'UvS', 'XrayS', '', 'QSO', 'QGroup', 'Q_Lens']
+                medType = ['G', 'IrS', 'PofG', 'RadioS', 'GPair', 'GGroup', 'GClstr', 'EmLS', 'RadioS', 'UvS', 'UvES', '']
+                largeType = ['G', 'PofG', 'GPair', 'GGroup', 'GClstr']
+                if len(a) > 0:
+                    a = getNEDInfo(a)
+                    if (size == 'large'):
+                        print("L: picking the closest NED galaxy within 20 arcsec", file=f)
+
+                        tempA = a[a['NED_type'].isin(largeType)]
+                        if len(tempA) > 0:
+                            a = tempA
+                        tempA = a[a['NED_type'] == 'G']
+                        if len(tempA) > 0:
+                            a = tempA
 
-                coords = wcs.wcs_pix2world(endPoint[0], endPoint[1], 0., ra_dec_order = True) # Note the third argument, set to 0, which indicates whether the pixel coordinates should be treated as starting from (1, 1) (as FITS files do) or from (0, 0)
-                print("Final ra, dec after GD : %f %f"% (coords[0], coords[1]), file=f)
-                col = '#D34E24'
-                col2 = '#B54A24'
-                #lookup by ra, dec
-                try:
-                    if size == 'large':
-                        a = query_ps1_noname(float(coords[0]), float(coords[1]), 20)
-                    else:
-                        a = query_ps1_noname(float(coords[0]), float(coords[1]), 5)
-                except TypeError:
-                     continue
-                if a:
-                    print("Found a host here!", file=f)
-                    a = ascii.read(a)
-                    a = a.to_pandas()
-                    a.sort_values(by=['distance'], inplace=True)
-
-                    a = a[a['nDetections'] > 1]
-                    smallType = ['AbLS', 'EmLS' , 'EmObj', 'G', 'GammaS', 'GClstr', 'GGroup', 'GPair', 'GTrpl', 'G_Lens', 'IrS', 'PofG', 'RadioS', 'UvES', 'UvS', 'XrayS', '', 'QSO', 'QGroup', 'Q_Lens']
-                    medType = ['G', 'IrS', 'PofG', 'RadioS', 'GPair', 'GGroup', 'GClstr', 'EmLS', 'RadioS', 'UvS', 'UvES', '']
-                    largeType = ['G', 'PofG', 'GPair', 'GGroup', 'GClstr']
-                    if len(a) > 0:
-                        a = getNEDInfo(a)
-                        if (size == 'large'):
-                            print("L: picking the closest NED galaxy within 20 arcsec", file=f)
-
-                            tempA = a[a['NED_type'].isin(largeType)]
-                            if len(tempA) > 0:
-                                a = tempA
-                            tempA = a[a['NED_type'] == 'G']
-                            if len(tempA) > 0:
-                                a = tempA
-
-                            if len(a) > 1:
-                                a = a.iloc[[0]]
-                        elif (size == 'medium'):
-                            print("M: Picking the closest NED galaxy within 5 arcsec", file=f)
-                            tempA = a[a['NED_type'].isin(medType)]
-                            if len(tempA) > 0:
-                                a = tempA
-                            if len(a) > 1:
-                                a = a.iloc[[0]]
-                        else:
-                            tempA = a[a['NED_type'].isin(smallType)]
-                            if len(tempA) > 0:
-                                a = tempA
+                        if len(a) > 1:
+                            a = a.iloc[[0]]
+                    elif (size == 'medium'):
+                        print("M: Picking the closest NED galaxy within 5 arcsec", file=f)
+                        tempA = a[a['NED_type'].isin(medType)]
+                        if len(tempA) > 0:
+                            a = tempA
+                        if len(a) > 1:
                             a = a.iloc[[0]]
-                            print("S: Picking the closest non-stellar source within 5 arcsec", file=f)
-                        print("Nice! Host association chosen.", file=f)
-                        print("NED type: %s" % a['NED_type'].values[0], file=f)
-                        print(a['objID'].values[0], file=f)
-                        print("Chosen Host RA and DEC: %f %f"% (a['raMean'], a['decMean']), file=f)
-                        SN_dict_postDLR[transient_name] = a['objID'].values[0]
-                        print("Dict value: %i"%SN_dict_postDLR[transient_name],file=f)
-                        N = len(hostDF)
-                        hostDF = pd.concat([hostDF, a], ignore_index=True)
-                        N2 = len(hostDF)
-                        if N2 != (N+1):
-                            print("ERROR! Value not concatenated!!", file=f)
-                            return
-                        finalRA = np.array(a['raMean'])
-                        finalDEC = np.array(a['decMean'])
-                        col = 'tab:green'
-                        col2 = '#078840'
                     else:
-                        unchanged.append(transient_name)
+                        tempA = a[a['NED_type'].isin(smallType)]
+                        if len(tempA) > 0:
+                            a = tempA
+                        a = a.iloc[[0]]
+                        print("S: Picking the closest non-stellar source within 5 arcsec", file=f)
+                    print("Nice! Host association chosen.", file=f)
+                    print("NED type: %s" % a['NED_type'].values[0], file=f)
+                    print(a['objID'].values[0], file=f)
+                    print("Chosen Host RA and DEC: %f %f"% (a['raMean'], a['decMean']), file=f)
+                    SN_dict_postDLR[transient_name] = a['objID'].values[0]
+                    print("Dict value: %i"%SN_dict_postDLR[transient_name],file=f)
+                    N = len(hostDF)
+                    hostDF = pd.concat([hostDF, a], ignore_index=True)
+                    N2 = len(hostDF)
+                    if N2 != (N+1):
+                        print("ERROR! Value not concatenated!!", file=f)
+                        return
+                    finalRA = np.array(a['raMean'])
+                    finalDEC = np.array(a['decMean'])
+                    col = 'tab:green'
+                    col2 = '#078840'
                 else:
                     unchanged.append(transient_name)
-                if plot:
-                    fig = plt.figure(figsize=(20,20))
-                    ax = fig.gca()
-                    ax.imshow(i_img, norm=colors.PowerNorm(gamma = 0.5, vmin=1, vmax=1.e4), cmap='gray')#, cmap='gray', norm=LogNorm())
-                    it_array = np.array(start)
-                    ax.plot(it_array.T[0], it_array.T[1], "--", lw=5, c=col, zorder=20)
-                    ax.scatter([int(px/2)], [int(px/2)], marker='*', s=1000, color='#f3a712', zorder=50)
-                    ax.scatter(endPoint[0], endPoint[1], marker='*', lw=4, s=1000, facecolor='#f3a712', edgecolor=col2, zorder=200)
-                    ax.quiver(X[::n_plot,::n_plot], Y[::n_plot,::n_plot], dx[::n_plot,::n_plot], dy[::n_plot,::n_plot], color='#845C9B', angles='xy', scale_units = 'xy')
-                    plt.axis('off')
-                    plt.savefig("quiverMaps/quiverMap_%s.png"%transient_name, bbox_inches='tight')
-                    plt.close()
-                N_associated += 1
-            f.flush()
-            if N_associated%10 == 0:
-                print("N_associated = %i"%N_associated,file=f)
-                print("Size of table = %i"%len(hostDF),file=f)
-                print("Saving the modified way!")
-                with open(path+"/dictionaries/gals_postGD.p", 'wb') as fp:
-                    #pickle.dump(SN_dict_postDLR, fp, protocol=pickle.HIGHEST_PROTOCOL)
-                    dump(SN_dict_postDLR, fp)
-                hostDF.to_csv(path+"/hostDF_postGD.tar.gz", index=False)
-        #except:
-        #     continue
+            else:
+                unchanged.append(transient_name)
+            if plot:
+                fig = plt.figure(figsize=(20,20))
+                ax = fig.gca()
+                ax.imshow(i_img, norm=colors.PowerNorm(gamma = 0.5, vmin=1, vmax=1.e4), cmap='gray')
+                it_array = np.array(start)
+                ax.plot(it_array.T[0], it_array.T[1], "--", lw=5, c=col, zorder=20)
+                ax.scatter([int(px/2)], [int(px/2)], marker='*', s=1000, color='#f3a712', zorder=50)
+                ax.scatter(endPoint[0], endPoint[1], marker='*', lw=4, s=1000, facecolor='#f3a712', edgecolor=col2, zorder=200)
+                ax.quiver(X[::n_plot,::n_plot], Y[::n_plot,::n_plot], dx[::n_plot,::n_plot], dy[::n_plot,::n_plot], color='#845C9B', angles='xy', scale_units = 'xy')
+                plt.axis('off')
+                plt.savefig("quiverMaps/quiverMap_%s.png"%transient_name, bbox_inches='tight')
+                plt.close()
+            N_associated += 1
+        f.flush()
+        if N_associated%10 == 0:
+            print("N_associated = %i"%N_associated,file=f)
+            print("Size of table = %i"%len(hostDF),file=f)
+            print("Saving the modified way!")
+            with open(path+"/dictionaries/gals_postGD.p", 'wb') as fp:
+                dump(SN_dict_postDLR, fp)
+            hostDF.to_csv(path+"/hostDF_postGD.tar.gz", index=False)
 
     with open(path+"/dictionaries/gals_postGD.p", 'wb') as fp:
-        #pickle.dump(SN_dict_postDLR, fp, protocol=pickle.HIGHEST_PROTOCOL)
         dump(SN_dict_postDLR, fp)
     hostDF.to_csv(path+"/hostDF_postGD.tar.gz", index=False)
     print("Total Download time: %.2f\n"%totalDTime, file=f)
     endGATime = time.time()
     totalGATime = endGATime - startGATime
     print("Total Gradient Ascent time:%.2f\n"%totalGATime, file=f)
     f.close()
```

### Comparing `astro_ghost-0.2.3/astro_ghost/hostMatching.py` & `astro_ghost-0.2.4/astro_ghost/hostMatching.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,22 +3,36 @@
 import pandas as pd
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.coordinates import Angle
 import os
 import sys
 from datetime import datetime
-from astropy import units as u
-from astropy.coordinates import SkyCoord
-import pandas as pd
-import numpy as np
 import pickle
 from collections import Counter
 
 def build_ML_df(dic, hostDF, transientDF):
+    """Consolidates the final host associations into a single dataframe.
+
+    Parameters
+    ----------
+    dic : dictionary
+        key,value pairs of transient name, list of associated host PS1 objIDs
+        (should be one-to-one except where the association failed).
+    hostDF : Pandas DataFrame
+        PS1 properties for all host galaxies.
+    transientDF : Pandas DataFrame
+        TNS properties for all transients.
+
+    Returns
+    -------
+    hostDF : Pandas DataFrame
+        The final consolidated DF of transient & host galaxy properties.
+
+    """
     hostDF = hostDF.reset_index(drop=True)
     hostDF = hostDF.drop_duplicates(subset=['objID'],ignore_index=True)
     hostDF["TransientClass"] = ""
     hostDF["TransientName"] = ""
     colNames = set(transientDF.columns.values)
     colNames.remove('HostName')
     colNames.remove('RA')
@@ -47,13 +61,10 @@
             if len(transCoord) > 1:
                 transCoord = transCoord[0]
             hostDF.loc[idx, "TransientRA"] = transCoord.ra.deg
             hostDF.loc[idx, "TransientDEC"] = transCoord.dec.deg
             #adding all the extra columns that we haven't added yet
             for val in colNames:
                 hostDF.loc[idx, "Transient"+val.replace(" ", "")] = transientDF.loc[idx_transient, val].to_string(index=False).strip()
-            #hostDF.loc[idx, "TransientDiscoveryMag"] = transientDF.loc[idx_transient, 'Discovery Mag'].to_string(index=False).strip()
-            #hostDF.loc[idx, "TransientRedshift"] = transientDF.loc[idx_transient, 'Redshift'].to_string(index=False).strip()
     hostDF = hostDF[hostDF["TransientClass"] != ""]
-    #hostDF = hostDF.drop_duplicates(subset=hostDF.columns.difference(['distance']))
     hostDF = hostDF.reset_index(drop=True)
     return hostDF
```

### Comparing `astro_ghost-0.2.3/astro_ghost/stellarLocus.py` & `astro_ghost-0.2.4/astro_ghost/stellarLocus.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,68 @@
 import seaborn as sns
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
-import matplotlib
-import astropy.table as at
+import matplotlib.colors import LogNorm
+from astropy.table import Table
 import scipy.interpolate as scinterp
 import pkg_resources
 
-# recalibration done via https://iopscience.iop.org/article/10.3847/0004-637X/822/2/66
-# Hypercalibration: A Pan-starrs1-Based recalibration of the sloan digital sky survey
-# photometry (Finkbeiner et al., 2016)
 def convert_to_SDSS(conversions, g_iPS1, band, mPS1):
+    """Convert PS1 to SDSS photometry. Recalibration done via the coefficients in
+       Hypercalibration: A Pan-starrs1-Based recalibration of the sloan digital sky survey
+       photometry (Finkbeiner et al., 2016). Publication can be found at
+       https://iopscience.iop.org/article/10.3847/0004-637X/822/2/66.
+
+    Parameters
+    ----------
+    conversions : Pandas DataFrame
+        Coefficients from Finkbeiner et al., 2016.
+    g_iPS1 : float
+        Apparent g - i color of the source in PS1.
+    band : str
+        Band in which to calculate the conversion.
+    mPS1 : float
+        AB apparent magnitude of the source in PS1.
+
+    Returns
+    -------
+    mSDSS, float
+        Estimated AB apparent magnitude of the source in SDSS.
+
+    """
     a0 = conversions.loc[conversions['Band'] == band, 'a_0'].values[0]
     a1 = conversions.loc[conversions['Band'] == band, 'a_1'].values[0]
     a2 = conversions.loc[conversions['Band'] == band, 'a_2'].values[0]
     a3 = conversions.loc[conversions['Band'] == band, 'a_3'].values[0]
     mPS1_mSDSS = a0 + a1*g_iPS1 + a2*g_iPS1**2 + a3*g_iPS1**3
     mSDSS = mPS1 - (mPS1_mSDSS)
     return mSDSS
 
-# Calculate 7DCD (actually a 4DCD here, because we only have these 4 colors) and
-# store value in new column in dataframe
-# stellar_loci - the table of stellar loci taken from PS1 (Tonry et al.)
-# df - the dataframe of potential hosts
 def calc_7DCD(df):
-    #read the stellar locus table from SDSS
+    """Calculates the color distance (7DCD) of objects in df from the
+       stellar locus from Tonry et al., 2012.
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+        Dataframe of PS1 objects.
+
+    Returns
+    -------
+    df : Pandas DataFrame
+        The same dataframe as input, with new column 7DCD.
+
+    """
     df.replace(999.00, np.nan)
     df.replace(-999.00, np.nan)
 
+    #read the stellar locus table from SDSS
     stream = pkg_resources.resource_stream(__name__, 'tonry_ps1_locus.txt')
-    
-    skt = at.Table.read(stream, format='ascii')
+    skt = Table.read(stream, format='ascii')
 
     gr = scinterp.interp1d(skt['ri'], skt['gr'], kind='cubic', fill_value='extrapolate')
     iz = scinterp.interp1d(skt['ri'], skt['iz'], kind='cubic', fill_value='extrapolate')
     zy = scinterp.interp1d(skt['ri'], skt['zy'], kind='cubic', fill_value='extrapolate')
     ri = np.arange(-0.4, 2.01, 0.001)
 
     gr_new = gr(ri)
@@ -60,33 +88,50 @@
         temp_7DCD_1val_zy = (df.loc[i,"z-y"] - zy_new)**2/df.loc[i, "z-yErr"]
 
         temp_7DCD_1val = temp_7DCD_1val_gr + temp_7DCD_1val_ri + temp_7DCD_1val_iz + temp_7DCD_1val_zy
 
         df.loc[i,"7DCD"] = np.nanmin(np.array(temp_7DCD_1val))
     return df
 
-def plotLocus(df, color=0, save=0, type="", timestamp=""):
+def plotLocus(df, color=False, save=False, type="", timestamp=""):
+    """Plots the color-color distribution of objects in df along with the Tonry et al., 2012
+       PS1 stellar locus.
+
+    Parameters
+    ----------
+    df : Pandas DataFrame
+        Description of parameter `df`.
+    color : bool
+        If True, color objects by their distance from the stellar locus.
+    save : bool
+        If True, saves the image.
+    type : str
+        Can be "Gals" for galaxies or "Stars" for stars. Only relevant for
+        coloring the distributions.
+    timestamp : str
+        Timestamp to append to the saved plot filename.
+
+    """
     if color:
         plt.figure(figsize=(8,8))
-        plt.scatter(df["i-z"], df["g-r"], c=df["7DCD"], s=2, alpha=0.8, norm=matplotlib.colors.LogNorm())
+        plt.scatter(df["i-z"], df["g-r"], c=df["7DCD"], s=2, alpha=0.8, norm=LogNorm())
         plt.xlim(-0.75, 1)
         plt.clim(0.1, 1000)
         plt.ylim(-0.5, 2)
         plt.xlabel("i-z")
         plt.ylabel("g-r")
         cbar = plt.colorbar()
-        cbar.set_label("3D Color Distance")
+        cbar.set_label("4D Color Distance")
         if save:
-
             plt.savefig("PS1_%s_StellarLocus_%s_Colored.pdf"%(type, timestamp))
         else:
             plt.show()
     else:
         #read the stellar locus table from PS1
-        skt = at.Table.read('./tonry_ps1_locus.txt', format='ascii')
+        skt = Table.read('./tonry_ps1_locus.txt', format='ascii')
 
         gr = scinterp.interp1d(skt['ri'], skt['gr'], kind='cubic', fill_value='extrapolate')
         iz = scinterp.interp1d(skt['ri'], skt['iz'], kind='cubic', fill_value='extrapolate')
         zy = scinterp.interp1d(skt['ri'], skt['zy'], kind='cubic', fill_value='extrapolate')
         ri = np.arange(-0.4, 2.01, 0.001)
 
         gr_new = gr(ri)
```

### Comparing `astro_ghost-0.2.3/astro_ghost/tutorial.py` & `astro_ghost-0.2.4/astro_ghost/tutorial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import os
 import sys
 from astro_ghost.PS1QueryFunctions import getAllPostageStamps
 from astro_ghost.TNSQueryFunctions import getTNSSpectra
 from astro_ghost.NEDQueryFunctions import getNEDSpectra
 from astro_ghost.ghostHelperFunctions import *
 from astropy.coordinates import SkyCoord
-from astro_ghost.classifier import classify
 from astropy import units as u
 import pandas as pd
 from datetime import datetime
 import astro_ghost
 
 #we want to include print statements so we know what the algorithm is doing
 verbose = 1
 
 
-#download the database from ghost.ncsa.illinois.edu
+#Download the GHOST database.
 #note: real=False creates an empty database, which
 #allows you to use the association methods without
 #needing to download the full database first
 getGHOST(real=True, verbose=verbose, installpath='/where/to/install/GHOSTdb?/')
 
 #create a list of the supernova names and their skycoords (these three are from TNS)
 snName = ['SN 2012dt', 'SN 1998bn', 'SN 1957B']
@@ -29,18 +28,14 @@
            SkyCoord(186.26125*u.deg, +12.899444*u.deg, frame='icrs')]
 
 # run the association algorithm!
 # this first checks the GHOST database for a SN by name, then by coordinates, and
 # if we have no match then it manually associates them.
 hosts = getTransientHosts(snName, snCoord, verbose=verbose, starcut='normal', ascentMatch=True, px=64, savepath='/path/to/savedir/', GHOSTpath='/where/did/you/install/GHOSTdb?/')
 
-
-# classify transients
-hosts_wPredictions = classify(hosts)
-
 #create directories to store the host spectra, the transient spectra, and the postage stamps
 hSpecPath = "./hostSpectra/"
 tSpecPath = "./SNspectra/"
 psPath = "./hostPostageStamps/"
 paths = [hSpecPath, tSpecPath, psPath]
 for tempPath in paths:
     if not os.path.exists(tempPath):
@@ -83,11 +78,11 @@
 
 # 5. get an image of the host galaxy system associated with a supernova (by supernova name)
 getHostImage(snName, save=0)
 
 # 6. Find all supernova-host galaxy matches within a certain search radius (in arcseconds)
 coneSearchPairs(supernovaCoord[0], 1.e3)
 
-#7. Beta: find photometric redshift of host galaxies matches:
+#7. Find photometric redshift of host galaxies matches:
 from astro_ghost.photoz_helper import calc_photoz
 posterior_dict, hosts = calc_photoz(hosts)
 print(hosts['photo_z'].values)
```

### Comparing `astro_ghost-0.2.3/astro_ghost/tutorial_databaseSearch.py` & `astro_ghost-0.2.4/astro_ghost/tutorial_databaseSearch.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-0.2.4/astro_ghost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-0.2.3/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-0.2.4/astro_ghost.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -8,40 +8,36 @@
 tox.ini
 .github/workflows/docs.yml
 .github/workflows/tests.yml
 astro_ghost/DLR.py
 astro_ghost/NEDQueryFunctions.py
 astro_ghost/PS1QueryFunctions.py
 astro_ghost/SimbadQueryFunctions.py
-astro_ghost/Star_Galaxy_IdealModel.sav
-astro_ghost/Star_Galaxy_RealisticModel.sav
 astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
 astro_ghost/TNSQueryFunctions.py
 astro_ghost/__init__.py
 astro_ghost/_version.py
-astro_ghost/classifier.py
 astro_ghost/conftest.py
-astro_ghost/dimensionalityReduction.py
 astro_ghost/ghostHelperFunctions.py
 astro_ghost/gradientAscent.py
 astro_ghost/hostMatching.py
 astro_ghost/photoz_helper.py
 astro_ghost/sourceCleaning.py
 astro_ghost/starSeparation.py
 astro_ghost/stellarLocus.py
 astro_ghost/tonry_ps1_locus.txt
-astro_ghost/transientHelperFunctions.py
 astro_ghost/tutorial.py
 astro_ghost/tutorial_databaseSearch.py
 astro_ghost.egg-info/PKG-INFO
 astro_ghost.egg-info/SOURCES.txt
 astro_ghost.egg-info/dependency_links.txt
 astro_ghost.egg-info/not-zip-safe
 astro_ghost.egg-info/requires.txt
 astro_ghost.egg-info/top_level.txt
+database/GHOST.csv
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 licenses/LICENSE.rst
 licenses/README.rst
 tests/__init__.py
```

### Comparing `astro_ghost-0.2.3/docs/Makefile` & `astro_ghost-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/docs/conf.py` & `astro_ghost-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/docs/index.rst` & `astro_ghost-0.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/docs/make.bat` & `astro_ghost-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/licenses/LICENSE.rst` & `astro_ghost-0.2.4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/setup.cfg` & `astro_ghost-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-0.2.3/setup.py` & `astro_ghost-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "0.2.3"
+version = "0.2.4"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-0.2.3/tox.ini` & `astro_ghost-0.2.4/tox.ini`

 * *Files identical despite different names*

