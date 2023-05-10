# Comparing `tmp/sensorbucket-1.0.0.tar.gz` & `tmp/sensorbucket-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensorbucket-1.0.0.tar", last modified: Wed May 10 09:41:21 2023, max compression
+gzip compressed data, was "sensorbucket-1.0.1.tar", last modified: Wed May 10 11:19:10 2023, max compression
```

## Comparing `sensorbucket-1.0.0.tar` & `sensorbucket-1.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      816 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/PKG-INFO
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     7280 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/README.md
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.023907 sensorbucket-1.0.0/openapi_client/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     4124 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/__init__.py
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.023907 sensorbucket-1.0.0/openapi_client/api/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      276 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/__init__.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    73878 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/devices_api.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    25492 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/measurements_api.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    41586 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/pipelines_api.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     8949 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api/uplink_api.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    30485 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api_client.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      844 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/api_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    15684 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/configuration.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     5599 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/exceptions.py
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/openapi_client/models/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3352 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/__init__.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2761 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_device201_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3030 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_device_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2470 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_device_sensor201_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2785 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_pipeline200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2532 2023-05-10 09:31:33.000000 sensorbucket-1.0.0/openapi_client/models/create_pipeline_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2970 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/create_sensor_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2943 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/datastream.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2470 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/delete_device_sensor200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3682 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/device.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2446 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/disable_pipeline200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2737 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/get_device200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2761 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/get_pipeline200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3499 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_datastreams200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2921 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_datastreams200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3499 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_device_sensors200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2921 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_device_sensors200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3451 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_devices200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2873 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_devices200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3475 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_pipelines200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2897 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/list_pipelines200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     6406 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/measurement.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2992 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/paginated_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2500 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/paginated_response_links.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2836 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/pipeline.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3519 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/query_measurements200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2941 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/query_measurements200_response_all_of.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3067 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/sensor.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2422 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/update_device200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2965 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/update_device_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2785 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/update_pipeline200_response.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2807 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/models/update_pipeline_request.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)    13245 2023-05-10 09:31:34.000000 sensorbucket-1.0.0/openapi_client/rest.py
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      713 2023-05-10 09:39:16.000000 sensorbucket-1.0.0/pyproject.toml
-drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/sensorbucket.egg-info/
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)      816 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/PKG-INFO
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2153 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/SOURCES.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)        1 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/dependency_links.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       58 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/requires.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       15 2023-05-10 09:41:21.000000 sensorbucket-1.0.0/sensorbucket.egg-info/top_level.txt
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)       69 2023-05-10 09:41:21.027241 sensorbucket-1.0.0/setup.cfg
--rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2134 2023-05-10 09:41:14.000000 sensorbucket-1.0.0/setup.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.371816 sensorbucket-1.0.1/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      813 2023-05-10 11:19:10.371816 sensorbucket-1.0.1/PKG-INFO
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     7260 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/README.md
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      675 2023-05-10 11:18:49.000000 sensorbucket-1.0.1/pyproject.toml
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.368483 sensorbucket-1.0.1/sensorbucket/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     4036 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/__init__.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.368483 sensorbucket-1.0.1/sensorbucket/api/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      268 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/__init__.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    73852 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/devices_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    25482 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/measurements_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    41566 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/pipelines_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     8943 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api/uplink_api.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    30473 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api_client.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      844 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/api_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    15678 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/configuration.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     5599 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/exceptions.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.371816 sensorbucket-1.0.1/sensorbucket/models/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3290 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/__init__.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2759 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_device201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3030 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_device_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2470 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_device_sensor201_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2783 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2532 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_pipeline_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2970 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/create_sensor_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2943 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/datastream.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2470 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/delete_device_sensor200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3680 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/device.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2446 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/disable_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2735 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/get_device200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2759 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/get_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3495 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_datastreams200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2919 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_datastreams200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3495 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_device_sensors200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2919 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_device_sensors200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3447 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_devices200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2871 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_devices200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3471 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_pipelines200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2895 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/list_pipelines200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     6406 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/measurement.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2990 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/paginated_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2500 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/paginated_response_links.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2836 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/pipeline.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3515 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/query_measurements200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2939 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/query_measurements200_response_all_of.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     3067 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/sensor.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2422 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/update_device200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2965 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/update_device_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2783 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/update_pipeline200_response.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2807 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/models/update_pipeline_request.py
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)    13243 2023-05-10 11:15:39.000000 sensorbucket-1.0.1/sensorbucket/rest.py
+drwxr-xr-x   0 timvosch  (1000) timvosch  (1000)        0 2023-05-10 11:19:10.368483 sensorbucket-1.0.1/sensorbucket.egg-info/
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)      813 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/PKG-INFO
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2067 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/SOURCES.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)        1 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/dependency_links.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       58 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/requires.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       13 2023-05-10 11:19:10.000000 sensorbucket-1.0.1/sensorbucket.egg-info/top_level.txt
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)       69 2023-05-10 11:19:10.371816 sensorbucket-1.0.1/setup.cfg
+-rw-r--r--   0 timvosch  (1000) timvosch  (1000)     2131 2023-05-10 11:19:04.000000 sensorbucket-1.0.1/setup.py
```

### Comparing `sensorbucket-1.0.0/PKG-INFO` & `sensorbucket-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sensorbucket
-Version: 1.0.0
-Summary: Sensorbucket client
+Version: 1.0.1
+Summary: Sensorbucket API
 Home-page: https://sensorbucket.nl
 Author: Tim van Osch
 Author-email: info@pollex.nl
 License: EUPLv1.2
 Keywords: OpenAPI,OpenAPI-Generator,Sensorbucket API
 Description-Content-Type: text/markdown
```

### Comparing `sensorbucket-1.0.0/README.md` & `sensorbucket-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# openapi-client
+# sensorbucket
 SensorBucket processes data from different sources and devices into a single standardized format. 
 An applications connected to SensorBucket, can use all devices SensorBucket supports.
 
 Missing a device or source? SensorBucket is designed to be scalable and extendable. Create your own worker
 that receives data from an AMQP source, process said data and output in the expected worker output format.
 
 Find out more at: https://developer.sensorbucket.nl/
@@ -29,69 +29,69 @@
 ```sh
 pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
 ```
 (you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
-import openapi_client
+import sensorbucket
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import openapi_client
+import sensorbucket
 ```
 
 ### Tests
 
 Execute `pytest` to run the tests.
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
 import time
-import openapi_client
-from openapi_client.rest import ApiException
+import sensorbucket
+from sensorbucket.rest import ApiException
 from pprint import pprint
 
 # Defining the host is optional and defaults to https://sensorbucket.nl/api
 # See configuration.py for a list of all supported configuration parameters.
-configuration = openapi_client.Configuration(
+configuration = sensorbucket.Configuration(
     host = "https://sensorbucket.nl/api"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
 # Configure HTTP basic authorization: basicAuth
-configuration = openapi_client.Configuration(
+configuration = sensorbucket.Configuration(
     username = os.environ["USERNAME"],
     password = os.environ["PASSWORD"]
 )
 
 
 # Enter a context with an instance of the API client
-with openapi_client.ApiClient(configuration) as api_client:
+with sensorbucket.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = openapi_client.DevicesApi(api_client)
-    create_device_request = openapi_client.CreateDeviceRequest() # CreateDeviceRequest |  (optional)
+    api_instance = sensorbucket.DevicesApi(api_client)
+    create_device_request = sensorbucket.CreateDeviceRequest() # CreateDeviceRequest |  (optional)
 
     try:
         # Create device
         api_response = api_instance.create_device(create_device_request=create_device_request)
         print("The response of DevicesApi->create_device:\n")
         pprint(api_response)
     except ApiException as e:
```

### Comparing `sensorbucket-1.0.0/openapi_client/__init__.py` & `sensorbucket-1.0.1/sensorbucket/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,55 +14,55 @@
     Do not edit the class manually.
 """
 
 
 __version__ = "1.0.0"
 
 # import apis into sdk package
-from openapi_client.api.devices_api import DevicesApi
-from openapi_client.api.measurements_api import MeasurementsApi
-from openapi_client.api.pipelines_api import PipelinesApi
-from openapi_client.api.uplink_api import UplinkApi
+from sensorbucket.api.devices_api import DevicesApi
+from sensorbucket.api.measurements_api import MeasurementsApi
+from sensorbucket.api.pipelines_api import PipelinesApi
+from sensorbucket.api.uplink_api import UplinkApi
 
 # import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.api_client import ApiClient
-from openapi_client.configuration import Configuration
-from openapi_client.exceptions import OpenApiException
-from openapi_client.exceptions import ApiTypeError
-from openapi_client.exceptions import ApiValueError
-from openapi_client.exceptions import ApiKeyError
-from openapi_client.exceptions import ApiAttributeError
-from openapi_client.exceptions import ApiException
+from sensorbucket.api_response import ApiResponse
+from sensorbucket.api_client import ApiClient
+from sensorbucket.configuration import Configuration
+from sensorbucket.exceptions import OpenApiException
+from sensorbucket.exceptions import ApiTypeError
+from sensorbucket.exceptions import ApiValueError
+from sensorbucket.exceptions import ApiKeyError
+from sensorbucket.exceptions import ApiAttributeError
+from sensorbucket.exceptions import ApiException
 
 # import models into sdk package
-from openapi_client.models.create_device201_response import CreateDevice201Response
-from openapi_client.models.create_device_request import CreateDeviceRequest
-from openapi_client.models.create_device_sensor201_response import CreateDeviceSensor201Response
-from openapi_client.models.create_pipeline200_response import CreatePipeline200Response
-from openapi_client.models.create_pipeline_request import CreatePipelineRequest
-from openapi_client.models.create_sensor_request import CreateSensorRequest
-from openapi_client.models.datastream import Datastream
-from openapi_client.models.delete_device_sensor200_response import DeleteDeviceSensor200Response
-from openapi_client.models.device import Device
-from openapi_client.models.disable_pipeline200_response import DisablePipeline200Response
-from openapi_client.models.get_device200_response import GetDevice200Response
-from openapi_client.models.get_pipeline200_response import GetPipeline200Response
-from openapi_client.models.list_datastreams200_response import ListDatastreams200Response
-from openapi_client.models.list_datastreams200_response_all_of import ListDatastreams200ResponseAllOf
-from openapi_client.models.list_device_sensors200_response import ListDeviceSensors200Response
-from openapi_client.models.list_device_sensors200_response_all_of import ListDeviceSensors200ResponseAllOf
-from openapi_client.models.list_devices200_response import ListDevices200Response
-from openapi_client.models.list_devices200_response_all_of import ListDevices200ResponseAllOf
-from openapi_client.models.list_pipelines200_response import ListPipelines200Response
-from openapi_client.models.list_pipelines200_response_all_of import ListPipelines200ResponseAllOf
-from openapi_client.models.measurement import Measurement
-from openapi_client.models.paginated_response import PaginatedResponse
-from openapi_client.models.paginated_response_links import PaginatedResponseLinks
-from openapi_client.models.pipeline import Pipeline
-from openapi_client.models.query_measurements200_response import QueryMeasurements200Response
-from openapi_client.models.query_measurements200_response_all_of import QueryMeasurements200ResponseAllOf
-from openapi_client.models.sensor import Sensor
-from openapi_client.models.update_device200_response import UpdateDevice200Response
-from openapi_client.models.update_device_request import UpdateDeviceRequest
-from openapi_client.models.update_pipeline200_response import UpdatePipeline200Response
-from openapi_client.models.update_pipeline_request import UpdatePipelineRequest
+from sensorbucket.models.create_device201_response import CreateDevice201Response
+from sensorbucket.models.create_device_request import CreateDeviceRequest
+from sensorbucket.models.create_device_sensor201_response import CreateDeviceSensor201Response
+from sensorbucket.models.create_pipeline200_response import CreatePipeline200Response
+from sensorbucket.models.create_pipeline_request import CreatePipelineRequest
+from sensorbucket.models.create_sensor_request import CreateSensorRequest
+from sensorbucket.models.datastream import Datastream
+from sensorbucket.models.delete_device_sensor200_response import DeleteDeviceSensor200Response
+from sensorbucket.models.device import Device
+from sensorbucket.models.disable_pipeline200_response import DisablePipeline200Response
+from sensorbucket.models.get_device200_response import GetDevice200Response
+from sensorbucket.models.get_pipeline200_response import GetPipeline200Response
+from sensorbucket.models.list_datastreams200_response import ListDatastreams200Response
+from sensorbucket.models.list_datastreams200_response_all_of import ListDatastreams200ResponseAllOf
+from sensorbucket.models.list_device_sensors200_response import ListDeviceSensors200Response
+from sensorbucket.models.list_device_sensors200_response_all_of import ListDeviceSensors200ResponseAllOf
+from sensorbucket.models.list_devices200_response import ListDevices200Response
+from sensorbucket.models.list_devices200_response_all_of import ListDevices200ResponseAllOf
+from sensorbucket.models.list_pipelines200_response import ListPipelines200Response
+from sensorbucket.models.list_pipelines200_response_all_of import ListPipelines200ResponseAllOf
+from sensorbucket.models.measurement import Measurement
+from sensorbucket.models.paginated_response import PaginatedResponse
+from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
+from sensorbucket.models.pipeline import Pipeline
+from sensorbucket.models.query_measurements200_response import QueryMeasurements200Response
+from sensorbucket.models.query_measurements200_response_all_of import QueryMeasurements200ResponseAllOf
+from sensorbucket.models.sensor import Sensor
+from sensorbucket.models.update_device200_response import UpdateDevice200Response
+from sensorbucket.models.update_device_request import UpdateDeviceRequest
+from sensorbucket.models.update_pipeline200_response import UpdatePipeline200Response
+from sensorbucket.models.update_pipeline_request import UpdatePipelineRequest
```

### Comparing `sensorbucket-1.0.0/openapi_client/api/devices_api.py` & `sensorbucket-1.0.1/sensorbucket/api/devices_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,28 @@
 from typing_extensions import Annotated
 from typing import Generator 
 
 from pydantic import Field, StrictFloat, StrictInt, StrictStr
 
 from typing import Optional, Union
 
-from openapi_client.models.create_device201_response import CreateDevice201Response
-from openapi_client.models.create_device_request import CreateDeviceRequest
-from openapi_client.models.create_device_sensor201_response import CreateDeviceSensor201Response
-from openapi_client.models.create_sensor_request import CreateSensorRequest
-from openapi_client.models.delete_device_sensor200_response import DeleteDeviceSensor200Response
-from openapi_client.models.get_device200_response import GetDevice200Response
-from openapi_client.models.list_device_sensors200_response import ListDeviceSensors200Response
-from openapi_client.models.list_devices200_response import ListDevices200Response
-from openapi_client.models.update_device200_response import UpdateDevice200Response
-from openapi_client.models.update_device_request import UpdateDeviceRequest
+from sensorbucket.models.create_device201_response import CreateDevice201Response
+from sensorbucket.models.create_device_request import CreateDeviceRequest
+from sensorbucket.models.create_device_sensor201_response import CreateDeviceSensor201Response
+from sensorbucket.models.create_sensor_request import CreateSensorRequest
+from sensorbucket.models.delete_device_sensor200_response import DeleteDeviceSensor200Response
+from sensorbucket.models.get_device200_response import GetDevice200Response
+from sensorbucket.models.list_device_sensors200_response import ListDeviceSensors200Response
+from sensorbucket.models.list_devices200_response import ListDevices200Response
+from sensorbucket.models.update_device200_response import UpdateDevice200Response
+from sensorbucket.models.update_device_request import UpdateDeviceRequest
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from sensorbucket.api_client import ApiClient
+from sensorbucket.api_response import ApiResponse
+from sensorbucket.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 class DevicesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
```

### Comparing `sensorbucket-1.0.0/openapi_client/api/measurements_api.py` & `sensorbucket-1.0.1/sensorbucket/api/measurements_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 from typing_extensions import Annotated
 from typing import Generator 
 
 from pydantic import Field, StrictFloat, StrictInt, StrictStr
 
 from typing import Optional, Union
 
-from openapi_client.models.list_datastreams200_response import ListDatastreams200Response
-from openapi_client.models.query_measurements200_response import QueryMeasurements200Response
+from sensorbucket.models.list_datastreams200_response import ListDatastreams200Response
+from sensorbucket.models.query_measurements200_response import QueryMeasurements200Response
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from sensorbucket.api_client import ApiClient
+from sensorbucket.api_response import ApiResponse
+from sensorbucket.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 class MeasurementsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
```

### Comparing `sensorbucket-1.0.0/openapi_client/api/pipelines_api.py` & `sensorbucket-1.0.1/sensorbucket/api/pipelines_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 from typing_extensions import Annotated
 from typing import Generator 
 
 from pydantic import Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist
 
 from typing import Optional, Union
 
-from openapi_client.models.create_pipeline200_response import CreatePipeline200Response
-from openapi_client.models.create_pipeline_request import CreatePipelineRequest
-from openapi_client.models.disable_pipeline200_response import DisablePipeline200Response
-from openapi_client.models.get_pipeline200_response import GetPipeline200Response
-from openapi_client.models.list_pipelines200_response import ListPipelines200Response
-from openapi_client.models.update_pipeline200_response import UpdatePipeline200Response
-from openapi_client.models.update_pipeline_request import UpdatePipelineRequest
+from sensorbucket.models.create_pipeline200_response import CreatePipeline200Response
+from sensorbucket.models.create_pipeline_request import CreatePipelineRequest
+from sensorbucket.models.disable_pipeline200_response import DisablePipeline200Response
+from sensorbucket.models.get_pipeline200_response import GetPipeline200Response
+from sensorbucket.models.list_pipelines200_response import ListPipelines200Response
+from sensorbucket.models.update_pipeline200_response import UpdatePipeline200Response
+from sensorbucket.models.update_pipeline_request import UpdatePipelineRequest
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from sensorbucket.api_client import ApiClient
+from sensorbucket.api_response import ApiResponse
+from sensorbucket.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 class PipelinesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
```

### Comparing `sensorbucket-1.0.0/openapi_client/api/uplink_api.py` & `sensorbucket-1.0.1/sensorbucket/api/uplink_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 from typing import Generator 
 
 from pydantic import Field, StrictStr
 
 from typing import Any, Dict, Optional
 
 
-from openapi_client.api_client import ApiClient
-from openapi_client.api_response import ApiResponse
-from openapi_client.exceptions import (  # noqa: F401
+from sensorbucket.api_client import ApiClient
+from sensorbucket.api_response import ApiResponse
+from sensorbucket.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 class UplinkApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
```

### Comparing `sensorbucket-1.0.0/openapi_client/api_client.py` & `sensorbucket-1.0.1/sensorbucket/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
 
-from openapi_client.configuration import Configuration
-from openapi_client.api_response import ApiResponse
-import openapi_client.models
-from openapi_client import rest
-from openapi_client.exceptions import ApiValueError, ApiException
+from sensorbucket.configuration import Configuration
+from sensorbucket.api_response import ApiResponse
+import sensorbucket.models
+from sensorbucket import rest
+from sensorbucket.exceptions import ApiValueError, ApiException
 
 
 class ApiClient(object):
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -338,15 +338,15 @@
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in data.items()}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
-                klass = getattr(openapi_client.models, klass)
+                klass = getattr(sensorbucket.models, klass)
 
         if klass in self.PRIMITIVE_TYPES:
             return self.__deserialize_primitive(data, klass)
         elif klass == object:
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
```

### Comparing `sensorbucket-1.0.0/openapi_client/api_response.py` & `sensorbucket-1.0.1/sensorbucket/api_response.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/configuration.py` & `sensorbucket-1.0.1/sensorbucket/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 import http.client as httplib
-from openapi_client.exceptions import ApiValueError
+from sensorbucket.exceptions import ApiValueError
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
@@ -62,15 +62,15 @@
         securitySchemes:
           http_basic_auth:
             type: http
             scheme: basic
 
     Configure API client with HTTP basic authentication:
 
-conf = openapi_client.Configuration(
+conf = sensorbucket.Configuration(
     username='the-user',
     password='the-password',
 )
 
     """
 
     _default = None
@@ -121,15 +121,15 @@
         """
         self.access_token = access_token
         """Access token
         """
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("openapi_client")
+        self.logger["package_logger"] = logging.getLogger("sensorbucket")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
```

### Comparing `sensorbucket-1.0.0/openapi_client/exceptions.py` & `sensorbucket-1.0.1/sensorbucket/exceptions.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/__init__.py` & `sensorbucket-1.0.1/sensorbucket/models/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,38 +11,38 @@
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 # import models into model package
-from openapi_client.models.create_device201_response import CreateDevice201Response
-from openapi_client.models.create_device_request import CreateDeviceRequest
-from openapi_client.models.create_device_sensor201_response import CreateDeviceSensor201Response
-from openapi_client.models.create_pipeline200_response import CreatePipeline200Response
-from openapi_client.models.create_pipeline_request import CreatePipelineRequest
-from openapi_client.models.create_sensor_request import CreateSensorRequest
-from openapi_client.models.datastream import Datastream
-from openapi_client.models.delete_device_sensor200_response import DeleteDeviceSensor200Response
-from openapi_client.models.device import Device
-from openapi_client.models.disable_pipeline200_response import DisablePipeline200Response
-from openapi_client.models.get_device200_response import GetDevice200Response
-from openapi_client.models.get_pipeline200_response import GetPipeline200Response
-from openapi_client.models.list_datastreams200_response import ListDatastreams200Response
-from openapi_client.models.list_datastreams200_response_all_of import ListDatastreams200ResponseAllOf
-from openapi_client.models.list_device_sensors200_response import ListDeviceSensors200Response
-from openapi_client.models.list_device_sensors200_response_all_of import ListDeviceSensors200ResponseAllOf
-from openapi_client.models.list_devices200_response import ListDevices200Response
-from openapi_client.models.list_devices200_response_all_of import ListDevices200ResponseAllOf
-from openapi_client.models.list_pipelines200_response import ListPipelines200Response
-from openapi_client.models.list_pipelines200_response_all_of import ListPipelines200ResponseAllOf
-from openapi_client.models.measurement import Measurement
-from openapi_client.models.paginated_response import PaginatedResponse
-from openapi_client.models.paginated_response_links import PaginatedResponseLinks
-from openapi_client.models.pipeline import Pipeline
-from openapi_client.models.query_measurements200_response import QueryMeasurements200Response
-from openapi_client.models.query_measurements200_response_all_of import QueryMeasurements200ResponseAllOf
-from openapi_client.models.sensor import Sensor
-from openapi_client.models.update_device200_response import UpdateDevice200Response
-from openapi_client.models.update_device_request import UpdateDeviceRequest
-from openapi_client.models.update_pipeline200_response import UpdatePipeline200Response
-from openapi_client.models.update_pipeline_request import UpdatePipelineRequest
+from sensorbucket.models.create_device201_response import CreateDevice201Response
+from sensorbucket.models.create_device_request import CreateDeviceRequest
+from sensorbucket.models.create_device_sensor201_response import CreateDeviceSensor201Response
+from sensorbucket.models.create_pipeline200_response import CreatePipeline200Response
+from sensorbucket.models.create_pipeline_request import CreatePipelineRequest
+from sensorbucket.models.create_sensor_request import CreateSensorRequest
+from sensorbucket.models.datastream import Datastream
+from sensorbucket.models.delete_device_sensor200_response import DeleteDeviceSensor200Response
+from sensorbucket.models.device import Device
+from sensorbucket.models.disable_pipeline200_response import DisablePipeline200Response
+from sensorbucket.models.get_device200_response import GetDevice200Response
+from sensorbucket.models.get_pipeline200_response import GetPipeline200Response
+from sensorbucket.models.list_datastreams200_response import ListDatastreams200Response
+from sensorbucket.models.list_datastreams200_response_all_of import ListDatastreams200ResponseAllOf
+from sensorbucket.models.list_device_sensors200_response import ListDeviceSensors200Response
+from sensorbucket.models.list_device_sensors200_response_all_of import ListDeviceSensors200ResponseAllOf
+from sensorbucket.models.list_devices200_response import ListDevices200Response
+from sensorbucket.models.list_devices200_response_all_of import ListDevices200ResponseAllOf
+from sensorbucket.models.list_pipelines200_response import ListPipelines200Response
+from sensorbucket.models.list_pipelines200_response_all_of import ListPipelines200ResponseAllOf
+from sensorbucket.models.measurement import Measurement
+from sensorbucket.models.paginated_response import PaginatedResponse
+from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
+from sensorbucket.models.pipeline import Pipeline
+from sensorbucket.models.query_measurements200_response import QueryMeasurements200Response
+from sensorbucket.models.query_measurements200_response_all_of import QueryMeasurements200ResponseAllOf
+from sensorbucket.models.sensor import Sensor
+from sensorbucket.models.update_device200_response import UpdateDevice200Response
+from sensorbucket.models.update_device_request import UpdateDeviceRequest
+from sensorbucket.models.update_pipeline200_response import UpdatePipeline200Response
+from sensorbucket.models.update_pipeline_request import UpdatePipelineRequest
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/create_device201_response.py` & `sensorbucket-1.0.1/sensorbucket/models/create_device201_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.device import Device
+from sensorbucket.models.device import Device
 
 class CreateDevice201Response(BaseModel):
     """
     CreateDevice201Response
     """
     message: Optional[StrictStr] = None
     data: Optional[Device] = None
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/create_device_request.py` & `sensorbucket-1.0.1/sensorbucket/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/create_device_sensor201_response.py` & `sensorbucket-1.0.1/sensorbucket/models/create_device_sensor201_response.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/create_pipeline200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/update_pipeline200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.pipeline import Pipeline
+from sensorbucket.models.pipeline import Pipeline
 
-class CreatePipeline200Response(BaseModel):
+class UpdatePipeline200Response(BaseModel):
     """
-    CreatePipeline200Response
+    UpdatePipeline200Response
     """
     message: Optional[StrictStr] = None
     data: Optional[Pipeline] = None
     __properties = ["message", "data"]
 
     class Config:
         """Pydantic configuration"""
@@ -41,37 +41,37 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CreatePipeline200Response:
-        """Create an instance of CreatePipeline200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdatePipeline200Response:
+        """Create an instance of UpdatePipeline200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CreatePipeline200Response:
-        """Create an instance of CreatePipeline200Response from a dict"""
+    def from_dict(cls, obj: dict) -> UpdatePipeline200Response:
+        """Create an instance of UpdatePipeline200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CreatePipeline200Response.parse_obj(obj)
+            return UpdatePipeline200Response.parse_obj(obj)
 
-        _obj = CreatePipeline200Response.parse_obj({
+        _obj = UpdatePipeline200Response.parse_obj({
             "message": obj.get("message"),
             "data": Pipeline.from_dict(obj.get("data")) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/create_pipeline_request.py` & `sensorbucket-1.0.1/sensorbucket/models/create_pipeline_request.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/create_sensor_request.py` & `sensorbucket-1.0.1/sensorbucket/models/create_sensor_request.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/datastream.py` & `sensorbucket-1.0.1/sensorbucket/models/datastream.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/delete_device_sensor200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/delete_device_sensor200_response.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/device.py` & `sensorbucket-1.0.1/sensorbucket/models/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional, Union
 from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr, conlist
-from openapi_client.models.sensor import Sensor
+from sensorbucket.models.sensor import Sensor
 
 class Device(BaseModel):
     """
     Device
     """
     id: Optional[Union[StrictFloat, StrictInt]] = None
     code: Optional[StrictStr] = None
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/disable_pipeline200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/disable_pipeline200_response.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/get_device200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/get_device200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.device import Device
+from sensorbucket.models.device import Device
 
 class GetDevice200Response(BaseModel):
     """
     GetDevice200Response
     """
     message: Optional[StrictStr] = None
     data: Optional[Device] = None
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/get_pipeline200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/get_pipeline200_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.pipeline import Pipeline
+from sensorbucket.models.pipeline import Pipeline
 
 class GetPipeline200Response(BaseModel):
     """
     GetPipeline200Response
     """
     message: Optional[StrictStr] = None
     data: Optional[Pipeline] = None
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/list_datastreams200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/list_datastreams200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field, StrictInt, conlist
-from openapi_client.models.datastream import Datastream
-from openapi_client.models.paginated_response_links import PaginatedResponseLinks
+from sensorbucket.models.datastream import Datastream
+from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
 
 class ListDatastreams200Response(BaseModel):
     """
     ListDatastreams200Response
     """
     links: PaginatedResponseLinks = Field(...)
     page_size: StrictInt = Field(...)
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/list_datastreams200_response_all_of.py` & `sensorbucket-1.0.1/sensorbucket/models/list_datastreams200_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from openapi_client.models.datastream import Datastream
+from sensorbucket.models.datastream import Datastream
 
 class ListDatastreams200ResponseAllOf(BaseModel):
     """
     ListDatastreams200ResponseAllOf
     """
     data: Optional[conlist(Datastream)] = None
     __properties = ["data"]
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/list_device_sensors200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/list_device_sensors200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field, StrictInt, conlist
-from openapi_client.models.paginated_response_links import PaginatedResponseLinks
-from openapi_client.models.sensor import Sensor
+from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
+from sensorbucket.models.sensor import Sensor
 
 class ListDeviceSensors200Response(BaseModel):
     """
     ListDeviceSensors200Response
     """
     links: PaginatedResponseLinks = Field(...)
     page_size: StrictInt = Field(...)
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/list_device_sensors200_response_all_of.py` & `sensorbucket-1.0.1/sensorbucket/models/list_device_sensors200_response_all_of.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from openapi_client.models.sensor import Sensor
+from sensorbucket.models.sensor import Sensor
 
 class ListDeviceSensors200ResponseAllOf(BaseModel):
     """
     ListDeviceSensors200ResponseAllOf
     """
     data: Optional[conlist(Sensor)] = None
     __properties = ["data"]
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/list_devices200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/list_devices200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field, StrictInt, conlist
-from openapi_client.models.device import Device
-from openapi_client.models.paginated_response_links import PaginatedResponseLinks
+from sensorbucket.models.device import Device
+from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
 
 class ListDevices200Response(BaseModel):
     """
     ListDevices200Response
     """
     links: PaginatedResponseLinks = Field(...)
     page_size: StrictInt = Field(...)
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/list_devices200_response_all_of.py` & `sensorbucket-1.0.1/sensorbucket/models/list_devices200_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from openapi_client.models.device import Device
+from sensorbucket.models.device import Device
 
 class ListDevices200ResponseAllOf(BaseModel):
     """
     ListDevices200ResponseAllOf
     """
     data: Optional[conlist(Device)] = None
     __properties = ["data"]
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/list_pipelines200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/list_pipelines200_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field, StrictInt, conlist
-from openapi_client.models.paginated_response_links import PaginatedResponseLinks
-from openapi_client.models.pipeline import Pipeline
+from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
+from sensorbucket.models.pipeline import Pipeline
 
 class ListPipelines200Response(BaseModel):
     """
     ListPipelines200Response
     """
     links: PaginatedResponseLinks = Field(...)
     page_size: StrictInt = Field(...)
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/list_pipelines200_response_all_of.py` & `sensorbucket-1.0.1/sensorbucket/models/list_pipelines200_response_all_of.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from openapi_client.models.pipeline import Pipeline
+from sensorbucket.models.pipeline import Pipeline
 
 class ListPipelines200ResponseAllOf(BaseModel):
     """
     ListPipelines200ResponseAllOf
     """
     data: Optional[conlist(Pipeline)] = None
     __properties = ["data"]
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/measurement.py` & `sensorbucket-1.0.1/sensorbucket/models/measurement.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/paginated_response.py` & `sensorbucket-1.0.1/sensorbucket/models/paginated_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, List
 from pydantic import BaseModel, Field, StrictInt, conlist
-from openapi_client.models.paginated_response_links import PaginatedResponseLinks
+from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
 
 class PaginatedResponse(BaseModel):
     """
     PaginatedResponse
     """
     links: PaginatedResponseLinks = Field(...)
     page_size: StrictInt = Field(...)
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/paginated_response_links.py` & `sensorbucket-1.0.1/sensorbucket/models/paginated_response_links.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/pipeline.py` & `sensorbucket-1.0.1/sensorbucket/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/query_measurements200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/query_measurements200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
 from pydantic import BaseModel, Field, StrictInt, conlist
-from openapi_client.models.measurement import Measurement
-from openapi_client.models.paginated_response_links import PaginatedResponseLinks
+from sensorbucket.models.measurement import Measurement
+from sensorbucket.models.paginated_response_links import PaginatedResponseLinks
 
 class QueryMeasurements200Response(BaseModel):
     """
     QueryMeasurements200Response
     """
     links: PaginatedResponseLinks = Field(...)
     page_size: StrictInt = Field(...)
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/query_measurements200_response_all_of.py` & `sensorbucket-1.0.1/sensorbucket/models/query_measurements200_response_all_of.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from openapi_client.models.measurement import Measurement
+from sensorbucket.models.measurement import Measurement
 
 class QueryMeasurements200ResponseAllOf(BaseModel):
     """
     QueryMeasurements200ResponseAllOf
     """
     data: Optional[conlist(Measurement)] = None
     __properties = ["data"]
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/sensor.py` & `sensorbucket-1.0.1/sensorbucket/models/sensor.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/update_device200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/update_device200_response.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/update_device_request.py` & `sensorbucket-1.0.1/sensorbucket/models/update_device_request.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/models/update_pipeline200_response.py` & `sensorbucket-1.0.1/sensorbucket/models/create_pipeline200_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, StrictStr
-from openapi_client.models.pipeline import Pipeline
+from sensorbucket.models.pipeline import Pipeline
 
-class UpdatePipeline200Response(BaseModel):
+class CreatePipeline200Response(BaseModel):
     """
-    UpdatePipeline200Response
+    CreatePipeline200Response
     """
     message: Optional[StrictStr] = None
     data: Optional[Pipeline] = None
     __properties = ["message", "data"]
 
     class Config:
         """Pydantic configuration"""
@@ -41,37 +41,37 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdatePipeline200Response:
-        """Create an instance of UpdatePipeline200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> CreatePipeline200Response:
+        """Create an instance of CreatePipeline200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdatePipeline200Response:
-        """Create an instance of UpdatePipeline200Response from a dict"""
+    def from_dict(cls, obj: dict) -> CreatePipeline200Response:
+        """Create an instance of CreatePipeline200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return UpdatePipeline200Response.parse_obj(obj)
+            return CreatePipeline200Response.parse_obj(obj)
 
-        _obj = UpdatePipeline200Response.parse_obj({
+        _obj = CreatePipeline200Response.parse_obj({
             "message": obj.get("message"),
             "data": Pipeline.from_dict(obj.get("data")) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `sensorbucket-1.0.0/openapi_client/models/update_pipeline_request.py` & `sensorbucket-1.0.1/sensorbucket/models/update_pipeline_request.py`

 * *Files identical despite different names*

### Comparing `sensorbucket-1.0.0/openapi_client/rest.py` & `sensorbucket-1.0.1/sensorbucket/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import logging
 import re
 import ssl
 
 from urllib.parse import urlencode, quote_plus
 import urllib3
 
-from openapi_client.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from sensorbucket.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `sensorbucket-1.0.0/sensorbucket.egg-info/PKG-INFO` & `sensorbucket-1.0.1/sensorbucket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sensorbucket
-Version: 1.0.0
-Summary: Sensorbucket client
+Version: 1.0.1
+Summary: Sensorbucket API
 Home-page: https://sensorbucket.nl
 Author: Tim van Osch
 Author-email: info@pollex.nl
 License: EUPLv1.2
 Keywords: OpenAPI,OpenAPI-Generator,Sensorbucket API
 Description-Content-Type: text/markdown
```

### Comparing `sensorbucket-1.0.0/setup.py` & `sensorbucket-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "sensorbucket"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
-    description="Sensorbucket client",
+    description="Sensorbucket API",
     author="Tim van Osch",
     author_email="info@pollex.nl",
     url="https://sensorbucket.nl",
     keywords=["OpenAPI", "OpenAPI-Generator", "Sensorbucket API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
```

