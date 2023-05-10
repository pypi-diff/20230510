# Comparing `tmp/cluster_experiments-0.8.0.tar.gz` & `tmp/cluster_experiments-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.8.0.tar", last modified: Wed May 10 11:17:58 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.8.1.tar", last modified: Wed May 10 12:57:00 2023, max compression
```

## Comparing `cluster_experiments-0.8.0.tar` & `cluster_experiments-0.8.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.718049 cluster_experiments-0.8.0/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.8.0/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.8.0/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-10 11:17:58.717511 cluster_experiments-0.8.0/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7603 2023-05-10 11:17:47.000000 cluster_experiments-0.8.0/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.659973 cluster_experiments-0.8.0/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1760 2023-05-10 11:17:47.000000 cluster_experiments-0.8.0/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.8.0/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    21014 2023-05-09 15:17:29.000000 cluster_experiments-0.8.0/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    16391 2023-05-10 11:17:47.000000 cluster_experiments-0.8.0/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19753 2023-05-09 09:26:42.000000 cluster_experiments-0.8.0/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4784 2023-05-10 11:17:47.000000 cluster_experiments-0.8.0/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.8.0/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.8.0/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.8.0/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.666448 cluster_experiments-0.8.0/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-10 11:17:58.000000 cluster_experiments-0.8.0/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1481 2023-05-10 11:17:58.000000 cluster_experiments-0.8.0/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-10 11:17:58.000000 cluster_experiments-0.8.0/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-10 11:17:58.000000 cluster_experiments-0.8.0/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-10 11:17:58.000000 cluster_experiments-0.8.0/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-10 11:17:58.718264 cluster_experiments-0.8.0/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-10 11:17:47.000000 cluster_experiments-0.8.0/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.678341 cluster_experiments-0.8.0/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.8.0/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.682808 cluster_experiments-0.8.0/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.0/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-05-09 15:17:29.000000 cluster_experiments-0.8.0/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.8.0/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.687246 cluster_experiments-0.8.0/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.0/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.8.0/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.8.0/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2406 2023-05-09 09:26:42.000000 cluster_experiments-0.8.0/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.689966 cluster_experiments-0.8.0/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.0/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9422 2023-05-10 11:17:47.000000 cluster_experiments-0.8.0/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.705044 cluster_experiments-0.8.0/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.0/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3283 2023-05-09 09:26:42.000000 cluster_experiments-0.8.0/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.8.0/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.8.0/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.8.0/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.8.0/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.8.0/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      941 2023-05-09 09:26:42.000000 cluster_experiments-0.8.0/tests/power_analysis/test_seed.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3107 2023-05-09 09:26:42.000000 cluster_experiments-0.8.0/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 11:17:58.715561 cluster_experiments-0.8.0/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.0/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.8.0/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.8.0/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.8.0/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.8.0/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.8.0/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2282 2023-05-10 11:17:47.000000 cluster_experiments-0.8.0/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.8.0/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.8.0/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.8.0/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.601783 cluster_experiments-0.8.1/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.8.1/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.8.1/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-10 12:57:00.599527 cluster_experiments-0.8.1/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7603 2023-05-10 11:17:47.000000 cluster_experiments-0.8.1/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.540660 cluster_experiments-0.8.1/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1760 2023-05-10 11:17:47.000000 cluster_experiments-0.8.1/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.8.1/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    21014 2023-05-09 15:17:29.000000 cluster_experiments-0.8.1/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    16391 2023-05-10 11:17:47.000000 cluster_experiments-0.8.1/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19753 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4748 2023-05-10 12:56:47.000000 cluster_experiments-0.8.1/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.8.1/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.8.1/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.8.1/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.549134 cluster_experiments-0.8.1/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1481 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-10 12:57:00.000000 cluster_experiments-0.8.1/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-10 12:57:00.602026 cluster_experiments-0.8.1/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-10 12:56:47.000000 cluster_experiments-0.8.1/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.562217 cluster_experiments-0.8.1/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.8.1/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.566452 cluster_experiments-0.8.1/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.1/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-05-09 15:17:29.000000 cluster_experiments-0.8.1/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.8.1/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.570642 cluster_experiments-0.8.1/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.8.1/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.8.1/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2406 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.573227 cluster_experiments-0.8.1/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.1/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9410 2023-05-10 12:56:47.000000 cluster_experiments-0.8.1/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.587919 cluster_experiments-0.8.1/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3283 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.8.1/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.8.1/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.8.1/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      941 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/tests/power_analysis/test_seed.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3107 2023-05-09 09:26:42.000000 cluster_experiments-0.8.1/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-10 12:57:00.598063 cluster_experiments-0.8.1/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.8.1/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.8.1/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.8.1/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.8.1/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.8.1/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.8.1/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2282 2023-05-10 11:17:47.000000 cluster_experiments-0.8.1/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.8.1/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.8.1/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.8.1/tests/utils.py
```

### Comparing `cluster_experiments-0.8.0/LICENSE` & `cluster_experiments-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/README.md` & `cluster_experiments-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments/__init__.py` & `cluster_experiments-0.8.1/cluster_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments/cupac.py` & `cluster_experiments-0.8.1/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.8.1/cluster_experiments/experiment_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments/perturbator.py` & `cluster_experiments-0.8.1/cluster_experiments/perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments/power_analysis.py` & `cluster_experiments-0.8.1/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments/power_config.py` & `cluster_experiments-0.8.1/cluster_experiments/power_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,17 +122,17 @@
 
     seed: Optional[int] = None
 
 
 perturbator_mapping = {
     "binary": BinaryPerturbator,
     "uniform": UniformPerturbator,
-    "relative_positive_perturbator": RelativePositivePerturbator,
-    "normal_perturbator": NormalPerturbator,
-    "beta_relative_positive_perturbator": BetaRelativePositivePerturbator,
+    "relative_positive": RelativePositivePerturbator,
+    "normal": NormalPerturbator,
+    "beta_relative_positive": BetaRelativePositivePerturbator,
 }
 
 splitter_mapping = {
     "clustered": ClusteredSplitter,
     "clustered_balance": BalancedClusteredSplitter,
     "non_clustered": NonClusteredSplitter,
     "clustered_stratified": StratifiedClusteredSplitter,
```

### Comparing `cluster_experiments-0.8.0/cluster_experiments/random_splitter.py` & `cluster_experiments-0.8.1/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments/washover.py` & `cluster_experiments-0.8.1/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.8.1/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.8.1/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/setup.py` & `cluster_experiments-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.8.0",
+    version="0.8.1",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.8.0/tests/analysis/test_analysis.py` & `cluster_experiments-0.8.1/tests/analysis/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/cupac/test_aggregator.py` & `cluster_experiments-0.8.1/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.8.1/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/examples.py` & `cluster_experiments-0.8.1/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.8.1/tests/perturbator/test_perturbator.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     assert np.var(perturbated_values) == np.var(effect)
 
 
 def test_normal_perturbator_from_config():
     config = PowerConfig(
         analysis="gee",
         splitter="clustered_balance",
-        perturbator="normal_perturbator",
+        perturbator="normal",
         cluster_cols=["cluster"],
         n_simulations=100,
     )
     np = NormalPerturbator.from_config(config)
     assert isinstance(np, NormalPerturbator)
```

### Comparing `cluster_experiments-0.8.0/tests/power_analysis/conftest.py` & `cluster_experiments-0.8.1/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.8.1/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.8.1/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.8.1/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.8.1/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.8.1/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/power_analysis/test_seed.py` & `cluster_experiments-0.8.1/tests/power_analysis/test_seed.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.8.1/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/splitter/conftest.py` & `cluster_experiments-0.8.1/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/splitter/test_splitter.py` & `cluster_experiments-0.8.1/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.8.1/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/splitter/test_time_col.py` & `cluster_experiments-0.8.1/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/splitter/test_washover.py` & `cluster_experiments-0.8.1/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/test_docs.py` & `cluster_experiments-0.8.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/test_non_clustered.py` & `cluster_experiments-0.8.1/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.8.0/tests/utils.py` & `cluster_experiments-0.8.1/tests/utils.py`

 * *Files identical despite different names*

