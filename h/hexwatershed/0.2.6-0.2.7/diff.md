# Comparing `tmp/hexwatershed-0.2.6.tar.gz` & `tmp/hexwatershed-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexwatershed-0.2.6.tar", last modified: Wed May 10 03:20:04 2023, max compression
+gzip compressed data, was "hexwatershed-0.2.7.tar", last modified: Wed May 10 04:04:27 2023, max compression
```

## Comparing `hexwatershed-0.2.6.tar` & `hexwatershed-0.2.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:20:04.441585 hexwatershed-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-10 03:20:04.441585 hexwatershed-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:20:04.437585 hexwatershed-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4863 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:20:04.437585 hexwatershed-0.2.6/hexwatershed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-10 03:20:04.000000 hexwatershed-0.2.6/hexwatershed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-10 03:20:04.000000 hexwatershed-0.2.6/hexwatershed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:20:04.000000 hexwatershed-0.2.6/hexwatershed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 03:20:04.000000 hexwatershed-0.2.6/hexwatershed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:20:04.000000 hexwatershed-0.2.6/hexwatershed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:20:04.437585 hexwatershed-0.2.6/pyhexwatershed/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:20:04.437585 hexwatershed-0.2.6/pyhexwatershed/_bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)   430360 2023-05-10 03:20:03.000000 hexwatershed-0.2.6/pyhexwatershed/_bin/hexwatershed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:20:04.437585 hexwatershed-0.2.6/pyhexwatershed/algorithm/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/algorithm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:20:04.437585 hexwatershed-0.2.6/pyhexwatershed/algorithm/auxiliary/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/algorithm/auxiliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/algorithm/auxiliary/gdal_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/algorithm/auxiliary/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:20:04.441585 hexwatershed-0.2.6/pyhexwatershed/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/classes/_hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45475 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/classes/_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)    46594 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/classes/pycase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/pyhexwatershed_create_template_configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyhexwatershed/pyhexwatershed_read_model_configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-10 03:20:04.441585 hexwatershed-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-10 03:19:37.000000 hexwatershed-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:27.252481 hexwatershed-0.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4863 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/hexwatershed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-10 04:04:27.000000 hexwatershed-0.2.7/hexwatershed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-10 04:04:27.000000 hexwatershed-0.2.7/hexwatershed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:04:27.000000 hexwatershed-0.2.7/hexwatershed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 04:04:27.000000 hexwatershed-0.2.7/hexwatershed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 04:04:27.000000 hexwatershed-0.2.7/hexwatershed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/pyhexwatershed/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/pyhexwatershed/_bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   430360 2023-05-10 04:04:26.000000 hexwatershed-0.2.7/pyhexwatershed/_bin/hexwatershed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/pyhexwatershed/algorithm/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/algorithm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/pyhexwatershed/algorithm/auxiliary/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/algorithm/auxiliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/algorithm/auxiliary/gdal_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/algorithm/auxiliary/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/pyhexwatershed/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/classes/_hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45475 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/classes/_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46594 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/classes/pycase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/pyhexwatershed_create_template_configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyhexwatershed/pyhexwatershed_read_model_configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-10 04:04:27.256482 hexwatershed-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-10 04:04:05.000000 hexwatershed-0.2.7/setup.py
```

### Comparing `hexwatershed-0.2.6/CONTRIBUTING.rst` & `hexwatershed-0.2.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/LICENSE.md` & `hexwatershed-0.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/PKG-INFO` & `hexwatershed-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexwatershed
-Version: 0.2.6
+Version: 0.2.7
 Summary: A mesh-independent flow direction model for hydrologic models
 Home-page: https://github.com/changliao1025/pyhexwatershed
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Description: 
         ## `HexWatershed`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hexwatershed Version: 0.2.6 Summary: A mesh-
+Metadata-Version: 2.1 Name: hexwatershed Version: 0.2.7 Summary: A mesh-
 independent flow direction model for hydrologic models Home-page: https://
 github.com/changliao1025/pyhexwatershed Author: Chang Liao Author-email:
 chang.liao@pnnl.gov License: custom Description: ## `HexWatershed` [![DOI]
 (https://zenodo.org/badge/235201194.svg)](https://zenodo.org/badge/latestdoi/
 235201194) HexWatershed: a mesh independent flow direction model for
 hydrological models. This Python package provides a `Python` interface to the
 underlying `HexWatershed` model. `HexWatershed` has been compiled and tested on
```

### Comparing `hexwatershed-0.2.6/README.md` & `hexwatershed-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/docs/Makefile` & `hexwatershed-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/docs/conf.py` & `hexwatershed-0.2.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/docs/installation.rst` & `hexwatershed-0.2.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/docs/make.bat` & `hexwatershed-0.2.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/hexwatershed.egg-info/PKG-INFO` & `hexwatershed-0.2.7/hexwatershed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexwatershed
-Version: 0.2.6
+Version: 0.2.7
 Summary: A mesh-independent flow direction model for hydrologic models
 Home-page: https://github.com/changliao1025/pyhexwatershed
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Description: 
         ## `HexWatershed`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hexwatershed Version: 0.2.6 Summary: A mesh-
+Metadata-Version: 2.1 Name: hexwatershed Version: 0.2.7 Summary: A mesh-
 independent flow direction model for hydrologic models Home-page: https://
 github.com/changliao1025/pyhexwatershed Author: Chang Liao Author-email:
 chang.liao@pnnl.gov License: custom Description: ## `HexWatershed` [![DOI]
 (https://zenodo.org/badge/235201194.svg)](https://zenodo.org/badge/latestdoi/
 235201194) HexWatershed: a mesh independent flow direction model for
 hydrological models. This Python package provides a `Python` interface to the
 underlying `HexWatershed` model. `HexWatershed` has been compiled and tested on
```

### Comparing `hexwatershed-0.2.6/hexwatershed.egg-info/SOURCES.txt` & `hexwatershed-0.2.7/hexwatershed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/pyhexwatershed/_bin/hexwatershed` & `hexwatershed-0.2.7/pyhexwatershed/_bin/hexwatershed`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/pyhexwatershed/algorithm/auxiliary/gdal_function.py` & `hexwatershed-0.2.7/pyhexwatershed/algorithm/auxiliary/gdal_function.py`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/pyhexwatershed/algorithm/auxiliary/statistics.py` & `hexwatershed-0.2.7/pyhexwatershed/algorithm/auxiliary/statistics.py`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/pyhexwatershed/classes/_hpc.py` & `hexwatershed-0.2.7/pyhexwatershed/classes/_hpc.py`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/pyhexwatershed/classes/_visual.py` & `hexwatershed-0.2.7/pyhexwatershed/classes/_visual.py`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/pyhexwatershed/classes/pycase.py` & `hexwatershed-0.2.7/pyhexwatershed/classes/pycase.py`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/pyhexwatershed/pyhexwatershed_create_template_configuration_file.py` & `hexwatershed-0.2.7/pyhexwatershed/pyhexwatershed_create_template_configuration_file.py`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/pyhexwatershed/pyhexwatershed_read_model_configuration_file.py` & `hexwatershed-0.2.7/pyhexwatershed/pyhexwatershed_read_model_configuration_file.py`

 * *Files identical despite different names*

### Comparing `hexwatershed-0.2.6/setup.py` & `hexwatershed-0.2.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 
 import io
 import os
-import sys
 import subprocess
 import shutil
 
 from setuptools import setup, find_packages, Command
 from packaging import version
 
+# Run git submodule sync
+subprocess.call(['git', 'submodule', 'sync'])
+
+# Run git submodule update --init --recursive
+subprocess.call(['git', 'submodule', 'update', '--init', '--recursive'])
+
 NAME = "hexwatershed"
 DESCRIPTION = \
     "A mesh-independent flow direction model for hydrologic models"
 AUTHOR = "Chang Liao"
 AUTHOR_EMAIL = "chang.liao@pnnl.gov"
 URL = "https://github.com/changliao1025/pyhexwatershed"
-VERSION = "0.2.6"
+VERSION = "0.2.7"
 REQUIRES_PYTHON = ">=3.8.0"
 KEYWORDS = "hexwatershed hexagon"
 
 REQUIRED = [
     "packaging",
     "numpy",
     "matplotlib",
@@ -73,46 +78,41 @@
     def run(self):
         """
         The actual cmake-based build steps for hexwatershed
 
         """
         if (self.dry_run): return
 
-        # Define the Git command to download the submodule
-        git_command = "git submodule update --init --recursive"
-
         cwd_pointer = os.getcwd()
 
         try:
             self.announce("cmake config.", level=3)
 
             source_path = os.path.join(
                 HERE, "external", "hexwatershed")
             # Run the command using subprocess
-            #if os.path.exists(source_path):
-            #    shutil.rmtree(source_path, ignore_errors=True)
-
-            print("Download submodule")
-            subprocess.run(git_command.split(), check=True)
+            if os.path.exists(source_path):
+                pass
+            else:
+                print('source path does not exist:', source_path)
+            
 
-            builds_path = \
-                os.path.join(source_path, "build")
+            builds_path =  os.path.join(source_path, "build")
 
-            if os.path.exists(builds_path):
-                #os.makedirs(builds_path, exist_ok=True)
+            if os.path.exists(builds_path):                
                 sFilename_cache  = os.path.join(builds_path, "CMakeCache.txt")
                 if os.path.exists(sFilename_cache):
                     os.remove(sFilename_cache)
                 else:
                     #print('File or directory does not exist')
                     pass
 
                 pass
             else:
-                print('build path does not exist!')
+                print('build path does not exist:', builds_path)
 
             exesrc_path = \
                 os.path.join(source_path, "bin")
 
             libsrc_path = \
                 os.path.join(source_path, "lib")
```

