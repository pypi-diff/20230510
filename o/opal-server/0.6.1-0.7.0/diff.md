# Comparing `tmp/opal-server-0.6.1.tar.gz` & `tmp/opal-server-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-server-0.6.1.tar", last modified: Mon May  1 17:32:28 2023, max compression
+gzip compressed data, was "opal-server-0.7.0.tar", last modified: Wed May 10 19:01:52 2023, max compression
```

## Comparing `opal-server-0.6.1.tar` & `opal-server-0.7.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.175556 opal-server-0.6.1/
--rw-r--r--   0 roekatz    (501) staff       (20)     8558 2023-05-01 17:32:28.175362 opal-server-0.6.1/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.170313 opal-server-0.6.1/opal_server/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-04-19 15:20:19.000000 opal-server-0.6.1/opal_server/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    10418 2023-04-19 15:20:19.000000 opal-server-0.6.1/opal_server/config.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.171965 opal-server-0.6.1/opal_server/data/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/data/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5297 2022-12-08 13:45:19.000000 opal-server-0.6.1/opal_server/data/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-03-27 15:01:56.000000 opal-server-0.6.1/opal_server/data/data_update_publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)    13130 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/git_fetcher.py
--rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/loadlimiting.py
--rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/main.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.172173 opal-server-0.6.1/opal_server/policy/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/policy/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.172454 opal-server-0.6.1/opal_server/policy/bundles/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/policy/bundles/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4444 2023-02-14 09:43:53.000000 opal-server-0.6.1/opal_server/policy/bundles/api.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.173033 opal-server-0.6.1/opal_server/policy/watcher/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/policy/watcher/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4459 2023-02-28 14:04:36.000000 opal-server-0.6.1/opal_server/policy/watcher/callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5669 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/policy/watcher/factory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-04-29 17:08:57.000000 opal-server-0.6.1/opal_server/policy/watcher/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.173801 opal-server-0.6.1/opal_server/policy/webhook/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/policy/webhook/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5691 2023-05-01 10:44:58.000000 opal-server-0.6.1/opal_server/policy/webhook/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-02-14 09:43:53.000000 opal-server-0.6.1/opal_server/policy/webhook/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/policy/webhook/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3659 2023-04-18 15:25:03.000000 opal-server-0.6.1/opal_server/pubsub.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1390 2022-12-08 13:45:19.000000 opal-server-0.6.1/opal_server/redis.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.174748 opal-server-0.6.1/opal_server/scopes/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/scopes/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12600 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/scopes/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/scopes/loader.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1325 2022-12-08 13:45:19.000000 opal-server-0.6.1/opal_server/scopes/scope_repository.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7285 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/scopes/service.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2811 2023-04-19 08:36:33.000000 opal-server-0.6.1/opal_server/scopes/task.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.175128 opal-server-0.6.1/opal_server/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1423 2022-12-08 13:45:19.000000 opal-server-0.6.1/opal_server/security/api.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal-server-0.6.1/opal_server/security/jwks.py
--rw-r--r--   0 roekatz    (501) staff       (20)    17522 2023-05-01 10:44:58.000000 opal-server-0.6.1/opal_server/server.py
--rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-04-30 12:13:52.000000 opal-server-0.6.1/opal_server/statistics.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:28.171591 opal-server-0.6.1/opal_server.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     8558 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     1246 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/entry_points.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      546 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-05-01 17:32:28.000000 opal-server-0.6.1/opal_server.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-05-01 17:32:28.175598 opal-server-0.6.1/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2979 2022-12-08 13:40:17.000000 opal-server-0.6.1/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.878517 opal-server-0.7.0/
+-rw-r--r--   0 asafc      (501) staff       (20)     8558 2023-05-10 19:01:52.878184 opal-server-0.7.0/PKG-INFO
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.874484 opal-server-0.7.0/opal_server/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2136 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/cli.py
+-rw-r--r--   0 asafc      (501) staff       (20)    10459 2023-05-10 17:44:40.000000 opal-server-0.7.0/opal_server/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.875663 opal-server-0.7.0/opal_server/data/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/data/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5297 2022-10-12 14:50:19.000000 opal-server-0.7.0/opal_server/data/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6110 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/data/data_update_publisher.py
+-rw-r--r--   0 asafc      (501) staff       (20)    13130 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/git_fetcher.py
+-rw-r--r--   0 asafc      (501) staff       (20)      987 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/loadlimiting.py
+-rw-r--r--   0 asafc      (501) staff       (20)      153 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/main.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.875775 opal-server-0.7.0/opal_server/policy/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/policy/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.875946 opal-server-0.7.0/opal_server/policy/bundles/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/policy/bundles/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4447 2023-05-10 17:44:40.000000 opal-server-0.7.0/opal_server/policy/bundles/api.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.876374 opal-server-0.7.0/opal_server/policy/watcher/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/policy/watcher/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4459 2023-02-27 16:56:34.000000 opal-server-0.7.0/opal_server/policy/watcher/callbacks.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5689 2023-05-10 17:44:40.000000 opal-server-0.7.0/opal_server/policy/watcher/factory.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4283 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/policy/watcher/task.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.876837 opal-server-0.7.0/opal_server/policy/webhook/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/policy/webhook/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5691 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/policy/webhook/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6110 2023-02-24 20:59:56.000000 opal-server-0.7.0/opal_server/policy/webhook/deps.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1234 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/policy/webhook/listener.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1331 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/publisher.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3659 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/pubsub.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1390 2022-10-11 10:23:16.000000 opal-server-0.7.0/opal_server/redis.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.877665 opal-server-0.7.0/opal_server/scopes/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/scopes/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12600 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/scopes/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1621 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/scopes/loader.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1325 2022-10-11 10:23:16.000000 opal-server-0.7.0/opal_server/scopes/scope_repository.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7285 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/scopes/service.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2811 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/scopes/task.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.877992 opal-server-0.7.0/opal_server/security/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/security/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1423 2022-10-11 10:23:16.000000 opal-server-0.7.0/opal_server/security/api.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1277 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/security/jwks.py
+-rw-r--r--   0 asafc      (501) staff       (20)    17522 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/server.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12533 2023-02-01 11:46:28.000000 opal-server-0.7.0/opal_server/statistics.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.875306 opal-server-0.7.0/opal_server.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)     8558 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1246 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       52 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/entry_points.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      565 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       12 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-10 19:01:52.878557 opal-server-0.7.0/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)     2979 2022-10-01 21:13:25.000000 opal-server-0.7.0/setup.py
```

### Comparing `opal-server-0.6.1/PKG-INFO` & `opal-server-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.6.1
+Version: 0.7.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
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
-Metadata-Version: 2.1 Name: opal-server Version: 0.6.1 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
```

### Comparing `opal-server-0.6.1/opal_server/cli.py` & `opal-server-0.7.0/opal_server/cli.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/config.py` & `opal-server-0.7.0/opal_server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             "push_event_value": "push",
         },
     )
 
     POLICY_REPO_POLLING_INTERVAL = confi.int("POLICY_REPO_POLLING_INTERVAL", 0)
 
     ALLOWED_ORIGINS = confi.list("ALLOWED_ORIGINS", ["*"])
-    OPA_FILE_EXTENSIONS = (".rego", ".json")
+    FILTER_FILE_EXTENSIONS = confi.list("FILTER_FILE_EXTENSIONS", [".rego", ".json"])
     BUNDLE_IGNORE = confi.list("BUNDLE_IGNORE", [])
 
     NO_RPC_LOGS = confi.bool("NO_RPC_LOGS", True)
 
     # client-api server
     SERVER_WORKER_COUNT = confi.int(
         "SERVER_WORKER_COUNT",
```

### Comparing `opal-server-0.6.1/opal_server/data/api.py` & `opal-server-0.7.0/opal_server/data/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/data/data_update_publisher.py` & `opal-server-0.7.0/opal_server/data/data_update_publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/git_fetcher.py` & `opal-server-0.7.0/opal_server/git_fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/loadlimiting.py` & `opal-server-0.7.0/opal_server/loadlimiting.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/policy/bundles/api.py` & `opal-server-0.7.0/opal_server/policy/bundles/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         None,
         description="hash of previous bundle already downloaded, server will return a diff bundle.",
     ),
 ):
     maker = BundleMaker(
         repo,
         in_directories=set(input_paths),
-        extensions=opal_server_config.OPA_FILE_EXTENSIONS,
+        extensions=opal_server_config.FILTER_FILE_EXTENSIONS,
         root_manifest_path=opal_server_config.POLICY_REPO_MANIFEST_PATH,
         bundle_ignore=opal_server_config.BUNDLE_IGNORE,
     )
     # check if commit exist in the repo
     revision = None
     if base_hash:
         try:
```

### Comparing `opal-server-0.6.1/opal_server/policy/watcher/callbacks.py` & `opal-server-0.7.0/opal_server/policy/watcher/callbacks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/policy/watcher/factory.py` & `opal-server-0.7.0/opal_server/policy/watcher/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         remote_source_url(str): the base address to request the policy from
         clone_path_finder(RepoClonePathFinder): from which the local dir path for the repo clone would be retrieved
         branch_name(str):  name of remote branch in git to pull
         ssh_key (str, optional): private ssh key used to gain access to the cloned repo
         polling_interval(int):  how many seconds need to wait between polling
         request_timeout(int):  how many seconds need to wait until timeout
         policy_bundle_token(int):  auth token to include in connections to OPAL server. Defaults to POLICY_BUNDLE_SERVER_TOKEN.
-        extensions(list(str), optional):  list of extantions to check when new policy arrive default is OPA_FILE_EXTENSIONS
+        extensions(list(str), optional):  list of extantions to check when new policy arrive default is FILTER_FILE_EXTENSIONS
         bundle_ignore(list(str), optional):  list of glob paths to use for excluding files from bundle default is OPA_BUNDLE_IGNORE
     """
     if opal_server_config.SCOPES:
         return ScopesPolicyWatcherTask(pubsub_endpoint)
 
     # load defaults
     source_type = load_conf_if_none(source_type, opal_server_config.POLICY_SOURCE_TYPE)
@@ -73,15 +73,17 @@
     )
     request_timeout = load_conf_if_none(
         request_timeout, opal_server_config.POLICY_REPO_CLONE_TIMEOUT
     )
     policy_bundle_token = load_conf_if_none(
         policy_bundle_token, opal_server_config.POLICY_BUNDLE_SERVER_TOKEN
     )
-    extensions = load_conf_if_none(extensions, opal_server_config.OPA_FILE_EXTENSIONS)
+    extensions = load_conf_if_none(
+        extensions, opal_server_config.FILTER_FILE_EXTENSIONS
+    )
     bundle_ignore = load_conf_if_none(bundle_ignore, opal_server_config.BUNDLE_IGNORE)
     if source_type == PolicySourceTypes.Git:
         remote_source_url = load_conf_if_none(
             remote_source_url, opal_server_config.POLICY_REPO_URL
         )
         if remote_source_url is None:
             logger.warning(
```

### Comparing `opal-server-0.6.1/opal_server/policy/watcher/task.py` & `opal-server-0.7.0/opal_server/policy/watcher/task.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/policy/webhook/api.py` & `opal-server-0.7.0/opal_server/policy/webhook/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/policy/webhook/deps.py` & `opal-server-0.7.0/opal_server/policy/webhook/deps.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/policy/webhook/listener.py` & `opal-server-0.7.0/opal_server/policy/webhook/listener.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/publisher.py` & `opal-server-0.7.0/opal_server/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/pubsub.py` & `opal-server-0.7.0/opal_server/pubsub.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/redis.py` & `opal-server-0.7.0/opal_server/redis.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/scopes/api.py` & `opal-server-0.7.0/opal_server/scopes/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/scopes/loader.py` & `opal-server-0.7.0/opal_server/scopes/loader.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/scopes/scope_repository.py` & `opal-server-0.7.0/opal_server/scopes/scope_repository.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/scopes/service.py` & `opal-server-0.7.0/opal_server/scopes/service.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/scopes/task.py` & `opal-server-0.7.0/opal_server/scopes/task.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/security/api.py` & `opal-server-0.7.0/opal_server/security/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/security/jwks.py` & `opal-server-0.7.0/opal_server/security/jwks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/server.py` & `opal-server-0.7.0/opal_server/server.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server/statistics.py` & `opal-server-0.7.0/opal_server/statistics.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server.egg-info/PKG-INFO` & `opal-server-0.7.0/opal_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.6.1
+Version: 0.7.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
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
-Metadata-Version: 2.1 Name: opal-server Version: 0.6.1 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
```

### Comparing `opal-server-0.6.1/opal_server.egg-info/SOURCES.txt` & `opal-server-0.7.0/opal_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-server-0.6.1/opal_server.egg-info/requires.txt` & `opal-server-0.7.0/opal_server.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 websockets<11,>=10.3
 ddtrace<2,>=1.1.4
 slowapi<1,>=0.1.5
 aioredis<3,>=2.0.1
 pygit2<2,>=1.9.2
 asgiref<4,>=3.5.2
 redis<5,>=4.3.4
-opal-common==0.6.1
+opal-common==0.7.0
 charset-normalizer<3,>=2.0.12
 idna<4,>=3.3
 typer<1,>=0.4.1
 fastapi<1,>=0.78.0
 fastapi_websocket_pubsub==0.3.3
 fastapi_websocket_rpc<1,>=0.1.21
 gunicorn<21,>=20.1.0
 pydantic[email]<2,>=1.9.1
 uvicorn[standard]<1,>=0.17.6
 fastapi-utils<1,>=0.2.1
+setuptools>=65.5.1
 
 [:python_version < "3.8"]
 typing-extensions
```

### Comparing `opal-server-0.6.1/setup.py` & `opal-server-0.7.0/setup.py`

 * *Files identical despite different names*

