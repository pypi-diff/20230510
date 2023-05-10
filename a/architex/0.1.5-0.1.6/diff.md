# Comparing `tmp/architex-0.1.5.tar.gz` & `tmp/architex-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architex-0.1.5.tar", max compression
+gzip compressed data, was "architex-0.1.6.tar", max compression
```

## Comparing `architex-0.1.5.tar` & `architex-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.5/README.md
--rw-r--r--   0        0        0      426 2023-05-10 07:16:44.656961 architex-0.1.5/architex/__init__.py
--rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.5/architex/__main__.py
--rw-r--r--   0        0        0    10616 2023-05-10 07:01:04.703268 architex-0.1.5/architex/controller.py
--rw-r--r--   0        0        0      936 2023-05-10 07:11:17.514948 architex-0.1.5/architex/view.py
--rw-r--r--   0        0        0      538 2023-05-10 07:16:44.479897 architex-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.5/setup.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.6/README.md
+-rw-r--r--   0        0        0      426 2023-05-10 12:49:37.748401 architex-0.1.6/architex/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.6/architex/__main__.py
+-rw-r--r--   0        0        0    10697 2023-05-10 12:48:55.614362 architex-0.1.6/architex/controller.py
+-rw-r--r--   0        0        0      936 2023-05-10 07:11:17.514948 architex-0.1.6/architex/view.py
+-rw-r--r--   0        0        0      538 2023-05-10 12:49:37.572565 architex-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.6/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.6/PKG-INFO
```

### Comparing `architex-0.1.5/architex/controller.py` & `architex-0.1.6/architex/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,16 +205,17 @@
         None
     for filepath in filepaths:
         if (".yml" in filepath or ".yaml" in filepath):
             file = open(filepath)
             loadedYaml = {}
             try:
                 loadedYaml = yaml.load(file, Loader=SafeLoader)
+                loadedYaml = {} if loadedYaml is None else loadedYaml
             except:
-                None
+                loadedYaml = {}
             if loadedYaml.get("services"):
                 docker_composes.append(loadedYaml)
                 compose_files.append(filepath)
             file.close()
 
     reponame = "current"
     if (search):
```

### Comparing `architex-0.1.5/architex/view.py` & `architex-0.1.6/architex/view.py`

 * *Files identical despite different names*

### Comparing `architex-0.1.5/pyproject.toml` & `architex-0.1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "architex"
-version = "0.1.5"
+version = "0.1.6"
 description = "Draw your software architecture diagram automagically"
 authors = ["Miko <jherjati@gmail.com>"]
 readme = "README.md"
 packages = [{include = "architex"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `architex-0.1.5/setup.py` & `architex-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pytest==6.2.4',
  'pyyaml>=5.0,<6.0',
  'shellingham==1.4.0',
  'typer==0.3.2']
 
 setup_kwargs = {
     'name': 'architex',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Draw your software architecture diagram automagically',
     'long_description': 'A package to auto draw your software architecture diagram from your source code.\n\nCurrent limitation :\nYour source code should be consist of docker compose (required) and nginx (optional) configuration file.\n',
     'author': 'Miko',
     'author_email': 'jherjati@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `architex-0.1.5/PKG-INFO` & `architex-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architex
-Version: 0.1.5
+Version: 0.1.6
 Summary: Draw your software architecture diagram automagically
 Author: Miko
 Author-email: jherjati@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

