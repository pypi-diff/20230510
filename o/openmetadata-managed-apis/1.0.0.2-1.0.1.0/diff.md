# Comparing `tmp/openmetadata_managed_apis-1.0.0.2.tar.gz` & `tmp/openmetadata_managed_apis-1.0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata_managed_apis-1.0.0.2.tar", last modified: Thu May  4 11:49:25 2023, max compression
+gzip compressed data, was "openmetadata_managed_apis-1.0.1.0.tar", last modified: Wed May 10 09:08:14 2023, max compression
```

## Comparing `openmetadata_managed_apis-1.0.0.2.tar` & `openmetadata_managed_apis-1.0.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.400460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.400460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/apis_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.400460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/run_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/kill_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/resources/dag_runner.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/views/rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.400460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/views/templates/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/views/templates/rest_api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/data_insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/workflow_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:49:25.400460 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-04 11:49:21.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-04 11:49:21.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:49:21.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 11:49:21.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:49:07.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-04 11:49:21.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 11:49:21.000000 openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:49:25.404460 openmetadata_managed_apis-1.0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-04 11:47:50.000000 openmetadata_managed_apis-1.0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.468609 openmetadata_managed_apis-1.0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-10 09:08:14.468609 openmetadata_managed_apis-1.0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.460609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.460609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/apis_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.464609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/run_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.464609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/kill_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.464609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/resources/dag_runner.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.464609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.464609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/views/rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.460609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.464609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/views/templates/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/views/templates/rest_api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.464609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.468609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/data_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/workflow_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:08:14.460609 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-10 09:08:10.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-10 09:08:10.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:08:10.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-10 09:08:10.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:07:55.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-10 09:08:10.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 09:08:10.000000 openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:08:14.468609 openmetadata_managed_apis-1.0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-10 09:06:39.000000 openmetadata_managed_apis-1.0.1.0/setup.py
```

### Comparing `openmetadata_managed_apis-1.0.0.2/PKG-INFO` & `openmetadata_managed_apis-1.0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata_managed_apis
-Version: 1.0.0.2
+Version: 1.0.1.0
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.0.0.2/README.md` & `openmetadata_managed_apis-1.0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/__init__.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/apis_metadata.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/apis_metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/app.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/app.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/config.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/error_handlers.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/error_handlers.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/response.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/response.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/delete.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/deploy.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/disable.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/disable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/enable.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/enable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/health.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/health.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/ip.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/ip.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/kill.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/kill.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/last_dag_logs.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/run_automation.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/status.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,32 +5,24 @@
 #  http://www.apache.org/licenses/LICENSE-2.0
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """
-Test the connection against a source system
+Return a list of the 10 last status for the ingestion Pipeline
 """
 import traceback
 from typing import Callable
 
-from flask import Blueprint, Response, request
+from flask import Blueprint, Response
 from openmetadata_managed_apis.api.response import ApiResponse
+from openmetadata_managed_apis.api.utils import get_arg_dag_id, get_arg_only_queued
+from openmetadata_managed_apis.operations.status import status
 from openmetadata_managed_apis.utils.logger import routes_logger
-from openmetadata_managed_apis.workflows.ingestion.credentials_builder import (
-    build_secrets_manager_credentials,
-)
-from pydantic import ValidationError
-
-from metadata.automations.runner import execute
-from metadata.generated.schema.entity.automations.workflow import (
-    Workflow as AutomationWorkflow,
-)
-from metadata.utils.secrets.secrets_manager_factory import SecretsManagerFactory
 
 logger = routes_logger()
 
 
 def get_fn(blueprint: Blueprint) -> Callable:
     """
     Return the function loaded to a route
@@ -40,51 +32,28 @@
 
     # Lazy import the requirements
     # pylint: disable=import-outside-toplevel
     from airflow.api_connexion import security
     from airflow.security import permissions
     from airflow.www.app import csrf
 
-    @blueprint.route("/run_automation", methods=["POST"])
+    @blueprint.route("/status", methods=["GET"])
     @csrf.exempt
     @security.requires_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_DAG)])
-    def run_automation() -> Response:
+    def dag_status() -> Response:
         """
-        Given a WorkflowSource Schema, create the engine
-        and test the connection
+        Check the status of a DAG runs
         """
-
-        json_request = request.get_json(cache=False)
-
+        dag_id = get_arg_dag_id()
+        only_queued = get_arg_only_queued()
         try:
-            # TODO: Prepare `parse_automation_workflow_gracefully`
-            automation_workflow: AutomationWorkflow = AutomationWorkflow.parse_obj(
-                json_request
-            )
-
-            execute(automation_workflow)
-
-            return ApiResponse.success(
-                {
-                    "message": f"Workflow [{automation_workflow.name}] has been triggered."
-                }
-            )
-
-        except ValidationError as err:
-            msg = f"Request Validation Error parsing payload: {err}"
-            logger.debug(traceback.format_exc())
-            logger.error(msg)
-            return ApiResponse.error(
-                status=ApiResponse.STATUS_BAD_REQUEST,
-                error=msg,
-            )
+            return status(dag_id, only_queued)
 
         except Exception as exc:
-            msg = f"Error running automation workflow due to [{exc}] "
             logger.debug(traceback.format_exc())
-            logger.error(msg)
+            logger.error(f"Failed to get dag [{dag_id}] status: {exc}")
             return ApiResponse.error(
                 status=ApiResponse.STATUS_SERVER_ERROR,
-                error=msg,
+                error=f"Failed to get status for [{dag_id}] due to [{exc}] ",
             )
 
-    return run_automation
+    return dag_status
```

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/status.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/routes/trigger.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 #  http://www.apache.org/licenses/LICENSE-2.0
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """
-Return a list of the 10 last status for the ingestion Pipeline
+Trigger endpoint
 """
 import traceback
 from typing import Callable
 
-from flask import Blueprint, Response
+from flask import Blueprint, Response, request
 from openmetadata_managed_apis.api.response import ApiResponse
-from openmetadata_managed_apis.api.utils import get_arg_dag_id, get_arg_only_queued
-from openmetadata_managed_apis.operations.status import status
+from openmetadata_managed_apis.api.utils import get_request_arg, get_request_dag_id
+from openmetadata_managed_apis.operations.trigger import trigger
 from openmetadata_managed_apis.utils.logger import routes_logger
 
 logger = routes_logger()
 
 
 def get_fn(blueprint: Blueprint) -> Callable:
     """
@@ -32,28 +32,31 @@
 
     # Lazy import the requirements
     # pylint: disable=import-outside-toplevel
     from airflow.api_connexion import security
     from airflow.security import permissions
     from airflow.www.app import csrf
 
-    @blueprint.route("/status", methods=["GET"])
+    @blueprint.route("/trigger", methods=["POST"])
     @csrf.exempt
-    @security.requires_access([(permissions.ACTION_CAN_READ, permissions.RESOURCE_DAG)])
-    def dag_status() -> Response:
+    @security.requires_access([(permissions.ACTION_CAN_EDIT, permissions.RESOURCE_DAG)])
+    def trigger_dag() -> Response:
         """
-        Check the status of a DAG runs
+        Trigger a dag run
         """
-        dag_id = get_arg_dag_id()
-        only_queued = get_arg_only_queued()
+        dag_id = get_request_dag_id()
+
         try:
-            return status(dag_id, only_queued)
+            run_id = get_request_arg(request, "run_id", raise_missing=False)
+            response = trigger(dag_id, run_id)
+
+            return response
 
         except Exception as exc:
             logger.debug(traceback.format_exc())
-            logger.error(f"Failed to get dag [{dag_id}] status: {exc}")
+            logger.error(f"Failed to trigger dag [{dag_id}]: {exc}")
             return ApiResponse.error(
                 status=ApiResponse.STATUS_SERVER_ERROR,
-                error=f"Failed to get status for [{dag_id}] due to [{exc}] ",
+                error=f"Workflow [{dag_id}] has filed to trigger due to [{exc}] ",
             )
 
-    return dag_status
+    return trigger_dag
```

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/routes/trigger.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/delete.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,58 +5,61 @@
 #  http://www.apache.org/licenses/LICENSE-2.0
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """
-Trigger endpoint
+Module containing the logic to delete a DAG
 """
-import traceback
-from typing import Callable
+import os
+from pathlib import Path
 
-from flask import Blueprint, Response, request
+from airflow import settings
+from airflow.models import DagModel, DagRun
+from flask import Response
+from openmetadata_managed_apis.api.config import (
+    AIRFLOW_DAGS_FOLDER,
+    DAG_GENERATED_CONFIGS,
+)
 from openmetadata_managed_apis.api.response import ApiResponse
-from openmetadata_managed_apis.api.utils import get_request_arg, get_request_dag_id
-from openmetadata_managed_apis.operations.trigger import trigger
-from openmetadata_managed_apis.utils.logger import routes_logger
 
-logger = routes_logger()
 
-
-def get_fn(blueprint: Blueprint) -> Callable:
+def delete_dag_id(dag_id: str) -> Response:
     """
-    Return the function loaded to a route
-    :param blueprint: Flask Blueprint to assign route to
-    :return: routed function
+    Delete a DAG dag_id from the filesystem and airflow db.
+    We clean:
+    - py file in AIRFLOW_DAGS_FOLDER
+    - config file in DAG_GENERATED_CONFIGS
+    - DagModel and DagRun entries in airflow db
+    :param dag_id: DAG to delete
+    :return: API Response
     """
 
-    # Lazy import the requirements
-    # pylint: disable=import-outside-toplevel
-    from airflow.api_connexion import security
-    from airflow.security import permissions
-    from airflow.www.app import csrf
-
-    @blueprint.route("/trigger", methods=["POST"])
-    @csrf.exempt
-    @security.requires_access([(permissions.ACTION_CAN_EDIT, permissions.RESOURCE_DAG)])
-    def trigger_dag() -> Response:
-        """
-        Trigger a dag run
-        """
-        dag_id = get_request_dag_id()
-
-        try:
-            run_id = get_request_arg(request, "run_id", raise_missing=False)
-            response = trigger(dag_id, run_id)
-
-            return response
-
-        except Exception as exc:
-            logger.debug(traceback.format_exc())
-            logger.error(f"Failed to trigger dag [{dag_id}]: {exc}")
-            return ApiResponse.error(
-                status=ApiResponse.STATUS_SERVER_ERROR,
-                error=f"Workflow [{dag_id}] has filed to trigger due to [{exc}] ",
-            )
+    dag_py_file = Path(AIRFLOW_DAGS_FOLDER) / f"{dag_id}.py"
+    config_file = Path(DAG_GENERATED_CONFIGS) / f"{dag_id}.json"
 
-    return trigger_dag
+    deleted_file = False
+    if dag_py_file.is_file():
+        deleted_file = True
+        os.remove(dag_py_file.absolute())
+
+    deleted_config = False
+    if config_file.is_file():
+        deleted_config = True
+        os.remove(config_file.absolute())
+
+    with settings.Session() as session:
+        deleted_dags = (
+            session.query(DagModel).filter(DagModel.dag_id == dag_id).delete()
+        )
+        session.query(DagRun).filter(DagRun.dag_id == dag_id).delete()
+        session.commit()
+
+    if deleted_dags > 0 and deleted_file and deleted_config:
+        return ApiResponse.success({"message": f"DAG [{dag_id}] has been deleted"})
+
+    return ApiResponse.error(
+        status=ApiResponse.STATUS_SERVER_ERROR,
+        error=f"Could not find and delete {dag_id}. Deleted dags: {deleted_dags}; "
+        + f"deleted {dag_py_file}: {deleted_file}",
+    )
```

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/api/utils.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/api/utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/deploy.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/kill_all.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/kill_all.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/last_dag_logs.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/state.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/state.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/status.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/operations/trigger.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/operations/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/plugin.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/plugin.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/utils/logger.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/utils/parser.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/utils/parser.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/views/rest_api.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/views/rest_api.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/views/templates/rest_api/index.html` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/views/templates/rest_api/index.html`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/config.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/common.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,14 @@
     ParsingConfigurationError,
 )
 from metadata.ingestion.api.workflow import Workflow
 from metadata.ingestion.ometa.utils import model_str
 
 logger = workflow_logger()
 
-# logging.getLogger("airflow.task.operators").setLevel(logging.WARNING)
-
 
 class InvalidServiceException(Exception):
     """
     The service type we received is not supported
     """
 
 
@@ -251,15 +249,17 @@
     """
     Prepare kwargs to send to DAG
     :param ingestion_pipeline: pipeline configs
     :return: dict to use as kwargs
     """
     return {
         "dag_id": clean_dag_id(ingestion_pipeline.name.__root__),
-        "description": ingestion_pipeline.description,
+        "description": ingestion_pipeline.description.__root__
+        if ingestion_pipeline.description is not None
+        else None,
         "start_date": ingestion_pipeline.airflowConfig.startDate.__root__
         if ingestion_pipeline.airflowConfig.startDate
         else airflow.utils.dates.days_ago(1),
         "end_date": ingestion_pipeline.airflowConfig.endDate.__root__
         if ingestion_pipeline.airflowConfig.endDate
         else None,
         "concurrency": ingestion_pipeline.airflowConfig.concurrency,
```

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,17 @@
     SecretsManagerProvider,
 )
 from metadata.ingestion.models.custom_pydantic import CustomSecretStr
 from metadata.utils.secrets.secrets_manager import SECRET_MANAGER_AIRFLOW_CONF
 
 
 def build_aws_credentials() -> Optional[AWSCredentials]:
-    if conf.has_section(SECRET_MANAGER_AIRFLOW_CONF):
-        credentials = AWSCredentials(
-            awsRegion=conf.get(SECRET_MANAGER_AIRFLOW_CONF, "aws_region", fallback="")
-        )
+    aws_region = conf.get(SECRET_MANAGER_AIRFLOW_CONF, "aws_region", fallback=None)
+    if aws_region:
+        credentials = AWSCredentials(awsRegion=aws_region)
         credentials.awsAccessKeyId = conf.get(
             SECRET_MANAGER_AIRFLOW_CONF, "aws_access_key_id", fallback=""
         )
         credentials.awsSecretAccessKey = CustomSecretStr(
             conf.get(SECRET_MANAGER_AIRFLOW_CONF, "aws_secret_access_key", fallback="")
         )
         return credentials
```

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/data_insight.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/data_insight.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/dbt.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/dbt.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/es_reindex.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/lineage.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/lineage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/metadata.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/profiler.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/profiler.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/registry.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/registry.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/test_suite.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/test_suite.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/ingestion/usage.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/ingestion/usage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/workflow_builder.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/workflow_builder.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis/workflows/workflow_factory.py` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis/workflows/workflow_factory.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/PKG-INFO` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata-managed-apis
-Version: 1.0.0.2
+Version: 1.0.1.0
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.0.0.2/openmetadata_managed_apis.egg-info/SOURCES.txt` & `openmetadata_managed_apis-1.0.1.0/openmetadata_managed_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.0.2/setup.py` & `openmetadata_managed_apis-1.0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 }
 
 setup(
     name=PLUGIN_NAME,
     packages=find_packages(include=[f"{PLUGIN_NAME}.*", PLUGIN_NAME]),
     include_package_data=True,
     package_data={PLUGIN_NAME: get_package_data()},
-    version="1.0.0.2",
+    version="1.0.1.0",
     url="https://open-metadata.org/",
     author="OpenMetadata Committers",
     license="Apache License 2.0",
     description="Airflow REST APIs to create and manage DAGS",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     entry_points={
```

