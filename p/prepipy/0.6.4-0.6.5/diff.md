# Comparing `tmp/prepipy-0.6.4.tar.gz` & `tmp/prepipy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepipy-0.6.4.tar", max compression
+gzip compressed data, was "prepipy-0.6.5.tar", max compression
```

## Comparing `prepipy-0.6.4.tar` & `prepipy-0.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35823 2022-09-29 09:47:18.805206 prepipy-0.6.4/LICENSE
--rw-r--r--   0        0        0     1104 2023-04-28 17:17:22.866742 prepipy-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     6507 2023-04-28 17:16:37.889028 prepipy-0.6.4/README.md
--rw-r--r--   0        0        0        0 2023-04-23 11:55:03.000536 prepipy-0.6.4/src/prepipy/__init__.py
--rw-r--r--   0        0        0     7617 2023-04-23 23:11:52.299277 prepipy-0.6.4/src/prepipy/auxiliaries.py
--rw-r--r--   0        0        0     1291 2023-03-22 14:05:29.668486 prepipy-0.6.4/src/prepipy/config/config_comments.yml
--rw-r--r--   0        0        0      870 2023-04-23 23:31:32.143543 prepipy-0.6.4/src/prepipy/config/logging_config.yml
--rw-r--r--   0        0        0      549 2023-03-30 22:08:20.988049 prepipy-0.6.4/src/prepipy/config/masking_example.yml
--rw-r--r--   0        0        0     1565 2023-03-31 09:38:15.114796 prepipy-0.6.4/src/prepipy/config_file_examples/bands.yml
--rw-r--r--   0        0        0     1736 2023-03-31 09:38:15.114796 prepipy-0.6.4/src/prepipy/config_file_examples/config_single.yml
--rw-r--r--   0        0        0      184 2023-03-31 09:38:15.114796 prepipy-0.6.4/src/prepipy/config_file_examples/mask.yml
--rw-r--r--   0        0        0     3535 2023-03-31 09:38:20.474789 prepipy-0.6.4/src/prepipy/configuration.py
--rw-r--r--   0        0        0    47850 2023-04-23 23:11:35.981625 prepipy-0.6.4/src/prepipy/framework.py
--rw-r--r--   0        0        0     7094 2023-04-23 18:55:59.195121 prepipy-0.6.4/src/prepipy/framework_sources.py
--rw-r--r--   0        0        0     2502 2023-04-23 23:11:23.068772 prepipy-0.6.4/src/prepipy/masking.py
--rw-r--r--   0        0        0       68 2023-03-31 21:09:47.636364 prepipy-0.6.4/src/prepipy/resources/grey_values.yml
--rw-r--r--   0        0        0     1044 2023-03-12 22:50:46.683730 prepipy-0.6.4/src/prepipy/resources/html_templates.yml
--rw-r--r--   0        0        0      468 2023-03-12 22:50:46.685849 prepipy-0.6.4/src/prepipy/resources/stiff_params.yml
--rw-r--r--   0        0        0    19395 2023-04-23 23:11:12.370453 prepipy-0.6.4/src/prepipy/rgbcombo.py
--rw-r--r--   0        0        0     7831 1970-01-01 00:00:00.000000 prepipy-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-09-29 09:47:18.805206 prepipy-0.6.5/LICENSE
+-rw-r--r--   0        0        0     1104 2023-05-10 08:57:23.368043 prepipy-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     6507 2023-04-28 17:16:37.889028 prepipy-0.6.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 11:55:03.000536 prepipy-0.6.5/src/prepipy/__init__.py
+-rw-r--r--   0        0        0     7617 2023-04-23 23:11:52.299277 prepipy-0.6.5/src/prepipy/auxiliaries.py
+-rw-r--r--   0        0        0     1291 2023-03-22 14:05:29.668486 prepipy-0.6.5/src/prepipy/config/config_comments.yml
+-rw-r--r--   0        0        0      870 2023-04-23 23:31:32.143543 prepipy-0.6.5/src/prepipy/config/logging_config.yml
+-rw-r--r--   0        0        0      549 2023-03-30 22:08:20.988049 prepipy-0.6.5/src/prepipy/config/masking_example.yml
+-rw-r--r--   0        0        0     1565 2023-03-31 09:38:15.114796 prepipy-0.6.5/src/prepipy/config_file_examples/bands.yml
+-rw-r--r--   0        0        0     1736 2023-03-31 09:38:15.114796 prepipy-0.6.5/src/prepipy/config_file_examples/config_single.yml
+-rw-r--r--   0        0        0      184 2023-03-31 09:38:15.114796 prepipy-0.6.5/src/prepipy/config_file_examples/mask.yml
+-rw-r--r--   0        0        0     3535 2023-03-31 09:38:20.474789 prepipy-0.6.5/src/prepipy/configuration.py
+-rw-r--r--   0        0        0    47850 2023-04-23 23:11:35.981625 prepipy-0.6.5/src/prepipy/framework.py
+-rw-r--r--   0        0        0     7094 2023-04-23 18:55:59.195121 prepipy-0.6.5/src/prepipy/framework_sources.py
+-rw-r--r--   0        0        0     2502 2023-04-23 23:11:23.068772 prepipy-0.6.5/src/prepipy/masking.py
+-rw-r--r--   0        0        0       68 2023-03-31 21:09:47.636364 prepipy-0.6.5/src/prepipy/resources/grey_values.yml
+-rw-r--r--   0        0        0     1044 2023-03-12 22:50:46.683730 prepipy-0.6.5/src/prepipy/resources/html_templates.yml
+-rw-r--r--   0        0        0      468 2023-03-12 22:50:46.685849 prepipy-0.6.5/src/prepipy/resources/stiff_params.yml
+-rw-r--r--   0        0        0    19395 2023-04-23 23:11:12.370453 prepipy-0.6.5/src/prepipy/rgbcombo.py
+-rw-r--r--   0        0        0     7831 1970-01-01 00:00:00.000000 prepipy-0.6.5/PKG-INFO
```

### Comparing `prepipy-0.6.4/LICENSE` & `prepipy-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/pyproject.toml` & `prepipy-0.6.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prepipy"
-version = "0.6.4"
+version = "0.6.5"
 description = "Provides the ability to stretch and combine astronomical images from multiple bands into (RGB) colour images."
 authors = ["Fabian Haberhauer <fabian.haberhauer@univie.ac.at>"]
 maintainers = ["teutoburg <ghost@instruct.at>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/teutoburg/prepipy"
 classifiers = [
@@ -19,15 +19,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Pillow = "^9.4"
 astropy = "^5.1"
 matplotlib = "^3.7"
 tqdm = "^4.64"
-numpy = "^1.23"
+numpy = "^1.21"
 "ruamel.yaml" = "^0.17.21"
 colorama = "^0.4.6"
 regions = "^0.6"
 
 [tool.poetry.scripts]
 rgbcombo = "prepipy.rgbcombo:main"
```

### Comparing `prepipy-0.6.4/README.md` & `prepipy-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/auxiliaries.py` & `prepipy-0.6.5/src/prepipy/auxiliaries.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/config/config_comments.yml` & `prepipy-0.6.5/src/prepipy/config/config_comments.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/config/logging_config.yml` & `prepipy-0.6.5/src/prepipy/config/logging_config.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/config/masking_example.yml` & `prepipy-0.6.5/src/prepipy/config/masking_example.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/config_file_examples/bands.yml` & `prepipy-0.6.5/src/prepipy/config_file_examples/bands.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/config_file_examples/config_single.yml` & `prepipy-0.6.5/src/prepipy/config_file_examples/config_single.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/configuration.py` & `prepipy-0.6.5/src/prepipy/configuration.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/framework.py` & `prepipy-0.6.5/src/prepipy/framework.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/framework_sources.py` & `prepipy-0.6.5/src/prepipy/framework_sources.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/masking.py` & `prepipy-0.6.5/src/prepipy/masking.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/resources/html_templates.yml` & `prepipy-0.6.5/src/prepipy/resources/html_templates.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/src/prepipy/rgbcombo.py` & `prepipy-0.6.5/src/prepipy/rgbcombo.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.4/PKG-INFO` & `prepipy-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepipy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Provides the ability to stretch and combine astronomical images from multiple bands into (RGB) colour images.
 Home-page: https://github.com/teutoburg/prepipy
 License: GPL-3.0-or-later
 Author: Fabian Haberhauer
 Author-email: fabian.haberhauer@univie.ac.at
 Maintainer: teutoburg
 Maintainer-email: ghost@instruct.at
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Dist: Pillow (>=9.4,<10.0)
 Requires-Dist: astropy (>=5.1,<6.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: matplotlib (>=3.7,<4.0)
-Requires-Dist: numpy (>=1.23,<2.0)
+Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: regions (>=0.6,<0.7)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: tqdm (>=4.64,<5.0)
 Project-URL: Repository, https://github.com/teutoburg/prepipy
 Description-Content-Type: text/markdown
 
 # prepipy
```

