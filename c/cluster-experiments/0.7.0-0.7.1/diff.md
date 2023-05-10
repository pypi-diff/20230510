# Comparing `tmp/cluster_experiments-0.7.0.tar.gz` & `tmp/cluster_experiments-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cluster_experiments-0.7.0.tar", last modified: Tue May  9 07:58:22 2023, max compression
+gzip compressed data, was "dist/cluster_experiments-0.7.1.tar", last modified: Tue May  9 15:19:19 2023, max compression
```

## Comparing `cluster_experiments-0.7.0.tar` & `cluster_experiments-0.7.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.776365 cluster_experiments-0.7.0/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.7.0/LICENSE
--rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.7.0/MANIFEST.in
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-09 07:58:22.775724 cluster_experiments-0.7.0/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     7150 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/README.md
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.705041 cluster_experiments-0.7.0/cluster_experiments/
--rw-r--r--   0 davidmasip   (502) staff       (20)     1512 2023-04-05 14:50:51.000000 cluster_experiments-0.7.0/cluster_experiments/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.7.0/cluster_experiments/cupac.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    18320 2023-04-28 14:00:38.000000 cluster_experiments-0.7.0/cluster_experiments/experiment_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5609 2023-05-09 07:57:58.000000 cluster_experiments-0.7.0/cluster_experiments/perturbator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    19753 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/cluster_experiments/power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     4342 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/cluster_experiments/power_config.py
--rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.7.0/cluster_experiments/random_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.7.0/cluster_experiments/utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.7.0/cluster_experiments/washover.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.713376 cluster_experiments-0.7.0/cluster_experiments.egg-info/
--rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/PKG-INFO
--rw-r--r--   0 davidmasip   (502) staff       (20)     1481 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/requires.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-09 07:58:22.000000 cluster_experiments-0.7.0/cluster_experiments.egg-info/top_level.txt
--rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-09 07:58:22.776542 cluster_experiments-0.7.0/setup.cfg
--rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/setup.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.726593 cluster_experiments-0.7.0/tests/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.7.0/tests/__init__.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.731282 cluster_experiments-0.7.0/tests/analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.0/tests/analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3771 2023-03-01 11:45:41.000000 cluster_experiments-0.7.0/tests/analysis/test_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.7.0/tests/analysis/test_ols_analysis.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.736343 cluster_experiments-0.7.0/tests/cupac/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/cupac/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.7.0/tests/cupac/test_aggregator.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.7.0/tests/cupac/test_cupac_handler.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2406 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/tests/examples.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.739573 cluster_experiments-0.7.0/tests/perturbator/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.0/tests/perturbator/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2879 2023-05-08 15:13:10.000000 cluster_experiments-0.7.0/tests/perturbator/test_perturbator.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.764530 cluster_experiments-0.7.0/tests/power_analysis/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/power_analysis/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3283 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/tests/power_analysis/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/power_analysis/test_cupac_power.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/power_analysis/test_multivariate.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.7.0/tests/power_analysis/test_parallel.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.7.0/tests/power_analysis/test_power_analysis.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.7.0/tests/power_analysis/test_power_raises.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      941 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/tests/power_analysis/test_seed.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3107 2023-05-09 07:58:01.000000 cluster_experiments-0.7.0/tests/power_analysis/test_switchback_power.py
-drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 07:58:22.774551 cluster_experiments-0.7.0/tests/splitter/
--rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.0/tests/splitter/__init__.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.7.0/tests/splitter/conftest.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.7.0/tests/splitter/test_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.7.0/tests/splitter/test_switchback_splitter.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.7.0/tests/splitter/test_time_col.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.7.0/tests/splitter/test_washover.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2042 2023-04-05 14:50:51.000000 cluster_experiments-0.7.0/tests/test_docs.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.7.0/tests/test_non_clustered.py
--rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.7.0/tests/test_utils.py
--rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.7.0/tests/utils.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.697638 cluster_experiments-0.7.1/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1067 2022-09-02 16:02:23.000000 cluster_experiments-0.7.1/LICENSE
+-rw-r--r--   0 davidmasip   (502) staff       (20)       16 2022-08-05 13:17:06.000000 cluster_experiments-0.7.1/MANIFEST.in
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-09 15:19:19.696660 cluster_experiments-0.7.1/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7253 2023-05-09 15:17:29.000000 cluster_experiments-0.7.1/README.md
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.628936 cluster_experiments-0.7.1/cluster_experiments/
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1568 2023-05-09 15:17:29.000000 cluster_experiments-0.7.1/cluster_experiments/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     7578 2023-04-14 13:06:22.000000 cluster_experiments-0.7.1/cluster_experiments/cupac.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    21014 2023-05-09 15:17:29.000000 cluster_experiments-0.7.1/cluster_experiments/experiment_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5608 2023-05-09 09:50:57.000000 cluster_experiments-0.7.1/cluster_experiments/perturbator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    19753 2023-05-09 09:26:42.000000 cluster_experiments-0.7.1/cluster_experiments/power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4403 2023-05-09 15:17:29.000000 cluster_experiments-0.7.1/cluster_experiments/power_config.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)    17741 2023-05-08 15:05:16.000000 cluster_experiments-0.7.1/cluster_experiments/random_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      496 2023-02-10 16:31:12.000000 cluster_experiments-0.7.1/cluster_experiments/utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6137 2023-04-12 08:53:42.000000 cluster_experiments-0.7.1/cluster_experiments/washover.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.638150 cluster_experiments-0.7.1/cluster_experiments.egg-info/
+-rw-r--r--   0 davidmasip   (502) staff       (20)      173 2023-05-09 15:19:19.000000 cluster_experiments-0.7.1/cluster_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1481 2023-05-09 15:19:19.000000 cluster_experiments-0.7.1/cluster_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)        1 2023-05-09 15:19:19.000000 cluster_experiments-0.7.1/cluster_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-09 15:19:19.000000 cluster_experiments-0.7.1/cluster_experiments.egg-info/requires.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       26 2023-05-09 15:19:19.000000 cluster_experiments-0.7.1/cluster_experiments.egg-info/top_level.txt
+-rw-r--r--   0 davidmasip   (502) staff       (20)       38 2023-05-09 15:19:19.697909 cluster_experiments-0.7.1/setup.cfg
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1223 2023-05-09 15:17:29.000000 cluster_experiments-0.7.1/setup.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.648748 cluster_experiments-0.7.1/tests/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-10-21 09:42:28.000000 cluster_experiments-0.7.1/tests/__init__.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.654421 cluster_experiments-0.7.1/tests/analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.1/tests/analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     4251 2023-05-09 15:17:29.000000 cluster_experiments-0.7.1/tests/analysis/test_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      488 2023-04-24 11:36:52.000000 cluster_experiments-0.7.1/tests/analysis/test_ols_analysis.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.660147 cluster_experiments-0.7.1/tests/cupac/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.7.1/tests/cupac/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1583 2023-04-24 11:36:52.000000 cluster_experiments-0.7.1/tests/cupac/test_aggregator.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2610 2023-04-14 15:07:31.000000 cluster_experiments-0.7.1/tests/cupac/test_cupac_handler.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2406 2023-05-09 09:26:42.000000 cluster_experiments-0.7.1/tests/examples.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.663833 cluster_experiments-0.7.1/tests/perturbator/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.1/tests/perturbator/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2879 2023-05-08 15:13:10.000000 cluster_experiments-0.7.1/tests/perturbator/test_perturbator.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.683654 cluster_experiments-0.7.1/tests/power_analysis/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-30 09:27:02.000000 cluster_experiments-0.7.1/tests/power_analysis/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3283 2023-05-09 09:26:42.000000 cluster_experiments-0.7.1/tests/power_analysis/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2121 2022-12-30 09:27:02.000000 cluster_experiments-0.7.1/tests/power_analysis/test_cupac_power.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3078 2022-12-30 09:27:02.000000 cluster_experiments-0.7.1/tests/power_analysis/test_multivariate.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1088 2023-04-12 09:19:03.000000 cluster_experiments-0.7.1/tests/power_analysis/test_parallel.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     6082 2023-04-28 14:00:38.000000 cluster_experiments-0.7.1/tests/power_analysis/test_power_analysis.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3931 2022-12-30 09:27:02.000000 cluster_experiments-0.7.1/tests/power_analysis/test_power_raises.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      941 2023-05-09 09:26:42.000000 cluster_experiments-0.7.1/tests/power_analysis/test_seed.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3107 2023-05-09 09:26:42.000000 cluster_experiments-0.7.1/tests/power_analysis/test_switchback_power.py
+drwxr-xr-x   0 davidmasip   (502) staff       (20)        0 2023-05-09 15:19:19.695012 cluster_experiments-0.7.1/tests/splitter/
+-rw-r--r--   0 davidmasip   (502) staff       (20)        0 2022-12-23 16:22:32.000000 cluster_experiments-0.7.1/tests/splitter/__init__.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     5686 2023-05-08 15:05:16.000000 cluster_experiments-0.7.1/tests/splitter/conftest.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     9412 2022-12-23 16:22:32.000000 cluster_experiments-0.7.1/tests/splitter/test_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3579 2022-12-27 08:21:57.000000 cluster_experiments-0.7.1/tests/splitter/test_switchback_splitter.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2882 2023-02-10 16:31:12.000000 cluster_experiments-0.7.1/tests/splitter/test_time_col.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     3157 2023-04-12 08:53:42.000000 cluster_experiments-0.7.1/tests/splitter/test_washover.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2096 2023-05-09 15:17:29.000000 cluster_experiments-0.7.1/tests/test_docs.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     2727 2022-12-19 11:37:00.000000 cluster_experiments-0.7.1/tests/test_non_clustered.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)      208 2023-03-01 11:31:23.000000 cluster_experiments-0.7.1/tests/test_utils.py
+-rw-r--r--   0 davidmasip   (502) staff       (20)     1325 2023-04-24 11:36:52.000000 cluster_experiments-0.7.1/tests/utils.py
```

### Comparing `cluster_experiments-0.7.0/LICENSE` & `cluster_experiments-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/README.md` & `cluster_experiments-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
         * `BalancedSwitchbackSplitter`: to split data based on clusters and dates, for switchback experiments, balancing treatment and control among all clusters
         * `StratifiedSwitchbackSplitter`: to split data based on clusters and dates, for switchback experiments, balancing the number of clusters in each stratus
         * Washover for switchback experiments:
             * `EmptyWashover`: no washover done at all.
             * `ConstantWashover`: accepts a timedelta parameter and removes the data when we switch from A to B for the timedelta interval.
 * Regarding analysis:
     * `GeeExperimentAnalysis`: to run GEE analysis on the results of a clustered design
+    * `MLMExperimentAnalysis`: to run Mixed Linear Model analysis on the results of a clustered design
     * `TTestClusteredAnalysis`: to run a t-test on aggregated data for clusters
     * `PairedTTestClusteredAnalysis`: to run a paired t-test on aggregated data for clusters
     * `ClusteredOLSAnalysis`: to run OLS analysis on the results of a clustered design
     * `OLSAnalysis`: to run OLS analysis for non-clustered data
     * `TargetAggregation`: to add pre-experimental data of the outcome to reduce variance
 * Other:
     * `PowerConfig`: to conviently configure `PowerAnalysis` class
```

### Comparing `cluster_experiments-0.7.0/cluster_experiments/__init__.py` & `cluster_experiments-0.7.1/cluster_experiments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from cluster_experiments.cupac import EmptyRegressor, TargetAggregation
 from cluster_experiments.experiment_analysis import (
     ClusteredOLSAnalysis,
     ExperimentAnalysis,
     GeeExperimentAnalysis,
+    MLMExperimentAnalysis,
     OLSAnalysis,
     PairedTTestClusteredAnalysis,
     TTestClusteredAnalysis,
 )
 from cluster_experiments.perturbator import (
     BinaryPerturbator,
     Perturbator,
@@ -47,8 +48,9 @@
     "StratifiedSwitchbackSplitter",
     "ClusteredOLSAnalysis",
     "TTestClusteredAnalysis",
     "PairedTTestClusteredAnalysis",
     "EmptyWashover",
     "ConstantWashover",
     "Washover",
+    "MLMExperimentAnalysis",
 ]
```

### Comparing `cluster_experiments-0.7.0/cluster_experiments/cupac.py` & `cluster_experiments-0.7.1/cluster_experiments/cupac.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/cluster_experiments/experiment_analysis.py` & `cluster_experiments-0.7.1/cluster_experiments/experiment_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -535,7 +535,90 @@
         """Creates an OLSAnalysis object from a PowerConfig object"""
         return cls(
             target_col=config.target_col,
             treatment_col=config.treatment_col,
             treatment=config.treatment,
             covariates=config.covariates,
         )
+
+
+class MLMExperimentAnalysis(ExperimentAnalysis):
+    """
+    Class to run Mixed Linear Models clustered analysis
+
+    Arguments:
+        cluster_cols: list of columns to use as clusters
+        target_col: name of the column containing the variable to measure
+        treatment_col: name of the column containing the treatment variable
+        treatment: name of the treatment to use as the treated group
+        covariates: list of columns to use as covariates
+
+    Usage:
+
+    ```python
+    from cluster_experiments.experiment_analysis import MLMExperimentAnalysis
+    import pandas as pd
+
+    df = pd.DataFrame({
+        'x': [1, 2, 3, 0, 0, 1],
+        'treatment': ["A"] * 3 + ["B"] * 3,
+        'cluster': [1] * 6,
+    })
+
+    MLMExperimentAnalysis(
+        cluster_cols=['cluster'],
+        target_col='x',
+    ).get_pvalue(df)
+    ```
+    """
+
+    def __init__(
+        self,
+        cluster_cols: List[str],
+        target_col: str = "target",
+        treatment_col: str = "treatment",
+        treatment: str = "B",
+        covariates: Optional[List[str]] = None,
+    ):
+        super().__init__(
+            target_col=target_col,
+            treatment_col=treatment_col,
+            cluster_cols=cluster_cols,
+            treatment=treatment,
+            covariates=covariates,
+        )
+        self.regressors = [self.treatment_col] + self.covariates
+        self.formula = f"{self.target_col} ~ {' + '.join(self.regressors)}"
+
+        self.re_formula = None
+        self.vc_formula = None
+
+    def fit_mlm(self, df: pd.DataFrame) -> sm.MixedLM:
+        """Returns the fitted MLM model"""
+        return sm.MixedLM.from_formula(
+            formula=self.formula,
+            data=df,
+            groups=self._get_cluster_column(df),
+            re_formula=self.re_formula,
+            vc_formula=self.vc_formula,
+        ).fit()
+
+    def analysis_pvalue(self, df: pd.DataFrame, verbose: bool = False) -> float:
+        """Returns the p-value of the analysis
+        Arguments:
+            df: dataframe containing the data to analyze
+            verbose (Optional): bool, prints the regression summary if True
+        """
+        results_mlm = self.fit_mlm(df)
+        if verbose:
+            print(results_mlm.summary())
+
+        return results_mlm.pvalues[self.treatment_col]
+
+    def analysis_point_estimate(self, df: pd.DataFrame, verbose: bool = False) -> float:
+        """Returns the point estimate of the analysis
+        Arguments:
+            df: dataframe containing the data to analyze
+            verbose (Optional): bool, prints the regression summary if True
+        """
+        results_mlm = self.fit_mlm(df)
+        return results_mlm.params[self.treatment_col]
```

### Comparing `cluster_experiments-0.7.0/cluster_experiments/perturbator.py` & `cluster_experiments-0.7.1/cluster_experiments/perturbator.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         if n >= len(df):
             return df
         return df.sample(n=n)
 
     def _data_checks(self, df: pd.DataFrame, average_effect: float) -> None:
         """Check that outcome is indeed binary, and average effect is in (-1, 1)"""
 
-        if set(df[self.target_col].unique()) != {0, 1}:
+        if set(df[self.target_col].unique()) - {0, 1}:
             raise ValueError(
                 f"Target column must be binary, found {set(df[self.target_col].unique())}"
             )
 
         if average_effect > 1 or average_effect < -1:
             raise ValueError(
                 f"Average effect must be in (-1, 1), found {average_effect}"
```

### Comparing `cluster_experiments-0.7.0/cluster_experiments/power_analysis.py` & `cluster_experiments-0.7.1/cluster_experiments/power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/cluster_experiments/power_config.py` & `cluster_experiments-0.7.1/cluster_experiments/power_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import dataclass
 from typing import List, Optional
 
 from cluster_experiments.cupac import EmptyRegressor, TargetAggregation
 from cluster_experiments.experiment_analysis import (
     ClusteredOLSAnalysis,
     GeeExperimentAnalysis,
+    MLMExperimentAnalysis,
     OLSAnalysis,
     PairedTTestClusteredAnalysis,
     TTestClusteredAnalysis,
 )
 from cluster_experiments.perturbator import BinaryPerturbator, UniformPerturbator
 from cluster_experiments.random_splitter import (
     BalancedClusteredSplitter,
@@ -131,10 +132,11 @@
 
 analysis_mapping = {
     "gee": GeeExperimentAnalysis,
     "ols_non_clustered": OLSAnalysis,
     "ols_clustered": ClusteredOLSAnalysis,
     "ttest_clustered": TTestClusteredAnalysis,
     "paired_ttest_clustered": PairedTTestClusteredAnalysis,
+    "mlm": MLMExperimentAnalysis,
 }
 
 cupac_model_mapping = {"": EmptyRegressor, "mean_cupac_model": TargetAggregation}
```

### Comparing `cluster_experiments-0.7.0/cluster_experiments/random_splitter.py` & `cluster_experiments-0.7.1/cluster_experiments/random_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/cluster_experiments/washover.py` & `cluster_experiments-0.7.1/cluster_experiments/washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/cluster_experiments.egg-info/SOURCES.txt` & `cluster_experiments-0.7.1/cluster_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/cluster_experiments.egg-info/requires.txt` & `cluster_experiments-0.7.1/cluster_experiments.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/setup.py` & `cluster_experiments-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     "matplotlib==3.4.3",
 ]
 
 dev_packages = test_packages + util_packages + docs_packages
 
 setup(
     name="cluster_experiments",
-    version="0.7.0",
+    version="0.7.1",
     packages=find_packages(),
     extras_require={
         "dev": dev_packages,
         "test": test_packages,
         "only-test": only_test_packages,
         "docs": docs_packages,
     },
```

### Comparing `cluster_experiments-0.7.0/tests/analysis/test_analysis.py` & `cluster_experiments-0.7.1/tests/analysis/test_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 from cluster_experiments.experiment_analysis import (
     ExperimentAnalysis,
     GeeExperimentAnalysis,
+    MLMExperimentAnalysis,
     PairedTTestClusteredAnalysis,
     TTestClusteredAnalysis,
 )
 from tests.examples import analysis_df, generate_clustered_data, generate_random_data
 
 
 @pytest.fixture
@@ -47,14 +48,27 @@
     analysis_df_full = pd.concat([analysis_df for _ in range(100)])
     analyser = GeeExperimentAnalysis(
         cluster_cols=["cluster", "date"],
     )
     assert analyser.get_pvalue(analysis_df_full) >= 0
 
 
+def test_mlm_analysis(analysis_df_diff):
+    analyser = MLMExperimentAnalysis(
+        cluster_cols=["cluster", "date"],
+    )
+    # Changing just one observation so we have a p value
+    analysis_df_diff.loc[1, "target"] = 0.00001
+
+    p_value = analyser.get_pvalue(analysis_df_diff)
+    point_estimate = analyser.get_point_estimate(analysis_df_diff)
+    assert np.isclose(p_value, 0, atol=1e-5)
+    assert np.isclose(point_estimate, 0.1, atol=1e-5)
+
+
 def test_ttest(analysis_df_diff):
 
     analyser = TTestClusteredAnalysis(cluster_cols=["cluster"])
 
     assert 0.05 >= analyser.get_pvalue(analysis_df_diff) >= 0
```

### Comparing `cluster_experiments-0.7.0/tests/cupac/test_aggregator.py` & `cluster_experiments-0.7.1/tests/cupac/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/cupac/test_cupac_handler.py` & `cluster_experiments-0.7.1/tests/cupac/test_cupac_handler.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/examples.py` & `cluster_experiments-0.7.1/tests/examples.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/perturbator/test_perturbator.py` & `cluster_experiments-0.7.1/tests/perturbator/test_perturbator.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/power_analysis/conftest.py` & `cluster_experiments-0.7.1/tests/power_analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/power_analysis/test_cupac_power.py` & `cluster_experiments-0.7.1/tests/power_analysis/test_cupac_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/power_analysis/test_multivariate.py` & `cluster_experiments-0.7.1/tests/power_analysis/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/power_analysis/test_parallel.py` & `cluster_experiments-0.7.1/tests/power_analysis/test_parallel.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/power_analysis/test_power_analysis.py` & `cluster_experiments-0.7.1/tests/power_analysis/test_power_analysis.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/power_analysis/test_power_raises.py` & `cluster_experiments-0.7.1/tests/power_analysis/test_power_raises.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/power_analysis/test_seed.py` & `cluster_experiments-0.7.1/tests/power_analysis/test_seed.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/power_analysis/test_switchback_power.py` & `cluster_experiments-0.7.1/tests/power_analysis/test_switchback_power.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/splitter/conftest.py` & `cluster_experiments-0.7.1/tests/splitter/conftest.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/splitter/test_splitter.py` & `cluster_experiments-0.7.1/tests/splitter/test_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/splitter/test_switchback_splitter.py` & `cluster_experiments-0.7.1/tests/splitter/test_switchback_splitter.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/splitter/test_time_col.py` & `cluster_experiments-0.7.1/tests/splitter/test_time_col.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/splitter/test_washover.py` & `cluster_experiments-0.7.1/tests/splitter/test_washover.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/test_docs.py` & `cluster_experiments-0.7.1/tests/test_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ClusteredOLSAnalysis,
     ClusteredSplitter,
     ConstantWashover,
     EmptyRegressor,
     EmptyWashover,
     ExperimentAnalysis,
     GeeExperimentAnalysis,
+    MLMExperimentAnalysis,
     NonClusteredSplitter,
     OLSAnalysis,
     PairedTTestClusteredAnalysis,
     Perturbator,
     PowerAnalysis,
     PowerConfig,
     RandomSplitter,
@@ -49,14 +50,15 @@
     UniformPerturbator,
     _original_time_column,
     ConstantWashover,
     EmptyWashover,
     BalancedSwitchbackSplitter,
     StratifiedSwitchbackSplitter,
     SwitchbackSplitter,
+    MLMExperimentAnalysis,
 ]
 
 
 def flatten(items):
     """Flattens a list"""
     return [item for sublist in items for item in sublist]
```

### Comparing `cluster_experiments-0.7.0/tests/test_non_clustered.py` & `cluster_experiments-0.7.1/tests/test_non_clustered.py`

 * *Files identical despite different names*

### Comparing `cluster_experiments-0.7.0/tests/utils.py` & `cluster_experiments-0.7.1/tests/utils.py`

 * *Files identical despite different names*

