# Comparing `tmp/netunicorn-connector-docker-0.1.1.tar.gz` & `tmp/netunicorn-connector-docker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-docker-0.1.1.tar", last modified: Tue Apr 11 09:45:16 2023, max compression
+gzip compressed data, was "netunicorn-connector-docker-0.1.2.tar", last modified: Wed May 10 04:39:41 2023, max compression
```

## Comparing `netunicorn-connector-docker-0.1.1.tar` & `netunicorn-connector-docker-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.393097 netunicorn-connector-docker-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.393097 netunicorn-connector-docker-0.1.1/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.393097 netunicorn-connector-docker-0.1.1/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.393097 netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/connectors/docker_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:39:41.569633 netunicorn-connector-docker-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 04:39:30.000000 netunicorn-connector-docker-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-10 04:39:41.569633 netunicorn-connector-docker-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-10 04:39:30.000000 netunicorn-connector-docker-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 04:39:30.000000 netunicorn-connector-docker-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:39:41.569633 netunicorn-connector-docker-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:39:41.565633 netunicorn-connector-docker-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:39:41.565633 netunicorn-connector-docker-0.1.2/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:39:41.565633 netunicorn-connector-docker-0.1.2/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:39:41.565633 netunicorn-connector-docker-0.1.2/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:39:41.565633 netunicorn-connector-docker-0.1.2/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 04:39:30.000000 netunicorn-connector-docker-0.1.2/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-05-10 04:39:30.000000 netunicorn-connector-docker-0.1.2/src/netunicorn/director/infrastructure/connectors/docker_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:39:41.569633 netunicorn-connector-docker-0.1.2/src/netunicorn_connector_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-10 04:39:41.000000 netunicorn-connector-docker-0.1.2/src/netunicorn_connector_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-10 04:39:41.000000 netunicorn-connector-docker-0.1.2/src/netunicorn_connector_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:39:41.000000 netunicorn-connector-docker-0.1.2/src/netunicorn_connector_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:39:41.000000 netunicorn-connector-docker-0.1.2/src/netunicorn_connector_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:39:41.000000 netunicorn-connector-docker-0.1.2/src/netunicorn_connector_docker.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-docker-0.1.1/LICENSE` & `netunicorn-connector-docker-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-docker-0.1.1/pyproject.toml` & `netunicorn-connector-docker-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "netunicorn-connector-docker"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "Local Docker connector for netunicorn"
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
     "docker",
     "returns",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/connectors/docker_connector.py` & `netunicorn-connector-docker-0.1.2/src/netunicorn/director/infrastructure/connectors/docker_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
         if configuration is None:
             self.base_url = 'unix://var/run/docker.sock'
             self.default_network = None
         else:
             with open(configuration, 'r') as f:
                 config = yaml.safe_load(f)
-            self.base_url = config['netunicorn.infrastructure.connectors.docker.base_url']
-            self.default_network = config.get('netunicorn.infrastructure.providers.docker.default_network', None)
+            self.base_url = config['netunicorn.docker.base_url']
+            self.default_network = config.get('netunicorn.docker.default_network', None)
 
         self.client = docker.DockerClient(base_url=self.base_url)
         self.netunicorn_gateway = netunicorn_gateway
         self.logger = logger or logging.getLogger(__name__)
         self.nodename = 'dockerhost'
 
         version = self.client.version()
@@ -79,15 +79,17 @@
             authentication_context: Optional[dict[str, str]] = None,
             *args: Any,
             **kwargs: Any,
     ) -> Nodes:
         pool = CountableNodePool([
             Node(
                 name=self.nodename,
-                properties={},
+                properties={
+                    "netunicorn-environments": {"DockerImage"}
+                },
                 architecture=self.architecture
             )
         ])
         self.logger.debug(f"Returning nodes: {pool}")
         return pool
 
     async def deploy(
```

