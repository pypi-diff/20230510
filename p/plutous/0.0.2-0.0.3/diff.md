# Comparing `tmp/plutous-0.0.2.tar.gz` & `tmp/plutous-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous-0.0.2.tar", max compression
+gzip compressed data, was "plutous-0.0.3.tar", max compression
```

## Comparing `plutous-0.0.2.tar` & `plutous-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.2/LICENSE
--rw-r--r--   0        0        0       31 2023-05-10 14:19:17.579815 plutous-0.0.2/README.md
--rw-r--r--   0        0        0       21 2023-05-10 15:10:38.768360 plutous-0.0.2/plutous/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.2/plutous/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:48:51.210763 plutous-0.0.2/plutous/cli/main.py
--rw-r--r--   0        0        0      463 2023-05-10 15:09:23.919002 plutous-0.0.2/plutous/config.py
--rw-r--r--   0        0        0      226 2023-05-10 15:09:29.119375 plutous-0.0.2/plutous/database.py
--rw-r--r--   0        0        0      662 2023-05-10 15:10:44.056739 plutous-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 plutous-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 14:19:17.579815 plutous-0.0.3/LICENSE
+-rw-r--r--   0        0        0       31 2023-05-10 14:19:17.579815 plutous-0.0.3/README.md
+-rw-r--r--   0        0        0       87 2023-05-10 17:26:37.357823 plutous-0.0.3/plutous/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.206763 plutous-0.0.3/plutous/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:51.210763 plutous-0.0.3/plutous/cli/main.py
+-rw-r--r--   0        0        0      463 2023-05-10 15:09:23.919002 plutous-0.0.3/plutous/config.py
+-rw-r--r--   0        0        0      226 2023-05-10 15:09:29.119375 plutous-0.0.3/plutous/database.py
+-rw-r--r--   0        0        0      668 2023-05-10 17:26:33.977554 plutous-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 plutous-0.0.3/PKG-INFO
```

### Comparing `plutous-0.0.2/LICENSE` & `plutous-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous-0.0.2/pyproject.toml` & `plutous-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "plutous"
-version = "0.0.2"
+version = "0.0.3"
 description = "Plutous Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.10,<3.11"
 SQLAlchemy = ">=2.0.12"
 typer = ">=0.9.0"
 alembic = ">=1.10.4"
 pydantic = ">=1.10.7"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.3.0"
```

### Comparing `plutous-0.0.2/PKG-INFO` & `plutous-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: plutous
-Version: 0.0.2
+Version: 0.0.3
 Summary: Plutous Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: SQLAlchemy (>=2.0.12)
 Requires-Dist: alembic (>=1.10.4)
 Requires-Dist: pydantic (>=1.10.7)
 Requires-Dist: typer (>=0.9.0)
 Description-Content-Type: text/markdown
```

