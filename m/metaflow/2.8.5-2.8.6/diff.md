# Comparing `tmp/metaflow-2.8.5.tar.gz` & `tmp/metaflow-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-2.8.5.tar", last modified: Sat May  6 00:04:29 2023, max compression
+gzip compressed data, was "metaflow-2.8.6.tar", last modified: Wed May 10 18:50:40 2023, max compression
```

## Comparing `metaflow-2.8.5.tar` & `metaflow-2.8.6.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-06 00:04:13.000000 metaflow-2.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 00:04:13.000000 metaflow-2.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-06 00:04:29.575784 metaflow-2.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-06 00:04:13.000000 metaflow-2.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.551784 metaflow-2.8.5/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.551784 metaflow-2.8.5/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.555784 metaflow-2.8.5/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.555784 metaflow-2.8.5/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.555784 metaflow-2.8.5/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.555784 metaflow-2.8.5/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.555784 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.555784 metaflow-2.8.5/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69157 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.555784 metaflow-2.8.5/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31165 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.555784 metaflow-2.8.5/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.559784 metaflow-2.8.5/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.559784 metaflow-2.8.5/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.559784 metaflow-2.8.5/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.559784 metaflow-2.8.5/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.559784 metaflow-2.8.5/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31282 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.559784 metaflow-2.8.5/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.559784 metaflow-2.8.5/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.559784 metaflow-2.8.5/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    96242 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.563784 metaflow-2.8.5/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.563784 metaflow-2.8.5/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.563784 metaflow-2.8.5/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.563784 metaflow-2.8.5/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.563784 metaflow-2.8.5/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.563784 metaflow-2.8.5/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.567784 metaflow-2.8.5/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.567784 metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.567784 metaflow-2.8.5/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.567784 metaflow-2.8.5/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.567784 metaflow-2.8.5/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.567784 metaflow-2.8.5/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13314 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26188 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.571784 metaflow-2.8.5/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.547784 metaflow-2.8.5/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.575784 metaflow-2.8.5/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-06 00:04:13.000000 metaflow-2.8.5/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:04:29.551784 metaflow-2.8.5/metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-06 00:04:29.000000 metaflow-2.8.5/metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-06 00:04:29.000000 metaflow-2.8.5/metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:04:29.000000 metaflow-2.8.5/metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 00:04:29.000000 metaflow-2.8.5/metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 00:04:29.000000 metaflow-2.8.5/metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 00:04:29.000000 metaflow-2.8.5/metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-06 00:04:29.575784 metaflow-2.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-06 00:04:13.000000 metaflow-2.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-10 18:50:27.000000 metaflow-2.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 18:50:27.000000 metaflow-2.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-10 18:50:40.921571 metaflow-2.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-10 18:50:27.000000 metaflow-2.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.869568 metaflow-2.8.6/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.873568 metaflow-2.8.6/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.873568 metaflow-2.8.6/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.877569 metaflow-2.8.6/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.877569 metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.877569 metaflow-2.8.6/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.877569 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69157 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31165 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.885569 metaflow-2.8.6/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.889569 metaflow-2.8.6/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97596 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.897570 metaflow-2.8.6/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.897570 metaflow-2.8.6/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.897570 metaflow-2.8.6/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.901570 metaflow-2.8.6/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.901570 metaflow-2.8.6/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.909571 metaflow-2.8.6/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.909571 metaflow-2.8.6/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19778 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27804 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.857568 metaflow-2.8.6/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.873568 metaflow-2.8.6/metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 18:50:40.921571 metaflow-2.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-10 18:50:27.000000 metaflow-2.8.6/setup.py
```

### Comparing `metaflow-2.8.5/LICENSE` & `metaflow-2.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/PKG-INFO` & `metaflow-2.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.8.5
+Version: 2.8.6
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.8.5/README.md` & `metaflow-2.8.6/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/__init__.py` & `metaflow-2.8.6/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/__init__.py` & `metaflow-2.8.6/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/_bashcomplete.py` & `metaflow-2.8.6/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/_compat.py` & `metaflow-2.8.6/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/_termui_impl.py` & `metaflow-2.8.6/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/_textwrap.py` & `metaflow-2.8.6/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/_unicodefun.py` & `metaflow-2.8.6/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/_winconsole.py` & `metaflow-2.8.6/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/core.py` & `metaflow-2.8.6/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/decorators.py` & `metaflow-2.8.6/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/exceptions.py` & `metaflow-2.8.6/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/formatting.py` & `metaflow-2.8.6/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/globals.py` & `metaflow-2.8.6/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/parser.py` & `metaflow-2.8.6/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/termui.py` & `metaflow-2.8.6/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/testing.py` & `metaflow-2.8.6/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/types.py` & `metaflow-2.8.6/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/click/utils.py` & `metaflow-2.8.6/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_5/zipp.py` & `metaflow-2.8.6/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/typing_extensions.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/_vendor/v3_6/zipp.py` & `metaflow-2.8.6/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/cli.py` & `metaflow-2.8.6/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/cli_args.py` & `metaflow-2.8.6/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/client/core.py` & `metaflow-2.8.6/metaflow/client/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/client/filecache.py` & `metaflow-2.8.6/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/cmd/configure_cmd.py` & `metaflow-2.8.6/metaflow/cmd/configure_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/cmd/main_cli.py` & `metaflow-2.8.6/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/cmd/tutorials_cmd.py` & `metaflow-2.8.6/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/cmd_with_io.py` & `metaflow-2.8.6/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/current.py` & `metaflow-2.8.6/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/datastore/content_addressed_store.py` & `metaflow-2.8.6/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/datastore/datastore_set.py` & `metaflow-2.8.6/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/datastore/datastore_storage.py` & `metaflow-2.8.6/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/datastore/flow_datastore.py` & `metaflow-2.8.6/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/datastore/task_datastore.py` & `metaflow-2.8.6/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/debug.py` & `metaflow-2.8.6/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/decorators.py` & `metaflow-2.8.6/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/event_logger.py` & `metaflow-2.8.6/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/events.py` & `metaflow-2.8.6/metaflow/events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/exception.py` & `metaflow-2.8.6/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/extension_support/__init__.py` & `metaflow-2.8.6/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/extension_support/cmd.py` & `metaflow-2.8.6/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/extension_support/integrations.py` & `metaflow-2.8.6/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/extension_support/plugins.py` & `metaflow-2.8.6/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/flowspec.py` & `metaflow-2.8.6/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/graph.py` & `metaflow-2.8.6/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/includefile.py` & `metaflow-2.8.6/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/integrations.py` & `metaflow-2.8.6/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/lint.py` & `metaflow-2.8.6/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/metadata/heartbeat.py` & `metaflow-2.8.6/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/metadata/metadata.py` & `metaflow-2.8.6/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/metadata/util.py` & `metaflow-2.8.6/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/metaflow_config.py` & `metaflow-2.8.6/metaflow/metaflow_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 DEFAULT_EVENT_LOGGER = from_conf("DEFAULT_EVENT_LOGGER", "nullSidecarLogger")
 DEFAULT_METADATA = from_conf("DEFAULT_METADATA", "local")
 DEFAULT_MONITOR = from_conf("DEFAULT_MONITOR", "nullSidecarMonitor")
 DEFAULT_PACKAGE_SUFFIXES = from_conf("DEFAULT_PACKAGE_SUFFIXES", ".py,.R,.RDS")
 DEFAULT_AWS_CLIENT_PROVIDER = from_conf("DEFAULT_AWS_CLIENT_PROVIDER", "boto3")
 DEFAULT_SECRETS_BACKEND_TYPE = from_conf("DEFAULT_SECRETS_BACKEND_TYPE")
 
+###
+# User configuration
+###
+USER = from_conf("USER")
+
 
 ###
 # Datastore configuration
 ###
 # Path to the local directory to store artifacts for 'local' datastore.
 DATASTORE_LOCAL_DIR = ".metaflow"
 DATASTORE_SYSROOT_LOCAL = from_conf("DATASTORE_SYSROOT_LOCAL")
@@ -264,14 +269,17 @@
 # Kubernetes namespace to use for all objects created by Metaflow
 KUBERNETES_NAMESPACE = from_conf("KUBERNETES_NAMESPACE", "default")
 # Default service account to use by K8S jobs created by Metaflow
 KUBERNETES_SERVICE_ACCOUNT = from_conf("KUBERNETES_SERVICE_ACCOUNT")
 # Default node selectors to use by K8S jobs created by Metaflow - foo=bar,baz=bab
 KUBERNETES_NODE_SELECTOR = from_conf("KUBERNETES_NODE_SELECTOR", "")
 KUBERNETES_TOLERATIONS = from_conf("KUBERNETES_TOLERATIONS", "")
+KUBERNETES_PERSISTENT_VOLUME_CLAIMS = from_conf(
+    "KUBERNETES_PERSISTENT_VOLUME_CLAIMS", ""
+)
 KUBERNETES_SECRETS = from_conf("KUBERNETES_SECRETS", "")
 # Default GPU vendor to use by K8S jobs created by Metaflow (supports nvidia, amd)
 KUBERNETES_GPU_VENDOR = from_conf("KUBERNETES_GPU_VENDOR", "nvidia")
 # Default container image for K8S
 KUBERNETES_CONTAINER_IMAGE = from_conf(
     "KUBERNETES_CONTAINER_IMAGE", DEFAULT_CONTAINER_IMAGE
 )
```

### Comparing `metaflow-2.8.5/metaflow/metaflow_config_funcs.py` & `metaflow-2.8.6/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/metaflow_environment.py` & `metaflow-2.8.6/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/metaflow_version.py` & `metaflow-2.8.6/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/mflog/__init__.py` & `metaflow-2.8.6/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/mflog/mflog.py` & `metaflow-2.8.6/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/mflog/save_logs.py` & `metaflow-2.8.6/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/mflog/save_logs_periodically.py` & `metaflow-2.8.6/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/mflog/tee.py` & `metaflow-2.8.6/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/monitor.py` & `metaflow-2.8.6/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/multicore_utils.py` & `metaflow-2.8.6/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/package.py` & `metaflow-2.8.6/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/parameters.py` & `metaflow-2.8.6/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/__init__.py` & `metaflow-2.8.6/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/airflow/airflow.py` & `metaflow-2.8.6/metaflow/plugins/airflow/airflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,15 +638,15 @@
             kube_deco = dict(
                 [deco for deco in node.decorators if deco.name == "kubernetes"][
                     0
                 ].attributes
             )
             if kube_deco:
                 # Only guard against use_tmpfs and tmpfs_size as these determine if tmpfs is enabled.
-                for attr in ["use_tmpfs", "tmpfs_size"]:
+                for attr in ["use_tmpfs", "tmpfs_size", "persistent_volume_claims"]:
                     if kube_deco[attr]:
                         raise AirflowException(
                             "tmpfs attribute *%s* is currently not supported on Airflow "
                             "for the @kubernetes decorator on step *%s*"
                             % (attr, node.name)
                         )
```

### Comparing `metaflow-2.8.5/metaflow/plugins/airflow/airflow_cli.py` & `metaflow-2.8.6/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/airflow/airflow_decorator.py` & `metaflow-2.8.6/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/airflow/airflow_utils.py` & `metaflow-2.8.6/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/airflow/plumbing/set_parameters.py` & `metaflow-2.8.6/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/airflow/sensors/base_sensor.py` & `metaflow-2.8.6/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `metaflow-2.8.6/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/airflow/sensors/s3_sensor.py` & `metaflow-2.8.6/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/argo/argo_client.py` & `metaflow-2.8.6/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/argo/argo_events.py` & `metaflow-2.8.6/metaflow/plugins/argo/argo_events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/argo/argo_workflows.py` & `metaflow-2.8.6/metaflow/plugins/argo/argo_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -845,15 +845,15 @@
                 "--metadata=%s" % self.metadata.TYPE,
                 "--environment=%s" % self.environment.TYPE,
                 "--datastore=%s" % self.flow_datastore.TYPE,
                 "--datastore-root=%s" % self.flow_datastore.datastore_root,
                 "--event-logger=%s" % self.event_logger.TYPE,
                 "--monitor=%s" % self.monitor.TYPE,
                 "--no-pylint",
-                "--with=argo_workflows_internal:auto-emit-argo-events=%s"
+                "--with=argo_workflows_internal:auto-emit-argo-events=%i"
                 % self.auto_emit_argo_events,
             ]
 
             if node.name == "start":
                 # Execute `init` before any step of the workflow executes
                 task_id_params = "%s-params" % task_id
                 init = (
@@ -1116,14 +1116,15 @@
                 .empty_dir_volume("out")
                 # Set tmpfs emptyDir volume if enabled
                 .empty_dir_volume(
                     "tmpfs-ephemeral-volume",
                     medium="Memory",
                     size_limit=tmpfs_size if tmpfs_enabled else 0,
                 )
+                .pvc_volumes(resources.get("persistent_volume_claims"))
                 # Set node selectors
                 .node_selectors(resources.get("node_selector"))
                 .tolerations(resources.get("tolerations"))
                 # Set container
                 .container(
                     # TODO: Unify the logic with kubernetes.py
                     # Important note - Unfortunately, V1Container uses snakecase while
@@ -1204,14 +1205,26 @@
                                     kubernetes_sdk.V1VolumeMount(
                                         name="tmpfs-ephemeral-volume",
                                         mount_path=tmpfs_path,
                                     )
                                 ]
                                 if tmpfs_enabled
                                 else []
+                            )
+                            + (
+                                [
+                                    kubernetes_sdk.V1VolumeMount(
+                                        name=claim, mount_path=path
+                                    )
+                                    for claim, path in resources.get(
+                                        "persistent_volume_claims"
+                                    ).items()
+                                ]
+                                if resources.get("persistent_volume_claims") is not None
+                                else []
                             ),
                         ).to_dict()
                     )
                 )
             )
 
     def _compile_sensor(self):
@@ -1834,14 +1847,34 @@
                     **({"sizeLimit": "{}Mi".format(size_limit)} if size_limit else {}),
                     **({"medium": medium} if medium else {}),
                 },
             }
         )
         return self
 
+    def pvc_volumes(self, pvcs=None):
+        """
+        Create and attach Persistent Volume Claims as volumes.
+
+        Parameters:
+        -----------
+        pvcs: Optional[Dict]
+            a dictionary of pvc's and the paths they should be mounted to. e.g.
+            {"pv-claim-1": "/mnt/path1", "pv-claim-2": "/mnt/path2"}
+        """
+        if pvcs is None:
+            return self
+        if "volumes" not in self.payload:
+            self.payload["volumes"] = []
+        for claim in pvcs.keys():
+            self.payload["volumes"].append(
+                {"name": claim, "persistentVolumeClaim": {"claimName": claim}}
+            )
+        return self
+
     def node_selectors(self, node_selectors):
         if "nodeSelector" not in self.payload:
             self.payload["nodeSelector"] = {}
         if node_selectors:
             self.payload["nodeSelector"].update(node_selectors)
         return self
```

### Comparing `metaflow-2.8.5/metaflow/plugins/argo/argo_workflows_cli.py` & `metaflow-2.8.6/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/argo/argo_workflows_decorator.py` & `metaflow-2.8.6/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/argo/process_input_paths.py` & `metaflow-2.8.6/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/aws_client.py` & `metaflow-2.8.6/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/aws_utils.py` & `metaflow-2.8.6/metaflow/plugins/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/batch/batch.py` & `metaflow-2.8.6/metaflow/plugins/aws/batch/batch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/batch/batch_cli.py` & `metaflow-2.8.6/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/batch/batch_client.py` & `metaflow-2.8.6/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/batch/batch_decorator.py` & `metaflow-2.8.6/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `metaflow-2.8.6/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/production_token.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/step_functions.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/step_functions_client.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/azure/azure_tail.py` & `metaflow-2.8.6/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/azure/azure_utils.py` & `metaflow-2.8.6/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/azure/blob_service_client_factory.py` & `metaflow-2.8.6/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/azure/includefile_support.py` & `metaflow-2.8.6/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_cli.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_client.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_datastore.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_decorator.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/__init__.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/base.html` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/basic.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/bundle.css` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/card.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/main.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/components.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/main.js` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/renderer_tools.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_modules/test_cards.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/card_resolver.py` & `metaflow-2.8.6/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/component_serializer.py` & `metaflow-2.8.6/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/cards/exception.py` & `metaflow-2.8.6/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/catch_decorator.py` & `metaflow-2.8.6/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/conda/__init__.py` & `metaflow-2.8.6/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/conda/batch_bootstrap.py` & `metaflow-2.8.6/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/conda/conda.py` & `metaflow-2.8.6/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/conda/conda_environment.py` & `metaflow-2.8.6/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/conda/conda_flow_decorator.py` & `metaflow-2.8.6/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/conda/conda_step_decorator.py` & `metaflow-2.8.6/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datastores/azure_storage.py` & `metaflow-2.8.6/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datastores/gs_storage.py` & `metaflow-2.8.6/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datastores/local_storage.py` & `metaflow-2.8.6/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datastores/s3_storage.py` & `metaflow-2.8.6/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datatools/__init__.py` & `metaflow-2.8.6/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datatools/local.py` & `metaflow-2.8.6/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datatools/s3/s3.py` & `metaflow-2.8.6/metaflow/plugins/datatools/s3/s3.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datatools/s3/s3op.py` & `metaflow-2.8.6/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datatools/s3/s3tail.py` & `metaflow-2.8.6/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/datatools/s3/s3util.py` & `metaflow-2.8.6/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/debug_logger.py` & `metaflow-2.8.6/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/debug_monitor.py` & `metaflow-2.8.6/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/__init__.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/client.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/client_modules.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/communication/bytestream.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/communication/channel.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/communication/utils.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/consts.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/data_transferer.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/exception_transferer.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/override_decorators.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/server.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/stub.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/env_escape/utils.py` & `metaflow-2.8.6/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/environment_decorator.py` & `metaflow-2.8.6/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/events_decorator.py` & `metaflow-2.8.6/metaflow/plugins/events_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/frameworks/pytorch.py` & `metaflow-2.8.6/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/gcp/gs_storage_client_factory.py` & `metaflow-2.8.6/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/gcp/gs_tail.py` & `metaflow-2.8.6/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/gcp/gs_utils.py` & `metaflow-2.8.6/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/gcp/includefile_support.py` & `metaflow-2.8.6/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes.py` & `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         memory=None,
         use_tmpfs=None,
         tmpfs_tempdir=None,
         tmpfs_size=None,
         tmpfs_path=None,
         run_time_limit=None,
         env=None,
+        persistent_volume_claims=None,
         tolerations=None,
     ):
         if env is None:
             env = {}
 
         job = (
             KubernetesClient()
@@ -189,14 +190,15 @@
                 retries=0,
                 step_name=step_name,
                 tolerations=tolerations,
                 use_tmpfs=use_tmpfs,
                 tmpfs_tempdir=tmpfs_tempdir,
                 tmpfs_size=tmpfs_size,
                 tmpfs_path=tmpfs_path,
+                persistent_volume_claims=persistent_volume_claims,
             )
             .environment_variable("METAFLOW_CODE_SHA", code_package_sha)
             .environment_variable("METAFLOW_CODE_URL", code_package_url)
             .environment_variable("METAFLOW_CODE_DS", code_package_ds)
             .environment_variable("METAFLOW_USER", user)
             .environment_variable("METAFLOW_SERVICE_URL", SERVICE_INTERNAL_URL)
             .environment_variable(
```

### Comparing `metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes_cli.py` & `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,17 @@
 @click.option("--tmpfs-path", help="tmpfs requirement for Kubernetes pod.")
 @click.option(
     "--run-time-limit",
     default=5 * 24 * 60 * 60,  # Default is set to 5 days
     help="Run time limit in seconds for Kubernetes pod.",
 )
 @click.option(
+    "--persistent-volume-claims", type=JSONTypeClass(), default=None, multiple=False
+)
+@click.option(
     "--tolerations",
     default=None,
     type=JSONTypeClass(),
     multiple=False,
 )
 @click.pass_context
 def step(
@@ -115,14 +118,15 @@
     gpu=None,
     gpu_vendor=None,
     use_tmpfs=None,
     tmpfs_tempdir=None,
     tmpfs_size=None,
     tmpfs_path=None,
     run_time_limit=None,
+    persistent_volume_claims=None,
     tolerations=None,
     **kwargs
 ):
     def echo(msg, stream="stderr", job_id=None, **kwargs):
         msg = util.to_unicode(msg)
         if job_id:
             msg = "[%s] %s" % (job_id, msg)
@@ -227,14 +231,15 @@
                 gpu_vendor=gpu_vendor,
                 use_tmpfs=use_tmpfs,
                 tmpfs_tempdir=tmpfs_tempdir,
                 tmpfs_size=tmpfs_size,
                 tmpfs_path=tmpfs_path,
                 run_time_limit=run_time_limit,
                 env=env,
+                persistent_volume_claims=persistent_volume_claims,
                 tolerations=tolerations,
             )
     except Exception as e:
         traceback.print_exc(chain=False)
         _sync_metadata()
         sys.exit(METAFLOW_EXIT_DISALLOW_RETRY)
     try:
```

### Comparing `metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes_client.py` & `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     KUBERNETES_GPU_VENDOR,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
     KUBERNETES_TOLERATIONS,
     KUBERNETES_SERVICE_ACCOUNT,
     KUBERNETES_SECRETS,
     KUBERNETES_FETCH_EC2_METADATA,
+    KUBERNETES_PERSISTENT_VOLUME_CLAIMS,
 )
 from metaflow.plugins.resources_decorator import ResourcesDecorator
 from metaflow.plugins.timeout_decorator import get_run_time_limit_for_task
 from metaflow.sidecar import Sidecar
 
 from ..aws.aws_utils import get_docker_registry, get_ec2_instance_metadata
 
@@ -92,14 +93,15 @@
         "gpu_vendor": None,
         "tolerations": None,  # e.g., [{"key": "arch", "operator": "Equal", "value": "amd"},
         #                              {"key": "foo", "operator": "Equal", "value": "bar"}]
         "use_tmpfs": None,
         "tmpfs_tempdir": True,
         "tmpfs_size": None,
         "tmpfs_path": "/metaflow_temp",
+        "persistent_volume_claims": None,  # e.g., {"pvc-name": "/mnt/vol", "another-pvc": "/mnt/vol2"}
     }
     package_url = None
     package_sha = None
     run_time_limit = None
 
     def __init__(self, attributes=None, statically_defined=False):
         super(KubernetesDecorator, self).__init__(attributes, statically_defined)
@@ -110,14 +112,21 @@
             self.attributes["service_account"] = KUBERNETES_SERVICE_ACCOUNT
         if not self.attributes["gpu_vendor"]:
             self.attributes["gpu_vendor"] = KUBERNETES_GPU_VENDOR
         if not self.attributes["node_selector"] and KUBERNETES_NODE_SELECTOR:
             self.attributes["node_selector"] = KUBERNETES_NODE_SELECTOR
         if not self.attributes["tolerations"] and KUBERNETES_TOLERATIONS:
             self.attributes["tolerations"] = json.loads(KUBERNETES_TOLERATIONS)
+        if (
+            not self.attributes["persistent_volume_claims"]
+            and KUBERNETES_PERSISTENT_VOLUME_CLAIMS
+        ):
+            self.attributes["persistent_volume_claims"] = json.loads(
+                KUBERNETES_PERSISTENT_VOLUME_CLAIMS
+            )
 
         if isinstance(self.attributes["node_selector"], str):
             self.attributes["node_selector"] = self.parse_node_selector(
                 self.attributes["node_selector"].split(",")
             )
 
         if self.attributes["tolerations"]:
@@ -313,15 +322,15 @@
             for k, v in self.attributes.items():
                 if k == "namespace":
                     cli_args.command_options["k8s_namespace"] = v
                 elif k == "node_selector" and v:
                     cli_args.command_options[k] = ",".join(
                         ["=".join([key, str(val)]) for key, val in v.items()]
                     )
-                elif k == "tolerations":
+                elif k in ["tolerations", "persistent_volume_claims"]:
                     cli_args.command_options[k] = json.dumps(v)
                 else:
                     cli_args.command_options[k] = v
             cli_args.command_options["run-time-limit"] = self.run_time_limit
             cli_args.entrypoint[0] = sys.executable
 
     def task_pre_step(
```

### Comparing `metaflow-2.8.5/metaflow/plugins/kubernetes/kubernetes_job.py` & `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,22 +162,37 @@
                                             self._kwargs["gpu"]
                                         )
                                         for k in [0]
                                         # Don't set GPU limits if gpu isn't specified.
                                         if self._kwargs["gpu"] is not None
                                     },
                                 ),
-                                volume_mounts=[
-                                    client.V1VolumeMount(
-                                        mount_path=self._kwargs.get("tmpfs_path"),
-                                        name="tmpfs-ephemeral-volume",
-                                    )
-                                ]
-                                if tmpfs_enabled
-                                else [],
+                                volume_mounts=(
+                                    [
+                                        client.V1VolumeMount(
+                                            mount_path=self._kwargs.get("tmpfs_path"),
+                                            name="tmpfs-ephemeral-volume",
+                                        )
+                                    ]
+                                    if tmpfs_enabled
+                                    else []
+                                )
+                                + (
+                                    [
+                                        client.V1VolumeMount(
+                                            mount_path=path, name=claim
+                                        )
+                                        for claim, path in self._kwargs[
+                                            "persistent_volume_claims"
+                                        ].items()
+                                    ]
+                                    if self._kwargs["persistent_volume_claims"]
+                                    is not None
+                                    else []
+                                ),
                             )
                         ],
                         node_selector=self._kwargs.get("node_selector"),
                         # TODO (savin): Support image_pull_secrets
                         # image_pull_secrets=?,
                         # TODO (savin): Support preemption policies
                         # preemption_policy=?,
@@ -191,26 +206,43 @@
                         service_account_name=self._kwargs["service_account"],
                         # Terminate the container immediately on SIGTERM
                         termination_grace_period_seconds=0,
                         tolerations=[
                             client.V1Toleration(**toleration)
                             for toleration in self._kwargs.get("tolerations") or []
                         ],
-                        volumes=[
-                            client.V1Volume(
-                                name="tmpfs-ephemeral-volume",
-                                empty_dir=client.V1EmptyDirVolumeSource(
-                                    medium="Memory",
-                                    # Add default unit as ours differs from Kubernetes default.
-                                    size_limit="{}Mi".format(tmpfs_size),
-                                ),
-                            )
-                        ]
-                        if tmpfs_enabled
-                        else [],
+                        volumes=(
+                            [
+                                client.V1Volume(
+                                    name="tmpfs-ephemeral-volume",
+                                    empty_dir=client.V1EmptyDirVolumeSource(
+                                        medium="Memory",
+                                        # Add default unit as ours differs from Kubernetes default.
+                                        size_limit="{}Mi".format(tmpfs_size),
+                                    ),
+                                )
+                            ]
+                            if tmpfs_enabled
+                            else []
+                        )
+                        + (
+                            [
+                                client.V1Volume(
+                                    name=claim,
+                                    persistent_volume_claim=client.V1PersistentVolumeClaimVolumeSource(
+                                        claim_name=claim
+                                    ),
+                                )
+                                for claim in self._kwargs[
+                                    "persistent_volume_claims"
+                                ].keys()
+                            ]
+                            if self._kwargs["persistent_volume_claims"] is not None
+                            else []
+                        ),
                         # TODO (savin): Set termination_message_policy
                     ),
                 ),
             ),
         )
         return self
```

### Comparing `metaflow-2.8.5/metaflow/plugins/metadata/local.py` & `metaflow-2.8.6/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/metadata/service.py` & `metaflow-2.8.6/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/package_cli.py` & `metaflow-2.8.6/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/parallel_decorator.py` & `metaflow-2.8.6/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/project_decorator.py` & `metaflow-2.8.6/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/resources_decorator.py` & `metaflow-2.8.6/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/retry_decorator.py` & `metaflow-2.8.6/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/secrets/secrets_decorator.py` & `metaflow-2.8.6/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/storage_executor.py` & `metaflow-2.8.6/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/tag_cli.py` & `metaflow-2.8.6/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/test_unbounded_foreach_decorator.py` & `metaflow-2.8.6/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/plugins/timeout_decorator.py` & `metaflow-2.8.6/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/procpoll.py` & `metaflow-2.8.6/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/pylint_wrapper.py` & `metaflow-2.8.6/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/runtime.py` & `metaflow-2.8.6/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/sidecar/sidecar.py` & `metaflow-2.8.6/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/sidecar/sidecar_messages.py` & `metaflow-2.8.6/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/sidecar/sidecar_subprocess.py` & `metaflow-2.8.6/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/sidecar/sidecar_worker.py` & `metaflow-2.8.6/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tagging_util.py` & `metaflow-2.8.6/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/task.py` & `metaflow-2.8.6/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/00-helloworld/helloworld.py` & `metaflow-2.8.6/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/01-playlist/README.md` & `metaflow-2.8.6/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/01-playlist/movies.csv` & `metaflow-2.8.6/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/01-playlist/playlist.ipynb` & `metaflow-2.8.6/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/01-playlist/playlist.py` & `metaflow-2.8.6/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/02-statistics/README.md` & `metaflow-2.8.6/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/02-statistics/movies.csv` & `metaflow-2.8.6/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/02-statistics/stats.ipynb` & `metaflow-2.8.6/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/02-statistics/stats.py` & `metaflow-2.8.6/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/03-playlist-redux/README.md` & `metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/03-playlist-redux/playlist.py` & `metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/04-playlist-plus/README.md` & `metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/04-playlist-plus/playlist.py` & `metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/05-hello-cloud/README.md` & `metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/06-statistics-redux/README.md` & `metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/07-worldview/worldview.ipynb` & `metaflow-2.8.6/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/08-autopilot/README.md` & `metaflow-2.8.6/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `metaflow-2.8.6/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow/util.py` & `metaflow-2.8.6/metaflow/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,18 +156,19 @@
 
 
 def get_username():
     """
     Return the name of the current user, or None if the current user
     could not be determined.
     """
+    from metaflow.metaflow_config import USER
+
     # note: the order of the list matters
-    ENVVARS = ["METAFLOW_USER", "SUDO_USER", "USERNAME", "USER"]
-    for var in ENVVARS:
-        user = os.environ.get(var)
+    ENVVARS = ["SUDO_USER", "USERNAME", "USER"]
+    for user in [USER] + [os.environ.get(x) for x in ENVVARS]:
         if user and user != "root":
             return user
     return None
 
 
 def resolve_identity_as_tuple():
     prod_token = os.environ.get("METAFLOW_PRODUCTION_TOKEN")
@@ -240,15 +241,14 @@
         return top_package_name, top_package_version
 
     except AttributeError:
         return top_package_name, None
 
 
 def compress_list(lst, separator=",", rangedelim=":", zlibmarker="!", zlibmin=500):
-
     bad_items = [x for x in lst if separator in x or rangedelim in x or zlibmarker in x]
     if bad_items:
         raise MetaflowInternalError(
             "Item '%s' includes a delimiter character "
             "so it can't be compressed" % bad_items[0]
         )
     # Three output modes:
```

### Comparing `metaflow-2.8.5/metaflow/vendor.py` & `metaflow-2.8.6/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/metaflow.egg-info/PKG-INFO` & `metaflow-2.8.6/metaflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.8.5
+Version: 2.8.6
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.8.5/metaflow.egg-info/SOURCES.txt` & `metaflow-2.8.6/metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.5/setup.py` & `metaflow-2.8.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.8.5"
+version = "2.8.6"
 
 setup(
     include_package_data=True,
     name="metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

