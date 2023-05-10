# Comparing `tmp/gen_pop_linkml2sheets-0.1.3.tar.gz` & `tmp/gen_pop_linkml2sheets-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_pop_linkml2sheets-0.1.3.tar", max compression
+gzip compressed data, was "gen_pop_linkml2sheets-0.1.4.tar", max compression
```

## Comparing `gen_pop_linkml2sheets-0.1.3.tar` & `gen_pop_linkml2sheets-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     4403 2023-05-10 13:29:28.451789 gen_pop_linkml2sheets-0.1.3/README.md
--rw-r--r--   0        0        0     2365 2023-05-10 13:45:10.707541 gen_pop_linkml2sheets-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-10 12:49:52.112547 gen_pop_linkml2sheets-0.1.3/src/gen_pop_linkml2sheets/__init__.py
--rw-r--r--   0        0        0     3748 2023-05-10 13:19:45.340546 gen_pop_linkml2sheets-0.1.3/src/gen_pop_linkml2sheets/generate_and_populate_template.py
--rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-10 12:40:56.283705 gen_pop_linkml2sheets-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     4403 2023-05-10 13:29:28.451789 gen_pop_linkml2sheets-0.1.4/README.md
+-rw-r--r--   0        0        0     2365 2023-05-10 17:46:46.678845 gen_pop_linkml2sheets-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3748 2023-05-10 13:19:45.340546 gen_pop_linkml2sheets-0.1.4/src/gen_pop_linkml2sheets/generate_and_populate_template.py
+-rw-r--r--   0        0        0     5125 1970-01-01 00:00:00.000000 gen_pop_linkml2sheets-0.1.4/PKG-INFO
```

### Comparing `gen_pop_linkml2sheets-0.1.3/LICENSE.md` & `gen_pop_linkml2sheets-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.3/README.md` & `gen_pop_linkml2sheets-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.3/pyproject.toml` & `gen_pop_linkml2sheets-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gen-pop-linkml2sheets"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Mark Andrew Miller <MAM@lbl.gov>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/turbomam/gen-pop-linkml2sheets"
 repository = "https://github.com/turbomam/gen-pop-linkml2sheets"
```

### Comparing `gen_pop_linkml2sheets-0.1.3/src/gen_pop_linkml2sheets/generate_and_populate_template.py` & `gen_pop_linkml2sheets-0.1.4/src/gen_pop_linkml2sheets/generate_and_populate_template.py`

 * *Files identical despite different names*

### Comparing `gen_pop_linkml2sheets-0.1.3/PKG-INFO` & `gen_pop_linkml2sheets-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-pop-linkml2sheets
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/turbomam/gen-pop-linkml2sheets
 License: MIT
 Author: Mark Andrew Miller
 Author-email: MAM@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.3 Summary: Home-
+Metadata-Version: 2.1 Name: gen-pop-linkml2sheets Version: 0.1.4 Summary: Home-
 page: https://github.com/turbomam/gen-pop-linkml2sheets License: MIT Author:
 Mark Andrew Miller Author-email: MAM@lbl.gov Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: linkml (>=1.5.2,<2.0.0) Requires-
 Dist: pandas (>=1.3.4,<2.0.0) Requires-Dist: schemasheets (>=0.1.21,<0.2.0)
```

