# Comparing `tmp/resotolib-3.4.1.tar.gz` & `tmp/resotolib-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.4.1.tar", last modified: Fri Apr 28 15:13:59 2023, max compression
+gzip compressed data, was "resotolib-3.4.2.tar", last modified: Wed May 10 12:25:37 2023, max compression
```

## Comparing `resotolib-3.4.1.tar` & `resotolib-3.4.2.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 15:10:57.000000 resotolib-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-28 15:13:59.747479 resotolib-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-28 15:10:57.000000 resotolib-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-28 15:10:57.000000 resotolib-3.4.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 15:10:57.000000 resotolib-3.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.739479 resotolib-3.4.1/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.739479 resotolib-3.4.1/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.739479 resotolib-3.4.1/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40989 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/log/logstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    22777 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.743479 resotolib-3.4.1/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-04-28 15:10:57.000000 resotolib-3.4.1/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.739479 resotolib-3.4.1/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 15:13:59.000000 resotolib-3.4.1/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 15:13:59.747479 resotolib-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-28 15:10:57.000000 resotolib-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/test/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/asynchronous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/test/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/asynchronous/web/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:13:59.747479 resotolib-3.4.1/test/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/custom_command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/model_check_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/model_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/progress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/core/tasks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/durations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/json_bender_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/parse_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-28 15:10:57.000000 resotolib-3.4.1/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 12:22:37.000000 resotolib-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-10 12:25:37.406532 resotolib-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-10 12:22:37.000000 resotolib-3.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 12:22:37.000000 resotolib-3.4.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-10 12:22:37.000000 resotolib-3.4.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40989 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.402532 resotolib-3.4.2/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.402532 resotolib-3.4.2/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/log/logstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22777 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.402532 resotolib-3.4.2/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.402532 resotolib-3.4.2/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-10 12:25:37.406532 resotolib-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 12:22:37.000000 resotolib-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/test/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/asynchronous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/test/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/asynchronous/web/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/custom_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/model_check_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/model_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/progress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/tasks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/durations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/json_bender_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/parse_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_x509.py
```

### Comparing `resotolib-3.4.1/PKG-INFO` & `resotolib-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.4.1
+Version: 3.4.2
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotolib-3.4.1/README.md` & `resotolib-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/args.py` & `resotolib-3.4.2/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/asynchronous/periodic.py` & `resotolib-3.4.2/resotolib/asynchronous/periodic.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/asynchronous/web/auth.py` & `resotolib-3.4.2/resotolib/asynchronous/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/asynchronous/web/runner.py` & `resotolib-3.4.2/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.4.2/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/baseplugin.py` & `resotolib-3.4.2/resotolib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/baseresources.py` & `resotolib-3.4.2/resotolib/baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/config.py` & `resotolib-3.4.2/resotolib/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/__init__.py` & `resotolib-3.4.2/resotolib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/actions.py` & `resotolib-3.4.2/resotolib/core/actions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/ca.py` & `resotolib-3.4.2/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/config.py` & `resotolib-3.4.2/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/custom_command.py` & `resotolib-3.4.2/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/events.py` & `resotolib-3.4.2/resotolib/core/events.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/model_check.py` & `resotolib-3.4.2/resotolib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/model_export.py` & `resotolib-3.4.2/resotolib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/progress.py` & `resotolib-3.4.2/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/core/search.py` & `resotolib-3.4.2/resotolib/core/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,23 @@
         headers = {"Accept": "application/x-ndjson", "Content-Type": "text/plain"}
         execute_endpoint = f"{self.base_uri}/cli/execute"
         if self.graph_name:
             query_string = urlencode({"graph": self.graph_name})
             execute_endpoint += f"?{query_string}"
         return self.post(execute_endpoint, command, headers, verify=self.verify)
 
-    def search(self, search: str, edge_type: Optional[EdgeType] = None) -> Iterator[Json]:
+    def search(self, search: str, edge_type: Optional[EdgeType] = None, section: str = "reported") -> Iterator[Json]:
         log.debug(f"Sending search {search}")
         headers = {"Accept": "application/x-ndjson"}
         search_endpoint = self.search_uri
+        query = {"section": section}
         if edge_type is not None:
-            query_string = urlencode({"edge_type": edge_type.value})
-            search_endpoint += f"?{query_string}"
+            query["edge_type"] = edge_type.value
+        query_string = urlencode(query)
+        search_endpoint += f"?{query_string}"
         return self.post(search_endpoint, search, headers, verify=self.verify)
 
     @staticmethod
     def post(uri: str, data: str, headers: Dict[str, str], verify: Optional[str] = None) -> Iterator[Json]:
         if getattr(ArgumentParser.args, "psk", None):
             encode_jwt_to_headers(headers, {}, ArgumentParser.args.psk)
         r = requests.post(uri, data=data, headers=headers, stream=True, verify=verify)
```

### Comparing `resotolib-3.4.1/resotolib/core/tasks.py` & `resotolib-3.4.2/resotolib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/durations.py` & `resotolib-3.4.2/resotolib/durations.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,21 @@
 duration_parser = single_duration_parser.sep_by(time_unit_combination.optional(), min=1).map(combine_durations)
 
 
 def parse_duration(ds: str) -> timedelta:
     return timedelta(seconds=duration_parser.parse(ds))
 
 
+def parse_optional_duration(ds: str) -> Optional[timedelta]:
+    try:
+        return parse_duration(ds)
+    except Exception:
+        return None
+
+
 def duration_str(duration: timedelta, precision: Optional[int] = 0, down_to_unit: Optional[str] = None) -> str:
     """
     Convert a timedelta to a string representing the duration human-readable short unit syntax.
     Examples: 3d2h, 2min42s
     :param duration: the duration to convert
     :param precision: the number of units to use to represent the duration.
     :param down_to_unit: use all units starting from the biggest one until the given unit.
```

### Comparing `resotolib-3.4.1/resotolib/event.py` & `resotolib-3.4.2/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/graph/__init__.py` & `resotolib-3.4.2/resotolib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/graph/graph_extensions.py` & `resotolib-3.4.2/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/json.py` & `resotolib-3.4.2/resotolib/json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/json_bender.py` & `resotolib-3.4.2/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/lock.py` & `resotolib-3.4.2/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/log/logstream.py` & `resotolib-3.4.2/resotolib/log/logstream.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/logger.py` & `resotolib-3.4.2/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/parse_util.py` & `resotolib-3.4.2/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/proc.py` & `resotolib-3.4.2/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/tree.py` & `resotolib-3.4.2/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/utils.py` & `resotolib-3.4.2/resotolib/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/__init__.py` & `resotolib-3.4.2/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/metrics.py` & `resotolib-3.4.2/resotolib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.4.2/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.4.2/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.4.2/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/static/favicon-16x16.png` & `resotolib-3.4.2/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/static/favicon-32x32.png` & `resotolib-3.4.2/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/static/index.html` & `resotolib-3.4.2/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/static/mstile-150x150.png` & `resotolib-3.4.2/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/web/static/picnic.min.css` & `resotolib-3.4.2/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/resotolib/x509.py` & `resotolib-3.4.2/resotolib/x509.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import base64
 import certifi
 from ipaddress import (
     ip_address,
     ip_network,
     IPv4Address,
     IPv6Address,
     IPv4Network,
@@ -14,19 +15,22 @@
 from resotolib.utils import get_local_hostnames, get_local_ip_addresses
 from datetime import datetime, timedelta, timezone
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
+from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives.asymmetric.rsa import (
     RSAPrivateKey,
+    RSAPublicKey,
     generate_private_key,
 )
 from cryptography.x509.base import Certificate, CertificateSigningRequest
+from cryptography.exceptions import InvalidSignature
 from typing import List, Optional, Tuple, Union, Dict, Any
 
 
 def gen_rsa_key(key_size: int = 2048) -> RSAPrivateKey:
     return generate_private_key(public_exponent=65537, key_size=key_size, backend=default_backend())
 
 
@@ -277,7 +281,40 @@
         return ip_network(ip)
     else:
         return ip_address(ip)
 
 
 def cert_fingerprint(cert: Certificate, hash_algorithm: str = "SHA256") -> str:
     return ":".join(f"{b:02X}" for b in cert.fingerprint(getattr(hashes, hash_algorithm.upper())()))
+
+
+def cert_is_signed_by_ca(cert: Certificate, ca_cert: Certificate) -> bool:
+    try:
+        public_key = ca_cert.public_key()
+        signature_hash_algorithm = cert.signature_hash_algorithm
+        assert isinstance(public_key, RSAPublicKey)
+        assert isinstance(signature_hash_algorithm, hashes.HashAlgorithm)
+        public_key.verify(
+            cert.signature,
+            cert.tbs_certificate_bytes,
+            padding.PKCS1v15(),
+            signature_hash_algorithm,
+        )
+        return True
+    except InvalidSignature:
+        return False
+
+
+def x5t_any(cert: Certificate, hash_algorithm: str) -> str:
+    public_bytes = cert.public_bytes(serialization.Encoding.DER)
+    hash_instance = hashes.Hash(getattr(hashes, hash_algorithm.upper())(), default_backend())
+    hash_instance.update(public_bytes)
+    thumbprint = hash_instance.finalize()
+    return base64.urlsafe_b64encode(thumbprint).rstrip(b"=").decode("utf-8")
+
+
+def x5t(cert: Certificate) -> str:
+    return x5t_any(cert, "SHA1")
+
+
+def x5t_s256(cert: Certificate) -> str:
+    return x5t_any(cert, "SHA256")
```

### Comparing `resotolib-3.4.1/resotolib.egg-info/PKG-INFO` & `resotolib-3.4.2/resotolib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.4.1
+Version: 3.4.2
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotolib-3.4.1/resotolib.egg-info/SOURCES.txt` & `resotolib-3.4.2/resotolib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 resotolib.egg-info/SOURCES.txt
 resotolib.egg-info/dependency_links.txt
 resotolib.egg-info/not-zip-safe
 resotolib.egg-info/requires.txt
 resotolib.egg-info/top_level.txt
 resotolib/asynchronous/__init__.py
 resotolib/asynchronous/periodic.py
+resotolib/asynchronous/utils.py
 resotolib/asynchronous/web/__init__.py
 resotolib/asynchronous/web/auth.py
 resotolib/asynchronous/web/runner.py
 resotolib/asynchronous/web/ws_handler.py
 resotolib/core/__init__.py
 resotolib/core/actions.py
 resotolib/core/ca.py
```

### Comparing `resotolib-3.4.1/setup.py` & `resotolib-3.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/asynchronous/web/test_auth.py` & `resotolib-3.4.2/test/asynchronous/web/test_auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/core/custom_command_test.py` & `resotolib-3.4.2/test/core/custom_command_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/core/model_check_test.py` & `resotolib-3.4.2/test/core/model_check_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/core/model_export_test.py` & `resotolib-3.4.2/test/core/model_export_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/core/progress_test.py` & `resotolib-3.4.2/test/core/progress_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/core/tasks_test.py` & `resotolib-3.4.2/test/core/tasks_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/durations_test.py` & `resotolib-3.4.2/test/durations_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/json_bender_test.py` & `resotolib-3.4.2/test/json_bender_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/parse_util_test.py` & `resotolib-3.4.2/test/parse_util_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_args.py` & `resotolib-3.4.2/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_baseresources.py` & `resotolib-3.4.2/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_config.py` & `resotolib-3.4.2/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_graph.py` & `resotolib-3.4.2/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_graph_extensions.py` & `resotolib-3.4.2/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_json.py` & `resotolib-3.4.2/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_jwt.py` & `resotolib-3.4.2/test/test_jwt.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,27 @@
     encode_jwt_to_headers,
 )
 from jwt import (
     InvalidSignatureError,
     ExpiredSignatureError,
     ImmatureSignatureError,
     MissingRequiredClaimError,
+    get_unverified_header,
+)
+from resotolib.x509 import (
+    bootstrap_ca,
+    gen_rsa_key,
+    gen_csr,
+    sign_csr,
+    cert_is_signed_by_ca,
+    x5t_s256,
 )
 
 
-def test_jwt():
+def test_jwt_psk():
     psk = "somesecret"
     payload = {"Hello": "World"}
     j1 = encode_jwt(payload, psk, expire_in=-1)
     j2 = encode_jwt(payload, psk, expire_in=-1)
     past_date = datetime.datetime.now() - datetime.timedelta(30)
     future_date = datetime.datetime.now() + datetime.timedelta(30)
 
@@ -48,7 +57,21 @@
     assert decode_jwt(valid_jwt, psk).get("Hello") == "World"
     with pytest.raises(ImmatureSignatureError) as e:
         decode_jwt(not_yet_valid_jwt, psk)
     assert str(e.value).startswith("The token is not yet valid")
     with pytest.raises(MissingRequiredClaimError) as e:
         decode_jwt(j1, psk, options={"require": ["exp"]})
     assert str(e.value) == 'Token is missing the "exp" claim'
+
+
+def test_jwt_pki():
+    ca_key, ca_cert = bootstrap_ca()
+    cert_key = gen_rsa_key()
+    cert_crt = sign_csr(gen_csr(cert_key), ca_key, ca_cert)
+    payload = {"Hello": "World"}
+    jwt = encode_jwt(payload, cert_key, expire_in=-1)
+    assert cert_is_signed_by_ca(cert_crt, ca_cert)
+    assert decode_jwt(jwt, cert_crt) == payload
+
+    jwt = encode_jwt(payload, cert_key, cert=cert_crt)
+    assert decode_jwt(jwt, cert_crt).get("Hello") == "World"
+    assert get_unverified_header(jwt).get("x5t#S256") == x5t_s256(cert_crt)
```

### Comparing `resotolib-3.4.1/test/test_plugin.py` & `resotolib-3.4.2/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_tree.py` & `resotolib-3.4.2/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_utils.py` & `resotolib-3.4.2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_web.py` & `resotolib-3.4.2/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.1/test/test_x509.py` & `resotolib-3.4.2/test/test_x509.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     write_cert_to_file,
     write_key_to_file,
     load_csr_from_file,
     load_cert_from_file,
     load_key_from_file,
     key_to_bytes,
     cert_fingerprint,
+    cert_is_signed_by_ca,
 )
 
 
 def test_x509():
     with tempfile.TemporaryDirectory() as tmp:
         ca_key, ca_cert = bootstrap_ca()
         cert_key = gen_rsa_key()
@@ -51,7 +52,8 @@
         assert loaded_ca_cert == ca_cert
         assert loaded_cert_csr == cert_csr
         assert loaded_cert_crt == cert_crt
         assert cert_fingerprint(loaded_ca_cert) == cert_fingerprint(ca_cert)
         assert cert_fingerprint(loaded_cert_crt) == cert_fingerprint(cert_crt)
         assert key_to_bytes(ca_key) == key_to_bytes(loaded_ca_key)
         assert key_to_bytes(cert_key) == key_to_bytes(loaded_cert_key)
+        assert cert_is_signed_by_ca(cert_crt, ca_cert)
```

