# Comparing `tmp/hyperparameter-tuning-0.1.9.tar.gz` & `tmp/hyperparameter-tuning-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparameter-tuning-0.1.9.tar", last modified: Fri Dec 16 14:25:56 2022, max compression
+gzip compressed data, was "hyperparameter-tuning-0.2.0.tar", last modified: Wed May 10 11:46:56 2023, max compression
```

## Comparing `hyperparameter-tuning-0.1.9.tar` & `hyperparameter-tuning-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:25:56.630912 hyperparameter-tuning-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2022-12-16 14:25:56.630912 hyperparameter-tuning-0.1.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2420 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:25:56.630912 hyperparameter-tuning-0.1.9/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/requirements/plotting.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-16 14:25:56.630912 hyperparameter-tuning-0.1.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3722 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:25:56.630912 hyperparameter-tuning-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:25:56.630912 hyperparameter-tuning-0.1.9/src/hpt/
--rwxr-xr-x   0 runner    (1001) docker     (123)       51 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/binarize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6337 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/evaluation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7042 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/thresholding_evaluation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10477 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:25:56.630912 hyperparameter-tuning-0.1.9/src/hpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/utils/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/utils/classpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    11702 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/utils/fairness_criteria.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5238 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/utils/load_yaml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3518 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/utils/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-16 14:25:43.000000 hyperparameter-tuning-0.1.9/src/hpt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 14:25:56.630912 hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2022-12-16 14:25:56.000000 hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-16 14:25:56.000000 hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 14:25:56.000000 hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 14:25:56.000000 hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-16 14:25:56.000000 hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-16 14:25:56.000000 hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:46:56.095421 hyperparameter-tuning-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-10 11:46:56.095421 hyperparameter-tuning-0.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2420 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:46:56.091421 hyperparameter-tuning-0.2.0/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/requirements/plotting.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:46:56.095421 hyperparameter-tuning-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:46:56.091421 hyperparameter-tuning-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:46:56.091421 hyperparameter-tuning-0.2.0/src/hpt/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      149 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/binarize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7083 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/evaluation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7252 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/thresholding_evaluation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11728 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:46:56.091421 hyperparameter-tuning-0.2.0/src/hpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/utils/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/utils/classpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/utils/fairness_criteria.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5473 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/utils/load_yaml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3518 2023-05-10 11:46:41.000000 hyperparameter-tuning-0.2.0/src/hpt/utils/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:46:56.095421 hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-10 11:46:56.000000 hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-10 11:46:56.000000 hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:46:56.000000 hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:46:55.000000 hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 11:46:56.000000 hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 11:46:56.000000 hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/top_level.txt
```

### Comparing `hyperparameter-tuning-0.1.9/LICENSE` & `hyperparameter-tuning-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.1.9/PKG-INFO` & `hyperparameter-tuning-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameter-tuning
-Version: 0.1.9
+Version: 0.2.0
 Summary: A minimal framework for running hyperparameter tuning
 Home-page: https://github.com/AndreFCruz/hpt
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,hyperparameter,tuning,fairness
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hyperparameter-tuning-0.1.9/README.md` & `hyperparameter-tuning-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.1.9/setup.py` & `hyperparameter-tuning-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 requirements_plotting = load_requirements(REQUIREMENTS_PLOTTING_PATH)
 
 
 # ---------------------------------------------------------------------------- #
 #                                   Version                                    #
 # ---------------------------------------------------------------------------- #
 SRC_PATH = ROOT_PATH / 'src' / 'hpt'
-VERSION_PATH = SRC_PATH / 'version.py'
+VERSION_PATH = SRC_PATH / '_version.py'
 
 with VERSION_PATH.open('rb') as version_file:
     exec(version_file.read())
 
 
 # ---------------------------------------------------------------------------- #
 #                                   SETUP                                      #
```

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/binarize.py` & `hyperparameter-tuning-0.2.0/src/hpt/binarize.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         y_true: np.ndarray,
         y_pred_scores: np.ndarray,
         threshold: Optional[float] = None,
         tpr: Optional[float] = None,
         fpr: Optional[float] = None,
         ppr: Optional[int] = None,
         random_seed: Optional[int] = 42,
-    ) -> np.ndarray:
+) -> np.ndarray:
     """Discretizes the given score predictions into binary labels,
     according to the provided target metric for thresholding.
 
     Parameters
     ----------
     y_true : np.ndarray
         The true binary labels
@@ -48,15 +48,15 @@
         f"Please provide exactly one of (threshold, fpr, tpr, ppr); got "
         f"{(threshold, fpr, tpr, ppr)}."
     )
 
     # If threshold provided, just binarize it, no untying necessary
     if threshold:
         return (y_pred_scores >= threshold).astype(int)
-    
+
     # Otherwise, we need to compute the allowed value for the numerator
     # and corresponding threshold (plus, may require random untying)
     label_pos = np.count_nonzero(y_true)
     label_neg = np.count_nonzero(1 - y_true)
     assert (total := label_pos + label_neg) == len(y_true)  # sanity check
 
     # Indices of predictions ordered by score, descending
@@ -73,30 +73,32 @@
     # (LPs for TPR, LNs for FPR, and all samples for PPR)
     # (related to the metric's denominator)
     target_samples_mask: np.ndarray
     if tpr:
         # TPs budget to ensure >= the target TPR
         positive_preds_budget = math.ceil(tpr * label_pos)
         target_samples_mask = y_true_sorted == 1  # label positive samples
-    
+        non_target_samples_mask = y_true_sorted == 0  # label negative samples
+
     elif fpr:
         # FPs budget to ensure <= the target FPR
         positive_preds_budget = math.floor(fpr * label_neg)
         target_samples_mask = y_true_sorted == 0  # label negative samples
+        non_target_samples_mask = y_true_sorted == 1  # label positive samples
 
     elif ppr:
         # PPs budget to ensure <= the target PPR
         positive_preds_budget = math.floor(ppr * total)
-        target_samples_mask = np.ones_like(y_true_sorted).astype(bool) # all samples
+        target_samples_mask = np.ones_like(y_true_sorted).astype(bool)  # all samples
 
     # Indices of target samples (relevant for the target metric), ordered by descending score
     target_samples_indices = y_pred_sorted_indices[target_samples_mask]
 
     # Find the threshold at which the specified numerator_budget is met
-    threshold_idx = target_samples_indices[positive_preds_budget]
+    threshold_idx = target_samples_indices[(positive_preds_budget - 1)]
     threshold = y_pred_scores[threshold_idx]
 
     ####################################
     # Code for random untying follows: #
     ####################################
     y_pred_binary = (y_pred_scores >= threshold).astype(int)
 
@@ -119,35 +121,58 @@
         # 2.1. if target was not met, compute number of extra predicted positives
         extra_pos_preds = actual_pos_preds - positive_preds_budget
 
         # 2.2. randomly select extra_pos_preds among the relevant
         # samples (either TPs or FPs or PPs) with the same score
         rng = np.random.RandomState(random_seed)
 
-        samples_at_target_threshold_mask = (y_pred_scores[y_pred_sorted_indices] == threshold)
-
-        target_samples_at_target_threshold_indices = (
-            y_pred_sorted_indices[
-                samples_at_target_threshold_mask &      # Filter for samples at target threshold
-                target_samples_mask                     # Filter for relevant (target) samples
-            ]
+        samples_at_target_threshold_mask = (
+            y_pred_scores[y_pred_sorted_indices] == threshold
         )
 
+        target_samples_at_target_threshold_indices = y_pred_sorted_indices[
+            samples_at_target_threshold_mask
+            & target_samples_mask  # Filter for samples at target threshold  # Filter for relevant (target) samples
+        ]
+
         # # The extra number of positive predictions must be fully explained by this score tie
         # import ipdb; ipdb.set_trace()   # TODO: figure out why this assertion fails
         # assert extra_pos_preds < len(target_samples_at_target_threshold_indices)
 
         extra_pos_preds_indices = rng.choice(
             target_samples_at_target_threshold_indices,
             size=extra_pos_preds,
-            replace=False)
+            replace=False,
+        )
 
         # 2.3. give extra_pos_preds_indices a negative prediction
         y_pred_binary[extra_pos_preds_indices] = 0
 
+        # 2.4. Randomly sample the non-target labels at same rate
+        if tpr or fpr:
+            sampled_fraction = 1 - (positive_preds_budget / actual_pos_preds)
+
+            non_target_samples_at_target_threshold_indices = y_pred_sorted_indices[
+                samples_at_target_threshold_mask
+                & non_target_samples_mask  # Filter for samples at target threshold  # Filter for positive samples
+            ]
+            num_samples = (
+                non_target_samples_at_target_threshold_indices.shape[0]
+                * sampled_fraction
+            )
+
+            num_samples = int(round(num_samples, 0))
+
+            if num_samples:
+                extra_neg_preds_indices = rng.choice(
+                    non_target_samples_at_target_threshold_indices,
+                    size=num_samples,
+                    replace=False,
+                )
+                y_pred_binary[extra_neg_preds_indices] = 0
 
     # Sanity check: the number of positive_preds_budget should now be exactly fulfilled
     assert np.sum(y_pred_binary[target_samples_indices]) == positive_preds_budget
 
     return y_pred_binary
 
 
@@ -158,15 +183,15 @@
         equalize_tpr: Optional[bool] = False,
         equalize_fpr: Optional[bool] = False,
         false_negative_cost: Optional[float] = 1,
         false_positive_cost: Optional[float] = 1,
         # allowed_tpr_gap: Optional[float] = 0.0,
         # allowed_fpr_gap: Optional[float] = 0.0,
         random_seed: Optional[int] = 42,
-    ) -> np.ndarray:
+) -> np.ndarray:
     """Discretizes the given score predictions into binary labels, according
     to the provided fairness criteria - equalize TPR, FPR, or both.
 
     Parameters
     ----------
     y_true : np.ndarray
         The true binary labels.
@@ -191,47 +216,51 @@
         (e.g.,  in the case of equal odds - equalizing both TPR and FPR).
 
     Returns
     -------
     np.ndarray
         The binarized predictions.
     """
-    assert equalize_fpr or equalize_tpr, \
-        "Must target either equal FPR or equal TPR or both, got neither."
-    
+    assert (
+        equalize_fpr or equalize_tpr
+    ), "Must target either equal FPR or equal TPR or both, got neither."
+
     # The threshold is computed from the ratio of FPs and FNs,
     # and assumes the underlying classifier is approximately calibrated
     # i.e., a threshold of t=0.5 indicates equal likelihood of paying the FP
     # cost or the FN cost
     threshold = false_positive_cost / (false_positive_cost + false_negative_cost)
 
     # TODO: remove this discretization in the future???
     n_score_bins = 200
     y_pred_scores = (y_pred_scores * n_score_bins).astype(int) / n_score_bins
     # for now it makes things easier if we just use a fixed number of thresholds
     # (this, however, will create many ties...)
     raise NotImplementedError()
-    import ipdb; ipdb.set_trace()
+    import ipdb
+
+    ipdb.set_trace()
 
     # Construct CDF and Performance arrays to compute fairness criteria
     unique_groups = np.unique(sensitive_attribute)
 
-    data = pd.DataFrame({
-        'score': y_pred_scores,
-        'label': y_true,
-        **{
-            f'group={group}': (sensitive_attribute == group).astype(int)
-            for group in unique_groups
-        },
-    })
+    data = pd.DataFrame(
+        {
+            "score": y_pred_scores,
+            "label": y_true,
+            **{
+                f"group={group}": (sensitive_attribute == group).astype(int)
+                for group in unique_groups
+            },
+        }
+    )
 
-    cdfs = data.groupby(['score', 'label']).cumsum()
+    cdfs = data.groupby(["score", "label"]).cumsum()
     # TODO: construct CDF array and Performance array (perhaps separately, this is getting tricky...)
 
-
     # # Unique groups
     # unique_groups = np.unique(sensitive_attribute)
 
     # # Thresholds support (all available unique thresholds)
     # unique_thresholds = np.unique(y_pred_scores)
 
     # # Count number of samples per group
@@ -240,55 +269,50 @@
     # data = defaultdict(lambda: {''})
     # for idx in y_pred_sorted_indices:
     #     score = y_pred_scores[idx]
     #     data.append((score, {
     #         ''
     #     }))
 
-
-
-
     # Generate DataFrames for CDF, Performance, and Total per group, where:
     # > cdf[group_][score_] = proportion of members of group_ with score below score_
     # TODO
     cdfs = ...
 
     # > perf[group_][score_] = proportion of members of that group_ and score_ that have a positive label
-    performance = ...   # TODO...
+    performance = ...  # TODO...
 
     # > totals[group_] = total number of group_ members
     totals = {}
 
     # Construct CriteriaData object to compute fairness criteria and thresholds
     data = CriteriaData(cdfs, performance, totals)
 
     # > groupwise_thresholds[group_] = threshold used for group_
     # TODO: check if it is 1{f(X) >= threshold} or 1{f(X) > threshold}
     groupwise_thresholds: dict
-    if equalize_tpr and equalize_fpr:   # Equal odds
-
+    if equalize_tpr and equalize_fpr:  # Equal odds
         # TODO
         # - use data.two_sided_optimum to get optimal Equal Odds point (under all ROC curves)
         # - somehow binarize predictions such that this is met (with randomization for a portion of predictions)
 
         rng = np.random.RandomState(random_seed)
         pass
 
-    elif equalize_tpr:                  # Equal opportunity among Y=1
+    elif equalize_tpr:  # Equal opportunity among Y=1
         groupwise_thresholds = data.opportunity_cutoffs(target_rate=threshold)
-    
-    elif equalize_fpr:                  # Equal opportunity among Y=0
+
+    elif equalize_fpr:  # Equal opportunity among Y=0
         raise NotImplementedError(
-            "Equalizing TNR or FPR is not yet implemented as a fairness "
-            "criterion."
+            "Equalizing TNR or FPR is not yet implemented as a fairness " "criterion."
         )
-    
+
     # Binarize predictions with the given thresholds
     y_pred_binary = np.zeros_like(y_true)
 
     for group_ in unique_groups:
         group_mask = sensitive_attribute == group_
         y_pred_binary[group_mask] = (
             y_pred_scores[group_mask] >= groupwise_thresholds[group_]
         ).astype(int)
-    
+
     return y_pred_binary
```

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/evaluation.py` & `hyperparameter-tuning-0.2.0/src/hpt/evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A set of functions to evaluate predictions on common performance
 and fairness metrics, possibly at a specified FPR or FNR target.
 """
 
 from typing import Optional
 
 import numpy as np
-from sklearn.metrics import confusion_matrix
+from sklearn.metrics import confusion_matrix, log_loss, mean_squared_error
 
 from .binarize import compute_binary_predictions
 
 
 def safe_division(a: float, b: float):
     return 0 if b == 0 else a / b
 
@@ -47,19 +47,24 @@
     
     # Accuracy
     results["accuracy"] = (tp + tn) / total
 
     # True Positive Rate (Recall)
     results["tpr"] = safe_division(tp, label_pos)
 
+    # False Negative Rate (1 - TPR)
+    results["fnr"] = safe_division(fn, label_pos)
+    assert results["tpr"] + results["fnr"] == 1
+
     # False Positive Rate
     results["fpr"] = safe_division(fp, label_neg)
 
     # True Negative Rate
-    # results["tnr"] = tn / label_neg
+    results["tnr"] = safe_division(tn, label_neg)
+    assert results["tnr"] + results["fpr"] == 1
 
     # Precision
     results["precision"] = safe_division(tp, pred_pos)
 
     # Positive Prediction Rate
     results["ppr"] = safe_division(pred_pos, total)
 
@@ -144,20 +149,22 @@
 
         # Metrics' absolute difference
         diff_name = f"{metric_name}_diff"
         results[diff_name] = max(curr_metric_results) - min(curr_metric_results)
 
     
     # Equal odds: maximum constraint violation for TPR and FPR equality
+    # i.e., the smallest ratio
     results["equal_odds_ratio"] = min(
         results["tpr_ratio"],           # why not FNR ratio here?
         results["fpr_ratio"],           # why not TNR ratio here?
     )
 
-    results["equal_odds_diff"] = min(
+    # or the largest absolute difference
+    results["equal_odds_diff"] = max(
         results["tpr_diff"],            # same as FNR diff
         results["fpr_diff"],            # same as TNR diff
     )
 
     # Optionally, return group-wise metrics as well
     if return_groupwise_metrics:
         results.update(groupwise_metrics)
@@ -165,28 +172,32 @@
     return results
 
 
 def evaluate_predictions(
         y_true: np.ndarray,
         y_pred_scores: np.ndarray,
         sensitive_attribute: Optional[np.ndarray] = None,
+        return_groupwise_metrics: bool = False,
         **threshold_target,
     ) -> dict:
     """Evaluates the given predictions on both performance and fairness
     metrics (if `sensitive_attribute` is provided).
 
     Parameters
     ----------
     y_true : np.ndarray
         The true labels.
     y_pred_scores : np.ndarray
         The predicted scores.
-    sensitive_attribute : np.ndarray
-        The sensitive attribute - which protected group each sample belongs
-        to.
+    sensitive_attribute : np.ndarray, optional
+        The sensitive attribute - which protected group each sample belongs to.
+        If not provided, will not compute fairness metrics.
+    return_groupwise_metrics : bool
+        Whether to return groupwise performance metrics (requires providing
+        `sensitive_attribute`).
 
     Returns
     -------
     dict
         A dictionary of (key, value) -> (metric_name, metric_value).
     """
 
@@ -194,15 +205,21 @@
     y_pred_binary = compute_binary_predictions(
         y_true, y_pred_scores, **threshold_target,
     )
 
     # Compute global performance metrics
     results = evaluate_performance(y_true, y_pred_binary)
 
+    # Compute loss metrics
+    results.update({
+        "squared_loss": mean_squared_error(y_true, y_pred_scores),
+        "log_loss": log_loss(y_true, y_pred_scores),
+    })
+
     # (Optionally) Compute fairness metrics
     if sensitive_attribute is not None:
         results.update(evaluate_fairness(
             y_true, y_pred_binary, sensitive_attribute,
-            return_groupwise_metrics=False,
+            return_groupwise_metrics=return_groupwise_metrics,
         ))
 
     return results
```

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/suggest.py` & `hyperparameter-tuning-0.2.0/src/hpt/suggest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 """Module to suggest and sample hyperparameters from distributions defined in
 a hyperparameter space.
 """
 import logging
+from pathlib import Path
 from copy import deepcopy
 from typing import Iterable, Union
 
 from optuna.trial import BaseTrial
 
 from .utils.trial import RandomValueTrial
 from .utils.load_yaml import load_hyperparameter_space
 
 
 def suggest_random_hyperparams(
-        hyperparameter_space: Union[dict, str],
+        hyperparameter_space: Union[dict, str, Path],
         seed: int,
     ) -> dict:
     """Suggests a random set of hyperparameters from the given hyperparameter space.
     
     NOTE: this is a deterministic function of the given seed number; the seed must
     itself be randomly drawn for each function call if you want to get a random sample
     of hyperparameter configurations.
 
     Parameters
     ----------
-    hyperparameter_space : Union[dict, str]
+    hyperparameter_space : Union[dict, str, Path]
         A dict or a path to a YAML file representing a hyperparameter space.
-        Please pre-load the YAML file and provide it as a dict here, as otherwise
-        this call will be unnecessarilly inefficient.
+        If a path is provided, this function will load the hyperparameter space
+        from the given path. Else, if a dict is provided, it will assume the 
+        hyperparameter space has already been loaded (this prevents 
+        unnecessarily re-loading the same file multiple times from disk.)
     seed : int
         The random seed used to generate the random set of hyperparameters.
         This function is a deterministic function of the seed provided.
 
     Returns
     -------
     dict
         A set of hyperparameters that was randomly drawn from the given
         hyperparameter space.
     """
 
     # If provided a path to a YAML file instead of a pre-loaded hyperparameter space
-    if isinstance(hyperparameter_space, str):
+    if isinstance(hyperparameter_space, (str, Path)):
         # Load (and validate) the given hyperparameter space
         # NOTE: you should really pre-load the YAML, doing it here will be inefficient
         hyperparameter_space = load_hyperparameter_space(hyperparameter_space)
 
     return suggest_callable_hyperparams(
         RandomValueTrial(seed=seed),
         hyperparameter_space,
```

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/thresholding_evaluation.py` & `hyperparameter-tuning-0.2.0/src/hpt/thresholding_evaluation.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/tuner.py` & `hyperparameter-tuning-0.2.0/src/hpt/tuner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """A simple wrapper for optuna hyperparameter tuners.
 """
 
 import re
+import time
 import logging
 import dataclasses
 from pathlib import Path
 from functools import partial
 from inspect import signature
 from typing import Callable, Optional, Union, List
 
@@ -31,14 +32,15 @@
     class TrialResults:
         id: int
         hyperparameters: dict
         validation_results: dict
         test_results: dict = None
         train_results: dict = None
         model: BaseLearner = None
+        fit_time: float = None
         algorithm: str = None
 
         def __post_init__(self):
             # Extract algorithm name from hyperparameters
             match = re.match(
                 r'^(?:.+[.])?(?P<algorithm>\w+)$',
                 self.hyperparameters['classpath'])
@@ -106,22 +108,36 @@
 
             model.fit(X_train, y_train)
 
         return model
     
     @property
     def results(self):
+        # By default, returns validation results
+        return self.get_results('validation')
+
+    def get_results(self, type_: str = 'validation'):
+        _get_results_helper: callable
+        if type_ in ('val', 'validation'):
+            _get_results_helper = lambda r: r.validation_results
+        elif type_ in ('test', 'testing'):
+            _get_results_helper = lambda r: r.test_results
+        elif type_ in ('train', 'training'):
+            _get_results_helper = lambda r: r.train_results
+        else:
+            raise ValueError(f"Value of type_='{type_}' is invalid.")
+
         return pd.DataFrame(
             data=[{
                 'algorithm': r.algorithm,
-                **r.validation_results,
+                **_get_results_helper(r),
             } for r in self._models_results],
             index=[r.id for r in self._models_results],
         )
-    
+
     @property
     def all_results(self):
         return self._models_results
     
     @property
     def best_trial(self):
         results = self.results.copy()
@@ -150,30 +166,40 @@
             s_val = None,
             X_test = None,
             y_test = None,
             s_test = None,
             other_eval_metric: Optional[str] = None,
             alpha: Optional[float] = 0.50,
             eval_func: Optional[Callable[..., dict]] = None,
+            return_groupwise_metrics: bool = False,
             **threshold_target,
         ):
         self.X_train, self.y_train, self.s_train = (X_train, y_train, s_train)
         self.X_val, self.y_val, self.s_val = (X_val, y_val, s_val)
         self.X_test, self.y_test, self.s_test = (X_test, y_test, s_test)
 
         self.hyperparameter_space = hyperparameter_space
         if isinstance(hyperparameter_space, (str, Path)):
             self.hyperparameter_space = load_hyperparameter_space(str(hyperparameter_space))
 
         self.eval_metric = eval_metric
         self.other_eval_metric = other_eval_metric
         self.alpha = alpha
         assert alpha is None or (0 <= alpha <= 1)
-        self.eval_func = eval_func or evaluate_predictions
-        self.eval_func = partial(self.eval_func, **threshold_target)
+
+        # Running custom evaluation function
+        if eval_func is not None:
+            self.eval_func = eval_func
+
+        # Using the default evaluation function with the provided threshold target
+        else:
+            self.eval_func = partial(
+                evaluate_predictions,
+                return_groupwise_metrics=return_groupwise_metrics,
+                **threshold_target)
 
         # Store all results in a list as models are trained
         self._models_results: List[ObjectiveFunction.TrialResults] = list()
     
     def evaluate_model(
             self,
             model: BaseLearner,
@@ -200,33 +226,38 @@
         # Sample hyperparameters
         hyperparams = suggest_callable_hyperparams(trial, self.hyperparameter_space)
 
         # Construct model
         model = self.instantiate_model(**hyperparams)
 
         # Train model
+        start_time = time.process_time()    # TODO: log wall-clock time as well
         self.fit_model(model, self.X_train, self.y_train, self.s_train)
+        elapsed_process_time = time.process_time() - start_time
+        logging.info(f"Trial {trial.number} took {elapsed_process_time}s to train.")
 
         # Evaluate model on validation data
         val_results = self.evaluate_model(
             model=model, X=self.X_val, y=self.y_val, s=self.s_val)
         
         # Optionally, evaluate on test data as well (just to save results)
+        test_results = None
         if self.X_test is not None and self.y_test is not None:
             test_results = self.evaluate_model(
                 model=model, X=self.X_test, y=self.y_test, s=self.s_test)
 
         # Store trial's results
         self._models_results.append(
             self.TrialResults(
                 id=trial.number,
                 hyperparameters=hyperparams,
                 validation_results=val_results,
                 test_results=test_results,
                 model=model,
+                fit_time=elapsed_process_time,
             ))
 
         # Return scalarized evaluation metric
         if self.other_eval_metric:
             assert self.alpha is not None
             return (
                 val_results[self.eval_metric] * self.alpha + 
@@ -282,16 +313,16 @@
         best_trial_results = self.best_trial.validation_results
         sns.scatterplot(
             x=[best_trial_results[x_axis]], y=[best_trial_results[y_axis]],
             color='red', marker='*', s=100,
             label='best model',
         )
 
-        plt.xlabel(f"{x_axis.title()})")
-        plt.ylabel(f"{y_axis.title()})")
+        plt.xlabel(f"{x_axis.title()}")
+        plt.ylabel(f"{y_axis.title()}")
 
         plt.title("Hyperparameter Search")
 
         if pyplot_show:
             plt.show()
```

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/utils/classpath.py` & `hyperparameter-tuning-0.2.0/src/hpt/utils/classpath.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/utils/dict.py` & `hyperparameter-tuning-0.2.0/src/hpt/utils/dict.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/utils/fairness_criteria.py` & `hyperparameter-tuning-0.2.0/src/hpt/utils/fairness_criteria.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/utils/load_yaml.py` & `hyperparameter-tuning-0.2.0/src/hpt/utils/load_yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Utils specific to the tuners module.
 
 Author: @sgpjesus
 """
+import logging
 from inspect import signature
 from numbers import Number
 from typing import Union
+from pathlib import Path
 
 import yaml
 from schema import And
 from schema import Optional as Optional_
 from schema import Or, Schema
 
 from .classpath import import_object
@@ -126,15 +128,15 @@
                 )
             },
         },
     }
 )
 
 
-def load_hyperparameter_space(path_or_dict: Union[str, dict]) -> dict:
+def load_hyperparameter_space(path_or_dict: Union[str, Path, dict]) -> dict:
     """Loads the hyperparameter space encoded as a YAML in the given path.
     If given a dict, space is already loaded and this function will return the
     same object.
 
     Parameters
     ----------
     path_or_dict : Union[str, dict]
@@ -142,25 +144,34 @@
         hyperparameter space following the expected structure.
 
     Returns
     -------
     The loaded hyperparameter space.
     """
     # Read hyperparameter space from the YAML file (if given)
-    if isinstance(path_or_dict, str):
+    if isinstance(path_or_dict, (str, Path)):
+        path_obj = Path(path_or_dict).resolve()
+        logging.debug(
+            f"Loading hyperparameter space from the following YAML file: "
+            f"{path_obj}")
+
         try:
-            with open(path_or_dict, "r") as f_in:
+            with open(str(path_obj), "r") as f_in:
                 hyperparameter_space = yaml.safe_load(f_in)
+
         except yaml.YAMLError as err:
             raise ValueError(f"{err}. Did you pass a valid YAML file ?") from err
-    # Else, assume the given dictionary describes hyperparameter space
+
+    # Else, assume the given dictionary describes a hyperparameter space
     elif isinstance(path_or_dict, dict):
         hyperparameter_space = path_or_dict
+
     else:
         raise ValueError(
             "Invalid value for `learner_hyperparams`. "
             "Must be either a path to a YAML file or a dict following the same structure."
         )
+
     # validate the configuration file
     HYPERPARAMETER_SPACE_SCHEMA.validate(hyperparameter_space)
 
     return hyperparameter_space
```

### Comparing `hyperparameter-tuning-0.1.9/src/hpt/utils/trial.py` & `hyperparameter-tuning-0.2.0/src/hpt/utils/trial.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/PKG-INFO` & `hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameter-tuning
-Version: 0.1.9
+Version: 0.2.0
 Summary: A minimal framework for running hyperparameter tuning
 Home-page: https://github.com/AndreFCruz/hpt
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,hyperparameter,tuning,fairness
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hyperparameter-tuning-0.1.9/src/hyperparameter_tuning.egg-info/SOURCES.txt` & `hyperparameter-tuning-0.2.0/src/hyperparameter_tuning.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 MANIFEST.in
 README.md
 setup.py
 requirements/main.txt
 requirements/plotting.txt
 requirements/test.txt
 src/hpt/__init__.py
+src/hpt/_version.py
 src/hpt/binarize.py
 src/hpt/evaluation.py
 src/hpt/suggest.py
 src/hpt/thresholding_evaluation.py
 src/hpt/tuner.py
-src/hpt/version.py
 src/hpt/utils/__init__.py
 src/hpt/utils/api.py
 src/hpt/utils/classpath.py
 src/hpt/utils/dict.py
 src/hpt/utils/fairness_criteria.py
 src/hpt/utils/load_yaml.py
 src/hpt/utils/trial.py
```

