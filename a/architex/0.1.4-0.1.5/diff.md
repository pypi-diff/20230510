# Comparing `tmp/architex-0.1.4.tar.gz` & `tmp/architex-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "architex-0.1.4.tar", max compression
+gzip compressed data, was "architex-0.1.5.tar", max compression
```

## Comparing `architex-0.1.4.tar` & `architex-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.4/README.md
--rw-r--r--   0        0        0      426 2023-05-10 06:20:06.238273 architex-0.1.4/architex/__init__.py
--rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.4/architex/__main__.py
--rw-r--r--   0        0        0    10340 2023-05-10 06:19:23.470825 architex-0.1.4/architex/controller.py
--rw-r--r--   0        0        0      858 2023-05-10 05:14:18.112010 architex-0.1.4/architex/view.py
--rw-r--r--   0        0        0      538 2023-05-10 06:20:06.074900 architex-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.4/setup.py
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      208 2023-05-10 05:34:05.741414 architex-0.1.5/README.md
+-rw-r--r--   0        0        0      426 2023-05-10 07:16:44.656961 architex-0.1.5/architex/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-10 05:11:37.507795 architex-0.1.5/architex/__main__.py
+-rw-r--r--   0        0        0    10616 2023-05-10 07:01:04.703268 architex-0.1.5/architex/controller.py
+-rw-r--r--   0        0        0      936 2023-05-10 07:11:17.514948 architex-0.1.5/architex/view.py
+-rw-r--r--   0        0        0      538 2023-05-10 07:16:44.479897 architex-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 architex-0.1.5/setup.py
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 architex-0.1.5/PKG-INFO
```

### Comparing `architex-0.1.4/architex/controller.py` & `architex-0.1.5/architex/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,35 +192,46 @@
                 )
                 containers[target_container_name] = target_container
 
             containers[nginx_container_name] >> Relationship(
                 f'{location_block.get("args")[0]} fastcgi pass') >> target_container
 
 
-def start_drawing(repo_path):
+def start_drawing(repo_path, search):
     docker_composes, compose_files = [], []
-    filepaths = get_filepaths(repo_path)
+    filepaths = get_filepaths(repo_path[0]) if search else repo_path
+    if (search):
+        repo_path = repo_path[0]
+    else:
+        None
     for filepath in filepaths:
         if (".yml" in filepath or ".yaml" in filepath):
             file = open(filepath)
-            loadedYaml = yaml.load(file, Loader=SafeLoader)
+            loadedYaml = {}
+            try:
+                loadedYaml = yaml.load(file, Loader=SafeLoader)
+            except:
+                None
             if loadedYaml.get("services"):
                 docker_composes.append(loadedYaml)
                 compose_files.append(filepath)
             file.close()
 
-    reponame = repo_path.split("/")[-1] if "/" in repo_path else "current"
+    reponame = "current"
+    if (search):
+        reponame = repo_path.split(
+            "/")[-1] if "/" in repo_path else "current"
     with Diagram(f'{reponame} Architectural Diagram', filename=f'{reponame}_architecture',  graph_attr=graph_attr, show=False):
         containers, databases, user = {}, {}, Person(
             name="User", description="General User")
 
         for index, docker_compose in enumerate(docker_composes):
             populate_databases(docker_compose, databases)
             populate_containers(docker_compose, containers,
-                                compose_files[index], repo_path)
+                                compose_files[index], repo_path if search else "")
             get_compose_relationships(
                 docker_compose, containers, databases, user)
 
         for item in global_names:
             nginx_filepath = item.get("nginx_path")
             if nginx_filepath:
                 get_nginx_relationships(
```

### Comparing `architex-0.1.4/architex/view.py` & `architex-0.1.5/architex/view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module provides the architex CLI."""
 
 import typer
-from typing import Optional
+from typing import Optional, List
 from architex import (ERRORS, __app_name__, __version__, controller)
 
 app = typer.Typer()
 
 
 def _version_callback(value: bool) -> None:
     if value:
@@ -25,15 +25,16 @@
     )
 ) -> None:
     return
 
 
 @app.command()
 def draw(
-    repo_path: str = typer.Argument(...),
+    repo_path: List[str] = typer.Argument(...),
+    search: bool = typer.Option(False, "--search", "-s"),
 ) -> None:
     """Draw software architecture diagram."""
-    controller.start_drawing(repo_path)
+    controller.start_drawing(repo_path, search)
     typer.secho(
         f"""Your architectural diagram is completed""",
         fg=typer.colors.GREEN,
     )
```

### Comparing `architex-0.1.4/pyproject.toml` & `architex-0.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "architex"
-version = "0.1.4"
+version = "0.1.5"
 description = "Draw your software architecture diagram automagically"
 authors = ["Miko <jherjati@gmail.com>"]
 readme = "README.md"
 packages = [{include = "architex"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `architex-0.1.4/setup.py` & `architex-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pytest==6.2.4',
  'pyyaml>=5.0,<6.0',
  'shellingham==1.4.0',
  'typer==0.3.2']
 
 setup_kwargs = {
     'name': 'architex',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Draw your software architecture diagram automagically',
     'long_description': 'A package to auto draw your software architecture diagram from your source code.\n\nCurrent limitation :\nYour source code should be consist of docker compose (required) and nginx (optional) configuration file.\n',
     'author': 'Miko',
     'author_email': 'jherjati@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `architex-0.1.4/PKG-INFO` & `architex-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: architex
-Version: 0.1.4
+Version: 0.1.5
 Summary: Draw your software architecture diagram automagically
 Author: Miko
 Author-email: jherjati@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

