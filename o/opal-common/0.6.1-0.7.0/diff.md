# Comparing `tmp/opal-common-0.6.1.tar.gz` & `tmp/opal-common-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-common-0.6.1.tar", last modified: Mon May  1 17:32:27 2023, max compression
+gzip compressed data, was "opal-common-0.7.0.tar", last modified: Wed May 10 19:01:52 2023, max compression
```

## Comparing `opal-common-0.6.1.tar` & `opal-common-0.7.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.261156 opal-common-0.6.1/
--rw-r--r--   0 roekatz    (501) staff       (20)     8348 2023-05-01 17:32:27.260980 opal-common-0.6.1/PKG-INFO
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.245139 opal-common-0.6.1/opal_common/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      797 2022-12-08 13:45:19.000000 opal-common-0.6.1/opal_common/async_utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.247190 opal-common-0.6.1/opal_common/authentication/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/authentication/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1477 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/authentication/authz.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3267 2022-12-08 13:45:19.000000 opal-common-0.6.1/opal_common/authentication/casting.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5016 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/authentication/deps.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4669 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/authentication/signer.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.247454 opal-common-0.6.1/opal_common/authentication/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/authentication/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    17336 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/authentication/tests/jwt_signer_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)      958 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/authentication/types.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4225 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/authentication/verifier.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.248432 opal-common-0.6.1/opal_common/cli/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/cli/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6657 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/cli/commands.py
--rw-r--r--   0 roekatz    (501) staff       (20)      703 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/cli/docs.py
--rw-r--r--   0 roekatz    (501) staff       (20)      167 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/cli/typer_app.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.249263 opal-common-0.6.1/opal_common/confi/
--rw-r--r--   0 roekatz    (501) staff       (20)       21 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/confi/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2278 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/confi/cli.py
--rw-r--r--   0 roekatz    (501) staff       (20)    13780 2023-04-18 15:25:03.000000 opal-common-0.6.1/opal_common/confi/confi.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2719 2023-04-18 15:25:03.000000 opal-common-0.6.1/opal_common/confi/types.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6648 2023-04-18 15:25:03.000000 opal-common-0.6.1/opal_common/config.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1492 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/corn_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6050 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/emport.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.250379 opal-common-0.6.1/opal_common/fetcher/
--rw-r--r--   0 roekatz    (501) staff       (20)      143 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.251220 opal-common-0.6.1/opal_common/fetcher/engine/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/engine/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2653 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/engine/base_fetching_engine.py
--rw-r--r--   0 roekatz    (501) staff       (20)      296 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/engine/core_callbacks.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1536 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/engine/fetch_worker.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8485 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/fetcher/engine/fetching_engine.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1191 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/events.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2548 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/fetcher/fetch_provider.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3030 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/fetcher_register.py
--rw-r--r--   0 roekatz    (501) staff       (20)      116 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/logger.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.251931 opal-common-0.6.1/opal_common/fetcher/providers/
--rw-r--r--   0 roekatz    (501) staff       (20)       67 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/providers/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1710 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3525 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/providers/http_fetch_provider.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.252534 opal-common-0.6.1/opal_common/fetcher/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1917 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/fetcher/tests/failure_handler_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4260 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/tests/http_fetch_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2140 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/fetcher/tests/rpc_fetch_test.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.254673 opal-common-0.6.1/opal_common/git/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/git/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5461 2023-02-14 09:43:53.000000 opal-common-0.6.1/opal_common/git/branch_tracker.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15616 2023-04-18 15:25:03.000000 opal-common-0.6.1/opal_common/git/bundle_maker.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1887 2023-04-04 08:50:35.000000 opal-common-0.6.1/opal_common/git/bundle_utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8684 2023-04-04 08:50:50.000000 opal-common-0.6.1/opal_common/git/commit_viewer.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7948 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/git/diff_viewer.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1580 2023-02-14 09:43:53.000000 opal-common-0.6.1/opal_common/git/env.py
--rw-r--r--   0 roekatz    (501) staff       (20)      299 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/git/exceptions.py
--rw-r--r--   0 roekatz    (501) staff       (20)     8535 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/git/repo_cloner.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4237 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/git/tar_file_to_local_git_extractor.py
--rw-r--r--   0 roekatz    (501) staff       (20)      182 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/http.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1832 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/logger.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.255526 opal-common-0.6.1/opal_common/logging/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/logging/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      412 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/logging/decorators.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1166 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/logging/filter.py
--rw-r--r--   0 roekatz    (501) staff       (20)      617 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/logging/formatter.py
--rw-r--r--   0 roekatz    (501) staff       (20)      700 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/logging/intercept.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1355 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/logging/thirdparty.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3520 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/middleware.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.255961 opal-common-0.6.1/opal_common/opa/
--rw-r--r--   0 roekatz    (501) staff       (20)       88 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/opa/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      576 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/opa/parsing.py
--rw-r--r--   0 roekatz    (501) staff       (20)      499 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/opa/paths.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4067 2023-04-20 14:50:53.000000 opal-common-0.6.1/opal_common/paths.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.257616 opal-common-0.6.1/opal_common/schemas/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/schemas/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6313 2023-04-19 08:36:33.000000 opal-common-0.6.1/opal_common/schemas/data.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1387 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/schemas/policy.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1767 2023-02-14 09:43:53.000000 opal-common-0.6.1/opal_common/schemas/policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)      508 2023-04-04 11:14:44.000000 opal-common-0.6.1/opal_common/schemas/scopes.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1573 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/schemas/security.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2003 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/schemas/store.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1438 2023-03-12 07:32:46.000000 opal-common-0.6.1/opal_common/schemas/webhook.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.258211 opal-common-0.6.1/opal_common/security/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/security/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      799 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/security/sslcontext.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3294 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/security/tarsafe.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.258945 opal-common-0.6.1/opal_common/sources/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/sources/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     9414 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/sources/api_policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4283 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/sources/base_policy_source.py
--rw-r--r--   0 roekatz    (501) staff       (20)     4238 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/sources/git_policy_source.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.259554 opal-common-0.6.1/opal_common/synchronization/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/synchronization/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1294 2023-01-19 13:43:15.000000 opal-common-0.6.1/opal_common/synchronization/expiring_redis_lock.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2990 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/synchronization/named_lock.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.260043 opal-common-0.6.1/opal_common/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/tests/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     9622 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/tests/path_utils_test.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1223 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/tests/url_utils_test.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.260684 opal-common-0.6.1/opal_common/topics/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/topics/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2371 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/topics/listener.py
--rw-r--r--   0 roekatz    (501) staff       (20)     6517 2023-04-19 08:36:33.000000 opal-common-0.6.1/opal_common/topics/publisher.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1054 2023-03-27 15:01:56.000000 opal-common-0.6.1/opal_common/topics/utils.py
--rw-r--r--   0 roekatz    (501) staff       (20)      988 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/urls.py
--rw-r--r--   0 roekatz    (501) staff       (20)     5917 2022-12-08 13:40:17.000000 opal-common-0.6.1/opal_common/utils.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-05-01 17:32:27.245941 opal-common-0.6.1/opal_common.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     8348 2023-05-01 17:32:27.000000 opal-common-0.6.1/opal_common.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     3198 2023-05-01 17:32:27.000000 opal-common-0.6.1/opal_common.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-05-01 17:32:27.000000 opal-common-0.6.1/opal_common.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      452 2023-05-01 17:32:27.000000 opal-common-0.6.1/opal_common.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-05-01 17:32:27.000000 opal-common-0.6.1/opal_common.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-05-01 17:32:27.261198 opal-common-0.6.1/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     2601 2022-12-08 13:40:17.000000 opal-common-0.6.1/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.319177 opal-common-0.7.0/
+-rw-r--r--   0 asafc      (501) staff       (20)     8348 2023-05-10 19:01:52.318951 opal-common-0.7.0/PKG-INFO
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.309658 opal-common-0.7.0/opal_common/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      797 2022-10-11 10:23:16.000000 opal-common-0.7.0/opal_common/async_utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.311000 opal-common-0.7.0/opal_common/authentication/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1477 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/authz.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3267 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/casting.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5016 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/deps.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4669 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/signer.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.311211 opal-common-0.7.0/opal_common/authentication/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)    17336 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/tests/jwt_signer_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)      958 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/types.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4225 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/authentication/verifier.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.311659 opal-common-0.7.0/opal_common/cli/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/cli/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6657 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/cli/commands.py
+-rw-r--r--   0 asafc      (501) staff       (20)      703 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/cli/docs.py
+-rw-r--r--   0 asafc      (501) staff       (20)      167 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/cli/typer_app.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.312085 opal-common-0.7.0/opal_common/confi/
+-rw-r--r--   0 asafc      (501) staff       (20)       21 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/confi/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2278 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/confi/cli.py
+-rw-r--r--   0 asafc      (501) staff       (20)    13780 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/confi/confi.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2719 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/confi/types.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6831 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/config.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1492 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/corn_utils.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6050 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/emport.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.312413 opal-common-0.7.0/opal_common/engine/
+-rw-r--r--   0 asafc      (501) staff       (20)       90 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/engine/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      576 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/engine/parsing.py
+-rw-r--r--   0 asafc      (501) staff       (20)      593 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/engine/paths.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.312968 opal-common-0.7.0/opal_common/fetcher/
+-rw-r--r--   0 asafc      (501) staff       (20)      143 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.313480 opal-common-0.7.0/opal_common/fetcher/engine/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/engine/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2653 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/engine/base_fetching_engine.py
+-rw-r--r--   0 asafc      (501) staff       (20)      296 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/engine/core_callbacks.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1536 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/engine/fetch_worker.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8485 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/fetcher/engine/fetching_engine.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/events.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2548 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/fetcher/fetch_provider.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3030 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/fetcher_register.py
+-rw-r--r--   0 asafc      (501) staff       (20)      116 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/logger.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.313832 opal-common-0.7.0/opal_common/fetcher/providers/
+-rw-r--r--   0 asafc      (501) staff       (20)       67 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/providers/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1710 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3525 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/providers/http_fetch_provider.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.314236 opal-common-0.7.0/opal_common/fetcher/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1917 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/fetcher/tests/failure_handler_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4291 2023-05-10 17:44:36.000000 opal-common-0.7.0/opal_common/fetcher/tests/http_fetch_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2140 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/fetcher/tests/rpc_fetch_test.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.315286 opal-common-0.7.0/opal_common/git/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/git/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5461 2023-02-01 11:46:28.000000 opal-common-0.7.0/opal_common/git/branch_tracker.py
+-rw-r--r--   0 asafc      (501) staff       (20)    15557 2023-05-10 17:44:40.000000 opal-common-0.7.0/opal_common/git/bundle_maker.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1887 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/git/bundle_utils.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8684 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/git/commit_viewer.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7948 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/git/diff_viewer.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1580 2023-02-01 11:46:28.000000 opal-common-0.7.0/opal_common/git/env.py
+-rw-r--r--   0 asafc      (501) staff       (20)      299 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/git/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8535 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/git/repo_cloner.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4237 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/git/tar_file_to_local_git_extractor.py
+-rw-r--r--   0 asafc      (501) staff       (20)      182 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/http.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1832 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/logger.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.315895 opal-common-0.7.0/opal_common/logging/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      412 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/decorators.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1166 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/filter.py
+-rw-r--r--   0 asafc      (501) staff       (20)      617 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/formatter.py
+-rw-r--r--   0 asafc      (501) staff       (20)      700 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/intercept.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1355 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/logging/thirdparty.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3520 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/middleware.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4067 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/paths.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.316740 opal-common-0.7.0/opal_common/schemas/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6313 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/schemas/data.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1387 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/policy.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1767 2023-02-24 20:59:56.000000 opal-common-0.7.0/opal_common/schemas/policy_source.py
+-rw-r--r--   0 asafc      (501) staff       (20)      508 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/scopes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1573 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/security.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2003 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/schemas/store.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1438 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/schemas/webhook.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.317101 opal-common-0.7.0/opal_common/security/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/security/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      799 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/security/sslcontext.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3294 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/security/tarsafe.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.317589 opal-common-0.7.0/opal_common/sources/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/sources/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9414 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/sources/api_policy_source.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4283 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/sources/base_policy_source.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4238 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/sources/git_policy_source.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.317950 opal-common-0.7.0/opal_common/synchronization/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/synchronization/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1294 2023-02-01 11:46:28.000000 opal-common-0.7.0/opal_common/synchronization/expiring_redis_lock.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2990 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/synchronization/named_lock.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.318272 opal-common-0.7.0/opal_common/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9622 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/tests/path_utils_test.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1223 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/tests/url_utils_test.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.318728 opal-common-0.7.0/opal_common/topics/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/topics/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2371 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/topics/listener.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6517 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/topics/publisher.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1054 2023-05-10 06:45:11.000000 opal-common-0.7.0/opal_common/topics/utils.py
+-rw-r--r--   0 asafc      (501) staff       (20)      988 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/urls.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5917 2022-10-01 21:13:25.000000 opal-common-0.7.0/opal_common/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.310246 opal-common-0.7.0/opal_common.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)     8348 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     3207 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      471 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       12 2023-05-10 19:01:52.000000 opal-common-0.7.0/opal_common.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-10 19:01:52.319215 opal-common-0.7.0/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)     2601 2022-10-01 21:13:25.000000 opal-common-0.7.0/setup.py
```

### Comparing `opal-common-0.6.1/PKG-INFO` & `opal-common-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.6.1
+Version: 0.7.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
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
-Metadata-Version: 2.1 Name: opal-common Version: 0.6.1 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `opal-common-0.6.1/opal_common/async_utils.py` & `opal-common-0.7.0/opal_common/async_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/authentication/authz.py` & `opal-common-0.7.0/opal_common/authentication/authz.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/authentication/casting.py` & `opal-common-0.7.0/opal_common/authentication/casting.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/authentication/deps.py` & `opal-common-0.7.0/opal_common/authentication/deps.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/authentication/signer.py` & `opal-common-0.7.0/opal_common/authentication/signer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/authentication/tests/jwt_signer_test.py` & `opal-common-0.7.0/opal_common/authentication/tests/jwt_signer_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/authentication/types.py` & `opal-common-0.7.0/opal_common/authentication/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/authentication/verifier.py` & `opal-common-0.7.0/opal_common/authentication/verifier.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/cli/commands.py` & `opal-common-0.7.0/opal_common/cli/commands.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/cli/docs.py` & `opal-common-0.7.0/opal_common/cli/docs.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/confi/cli.py` & `opal-common-0.7.0/opal_common/confi/cli.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/confi/confi.py` & `opal-common-0.7.0/opal_common/confi/confi.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/confi/types.py` & `opal-common-0.7.0/opal_common/confi/types.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/config.py` & `opal-common-0.7.0/opal_common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,10 +149,15 @@
         "AUTH_JWT_ALGORITHM",
         JWTAlgorithm,
         getattr(JWTAlgorithm, "RS256"),
         description="jwt algorithm, possible values: see: https://pyjwt.readthedocs.io/en/stable/algorithms.html",
     )
     AUTH_JWT_AUDIENCE = confi.str("AUTH_JWT_AUDIENCE", "https://api.opal.ac/v1/")
     AUTH_JWT_ISSUER = confi.str("AUTH_JWT_ISSUER", f"https://opal.ac/")
+    POLICY_REPO_POLICY_EXTENSIONS = confi.list(
+        "POLICY_REPO_POLICY_EXTENSIONS",
+        [".rego"],
+        description="List of extensions to serve as policy modules",
+    )
 
 
 opal_common_config = OpalCommonConfig(prefix="OPAL_")
```

### Comparing `opal-common-0.6.1/opal_common/corn_utils.py` & `opal-common-0.7.0/opal_common/corn_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/emport.py` & `opal-common-0.7.0/opal_common/emport.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/engine/base_fetching_engine.py` & `opal-common-0.7.0/opal_common/fetcher/engine/base_fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/engine/fetch_worker.py` & `opal-common-0.7.0/opal_common/fetcher/engine/fetch_worker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/engine/fetching_engine.py` & `opal-common-0.7.0/opal_common/fetcher/engine/fetching_engine.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/events.py` & `opal-common-0.7.0/opal_common/fetcher/events.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/fetch_provider.py` & `opal-common-0.7.0/opal_common/fetcher/fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/fetcher_register.py` & `opal-common-0.7.0/opal_common/fetcher/fetcher_register.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py` & `opal-common-0.7.0/opal_common/fetcher/providers/fastapi_rpc_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/providers/http_fetch_provider.py` & `opal-common-0.7.0/opal_common/fetcher/providers/http_fetch_provider.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/tests/failure_handler_test.py` & `opal-common-0.7.0/opal_common/fetcher/tests/failure_handler_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/fetcher/tests/http_fetch_test.py` & `opal-common-0.7.0/opal_common/fetcher/tests/http_fetch_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import asyncio
 from multiprocessing import Process
 
 import pytest
 import uvicorn
 from fastapi import Depends, FastAPI, Header, HTTPException
+from flaky import flaky
 from opal_common.fetcher import FetchingEngine
 from opal_common.fetcher.providers.http_fetch_provider import HttpFetcherConfig
 
 # Configurable
 PORT = int(os.environ.get("PORT") or "9110")
 BASE_URL = f"http://localhost:{PORT}"
 DATA_ROUTE = f"/data"
@@ -119,14 +120,15 @@
         config = {"headers": {"X-TOKEN": SECRET_TOKEN}}
         # fetch with bearer token authorization
         await engine.queue_url(f"{BASE_URL}{AUTHORIZED_DATA_ROUTE}", callback, config)
         await asyncio.wait_for(got_data_event.wait(), 5)
         assert got_data_event.is_set()
 
 
+@flaky
 @pytest.mark.asyncio
 async def test_external_http_get():
     """Test simple http get on external (https://freegeoip.app/) site Checking
     we get a JSON with the data we expected (the IP we queried)"""
     got_data_event = asyncio.Event()
     async with FetchingEngine() as engine:
         url = "https://httpbin.org/anything"
```

### Comparing `opal-common-0.6.1/opal_common/fetcher/tests/rpc_fetch_test.py` & `opal-common-0.7.0/opal_common/fetcher/tests/rpc_fetch_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/git/branch_tracker.py` & `opal-common-0.7.0/opal_common/git/branch_tracker.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/git/bundle_maker.py` & `opal-common-0.7.0/opal_common/git/bundle_maker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from functools import partial
 from pathlib import Path
 from typing import List, Optional, Set
 
 from git import Repo
 from git.objects import Commit
+from opal_common.engine import get_rego_package, is_data_module, is_policy_module
 from opal_common.git.commit_viewer import (
     CommitViewer,
     VersionedDirectory,
     VersionedFile,
     find_ignore_match,
     has_extension,
     is_under_directories,
 )
 from opal_common.git.diff_viewer import (
     DiffViewer,
     diffed_file_has_extension,
     diffed_file_is_under_directories,
 )
 from opal_common.logger import logger
-from opal_common.opa import get_rego_package, is_data_module, is_rego_module
 from opal_common.paths import PathUtils
 from opal_common.schemas.policy import (
     DataModule,
     DeletedFiles,
     PolicyBundle,
     RegoModule,
 )
@@ -252,26 +252,24 @@
                 contents = source_file.read()
                 path = source_file.path
 
                 if is_data_module(path):
                     data_modules.append(
                         DataModule(path=str(path.parent), data=contents)
                     )
-                elif is_rego_module(path):
+                    manifest.append(str(path))
+                elif is_policy_module(path):
                     policy_modules.append(
                         RegoModule(
                             path=str(path),
                             package_name=get_rego_package(contents) or "",
                             rego=contents,
                         )
                     )
-                else:
-                    continue
-
-                manifest.append(str(path))  # only returns the relative path
+                    manifest.append(str(path))
 
             return PolicyBundle(
                 manifest=self._sort_manifest(manifest, explicit_manifest),
                 hash=commit.hexsha,
                 data_modules=data_modules,
                 policy_modules=policy_modules,
             )
@@ -318,34 +316,32 @@
 
                 if is_data_module(path):
                     data_modules.append(
                         # in OPA, the data module path is the containing directory
                         # i.e: /path/to/data.json will put the json contents under "/path/to" in the opa tree
                         DataModule(path=str(path.parent), data=contents)
                     )
-                elif is_rego_module(path):
+                    manifest.append(str(path))
+                elif is_policy_module(path):
                     policy_modules.append(
                         RegoModule(
                             path=str(path),
                             package_name=get_rego_package(contents) or "",
                             rego=contents,
                         )
                     )
-                else:
-                    continue
-
-                manifest.append(str(path))  # only returns the relative path
+                    manifest.append(str(path))
 
             for source_file in viewer.deleted_files(filter):
                 path = source_file.path
 
                 if is_data_module(path):
                     # in OPA, the data module path is the containing directory (see above)
                     deleted_data_modules.append(str(path.parent))
-                elif is_rego_module(path):
+                elif is_policy_module(path):
                     deleted_policy_modules.append(path)
 
             if deleted_data_modules or deleted_policy_modules:
                 deleted_policies = self._sort_manifest(
                     deleted_policy_modules, explicit_manifest
                 )
                 deleted_policies.reverse()  # when removed, dependent policies should be removed first
```

### Comparing `opal-common-0.6.1/opal_common/git/bundle_utils.py` & `opal-common-0.7.0/opal_common/git/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/git/commit_viewer.py` & `opal-common-0.7.0/opal_common/git/commit_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/git/diff_viewer.py` & `opal-common-0.7.0/opal_common/git/diff_viewer.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/git/env.py` & `opal-common-0.7.0/opal_common/git/env.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/git/repo_cloner.py` & `opal-common-0.7.0/opal_common/git/repo_cloner.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/git/tar_file_to_local_git_extractor.py` & `opal-common-0.7.0/opal_common/git/tar_file_to_local_git_extractor.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/logger.py` & `opal-common-0.7.0/opal_common/logger.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/logging/filter.py` & `opal-common-0.7.0/opal_common/logging/filter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/logging/formatter.py` & `opal-common-0.7.0/opal_common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/logging/intercept.py` & `opal-common-0.7.0/opal_common/logging/intercept.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/logging/thirdparty.py` & `opal-common-0.7.0/opal_common/logging/thirdparty.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/middleware.py` & `opal-common-0.7.0/opal_common/middleware.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/opa/parsing.py` & `opal-common-0.7.0/opal_common/engine/parsing.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/paths.py` & `opal-common-0.7.0/opal_common/paths.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/schemas/data.py` & `opal-common-0.7.0/opal_common/schemas/data.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/schemas/policy.py` & `opal-common-0.7.0/opal_common/schemas/policy.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/schemas/policy_source.py` & `opal-common-0.7.0/opal_common/schemas/policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/schemas/security.py` & `opal-common-0.7.0/opal_common/schemas/security.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/schemas/store.py` & `opal-common-0.7.0/opal_common/schemas/store.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/schemas/webhook.py` & `opal-common-0.7.0/opal_common/schemas/webhook.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/security/sslcontext.py` & `opal-common-0.7.0/opal_common/security/sslcontext.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/security/tarsafe.py` & `opal-common-0.7.0/opal_common/security/tarsafe.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/sources/api_policy_source.py` & `opal-common-0.7.0/opal_common/sources/api_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/sources/base_policy_source.py` & `opal-common-0.7.0/opal_common/sources/base_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/sources/git_policy_source.py` & `opal-common-0.7.0/opal_common/sources/git_policy_source.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/synchronization/expiring_redis_lock.py` & `opal-common-0.7.0/opal_common/synchronization/expiring_redis_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/synchronization/named_lock.py` & `opal-common-0.7.0/opal_common/synchronization/named_lock.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/tests/path_utils_test.py` & `opal-common-0.7.0/opal_common/tests/path_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/tests/url_utils_test.py` & `opal-common-0.7.0/opal_common/tests/url_utils_test.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/topics/listener.py` & `opal-common-0.7.0/opal_common/topics/listener.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/topics/publisher.py` & `opal-common-0.7.0/opal_common/topics/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/topics/utils.py` & `opal-common-0.7.0/opal_common/topics/utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/urls.py` & `opal-common-0.7.0/opal_common/urls.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common/utils.py` & `opal-common-0.7.0/opal_common/utils.py`

 * *Files identical despite different names*

### Comparing `opal-common-0.6.1/opal_common.egg-info/PKG-INFO` & `opal-common-0.7.0/opal_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-common
-Version: 0.6.1
+Version: 0.7.0
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. opal-common contains common code used by both opal-client and opal-server.
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
-Metadata-Version: 2.1 Name: opal-common Version: 0.6.1 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-common Version: 0.7.0 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. opal-common contains
 common code used by both opal-client and opal-server. Home-page: https://
 github.com/permitio/opal Author: Or Weis, Asaf Cohen Author-email: or@permit.io
 License: Apache 2.0 Classifier: Operating System :: OS Independent Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `opal-common-0.6.1/opal_common.egg-info/SOURCES.txt` & `opal-common-0.7.0/opal_common.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 opal_common/cli/commands.py
 opal_common/cli/docs.py
 opal_common/cli/typer_app.py
 opal_common/confi/__init__.py
 opal_common/confi/cli.py
 opal_common/confi/confi.py
 opal_common/confi/types.py
+opal_common/engine/__init__.py
+opal_common/engine/parsing.py
+opal_common/engine/paths.py
 opal_common/fetcher/__init__.py
 opal_common/fetcher/events.py
 opal_common/fetcher/fetch_provider.py
 opal_common/fetcher/fetcher_register.py
 opal_common/fetcher/logger.py
 opal_common/fetcher/engine/__init__.py
 opal_common/fetcher/engine/base_fetching_engine.py
@@ -61,17 +64,14 @@
 opal_common/git/tar_file_to_local_git_extractor.py
 opal_common/logging/__init__.py
 opal_common/logging/decorators.py
 opal_common/logging/filter.py
 opal_common/logging/formatter.py
 opal_common/logging/intercept.py
 opal_common/logging/thirdparty.py
-opal_common/opa/__init__.py
-opal_common/opa/parsing.py
-opal_common/opa/paths.py
 opal_common/schemas/__init__.py
 opal_common/schemas/data.py
 opal_common/schemas/policy.py
 opal_common/schemas/policy_source.py
 opal_common/schemas/scopes.py
 opal_common/schemas/security.py
 opal_common/schemas/store.py
```

### Comparing `opal-common-0.6.1/setup.py` & `opal-common-0.7.0/setup.py`

 * *Files identical despite different names*

