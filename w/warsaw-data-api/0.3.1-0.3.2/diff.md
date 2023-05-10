# Comparing `tmp/warsaw_data_api-0.3.1.tar.gz` & `tmp/warsaw_data_api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warsaw_data_api-0.3.1.tar", max compression
+gzip compressed data, was "warsaw_data_api-0.3.2.tar", max compression
```

## Comparing `warsaw_data_api-0.3.1.tar` & `warsaw_data_api-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1098 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     1692 2023-05-10 15:06:01.425547 warsaw_data_api-0.3.1/README.md
--rw-r--r--   0        0        0      608 2023-05-10 15:06:01.429547 warsaw_data_api-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      234 2023-05-10 15:06:01.425547 warsaw_data_api-0.3.1/warsaw_data_api/__init__.py
--rw-r--r--   0        0        0      688 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/warsaw_data_api/exceptions.py
--rw-r--r--   0        0        0      297 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/warsaw_data_api/session.py
--rw-r--r--   0        0        0     4692 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/warsaw_data_api/ztm/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-10 15:06:00.637544 warsaw_data_api-0.3.1/warsaw_data_api/ztm/models.py
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 warsaw_data_api-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-10 15:32:31.693087 warsaw_data_api-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     1692 2023-05-10 15:32:32.533118 warsaw_data_api-0.3.2/README.md
+-rw-r--r--   0        0        0      648 2023-05-10 15:32:32.537118 warsaw_data_api-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-05-10 15:32:32.533118 warsaw_data_api-0.3.2/warsaw_data_api/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-10 15:32:31.697087 warsaw_data_api-0.3.2/warsaw_data_api/exceptions.py
+-rw-r--r--   0        0        0      297 2023-05-10 15:32:31.697087 warsaw_data_api-0.3.2/warsaw_data_api/session.py
+-rw-r--r--   0        0        0     4692 2023-05-10 15:32:31.697087 warsaw_data_api-0.3.2/warsaw_data_api/ztm/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-10 15:32:31.697087 warsaw_data_api-0.3.2/warsaw_data_api/ztm/models.py
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 warsaw_data_api-0.3.2/PKG-INFO
```

### Comparing `warsaw_data_api-0.3.1/LICENSE.md` & `warsaw_data_api-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `warsaw_data_api-0.3.1/README.md` & `warsaw_data_api-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `warsaw_data_api-0.3.1/pyproject.toml` & `warsaw_data_api-0.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warsaw-data-api"
-version = "0.3.1"
+version = "0.3.2"
 description = "Warsaw data python api"
 authors = ["Radoslaw Wielonski"]
 license = "MIT"
 homepage = "https://github.com/radekwielonski/warsaw-data-api"
 readme = "README.md"
 
 [tool.semantic_release]
@@ -19,7 +19,10 @@
     "README.md:rev: v{version}",
 ]
 major_on_zero = false
 branch = "master"
 upload_to_PyPI = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
+
+[build-system]
+requires = ["requests"]
```

### Comparing `warsaw_data_api-0.3.1/warsaw_data_api/exceptions.py` & `warsaw_data_api-0.3.2/warsaw_data_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `warsaw_data_api-0.3.1/warsaw_data_api/ztm/__init__.py` & `warsaw_data_api-0.3.2/warsaw_data_api/ztm/__init__.py`

 * *Files identical despite different names*

### Comparing `warsaw_data_api-0.3.1/warsaw_data_api/ztm/models.py` & `warsaw_data_api-0.3.2/warsaw_data_api/ztm/models.py`

 * *Files identical despite different names*

### Comparing `warsaw_data_api-0.3.1/PKG-INFO` & `warsaw_data_api-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warsaw-data-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: Warsaw data python api
 Home-page: https://github.com/radekwielonski/warsaw-data-api
 License: MIT
 Author: Radoslaw Wielonski
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

