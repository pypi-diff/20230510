# Comparing `tmp/sarus-0.6.0.dev0.tar.gz` & `tmp/sarus-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sarus-0.6.0.dev0.tar", last modified: Tue May  2 06:50:18 2023, max compression
+gzip compressed data, was "sarus-0.6.1.tar", last modified: Wed May 10 18:38:07 2023, max compression
```

## Comparing `sarus-0.6.0.dev0.tar` & `sarus-0.6.1.tar`

### file list

```diff
@@ -1,101 +1,104 @@
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/
--rw-rw-r--   0 vl        (1001) vl        (1002)      100 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/pyproject.toml
--rwxrwxr-x   0 vl        (1001) vl        (1002)      111 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/setup.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      663 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/README.rst
--rw-rw-r--   0 vl        (1001) vl        (1002)       25 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/MANIFEST.in
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/
--rw-rw-r--   0 vl        (1001) vl        (1002)      743 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/debug.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/xgboost/
--rw-rw-r--   0 vl        (1001) vl        (1002)      213 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/xgboost/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      755 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/xgboost/xgboost.py
--rw-rw-r--   0 vl        (1001) vl        (1002)    10518 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/utils.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/pandas/
--rw-rw-r--   0 vl        (1001) vl        (1002)      197 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     4918 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/dataframe.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      822 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/core.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      206 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/io.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/std/
--rw-rw-r--   0 vl        (1001) vl        (1002)      154 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/std/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     1074 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/std/types.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/
--rw-rw-r--   0 vl        (1001) vl        (1002)       81 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      841 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/profile_report.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      549 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/__init__.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/
--rw-rw-r--   0 vl        (1001) vl        (1002)      100 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)    16606 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/dataframe.py
--rw-rw-r--   0 vl        (1001) vl        (1002)       42 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/__init__.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/
--rw-rw-r--   0 vl        (1001) vl        (1002)      132 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)    42361 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/model.py
--rw-rw-r--   0 vl        (1001) vl        (1002)    13194 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vl        (1001) vl        (1002)    13051 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/config.yaml
--rw-rw-r--   0 vl        (1001) vl        (1002)     1708 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/typing.py
--rw-rw-r--   0 vl        (1001) vl        (1002)    55988 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/sarus.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/plotly/
--rw-rw-r--   0 vl        (1001) vl        (1002)      108 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/plotly/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      138 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/plotly/express.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/tensorflow/
--rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/tensorflow/__init__.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/context/
--rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      302 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/typing.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     3069 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/local_sdk.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     1461 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/wrapper_factory.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/sklearn/
--rw-rw-r--   0 vl        (1001) vl        (1002)      766 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/compose.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      680 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      566 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/impute.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      174 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/metrics.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      594 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/svm.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      668 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     1569 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      814 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      558 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     6604 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/cluster.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      177 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/inspection.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     1112 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vl        (1001) vl        (1002)    11437 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/ensemble.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/scripts/
--rw-rw-r--   0 vl        (1001) vl        (1002)     4618 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/scripts/generate_op_list.py
--rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/scripts/__init__.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/numpy/
--rw-rw-r--   0 vl        (1001) vl        (1002)      337 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)       81 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/random.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      963 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/scalars.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/storage/
--rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/storage/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     4552 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/storage/legacy_local.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/imblearn/
--rw-rw-r--   0 vl        (1001) vl        (1002)      265 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      556 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/under_sampling.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      558 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      578 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vl        (1001) vl        (1002)    14156 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/dataspec_wrapper.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/manager/
--rw-rw-r--   0 vl        (1001) vl        (1002)    19293 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     1949 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     1595 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/value_remote.py
--rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     2556 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/typing.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     6201 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/dataspec_api.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     5360 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/arrow_local.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     3733 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     4599 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/value_local.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     3352 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/parquet_local.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/manager/ops/
--rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      921 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/ops/api.py
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/skopt/
--rw-rw-r--   0 vl        (1001) vl        (1002)      223 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/skopt/__init__.py
--rw-rw-r--   0 vl        (1001) vl        (1002)      929 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/skopt/searchcv.py
--rw-rw-r--   0 vl        (1001) vl        (1002)     1830 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/PKG-INFO
-drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/
--rw-rw-r--   0 vl        (1001) vl        (1002)        6 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/top_level.txt
--rw-rw-r--   0 vl        (1001) vl        (1002)        1 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vl        (1001) vl        (1002)     2036 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vl        (1001) vl        (1002)        1 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vl        (1001) vl        (1002)     1830 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vl        (1001) vl        (1002)      344 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/requires.txt
--rwxrwxr-x   0 vl        (1001) vl        (1002)     1301 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/setup.cfg
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.1/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-10 18:38:07.212508 sarus-0.6.1/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.1/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.1/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.200508 sarus-0.6.1/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-10 13:10:09.000000 sarus-0.6.1/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13051 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13713 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/legacy/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.1/sarus/legacy/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.1/sarus/legacy/pandas/dataframe.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.1/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5351 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1925 2023-05-10 18:35:08.000000 sarus-0.6.1/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1239 2023-05-10 18:35:08.000000 sarus-0.6.1/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3734 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6201 2023-05-10 13:10:09.000000 sarus-0.6.1/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3352 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    19300 2023-05-10 13:10:09.000000 sarus-0.6.1/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2556 2023-05-04 12:45:45.000000 sarus-0.6.1/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4591 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1572 2023-05-10 18:35:08.000000 sarus-0.6.1/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    55942 2023-05-10 13:10:09.000000 sarus-0.6.1/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4618 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.208508 sarus-0.6.1/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1112 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1569 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1074 2022-11-29 13:03:29.000000 sarus-0.6.1/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/storage/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.1/sarus/storage/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.1/sarus/storage/legacy_local.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1780 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11037 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.1/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.1/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      755 2023-05-05 09:59:58.000000 sarus-0.6.1/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.204508 sarus-0.6.1/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-10 18:38:06.000000 sarus-0.6.1/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2086 2023-05-10 18:38:07.000000 sarus-0.6.1/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-10 18:38:06.000000 sarus-0.6.1/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.1/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      349 2023-05-10 18:38:06.000000 sarus-0.6.1/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-10 18:38:06.000000 sarus-0.6.1/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1306 2023-05-10 18:38:07.212508 sarus-0.6.1/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-10 18:37:18.000000 sarus-0.6.1/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-10 18:38:07.212508 sarus-0.6.1/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.1/tests/test_sanity.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sarus-0.6.0.dev0/README.rst` & `sarus-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/debug.py` & `sarus-0.6.1/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/xgboost/xgboost.py` & `sarus-0.6.1/sarus/xgboost/xgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_init
+from sarus.utils import register_ops, sarus_init, sarus_method
 
 try:
     import xgboost
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
```

### Comparing `sarus-0.6.0.dev0/sarus/utils.py` & `sarus-0.6.1/sarus/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,25 @@
     for key in keys:
         if module_conf is None:
             return
         module_conf = module_conf.get(key)
     return module_conf
 
 
-def eval(x: Any, target_epsilon: Optional[float] = None) -> st.DataSpecValue:
+def eval(
+    x: Any,
+    target_epsilon: Optional[float] = None,
+    verbose: Optional[int] = None,
+) -> st.DataSpecValue:
     """Recursively evaluates DataSpecWrappers to values."""
     if isinstance(x, DataSpecWrapper):
-        return x.__sarus_eval__(target_epsilon)
+        if verbose is None:
+            context: LocalSDKContext = global_context()
+            verbose = context.verbose()
+        return x.__sarus_eval__(target_epsilon, verbose)
 
     if target_epsilon is not None:
         logger.warning(
             "Ignoring `target_epsilon` since the evaluated object"
             " is not a Sarus object."
         )
 
@@ -195,14 +202,19 @@
         i: arg
         for i, arg in enumerate(args)
         if not isinstance(arg, DataSpecWrapper)
     }
     ds_args_pos = [
         i for i, arg in enumerate(args) if isinstance(arg, DataSpecWrapper)
     ]
+    ds_arg_types = {
+        i: str(arg.__wraps__)
+        for i, arg in enumerate(args)
+        if isinstance(arg, DataSpecWrapper)
+    }
     ds_args = [
         arg.dataspec(DataSpecVariant.USER_DEFINED)
         for arg in args
         if isinstance(arg, DataSpecWrapper)
     ]
     py_kwargs = {
         name: arg
@@ -210,19 +222,25 @@
         if not isinstance(arg, DataSpecWrapper)
     }
     ds_kwargs = {
         name: arg.dataspec(DataSpecVariant.USER_DEFINED)
         for name, arg in kwargs.items()
         if isinstance(arg, DataSpecWrapper)
     }
+    ds_kwargs_types = {
+        name: str(arg.__wraps__)
+        for name, arg in kwargs.items()
+        if isinstance(arg, DataSpecWrapper)
+    }
     transform = external(
         id=code_name,
         py_args=py_args,
         py_kwargs=py_kwargs,
         ds_args_pos=ds_args_pos,
+        ds_types={**ds_arg_types, **ds_kwargs_types},
     )
     new_dataspec = transform(*ds_args, **ds_kwargs)
     return new_dataspec
 
 
 def _sarus_op(
     code_name: str,
```

### Comparing `sarus-0.6.0.dev0/sarus/pandas/dataframe.py` & `sarus-0.6.1/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/pandas/core.py` & `sarus-0.6.1/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/std/types.py` & `sarus-0.6.1/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/__init__.py` & `sarus-0.6.1/sarus/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.6.0.dev0"
+VERSION = "0.6.0"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.6.0.dev0/sarus/legacy/pandas/dataframe.py` & `sarus-0.6.1/sarus/legacy/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/legacy/tensorflow/model.py` & `sarus-0.6.1/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/legacy/tensorflow/dataset.py` & `sarus-0.6.1/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/config.yaml` & `sarus-0.6.1/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/typing.py` & `sarus-0.6.1/sarus/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,17 @@
         ...
 
     def dataspec(
         self, kind: DataSpecVariant = DataSpecVariant.USER_DEFINED
     ) -> st.DataSpec:
         ...
 
-    def __sarus_eval__(self) -> st.DataSpecValue:
+    def __sarus_eval__(
+        self, target_epsilon: Optional[float] = None, verbose: int = 1
+    ) -> st.DataSpecValue:
         """Return value of synthetic variant."""
         ...
 
 
 class DataSpecWrapperFactory(Protocol):
     def register(
         self,
```

### Comparing `sarus-0.6.0.dev0/sarus/sarus.py` & `sarus-0.6.1/sarus/sarus.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,75 +22,64 @@
 from __future__ import annotations  # noqa: F407
 
 import base64
 import datetime
 import decimal
 import getpass
 import hashlib
+import http
 import io
 import json
 import logging
 import os
-import pickle as pkl
 import re
 import sys
 import tarfile
 import tempfile
 import textwrap
 import time
 import typing as t
 import warnings
 import webbrowser
 from dataclasses import dataclass
 from io import BytesIO
-import http
 from typing import Any, Dict, List, Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 import sarus_data_spec
 from PIL import Image
 from requests import Session
+from sarus_data_spec.attribute import attach_properties
 
 import sarus.typing as srt
 from sarus.dataspec_wrapper import DataSpecWrapper
 from sarus.manager.dataspec_api import (
     compile_dataspec,
-    pull_dataspec_graph,
     get_dataspec,
+    pull_dataspec_graph,
+    raise_response,
 )
 from sarus.manager.typing import SDKManager
-from sarus.manager.dataspec_api import raise_response
 from sarus.pandas.dataframe import DataFrame
-from sarus_data_spec.attribute import attach_properties
 
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import sarus_data_spec.protobuf as sp
     import sarus_data_spec.typing as st
-    from sarus_data_spec.constants import (
-        ARROW_TASK,
-        CACHE,
-        CACHE_PATH,
-        SCHEMA_TASK,
-    )
+    from sarus_data_spec.constants import BIG_DATA_TASK, SCHEMA_TASK
     from sarus_data_spec.context import push_global_context
     from sarus_data_spec.dataspec_rewriter.simple_rules import attach_variant
     from sarus_data_spec.dataspec_validator.privacy_limit import (
         DeltaEpsilonLimit,
     )
-    from sarus_data_spec.protobuf.utilities import (
-        deserialize,
-        dict_deserialize,
-        serialize,
-    )
-    from sarus_data_spec.status import last_statuses, ready
+    from sarus_data_spec.protobuf.utilities import dict_deserialize
     from sarus_data_spec.transform import extract, select_sql
     from sarus_data_spec.variant_constraint import (
         mock_constraint,
         pep_constraint,
     )
 
     from sarus.context.local_sdk import LocalSDKContext
@@ -1124,36 +1113,40 @@
             r"(?:/?|[/?]\S+)$",
             re.IGNORECASE,
         )
         return re.match(regex, url) is not None
 
     def __init__(
         self,
-        url="http://0.0.0.0:5000",
-        google_login=False,
-        email=None,
-        password=None,
+        url: str = "http://0.0.0.0:5000",
+        google_login: bool = False,
+        email: Optional[str] = None,
+        password: Optional[str] = None,
+        verbose: int = 1,
     ):
         # TODO : progress bar self.progress_bar = Progbar(100,
         # stateful_metrics=None)
 
         if self._url_validator(url):
             self.base_url = url
         else:
             raise Exception("Bad url")
         self._session = Session()
         if google_login:
             self._oidc_login()
         else:
             self._credentials_login(email, password)
 
-        self._context = LocalSDKContext(self)
+        self._context = LocalSDKContext(self, verbose=verbose)
         self._context.set_sync_policy(srt.SyncPolicy.SEND_ON_VALUE)
         push_global_context(self._context)
 
+    def set_verbose(self, verbose: int) -> None:
+        self._context._verbose = verbose
+
     def context(self) -> LocalSDKContext:
         return self._context
 
     def url(self):
         return self.base_url
 
     def session(self):
```

### Comparing `sarus-0.6.0.dev0/sarus/context/local_sdk.py` & `sarus-0.6.1/sarus/context/local_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 
 from ..typing import SyncPolicy
 
 
 class LocalSDKContext(PublicContext):
     """A default context"""
 
-    def __init__(self, client: Client) -> None:
+    def __init__(self, client: Client, verbose: int = 1) -> None:
         super().__init__()
         self._storage = Storage()  # type:ignore
         self._sync_policy = SyncPolicy.SEND_ON_INIT
         self.client = client
         self._manager = manager(self.storage(), self.client)
+        self._verbose = verbose
 
         self._dataspec_factory = Factory()
         self.factory().register(
             sp.type_name(sp.Dataset),
             lambda protobuf, store: Dataset(cast(sp.Dataset, protobuf), store),
         )
         self.factory().register(
@@ -70,14 +71,17 @@
             sarus_wrapper_class,
         ) in MetaWrapper._wrapper_classes:
             self._wrapper_factory.register(
                 python_classname=python_classname,
                 sarus_wrapper_class=sarus_wrapper_class,
             )
 
+    def verbose(self) -> int:
+        return self._verbose
+
     def factory(self) -> Factory:
         return self._dataspec_factory
 
     def wrapper_factory(self) -> DataSpecWrapperFactory:
         return self._wrapper_factory
 
     def storage(self) -> Storage:
```

### Comparing `sarus-0.6.0.dev0/sarus/wrapper_factory.py` & `sarus-0.6.1/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/compose.py` & `sarus-0.6.1/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/__init__.py` & `sarus-0.6.1/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/impute.py` & `sarus-0.6.1/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/svm.py` & `sarus-0.6.1/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/linear_model.py` & `sarus-0.6.1/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/preprocessing.py` & `sarus-0.6.1/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/decomposition.py` & `sarus-0.6.1/sarus/sklearn/decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_init
+from sarus.utils import register_ops, sarus_init, sarus_method
 
 try:
     import sklearn.decomposition as decomposition
     from sklearn.decomposition import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
```

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/pipeline.py` & `sarus-0.6.1/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/cluster.py` & `sarus-0.6.1/sarus/sklearn/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import numpy as np
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_init
+from sarus.utils import register_ops, sarus_init, sarus_method
 
 try:
     from sklearn import cluster
     from sklearn.cluster import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
```

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/model_selection.py` & `sarus-0.6.1/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/sklearn/ensemble.py` & `sarus-0.6.1/sarus/sklearn/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import sarus_data_spec.protobuf as sp
 
 from sarus.dataspec_wrapper import DataSpecWrapper
-from sarus.utils import register_ops, sarus_method, sarus_init
+from sarus.utils import register_ops, sarus_init, sarus_method
 
 try:
     import sklearn.ensemble as ensemble
     from sklearn.ensemble import *
 except ModuleNotFoundError:
     pass  # error message in sarus_data_spec.typing
```

### Comparing `sarus-0.6.0.dev0/sarus/scripts/generate_op_list.py` & `sarus-0.6.1/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/numpy/scalars.py` & `sarus-0.6.1/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/storage/legacy_local.py` & `sarus-0.6.1/sarus/storage/legacy_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/imblearn/under_sampling.py` & `sarus-0.6.1/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/imblearn/pipeline.py` & `sarus-0.6.1/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/imblearn/over_sampling.py` & `sarus-0.6.1/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/dataspec_wrapper.py` & `sarus-0.6.1/sarus/dataspec_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from __future__ import annotations
 
 import inspect
 import logging
-import warnings
 from typing import (
     Any,
     Dict,
     Generic,
-    Iterator,
     List,
     Optional,
     Tuple,
     TypeVar,
     cast,
     get_args,
 )
 
-import pandas as pd
-import pyarrow as pa
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 from sarus_data_spec.context import global_context
 from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
 
 from sarus.context.typing import LocalSDKContext
 from sarus.manager.typing import SDKManager
@@ -344,22 +340,15 @@
                 "This might be due to privacy budget "
                 "constraints or some operations not "
                 "compilable with Differential Privacy."
             )
 
         if alt_dataspec.prototype() == sp.Dataset:
             dataset = cast(st.Dataset, alt_dataspec)
-            mapping = {key: val for val, key in MetaWrapper._wrapper_classes}
-            python_class = mapping[type(self)]
-            if python_class == str(pd.DataFrame):
-                value = dataset.to_pandas()
-            elif python_class == str(Iterator[pa.RecordBatch]):
-                value = dataset.to_arrow()
-            else:
-                raise TypeError(f"Dataset not viewable as {python_class}")
+            value = dataset.to(self.__wraps__)
         else:
             scalar = cast(st.Scalar, alt_dataspec)
             value = cast(st.Scalar, scalar.value())
 
         if verbose >= 1:
             message = alt_policy.value
             if alt_policy == DataspecPrivacyPolicy.DP:
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/sdk_manager.py` & `sarus-0.6.1/sarus/manager/sdk_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,37 +8,39 @@
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.status as stt
 import sarus_data_spec.storage.typing as storage_typing
 import sarus_data_spec.typing as st
 from sarus_data_spec.attribute import attach_properties
 from sarus_data_spec.constants import (
     ARROW_TASK,
-    SCALAR_TASK,
     BIG_DATA_TASK,
     IS_BIG_DATA,
+    SCALAR_TASK,
 )
+from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
+from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
 from sarus_data_spec.manager.base import Base
 from sarus_data_spec.manager.computations.base import BaseComputation
 from sarus_data_spec.manager.computations.local.schema import SchemaComputation
-from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
-from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
-from .arrow_local import ToArrowComputation
-from .value_local import ValueComputation
-from .cache_scalar_local import CacheScalarComputation
-from .parquet_local import ToParquetComputation
-import sarus.manager.dataspec_api as api
-import sarus.manager.ops.api as api_ops
-from sarus_data_spec.manager.ops.source.routing import SourceScalar
-from sarus.typing import ADMIN_DS, MOCK, PYTHON_TYPE, Client
 from sarus_data_spec.manager.ops.processor.routing import (
     TransformedDataset,
     TransformedScalar,
 )
+from sarus_data_spec.manager.ops.source.routing import SourceScalar
+
+import sarus.manager.dataspec_api as api
+import sarus.manager.ops.api as api_ops
+from sarus.typing import ADMIN_DS, MOCK, PYTHON_TYPE, Client
+
 
+from .arrow_local import ToArrowComputation
 from .arrow_remote import ToArrowComputationOnServer
+from .cache_scalar_local import CacheScalarComputation
+from .parquet_local import ToParquetComputation
+from .value_local import ValueComputation
 from .value_remote import ValueComputationOnServer
 
 
 class SDKManager(Base):
     """The Manager of the SDK running on the client side.
 
     This Manager has two additional functionalities compared to the
@@ -426,15 +428,15 @@
         else:
             msg = "No status found."
         if msg:
             msg = "\n" + msg
 
         if dataspec.is_pep():
             label_type = f"{label_type} (PEP)"
-        if self.query_manager().is_dp(dataspec):
+        if self.dataspec_validator().is_dp(dataspec):
             label_type = f"{label_type} (DP)"
 
         label = f"{label_type}: {symbol}{msg}"
 
         return (
             f'"{dataspec.uuid()}"[label="{label}", '
             f'fillcolor="{fillcolor}", color="{color}", shape={shape}]'
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/arrow_remote.py` & `sarus-0.6.1/sarus/manager/arrow_remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import typing as t
 
 import pyarrow as pa
-
+import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import ARROW_TASK
-from sarus_data_spec.manager.computations.remote.base import RemoteComputation
 from sarus_data_spec.manager.computations.base import (
     ErrorCatchingAsyncIterator,
 )
-import sarus_data_spec.status as stt
-from .dataspec_api import dataset_result, launch_dataspec, dataspec_status
+from sarus.manager.base_remote import RemoteComputation
+from .dataspec_api import dataset_result, dataspec_status, launch_dataspec
 
 
 class ToArrowComputationOnServer(
     RemoteComputation[t.AsyncIterator[pa.RecordBatch]]
 ):
     """ToArrowComputation on the Sarus server through the REST API."""
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/value_remote.py` & `sarus-0.6.1/sarus/manager/value_remote.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
+import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import SCALAR_TASK
-from sarus_data_spec.manager.computations.remote.base import RemoteComputation
+from sarus.manager.base_remote import RemoteComputation
 
-from .dataspec_api import launch_dataspec, scalar_result, dataspec_status
-import sarus_data_spec.status as stt
+from .dataspec_api import dataspec_status, launch_dataspec, scalar_result
 
 
 class ValueComputationOnServer(RemoteComputation[t.Any]):
     """ValueComputation on the Sarus server through the REST API."""
 
     task_name = SCALAR_TASK
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/typing.py` & `sarus-0.6.1/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/manager/dataspec_api.py` & `sarus-0.6.1/sarus/manager/dataspec_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
+import json
 import pickle as pkl
 import typing as t
-import json
 from http import HTTPStatus
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 from requests import Response
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/arrow_local.py` & `sarus-0.6.1/sarus/manager/arrow_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import logging
 import traceback
 import typing as t
 
 import pyarrow as pa
 import pyarrow.parquet as pq
-
+import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import ARROW_TASK
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.manager.base import Base
-from sarus_data_spec.manager.computations.local.base import LocalComputation
-from sarus.manager.parquet_local import (
-    ToParquetComputation,
-)
 from sarus_data_spec.manager.computations.base import (
     ErrorCatchingAsyncIterator,
 )
+from sarus_data_spec.manager.computations.local.base import LocalComputation
+
 from sarus.manager.arrow_remote import ToArrowComputationOnServer
-import sarus_data_spec.status as stt
+from sarus.manager.parquet_local import ToParquetComputation
 
 logger = logging.getLogger(__name__)
 
 
 class ToArrowComputation(LocalComputation[t.AsyncIterator[pa.RecordBatch]]):
     task_name = ARROW_TASK
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/cache_scalar_local.py` & `sarus-0.6.1/sarus/manager/cache_scalar_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import logging
 import os
 import pickle as pkl
 import traceback
 import typing as t
 
+import sarus_data_spec.protobuf as sp
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import (
     CACHE_PATH,
     CACHE_PROTO,
     CACHE_SCALAR_TASK,
     CACHE_TYPE,
     ScalarCaching,
 )
 from sarus_data_spec.manager.base import Base
 from sarus_data_spec.manager.computations.local.base import LocalComputation
-from sarus.manager.value_remote import ValueComputationOnServer
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.status import DataSpecErrorStatus, error, ready
-import sarus_data_spec.protobuf as sp
+
+from sarus.manager.value_remote import ValueComputationOnServer
 
 logger = logging.getLogger(__name__)
 
 
 class CacheScalarComputation(LocalComputation[t.Tuple[str, str]]):
     """Class responsible for handling the caching
     in of a scalar. It wraps a ValueComputation to get the value."""
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/value_local.py` & `sarus-0.6.1/sarus/manager/value_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import logging
 import pickle as pkl
 import traceback
 import typing as t
 
+import sarus_data_spec.protobuf as sp
+import sarus_data_spec.status as stt
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import SCALAR_TASK, ScalarCaching
 from sarus_data_spec.manager.base import Base
 from sarus_data_spec.manager.computations.local.base import LocalComputation
-from sarus.manager.cache_scalar_local import (
-    CacheScalarComputation,
-)
-from sarus.manager.value_remote import ValueComputationOnServer
 from sarus_data_spec.scalar import Scalar
-import sarus_data_spec.protobuf as sp
-import sarus_data_spec.status as stt
+
+from sarus.manager.cache_scalar_local import CacheScalarComputation
+from sarus.manager.value_remote import ValueComputationOnServer
 
 logger = logging.getLogger(__name__)
 
 
 class ValueComputation(LocalComputation[t.Any]):
     """Class responsible for handling the computation
     of scalars."""
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/parquet_local.py` & `sarus-0.6.1/sarus/manager/parquet_local.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 import os
 import traceback
 import typing as t
 
 import pyarrow as pa
 import pyarrow.parquet as pq
-
 from sarus_data_spec import typing as st
 from sarus_data_spec.constants import CACHE_PATH, TO_PARQUET_TASK
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.manager.base import Base
-from sarus.manager.arrow_remote import ToArrowComputationOnServer
-from sarus_data_spec.status import DataSpecErrorStatus, error, ready
 from sarus_data_spec.manager.computations.local.base import LocalComputation
+from sarus_data_spec.status import DataSpecErrorStatus, error, ready
+
+from sarus.manager.arrow_remote import ToArrowComputationOnServer
 
 logger = logging.getLogger(__name__)
 
 BATCH_SIZE = 10000
 
 
 class ToParquetComputation(LocalComputation[str]):
```

### Comparing `sarus-0.6.0.dev0/sarus/manager/ops/api.py` & `sarus-0.6.1/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/sarus/skopt/searchcv.py` & `sarus-0.6.1/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0.dev0/PKG-INFO` & `sarus-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,17 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.0.dev0
+Version: 0.6.1
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
+Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
-Description: 
-        Sarus
-        
-        ===
-        
-        Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
-        
-        Installation
-        ------------
-        
-        PIP
-        ^^^
-        
-        To install locally the latest available version :
-        
-        ``pip install sarus``
-        
-        Usage
-        -----
-        
-        Client
-        ^^^^^^
-        
-        Use this class to connect to **Sarus Gateway**.
-        
-        .. code-block:: python
-        
-           from sarus import Client
-        
-           client = Client(url="http://admin.sarus.tech:5000")
-           available = client.available_datasets()
-           print(f'Datasets available on the server: {available}')
-        
 Keywords: differential privacy,AI,Data privacy
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -54,7 +21,40 @@
 Provides-Extra: imblearn
 Provides-Extra: tensorflow
 Provides-Extra: pandas_profiling
 Provides-Extra: plotly
 Provides-Extra: xgboost
 Provides-Extra: skopt
 Provides-Extra: tests
+
+
+Sarus
+
+===
+
+Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
+
+Installation
+------------
+
+PIP
+^^^
+
+To install locally the latest available version :
+
+``pip install sarus``
+
+Usage
+-----
+
+Client
+^^^^^^
+
+Use this class to connect to **Sarus Gateway**.
+
+.. code-block:: python
+
+   from sarus import Client
+
+   client = Client(url="http://admin.sarus.tech:5000")
+   available = client.available_datasets()
+   print(f'Datasets available on the server: {available}')
```

### Comparing `sarus-0.6.0.dev0/sarus.egg-info/SOURCES.txt` & `sarus-0.6.1/sarus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 sarus/legacy/pandas/dataframe.py
 sarus/legacy/tensorflow/__init__.py
 sarus/legacy/tensorflow/dataset.py
 sarus/legacy/tensorflow/model.py
 sarus/manager/__init__.py
 sarus/manager/arrow_local.py
 sarus/manager/arrow_remote.py
+sarus/manager/base_remote.py
 sarus/manager/cache_scalar_local.py
 sarus/manager/dataspec_api.py
 sarus/manager/parquet_local.py
 sarus/manager/sdk_manager.py
 sarus/manager/typing.py
 sarus/manager/value_local.py
 sarus/manager/value_remote.py
@@ -72,8 +73,9 @@
 sarus/skopt/searchcv.py
 sarus/std/__init__.py
 sarus/std/types.py
 sarus/storage/__init__.py
 sarus/storage/legacy_local.py
 sarus/tensorflow/__init__.py
 sarus/xgboost/__init__.py
-sarus/xgboost/xgboost.py
+sarus/xgboost/xgboost.py
+tests/test_sanity.py
```

### Comparing `sarus-0.6.0.dev0/sarus.egg-info/PKG-INFO` & `sarus-0.6.1/sarus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,17 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.0.dev0
+Version: 0.6.1
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
+Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
-Description: 
-        Sarus
-        
-        ===
-        
-        Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
-        
-        Installation
-        ------------
-        
-        PIP
-        ^^^
-        
-        To install locally the latest available version :
-        
-        ``pip install sarus``
-        
-        Usage
-        -----
-        
-        Client
-        ^^^^^^
-        
-        Use this class to connect to **Sarus Gateway**.
-        
-        .. code-block:: python
-        
-           from sarus import Client
-        
-           client = Client(url="http://admin.sarus.tech:5000")
-           available = client.available_datasets()
-           print(f'Datasets available on the server: {available}')
-        
 Keywords: differential privacy,AI,Data privacy
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -54,7 +21,40 @@
 Provides-Extra: imblearn
 Provides-Extra: tensorflow
 Provides-Extra: pandas_profiling
 Provides-Extra: plotly
 Provides-Extra: xgboost
 Provides-Extra: skopt
 Provides-Extra: tests
+
+
+Sarus
+
+===
+
+Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
+
+Installation
+------------
+
+PIP
+^^^
+
+To install locally the latest available version :
+
+``pip install sarus``
+
+Usage
+-----
+
+Client
+^^^^^^
+
+Use this class to connect to **Sarus Gateway**.
+
+.. code-block:: python
+
+   from sarus import Client
+
+   client = Client(url="http://admin.sarus.tech:5000")
+   available = client.available_datasets()
+   print(f'Datasets available on the server: {available}')
```

### Comparing `sarus-0.6.0.dev0/setup.cfg` & `sarus-0.6.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.0.0
+	sarus-data-spec-public==3.1.2.dev0
 	matplotlib>=3.1
 	cloudpickle>=1.2, <2.1
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.1.1
 	scipy==1.9.0
```

