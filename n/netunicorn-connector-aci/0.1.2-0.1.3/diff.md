# Comparing `tmp/netunicorn-connector-aci-0.1.2.tar.gz` & `tmp/netunicorn-connector-aci-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-aci-0.1.2.tar", last modified: Sun Apr 30 06:58:59 2023, max compression
+gzip compressed data, was "netunicorn-connector-aci-0.1.3.tar", last modified: Wed May 10 04:35:45 2023, max compression
```

## Comparing `netunicorn-connector-aci-0.1.2.tar` & `netunicorn-connector-aci-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-04-30 06:58:47.000000 netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/connectors/aci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:58:59.303641 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 06:58:59.000000 netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:35:45.795686 netunicorn-connector-aci-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-10 04:35:31.000000 netunicorn-connector-aci-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-10 04:35:45.795686 netunicorn-connector-aci-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-10 04:35:31.000000 netunicorn-connector-aci-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-10 04:35:31.000000 netunicorn-connector-aci-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:35:45.795686 netunicorn-connector-aci-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:35:45.791686 netunicorn-connector-aci-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:35:45.791686 netunicorn-connector-aci-0.1.3/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:35:45.791686 netunicorn-connector-aci-0.1.3/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:35:45.791686 netunicorn-connector-aci-0.1.3/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:35:45.795686 netunicorn-connector-aci-0.1.3/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:35:31.000000 netunicorn-connector-aci-0.1.3/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-10 04:35:31.000000 netunicorn-connector-aci-0.1.3/src/netunicorn/director/infrastructure/connectors/aci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:35:45.795686 netunicorn-connector-aci-0.1.3/src/netunicorn_connector_aci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-10 04:35:45.000000 netunicorn-connector-aci-0.1.3/src/netunicorn_connector_aci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-10 04:35:45.000000 netunicorn-connector-aci-0.1.3/src/netunicorn_connector_aci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:35:45.000000 netunicorn-connector-aci-0.1.3/src/netunicorn_connector_aci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 04:35:45.000000 netunicorn-connector-aci-0.1.3/src/netunicorn_connector_aci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:35:45.000000 netunicorn-connector-aci-0.1.3/src/netunicorn_connector_aci.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-aci-0.1.2/LICENSE` & `netunicorn-connector-aci-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-aci-0.1.2/PKG-INFO` & `netunicorn-connector-aci-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-aci
-Version: 0.1.2
+Version: 0.1.3
 Summary: Azure Container Instances connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-aci-0.1.2/README.md` & `netunicorn-connector-aci-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-aci-0.1.2/pyproject.toml` & `netunicorn-connector-aci-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [project]
 name = "netunicorn-connector-aci"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "Azure Container Instances connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "netunicorn-director-infrastructure >= 0.2.0",
-    "netunicorn-base >= 0.3.0",
+    "netunicorn-base >= 0.3.1",
     "pyyaml",
     "returns",
     "azure-mgmt-resource",
     "azure-mgmt-containerinstance",
     "azure-identity",
 ]
```

### Comparing `netunicorn-connector-aci-0.1.2/src/netunicorn/director/infrastructure/connectors/aci.py` & `netunicorn-connector-aci-0.1.3/src/netunicorn/director/infrastructure/connectors/aci.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,14 +140,15 @@
         available_node_types = [
             Node(
                 name="aci-",
                 architecture=Architecture.LINUX_AMD64,
                 properties={
                     "memory_in_gb": 1,
                     "cpu": 1,
+                    "netunicorn-environments": {"DockerImage"}
                 },
             )
         ]
         return UncountableNodePool(node_template=available_node_types)
 
     async def deploy(
         self,
```

### Comparing `netunicorn-connector-aci-0.1.2/src/netunicorn_connector_aci.egg-info/PKG-INFO` & `netunicorn-connector-aci-0.1.3/src/netunicorn_connector_aci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-aci
-Version: 0.1.2
+Version: 0.1.3
 Summary: Azure Container Instances connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

