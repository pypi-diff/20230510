# Comparing `tmp/architex-0.1.0.tar.gz` & `tmp/architex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architex-0.1.0.tar", max compression
+gzip compressed data, was "architex-0.1.1.tar", max compression
```

## Comparing `architex-0.1.0.tar` & `architex-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.0/README.md
--rw-r--r--   0        0        0      426 2023-05-10 05:11:35.340660 architex-0.1.0/architex/__init__.py
--rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.0/architex/__main__.py
--rw-r--r--   0        0        0    10253 2023-05-10 05:30:21.086297 architex-0.1.0/architex/controller.py
--rw-r--r--   0        0        0      858 2023-05-10 05:14:18.112010 architex-0.1.0/architex/view.py
--rw-r--r--   0        0        0      539 2023-05-10 05:41:52.814679 architex-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 architex-0.1.0/setup.py
--rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 architex-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.1/README.md
+-rw-r--r--   0        0        0      426 2023-05-10 05:11:35.340660 architex-0.1.1/architex/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.1/architex/__main__.py
+-rw-r--r--   0        0        0    10253 2023-05-10 05:30:21.086297 architex-0.1.1/architex/controller.py
+-rw-r--r--   0        0        0      858 2023-05-10 05:14:18.112010 architex-0.1.1/architex/view.py
+-rw-r--r--   0        0        0      538 2023-05-10 05:51:13.073728 architex-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.1/setup.py
+-rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 architex-0.1.1/PKG-INFO
```

### Comparing `architex-0.1.0/architex/controller.py` & `architex-0.1.1/architex/controller.py`

 * *Files identical despite different names*

### Comparing `architex-0.1.0/architex/view.py` & `architex-0.1.1/architex/view.py`

 * *Files identical despite different names*

### Comparing `architex-0.1.0/pyproject.toml` & `architex-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "architex"
-version = "0.1.0"
+version = "0.1.1"
 description = "Draw your software architecture diagram automagically"
 authors = ["Miko <jherjati@gmail.com>"]
 readme = "README.md"
 packages = [{include = "architex"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.6"
 pyyaml = "^6.0"
 diagrams = "^0.23.3"
 crossplane = "^0.5.8"
 typer = "0.3.2"
 colorama = "0.4.4"
 shellingham = "1.4.0"
 pytest = "6.2.4"
```

### Comparing `architex-0.1.0/setup.py` & `architex-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
  'pytest==6.2.4',
  'pyyaml>=6.0,<7.0',
  'shellingham==1.4.0',
  'typer==0.3.2']
 
 setup_kwargs = {
     'name': 'architex',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Draw your software architecture diagram automagically',
     'long_description': 'A package to auto draw your software architecture diagram from your source code.\n\nCurrent limitation :\nYour source code should be consist of docker compose (required) and nginx (optional) configuration file.\n',
     'author': 'Miko',
     'author_email': 'jherjati@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.11,<4.0',
+    'python_requires': '>=3.6,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

