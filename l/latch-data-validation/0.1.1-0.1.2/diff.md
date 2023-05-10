# Comparing `tmp/latch_data_validation-0.1.1.tar.gz` & `tmp/latch_data_validation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_data_validation-0.1.1.tar", max compression
+gzip compressed data, was "latch_data_validation-0.1.2.tar", max compression
```

## Comparing `latch_data_validation-0.1.1.tar` & `latch_data_validation-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     7052 2023-04-27 17:16:11.680791 latch_data_validation-0.1.1/LICENSE
--rw-r--r--   0        0        0       25 2023-04-27 17:17:21.170023 latch_data_validation-0.1.1/README.md
--rw-r--r--   0        0        0    12592 2023-04-27 17:18:23.749982 latch_data_validation-0.1.1/latch_data_validation/data_validation.py
--rw-r--r--   0        0        0      832 2023-04-27 21:00:56.957200 latch_data_validation-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 latch_data_validation-0.1.1/setup.py
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 latch_data_validation-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 17:16:11.680791 latch_data_validation-0.1.2/LICENSE
+-rw-r--r--   0        0        0       25 2023-04-27 17:17:21.170023 latch_data_validation-0.1.2/README.md
+-rw-r--r--   0        0        0    12592 2023-04-27 17:18:23.749982 latch_data_validation-0.1.2/latch_data_validation/data_validation.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:37:35.452943 latch_data_validation-0.1.2/latch_data_validation/py.typed
+-rw-r--r--   0        0        0      832 2023-05-09 21:37:51.846861 latch_data_validation-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 latch_data_validation-0.1.2/setup.py
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 latch_data_validation-0.1.2/PKG-INFO
```

### Comparing `latch_data_validation-0.1.1/LICENSE` & `latch_data_validation-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_data_validation-0.1.1/latch_data_validation/data_validation.py` & `latch_data_validation-0.1.2/latch_data_validation/data_validation.py`

 * *Files identical despite different names*

### Comparing `latch_data_validation-0.1.1/pyproject.toml` & `latch_data_validation-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-data-validation"
-version = "0.1.1"
+version = "0.1.2"
 description = "Data validation for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_data_validation"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_data_validation-0.1.1/setup.py` & `latch_data_validation-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['opentelemetry-api>=1.15.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'latch-data-validation',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Data validation for latch python backend services',
     'long_description': '# python-data-validation\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

