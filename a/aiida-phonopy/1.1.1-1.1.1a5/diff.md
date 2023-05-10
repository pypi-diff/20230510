# Comparing `tmp/aiida-phonopy-1.1.1.tar.gz` & `tmp/aiida-phonopy-1.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-phonopy-1.1.1.tar", last modified: Wed May 10 12:29:28 2023, max compression
+gzip compressed data, was "aiida-phonopy-1.1.1a5.tar", last modified: Fri May  5 10:22:11 2023, max compression
```

## Comparing `aiida-phonopy-1.1.1.tar` & `aiida-phonopy-1.1.1a5.tar`

### file list

```diff
@@ -1,49 +1,46 @@
--rw-r--r--   0        0        0     6148 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/.DS_Store
--rw-r--r--   0        0        0     3763 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2397 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1512 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/.github/workflows/validate_release_tag.py
--rw-r--r--   0        0        0      501 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/.gitignore
--rw-r--r--   0        0        0     1034 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      300 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/.readthedocs.yml
--rw-r--r--   0        0        0     4299 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1085 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1816 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/README.md
--rw-r--r--   0        0        0      155 2023-05-10 12:29:22.971444 aiida-phonopy-1.1.1/docker-compose.yml
--rw-r--r--   0        0        0      455 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/environment.yml
--rw-r--r--   0        0        0    52380 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/FORCE_SETS
--rw-r--r--   0        0        0    21945 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/phonopy.yaml
--rw-r--r--   0        0        0    52380 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/FORCE_SETS
--rw-r--r--   0        0        0       41 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/aiida.in
--rw-r--r--   0        0        0     1538 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/aiida.out
--rw-r--r--   0        0        0    58620 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/band.hdf5
--rw-r--r--   0        0        0    43797 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/force_constants.hdf5
--rw-r--r--   0        0        0     2445 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/irreps.yaml
--rw-r--r--   0        0        0    39220 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/mesh.hdf5
--rw-r--r--   0        0        0    21837 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/phonopy.yaml
--rw-r--r--   0        0        0     2336 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/qpoints.hdf5
--rw-r--r--   0        0        0    33644 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/thermal_properties.yaml
--rw-r--r--   0        0        0     1254 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/BaTiO3/script.py
--rw-r--r--   0        0        0    49210 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/examples/Si/preprocess.ipynb
--rw-r--r--   0        0        0     3514 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       91 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/calculations/__init__.py
--rw-r--r--   0        0        0       62 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/calculations/functions/__init__.py
--rw-r--r--   0        0        0    10711 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/calculations/functions/data_utils.py
--rw-r--r--   0        0        0     4037 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/calculations/functions/link_structures.py
--rw-r--r--   0        0        0    18250 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/calculations/phonopy.py
--rw-r--r--   0        0        0      271 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/data/__init__.py
--rw-r--r--   0        0        0     4298 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/data/force_constants.py
--rw-r--r--   0        0        0    10128 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/data/phonopy.py
--rw-r--r--   0        0        0    13397 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/data/preprocess.py
--rw-r--r--   0        0        0    21571 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/data/raw.py
--rw-r--r--   0        0        0       65 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/parsers/__init__.py
--rw-r--r--   0        0        0     2450 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/parsers/base.py
--rw-r--r--   0        0        0    18608 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/parsers/phonopy.py
--rw-r--r--   0        0        0        0 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/parsers/raw_parsers/__init__.py
--rw-r--r--   0        0        0     1080 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/parsers/raw_parsers/phonopy.py
--rw-r--r--   0        0        0        0 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/utils/__init__.py
--rw-r--r--   0        0        0     2138 2023-05-10 12:29:22.987444 aiida-phonopy-1.1.1/src/aiida_phonopy/utils/mapping.py
--rw-r--r--   0        0        0      688 2023-05-10 12:29:22.991444 aiida-phonopy-1.1.1/src/aiida_phonopy/utils/resources.py
--rw-r--r--   0        0        0        0 2023-05-10 12:29:22.991444 aiida-phonopy-1.1.1/src/aiida_phonopy/workflows/__init__.py
--rw-r--r--   0        0        0    15542 2023-05-10 12:29:22.991444 aiida-phonopy-1.1.1/src/aiida_phonopy/workflows/phonopy.py
--rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 aiida-phonopy-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3763 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2397 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1512 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0      392 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.gitignore
+-rw-r--r--   0        0        0     1034 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      239 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.readthedocs.yml
+-rw-r--r--   0        0        0     4028 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/CHANGELOG.md
+-rw-r--r--   0        0        0     1085 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/LICENSE.txt
+-rw-r--r--   0        0        0     1816 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/README.md
+-rw-r--r--   0        0        0      155 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/docker-compose.yml
+-rw-r--r--   0        0        0    52380 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/FORCE_SETS
+-rw-r--r--   0        0        0    21945 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/phonopy.yaml
+-rw-r--r--   0        0        0    52380 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/FORCE_SETS
+-rw-r--r--   0        0        0       41 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/aiida.in
+-rw-r--r--   0        0        0     1538 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/aiida.out
+-rw-r--r--   0        0        0    58620 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/band.hdf5
+-rw-r--r--   0        0        0    43797 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/force_constants.hdf5
+-rw-r--r--   0        0        0     2445 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/irreps.yaml
+-rw-r--r--   0        0        0    39220 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/mesh.hdf5
+-rw-r--r--   0        0        0    21837 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/phonopy.yaml
+-rw-r--r--   0        0        0     2336 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/qpoints.hdf5
+-rw-r--r--   0        0        0    33644 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/thermal_properties.yaml
+-rw-r--r--   0        0        0     1254 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/script.py
+-rw-r--r--   0        0        0     3220 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/__init__.py
+-rw-r--r--   0        0        0    10762 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/data_utils.py
+-rw-r--r--   0        0        0     4037 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/link_structures.py
+-rw-r--r--   0        0        0    18068 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/phonopy.py
+-rw-r--r--   0        0        0      271 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/__init__.py
+-rw-r--r--   0        0        0     4299 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/force_constants.py
+-rw-r--r--   0        0        0    10147 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/phonopy.py
+-rw-r--r--   0        0        0    13302 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/preprocess.py
+-rw-r--r--   0        0        0    21446 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/raw.py
+-rw-r--r--   0        0        0       65 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/__init__.py
+-rw-r--r--   0        0        0     2450 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/base.py
+-rw-r--r--   0        0        0    18608 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/phonopy.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/raw_parsers/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/raw_parsers/phonopy.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/__init__.py
+-rw-r--r--   0        0        0     2138 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/mapping.py
+-rw-r--r--   0        0        0      688 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/resources.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/workflows/__init__.py
+-rw-r--r--   0        0        0    15542 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/workflows/phonopy.py
+-rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 aiida-phonopy-1.1.1a5/PKG-INFO
```

### Comparing `aiida-phonopy-1.1.1/.github/workflows/cd.yml` & `aiida-phonopy-1.1.1a5/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/.github/workflows/ci.yml` & `aiida-phonopy-1.1.1a5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/.github/workflows/validate_release_tag.py` & `aiida-phonopy-1.1.1a5/.github/workflows/validate_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/.pre-commit-config.yaml` & `aiida-phonopy-1.1.1a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/CHANGELOG.md` & `aiida-phonopy-1.1.1a5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 # Changelog
 
-## v1.1.1 - 2023-05-10
-
-[full changelog](https://github.com/aiida-phonopy/aiida-phonopy/compare/v1.1.1...v1.1.0)
-
-This release comes with some bug fixes of the previous version for data storage,
-it improves the docstrings and typing, and finally adds the documentation.
-
 ## v1.1.0 - 2023-05-02
 
 [full changelog](https://github.com/aiida-phonopy/aiida-phonopy/compare/v1.1.0...v1.0.0)
 
 In this release we apply some improvements in the way the data is stored, and refactor the calculation utils to make names shorter and more comprehensible.
 
 ## v1.0.0 - 2022-11-0X
```

### Comparing `aiida-phonopy-1.1.1/LICENSE.txt` & `aiida-phonopy-1.1.1a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/README.md` & `aiida-phonopy-1.1.1a5/README.md`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/FORCE_SETS` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/phonopy.yaml` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/FORCE_SETS` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/aiida.out` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/aiida.out`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/band.hdf5` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/band.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/force_constants.hdf5` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/force_constants.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/irreps.yaml` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/irreps.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/mesh.hdf5` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/mesh.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/phonopy.yaml` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/qpoints.hdf5` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/qpoints.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/ref_out/thermal_properties.yaml` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/thermal_properties.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/examples/BaTiO3/script.py` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/script.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/pyproject.toml` & `aiida-phonopy-1.1.1a5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -42,28 +42,19 @@
 ]
 tests = [
     'pgtest~=1.3',
     'pytest~=6.0',
     'pytest-regressions~=2.3',
 ]
 docs = [
-    'myst-nb~=0.17',
-    'jupytext>=1.11.2,<1.15.0',
-    # 'sphinx-book-theme==1.0.0rc2',
-    # 'sphinx-design2',
-    # 'sphinx-autodoc2~=0.4.2',
-    'sphinx-togglebutton',
-    'sphinx~=5.2',
-    'sphinx-copybutton~=0.5.2',
-    'sphinx-book-theme~=1.0.1',
-    # 'sphinx-click~=4.4.0',
-    'sphinx-design~=0.4.1',
-    'sphinxcontrib-details-directive~=0.1.0',
-    'sphinx-autoapi~=2.0.1',
-    #'myst_parser~=1.0.0',
+    "Sphinx",
+    "docutils",
+    "sphinx-copybutton~=0.3.0",
+    "sphinx-book-theme~=0.1.0",
+    "sphinx-click~=2.7.1",
 ]
 
 [project.entry-points.'aiida.data']
 'phonopy.raw' = 'aiida_phonopy.data.raw:RawData'
 'phonopy.preprocess' = 'aiida_phonopy.data.preprocess:PreProcessData'
 'phonopy.phonopy' = 'aiida_phonopy.data.phonopy:PhonopyData'
 'phonopy.force_constants' = 'aiida_phonopy.data.force_constants:ForceConstantsData'
```

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/calculations/functions/data_utils.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/data_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 # -*- coding: utf-8 -*-
 """Calcfunctions Utils for aiida-phonopy DataTypes."""
 from __future__ import annotations
 
 from aiida import orm
 from aiida.engine import calcfunction
-from aiida.plugins import DataFactory
+
+from aiida_phonopy.data import PhonopyData, PreProcessData
 
 __all__ = (
     'get_unitcell', 'get_primitive', 'get_supercell', 'get_supercells_with_displacements', 'get_displacements',
     'get_preprocess_with_new_displacements', 'generate_preprocess_data', 'generate_phonopy_data', 'CalcfunctionMixin'
 )
 
 
 @calcfunction
-def get_unitcell(preprocess_data) -> orm.StructureData:
+def get_unitcell(preprocess_data: PreProcessData) -> orm.StructureData:
     """Get the unitcell of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_unitcell()
     return structure_data
 
 
 @calcfunction
-def get_primitive(preprocess_data) -> orm.StructureData:
+def get_primitive(preprocess_data: PreProcessData) -> orm.StructureData:
     """Get the primitive cell of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_primitive_cell()
     return structure_data
 
 
 @calcfunction
-def get_supercell(preprocess_data) -> orm.StructureData:
+def get_supercell(preprocess_data: PreProcessData) -> orm.StructureData:
     """Get the supercell (pristine) of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_supercell()
     return structure_data
 
 
 @calcfunction
-def get_supercells_with_displacements(preprocess_data) -> dict:
+def get_supercells_with_displacements(preprocess_data: PreProcessData) -> dict[orm.StructureData]:
     """Get the supercells with displacements of a PreProcessData as a StructureData."""
     structures_data = preprocess_data.get_supercells_with_displacements()
     return structures_data
 
 
 @calcfunction
-def get_displacements(preprocess_data) -> orm.ArrayData:
+def get_displacements(preprocess_data: PreProcessData) -> orm.ArrayData:
     """Get the displacements of a PreProcessData as an ArrayData with array name `displacements`."""
     displacements = preprocess_data.get_displacements()
     the_displacements = orm.ArrayData()
     the_displacements.set_array('displacements', displacements)
 
     return the_displacements
 
@@ -59,31 +60,30 @@
     symprec: orm.Float | None = None,
     is_symmetry: orm.Float | None = None,
     distinguish_kinds: orm.Bool | None = None,
 ):
     """Return a complete stored PreProcessData node.
 
     :param structure: structure data node representing the unitcell
-    :type structure: :class:`~aiida.orm.StructureData`
+    :type structure: orm.StructureData
     :param displacement_generator: dictionary containing the info for generating the displacements
-    :type displacement_generator: :class:`~aiida.orm.Dict`
+    :type displacement_generator: orm.Dict
     :param supercell_matrix: supercell matrix, defaults to diag(1,1,1)
-    :type supercell_matrix: :class:`~aiida.orm.List`, Optional
+    :type supercell_matrix: orm.List, optional
     :param primitive_matrix: primitive matrix, defaults to "auto"
-    :type primitive_matrix: :class:`~aiida.orm.List`, Optional
+    :type primitive_matrix: orm.List or orm.List, optional
     :param symprec: symmetry precision on atoms, defaults to 1e-5
-    :type symprec: :class:`~aiida.orm.Float`, Optional
+    :type symprec: orm.Float, optional
     :param is_symmetry: if using space group symmetry, defaults to True
-    :type is_symmetry: :class:`~aiida.orm.Bool`, Optional
+    :type is_symmetry: orm.Bool, optional
     :param distinguish_kinds: if distinguish names of same specie by symmetry, defaults to True
-    :type distinguish_kinds: :class:`~aiida.orm.Bool`, Optional
+    :type distinguish_kinds: orm.Bool, optional
 
     :return: PreProcessData node
     """
-    PreProcessData = DataFactory('phonopy.preprocess')
     kwargs = {}
 
     kwargs['structure'] = structure
 
     if displacement_generator is not None:
         displ_generator = displacement_generator.get_dict()
     else:
@@ -122,17 +122,18 @@
 
     preprocess.set_displacements(**displ_generator)
 
     return preprocess
 
 
 @calcfunction
-def get_preprocess_with_new_displacements(preprocess_data, displacement_generator: orm.Dict):
+def get_preprocess_with_new_displacements(
+    preprocess_data: PreProcessData, displacement_generator: orm.Dict
+) -> PreProcessData:
     """Get a new PreProcessData from an old one from new displacement generator settings."""
-    PreProcessData = DataFactory('phonopy.preprocess')
     displacement_dataset = preprocess_data.generate_displacement_dataset(**displacement_generator.get_dict())
 
     preprocess = PreProcessData(
         structure=preprocess_data.get_unitcell(),
         supercell_matrix=preprocess_data.supercell_matrix,
         primitive_matrix=preprocess_data.primitive_matrix,
         symprec=preprocess_data.symprec,
@@ -143,16 +144,19 @@
     preprocess.set_displacements_from_dataset(displacement_dataset)
 
     return preprocess
 
 
 @calcfunction
 def generate_phonopy_data(
-    preprocess_data, nac_parameters: orm.ArrayData | None = None, forces_index: orm.Int | None = None, **forces_dict
-):
+    preprocess_data: PreProcessData,
+    nac_parameters: orm.ArrayData | None = None,
+    forces_index: orm.Int | None = None,
+    **forces_dict
+) -> PhonopyData:
     """Create a PhonopyData node from a PreProcess(Phonopy)Data node.
 
     `Forces` must be passed as **kwargs**, since we are calling a calcfunction with a variable
     number of supercells forces.
 
     :param nac_parameters: ArrayData containing 'dielectric' and 'born_charges' as arrays
         with their correct shape
@@ -167,15 +171,14 @@
             <==>
             {'supercell_1':StructureData, 'supercell_2':StructureData}
             and forces in each ArrayData stored as 'forces',
             i.e. ArrayData.get_array('forces') must not raise error
 
         .. note: if residual forces would be stored, label it with 0 as suffix.
     """
-    PhonopyData = DataFactory('phonopy.phonopy')
     prefix = 'forces'
 
     forces_0 = forces_dict.pop(f'{prefix}_0', None)
     # Setting the dictionary of forces
     dict_of_forces = {}
 
     for key, value in forces_dict.items():
@@ -198,15 +201,15 @@
 
     return new_phonopy_data
 
 
 class CalcfunctionMixin:
     """Set of calcfunctions to be called from the aiida-phonopy DataTypes."""
 
-    def __init__(self, data_node):
+    def __init__(self, data_node: PreProcessData | PhonopyData):
         """Instantiate the class."""
         self._data_node = data_node
 
     def get_unitcell(self) -> orm.StructureData:
         """Get the unitcell as a StructureData through a calfunction."""
         return get_unitcell(preprocess_data=self._data_node)
 
@@ -214,34 +217,37 @@
         """Get the primitive cell as a StructureData through a calfunction."""
         return get_primitive(preprocess_data=self._data_node)
 
     def get_supercell(self) -> orm.StructureData:
         """Get the supercell (pristine) as a StructureData through a calfunction."""
         return get_supercell(preprocess_data=self._data_node)
 
-    def get_supercells_with_displacements(self) -> dict:
+    def get_supercells_with_displacements(self) -> dict[orm.StructureData]:
         """Get the supercells with displacements as a StructureData through a calfunction."""
         return get_supercells_with_displacements(preprocess_data=self._data_node)
 
     def get_displacements(self) -> orm.ArrayData:
         """Get the displacements as an ArrayData through a calfunction."""
         return get_displacements(preprocess_data=self._data_node)
 
-    def get_preprocess_with_new_displacements(self, displacement_generator: orm.Dict):
+    def get_preprocess_with_new_displacements(self, displacement_generator: orm.Dict) -> PreProcessData:
         """Create a PreProcessData node from a PreProcess/PhonopyData with a new set of displacements.
 
         :param displacement_generator: a `storable` dictionary
         """
         return get_preprocess_with_new_displacements(
             preprocess_data=self._data_node, displacement_generator=displacement_generator
         )
 
     def generate_phonopy_data(
-        self, nac_parameters: orm.ArrayData | None = None, forces_index: orm.Int | None = None, **forces_dict
-    ):
+        self,
+        nac_parameters: orm.ArrayData | None = None,
+        forces_index: orm.Int | None = None,
+        **forces_dict
+    ) -> PhonopyData:
         """Create a PhonopyData node from a PreProcess(Phonopy)Data node.
 
         `Forces` must be passed as **kwargs**, since we are calling a calcfunction with a variable
         number of supercells forces.
 
         :param nac_parameters: ArrayData containing 'dielectric' and 'born_charges' as arrays
             with their correct shape
```

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/calculations/functions/link_structures.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/link_structures.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/calculations/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/phonopy.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,21 +396,18 @@
 
     def write_calculation_input(self, folder, parameters: dict, filename: str):
         """Write in `folder` the input file containing the information regarding the calculation."""
         characters = []  # single characters to be written
 
         # appending eventual blocked keys to parameters
         if 'force_constants' in self.inputs:
-            parameters.update({'FORCE_CONSTANTS': 'READ'})
-            if self.inputs.force_constants.has_nac_parameters():
-                parameters.setdefault('NAC', True)
+            parameters.append({'FORCE_CONSTANTS': 'READ'})
 
-        if 'phonopy_data' in self.inputs:
-            if self.inputs.phonopy_data.has_nac_parameters():
-                parameters.setdefault('NAC', True)
+        if 'nac_parameters' in self.inputs:
+            parameters.append({'NAC': True})
 
         # if not "SYMMETRY_TOLERANCE" in parameters.keys():
         #     symprec = self.inputs.phonopy_data.symprec
         #     parameters.update({"SYMMETRY_TOLERANCE":symprec})
 
         # write potential huge outputs in `.hdf5` format, and read force constants from this format too
         parameters.update({'HDF5': True})
```

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/data/force_constants.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/force_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         **kwargs
     ):
         """Instantiate the class.
 
         The minimal input is to define either the `structure` or the `phonopy_atoms` input.
         They cannot be specified at the same time.
 
-        :param structure: a :class:`~aiida.orm.StructureData` node
+        :param structure: an :class:`~aiida.orm.StructureData` node
         :param phononpy_atoms: a :class:`~phonopy.structure.cells.PhonopyAtoms` instance
         :param supercell_matrix: a (3,3) shape array describing the supercell transformation
         :param primitive_matrix: a (3,3) shape array describing the primite transformation
         :param symprec: precision tollerance for symmetry analysis
         :param is_symmetry: whether using symmetries
         :distinguish_kinds: it stores a mapping between kinds and chemical symbols;
             by default Phonopy does not support kind,
```

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/data/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/phonopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         """Set displacements cannot be accessed from PhonopyData."""
         raise RuntimeError('`displacements` cannot be changed for this Data')
 
     def get_phonopy_instance(self, subtract_residual_forces: bool | None = None, **kwargs) -> Phonopy:
         """Return a :class:`~phonopy.Phonopy` object with forces and nac parameters (if set).
 
         :param subtract_residual_forces: whether or not subract residual forces (if set)
-        :type subtract_residual_forces: bool
+        :type subtract_residual_forces: bool, defaults to False
         :param kwargs: see :func:`aiida_phonopy.data.preprocess.PreProcessData.get_phonopy_instance`
             * symmetrize_nac: whether or not to symmetrize the nac parameters
                 using point group symmetry; bool, defaults to self.is_symmetry
             * factor_nac: factor for non-analytical corrections;
                 float, defaults to Hartree*Bohr
         """
         if not isinstance(subtract_residual_forces, bool) and subtract_residual_forces is not None:
```

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/data/preprocess.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,19 +175,18 @@
             raise ValueError('type not accepted')
 
         self._set_displacements(_serialize(copy.deepcopy(ph.dataset)))
 
     def get_phonopy_instance(self, symmetrize_nac: bool = None, factor_nac: float | None = None, **kwargs):
         """Return a :class:`~phonopy.Phonopy` object with the current values.
 
-        :param symmetrize_nac: whether or not to symmetrize the nac parameters using point group symmetry;
-            defaults to self.is_symmetry
-        :type symmetrize_nac: bool
-        :param factor_nac: factor for non-analytical corrections; defaults to Hartree*Bohr
-        :type factor_nac: float
+        :param symmetrize_nac: whether or not to symmetrize the nac parameters using point group symmetry.
+        :type symmetrize_nac: bool, defaults to self.is_symmetry
+        :param factor_nac: factor for non-analytical corrections
+        :type factor_nac: float, defaults to Hartree*Bohr
         :param kwargs: for internal use to set the primitive cell
         """
         ph = super().get_phonopy_instance(symmetrize_nac, factor_nac, **kwargs)
         if self.displacement_dataset is not None:
             ph.dataset = self.displacement_dataset
         return ph
 
@@ -268,28 +267,28 @@
         symprec: float | None = None,
         is_symmetry: bool | None = None,
         distinguish_kinds: bool | None = None,
     ):
         """Return a complete stored PreProcessData node.
 
         :param structure: structure data node representing the unitcell
-        :type structure: :class:`~aiida.orm.StructureData`
+        :type structure: orm.StructureData
         :param displacement_generator: dictionary containing the info for generating the displacements,
             defaults to phonopy default (see phonopy doc)
         :type displacement_generator: orm.Dict
         :param supercell_matrix: supercell matrix, defaults to diag(1,1,1)
-        :type supercell_matrix: :class:`~aiida.orm.List`, Optional
+        :type supercell_matrix: orm.List, optional
         :param primitive_matrix: primitive matrix, defaults to "auto"
-        :type primitive_matrix: :class:`~aiida.orm.List`, Optional
+        :type primitive_matrix: orm.List or orm.List, optional
         :param symprec: symmetry precision on atoms, defaults to 1e-5
-        :type symprec: :class:`~aiida.orm.Float`, Optional
+        :type symprec: orm.Float, optional
         :param is_symmetry: if using space group symmetry, defaults to True
-        :type is_symmetry: :class:`~aiida.orm.Bool`, Optional
+        :type is_symmetry: orm.Bool, optional
         :param distinguish_kinds: if distinguish names of same specie by symmetry, defaults to True
-        :type distinguish_kinds: :class:`~aiida.orm.Bool`, Optional
+        :type distinguish_kinds: orm.Bool, optional
 
         :return: PreProcessData node
         """
         from aiida_phonopy.calculations.functions.data_utils import generate_preprocess_data
 
         kwargs = {}
```

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/data/raw.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 
 
 def _get_valid_matrix(matrix: list | np.ndarray) -> np.ndarray:
     """Get and validate the `supercell_matrix` and `primitive_matrix` inputs.
 
     :param matrix: (3,1) or (3,3) shape array
-    :type matrix: :class:`list`, :class:`~aiida.orm.List`, :class:`numpy.ndarray`
+    :type matrix: list, orm.List, numpy.ndarray
     :return: a (3,3) numpy.ndarray
     :raises:
         * TypeError: if it is not a valid array type and if the array does not contain only numbers
         * ValueError: if the array is not of the correct shape
     """
     if not isinstance(matrix, (list, orm.List, np.ndarray)):
         raise TypeError("only `list`, `aiida.orm.List` and `numpy.ndarray` (and 'auto' as string for primitive)")
@@ -240,15 +240,15 @@
         """
         return self.base.attributes.get('supercell_matrix')
 
     def _set_supercell_matrix(self, value: list | np.ndarray):
         """Set the Phonopy supercell matrix.
 
         :param value: (3,3) or (3,1) shape array
-        :type value: :class:`list`, :class:`~aiida.orm.List`, :class:`numpy.ndarray`
+        :type value: list, orm.List, numpy.ndarray
 
         :raises ModificationNotAllowed: if object is already stored
         """
         self._if_can_modify()
         the_supercell_matrix = _get_valid_matrix(value)
 
         self.base.attributes.set('supercell_matrix', deepcopy(the_supercell_matrix))
@@ -260,16 +260,16 @@
         :return: a (3,3) shape array
         """
         return self.base.attributes.get('primitive_matrix')
 
     def _set_primitive_matrix(self, value: list | np.ndarray):
         """Set the primitive matrix.
 
-        :param value: (3,3) or (3,1) shape array, or 'auto"
-        :type value: :class:`list`, :class:`~aiida.orm.List`, :class:`numpy.ndarray`, :class:`str`
+        :param value: (3,3) or (3,1) shape array, or str
+        :type value: list, orm.List, numpy.ndarray, str
         :raises ModificationNotAllowed: if object is already stored
         """
         self._if_can_modify()
 
         if isinstance(value, str):
             the_primitive_matrix = self.get_phonopy_instance(**{'primitive': value}).primitive_matrix
         else:
@@ -374,19 +374,18 @@
         return PhonopyAtoms(**kwargs)
 
     def get_phonopy_instance(
         self, symmetrize_nac: bool | None = None, factor_nac: float | None = None, **kwargs
     ) -> Phonopy:
         """Return a :py:class:`phonopy.Phonopy` object with the current values.
 
-        :param symmetrize_nac: whether or not to symmetrize the nac parameters using point group symmetry;
-            defaults to self.is_symmetry
-        :type symmetrize_nac: bool
-        :param factor_nac: factor for non-analytical corrections; defaults to Hartree*Bohr
-        :type factor_nac: float
+        :param symmetrize_nac: whether or not to symmetrize the nac parameters using point group symmetry.
+        :type symmetrize_nac: bool, defaults to self.is_symmetry
+        :param factor_nac: factor for non-analytical corrections
+        :type factor_nac: float, defaults to Hartree*Bohr
         :param kwargs: for internal use to set the primitive cell
         """
         from phonopy.structure.symmetry import symmetrize_borns_and_epsilon
         from phonopy.units import Bohr, Hartree
 
         distinguish = kwargs.pop('distinguish', self.distinguish_kinds)
         unitcell = self._get_phonopy_atoms_unitcell(distinguish)
```

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/parsers/base.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/base.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/parsers/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/parsers/raw_parsers/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/raw_parsers/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/utils/mapping.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/utils/resources.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/resources.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/src/aiida_phonopy/workflows/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/workflows/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.1/PKG-INFO` & `aiida-phonopy-1.1.1a5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-phonopy
-Version: 1.1.1
+Version: 1.1.1a5
 Summary: The official AiiDA plugin for Phonopy
 Keywords: aiida,phonopy,workflows
 Author-email: Lorenzo Bastonero <bastonero.lorenzo@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -14,23 +14,19 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Dist: aiida-core>=2.0.0,<3.0.0
 Requires-Dist: phonopy>=2.14,<3.0.0
-Requires-Dist: myst-nb~=0.17 ; extra == "docs"
-Requires-Dist: jupytext>=1.11.2,<1.15.0 ; extra == "docs"
-Requires-Dist: sphinx-togglebutton ; extra == "docs"
-Requires-Dist: sphinx~=5.2 ; extra == "docs"
-Requires-Dist: sphinx-copybutton~=0.5.2 ; extra == "docs"
-Requires-Dist: sphinx-book-theme~=1.0.1 ; extra == "docs"
-Requires-Dist: sphinx-design~=0.4.1 ; extra == "docs"
-Requires-Dist: sphinxcontrib-details-directive~=0.1.0 ; extra == "docs"
-Requires-Dist: sphinx-autoapi~=2.0.1 ; extra == "docs"
+Requires-Dist: Sphinx ; extra == "docs"
+Requires-Dist: docutils ; extra == "docs"
+Requires-Dist: sphinx-copybutton~=0.3.0 ; extra == "docs"
+Requires-Dist: sphinx-book-theme~=0.1.0 ; extra == "docs"
+Requires-Dist: sphinx-click~=2.7.1 ; extra == "docs"
 Requires-Dist: pre-commit~=2.17 ; extra == "pre-commit"
 Requires-Dist: pylint==2.17.2 ; extra == "pre-commit"
 Requires-Dist: pylint-aiida~=0.1.1 ; extra == "pre-commit"
 Requires-Dist: toml ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3 ; extra == "tests"
 Requires-Dist: pytest~=6.0 ; extra == "tests"
 Requires-Dist: pytest-regressions~=2.3 ; extra == "tests"
```

