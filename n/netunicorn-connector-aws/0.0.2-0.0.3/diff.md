# Comparing `tmp/netunicorn-connector-aws-0.0.2.tar.gz` & `tmp/netunicorn-connector-aws-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-aws-0.0.2.tar", last modified: Wed May 10 04:37:49 2023, max compression
+gzip compressed data, was "netunicorn-connector-aws-0.0.3.tar", last modified: Wed May 10 10:26:38 2023, max compression
```

## Comparing `netunicorn-connector-aws-0.0.2.tar` & `netunicorn-connector-aws-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 04:37:38.000000 netunicorn-connector-aws-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-10 04:37:38.000000 netunicorn-connector-aws-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-10 04:37:38.000000 netunicorn-connector-aws-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:37:38.000000 netunicorn-connector-aws-0.0.2/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-05-10 04:37:38.000000 netunicorn-connector-aws-0.0.2/src/netunicorn/director/infrastructure/connectors/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:37:49.438792 netunicorn-connector-aws-0.0.2/src/netunicorn_connector_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 04:37:49.000000 netunicorn-connector-aws-0.0.2/src/netunicorn_connector_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-10 04:37:49.000000 netunicorn-connector-aws-0.0.2/src/netunicorn_connector_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:37:49.000000 netunicorn-connector-aws-0.0.2/src/netunicorn_connector_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 04:37:49.000000 netunicorn-connector-aws-0.0.2/src/netunicorn_connector_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:37:49.000000 netunicorn-connector-aws-0.0.2/src/netunicorn_connector_aws.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 10:26:26.000000 netunicorn-connector-aws-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-10 10:26:26.000000 netunicorn-connector-aws-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-10 10:26:26.000000 netunicorn-connector-aws-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:26:26.000000 netunicorn-connector-aws-0.0.3/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-05-10 10:26:26.000000 netunicorn-connector-aws-0.0.3/src/netunicorn/director/infrastructure/connectors/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:26:38.012381 netunicorn-connector-aws-0.0.3/src/netunicorn_connector_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 10:26:38.000000 netunicorn-connector-aws-0.0.3/src/netunicorn_connector_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-10 10:26:38.000000 netunicorn-connector-aws-0.0.3/src/netunicorn_connector_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:26:38.000000 netunicorn-connector-aws-0.0.3/src/netunicorn_connector_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 10:26:38.000000 netunicorn-connector-aws-0.0.3/src/netunicorn_connector_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 10:26:38.000000 netunicorn-connector-aws-0.0.3/src/netunicorn_connector_aws.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-aws-0.0.2/LICENSE` & `netunicorn-connector-aws-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-aws-0.0.2/PKG-INFO` & `netunicorn-connector-aws-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-aws
-Version: 0.0.2
+Version: 0.0.3
 Summary: AWS connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-aws-0.0.2/README.md` & `netunicorn-connector-aws-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-aws-0.0.2/pyproject.toml` & `netunicorn-connector-aws-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-connector-aws"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "AWS connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-connector-aws-0.0.2/src/netunicorn/director/infrastructure/connectors/aws.py` & `netunicorn-connector-aws-0.0.3/src/netunicorn/director/infrastructure/connectors/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,30 +78,37 @@
         self.ecs_client = boto3.client(
             "ecs",
             region_name=self.default_region,
             aws_access_key_id=self.access_key,
             aws_secret_access_key=self.secret_key,
         )
 
-        clusters = self.ecs_client.list_clusters()
-        if self.cluster not in clusters["clusterArns"]:
+        clusters = self.__get_cluster_names()
+        if self.cluster not in clusters:
             self.logger.info(f"Cluster {self.cluster} does not exist, creating...")
             self.ecs_client.create_cluster(
                 clusterName=self.cluster,
                 capacityProviders=["FARGATE"],
                 defaultCapacityProviderStrategy=[
                     {
                         "capacityProvider": "FARGATE",
                     }
                 ],
             )
 
         self.cleaner_task: Optional[asyncio.Task] = None
         self.logger.info("AWS Fargate connector initialized")
 
+    def __get_cluster_names(self) -> set[str]:
+        clusters = self.ecs_client.list_clusters()
+        result = set()
+        for cluster in clusters["clusterArns"]:
+            result.add(cluster.split("/")[1])
+        return result
+
     async def __periodic_cleaner(self) -> NoReturn:
         """
         Periodically clean stopped containers and deregistered tasks
         """
         self.logger.info("Starting AWS Fargate cleaner")
         while True:
             try:
@@ -222,16 +229,16 @@
         return False
 
     async def initialize(self, *args: Any, **kwargs: Any) -> None:
         self.cleaner_task = asyncio.create_task(self.__periodic_cleaner())
 
     async def health(self, *args: Any, **kwargs: Any) -> Tuple[bool, str]:
         try:
-            clusters = self.ecs_client.list_clusters()
-            if self.cluster not in clusters["clusterArns"]:
+            clusters = self.__get_cluster_names()
+            if self.cluster not in clusters:
                 return False, f"Cluster {self.cluster} is not found"
             return True, ""
         except Exception as e:
             self.logger.exception(e)
             return False, str(e)
 
     async def shutdown(self, *args: Any, **kwargs: Any) -> None:
```

### Comparing `netunicorn-connector-aws-0.0.2/src/netunicorn_connector_aws.egg-info/PKG-INFO` & `netunicorn-connector-aws-0.0.3/src/netunicorn_connector_aws.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-aws
-Version: 0.0.2
+Version: 0.0.3
 Summary: AWS connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

