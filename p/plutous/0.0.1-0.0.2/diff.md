# Comparing `tmp/plutous-0.0.1.tar.gz` & `tmp/plutous-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous-0.0.1.tar", max compression
+gzip compressed data, was "plutous-0.0.2.tar", max compression
```

## Comparing `plutous-0.0.1.tar` & `plutous-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.1/LICENSE
--rw-r--r--   0        0        0       31 2023-05-10 14:19:17.579815 plutous-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-10 14:28:26.335096 plutous-0.0.1/plutous/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.1/plutous/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.210763 plutous-0.0.1/plutous/cli/main.py
--rw-r--r--   0        0        0      471 2023-05-10 14:48:08.127679 plutous-0.0.1/plutous/config.py
--rw-r--r--   0        0        0      431 2023-05-10 14:50:54.719604 plutous-0.0.1/plutous/database.py
--rw-r--r--   0        0        0      662 2023-05-10 14:43:59.277868 plutous-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 plutous-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.2/LICENSE
+-rw-r--r--   0        0        0       31 2023-05-10 14:19:17.579815 plutous-0.0.2/README.md
+-rw-r--r--   0        0        0       21 2023-05-10 15:10:38.768360 plutous-0.0.2/plutous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.2/plutous/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.210763 plutous-0.0.2/plutous/cli/main.py
+-rw-r--r--   0        0        0      463 2023-05-10 15:09:23.919002 plutous-0.0.2/plutous/config.py
+-rw-r--r--   0        0        0      226 2023-05-10 15:09:29.119375 plutous-0.0.2/plutous/database.py
+-rw-r--r--   0        0        0      662 2023-05-10 15:10:44.056739 plutous-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 plutous-0.0.2/PKG-INFO
```

### Comparing `plutous-0.0.1/LICENSE` & `plutous-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous-0.0.1/pyproject.toml` & `plutous-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous"
-version = "0.0.1"
+version = "0.0.2"
 description = "Plutous Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `plutous-0.0.1/PKG-INFO` & `plutous-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutous
-Version: 0.0.1
+Version: 0.0.2
 Summary: Plutous Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

