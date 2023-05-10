# Comparing `tmp/plutous-0.0.3.tar.gz` & `tmp/plutous-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous-0.0.3.tar", max compression
+gzip compressed data, was "plutous-0.0.4.tar", max compression
```

## Comparing `plutous-0.0.3.tar` & `plutous-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.3/LICENSE
--rw-r--r--   0        0        0       31 2023-05-10 14:19:17.579815 plutous-0.0.3/README.md
--rw-r--r--   0        0        0       87 2023-05-10 17:26:37.357823 plutous-0.0.3/plutous/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.3/plutous/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.210763 plutous-0.0.3/plutous/cli/main.py
--rw-r--r--   0        0        0      463 2023-05-10 15:09:23.919002 plutous-0.0.3/plutous/config.py
--rw-r--r--   0        0        0      226 2023-05-10 15:09:29.119375 plutous-0.0.3/plutous/database.py
--rw-r--r--   0        0        0      668 2023-05-10 17:26:33.977554 plutous-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 plutous-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.4/LICENSE
+-rw-r--r--   0        0        0       31 2023-05-10 14:19:17.579815 plutous-0.0.4/README.md
+-rw-r--r--   0        0        0       87 2023-05-10 17:56:59.554870 plutous-0.0.4/plutous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.4/plutous/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.210763 plutous-0.0.4/plutous/cli/main.py
+-rw-r--r--   0        0        0      699 2023-05-10 17:42:46.866990 plutous-0.0.4/plutous/config.py
+-rw-r--r--   0        0        0      226 2023-05-10 15:09:29.119375 plutous-0.0.4/plutous/database.py
+-rw-r--r--   0        0        0      668 2023-05-10 17:57:14.416053 plutous-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 plutous-0.0.4/PKG-INFO
```

### Comparing `plutous-0.0.3/LICENSE` & `plutous-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous-0.0.3/pyproject.toml` & `plutous-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous"
-version = "0.0.3"
+version = "0.0.4"
 description = "Plutous Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `plutous-0.0.3/PKG-INFO` & `plutous-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutous
-Version: 0.0.3
+Version: 0.0.4
 Summary: Plutous Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

