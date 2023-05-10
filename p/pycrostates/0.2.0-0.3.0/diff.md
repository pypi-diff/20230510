# Comparing `tmp/pycrostates-0.2.0.tar.gz` & `tmp/pycrostates-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrostates-0.2.0.tar", last modified: Fri Sep 30 15:27:29 2022, max compression
+gzip compressed data, was "pycrostates-0.3.0.tar", last modified: Wed May 10 11:28:27 2023, max compression
```

## Comparing `pycrostates-0.2.0.tar` & `pycrostates-0.3.0.tar`

### file list

```diff
@@ -1,68 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.671565 pycrostates-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-09-30 15:26:46.000000 pycrostates-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10292 2022-09-30 15:27:29.671565 pycrostates-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7141 2022-09-30 15:26:46.000000 pycrostates-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.663565 pycrostates-0.2.0/pycrostates/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.663565 pycrostates-0.2.0/pycrostates/cluster/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    43430 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/cluster/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14054 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/cluster/kmeans.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.663565 pycrostates-0.2.0/pycrostates/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.663565 pycrostates-0.2.0/pycrostates/datasets/lemon/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/datasets/lemon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.667565 pycrostates-0.2.0/pycrostates/datasets/lemon/data/
--rw-r--r--   0 runner    (1001) docker     (121)    67396 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/datasets/lemon/data/PREPROCESSED_LEMON_registry.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/datasets/lemon/lemon.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.667565 pycrostates-0.2.0/pycrostates/html_templates/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/html_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/html_templates/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.667565 pycrostates-0.2.0/pycrostates/html_templates/repr/
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/html_templates/repr/BaseCluster.html.jinja
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/html_templates/repr/BaseSegmentation.html.jinja
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/html_templates/repr/ChData.html.jinja
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/html_templates/repr/ModKMeans.html.jinja
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.667565 pycrostates-0.2.0/pycrostates/io/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4518 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/io/ch_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    18892 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/io/fiff.py
--rw-r--r--   0 runner    (1001) docker     (121)    19084 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/io/meas_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/io/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.667565 pycrostates-0.2.0/pycrostates/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/metrics/calinski_harabasz.py
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/metrics/davies_bouldin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/metrics/dunn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/metrics/silhouette.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.667565 pycrostates-0.2.0/pycrostates/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5854 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/preprocessing/extract_gfp_peaks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6427 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/preprocessing/resample.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.667565 pycrostates-0.2.0/pycrostates/segmentation/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16735 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/segmentation/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.671565 pycrostates-0.2.0/pycrostates/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9180 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/utils/_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/utils/_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6501 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/utils/_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/utils/_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     7239 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/utils/_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3515 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/utils/mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5360 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.671565 pycrostates-0.2.0/pycrostates/viz/
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/viz/cluster_centers.py
--rw-r--r--   0 runner    (1001) docker     (121)     7976 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pycrostates/viz/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-30 15:27:29.663565 pycrostates-0.2.0/pycrostates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10292 2022-09-30 15:27:29.000000 pycrostates-0.2.0/pycrostates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-09-30 15:27:29.000000 pycrostates-0.2.0/pycrostates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-30 15:27:29.000000 pycrostates-0.2.0/pycrostates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-30 15:27:29.000000 pycrostates-0.2.0/pycrostates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-30 15:27:29.000000 pycrostates-0.2.0/pycrostates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-09-30 15:26:46.000000 pycrostates-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-30 15:27:29.671565 pycrostates-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-30 15:26:46.000000 pycrostates-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.480520 pycrostates-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-10 11:27:50.000000 pycrostates-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-10 11:28:27.476520 pycrostates-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-10 11:27:50.000000 pycrostates-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.472520 pycrostates-0.3.0/pycrostates/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.472520 pycrostates-0.3.0/pycrostates/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44509 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/cluster/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/cluster/aahc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/cluster/kmeans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.472520 pycrostates-0.3.0/pycrostates/cluster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/cluster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/cluster/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.472520 pycrostates-0.3.0/pycrostates/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.472520 pycrostates-0.3.0/pycrostates/datasets/lemon/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/datasets/lemon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.472520 pycrostates-0.3.0/pycrostates/datasets/lemon/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    67396 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/datasets/lemon/data/PREPROCESSED_LEMON_registry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/datasets/lemon/lemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.472520 pycrostates-0.3.0/pycrostates/html_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/html_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/html_templates/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.476520 pycrostates-0.3.0/pycrostates/html_templates/repr/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/html_templates/repr/AAHCluster.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/html_templates/repr/BaseCluster.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/html_templates/repr/BaseSegmentation.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/html_templates/repr/ChData.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/html_templates/repr/ModKMeans.html.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.476520 pycrostates-0.3.0/pycrostates/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/io/ch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/io/fiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/io/meas_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/io/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.476520 pycrostates-0.3.0/pycrostates/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/metrics/calinski_harabasz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/metrics/davies_bouldin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/metrics/dunn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/metrics/silhouette.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.476520 pycrostates-0.3.0/pycrostates/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/preprocessing/extract_gfp_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/preprocessing/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/preprocessing/spatial_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.476520 pycrostates-0.3.0/pycrostates/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/segmentation/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/segmentation/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/segmentation/transitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.476520 pycrostates-0.3.0/pycrostates/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.476520 pycrostates-0.3.0/pycrostates/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/viz/cluster_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pycrostates/viz/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:28:27.472520 pycrostates-0.3.0/pycrostates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-10 11:28:27.000000 pycrostates-0.3.0/pycrostates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-10 11:28:27.000000 pycrostates-0.3.0/pycrostates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:28:27.000000 pycrostates-0.3.0/pycrostates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-10 11:28:27.000000 pycrostates-0.3.0/pycrostates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 11:28:27.000000 pycrostates-0.3.0/pycrostates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-10 11:27:50.000000 pycrostates-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:28:27.480520 pycrostates-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:27:50.000000 pycrostates-0.3.0/setup.py
```

### Comparing `pycrostates-0.2.0/LICENSE` & `pycrostates-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/PKG-INFO` & `pycrostates-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrostates
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple open source Python package for EEG microstate segmentation.
 Author-email: Victor Férat <victor.ferat@unige.ch>
 Maintainer-email: Victor Férat <victor.ferat@unige.ch>, Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Victor Férat
         All rights reserved.
@@ -39,23 +39,24 @@
 Project-URL: source, https://github.com/vferat/pycrostates
 Project-URL: tracker, https://github.com/vferat/pycrostates/issues
 Keywords: python,neuroscience,neuroimaging,eeg,microstates,brain
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
@@ -63,14 +64,15 @@
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![PyPI version](https://badge.fury.io/py/pycrostates.svg)](https://badge.fury.io/py/pycrostates)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycrostates.svg)](https://anaconda.org/conda-forge/pycrostates)
 [![Documentation Status](https://readthedocs.org/projects/pycrostates/badge/?version=latest)](https://pycrostates.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://dev.azure.com/vferat/pycrostates/_apis/build/status/vferat.pycrostates?branchName=main)](https://dev.azure.com/vferat/pycrostates/_build/latest?definitionId=1&branchName=main)
 [![codecov](https://codecov.io/gh/vferat/pycrostates/branch/master/graph/badge.svg?token=47COGGCGX8)](https://codecov.io/gh/vferat/pycrostates)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/029e425f90614943b0a944e03922b637)](https://www.codacy.com/gh/vferat/pycrostates/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vferat/pycrostates&amp;utm_campaign=Badge_Grade)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04564/status.svg)](https://doi.org/10.21105/joss.04564)
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_white.png">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_black.png">
   <img alt="Pycrostate logo" src="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_black.png">
 </picture>
 
@@ -88,26 +90,26 @@
 ## Installation
 [![Downloads](https://pepy.tech/badge/pycrostates/month)](https://pepy.tech/project/pycrostates)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pycrostates/badges/downloads.svg)](https://anaconda.org/conda-forge/pycrostates)
 
 Installation instructions can be found [here](https://pycrostates.readthedocs.io/en/latest/install.html).
 
 ## Citing
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6915329.svg)](https://doi.org/10.5281/zenodo.6915329)
-[![status](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3/status.svg)](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04564/status.svg)](https://doi.org/10.21105/joss.04564)
 
-To cite specific version numbers of the software, you can use the DOIs provided by [Zenodo](https://doi.org/10.5281/zenodo.6915329).
-The canonical journal article reference is currently under review at the [JOSS](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3) journal and can't be cited yet.
+The associated paper can be retrieved here: https://joss.theoj.org/papers/10.21105/joss.04564
+To cite specific version numbers of the software, you can use the DOIs provided
+by [Zenodo](https://zenodo.org/record/7129852).
 
 ## Contributing
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Pycrostates welcomes contributions from anyone interested in improving this project. These contributions can take the form of bug reports/fixes, feature requests/additions, documentation revision and new tutorials.
 
 In all cases, it is recommended to [open a new issue](https://github.com/vferat/pycrostates/issues/new/choose) on Github to discuss the best way to integrate a contribution.
 
 Check the [Contribution Guide](https://github.com/vferat/pycrostates/blob/main/CONTRIBUTING.md) if you want to make a changes to Pycrostates.
@@ -116,19 +118,22 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://vferat.github.io/about/"><img src="https://avatars.githubusercontent.com/u/28844486?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Victor Férat</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Tests">⚠️</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Documentation">📖</a> <a href="#ideas-vferat" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-vferat" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-vferat" title="Maintenance">🚧</a> <a href="#projectManagement-vferat" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Avferat" title="Reviewed Pull Requests">👀</a></td>
-    <td align="center"><a href="https://github.com/mscheltienne"><img src="https://avatars.githubusercontent.com/u/73893616?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mathieu Scheltienne</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Documentation">📖</a> <a href="#ideas-mscheltienne" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-mscheltienne" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-mscheltienne" title="Maintenance">🚧</a> <a href="#projectManagement-mscheltienne" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Amscheltienne" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://github.com/LouPlanchamp"><img src="https://avatars.githubusercontent.com/u/107875645?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Lou</b></sub></a><br /><a href="#design-LouPlanchamp" title="Design">🎨</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center"><a href="https://vferat.github.io/about/"><img src="https://avatars.githubusercontent.com/u/28844486?v=4?s=100" width="100px;" alt="Victor Férat"/><br /><sub><b>Victor Férat</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Tests">⚠️</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Documentation">📖</a> <a href="#ideas-vferat" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-vferat" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-vferat" title="Maintenance">🚧</a> <a href="#projectManagement-vferat" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Avferat" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center"><a href="https://github.com/mscheltienne"><img src="https://avatars.githubusercontent.com/u/73893616?v=4?s=100" width="100px;" alt="Mathieu Scheltienne"/><br /><sub><b>Mathieu Scheltienne</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Documentation">📖</a> <a href="#ideas-mscheltienne" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-mscheltienne" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-mscheltienne" title="Maintenance">🚧</a> <a href="#projectManagement-mscheltienne" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Amscheltienne" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Tests">⚠️</a></td>
+      <td align="center"><a href="https://github.com/LouPlanchamp"><img src="https://avatars.githubusercontent.com/u/107875645?v=4?s=100" width="100px;" alt="Lou"/><br /><sub><b>Lou</b></sub></a><br /><a href="#design-LouPlanchamp" title="Design">🎨</a></td>
+      <td align="center"><a href="https://github.com/rkobler"><img src="https://avatars.githubusercontent.com/u/22491497?v=4?s=100" width="100px;" alt="rkobler"/><br /><sub><b>rkobler</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Documentation">📖</a> <a href="#ideas-rkobler" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Tests">⚠️</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `pycrostates-0.2.0/README.md` & `pycrostates-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![PyPI version](https://badge.fury.io/py/pycrostates.svg)](https://badge.fury.io/py/pycrostates)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycrostates.svg)](https://anaconda.org/conda-forge/pycrostates)
 [![Documentation Status](https://readthedocs.org/projects/pycrostates/badge/?version=latest)](https://pycrostates.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://dev.azure.com/vferat/pycrostates/_apis/build/status/vferat.pycrostates?branchName=main)](https://dev.azure.com/vferat/pycrostates/_build/latest?definitionId=1&branchName=main)
 [![codecov](https://codecov.io/gh/vferat/pycrostates/branch/master/graph/badge.svg?token=47COGGCGX8)](https://codecov.io/gh/vferat/pycrostates)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/029e425f90614943b0a944e03922b637)](https://www.codacy.com/gh/vferat/pycrostates/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vferat/pycrostates&amp;utm_campaign=Badge_Grade)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04564/status.svg)](https://doi.org/10.21105/joss.04564)
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_white.png">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_black.png">
   <img alt="Pycrostate logo" src="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_black.png">
 </picture>
 
@@ -26,26 +27,26 @@
 ## Installation
 [![Downloads](https://pepy.tech/badge/pycrostates/month)](https://pepy.tech/project/pycrostates)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pycrostates/badges/downloads.svg)](https://anaconda.org/conda-forge/pycrostates)
 
 Installation instructions can be found [here](https://pycrostates.readthedocs.io/en/latest/install.html).
 
 ## Citing
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6915329.svg)](https://doi.org/10.5281/zenodo.6915329)
-[![status](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3/status.svg)](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04564/status.svg)](https://doi.org/10.21105/joss.04564)
 
-To cite specific version numbers of the software, you can use the DOIs provided by [Zenodo](https://doi.org/10.5281/zenodo.6915329).
-The canonical journal article reference is currently under review at the [JOSS](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3) journal and can't be cited yet.
+The associated paper can be retrieved here: https://joss.theoj.org/papers/10.21105/joss.04564
+To cite specific version numbers of the software, you can use the DOIs provided
+by [Zenodo](https://zenodo.org/record/7129852).
 
 ## Contributing
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Pycrostates welcomes contributions from anyone interested in improving this project. These contributions can take the form of bug reports/fixes, feature requests/additions, documentation revision and new tutorials.
 
 In all cases, it is recommended to [open a new issue](https://github.com/vferat/pycrostates/issues/new/choose) on Github to discuss the best way to integrate a contribution.
 
 Check the [Contribution Guide](https://github.com/vferat/pycrostates/blob/main/CONTRIBUTING.md) if you want to make a changes to Pycrostates.
@@ -54,19 +55,22 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://vferat.github.io/about/"><img src="https://avatars.githubusercontent.com/u/28844486?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Victor Férat</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Tests">⚠️</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Documentation">📖</a> <a href="#ideas-vferat" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-vferat" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-vferat" title="Maintenance">🚧</a> <a href="#projectManagement-vferat" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Avferat" title="Reviewed Pull Requests">👀</a></td>
-    <td align="center"><a href="https://github.com/mscheltienne"><img src="https://avatars.githubusercontent.com/u/73893616?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mathieu Scheltienne</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Documentation">📖</a> <a href="#ideas-mscheltienne" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-mscheltienne" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-mscheltienne" title="Maintenance">🚧</a> <a href="#projectManagement-mscheltienne" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Amscheltienne" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://github.com/LouPlanchamp"><img src="https://avatars.githubusercontent.com/u/107875645?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Lou</b></sub></a><br /><a href="#design-LouPlanchamp" title="Design">🎨</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center"><a href="https://vferat.github.io/about/"><img src="https://avatars.githubusercontent.com/u/28844486?v=4?s=100" width="100px;" alt="Victor Férat"/><br /><sub><b>Victor Férat</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Tests">⚠️</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Documentation">📖</a> <a href="#ideas-vferat" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-vferat" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-vferat" title="Maintenance">🚧</a> <a href="#projectManagement-vferat" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Avferat" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center"><a href="https://github.com/mscheltienne"><img src="https://avatars.githubusercontent.com/u/73893616?v=4?s=100" width="100px;" alt="Mathieu Scheltienne"/><br /><sub><b>Mathieu Scheltienne</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Documentation">📖</a> <a href="#ideas-mscheltienne" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-mscheltienne" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-mscheltienne" title="Maintenance">🚧</a> <a href="#projectManagement-mscheltienne" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Amscheltienne" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Tests">⚠️</a></td>
+      <td align="center"><a href="https://github.com/LouPlanchamp"><img src="https://avatars.githubusercontent.com/u/107875645?v=4?s=100" width="100px;" alt="Lou"/><br /><sub><b>Lou</b></sub></a><br /><a href="#design-LouPlanchamp" title="Design">🎨</a></td>
+      <td align="center"><a href="https://github.com/rkobler"><img src="https://avatars.githubusercontent.com/u/22491497?v=4?s=100" width="100px;" alt="rkobler"/><br /><sub><b>rkobler</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Documentation">📖</a> <a href="#ideas-rkobler" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Tests">⚠️</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `pycrostates-0.2.0/pycrostates/_typing.py` & `pycrostates-0.3.0/pycrostates/_typing.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,9 +19,15 @@
 
 class CHInfo(ABC):
     """Typing for CHInfo."""
 
     pass
 
 
+class Cluster(ABC):
+    """Typing for a clustering class."""
+
+    pass
+
+
 RANDomState = Optional[Union[int, RandomState, Generator]]
 Picks = Optional[Union[str, NDArray[int]]]
```

### Comparing `pycrostates-0.2.0/pycrostates/cluster/_base.py` & `pycrostates-0.3.0/pycrostates/cluster/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-from abc import ABC, abstractmethod
+from abc import abstractmethod
 from copy import copy, deepcopy
 from itertools import groupby
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from matplotlib.axes import Axes
 from mne import BaseEpochs, pick_info
 from mne.annotations import _annotations_starts_stops
 from mne.io import BaseRaw
 from mne.io.pick import _picks_to_idx
 from numpy.typing import NDArray
 from scipy.signal import convolve2d
 
-from .._typing import CHData, Picks
+from .._typing import CHData, Cluster, Picks
 from ..segmentation import EpochsSegmentation, RawSegmentation
 from ..utils import _corr_vectors
 from ..utils._checks import (
-    _check_n_jobs,
     _check_picks_uniqueness,
     _check_reject_by_annotation,
     _check_tmin_tmax,
     _check_type,
     _check_value,
 )
 from ..utils._docs import fill_doc
 from ..utils._logs import logger, verbose
 from ..utils.mixin import ChannelsMixin, ContainsMixin, MontageMixin
 from ..viz import plot_cluster_centers
+from .utils import optimize_order
 
 
-class _BaseCluster(ABC, ChannelsMixin, ContainsMixin, MontageMixin):
+class _BaseCluster(Cluster, ChannelsMixin, ContainsMixin, MontageMixin):
     """Base Class for Microstates Clustering algorithms."""
 
     @abstractmethod
     def __init__(self):
         self._n_clusters = None
         self._cluster_names = None
         self._cluster_centers_ = None
+        self._ignore_polarity = None
 
         # fit variables
         self._info = None
         self._fitted_data = None
         self._labels_ = None
         self._fitted = False
 
@@ -181,22 +182,24 @@
         assert self._cluster_centers_ is None
         assert self._info is None
         assert self._fitted_data is None
         assert self._labels_ is None
 
     @abstractmethod
     @fill_doc
+    @verbose
     def fit(
         self,
         inst: Union[BaseRaw, BaseEpochs, CHData],
         picks: Picks = "eeg",
         tmin: Optional[Union[int, float]] = None,
         tmax: Optional[Union[int, float]] = None,
         reject_by_annotation: bool = True,
-        n_jobs: int = 1,
+        *,
+        verbose: Optional[str] = None,
     ) -> NDArray[float]:
         """Compute cluster centers.
 
         Parameters
         ----------
         inst : Raw | Epochs | ChData
             MNE `~mne.io.Raw`, `~mne.Epochs` or `~pycrostates.io.ChData` object
@@ -209,20 +212,19 @@
             string values “all” to pick all channels, or “data” to pick data
             channels. ``"eeg"`` (default) will pick all eeg channels.
             Note that channels in ``info['bads']`` will be included if their
             names or indices are explicitly provided.
         %(tmin_raw)s
         %(tmax_raw)s
         %(reject_by_annotation_raw)s
-        %(n_jobs)s
+        %(verbose)s
         """
         from ..io import ChData, ChInfo
 
         self._check_unfitted()
-        n_jobs = _check_n_jobs(n_jobs)
         _check_type(inst, (BaseRaw, BaseEpochs, ChData), item_name="inst")
         if isinstance(inst, (BaseRaw, BaseEpochs)):
             tmin, tmax = _check_tmin_tmax(inst, tmin, tmax)
         if isinstance(inst, BaseRaw):
             reject_by_annotation = _check_reject_by_annotation(
                 reject_by_annotation
             )
@@ -359,37 +361,57 @@
         order: Optional[
             Union[
                 List[int],
                 Tuple[int, ...],
                 NDArray[int],
             ]
         ] = None,
+        template: Optional[Cluster] = None,
     ) -> None:
-        """Reorder the clusters.
+        """
+        Reorder the clusters of the fitted model.
+
+        Specify one of the following arguments to change the current order:
+
+        * ``mapping``: a dictionary that maps old cluster positions
+          to new positions,
+        * ``order``: a 1D iterable containing the new order,
+        * ``template``: a fitted clustering algorithm used as a reference
+           to match the order.
+
+        Only one argument can be set at a time.
 
         Parameters
         ----------
         mapping : dict
             Mapping from the old order to the new order.
             key: old position, value: new position.
         order : list of int | tuple of int | array of int
             1D iterable containing the new order.
+            Positions are 0-indexed.
+        template : :ref:`cluster`
+            Fitted clustering algorithm use as template for
+            ordering optimization. For more details about the
+            current implementation, check the
+            :func:`pycrostates.cluster.utils.optimize_order`
+            documentation.
 
         Notes
         -----
-        The positions are 0-indexed.
         Operates in-place.
         """
         self._check_fit()
 
-        if mapping is not None and order is not None:
+        if sum(x is not None for x in (mapping, order, template)) > 1:
             raise ValueError(
-                "Only one of 'mapping' or 'order' must be provided."
+                "Only one of 'mapping', 'order' or 'template' "
+                "must be provided."
             )
 
+        # Mapping
         if mapping is not None:
             _check_type(mapping, (dict,), item_name="mapping")
             valids = tuple(range(self._n_clusters))
             for key in mapping:
                 _check_value(key, valids, item_name="old position")
             for value in mapping.values():
                 _check_value(value, valids, item_name="new position")
@@ -415,14 +437,15 @@
             order = list(range(self._n_clusters))
             for key, value in mapping.items():
                 order[key] = value
                 order[value] = key
             # sanity-check
             assert len(set(order)) == self._n_clusters
 
+        # Order
         elif order is not None:
             _check_type(order, (list, tuple, np.ndarray), item_name="order")
             if isinstance(order, np.ndarray) and len(order.shape) != 1:
                 raise ValueError(
                     "Argument 'order' should be a 1D iterable and not a "
                     f"{len(order.shape)}D iterable."
                 )
@@ -432,17 +455,21 @@
             if len(order) != self._n_clusters:
                 raise ValueError(
                     "Argument 'order' should contain 'n_clusters': "
                     f"{self._n_clusters} elements. Provided '{len(order)}'."
                 )
             order = list(order)
 
+        # Cluster
+        elif template is not None:
+            order = optimize_order(self, template)
+
         else:
             logger.warning(
-                "Either 'mapping' or 'order' should not be 'None' "
+                "Either 'mapping', 'order' or 'template' should not be 'None' "
                 "for method 'reorder_clusters' to operate."
             )
             return
 
         # re-order
         self._cluster_centers_ = self._cluster_centers_[order]
         self._cluster_names = [self._cluster_names[k] for k in order]
@@ -507,15 +534,19 @@
         # Invert maps
         for k, cluster in enumerate(self._cluster_centers_):
             if invert[k]:
                 self._cluster_centers_[k] = -cluster
 
     @fill_doc
     def plot(
-        self, axes: Optional[Axes] = None, *, block: bool = False, **kwargs
+        self,
+        axes: Optional[Union[Axes, NDArray[Axes]]] = None,
+        *,
+        block: bool = False,
+        **kwargs,
     ):
         """
         Plot cluster centers as topographic maps.
 
         Parameters
         ----------
         %(axes_topo)s
@@ -550,14 +581,15 @@
         ----------
         fname : path-like
             Path to the ``.fif`` file where the clustering solution is saved.
         """
         self._check_fit()
         _check_type(fname, ("path-like",), "fname")
 
+    @fill_doc
     @verbose
     def predict(
         self,
         inst: Union[BaseRaw, BaseEpochs],
         picks: Picks = None,
         factor: int = 0,
         half_window_size: int = 1,
@@ -760,15 +792,15 @@
 
         # logging messages
         if factor == 0:
             logger.info("Segmenting data without smoothing.")
         else:
             logger.info(
                 "Segmenting data with factor %s and effective smoothing "
-                "window size: %.4f (ms).",
+                "window size: %.4f (s).",
                 factor,
                 (2 * half_window_size + 1) / inst.info["sfreq"],
             )
         if min_segment_length > 0:
             logger.info(
                 "Rejecting segments shorter than %.4f (ms).",
                 min_segment_length / inst.info["sfreq"],
```

### Comparing `pycrostates-0.2.0/pycrostates/cluster/kmeans.py` & `pycrostates-0.3.0/pycrostates/cluster/kmeans.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import numpy as np
 from mne import BaseEpochs
 from mne.io import BaseRaw
 from mne.parallel import parallel_func
 from numpy.random import Generator, RandomState
 from numpy.typing import NDArray
 
-from .._typing import Picks, RANDomState
+from .._typing import CHData, Picks, RANDomState
 from ..utils import _corr_vectors
-from ..utils._checks import _check_random_state, _check_type
+from ..utils._checks import _check_n_jobs, _check_random_state, _check_type
 from ..utils._docs import copy_doc, fill_doc
-from ..utils._logs import _set_verbose, logger
+from ..utils._logs import logger
 from ._base import _BaseCluster
 
 
 @fill_doc
 class ModKMeans(_BaseCluster):
     r"""Modified K-Means clustering algorithm.
 
@@ -77,15 +77,15 @@
             ch_types, ch_counts = np.unique(
                 self.get_channel_types(), return_counts=True
             )
             ch_repr = [
                 f"{ch_count} {ch_type.upper()}"
                 for ch_type, ch_count in zip(ch_types, ch_counts)
             ]
-            GEV = int(self._GEV_ * 100)
+            GEV = f"{self._GEV_ * 100:.2f}"
         else:
             n_samples = None
             ch_repr = None
             GEV = None
 
         return template.render(
             name=self.__class__.__name__,
@@ -96,15 +96,14 @@
             fitted=self._fitted,
             n_samples=n_samples,
             ch_repr=ch_repr,
         )
 
     @copy_doc(_BaseCluster.__eq__)
     def __eq__(self, other: Any) -> bool:
-        """Equality == method."""
         if isinstance(other, ModKMeans):
             if not super().__eq__(other):
                 return False
 
             attributes = (
                 "_n_init",
                 "_max_iter",
@@ -123,42 +122,64 @@
                     return False
 
             return True
         return False
 
     @copy_doc(_BaseCluster.__ne__)
     def __ne__(self, other: Any) -> bool:
-        """Different != method."""
         return not self.__eq__(other)
 
     @copy_doc(_BaseCluster._check_fit)
     def _check_fit(self):
         super()._check_fit()
         # sanity-check
         assert self.GEV_ is not None
 
-    @copy_doc(_BaseCluster.fit)
     @fill_doc
     def fit(
         self,
-        inst: Union[BaseRaw, BaseEpochs],
+        inst: Union[BaseRaw, BaseEpochs, CHData],
         picks: Picks = "eeg",
         tmin: Optional[Union[int, float]] = None,
         tmax: Optional[Union[int, float]] = None,
         reject_by_annotation: bool = True,
         n_jobs: int = 1,
         *,
         verbose: Optional[str] = None,
     ) -> None:
-        """
+        """Compute cluster centers.
+
+        Parameters
+        ----------
+        inst : Raw | Epochs | ChData
+            MNE `~mne.io.Raw`, `~mne.Epochs` or `~pycrostates.io.ChData` object
+            from which to extract :term:`cluster centers`.
+        picks : str | list | slice | None
+            Channels to include. Note that all channels selected must have the
+            same type. Slices and lists of integers will be interpreted as
+            channel indices. In lists, channel name strings (e.g.
+            ``['Fp1', 'Fp2']``) will pick the given channels. Can also be the
+            string values “all” to pick all channels, or “data” to pick data
+            channels. ``"eeg"`` (default) will pick all eeg channels.
+            Note that channels in ``info['bads']`` will be included if their
+            names or indices are explicitly provided.
+        %(tmin_raw)s
+        %(tmax_raw)s
+        %(reject_by_annotation_raw)s
+        %(n_jobs)s
         %(verbose)s
         """
-        _set_verbose(verbose)  # TODO: decorator nesting is failing
+        n_jobs = _check_n_jobs(n_jobs)
         data = super().fit(
-            inst, picks, tmin, tmax, reject_by_annotation, n_jobs
+            inst,
+            picks=picks,
+            tmin=tmin,
+            tmax=tmax,
+            reject_by_annotation=reject_by_annotation,
+            verbose=verbose,
         )
 
         inits = self._random_state.randint(
             low=0, high=100 * self._n_init, size=(self._n_init)
         )
 
         if n_jobs == 1:
@@ -211,14 +232,15 @@
             self.fitted = False  # reset variables related to fit
             return  # break early
 
         self._GEV_ = best_gev
         self._cluster_centers_ = best_maps
         self._labels_ = best_segmentation
         self._fitted = True
+        self._ignore_polarity = True
 
     @copy_doc(_BaseCluster.save)
     def save(self, fname: Union[str, Path]):
         super().save(fname)
         # TODO: to be replaced by a general writer than infers the writer from
         # the file extension.
         from ..io.fiff import _write_cluster  # pylint: disable=C0415
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycrostates-0.2.0/pycrostates/datasets/lemon/data/PREPROCESSED_LEMON_registry.txt` & `pycrostates-0.3.0/pycrostates/datasets/lemon/data/PREPROCESSED_LEMON_registry.txt`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/datasets/lemon/lemon.py` & `pycrostates-0.3.0/pycrostates/datasets/lemon/lemon.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/html_templates/repr/BaseCluster.html.jinja` & `pycrostates-0.3.0/pycrostates/html_templates/repr/BaseCluster.html.jinja`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/html_templates/repr/ModKMeans.html.jinja` & `pycrostates-0.3.0/pycrostates/html_templates/repr/ModKMeans.html.jinja`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/io/ch_data.py` & `pycrostates-0.3.0/pycrostates/io/ch_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -134,15 +134,49 @@
         picks = _picks_to_idx(self._info, picks, exclude=exclude)
         info = pick_info(self._info, picks, copy=False)
         data = self._data[picks, :]
         self._info = info
         self._data = data
         return self
 
+    def _get_channel_positions(self, picks=None):
+        """Get channel locations from info.
+
+        Parameters
+        ----------
+        picks : str | list | slice | None
+            None selects the good data channels.
+
+        Returns
+        -------
+        pos : array of shape (n_channels, 3)
+            Channel X/Y/Z locations.
+        """
+        picks = _picks_to_idx(self.info, picks)
+        chs = self.info["chs"]
+        pos = np.array([chs[k]["loc"][:3] for k in picks])
+        n_zero = np.sum(np.sum(np.abs(pos), axis=1) == 0)
+        if n_zero > 1:  # XXX some systems have origin (0, 0, 0)
+            raise ValueError(
+                "Could not extract channel positions for "
+                f"{n_zero} channels."
+            )
+        return pos
+
     # --------------------------------------------------------------------
     @property
     def info(self) -> CHInfo:
         """Atemporal measurement information.
 
         :type: ChInfo
         """
         return self._info
+
+    @property
+    def ch_names(self):
+        """Channel names."""
+        return self.info["ch_names"]
+
+    @property
+    def preload(self):
+        """Preload required by some MNE functions."""
+        return True
```

### Comparing `pycrostates-0.2.0/pycrostates/io/fiff.py` & `pycrostates-0.3.0/pycrostates/io/fiff.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     write_string,
 )
 from mne.transforms import Transform, invert_transform
 from numpy.typing import NDArray
 
 from .. import __version__
 from .._typing import CHInfo
-from ..cluster import ModKMeans
+from ..cluster import AAHCluster, ModKMeans
 from ..utils._checks import _check_type, _check_value
 from ..utils._docs import fill_doc
 from ..utils._logs import logger
 
 # ----------------------------------------------------------------------------
 """
 To store a clustering solution, the FIFF tags for ICA are used.
@@ -106,15 +106,15 @@
     _check_type(cluster_centers_, (np.ndarray,), "cluster_centers_")
     if cluster_centers_.ndim != 2:
         raise ValueError("Argument 'cluster_centers_' should be a 2D array.")
     _check_type(chinfo, (Info, ChInfo), "chinfo")
     if isinstance(chinfo, Info):
         chinfo = ChInfo(chinfo)  # convert to ChInfo if a MNE Info is provided
     _check_type(algorithm, (str,), "algorithm")
-    _check_value(algorithm, ("ModKMeans",), "algorithm")
+    _check_value(algorithm, ("ModKMeans", "AAHCluster"), "algorithm")
     _check_type(cluster_names, (list,), "cluster_names")
     if len(cluster_names) != cluster_centers_.shape[0]:
         raise ValueError(
             "Argument 'cluster_names' and 'cluster_centers_' shapes do not "
             "match."
         )
     _check_type(fitted_data, (np.ndarray,), "fitted_data")
@@ -174,14 +174,18 @@
 def _prepare_kwargs(algorithm: str, kwargs: dict):
     """Prepare params to save from kwargs."""
     valids = {
         "ModKMeans": {
             "parameters": ["n_init", "max_iter", "tol"],
             "variables": ["GEV_"],
         },
+        "AAHCluster": {
+            "parameters": ["ignore_polarity", "normalize_input"],
+            "variables": ["GEV_"],
+        },
     }
 
     # retrieve list of expected kwargs for this algorithm
     expected = set(reduce(operator.concat, valids[algorithm].values()))
 
     # check that we do have a value provided for each expected key
     keys = set(key for key in kwargs if kwargs[key] is not None)
@@ -198,21 +202,33 @@
     fit_parameters = dict(algorithm=algorithm, version=__version__)
     fit_variables = {}
     for key, value in kwargs.items():
         if key not in expected:
             continue
 
         # ModKMeans
-        if key == "n_init":
-            fit_parameters["n_init"] = ModKMeans._check_n_init(value)
-        elif key == "max_iter":
-            fit_parameters["max_iter"] = ModKMeans._check_max_iter(value)
-        elif key == "tol":
-            fit_parameters["tol"] = ModKMeans._check_tol(value)
-        elif key == "GEV_":
+        # pylint: disable=protected-access
+        if algorithm == "ModKMeans":
+            if key == "n_init":
+                fit_parameters["n_init"] = ModKMeans._check_n_init(value)
+            elif key == "max_iter":
+                fit_parameters["max_iter"] = ModKMeans._check_max_iter(value)
+            elif key == "tol":
+                fit_parameters["tol"] = ModKMeans._check_tol(value)
+        elif algorithm == "AAHCluster":
+            if key == "ignore_polarity":
+                fit_parameters[
+                    "ignore_polarity"
+                ] = AAHCluster._check_ignore_polarity(value)
+            elif key == "normalize_input":
+                fit_parameters[
+                    "normalize_input"
+                ] = AAHCluster._check_normalize_input(value)
+        # pylint: enable=protected-access
+        if key == "GEV_":
             _check_type(value, ("numeric",), "GEV_")
             if value < 0 or 1 < value:
                 raise ValueError(
                     "Argument 'GEV_' should be a percentage between 0 and 1. "
                     f"Provided: '{value}'."
                 )
             fit_variables["GEV_"] = value
@@ -306,15 +322,18 @@
             "One of the required tag was not found in .fif file."
         )
     algorithm, version = _check_fit_parameters_and_variables(
         fit_parameters, fit_variables
     )
 
     # reconstruct cluster instance
-    function = {"ModKMeans": _create_ModKMeans}
+    function = {
+        "ModKMeans": _create_ModKMeans,
+        "AAHCluster": _create_AAHCluster,
+    }
 
     return (
         function[algorithm](
             cluster_centers_,
             info,
             cluster_names,
             fitted_data,
@@ -332,14 +351,18 @@
 ):
     """Check that we have all the keys we are looking for and return algo."""
     valids = {
         "ModKMeans": {
             "parameters": ["n_init", "max_iter", "tol"],
             "variables": ["GEV_"],
         },
+        "AAHCluster": {
+            "parameters": ["ignore_polarity", "normalize_input"],
+            "variables": ["GEV_"],
+        },
     }
     if "algorithm" not in fit_parameters:
         raise ValueError("Key 'algorithm' is missing from .fif file.")
     if "version" not in fit_parameters:
         raise ValueError("Key 'version' is missing from .fif file.")
     algorithm = fit_parameters["algorithm"]
     if algorithm not in valids:
@@ -375,14 +398,43 @@
     cluster._fitted_data = fitted_data
     cluster._labels_ = labels_
     cluster._GEV_ = GEV_
     cluster._fitted = True
     return cluster
 
 
+def _create_AAHCluster(
+    cluster_centers_: NDArray[float],
+    info: CHInfo,
+    cluster_names: List[str],
+    fitted_data: NDArray[float],
+    labels_: NDArray[int],
+    ignore_polarity: bool,  # pylint: disable=unused-argument
+    normalize_input: bool,
+    GEV_: float,
+):
+    """Create a AAHCluster object."""
+    cluster = AAHCluster(
+        cluster_centers_.shape[0],
+        # TODO : ignor_polarity=True for now.
+        # After _BaseCluster and Metric support ignore_polarity
+        # make the parameter an argument
+        # ignore_polarity,
+        normalize_input,
+    )
+    cluster._cluster_centers_ = cluster_centers_
+    cluster._info = info
+    cluster._cluster_names = cluster_names
+    cluster._fitted_data = fitted_data
+    cluster._labels_ = labels_
+    cluster._GEV_ = GEV_
+    cluster._fitted = True
+    return cluster
+
+
 # ----------------------------------------------------------------------------
 def _write_meas_info(fid, info: CHInfo):
     """Write measurement info into a file id (from a fif file).
 
     Parameters
     ----------
     fid : file
@@ -556,14 +608,16 @@
 # ----------------------------------------------------------------------------
 def _serialize(dict_: dict, outer_sep: str = ";", inner_sep: str = ":"):
     """Aux function."""
     s = []
     for key, value in dict_.items():
         if callable(value):
             value = value.__name__
+        elif isinstance(value, bool):
+            pass
         elif isinstance(value, Integral):
             value = int(value)
         elif isinstance(value, dict):
             # py35 json does not support numpy int64
             for subkey, subvalue in value.items():
                 if isinstance(subvalue, list):
                     if len(subvalue) > 0:
```

### Comparing `pycrostates-0.2.0/pycrostates/io/meas_info.py` & `pycrostates-0.3.0/pycrostates/io/meas_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     _check_dev_head_t,
     _unique_channel_names,
 )
 from mne.io.pick import get_channel_type_constants
 from mne.io.proj import Projection
 from mne.io.tag import _ch_coord_dict
 from mne.transforms import Transform
+from mne.utils import check_version
 
 from .._typing import CHInfo
 from ..utils._checks import _check_type, _IntLike
 from ..utils._logs import logger
 
 
 class ChInfo(CHInfo, Info):
@@ -371,15 +372,23 @@
                 return False
 
             # compare coordinate transformation
             for transform in ("ctf_head_t", "dev_ctf_t", "dev_head_t"):
                 if self[transform] != other[transform]:
                     return False
 
-            # TODO: compare compensation grades and projs
+            # compare projs, compatible with mne 1.2 and above
+            if len(self["projs"]) != len(other["projs"]):
+                return False
+            if check_version("mne", "1.2"):
+                for proj1, proj2 in zip(self["projs"], other["projs"]):
+                    if proj1 != proj2:
+                        return False
+
+            # TODO: compare compensation grades
 
             if self["bads"] != other["bads"]:
                 logger.warning("Both info do not have the same bad channels.")
 
             return True
         else:
             return False
```

### Comparing `pycrostates-0.2.0/pycrostates/io/reader.py` & `pycrostates-0.3.0/pycrostates/io/reader.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/metrics/calinski_harabasz.py` & `pycrostates-0.3.0/pycrostates/metrics/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/metrics/davies_bouldin.py` & `pycrostates-0.3.0/pycrostates/metrics/davies_bouldin.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/metrics/dunn.py` & `pycrostates-0.3.0/pycrostates/metrics/dunn.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/metrics/silhouette.py` & `pycrostates-0.3.0/pycrostates/metrics/silhouette.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/preprocessing/extract_gfp_peaks.py` & `pycrostates-0.3.0/pycrostates/preprocessing/extract_gfp_peaks.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/preprocessing/resample.py` & `pycrostates-0.3.0/pycrostates/preprocessing/resample.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/segmentation/segmentation.py` & `pycrostates-0.3.0/pycrostates/segmentation/_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from mne.io import BaseRaw
 from numpy.typing import NDArray
 
 from ..utils import _corr_vectors
 from ..utils._checks import _check_type
 from ..utils._docs import fill_doc
 from ..utils._logs import logger
-from ..viz import (
-    plot_cluster_centers,
-    plot_epoch_segmentation,
-    plot_raw_segmentation,
+from ..viz import plot_cluster_centers
+from .transitions import (
+    _compute_expected_transition_matrix,
+    _compute_transition_matrix,
 )
 
 
 @fill_doc
 class _BaseSegmentation(ABC):
     """Base class for a Microstates segmentation.
 
@@ -98,62 +98,201 @@
         return_dist : bool
             If True, return the parameters distributions.
 
         Returns
         -------
         dict : dict
             Dictionaries containing microstate parameters as key/value pairs.
-            Keys are named as follow: ``'{microstate name}_{parameter}'``.
+            Keys are named as follow: ``'{microstate name}_{parameter name}'``.
 
             Available parameters are listed below:
 
-            * mean_corr : Mean correlation
-                  Mean correlation value of each time point assigned to a
-                  given state.
-            * gev : Global explained variance
-                   Total explained variance expressed by a given state.
-                   It is the sum of global explained variance values of each
-                   time point assigned to a given state.
-            * timecov : Time coverage
-                   The proportion of time during which a given state is
-                   active. This metric is expressed in percentage (%%).
-            * meandurs : Mean duration
-                   Mean temporal duration segments assigned to a given state.
-                   This metric is expressed in seconds (s).
-            * occurrences : occurrences
-                   Mean number of segment assigned to a given state per
-                   second. This metrics is expressed in segment per second
-                   ( . / s).
-
-            If return_dist is set to ``True``, also return the following
-            distributions:
-
-            * dist_corr : Distribution of correlations
-                   Correlation values of each time point assigned to a given
-                   state.
-            * dist_gev : Distribution of global explained variances
-                   Global explained variance values of each time point
-                   assigned to a given state.
-            * dist_durs : Distribution of durations.
-                   Duration of each segments assigned to a given state.
-                   Each value is expressed in seconds (s).
+            * ``mean_corr``: Mean correlation value for each time point
+              assigned to a given state.
+            * ``gev``: Global explained variance expressed by a given state.
+              It is the sum of global explained variance values of each
+              time point assigned to a given state.
+            * ``timecov``: Time coverage, the proportion of time during which
+              a given state is active. This metric is expressed as a ratio.
+            * ``meandurs``: Mean durations of segments assigned to a given
+              state. This metric is expressed in seconds (s).
+            * ``occurrences``: Occurrences per second, the mean number of
+              segment assigned to a given state per second. This metrics is
+              expressed in segment per second.
+            * ``dist_corr`` (req. ``return_dist=True``): Distribution of
+              correlations values of each time point assigned to a given state.
+            * ``dist_gev`` (req. ``return_dist=True``): Distribution of global
+              explained variances values of each time point assigned to a given
+              state.
+            * ``dist_durs`` (req. ``return_dist=True``): Distribution of
+              durations of each segments assigned to a given state. Each value
+              is expressed in seconds (s).
+
+        Warnings
+        --------
+        When working with `~mne.Epochs`, this method will put together
+        segments of all epochs. This could lead to wrong interpretation
+        especially on state durations. To avoid this behaviour,
+        make sure to set the ``reject_edges`` parameter to ``True``
+        when creating the segmentation.
         """
-        return _BaseSegmentation._compute_microstate_parameters(
-            self._labels.copy(),
-            self._inst.get_data(),
-            self._cluster_centers_,
-            self._cluster_names,
-            self._inst.info["sfreq"],
-            norm_gfp=norm_gfp,
-            return_dist=return_dist,
+        _check_type(norm_gfp, (bool,), "norm_gfp")
+        _check_type(return_dist, (bool,), "return_dist")
+
+        # retrieve sampling frequency for convenience
+        sfreq = self._inst.info["sfreq"]
+
+        # don't copy the data/labels array, get_data, swapaxes, reshape are
+        # returning a new view of the array, which is fine since we do not
+        # modify it.
+        labels = self._labels  # same pointer, no memory overhead.
+        if isinstance(self._inst, BaseRaw):
+            data = self._inst.get_data()
+            # sanity-checks
+            assert labels.ndim == 1
+            assert data.ndim == 2
+            assert labels.size == data.shape[1]
+        elif isinstance(self._inst, BaseEpochs):
+            data = self._inst.get_data()
+            # sanity-checks
+            assert labels.ndim == 2
+            assert data.ndim == 3
+            assert labels.size == data.shape[0] * data.shape[2]
+            # create a 2D view of the data array
+            data = np.swapaxes(data, 0, 1)
+            data = data.reshape(data.shape[0], -1)
+            # create a 1D view of the labels array
+            labels = labels.reshape(-1)
+
+        gfp = np.std(data, axis=0)
+        if norm_gfp:
+            labeled = np.argwhere(labels != -1)  # ignore unlabeled segments
+            gfp /= np.linalg.norm(gfp[labeled])  # normalize
+
+        segments = [(s, list(group)) for s, group in itertools.groupby(labels)]
+
+        params = dict()
+        for s, state in enumerate(self._cluster_centers_):
+            state_name = self._cluster_names[s]
+            arg_where = np.argwhere(labels == s)
+            if len(arg_where) != 0:
+                labeled_tp = data.T[arg_where][:, 0, :].T
+                labeled_gfp = gfp[arg_where][:, 0]
+                state_array = np.array([state] * len(arg_where)).transpose()
+
+                dist_corr = _corr_vectors(state_array, labeled_tp)
+                params[f"{state_name}_mean_corr"] = np.mean(np.abs(dist_corr))
+                dist_gev = (labeled_gfp * dist_corr) ** 2 / np.sum(gfp**2)
+                params[f"{state_name}_gev"] = np.sum(dist_gev)
+
+                s_segments = np.array(
+                    [len(group) for s_, group in segments if s_ == s]
+                )
+                occurrences = (
+                    len(s_segments) / len(np.where(labels != -1)[0]) * sfreq
+                )
+                params[f"{state_name}_occurrences"] = occurrences
+
+                timecov = np.sum(s_segments) / len(np.where(labels != -1)[0])
+                params[f"{state_name}_timecov"] = timecov
+
+                dist_durs = s_segments / sfreq
+                params[f"{state_name}_meandurs"] = np.mean(dist_durs)
+
+                if return_dist:
+                    params[f"{state_name}_dist_corr"] = dist_corr
+                    params[f"{state_name}_dist_gev"] = dist_gev
+                    params[f"{state_name}_dist_durs"] = dist_durs
+
+            else:
+                params[f"{state_name}_mean_corr"] = 0.0
+                params[f"{state_name}_gev"] = 0.0
+                params[f"{state_name}_timecov"] = 0.0
+                params[f"{state_name}_meandurs"] = 0.0
+                params[f"{state_name}_occurrences"] = 0.0
+
+                if return_dist:
+                    params[f"{state_name}_dist_corr"] = np.array(
+                        [], dtype=float
+                    )
+                    params[f"{state_name}_dist_gev"] = np.array(
+                        [], dtype=float
+                    )
+                    params[f"{state_name}_dist_durs"] = np.array(
+                        [], dtype=float
+                    )
+
+        params["unlabeled"] = len(np.argwhere(labels == -1)) / len(gfp)
+        return params
+
+    def compute_transition_matrix(self, stat="probability", ignore_self=True):
+        """Compute the observed transition matrix.
+
+        Count the number of transitions from one state to another
+        and aggregate the result as statistic.
+        Transition "from" and "to" unlabeled segments ``-1`` are ignored.
+
+        Parameters
+        ----------
+        %(stat_transition)s
+        %(ignore_self)s
+
+        Returns
+        -------
+        %(transition_matrix)s
+
+        Warnings
+        --------
+        When working with `~mne.Epochs`, this method will take into account
+        transitions that occur between epochs. This could lead to wrong
+        interpretation when working with discontinuous data.
+        To avoid this behaviour, make sure to set the ``reject_edges``
+        parameter to ``True`` when predicting the segmentation.
+        """
+        return _compute_transition_matrix(
+            self._labels,
+            self._cluster_centers_.shape[0],
+            stat,
+            ignore_self,
+        )
+
+    @fill_doc
+    def compute_expected_transition_matrix(
+        self, stat="probability", ignore_self=True
+    ):
+        """Compute the expected transition matrix.
+
+        Compute the theoretical transition matrix as if time course was
+        ignored, but microstate proportions kept (i.e. shuffled segmentation).
+        This matrix can be used to quantify/correct the effect of microstate
+        time coverage on the observed transition matrix obtained with
+        the method ``compute_expected_transition_matrix``.
+        Transition "from" and "to" unlabeled segments ``-1`` are ignored.
+
+        Parameters
+        ----------
+        %(stat_expected_transitions)s
+        %(ignore_self)s
+
+        Returns
+        -------
+        %(transition_matrix)s
+        """  # noqa: E501
+        return _compute_expected_transition_matrix(
+            self._labels,
+            n_clusters=self._cluster_centers_.shape[0],
+            stat=stat,
+            ignore_self=ignore_self,
         )
 
     @fill_doc
     def plot_cluster_centers(
-        self, axes: Optional[Axes] = None, *, block: bool = False
+        self,
+        axes: Optional[Union[Axes, NDArray[Axes]]] = None,
+        block: bool = False,
     ):
         """Plot cluster centers as topographic maps.
 
         Parameters
         ----------
         %(axes_topo)s
         %(block)s
@@ -207,95 +346,20 @@
             "reject_by_annotation",
         )
         # Let the door open for custom prediction with different keys, so log
         # a warning instead of raising.
         for key in predict_parameters.keys():
             if key not in valid_keys:
                 logger.warning(
-                    f"The key '{key}' in predict_parameters is not part of "
-                    "the default set of keys supported by pycrostates."
+                    "The key '%s' in predict_parameters is not part of "
+                    "the default set of keys supported by pycrostates.",
+                    key,
                 )
         return predict_parameters
 
-    @staticmethod
-    def _compute_microstate_parameters(
-        labels: NDArray[int],
-        data: NDArray[float],
-        maps: NDArray[float],
-        maps_names: List[str],
-        sfreq: Union[int, float],
-        norm_gfp: bool = True,
-        return_dist: bool = False,
-    ):
-        """Compute microstate parameters."""
-        assert (data.ndim == 3 and labels.ndim == 2) or (
-            data.ndim == 2 and labels.ndim == 1
-        )
-        if data.ndim == 3:  # epochs
-            data = np.swapaxes(data, 0, 1)
-            data = data.reshape(data.shape[0], -1)
-            labels = labels.reshape(-1)
-
-        _check_type(norm_gfp, (bool,), "norm_gfp")
-        _check_type(return_dist, (bool,), "return_dist")
-
-        gfp = np.std(data, axis=0)
-        if norm_gfp:
-            gfp /= np.linalg.norm(gfp)
-
-        segments = [(s, list(group)) for s, group in itertools.groupby(labels)]
-
-        d = {}
-        for s, state in enumerate(maps):
-            state_name = maps_names[s]
-            arg_where = np.argwhere(labels == s)
-            if len(arg_where) != 0:
-                labeled_tp = data.T[arg_where][:, 0, :].T
-                labeled_gfp = gfp[arg_where][:, 0]
-                state_array = np.array([state] * len(arg_where)).transpose()
-
-                dist_corr = _corr_vectors(state_array, labeled_tp)
-                d[f"{state_name}_mean_corr"] = np.mean(np.abs(dist_corr))
-                dist_gev = (labeled_gfp * dist_corr) ** 2 / np.sum(gfp**2)
-                d[f"{state_name}_gev"] = np.sum(dist_gev)
-
-                s_segments = np.array(
-                    [len(group) for s_, group in segments if s_ == s]
-                )
-                occurrences = (
-                    len(s_segments) / len(np.where(labels != -1)[0]) * sfreq
-                )
-                d[f"{state_name}_occurrences"] = occurrences
-
-                timecov = np.sum(s_segments) / len(np.where(labels != -1)[0])
-                d[f"{state_name}_timecov"] = timecov
-
-                dist_durs = s_segments / sfreq
-                d[f"{state_name}_meandurs"] = np.mean(dist_durs)
-
-                if return_dist:
-                    d[f"{state_name}_dist_corr"] = dist_corr
-                    d[f"{state_name}_dist_gev"] = dist_gev
-                    d[f"{state_name}_dist_durs"] = dist_durs
-
-            else:
-                d[f"{state_name}_mean_corr"] = 0
-                d[f"{state_name}_gev"] = 0
-                d[f"{state_name}_timecov"] = 0
-                d[f"{state_name}_meandurs"] = 0
-                d[f"{state_name}_occurrences"] = 0
-
-                if return_dist:
-                    d[f"{state_name}_dist_corr"] = np.array([])
-                    d[f"{state_name}_dist_gev"] = np.array([])
-                    d[f"{state_name}_dist_durs"] = np.array([])
-
-        d["unlabeled"] = len(np.argwhere(labels == -1)) / len(gfp)
-        return d
-
     # --------------------------------------------------------------------
     @property
     def predict_parameters(self) -> dict:
         """Parameters used to predict the current segmentation.
 
         :type: `dict`
         """
@@ -327,173 +391,7 @@
     @property
     def cluster_names(self) -> List[str]:
         """Name of the cluster centers.
 
         :type: `list`
         """
         return self._cluster_names.copy()
-
-
-@fill_doc
-class RawSegmentation(_BaseSegmentation):
-    """
-    Contains the segmentation of a `~mne.io.Raw` instance.
-
-    Parameters
-    ----------
-    %(labels_raw)s
-    raw : Raw
-        `~mne.io.Raw` instance used for prediction.
-    %(cluster_centers_seg)s
-    %(cluster_names)s
-    %(predict_parameters)s
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        _check_type(self._inst, (BaseRaw,), item_name="raw")
-        if self._labels.ndim != 1:
-            raise ValueError(
-                "Argument 'labels' should be a 1D array. The provided array "
-                f"shape is {self._labels.shape} which has {self._labels.ndim} "
-                "dimensions."
-            )
-
-        if self._inst.times.size != self._labels.shape[-1]:
-            raise ValueError(
-                "Provided MNE raw and labels do not have the same number "
-                f"of samples. The 'raw' has {self._inst.times.size} samples, "
-                f"while the 'labels' has {self._labels.shape[-1]} samples."
-            )
-
-    @fill_doc
-    def plot(
-        self,
-        tmin: Optional[Union[int, float]] = None,
-        tmax: Optional[Union[int, float]] = None,
-        cmap: Optional[str] = None,
-        axes: Optional[Axes] = None,
-        cbar_axes: Optional[Axes] = None,
-        *,
-        block: bool = False,
-        verbose: Optional[str] = None,
-    ):
-        """Plot the segmentation.
-
-        Parameters
-        ----------
-        %(tmin_raw)s
-        %(tmax_raw)s
-        %(cmap)s
-        %(axes_seg)s
-        %(axes_cbar)s
-        %(block)s
-        %(verbose)s
-
-        Returns
-        -------
-        fig : Figure
-            Matplotlib figure containing the segmentation.
-        """
-        # Error checking on the input is performed in the viz function.
-        return plot_raw_segmentation(
-            labels=self._labels,
-            raw=self._inst,
-            n_clusters=self._cluster_centers_.shape[0],
-            cluster_names=self._cluster_names,
-            tmin=tmin,
-            tmax=tmax,
-            cmap=cmap,
-            axes=axes,
-            cbar_axes=cbar_axes,
-            block=block,
-            verbose=verbose,
-        )
-
-    # --------------------------------------------------------------------
-    @property
-    def raw(self) -> BaseRaw:
-        """`~mne.io.Raw` instance from which the segmentation was computed."""
-        return self._inst.copy()
-
-
-@fill_doc
-class EpochsSegmentation(_BaseSegmentation):
-    """Contains the segmentation of an `~mne.Epochs` instance.
-
-    Parameters
-    ----------
-    %(labels_epo)s
-    epochs : Epochs
-        `~mne.Epochs` instance used for prediction.
-    %(cluster_centers_seg)s
-    %(cluster_names)s
-    %(predict_parameters)s
-    """
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        _check_type(self._inst, (BaseEpochs,), "epochs")
-
-        if self._labels.ndim != 2:
-            raise ValueError(
-                "Argument 'labels' should be a 2D array. The provided array "
-                f"shape is {self._labels.shape} which has {self._labels.ndim} "
-                "dimensions."
-            )
-        if len(self._inst) != self._labels.shape[0]:
-            raise ValueError(
-                "Provided MNE instance and labels do not have the same number "
-                f"of epochs. The 'MNE instance' has {len(self._inst)} epochs, "
-                f"while the 'labels' has {self._labels.shape[0]} epochs."
-            )
-        if self._inst.times.size != self._labels.shape[-1]:
-            raise ValueError(
-                "Provided MNE epochs and labels do not have the same number "
-                f"of samples. The 'epochs' have {self._inst.times.size} "
-                f"samples, while the 'labels' has {self._labels.shape[-1]} "
-                "samples."
-            )
-
-    @fill_doc
-    def plot(
-        self,
-        cmap: Optional[str] = None,
-        axes: Optional[Axes] = None,
-        cbar_axes: Optional[Axes] = None,
-        *,
-        block: bool = False,
-        verbose=None,
-    ):
-        """Plot segmentation.
-
-        Parameters
-        ----------
-        %(cmap)s
-        %(axes_seg)s
-        %(axes_cbar)s
-        %(block)s
-        %(verbose)s
-
-        Returns
-        -------
-        fig : Figure
-            Matplotlib figure containing the segmentation.
-        """
-        # Error checking on the input is performed in the viz function.
-        return plot_epoch_segmentation(
-            labels=self._labels,
-            epochs=self._inst,
-            n_clusters=self._cluster_centers_.shape[0],
-            cluster_names=self._cluster_names,
-            cmap=cmap,
-            axes=axes,
-            cbar_axes=cbar_axes,
-            block=block,
-            verbose=verbose,
-        )
-
-    # --------------------------------------------------------------------
-    @property
-    def epochs(self) -> BaseEpochs:
-        """`~mne.Epochs` instance from which the segmentation was computed."""
-        return self._inst.copy()
```

### Comparing `pycrostates-0.2.0/pycrostates/utils/_checks.py` & `pycrostates-0.3.0/pycrostates/utils/_checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Utility functions for checking types and values. Inspired from MNE."""
 
+import logging
 import multiprocessing as mp
 import operator
 import os
 from itertools import product
 from pathlib import Path
+from typing import Any
 
 import numpy as np
 from matplotlib.axes import Axes
 from mne import pick_info
 from mne.utils import check_random_state
 
+from ._docs import fill_doc
+
 
 def _ensure_int(item, item_name=None):
     """
     Ensure a variable is an integer.
 
     Parameters
     ----------
@@ -291,7 +295,52 @@
         channels_msg = ", ".join(
             "%s '%s' channel(s)" % t for t in zip(counts, ch_types)
         )
         raise ValueError(
             "Only one datatype can be selected, but 'picks' "
             f"results in {channels_msg}."
         )
+
+
+@fill_doc
+def _check_verbose(verbose: Any) -> int:
+    """Check that the value of verbose is valid.
+
+    Parameters
+    ----------
+    %(verbose)s
+
+    Returns
+    -------
+    verbose : int
+        The verbosity level as an integer.
+    """
+    logging_types = dict(
+        DEBUG=logging.DEBUG,
+        INFO=logging.INFO,
+        WARNING=logging.WARNING,
+        ERROR=logging.ERROR,
+        CRITICAL=logging.CRITICAL,
+    )
+
+    _check_type(verbose, (bool, str, "int", None), item_name="verbose")
+
+    if verbose is None:
+        verbose = logging.WARNING
+    elif isinstance(verbose, str):
+        verbose = verbose.upper()
+        _check_value(verbose, logging_types, item_name="verbose")
+        verbose = logging_types[verbose]
+    elif isinstance(verbose, bool):
+        if verbose:
+            verbose = logging.INFO
+        else:
+            verbose = logging.WARNING
+    elif isinstance(verbose, int):
+        verbose = _ensure_int(verbose)
+        if verbose <= 0:
+            raise ValueError(
+                "Argument 'verbose' can not be a negative integer, "
+                f"{verbose} is invalid."
+            )
+
+    return verbose
```

### Comparing `pycrostates-0.2.0/pycrostates/utils/_config.py` & `pycrostates-0.3.0/pycrostates/utils/_config.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/utils/_docs.py` & `pycrostates-0.3.0/pycrostates/utils/_docs.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,33 +16,42 @@
 keys: Tuple[str, ...] = (
     "n_jobs",
     "picks_all",
     "random_state",
     "tmin_raw",
     "tmax_raw",
     "reject_by_annotation_raw",
-    "verbose",
 )
 
 for key in keys:
     entry = docdict_mne[key]
     if ".. versionchanged::" in entry:
         entry = entry.replace(
             ".. versionchanged::", ".. versionchanged:: MNE "
         )
     if ".. versionadded::" in entry:
         entry = entry.replace(".. versionadded::", ".. versionadded:: MNE ")
     docdict[key] = entry
 
+docdict[
+    "verbose"
+] = """
+verbose : int | str | bool | None
+    Sets the verbosity level. The verbosity increases gradually between
+    ``"CRITICAL"``, ``"ERROR"``, ``"WARNING"``, ``"INFO"`` and ``"DEBUG"``.
+    If None is provided, the verbosity is set to ``"WARNING"``.
+    If a bool is provided, the verbosity is set to ``"WARNING"`` for False and
+    to ``"INFO"`` for True."""
+
 # ---- Clusters ----
 docdict[
     "n_clusters"
 ] = """
 n_clusters : int
-    The number of clusters, i.e. the number of microstates, to look for.
+    The number of clusters, i.e. the number of microstates.
 """
 docdict[
     "cluster_centers"
 ] = """
 cluster_centers : array (n_clusters, n_channels)
     Fitted clusters, i.e. the microstates maps."""
 docdict[
@@ -73,34 +82,73 @@
     "cluster_centers_seg"
 ] = """
 cluster_centers : array (n_clusters, n_channels)
      Clusters, i.e. the microstates maps used to compute the segmentation."""
 docdict[
     "labels_raw"
 ] = """
-labels : array (n_samples, )
+labels : array of shape ``(n_samples,)``
     Microstates labels attributed to each sample, i.e. the segmentation."""
 docdict[
     "labels_epo"
 ] = """
-labels : array (n_epochs, n_samples)
+labels : array of shape ``(n_epochs, n_samples)``
+    Microstates labels attributed to each sample, i.e. the segmentation."""
+docdict[
+    "labels_transition"
+] = """
+labels : array of shape ``(n_samples,)`` or ``(n_epochs, n_samples)``
     Microstates labels attributed to each sample, i.e. the segmentation."""
 # TODO: predict_parameters docstring is missing.
 docdict[
     "predict_parameters"
 ] = """
 predict_parameters : dict | None
     The prediction parameters."""
+docdict[
+    "stat_transition"
+] = """
+stat : str
+    Aggregate statistic to compute transitions. Can be:
+
+    * ``count``: show the number of observations of each transition.
+    * ``probability`` or ``proportion``: normalize count such as the
+      probabilities along the first axis is always equal to ``1``.
+    * ``percent``: normalize count such as the
+      probabilities along the first axis is always equal to ``100``."""
+docdict[
+    "stat_expected_transitions"
+] = """
+stat : str
+    Aggregate statistic to compute transitions. Can be:
+
+    * ``probability`` or ``proportion``: normalize count such as the
+      probabilities along the first axis is always equal to ``1``.
+    * ``percent``: normalize count such as the
+      probabilities along the first axis is always equal to ``100``."""
+docdict[
+    "ignore_self"
+] = """
+ignore_self : bool
+    If True, ignores the transition from one state to itself.
+    This is equivalent to setting the duration of all states to 1 sample."""
+docdict[
+    "transition_matrix"
+] = """
+T : array of shape ``(n_cluster, n_cluster)``
+    Array of transition probability values from one label to another.
+    First axis indicates state ``"from"``. Second axis indicates state
+    ``"to"``."""
 
 # ------ Viz -------
 docdict[
     "cmap"
 ] = """
-cmap : str | None
-    The name of a colormap known to Matplotlib."""
+cmap : str | colormap | None
+    The colormap to use. If None, ``viridis`` is used."""
 docdict[
     "block"
 ] = """
 block : bool
     Whether to halt program execution until the figure is closed."""
 docdict[
     "axes_topo"
```

### Comparing `pycrostates-0.2.0/pycrostates/utils/_imports.py` & `pycrostates-0.3.0/pycrostates/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/utils/mixin.py` & `pycrostates-0.3.0/pycrostates/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/utils/utils.py` & `pycrostates-0.3.0/pycrostates/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pycrostates-0.2.0/pycrostates/viz/cluster_centers.py` & `pycrostates-0.3.0/pycrostates/viz/cluster_centers.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 @fill_doc
 def plot_cluster_centers(
     cluster_centers: NDArray[float],
     info: Union[Info, CHInfo],
     cluster_names: List[str] = None,
-    axes: Optional[Axes] = None,
+    axes: Optional[Union[Axes, NDArray[Axes]]] = None,
     *,
     block: bool = False,
     **kwargs,
 ):
     """Create topographic maps for cluster centers.
 
     Parameters
```

### Comparing `pycrostates-0.2.0/pycrostates/viz/segmentation.py` & `pycrostates-0.3.0/pycrostates/viz/segmentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Visualisation module for plotting segmentations."""
 
 from typing import List, Optional, Union
 
 import numpy as np
-from matplotlib import colors
+from matplotlib import colormaps, colors
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from mne import BaseEpochs
 from mne.io import BaseRaw
+from mne.utils import check_version
 from numpy.typing import NDArray
 
 from ..utils._checks import _check_type
 from ..utils._docs import fill_doc
-from ..utils._logs import _set_verbose, logger
+from ..utils._logs import logger, verbose
 
 
 @fill_doc
 def plot_raw_segmentation(
     labels: NDArray[int],
     raw: BaseRaw,
     n_clusters: int,
@@ -190,40 +191,40 @@
     axes.vlines(x, 0, gfp.max(), linestyles="dashed", colors="black")
 
     if show:
         plt.show(block=block)
     return fig
 
 
+@verbose
 def _plot_segmentation(
     labels: NDArray[int],
     gfp: NDArray[float],
     times: NDArray[float],
     n_clusters: int,
     cluster_names: List[str] = None,
-    cmap: Optional[str] = None,
+    cmap: Optional[Union[str, colors.Colormap]] = None,
     axes: Optional[Axes] = None,
     cbar_axes: Optional[Axes] = None,
     *,
     verbose: Optional[str] = None,
     **kwargs,
 ):
     """Code snippet to plot segmentation for raw and epochs."""
-    _set_verbose(verbose)
     _check_type(labels, (np.ndarray,), "labels")  # 1D array (n_times, )
     _check_type(gfp, (np.ndarray,), "gfp")  # 1D array (n_times, )
     _check_type(times, (np.ndarray,), "times")  # 1D array (n_times, )
     _check_type(n_clusters, ("int",), "n_clusters")
     if n_clusters <= 0:
         raise ValueError(
             f"Provided number of clusters {n_clusters} is invalid. The number "
             "of clusters must be strictly positive."
         )
     _check_type(cluster_names, (None, list, tuple), "cluster_names")
-    _check_type(cmap, (None, str), "cmap")
+    _check_type(cmap, (None, str, colors.Colormap), "cmap")
     _check_type(axes, (None, Axes), "ax")
     _check_type(cbar_axes, (None, Axes), "cbar_ax")
 
     # check cluster_names
     if cluster_names is None:
         cluster_names = [str(k) for k in range(1, n_clusters + 1)]
     if len(cluster_names) != n_clusters:
@@ -251,15 +252,15 @@
     if "linewidth" not in kwargs:
         kwargs["linewidth"] = 0.2
 
     # define states and colors
     state_labels = [-1] + list(range(n_clusters))
     cluster_names = ["unlabeled"] + cluster_names
     n_colors = n_clusters + 1
-    cmap = plt.cm.get_cmap(cmap, n_colors)
+    cmap = _compatibility_cmap(cmap, n_colors)
 
     # plot
     axes.plot(times, gfp, **kwargs)
     for state, color in zip(state_labels, cmap.colors):
         pos = np.where(labels == state)[0]
         if len(pos):
             pos = np.unique([pos, pos + 1])
@@ -287,7 +288,34 @@
     sm.set_array([])
     colorbar = plt.colorbar(
         sm, cax=cbar_axes, ax=axes, ticks=[i + 0.5 for i in range(n_colors)]
     )
     colorbar.ax.set_yticklabels(cluster_names)
 
     return fig, axes, show
+
+
+def _compatibility_cmap(
+    cmap: Optional[Union[str, colors.Colormap]],
+    n_colors: int,
+):
+    """Convert the 'cmap' argument to a colormap.
+
+    Matplotlib 3.6 introduced a deprecation of plt.cm.get_cmap().
+    When support for the 3.6 version is dropped, this checker can be removed.
+    """
+    if check_version("matplotlib", "3.6"):
+        if cmap is None:
+            cmap = colormaps["viridis"]
+        elif isinstance(cmap, str):
+            cmap = colormaps[cmap]  # the cmap name is checked by matplotlib
+        cmap = cmap.resampled(n_colors)
+    else:
+        if isinstance(cmap, (str, type(None))):
+            cmap = plt.cm.get_cmap(cmap, n_colors)
+        else:
+            raise RuntimeError(
+                "User-defined colormaps are supported as of matplotlib 3.6 "
+                "and above. Please update matplotlib or provide a colormap "
+                "name as a string."
+            )
+    return cmap
```

### Comparing `pycrostates-0.2.0/pycrostates.egg-info/PKG-INFO` & `pycrostates-0.3.0/pycrostates.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrostates
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple open source Python package for EEG microstate segmentation.
 Author-email: Victor Férat <victor.ferat@unige.ch>
 Maintainer-email: Victor Férat <victor.ferat@unige.ch>, Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Victor Férat
         All rights reserved.
@@ -39,23 +39,24 @@
 Project-URL: source, https://github.com/vferat/pycrostates
 Project-URL: tracker, https://github.com/vferat/pycrostates/issues
 Keywords: python,neuroscience,neuroimaging,eeg,microstates,brain
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
@@ -63,14 +64,15 @@
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![PyPI version](https://badge.fury.io/py/pycrostates.svg)](https://badge.fury.io/py/pycrostates)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/pycrostates.svg)](https://anaconda.org/conda-forge/pycrostates)
 [![Documentation Status](https://readthedocs.org/projects/pycrostates/badge/?version=latest)](https://pycrostates.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://dev.azure.com/vferat/pycrostates/_apis/build/status/vferat.pycrostates?branchName=main)](https://dev.azure.com/vferat/pycrostates/_build/latest?definitionId=1&branchName=main)
 [![codecov](https://codecov.io/gh/vferat/pycrostates/branch/master/graph/badge.svg?token=47COGGCGX8)](https://codecov.io/gh/vferat/pycrostates)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/029e425f90614943b0a944e03922b637)](https://www.codacy.com/gh/vferat/pycrostates/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vferat/pycrostates&amp;utm_campaign=Badge_Grade)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04564/status.svg)](https://doi.org/10.21105/joss.04564)
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_white.png">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_black.png">
   <img alt="Pycrostate logo" src="https://raw.githubusercontent.com/vferat/pycrostates/main/docs/_static/logos/Pycrostates_logo_black.png">
 </picture>
 
@@ -88,26 +90,26 @@
 ## Installation
 [![Downloads](https://pepy.tech/badge/pycrostates/month)](https://pepy.tech/project/pycrostates)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pycrostates/badges/downloads.svg)](https://anaconda.org/conda-forge/pycrostates)
 
 Installation instructions can be found [here](https://pycrostates.readthedocs.io/en/latest/install.html).
 
 ## Citing
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6915329.svg)](https://doi.org/10.5281/zenodo.6915329)
-[![status](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3/status.svg)](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04564/status.svg)](https://doi.org/10.21105/joss.04564)
 
-To cite specific version numbers of the software, you can use the DOIs provided by [Zenodo](https://doi.org/10.5281/zenodo.6915329).
-The canonical journal article reference is currently under review at the [JOSS](https://joss.theoj.org/papers/be7e10c061e28f5694cb7366aef445a3) journal and can't be cited yet.
+The associated paper can be retrieved here: https://joss.theoj.org/papers/10.21105/joss.04564
+To cite specific version numbers of the software, you can use the DOIs provided
+by [Zenodo](https://zenodo.org/record/7129852).
 
 ## Contributing
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 Pycrostates welcomes contributions from anyone interested in improving this project. These contributions can take the form of bug reports/fixes, feature requests/additions, documentation revision and new tutorials.
 
 In all cases, it is recommended to [open a new issue](https://github.com/vferat/pycrostates/issues/new/choose) on Github to discuss the best way to integrate a contribution.
 
 Check the [Contribution Guide](https://github.com/vferat/pycrostates/blob/main/CONTRIBUTING.md) if you want to make a changes to Pycrostates.
@@ -116,19 +118,22 @@
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="https://vferat.github.io/about/"><img src="https://avatars.githubusercontent.com/u/28844486?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Victor Férat</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Tests">⚠️</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Documentation">📖</a> <a href="#ideas-vferat" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-vferat" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-vferat" title="Maintenance">🚧</a> <a href="#projectManagement-vferat" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Avferat" title="Reviewed Pull Requests">👀</a></td>
-    <td align="center"><a href="https://github.com/mscheltienne"><img src="https://avatars.githubusercontent.com/u/73893616?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mathieu Scheltienne</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Documentation">📖</a> <a href="#ideas-mscheltienne" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-mscheltienne" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-mscheltienne" title="Maintenance">🚧</a> <a href="#projectManagement-mscheltienne" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Amscheltienne" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Tests">⚠️</a></td>
-    <td align="center"><a href="https://github.com/LouPlanchamp"><img src="https://avatars.githubusercontent.com/u/107875645?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Lou</b></sub></a><br /><a href="#design-LouPlanchamp" title="Design">🎨</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center"><a href="https://vferat.github.io/about/"><img src="https://avatars.githubusercontent.com/u/28844486?v=4?s=100" width="100px;" alt="Victor Férat"/><br /><sub><b>Victor Férat</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Tests">⚠️</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=vferat" title="Documentation">📖</a> <a href="#ideas-vferat" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-vferat" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-vferat" title="Maintenance">🚧</a> <a href="#projectManagement-vferat" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Avferat" title="Reviewed Pull Requests">👀</a></td>
+      <td align="center"><a href="https://github.com/mscheltienne"><img src="https://avatars.githubusercontent.com/u/73893616?v=4?s=100" width="100px;" alt="Mathieu Scheltienne"/><br /><sub><b>Mathieu Scheltienne</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Documentation">📖</a> <a href="#ideas-mscheltienne" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-mscheltienne" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-mscheltienne" title="Maintenance">🚧</a> <a href="#projectManagement-mscheltienne" title="Project Management">📆</a> <a href="https://github.com/vferat/pycrostates/pulls?q=is%3Apr+reviewed-by%3Amscheltienne" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/vferat/pycrostates/commits?author=mscheltienne" title="Tests">⚠️</a></td>
+      <td align="center"><a href="https://github.com/LouPlanchamp"><img src="https://avatars.githubusercontent.com/u/107875645?v=4?s=100" width="100px;" alt="Lou"/><br /><sub><b>Lou</b></sub></a><br /><a href="#design-LouPlanchamp" title="Design">🎨</a></td>
+      <td align="center"><a href="https://github.com/rkobler"><img src="https://avatars.githubusercontent.com/u/22491497?v=4?s=100" width="100px;" alt="rkobler"/><br /><sub><b>rkobler</b></sub></a><br /><a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Code">💻</a> <a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Documentation">📖</a> <a href="#ideas-rkobler" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/vferat/pycrostates/commits?author=rkobler" title="Tests">⚠️</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

### Comparing `pycrostates-0.2.0/pycrostates.egg-info/SOURCES.txt` & `pycrostates-0.3.0/pycrostates.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 pycrostates.egg-info/PKG-INFO
 pycrostates.egg-info/SOURCES.txt
 pycrostates.egg-info/dependency_links.txt
 pycrostates.egg-info/requires.txt
 pycrostates.egg-info/top_level.txt
 pycrostates/cluster/__init__.py
 pycrostates/cluster/_base.py
+pycrostates/cluster/aahc.py
 pycrostates/cluster/kmeans.py
+pycrostates/cluster/utils/__init__.py
+pycrostates/cluster/utils/utils.py
 pycrostates/datasets/__init__.py
 pycrostates/datasets/lemon/__init__.py
 pycrostates/datasets/lemon/lemon.py
 pycrostates/datasets/lemon/data/PREPROCESSED_LEMON_registry.txt
 pycrostates/html_templates/__init__.py
 pycrostates/html_templates/_templates.py
+pycrostates/html_templates/repr/AAHCluster.html.jinja
 pycrostates/html_templates/repr/BaseCluster.html.jinja
 pycrostates/html_templates/repr/BaseSegmentation.html.jinja
 pycrostates/html_templates/repr/ChData.html.jinja
 pycrostates/html_templates/repr/ModKMeans.html.jinja
 pycrostates/io/__init__.py
 pycrostates/io/ch_data.py
 pycrostates/io/fiff.py
@@ -32,20 +36,24 @@
 pycrostates/metrics/calinski_harabasz.py
 pycrostates/metrics/davies_bouldin.py
 pycrostates/metrics/dunn.py
 pycrostates/metrics/silhouette.py
 pycrostates/preprocessing/__init__.py
 pycrostates/preprocessing/extract_gfp_peaks.py
 pycrostates/preprocessing/resample.py
+pycrostates/preprocessing/spatial_filter.py
 pycrostates/segmentation/__init__.py
+pycrostates/segmentation/_base.py
 pycrostates/segmentation/segmentation.py
+pycrostates/segmentation/transitions.py
 pycrostates/utils/__init__.py
 pycrostates/utils/_checks.py
 pycrostates/utils/_config.py
 pycrostates/utils/_docs.py
+pycrostates/utils/_fixes.py
 pycrostates/utils/_imports.py
 pycrostates/utils/_logs.py
 pycrostates/utils/mixin.py
 pycrostates/utils/utils.py
 pycrostates/viz/__init__.py
 pycrostates/viz/cluster_centers.py
 pycrostates/viz/segmentation.py
```

### Comparing `pycrostates-0.2.0/pyproject.toml` & `pycrostates-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ['setuptools >= 61.0.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'pycrostates'
-version = '0.2.0'
+version = '0.3.0'
 description = 'A simple open source Python package for EEG microstate segmentation.'
 readme = 'README.md'
 license = {file = 'LICENSE'}
-requires-python = '>=3.7'
+requires-python = '>=3.8'
 authors = [
     {name = 'Victor Férat', email = 'victor.ferat@unige.ch'},
 ]
 maintainers = [
     {name = 'Victor Férat', email = 'victor.ferat@unige.ch'},
     {name = 'Mathieu Scheltienne', email = 'mathieu.scheltienne@fcbg.ch'},
 ]
@@ -25,34 +25,34 @@
     'brain',
 ]
 classifiers = [
     'Operating System :: Microsoft :: Windows',
     'Operating System :: Unix',
     'Operating System :: MacOS',
     'Programming Language :: Python :: 3 :: Only',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Natural Language :: English',
     'License :: OSI Approved :: BSD License',
     'Intended Audience :: Science/Research',
+    'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering',
 ]
 dependencies = [
     'numpy>=1.21',
     'scipy',
     'mne>=1.0.0',
     'joblib',
     'matplotlib',
     'scikit-learn',
     'pooch',
     'decorator',
     'jinja2',
-    'importlib-metadata; python_version < "3.8"',
     'importlib-resources; python_version < "3.9"',
 ]
 
 [project.optional-dependencies]
 build = ['build', 'twine']
 docs = [
     'memory-profiler',
@@ -62,16 +62,18 @@
     'pymatreader',
     'sphinx',
     'sphinxcontrib-bibtex',
     'sphinx-copybutton',
     'sphinx-design',
     'sphinx_gallery',
     'sphinx-issues',
+    'seaborn',
 ]
 style = [
+    'bibclean',
     'black',
     'codespell',
     'isort',
     'flake8',
     'pydocstyle[toml]',
 ]
 test = [
@@ -124,21 +126,40 @@
 multi_line_output = 3
 line_length = 79
 py_version = 37
 extend_skip_glob = [
     'setup.py',
     'docs/*',
     'tutorials/*',
-    'pycrostates/html_templates/repr/*'
+    'pycrostates/html_templates/repr/*',
 ]
 
 [tool.pydocstyle]
 convention = 'numpy'
 ignore-decorators= '(copy_doc|property|.*setter|.*getter)'
 match = '^(?!setup|__init__|test_).*\.py'
 match-dir = '^(?!docs|tutorials|build|dist|\.).*'
 add_ignore = 'D100,D104,D107'
 
 [tool.pytest.ini_options]
+minversion = '6.0'
+addopts = '--durations 20 --junit-xml=junit-results.xml --verbose'
 filterwarnings = [
     "ignore:Matplotlib is currently using agg:UserWarning",
 ]
+
+[tool.coverage.run]
+branch = true
+cover_pylib = false
+omit = [
+    '**/__init__.py',
+    '**/pycrostates/_version.py',
+    '**/pycrostates/utils/_fixes.py',
+    '**/tests/**',
+]
+
+[tool.coverage.report]
+exclude_lines = [
+    'pragma: no cover',
+    'if __name__ == .__main__.:',
+]
+precision = 2
```

