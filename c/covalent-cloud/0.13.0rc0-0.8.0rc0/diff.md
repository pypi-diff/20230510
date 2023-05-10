# Comparing `tmp/covalent-cloud-0.13.0rc0.tar.gz` & `tmp/covalent-cloud-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-cloud-0.13.0rc0.tar", last modified: Tue May  9 21:11:48 2023, max compression
+gzip compressed data, was "covalent-cloud-0.8.0rc0.tar", last modified: Sat Apr 29 00:10:27 2023, max compression
```

## Comparing `covalent-cloud-0.13.0rc0.tar` & `covalent-cloud-0.8.0rc0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.099182 covalent-cloud-0.13.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-09 21:11:48.095182 covalent-cloud-0.13.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.083182 covalent-cloud-0.13.0rc0/covalent_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.087182 covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/electron.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/transport_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.087182 covalent-cloud-0.13.0rc0/covalent_cloud/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.087182 covalent-cloud-0.13.0rc0/covalent_cloud/cloud_executor/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/cloud_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/cloud_executor/cloud_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.087182 covalent-cloud-0.13.0rc0/covalent_cloud/cloud_executor/models/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/cloud_executor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/cloud_executor/models/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/cloud_executor/models/sw_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.091182 covalent-cloud-0.13.0rc0/covalent_cloud/dispatch_management/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/dispatch_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/dispatch_management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/dispatch_management/interface_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/dispatch_management/results_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.091182 covalent-cloud-0.13.0rc0/covalent_cloud/service_account_interface/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/service_account_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/service_account_interface/auth_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/service_account_interface/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.091182 covalent-cloud-0.13.0rc0/covalent_cloud/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.091182 covalent-cloud-0.13.0rc0/covalent_cloud/shared/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/classes/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/classes/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.095182 covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/electron.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/result.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/transport_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.095182 covalent-cloud-0.13.0rc0/covalent_cloud/software_environment/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/software_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.095182 covalent-cloud-0.13.0rc0/covalent_cloud/swe_management/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/swe_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/covalent_cloud/swe_management/swe_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.087182 covalent-cloud-0.13.0rc0/covalent_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-09 21:11:47.000000 covalent-cloud-0.13.0rc0/covalent_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-09 21:11:47.000000 covalent-cloud-0.13.0rc0/covalent_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:11:47.000000 covalent-cloud-0.13.0rc0/covalent_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 21:11:47.000000 covalent-cloud-0.13.0rc0/covalent_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 21:11:47.000000 covalent-cloud-0.13.0rc0/covalent_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 21:11:48.099182 covalent-cloud-0.13.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.083182 covalent-cloud-0.13.0rc0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.095182 covalent-cloud-0.13.0rc0/tests/dispatch_management_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/dispatch_management_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/dispatch_management_tests/future_classes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/dispatch_management_tests/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/dispatch_management_tests/interface_functions_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.095182 covalent-cloud-0.13.0rc0/tests/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.095182 covalent-cloud-0.13.0rc0/tests/shared/classes/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/shared/classes/APIClient_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/shared/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:11:48.095182 covalent-cloud-0.13.0rc0/tests/swe_management_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/swe_management_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-09 21:11:38.000000 covalent-cloud-0.13.0rc0/tests/swe_management_tests/swe_manager_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/cloud_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/sw_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/interface_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/results_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/auth_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/software_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/software_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/swe_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/future_classes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/interface_functions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/shared/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/classes/APIClient_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/swe_management_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/swe_management_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/swe_management_tests/swe_manager_test.py
```

### Comparing `covalent-cloud-0.13.0rc0/LICENSE` & `covalent-cloud-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/PKG-INFO` & `covalent-cloud-0.8.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent-cloud
-Version: 0.13.0rc0
+Version: 0.8.0rc0
 Summary: Covalent Cloud SDK
 Home-page: https://github.com/AgnostiqHQ/covalent-cloud-sdk
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-cloud-sdk/archive/v0.13.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent-cloud-sdk/archive/v0.8.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         [![covalent](https://img.shields.io/badge/covalent-0.208.0rc0-purple)](https://github.com/AgnostiqHQ/covalent)
         [![agpl](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0.en.html)
```

### Comparing `covalent-cloud-0.13.0rc0/README.md` & `covalent-cloud-0.8.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/common.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/common.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/electron.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/lattice.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/result.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/result.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/_serialize/transport_graph.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/transport_graph.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/cloud_executor/cloud_executor.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/cloud_executor.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/dispatch_management/helpers.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,26 +255,15 @@
     total = len(assets)
     _upload_futures = []
     for i, asset in enumerate(assets):
         # _upload_asset(asset.uri, asset.remote_uri)
         fut = _dispatch_executor.submit(_upload_asset, asset.uri, asset.remote_uri)
         _upload_futures.append(fut)
         # app_log.debug(f"uploading {i+1} out of {total} assets.")
-    done, incomplete = wait(_upload_futures)
-    if len(done) < total:
-        raise RuntimeError("Failed to upload some assets")
-
-    _exceptions = []
-    for fut in done:
-        ex = fut.exception(timeout=0.1)
-        if ex:
-            _exceptions.append(ex)
-    if len(_exceptions) > 0:
-        print(f"Failed to upload {len(_exceptions)} out of {total} assets", file=sys.stderr)
-        raise RuntimeError(f"Failed to upload {len(_exceptions)} out of {total} assets")
+    wait(_upload_futures)
 
 
 def _upload_asset(local_uri, remote_uri):
     scheme_prefix = "file://"
     if local_uri.startswith(scheme_prefix):
         local_path = local_uri[len(scheme_prefix) :]
     else:
```

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/dispatch_management/interface_functions.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/interface_functions.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/dispatch_management/results_manager.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/results_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/service_account_interface/auth_config_manager.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/auth_config_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/shared/classes/api.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,36 +61,32 @@
         uri = uri_components.url
         options = self.get_request_options(request_options)
         return uri, options
 
     def post(self, endpoint, request_options=None):
         uri, options = self.prepare_request(endpoint, request_options)
         res = requests.post(uri, **options)
-        res.raise_for_status()
 
         return res
 
     def get(self, endpoint, request_options=None):
         uri, options = self.prepare_request(endpoint, request_options)
         res = requests.get(uri, **options)
-        res.raise_for_status()
 
         return res
 
     def delete(self, endpoint, request_options=None):
         uri, options = self.prepare_request(endpoint, request_options)
         res = requests.delete(uri, **options)
-        res.raise_for_status()
 
         return res
 
     def put(self, endpoint, request_options=None):
         uri, options = self.prepare_request(endpoint, request_options)
         res = requests.put(uri, **options)
-        res.raise_for_status()
 
         return res
 
 
 class DispatcherAPI(APIClient):
     def __init__(self, headers={}, settings: Settings = settings) -> None:
         super().__init__(
```

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/shared/classes/settings.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/settings.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/electron.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/lattice.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/shared/schemas/result.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/result.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud/swe_management/swe_manager.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/swe_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,30 +109,28 @@
     with tempfile.NamedTemporaryFile(mode="w", suffix=".yml", delete=False) as definition_file:
 
         yaml.dump(yaml_template, definition_file, default_flow_style=False)
 
         client = get_client()
 
         # Open a separate reader in binary mode per Requests doc
-        try:
-            with open(definition_file.name, "rb") as def_file_reader:
-                response = client.post(
-                    "/api/v2/envs",
-                    {
-                        "files": {"definition": def_file_reader},
-                        "data": {"name": name, "variables": json.dumps(variables)},
-                    },
-                )
-        except requests.exceptions.HTTPError as e:
-            if e.response.status_code == 400:
-                print("Environment Already Exists.")
-                return
-            else:
-                raise
+        with open(definition_file.name, "rb") as def_file_reader:
+            response = client.post(
+                "/api/v2/envs",
+                {
+                    "files": {"definition": def_file_reader},
+                    "data": {"name": name, "variables": json.dumps(variables)},
+                },
+            )
+
+        if response.status_code == 400:
+            print("Environment Already Exists.")
+            return
 
+        response.raise_for_status()
         response_body = response.json()
 
     print(f"Name: {response_body['name']}")
     print(f"Status: {response_body['status']}")
     print(f"Estimated Time: {response_body['estimated_time']}")
 
     print("Environment file contains:")
```

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud.egg-info/PKG-INFO` & `covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent-cloud
-Version: 0.13.0rc0
+Version: 0.8.0rc0
 Summary: Covalent Cloud SDK
 Home-page: https://github.com/AgnostiqHQ/covalent-cloud-sdk
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-cloud-sdk/archive/v0.13.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent-cloud-sdk/archive/v0.8.0.tar.gz
 Description: &nbsp;
         
         <div align="center">
         
         [![covalent](https://img.shields.io/badge/covalent-0.208.0rc0-purple)](https://github.com/AgnostiqHQ/covalent)
         [![agpl](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0.en.html)
```

### Comparing `covalent-cloud-0.13.0rc0/covalent_cloud.egg-info/SOURCES.txt` & `covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/pyproject.toml` & `covalent-cloud-0.8.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/setup.py` & `covalent-cloud-0.8.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/tests/dispatch_management_tests/future_classes_test.py` & `covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/future_classes_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/tests/dispatch_management_tests/helpers_test.py` & `covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/tests/dispatch_management_tests/interface_functions_test.py` & `covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/interface_functions_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/tests/shared/classes/APIClient_test.py` & `covalent-cloud-0.8.0rc0/tests/shared/classes/APIClient_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.13.0rc0/tests/swe_management_tests/swe_manager_test.py` & `covalent-cloud-0.8.0rc0/tests/swe_management_tests/swe_manager_test.py`

 * *Files identical despite different names*

