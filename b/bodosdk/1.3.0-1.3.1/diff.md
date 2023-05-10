# Comparing `tmp/bodosdk-1.3.0.tar.gz` & `tmp/bodosdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-1.3.0.tar", last modified: Thu May  4 04:38:57 2023, max compression
+gzip compressed data, was "bodosdk-1.3.1.tar", last modified: Wed May 10 04:20:48 2023, max compression
```

## Comparing `bodosdk-1.3.0.tar` & `bodosdk-1.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-04 04:38:51.000000 bodosdk-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-04 04:38:51.000000 bodosdk-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-04 04:38:57.904533 bodosdk-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    35454 2023-05-04 04:38:51.000000 bodosdk-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    12693 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/client/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.904533 bodosdk-1.3.0/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    14687 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-04 04:38:51.000000 bodosdk-1.3.0/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 04:38:57.900533 bodosdk-1.3.0/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-04 04:38:57.000000 bodosdk-1.3.0/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-04 04:38:57.904533 bodosdk-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-05-04 04:38:51.000000 bodosdk-1.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-05-04 04:38:51.000000 bodosdk-1.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.287792 bodosdk-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-05-10 04:20:40.000000 bodosdk-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-10 04:20:40.000000 bodosdk-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-10 04:20:48.287792 bodosdk-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    35454 2023-05-10 04:20:40.000000 bodosdk-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.287792 bodosdk-1.3.1/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-10 04:20:48.287792 bodosdk-1.3.1/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.279792 bodosdk-1.3.1/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8160 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1494 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.283792 bodosdk-1.3.1/bodosdk/client/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12094 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.287792 bodosdk-1.3.1/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14687 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-05-10 04:20:40.000000 bodosdk-1.3.1/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 04:20:48.275792 bodosdk-1.3.1/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-10 04:20:48.000000 bodosdk-1.3.1/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-10 04:20:48.287792 bodosdk-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-05-10 04:20:40.000000 bodosdk-1.3.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-05-10 04:20:40.000000 bodosdk-1.3.1/versioneer.py
```

### Comparing `bodosdk-1.3.0/LICENSE` & `bodosdk-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/PKG-INFO` & `bodosdk-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodosdk-1.3.0/README.md` & `bodosdk-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/auth.py` & `bodosdk-1.3.1/bodosdk/api/auth.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/base.py` & `bodosdk-1.3.1/bodosdk/api/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/catalog.py` & `bodosdk-1.3.1/bodosdk/api/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/cloud_config.py` & `bodosdk-1.3.1/bodosdk/api/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/cluster.py` & `bodosdk-1.3.1/bodosdk/api/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/instance_role.py` & `bodosdk-1.3.1/bodosdk/api/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/job.py` & `bodosdk-1.3.1/bodosdk/api/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,27 @@
             raise ResourceNotFound
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable(resp.content)
         json_data = resp.json()
         return BatchJobDefinitionResponse(**json_data)
 
     @validate_arguments
+    def get_batch_job_definition_by_name(self, name: str) -> BatchJobDefinitionResponse:
+        headers = self.get_auth_header()
+        resp = self._requests.get(
+            f"{self.get_resource_url()}/batch_job_def/name/{name}", headers=headers
+        )
+        if resp.status_code == 404:
+            raise ResourceNotFound
+        if str(resp.status_code).startswith("5"):
+            raise ServiceUnavailable
+        json_data = resp.json()
+        return BatchJobDefinitionResponse(**json_data)
+
+    @validate_arguments
     def update_batch_job_definition(
         self, uuid: UUID, config_override: JobConfigOverride
     ) -> BatchJobDefinitionResponse:
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
         resp = self._requests.patch(
             f"{self.get_resource_url()}/batch_job_def/{uuid}",
@@ -302,14 +315,26 @@
         )
         if resp.status_code == 404:
             raise ResourceNotFound
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
         return
 
+    def cancel_all_job_runs(self, cluster_uuids: Union[List[str], List[UUID]]) -> None:
+        headers = self.get_auth_header()
+        query_string = build_query_string({"cluster_ids": cluster_uuids})
+        resp = self._requests.delete(
+            f"{self.get_resource_url()}/runs{query_string}", headers=headers
+        )
+        if resp.status_code == 404:
+            raise ResourceNotFound
+        if str(resp.status_code).startswith("5"):
+            raise ServiceUnavailable
+        return
+
     @validate_arguments
     def list_job_runs(
         self,
         job_type: List[JobRunType] = None,
         batch_job_id: Union[List[UUID], None] = None,
         status: Union[List[JobRunStatus], None] = None,
         cluster_id: Union[List[UUID], None] = None,
```

### Comparing `bodosdk-1.3.0/bodosdk/api/request_wrapper.py` & `bodosdk-1.3.1/bodosdk/api/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/secret_group.py` & `bodosdk-1.3.1/bodosdk/api/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/secrets.py` & `bodosdk-1.3.1/bodosdk/api/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/api/workspace.py` & `bodosdk-1.3.1/bodosdk/api/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/client/base.py` & `bodosdk-1.3.1/bodosdk/client/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/client/catalog.py` & `bodosdk-1.3.1/bodosdk/client/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/client/cloud_config.py` & `bodosdk-1.3.1/bodosdk/client/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/client/cluster.py` & `bodosdk-1.3.1/bodosdk/client/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/client/instance_role.py` & `bodosdk-1.3.1/bodosdk/client/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/client/job.py` & `bodosdk-1.3.1/bodosdk/client/job.py`

 * *Files 17% similar despite different names*

```diff
@@ -170,14 +170,29 @@
         :raises ResourceNotFound:
         """
         try:
             return self._api.get_batch_job_definition(uuid)
         except Exception as exception:
             raise exception
 
+    def get_batch_job_definition_by_name(self, name: str) -> BatchJobDefinitionResponse:
+        """
+        Gets specific batch job definition from workspace
+
+        :param name:
+        :type name: str
+        :return: batch job definition
+        :rtype: BatchJobDefinition
+        :raises ResourceNotFound:
+        """
+        try:
+            return self._api.get_batch_job_definition_by_name(name)
+        except Exception as exception:
+            raise exception
+
     def create_batch_job_definition(
         self, create_batch_job_definition: CreateBatchJobDefinition
     ) -> BatchJobDefinitionResponse:
         """
         Creates a batch job definition
 
         :param create_batch_job_definition:
@@ -206,33 +221,73 @@
         try:
             self._api.delete_batch_job_definition(uuid)
         except Exception as exception:
             raise exception
 
     def list_batch_job_runs(
         self,
-        batch_job_id: List[UUID] = None,
+        batch_job_ids: List[UUID] = None,
         status: List[JobRunStatus] = None,
         cluster_id: List[UUID] = None,
         started_at: datetime = None,
         finished_at: datetime = None,
     ) -> List[JobRunResponse]:
         batch_job_runs = self._api.list_job_runs(
             job_type=[JobRunType.BATCH],
-            batch_job_id=batch_job_id,
+            batch_job_id=batch_job_ids,
             status=status,
             cluster_id=cluster_id,
             started_at=started_at,
             finished_at=finished_at,
         )
 
         if len(batch_job_runs) == 0:
             logging.warning("No batch job runs found.")
         return batch_job_runs
 
+    def list_batch_job_runs_by_names(
+        self,
+        batch_job_names: List[str] = None,
+        status: List[JobRunStatus] = None,
+        cluster_id: List[UUID] = None,
+        started_at: datetime = None,
+        finished_at: datetime = None,
+    ) -> List[JobRunResponse]:
+        """
+        List all batch job runs in workspace using batch job name
+
+        :param batch_job_names:
+        :type batch_job_names: List[str]
+        :param status:
+        :type status: List[JobRunStatus]
+        :param cluster_id:
+        :type cluster_id: List[UUID]
+        :param started_at:
+        :type started_at: datetime
+        :param finished_at:
+        :type finished_at: datetime
+        :return: list of batch job runs
+        :rtype: List[JobRunResponse]
+
+        """
+        batch_job_ids = []
+        for name in batch_job_names:
+            batch_job_def_uuid = self.get_batch_job_definition_by_name(name).uuid
+            batch_job_ids.append(batch_job_def_uuid)
+
+        batch_job_runs = self._api.list_job_runs(
+            job_type=[JobRunType.BATCH],
+            batch_job_id=batch_job_ids,
+            status=status,
+            cluster_id=cluster_id,
+            started_at=started_at,
+            finished_at=finished_at,
+        )
+        return batch_job_runs
+
     def get_batch_job_run(self, uuid: Union[str, UUID]) -> JobRunResponse:
         """
         Gets specific batch job run from workspace
 
         :param uuid:
         :type uuid: Union[str, UUID]
         :return: batch job run
@@ -297,7 +352,33 @@
         """
         try:
             job_run = self._api.create_sql_job_run(create_sql_job_run)
             logging.info(f"Sql job run {job_run.uuid} submitted.")
             return job_run
         except Exception as exception:
             raise exception
+
+    def cancel_batch_job_run(self, uuid: Union[str, UUID]) -> None:
+        """
+        Cancels batch job run
+
+        :param uuid:
+        :type uuid: Union[str, UUID]
+        :return: None
+        :rtype: None
+        :raises ResourceNotFound:
+        """
+        try:
+            self._api.cancel_batch_job_run(uuid)
+        except Exception as exception:
+            raise exception
+
+    def cancelAllJobRuns(self, cluster_uuids: Union[List[str], List[UUID]] = None):
+        """
+        Cancels all job runs in workspace or for specified clusters
+
+        :return: None
+        """
+        try:
+            self._api.cancel_all_job_runs(cluster_uuids)
+        except Exception as exception:
+            raise exception
```

### Comparing `bodosdk-1.3.0/bodosdk/client/secret_group.py` & `bodosdk-1.3.1/bodosdk/client/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/client/secrets.py` & `bodosdk-1.3.1/bodosdk/client/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/client/workspace.py` & `bodosdk-1.3.1/bodosdk/client/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/models/__init__.py` & `bodosdk-1.3.1/bodosdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/models/base.py` & `bodosdk-1.3.1/bodosdk/models/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/models/catalog.py` & `bodosdk-1.3.1/bodosdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/models/cloud_config.py` & `bodosdk-1.3.1/bodosdk/models/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/models/cluster.py` & `bodosdk-1.3.1/bodosdk/models/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/models/job.py` & `bodosdk-1.3.1/bodosdk/models/job.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk/models/workspace.py` & `bodosdk-1.3.1/bodosdk/models/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/bodosdk.egg-info/PKG-INFO` & `bodosdk-1.3.1/bodosdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodosdk-1.3.0/bodosdk.egg-info/SOURCES.txt` & `bodosdk-1.3.1/bodosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/setup.py` & `bodosdk-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.3.0/versioneer.py` & `bodosdk-1.3.1/versioneer.py`

 * *Files identical despite different names*

