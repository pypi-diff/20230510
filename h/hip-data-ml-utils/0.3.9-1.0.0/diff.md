# Comparing `tmp/hip_data_ml_utils-0.3.9.tar.gz` & `tmp/hip_data_ml_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hip_data_ml_utils-0.3.9.tar", max compression
+gzip compressed data, was "hip_data_ml_utils-1.0.0.tar", max compression
```

## Comparing `hip_data_ml_utils-0.3.9.tar` & `hip_data_ml_utils-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1085 2023-04-05 01:12:16.471062 hip_data_ml_utils-0.3.9/LICENSE.txt
--rwxr-xr-x   0        0        0     1548 2023-04-05 01:12:16.471062 hip_data_ml_utils-0.3.9/README.md
--rwxr-xr-x   0        0        0        0 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/core/__init__.py
--rwxr-xr-x   0        0        0      484 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/core/config.py
--rw-r--r--   0        0        0     2158 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/core/databricks_utils.py
--rw-r--r--   0        0        0     3119 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/core/pyathena_utils.py
--rwxr-xr-x   0        0        0        0 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/__init__.py
--rw-r--r--   0        0        0     6616 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py
--rw-r--r--   0        0        0     2708 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py
--rw-r--r--   0        0        0     5287 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py
--rw-r--r--   0        0        0     4470 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py
--rwxr-xr-x   0        0        0        0 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/pyathena_client/__init__.py
--rw-r--r--   0        0        0     4368 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/hip_data_ml_utils/pyathena_client/client.py
--rw-r--r--   0        0        0     1284 2023-04-05 01:12:16.479062 hip_data_ml_utils-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     3791 1970-01-01 00:00:00.000000 hip_data_ml_utils-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-10 00:04:07.293082 hip_data_ml_utils-1.0.0/LICENSE.txt
+-rwxr-xr-x   0        0        0     1548 2023-05-10 00:04:07.293082 hip_data_ml_utils-1.0.0/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-10 00:04:07.297082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/core/__init__.py
+-rwxr-xr-x   0        0        0      642 2023-05-10 00:04:07.297082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/core/config.py
+-rw-r--r--   0        0        0     2158 2023-05-10 00:04:07.297082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/core/databricks_utils.py
+-rw-r--r--   0        0        0     3119 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/core/pyathena_utils.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/__init__.py
+-rw-r--r--   0        0        0     7529 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py
+-rw-r--r--   0        0        0     2578 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py
+-rw-r--r--   0        0        0     6370 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py
+-rw-r--r--   0        0        0     4470 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/pyathena_client/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/hip_data_ml_utils/pyathena_client/client.py
+-rw-r--r--   0        0        0     1284 2023-05-10 00:04:07.301082 hip_data_ml_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3791 1970-01-01 00:00:00.000000 hip_data_ml_utils-1.0.0/PKG-INFO
```

### Comparing `hip_data_ml_utils-0.3.9/LICENSE.txt` & `hip_data_ml_utils-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-0.3.9/README.md` & `hip_data_ml_utils-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-0.3.9/hip_data_ml_utils/core/databricks_utils.py` & `hip_data_ml_utils-1.0.0/hip_data_ml_utils/core/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-0.3.9/hip_data_ml_utils/core/pyathena_utils.py` & `hip_data_ml_utils-1.0.0/hip_data_ml_utils/core/pyathena_utils.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py` & `hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/mlflow_model_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -104,14 +104,47 @@
 
     if key_value_metrics is None:
         return model_metrics_informtion
 
     return model_metrics_informtion[key_value_metrics]
 
 
+def mlflow_get_model_version(
+    mlflow_client: mlflow.tracking.client.MlflowClient,
+    name: str,
+    stage: str = "Production",
+) -> int:
+    """
+    function to get model version of "Staging" or "Production"
+
+    Parameters
+    ----------
+    mlflow_client: mlflow.tracking.client.MlflowClient,
+        initialised mlflow client
+    name: str
+        name of registered model
+    stage: str
+        stage of registered model; Staging or Production
+
+    Returns
+    -------
+    int
+        return the model version of specified registered model tag
+    """
+
+    if stage not in ["Staging", "Production"]:
+        raise ValueError("stage can only be Staging or Production")
+
+    for _, rm in enumerate(mlflow_client.search_model_versions(f"name='{name}'")):
+        if rm.current_stage == stage:
+            return int(rm.version)
+
+    raise ValueError(f"There is no model version with the tag of '{stage}")
+
+
 def mlflow_get_both_registered_model_info_run_id(
     name: str,
     mlflow_client: mlflow.tracking.client.MlflowClient,
     run_id: str = None,
     stage: str = "Production",
 ) -> Tuple[str, Dict]:
     """
```

### Comparing `hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py` & `hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/mlflow_prediction_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 def get_requests(
     model_name: str,
     databricks_cluster_hostname: str,
     databricks_workspace_token: str,
     settings: dict,
     keywords: str,
-    stage_env: str = "Production",
     request_time_out: int = 60,
 ) -> int:
     """
     function to validate response from model endpoint
 
     Parameters
     ----------
@@ -48,29 +47,27 @@
         hostname of the databricks cluster
     databricks_workspace_token: str
         token of the databricks workspace
     settings: dict
         repo settings and configuration
     keywords: str
         keywords to be used for prediction
-    stage_env: str
-        stage of the registered model (e.g. Staging or Production)
     request_time_out: int
         time out for the request
 
     Returns
     -------
     bool
         True if the endpoint was enabled successfully
         raise an exception otherwise
     """
 
     url = (
-        f"""{databricks_cluster_hostname}/model-endpoint/"""
-        f"""{model_name}/{stage_env}/invocations"""
+        f"""{databricks_cluster_hostname}/serving-endpoints/"""
+        f"""{model_name}/invocations"""
     )
     headers = {
         "Authorization": f"Bearer {databricks_workspace_token}",
         "Content-Type": "application/json",
     }
 
     data_json = {
```

### Comparing `hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py` & `hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/mlflow_serve.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import logging
 
 import polling
 import requests
 
+from hip_data_ml_utils.core.config import settings
+
 log = logging.getLogger(__name__)
 
 
 def enable_endpoint(
     databricks_api_url: str,
     model_name: str,
     databricks_cluster_hostname: str,
     databricks_workspace_token: str,
+    dbfs_table_path: str,
+    model_version: int,
     request_time_out: int = 60,
 ) -> bool:
     """
     function to enable the endpoint of a registered model
 
     Parameters
     ----------
@@ -22,38 +26,65 @@
         url of the databricks api
     model_name: str
         name of the registered model
     databricks_cluster_hostname: str
         hostname of the databricks cluster
     databricks_workspace_token: str
         token of the databricks workspace
+    dbfs_table_path: str
+        dbfs file path for inference logging table
+    model_version: inte
+        registered model version of specified stage tag
     request_time_out: int
         timeout for the request
 
     Returns
     -------
     bool
         True if the endpoint was enabled successfully
         raise an exception otherwise
     """
 
     url = f"{databricks_cluster_hostname}/{databricks_api_url}"
-    headers = {"Authorization": f"Bearer {databricks_workspace_token}"}
-    json = {"registered_model_name": model_name}
+    headers = {
+        "Context-Type": "text/json",
+        "Authorization": f"Bearer {databricks_workspace_token}",
+    }
+
+    json = {
+        "name": model_name,
+        "config": {
+            "served_models": [
+                {
+                    "model_name": model_name,
+                    "model_version": model_version,
+                    "workload_size": settings.MODEL_SERVING_WORKLOAD_SIZE,
+                    "scale_to_zero_enabled": settings.MODEL_SERVING_SCALE_TO_ZERO,
+                }
+            ]
+        },
+        "inference_table_config": {"dbfs_destination_path": dbfs_table_path},
+    }
 
     response = requests.post(
         url=url,
         headers=headers,
         json=json,
         timeout=request_time_out,
     )
-    if response.status_code != 200:
-        response.raise_for_status()
+    if response.status_code == 200:
+        return True
+    if (response.status_code == 400) & (
+        response.json()["error_code"] == "RESOURCE_ALREADY_EXISTS"
+    ):
+        return True
 
-    return True
+    response.raise_for_status()
+
+    return False
 
 
 def get_endpoint_state_status(response_json: dict) -> str:
     """
     function that returns endpoint state
 
     Parameters
@@ -63,15 +94,15 @@
 
     Returns
     -------
     str
         returns the state of the endpoint
     """
     try:
-        return response_json["endpoint_status"]["state"]
+        return response_json["state"]["ready"]
     except Exception:
         return "NOT_READY"
 
 
 def get_endpoint_status(
     databricks_api_url: str,
     model_name: str,
@@ -104,28 +135,29 @@
     Returns
     -------
     bool
         True if the endpoint is ready
         raise an exception otherwise
     """
 
-    url = f"{databricks_cluster_hostname}/{databricks_api_url}"
-    headers = {"Authorization": f"Bearer {databricks_workspace_token}"}
-    json = {"registered_model_name": model_name}
+    url = f"{databricks_cluster_hostname}/{databricks_api_url}/{model_name}"
+    headers = {
+        "Context-Type": "text/json",
+        "Authorization": f"Bearer {databricks_workspace_token}",
+    }
 
     polling_response = polling.poll(
         lambda: get_endpoint_state_status(
             requests.get(
                 url=url,
                 headers=headers,
-                json=json,
                 timeout=request_time_out,
             ).json()
         )
-        == "ENDPOINT_STATE_READY",
+        == "READY",
         step=polling_step,
         ignore_exceptions=(requests.exceptions.ConnectionError,),
         poll_forever=False,
         max_tries=polling_max_tries,
     )
 
     if not polling_response:
@@ -133,58 +165,64 @@
 
     return True
 
 
 def update_compute_config(
     databricks_api_url: str,
     model_name: str,
-    stage: str,
     databricks_cluster_hostname: str,
     databricks_workspace_token: str,
     workload_size_id: str,
     scale_to_zero_enabled: str,
+    model_version: int,
     request_time_out: int = 60,
 ) -> int:
     """
     function to scale the endpoint to zero
 
     Parameters
     ----------
     databricks_api_url: str
         url of the databricks api
     model_name: str
         name of the registered model
-    stage: str
-        stage of the registered model (e.g. Staging or Production)
     databricks_cluster_hostname: str
         hostname of the databricks cluster
     databricks_workspace_token: str
         token of the databricks workspace
     workload_size_id: str
         workload size id of the endpoint (e.g. Small, Medium, Large)
     scale_to_zero_enabled: str
         flag to enable/disable scaling to zero
         "true" to enable scaling to zero
         "false" to disable scaling to zero
+    model_version: int
+        registered model version of specified stage tag
     request_time_out: int
         timeout for the request
 
     Returns
     -------
     int
         0 if the compute config is updated successfully, 1 otherwise
     """
-    url = f"{databricks_cluster_hostname}/{databricks_api_url}"
+    url = f"{databricks_cluster_hostname}/{databricks_api_url}/{model_name}/config"
     headers = {"Authorization": f"Bearer {databricks_workspace_token}"}
     json = {
-        "registered_model_name": model_name,
-        "stage": stage.capitalize(),
-        "desired_workload_config_spec": {
-            "workload_size_id": f"{workload_size_id.capitalize()}",
-            "scale_to_zero_enabled": f"{scale_to_zero_enabled}",
+        "served_models": [
+            {
+                "name": model_name,
+                "model_name": model_name,
+                "model_version": model_version,
+                "workload_size": f"{workload_size_id.capitalize()}",
+                "scale_to_zero_enabled": f"{scale_to_zero_enabled}",
+            }
+        ],
+        "traffic_config": {
+            "routes": [{"served_model_name": model_name, "traffic_percentage": 100}]
         },
     }
 
     compute_config_response = requests.put(
         url=url,
         headers=headers,
         json=json,
```

### Comparing `hip_data_ml_utils-0.3.9/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py` & `hip_data_ml_utils-1.0.0/hip_data_ml_utils/mlflow_databricks/mlflow_tracker.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-0.3.9/hip_data_ml_utils/pyathena_client/client.py` & `hip_data_ml_utils-1.0.0/hip_data_ml_utils/pyathena_client/client.py`

 * *Files identical despite different names*

### Comparing `hip_data_ml_utils-0.3.9/pyproject.toml` & `hip_data_ml_utils-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hip_data_ml_utils"
-version = "0.3.9"
+version = "1.0.0"
 description = "Common Python tools and utilities for Hipages ML work"
 authors = ["Hipages Data Team <datascience@hipagesgroup.com.au>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `hip_data_ml_utils-0.3.9/PKG-INFO` & `hip_data_ml_utils-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hip-data-ml-utils
-Version: 0.3.9
+Version: 1.0.0
 Summary: Common Python tools and utilities for Hipages ML work
 License: MIT
 Author: Hipages Data Team
 Author-email: datascience@hipagesgroup.com.au
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

