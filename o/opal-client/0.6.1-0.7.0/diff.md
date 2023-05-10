# Comparing `tmp/opal-client-0.6.1.tar.gz` & `tmp/opal-client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-client-0.6.1.tar", last modified: Mon May  1 17:32:27 2023, max compression
+gzip compressed data, was "opal-client-0.7.0.tar", last modified: Wed May 10 19:01:52 2023, max compression
```

## Comparing `opal-client-0.6.1.tar` & `opal-client-0.7.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.699254 opal-client-0.6.1/
--rw-r--r--   0 roekatz    (501) staff       (20)     8464 2023-05-01 17:32:27.699079 opal-client-0.6.1/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.692278 opal-client-0.6.1/opal_client/
--rw-r--r--   0 roekatz    (501) staff       (20)       31 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.693941 opal-client-0.6.1/opal_client/callbacks/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/callbacks/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3034 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/callbacks/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4329 2023-04-18 15:25:03.000000 opal-client-0.6.1/opal_client/callbacks/register.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2960 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/callbacks/reporter.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2184 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    18495 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    10106 2023-04-20 15:05:49.000000 opal-client-0.6.1/opal_client/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.694868 opal-client-0.6.1/opal_client/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      863 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4286 2022-12-08 13:45:19.000000 opal-client-0.6.1/opal_client/data/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      842 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/data/rpc.py
--rw-r--r--   0 roekatz    (501) staff       (20)    19105 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/data/updater.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2220 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/limiter.py
--rw-r--r--   0 roekatz    (501) staff       (20)       33 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)       96 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.695634 opal-client-0.6.1/opal_client/opa/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/opa/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.695803 opal-client-0.6.1/opal_client/opa/healthcheck/
--rw-r--r--   0 roekatz    (501) staff       (20)     1123 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/opa/healthcheck/opal.rego
--rw-r--r--   0 roekatz    (501) staff       (20)     3047 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/opa/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3144 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/opa/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8116 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/opa/runner.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.696776 opal-client-0.6.1/opal_client/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/policy/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      501 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/policy/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4968 2023-01-19 13:43:15.000000 opal-client-0.6.1/opal_client/policy/fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1797 2023-01-19 13:43:15.000000 opal-client-0.6.1/opal_client/policy/options.py
--rw-r--r--   0 roekatz    (501) staff       (20)      596 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/policy/topics.py
--rw-r--r--   0 roekatz    (501) staff       (20)    13408 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/policy/updater.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.698011 opal-client-0.6.1/opal_client/policy_store/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/policy_store/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1650 2023-03-12 10:36:51.000000 opal-client-0.6.1/opal_client/policy_store/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8421 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/policy_store/base_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2352 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/policy_store/mock_policy_store_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)    32153 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/policy_store/opa_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5401 2023-04-29 17:08:57.000000 opal-client-0.6.1/opal_client/policy_store/policy_store_client_factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1795 2023-03-12 10:36:51.000000 opal-client-0.6.1/opal_client/policy_store/schemas.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.698764 opal-client-0.6.1/opal_client/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7279 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/tests/data_updater_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1960 2023-04-19 08:36:33.000000 opal-client-0.6.1/opal_client/tests/opa_client_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4415 2023-03-27 15:01:56.000000 opal-client-0.6.1/opal_client/tests/server_to_client_intergation_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      322 2022-12-08 13:40:17.000000 opal-client-0.6.1/opal_client/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.693142 opal-client-0.6.1/opal_client.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     8464 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1445 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      417 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-05-01 17:32:27.000000 opal-client-0.6.1/opal_client.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-05-01 17:32:27.699295 opal-client-0.6.1/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2831 2022-12-08 13:40:17.000000 opal-client-0.6.1/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.622918 opal-client-0.7.0/
+-rw-r--r--   0 asafc      (501) staff       (20)     8464 2023-05-10 19:01:52.622656 opal-client-0.7.0/PKG-INFO
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.617684 opal-client-0.7.0/opal_client/
+-rw-r--r--   0 asafc      (501) staff       (20)       31 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.618972 opal-client-0.7.0/opal_client/callbacks/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/callbacks/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3034 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/callbacks/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4329 2022-12-02 16:23:06.000000 opal-client-0.7.0/opal_client/callbacks/register.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2960 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/callbacks/reporter.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2213 2023-05-10 17:44:36.000000 opal-client-0.7.0/opal_client/cli.py
+-rw-r--r--   0 asafc      (501) staff       (20)    19776 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/client.py
+-rw-r--r--   0 asafc      (501) staff       (20)    10945 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.619510 opal-client-0.7.0/opal_client/data/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/data/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      863 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/data/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4286 2022-10-12 14:50:19.000000 opal-client-0.7.0/opal_client/data/fetcher.py
+-rw-r--r--   0 asafc      (501) staff       (20)      842 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/data/rpc.py
+-rw-r--r--   0 asafc      (501) staff       (20)    19105 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/data/updater.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.620090 opal-client-0.7.0/opal_client/engine/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.620200 opal-client-0.7.0/opal_client/engine/healthcheck/
+-rw-r--r--   0 asafc      (501) staff       (20)     1123 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/healthcheck/opal.rego
+-rw-r--r--   0 asafc      (501) staff       (20)     3517 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5702 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/options.py
+-rw-r--r--   0 asafc      (501) staff       (20)    10724 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/engine/runner.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2220 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/limiter.py
+-rw-r--r--   0 asafc      (501) staff       (20)       33 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)       96 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/main.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.621151 opal-client-0.7.0/opal_client/policy/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/policy/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      501 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/policy/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4968 2023-02-01 11:46:28.000000 opal-client-0.7.0/opal_client/policy/fetcher.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1797 2023-02-01 11:46:28.000000 opal-client-0.7.0/opal_client/policy/options.py
+-rw-r--r--   0 asafc      (501) staff       (20)      596 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/policy/topics.py
+-rw-r--r--   0 asafc      (501) staff       (20)    13450 2023-05-10 17:44:36.000000 opal-client-0.7.0/opal_client/policy/updater.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.622068 opal-client-0.7.0/opal_client/policy_store/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/policy_store/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1650 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/policy_store/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8442 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/base_policy_store_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12318 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/cedar_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2352 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/policy_store/mock_policy_store_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)    32177 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/opa_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5741 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/policy_store_client_factory.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1815 2023-05-10 17:44:40.000000 opal-client-0.7.0/opal_client/policy_store/schemas.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.622485 opal-client-0.7.0/opal_client/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7279 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/tests/data_updater_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1960 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/tests/opa_client_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4415 2023-05-10 06:45:11.000000 opal-client-0.7.0/opal_client/tests/server_to_client_intergation_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)      322 2022-10-01 21:13:25.000000 opal-client-0.7.0/opal_client/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.618529 opal-client-0.7.0/opal_client.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)     8464 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1501 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       52 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/entry_points.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      436 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       12 2023-05-10 19:01:52.000000 opal-client-0.7.0/opal_client.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-10 19:01:52.622958 opal-client-0.7.0/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)     2834 2023-05-10 17:44:40.000000 opal-client-0.7.0/setup.py
```

### Comparing `opal-client-0.6.1/PKG-INFO` & `opal-client-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.6.1
+Version: 0.7.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.6.1 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
```

### Comparing `opal-client-0.6.1/opal_client/callbacks/api.py` & `opal-client-0.7.0/opal_client/callbacks/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/callbacks/register.py` & `opal-client-0.7.0/opal_client/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/callbacks/reporter.py` & `opal-client-0.7.0/opal_client/callbacks/reporter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/cli.py` & `opal-client-0.7.0/opal_client/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 root_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), os.path.pardir))
 sys.path.append(root_dir)
 
 from opal_client.config import opal_client_config
 from opal_common.cli.docs import MainTexts
 from opal_common.cli.typer_app import get_typer_app
 from opal_common.config import opal_common_config
-from opal_common.corn_utils import run_gunicorn, run_uvicorn
 
 app = get_typer_app()
 
 
 @app.command()
 def run(engine_type: str = typer.Option("uvicron", help="uvicorn or gunicorn")):
     """Run the client as a daemon."""
     typer.echo(f"-- Starting OPAL client (with {engine_type}) --")
+    from opal_common.corn_utils import run_gunicorn, run_uvicorn
 
     if engine_type == "gunicorn":
         app: FastAPI
         from opal_client.main import app
 
         run_gunicorn(
             app,
@@ -59,13 +59,16 @@
         if ctx.invoked_subcommand is None or ctx.invoked_subcommand == "run":
             typer.secho(main_texts.header, bold=True, fg=typer.colors.MAGENTA)
         if ctx.invoked_subcommand is None:
             typer.echo(ctx.get_usage())
             typer.echo(main_texts.docs)
 
     opal_client_config.cli(
-        [opal_common_config], typer_app=app, help=main_texts.docs, on_start=on_start
+        [opal_common_config],
+        typer_app=app,
+        help=main_texts.docs,
+        on_start=on_start,
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `opal-client-0.6.1/opal_client/client.py` & `opal-client-0.7.0/opal_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import asyncio
 import functools
 import os
 import signal
 import uuid
 from logging import disable
-from typing import List, Optional
+from typing import Awaitable, Callable, List, Literal, Optional, Union
 
 import aiofiles
 import aiofiles.os
 import aiohttp
 import websockets
 from fastapi import FastAPI, status
 from fastapi.responses import JSONResponse
 from opal_client.callbacks.api import init_callbacks_api
 from opal_client.callbacks.register import CallbacksRegister
 from opal_client.config import PolicyStoreTypes, opal_client_config
 from opal_client.data.api import init_data_router
 from opal_client.data.fetcher import DataFetcher
 from opal_client.data.updater import DataUpdater
+from opal_client.engine.options import CedarServerOptions, OpaServerOptions
+from opal_client.engine.runner import CedarRunner, OpaRunner
 from opal_client.limiter import StartupLoadLimiter
-from opal_client.opa.options import OpaServerOptions
-from opal_client.opa.runner import OpaRunner
 from opal_client.policy.api import init_policy_router
 from opal_client.policy.updater import PolicyUpdater
 from opal_client.policy_store.api import init_policy_store_router
 from opal_client.policy_store.base_policy_store_client import BasePolicyStoreClient
 from opal_client.policy_store.policy_store_client_factory import (
     PolicyStoreClientFactory,
 )
@@ -42,14 +42,16 @@
         policy_store_type: PolicyStoreTypes = None,
         policy_store: BasePolicyStoreClient = None,
         data_updater: DataUpdater = None,
         data_topics: List[str] = None,
         policy_updater: PolicyUpdater = None,
         inline_opa_enabled: bool = None,
         inline_opa_options: OpaServerOptions = None,
+        inline_cedar_enabled: bool = None,
+        inline_cedar_options: CedarServerOptions = None,
         verifier: Optional[JWTVerifier] = None,
         store_backup_path: Optional[str] = None,
         store_backup_interval: Optional[int] = None,
         offline_mode_enabled: bool = False,
     ) -> None:
         """
         Args:
@@ -63,16 +65,16 @@
         # defaults
         policy_store_type: PolicyStoreTypes = (
             policy_store_type or opal_client_config.POLICY_STORE_TYPE
         )
         inline_opa_enabled: bool = (
             inline_opa_enabled or opal_client_config.INLINE_OPA_ENABLED
         )
-        inline_opa_options: OpaServerOptions = (
-            inline_opa_options or opal_client_config.INLINE_OPA_CONFIG
+        inline_cedar_enabled: bool = (
+            inline_cedar_enabled or opal_client_config.INLINE_CEDAR_ENABLED
         )
         opal_client_identifier: str = (
             opal_client_config.OPAL_CLIENT_STAT_ID or f"CLIENT_{uuid.uuid4().hex}"
         )
         # set logs
         configure_logs()
 
@@ -136,37 +138,20 @@
                     opal_client_id=opal_client_identifier,
                 )
         else:
             self.data_updater = None
 
         # Internal services
         # Policy store
-        if self.policy_store_type == PolicyStoreTypes.OPA and inline_opa_enabled:
-            rehydration_callbacks = [
-                # refetches policy code (e.g: rego) and static data from server
-                functools.partial(
-                    self.policy_updater.update_policy, force_full_update=True
-                ),
-            ]
-
-            if self.data_updater:
-                rehydration_callbacks.append(
-                    functools.partial(
-                        self.data_updater.get_base_policy_data,
-                        data_fetch_reason="policy store rehydration",
-                    )
-                )
-
-            self.opa_runner = OpaRunner.setup_opa_runner(
-                options=inline_opa_options,
-                piped_logs_format=opal_client_config.INLINE_OPA_LOG_FORMAT,
-                rehydration_callbacks=rehydration_callbacks,
-            )
-        else:
-            self.opa_runner = False
+        self.engine_runner = self._init_engine_runner(
+            inline_opa_enabled,
+            inline_cedar_enabled,
+            inline_opa_options,
+            inline_cedar_options,
+        )
 
         custom_ssl_context = get_custom_ssl_context()
         if (
             opal_common_config.CLIENT_SELF_SIGNED_CERTIFICATES_ALLOWED
             and custom_ssl_context is not None
         ):
             logger.warning(
@@ -193,14 +178,57 @@
             store_backup_interval or opal_client_config.STORE_BACKUP_INTERVAL
         )
         self._backup_loaded = False
 
         # init fastapi app
         self.app: FastAPI = self._init_fast_api_app()
 
+    def _init_engine_runner(
+        self,
+        inline_opa_enabled: bool,
+        inline_cedar_enabled: bool,
+        inline_opa_options: Optional[OpaServerOptions] = None,
+        inline_cedar_options: Optional[CedarServerOptions] = None,
+    ) -> Union[OpaRunner, CedarRunner, Literal[False]]:
+        if inline_opa_enabled and self.policy_store_type == PolicyStoreTypes.OPA:
+            inline_opa_options = (
+                inline_opa_options or opal_client_config.INLINE_OPA_CONFIG
+            )
+            rehydration_callbacks = [
+                # refetches policy code (e.g: rego) and static data from server
+                functools.partial(
+                    self.policy_updater.update_policy, force_full_update=True
+                ),
+            ]
+
+            if self.data_updater:
+                rehydration_callbacks.append(
+                    functools.partial(
+                        self.data_updater.get_base_policy_data,
+                        data_fetch_reason="policy store rehydration",
+                    )
+                )
+
+            return OpaRunner.setup_opa_runner(
+                options=inline_opa_options,
+                piped_logs_format=opal_client_config.INLINE_OPA_LOG_FORMAT,
+                rehydration_callbacks=rehydration_callbacks,
+            )
+
+        elif inline_cedar_enabled and self.policy_store_type == PolicyStoreTypes.CEDAR:
+            inline_cedar_options = (
+                inline_cedar_options or opal_client_config.INLINE_CEDAR_CONFIG
+            )
+            return CedarRunner.setup_cedar_runner(
+                options=inline_cedar_options,
+                piped_logs_format=opal_client_config.INLINE_CEDAR_LOG_FORMAT,
+            )
+
+        return False
+
     def _init_fast_api_app(self):
         """inits the fastapi app object."""
         app = FastAPI(
             title="OPAL Client",
             description="OPAL is an administration layer for Open Policy Agent (OPA), detecting changes"
             + " to both policy and data and pushing live updates to your agents. The opal client is"
             + " deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to"
@@ -282,45 +310,51 @@
             if self.offline_mode_enabled:
                 await self.backup_store()
 
             await self.stop_client_background_tasks()
 
         return app
 
+    async def _run_or_delay_for_engine_runner(
+        self, callback: Callable[[], Awaitable[None]]
+    ):
+        if self.engine_runner:
+            # runs the callback after policy store is up
+            self.engine_runner.register_process_initial_start_callbacks([callback])
+            async with self.engine_runner:
+                await self.engine_runner.wait_until_done()
+            return
+
+        # we do not run the policy store in the same container
+        # therefore we can immediately run the callback
+        await callback()
+
     async def start_client_background_tasks(self):
         """Launch OPAL client long-running tasks:
 
         - Policy Store runner (e.g: Opa Runner)
         - Policy Updater
         - Data Updater
 
         If there is a policy store to run, we wait until its up before launching dependent tasks.
         """
         if self._startup_wait:
             await self._startup_wait()
 
-        if self.opa_runner:
-            # runs the policy store dependent tasks after policy store is up
-            self.opa_runner.register_opa_initial_start_callbacks(
-                [self.launch_policy_store_dependent_tasks]
-            )
-            async with self.opa_runner:
-                await self.opa_runner.wait_until_done()
-        else:
-            # we do not run the policy store in the same container
-            # therefore we can immediately launch dependent tasks
-            await self.launch_policy_store_dependent_tasks()
+        await self._run_or_delay_for_engine_runner(
+            self.launch_policy_store_dependent_tasks
+        )
 
     async def stop_client_background_tasks(self):
         """stops all background tasks (called on shutdown event)"""
         logger.info("stopping background tasks...")
 
         # stopping opa runner
-        if self.opa_runner:
-            await self.opa_runner.stop()
+        if self.engine_runner:
+            await self.engine_runner.stop()
 
         # stopping updater tasks (each updater runs a pub/sub client)
         logger.info("trying to shutdown DataUpdater and PolicyUpdater gracefully...")
         tasks: List[asyncio.Task] = []
         if self.data_updater:
             tasks.append(asyncio.create_task(self.data_updater.stop()))
         if self.policy_updater:
```

### Comparing `opal-client-0.6.1/opal_client/config.py` & `opal-client-0.7.0/opal_client/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from enum import Enum
 
-from opal_client.opa.options import OpaServerOptions
+from opal_client.engine.options import CedarServerOptions, OpaServerOptions
 from opal_client.policy.options import PolicyConnRetryOptions
 from opal_client.policy_store.schemas import PolicyStoreAuth, PolicyStoreTypes
 from opal_common.confi import Confi, confi
 from opal_common.config import opal_common_config
 from opal_common.fetcher.providers.http_fetch_provider import HttpFetcherConfig
 from opal_common.schemas.data import DEFAULT_DATA_TOPIC, UpdateCallback
 
 
 # Opal Client general configuration -------------------------------------------
-class OpaLogFormat(str, Enum):
+class EngineLogFormat(str, Enum):
     NONE = "none"  # no opa logs are piped
     MINIMAL = "minimal"  # only the event name is logged
     HTTP = "http"  # tries to extract http method, path and response status code
     FULL = "full"  # logs the entire data dict returned
 
 
 class OpalClientConfig(Confi):
@@ -92,16 +92,34 @@
     INLINE_OPA_CONFIG = confi.model(
         "INLINE_OPA_CONFIG",
         OpaServerOptions,
         {},  # defaults are being set according to OpaServerOptions pydantic definitions (see class)
         description="cli options used when running `opa run --server` inline",
     )
 
-    INLINE_OPA_LOG_FORMAT: OpaLogFormat = confi.enum(
-        "INLINE_OPA_LOG_FORMAT", OpaLogFormat, OpaLogFormat.NONE
+    INLINE_OPA_LOG_FORMAT: EngineLogFormat = confi.enum(
+        "INLINE_OPA_LOG_FORMAT", EngineLogFormat, EngineLogFormat.NONE
+    )
+
+    # Cedar runner configuration (Cedar-engine can optionally be run by OPAL) ----------------
+
+    # whether or not OPAL should run the Cedar agent by itself in the same container
+    INLINE_CEDAR_ENABLED = confi.bool("INLINE_CEDAR_ENABLED", True)
+
+    # if inline Cedar is indeed enabled, user can pass cli options
+    # (configuration) that affects how the agent will run
+    INLINE_CEDAR_CONFIG = confi.model(
+        "INLINE_CEDAR_CONFIG",
+        CedarServerOptions,
+        {},  # defaults are being set according to CedarServerOptions pydantic definitions (see class)
+        description="cli options used when running the Cedar agent inline",
+    )
+
+    INLINE_CEDAR_LOG_FORMAT: EngineLogFormat = confi.enum(
+        "INLINE_CEDAR_LOG_FORMAT", EngineLogFormat, EngineLogFormat.NONE
     )
 
     # configuration for fastapi routes
     ALLOWED_ORIGINS = ["*"]
 
     # general configuration for pub/sub clients
     KEEP_ALIVE_INTERVAL = confi.int("KEEP_ALIVE_INTERVAL", 0)
@@ -234,15 +252,15 @@
 
     OPAL_CLIENT_STAT_ID = confi.str(
         "OPAL_CLIENT_STAT_ID",
         None,
         description="Unique client statistics identifier",
     )
 
-    OPA_HEALTH_CHECK_POLICY_PATH = "opa/healthcheck/opal.rego"
+    OPA_HEALTH_CHECK_POLICY_PATH = "engine/healthcheck/opal.rego"
 
     SCOPE_ID = confi.str("SCOPE_ID", "default", description="OPAL Scope ID")
 
     STORE_BACKUP_PATH = confi.str(
         "STORE_BACKUP_PATH",
         "/opal/backup/opa.json",
         description="Path to backup policy store's data to",
@@ -256,15 +274,15 @@
         "OFFLINE_MODE_ENABLED",
         False,
         description="If set, opal client will try to load policy store from backup file and operate even if server is unreachable. Ignored if INLINE_OPA_ENABLED=False",
     )
 
     def on_load(self):
         # LOGGER
-        if self.INLINE_OPA_LOG_FORMAT == OpaLogFormat.NONE:
+        if self.INLINE_OPA_LOG_FORMAT == EngineLogFormat.NONE:
             opal_common_config.LOG_MODULE_EXCLUDE_LIST.append("opal_client.opa.logger")
             # re-assign to apply to internal confi-entries as well
             opal_common_config.LOG_MODULE_EXCLUDE_LIST = (
                 opal_common_config.LOG_MODULE_EXCLUDE_LIST
             )
```

### Comparing `opal-client-0.6.1/opal_client/data/api.py` & `opal-client-0.7.0/opal_client/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/data/fetcher.py` & `opal-client-0.7.0/opal_client/data/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/data/rpc.py` & `opal-client-0.7.0/opal_client/data/rpc.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/data/updater.py` & `opal-client-0.7.0/opal_client/data/updater.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/limiter.py` & `opal-client-0.7.0/opal_client/limiter.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/opa/healthcheck/opal.rego` & `opal-client-0.7.0/opal_client/engine/healthcheck/opal.rego`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/opa/logger.py` & `opal-client-0.7.0/opal_client/engine/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 from enum import Enum
 from typing import Optional
 
-from opal_client.config import OpaLogFormat
+from opal_client.config import EngineLogFormat
 from opal_client.logger import logger
 
 
 def logging_level_from_string(level: str) -> int:
     """logger.log() requires an int logging level."""
     level = level.lower()
     if level == "info":
@@ -22,39 +22,39 @@
         return logging.WARNING
     elif level == "debug":
         return logging.DEBUG
     # default
     return logging.INFO
 
 
-async def pipe_opa_logs(stream, logs_format: OpaLogFormat):
+async def pipe_opa_logs(stream, logs_format: EngineLogFormat):
     """gets a stream of logs from the opa process, and logs it into the main
     opal log."""
-    if logs_format == OpaLogFormat.NONE:
+    if logs_format == EngineLogFormat.NONE:
         return
 
     while True:
         line = await stream.readline()
         if not line:
             break
         try:
             log_line = json.loads(line)
             level = logging.getLevelName(
                 logging_level_from_string(log_line.pop("level", "info"))
             )
             msg = log_line.pop("msg", None)
 
             logged = False
-            if logs_format == OpaLogFormat.MINIMAL:
+            if logs_format == EngineLogFormat.MINIMAL:
                 logged = log_event_name(level, msg)
-            elif logs_format == OpaLogFormat.HTTP:
+            elif logs_format == EngineLogFormat.HTTP:
                 logged = log_formatted_http_details(level, msg, log_line)
 
             # always fall back to log the entire line
-            if not logged or logs_format == OpaLogFormat.FULL:
+            if not logged or logs_format == EngineLogFormat.FULL:
                 log_entire_dict(level, msg, log_line)
         except json.JSONDecodeError:
             logger.info(line)
 
 
 def log_event_name(level: str, msg: Optional[str]) -> bool:
     if msg is not None:
@@ -91,7 +91,26 @@
 
     try:
         log_line = json.dumps(log_line)  # should be ok, originated in json
     except:
         pass  # fallback to dict
     logger.opt(colors=True).log(level, format, msg=msg, log_line=log_line)
     return True
+
+
+async def pipe_simple_logs(stream, logs_format: EngineLogFormat):
+    """Gets a stream of logs from the engine process, and logs it into the main
+    opal log."""
+    if logs_format == EngineLogFormat.NONE:
+        return
+
+    while True:
+        line = await stream.readline()
+        if not line:
+            break
+
+        try:
+            line = line.decode().strip()
+        except UnicodeDecodeError:
+            ...
+
+        logger.info(line)
```

### Comparing `opal-client-0.6.1/opal_client/opa/runner.py` & `opal-client-0.7.0/opal_client/engine/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import time
 from typing import Callable, Coroutine, List, Optional
 
 import psutil
-from opal_client.config import OpaLogFormat
+from opal_client.config import EngineLogFormat
+from opal_client.engine.logger import pipe_opa_logs, pipe_simple_logs
+from opal_client.engine.options import CedarServerOptions, OpaServerOptions
 from opal_client.logger import logger
-from opal_client.opa.logger import pipe_opa_logs
-from opal_client.opa.options import OpaServerOptions
 from tenacity import retry, wait_random_exponential
 
 AsyncCallback = Callable[[], Coroutine]
 
 
 async def wait_until_process_is_up(
     process_pid: int,
@@ -21,109 +21,101 @@
     """waits until the pid of the process exists, then optionally runs a
     callback.
 
     optionally receives a timeout to give up.
     """
     start_time = time.time()
     while not psutil.pid_exists(process_pid):
-        if timeout is not None and start_time - time() > timeout:
+        if timeout is not None and start_time - time.time() > timeout:
             break
         await asyncio.sleep(wait_interval)
     if callback is not None:
         await callback()
 
 
-class OpaRunner:
-    """Runs OPA in a supervised subprocess.
+class PolicyEngineRunner:
+    """Runs the policy engine in a supervised subprocess.
 
-    - if the OPA process fails, OPA runner will restart the process.
-    - OPA runner can register callbacks on the lifecycle of OPA,
-    making it easy to keep the OPA cache hydrated (up-to-date).
-    - OPA runner can pipe the logs of the OPA process into OPAL logger.
+    - if the process fails, the runner will restart the process.
+    - The runner can register callbacks on the lifecycle of OPA,
+    making it easy to keep the policy engine cache hydrated (up-to-date).
+    - The runner can pipe the logs of the process into OPAL logger.
     """
 
     def __init__(
         self,
-        options: Optional[OpaServerOptions] = None,
-        piped_logs_format: OpaLogFormat = OpaLogFormat.NONE,
+        piped_logs_format: EngineLogFormat = EngineLogFormat.NONE,
     ):
-        self._options = options or OpaServerOptions()
         self._stopped = False
-        self._process = None
+        self._process: Optional[asyncio.subprocess.Process] = None
         self._should_stop: Optional[asyncio.Event] = None
         self._run_task: Optional[asyncio.Task] = None
-        self._on_opa_initial_start_callbacks: List[AsyncCallback] = []
-        self._on_opa_restart_callbacks: List[AsyncCallback] = []
+        self._on_process_initial_start_callbacks: List[AsyncCallback] = []
+        self._on_process_restart_callbacks: List[AsyncCallback] = []
         self._process_was_never_up_before = True
         self._piped_logs_format = piped_logs_format
 
+    @property
+    def command(self) -> str:
+        raise NotImplementedError()
+
     async def __aenter__(self):
         self.start()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.stop()
 
     def start(self):
-        """starts the opa runner task, and launches the OPA subprocess."""
-        logger.info("Launching opa runner")
+        """starts the runner task, and launches the OPA subprocess."""
+        logger.info("Launching engine runner")
         self._run_task = asyncio.create_task(self._run())
 
     async def stop(self):
-        """stops the opa runner task (and terminates OPA)"""
+        """stops the runner task (and terminates OPA)"""
         self._init_events()
         if not self._should_stop.is_set():
-            logger.info("Stopping opa runner")
+            logger.info("Stopping policy engine runner")
             self._should_stop.set()
-            self._terminate_opa()
+            logger.info("Stopping policy engine")
+            self._process.terminate()
             await asyncio.sleep(1)  # wait for opa process to go down
 
         if self._run_task is not None:
             await self._run_task
         self._run_task = None
 
     async def wait_until_done(self):
-        """waits until the OPA runner task is complete.
+        """waits until the engine runner task is complete.
 
-        this is great when using opa runner as a context manager.
+        this is great when using engine runner as a context manager.
         """
         if self._run_task is not None:
             await self._run_task
 
-    @property
-    def command(self):
-        opts = self._options.get_cli_options_dict()
-        opts_string = " ".join([f"{k}={v}" for k, v in opts.items()])
-        startup_files = self._options.get_opa_startup_files()
-        return f"opa run --server {opts_string} {startup_files}".strip()
-
-    def _terminate_opa(self):
-        logger.info("Stopping OPA")
-        self._process.terminate()
-
     async def _run(self):
         self._init_events()
         while not self._should_stop.is_set():
             for task in asyncio.as_completed(
-                [self._run_opa_until_terminated(), self._should_stop.wait()]
+                [self._run_process_until_terminated(), self._should_stop.wait()]
             ):
                 await task
                 break
 
     @retry(wait=wait_random_exponential(multiplier=0.5, max=10))
-    async def _run_opa_until_terminated(self) -> int:
-        """This function runs opa server as a subprocess.
+    async def _run_process_until_terminated(self) -> int:
+        """This function runs the policy engine as a subprocess.
 
         it returns only when the process terminates.
         """
-        logger.info("Running OPA inline: {command}", command=self.command)
+        logger.info("Running policy engine inline: {command}", command=self.command)
 
         logs_sink = (
             asyncio.subprocess.DEVNULL
-            if self._piped_logs_format == OpaLogFormat.NONE
+            if self._piped_logs_format == EngineLogFormat.NONE
             else asyncio.subprocess.PIPE
         )
 
         self._process = await asyncio.create_subprocess_shell(
             self.command,
             stdout=logs_sink,
             stderr=logs_sink,
@@ -133,86 +125,158 @@
         # waits until the process is up, then runs a callback
         asyncio.create_task(
             wait_until_process_is_up(
                 self._process.pid, callback=self._run_start_callbacks
             )
         )
 
-        if self._piped_logs_format != OpaLogFormat.NONE:
+        if self._piped_logs_format != EngineLogFormat.NONE:
             await asyncio.wait(
                 [
-                    pipe_opa_logs(self._process.stdout, self._piped_logs_format),
-                    pipe_opa_logs(self._process.stderr, self._piped_logs_format),
+                    self.pipe_logs(self._process.stdout, self._piped_logs_format),
+                    self.pipe_logs(self._process.stderr, self._piped_logs_format),
                 ]
             )
 
         return_code = await self._process.wait()
         logger.info(
-            "OPA exited with return code: {return_code}", return_code=return_code
+            "Policy engine exited with return code: {return_code}",
+            return_code=return_code,
         )
-        if return_code > 0:  # exception in running opa
-            raise Exception(f"OPA exited with return code: {return_code}")
+        if return_code > 0:  # exception in running process
+            raise Exception(f"Policy engine exited with return code: {return_code}")
         return return_code
 
-    def register_opa_initial_start_callbacks(self, callbacks: List[AsyncCallback]):
+    def register_process_initial_start_callbacks(self, callbacks: List[AsyncCallback]):
         """register a callback to run when OPA is started the first time."""
-        self._on_opa_initial_start_callbacks.extend(callbacks)
+        self._on_process_initial_start_callbacks.extend(callbacks)
 
-    def register_opa_restart_callbacks(self, callbacks: List[AsyncCallback]):
+    def register_process_restart_callbacks(self, callbacks: List[AsyncCallback]):
         """register a callback to run when OPA is restarted (i.e: OPA was
         already up, then got terminated, and now is up again).
 
         this is most often used to keep OPA's cache (policy and data)
         up-to-date, since OPA is started without policy or data. With
         empty cache, OPA cannot evaluate authorization queries
         correctly.
         """
-        self._on_opa_restart_callbacks.extend(callbacks)
+        self._on_process_restart_callbacks.extend(callbacks)
 
     async def _run_start_callbacks(self):
         """runs callbacks after OPA process starts."""
         # TODO: make policy store expose the /health api of OPA
         await asyncio.sleep(1)
 
         if self._process_was_never_up_before:
             # no need to rehydrate the first time
             self._process_was_never_up_before = False
-            logger.info("Running OPA initial start callbacks")
+            logger.info("Running policy engine initial start callbacks")
             asyncio.create_task(
-                self._run_callbacks(self._on_opa_initial_start_callbacks)
+                self._run_callbacks(self._on_process_initial_start_callbacks)
             )
         else:
-            logger.info("Running OPA rehydration callbacks")
-            asyncio.create_task(self._run_callbacks(self._on_opa_restart_callbacks))
+            logger.info("Running policy engine rehydration callbacks")
+            asyncio.create_task(self._run_callbacks(self._on_process_restart_callbacks))
 
     async def _run_callbacks(self, callbacks: List[AsyncCallback]):
         return await asyncio.gather(*(callback() for callback in callbacks))
 
     def _init_events(self):
         if self._should_stop is None:
             self._should_stop = asyncio.Event()
 
+    async def pipe_logs(self, stream, logs_format: EngineLogFormat):
+        raise NotImplementedError()
+
+
+class OpaRunner(PolicyEngineRunner):
+    def __init__(
+        self,
+        options: Optional[OpaServerOptions] = None,
+        piped_logs_format: EngineLogFormat = EngineLogFormat.NONE,
+    ):
+        super().__init__(piped_logs_format)
+        self._options = options or OpaServerOptions()
+
+    async def pipe_logs(self, stream, logs_format: EngineLogFormat):
+        return await pipe_opa_logs(stream, logs_format)
+
+    @property
+    def command(self) -> str:
+        opts = self._options.get_cli_options_dict()
+        opts_string = " ".join([f"{k}={v}" for k, v in opts.items()])
+        startup_files = self._options.get_opa_startup_files()
+        return f"opa run --server {opts_string} {startup_files}".strip()
+
     @staticmethod
     def setup_opa_runner(
         options: Optional[OpaServerOptions] = None,
-        piped_logs_format: OpaLogFormat = OpaLogFormat.NONE,
+        piped_logs_format: EngineLogFormat = EngineLogFormat.NONE,
         initial_start_callbacks: Optional[List[AsyncCallback]] = None,
         rehydration_callbacks: Optional[List[AsyncCallback]] = None,
     ):
         """factory for OpaRunner, accept optional callbacks to run in certain
         lifecycle events.
 
         Initial Start Callbacks:
-            The first time we start opa, we might want to do certain actions (like launch tasks)
+            The first time we start the engine, we might want to do certain actions (like launch tasks)
             that are dependent on the policy store being up (such as PolicyUpdater, DataUpdater).
 
         Rehydration Callbacks:
-            when opa restarts, its cache is clean and it does not have the state necessary
+            when the engine restarts, its cache is clean and it does not have the state necessary
             to handle authorization queries. therefore it is necessary that we rehydrate the
             cache with fresh state fetched from the server.
         """
         opa_runner = OpaRunner(options=options, piped_logs_format=piped_logs_format)
         if initial_start_callbacks:
-            opa_runner.register_opa_initial_start_callbacks(initial_start_callbacks)
+            opa_runner.register_process_initial_start_callbacks(initial_start_callbacks)
         if rehydration_callbacks:
-            opa_runner.register_opa_restart_callbacks(rehydration_callbacks)
+            opa_runner.register_process_restart_callbacks(rehydration_callbacks)
         return opa_runner
+
+
+class CedarRunner(PolicyEngineRunner):
+    def __init__(
+        self,
+        options: Optional[CedarServerOptions] = None,
+        piped_logs_format: EngineLogFormat = EngineLogFormat.NONE,
+    ):
+        super().__init__(piped_logs_format)
+        self._options = options or CedarServerOptions()
+
+    @property
+    def command(self) -> str:
+        return self._options.get_cmdline()
+
+    @staticmethod
+    def setup_cedar_runner(
+        options: Optional[CedarServerOptions] = None,
+        piped_logs_format: EngineLogFormat = EngineLogFormat.NONE,
+        initial_start_callbacks: Optional[List[AsyncCallback]] = None,
+        rehydration_callbacks: Optional[List[AsyncCallback]] = None,
+    ):
+        """Factory for CedarRunner, accept optional callbacks to run in certain
+        lifecycle events.
+
+        Initial Start Callbacks:
+            The first time we start the engine, we might want to do certain actions (like launch tasks)
+            that are dependent on the policy store being up (such as PolicyUpdater, DataUpdater).
+
+        Rehydration Callbacks:
+            when the engine restarts, its cache is clean and it does not have the state necessary
+            to handle authorization queries. therefore it is necessary that we rehydrate the
+            cache with fresh state fetched from the server.
+        """
+        cedar_runner = CedarRunner(options=options, piped_logs_format=piped_logs_format)
+
+        if initial_start_callbacks:
+            cedar_runner.register_process_initial_start_callbacks(
+                initial_start_callbacks
+            )
+
+        if rehydration_callbacks:
+            cedar_runner.register_process_restart_callbacks(rehydration_callbacks)
+
+        return cedar_runner
+
+    async def pipe_logs(self, stream, logs_format: EngineLogFormat):
+        return await pipe_simple_logs(stream, logs_format)
```

### Comparing `opal-client-0.6.1/opal_client/policy/fetcher.py` & `opal-client-0.7.0/opal_client/policy/fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/policy/options.py` & `opal-client-0.7.0/opal_client/policy/options.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/policy/topics.py` & `opal-client-0.7.0/opal_client/policy/topics.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/policy/updater.py` & `opal-client-0.7.0/opal_client/policy/updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                 else:
                     deleted_files = (
                         None
                         if bundle.deleted_files is None
                         else bundle.deleted_files.dict()
                     )
                     logger.info(
-                        "got policy bundle (delta): '{diff_against_hash}' -> '{commit_hash}'",
+                        "got policy bundle (delta): '{diff_against_hash}' -> '{commit_hash}', manifest: {manifest}, deleted: {deleted}",
                         commit_hash=bundle.hash,
                         diff_against_hash=bundle.old_hash,
                         manifest=bundle.manifest,
                         deleted=deleted_files,
                     )
         except Exception as err:
             bundle_error = repr(err)
```

### Comparing `opal-client-0.6.1/opal_client/policy_store/api.py` & `opal-client-0.7.0/opal_client/policy_store/api.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/policy_store/base_policy_store_client.py` & `opal-client-0.7.0/opal_client/policy_store/base_policy_store_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import uuid
-from asyncio import StreamReader, StreamWriter
 from datetime import datetime
 from functools import partial
 from inspect import signature
 from typing import Any, Dict, List, Optional, Union
 
+from aiofiles.threadpool.text import AsyncTextIOWrapper
 from opal_client.config import opal_client_config
 from opal_client.logger import logger
 from opal_common.schemas.data import JsonableValue
 from opal_common.schemas.policy import PolicyBundle
 from opal_common.schemas.store import RemoteStatus, StoreTransaction
 from pydantic import BaseModel
 
@@ -63,18 +63,18 @@
 
     async def log_transaction(self, transaction: StoreTransaction):
         raise NotImplementedError()
 
     async def is_healthy(self) -> bool:
         raise NotImplementedError()
 
-    async def full_export(self, writer: StreamWriter) -> None:
+    async def full_export(self, writer: AsyncTextIOWrapper) -> None:
         raise NotImplementedError()
 
-    async def full_import(self, reader: StreamReader) -> None:
+    async def full_import(self, reader: AsyncTextIOWrapper) -> None:
         raise NotImplementedError()
 
 
 class PolicyStoreTransactionContextManager(AbstractPolicyStore):
     def __init__(
         self,
         policy_store: "BasePolicyStoreClient",
```

### Comparing `opal-client-0.6.1/opal_client/policy_store/mock_policy_store_client.py` & `opal-client-0.7.0/opal_client/policy_store/mock_policy_store_client.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/policy_store/opa_client.py` & `opal-client-0.7.0/opal_client/policy_store/opa_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import asyncio
 import functools
 import json
 import time
-from asyncio import StreamReader, StreamWriter
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Set
 from urllib.parse import urlencode
 
 import aiohttp
 import dpath
+from aiofiles.threadpool.text import AsyncTextIOWrapper
 from fastapi import Response, status
 from opal_client.config import opal_client_config
 from opal_client.logger import logger
 from opal_client.policy_store.base_policy_store_client import (
     BasePolicyStoreClient,
     JsonableValue,
 )
 from opal_client.policy_store.schemas import PolicyStoreAuth
 from opal_client.utils import proxy_response
+from opal_common.engine.parsing import get_rego_package
 from opal_common.git.bundle_utils import BundleUtils
-from opal_common.opa.parsing import get_rego_package
 from opal_common.paths import PathUtils
 from opal_common.schemas.policy import DataModule, PolicyBundle, RegoModule
 from opal_common.schemas.store import JSONPatchAction, StoreTransaction, TransactionType
 from pydantic import BaseModel
 from tenacity import RetryError, retry
 
 JSONPatchDocument = List[JSONPatchAction]
@@ -815,22 +815,22 @@
 
     async def is_ready(self) -> bool:
         return self._transaction_state.ready
 
     async def is_healthy(self) -> bool:
         return self._transaction_state.healthy
 
-    async def full_export(self, writer: StreamWriter) -> None:
+    async def full_export(self, writer: AsyncTextIOWrapper) -> None:
         policies = await self.get_policies()
         data = self._policy_data_cache.get_data()
         await writer.write(
             json.dumps({"policies": policies, "data": data}, default=str)
         )
 
-    async def full_import(self, reader: StreamReader) -> None:
+    async def full_import(self, reader: AsyncTextIOWrapper) -> None:
         import_data = json.loads(await reader.read())
 
         await OpaClient._attempt_operations_with_postponed_failure_retry(
             [
                 functools.partial(self.set_policy, policy_id=id, policy_code=raw)
                 for id, raw in import_data["policies"].items()
             ]
```

### Comparing `opal-client-0.6.1/opal_client/policy_store/policy_store_client_factory.py` & `opal-client-0.7.0/opal_client/policy_store/policy_store_client_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,39 +102,51 @@
         oauth_server = oauth_server or opal_client_config.POLICY_STORE_AUTH_OAUTH_SERVER
         data_updater_enabled = (
             data_updater_enabled
             if data_updater_enabled is not None
             else opal_client_config.DATA_UPDATER_ENABLED
         )
 
+        res: Optional[BasePolicyStoreClient] = None
+
         # OPA
         if PolicyStoreTypes.OPA == store_type:
             from opal_client.policy_store.opa_client import OpaClient
 
             res = OpaClient(
                 url,
                 opa_auth_token=store_token,
                 auth_type=auth_type,
                 oauth_client_id=oauth_client_id,
                 oauth_client_secret=oauth_client_secret,
                 oauth_server=oauth_server,
                 data_updater_enabled=data_updater_enabled,
                 cache_policy_data=offline_mode_enabled,
             )
+        elif PolicyStoreTypes.CEDAR == store_type:
+            from opal_client.policy_store.cedar_client import CedarClient
+
+            res = CedarClient(
+                url,
+                cedar_auth_token=store_token,
+                auth_type=auth_type,
+            )
         # MOCK
         elif PolicyStoreTypes.MOCK == store_type:
             from opal_client.policy_store.mock_policy_store_client import (
                 MockPolicyStoreClient,
             )
 
             res = MockPolicyStoreClient()
-        else:
+
+        if res is None:
             raise InvalidPolicyStoreTypeException(
                 f"{store_type} is not a valid policy store type"
             )
+
         # save to cache
         if save_to_cache:
             cls.CACHE[cls.get_cache_key(store_type, url)] = res
         # return the result
         return res
 
     @staticmethod
```

### Comparing `opal-client-0.6.1/opal_client/policy_store/schemas.py` & `opal-client-0.7.0/opal_client/policy_store/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Optional
 
 from pydantic import BaseModel, Field, validator
 
 
 class PolicyStoreTypes(Enum):
     OPA = "OPA"
+    CEDAR = "CEDAR"
     MOCK = "MOCK"
 
 
 class PolicyStoreAuth(Enum):
     NONE = "none"
     TOKEN = "token"
     OAUTH = "oauth"
```

### Comparing `opal-client-0.6.1/opal_client/tests/data_updater_test.py` & `opal-client-0.7.0/opal_client/tests/data_updater_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/tests/opa_client_test.py` & `opal-client-0.7.0/opal_client/tests/opa_client_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client/tests/server_to_client_intergation_test.py` & `opal-client-0.7.0/opal_client/tests/server_to_client_intergation_test.py`

 * *Files identical despite different names*

### Comparing `opal-client-0.6.1/opal_client.egg-info/PKG-INFO` & `opal-client-0.7.0/opal_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-client
-Version: 0.6.1
+Version: 0.7.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-client is deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by connecting to an opal-server and subscribing to pub/sub updates for policy and policy data changes.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-client Version: 0.6.1 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-client Version: 0.7.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-client is
 deployed alongside a policy-store (e.g: OPA), keeping it up-to-date, by
 connecting to an opal-server and subscribing to pub/sub updates for policy and
 policy data changes. Home-page: https://github.com/permitio/opal Author: Or
 Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved ::
```

### Comparing `opal-client-0.6.1/opal_client.egg-info/SOURCES.txt` & `opal-client-0.7.0/opal_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 opal_client/callbacks/register.py
 opal_client/callbacks/reporter.py
 opal_client/data/__init__.py
 opal_client/data/api.py
 opal_client/data/fetcher.py
 opal_client/data/rpc.py
 opal_client/data/updater.py
-opal_client/opa/__init__.py
-opal_client/opa/logger.py
-opal_client/opa/options.py
-opal_client/opa/runner.py
-opal_client/opa/healthcheck/opal.rego
+opal_client/engine/__init__.py
+opal_client/engine/logger.py
+opal_client/engine/options.py
+opal_client/engine/runner.py
+opal_client/engine/healthcheck/opal.rego
 opal_client/policy/__init__.py
 opal_client/policy/api.py
 opal_client/policy/fetcher.py
 opal_client/policy/options.py
 opal_client/policy/topics.py
 opal_client/policy/updater.py
 opal_client/policy_store/__init__.py
 opal_client/policy_store/api.py
 opal_client/policy_store/base_policy_store_client.py
+opal_client/policy_store/cedar_client.py
 opal_client/policy_store/mock_policy_store_client.py
 opal_client/policy_store/opa_client.py
 opal_client/policy_store/policy_store_client_factory.py
 opal_client/policy_store/schemas.py
 opal_client/tests/__init__.py
 opal_client/tests/data_updater_test.py
 opal_client/tests/opa_client_test.py
```

### Comparing `opal-client-0.6.1/setup.py` & `opal-client-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     " an opal-server and subscribing to pub/sub updates for policy and policy data changes.",
     long_description_content_type="text/markdown",
     long_description=get_long_description(),
     url="https://github.com/permitio/opal",
     license=about.__license__,
     packages=find_packages(include=("opal_client*",)),
     package_data={
-        "": ["opa/healthcheck/opal.rego"],
+        "": ["engine/healthcheck/opal.rego"],
     },
     classifiers=[
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

