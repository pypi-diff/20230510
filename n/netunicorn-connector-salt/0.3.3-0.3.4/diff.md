# Comparing `tmp/netunicorn-connector-salt-0.3.3.tar.gz` & `tmp/netunicorn-connector-salt-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-salt-0.3.3.tar", last modified: Tue Apr 11 10:09:21 2023, max compression
+gzip compressed data, was "netunicorn-connector-salt-0.3.4.tar", last modified: Wed May 10 04:48:47 2023, max compression
```

## Comparing `netunicorn-connector-salt-0.3.3.tar` & `netunicorn-connector-salt-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.408581 netunicorn-connector-salt-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-11 10:09:21.408581 netunicorn-connector-salt-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:09:21.408581 netunicorn-connector-salt-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/connectors/salt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.408581 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.336055 netunicorn-connector-salt-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.336055 netunicorn-connector-salt-0.3.4/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.336055 netunicorn-connector-salt-0.3.4/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.336055 netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22393 2023-05-10 04:48:28.000000 netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/connectors/salt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:47.340055 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:48:47.000000 netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-salt-0.3.3/LICENSE` & `netunicorn-connector-salt-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.3/PKG-INFO` & `netunicorn-connector-salt-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.3
+Version: 0.3.4
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-salt-0.3.3/README.md` & `netunicorn-connector-salt-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.3/pyproject.toml` & `netunicorn-connector-salt-0.3.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "netunicorn-connector-salt"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "SaltStack connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "netunicorn-base >= 0.2.6",
+    "netunicorn-base >= 0.3.1",
     "pyyaml",
     "returns",
     "aiohttp"
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/connectors/salt_connector.py` & `netunicorn-connector-salt-0.3.4/src/netunicorn/director/infrastructure/connectors/salt_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         self.config = {}
         if config_file:
             with open(config_file, "r") as f:
                 self.config = yaml.safe_load(f)
 
         self.PUBLIC_GRAINS: list[str] = self.config.get(
-            "netunicorn.connector.salt.public_grains", ["location", "osarch", "kernel"]
+            "netunicorn.connector.salt.public_grains", ["location", "osarch", "kernel", "netunicorn-environments"]
         )
 
         self.endpoint = self.config.get(
             "netunicorn.connector.salt.endpoint"
         ).removesuffix("/")
         self.runpoint = self.endpoint + "/run"
         self.username = self.config.get("netunicorn.connector.salt.username")
@@ -111,14 +111,16 @@
         for node_name, node_grains in nodes.items():
             if not node_grains:
                 continue
             instance = Node(
                 name=node_name,
                 properties=node_grains,
             )
+            if "netunicorn-environments" in instance.properties and len(instance.properties["netunicorn-environments"]) == 0:
+                del instance.properties["netunicorn-environments"]
             architecture = f'{instance.properties.get("kernel", "").lower()}/{instance.properties.get("osarch", "").lower()}'
             try:
                 instance.architecture = Architecture(architecture)
             except Exception as e:
                 self.logger.warning(
                     f"Unknown architecture {architecture} for node {instance.name}, {e}"
                 )
```

### Comparing `netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/PKG-INFO` & `netunicorn-connector-salt-0.3.4/src/netunicorn_connector_salt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.3
+Version: 0.3.4
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

