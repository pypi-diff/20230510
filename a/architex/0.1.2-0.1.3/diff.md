# Comparing `tmp/architex-0.1.2.tar.gz` & `tmp/architex-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architex-0.1.2.tar", max compression
+gzip compressed data, was "architex-0.1.3.tar", max compression
```

## Comparing `architex-0.1.2.tar` & `architex-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.2/README.md
--rw-r--r--   0        0        0      426 2023-05-10 05:11:35.340660 architex-0.1.2/architex/__init__.py
--rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.2/architex/__main__.py
--rw-r--r--   0        0        0    10253 2023-05-10 05:30:21.086297 architex-0.1.2/architex/controller.py
--rw-r--r--   0        0        0      858 2023-05-10 05:14:18.112010 architex-0.1.2/architex/view.py
--rw-r--r--   0        0        0      538 2023-05-10 05:56:48.055920 architex-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.2/setup.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.3/README.md
+-rw-r--r--   0        0        0      426 2023-05-10 05:59:03.419086 architex-0.1.3/architex/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.3/architex/__main__.py
+-rw-r--r--   0        0        0    10253 2023-05-10 05:30:21.086297 architex-0.1.3/architex/controller.py
+-rw-r--r--   0        0        0      858 2023-05-10 05:14:18.112010 architex-0.1.3/architex/view.py
+-rw-r--r--   0        0        0      538 2023-05-10 05:59:08.608146 architex-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.3/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.3/PKG-INFO
```

### Comparing `architex-0.1.2/architex/controller.py` & `architex-0.1.3/architex/controller.py`

 * *Files identical despite different names*

### Comparing `architex-0.1.2/architex/view.py` & `architex-0.1.3/architex/view.py`

 * *Files identical despite different names*

### Comparing `architex-0.1.2/pyproject.toml` & `architex-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "architex"
-version = "0.1.2"
+version = "0.1.3"
 description = "Draw your software architecture diagram automagically"
 authors = ["Miko <jherjati@gmail.com>"]
 readme = "README.md"
 packages = [{include = "architex"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `architex-0.1.2/setup.py` & `architex-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pytest==6.2.4',
  'pyyaml>=5.0,<6.0',
  'shellingham==1.4.0',
  'typer==0.3.2']
 
 setup_kwargs = {
     'name': 'architex',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Draw your software architecture diagram automagically',
     'long_description': 'A package to auto draw your software architecture diagram from your source code.\n\nCurrent limitation :\nYour source code should be consist of docker compose (required) and nginx (optional) configuration file.\n',
     'author': 'Miko',
     'author_email': 'jherjati@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `architex-0.1.2/PKG-INFO` & `architex-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architex
-Version: 0.1.2
+Version: 0.1.3
 Summary: Draw your software architecture diagram automagically
 Author: Miko
 Author-email: jherjati@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

