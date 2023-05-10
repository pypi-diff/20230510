# Comparing `tmp/tributary-0.2.0.tar.gz` & `tmp/tributary-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tributary-0.2.0.tar", last modified: Wed May 11 00:34:04 2022, max compression
+gzip compressed data, was "tributary-0.2.1.tar", last modified: Wed May 10 10:37:47 2023, max compression
```

## Comparing `tributary-0.2.0.tar` & `tributary-0.2.1.tar`

### file list

```diff
@@ -1,185 +1,184 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.365054 tributary-0.2.0/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3222 2018-09-08 03:00:36.000000 tributary-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 timkpaine   (501) staff       (20)     1752 2022-02-14 17:32:14.000000 tributary-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 timkpaine   (501) staff       (20)    11347 2020-09-04 13:58:13.000000 tributary-0.2.0/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      554 2022-04-03 03:33:25.000000 tributary-0.2.0/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     1996 2022-04-30 03:08:42.000000 tributary-0.2.0/Makefile
--rw-r--r--   0 timkpaine   (501) staff       (20)     5671 2022-05-11 00:34:04.365212 tributary-0.2.0/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     4914 2022-02-14 17:32:14.000000 tributary-0.2.0/README.md
--rw-r--r--   0 timkpaine   (501) staff       (20)      106 2021-11-24 03:42:05.000000 tributary-0.2.0/pyproject.toml
--rw-r--r--   0 timkpaine   (501) staff       (20)     1160 2022-05-11 00:34:04.365937 tributary-0.2.0/setup.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)     2564 2022-04-03 03:33:25.000000 tributary-0.2.0/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.294733 tributary-0.2.0/tributary/
--rw-r--r--   0 timkpaine   (501) staff       (20)      225 2020-11-17 00:05:34.000000 tributary-0.2.0/tributary/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       22 2022-04-03 03:33:25.000000 tributary-0.2.0/tributary/_version.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2040 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/base.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.298831 tributary-0.2.0/tributary/functional/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3944 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/functional/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4621 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/functional/input.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2018-09-20 20:12:56.000000 tributary-0.2.0/tributary/functional/output.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1089 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/functional/utils.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.299661 tributary-0.2.0/tributary/incubating/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/incubating/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1536 2022-03-06 16:56:06.000000 tributary-0.2.0/tributary/incubating/ast_experiments.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.304068 tributary-0.2.0/tributary/lazy/
--rw-r--r--   0 timkpaine   (501) staff       (20)      167 2022-02-23 19:38:26.000000 tributary-0.2.0/tributary/lazy/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       80 2022-03-06 16:56:06.000000 tributary-0.2.0/tributary/lazy/base.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.309112 tributary-0.2.0/tributary/lazy/calculations/
--rw-r--r--   0 timkpaine   (501) staff       (20)       87 2021-11-27 03:44:18.000000 tributary-0.2.0/tributary/lazy/calculations/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1162 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/lazy/calculations/basket.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2375 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/lazy/calculations/finance.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    18811 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/lazy/calculations/ops.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1091 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/lazy/calculations/rolling.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       40 2020-03-03 20:57:23.000000 tributary-0.2.0/tributary/lazy/calculations/utils.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.310647 tributary-0.2.0/tributary/lazy/control/
--rw-r--r--   0 timkpaine   (501) staff       (20)       24 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/lazy/control/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1236 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/lazy/control/control.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       35 2020-07-19 00:53:06.000000 tributary-0.2.0/tributary/lazy/control/utils.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      706 2021-11-22 20:18:42.000000 tributary-0.2.0/tributary/lazy/dd3.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1368 2022-03-06 16:56:06.000000 tributary-0.2.0/tributary/lazy/decorator.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3277 2022-03-06 16:56:06.000000 tributary-0.2.0/tributary/lazy/graph.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.311303 tributary-0.2.0/tributary/lazy/input/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-17 22:44:21.000000 tributary-0.2.0/tributary/lazy/input/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    17919 2022-03-06 16:56:06.000000 tributary-0.2.0/tributary/lazy/node.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.312130 tributary-0.2.0/tributary/lazy/output/
--rw-r--r--   0 timkpaine   (501) staff       (20)       50 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/lazy/output/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5571 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/lazy/output/output.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2580 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/lazy/utils.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.312655 tributary-0.2.0/tributary/parser/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3472 2022-03-06 16:56:06.000000 tributary-0.2.0/tributary/parser/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.316897 tributary-0.2.0/tributary/streaming/
--rw-r--r--   0 timkpaine   (501) staff       (20)      418 2021-11-22 20:27:41.000000 tributary-0.2.0/tributary/streaming/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/streaming/base.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.319902 tributary-0.2.0/tributary/streaming/calculations/
--rw-r--r--   0 timkpaine   (501) staff       (20)       87 2021-11-22 20:16:56.000000 tributary-0.2.0/tributary/streaming/calculations/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      615 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/streaming/calculations/basket.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1565 2022-05-11 00:32:44.000000 tributary-0.2.0/tributary/streaming/calculations/finance.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10370 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/calculations/ops.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6518 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/calculations/rolling.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       69 2020-08-24 03:23:45.000000 tributary-0.2.0/tributary/streaming/calculations/utils.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.321527 tributary-0.2.0/tributary/streaming/control/
--rw-r--r--   0 timkpaine   (501) staff       (20)       24 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/streaming/control/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1122 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/streaming/control/control.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       35 2020-07-19 00:53:06.000000 tributary-0.2.0/tributary/streaming/control/utils.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1535 2021-11-22 20:18:42.000000 tributary-0.2.0/tributary/streaming/dd3.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3202 2021-11-22 20:27:41.000000 tributary-0.2.0/tributary/streaming/graph.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.326883 tributary-0.2.0/tributary/streaming/input/
--rw-r--r--   0 timkpaine   (501) staff       (20)      697 2021-11-22 20:16:56.000000 tributary-0.2.0/tributary/streaming/input/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      903 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/file.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6810 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/http.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4638 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/input.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1837 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/kafka.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1568 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/postgres.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1088 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/process.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1636 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/socketio.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      958 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/sse.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5913 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/input/ws.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    14167 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/node.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.332141 tributary-0.2.0/tributary/streaming/output/
--rw-r--r--   0 timkpaine   (501) staff       (20)      652 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2379 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/email.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      937 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/file.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6714 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/http.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1425 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/kafka.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5463 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/streaming/output/output.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1205 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/postgres.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1422 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/socketio.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5356 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/sse.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      880 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/text.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7919 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/output/ws.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5048 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/streaming/scheduler.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3256 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/streaming/serialize.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10452 2022-05-11 00:32:44.000000 tributary-0.2.0/tributary/streaming/utils.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.332654 tributary-0.2.0/tributary/symbolic/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3067 2022-03-06 16:56:06.000000 tributary-0.2.0/tributary/symbolic/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.333626 tributary-0.2.0/tributary/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-06 20:47:28.000000 tributary-0.2.0/tributary/tests/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.335673 tributary-0.2.0/tributary/tests/functional/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-06 20:47:28.000000 tributary-0.2.0/tributary/tests/functional/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      720 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/functional/test_functional.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      245 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/tests/functional/test_input_func.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-06 20:47:28.000000 tributary-0.2.0/tributary/tests/functional/test_output_func.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-06 20:47:28.000000 tributary-0.2.0/tributary/tests/functional/test_utils_func.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.339723 tributary-0.2.0/tributary/tests/lazy/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-06 20:47:28.000000 tributary-0.2.0/tributary/tests/lazy/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.342825 tributary-0.2.0/tributary/tests/lazy/calculations/
--rw-r--r--   0 timkpaine   (501) staff       (20)      951 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/calculations/test_basket_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5447 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/lazy/calculations/test_dual_ops_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2318 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/calculations/test_finance_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4385 2020-11-19 04:34:18.000000 tributary-0.2.0/tributary/tests/lazy/calculations/test_ops_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)       28 2020-11-17 00:05:34.000000 tributary-0.2.0/tributary/tests/lazy/calculations/test_rolling_lazy.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.343876 tributary-0.2.0/tributary/tests/lazy/control/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-07-19 00:53:06.000000 tributary-0.2.0/tributary/tests/lazy/control/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      411 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/control/test_if_lazy.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.344521 tributary-0.2.0/tributary/tests/lazy/input/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-07-19 00:53:06.000000 tributary-0.2.0/tributary/tests/lazy/input/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.345004 tributary-0.2.0/tributary/tests/lazy/output/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-07-19 00:53:06.000000 tributary-0.2.0/tributary/tests/lazy/output/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      452 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/output/test_output_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6501 2020-11-19 04:34:18.000000 tributary-0.2.0/tributary/tests/lazy/test_api_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      207 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/test_declarative_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      288 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/test_fix_value_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2254 2022-03-06 16:56:06.000000 tributary-0.2.0/tributary/tests/lazy/test_graph_class_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      695 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/test_method_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      324 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/test_tolerance_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1018 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/test_tweaks_lazy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1350 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/lazy/test_utils_lazy.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.348544 tributary-0.2.0/tributary/tests/streaming/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-17 22:44:21.000000 tributary-0.2.0/tributary/tests/streaming/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.351999 tributary-0.2.0/tributary/tests/streaming/calculations/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-17 22:44:21.000000 tributary-0.2.0/tributary/tests/streaming/calculations/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      786 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/calculations/test_basket_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-17 22:44:21.000000 tributary-0.2.0/tributary/tests/streaming/calculations/test_calculations_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10446 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/calculations/test_dual_ops_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1856 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/tests/streaming/calculations/test_finance_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5989 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/calculations/test_ops_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2306 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/calculations/test_rolling_streaming.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.352853 tributary-0.2.0/tributary/tests/streaming/control/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-07-19 00:53:06.000000 tributary-0.2.0/tributary/tests/streaming/control/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      440 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/streaming/control/test_if_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      317 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/tests/streaming/echo.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.358093 tributary-0.2.0/tributary/tests/streaming/input/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-17 22:44:21.000000 tributary-0.2.0/tributary/tests/streaming/input/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      908 2020-11-17 00:05:34.000000 tributary-0.2.0/tributary/tests/streaming/input/test_file_data.csv
--rw-r--r--   0 timkpaine   (501) staff       (20)      710 2020-11-17 00:05:34.000000 tributary-0.2.0/tributary/tests/streaming/input/test_file_data.json
--rw-r--r--   0 timkpaine   (501) staff       (20)     4785 2020-11-19 04:34:18.000000 tributary-0.2.0/tributary/tests/streaming/input/test_file_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      923 2021-11-22 20:18:42.000000 tributary-0.2.0/tributary/tests/streaming/input/test_http_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2689 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/input/test_input_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      505 2020-11-19 04:34:18.000000 tributary-0.2.0/tributary/tests/streaming/input/test_postgres_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      947 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/streaming/input/test_process_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-11-19 04:34:18.000000 tributary-0.2.0/tributary/tests/streaming/input/test_sse_streaming.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.362045 tributary-0.2.0/tributary/tests/streaming/output/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-17 22:44:21.000000 tributary-0.2.0/tributary/tests/streaming/output/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      748 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/output/test_file_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1250 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/output/test_http_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      494 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/output/test_kafka_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      796 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/output/test_output_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      677 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/output/test_postgres_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      485 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/output/test_socketio_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-11-19 04:34:18.000000 tributary-0.2.0/tributary/tests/streaming/output/test_sse_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      755 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/output/test_ws_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10365 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/test_api_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2450 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/test_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      791 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/streaming/test_timing_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5743 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/streaming/test_utils_streaming.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.362712 tributary-0.2.0/tributary/tests/symbolic/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-06 20:47:28.000000 tributary-0.2.0/tributary/tests/symbolic/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3221 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/symbolic/test_symbolic.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      194 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/tests/test_base.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.363191 tributary-0.2.0/tributary/tests/test_data/
--rw-r--r--   0 timkpaine   (501) staff       (20)     4449 2020-02-06 20:47:28.000000 tributary-0.2.0/tributary/tests/test_data/ohlc.csv
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.364414 tributary-0.2.0/tributary/tests/utils/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-04-26 00:22:34.000000 tributary-0.2.0/tributary/tests/utils/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2004 2022-02-14 17:32:14.000000 tributary-0.2.0/tributary/tests/utils/test_extract_parameters.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2011 2022-02-23 19:14:28.000000 tributary-0.2.0/tributary/tests/utils/test_lazy_to_streaming.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      588 2020-11-17 00:05:36.000000 tributary-0.2.0/tributary/thread.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.364865 tributary-0.2.0/tributary/ts/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2020-02-06 20:48:28.000000 tributary-0.2.0/tributary/ts/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3968 2022-02-14 21:24:16.000000 tributary-0.2.0/tributary/utils.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2022-05-11 00:34:04.297094 tributary-0.2.0/tributary.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     5671 2022-05-11 00:34:03.000000 tributary-0.2.0/tributary.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)     5826 2022-05-11 00:34:03.000000 tributary-0.2.0/tributary.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2022-05-11 00:34:03.000000 tributary-0.2.0/tributary.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2022-04-03 03:08:40.000000 tributary-0.2.0/tributary.egg-info/not-zip-safe
--rw-r--r--   0 timkpaine   (501) staff       (20)     1705 2022-05-11 00:34:03.000000 tributary-0.2.0/tributary.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       10 2022-05-11 00:34:03.000000 tributary-0.2.0/tributary.egg-info/top_level.txt
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.717204 tributary-0.2.1/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1752 2023-03-21 17:18:35.000000 tributary-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11347 2023-03-21 17:18:35.000000 tributary-0.2.1/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      554 2023-03-21 17:18:35.000000 tributary-0.2.1/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1996 2023-03-21 17:18:35.000000 tributary-0.2.1/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5717 2023-05-10 10:37:47.717303 tributary-0.2.1/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4976 2023-05-10 10:36:50.000000 tributary-0.2.1/README.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)      106 2023-03-21 17:18:35.000000 tributary-0.2.1/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1060 2023-05-10 10:37:47.717659 tributary-0.2.1/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2567 2023-05-10 10:24:53.000000 tributary-0.2.1/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.694069 tributary-0.2.1/tributary/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      225 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       22 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/_version.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2111 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/base.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.696036 tributary-0.2.1/tributary/functional/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3944 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/functional/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4621 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/functional/input.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/functional/output.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1089 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/functional/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.696298 tributary-0.2.1/tributary/incubating/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/incubating/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1536 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/incubating/ast_experiments.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.697490 tributary-0.2.1/tributary/lazy/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      167 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       80 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/base.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.698481 tributary-0.2.1/tributary/lazy/calculations/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       87 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/calculations/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1162 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/calculations/basket.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2375 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/calculations/finance.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    18944 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/calculations/ops.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1091 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/calculations/rolling.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       40 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/calculations/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.698958 tributary-0.2.1/tributary/lazy/control/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       24 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/control/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1236 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/control/control.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       35 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/control/utils.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      706 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/dd3.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1368 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/decorator.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3277 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/graph.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.699110 tributary-0.2.1/tributary/lazy/input/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/input/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    17919 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/node.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.699392 tributary-0.2.1/tributary/lazy/output/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       50 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/output/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5571 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/output/output.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2580 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/lazy/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.699578 tributary-0.2.1/tributary/parser/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3472 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/parser/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.701173 tributary-0.2.1/tributary/streaming/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      418 2023-05-10 08:56:55.000000 tributary-0.2.1/tributary/streaming/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/base.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.702431 tributary-0.2.1/tributary/streaming/calculations/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       87 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/calculations/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      615 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/calculations/basket.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1565 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/calculations/finance.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10503 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/calculations/ops.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6518 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/calculations/rolling.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       69 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/calculations/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.702895 tributary-0.2.1/tributary/streaming/control/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       24 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/control/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1122 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/control/control.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       35 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/control/utils.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1634 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/streaming/dd3.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3563 2023-05-10 10:36:50.000000 tributary-0.2.1/tributary/streaming/graph.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.705108 tributary-0.2.1/tributary/streaming/input/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      697 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/input/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      903 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/input/file.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6809 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/streaming/input/http.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4638 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/input/input.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1836 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/streaming/input/kafka.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1568 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/input/postgres.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1088 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/input/process.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1636 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/input/socketio.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      958 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/input/sse.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5912 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/streaming/input/ws.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    14174 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/streaming/node.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.706827 tributary-0.2.1/tributary/streaming/output/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      652 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2379 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/email.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      937 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/file.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6714 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/http.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1425 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/kafka.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5463 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/output.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1205 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/postgres.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1422 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/socketio.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5356 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/sse.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      879 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/streaming/output/text.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     7919 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/output/ws.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5048 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/scheduler.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3256 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/serialize.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10452 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/streaming/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.706985 tributary-0.2.1/tributary/symbolic/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3067 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/symbolic/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.707248 tributary-0.2.1/tributary/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.707961 tributary-0.2.1/tributary/tests/functional/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/functional/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      720 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/functional/test_functional.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      245 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/functional/test_input_func.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/functional/test_output_func.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/functional/test_utils_func.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.709415 tributary-0.2.1/tributary/tests/lazy/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.710308 tributary-0.2.1/tributary/tests/lazy/calculations/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      951 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/calculations/test_basket_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5447 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/calculations/test_dual_ops_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2544 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/tests/lazy/calculations/test_finance_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4385 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/calculations/test_ops_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)       28 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/calculations/test_rolling_lazy.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.710625 tributary-0.2.1/tributary/tests/lazy/control/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/control/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      411 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/control/test_if_lazy.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.710797 tributary-0.2.1/tributary/tests/lazy/input/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/input/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.711034 tributary-0.2.1/tributary/tests/lazy/output/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/output/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      452 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/output/test_output_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     6501 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/test_api_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      207 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/test_declarative_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      288 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/test_fix_value_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2254 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/test_graph_class_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      695 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/test_method_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      324 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/test_tolerance_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1018 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/test_tweaks_lazy.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1350 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/lazy/test_utils_lazy.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.711930 tributary-0.2.1/tributary/tests/streaming/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/__init__.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.713025 tributary-0.2.1/tributary/tests/streaming/calculations/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/calculations/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      786 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/calculations/test_basket_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/calculations/test_calculations_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10446 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/calculations/test_dual_ops_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2086 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/tests/streaming/calculations/test_finance_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5989 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/calculations/test_ops_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2306 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/calculations/test_rolling_streaming.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.713297 tributary-0.2.1/tributary/tests/streaming/control/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/control/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      440 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/control/test_if_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      317 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/echo.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.714737 tributary-0.2.1/tributary/tests/streaming/input/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      908 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/test_file_data.csv
+-rw-r--r--   0 timkpaine   (501) staff       (20)      710 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/test_file_data.json
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4785 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/test_file_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      923 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/test_http_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2689 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/test_input_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      505 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/test_postgres_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      947 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/test_process_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/input/test_sse_streaming.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.716007 tributary-0.2.1/tributary/tests/streaming/output/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      748 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/test_file_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1250 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/test_http_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      494 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/test_kafka_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      796 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/test_output_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      677 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/test_postgres_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      485 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/test_socketio_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/test_sse_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      755 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/output/test_ws_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)    10365 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/test_api_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2450 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/test_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      791 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/streaming/test_timing_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5742 2023-05-10 10:24:53.000000 tributary-0.2.1/tributary/tests/streaming/test_utils_streaming.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.716271 tributary-0.2.1/tributary/tests/symbolic/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/symbolic/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3221 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/symbolic/test_symbolic.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      194 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/test_base.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.716440 tributary-0.2.1/tributary/tests/test_data/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4449 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/test_data/ohlc.csv
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.716920 tributary-0.2.1/tributary/tests/utils/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/utils/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2004 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/utils/test_extract_parameters.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2011 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/tests/utils/test_lazy_to_streaming.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      588 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/thread.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.717079 tributary-0.2.1/tributary/ts/
+-rw-r--r--   0 timkpaine   (501) staff       (20)        0 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/ts/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     3968 2023-03-21 17:18:35.000000 tributary-0.2.1/tributary/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-05-10 10:37:47.695323 tributary-0.2.1/tributary.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5717 2023-05-10 10:37:47.000000 tributary-0.2.1/tributary.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5807 2023-05-10 10:37:47.000000 tributary-0.2.1/tributary.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-05-10 10:37:47.000000 tributary-0.2.1/tributary.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-05-09 22:33:04.000000 tributary-0.2.1/tributary.egg-info/not-zip-safe
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1703 2023-05-10 10:37:47.000000 tributary-0.2.1/tributary.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       10 2023-05-10 10:37:47.000000 tributary-0.2.1/tributary.egg-info/top_level.txt
```

### Comparing `tributary-0.2.0/CONTRIBUTING.md` & `tributary-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/LICENSE` & `tributary-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/MANIFEST.in` & `tributary-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/Makefile` & `tributary-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/PKG-INFO` & `tributary-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,355 +1,358 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7472 6962  : 2.1.Name: trib
 00000020: 7574 6172 790a 5665 7273 696f 6e3a 2030  utary.Version: 0
-00000030: 2e32 2e30 0a53 756d 6d61 7279 3a20 5374  .2.0.Summary: St
+00000030: 2e32 2e31 0a53 756d 6d61 7279 3a20 5374  .2.1.Summary: St
 00000040: 7265 616d 696e 6720 7265 6163 7469 7665  reaming reactive
 00000050: 2061 6e64 2064 6174 6166 6c6f 7720 6772   and dataflow gr
 00000060: 6170 6873 2069 6e20 5079 7468 6f6e 0a48  aphs in Python.H
 00000070: 6f6d 652d 7061 6765 3a20 6874 7470 733a  ome-page: https:
-00000080: 2f2f 6769 7468 7562 2e63 6f6d 2f74 696d  //github.com/tim
-00000090: 6b70 6169 6e65 2f74 7269 6275 7461 7279  kpaine/tributary
-000000a0: 0a41 7574 686f 723a 2054 696d 2050 6169  .Author: Tim Pai
-000000b0: 6e65 0a41 7574 686f 722d 656d 6169 6c3a  ne.Author-email:
-000000c0: 2074 2e70 6169 6e65 3135 3440 676d 6169   t.paine154@gmai
-000000d0: 6c2e 636f 6d0a 4c69 6365 6e73 653a 2041  l.com.License: A
-000000e0: 7061 6368 6520 322e 300a 4b65 7977 6f72  pache 2.0.Keywor
-000000f0: 6473 3a20 7374 7265 616d 696e 6720 6c61  ds: streaming la
-00000100: 7a79 2067 7261 7068 2064 6167 2064 6174  zy graph dag dat
-00000110: 6166 6c6f 7720 7265 6163 7469 7665 0a50  aflow reactive.P
-00000120: 6c61 7466 6f72 6d3a 2055 4e4b 4e4f 574e  latform: UNKNOWN
-00000130: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-00000140: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000150: 3a3a 2033 202d 2041 6c70 6861 0a43 6c61  :: 3 - Alpha.Cla
-00000160: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000170: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000180: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
-00000190: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000001a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001b0: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
-000001c0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-000001f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000220: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-00000230: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000240: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000250: 2033 2e31 300a 5265 7175 6972 6573 2d50   3.10.Requires-P
-00000260: 7974 686f 6e3a 203e 3d33 2e37 0a44 6573  ython: >=3.7.Des
-00000270: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000280: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000290: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
-000002a0: 7472 613a 2064 6576 0a50 726f 7669 6465  tra: dev.Provide
-000002b0: 732d 4578 7472 613a 2064 6576 656c 6f70  s-Extra: develop
-000002c0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000002d0: 2066 756e 6374 696f 6e61 6c0a 4c69 6365   functional.Lice
-000002e0: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-000002f0: 450a 0a23 203c 6120 6872 6566 3d22 6874  E..# <a href="ht
-00000300: 7470 733a 2f2f 7472 6962 7574 6172 792e  tps://tributary.
-00000310: 7265 6164 7468 6564 6f63 732e 696f 223e  readthedocs.io">
-00000320: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000330: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000340: 636f 6e74 656e 742e 636f 6d2f 7469 6d6b  content.com/timk
-00000350: 7061 696e 652f 7472 6962 7574 6172 792f  paine/tributary/
-00000360: 6d61 696e 2f64 6f63 732f 696d 672f 6963  main/docs/img/ic
-00000370: 6f6e 2e70 6e67 2220 7769 6474 683d 2233  on.png" width="3
-00000380: 3030 223e 3c2f 613e 0a50 7974 686f 6e20  00"></a>.Python 
-00000390: 4461 7461 2053 7472 6561 6d73 0a0a 5b21  Data Streams..[!
-000003a0: 5b42 7569 6c64 2053 7461 7475 735d 2868  [Build Status](h
-000003b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000003c0: 6d2f 7469 6d6b 7061 696e 652f 7472 6962  m/timkpaine/trib
-000003d0: 7574 6172 792f 776f 726b 666c 6f77 732f  utary/workflows/
-000003e0: 4275 696c 6425 3230 5374 6174 7573 2f62  Build%20Status/b
-000003f0: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
-00000400: 6d61 696e 295d 2868 7474 7073 3a2f 2f67  main)](https://g
-00000410: 6974 6875 622e 636f 6d2f 7469 6d6b 7061  ithub.com/timkpa
-00000420: 696e 652f 7472 6962 7574 6172 792f 6163  ine/tributary/ac
-00000430: 7469 6f6e 733f 7175 6572 793d 776f 726b  tions?query=work
-00000440: 666c 6f77 2533 4125 3232 4275 696c 642b  flow%3A%22Build+
-00000450: 5374 6174 7573 2532 3229 0a5b 215b 436f  Status%22).[![Co
-00000460: 7665 7261 6765 5d28 6874 7470 733a 2f2f  verage](https://
-00000470: 636f 6465 636f 762e 696f 2f67 682f 7469  codecov.io/gh/ti
-00000480: 6d6b 7061 696e 652f 7472 6962 7574 6172  mkpaine/tributar
-00000490: 792f 6272 616e 6368 2f6d 6169 6e2f 6772  y/branch/main/gr
-000004a0: 6170 682f 6261 6467 652e 7376 6729 5d28  aph/badge.svg)](
-000004b0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
-000004c0: 696f 2f67 682f 7469 6d6b 7061 696e 652f  io/gh/timkpaine/
-000004d0: 7472 6962 7574 6172 7929 0a5b 215b 5079  tributary).[![Py
-000004e0: 5049 5d28 6874 7470 733a 2f2f 696d 672e  PI](https://img.
-000004f0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000500: 6c2f 7472 6962 7574 6172 792e 7376 6729  l/tributary.svg)
-00000510: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
-00000520: 7974 686f 6e2e 6f72 672f 7079 7069 2f74  ython.org/pypi/t
-00000530: 7269 6275 7461 7279 290a 5b21 5b50 7950  ributary).[![PyP
-00000540: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
-00000550: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000560: 2f74 7269 6275 7461 7279 2e73 7667 295d  /tributary.svg)]
-00000570: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
-00000580: 7468 6f6e 2e6f 7267 2f70 7970 692f 7472  thon.org/pypi/tr
-00000590: 6962 7574 6172 7929 0a5b 215b 4269 6e64  ibutary).[![Bind
-000005a0: 6572 5d28 6874 7470 733a 2f2f 6d79 6269  er](https://mybi
-000005b0: 6e64 6572 2e6f 7267 2f62 6164 6765 5f6c  nder.org/badge_l
-000005c0: 6f67 6f2e 7376 6729 5d28 6874 7470 733a  ogo.svg)](https:
-000005d0: 2f2f 6d79 6269 6e64 6572 2e6f 7267 2f76  //mybinder.org/v
-000005e0: 322f 6768 2f74 696d 6b70 6169 6e65 2f74  2/gh/timkpaine/t
-000005f0: 7269 6275 7461 7279 2f6d 6169 6e3f 7572  ributary/main?ur
-00000600: 6c70 6174 683d 6c61 6229 0a0a 0a54 7269  lpath=lab)...Tri
-00000610: 6275 7461 7279 2069 7320 6120 6c69 6272  butary is a libr
-00000620: 6172 7920 666f 7220 636f 6e73 7472 7563  ary for construc
-00000630: 7469 6e67 2064 6174 6166 6c6f 7720 6772  ting dataflow gr
-00000640: 6170 6873 2069 6e20 7079 7468 6f6e 2e20  aphs in python. 
-00000650: 556e 6c69 6b65 206d 616e 7920 6f74 6865  Unlike many othe
-00000660: 7220 4441 4720 6c69 6272 6172 6965 7320  r DAG libraries 
-00000670: 696e 2070 7974 686f 6e20 285b 6169 7266  in python ([airf
-00000680: 6c6f 775d 2868 7474 7073 3a2f 2f61 6972  low](https://air
-00000690: 666c 6f77 2e61 7061 6368 652e 6f72 6729  flow.apache.org)
-000006a0: 2c20 5b6c 7569 6769 5d28 6874 7470 733a  , [luigi](https:
-000006b0: 2f2f 6c75 6967 692e 7265 6164 7468 6564  //luigi.readthed
-000006c0: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-000006d0: 2f29 2c20 5b70 7265 6665 6374 5d28 6874  /), [prefect](ht
-000006e0: 7470 733a 2f2f 646f 6373 2e70 7265 6665  tps://docs.prefe
-000006f0: 6374 2e69 6f29 2c20 5b64 6167 7374 6572  ct.io), [dagster
-00000700: 5d28 6874 7470 733a 2f2f 646f 6373 2e64  ](https://docs.d
-00000710: 6167 7374 6572 2e69 6f29 2c20 5b64 6173  agster.io), [das
-00000720: 6b5d 2868 7474 7073 3a2f 2f64 6173 6b2e  k](https://dask.
-00000730: 6f72 6729 2c20 5b6b 6564 726f 5d28 6874  org), [kedro](ht
-00000740: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000750: 2f71 7561 6e74 756d 626c 6163 6b6c 6162  /quantumblacklab
-00000760: 732f 6b65 6472 6f29 2c20 6574 6329 2c20  s/kedro), etc), 
-00000770: 7472 6962 7574 6172 7920 6973 206e 6f74  tributary is not
-00000780: 2064 6573 6967 6e65 6420 7769 7468 2064   designed with d
-00000790: 6174 612f 6574 6c20 7069 7065 6c69 6e65  ata/etl pipeline
-000007a0: 7320 6f72 2073 6368 6564 756c 696e 6720  s or scheduling 
-000007b0: 696e 206d 696e 642e 2049 6e73 7465 6164  in mind. Instead
-000007c0: 2c20 7472 6962 7574 6172 7920 6973 206d  , tributary is m
-000007d0: 6f72 6520 7369 6d69 6c61 7220 746f 206c  ore similar to l
-000007e0: 6962 7261 7269 6573 206c 696b 6520 5b6d  ibraries like [m
-000007f0: 6466 5d28 6874 7470 733a 2f2f 6769 7468  df](https://gith
-00000800: 7562 2e63 6f6d 2f6d 616e 2d67 726f 7570  ub.com/man-group
-00000810: 2f6d 6466 292c 205b 7079 756e 676f 5d28  /mdf), [pyungo](
-00000820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000830: 6f6d 2f63 6564 7269 636c 6572 6f79 2f70  om/cedricleroy/p
-00000840: 7975 6e67 6f29 2c20 5b73 7472 6561 6d7a  yungo), [streamz
-00000850: 5d28 6874 7470 733a 2f2f 7374 7265 616d  ](https://stream
-00000860: 7a2e 7265 6164 7468 6564 6f63 732e 696f  z.readthedocs.io
-00000870: 2f65 6e2f 6c61 7465 7374 2f29 2c20 6f72  /en/latest/), or
-00000880: 205b 7079 6675 6e63 7469 6f6e 616c 5d28   [pyfunctional](
-00000890: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000008a0: 6f6d 2f45 6e74 696c 5a68 612f 5079 4675  om/EntilZha/PyFu
-000008b0: 6e63 7469 6f6e 616c 292c 2069 6e20 7468  nctional), in th
-000008c0: 6174 2069 7420 6973 2064 6573 6967 6e65  at it is designe
-000008d0: 6420 746f 2062 6520 7573 6564 2061 7320  d to be used as 
-000008e0: 7468 6520 696d 706c 656d 656e 7461 7469  the implementati
-000008f0: 6f6e 2066 6f72 2061 2064 6174 6120 6d6f  on for a data mo
-00000900: 6465 6c2e 204f 6e65 2073 7563 6820 6578  del. One such ex
-00000910: 616d 706c 6520 6973 2074 6865 205b 6772  ample is the [gr
-00000920: 6565 6b73 5d28 6874 7470 733a 2f2f 6769  eeks](https://gi
-00000930: 7468 7562 2e63 6f6d 2f74 696d 6b70 6169  thub.com/timkpai
-00000940: 6e65 2f67 7265 656b 7329 206c 6962 7261  ne/greeks) libra
-00000950: 7279 2c20 7768 6963 6820 6c65 7665 7261  ry, which levera
-00000960: 6765 7320 7472 6962 7574 6172 7920 746f  ges tributary to
-00000970: 2062 7569 6c64 2064 6174 6120 6d6f 6465   build data mode
-00000980: 6c73 2066 6f72 205b 6f70 7469 6f6e 7320  ls for [options 
-00000990: 7072 6963 696e 675d 2868 7474 7073 3a2f  pricing](https:/
-000009a0: 2f77 7777 2e69 6e76 6573 746f 7065 6469  /www.investopedi
-000009b0: 612e 636f 6d2f 6172 7469 636c 6573 2f6f  a.com/articles/o
-000009c0: 7074 696f 6e69 6e76 6573 746f 722f 3037  ptioninvestor/07
-000009d0: 2f6f 7074 696f 6e73 5f62 6561 745f 6d61  /options_beat_ma
-000009e0: 726b 6574 2e61 7370 292e 200a 0a21 5b5d  rket.asp). ..![]
-000009f0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
-00000a00: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000a10: 6f6d 2f74 696d 6b70 6169 6e65 2f74 7269  om/timkpaine/tri
-00000a20: 6275 7461 7279 2f6d 6169 6e2f 646f 6373  butary/main/docs
-00000a30: 2f69 6d67 2f65 7861 6d70 6c65 2e67 6966  /img/example.gif
-00000a40: 290a 0a0a 2320 496e 7374 616c 6c61 7469  )...# Installati
-00000a50: 6f6e 0a49 6e73 7461 6c6c 2077 6974 6820  on.Install with 
-00000a60: 7069 703a 0a0a 6070 6970 2069 6e73 7461  pip:..`pip insta
-00000a70: 6c6c 2074 7269 6275 7461 7279 600a 0a6f  ll tributary`..o
-00000a80: 7220 7769 7468 2063 6f6e 6461 3a0a 0a60  r with conda:..`
-00000a90: 636f 6e64 6120 696e 7374 616c 6c20 2d63  conda install -c
-00000aa0: 2063 6f6e 6461 2d66 6f72 6765 2074 7269   conda-forge tri
-00000ab0: 6275 7461 7279 600a 0a6f 7220 6672 6f6d  butary`..or from
-00000ac0: 2073 6f75 7263 653a 0a0a 6070 7974 686f   source:..`pytho
-00000ad0: 6e20 7365 7475 702e 7079 2069 6e73 7461  n setup.py insta
-00000ae0: 6c6c 600a 0a4e 6f74 653a 2049 6620 696e  ll`..Note: If in
-00000af0: 7374 616c 6c69 6e67 2066 726f 6d20 736f  stalling from so
-00000b00: 7572 6365 206f 7220 7769 7468 2070 6970  urce or with pip
-00000b10: 2c20 796f 7527 6c6c 2061 6c73 6f20 6e65  , you'll also ne
-00000b20: 6564 205b 4772 6170 6876 697a 2069 7473  ed [Graphviz its
-00000b30: 656c 665d 2868 7474 7073 3a2f 2f77 7777  elf](https://www
-00000b40: 2e67 7261 7068 7669 7a2e 6f72 672f 646f  .graphviz.org/do
-00000b50: 776e 6c6f 6164 2f29 2069 6620 796f 7520  wnload/) if you 
-00000b60: 7761 6e74 2074 6f20 7669 7375 616c 697a  want to visualiz
-00000b70: 6520 7468 6520 6772 6170 6820 7573 696e  e the graph usin
-00000b80: 6720 7468 6520 602e 6772 6170 6876 697a  g the `.graphviz
-00000b90: 2829 6020 6d65 7468 6f64 2e0a 0a23 2053  ()` method...# S
-00000ba0: 7472 6561 6d20 5479 7065 730a 5472 6962  tream Types.Trib
-00000bb0: 7574 6172 7920 6f66 6665 7273 2073 6576  utary offers sev
-00000bc0: 6572 616c 206b 696e 6473 206f 6620 7374  eral kinds of st
-00000bd0: 7265 616d 733a 0a0a 2323 2053 7472 6561  reams:..## Strea
-00000be0: 6d69 6e67 0a54 6865 7365 2061 7265 2073  ming.These are s
-00000bf0: 796e 6368 726f 6e6f 7573 2c20 7265 6163  ynchronous, reac
-00000c00: 7469 7665 2064 6174 6120 7374 7265 616d  tive data stream
-00000c10: 732c 2062 7569 6c74 2075 7369 6e67 2061  s, built using a
-00000c20: 7379 6e63 6872 6f6e 6f75 7320 7079 7468  synchronous pyth
-00000c30: 6f6e 2067 656e 6572 6174 6f72 732e 2054  on generators. T
-00000c40: 6865 7920 6172 6520 6465 7369 676e 6564  hey are designed
-00000c50: 2074 6f20 6d69 6d69 6320 636f 6d70 6c65   to mimic comple
-00000c60: 7820 6576 656e 7420 7072 6f63 6573 736f  x event processo
-00000c70: 7273 2069 6e20 7465 726d 7320 6f66 2065  rs in terms of e
-00000c80: 7665 6e74 206f 7264 6572 696e 672e 0a0a  vent ordering...
-00000c90: 2323 2046 756e 6374 696f 6e61 6c0a 5468  ## Functional.Th
-00000ca0: 6573 6520 6172 6520 6675 6e63 7469 6f6e  ese are function
-00000cb0: 616c 2073 7472 6561 6d73 2c20 6275 696c  al streams, buil
-00000cc0: 7420 6279 2063 7572 7279 696e 6720 7079  t by currying py
-00000cd0: 7468 6f6e 2066 756e 6374 696f 6e73 2028  thon functions (
-00000ce0: 6361 6c6c 6261 636b 7329 2e20 0a0a 2323  callbacks). ..##
-00000cf0: 204c 617a 790a 5468 6573 6520 6172 6520   Lazy.These are 
-00000d00: 6c61 7a69 6c79 2d65 7661 6c75 6174 6564  lazily-evaluated
-00000d10: 2070 7974 686f 6e20 7374 7265 616d 732c   python streams,
-00000d20: 2077 6865 7265 206f 7574 7075 7473 2061   where outputs a
-00000d30: 7265 2070 726f 706f 6761 7465 6420 6f6e  re propogated on
-00000d40: 6c79 2061 7320 696e 7075 7473 2063 6861  ly as inputs cha
-00000d50: 6e67 652e 2054 6865 7920 6172 6520 696d  nge. They are im
-00000d60: 706c 656d 656e 7465 6420 6173 2064 6972  plemented as dir
-00000d70: 6563 7465 6420 6163 7963 6c69 6320 6772  ected acyclic gr
-00000d80: 6170 6873 2e0a 0a23 2045 7861 6d70 6c65  aphs...# Example
-00000d90: 730a 2d20 5b53 7472 6561 6d69 6e67 5d28  s.- [Streaming](
-00000da0: 646f 6373 2f65 7861 6d70 6c65 732f 7374  docs/examples/st
-00000db0: 7265 616d 696e 672f 7374 7265 616d 696e  reaming/streamin
-00000dc0: 672e 6d64 293a 2049 6e20 7468 6973 2065  g.md): In this e
-00000dd0: 7861 6d70 6c65 2c20 7765 2063 6f6e 7374  xample, we const
-00000de0: 7275 6374 2061 2076 6172 6965 7479 206f  ruct a variety o
-00000df0: 6620 666f 7277 6172 6420 7072 6f70 6f67  f forward propog
-00000e00: 6174 696e 6720 7265 6163 7469 7665 2067  ating reactive g
-00000e10: 7261 7068 732e 0a2d 205b 4c61 7a79 5d28  raphs..- [Lazy](
-00000e20: 646f 6373 2f65 7861 6d70 6c65 732f 6c61  docs/examples/la
-00000e30: 7a79 2f6c 617a 792e 6d64 293a 2049 6e20  zy/lazy.md): In 
-00000e40: 7468 6973 2065 7861 6d70 6c65 2c20 7765  this example, we
-00000e50: 2063 6f6e 7374 7275 6374 2061 2076 6172   construct a var
-00000e60: 6965 7479 206f 6620 6c61 7a69 6c79 2d65  iety of lazily-e
-00000e70: 7661 6c75 6174 6564 2064 6972 6563 7465  valuated directe
-00000e80: 6420 6163 7963 6c69 6320 636f 6d70 7574  d acyclic comput
-00000e90: 6174 696f 6e20 6772 6170 6873 2e20 0a2d  ation graphs. .-
-00000ea0: 205b 4175 746f 6d61 7469 6320 4469 6666   [Automatic Diff
-00000eb0: 6572 656e 7469 6174 696f 6e5d 2864 6f63  erentiation](doc
-00000ec0: 732f 6578 616d 706c 6573 2f61 7574 6f64  s/examples/autod
-00000ed0: 6966 662f 6175 746f 6469 6666 2e6d 6429  iff/autodiff.md)
-00000ee0: 3a20 496e 2074 6869 7320 6578 616d 706c  : In this exampl
-00000ef0: 652c 2077 6520 7573 6520 6074 7269 6275  e, we use `tribu
-00000f00: 7461 7279 6020 746f 2070 6572 666f 726d  tary` to perform
-00000f10: 2061 7574 6f6d 6174 6963 2064 6966 6665   automatic diffe
-00000f20: 7265 6e74 6961 7469 6f6e 206f 6e20 626f  rentiation on bo
-00000f30: 7468 206c 617a 7920 616e 6420 7374 7265  th lazy and stre
-00000f40: 616d 696e 6720 6772 6170 6873 2e0a 0a23  aming graphs...#
-00000f50: 2047 7261 7068 2056 6973 7561 6c69 7a61   Graph Visualiza
-00000f60: 7469 6f6e 0a59 6f75 2063 616e 2076 6973  tion.You can vis
-00000f70: 7561 6c69 7a65 2074 6865 2067 7261 7068  ualize the graph
-00000f80: 2077 6974 6820 4772 6170 6876 697a 2e20   with Graphviz. 
-00000f90: 416c 6c20 7374 7265 616d 696e 6720 616e  All streaming an
-00000fa0: 6420 6c61 7a79 206e 6f64 6573 2073 7570  d lazy nodes sup
-00000fb0: 706f 7274 2061 2060 6772 6170 6876 697a  port a `graphviz
-00000fc0: 6020 6d65 7468 6f64 2e0a 0a53 7472 6561  ` method...Strea
-00000fd0: 6d69 6e67 2061 6e64 206c 617a 7920 6e6f  ming and lazy no
-00000fe0: 6465 7320 616c 736f 2073 7570 706f 7274  des also support
-00000ff0: 205b 6970 7964 6167 7265 6433 5d28 6874   [ipydagred3](ht
-00001000: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001010: 2f74 696d 6b70 6169 6e65 2f69 7079 6461  /timkpaine/ipyda
-00001020: 6772 6564 3329 2066 6f72 206c 6976 6520  gred3) for live 
-00001030: 7570 6461 7465 206d 6f6e 6974 6f72 696e  update monitorin
-00001040: 672e 0a0a 2323 2053 7472 6561 6d69 6e67  g...## Streaming
-00001050: 0a21 5b5d 2868 7474 7073 3a2f 2f72 6177  .![](https://raw
-00001060: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00001070: 6e74 2e63 6f6d 2f74 696d 6b70 6169 6e65  nt.com/timkpaine
-00001080: 2f74 7269 6275 7461 7279 2f6d 6169 6e2f  /tributary/main/
-00001090: 646f 6373 2f69 6d67 2f73 7472 6561 6d69  docs/img/streami
-000010a0: 6e67 2f64 6167 7265 6433 2e67 6966 290a  ng/dagred3.gif).
-000010b0: 0a48 6572 6520 6772 6565 6e20 696e 6469  .Here green indi
-000010c0: 6361 7465 7320 6578 6563 7574 696e 672c  cates executing,
-000010d0: 2079 656c 6c6f 7720 696e 6469 6361 7465   yellow indicate
-000010e0: 7320 7374 616c 6c65 6420 666f 7220 6261  s stalled for ba
-000010f0: 636b 7072 6573 7375 7265 2c20 616e 6420  ckpressure, and 
-00001100: 7265 6420 696e 6469 6361 7465 7320 7468  red indicates th
-00001110: 6174 2060 5374 7265 616d 456e 6460 2068  at `StreamEnd` h
-00001120: 6173 2062 6565 6e20 7072 6f70 6f67 6174  as been propogat
-00001130: 6564 2028 652e 672e 2073 7472 6561 6d20  ed (e.g. stream 
-00001140: 6861 7320 656e 6465 6429 2e0a 0a23 2320  has ended)...## 
-00001150: 4c61 7a79 0a21 5b5d 2868 7474 7073 3a2f  Lazy.![](https:/
-00001160: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00001170: 6f6e 7465 6e74 2e63 6f6d 2f74 696d 6b70  ontent.com/timkp
-00001180: 6169 6e65 2f74 7269 6275 7461 7279 2f6d  aine/tributary/m
-00001190: 6169 6e2f 646f 6373 2f69 6d67 2f6c 617a  ain/docs/img/laz
-000011a0: 792f 6461 6772 6564 332e 6769 6629 0a0a  y/dagred3.gif)..
-000011b0: 4865 7265 2067 7265 656e 2069 6e64 6963  Here green indic
-000011c0: 6174 6573 2065 7865 6375 7469 6e67 2c20  ates executing, 
-000011d0: 616e 6420 7265 6420 696e 6469 6361 7465  and red indicate
-000011e0: 7320 7468 6174 2074 6865 206e 6f64 6520  s that the node 
-000011f0: 6973 2064 6972 7479 2e20 4e6f 7465 2074  is dirty. Note t
-00001200: 6865 2074 6865 2064 6574 6572 6d69 6e61  he the determina
-00001210: 7469 6f6e 2069 6620 6120 6e6f 6465 2069  tion if a node i
-00001220: 7320 6469 7274 7920 6973 2061 6c73 6f20  s dirty is also 
-00001230: 646f 6e65 206c 617a 696c 7920 2877 6520  done lazily (we 
-00001240: 6361 6e20 6368 6563 6b20 7769 7468 2060  can check with `
-00001250: 6973 4469 7274 7960 2077 6863 6968 2077  isDirty` whcih w
-00001260: 696c 6c20 7570 6461 7465 2074 6865 206e  ill update the n
-00001270: 6f64 6527 7320 6772 6170 6820 7374 6174  ode's graph stat
-00001280: 652e 0a0a 2323 2043 6174 616c 6f67 0a53  e...## Catalog.S
-00001290: 6565 2074 6865 205b 4341 5441 4c4f 475d  ee the [CATALOG]
-000012a0: 2843 4154 414c 4f47 2e6d 6429 2066 6f72  (CATALOG.md) for
-000012b0: 2061 2066 756c 6c20 6c69 7374 206f 6620   a full list of 
-000012c0: 6675 6e63 7469 6f6e 732c 2074 7261 6e73  functions, trans
-000012d0: 666f 726d 732c 2073 6f75 7263 6573 2c20  forms, sources, 
-000012e0: 616e 6420 7369 6e6b 732e 0a0a 2323 2053  and sinks...## S
-000012f0: 7570 706f 7274 202f 2043 6f6e 7472 6962  upport / Contrib
-00001300: 7574 6f72 730a 5468 616e 6b73 2074 6f20  utors.Thanks to 
-00001310: 7468 6520 666f 6c6c 6f77 696e 6720 6f72  the following or
-00001320: 6761 6e69 7a61 7469 6f6e 7320 666f 7220  ganizations for 
-00001330: 7072 6f76 6964 696e 6720 636f 6465 206f  providing code o
-00001340: 7220 6669 6e61 6e63 6961 6c20 7375 7070  r financial supp
-00001350: 6f72 742e 0a0a 0a3c 6120 6872 6566 3d22  ort....<a href="
-00001360: 6874 7470 733a 2f2f 6e65 6d6f 756c 6f75  https://nemoulou
-00001370: 732e 636f 6d22 3e3c 696d 6720 7372 633d  s.com"><img src=
-00001380: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00001390: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-000013a0: 6f6d 2f74 696d 6b70 6169 6e65 2f74 7269  om/timkpaine/tri
-000013b0: 6275 7461 7279 2f6d 6169 6e2f 646f 6373  butary/main/docs
-000013c0: 2f69 6d67 2f6e 656d 2e70 6e67 2220 7769  /img/nem.png" wi
-000013d0: 6474 683d 2235 3022 3e3c 2f61 3e0a 0a3c  dth="50"></a>..<
-000013e0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000013f0: 6e65 6d6f 756c 6f75 732e 636f 6d22 3e4e  nemoulous.com">N
-00001400: 656d 6f75 6c6f 7573 3c2f 613e 0a0a 2323  emoulous</a>..##
-00001410: 204c 6963 656e 7365 0a54 6869 7320 736f   License.This so
-00001420: 6674 7761 7265 2069 7320 6c69 6365 6e73  ftware is licens
-00001430: 6564 2075 6e64 6572 2074 6865 2041 7061  ed under the Apa
-00001440: 6368 6520 322e 3020 6c69 6365 6e73 652e  che 2.0 license.
-00001450: 2053 6565 2074 6865 205b 4c49 4345 4e53   See the [LICENS
-00001460: 455d 284c 4943 454e 5345 2920 6669 6c65  E](LICENSE) file
-00001470: 2066 6f72 2064 6574 6169 6c73 2e0a 0a23   for details...#
-00001480: 2320 416c 7465 726e 6174 6976 6573 0a48  # Alternatives.H
-00001490: 6572 6520 6973 2061 6e20 696e 636f 6d70  ere is an incomp
-000014a0: 6c65 7465 206c 6973 7420 6f66 206c 6962  lete list of lib
-000014b0: 7261 7269 6573 2077 6869 6368 2069 6d70  raries which imp
-000014c0: 6c65 6d65 6e74 2073 696d 696c 6172 2f6f  lement similar/o
-000014d0: 7665 726c 6170 7069 6e67 2066 756e 6374  verlapping funct
-000014e0: 696f 6e61 6c69 7479 0a0a 2d20 5b6d 616e  ionality..- [man
-000014f0: 2d67 726f 7570 2f6d 6466 5d28 6874 7470  -group/mdf](http
-00001500: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00001510: 616e 2d67 726f 7570 2f6d 6466 290a 2d20  an-group/mdf).- 
-00001520: 5b63 6564 7269 636c 6572 6f79 2f70 7975  [cedricleroy/pyu
-00001530: 6e67 6f5d 2868 7474 7073 3a2f 2f67 6974  ngo](https://git
-00001540: 6875 622e 636f 6d2f 6365 6472 6963 6c65  hub.com/cedricle
-00001550: 726f 792f 7079 756e 676f 290a 2d20 5b70  roy/pyungo).- [p
-00001560: 7974 686f 6e2d 7374 7265 616d 7a2f 7374  ython-streamz/st
-00001570: 7265 616d 7a5d 2868 7474 7073 3a2f 2f67  reamz](https://g
-00001580: 6974 6875 622e 636f 6d2f 7079 7468 6f6e  ithub.com/python
-00001590: 2d73 7472 6561 6d7a 2f73 7472 6561 6d7a  -streamz/streamz
-000015a0: 290a 2d20 5b45 6e74 696c 5a68 612f 7079  ).- [EntilZha/py
-000015b0: 6675 6e63 7469 6f6e 616c 5d28 6874 7470  functional](http
-000015c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
-000015d0: 6e74 696c 5a68 612f 5079 4675 6e63 7469  ntilZha/PyFuncti
-000015e0: 6f6e 616c 290a 2d20 5b73 7469 7463 6866  onal).- [stitchf
-000015f0: 6978 2f68 616d 696c 746f 6e5d 2868 7474  ix/hamilton](htt
-00001600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001610: 7374 6974 6368 6669 782f 6861 6d69 6c74  stitchfix/hamilt
-00001620: 6f6e 290a 0a0a 0a                        on)....
+00000080: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7472  //github.com/str
+00000090: 6561 6d6c 6574 2d64 6576 2f74 7269 6275  eamlet-dev/tribu
+000000a0: 7461 7279 0a41 7574 686f 723a 2054 696d  tary.Author: Tim
+000000b0: 2050 6169 6e65 0a41 7574 686f 722d 656d   Paine.Author-em
+000000c0: 6169 6c3a 2074 2e70 6169 6e65 3135 3440  ail: t.paine154@
+000000d0: 676d 6169 6c2e 636f 6d0a 4c69 6365 6e73  gmail.com.Licens
+000000e0: 653a 2041 7061 6368 6520 322e 300a 4b65  e: Apache 2.0.Ke
+000000f0: 7977 6f72 6473 3a20 7374 7265 616d 696e  ywords: streamin
+00000100: 6720 6c61 7a79 2067 7261 7068 2064 6167  g lazy graph dag
+00000110: 2064 6174 6166 6c6f 7720 7265 6163 7469   dataflow reacti
+00000120: 7665 0a43 6c61 7373 6966 6965 723a 2044  ve.Classifier: D
+00000130: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
+00000140: 7320 3a3a 2033 202d 2041 6c70 6861 0a43  s :: 3 - Alpha.C
+00000150: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000160: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000170: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
+00000180: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000190: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+000001b0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000001c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001e0: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
+000001f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000200: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000210: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
+00000220: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000240: 3a3a 2033 2e31 300a 5265 7175 6972 6573  :: 3.10.Requires
+00000250: 2d50 7974 686f 6e3a 203e 3d33 2e37 0a44  -Python: >=3.7.D
+00000260: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000270: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000280: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
+00000290: 4578 7472 613a 2064 6576 0a50 726f 7669  Extra: dev.Provi
+000002a0: 6465 732d 4578 7472 613a 2064 6576 656c  des-Extra: devel
+000002b0: 6f70 0a50 726f 7669 6465 732d 4578 7472  op.Provides-Extr
+000002c0: 613a 2066 756e 6374 696f 6e61 6c0a 4c69  a: functional.Li
+000002d0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+000002e0: 4e53 450a 0a23 203c 696d 6720 7372 633d  NSE..# <img src=
+000002f0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000300: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000310: 6f6d 2f73 7472 6561 6d6c 6574 2d64 6576  om/streamlet-dev
+00000320: 2f74 7269 6275 7461 7279 2f6d 6169 6e2f  /tributary/main/
+00000330: 646f 6373 2f69 6d67 2f69 636f 6e2e 706e  docs/img/icon.pn
+00000340: 6722 2077 6964 7468 3d22 3330 3022 3e0a  g" width="300">.
+00000350: 5079 7468 6f6e 2044 6174 6120 5374 7265  Python Data Stre
+00000360: 616d 730a 0a5b 215b 4275 696c 6420 5374  ams..[![Build St
+00000370: 6174 7573 5d28 6874 7470 733a 2f2f 6769  atus](https://gi
+00000380: 7468 7562 2e63 6f6d 2f73 7472 6561 6d6c  thub.com/streaml
+00000390: 6574 2d64 6576 2f74 7269 6275 7461 7279  et-dev/tributary
+000003a0: 2f77 6f72 6b66 6c6f 7773 2f42 7569 6c64  /workflows/Build
+000003b0: 2532 3053 7461 7475 732f 6261 6467 652e  %20Status/badge.
+000003c0: 7376 673f 6272 616e 6368 3d6d 6169 6e29  svg?branch=main)
+000003d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000003e0: 2e63 6f6d 2f73 7472 6561 6d6c 6574 2d64  .com/streamlet-d
+000003f0: 6576 2f74 7269 6275 7461 7279 2f61 6374  ev/tributary/act
+00000400: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
+00000410: 6c6f 7725 3341 2532 3242 7569 6c64 2b53  low%3A%22Build+S
+00000420: 7461 7475 7325 3232 290a 5b21 5b43 6f76  tatus%22).[![Cov
+00000430: 6572 6167 655d 2868 7474 7073 3a2f 2f63  erage](https://c
+00000440: 6f64 6563 6f76 2e69 6f2f 6768 2f73 7472  odecov.io/gh/str
+00000450: 6561 6d6c 6574 2d64 6576 2f74 7269 6275  eamlet-dev/tribu
+00000460: 7461 7279 2f62 7261 6e63 682f 6d61 696e  tary/branch/main
+00000470: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+00000480: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00000490: 6f76 2e69 6f2f 6768 2f73 7472 6561 6d6c  ov.io/gh/streaml
+000004a0: 6574 2d64 6576 2f74 7269 6275 7461 7279  et-dev/tributary
+000004b0: 290a 5b21 5b50 7950 495d 2868 7474 7073  ).[![PyPI](https
+000004c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004d0: 6f2f 7079 7069 2f6c 2f74 7269 6275 7461  o/pypi/l/tributa
+000004e0: 7279 2e73 7667 295d 2868 7474 7073 3a2f  ry.svg)](https:/
+000004f0: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+00000500: 2f70 7970 692f 7472 6962 7574 6172 7929  /pypi/tributary)
+00000510: 0a5b 215b 5079 5049 5d28 6874 7470 733a  .[![PyPI](https:
+00000520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000530: 2f70 7970 692f 762f 7472 6962 7574 6172  /pypi/v/tributar
+00000540: 792e 7376 6729 5d28 6874 7470 733a 2f2f  y.svg)](https://
+00000550: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
+00000560: 7079 7069 2f74 7269 6275 7461 7279 290a  pypi/tributary).
+00000570: 5b21 5b42 696e 6465 725d 2868 7474 7073  [![Binder](https
+00000580: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
+00000590: 6261 6467 655f 6c6f 676f 2e73 7667 295d  badge_logo.svg)]
+000005a0: 2868 7474 7073 3a2f 2f6d 7962 696e 6465  (https://mybinde
+000005b0: 722e 6f72 672f 7632 2f67 682f 7374 7265  r.org/v2/gh/stre
+000005c0: 616d 6c65 742d 6465 762f 7472 6962 7574  amlet-dev/tribut
+000005d0: 6172 792f 6d61 696e 3f75 726c 7061 7468  ary/main?urlpath
+000005e0: 3d6c 6162 290a 0a0a 5472 6962 7574 6172  =lab)...Tributar
+000005f0: 7920 6973 2061 206c 6962 7261 7279 2066  y is a library f
+00000600: 6f72 2063 6f6e 7374 7275 6374 696e 6720  or constructing 
+00000610: 6461 7461 666c 6f77 2067 7261 7068 7320  dataflow graphs 
+00000620: 696e 2070 7974 686f 6e2e 2055 6e6c 696b  in python. Unlik
+00000630: 6520 6d61 6e79 206f 7468 6572 2044 4147  e many other DAG
+00000640: 206c 6962 7261 7269 6573 2069 6e20 7079   libraries in py
+00000650: 7468 6f6e 2028 5b61 6972 666c 6f77 5d28  thon ([airflow](
+00000660: 6874 7470 733a 2f2f 6169 7266 6c6f 772e  https://airflow.
+00000670: 6170 6163 6865 2e6f 7267 292c 205b 6c75  apache.org), [lu
+00000680: 6967 695d 2868 7474 7073 3a2f 2f6c 7569  igi](https://lui
+00000690: 6769 2e72 6561 6474 6865 646f 6373 2e69  gi.readthedocs.i
+000006a0: 6f2f 656e 2f73 7461 626c 652f 292c 205b  o/en/stable/), [
+000006b0: 7072 6566 6563 745d 2868 7474 7073 3a2f  prefect](https:/
+000006c0: 2f64 6f63 732e 7072 6566 6563 742e 696f  /docs.prefect.io
+000006d0: 292c 205b 6461 6773 7465 725d 2868 7474  ), [dagster](htt
+000006e0: 7073 3a2f 2f64 6f63 732e 6461 6773 7465  ps://docs.dagste
+000006f0: 722e 696f 292c 205b 6461 736b 5d28 6874  r.io), [dask](ht
+00000700: 7470 733a 2f2f 6461 736b 2e6f 7267 292c  tps://dask.org),
+00000710: 205b 6b65 6472 6f5d 2868 7474 7073 3a2f   [kedro](https:/
+00000720: 2f67 6974 6875 622e 636f 6d2f 7175 616e  /github.com/quan
+00000730: 7475 6d62 6c61 636b 6c61 6273 2f6b 6564  tumblacklabs/ked
+00000740: 726f 292c 2065 7463 292c 2074 7269 6275  ro), etc), tribu
+00000750: 7461 7279 2069 7320 6e6f 7420 6465 7369  tary is not desi
+00000760: 676e 6564 2077 6974 6820 6461 7461 2f65  gned with data/e
+00000770: 746c 2070 6970 656c 696e 6573 206f 7220  tl pipelines or 
+00000780: 7363 6865 6475 6c69 6e67 2069 6e20 6d69  scheduling in mi
+00000790: 6e64 2e20 496e 7374 6561 642c 2074 7269  nd. Instead, tri
+000007a0: 6275 7461 7279 2069 7320 6d6f 7265 2073  butary is more s
+000007b0: 696d 696c 6172 2074 6f20 6c69 6272 6172  imilar to librar
+000007c0: 6965 7320 6c69 6b65 205b 6d64 665d 2868  ies like [mdf](h
+000007d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000007e0: 6d2f 6d61 6e2d 6772 6f75 702f 6d64 6629  m/man-group/mdf)
+000007f0: 2c20 5b6c 6f6d 616e 5d28 6874 7470 733a  , [loman](https:
+00000800: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 616e  //github.com/jan
+00000810: 7573 6865 6e64 6572 736f 6e61 7373 6574  ushendersonasset
+00000820: 616c 6c6f 6361 7469 6f6e 2f6c 6f6d 616e  allocation/loman
+00000830: 292c 205b 7079 756e 676f 5d28 6874 7470  ), [pyungo](http
+00000840: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000850: 6564 7269 636c 6572 6f79 2f70 7975 6e67  edricleroy/pyung
+00000860: 6f29 2c20 5b73 7472 6561 6d7a 5d28 6874  o), [streamz](ht
+00000870: 7470 733a 2f2f 7374 7265 616d 7a2e 7265  tps://streamz.re
+00000880: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000890: 6c61 7465 7374 2f29 2c20 6f72 205b 7079  latest/), or [py
+000008a0: 6675 6e63 7469 6f6e 616c 5d28 6874 7470  functional](http
+000008b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
+000008c0: 6e74 696c 5a68 612f 5079 4675 6e63 7469  ntilZha/PyFuncti
+000008d0: 6f6e 616c 292c 2069 6e20 7468 6174 2069  onal), in that i
+000008e0: 7420 6973 2064 6573 6967 6e65 6420 746f  t is designed to
+000008f0: 2062 6520 7573 6564 2061 7320 7468 6520   be used as the 
+00000900: 696d 706c 656d 656e 7461 7469 6f6e 2066  implementation f
+00000910: 6f72 2061 2064 6174 6120 6d6f 6465 6c2e  or a data model.
+00000920: 204f 6e65 2073 7563 6820 6578 616d 706c   One such exampl
+00000930: 6520 6973 2074 6865 205b 6772 6565 6b73  e is the [greeks
+00000940: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000950: 2e63 6f6d 2f73 7472 6561 6d6c 6574 2d64  .com/streamlet-d
+00000960: 6576 2f67 7265 656b 7329 206c 6962 7261  ev/greeks) libra
+00000970: 7279 2c20 7768 6963 6820 6c65 7665 7261  ry, which levera
+00000980: 6765 7320 7472 6962 7574 6172 7920 746f  ges tributary to
+00000990: 2062 7569 6c64 2064 6174 6120 6d6f 6465   build data mode
+000009a0: 6c73 2066 6f72 205b 6f70 7469 6f6e 7320  ls for [options 
+000009b0: 7072 6963 696e 675d 2868 7474 7073 3a2f  pricing](https:/
+000009c0: 2f77 7777 2e69 6e76 6573 746f 7065 6469  /www.investopedi
+000009d0: 612e 636f 6d2f 6172 7469 636c 6573 2f6f  a.com/articles/o
+000009e0: 7074 696f 6e69 6e76 6573 746f 722f 3037  ptioninvestor/07
+000009f0: 2f6f 7074 696f 6e73 5f62 6561 745f 6d61  /options_beat_ma
+00000a00: 726b 6574 2e61 7370 292e 200a 0a21 5b5d  rket.asp). ..![]
+00000a10: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00000a20: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000a30: 6f6d 2f73 7472 6561 6d6c 6574 2d64 6576  om/streamlet-dev
+00000a40: 2f74 7269 6275 7461 7279 2f6d 6169 6e2f  /tributary/main/
+00000a50: 646f 6373 2f69 6d67 2f65 7861 6d70 6c65  docs/img/example
+00000a60: 2e67 6966 290a 0a0a 2320 496e 7374 616c  .gif)...# Instal
+00000a70: 6c61 7469 6f6e 0a49 6e73 7461 6c6c 2077  lation.Install w
+00000a80: 6974 6820 7069 703a 0a0a 6070 6970 2069  ith pip:..`pip i
+00000a90: 6e73 7461 6c6c 2074 7269 6275 7461 7279  nstall tributary
+00000aa0: 600a 0a6f 7220 7769 7468 2063 6f6e 6461  `..or with conda
+00000ab0: 3a0a 0a60 636f 6e64 6120 696e 7374 616c  :..`conda instal
+00000ac0: 6c20 2d63 2063 6f6e 6461 2d66 6f72 6765  l -c conda-forge
+00000ad0: 2074 7269 6275 7461 7279 600a 0a6f 7220   tributary`..or 
+00000ae0: 6672 6f6d 2073 6f75 7263 653a 0a0a 6070  from source:..`p
+00000af0: 7974 686f 6e20 7365 7475 702e 7079 2069  ython setup.py i
+00000b00: 6e73 7461 6c6c 600a 0a4e 6f74 653a 2049  nstall`..Note: I
+00000b10: 6620 696e 7374 616c 6c69 6e67 2066 726f  f installing fro
+00000b20: 6d20 736f 7572 6365 206f 7220 7769 7468  m source or with
+00000b30: 2070 6970 2c20 796f 7527 6c6c 2061 6c73   pip, you'll als
+00000b40: 6f20 6e65 6564 205b 4772 6170 6876 697a  o need [Graphviz
+00000b50: 2069 7473 656c 665d 2868 7474 7073 3a2f   itself](https:/
+00000b60: 2f77 7777 2e67 7261 7068 7669 7a2e 6f72  /www.graphviz.or
+00000b70: 672f 646f 776e 6c6f 6164 2f29 2069 6620  g/download/) if 
+00000b80: 796f 7520 7761 6e74 2074 6f20 7669 7375  you want to visu
+00000b90: 616c 697a 6520 7468 6520 6772 6170 6820  alize the graph 
+00000ba0: 7573 696e 6720 7468 6520 602e 6772 6170  using the `.grap
+00000bb0: 6876 697a 2829 6020 6d65 7468 6f64 2e0a  hviz()` method..
+00000bc0: 0a23 2053 7472 6561 6d20 5479 7065 730a  .# Stream Types.
+00000bd0: 5472 6962 7574 6172 7920 6f66 6665 7273  Tributary offers
+00000be0: 2073 6576 6572 616c 206b 696e 6473 206f   several kinds o
+00000bf0: 6620 7374 7265 616d 733a 0a0a 2323 2053  f streams:..## S
+00000c00: 7472 6561 6d69 6e67 0a54 6865 7365 2061  treaming.These a
+00000c10: 7265 2073 796e 6368 726f 6e6f 7573 2c20  re synchronous, 
+00000c20: 7265 6163 7469 7665 2064 6174 6120 7374  reactive data st
+00000c30: 7265 616d 732c 2062 7569 6c74 2075 7369  reams, built usi
+00000c40: 6e67 2061 7379 6e63 6872 6f6e 6f75 7320  ng asynchronous 
+00000c50: 7079 7468 6f6e 2067 656e 6572 6174 6f72  python generator
+00000c60: 732e 2054 6865 7920 6172 6520 6465 7369  s. They are desi
+00000c70: 676e 6564 2074 6f20 6d69 6d69 6320 636f  gned to mimic co
+00000c80: 6d70 6c65 7820 6576 656e 7420 7072 6f63  mplex event proc
+00000c90: 6573 736f 7273 2069 6e20 7465 726d 7320  essors in terms 
+00000ca0: 6f66 2065 7665 6e74 206f 7264 6572 696e  of event orderin
+00000cb0: 672e 0a0a 2323 2046 756e 6374 696f 6e61  g...## Functiona
+00000cc0: 6c0a 5468 6573 6520 6172 6520 6675 6e63  l.These are func
+00000cd0: 7469 6f6e 616c 2073 7472 6561 6d73 2c20  tional streams, 
+00000ce0: 6275 696c 7420 6279 2063 7572 7279 696e  built by curryin
+00000cf0: 6720 7079 7468 6f6e 2066 756e 6374 696f  g python functio
+00000d00: 6e73 2028 6361 6c6c 6261 636b 7329 2e20  ns (callbacks). 
+00000d10: 0a0a 2323 204c 617a 790a 5468 6573 6520  ..## Lazy.These 
+00000d20: 6172 6520 6c61 7a69 6c79 2d65 7661 6c75  are lazily-evalu
+00000d30: 6174 6564 2070 7974 686f 6e20 7374 7265  ated python stre
+00000d40: 616d 732c 2077 6865 7265 206f 7574 7075  ams, where outpu
+00000d50: 7473 2061 7265 2070 726f 706f 6761 7465  ts are propogate
+00000d60: 6420 6f6e 6c79 2061 7320 696e 7075 7473  d only as inputs
+00000d70: 2063 6861 6e67 652e 2054 6865 7920 6172   change. They ar
+00000d80: 6520 696d 706c 656d 656e 7465 6420 6173  e implemented as
+00000d90: 2064 6972 6563 7465 6420 6163 7963 6c69   directed acycli
+00000da0: 6320 6772 6170 6873 2e0a 0a23 2045 7861  c graphs...# Exa
+00000db0: 6d70 6c65 730a 2d20 5b53 7472 6561 6d69  mples.- [Streami
+00000dc0: 6e67 5d28 646f 6373 2f65 7861 6d70 6c65  ng](docs/example
+00000dd0: 732f 7374 7265 616d 696e 672f 7374 7265  s/streaming/stre
+00000de0: 616d 696e 672e 6d64 293a 2049 6e20 7468  aming.md): In th
+00000df0: 6973 2065 7861 6d70 6c65 2c20 7765 2063  is example, we c
+00000e00: 6f6e 7374 7275 6374 2061 2076 6172 6965  onstruct a varie
+00000e10: 7479 206f 6620 666f 7277 6172 6420 7072  ty of forward pr
+00000e20: 6f70 6f67 6174 696e 6720 7265 6163 7469  opogating reacti
+00000e30: 7665 2067 7261 7068 732e 0a2d 205b 4c61  ve graphs..- [La
+00000e40: 7a79 5d28 646f 6373 2f65 7861 6d70 6c65  zy](docs/example
+00000e50: 732f 6c61 7a79 2f6c 617a 792e 6d64 293a  s/lazy/lazy.md):
+00000e60: 2049 6e20 7468 6973 2065 7861 6d70 6c65   In this example
+00000e70: 2c20 7765 2063 6f6e 7374 7275 6374 2061  , we construct a
+00000e80: 2076 6172 6965 7479 206f 6620 6c61 7a69   variety of lazi
+00000e90: 6c79 2d65 7661 6c75 6174 6564 2064 6972  ly-evaluated dir
+00000ea0: 6563 7465 6420 6163 7963 6c69 6320 636f  ected acyclic co
+00000eb0: 6d70 7574 6174 696f 6e20 6772 6170 6873  mputation graphs
+00000ec0: 2e20 0a2d 205b 4175 746f 6d61 7469 6320  . .- [Automatic 
+00000ed0: 4469 6666 6572 656e 7469 6174 696f 6e5d  Differentiation]
+00000ee0: 2864 6f63 732f 6578 616d 706c 6573 2f61  (docs/examples/a
+00000ef0: 7574 6f64 6966 662f 6175 746f 6469 6666  utodiff/autodiff
+00000f00: 2e6d 6429 3a20 496e 2074 6869 7320 6578  .md): In this ex
+00000f10: 616d 706c 652c 2077 6520 7573 6520 6074  ample, we use `t
+00000f20: 7269 6275 7461 7279 6020 746f 2070 6572  ributary` to per
+00000f30: 666f 726d 2061 7574 6f6d 6174 6963 2064  form automatic d
+00000f40: 6966 6665 7265 6e74 6961 7469 6f6e 206f  ifferentiation o
+00000f50: 6e20 626f 7468 206c 617a 7920 616e 6420  n both lazy and 
+00000f60: 7374 7265 616d 696e 6720 6772 6170 6873  streaming graphs
+00000f70: 2e0a 0a23 2047 7261 7068 2056 6973 7561  ...# Graph Visua
+00000f80: 6c69 7a61 7469 6f6e 0a59 6f75 2063 616e  lization.You can
+00000f90: 2076 6973 7561 6c69 7a65 2074 6865 2067   visualize the g
+00000fa0: 7261 7068 2077 6974 6820 4772 6170 6876  raph with Graphv
+00000fb0: 697a 2e20 416c 6c20 7374 7265 616d 696e  iz. All streamin
+00000fc0: 6720 616e 6420 6c61 7a79 206e 6f64 6573  g and lazy nodes
+00000fd0: 2073 7570 706f 7274 2061 2060 6772 6170   support a `grap
+00000fe0: 6876 697a 6020 6d65 7468 6f64 2e0a 0a53  hviz` method...S
+00000ff0: 7472 6561 6d69 6e67 2061 6e64 206c 617a  treaming and laz
+00001000: 7920 6e6f 6465 7320 616c 736f 2073 7570  y nodes also sup
+00001010: 706f 7274 205b 6970 7964 6167 7265 6433  port [ipydagred3
+00001020: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001030: 2e63 6f6d 2f74 696d 6b70 6169 6e65 2f69  .com/timkpaine/i
+00001040: 7079 6461 6772 6564 3329 2066 6f72 206c  pydagred3) for l
+00001050: 6976 6520 7570 6461 7465 206d 6f6e 6974  ive update monit
+00001060: 6f72 696e 672e 0a0a 2323 2053 7472 6561  oring...## Strea
+00001070: 6d69 6e67 0a21 5b5d 2868 7474 7073 3a2f  ming.![](https:/
+00001080: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001090: 6f6e 7465 6e74 2e63 6f6d 2f73 7472 6561  ontent.com/strea
+000010a0: 6d6c 6574 2d64 6576 2f74 7269 6275 7461  mlet-dev/tributa
+000010b0: 7279 2f6d 6169 6e2f 646f 6373 2f69 6d67  ry/main/docs/img
+000010c0: 2f73 7472 6561 6d69 6e67 2f64 6167 7265  /streaming/dagre
+000010d0: 6433 2e67 6966 290a 0a48 6572 6520 6772  d3.gif)..Here gr
+000010e0: 6565 6e20 696e 6469 6361 7465 7320 6578  een indicates ex
+000010f0: 6563 7574 696e 672c 2079 656c 6c6f 7720  ecuting, yellow 
+00001100: 696e 6469 6361 7465 7320 7374 616c 6c65  indicates stalle
+00001110: 6420 666f 7220 6261 636b 7072 6573 7375  d for backpressu
+00001120: 7265 2c20 616e 6420 7265 6420 696e 6469  re, and red indi
+00001130: 6361 7465 7320 7468 6174 2060 5374 7265  cates that `Stre
+00001140: 616d 456e 6460 2068 6173 2062 6565 6e20  amEnd` has been 
+00001150: 7072 6f70 6f67 6174 6564 2028 652e 672e  propogated (e.g.
+00001160: 2073 7472 6561 6d20 6861 7320 656e 6465   stream has ende
+00001170: 6429 2e0a 0a23 2320 4c61 7a79 0a21 5b5d  d)...## Lazy.![]
+00001180: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00001190: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000011a0: 6f6d 2f73 7472 6561 6d6c 6574 2d64 6576  om/streamlet-dev
+000011b0: 2f74 7269 6275 7461 7279 2f6d 6169 6e2f  /tributary/main/
+000011c0: 646f 6373 2f69 6d67 2f6c 617a 792f 6461  docs/img/lazy/da
+000011d0: 6772 6564 332e 6769 6629 0a0a 4865 7265  gred3.gif)..Here
+000011e0: 2067 7265 656e 2069 6e64 6963 6174 6573   green indicates
+000011f0: 2065 7865 6375 7469 6e67 2c20 616e 6420   executing, and 
+00001200: 7265 6420 696e 6469 6361 7465 7320 7468  red indicates th
+00001210: 6174 2074 6865 206e 6f64 6520 6973 2064  at the node is d
+00001220: 6972 7479 2e20 4e6f 7465 2074 6865 2074  irty. Note the t
+00001230: 6865 2064 6574 6572 6d69 6e61 7469 6f6e  he determination
+00001240: 2069 6620 6120 6e6f 6465 2069 7320 6469   if a node is di
+00001250: 7274 7920 6973 2061 6c73 6f20 646f 6e65  rty is also done
+00001260: 206c 617a 696c 7920 2877 6520 6361 6e20   lazily (we can 
+00001270: 6368 6563 6b20 7769 7468 2060 6973 4469  check with `isDi
+00001280: 7274 7960 2077 6863 6968 2077 696c 6c20  rty` whcih will 
+00001290: 7570 6461 7465 2074 6865 206e 6f64 6527  update the node'
+000012a0: 7320 6772 6170 6820 7374 6174 652e 0a0a  s graph state...
+000012b0: 2323 2043 6174 616c 6f67 0a53 6565 2074  ## Catalog.See t
+000012c0: 6865 205b 4341 5441 4c4f 475d 2843 4154  he [CATALOG](CAT
+000012d0: 414c 4f47 2e6d 6429 2066 6f72 2061 2066  ALOG.md) for a f
+000012e0: 756c 6c20 6c69 7374 206f 6620 6675 6e63  ull list of func
+000012f0: 7469 6f6e 732c 2074 7261 6e73 666f 726d  tions, transform
+00001300: 732c 2073 6f75 7263 6573 2c20 616e 6420  s, sources, and 
+00001310: 7369 6e6b 732e 0a0a 2323 2053 7570 706f  sinks...## Suppo
+00001320: 7274 202f 2043 6f6e 7472 6962 7574 6f72  rt / Contributor
+00001330: 730a 5468 616e 6b73 2074 6f20 7468 6520  s.Thanks to the 
+00001340: 666f 6c6c 6f77 696e 6720 6f72 6761 6e69  following organi
+00001350: 7a61 7469 6f6e 7320 666f 7220 7072 6f76  zations for prov
+00001360: 6964 696e 6720 636f 6465 206f 7220 6669  iding code or fi
+00001370: 6e61 6e63 6961 6c20 7375 7070 6f72 742e  nancial support.
+00001380: 0a0a 0a3c 6120 6872 6566 3d22 6874 7470  ...<a href="http
+00001390: 733a 2f2f 6e65 6d6f 756c 6f75 732e 636f  s://nemoulous.co
+000013a0: 6d22 3e3c 696d 6720 7372 633d 2268 7474  m"><img src="htt
+000013b0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000013c0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+000013d0: 7472 6561 6d6c 6574 2d64 6576 2f74 7269  treamlet-dev/tri
+000013e0: 6275 7461 7279 2f6d 6169 6e2f 646f 6373  butary/main/docs
+000013f0: 2f69 6d67 2f6e 656d 2e70 6e67 2220 7769  /img/nem.png" wi
+00001400: 6474 683d 2235 3022 3e3c 2f61 3e0a 0a3c  dth="50"></a>..<
+00001410: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001420: 6e65 6d6f 756c 6f75 732e 636f 6d22 3e4e  nemoulous.com">N
+00001430: 656d 6f75 6c6f 7573 3c2f 613e 0a0a 2323  emoulous</a>..##
+00001440: 204c 6963 656e 7365 0a54 6869 7320 736f   License.This so
+00001450: 6674 7761 7265 2069 7320 6c69 6365 6e73  ftware is licens
+00001460: 6564 2075 6e64 6572 2074 6865 2041 7061  ed under the Apa
+00001470: 6368 6520 322e 3020 6c69 6365 6e73 652e  che 2.0 license.
+00001480: 2053 6565 2074 6865 205b 4c49 4345 4e53   See the [LICENS
+00001490: 455d 284c 4943 454e 5345 2920 6669 6c65  E](LICENSE) file
+000014a0: 2066 6f72 2064 6574 6169 6c73 2e0a 0a23   for details...#
+000014b0: 2320 416c 7465 726e 6174 6976 6573 0a48  # Alternatives.H
+000014c0: 6572 6520 6973 2061 6e20 696e 636f 6d70  ere is an incomp
+000014d0: 6c65 7465 206c 6973 7420 6f66 206c 6962  lete list of lib
+000014e0: 7261 7269 6573 2077 6869 6368 2069 6d70  raries which imp
+000014f0: 6c65 6d65 6e74 2073 696d 696c 6172 2f6f  lement similar/o
+00001500: 7665 726c 6170 7069 6e67 2066 756e 6374  verlapping funct
+00001510: 696f 6e61 6c69 7479 0a0a 2d20 5b6d 616e  ionality..- [man
+00001520: 2d67 726f 7570 2f6d 6466 5d28 6874 7470  -group/mdf](http
+00001530: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00001540: 616e 2d67 726f 7570 2f6d 6466 290a 2d20  an-group/mdf).- 
+00001550: 5b63 6564 7269 636c 6572 6f79 2f70 7975  [cedricleroy/pyu
+00001560: 6e67 6f5d 2868 7474 7073 3a2f 2f67 6974  ngo](https://git
+00001570: 6875 622e 636f 6d2f 6365 6472 6963 6c65  hub.com/cedricle
+00001580: 726f 792f 7079 756e 676f 290a 2d20 5b70  roy/pyungo).- [p
+00001590: 7974 686f 6e2d 7374 7265 616d 7a2f 7374  ython-streamz/st
+000015a0: 7265 616d 7a5d 2868 7474 7073 3a2f 2f67  reamz](https://g
+000015b0: 6974 6875 622e 636f 6d2f 7079 7468 6f6e  ithub.com/python
+000015c0: 2d73 7472 6561 6d7a 2f73 7472 6561 6d7a  -streamz/streamz
+000015d0: 290a 2d20 5b45 6e74 696c 5a68 612f 7079  ).- [EntilZha/py
+000015e0: 6675 6e63 7469 6f6e 616c 5d28 6874 7470  functional](http
+000015f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
+00001600: 6e74 696c 5a68 612f 5079 4675 6e63 7469  ntilZha/PyFuncti
+00001610: 6f6e 616c 290a 2d20 5b73 7469 7463 6866  onal).- [stitchf
+00001620: 6978 2f68 616d 696c 746f 6e5d 2868 7474  ix/hamilton](htt
+00001630: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001640: 7374 6974 6368 6669 782f 6861 6d69 6c74  stitchfix/hamilt
+00001650: 6f6e 290a 0a                             on)..
```

### Comparing `tributary-0.2.0/README.md` & `tributary-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,308 +1,311 @@
-00000000: 2320 3c61 2068 7265 663d 2268 7474 7073  # <a href="https
-00000010: 3a2f 2f74 7269 6275 7461 7279 2e72 6561  ://tributary.rea
-00000020: 6474 6865 646f 6373 2e69 6f22 3e3c 696d  dthedocs.io"><im
-00000030: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00000040: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000050: 7465 6e74 2e63 6f6d 2f74 696d 6b70 6169  tent.com/timkpai
-00000060: 6e65 2f74 7269 6275 7461 7279 2f6d 6169  ne/tributary/mai
-00000070: 6e2f 646f 6373 2f69 6d67 2f69 636f 6e2e  n/docs/img/icon.
-00000080: 706e 6722 2077 6964 7468 3d22 3330 3022  png" width="300"
-00000090: 3e3c 2f61 3e0a 5079 7468 6f6e 2044 6174  ></a>.Python Dat
-000000a0: 6120 5374 7265 616d 730a 0a5b 215b 4275  a Streams..[![Bu
-000000b0: 696c 6420 5374 6174 7573 5d28 6874 7470  ild Status](http
-000000c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-000000d0: 696d 6b70 6169 6e65 2f74 7269 6275 7461  imkpaine/tributa
-000000e0: 7279 2f77 6f72 6b66 6c6f 7773 2f42 7569  ry/workflows/Bui
-000000f0: 6c64 2532 3053 7461 7475 732f 6261 6467  ld%20Status/badg
-00000100: 652e 7376 673f 6272 616e 6368 3d6d 6169  e.svg?branch=mai
-00000110: 6e29 5d28 6874 7470 733a 2f2f 6769 7468  n)](https://gith
-00000120: 7562 2e63 6f6d 2f74 696d 6b70 6169 6e65  ub.com/timkpaine
-00000130: 2f74 7269 6275 7461 7279 2f61 6374 696f  /tributary/actio
-00000140: 6e73 3f71 7565 7279 3d77 6f72 6b66 6c6f  ns?query=workflo
-00000150: 7725 3341 2532 3242 7569 6c64 2b53 7461  w%3A%22Build+Sta
-00000160: 7475 7325 3232 290a 5b21 5b43 6f76 6572  tus%22).[![Cover
-00000170: 6167 655d 2868 7474 7073 3a2f 2f63 6f64  age](https://cod
-00000180: 6563 6f76 2e69 6f2f 6768 2f74 696d 6b70  ecov.io/gh/timkp
-00000190: 6169 6e65 2f74 7269 6275 7461 7279 2f62  aine/tributary/b
-000001a0: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
-000001b0: 2f62 6164 6765 2e73 7667 295d 2868 7474  /badge.svg)](htt
-000001c0: 7073 3a2f 2f63 6f64 6563 6f76 2e69 6f2f  ps://codecov.io/
-000001d0: 6768 2f74 696d 6b70 6169 6e65 2f74 7269  gh/timkpaine/tri
-000001e0: 6275 7461 7279 290a 5b21 5b50 7950 495d  butary).[![PyPI]
-000001f0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000200: 656c 6473 2e69 6f2f 7079 7069 2f6c 2f74  elds.io/pypi/l/t
-00000210: 7269 6275 7461 7279 2e73 7667 295d 2868  ributary.svg)](h
-00000220: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
-00000230: 6f6e 2e6f 7267 2f70 7970 692f 7472 6962  on.org/pypi/trib
-00000240: 7574 6172 7929 0a5b 215b 5079 5049 5d28  utary).[![PyPI](
-00000250: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000260: 6c64 732e 696f 2f70 7970 692f 762f 7472  lds.io/pypi/v/tr
-00000270: 6962 7574 6172 792e 7376 6729 5d28 6874  ibutary.svg)](ht
-00000280: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
-00000290: 6e2e 6f72 672f 7079 7069 2f74 7269 6275  n.org/pypi/tribu
-000002a0: 7461 7279 290a 5b21 5b42 696e 6465 725d  tary).[![Binder]
-000002b0: 2868 7474 7073 3a2f 2f6d 7962 696e 6465  (https://mybinde
-000002c0: 722e 6f72 672f 6261 6467 655f 6c6f 676f  r.org/badge_logo
-000002d0: 2e73 7667 295d 2868 7474 7073 3a2f 2f6d  .svg)](https://m
-000002e0: 7962 696e 6465 722e 6f72 672f 7632 2f67  ybinder.org/v2/g
-000002f0: 682f 7469 6d6b 7061 696e 652f 7472 6962  h/timkpaine/trib
-00000300: 7574 6172 792f 6d61 696e 3f75 726c 7061  utary/main?urlpa
-00000310: 7468 3d6c 6162 290a 0a0a 5472 6962 7574  th=lab)...Tribut
-00000320: 6172 7920 6973 2061 206c 6962 7261 7279  ary is a library
-00000330: 2066 6f72 2063 6f6e 7374 7275 6374 696e   for constructin
-00000340: 6720 6461 7461 666c 6f77 2067 7261 7068  g dataflow graph
-00000350: 7320 696e 2070 7974 686f 6e2e 2055 6e6c  s in python. Unl
-00000360: 696b 6520 6d61 6e79 206f 7468 6572 2044  ike many other D
-00000370: 4147 206c 6962 7261 7269 6573 2069 6e20  AG libraries in 
-00000380: 7079 7468 6f6e 2028 5b61 6972 666c 6f77  python ([airflow
-00000390: 5d28 6874 7470 733a 2f2f 6169 7266 6c6f  ](https://airflo
-000003a0: 772e 6170 6163 6865 2e6f 7267 292c 205b  w.apache.org), [
-000003b0: 6c75 6967 695d 2868 7474 7073 3a2f 2f6c  luigi](https://l
-000003c0: 7569 6769 2e72 6561 6474 6865 646f 6373  uigi.readthedocs
-000003d0: 2e69 6f2f 656e 2f73 7461 626c 652f 292c  .io/en/stable/),
-000003e0: 205b 7072 6566 6563 745d 2868 7474 7073   [prefect](https
-000003f0: 3a2f 2f64 6f63 732e 7072 6566 6563 742e  ://docs.prefect.
-00000400: 696f 292c 205b 6461 6773 7465 725d 2868  io), [dagster](h
-00000410: 7474 7073 3a2f 2f64 6f63 732e 6461 6773  ttps://docs.dags
-00000420: 7465 722e 696f 292c 205b 6461 736b 5d28  ter.io), [dask](
-00000430: 6874 7470 733a 2f2f 6461 736b 2e6f 7267  https://dask.org
-00000440: 292c 205b 6b65 6472 6f5d 2868 7474 7073  ), [kedro](https
-00000450: 3a2f 2f67 6974 6875 622e 636f 6d2f 7175  ://github.com/qu
-00000460: 616e 7475 6d62 6c61 636b 6c61 6273 2f6b  antumblacklabs/k
-00000470: 6564 726f 292c 2065 7463 292c 2074 7269  edro), etc), tri
-00000480: 6275 7461 7279 2069 7320 6e6f 7420 6465  butary is not de
-00000490: 7369 676e 6564 2077 6974 6820 6461 7461  signed with data
-000004a0: 2f65 746c 2070 6970 656c 696e 6573 206f  /etl pipelines o
-000004b0: 7220 7363 6865 6475 6c69 6e67 2069 6e20  r scheduling in 
-000004c0: 6d69 6e64 2e20 496e 7374 6561 642c 2074  mind. Instead, t
-000004d0: 7269 6275 7461 7279 2069 7320 6d6f 7265  ributary is more
-000004e0: 2073 696d 696c 6172 2074 6f20 6c69 6272   similar to libr
-000004f0: 6172 6965 7320 6c69 6b65 205b 6d64 665d  aries like [mdf]
-00000500: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000510: 636f 6d2f 6d61 6e2d 6772 6f75 702f 6d64  com/man-group/md
-00000520: 6629 2c20 5b70 7975 6e67 6f5d 2868 7474  f), [pyungo](htt
-00000530: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000540: 6365 6472 6963 6c65 726f 792f 7079 756e  cedricleroy/pyun
-00000550: 676f 292c 205b 7374 7265 616d 7a5d 2868  go), [streamz](h
-00000560: 7474 7073 3a2f 2f73 7472 6561 6d7a 2e72  ttps://streamz.r
-00000570: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000580: 2f6c 6174 6573 742f 292c 206f 7220 5b70  /latest/), or [p
-00000590: 7966 756e 6374 696f 6e61 6c5d 2868 7474  yfunctional](htt
-000005a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000005b0: 456e 7469 6c5a 6861 2f50 7946 756e 6374  EntilZha/PyFunct
-000005c0: 696f 6e61 6c29 2c20 696e 2074 6861 7420  ional), in that 
-000005d0: 6974 2069 7320 6465 7369 676e 6564 2074  it is designed t
-000005e0: 6f20 6265 2075 7365 6420 6173 2074 6865  o be used as the
-000005f0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-00000600: 666f 7220 6120 6461 7461 206d 6f64 656c  for a data model
-00000610: 2e20 4f6e 6520 7375 6368 2065 7861 6d70  . One such examp
-00000620: 6c65 2069 7320 7468 6520 5b67 7265 656b  le is the [greek
-00000630: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00000640: 622e 636f 6d2f 7469 6d6b 7061 696e 652f  b.com/timkpaine/
-00000650: 6772 6565 6b73 2920 6c69 6272 6172 792c  greeks) library,
-00000660: 2077 6869 6368 206c 6576 6572 6167 6573   which leverages
-00000670: 2074 7269 6275 7461 7279 2074 6f20 6275   tributary to bu
-00000680: 696c 6420 6461 7461 206d 6f64 656c 7320  ild data models 
-00000690: 666f 7220 5b6f 7074 696f 6e73 2070 7269  for [options pri
-000006a0: 6369 6e67 5d28 6874 7470 733a 2f2f 7777  cing](https://ww
-000006b0: 772e 696e 7665 7374 6f70 6564 6961 2e63  w.investopedia.c
-000006c0: 6f6d 2f61 7274 6963 6c65 732f 6f70 7469  om/articles/opti
-000006d0: 6f6e 696e 7665 7374 6f72 2f30 372f 6f70  oninvestor/07/op
-000006e0: 7469 6f6e 735f 6265 6174 5f6d 6172 6b65  tions_beat_marke
-000006f0: 742e 6173 7029 2e20 0a0a 215b 5d28 6874  t.asp). ..![](ht
-00000700: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00000710: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00000720: 7469 6d6b 7061 696e 652f 7472 6962 7574  timkpaine/tribut
-00000730: 6172 792f 6d61 696e 2f64 6f63 732f 696d  ary/main/docs/im
-00000740: 672f 6578 616d 706c 652e 6769 6629 0a0a  g/example.gif)..
-00000750: 0a23 2049 6e73 7461 6c6c 6174 696f 6e0a  .# Installation.
-00000760: 496e 7374 616c 6c20 7769 7468 2070 6970  Install with pip
-00000770: 3a0a 0a60 7069 7020 696e 7374 616c 6c20  :..`pip install 
-00000780: 7472 6962 7574 6172 7960 0a0a 6f72 2077  tributary`..or w
-00000790: 6974 6820 636f 6e64 613a 0a0a 6063 6f6e  ith conda:..`con
-000007a0: 6461 2069 6e73 7461 6c6c 202d 6320 636f  da install -c co
-000007b0: 6e64 612d 666f 7267 6520 7472 6962 7574  nda-forge tribut
-000007c0: 6172 7960 0a0a 6f72 2066 726f 6d20 736f  ary`..or from so
-000007d0: 7572 6365 3a0a 0a60 7079 7468 6f6e 2073  urce:..`python s
-000007e0: 6574 7570 2e70 7920 696e 7374 616c 6c60  etup.py install`
-000007f0: 0a0a 4e6f 7465 3a20 4966 2069 6e73 7461  ..Note: If insta
-00000800: 6c6c 696e 6720 6672 6f6d 2073 6f75 7263  lling from sourc
-00000810: 6520 6f72 2077 6974 6820 7069 702c 2079  e or with pip, y
-00000820: 6f75 276c 6c20 616c 736f 206e 6565 6420  ou'll also need 
-00000830: 5b47 7261 7068 7669 7a20 6974 7365 6c66  [Graphviz itself
-00000840: 5d28 6874 7470 733a 2f2f 7777 772e 6772  ](https://www.gr
-00000850: 6170 6876 697a 2e6f 7267 2f64 6f77 6e6c  aphviz.org/downl
-00000860: 6f61 642f 2920 6966 2079 6f75 2077 616e  oad/) if you wan
-00000870: 7420 746f 2076 6973 7561 6c69 7a65 2074  t to visualize t
-00000880: 6865 2067 7261 7068 2075 7369 6e67 2074  he graph using t
-00000890: 6865 2060 2e67 7261 7068 7669 7a28 2960  he `.graphviz()`
-000008a0: 206d 6574 686f 642e 0a0a 2320 5374 7265   method...# Stre
-000008b0: 616d 2054 7970 6573 0a54 7269 6275 7461  am Types.Tributa
-000008c0: 7279 206f 6666 6572 7320 7365 7665 7261  ry offers severa
-000008d0: 6c20 6b69 6e64 7320 6f66 2073 7472 6561  l kinds of strea
-000008e0: 6d73 3a0a 0a23 2320 5374 7265 616d 696e  ms:..## Streamin
-000008f0: 670a 5468 6573 6520 6172 6520 7379 6e63  g.These are sync
-00000900: 6872 6f6e 6f75 732c 2072 6561 6374 6976  hronous, reactiv
-00000910: 6520 6461 7461 2073 7472 6561 6d73 2c20  e data streams, 
-00000920: 6275 696c 7420 7573 696e 6720 6173 796e  built using asyn
-00000930: 6368 726f 6e6f 7573 2070 7974 686f 6e20  chronous python 
-00000940: 6765 6e65 7261 746f 7273 2e20 5468 6579  generators. They
-00000950: 2061 7265 2064 6573 6967 6e65 6420 746f   are designed to
-00000960: 206d 696d 6963 2063 6f6d 706c 6578 2065   mimic complex e
-00000970: 7665 6e74 2070 726f 6365 7373 6f72 7320  vent processors 
-00000980: 696e 2074 6572 6d73 206f 6620 6576 656e  in terms of even
-00000990: 7420 6f72 6465 7269 6e67 2e0a 0a23 2320  t ordering...## 
-000009a0: 4675 6e63 7469 6f6e 616c 0a54 6865 7365  Functional.These
-000009b0: 2061 7265 2066 756e 6374 696f 6e61 6c20   are functional 
-000009c0: 7374 7265 616d 732c 2062 7569 6c74 2062  streams, built b
-000009d0: 7920 6375 7272 7969 6e67 2070 7974 686f  y currying pytho
-000009e0: 6e20 6675 6e63 7469 6f6e 7320 2863 616c  n functions (cal
-000009f0: 6c62 6163 6b73 292e 200a 0a23 2320 4c61  lbacks). ..## La
-00000a00: 7a79 0a54 6865 7365 2061 7265 206c 617a  zy.These are laz
-00000a10: 696c 792d 6576 616c 7561 7465 6420 7079  ily-evaluated py
-00000a20: 7468 6f6e 2073 7472 6561 6d73 2c20 7768  thon streams, wh
-00000a30: 6572 6520 6f75 7470 7574 7320 6172 6520  ere outputs are 
-00000a40: 7072 6f70 6f67 6174 6564 206f 6e6c 7920  propogated only 
-00000a50: 6173 2069 6e70 7574 7320 6368 616e 6765  as inputs change
-00000a60: 2e20 5468 6579 2061 7265 2069 6d70 6c65  . They are imple
-00000a70: 6d65 6e74 6564 2061 7320 6469 7265 6374  mented as direct
-00000a80: 6564 2061 6379 636c 6963 2067 7261 7068  ed acyclic graph
-00000a90: 732e 0a0a 2320 4578 616d 706c 6573 0a2d  s...# Examples.-
-00000aa0: 205b 5374 7265 616d 696e 675d 2864 6f63   [Streaming](doc
-00000ab0: 732f 6578 616d 706c 6573 2f73 7472 6561  s/examples/strea
-00000ac0: 6d69 6e67 2f73 7472 6561 6d69 6e67 2e6d  ming/streaming.m
-00000ad0: 6429 3a20 496e 2074 6869 7320 6578 616d  d): In this exam
-00000ae0: 706c 652c 2077 6520 636f 6e73 7472 7563  ple, we construc
-00000af0: 7420 6120 7661 7269 6574 7920 6f66 2066  t a variety of f
-00000b00: 6f72 7761 7264 2070 726f 706f 6761 7469  orward propogati
-00000b10: 6e67 2072 6561 6374 6976 6520 6772 6170  ng reactive grap
-00000b20: 6873 2e0a 2d20 5b4c 617a 795d 2864 6f63  hs..- [Lazy](doc
-00000b30: 732f 6578 616d 706c 6573 2f6c 617a 792f  s/examples/lazy/
-00000b40: 6c61 7a79 2e6d 6429 3a20 496e 2074 6869  lazy.md): In thi
-00000b50: 7320 6578 616d 706c 652c 2077 6520 636f  s example, we co
-00000b60: 6e73 7472 7563 7420 6120 7661 7269 6574  nstruct a variet
-00000b70: 7920 6f66 206c 617a 696c 792d 6576 616c  y of lazily-eval
-00000b80: 7561 7465 6420 6469 7265 6374 6564 2061  uated directed a
-00000b90: 6379 636c 6963 2063 6f6d 7075 7461 7469  cyclic computati
-00000ba0: 6f6e 2067 7261 7068 732e 200a 2d20 5b41  on graphs. .- [A
-00000bb0: 7574 6f6d 6174 6963 2044 6966 6665 7265  utomatic Differe
-00000bc0: 6e74 6961 7469 6f6e 5d28 646f 6373 2f65  ntiation](docs/e
-00000bd0: 7861 6d70 6c65 732f 6175 746f 6469 6666  xamples/autodiff
-00000be0: 2f61 7574 6f64 6966 662e 6d64 293a 2049  /autodiff.md): I
-00000bf0: 6e20 7468 6973 2065 7861 6d70 6c65 2c20  n this example, 
-00000c00: 7765 2075 7365 2060 7472 6962 7574 6172  we use `tributar
-00000c10: 7960 2074 6f20 7065 7266 6f72 6d20 6175  y` to perform au
-00000c20: 746f 6d61 7469 6320 6469 6666 6572 656e  tomatic differen
-00000c30: 7469 6174 696f 6e20 6f6e 2062 6f74 6820  tiation on both 
-00000c40: 6c61 7a79 2061 6e64 2073 7472 6561 6d69  lazy and streami
-00000c50: 6e67 2067 7261 7068 732e 0a0a 2320 4772  ng graphs...# Gr
-00000c60: 6170 6820 5669 7375 616c 697a 6174 696f  aph Visualizatio
-00000c70: 6e0a 596f 7520 6361 6e20 7669 7375 616c  n.You can visual
-00000c80: 697a 6520 7468 6520 6772 6170 6820 7769  ize the graph wi
-00000c90: 7468 2047 7261 7068 7669 7a2e 2041 6c6c  th Graphviz. All
-00000ca0: 2073 7472 6561 6d69 6e67 2061 6e64 206c   streaming and l
-00000cb0: 617a 7920 6e6f 6465 7320 7375 7070 6f72  azy nodes suppor
-00000cc0: 7420 6120 6067 7261 7068 7669 7a60 206d  t a `graphviz` m
-00000cd0: 6574 686f 642e 0a0a 5374 7265 616d 696e  ethod...Streamin
-00000ce0: 6720 616e 6420 6c61 7a79 206e 6f64 6573  g and lazy nodes
-00000cf0: 2061 6c73 6f20 7375 7070 6f72 7420 5b69   also support [i
-00000d00: 7079 6461 6772 6564 335d 2868 7474 7073  pydagred3](https
-00000d10: 3a2f 2f67 6974 6875 622e 636f 6d2f 7469  ://github.com/ti
-00000d20: 6d6b 7061 696e 652f 6970 7964 6167 7265  mkpaine/ipydagre
-00000d30: 6433 2920 666f 7220 6c69 7665 2075 7064  d3) for live upd
-00000d40: 6174 6520 6d6f 6e69 746f 7269 6e67 2e0a  ate monitoring..
-00000d50: 0a23 2320 5374 7265 616d 696e 670a 215b  .## Streaming.![
-00000d60: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
-00000d70: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000d80: 636f 6d2f 7469 6d6b 7061 696e 652f 7472  com/timkpaine/tr
-00000d90: 6962 7574 6172 792f 6d61 696e 2f64 6f63  ibutary/main/doc
-00000da0: 732f 696d 672f 7374 7265 616d 696e 672f  s/img/streaming/
-00000db0: 6461 6772 6564 332e 6769 6629 0a0a 4865  dagred3.gif)..He
-00000dc0: 7265 2067 7265 656e 2069 6e64 6963 6174  re green indicat
-00000dd0: 6573 2065 7865 6375 7469 6e67 2c20 7965  es executing, ye
-00000de0: 6c6c 6f77 2069 6e64 6963 6174 6573 2073  llow indicates s
-00000df0: 7461 6c6c 6564 2066 6f72 2062 6163 6b70  talled for backp
-00000e00: 7265 7373 7572 652c 2061 6e64 2072 6564  ressure, and red
-00000e10: 2069 6e64 6963 6174 6573 2074 6861 7420   indicates that 
-00000e20: 6053 7472 6561 6d45 6e64 6020 6861 7320  `StreamEnd` has 
-00000e30: 6265 656e 2070 726f 706f 6761 7465 6420  been propogated 
-00000e40: 2865 2e67 2e20 7374 7265 616d 2068 6173  (e.g. stream has
-00000e50: 2065 6e64 6564 292e 0a0a 2323 204c 617a   ended)...## Laz
-00000e60: 790a 215b 5d28 6874 7470 733a 2f2f 7261  y.![](https://ra
-00000e70: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000e80: 656e 742e 636f 6d2f 7469 6d6b 7061 696e  ent.com/timkpain
-00000e90: 652f 7472 6962 7574 6172 792f 6d61 696e  e/tributary/main
-00000ea0: 2f64 6f63 732f 696d 672f 6c61 7a79 2f64  /docs/img/lazy/d
-00000eb0: 6167 7265 6433 2e67 6966 290a 0a48 6572  agred3.gif)..Her
-00000ec0: 6520 6772 6565 6e20 696e 6469 6361 7465  e green indicate
-00000ed0: 7320 6578 6563 7574 696e 672c 2061 6e64  s executing, and
-00000ee0: 2072 6564 2069 6e64 6963 6174 6573 2074   red indicates t
-00000ef0: 6861 7420 7468 6520 6e6f 6465 2069 7320  hat the node is 
-00000f00: 6469 7274 792e 204e 6f74 6520 7468 6520  dirty. Note the 
-00000f10: 7468 6520 6465 7465 726d 696e 6174 696f  the determinatio
-00000f20: 6e20 6966 2061 206e 6f64 6520 6973 2064  n if a node is d
-00000f30: 6972 7479 2069 7320 616c 736f 2064 6f6e  irty is also don
-00000f40: 6520 6c61 7a69 6c79 2028 7765 2063 616e  e lazily (we can
-00000f50: 2063 6865 636b 2077 6974 6820 6069 7344   check with `isD
-00000f60: 6972 7479 6020 7768 6369 6820 7769 6c6c  irty` whcih will
-00000f70: 2075 7064 6174 6520 7468 6520 6e6f 6465   update the node
-00000f80: 2773 2067 7261 7068 2073 7461 7465 2e0a  's graph state..
-00000f90: 0a23 2320 4361 7461 6c6f 670a 5365 6520  .## Catalog.See 
-00000fa0: 7468 6520 5b43 4154 414c 4f47 5d28 4341  the [CATALOG](CA
-00000fb0: 5441 4c4f 472e 6d64 2920 666f 7220 6120  TALOG.md) for a 
-00000fc0: 6675 6c6c 206c 6973 7420 6f66 2066 756e  full list of fun
-00000fd0: 6374 696f 6e73 2c20 7472 616e 7366 6f72  ctions, transfor
-00000fe0: 6d73 2c20 736f 7572 6365 732c 2061 6e64  ms, sources, and
-00000ff0: 2073 696e 6b73 2e0a 0a23 2320 5375 7070   sinks...## Supp
-00001000: 6f72 7420 2f20 436f 6e74 7269 6275 746f  ort / Contributo
-00001010: 7273 0a54 6861 6e6b 7320 746f 2074 6865  rs.Thanks to the
-00001020: 2066 6f6c 6c6f 7769 6e67 206f 7267 616e   following organ
-00001030: 697a 6174 696f 6e73 2066 6f72 2070 726f  izations for pro
-00001040: 7669 6469 6e67 2063 6f64 6520 6f72 2066  viding code or f
-00001050: 696e 616e 6369 616c 2073 7570 706f 7274  inancial support
-00001060: 2e0a 0a0a 3c61 2068 7265 663d 2268 7474  ....<a href="htt
-00001070: 7073 3a2f 2f6e 656d 6f75 6c6f 7573 2e63  ps://nemoulous.c
-00001080: 6f6d 223e 3c69 6d67 2073 7263 3d22 6874  om"><img src="ht
-00001090: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-000010a0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-000010b0: 7469 6d6b 7061 696e 652f 7472 6962 7574  timkpaine/tribut
-000010c0: 6172 792f 6d61 696e 2f64 6f63 732f 696d  ary/main/docs/im
-000010d0: 672f 6e65 6d2e 706e 6722 2077 6964 7468  g/nem.png" width
-000010e0: 3d22 3530 223e 3c2f 613e 0a0a 3c61 2068  ="50"></a>..<a h
-000010f0: 7265 663d 2268 7474 7073 3a2f 2f6e 656d  ref="https://nem
-00001100: 6f75 6c6f 7573 2e63 6f6d 223e 4e65 6d6f  oulous.com">Nemo
-00001110: 756c 6f75 733c 2f61 3e0a 0a23 2320 4c69  ulous</a>..## Li
-00001120: 6365 6e73 650a 5468 6973 2073 6f66 7477  cense.This softw
-00001130: 6172 6520 6973 206c 6963 656e 7365 6420  are is licensed 
-00001140: 756e 6465 7220 7468 6520 4170 6163 6865  under the Apache
-00001150: 2032 2e30 206c 6963 656e 7365 2e20 5365   2.0 license. Se
-00001160: 6520 7468 6520 5b4c 4943 454e 5345 5d28  e the [LICENSE](
-00001170: 4c49 4345 4e53 4529 2066 696c 6520 666f  LICENSE) file fo
-00001180: 7220 6465 7461 696c 732e 0a0a 2323 2041  r details...## A
-00001190: 6c74 6572 6e61 7469 7665 730a 4865 7265  lternatives.Here
-000011a0: 2069 7320 616e 2069 6e63 6f6d 706c 6574   is an incomplet
-000011b0: 6520 6c69 7374 206f 6620 6c69 6272 6172  e list of librar
-000011c0: 6965 7320 7768 6963 6820 696d 706c 656d  ies which implem
-000011d0: 656e 7420 7369 6d69 6c61 722f 6f76 6572  ent similar/over
-000011e0: 6c61 7070 696e 6720 6675 6e63 7469 6f6e  lapping function
-000011f0: 616c 6974 790a 0a2d 205b 6d61 6e2d 6772  ality..- [man-gr
-00001200: 6f75 702f 6d64 665d 2868 7474 7073 3a2f  oup/mdf](https:/
-00001210: 2f67 6974 6875 622e 636f 6d2f 6d61 6e2d  /github.com/man-
-00001220: 6772 6f75 702f 6d64 6629 0a2d 205b 6365  group/mdf).- [ce
-00001230: 6472 6963 6c65 726f 792f 7079 756e 676f  dricleroy/pyungo
-00001240: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001250: 2e63 6f6d 2f63 6564 7269 636c 6572 6f79  .com/cedricleroy
-00001260: 2f70 7975 6e67 6f29 0a2d 205b 7079 7468  /pyungo).- [pyth
-00001270: 6f6e 2d73 7472 6561 6d7a 2f73 7472 6561  on-streamz/strea
-00001280: 6d7a 5d28 6874 7470 733a 2f2f 6769 7468  mz](https://gith
-00001290: 7562 2e63 6f6d 2f70 7974 686f 6e2d 7374  ub.com/python-st
-000012a0: 7265 616d 7a2f 7374 7265 616d 7a29 0a2d  reamz/streamz).-
-000012b0: 205b 456e 7469 6c5a 6861 2f70 7966 756e   [EntilZha/pyfun
-000012c0: 6374 696f 6e61 6c5d 2868 7474 7073 3a2f  ctional](https:/
-000012d0: 2f67 6974 6875 622e 636f 6d2f 456e 7469  /github.com/Enti
-000012e0: 6c5a 6861 2f50 7946 756e 6374 696f 6e61  lZha/PyFunctiona
-000012f0: 6c29 0a2d 205b 7374 6974 6368 6669 782f  l).- [stitchfix/
-00001300: 6861 6d69 6c74 6f6e 5d28 6874 7470 733a  hamilton](https:
-00001310: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7469  //github.com/sti
-00001320: 7463 6866 6978 2f68 616d 696c 746f 6e29  tchfix/hamilton)
-00001330: 0a0a                                     ..
+00000000: 2320 3c69 6d67 2073 7263 3d22 6874 7470  # <img src="http
+00000010: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000020: 6572 636f 6e74 656e 742e 636f 6d2f 7374  ercontent.com/st
+00000030: 7265 616d 6c65 742d 6465 762f 7472 6962  reamlet-dev/trib
+00000040: 7574 6172 792f 6d61 696e 2f64 6f63 732f  utary/main/docs/
+00000050: 696d 672f 6963 6f6e 2e70 6e67 2220 7769  img/icon.png" wi
+00000060: 6474 683d 2233 3030 223e 0a50 7974 686f  dth="300">.Pytho
+00000070: 6e20 4461 7461 2053 7472 6561 6d73 0a0a  n Data Streams..
+00000080: 5b21 5b42 7569 6c64 2053 7461 7475 735d  [![Build Status]
+00000090: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000000a0: 636f 6d2f 7374 7265 616d 6c65 742d 6465  com/streamlet-de
+000000b0: 762f 7472 6962 7574 6172 792f 776f 726b  v/tributary/work
+000000c0: 666c 6f77 732f 4275 696c 6425 3230 5374  flows/Build%20St
+000000d0: 6174 7573 2f62 6164 6765 2e73 7667 3f62  atus/badge.svg?b
+000000e0: 7261 6e63 683d 6d61 696e 295d 2868 7474  ranch=main)](htt
+000000f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000100: 7374 7265 616d 6c65 742d 6465 762f 7472  streamlet-dev/tr
+00000110: 6962 7574 6172 792f 6163 7469 6f6e 733f  ibutary/actions?
+00000120: 7175 6572 793d 776f 726b 666c 6f77 2533  query=workflow%3
+00000130: 4125 3232 4275 696c 642b 5374 6174 7573  A%22Build+Status
+00000140: 2532 3229 0a5b 215b 436f 7665 7261 6765  %22).[![Coverage
+00000150: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
+00000160: 762e 696f 2f67 682f 7374 7265 616d 6c65  v.io/gh/streamle
+00000170: 742d 6465 762f 7472 6962 7574 6172 792f  t-dev/tributary/
+00000180: 6272 616e 6368 2f6d 6169 6e2f 6772 6170  branch/main/grap
+00000190: 682f 6261 6467 652e 7376 6729 5d28 6874  h/badge.svg)](ht
+000001a0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+000001b0: 2f67 682f 7374 7265 616d 6c65 742d 6465  /gh/streamlet-de
+000001c0: 762f 7472 6962 7574 6172 7929 0a5b 215b  v/tributary).[![
+000001d0: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
+000001e0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+000001f0: 692f 6c2f 7472 6962 7574 6172 792e 7376  i/l/tributary.sv
+00000200: 6729 5d28 6874 7470 733a 2f2f 7079 7069  g)](https://pypi
+00000210: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
+00000220: 2f74 7269 6275 7461 7279 290a 5b21 5b50  /tributary).[![P
+00000230: 7950 495d 2868 7474 7073 3a2f 2f69 6d67  yPI](https://img
+00000240: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000250: 2f76 2f74 7269 6275 7461 7279 2e73 7667  /v/tributary.svg
+00000260: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+00000270: 7079 7468 6f6e 2e6f 7267 2f70 7970 692f  python.org/pypi/
+00000280: 7472 6962 7574 6172 7929 0a5b 215b 4269  tributary).[![Bi
+00000290: 6e64 6572 5d28 6874 7470 733a 2f2f 6d79  nder](https://my
+000002a0: 6269 6e64 6572 2e6f 7267 2f62 6164 6765  binder.org/badge
+000002b0: 5f6c 6f67 6f2e 7376 6729 5d28 6874 7470  _logo.svg)](http
+000002c0: 733a 2f2f 6d79 6269 6e64 6572 2e6f 7267  s://mybinder.org
+000002d0: 2f76 322f 6768 2f73 7472 6561 6d6c 6574  /v2/gh/streamlet
+000002e0: 2d64 6576 2f74 7269 6275 7461 7279 2f6d  -dev/tributary/m
+000002f0: 6169 6e3f 7572 6c70 6174 683d 6c61 6229  ain?urlpath=lab)
+00000300: 0a0a 0a54 7269 6275 7461 7279 2069 7320  ...Tributary is 
+00000310: 6120 6c69 6272 6172 7920 666f 7220 636f  a library for co
+00000320: 6e73 7472 7563 7469 6e67 2064 6174 6166  nstructing dataf
+00000330: 6c6f 7720 6772 6170 6873 2069 6e20 7079  low graphs in py
+00000340: 7468 6f6e 2e20 556e 6c69 6b65 206d 616e  thon. Unlike man
+00000350: 7920 6f74 6865 7220 4441 4720 6c69 6272  y other DAG libr
+00000360: 6172 6965 7320 696e 2070 7974 686f 6e20  aries in python 
+00000370: 285b 6169 7266 6c6f 775d 2868 7474 7073  ([airflow](https
+00000380: 3a2f 2f61 6972 666c 6f77 2e61 7061 6368  ://airflow.apach
+00000390: 652e 6f72 6729 2c20 5b6c 7569 6769 5d28  e.org), [luigi](
+000003a0: 6874 7470 733a 2f2f 6c75 6967 692e 7265  https://luigi.re
+000003b0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000003c0: 7374 6162 6c65 2f29 2c20 5b70 7265 6665  stable/), [prefe
+000003d0: 6374 5d28 6874 7470 733a 2f2f 646f 6373  ct](https://docs
+000003e0: 2e70 7265 6665 6374 2e69 6f29 2c20 5b64  .prefect.io), [d
+000003f0: 6167 7374 6572 5d28 6874 7470 733a 2f2f  agster](https://
+00000400: 646f 6373 2e64 6167 7374 6572 2e69 6f29  docs.dagster.io)
+00000410: 2c20 5b64 6173 6b5d 2868 7474 7073 3a2f  , [dask](https:/
+00000420: 2f64 6173 6b2e 6f72 6729 2c20 5b6b 6564  /dask.org), [ked
+00000430: 726f 5d28 6874 7470 733a 2f2f 6769 7468  ro](https://gith
+00000440: 7562 2e63 6f6d 2f71 7561 6e74 756d 626c  ub.com/quantumbl
+00000450: 6163 6b6c 6162 732f 6b65 6472 6f29 2c20  acklabs/kedro), 
+00000460: 6574 6329 2c20 7472 6962 7574 6172 7920  etc), tributary 
+00000470: 6973 206e 6f74 2064 6573 6967 6e65 6420  is not designed 
+00000480: 7769 7468 2064 6174 612f 6574 6c20 7069  with data/etl pi
+00000490: 7065 6c69 6e65 7320 6f72 2073 6368 6564  pelines or sched
+000004a0: 756c 696e 6720 696e 206d 696e 642e 2049  uling in mind. I
+000004b0: 6e73 7465 6164 2c20 7472 6962 7574 6172  nstead, tributar
+000004c0: 7920 6973 206d 6f72 6520 7369 6d69 6c61  y is more simila
+000004d0: 7220 746f 206c 6962 7261 7269 6573 206c  r to libraries l
+000004e0: 696b 6520 5b6d 6466 5d28 6874 7470 733a  ike [mdf](https:
+000004f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 616e  //github.com/man
+00000500: 2d67 726f 7570 2f6d 6466 292c 205b 6c6f  -group/mdf), [lo
+00000510: 6d61 6e5d 2868 7474 7073 3a2f 2f67 6974  man](https://git
+00000520: 6875 622e 636f 6d2f 6a61 6e75 7368 656e  hub.com/janushen
+00000530: 6465 7273 6f6e 6173 7365 7461 6c6c 6f63  dersonassetalloc
+00000540: 6174 696f 6e2f 6c6f 6d61 6e29 2c20 5b70  ation/loman), [p
+00000550: 7975 6e67 6f5d 2868 7474 7073 3a2f 2f67  yungo](https://g
+00000560: 6974 6875 622e 636f 6d2f 6365 6472 6963  ithub.com/cedric
+00000570: 6c65 726f 792f 7079 756e 676f 292c 205b  leroy/pyungo), [
+00000580: 7374 7265 616d 7a5d 2868 7474 7073 3a2f  streamz](https:/
+00000590: 2f73 7472 6561 6d7a 2e72 6561 6474 6865  /streamz.readthe
+000005a0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+000005b0: 742f 292c 206f 7220 5b70 7966 756e 6374  t/), or [pyfunct
+000005c0: 696f 6e61 6c5d 2868 7474 7073 3a2f 2f67  ional](https://g
+000005d0: 6974 6875 622e 636f 6d2f 456e 7469 6c5a  ithub.com/EntilZ
+000005e0: 6861 2f50 7946 756e 6374 696f 6e61 6c29  ha/PyFunctional)
+000005f0: 2c20 696e 2074 6861 7420 6974 2069 7320  , in that it is 
+00000600: 6465 7369 676e 6564 2074 6f20 6265 2075  designed to be u
+00000610: 7365 6420 6173 2074 6865 2069 6d70 6c65  sed as the imple
+00000620: 6d65 6e74 6174 696f 6e20 666f 7220 6120  mentation for a 
+00000630: 6461 7461 206d 6f64 656c 2e20 4f6e 6520  data model. One 
+00000640: 7375 6368 2065 7861 6d70 6c65 2069 7320  such example is 
+00000650: 7468 6520 5b67 7265 656b 735d 2868 7474  the [greeks](htt
+00000660: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000670: 7374 7265 616d 6c65 742d 6465 762f 6772  streamlet-dev/gr
+00000680: 6565 6b73 2920 6c69 6272 6172 792c 2077  eeks) library, w
+00000690: 6869 6368 206c 6576 6572 6167 6573 2074  hich leverages t
+000006a0: 7269 6275 7461 7279 2074 6f20 6275 696c  ributary to buil
+000006b0: 6420 6461 7461 206d 6f64 656c 7320 666f  d data models fo
+000006c0: 7220 5b6f 7074 696f 6e73 2070 7269 6369  r [options prici
+000006d0: 6e67 5d28 6874 7470 733a 2f2f 7777 772e  ng](https://www.
+000006e0: 696e 7665 7374 6f70 6564 6961 2e63 6f6d  investopedia.com
+000006f0: 2f61 7274 6963 6c65 732f 6f70 7469 6f6e  /articles/option
+00000700: 696e 7665 7374 6f72 2f30 372f 6f70 7469  investor/07/opti
+00000710: 6f6e 735f 6265 6174 5f6d 6172 6b65 742e  ons_beat_market.
+00000720: 6173 7029 2e20 0a0a 215b 5d28 6874 7470  asp). ..![](http
+00000730: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000740: 6572 636f 6e74 656e 742e 636f 6d2f 7374  ercontent.com/st
+00000750: 7265 616d 6c65 742d 6465 762f 7472 6962  reamlet-dev/trib
+00000760: 7574 6172 792f 6d61 696e 2f64 6f63 732f  utary/main/docs/
+00000770: 696d 672f 6578 616d 706c 652e 6769 6629  img/example.gif)
+00000780: 0a0a 0a23 2049 6e73 7461 6c6c 6174 696f  ...# Installatio
+00000790: 6e0a 496e 7374 616c 6c20 7769 7468 2070  n.Install with p
+000007a0: 6970 3a0a 0a60 7069 7020 696e 7374 616c  ip:..`pip instal
+000007b0: 6c20 7472 6962 7574 6172 7960 0a0a 6f72  l tributary`..or
+000007c0: 2077 6974 6820 636f 6e64 613a 0a0a 6063   with conda:..`c
+000007d0: 6f6e 6461 2069 6e73 7461 6c6c 202d 6320  onda install -c 
+000007e0: 636f 6e64 612d 666f 7267 6520 7472 6962  conda-forge trib
+000007f0: 7574 6172 7960 0a0a 6f72 2066 726f 6d20  utary`..or from 
+00000800: 736f 7572 6365 3a0a 0a60 7079 7468 6f6e  source:..`python
+00000810: 2073 6574 7570 2e70 7920 696e 7374 616c   setup.py instal
+00000820: 6c60 0a0a 4e6f 7465 3a20 4966 2069 6e73  l`..Note: If ins
+00000830: 7461 6c6c 696e 6720 6672 6f6d 2073 6f75  talling from sou
+00000840: 7263 6520 6f72 2077 6974 6820 7069 702c  rce or with pip,
+00000850: 2079 6f75 276c 6c20 616c 736f 206e 6565   you'll also nee
+00000860: 6420 5b47 7261 7068 7669 7a20 6974 7365  d [Graphviz itse
+00000870: 6c66 5d28 6874 7470 733a 2f2f 7777 772e  lf](https://www.
+00000880: 6772 6170 6876 697a 2e6f 7267 2f64 6f77  graphviz.org/dow
+00000890: 6e6c 6f61 642f 2920 6966 2079 6f75 2077  nload/) if you w
+000008a0: 616e 7420 746f 2076 6973 7561 6c69 7a65  ant to visualize
+000008b0: 2074 6865 2067 7261 7068 2075 7369 6e67   the graph using
+000008c0: 2074 6865 2060 2e67 7261 7068 7669 7a28   the `.graphviz(
+000008d0: 2960 206d 6574 686f 642e 0a0a 2320 5374  )` method...# St
+000008e0: 7265 616d 2054 7970 6573 0a54 7269 6275  ream Types.Tribu
+000008f0: 7461 7279 206f 6666 6572 7320 7365 7665  tary offers seve
+00000900: 7261 6c20 6b69 6e64 7320 6f66 2073 7472  ral kinds of str
+00000910: 6561 6d73 3a0a 0a23 2320 5374 7265 616d  eams:..## Stream
+00000920: 696e 670a 5468 6573 6520 6172 6520 7379  ing.These are sy
+00000930: 6e63 6872 6f6e 6f75 732c 2072 6561 6374  nchronous, react
+00000940: 6976 6520 6461 7461 2073 7472 6561 6d73  ive data streams
+00000950: 2c20 6275 696c 7420 7573 696e 6720 6173  , built using as
+00000960: 796e 6368 726f 6e6f 7573 2070 7974 686f  ynchronous pytho
+00000970: 6e20 6765 6e65 7261 746f 7273 2e20 5468  n generators. Th
+00000980: 6579 2061 7265 2064 6573 6967 6e65 6420  ey are designed 
+00000990: 746f 206d 696d 6963 2063 6f6d 706c 6578  to mimic complex
+000009a0: 2065 7665 6e74 2070 726f 6365 7373 6f72   event processor
+000009b0: 7320 696e 2074 6572 6d73 206f 6620 6576  s in terms of ev
+000009c0: 656e 7420 6f72 6465 7269 6e67 2e0a 0a23  ent ordering...#
+000009d0: 2320 4675 6e63 7469 6f6e 616c 0a54 6865  # Functional.The
+000009e0: 7365 2061 7265 2066 756e 6374 696f 6e61  se are functiona
+000009f0: 6c20 7374 7265 616d 732c 2062 7569 6c74  l streams, built
+00000a00: 2062 7920 6375 7272 7969 6e67 2070 7974   by currying pyt
+00000a10: 686f 6e20 6675 6e63 7469 6f6e 7320 2863  hon functions (c
+00000a20: 616c 6c62 6163 6b73 292e 200a 0a23 2320  allbacks). ..## 
+00000a30: 4c61 7a79 0a54 6865 7365 2061 7265 206c  Lazy.These are l
+00000a40: 617a 696c 792d 6576 616c 7561 7465 6420  azily-evaluated 
+00000a50: 7079 7468 6f6e 2073 7472 6561 6d73 2c20  python streams, 
+00000a60: 7768 6572 6520 6f75 7470 7574 7320 6172  where outputs ar
+00000a70: 6520 7072 6f70 6f67 6174 6564 206f 6e6c  e propogated onl
+00000a80: 7920 6173 2069 6e70 7574 7320 6368 616e  y as inputs chan
+00000a90: 6765 2e20 5468 6579 2061 7265 2069 6d70  ge. They are imp
+00000aa0: 6c65 6d65 6e74 6564 2061 7320 6469 7265  lemented as dire
+00000ab0: 6374 6564 2061 6379 636c 6963 2067 7261  cted acyclic gra
+00000ac0: 7068 732e 0a0a 2320 4578 616d 706c 6573  phs...# Examples
+00000ad0: 0a2d 205b 5374 7265 616d 696e 675d 2864  .- [Streaming](d
+00000ae0: 6f63 732f 6578 616d 706c 6573 2f73 7472  ocs/examples/str
+00000af0: 6561 6d69 6e67 2f73 7472 6561 6d69 6e67  eaming/streaming
+00000b00: 2e6d 6429 3a20 496e 2074 6869 7320 6578  .md): In this ex
+00000b10: 616d 706c 652c 2077 6520 636f 6e73 7472  ample, we constr
+00000b20: 7563 7420 6120 7661 7269 6574 7920 6f66  uct a variety of
+00000b30: 2066 6f72 7761 7264 2070 726f 706f 6761   forward propoga
+00000b40: 7469 6e67 2072 6561 6374 6976 6520 6772  ting reactive gr
+00000b50: 6170 6873 2e0a 2d20 5b4c 617a 795d 2864  aphs..- [Lazy](d
+00000b60: 6f63 732f 6578 616d 706c 6573 2f6c 617a  ocs/examples/laz
+00000b70: 792f 6c61 7a79 2e6d 6429 3a20 496e 2074  y/lazy.md): In t
+00000b80: 6869 7320 6578 616d 706c 652c 2077 6520  his example, we 
+00000b90: 636f 6e73 7472 7563 7420 6120 7661 7269  construct a vari
+00000ba0: 6574 7920 6f66 206c 617a 696c 792d 6576  ety of lazily-ev
+00000bb0: 616c 7561 7465 6420 6469 7265 6374 6564  aluated directed
+00000bc0: 2061 6379 636c 6963 2063 6f6d 7075 7461   acyclic computa
+00000bd0: 7469 6f6e 2067 7261 7068 732e 200a 2d20  tion graphs. .- 
+00000be0: 5b41 7574 6f6d 6174 6963 2044 6966 6665  [Automatic Diffe
+00000bf0: 7265 6e74 6961 7469 6f6e 5d28 646f 6373  rentiation](docs
+00000c00: 2f65 7861 6d70 6c65 732f 6175 746f 6469  /examples/autodi
+00000c10: 6666 2f61 7574 6f64 6966 662e 6d64 293a  ff/autodiff.md):
+00000c20: 2049 6e20 7468 6973 2065 7861 6d70 6c65   In this example
+00000c30: 2c20 7765 2075 7365 2060 7472 6962 7574  , we use `tribut
+00000c40: 6172 7960 2074 6f20 7065 7266 6f72 6d20  ary` to perform 
+00000c50: 6175 746f 6d61 7469 6320 6469 6666 6572  automatic differ
+00000c60: 656e 7469 6174 696f 6e20 6f6e 2062 6f74  entiation on bot
+00000c70: 6820 6c61 7a79 2061 6e64 2073 7472 6561  h lazy and strea
+00000c80: 6d69 6e67 2067 7261 7068 732e 0a0a 2320  ming graphs...# 
+00000c90: 4772 6170 6820 5669 7375 616c 697a 6174  Graph Visualizat
+00000ca0: 696f 6e0a 596f 7520 6361 6e20 7669 7375  ion.You can visu
+00000cb0: 616c 697a 6520 7468 6520 6772 6170 6820  alize the graph 
+00000cc0: 7769 7468 2047 7261 7068 7669 7a2e 2041  with Graphviz. A
+00000cd0: 6c6c 2073 7472 6561 6d69 6e67 2061 6e64  ll streaming and
+00000ce0: 206c 617a 7920 6e6f 6465 7320 7375 7070   lazy nodes supp
+00000cf0: 6f72 7420 6120 6067 7261 7068 7669 7a60  ort a `graphviz`
+00000d00: 206d 6574 686f 642e 0a0a 5374 7265 616d   method...Stream
+00000d10: 696e 6720 616e 6420 6c61 7a79 206e 6f64  ing and lazy nod
+00000d20: 6573 2061 6c73 6f20 7375 7070 6f72 7420  es also support 
+00000d30: 5b69 7079 6461 6772 6564 335d 2868 7474  [ipydagred3](htt
+00000d40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000d50: 7469 6d6b 7061 696e 652f 6970 7964 6167  timkpaine/ipydag
+00000d60: 7265 6433 2920 666f 7220 6c69 7665 2075  red3) for live u
+00000d70: 7064 6174 6520 6d6f 6e69 746f 7269 6e67  pdate monitoring
+00000d80: 2e0a 0a23 2320 5374 7265 616d 696e 670a  ...## Streaming.
+00000d90: 215b 5d28 6874 7470 733a 2f2f 7261 772e  ![](https://raw.
+00000da0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000db0: 742e 636f 6d2f 7374 7265 616d 6c65 742d  t.com/streamlet-
+00000dc0: 6465 762f 7472 6962 7574 6172 792f 6d61  dev/tributary/ma
+00000dd0: 696e 2f64 6f63 732f 696d 672f 7374 7265  in/docs/img/stre
+00000de0: 616d 696e 672f 6461 6772 6564 332e 6769  aming/dagred3.gi
+00000df0: 6629 0a0a 4865 7265 2067 7265 656e 2069  f)..Here green i
+00000e00: 6e64 6963 6174 6573 2065 7865 6375 7469  ndicates executi
+00000e10: 6e67 2c20 7965 6c6c 6f77 2069 6e64 6963  ng, yellow indic
+00000e20: 6174 6573 2073 7461 6c6c 6564 2066 6f72  ates stalled for
+00000e30: 2062 6163 6b70 7265 7373 7572 652c 2061   backpressure, a
+00000e40: 6e64 2072 6564 2069 6e64 6963 6174 6573  nd red indicates
+00000e50: 2074 6861 7420 6053 7472 6561 6d45 6e64   that `StreamEnd
+00000e60: 6020 6861 7320 6265 656e 2070 726f 706f  ` has been propo
+00000e70: 6761 7465 6420 2865 2e67 2e20 7374 7265  gated (e.g. stre
+00000e80: 616d 2068 6173 2065 6e64 6564 292e 0a0a  am has ended)...
+00000e90: 2323 204c 617a 790a 215b 5d28 6874 7470  ## Lazy.![](http
+00000ea0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00000eb0: 6572 636f 6e74 656e 742e 636f 6d2f 7374  ercontent.com/st
+00000ec0: 7265 616d 6c65 742d 6465 762f 7472 6962  reamlet-dev/trib
+00000ed0: 7574 6172 792f 6d61 696e 2f64 6f63 732f  utary/main/docs/
+00000ee0: 696d 672f 6c61 7a79 2f64 6167 7265 6433  img/lazy/dagred3
+00000ef0: 2e67 6966 290a 0a48 6572 6520 6772 6565  .gif)..Here gree
+00000f00: 6e20 696e 6469 6361 7465 7320 6578 6563  n indicates exec
+00000f10: 7574 696e 672c 2061 6e64 2072 6564 2069  uting, and red i
+00000f20: 6e64 6963 6174 6573 2074 6861 7420 7468  ndicates that th
+00000f30: 6520 6e6f 6465 2069 7320 6469 7274 792e  e node is dirty.
+00000f40: 204e 6f74 6520 7468 6520 7468 6520 6465   Note the the de
+00000f50: 7465 726d 696e 6174 696f 6e20 6966 2061  termination if a
+00000f60: 206e 6f64 6520 6973 2064 6972 7479 2069   node is dirty i
+00000f70: 7320 616c 736f 2064 6f6e 6520 6c61 7a69  s also done lazi
+00000f80: 6c79 2028 7765 2063 616e 2063 6865 636b  ly (we can check
+00000f90: 2077 6974 6820 6069 7344 6972 7479 6020   with `isDirty` 
+00000fa0: 7768 6369 6820 7769 6c6c 2075 7064 6174  whcih will updat
+00000fb0: 6520 7468 6520 6e6f 6465 2773 2067 7261  e the node's gra
+00000fc0: 7068 2073 7461 7465 2e0a 0a23 2320 4361  ph state...## Ca
+00000fd0: 7461 6c6f 670a 5365 6520 7468 6520 5b43  talog.See the [C
+00000fe0: 4154 414c 4f47 5d28 4341 5441 4c4f 472e  ATALOG](CATALOG.
+00000ff0: 6d64 2920 666f 7220 6120 6675 6c6c 206c  md) for a full l
+00001000: 6973 7420 6f66 2066 756e 6374 696f 6e73  ist of functions
+00001010: 2c20 7472 616e 7366 6f72 6d73 2c20 736f  , transforms, so
+00001020: 7572 6365 732c 2061 6e64 2073 696e 6b73  urces, and sinks
+00001030: 2e0a 0a23 2320 5375 7070 6f72 7420 2f20  ...## Support / 
+00001040: 436f 6e74 7269 6275 746f 7273 0a54 6861  Contributors.Tha
+00001050: 6e6b 7320 746f 2074 6865 2066 6f6c 6c6f  nks to the follo
+00001060: 7769 6e67 206f 7267 616e 697a 6174 696f  wing organizatio
+00001070: 6e73 2066 6f72 2070 726f 7669 6469 6e67  ns for providing
+00001080: 2063 6f64 6520 6f72 2066 696e 616e 6369   code or financi
+00001090: 616c 2073 7570 706f 7274 2e0a 0a0a 3c61  al support....<a
+000010a0: 2068 7265 663d 2268 7474 7073 3a2f 2f6e   href="https://n
+000010b0: 656d 6f75 6c6f 7573 2e63 6f6d 223e 3c69  emoulous.com"><i
+000010c0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000010d0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+000010e0: 6e74 656e 742e 636f 6d2f 7374 7265 616d  ntent.com/stream
+000010f0: 6c65 742d 6465 762f 7472 6962 7574 6172  let-dev/tributar
+00001100: 792f 6d61 696e 2f64 6f63 732f 696d 672f  y/main/docs/img/
+00001110: 6e65 6d2e 706e 6722 2077 6964 7468 3d22  nem.png" width="
+00001120: 3530 223e 3c2f 613e 0a0a 3c61 2068 7265  50"></a>..<a hre
+00001130: 663d 2268 7474 7073 3a2f 2f6e 656d 6f75  f="https://nemou
+00001140: 6c6f 7573 2e63 6f6d 223e 4e65 6d6f 756c  lous.com">Nemoul
+00001150: 6f75 733c 2f61 3e0a 0a23 2320 4c69 6365  ous</a>..## Lice
+00001160: 6e73 650a 5468 6973 2073 6f66 7477 6172  nse.This softwar
+00001170: 6520 6973 206c 6963 656e 7365 6420 756e  e is licensed un
+00001180: 6465 7220 7468 6520 4170 6163 6865 2032  der the Apache 2
+00001190: 2e30 206c 6963 656e 7365 2e20 5365 6520  .0 license. See 
+000011a0: 7468 6520 5b4c 4943 454e 5345 5d28 4c49  the [LICENSE](LI
+000011b0: 4345 4e53 4529 2066 696c 6520 666f 7220  CENSE) file for 
+000011c0: 6465 7461 696c 732e 0a0a 2323 2041 6c74  details...## Alt
+000011d0: 6572 6e61 7469 7665 730a 4865 7265 2069  ernatives.Here i
+000011e0: 7320 616e 2069 6e63 6f6d 706c 6574 6520  s an incomplete 
+000011f0: 6c69 7374 206f 6620 6c69 6272 6172 6965  list of librarie
+00001200: 7320 7768 6963 6820 696d 706c 656d 656e  s which implemen
+00001210: 7420 7369 6d69 6c61 722f 6f76 6572 6c61  t similar/overla
+00001220: 7070 696e 6720 6675 6e63 7469 6f6e 616c  pping functional
+00001230: 6974 790a 0a2d 205b 6d61 6e2d 6772 6f75  ity..- [man-grou
+00001240: 702f 6d64 665d 2868 7474 7073 3a2f 2f67  p/mdf](https://g
+00001250: 6974 6875 622e 636f 6d2f 6d61 6e2d 6772  ithub.com/man-gr
+00001260: 6f75 702f 6d64 6629 0a2d 205b 6365 6472  oup/mdf).- [cedr
+00001270: 6963 6c65 726f 792f 7079 756e 676f 5d28  icleroy/pyungo](
+00001280: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001290: 6f6d 2f63 6564 7269 636c 6572 6f79 2f70  om/cedricleroy/p
+000012a0: 7975 6e67 6f29 0a2d 205b 7079 7468 6f6e  yungo).- [python
+000012b0: 2d73 7472 6561 6d7a 2f73 7472 6561 6d7a  -streamz/streamz
+000012c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000012d0: 2e63 6f6d 2f70 7974 686f 6e2d 7374 7265  .com/python-stre
+000012e0: 616d 7a2f 7374 7265 616d 7a29 0a2d 205b  amz/streamz).- [
+000012f0: 456e 7469 6c5a 6861 2f70 7966 756e 6374  EntilZha/pyfunct
+00001300: 696f 6e61 6c5d 2868 7474 7073 3a2f 2f67  ional](https://g
+00001310: 6974 6875 622e 636f 6d2f 456e 7469 6c5a  ithub.com/EntilZ
+00001320: 6861 2f50 7946 756e 6374 696f 6e61 6c29  ha/PyFunctional)
+00001330: 0a2d 205b 7374 6974 6368 6669 782f 6861  .- [stitchfix/ha
+00001340: 6d69 6c74 6f6e 5d28 6874 7470 733a 2f2f  milton](https://
+00001350: 6769 7468 7562 2e63 6f6d 2f73 7469 7463  github.com/stitc
+00001360: 6866 6978 2f68 616d 696c 746f 6e29 0a0a  hfix/hamilton)..
```

### Comparing `tributary-0.2.0/setup.cfg` & `tributary-0.2.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[bumpversion]
+current_version = 0.2.1
+commit = True
+tag = False
+
 [bdist_wheel]
 universal = 1
 
 [metadata]
 description_file = README.md
 long_description_content_type = text/markdown
 
@@ -17,27 +22,18 @@
 	tributary/lazy/output/__init__.py:F401
 	tributary/streaming/__init__.py:F401, F403
 	tributary/streaming/calculations/__init__.py:F401, F403
 	tributary/streaming/control/__init__.py:F401
 	tributary/streaming/input/__init__.py:F401, F403
 	tributary/streaming/output/__init__.py:F401
 
-[bumpversion]
-current_version = 0.2.0
-commit = True
-tag = False
-
 [bumpversion:file:tributary/_version.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
-[bumpversion:file:setup.py]
-search = version="{current_version}"
-replace = version="{new_version}"
-
 [bumpversion:file:docs/conf.py]
 search = version = "{current_version}"
 replace = version = "{new_version}"
 
 [check-manifest]
 ignore = 
 	tributary/tests/**
```

### Comparing `tributary-0.2.0/setup.py` & `tributary-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     "sympy>=1.5.1",
     "temporal-cache>=0.0.6",
     "tornado>=5.1.1",
     "twilio>=6.50.1",
 ]
 
 requires_dev = [
-    "black>=20.",
+    "black>=23",
     "check-manifest",
     "flake8>=3.7.8",
     "flake8-black>=0.2.1",
     "mock",
     "pybind11>=2.4.0",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
@@ -67,15 +67,15 @@
 
 setup(
     name=name,
     version=version,
     description="Streaming reactive and dataflow graphs in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/timkpaine/{name}".format(name=name),
+    url="https://github.com/streamlet-dev/{name}".format(name=name),
     author="Tim Paine",
     author_email="t.paine154@gmail.com",
     license="Apache 2.0",
     install_requires=requires,
     extras_require={
         "dev": requires_dev,
         "develop": requires_dev,
```

### Comparing `tributary-0.2.0/tributary/base.py` & `tributary-0.2.1/tributary/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,17 @@
         return False
 
     __ne__ = all_bin_ops
     __neg__ = all_un_ops
     __nonzero__ = all_un_ops
     __len__ = all_un_ops
 
+    def __repr__(self) -> str:
+        return self.__class__.__name__
+
 
 class StreamEnd(BaseNodeValue):
     """Indicates that a stream has nothing left in it"""
 
     instance = None
 
     def __new__(cls):
```

### Comparing `tributary-0.2.0/tributary/functional/__init__.py` & `tributary-0.2.1/tributary/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/functional/input.py` & `tributary-0.2.1/tributary/functional/input.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/functional/utils.py` & `tributary-0.2.1/tributary/functional/utils.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/incubating/ast_experiments.py` & `tributary-0.2.1/tributary/incubating/ast_experiments.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/calculations/basket.py` & `tributary-0.2.1/tributary/lazy/calculations/basket.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/calculations/finance.py` & `tributary-0.2.1/tributary/lazy/calculations/finance.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/calculations/ops.py` & `tributary-0.2.1/tributary/lazy/calculations/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,17 +578,21 @@
         return inputs[0].asin()
     elif ufunc == np.arccos:
         return inputs[0].acos()
     elif ufunc == np.arctan:
         return inputs[0].atan()
     elif ufunc == np.exp:
         return inputs[0].exp()
+    elif ufunc == np.log:
+        return inputs[0].log()
+    elif ufunc == np.sqrt:
+        return inputs[0].sqrt()
     elif ufunc == sp.special.erf:
         return inputs[0].erf()
-    raise NotImplementedError("Not Implemented!")
+    raise NotImplementedError("Not Implemented: {}".format(ufunc))
 
 
 def __array_function__(self, func, method, *inputs, **kwargs):
     if func == np.lib.scimath.log:
         return inputs[0][0].log()
     elif func == np.lib.scimath.sqrt:
         return inputs[0][0].sqrt()
```

### Comparing `tributary-0.2.0/tributary/lazy/calculations/rolling.py` & `tributary-0.2.1/tributary/lazy/calculations/rolling.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/control/control.py` & `tributary-0.2.1/tributary/lazy/control/control.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/dd3.py` & `tributary-0.2.1/tributary/lazy/dd3.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/decorator.py` & `tributary-0.2.1/tributary/lazy/decorator.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/graph.py` & `tributary-0.2.1/tributary/lazy/graph.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/node.py` & `tributary-0.2.1/tributary/lazy/node.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/output/output.py` & `tributary-0.2.1/tributary/lazy/output/output.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/lazy/utils.py` & `tributary-0.2.1/tributary/lazy/utils.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/parser/__init__.py` & `tributary-0.2.1/tributary/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/calculations/basket.py` & `tributary-0.2.1/tributary/streaming/calculations/basket.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/calculations/finance.py` & `tributary-0.2.1/tributary/streaming/calculations/finance.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/calculations/ops.py` & `tributary-0.2.1/tributary/streaming/calculations/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,17 +162,21 @@
         return inputs[0].asin()
     elif ufunc == np.arccos:
         return inputs[0].acos()
     elif ufunc == np.arctan:
         return inputs[0].atan()
     elif ufunc == np.exp:
         return inputs[0].exp()
+    elif ufunc == np.log:
+        return inputs[0].log()
+    elif ufunc == np.sqrt:
+        return inputs[0].sqrt()
     elif ufunc == sp.special.erf:
         return inputs[0].erf()
-    raise NotImplementedError("Not Implemented!")
+    raise NotImplementedError("Not Implemented: {}".format(ufunc))
 
 
 def __array_function__(self, func, method, *inputs, **kwargs):
     if func == np.lib.scimath.log:
         return inputs[0][0].log()
     elif func == np.lib.scimath.sqrt:
         return inputs[0][0].sqrt()
```

### Comparing `tributary-0.2.0/tributary/streaming/calculations/rolling.py` & `tributary-0.2.1/tributary/streaming/calculations/rolling.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/control/control.py` & `tributary-0.2.1/tributary/streaming/control/control.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/dd3.py` & `tributary-0.2.1/tributary/streaming/dd3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import asyncio
 
-_DD3_TRANSITION_DELAY = 0.1  # used so you can visually see the
+_DD3_TRANSITION_DELAY = 0.25  # used so you can visually see the
 # transition e.g. not too fast
 
 
+def set_transition_delay(amt):
+    global _DD3_TRANSITION_DELAY
+    _DD3_TRANSITION_DELAY = amt
+
+
 class _DagreD3Mixin(object):
     # ***********************
     # Dagre D3 integration
     # ***********************
 
     async def _startdd3g(self):
         """represent start of calculation with a dd3 node"""
```

### Comparing `tributary-0.2.0/tributary/streaming/graph.py` & `tributary-0.2.1/tributary/streaming/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import asyncio
 import sys
 from threading import Thread
 
 from ..base import StreamEnd, StreamNone, StreamRepeat, TributaryException  # noqa: F401
 
 
+# nest_asyncio.apply()
+
+
 class StreamingGraph(object):
     """internal representation of the entire graph state"""
 
     def __init__(self, node):
         self._stop = False
         self._starting_node = node  # noqa F405
 
@@ -81,28 +84,35 @@
     def run(self, blocking=True, newloop=False, start=True):
         if sys.platform == "win32":
             # Set to proactor event loop on window
             # (default in python 3.8+)
             loop = asyncio.ProactorEventLoop()
 
         else:
-
             if newloop:
+                # create a new loop
                 loop = asyncio.new_event_loop()
-
             else:
+                # get the current loop
                 loop = asyncio.get_event_loop()
 
         asyncio.set_event_loop(loop)
 
         task = loop.create_task(self._run())
 
         if blocking:
-            # block until done
+            # if loop is already running, make reentrant
             try:
+                if loop.is_running():
+
+                    async def wait(task):
+                        return await task
+
+                    return asyncio.run_coroutine_threadsafe(wait(task), loop)
+                # block until done
                 return loop.run_until_complete(task)
             except KeyboardInterrupt:
                 return
 
         if start:
             t = Thread(target=loop.run_until_complete, args=(task,))
             t.daemon = True
```

### Comparing `tributary-0.2.0/tributary/streaming/input/__init__.py` & `tributary-0.2.1/tributary/streaming/input/__init__.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/input/file.py` & `tributary-0.2.1/tributary/streaming/input/file.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/input/http.py` & `tributary-0.2.1/tributary/streaming/input/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         ):
             count = 0 if repeat >= 0 else float("-inf")  # make less than anything
             while count < repeat:
                 async with aiohttp.ClientSession() as session:
                     async with session.get(
                         url, cookies=cookies, proxy=proxies
                     ) as response:
-
                         if response_handler and callable(response_handler):
                             yield response_handler(response)
 
                         else:
                             msg = await response.text()
 
                             if msg is None or response.status != 200:
```

### Comparing `tributary-0.2.0/tributary/streaming/input/input.py` & `tributary-0.2.1/tributary/streaming/input/input.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/input/kafka.py` & `tributary-0.2.1/tributary/streaming/input/kafka.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,14 @@
             group=group,
             topics=topics,
             json=json,
             wrap=wrap,
             interval=interval,
         ):
             if self._consumer is None:
-
                 self._consumer = AIOKafkaConsumer(
                     *topics,
                     bootstrap_servers=servers,
                     group_id=group,
                     **consumer_kwargs
                 )
```

### Comparing `tributary-0.2.0/tributary/streaming/input/postgres.py` & `tributary-0.2.1/tributary/streaming/input/postgres.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/input/process.py` & `tributary-0.2.1/tributary/streaming/input/process.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/input/socketio.py` & `tributary-0.2.1/tributary/streaming/input/socketio.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/input/sse.py` & `tributary-0.2.1/tributary/streaming/input/sse.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/input/ws.py` & `tributary-0.2.1/tributary/streaming/input/ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         field (str): field to index result by
     """
 
     def __init__(self, url, json=False, wrap=False, field=None):
         async def _listen(url=url, json=json, wrap=wrap):
             session = aiohttp.ClientSession()
             async with session.ws_connect(url) as ws:
-
                 async for msg in ws:
                     if msg.type == aiohttp.WSMsgType.TEXT:
                         x = msg.data
                         if json:
                             x = JSON.loads(x)
                         if field:
                             x = x[field]
```

### Comparing `tributary-0.2.0/tributary/streaming/node.py` & `tributary-0.2.1/tributary/streaming/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,17 +136,17 @@
     def has(self, key):
         """Use this method to check attributes (convenience for hasattr)"""
         return hasattr(self, key)
 
     def set(self, key, value):
         """Use this method to set attributes
 
-        Since we often use attributes to track node state, let's make sure we don't clobber any important ones"""
+        Since we often use attributes to track node state, let's make sure we don't clobber any important ones
+        """
         if hasattr(self, "_initial_attrs") and key in self._initial_attrs:
-
             # if we've completed our construction, ensure critical attrs arent overloaded
             raise TributaryException(
                 "Overloading node-critical attribute: {}".format(key)
             )
 
         self._initial_attrs.append(key)
         super().__setattr__(key, value)
@@ -172,23 +172,23 @@
 
     def value(self):
         """get value from node"""
         return self._last
 
     async def __call__(self):
         """execute the callable if possible, and propogate values downstream"""
+        # Previously ended stream
+        if self._finished:
+            return await self._finish()
+
         # Downstream nodes can't process
         if self._backpressure():
             await self._waitdd3g()
             return StreamNone()
 
-        # Previously ended stream
-        if self._finished:
-            return await self._finish()
-
         # dd3g
         await self._startdd3g()
 
         # Sleep if needed
         if self._delay_interval:
             await asyncio.sleep(self._delay_interval)
 
@@ -311,20 +311,20 @@
                 # NOOP
                 self._last = self._last
             else:
                 self._last = _last
         else:
             self._last = _last
 
+        await self._enddd3g()
         await self._output(self._last)
 
         for i in range(len(self._active)):
             self._active[i] = StreamNone()
 
-        await self._enddd3g()
         if isinstance(self._last, StreamEnd):
             await self._finish()
 
     async def _finish(self):
         """mark this node as finished"""
         self._finished = True
         self._last = StreamEnd()
@@ -340,15 +340,14 @@
         return ret
 
     async def _output(self, ret):
         """output value to downstream nodes"""
         # if downstreams, output
         if not isinstance(ret, (StreamNone, StreamRepeat)):
             for down, i in self.downstream():
-
                 if self._drop:
                     if len(down._input[i]) > 0:
                         # do nothing
                         pass
 
                     elif not isinstance(down._active[i], StreamNone):
                         # do nothing
```

### Comparing `tributary-0.2.0/tributary/streaming/output/__init__.py` & `tributary-0.2.1/tributary/streaming/output/__init__.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/email.py` & `tributary-0.2.1/tributary/streaming/output/email.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/file.py` & `tributary-0.2.1/tributary/streaming/output/file.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/http.py` & `tributary-0.2.1/tributary/streaming/output/http.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/kafka.py` & `tributary-0.2.1/tributary/streaming/output/kafka.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/output.py` & `tributary-0.2.1/tributary/streaming/output/output.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/postgres.py` & `tributary-0.2.1/tributary/streaming/output/postgres.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/socketio.py` & `tributary-0.2.1/tributary/streaming/output/socketio.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/sse.py` & `tributary-0.2.1/tributary/streaming/output/sse.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/output/text.py` & `tributary-0.2.1/tributary/streaming/output/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
         async def _send(
             message,
             to=to,
             from_=from_,
             twilio=twilio,
         ):
-
             r = self._twilio_client.messages.create(to=to, from_=from_, body=message)
 
             return r, message
 
         super().__init__(func=_send, inputs=1)
         self._name = "TextMessage"
         node >> self
```

### Comparing `tributary-0.2.0/tributary/streaming/output/ws.py` & `tributary-0.2.1/tributary/streaming/output/ws.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/scheduler.py` & `tributary-0.2.1/tributary/streaming/scheduler.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/serialize.py` & `tributary-0.2.1/tributary/streaming/serialize.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/streaming/utils.py` & `tributary-0.2.1/tributary/streaming/utils.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/symbolic/__init__.py` & `tributary-0.2.1/tributary/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/functional/test_functional.py` & `tributary-0.2.1/tributary/tests/functional/test_functional.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/lazy/calculations/test_basket_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/calculations/test_basket_lazy.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/lazy/calculations/test_dual_ops_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/calculations/test_dual_ops_lazy.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/lazy/calculations/test_finance_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/calculations/test_finance_lazy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 import tributary.lazy as tl
 
 
 class TestFinance:
     def test_rsi(self):
-        df = pd.DataFrame(pd.util.testing.getTimeSeriesData(20))
+        try:
+            df = pd.DataFrame(pd.util.testing.getTimeSeriesData(20))
+        except AttributeError:
+            df = pd.DataFrame(pd._testing.getTimeSeriesData(20))
         adjust = False
         period = 14
         delta = df["A"].diff().shift(-1)
         up, down = delta.copy(), delta.copy()
         up[up < 0] = 0
         down[down > 0] = 0
         _gain = up.ewm(alpha=1.0 / period, adjust=adjust).mean()
@@ -27,15 +30,18 @@
             assert abs(n_rsi() - rsi[i]) < 0.003
 
         n = tl.Node(value=val)
         n_rsi = n.rsi(period=period, basket=True)
         assert n_rsi().tolist() == rsi.tolist()
 
     def test_macd(self):
-        df = pd.DataFrame(pd.util.testing.getTimeSeriesData(20))
+        try:
+            df = pd.DataFrame(pd.util.testing.getTimeSeriesData(20))
+        except AttributeError:
+            df = pd.DataFrame(pd._testing.getTimeSeriesData(20))
 
         period_fast = 12
         period_slow = 26
         signal = 9
         adjust = False
 
         EMA_fast = pd.Series(
```

### Comparing `tributary-0.2.0/tributary/tests/lazy/calculations/test_ops_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/calculations/test_ops_lazy.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/lazy/test_api_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/test_api_lazy.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/lazy/test_graph_class_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/test_graph_class_lazy.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/lazy/test_method_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/test_method_lazy.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/lazy/test_tweaks_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/test_tweaks_lazy.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/lazy/test_utils_lazy.py` & `tributary-0.2.1/tributary/tests/lazy/test_utils_lazy.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/calculations/test_basket_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/calculations/test_basket_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/calculations/test_dual_ops_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/calculations/test_dual_ops_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/calculations/test_finance_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/calculations/test_finance_streaming.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import pandas as pd
 import tributary.streaming as ts
 
 
 class TestFinance:
     def test_rsi(self):
-        vals = pd.DataFrame(pd.util.testing.getTimeSeriesData(20))
+        try:
+            vals = pd.DataFrame(pd.util.testing.getTimeSeriesData(20))
+        except AttributeError:
+            vals = pd.DataFrame(pd._testing.getTimeSeriesData(20))
         adjust = False
         period = 14
         delta = vals["A"].diff().shift(-1)
         up, down = delta.copy(), delta.copy()
         up[up < 0] = 0
         down[down > 0] = 0
         _gain = up.ewm(alpha=1.0 / period, adjust=adjust).mean()
@@ -21,15 +24,18 @@
         for x, y in zip(ret, rsi):
             if pd.isna(y):
                 continue
             print("({}, {})".format(x, y))
             assert abs(x - y) < 0.001
 
     def test_macd(self):
-        vals = pd.DataFrame(pd.util.testing.getTimeSeriesData(20))
+        try:
+            vals = pd.DataFrame(pd.util.testing.getTimeSeriesData(20))
+        except AttributeError:
+            vals = pd.DataFrame(pd._testing.getTimeSeriesData(20))
         period_fast = 12
         period_slow = 26
         signal = 9
         adjust = False
 
         EMA_fast = pd.Series(
             vals["A"].ewm(ignore_na=False, span=period_fast, adjust=adjust).mean(),
```

### Comparing `tributary-0.2.0/tributary/tests/streaming/calculations/test_ops_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/calculations/test_ops_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/calculations/test_rolling_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/calculations/test_rolling_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/input/test_file_data.csv` & `tributary-0.2.1/tributary/tests/streaming/input/test_file_data.csv`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/input/test_file_data.json` & `tributary-0.2.1/tributary/tests/streaming/input/test_file_data.json`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/input/test_file_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/input/test_file_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/input/test_http_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/input/test_http_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/input/test_input_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/input/test_input_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/input/test_process_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/input/test_process_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/output/test_file_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/output/test_file_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/output/test_http_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/output/test_http_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/output/test_output_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/output/test_output_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/output/test_postgres_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/output/test_postgres_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/output/test_ws_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/output/test_ws_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/test_api_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/test_api_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/test_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/test_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/test_timing_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/test_timing_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/streaming/test_utils_streaming.py` & `tributary-0.2.1/tributary/tests/streaming/test_utils_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,14 @@
 
         def func3():
             yield 2
             yield 4
             yield 6
 
         def reduce(node1_value, node2_value, node3_value, reducer_node):
-
             if not hasattr(reducer_node, "state"):
                 # on first call, make sure node tracks state
                 reducer_node.set("state", {"n1": None, "n2": None, "n3": None})
 
             if node1_value is not None:
                 reducer_node.state["n1"] = node1_value
```

### Comparing `tributary-0.2.0/tributary/tests/symbolic/test_symbolic.py` & `tributary-0.2.1/tributary/tests/symbolic/test_symbolic.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/test_data/ohlc.csv` & `tributary-0.2.1/tributary/tests/test_data/ohlc.csv`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/utils/test_extract_parameters.py` & `tributary-0.2.1/tributary/tests/utils/test_extract_parameters.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/tests/utils/test_lazy_to_streaming.py` & `tributary-0.2.1/tributary/tests/utils/test_lazy_to_streaming.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/thread.py` & `tributary-0.2.1/tributary/thread.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary/utils.py` & `tributary-0.2.1/tributary/utils.py`

 * *Files identical despite different names*

### Comparing `tributary-0.2.0/tributary.egg-info/PKG-INFO` & `tributary-0.2.1/tributary.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,355 +1,358 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7472 6962  : 2.1.Name: trib
 00000020: 7574 6172 790a 5665 7273 696f 6e3a 2030  utary.Version: 0
-00000030: 2e32 2e30 0a53 756d 6d61 7279 3a20 5374  .2.0.Summary: St
+00000030: 2e32 2e31 0a53 756d 6d61 7279 3a20 5374  .2.1.Summary: St
 00000040: 7265 616d 696e 6720 7265 6163 7469 7665  reaming reactive
 00000050: 2061 6e64 2064 6174 6166 6c6f 7720 6772   and dataflow gr
 00000060: 6170 6873 2069 6e20 5079 7468 6f6e 0a48  aphs in Python.H
 00000070: 6f6d 652d 7061 6765 3a20 6874 7470 733a  ome-page: https:
-00000080: 2f2f 6769 7468 7562 2e63 6f6d 2f74 696d  //github.com/tim
-00000090: 6b70 6169 6e65 2f74 7269 6275 7461 7279  kpaine/tributary
-000000a0: 0a41 7574 686f 723a 2054 696d 2050 6169  .Author: Tim Pai
-000000b0: 6e65 0a41 7574 686f 722d 656d 6169 6c3a  ne.Author-email:
-000000c0: 2074 2e70 6169 6e65 3135 3440 676d 6169   t.paine154@gmai
-000000d0: 6c2e 636f 6d0a 4c69 6365 6e73 653a 2041  l.com.License: A
-000000e0: 7061 6368 6520 322e 300a 4b65 7977 6f72  pache 2.0.Keywor
-000000f0: 6473 3a20 7374 7265 616d 696e 6720 6c61  ds: streaming la
-00000100: 7a79 2067 7261 7068 2064 6167 2064 6174  zy graph dag dat
-00000110: 6166 6c6f 7720 7265 6163 7469 7665 0a50  aflow reactive.P
-00000120: 6c61 7466 6f72 6d3a 2055 4e4b 4e4f 574e  latform: UNKNOWN
-00000130: 0a43 6c61 7373 6966 6965 723a 2044 6576  .Classifier: Dev
-00000140: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000150: 3a3a 2033 202d 2041 6c70 6861 0a43 6c61  :: 3 - Alpha.Cla
-00000160: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000170: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000180: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
-00000190: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000001a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001b0: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
-000001c0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
-000001f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000220: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-00000230: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000240: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000250: 2033 2e31 300a 5265 7175 6972 6573 2d50   3.10.Requires-P
-00000260: 7974 686f 6e3a 203e 3d33 2e37 0a44 6573  ython: >=3.7.Des
-00000270: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000280: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000290: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
-000002a0: 7472 613a 2064 6576 0a50 726f 7669 6465  tra: dev.Provide
-000002b0: 732d 4578 7472 613a 2064 6576 656c 6f70  s-Extra: develop
-000002c0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000002d0: 2066 756e 6374 696f 6e61 6c0a 4c69 6365   functional.Lice
-000002e0: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-000002f0: 450a 0a23 203c 6120 6872 6566 3d22 6874  E..# <a href="ht
-00000300: 7470 733a 2f2f 7472 6962 7574 6172 792e  tps://tributary.
-00000310: 7265 6164 7468 6564 6f63 732e 696f 223e  readthedocs.io">
-00000320: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000330: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00000340: 636f 6e74 656e 742e 636f 6d2f 7469 6d6b  content.com/timk
-00000350: 7061 696e 652f 7472 6962 7574 6172 792f  paine/tributary/
-00000360: 6d61 696e 2f64 6f63 732f 696d 672f 6963  main/docs/img/ic
-00000370: 6f6e 2e70 6e67 2220 7769 6474 683d 2233  on.png" width="3
-00000380: 3030 223e 3c2f 613e 0a50 7974 686f 6e20  00"></a>.Python 
-00000390: 4461 7461 2053 7472 6561 6d73 0a0a 5b21  Data Streams..[!
-000003a0: 5b42 7569 6c64 2053 7461 7475 735d 2868  [Build Status](h
-000003b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000003c0: 6d2f 7469 6d6b 7061 696e 652f 7472 6962  m/timkpaine/trib
-000003d0: 7574 6172 792f 776f 726b 666c 6f77 732f  utary/workflows/
-000003e0: 4275 696c 6425 3230 5374 6174 7573 2f62  Build%20Status/b
-000003f0: 6164 6765 2e73 7667 3f62 7261 6e63 683d  adge.svg?branch=
-00000400: 6d61 696e 295d 2868 7474 7073 3a2f 2f67  main)](https://g
-00000410: 6974 6875 622e 636f 6d2f 7469 6d6b 7061  ithub.com/timkpa
-00000420: 696e 652f 7472 6962 7574 6172 792f 6163  ine/tributary/ac
-00000430: 7469 6f6e 733f 7175 6572 793d 776f 726b  tions?query=work
-00000440: 666c 6f77 2533 4125 3232 4275 696c 642b  flow%3A%22Build+
-00000450: 5374 6174 7573 2532 3229 0a5b 215b 436f  Status%22).[![Co
-00000460: 7665 7261 6765 5d28 6874 7470 733a 2f2f  verage](https://
-00000470: 636f 6465 636f 762e 696f 2f67 682f 7469  codecov.io/gh/ti
-00000480: 6d6b 7061 696e 652f 7472 6962 7574 6172  mkpaine/tributar
-00000490: 792f 6272 616e 6368 2f6d 6169 6e2f 6772  y/branch/main/gr
-000004a0: 6170 682f 6261 6467 652e 7376 6729 5d28  aph/badge.svg)](
-000004b0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
-000004c0: 696f 2f67 682f 7469 6d6b 7061 696e 652f  io/gh/timkpaine/
-000004d0: 7472 6962 7574 6172 7929 0a5b 215b 5079  tributary).[![Py
-000004e0: 5049 5d28 6874 7470 733a 2f2f 696d 672e  PI](https://img.
-000004f0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000500: 6c2f 7472 6962 7574 6172 792e 7376 6729  l/tributary.svg)
-00000510: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
-00000520: 7974 686f 6e2e 6f72 672f 7079 7069 2f74  ython.org/pypi/t
-00000530: 7269 6275 7461 7279 290a 5b21 5b50 7950  ributary).[![PyP
-00000540: 495d 2868 7474 7073 3a2f 2f69 6d67 2e73  I](https://img.s
-00000550: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
-00000560: 2f74 7269 6275 7461 7279 2e73 7667 295d  /tributary.svg)]
-00000570: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
-00000580: 7468 6f6e 2e6f 7267 2f70 7970 692f 7472  thon.org/pypi/tr
-00000590: 6962 7574 6172 7929 0a5b 215b 4269 6e64  ibutary).[![Bind
-000005a0: 6572 5d28 6874 7470 733a 2f2f 6d79 6269  er](https://mybi
-000005b0: 6e64 6572 2e6f 7267 2f62 6164 6765 5f6c  nder.org/badge_l
-000005c0: 6f67 6f2e 7376 6729 5d28 6874 7470 733a  ogo.svg)](https:
-000005d0: 2f2f 6d79 6269 6e64 6572 2e6f 7267 2f76  //mybinder.org/v
-000005e0: 322f 6768 2f74 696d 6b70 6169 6e65 2f74  2/gh/timkpaine/t
-000005f0: 7269 6275 7461 7279 2f6d 6169 6e3f 7572  ributary/main?ur
-00000600: 6c70 6174 683d 6c61 6229 0a0a 0a54 7269  lpath=lab)...Tri
-00000610: 6275 7461 7279 2069 7320 6120 6c69 6272  butary is a libr
-00000620: 6172 7920 666f 7220 636f 6e73 7472 7563  ary for construc
-00000630: 7469 6e67 2064 6174 6166 6c6f 7720 6772  ting dataflow gr
-00000640: 6170 6873 2069 6e20 7079 7468 6f6e 2e20  aphs in python. 
-00000650: 556e 6c69 6b65 206d 616e 7920 6f74 6865  Unlike many othe
-00000660: 7220 4441 4720 6c69 6272 6172 6965 7320  r DAG libraries 
-00000670: 696e 2070 7974 686f 6e20 285b 6169 7266  in python ([airf
-00000680: 6c6f 775d 2868 7474 7073 3a2f 2f61 6972  low](https://air
-00000690: 666c 6f77 2e61 7061 6368 652e 6f72 6729  flow.apache.org)
-000006a0: 2c20 5b6c 7569 6769 5d28 6874 7470 733a  , [luigi](https:
-000006b0: 2f2f 6c75 6967 692e 7265 6164 7468 6564  //luigi.readthed
-000006c0: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
-000006d0: 2f29 2c20 5b70 7265 6665 6374 5d28 6874  /), [prefect](ht
-000006e0: 7470 733a 2f2f 646f 6373 2e70 7265 6665  tps://docs.prefe
-000006f0: 6374 2e69 6f29 2c20 5b64 6167 7374 6572  ct.io), [dagster
-00000700: 5d28 6874 7470 733a 2f2f 646f 6373 2e64  ](https://docs.d
-00000710: 6167 7374 6572 2e69 6f29 2c20 5b64 6173  agster.io), [das
-00000720: 6b5d 2868 7474 7073 3a2f 2f64 6173 6b2e  k](https://dask.
-00000730: 6f72 6729 2c20 5b6b 6564 726f 5d28 6874  org), [kedro](ht
-00000740: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000750: 2f71 7561 6e74 756d 626c 6163 6b6c 6162  /quantumblacklab
-00000760: 732f 6b65 6472 6f29 2c20 6574 6329 2c20  s/kedro), etc), 
-00000770: 7472 6962 7574 6172 7920 6973 206e 6f74  tributary is not
-00000780: 2064 6573 6967 6e65 6420 7769 7468 2064   designed with d
-00000790: 6174 612f 6574 6c20 7069 7065 6c69 6e65  ata/etl pipeline
-000007a0: 7320 6f72 2073 6368 6564 756c 696e 6720  s or scheduling 
-000007b0: 696e 206d 696e 642e 2049 6e73 7465 6164  in mind. Instead
-000007c0: 2c20 7472 6962 7574 6172 7920 6973 206d  , tributary is m
-000007d0: 6f72 6520 7369 6d69 6c61 7220 746f 206c  ore similar to l
-000007e0: 6962 7261 7269 6573 206c 696b 6520 5b6d  ibraries like [m
-000007f0: 6466 5d28 6874 7470 733a 2f2f 6769 7468  df](https://gith
-00000800: 7562 2e63 6f6d 2f6d 616e 2d67 726f 7570  ub.com/man-group
-00000810: 2f6d 6466 292c 205b 7079 756e 676f 5d28  /mdf), [pyungo](
-00000820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000830: 6f6d 2f63 6564 7269 636c 6572 6f79 2f70  om/cedricleroy/p
-00000840: 7975 6e67 6f29 2c20 5b73 7472 6561 6d7a  yungo), [streamz
-00000850: 5d28 6874 7470 733a 2f2f 7374 7265 616d  ](https://stream
-00000860: 7a2e 7265 6164 7468 6564 6f63 732e 696f  z.readthedocs.io
-00000870: 2f65 6e2f 6c61 7465 7374 2f29 2c20 6f72  /en/latest/), or
-00000880: 205b 7079 6675 6e63 7469 6f6e 616c 5d28   [pyfunctional](
-00000890: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000008a0: 6f6d 2f45 6e74 696c 5a68 612f 5079 4675  om/EntilZha/PyFu
-000008b0: 6e63 7469 6f6e 616c 292c 2069 6e20 7468  nctional), in th
-000008c0: 6174 2069 7420 6973 2064 6573 6967 6e65  at it is designe
-000008d0: 6420 746f 2062 6520 7573 6564 2061 7320  d to be used as 
-000008e0: 7468 6520 696d 706c 656d 656e 7461 7469  the implementati
-000008f0: 6f6e 2066 6f72 2061 2064 6174 6120 6d6f  on for a data mo
-00000900: 6465 6c2e 204f 6e65 2073 7563 6820 6578  del. One such ex
-00000910: 616d 706c 6520 6973 2074 6865 205b 6772  ample is the [gr
-00000920: 6565 6b73 5d28 6874 7470 733a 2f2f 6769  eeks](https://gi
-00000930: 7468 7562 2e63 6f6d 2f74 696d 6b70 6169  thub.com/timkpai
-00000940: 6e65 2f67 7265 656b 7329 206c 6962 7261  ne/greeks) libra
-00000950: 7279 2c20 7768 6963 6820 6c65 7665 7261  ry, which levera
-00000960: 6765 7320 7472 6962 7574 6172 7920 746f  ges tributary to
-00000970: 2062 7569 6c64 2064 6174 6120 6d6f 6465   build data mode
-00000980: 6c73 2066 6f72 205b 6f70 7469 6f6e 7320  ls for [options 
-00000990: 7072 6963 696e 675d 2868 7474 7073 3a2f  pricing](https:/
-000009a0: 2f77 7777 2e69 6e76 6573 746f 7065 6469  /www.investopedi
-000009b0: 612e 636f 6d2f 6172 7469 636c 6573 2f6f  a.com/articles/o
-000009c0: 7074 696f 6e69 6e76 6573 746f 722f 3037  ptioninvestor/07
-000009d0: 2f6f 7074 696f 6e73 5f62 6561 745f 6d61  /options_beat_ma
-000009e0: 726b 6574 2e61 7370 292e 200a 0a21 5b5d  rket.asp). ..![]
-000009f0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
-00000a00: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000a10: 6f6d 2f74 696d 6b70 6169 6e65 2f74 7269  om/timkpaine/tri
-00000a20: 6275 7461 7279 2f6d 6169 6e2f 646f 6373  butary/main/docs
-00000a30: 2f69 6d67 2f65 7861 6d70 6c65 2e67 6966  /img/example.gif
-00000a40: 290a 0a0a 2320 496e 7374 616c 6c61 7469  )...# Installati
-00000a50: 6f6e 0a49 6e73 7461 6c6c 2077 6974 6820  on.Install with 
-00000a60: 7069 703a 0a0a 6070 6970 2069 6e73 7461  pip:..`pip insta
-00000a70: 6c6c 2074 7269 6275 7461 7279 600a 0a6f  ll tributary`..o
-00000a80: 7220 7769 7468 2063 6f6e 6461 3a0a 0a60  r with conda:..`
-00000a90: 636f 6e64 6120 696e 7374 616c 6c20 2d63  conda install -c
-00000aa0: 2063 6f6e 6461 2d66 6f72 6765 2074 7269   conda-forge tri
-00000ab0: 6275 7461 7279 600a 0a6f 7220 6672 6f6d  butary`..or from
-00000ac0: 2073 6f75 7263 653a 0a0a 6070 7974 686f   source:..`pytho
-00000ad0: 6e20 7365 7475 702e 7079 2069 6e73 7461  n setup.py insta
-00000ae0: 6c6c 600a 0a4e 6f74 653a 2049 6620 696e  ll`..Note: If in
-00000af0: 7374 616c 6c69 6e67 2066 726f 6d20 736f  stalling from so
-00000b00: 7572 6365 206f 7220 7769 7468 2070 6970  urce or with pip
-00000b10: 2c20 796f 7527 6c6c 2061 6c73 6f20 6e65  , you'll also ne
-00000b20: 6564 205b 4772 6170 6876 697a 2069 7473  ed [Graphviz its
-00000b30: 656c 665d 2868 7474 7073 3a2f 2f77 7777  elf](https://www
-00000b40: 2e67 7261 7068 7669 7a2e 6f72 672f 646f  .graphviz.org/do
-00000b50: 776e 6c6f 6164 2f29 2069 6620 796f 7520  wnload/) if you 
-00000b60: 7761 6e74 2074 6f20 7669 7375 616c 697a  want to visualiz
-00000b70: 6520 7468 6520 6772 6170 6820 7573 696e  e the graph usin
-00000b80: 6720 7468 6520 602e 6772 6170 6876 697a  g the `.graphviz
-00000b90: 2829 6020 6d65 7468 6f64 2e0a 0a23 2053  ()` method...# S
-00000ba0: 7472 6561 6d20 5479 7065 730a 5472 6962  tream Types.Trib
-00000bb0: 7574 6172 7920 6f66 6665 7273 2073 6576  utary offers sev
-00000bc0: 6572 616c 206b 696e 6473 206f 6620 7374  eral kinds of st
-00000bd0: 7265 616d 733a 0a0a 2323 2053 7472 6561  reams:..## Strea
-00000be0: 6d69 6e67 0a54 6865 7365 2061 7265 2073  ming.These are s
-00000bf0: 796e 6368 726f 6e6f 7573 2c20 7265 6163  ynchronous, reac
-00000c00: 7469 7665 2064 6174 6120 7374 7265 616d  tive data stream
-00000c10: 732c 2062 7569 6c74 2075 7369 6e67 2061  s, built using a
-00000c20: 7379 6e63 6872 6f6e 6f75 7320 7079 7468  synchronous pyth
-00000c30: 6f6e 2067 656e 6572 6174 6f72 732e 2054  on generators. T
-00000c40: 6865 7920 6172 6520 6465 7369 676e 6564  hey are designed
-00000c50: 2074 6f20 6d69 6d69 6320 636f 6d70 6c65   to mimic comple
-00000c60: 7820 6576 656e 7420 7072 6f63 6573 736f  x event processo
-00000c70: 7273 2069 6e20 7465 726d 7320 6f66 2065  rs in terms of e
-00000c80: 7665 6e74 206f 7264 6572 696e 672e 0a0a  vent ordering...
-00000c90: 2323 2046 756e 6374 696f 6e61 6c0a 5468  ## Functional.Th
-00000ca0: 6573 6520 6172 6520 6675 6e63 7469 6f6e  ese are function
-00000cb0: 616c 2073 7472 6561 6d73 2c20 6275 696c  al streams, buil
-00000cc0: 7420 6279 2063 7572 7279 696e 6720 7079  t by currying py
-00000cd0: 7468 6f6e 2066 756e 6374 696f 6e73 2028  thon functions (
-00000ce0: 6361 6c6c 6261 636b 7329 2e20 0a0a 2323  callbacks). ..##
-00000cf0: 204c 617a 790a 5468 6573 6520 6172 6520   Lazy.These are 
-00000d00: 6c61 7a69 6c79 2d65 7661 6c75 6174 6564  lazily-evaluated
-00000d10: 2070 7974 686f 6e20 7374 7265 616d 732c   python streams,
-00000d20: 2077 6865 7265 206f 7574 7075 7473 2061   where outputs a
-00000d30: 7265 2070 726f 706f 6761 7465 6420 6f6e  re propogated on
-00000d40: 6c79 2061 7320 696e 7075 7473 2063 6861  ly as inputs cha
-00000d50: 6e67 652e 2054 6865 7920 6172 6520 696d  nge. They are im
-00000d60: 706c 656d 656e 7465 6420 6173 2064 6972  plemented as dir
-00000d70: 6563 7465 6420 6163 7963 6c69 6320 6772  ected acyclic gr
-00000d80: 6170 6873 2e0a 0a23 2045 7861 6d70 6c65  aphs...# Example
-00000d90: 730a 2d20 5b53 7472 6561 6d69 6e67 5d28  s.- [Streaming](
-00000da0: 646f 6373 2f65 7861 6d70 6c65 732f 7374  docs/examples/st
-00000db0: 7265 616d 696e 672f 7374 7265 616d 696e  reaming/streamin
-00000dc0: 672e 6d64 293a 2049 6e20 7468 6973 2065  g.md): In this e
-00000dd0: 7861 6d70 6c65 2c20 7765 2063 6f6e 7374  xample, we const
-00000de0: 7275 6374 2061 2076 6172 6965 7479 206f  ruct a variety o
-00000df0: 6620 666f 7277 6172 6420 7072 6f70 6f67  f forward propog
-00000e00: 6174 696e 6720 7265 6163 7469 7665 2067  ating reactive g
-00000e10: 7261 7068 732e 0a2d 205b 4c61 7a79 5d28  raphs..- [Lazy](
-00000e20: 646f 6373 2f65 7861 6d70 6c65 732f 6c61  docs/examples/la
-00000e30: 7a79 2f6c 617a 792e 6d64 293a 2049 6e20  zy/lazy.md): In 
-00000e40: 7468 6973 2065 7861 6d70 6c65 2c20 7765  this example, we
-00000e50: 2063 6f6e 7374 7275 6374 2061 2076 6172   construct a var
-00000e60: 6965 7479 206f 6620 6c61 7a69 6c79 2d65  iety of lazily-e
-00000e70: 7661 6c75 6174 6564 2064 6972 6563 7465  valuated directe
-00000e80: 6420 6163 7963 6c69 6320 636f 6d70 7574  d acyclic comput
-00000e90: 6174 696f 6e20 6772 6170 6873 2e20 0a2d  ation graphs. .-
-00000ea0: 205b 4175 746f 6d61 7469 6320 4469 6666   [Automatic Diff
-00000eb0: 6572 656e 7469 6174 696f 6e5d 2864 6f63  erentiation](doc
-00000ec0: 732f 6578 616d 706c 6573 2f61 7574 6f64  s/examples/autod
-00000ed0: 6966 662f 6175 746f 6469 6666 2e6d 6429  iff/autodiff.md)
-00000ee0: 3a20 496e 2074 6869 7320 6578 616d 706c  : In this exampl
-00000ef0: 652c 2077 6520 7573 6520 6074 7269 6275  e, we use `tribu
-00000f00: 7461 7279 6020 746f 2070 6572 666f 726d  tary` to perform
-00000f10: 2061 7574 6f6d 6174 6963 2064 6966 6665   automatic diffe
-00000f20: 7265 6e74 6961 7469 6f6e 206f 6e20 626f  rentiation on bo
-00000f30: 7468 206c 617a 7920 616e 6420 7374 7265  th lazy and stre
-00000f40: 616d 696e 6720 6772 6170 6873 2e0a 0a23  aming graphs...#
-00000f50: 2047 7261 7068 2056 6973 7561 6c69 7a61   Graph Visualiza
-00000f60: 7469 6f6e 0a59 6f75 2063 616e 2076 6973  tion.You can vis
-00000f70: 7561 6c69 7a65 2074 6865 2067 7261 7068  ualize the graph
-00000f80: 2077 6974 6820 4772 6170 6876 697a 2e20   with Graphviz. 
-00000f90: 416c 6c20 7374 7265 616d 696e 6720 616e  All streaming an
-00000fa0: 6420 6c61 7a79 206e 6f64 6573 2073 7570  d lazy nodes sup
-00000fb0: 706f 7274 2061 2060 6772 6170 6876 697a  port a `graphviz
-00000fc0: 6020 6d65 7468 6f64 2e0a 0a53 7472 6561  ` method...Strea
-00000fd0: 6d69 6e67 2061 6e64 206c 617a 7920 6e6f  ming and lazy no
-00000fe0: 6465 7320 616c 736f 2073 7570 706f 7274  des also support
-00000ff0: 205b 6970 7964 6167 7265 6433 5d28 6874   [ipydagred3](ht
-00001000: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001010: 2f74 696d 6b70 6169 6e65 2f69 7079 6461  /timkpaine/ipyda
-00001020: 6772 6564 3329 2066 6f72 206c 6976 6520  gred3) for live 
-00001030: 7570 6461 7465 206d 6f6e 6974 6f72 696e  update monitorin
-00001040: 672e 0a0a 2323 2053 7472 6561 6d69 6e67  g...## Streaming
-00001050: 0a21 5b5d 2868 7474 7073 3a2f 2f72 6177  .![](https://raw
-00001060: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00001070: 6e74 2e63 6f6d 2f74 696d 6b70 6169 6e65  nt.com/timkpaine
-00001080: 2f74 7269 6275 7461 7279 2f6d 6169 6e2f  /tributary/main/
-00001090: 646f 6373 2f69 6d67 2f73 7472 6561 6d69  docs/img/streami
-000010a0: 6e67 2f64 6167 7265 6433 2e67 6966 290a  ng/dagred3.gif).
-000010b0: 0a48 6572 6520 6772 6565 6e20 696e 6469  .Here green indi
-000010c0: 6361 7465 7320 6578 6563 7574 696e 672c  cates executing,
-000010d0: 2079 656c 6c6f 7720 696e 6469 6361 7465   yellow indicate
-000010e0: 7320 7374 616c 6c65 6420 666f 7220 6261  s stalled for ba
-000010f0: 636b 7072 6573 7375 7265 2c20 616e 6420  ckpressure, and 
-00001100: 7265 6420 696e 6469 6361 7465 7320 7468  red indicates th
-00001110: 6174 2060 5374 7265 616d 456e 6460 2068  at `StreamEnd` h
-00001120: 6173 2062 6565 6e20 7072 6f70 6f67 6174  as been propogat
-00001130: 6564 2028 652e 672e 2073 7472 6561 6d20  ed (e.g. stream 
-00001140: 6861 7320 656e 6465 6429 2e0a 0a23 2320  has ended)...## 
-00001150: 4c61 7a79 0a21 5b5d 2868 7474 7073 3a2f  Lazy.![](https:/
-00001160: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00001170: 6f6e 7465 6e74 2e63 6f6d 2f74 696d 6b70  ontent.com/timkp
-00001180: 6169 6e65 2f74 7269 6275 7461 7279 2f6d  aine/tributary/m
-00001190: 6169 6e2f 646f 6373 2f69 6d67 2f6c 617a  ain/docs/img/laz
-000011a0: 792f 6461 6772 6564 332e 6769 6629 0a0a  y/dagred3.gif)..
-000011b0: 4865 7265 2067 7265 656e 2069 6e64 6963  Here green indic
-000011c0: 6174 6573 2065 7865 6375 7469 6e67 2c20  ates executing, 
-000011d0: 616e 6420 7265 6420 696e 6469 6361 7465  and red indicate
-000011e0: 7320 7468 6174 2074 6865 206e 6f64 6520  s that the node 
-000011f0: 6973 2064 6972 7479 2e20 4e6f 7465 2074  is dirty. Note t
-00001200: 6865 2074 6865 2064 6574 6572 6d69 6e61  he the determina
-00001210: 7469 6f6e 2069 6620 6120 6e6f 6465 2069  tion if a node i
-00001220: 7320 6469 7274 7920 6973 2061 6c73 6f20  s dirty is also 
-00001230: 646f 6e65 206c 617a 696c 7920 2877 6520  done lazily (we 
-00001240: 6361 6e20 6368 6563 6b20 7769 7468 2060  can check with `
-00001250: 6973 4469 7274 7960 2077 6863 6968 2077  isDirty` whcih w
-00001260: 696c 6c20 7570 6461 7465 2074 6865 206e  ill update the n
-00001270: 6f64 6527 7320 6772 6170 6820 7374 6174  ode's graph stat
-00001280: 652e 0a0a 2323 2043 6174 616c 6f67 0a53  e...## Catalog.S
-00001290: 6565 2074 6865 205b 4341 5441 4c4f 475d  ee the [CATALOG]
-000012a0: 2843 4154 414c 4f47 2e6d 6429 2066 6f72  (CATALOG.md) for
-000012b0: 2061 2066 756c 6c20 6c69 7374 206f 6620   a full list of 
-000012c0: 6675 6e63 7469 6f6e 732c 2074 7261 6e73  functions, trans
-000012d0: 666f 726d 732c 2073 6f75 7263 6573 2c20  forms, sources, 
-000012e0: 616e 6420 7369 6e6b 732e 0a0a 2323 2053  and sinks...## S
-000012f0: 7570 706f 7274 202f 2043 6f6e 7472 6962  upport / Contrib
-00001300: 7574 6f72 730a 5468 616e 6b73 2074 6f20  utors.Thanks to 
-00001310: 7468 6520 666f 6c6c 6f77 696e 6720 6f72  the following or
-00001320: 6761 6e69 7a61 7469 6f6e 7320 666f 7220  ganizations for 
-00001330: 7072 6f76 6964 696e 6720 636f 6465 206f  providing code o
-00001340: 7220 6669 6e61 6e63 6961 6c20 7375 7070  r financial supp
-00001350: 6f72 742e 0a0a 0a3c 6120 6872 6566 3d22  ort....<a href="
-00001360: 6874 7470 733a 2f2f 6e65 6d6f 756c 6f75  https://nemoulou
-00001370: 732e 636f 6d22 3e3c 696d 6720 7372 633d  s.com"><img src=
-00001380: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00001390: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-000013a0: 6f6d 2f74 696d 6b70 6169 6e65 2f74 7269  om/timkpaine/tri
-000013b0: 6275 7461 7279 2f6d 6169 6e2f 646f 6373  butary/main/docs
-000013c0: 2f69 6d67 2f6e 656d 2e70 6e67 2220 7769  /img/nem.png" wi
-000013d0: 6474 683d 2235 3022 3e3c 2f61 3e0a 0a3c  dth="50"></a>..<
-000013e0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000013f0: 6e65 6d6f 756c 6f75 732e 636f 6d22 3e4e  nemoulous.com">N
-00001400: 656d 6f75 6c6f 7573 3c2f 613e 0a0a 2323  emoulous</a>..##
-00001410: 204c 6963 656e 7365 0a54 6869 7320 736f   License.This so
-00001420: 6674 7761 7265 2069 7320 6c69 6365 6e73  ftware is licens
-00001430: 6564 2075 6e64 6572 2074 6865 2041 7061  ed under the Apa
-00001440: 6368 6520 322e 3020 6c69 6365 6e73 652e  che 2.0 license.
-00001450: 2053 6565 2074 6865 205b 4c49 4345 4e53   See the [LICENS
-00001460: 455d 284c 4943 454e 5345 2920 6669 6c65  E](LICENSE) file
-00001470: 2066 6f72 2064 6574 6169 6c73 2e0a 0a23   for details...#
-00001480: 2320 416c 7465 726e 6174 6976 6573 0a48  # Alternatives.H
-00001490: 6572 6520 6973 2061 6e20 696e 636f 6d70  ere is an incomp
-000014a0: 6c65 7465 206c 6973 7420 6f66 206c 6962  lete list of lib
-000014b0: 7261 7269 6573 2077 6869 6368 2069 6d70  raries which imp
-000014c0: 6c65 6d65 6e74 2073 696d 696c 6172 2f6f  lement similar/o
-000014d0: 7665 726c 6170 7069 6e67 2066 756e 6374  verlapping funct
-000014e0: 696f 6e61 6c69 7479 0a0a 2d20 5b6d 616e  ionality..- [man
-000014f0: 2d67 726f 7570 2f6d 6466 5d28 6874 7470  -group/mdf](http
-00001500: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00001510: 616e 2d67 726f 7570 2f6d 6466 290a 2d20  an-group/mdf).- 
-00001520: 5b63 6564 7269 636c 6572 6f79 2f70 7975  [cedricleroy/pyu
-00001530: 6e67 6f5d 2868 7474 7073 3a2f 2f67 6974  ngo](https://git
-00001540: 6875 622e 636f 6d2f 6365 6472 6963 6c65  hub.com/cedricle
-00001550: 726f 792f 7079 756e 676f 290a 2d20 5b70  roy/pyungo).- [p
-00001560: 7974 686f 6e2d 7374 7265 616d 7a2f 7374  ython-streamz/st
-00001570: 7265 616d 7a5d 2868 7474 7073 3a2f 2f67  reamz](https://g
-00001580: 6974 6875 622e 636f 6d2f 7079 7468 6f6e  ithub.com/python
-00001590: 2d73 7472 6561 6d7a 2f73 7472 6561 6d7a  -streamz/streamz
-000015a0: 290a 2d20 5b45 6e74 696c 5a68 612f 7079  ).- [EntilZha/py
-000015b0: 6675 6e63 7469 6f6e 616c 5d28 6874 7470  functional](http
-000015c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
-000015d0: 6e74 696c 5a68 612f 5079 4675 6e63 7469  ntilZha/PyFuncti
-000015e0: 6f6e 616c 290a 2d20 5b73 7469 7463 6866  onal).- [stitchf
-000015f0: 6978 2f68 616d 696c 746f 6e5d 2868 7474  ix/hamilton](htt
-00001600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001610: 7374 6974 6368 6669 782f 6861 6d69 6c74  stitchfix/hamilt
-00001620: 6f6e 290a 0a0a 0a                        on)....
+00000080: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7472  //github.com/str
+00000090: 6561 6d6c 6574 2d64 6576 2f74 7269 6275  eamlet-dev/tribu
+000000a0: 7461 7279 0a41 7574 686f 723a 2054 696d  tary.Author: Tim
+000000b0: 2050 6169 6e65 0a41 7574 686f 722d 656d   Paine.Author-em
+000000c0: 6169 6c3a 2074 2e70 6169 6e65 3135 3440  ail: t.paine154@
+000000d0: 676d 6169 6c2e 636f 6d0a 4c69 6365 6e73  gmail.com.Licens
+000000e0: 653a 2041 7061 6368 6520 322e 300a 4b65  e: Apache 2.0.Ke
+000000f0: 7977 6f72 6473 3a20 7374 7265 616d 696e  ywords: streamin
+00000100: 6720 6c61 7a79 2067 7261 7068 2064 6167  g lazy graph dag
+00000110: 2064 6174 6166 6c6f 7720 7265 6163 7469   dataflow reacti
+00000120: 7665 0a43 6c61 7373 6966 6965 723a 2044  ve.Classifier: D
+00000130: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
+00000140: 7320 3a3a 2033 202d 2041 6c70 6861 0a43  s :: 3 - Alpha.C
+00000150: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000160: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000170: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a43  :: Python :: 3.C
+00000180: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000190: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+000001b0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000001c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001e0: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
+000001f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000200: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000210: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
+00000220: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000240: 3a3a 2033 2e31 300a 5265 7175 6972 6573  :: 3.10.Requires
+00000250: 2d50 7974 686f 6e3a 203e 3d33 2e37 0a44  -Python: >=3.7.D
+00000260: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000270: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000280: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
+00000290: 4578 7472 613a 2064 6576 0a50 726f 7669  Extra: dev.Provi
+000002a0: 6465 732d 4578 7472 613a 2064 6576 656c  des-Extra: devel
+000002b0: 6f70 0a50 726f 7669 6465 732d 4578 7472  op.Provides-Extr
+000002c0: 613a 2066 756e 6374 696f 6e61 6c0a 4c69  a: functional.Li
+000002d0: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
+000002e0: 4e53 450a 0a23 203c 696d 6720 7372 633d  NSE..# <img src=
+000002f0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+00000300: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000310: 6f6d 2f73 7472 6561 6d6c 6574 2d64 6576  om/streamlet-dev
+00000320: 2f74 7269 6275 7461 7279 2f6d 6169 6e2f  /tributary/main/
+00000330: 646f 6373 2f69 6d67 2f69 636f 6e2e 706e  docs/img/icon.pn
+00000340: 6722 2077 6964 7468 3d22 3330 3022 3e0a  g" width="300">.
+00000350: 5079 7468 6f6e 2044 6174 6120 5374 7265  Python Data Stre
+00000360: 616d 730a 0a5b 215b 4275 696c 6420 5374  ams..[![Build St
+00000370: 6174 7573 5d28 6874 7470 733a 2f2f 6769  atus](https://gi
+00000380: 7468 7562 2e63 6f6d 2f73 7472 6561 6d6c  thub.com/streaml
+00000390: 6574 2d64 6576 2f74 7269 6275 7461 7279  et-dev/tributary
+000003a0: 2f77 6f72 6b66 6c6f 7773 2f42 7569 6c64  /workflows/Build
+000003b0: 2532 3053 7461 7475 732f 6261 6467 652e  %20Status/badge.
+000003c0: 7376 673f 6272 616e 6368 3d6d 6169 6e29  svg?branch=main)
+000003d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000003e0: 2e63 6f6d 2f73 7472 6561 6d6c 6574 2d64  .com/streamlet-d
+000003f0: 6576 2f74 7269 6275 7461 7279 2f61 6374  ev/tributary/act
+00000400: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
+00000410: 6c6f 7725 3341 2532 3242 7569 6c64 2b53  low%3A%22Build+S
+00000420: 7461 7475 7325 3232 290a 5b21 5b43 6f76  tatus%22).[![Cov
+00000430: 6572 6167 655d 2868 7474 7073 3a2f 2f63  erage](https://c
+00000440: 6f64 6563 6f76 2e69 6f2f 6768 2f73 7472  odecov.io/gh/str
+00000450: 6561 6d6c 6574 2d64 6576 2f74 7269 6275  eamlet-dev/tribu
+00000460: 7461 7279 2f62 7261 6e63 682f 6d61 696e  tary/branch/main
+00000470: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
+00000480: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00000490: 6f76 2e69 6f2f 6768 2f73 7472 6561 6d6c  ov.io/gh/streaml
+000004a0: 6574 2d64 6576 2f74 7269 6275 7461 7279  et-dev/tributary
+000004b0: 290a 5b21 5b50 7950 495d 2868 7474 7073  ).[![PyPI](https
+000004c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004d0: 6f2f 7079 7069 2f6c 2f74 7269 6275 7461  o/pypi/l/tributa
+000004e0: 7279 2e73 7667 295d 2868 7474 7073 3a2f  ry.svg)](https:/
+000004f0: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+00000500: 2f70 7970 692f 7472 6962 7574 6172 7929  /pypi/tributary)
+00000510: 0a5b 215b 5079 5049 5d28 6874 7470 733a  .[![PyPI](https:
+00000520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000530: 2f70 7970 692f 762f 7472 6962 7574 6172  /pypi/v/tributar
+00000540: 792e 7376 6729 5d28 6874 7470 733a 2f2f  y.svg)](https://
+00000550: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
+00000560: 7079 7069 2f74 7269 6275 7461 7279 290a  pypi/tributary).
+00000570: 5b21 5b42 696e 6465 725d 2868 7474 7073  [![Binder](https
+00000580: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
+00000590: 6261 6467 655f 6c6f 676f 2e73 7667 295d  badge_logo.svg)]
+000005a0: 2868 7474 7073 3a2f 2f6d 7962 696e 6465  (https://mybinde
+000005b0: 722e 6f72 672f 7632 2f67 682f 7374 7265  r.org/v2/gh/stre
+000005c0: 616d 6c65 742d 6465 762f 7472 6962 7574  amlet-dev/tribut
+000005d0: 6172 792f 6d61 696e 3f75 726c 7061 7468  ary/main?urlpath
+000005e0: 3d6c 6162 290a 0a0a 5472 6962 7574 6172  =lab)...Tributar
+000005f0: 7920 6973 2061 206c 6962 7261 7279 2066  y is a library f
+00000600: 6f72 2063 6f6e 7374 7275 6374 696e 6720  or constructing 
+00000610: 6461 7461 666c 6f77 2067 7261 7068 7320  dataflow graphs 
+00000620: 696e 2070 7974 686f 6e2e 2055 6e6c 696b  in python. Unlik
+00000630: 6520 6d61 6e79 206f 7468 6572 2044 4147  e many other DAG
+00000640: 206c 6962 7261 7269 6573 2069 6e20 7079   libraries in py
+00000650: 7468 6f6e 2028 5b61 6972 666c 6f77 5d28  thon ([airflow](
+00000660: 6874 7470 733a 2f2f 6169 7266 6c6f 772e  https://airflow.
+00000670: 6170 6163 6865 2e6f 7267 292c 205b 6c75  apache.org), [lu
+00000680: 6967 695d 2868 7474 7073 3a2f 2f6c 7569  igi](https://lui
+00000690: 6769 2e72 6561 6474 6865 646f 6373 2e69  gi.readthedocs.i
+000006a0: 6f2f 656e 2f73 7461 626c 652f 292c 205b  o/en/stable/), [
+000006b0: 7072 6566 6563 745d 2868 7474 7073 3a2f  prefect](https:/
+000006c0: 2f64 6f63 732e 7072 6566 6563 742e 696f  /docs.prefect.io
+000006d0: 292c 205b 6461 6773 7465 725d 2868 7474  ), [dagster](htt
+000006e0: 7073 3a2f 2f64 6f63 732e 6461 6773 7465  ps://docs.dagste
+000006f0: 722e 696f 292c 205b 6461 736b 5d28 6874  r.io), [dask](ht
+00000700: 7470 733a 2f2f 6461 736b 2e6f 7267 292c  tps://dask.org),
+00000710: 205b 6b65 6472 6f5d 2868 7474 7073 3a2f   [kedro](https:/
+00000720: 2f67 6974 6875 622e 636f 6d2f 7175 616e  /github.com/quan
+00000730: 7475 6d62 6c61 636b 6c61 6273 2f6b 6564  tumblacklabs/ked
+00000740: 726f 292c 2065 7463 292c 2074 7269 6275  ro), etc), tribu
+00000750: 7461 7279 2069 7320 6e6f 7420 6465 7369  tary is not desi
+00000760: 676e 6564 2077 6974 6820 6461 7461 2f65  gned with data/e
+00000770: 746c 2070 6970 656c 696e 6573 206f 7220  tl pipelines or 
+00000780: 7363 6865 6475 6c69 6e67 2069 6e20 6d69  scheduling in mi
+00000790: 6e64 2e20 496e 7374 6561 642c 2074 7269  nd. Instead, tri
+000007a0: 6275 7461 7279 2069 7320 6d6f 7265 2073  butary is more s
+000007b0: 696d 696c 6172 2074 6f20 6c69 6272 6172  imilar to librar
+000007c0: 6965 7320 6c69 6b65 205b 6d64 665d 2868  ies like [mdf](h
+000007d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000007e0: 6d2f 6d61 6e2d 6772 6f75 702f 6d64 6629  m/man-group/mdf)
+000007f0: 2c20 5b6c 6f6d 616e 5d28 6874 7470 733a  , [loman](https:
+00000800: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 616e  //github.com/jan
+00000810: 7573 6865 6e64 6572 736f 6e61 7373 6574  ushendersonasset
+00000820: 616c 6c6f 6361 7469 6f6e 2f6c 6f6d 616e  allocation/loman
+00000830: 292c 205b 7079 756e 676f 5d28 6874 7470  ), [pyungo](http
+00000840: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000850: 6564 7269 636c 6572 6f79 2f70 7975 6e67  edricleroy/pyung
+00000860: 6f29 2c20 5b73 7472 6561 6d7a 5d28 6874  o), [streamz](ht
+00000870: 7470 733a 2f2f 7374 7265 616d 7a2e 7265  tps://streamz.re
+00000880: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000890: 6c61 7465 7374 2f29 2c20 6f72 205b 7079  latest/), or [py
+000008a0: 6675 6e63 7469 6f6e 616c 5d28 6874 7470  functional](http
+000008b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
+000008c0: 6e74 696c 5a68 612f 5079 4675 6e63 7469  ntilZha/PyFuncti
+000008d0: 6f6e 616c 292c 2069 6e20 7468 6174 2069  onal), in that i
+000008e0: 7420 6973 2064 6573 6967 6e65 6420 746f  t is designed to
+000008f0: 2062 6520 7573 6564 2061 7320 7468 6520   be used as the 
+00000900: 696d 706c 656d 656e 7461 7469 6f6e 2066  implementation f
+00000910: 6f72 2061 2064 6174 6120 6d6f 6465 6c2e  or a data model.
+00000920: 204f 6e65 2073 7563 6820 6578 616d 706c   One such exampl
+00000930: 6520 6973 2074 6865 205b 6772 6565 6b73  e is the [greeks
+00000940: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000950: 2e63 6f6d 2f73 7472 6561 6d6c 6574 2d64  .com/streamlet-d
+00000960: 6576 2f67 7265 656b 7329 206c 6962 7261  ev/greeks) libra
+00000970: 7279 2c20 7768 6963 6820 6c65 7665 7261  ry, which levera
+00000980: 6765 7320 7472 6962 7574 6172 7920 746f  ges tributary to
+00000990: 2062 7569 6c64 2064 6174 6120 6d6f 6465   build data mode
+000009a0: 6c73 2066 6f72 205b 6f70 7469 6f6e 7320  ls for [options 
+000009b0: 7072 6963 696e 675d 2868 7474 7073 3a2f  pricing](https:/
+000009c0: 2f77 7777 2e69 6e76 6573 746f 7065 6469  /www.investopedi
+000009d0: 612e 636f 6d2f 6172 7469 636c 6573 2f6f  a.com/articles/o
+000009e0: 7074 696f 6e69 6e76 6573 746f 722f 3037  ptioninvestor/07
+000009f0: 2f6f 7074 696f 6e73 5f62 6561 745f 6d61  /options_beat_ma
+00000a00: 726b 6574 2e61 7370 292e 200a 0a21 5b5d  rket.asp). ..![]
+00000a10: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00000a20: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000a30: 6f6d 2f73 7472 6561 6d6c 6574 2d64 6576  om/streamlet-dev
+00000a40: 2f74 7269 6275 7461 7279 2f6d 6169 6e2f  /tributary/main/
+00000a50: 646f 6373 2f69 6d67 2f65 7861 6d70 6c65  docs/img/example
+00000a60: 2e67 6966 290a 0a0a 2320 496e 7374 616c  .gif)...# Instal
+00000a70: 6c61 7469 6f6e 0a49 6e73 7461 6c6c 2077  lation.Install w
+00000a80: 6974 6820 7069 703a 0a0a 6070 6970 2069  ith pip:..`pip i
+00000a90: 6e73 7461 6c6c 2074 7269 6275 7461 7279  nstall tributary
+00000aa0: 600a 0a6f 7220 7769 7468 2063 6f6e 6461  `..or with conda
+00000ab0: 3a0a 0a60 636f 6e64 6120 696e 7374 616c  :..`conda instal
+00000ac0: 6c20 2d63 2063 6f6e 6461 2d66 6f72 6765  l -c conda-forge
+00000ad0: 2074 7269 6275 7461 7279 600a 0a6f 7220   tributary`..or 
+00000ae0: 6672 6f6d 2073 6f75 7263 653a 0a0a 6070  from source:..`p
+00000af0: 7974 686f 6e20 7365 7475 702e 7079 2069  ython setup.py i
+00000b00: 6e73 7461 6c6c 600a 0a4e 6f74 653a 2049  nstall`..Note: I
+00000b10: 6620 696e 7374 616c 6c69 6e67 2066 726f  f installing fro
+00000b20: 6d20 736f 7572 6365 206f 7220 7769 7468  m source or with
+00000b30: 2070 6970 2c20 796f 7527 6c6c 2061 6c73   pip, you'll als
+00000b40: 6f20 6e65 6564 205b 4772 6170 6876 697a  o need [Graphviz
+00000b50: 2069 7473 656c 665d 2868 7474 7073 3a2f   itself](https:/
+00000b60: 2f77 7777 2e67 7261 7068 7669 7a2e 6f72  /www.graphviz.or
+00000b70: 672f 646f 776e 6c6f 6164 2f29 2069 6620  g/download/) if 
+00000b80: 796f 7520 7761 6e74 2074 6f20 7669 7375  you want to visu
+00000b90: 616c 697a 6520 7468 6520 6772 6170 6820  alize the graph 
+00000ba0: 7573 696e 6720 7468 6520 602e 6772 6170  using the `.grap
+00000bb0: 6876 697a 2829 6020 6d65 7468 6f64 2e0a  hviz()` method..
+00000bc0: 0a23 2053 7472 6561 6d20 5479 7065 730a  .# Stream Types.
+00000bd0: 5472 6962 7574 6172 7920 6f66 6665 7273  Tributary offers
+00000be0: 2073 6576 6572 616c 206b 696e 6473 206f   several kinds o
+00000bf0: 6620 7374 7265 616d 733a 0a0a 2323 2053  f streams:..## S
+00000c00: 7472 6561 6d69 6e67 0a54 6865 7365 2061  treaming.These a
+00000c10: 7265 2073 796e 6368 726f 6e6f 7573 2c20  re synchronous, 
+00000c20: 7265 6163 7469 7665 2064 6174 6120 7374  reactive data st
+00000c30: 7265 616d 732c 2062 7569 6c74 2075 7369  reams, built usi
+00000c40: 6e67 2061 7379 6e63 6872 6f6e 6f75 7320  ng asynchronous 
+00000c50: 7079 7468 6f6e 2067 656e 6572 6174 6f72  python generator
+00000c60: 732e 2054 6865 7920 6172 6520 6465 7369  s. They are desi
+00000c70: 676e 6564 2074 6f20 6d69 6d69 6320 636f  gned to mimic co
+00000c80: 6d70 6c65 7820 6576 656e 7420 7072 6f63  mplex event proc
+00000c90: 6573 736f 7273 2069 6e20 7465 726d 7320  essors in terms 
+00000ca0: 6f66 2065 7665 6e74 206f 7264 6572 696e  of event orderin
+00000cb0: 672e 0a0a 2323 2046 756e 6374 696f 6e61  g...## Functiona
+00000cc0: 6c0a 5468 6573 6520 6172 6520 6675 6e63  l.These are func
+00000cd0: 7469 6f6e 616c 2073 7472 6561 6d73 2c20  tional streams, 
+00000ce0: 6275 696c 7420 6279 2063 7572 7279 696e  built by curryin
+00000cf0: 6720 7079 7468 6f6e 2066 756e 6374 696f  g python functio
+00000d00: 6e73 2028 6361 6c6c 6261 636b 7329 2e20  ns (callbacks). 
+00000d10: 0a0a 2323 204c 617a 790a 5468 6573 6520  ..## Lazy.These 
+00000d20: 6172 6520 6c61 7a69 6c79 2d65 7661 6c75  are lazily-evalu
+00000d30: 6174 6564 2070 7974 686f 6e20 7374 7265  ated python stre
+00000d40: 616d 732c 2077 6865 7265 206f 7574 7075  ams, where outpu
+00000d50: 7473 2061 7265 2070 726f 706f 6761 7465  ts are propogate
+00000d60: 6420 6f6e 6c79 2061 7320 696e 7075 7473  d only as inputs
+00000d70: 2063 6861 6e67 652e 2054 6865 7920 6172   change. They ar
+00000d80: 6520 696d 706c 656d 656e 7465 6420 6173  e implemented as
+00000d90: 2064 6972 6563 7465 6420 6163 7963 6c69   directed acycli
+00000da0: 6320 6772 6170 6873 2e0a 0a23 2045 7861  c graphs...# Exa
+00000db0: 6d70 6c65 730a 2d20 5b53 7472 6561 6d69  mples.- [Streami
+00000dc0: 6e67 5d28 646f 6373 2f65 7861 6d70 6c65  ng](docs/example
+00000dd0: 732f 7374 7265 616d 696e 672f 7374 7265  s/streaming/stre
+00000de0: 616d 696e 672e 6d64 293a 2049 6e20 7468  aming.md): In th
+00000df0: 6973 2065 7861 6d70 6c65 2c20 7765 2063  is example, we c
+00000e00: 6f6e 7374 7275 6374 2061 2076 6172 6965  onstruct a varie
+00000e10: 7479 206f 6620 666f 7277 6172 6420 7072  ty of forward pr
+00000e20: 6f70 6f67 6174 696e 6720 7265 6163 7469  opogating reacti
+00000e30: 7665 2067 7261 7068 732e 0a2d 205b 4c61  ve graphs..- [La
+00000e40: 7a79 5d28 646f 6373 2f65 7861 6d70 6c65  zy](docs/example
+00000e50: 732f 6c61 7a79 2f6c 617a 792e 6d64 293a  s/lazy/lazy.md):
+00000e60: 2049 6e20 7468 6973 2065 7861 6d70 6c65   In this example
+00000e70: 2c20 7765 2063 6f6e 7374 7275 6374 2061  , we construct a
+00000e80: 2076 6172 6965 7479 206f 6620 6c61 7a69   variety of lazi
+00000e90: 6c79 2d65 7661 6c75 6174 6564 2064 6972  ly-evaluated dir
+00000ea0: 6563 7465 6420 6163 7963 6c69 6320 636f  ected acyclic co
+00000eb0: 6d70 7574 6174 696f 6e20 6772 6170 6873  mputation graphs
+00000ec0: 2e20 0a2d 205b 4175 746f 6d61 7469 6320  . .- [Automatic 
+00000ed0: 4469 6666 6572 656e 7469 6174 696f 6e5d  Differentiation]
+00000ee0: 2864 6f63 732f 6578 616d 706c 6573 2f61  (docs/examples/a
+00000ef0: 7574 6f64 6966 662f 6175 746f 6469 6666  utodiff/autodiff
+00000f00: 2e6d 6429 3a20 496e 2074 6869 7320 6578  .md): In this ex
+00000f10: 616d 706c 652c 2077 6520 7573 6520 6074  ample, we use `t
+00000f20: 7269 6275 7461 7279 6020 746f 2070 6572  ributary` to per
+00000f30: 666f 726d 2061 7574 6f6d 6174 6963 2064  form automatic d
+00000f40: 6966 6665 7265 6e74 6961 7469 6f6e 206f  ifferentiation o
+00000f50: 6e20 626f 7468 206c 617a 7920 616e 6420  n both lazy and 
+00000f60: 7374 7265 616d 696e 6720 6772 6170 6873  streaming graphs
+00000f70: 2e0a 0a23 2047 7261 7068 2056 6973 7561  ...# Graph Visua
+00000f80: 6c69 7a61 7469 6f6e 0a59 6f75 2063 616e  lization.You can
+00000f90: 2076 6973 7561 6c69 7a65 2074 6865 2067   visualize the g
+00000fa0: 7261 7068 2077 6974 6820 4772 6170 6876  raph with Graphv
+00000fb0: 697a 2e20 416c 6c20 7374 7265 616d 696e  iz. All streamin
+00000fc0: 6720 616e 6420 6c61 7a79 206e 6f64 6573  g and lazy nodes
+00000fd0: 2073 7570 706f 7274 2061 2060 6772 6170   support a `grap
+00000fe0: 6876 697a 6020 6d65 7468 6f64 2e0a 0a53  hviz` method...S
+00000ff0: 7472 6561 6d69 6e67 2061 6e64 206c 617a  treaming and laz
+00001000: 7920 6e6f 6465 7320 616c 736f 2073 7570  y nodes also sup
+00001010: 706f 7274 205b 6970 7964 6167 7265 6433  port [ipydagred3
+00001020: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001030: 2e63 6f6d 2f74 696d 6b70 6169 6e65 2f69  .com/timkpaine/i
+00001040: 7079 6461 6772 6564 3329 2066 6f72 206c  pydagred3) for l
+00001050: 6976 6520 7570 6461 7465 206d 6f6e 6974  ive update monit
+00001060: 6f72 696e 672e 0a0a 2323 2053 7472 6561  oring...## Strea
+00001070: 6d69 6e67 0a21 5b5d 2868 7474 7073 3a2f  ming.![](https:/
+00001080: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001090: 6f6e 7465 6e74 2e63 6f6d 2f73 7472 6561  ontent.com/strea
+000010a0: 6d6c 6574 2d64 6576 2f74 7269 6275 7461  mlet-dev/tributa
+000010b0: 7279 2f6d 6169 6e2f 646f 6373 2f69 6d67  ry/main/docs/img
+000010c0: 2f73 7472 6561 6d69 6e67 2f64 6167 7265  /streaming/dagre
+000010d0: 6433 2e67 6966 290a 0a48 6572 6520 6772  d3.gif)..Here gr
+000010e0: 6565 6e20 696e 6469 6361 7465 7320 6578  een indicates ex
+000010f0: 6563 7574 696e 672c 2079 656c 6c6f 7720  ecuting, yellow 
+00001100: 696e 6469 6361 7465 7320 7374 616c 6c65  indicates stalle
+00001110: 6420 666f 7220 6261 636b 7072 6573 7375  d for backpressu
+00001120: 7265 2c20 616e 6420 7265 6420 696e 6469  re, and red indi
+00001130: 6361 7465 7320 7468 6174 2060 5374 7265  cates that `Stre
+00001140: 616d 456e 6460 2068 6173 2062 6565 6e20  amEnd` has been 
+00001150: 7072 6f70 6f67 6174 6564 2028 652e 672e  propogated (e.g.
+00001160: 2073 7472 6561 6d20 6861 7320 656e 6465   stream has ende
+00001170: 6429 2e0a 0a23 2320 4c61 7a79 0a21 5b5d  d)...## Lazy.![]
+00001180: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00001190: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000011a0: 6f6d 2f73 7472 6561 6d6c 6574 2d64 6576  om/streamlet-dev
+000011b0: 2f74 7269 6275 7461 7279 2f6d 6169 6e2f  /tributary/main/
+000011c0: 646f 6373 2f69 6d67 2f6c 617a 792f 6461  docs/img/lazy/da
+000011d0: 6772 6564 332e 6769 6629 0a0a 4865 7265  gred3.gif)..Here
+000011e0: 2067 7265 656e 2069 6e64 6963 6174 6573   green indicates
+000011f0: 2065 7865 6375 7469 6e67 2c20 616e 6420   executing, and 
+00001200: 7265 6420 696e 6469 6361 7465 7320 7468  red indicates th
+00001210: 6174 2074 6865 206e 6f64 6520 6973 2064  at the node is d
+00001220: 6972 7479 2e20 4e6f 7465 2074 6865 2074  irty. Note the t
+00001230: 6865 2064 6574 6572 6d69 6e61 7469 6f6e  he determination
+00001240: 2069 6620 6120 6e6f 6465 2069 7320 6469   if a node is di
+00001250: 7274 7920 6973 2061 6c73 6f20 646f 6e65  rty is also done
+00001260: 206c 617a 696c 7920 2877 6520 6361 6e20   lazily (we can 
+00001270: 6368 6563 6b20 7769 7468 2060 6973 4469  check with `isDi
+00001280: 7274 7960 2077 6863 6968 2077 696c 6c20  rty` whcih will 
+00001290: 7570 6461 7465 2074 6865 206e 6f64 6527  update the node'
+000012a0: 7320 6772 6170 6820 7374 6174 652e 0a0a  s graph state...
+000012b0: 2323 2043 6174 616c 6f67 0a53 6565 2074  ## Catalog.See t
+000012c0: 6865 205b 4341 5441 4c4f 475d 2843 4154  he [CATALOG](CAT
+000012d0: 414c 4f47 2e6d 6429 2066 6f72 2061 2066  ALOG.md) for a f
+000012e0: 756c 6c20 6c69 7374 206f 6620 6675 6e63  ull list of func
+000012f0: 7469 6f6e 732c 2074 7261 6e73 666f 726d  tions, transform
+00001300: 732c 2073 6f75 7263 6573 2c20 616e 6420  s, sources, and 
+00001310: 7369 6e6b 732e 0a0a 2323 2053 7570 706f  sinks...## Suppo
+00001320: 7274 202f 2043 6f6e 7472 6962 7574 6f72  rt / Contributor
+00001330: 730a 5468 616e 6b73 2074 6f20 7468 6520  s.Thanks to the 
+00001340: 666f 6c6c 6f77 696e 6720 6f72 6761 6e69  following organi
+00001350: 7a61 7469 6f6e 7320 666f 7220 7072 6f76  zations for prov
+00001360: 6964 696e 6720 636f 6465 206f 7220 6669  iding code or fi
+00001370: 6e61 6e63 6961 6c20 7375 7070 6f72 742e  nancial support.
+00001380: 0a0a 0a3c 6120 6872 6566 3d22 6874 7470  ...<a href="http
+00001390: 733a 2f2f 6e65 6d6f 756c 6f75 732e 636f  s://nemoulous.co
+000013a0: 6d22 3e3c 696d 6720 7372 633d 2268 7474  m"><img src="htt
+000013b0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+000013c0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f73  sercontent.com/s
+000013d0: 7472 6561 6d6c 6574 2d64 6576 2f74 7269  treamlet-dev/tri
+000013e0: 6275 7461 7279 2f6d 6169 6e2f 646f 6373  butary/main/docs
+000013f0: 2f69 6d67 2f6e 656d 2e70 6e67 2220 7769  /img/nem.png" wi
+00001400: 6474 683d 2235 3022 3e3c 2f61 3e0a 0a3c  dth="50"></a>..<
+00001410: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001420: 6e65 6d6f 756c 6f75 732e 636f 6d22 3e4e  nemoulous.com">N
+00001430: 656d 6f75 6c6f 7573 3c2f 613e 0a0a 2323  emoulous</a>..##
+00001440: 204c 6963 656e 7365 0a54 6869 7320 736f   License.This so
+00001450: 6674 7761 7265 2069 7320 6c69 6365 6e73  ftware is licens
+00001460: 6564 2075 6e64 6572 2074 6865 2041 7061  ed under the Apa
+00001470: 6368 6520 322e 3020 6c69 6365 6e73 652e  che 2.0 license.
+00001480: 2053 6565 2074 6865 205b 4c49 4345 4e53   See the [LICENS
+00001490: 455d 284c 4943 454e 5345 2920 6669 6c65  E](LICENSE) file
+000014a0: 2066 6f72 2064 6574 6169 6c73 2e0a 0a23   for details...#
+000014b0: 2320 416c 7465 726e 6174 6976 6573 0a48  # Alternatives.H
+000014c0: 6572 6520 6973 2061 6e20 696e 636f 6d70  ere is an incomp
+000014d0: 6c65 7465 206c 6973 7420 6f66 206c 6962  lete list of lib
+000014e0: 7261 7269 6573 2077 6869 6368 2069 6d70  raries which imp
+000014f0: 6c65 6d65 6e74 2073 696d 696c 6172 2f6f  lement similar/o
+00001500: 7665 726c 6170 7069 6e67 2066 756e 6374  verlapping funct
+00001510: 696f 6e61 6c69 7479 0a0a 2d20 5b6d 616e  ionality..- [man
+00001520: 2d67 726f 7570 2f6d 6466 5d28 6874 7470  -group/mdf](http
+00001530: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00001540: 616e 2d67 726f 7570 2f6d 6466 290a 2d20  an-group/mdf).- 
+00001550: 5b63 6564 7269 636c 6572 6f79 2f70 7975  [cedricleroy/pyu
+00001560: 6e67 6f5d 2868 7474 7073 3a2f 2f67 6974  ngo](https://git
+00001570: 6875 622e 636f 6d2f 6365 6472 6963 6c65  hub.com/cedricle
+00001580: 726f 792f 7079 756e 676f 290a 2d20 5b70  roy/pyungo).- [p
+00001590: 7974 686f 6e2d 7374 7265 616d 7a2f 7374  ython-streamz/st
+000015a0: 7265 616d 7a5d 2868 7474 7073 3a2f 2f67  reamz](https://g
+000015b0: 6974 6875 622e 636f 6d2f 7079 7468 6f6e  ithub.com/python
+000015c0: 2d73 7472 6561 6d7a 2f73 7472 6561 6d7a  -streamz/streamz
+000015d0: 290a 2d20 5b45 6e74 696c 5a68 612f 7079  ).- [EntilZha/py
+000015e0: 6675 6e63 7469 6f6e 616c 5d28 6874 7470  functional](http
+000015f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f45  s://github.com/E
+00001600: 6e74 696c 5a68 612f 5079 4675 6e63 7469  ntilZha/PyFuncti
+00001610: 6f6e 616c 290a 2d20 5b73 7469 7463 6866  onal).- [stitchf
+00001620: 6978 2f68 616d 696c 746f 6e5d 2868 7474  ix/hamilton](htt
+00001630: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001640: 7374 6974 6368 6669 782f 6861 6d69 6c74  stitchfix/hamilt
+00001650: 6f6e 290a 0a                             on)..
```

### Comparing `tributary-0.2.0/tributary.egg-info/SOURCES.txt` & `tributary-0.2.1/tributary.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 setup.cfg
```

### Comparing `tributary-0.2.0/tributary.egg-info/requires.txt` & `tributary-0.2.1/tributary.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 socketIO-client-nexus>=0.7.6
 sympy>=1.5.1
 temporal-cache>=0.0.6
 tornado>=5.1.1
 twilio>=6.50.1
 
 [dev]
-black>=20.
+black>=23
 check-manifest
 flake8>=3.7.8
 flake8-black>=0.2.1
 mock
 pybind11>=2.4.0
 pytest>=4.3.0
 pytest-cov>=2.6.1
@@ -60,15 +60,15 @@
 socketIO-client-nexus>=0.7.6
 sympy>=1.5.1
 temporal-cache>=0.0.6
 tornado>=5.1.1
 twilio>=6.50.1
 
 [develop]
-black>=20.
+black>=23
 check-manifest
 flake8>=3.7.8
 flake8-black>=0.2.1
 mock
 pybind11>=2.4.0
 pytest>=4.3.0
 pytest-cov>=2.6.1
```

