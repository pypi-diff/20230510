# Comparing `tmp/warsaw-data-api-0.3.0.tar.gz` & `tmp/warsaw_data_api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warsaw-data-api-0.3.0.tar", max compression
+gzip compressed data, was "warsaw_data_api-0.3.1.tar", max compression
```

## Comparing `warsaw-data-api-0.3.0.tar` & `warsaw_data_api-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1098 2021-12-21 17:32:49.384708 warsaw-data-api-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     1692 2021-12-21 17:32:50.164757 warsaw-data-api-0.3.0/README.md
--rw-r--r--   0        0        0      545 2021-12-21 17:32:50.168757 warsaw-data-api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      234 2021-12-21 17:32:50.164757 warsaw-data-api-0.3.0/warsaw_data_api/__init__.py
--rw-r--r--   0        0        0      688 2021-12-21 17:32:49.384708 warsaw-data-api-0.3.0/warsaw_data_api/exceptions.py
--rw-r--r--   0        0        0      297 2021-12-21 17:32:49.384708 warsaw-data-api-0.3.0/warsaw_data_api/session.py
--rw-r--r--   0        0        0     4692 2021-12-21 17:32:49.384708 warsaw-data-api-0.3.0/warsaw_data_api/ztm/__init__.py
--rw-r--r--   0        0        0     2214 2021-12-21 17:32:49.384708 warsaw-data-api-0.3.0/warsaw_data_api/ztm/models.py
--rw-r--r--   0        0        0     2296 2021-12-21 17:33:01.320442 warsaw-data-api-0.3.0/setup.py
--rw-r--r--   0        0        0     2413 2021-12-21 17:33:01.320798 warsaw-data-api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     1692 2023-05-10 15:06:01.425547 warsaw_data_api-0.3.1/README.md
+-rw-r--r--   0        0        0      608 2023-05-10 15:06:01.429547 warsaw_data_api-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-05-10 15:06:01.425547 warsaw_data_api-0.3.1/warsaw_data_api/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/warsaw_data_api/exceptions.py
+-rw-r--r--   0        0        0      297 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/warsaw_data_api/session.py
+-rw-r--r--   0        0        0     4692 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/warsaw_data_api/ztm/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/warsaw_data_api/ztm/models.py
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 warsaw_data_api-0.3.1/PKG-INFO
```

### Comparing `warsaw-data-api-0.3.0/LICENSE.md` & `warsaw_data_api-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `warsaw-data-api-0.3.0/README.md` & `warsaw_data_api-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `warsaw-data-api-0.3.0/pyproject.toml` & `warsaw_data_api-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "warsaw-data-api"
-version = "0.3.0"
+version = "0.3.1"
 description = "Warsaw data python api"
 authors = ["Radoslaw Wielonski"]
 license = "MIT"
+homepage = "https://github.com/radekwielonski/warsaw-data-api"
 readme = "README.md"
 
 [tool.semantic_release]
 version_variable = [
     "warsaw_data_api/__init__.py:__version__",
     "pyproject.toml:version"
 ]
```

### Comparing `warsaw-data-api-0.3.0/warsaw_data_api/exceptions.py` & `warsaw_data_api-0.3.1/warsaw_data_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `warsaw-data-api-0.3.0/warsaw_data_api/ztm/__init__.py` & `warsaw_data_api-0.3.1/warsaw_data_api/ztm/__init__.py`

 * *Files identical despite different names*

### Comparing `warsaw-data-api-0.3.0/warsaw_data_api/ztm/models.py` & `warsaw_data_api-0.3.1/warsaw_data_api/ztm/models.py`

 * *Files identical despite different names*

### Comparing `warsaw-data-api-0.3.0/PKG-INFO` & `warsaw_data_api-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: warsaw-data-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Warsaw data python api
+Home-page: https://github.com/radekwielonski/warsaw-data-api
 License: MIT
 Author: Radoslaw Wielonski
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Pythonic way to use Warsaw data API
 
 This package allow to fetch data from API provided by "UM Warszawa" - https://api.um.warszawa.pl/
 
 ## Current features
```

