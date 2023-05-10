# Comparing `tmp/architex-0.1.1.tar.gz` & `tmp/architex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architex-0.1.1.tar", max compression
+gzip compressed data, was "architex-0.1.2.tar", max compression
```

## Comparing `architex-0.1.1.tar` & `architex-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.1/README.md
--rw-r--r--   0        0        0      426 2023-05-10 05:11:35.340660 architex-0.1.1/architex/__init__.py
--rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.1/architex/__main__.py
--rw-r--r--   0        0        0    10253 2023-05-10 05:30:21.086297 architex-0.1.1/architex/controller.py
--rw-r--r--   0        0        0      858 2023-05-10 05:14:18.112010 architex-0.1.1/architex/view.py
--rw-r--r--   0        0        0      538 2023-05-10 05:51:13.073728 architex-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.1/setup.py
--rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 architex-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.2/README.md
+-rw-r--r--   0        0        0      426 2023-05-10 05:11:35.340660 architex-0.1.2/architex/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.2/architex/__main__.py
+-rw-r--r--   0        0        0    10253 2023-05-10 05:30:21.086297 architex-0.1.2/architex/controller.py
+-rw-r--r--   0        0        0      858 2023-05-10 05:14:18.112010 architex-0.1.2/architex/view.py
+-rw-r--r--   0        0        0      538 2023-05-10 05:56:48.055920 architex-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.2/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.2/PKG-INFO
```

### Comparing `architex-0.1.1/architex/controller.py` & `architex-0.1.2/architex/controller.py`

 * *Files identical despite different names*

### Comparing `architex-0.1.1/architex/view.py` & `architex-0.1.2/architex/view.py`

 * *Files identical despite different names*

### Comparing `architex-0.1.1/pyproject.toml` & `architex-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "architex"
-version = "0.1.1"
+version = "0.1.2"
 description = "Draw your software architecture diagram automagically"
 authors = ["Miko <jherjati@gmail.com>"]
 readme = "README.md"
 packages = [{include = "architex"}]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-pyyaml = "^6.0"
+python = "^3.7"
+pyyaml = "^5.0"
 diagrams = "^0.23.3"
 crossplane = "^0.5.8"
 typer = "0.3.2"
 colorama = "0.4.4"
 shellingham = "1.4.0"
 pytest = "6.2.4"
```

### Comparing `architex-0.1.1/setup.py` & `architex-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 {'': ['*']}
 
 install_requires = \
 ['colorama==0.4.4',
  'crossplane>=0.5.8,<0.6.0',
  'diagrams>=0.23.3,<0.24.0',
  'pytest==6.2.4',
- 'pyyaml>=6.0,<7.0',
+ 'pyyaml>=5.0,<6.0',
  'shellingham==1.4.0',
  'typer==0.3.2']
 
 setup_kwargs = {
     'name': 'architex',
-    'version': '0.1.1',
+    'version': '0.1.2',
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
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `architex-0.1.1/PKG-INFO` & `architex-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: architex
-Version: 0.1.1
+Version: 0.1.2
 Summary: Draw your software architecture diagram automagically
 Author: Miko
 Author-email: jherjati@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (==0.4.4)
 Requires-Dist: crossplane (>=0.5.8,<0.6.0)
 Requires-Dist: diagrams (>=0.23.3,<0.24.0)
 Requires-Dist: pytest (==6.2.4)
-Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: pyyaml (>=5.0,<6.0)
 Requires-Dist: shellingham (==1.4.0)
 Requires-Dist: typer (==0.3.2)
 Description-Content-Type: text/markdown
 
 A package to auto draw your software architecture diagram from your source code.
 
 Current limitation :
```

