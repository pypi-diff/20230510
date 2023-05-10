# Comparing `tmp/IQM-VIS-0.2.5.29.tar.gz` & `tmp/IQM-Vis-0.2.5.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IQM-VIS-0.2.5.29.tar", last modified: Mon Mar  6 11:12:35 2023, max compression
+gzip compressed data, was "IQM-Vis-0.2.5.63.tar", last modified: Wed May 10 12:08:31 2023, max compression
```

## Comparing `IQM-VIS-0.2.5.29.tar` & `IQM-Vis-0.2.5.63.tar`

### file list

```diff
@@ -1,52 +1,62 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.969485 IQM-VIS-0.2.5.29/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.965485 IQM-VIS-0.2.5.29/IQM_VIS/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.965485 IQM-VIS-0.2.5.29/IQM_VIS/UI/
--rw-rw-r--   0 matt      (1000) matt      (1000)       83 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/UI/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6381 2023-03-06 11:07:59.000000 IQM-VIS-0.2.5.29/IQM_VIS/UI/images.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     6475 2023-03-05 18:57:12.000000 IQM-VIS-0.2.5.29/IQM_VIS/UI/layout.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2111 2023-03-06 10:38:14.000000 IQM-VIS-0.2.5.29/IQM_VIS/UI/main.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      201 2022-11-24 10:49:31.000000 IQM-VIS-0.2.5.29/IQM_VIS/UI/style.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    11180 2023-03-06 11:10:24.000000 IQM-VIS-0.2.5.29/IQM_VIS/UI/widgets.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      240 2022-11-24 10:42:19.000000 IQM-VIS-0.2.5.29/IQM_VIS/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4411 2023-03-05 16:24:59.000000 IQM-VIS-0.2.5.29/IQM_VIS/data_api.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.965485 IQM-VIS-0.2.5.29/IQM_VIS/examples/
--rw-rw-r--   0 matt      (1000) matt      (1000)       75 2022-11-22 18:06:44.000000 IQM-VIS-0.2.5.29/IQM_VIS/examples/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2212 2023-03-06 09:26:45.000000 IQM-VIS-0.2.5.29/IQM_VIS/examples/dataset.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1730 2022-11-28 16:03:13.000000 IQM-VIS-0.2.5.29/IQM_VIS/examples/multiple.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      961 2022-11-28 16:12:03.000000 IQM-VIS-0.2.5.29/IQM_VIS/examples/simple.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.965485 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.965485 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.965485 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/layers/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/layers/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     9218 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/layers/divisive_normalisation.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    27784 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/pyramids.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.965485 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/utils/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/utils/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1485 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/utils/conv.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5359 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/utils/fourier.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    22712 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/expert/utils/pyramid_filters.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4319 2023-03-06 09:24:38.000000 IQM-VIS-0.2.5.29/IQM_VIS/image_metrics/metrics.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.969485 IQM-VIS-0.2.5.29/IQM_VIS/transformations/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-11-15 10:45:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/transformations/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5077 2022-12-12 16:41:07.000000 IQM-VIS-0.2.5.29/IQM_VIS/transformations/transforms.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4692 2023-03-05 19:14:33.000000 IQM-VIS-0.2.5.29/IQM_VIS/ui_wrapper.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.969485 IQM-VIS-0.2.5.29/IQM_VIS/utils/
--rw-rw-r--   0 matt      (1000) matt      (1000)      154 2022-12-05 18:34:37.000000 IQM-VIS-0.2.5.29/IQM_VIS/utils/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2563 2022-12-12 16:43:41.000000 IQM-VIS-0.2.5.29/IQM_VIS/utils/gui_utils.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1023 2022-12-05 18:35:13.000000 IQM-VIS-0.2.5.29/IQM_VIS/utils/image_utils.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     7155 2023-03-06 10:36:57.000000 IQM-VIS-0.2.5.29/IQM_VIS/utils/plot_utils.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.965485 IQM-VIS-0.2.5.29/IQM_VIS.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)     2315 2023-03-06 11:12:35.000000 IQM-VIS-0.2.5.29/IQM_VIS.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     1145 2023-03-06 11:12:35.000000 IQM-VIS-0.2.5.29/IQM_VIS.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-03-06 11:12:35.000000 IQM-VIS-0.2.5.29/IQM_VIS.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       69 2023-03-06 11:12:35.000000 IQM-VIS-0.2.5.29/IQM_VIS.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       14 2023-03-06 11:12:35.000000 IQM-VIS-0.2.5.29/IQM_VIS.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     2315 2023-03-06 11:12:35.969485 IQM-VIS-0.2.5.29/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     2065 2023-03-05 15:53:48.000000 IQM-VIS-0.2.5.29/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-03-06 11:12:35.969485 IQM-VIS-0.2.5.29/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      936 2023-03-06 11:11:47.000000 IQM-VIS-0.2.5.29/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-03-06 11:12:35.969485 IQM-VIS-0.2.5.29/tests/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2022-10-25 10:42:10.000000 IQM-VIS-0.2.5.29/tests/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1154 2022-10-25 10:30:48.000000 IQM-VIS-0.2.5.29/tests/test_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.815207 IQM-Vis-0.2.5.63/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.807207 IQM-Vis-0.2.5.63/IQM_Vis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.811207 IQM-Vis-0.2.5.63/IQM_Vis/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/custom_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/experiment_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/style-dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/style-light.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23294 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/UI/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.811207 IQM-Vis-0.2.5.63/IQM_Vis/data_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/data_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/data_handlers/data_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/data_handlers/data_api_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.811207 IQM-Vis-0.2.5.63/IQM_Vis/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.811207 IQM-Vis-0.2.5.63/IQM_Vis/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/images/HIQM.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/images/waves1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    17780 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/images/waves2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/images/waves3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/examples/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.811207 IQM-Vis-0.2.5.63/IQM_Vis/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    12685 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/metrics/IQMs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.811207 IQM-Vis-0.2.5.63/IQM_Vis/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/transformations/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/ui_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.815207 IQM-Vis-0.2.5.63/IQM_Vis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/utils/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/utils/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/IQM_Vis/utils/save_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.811207 IQM-Vis-0.2.5.63/IQM_Vis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-10 12:08:31.000000 IQM-Vis-0.2.5.63/IQM_Vis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-10 12:08:31.000000 IQM-Vis-0.2.5.63/IQM_Vis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:08:31.000000 IQM-Vis-0.2.5.63/IQM_Vis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 12:08:31.000000 IQM-Vis-0.2.5.63/IQM_Vis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 12:08:31.000000 IQM-Vis-0.2.5.63/IQM_Vis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-10 12:08:31.815207 IQM-Vis-0.2.5.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:08:31.815207 IQM-Vis-0.2.5.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:31.815207 IQM-Vis-0.2.5.63/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 12:08:19.000000 IQM-Vis-0.2.5.63/tests/test_inputs.py
```

### Comparing `IQM-VIS-0.2.5.29/IQM_VIS/examples/dataset.py` & `IQM-Vis-0.2.5.63/IQM_Vis/examples/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 import os
 import numpy as np
-import IQM_VIS
+import IQM_Vis
 
 
 def run():
     # metrics functions must return a single value
-    metric = {'MAE': IQM_VIS.metrics.MAE,
-              'MSE': IQM_VIS.metrics.MSE,
-              '1-SSIM': IQM_VIS.metrics.ssim()}
+    metric = {'MAE': IQM_Vis.IQMs.MAE(),
+              'MSE': IQM_Vis.IQMs.MSE(),
+              '1-SSIM': IQM_Vis.IQMs.SSIM()
+              }
 
     # metrics images return a numpy image
-    metric_images = {'MSE': IQM_VIS.metrics.MSE_image,
-                     'SSIM': IQM_VIS.metrics.SSIM_image()}
+    metric_images = {'MSE': IQM_Vis.IQMs.MSE(return_image=True),
+                     'SSIM': IQM_Vis.IQMs.SSIM(return_image=True)}
 
     # make dataset list of images
     file_path = os.path.dirname(os.path.abspath(__file__))
     dataset = [os.path.join(file_path, 'images', 'waves1.jpeg'),
                os.path.join(file_path, 'images', 'waves2.jpeg'),
-               os.path.join(file_path, 'images', 'wave3.jpeg')]
-    data = IQM_VIS.dataset_holder(dataset,
-                                  IQM_VIS.utils.load_image,
+               os.path.join(file_path, 'images', 'waves3.jpeg')]
+    data = IQM_Vis.dataset_holder(dataset,
                                   metric,
-                                  metric_images)
+                                  metric_images,
+                                  IQM_Vis.utils.load_image,
+                                  human_exp_csv=os.path.join(file_path, 'images', 'HIQM.csv'),
+                                  )
 
     # define the transformations
     transformations = {
-               'rotation':{'min':-180, 'max':180, 'function':IQM_VIS.transforms.rotation},    # normal input
-               'blur':{'min':1, 'max':41, 'normalise':'odd', 'function':IQM_VIS.transforms.blur},  # only odd ints
-               'brightness':{'min':-1.0, 'max':1.0, 'function':IQM_VIS.transforms.brightness},   # normal but with float
-               # 'threshold':{'min':-40, 'max':40, 'function':IQM_VIS.transforms.binary_threshold},
-               'jpeg compression':{'init_value':100, 'min':1, 'max':100, 'function':IQM_VIS.transforms.jpeg_compression},
+               'rotation':{'min':-180, 'max':180, 'function':IQM_Vis.transforms.rotation},    # normal input
+               'blur':{'min':1, 'max':41, 'normalise':'odd', 'function':IQM_Vis.transforms.blur},  # only odd ints
+               'brightness':{'min':-1.0, 'max':1.0, 'function':IQM_Vis.transforms.brightness},   # normal but with float
+               # 'threshold':{'min':-40, 'max':40, 'function':IQM_Vis.transforms.binary_threshold},
+               'jpg comp.':{'init_value':100, 'min':1, 'max':100, 'function':IQM_Vis.transforms.jpeg_compression},
                }
     # define any parameters that the metrics need (names shared across both metrics and metric_images)
     ssim_params = {'sigma': {'min':0.25, 'max':5.25, 'init_value': 1.5},  # for the guassian kernel
                    # 'kernel_size': {'min':1, 'max':41, 'normalise':'odd', 'init_value': 11},  # ignored if guassian kernel used
                    'k1': {'min':0.01, 'max':0.21, 'init_value': 0.01},
                    'k2': {'min':0.01, 'max':0.21, 'init_value': 0.03}}
 
     # use the API to create the UI
-    IQM_VIS.make_UI(data,
-                transformations,
-                metrics_avg_graph=True,
-                metric_params=ssim_params)
-
+    IQM_Vis.make_UI(data,
+                    transformations,
+                    metric_params=ssim_params,
+                    )
 
 if __name__ == '__main__':
     run()
```

### Comparing `IQM-VIS-0.2.5.29/IQM_VIS/examples/multiple.py` & `IQM-Vis-0.2.5.63/IQM_Vis/examples/experiment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import os
 import numpy as np
-import IQM_VIS
+import IQM_Vis
 
 
 def run():
-    file_path = os.path.dirname(os.path.abspath(__file__))
-
     # metrics functions must return a single value
-    metric = {'MAE': IQM_VIS.metrics.MAE,
-              'MSE': IQM_VIS.metrics.MSE,
-              '1-SSIM': IQM_VIS.metrics.ssim()}
+    metric = {} #IQM_Vis.metrics.get_all_metrics()
 
     # metrics images return a numpy image
-    metric_images = {'MSE': IQM_VIS.metrics.MSE_image,
-                     'SSIM': IQM_VIS.metrics.SSIM_image()}
+    metric_images = {}
+
+    # make dataset list of images
+    file_path = os.path.dirname(os.path.abspath(__file__))
+    dataset = [os.path.join(file_path, 'images', 'waves1.jpeg'),
+               os.path.join(file_path, 'images', 'waves2.jpeg'),
+               os.path.join(file_path, 'images', 'waves3.jpeg')]
+    data = IQM_Vis.dataset_holder(dataset,
+                                  metric,
+                                  metric_images,
+                                  IQM_Vis.utils.load_image,
+                                  )
 
-    # first row of images
-    row_1 = IQM_VIS.data_holder(('X1', IQM_VIS.utils.load_image(os.path.join(file_path, 'images', 'wave3.jpeg'))),
-                             ('X1', IQM_VIS.utils.load_image(os.path.join(file_path, 'images', 'wave3.jpeg'))),
-                             metric,
-                             metric_images)
-    # second row of images
-    row_2 = IQM_VIS.data_holder(('X1', IQM_VIS.utils.load_image(os.path.join(file_path, 'images', 'wave3.jpeg'))),
-                            ('X2', IQM_VIS.utils.load_image(os.path.join(file_path, 'images', 'waves1.jpeg'))),
-                             metric,
-                             metric_images)
     # define the transformations
     transformations = {
-               'rotation':{'min':-180, 'max':180, 'function':IQM_VIS.transforms.rotation},    # normal input
-               'blur':{'min':1, 'max':41, 'normalise':'odd', 'function':IQM_VIS.transforms.blur},  # only odd ints
-               'brightness':{'min':-1.0, 'max':1.0, 'function':IQM_VIS.transforms.brightness},   # normal but with float
+    'x_shift': {'min':-1.0, 'max':1.0, 'function':IQM_Vis.transforms.brightness, 'init_value': 0.0},
                }
+    # define any parameters that the metrics need (names shared across both metrics and metric_images)
+    ssim_params = {'sigma': {'min':0.25, 'max':5.25, 'init_value': 1.5},  # for the guassian kernel
+                   # 'kernel_size': {'min':1, 'max':41, 'normalise':'odd', 'init_value': 11},  # ignored if guassian kernel used
+                   'k1': {'min':0.01, 'max':0.21, 'init_value': 0.01},
+                   'k2': {'min':0.01, 'max':0.21, 'init_value': 0.03}}
 
     # use the API to create the UI
-    IQM_VIS.make_UI([row_1, row_2],
-                transformations,
-                metrics_avg_graph=True)
-
+    IQM_Vis.make_UI(data,
+                    transformations,
+                    metric_params=ssim_params,
+                    restrict_options=3
+                    )
 
 if __name__ == '__main__':
     run()
```

### Comparing `IQM-VIS-0.2.5.29/IQM_VIS/examples/simple.py` & `IQM-Vis-0.2.5.63/IQM_Vis/examples/simple.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import os
 import numpy as np
-import IQM_VIS
+import IQM_Vis
 
 
 def run():
     file_path = os.path.dirname(os.path.abspath(__file__))
     # define simple metrics
     metric = {'MAE': lambda im1, im2: np.abs(im1 - im2).mean()}
     metric_im = {'MAE': lambda im1, im2: np.abs(im1 - im2)}
     # add numpy image and the metrics to the data handler
-    data_store = IQM_VIS.data_holder(('X', IQM_VIS.utils.load_image(os.path.join(file_path, 'images', 'wave3.jpeg'))),
-                             ('X', IQM_VIS.utils.load_image(os.path.join(file_path, 'images', 'wave3.jpeg'))),
-                             metric,
-                             metric_im)
+    data_store = IQM_Vis.dataset_holder(image_list=[os.path.join(file_path, 'images', 'waves3.jpeg')],
+                                        metrics=metric,
+                                        metric_images=metric_im)
     # define the transformations
     trans = {'brightness': {'min':-1.0, 'max':1.0, 'init_value':0, 'function':lambda im, val: np.clip(im + val, 0, 1)}}
     # use the API to create the UI
-    IQM_VIS.make_UI([data_store],
-                trans,
-                metrics_info_format='text')
+    IQM_Vis.make_UI([data_store],
+                    trans,
+                    metrics_info_format='text')
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `IQM-VIS-0.2.5.29/IQM_VIS/utils/gui_utils.py` & `IQM-Vis-0.2.5.63/IQM_Vis/utils/gui_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,41 +7,44 @@
     from PyQt6.QtGui import QPixmap, QImage
     import matplotlib; matplotlib.use('Qt5Agg')
     from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
     from matplotlib.figure import Figure
     HEADLESS = False
 except ImportError:
     import warnings
-    warnings.warn('Can not load PyQt6 library - running IQM_VIS package in headless mode')
+    warnings.warn('Can not load PyQt6 library - running IQM_Vis package in headless mode')
     HEADLESS = True
 import numpy as np
 from skimage.util import img_as_ubyte
 from skimage.transform import resize
-import cv2
-from IQM_VIS.utils.image_utils import resize_to_longest_side
+from IQM_Vis.utils.image_utils import resize_to_longest_side, calibrate_brightness
 
 '''
 image helper functions
 '''
 # def resize_im_to(np_array, size):
 #     down_im = resize(np_array, size)
 #     return img_as_ubyte(down_im)
 
-def change_im(widget, im, resize=False):
+
+def change_im(widget, im, resize=False, rgb_brightness=250, display_brightness=250):
     '''
     given a numpy image, changes the given widget Frame
     '''
-    # first convert to three channel
+    # clip image to safe bounds
+    im = np.clip(im, 0, 1)
+    # convert to three channel
     if len(im.shape) == 2:
         im = im[..., np.newaxis]
     if im.shape[2] == 1:
         im = np.concatenate([im, im, im], axis=2)
     if resize:
         im = resize_to_longest_side(im, resize)
         im = img_as_ubyte(im)
+    im = calibrate_brightness(im, rgb_brightness, display_brightness)
     qimage = QImage(im,
                     im.shape[1],
                     im.shape[0],
                     im.shape[1]*im.shape[2],
                     QImage.Format.Format_RGB888)
     pixmap = QPixmap(qimage)
     widget.setPixmap(pixmap)
@@ -59,24 +62,32 @@
     elif len(string) < length:
         string = string + append_char*(length-len(string))
     return string
 
 def get_metric_image_name(metric, data_store):
     return metric+get_image_pair_name(data_store)
 
+def get_trans_dict_from_str(trans_str, return_dict=False):
+    trans = ' '.join(trans_str.split('::')[:-1])
+    trans_value = float(trans_str.split('::')[-1])
+    if return_dict == True:
+        return {trans: trans_value}
+    else:
+        return trans, trans_value
+
 def get_transformed_image_name(data_store):
-    return 'T('+data_store.get_transform_image_name()+')'
+    return 'T('+data_store.get_image_to_transform_name()+')'
 
 def get_image_pair_name(data_store):
     return str((data_store.get_reference_image_name(), get_transformed_image_name(data_store)))
 
 
 '''
 matplotlib widget utils
 '''
 if not HEADLESS:
     # Get a matplotlib canvas as a Qt Widget
     class MplCanvas(FigureCanvasQTAgg):
-        def __init__(self, parent=None, width=5, height=3, dpi=100, polar=False):
-            self.figure = Figure(figsize=(width, height), dpi=dpi)
+        def __init__(self, size=(3.5, 3.5), dpi=100, polar=False):
+            self.figure = Figure(figsize=size)  # , dpi=dpi)
             self.axes = self.figure.add_subplot(111, polar=polar)
             super(MplCanvas, self).__init__(self.figure)
```

### Comparing `IQM-VIS-0.2.5.29/IQM_VIS.egg-info/SOURCES.txt` & `IQM-Vis-0.2.5.63/IQM_Vis.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,49 @@
+MANIFEST.in
 README.md
+VERSION
+requirements.txt
 setup.py
-IQM_VIS/__init__.py
-IQM_VIS/data_api.py
-IQM_VIS/ui_wrapper.py
-IQM_VIS.egg-info/PKG-INFO
-IQM_VIS.egg-info/SOURCES.txt
-IQM_VIS.egg-info/dependency_links.txt
-IQM_VIS.egg-info/requires.txt
-IQM_VIS.egg-info/top_level.txt
-IQM_VIS/UI/__init__.py
-IQM_VIS/UI/images.py
-IQM_VIS/UI/layout.py
-IQM_VIS/UI/main.py
-IQM_VIS/UI/style.py
-IQM_VIS/UI/widgets.py
-IQM_VIS/examples/__init__.py
-IQM_VIS/examples/dataset.py
-IQM_VIS/examples/multiple.py
-IQM_VIS/examples/simple.py
-IQM_VIS/image_metrics/__init__.py
-IQM_VIS/image_metrics/metrics.py
-IQM_VIS/image_metrics/expert/__init__.py
-IQM_VIS/image_metrics/expert/pyramids.py
-IQM_VIS/image_metrics/expert/layers/__init__.py
-IQM_VIS/image_metrics/expert/layers/divisive_normalisation.py
-IQM_VIS/image_metrics/expert/utils/__init__.py
-IQM_VIS/image_metrics/expert/utils/conv.py
-IQM_VIS/image_metrics/expert/utils/fourier.py
-IQM_VIS/image_metrics/expert/utils/pyramid_filters.py
-IQM_VIS/transformations/__init__.py
-IQM_VIS/transformations/transforms.py
-IQM_VIS/utils/__init__.py
-IQM_VIS/utils/gui_utils.py
-IQM_VIS/utils/image_utils.py
-IQM_VIS/utils/plot_utils.py
+IQM_Vis/__init__.py
+IQM_Vis/ui_wrapper.py
+IQM_Vis.egg-info/PKG-INFO
+IQM_Vis.egg-info/SOURCES.txt
+IQM_Vis.egg-info/dependency_links.txt
+IQM_Vis.egg-info/requires.txt
+IQM_Vis.egg-info/top_level.txt
+IQM_Vis/UI/__init__.py
+IQM_Vis/UI/custom_widgets.py
+IQM_Vis/UI/experiment_mode.py
+IQM_Vis/UI/images.py
+IQM_Vis/UI/layout.py
+IQM_Vis/UI/main.py
+IQM_Vis/UI/style-dark.css
+IQM_Vis/UI/style-light.css
+IQM_Vis/UI/threads.py
+IQM_Vis/UI/utils.py
+IQM_Vis/UI/widgets.py
+IQM_Vis/data_handlers/__init__.py
+IQM_Vis/data_handlers/data_api.py
+IQM_Vis/data_handlers/data_api_abstract.py
+IQM_Vis/examples/__init__.py
+IQM_Vis/examples/all.py
+IQM_Vis/examples/dataset.py
+IQM_Vis/examples/dists.py
+IQM_Vis/examples/experiment.py
+IQM_Vis/examples/multiple.py
+IQM_Vis/examples/simple.py
+IQM_Vis/examples/images/HIQM.csv
+IQM_Vis/examples/images/__init__.py
+IQM_Vis/examples/images/waves1.jpeg
+IQM_Vis/examples/images/waves2.jpeg
+IQM_Vis/examples/images/waves3.jpeg
+IQM_Vis/metrics/IQMs.py
+IQM_Vis/metrics/__init__.py
+IQM_Vis/transformations/__init__.py
+IQM_Vis/transformations/transforms.py
+IQM_Vis/utils/__init__.py
+IQM_Vis/utils/gui_utils.py
+IQM_Vis/utils/image_utils.py
+IQM_Vis/utils/plot_utils.py
+IQM_Vis/utils/save_utils.py
 tests/__init__.py
 tests/test_inputs.py
```

### Comparing `IQM-VIS-0.2.5.29/setup.py` & `IQM-Vis-0.2.5.63/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,25 +3,36 @@
 
 
 def get_long_description():
     with open('README.md', encoding="utf-8") as f:
         text = f.read()
     return text
 
+def get_version():
+    with open('VERSION') as f:
+        ver = f.read()
+    while ver[-1] == '\n':
+        ver = ver[:-1]
+    return ver
 
-setup(name='IQM-VIS',
-      version='0.2.5.29',
+def dependencies_from_file(file_path):
+    required = []
+    with open(file_path) as f:
+        for l in f.readlines():
+            l_c = l.strip()
+            # get not empty lines and ones that do not start with python
+            # comment "#" (preceded by any number of white spaces)
+            if l_c and not l_c.startswith('#'):
+                required.append(l_c)
+    return required
+
+setup(name='IQM-Vis',
+      version=get_version(),
       packages=find_packages(),
-      install_requires=['numpy',
-                        'opencv-python',
-                        'scikit-image',
-                        'PyQt6',
-                        'matplotlib',
-                        'torch',
-                        'torchmetrics'],
-      # data_files=[('/', ['IQM_VIS/UI/style.css'])], # include non .py files needed
+      include_package_data=True,
+      install_requires=dependencies_from_file('./requirements.txt'),
       author="Matt Clifford",
       author_email="matt.clifford@bristol.ac.uk",
       description="Extendable user interface for the assessment of transformations on image metrics.",
       long_description=get_long_description(),
       long_description_content_type='text/markdown',
       )
```

### Comparing `IQM-VIS-0.2.5.29/tests/test_inputs.py` & `IQM-Vis-0.2.5.63/tests/test_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 test invalid input to api throws an error
 '''
 # Author: Matt Clifford <matt.clifford@bristol.ac.uk>
 import pytest
 import numpy as np
 
-from IQM_VIS import api
+from IQM_Vis import api
 
 def test_not_dict():
     with pytest.raises(TypeError) as val_error:
         api.make_UI([],
                 {'a':1},
                 {'a':1},
                 {'a':1},
```

