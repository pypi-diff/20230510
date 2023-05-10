# Comparing `tmp/py_module_parser-0.4.0.tar.gz` & `tmp/py_module_parser-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_module_parser-0.4.0.tar", max compression
+gzip compressed data, was "py_module_parser-0.4.0b0.tar", max compression
```

## Comparing `py_module_parser-0.4.0.tar` & `py_module_parser-0.4.0b0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1093 2023-05-09 19:52:20.665429 py_module_parser-0.4.0/LICENSE
--rw-r--r--   0        0        0     6368 2023-05-10 12:47:23.089037 py_module_parser-0.4.0/README.md
--rw-r--r--   0        0        0      214 2023-05-10 07:42:51.492515 py_module_parser-0.4.0/py_module_parser/__init__.py
--rw-r--r--   0        0        0     3579 2023-05-10 12:22:43.701669 py_module_parser-0.4.0/py_module_parser/models.py
--rw-r--r--   0        0        0    10326 2023-05-10 12:46:39.696490 py_module_parser-0.4.0/py_module_parser/parser.py
--rw-r--r--   0        0        0      320 2023-05-10 10:46:15.335512 py_module_parser-0.4.0/py_module_parser/utils.py
--rw-r--r--   0        0        0     1126 2023-05-10 12:50:26.080724 py_module_parser-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7693 1970-01-01 00:00:00.000000 py_module_parser-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-09 19:52:20.665429 py_module_parser-0.4.0b0/LICENSE
+-rw-r--r--   0        0        0     6368 2023-05-10 12:47:23.089037 py_module_parser-0.4.0b0/README.md
+-rw-r--r--   0        0        0      214 2023-05-10 07:42:51.492515 py_module_parser-0.4.0b0/py_module_parser/__init__.py
+-rw-r--r--   0        0        0     3579 2023-05-10 12:22:43.701669 py_module_parser-0.4.0b0/py_module_parser/models.py
+-rw-r--r--   0        0        0    10326 2023-05-10 12:46:39.696490 py_module_parser-0.4.0b0/py_module_parser/parser.py
+-rw-r--r--   0        0        0      320 2023-05-10 10:46:15.335512 py_module_parser-0.4.0b0/py_module_parser/utils.py
+-rw-r--r--   0        0        0     1128 2023-05-10 12:47:45.467073 py_module_parser-0.4.0b0/pyproject.toml
+-rw-r--r--   0        0        0     7695 1970-01-01 00:00:00.000000 py_module_parser-0.4.0b0/PKG-INFO
```

### Comparing `py_module_parser-0.4.0/LICENSE` & `py_module_parser-0.4.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_module_parser-0.4.0/README.md` & `py_module_parser-0.4.0b0/README.md`

 * *Files identical despite different names*

### Comparing `py_module_parser-0.4.0/py_module_parser/models.py` & `py_module_parser-0.4.0b0/py_module_parser/models.py`

 * *Files identical despite different names*

### Comparing `py_module_parser-0.4.0/py_module_parser/parser.py` & `py_module_parser-0.4.0b0/py_module_parser/parser.py`

 * *Files identical despite different names*

### Comparing `py_module_parser-0.4.0/pyproject.toml` & `py_module_parser-0.4.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-module-parser"
-version = "0.4.0"
+version = "0.4.0b0"
 description = "Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code."
 authors = ["Iuliia Volkova <xnuinside@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/xnuinside/py-module-parser"
 repository = "https://github.com/xnuinside/py-module-parser"
 classifiers = [
```

### Comparing `py_module_parser-0.4.0/PKG-INFO` & `py_module_parser-0.4.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-module-parser
-Version: 0.4.0
+Version: 0.4.0b0
 Summary: Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.
 Home-page: https://github.com/xnuinside/py-module-parser
 License: MIT
 Author: Iuliia Volkova
 Author-email: xnuinside@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

