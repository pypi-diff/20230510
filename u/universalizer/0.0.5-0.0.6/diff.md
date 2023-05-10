# Comparing `tmp/universalizer-0.0.5.tar.gz` & `tmp/universalizer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universalizer-0.0.5.tar", max compression
+gzip compressed data, was "universalizer-0.0.6.tar", max compression
```

## Comparing `universalizer-0.0.5.tar` & `universalizer-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1527 2022-09-21 21:51:45.814939 universalizer-0.0.5/LICENSE
--rw-r--r--   0        0        0     1315 2022-10-11 19:06:24.860957 universalizer-0.0.5/README.md
--rw-r--r--   0        0        0      830 2023-03-01 21:46:24.936112 universalizer-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       21 2022-09-28 21:12:26.731575 universalizer-0.0.5/universalizer/__init__.py
--rw-r--r--   0        0        0     5628 2022-12-14 18:12:29.236130 universalizer-0.0.5/universalizer/categories.py
--rw-r--r--   0        0        0     3299 2022-11-22 22:41:33.254886 universalizer-0.0.5/universalizer/cli.py
--rw-r--r--   0        0        0    18320 2023-03-01 21:45:45.761879 universalizer-0.0.5/universalizer/norm.py
--rw-r--r--   0        0        0     2024 2022-10-11 19:03:11.770956 universalizer-0.0.5/universalizer/oak_utils.py
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 universalizer-0.0.5/setup.py
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 universalizer-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1527 2022-09-21 21:51:45.814939 universalizer-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1315 2022-10-11 19:06:24.860957 universalizer-0.0.6/README.md
+-rw-r--r--   0        0        0      830 2023-05-10 18:58:40.061222 universalizer-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       21 2022-09-28 21:12:26.731575 universalizer-0.0.6/universalizer/__init__.py
+-rw-r--r--   0        0        0     5628 2022-12-14 18:12:29.236130 universalizer-0.0.6/universalizer/categories.py
+-rw-r--r--   0        0        0     3299 2022-11-22 22:41:33.254886 universalizer-0.0.6/universalizer/cli.py
+-rw-r--r--   0        0        0    18320 2023-03-01 21:45:45.761879 universalizer-0.0.6/universalizer/norm.py
+-rw-r--r--   0        0        0     2024 2022-10-11 19:03:11.770956 universalizer-0.0.6/universalizer/oak_utils.py
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 universalizer-0.0.6/PKG-INFO
```

### Comparing `universalizer-0.0.5/LICENSE` & `universalizer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `universalizer-0.0.5/README.md` & `universalizer-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `universalizer-0.0.5/universalizer/categories.py` & `universalizer-0.0.6/universalizer/categories.py`

 * *Files identical despite different names*

### Comparing `universalizer-0.0.5/universalizer/cli.py` & `universalizer-0.0.6/universalizer/cli.py`

 * *Files identical despite different names*

### Comparing `universalizer-0.0.5/universalizer/norm.py` & `universalizer-0.0.6/universalizer/norm.py`

 * *Files identical despite different names*

### Comparing `universalizer-0.0.5/universalizer/oak_utils.py` & `universalizer-0.0.6/universalizer/oak_utils.py`

 * *Files identical despite different names*

### Comparing `universalizer-0.0.5/PKG-INFO` & `universalizer-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universalizer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Provides functions for knowledge graph cleanup and identifier normalization.
 Home-page: https://github.com/Knowledge-Graph-Hub/universalizer
 License: BSD-3
 Keywords: kg-hub,knowledgegraphs,ontology
 Author: caufieldjh
 Author-email: j.harry.caufield@gmail.com
 Requires-Python: >=3.9,<3.12
@@ -13,15 +13,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: curies (>=0.4.0,<0.5.0)
-Requires-Dist: kgx (>=1.7.0,<2.0.0)
+Requires-Dist: kgx (>=2.0.0,<3.0.0)
 Requires-Dist: oaklib (>=0.1.48,<0.2.0)
 Requires-Dist: prefixmaps (>=0.1.3,<0.2.0)
 Requires-Dist: sssom (>=0.3.16,<0.4.0)
 Project-URL: Repository, https://github.com/Knowledge-Graph-Hub/universalizer
 Description-Content-Type: text/markdown
 
 # universalizer
```

