# Comparing `tmp/autumn8-1.0.3rc4.tar.gz` & `tmp/autumn8-1.0.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.3rc4.tar", last modified: Thu May  4 15:42:04 2023, max compression
+gzip compressed data, was "autumn8-1.0.5rc1.tar", last modified: Wed May 10 17:32:46 2023, max compression
```

## Comparing `autumn8-1.0.3rc4.tar` & `autumn8-1.0.5rc1.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.394769 autumn8-1.0.3rc4/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 15:42:04.394769 autumn8-1.0.3rc4/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.3rc4/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.374768 autumn8-1.0.3rc4/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.3rc4/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.3rc4/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.3rc4/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-04 13:24:26.000000 autumn8-1.0.3rc4/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1032 2023-04-17 13:57:37.000000 autumn8-1.0.3rc4/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4109 2023-05-04 15:33:49.000000 autumn8-1.0.3rc4/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16909 2023-05-04 15:33:49.000000 autumn8-1.0.3rc4/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.3rc4/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1795 2023-05-04 15:33:49.000000 autumn8-1.0.3rc4/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3304 2023-05-01 12:46:21.000000 autumn8-1.0.3rc4/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.3rc4/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-04 13:24:26.000000 autumn8-1.0.3rc4/autumn8/cli/pending_uploads.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.3rc4/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-04 15:40:42.000000 autumn8-1.0.3rc4/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.3rc4/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.3rc4/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.3rc4/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.3rc4/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.3rc4/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.3rc4/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.3rc4/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.3rc4/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.3rc4/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.3rc4/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.3rc4/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.3rc4/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.3rc4/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.3rc4/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.3rc4/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.3rc4/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.3rc4/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       25 2023-03-28 23:07:20.000000 autumn8-1.0.3rc4/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3637 2023-05-04 15:33:49.000000 autumn8-1.0.3rc4/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12591 2023-05-04 15:40:08.000000 autumn8-1.0.3rc4/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1491 2023-03-10 14:58:37.000000 autumn8-1.0.3rc4/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1149 2023-05-04 15:33:49.000000 autumn8-1.0.3rc4/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.3rc4/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.3rc4/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-04 13:24:26.000000 autumn8-1.0.3rc4/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.374768 autumn8-1.0.3rc4/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-04 15:42:04.000000 autumn8-1.0.3rc4/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1343 2023-05-04 15:42:04.000000 autumn8-1.0.3rc4/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-04 15:42:04.000000 autumn8-1.0.3rc4/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-04 15:42:04.000000 autumn8-1.0.3rc4/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-04 15:42:04.000000 autumn8-1.0.3rc4/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-04 15:42:04.000000 autumn8-1.0.3rc4/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-04 15:34:18.000000 autumn8-1.0.3rc4/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-04 15:42:04.394769 autumn8-1.0.3rc4/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.3rc4/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-04 15:42:04.384768 autumn8-1.0.3rc4/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      685 2023-03-28 23:07:20.000000 autumn8-1.0.3rc4/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.3rc4/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.027403 autumn8-1.0.5rc1/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-10 17:32:46.027403 autumn8-1.0.5rc1/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4075 2023-05-01 12:46:21.000000 autumn8-1.0.5rc1/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:45.997403 autumn8-1.0.5rc1/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc1/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.007403 autumn8-1.0.5rc1/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc1/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc1/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-09 16:01:44.000000 autumn8-1.0.5rc1/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-10 17:16:55.000000 autumn8-1.0.5rc1/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.007403 autumn8-1.0.5rc1/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     9136 2023-05-10 17:16:55.000000 autumn8-1.0.5rc1/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16089 2023-05-10 17:16:55.000000 autumn8-1.0.5rc1/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc1/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4094 2023-05-10 17:16:55.000000 autumn8-1.0.5rc1/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-10 17:16:55.000000 autumn8-1.0.5rc1/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-01 12:46:21.000000 autumn8-1.0.5rc1/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-09 16:01:44.000000 autumn8-1.0.5rc1/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-05 17:40:41.000000 autumn8-1.0.5rc1/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.007403 autumn8-1.0.5rc1/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-01 12:46:21.000000 autumn8-1.0.5rc1/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-10 17:32:00.000000 autumn8-1.0.5rc1/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.017403 autumn8-1.0.5rc1/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-01 12:46:21.000000 autumn8-1.0.5rc1/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-01 12:46:21.000000 autumn8-1.0.5rc1/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc1/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-01 12:46:21.000000 autumn8-1.0.5rc1/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-01 12:46:21.000000 autumn8-1.0.5rc1/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.017403 autumn8-1.0.5rc1/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc1/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc1/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc1/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc1/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc1/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.017403 autumn8-1.0.5rc1/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc1/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc1/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-03-28 23:07:20.000000 autumn8-1.0.5rc1/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-03-28 23:07:20.000000 autumn8-1.0.5rc1/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-03-28 23:07:20.000000 autumn8-1.0.5rc1/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-03-28 23:07:20.000000 autumn8-1.0.5rc1/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.027403 autumn8-1.0.5rc1/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-04-17 13:57:37.000000 autumn8-1.0.5rc1/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.027403 autumn8-1.0.5rc1/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-10 17:16:55.000000 autumn8-1.0.5rc1/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-05 17:40:41.000000 autumn8-1.0.5rc1/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11804 2023-05-09 16:01:44.000000 autumn8-1.0.5rc1/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1427 2023-05-10 17:16:55.000000 autumn8-1.0.5rc1/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-10 17:16:55.000000 autumn8-1.0.5rc1/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-05 17:40:41.000000 autumn8-1.0.5rc1/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-05 17:40:41.000000 autumn8-1.0.5rc1/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-05 17:40:41.000000 autumn8-1.0.5rc1/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-04-17 13:57:37.000000 autumn8-1.0.5rc1/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc1/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-09 16:01:44.000000 autumn8-1.0.5rc1/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:45.997403 autumn8-1.0.5rc1/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4295 2023-05-10 17:32:45.000000 autumn8-1.0.5rc1/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1436 2023-05-10 17:32:45.000000 autumn8-1.0.5rc1/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-10 17:32:45.000000 autumn8-1.0.5rc1/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-10 17:32:45.000000 autumn8-1.0.5rc1/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-10 17:32:45.000000 autumn8-1.0.5rc1/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-10 17:32:45.000000 autumn8-1.0.5rc1/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-09 16:01:44.000000 autumn8-1.0.5rc1/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-10 17:32:46.027403 autumn8-1.0.5rc1/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-03-28 23:07:20.000000 autumn8-1.0.5rc1/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-10 17:32:46.027403 autumn8-1.0.5rc1/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-09 16:01:44.000000 autumn8-1.0.5rc1/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-03-28 23:07:20.000000 autumn8-1.0.5rc1/tests/test_settings.py
```

### Comparing `autumn8-1.0.3rc4/PKG-INFO` & `autumn8-1.0.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.3rc4
+Version: 1.0.5rc1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.3rc4/README.md` & `autumn8-1.0.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/cli/analyze.py` & `autumn8-1.0.5rc1/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/cli/cli_environment.py` & `autumn8-1.0.5rc1/autumn8/cli/cli_environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,34 +3,37 @@
 from typing import Optional
 
 
 @dataclass
 class EnvironmentProperties:
     app_host: str
     s3_host: str
+    a8f_host: str
     s3_bucket_name: str
     s3_bucket_root_folder: Optional[str]
 
 
 # TODO remove - official CLI builds should only point toward production
 
 
 class CliEnvironment(enum.Enum):
-    value: EnvironmentProperties
     LOCALHOST = EnvironmentProperties(
         app_host="http://localhost",
         s3_host="http://localhost:4566",
+        a8f_host="http://localhost:7250",
         s3_bucket_name="predictor-bucket",
         s3_bucket_root_folder=None,
     )
     STAGING = EnvironmentProperties(
         app_host="http://staging.autumn8.ai",
         s3_host="https://s3-accelerate.amazonaws.com",
+        a8f_host="http://autumn8functions.default.aws.staging.autumn8.ai",
         s3_bucket_name="autodl-staging",
         s3_bucket_root_folder="autodl-staging",
     )
     PRODUCTION = EnvironmentProperties(
         app_host="https://autodl.autumn8.ai",
         s3_host="https://s3-accelerate.amazonaws.com",
+        a8f_host="https://autumn8functions.default.aws.autumn8.ai",
         s3_bucket_name="autodl-staging",
         s3_bucket_root_folder="autodl-production",
     )
```

### Comparing `autumn8-1.0.3rc4/autumn8/cli/commands/cloud.py` & `autumn8-1.0.5rc1/autumn8/lib/api/cloud.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,155 +1,132 @@
-import json
-from typing import Optional
+from typing import Any, Dict, Optional
 
-import click
-import questionary
+import requests
+from requests.auth import HTTPBasicAuth
 
-from autumn8.cli import options
 from autumn8.cli.cli_environment import CliEnvironment
-from autumn8.cli.interactive import normalize_args
 from autumn8.common.config.settings import CloudServiceProvider
 from autumn8.common.types import Sla
-from autumn8.lib import logging
-from autumn8.lib.api import cloud
+from autumn8.lib.api_creds import retrieve_api_creds
+from autumn8.lib.http import require_ok_response, url_with_params
 
-logger = logging.getLogger(__name__)
+DEFAULT_API_TIMEOUT = 60
 
 
-@click.group(context_settings={"token_normalize_func": normalize_args})
-def cloud_commands_group():
-    pass
-
-
-@cloud_commands_group.command()
-@options.use_environment
-@options.use_organization_id
-@options.use_quiet_mode
-@options.use_cloud_provider_picker(optional=True)
-@click.option(
-    "-m",
-    "--model_id",
-    help="Model ID to get the deployments for",
-    prompt_required=False,
-    default=None,
-)
-def list_deployments(
+def get_running_deployments(
     organization_id: int,
-    model_id: int,
     environment: CliEnvironment,
-    cloud_provider: CloudServiceProvider,
-    quiet,
+    model_id: Optional[int] = None,
+    service_provider: Optional[CloudServiceProvider] = None,
 ):
-    """List running deployments."""
-    logger.info("Fetching the list of deployments...")
-    deployments = cloud.get_running_deployments(
-        organization_id,
-        environment,
-        model_id=model_id,
-        service_provider=cloud_provider,
+    autodl_host = environment.value.app_host
+
+    params: Dict[str, Any] = {"organization_id": organization_id}
+    if model_id is not None:
+        params["model_id"] = model_id
+    if service_provider is not None:
+        params["service_provider"] = service_provider
+
+    deployments_api_route = f"{autodl_host}/api/cloud/deployments"
+    # TODO: wrap the requests library in a custom class to handle common logic like auth and headers for json
+    response = requests.get(
+        url_with_params(deployments_api_route, params),
+        headers={"Content-Type": "application/json"},
+        auth=HTTPBasicAuth(*retrieve_api_creds()),
+        timeout=DEFAULT_API_TIMEOUT,
     )
 
-    click.echo(json.dumps(deployments, indent=4))
-    return
+    require_ok_response(response)
+    return response.json()["deployments"]
 
 
-@cloud_commands_group.command()
-@click.option(
-    "-hw",
-    "-t",
-    "--machine_type",
-    type=str,
-    help="Server type to use for the deployment",
-    # TODO: add a better interactive prompt listing all available servers
-)
-@options.use_environment
-@options.use_organization_id
-@options.use_quiet_mode
-@click.option(
-    "-m",
-    "--model_id",
-    prompt=True,
-    type=int,
-    help="Model ID to deploy",
-    # TODO: add a better interactive prompt listing all available models
-)
-@click.option(
-    "-b",
-    "--deploy_best",
-    "autopick_machine_by_best_sla",
-    type=click.Choice(list(Sla), case_sensitive=False),
-    help="Let Autumn8 pick the server type automatically for the deployment",
-)
-@options.use_cloud_provider_picker(
-    # prompt disabled, as only A8F works atm
-    optional=True,
-    default_value=CloudServiceProvider.AUTUMN8,
-)
-def deploy(
+def deploy_by_best_sla(
     organization_id: int,
+    environment: CliEnvironment,
     model_id: int,
-    machine_type: Optional[str],
+    best_sla: Sla,
+    schedule_on: Optional[str],
+    deployment_id: Optional[str],
+    service_provider: CloudServiceProvider,
+):
+    autodl_host = environment.value.app_host
+
+    params = {
+        "organization_id": organization_id,
+        "model_id": model_id,
+        "best_sla": best_sla.value,
+        "schedule_on": schedule_on,
+        "deployment_id": deployment_id,
+        "cloud_service_provider": service_provider.value,
+    }
+
+    print("sending", params)
+
+    deployments_api_route = f"{autodl_host}/api/cloud/deployments/by_sla"
+    response = requests.post(
+        url_with_params(deployments_api_route, params),
+        headers={"Content-Type": "application/json"},
+        auth=HTTPBasicAuth(*retrieve_api_creds()),
+        timeout=DEFAULT_API_TIMEOUT,
+    )
+
+    require_ok_response(response)
+    return response.json()
+
+
+def deploy(
+    organization_id: int,
     environment: CliEnvironment,
-    cloud_provider: CloudServiceProvider,
-    autopick_machine_by_best_sla: Optional[Sla],
-    quiet,
+    model_id: int,
+    machine_type: str,
+    schedule_on: Optional[str],
+    deployment_id: Optional[str],
+    service_provider: CloudServiceProvider,
 ):
-    """Deploy a model from AutoDL onto cloud."""
+    autodl_host = environment.value.app_host
 
-    if machine_type is None and autopick_machine_by_best_sla is None:
-        machine_type = questionary.text(
-            message="Machine type (ie. c5.2xlarge)"
-        ).ask()
-
-    logger.info(
-        "Launching a new deployment with %s...",
-        machine_type or f"best {autopick_machine_by_best_sla}",
+    params = {
+        "organization_id": organization_id,
+        "model_id": model_id,
+        "machine_type": machine_type,
+        "schedule_on": schedule_on,
+        "deployment_id": deployment_id,
+        "cloud_service_provider": service_provider.value,
+    }
+
+    deployments_api_route = f"{autodl_host}/api/cloud/deployments"
+    response = requests.post(
+        url_with_params(deployments_api_route, params),
+        headers={"Content-Type": "application/json"},
+        auth=HTTPBasicAuth(*retrieve_api_creds()),
+        timeout=DEFAULT_API_TIMEOUT,
     )
-    if machine_type is not None:
-        deployments = cloud.deploy(
-            organization_id,
-            environment,
-            machine_type=machine_type,
-            service_provider=cloud_provider,
-            model_id=model_id,
-        )
-    else:
-        assert autopick_machine_by_best_sla is not None
-
-        deployments = cloud.deploy_by_best_sla(
-            organization_id,
-            environment,
-            best_sla=autopick_machine_by_best_sla,
-            service_provider=cloud_provider,
-            model_id=model_id,
-        )
-
-    click.echo(json.dumps(deployments, indent=4))
-
-
-@cloud_commands_group.command()
-@options.use_environment
-@options.use_organization_id
-@options.use_quiet_mode
-@options.use_cloud_provider_picker(
-    # prompt disabled, as only A8F works atm
-    optional=True,
-    default_value=CloudServiceProvider.AUTUMN8,
-)
-@click.option(
-    "-d",
-    "--deployment_id",
-    prompt=True,
-    help="ID of the deployment to terminate",
-)
+
+    require_ok_response(response)
+    return response.json()
+
+
 def terminate_deployment(
     organization_id: int,
-    deployment_id: str,
     environment: CliEnvironment,
-    cloud_provider: CloudServiceProvider,
-    quiet,
+    deployment_id: str,
+    service_provider: CloudServiceProvider,
 ):
-    """Terminate a running deployment."""
-    response = cloud.terminate_deployment(
-        organization_id, environment, deployment_id, cloud_provider
+    autodl_host = environment.value.app_host
+
+    params = {
+        "organization_id": organization_id,
+        "service_provider": service_provider.value,
+    }
+
+    deployments_api_route = (
+        f"{autodl_host}/api/cloud/deployments/{deployment_id}"
     )
-    click.echo(json.dumps(response, indent=4))
+    response = requests.delete(
+        url_with_params(deployments_api_route, params),
+        headers={"Content-Type": "application/json"},
+        auth=HTTPBasicAuth(*retrieve_api_creds()),
+        timeout=DEFAULT_API_TIMEOUT,
+    )
+
+    require_ok_response(response)
+    return response.json()
```

### Comparing `autumn8-1.0.3rc4/autumn8/cli/commands/models.py` & `autumn8-1.0.5rc1/autumn8/cli/commands/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,25 @@
 import time
 import uuid
 import zipfile
 from configparser import NoOptionError, NoSectionError
 from typing import List, Optional
 
 import click
-import jsonschema
 import questionary
-from jsonschema import validate
 
 from autumn8.cli import options
 from autumn8.cli.analyze import analyze_model_file, suggest_model_name
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.cli.examples import example_model_names
-from autumn8.cli.interactive import (
-    announce_model_upload_response,
-    normalize_args,
-)
+from autumn8.cli.interactive import announce_model_upload_response, normalize_args
+from autumn8.cli.validation import validate_input_dims_json, validate_input_file
 from autumn8.common.config.settings import supported_quants
-from autumn8.lib import api_creds, logging
+from autumn8.lib import api, api_creds, logging
 from autumn8.lib import service as autodl
-from autumn8.lib.api import lab
 
 USER_ID_LENGTH = len(str(uuid.uuid4()))
 API_KEY_LENGTH = 32
 
 logger = logging.getLogger(__name__)
 
 
@@ -79,60 +74,18 @@
             "API Key",
             validate=lambda api_key: len(api_key) == API_KEY_LENGTH,
         ).unsafe_ask()
     else:
         logger.info(f"API Key: {api_key}")
 
     api_creds.store_api_creds(user_id, api_key)
-    user_data = lab.fetch_user_data(environment)
+    user_data = api.user.fetch_user_data(environment)
     logger.info(f"Credentials set up successfully for {user_data['email']}!")
 
 
-INPUT_DIMS_JSONSCHEMA = {
-    "type": "array",
-    "minItems": 1,
-    "items": {
-        "type": "array",
-        "minItems": 1,
-        "items": {"type": "number"},
-    },
-}
-
-
-def validate_input_dims_json(jsonString):
-    if jsonString == "":
-        return True
-
-    try:
-        jsonData = json.loads(jsonString)
-        validate(instance=jsonData, schema=INPUT_DIMS_JSONSCHEMA)
-    except (
-        jsonschema.exceptions.ValidationError,
-        json.decoder.JSONDecodeError,
-    ):
-        return False
-    return True
-
-
-def validate_input_file(path):
-    if not os.path.exists(path):
-        return False
-
-    if not os.path.isfile(path):
-        return False
-
-    try:
-        with open(path, "r") as f:
-            jsonData = json.load(f)
-
-    except json.decoder.JSONDecodeError:
-        return False
-    return True
-
-
 def normalize_input_dims_for_api(input_dims):
     if not input_dims:
         return None
 
     inputs = json.loads(input_dims)
     inputs = [[str(dim) for dim in input] for input in inputs]
     return json.dumps(inputs, separators=(",", ":"))
@@ -502,15 +455,15 @@
     model_id: int,
     quiet: bool,
     **kwargs,
 ):
     """Get model data from AutoDL"""
     environment: CliEnvironment = kwargs["environment"]
 
-    model_info = lab.get_model(
+    model_info = api.lab.get_model(
         environment,
         organization_id,
         model_id,
     )
     announce_model_upload_response(model_info)
 
 
@@ -533,30 +486,30 @@
     quiet: bool,
     **kwargs,
 ):
     """Delete model from AutoDL"""
     environment: CliEnvironment = kwargs["environment"]
 
     if not auto_confirm:
-        model_info = lab.get_model(
+        model_info = api.lab.get_model(
             environment,
             organization_id,
             model_id,
         )
 
         logger.info("")
         logger.info("The details for your model are as follows:")
         click.echo(f"{json.dumps(model_info, indent=4)}")
         click.confirm(
             text="\n" + "Do you want to delete it?",
             abort=True,
             default=True,
         )
 
-    model_delete_response = lab.delete_model(
+    model_delete_response = api.lab.delete_model(
         environment,
         organization_id,
         model_id,
     )
     announce_model_upload_response(model_delete_response)
```

### Comparing `autumn8-1.0.3rc4/autumn8/cli/examples.py` & `autumn8-1.0.5rc1/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/cli/main.py` & `autumn8-1.0.5rc1/autumn8/cli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,34 +3,19 @@
 
 import click
 import questionary
 from questionary import Choice
 
 from autumn8.cli import options, pending_uploads
 from autumn8.cli.commands import cloud, models
-from autumn8.cli.interactive import (
-    announce_model_upload_response,
-    fetch_user_data,
-    normalize_args,
-)
+from autumn8.cli.interactive import announce_model_upload_response, normalize_args
 from autumn8.common._version import __version__
+from autumn8.lib import api
 from autumn8.lib.service import resume_upload_model
 
-# from autumn8.cli.cli_environment import CliEnvironment
-# from autumn8.common.config.s3 import init_s3_client
-
-# environment = CliEnvironment.STAGING
-# s3 = init_s3_client(environment.value.s3_host)
-# s3_bucket_name = environment.value.s3_bucket_name
-# mpus = s3.list_multipart_uploads(Bucket=s3_bucket_name, MaxUploads=200)
-
-# print("mpus", len(mpus["Uploads"]))
-# for mpu in mpus["Uploads"]:
-#     print(mpu["Key"])
-
 try:
     current_pending_uploads = pending_uploads.retrieve_pending_uploads()
 except (ValueError, AttributeError):
     # data format stored is incompatible with the current version
     # hope that the pending upload will get cleaned up by the S3 lifecycle policy
     # TODO: add the S3 lifecycle policy for that, lol - https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpu-abort-incomplete-mpu-lifecycle-config.html
     pending_uploads.forget_all_pending_uploads()
@@ -72,15 +57,15 @@
 
 @options.use_environment
 def test_connection(environment):
     """
     Test AutoDL connection with the current API key.
     Displays the user's email address upon successful connection.
     """
-    user_data = fetch_user_data(environment)
+    user_data = api.user.fetch_user_data(environment)
     print(f"Hello! You're authenticated as {user_data['email']}")
 
 
 @click.group(context_settings={"token_normalize_func": normalize_args})
 @click.version_option(version=__version__)
 def main():
     pass
```

### Comparing `autumn8-1.0.3rc4/autumn8/cli/options.py` & `autumn8-1.0.5rc1/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/cli/pending_uploads.py` & `autumn8-1.0.5rc1/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/common/config/cloud_info.py` & `autumn8-1.0.5rc1/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/common/config/settings.py` & `autumn8-1.0.5rc1/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/common/config/supported_instances.py` & `autumn8-1.0.5rc1/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/common/types.py` & `autumn8-1.0.5rc1/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/env/__init__.py` & `autumn8-1.0.5rc1/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/examples/mnist.py` & `autumn8-1.0.5rc1/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/examples/model.py` & `autumn8-1.0.5rc1/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.5rc1/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.5rc1/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/lib/__init__.py` & `autumn8-1.0.5rc1/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/lib/api/lab.py` & `autumn8-1.0.5rc1/autumn8/lib/api/lab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import io
 import json
-import os
-import urllib
-import urllib.parse
-from http import HTTPStatus
 from threading import Lock
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 import appdirs
 import boto3
 import httpx
 import requests
@@ -18,47 +14,26 @@
 from tqdm.contrib.concurrent import thread_map
 
 from autumn8.cli import pending_uploads
 from autumn8.cli.analyze import is_model_file_link_external, s3path_join
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.lib import logging
 from autumn8.lib.api_creds import retrieve_api_creds
+from autumn8.lib.http import require_ok_response, url_with_params
 
 DEFAULT_MAX_UPLOAD_WORKERS = 4
 
 APP_NAME = "autumn8"
 APP_AUTHOR = "autumn8"
 
 logger = logging.getLogger(__name__)
 
 data_dir = appdirs.user_data_dir(APP_NAME, APP_AUTHOR)
 
 
-def url_with_params(url: str, params: Dict[str, Union[str, int]]):
-    url_parse = urllib.parse.urlparse(url)
-    url_new_query = urllib.parse.urlencode(params)
-    url_parse = url_parse._replace(query=url_new_query)
-
-    new_url = urllib.parse.urlunparse(url_parse)
-    return new_url
-
-
-def require_ok_response(
-    response: Union[requests.Response, httpx.Response]
-) -> None:
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise Exception(
-            f"Received response {response.status_code}:\n{response.text}\n\nUser not authenticated; please run `autumn8-cli login` to authorize your CLI"
-        )
-    if response.status_code != HTTPStatus.OK:
-        raise Exception(
-            f"Received response {response.status_code}:\n{response.text}"
-        )
-
-
 def fetch_user_data(environment: CliEnvironment):
     user_id, api_key = None, None
     autodl_host = environment.value.app_host
     try:
         user_id, api_key = retrieve_api_creds()
     except:
         raise Exception(
```

### Comparing `autumn8-1.0.3rc4/autumn8/lib/api_creds.py` & `autumn8-1.0.5rc1/autumn8/lib/api_creds.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         app_config_dir = appdirs.user_config_dir(APP_NAME, APP_AUTHOR)
         app_config_path = os.path.join(app_config_dir, "autumn8.ini")
         config = configparser.ConfigParser()
         config.read(app_config_path)
         if not config.has_section("api_access"):
             config.add_section("api_access")
 
-        user_id = config.get("api_access", "user_id", fallback=None)
-        api_key = config.get("api_access", "api_key", fallback=None)
+        user_id = config.get("api_access", "user_id")
+        api_key = config.get("api_access", "api_key")
         return user_id, api_key
+    # TODO: pick a more specific set of exceptions here
     except Exception as exc:
         raise Exception(
             f"API key is missing! To configure API access, please visit your profile page and generate an API key, then run `autumn8-cli login`"
         ) from exc
```

### Comparing `autumn8-1.0.3rc4/autumn8/lib/logging.py` & `autumn8-1.0.5rc1/autumn8/lib/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # pyright: reportWildcardImportFromLibrary=false
 # pylint: disable=wildcard-import,unused-wildcard-import
 
 import logging
 import logging.config
 import os
 from logging import *
+from logging import Logger
 from logging import getLogger as oldGetLogger
 from typing import Optional
 
 import yaml
 
 with open(
     os.path.join(os.path.dirname(__file__), ".", "logging.yaml"),
```

### Comparing `autumn8-1.0.3rc4/autumn8/lib/logging.yaml` & `autumn8-1.0.5rc1/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/lib/package_resolver.py` & `autumn8-1.0.5rc1/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8/lib/service.py` & `autumn8-1.0.5rc1/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.5rc1/autumn8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.3rc4
+Version: 1.0.5rc1
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.3rc4/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.5rc1/autumn8.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 autumn8/cli/analyze.py
 autumn8/cli/cli_environment.py
 autumn8/cli/examples.py
 autumn8/cli/interactive.py
 autumn8/cli/main.py
 autumn8/cli/options.py
 autumn8/cli/pending_uploads.py
+autumn8/cli/validation.py
 autumn8/cli/commands/cloud.py
 autumn8/cli/commands/models.py
 autumn8/common/__init__.py
 autumn8/common/_version.py
 autumn8/common/types.py
 autumn8/common/config/__init__.py
 autumn8/common/config/cloud_info.py
@@ -35,16 +36,19 @@
 autumn8/examples/loadMnist.py
 autumn8/examples/mnist.py
 autumn8/examples/model.py
 autumn8/examples/sbert-alpha.py
 autumn8/examples/tensorflow_custom_layers.py
 autumn8/lib/__init__.py
 autumn8/lib/api_creds.py
+autumn8/lib/asyncio.py
+autumn8/lib/http.py
 autumn8/lib/logging.py
 autumn8/lib/logging.yaml
 autumn8/lib/package_resolver.py
 autumn8/lib/service.py
 autumn8/lib/api/__init__.py
 autumn8/lib/api/cloud.py
 autumn8/lib/api/lab.py
+autumn8/lib/api/user.py
 tests/test_io_bottleneck_detection.py
 tests/test_settings.py
```

### Comparing `autumn8-1.0.3rc4/pyproject.toml` & `autumn8-1.0.5rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.3rc4/tests/test_settings.py` & `autumn8-1.0.5rc1/tests/test_settings.py`

 * *Files identical despite different names*

