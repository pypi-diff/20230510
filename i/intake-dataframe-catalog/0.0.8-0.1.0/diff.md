# Comparing `tmp/intake_dataframe_catalog-0.0.8.tar.gz` & `tmp/intake_dataframe_catalog-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_dataframe_catalog-0.0.8.tar", last modified: Tue May  9 23:02:33 2023, max compression
+gzip compressed data, was "intake_dataframe_catalog-0.1.0.tar", last modified: Wed May 10 02:40:01 2023, max compression
```

## Comparing `intake_dataframe_catalog-0.0.8.tar` & `intake_dataframe_catalog-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:02:33.756687 intake_dataframe_catalog-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-09 23:02:33.756687 intake_dataframe_catalog-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 23:02:33.756687 intake_dataframe_catalog-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:02:33.756687 intake_dataframe_catalog-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:02:33.756687 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 23:02:33.756687 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:02:33.756687 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-09 23:02:33.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 23:02:33.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:02:33.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 23:02:33.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 23:02:33.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 23:02:33.000000 intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:02:33.756687 intake_dataframe_catalog-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-09 23:02:19.000000 intake_dataframe_catalog-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:40:01.044345 intake_dataframe_catalog-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-10 02:40:01.044345 intake_dataframe_catalog-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 02:40:01.044345 intake_dataframe_catalog-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:40:01.040345 intake_dataframe_catalog-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:40:01.044345 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 02:40:01.044345 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:40:01.044345 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-10 02:40:01.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-10 02:40:01.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 02:40:01.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 02:40:01.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 02:40:01.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 02:40:01.000000 intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:40:01.044345 intake_dataframe_catalog-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21401 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-10 02:39:45.000000 intake_dataframe_catalog-0.1.0/versioneer.py
```

### Comparing `intake_dataframe_catalog-0.0.8/LICENSE` & `intake_dataframe_catalog-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.8/PKG-INFO` & `intake_dataframe_catalog-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake_dataframe_catalog
-Version: 0.0.8
+Version: 0.1.0
 Summary: An intake driver for a searchable table of intake catalogs and associated metadata
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -19,19 +19,17 @@
 **A simple intake plugin for a searchable table of intake catalogs and associated metadata.**
 
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
-| Package       | |pypi|               |
+| Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI            | |tests| |pre-commit| |
-+---------------+----------------------+
-| CD            | |build|              |
+| CI/CD         | |ci| |cd|            |
 +---------------+----------------------+
 | Development   | |codecov| |black|    |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 Overview
@@ -64,25 +62,25 @@
         :target: https://intake-dataframe-catalog.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
         
 .. |pypi| image:: https://img.shields.io/pypi/v/intake-dataframe-catalog
         :target: https://pypi.org/project/intake-dataframe-catalog/
         :alt: Python Package Index Build
         
-.. |tests| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/tests.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/tests.yml
-        :alt: Package test status
-        
-.. |pre-commit| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/pre-commit.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/pre-commit.yml
-        :alt: Package pre-commit status
-        
-.. |build| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/release.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/release.yml
-        :alt: Build distribution status
+.. |conda| image:: https://anaconda.org/accessnri/intake-dataframe-catalog/badges/version.svg
+        :target: https://anaconda.org/accessnri/intake-dataframe-catalog
+        :alt: Conda Build
+
+.. |ci| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/ci.yml
+        :alt: Package CI test status
+        
+.. |cd| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/cd.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/cd.yml
+        :alt: Package CD status
         
 .. |codecov| image:: https://codecov.io/gh/ACCESS-NRI/intake-dataframe-catalog/branch/main/graph/badge.svg?token=4EZNH1HYAN
         :target: https://codecov.io/gh/ACCESS-NRI/intake-dataframe-catalog
         :alt: Code test coverage
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
```

### Comparing `intake_dataframe_catalog-0.0.8/README.rst` & `intake_dataframe_catalog-0.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 **A simple intake plugin for a searchable table of intake catalogs and associated metadata.**
 
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
-| Package       | |pypi|               |
+| Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI            | |tests| |pre-commit| |
-+---------------+----------------------+
-| CD            | |build|              |
+| CI/CD         | |ci| |cd|            |
 +---------------+----------------------+
 | Development   | |codecov| |black|    |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 Overview
@@ -50,25 +48,25 @@
         :target: https://intake-dataframe-catalog.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
         
 .. |pypi| image:: https://img.shields.io/pypi/v/intake-dataframe-catalog
         :target: https://pypi.org/project/intake-dataframe-catalog/
         :alt: Python Package Index Build
         
-.. |tests| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/tests.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/tests.yml
-        :alt: Package test status
-        
-.. |pre-commit| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/pre-commit.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/pre-commit.yml
-        :alt: Package pre-commit status
-        
-.. |build| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/release.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/release.yml
-        :alt: Build distribution status
+.. |conda| image:: https://anaconda.org/accessnri/intake-dataframe-catalog/badges/version.svg
+        :target: https://anaconda.org/accessnri/intake-dataframe-catalog
+        :alt: Conda Build
+
+.. |ci| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/ci.yml
+        :alt: Package CI test status
+        
+.. |cd| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/cd.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/cd.yml
+        :alt: Package CD status
         
 .. |codecov| image:: https://codecov.io/gh/ACCESS-NRI/intake-dataframe-catalog/branch/main/graph/badge.svg?token=4EZNH1HYAN
         :target: https://codecov.io/gh/ACCESS-NRI/intake-dataframe-catalog
         :alt: Code test coverage
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
```

### Comparing `intake_dataframe_catalog-0.0.8/pyproject.toml` & `intake_dataframe_catalog-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -43,8 +43,55 @@
 tag_prefix = "v"
 parentdir_prefix = "intake-dataframe-catalog-"
 
 [tool.coverage.run]
 omit = [
     "src/intake_dataframe_catalog/_version.py",
 ]
-  
+
+[tool.ruff]
+target-version = "py39"
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
+# E402: module level import not at top of file
+# E501: line too long - let black worry about that
+ignore = [
+    "E402",
+    "E501",
+]
+select = [
+    # Pyflakes
+    "F",
+    # Pycodestyle
+    "E",
+    "W",
+    # isort
+    "I",
+    # Pyupgrade
+    "UP",
+]
+
+[tool.ruff.mccabe]
+max-complexity = 18
+
+[tool.ruff.isort]
+known-first-party = ["intake_dataframe_catalog"]
+
```

### Comparing `intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog/_search.py` & `intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog/_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
 # Stolen and adapted from https://github.com/intake/intake-esm/blob/main/intake_esm/_search.py
 
+import itertools
 import re
 import typing
-import itertools
 
 import numpy as np
 import pandas as pd
 
 
 def _is_pattern(value: typing.Union[str, typing.Pattern]) -> bool:
     """
@@ -28,15 +28,17 @@
         for char in wildcard_chars:
             value_ = value_.replace(rf"\{char}", "")
         return any(char in value_ for char in wildcard_chars)
     except (TypeError, AttributeError):
         return False
 
 
-def _match_iterables(strings, pattern, regex):
+def _match_iterables(
+    strings: typing.Union[list, tuple, set], pattern: str, regex: bool
+):
     """
     Given an iterable of strings, return all that match the provided pattern
     as a set.
     """
     matches = []
     for string in strings:
         if regex:
```

### Comparing `intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog/core.py` & `intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
 import ast
-import tlz
 import typing
 import warnings
 from io import UnsupportedOperation
 
-import yaml
 import fsspec
-import pandas as pd
-
 import intake
+import pandas as pd
+import tlz
+import yaml
 from intake.catalog import Catalog
 from intake.catalog.local import LocalCatalogEntry
 
 from . import __version__
 from ._search import search
 
 pd.set_option("display.max_colwidth", 200)
```

### Comparing `intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/PKG-INFO` & `intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-dataframe-catalog
-Version: 0.0.8
+Version: 0.1.0
 Summary: An intake driver for a searchable table of intake catalogs and associated metadata
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -19,19 +19,17 @@
 **A simple intake plugin for a searchable table of intake catalogs and associated metadata.**
 
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
-| Package       | |pypi|               |
+| Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI            | |tests| |pre-commit| |
-+---------------+----------------------+
-| CD            | |build|              |
+| CI/CD         | |ci| |cd|            |
 +---------------+----------------------+
 | Development   | |codecov| |black|    |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 Overview
@@ -64,25 +62,25 @@
         :target: https://intake-dataframe-catalog.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
         
 .. |pypi| image:: https://img.shields.io/pypi/v/intake-dataframe-catalog
         :target: https://pypi.org/project/intake-dataframe-catalog/
         :alt: Python Package Index Build
         
-.. |tests| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/tests.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/tests.yml
-        :alt: Package test status
-        
-.. |pre-commit| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/pre-commit.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/pre-commit.yml
-        :alt: Package pre-commit status
-        
-.. |build| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/release.yml/badge.svg
-        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/release.yml
-        :alt: Build distribution status
+.. |conda| image:: https://anaconda.org/accessnri/intake-dataframe-catalog/badges/version.svg
+        :target: https://anaconda.org/accessnri/intake-dataframe-catalog
+        :alt: Conda Build
+
+.. |ci| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/ci.yml
+        :alt: Package CI test status
+        
+.. |cd| image:: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/cd.yml/badge.svg
+        :target: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/cd.yml
+        :alt: Package CD status
         
 .. |codecov| image:: https://codecov.io/gh/ACCESS-NRI/intake-dataframe-catalog/branch/main/graph/badge.svg?token=4EZNH1HYAN
         :target: https://codecov.io/gh/ACCESS-NRI/intake-dataframe-catalog
         :alt: Code test coverage
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
```

### Comparing `intake_dataframe_catalog-0.0.8/src/intake_dataframe_catalog.egg-info/SOURCES.txt` & `intake_dataframe_catalog-0.1.0/src/intake_dataframe_catalog.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 versioneer.py
 src/intake_dataframe_catalog/__init__.py
 src/intake_dataframe_catalog/_search.py
 src/intake_dataframe_catalog/_version.py
 src/intake_dataframe_catalog/core.py
 src/intake_dataframe_catalog.egg-info/PKG-INFO
```

### Comparing `intake_dataframe_catalog-0.0.8/tests/test_core.py` & `intake_dataframe_catalog-0.1.0/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
 import ast
 from io import UnsupportedOperation
 
+import intake
+import pandas as pd
 import pytest
-
 import xarray as xr
-import pandas as pd
-
-import intake
 from intake.source.csv import CSVSource
 from intake_esm.core import esm_datastore
 
 from intake_dataframe_catalog.core import DfFileCatalog, DfFileCatalogError
 
 
 @pytest.mark.parametrize("mode", ["r", "a", "r+"])
```

### Comparing `intake_dataframe_catalog-0.0.8/tests/test_search.py` & `intake_dataframe_catalog-0.1.0/tests/test_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
 import re
 
-import pytest
-
 import pandas as pd
+import pytest
 
 from intake_dataframe_catalog._search import _is_pattern, search
 
 
 @pytest.mark.parametrize(
     "value, expected",
     [
```

### Comparing `intake_dataframe_catalog-0.0.8/versioneer.py` & `intake_dataframe_catalog-0.1.0/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,22 +305,22 @@
 # pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
 # pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
 # pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
 # pylint:disable=attribute-defined-outside-init,too-many-arguments
 
 import configparser
 import errno
+import functools
 import json
 import os
 import re
 import subprocess
 import sys
 from pathlib import Path
-from typing import Callable, Dict
-import functools
+from typing import Callable
 
 have_tomllib = True
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     try:
         import tomli as tomllib
@@ -414,16 +414,16 @@
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
-LONG_VERSION_PY: Dict[str, str] = {}
-HANDLERS: Dict[str, Dict[str, Callable]] = {}
+LONG_VERSION_PY: dict[str, str] = {}
+HANDLERS: dict[str, dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
 
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
@@ -464,15 +464,15 @@
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
-            print("unable to find command, tried %s" % (commands,))
+            print(f"unable to find command, tried {commands}")
         return None, None
     stdout = process.communicate()[0].strip().decode()
     if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
@@ -1147,15 +1147,15 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        with open(versionfile_abs, "r") as fobj:
+        with open(versionfile_abs) as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
                 if line.strip().startswith("git_full ="):
                     mo = re.search(r'=\s*"(.*)"', line)
@@ -1349,15 +1349,15 @@
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+            pieces["error"] = "tag '{}' doesn't start with prefix '{}'".format(
                 full_tag,
                 tag_prefix,
             )
             return pieces
         pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
@@ -1401,15 +1401,15 @@
                 my_path = os.path.splitext(my_path)[0] + ".py"
             versioneer_file = os.path.relpath(my_path)
         except NameError:
             versioneer_file = "versioneer.py"
         files.append(versioneer_file)
     present = False
     try:
-        with open(".gitattributes", "r") as fobj:
+        with open(".gitattributes") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
                         break
     except OSError:
         pass
@@ -1490,15 +1490,15 @@
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
-    print("set %s to '%s'" % (filename, versions["version"]))
+    print("set {} to '{}'".format(filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
@@ -1795,15 +1795,15 @@
             return ver
         except NotThisMethod:
             pass
 
     try:
         ver = versions_from_file(versionfile_abs)
         if verbose:
-            print("got version from file %s %s" % (versionfile_abs, ver))
+            print(f"got version from file {versionfile_abs} {ver}")
         return ver
     except NotThisMethod:
         pass
 
     from_vcs_f = handlers.get("pieces_from_vcs")
     if from_vcs_f:
         try:
@@ -2183,15 +2183,15 @@
                 "VERSIONFILE_SOURCE": cfg.versionfile_source,
             }
         )
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
-            with open(ipy, "r") as f:
+            with open(ipy) as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
         snippet = INIT_PY_SNIPPET.format(module)
         if OLD_SNIPPET in old:
             print(" replacing boilerplate in %s" % ipy)
@@ -2215,15 +2215,15 @@
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
-    with open("setup.py", "r") as f:
+    with open("setup.py") as f:
         for line in f.readlines():
             if "import versioneer" in line:
                 found.add("import")
             if "versioneer.get_cmdclass()" in line:
                 found.add("cmdclass")
             if "versioneer.get_version()" in line:
                 found.add("get_version")
```

