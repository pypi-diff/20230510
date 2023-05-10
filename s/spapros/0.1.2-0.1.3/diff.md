# Comparing `tmp/spapros-0.1.2.tar.gz` & `tmp/spapros-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spapros-0.1.2.tar", max compression
+gzip compressed data, was "spapros-0.1.3.tar", max compression
```

## Comparing `spapros-0.1.2.tar` & `spapros-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1070 2023-02-27 20:47:25.046987 spapros-0.1.2/LICENSE
--rw-r--r--   0        0        0     3096 2023-02-27 20:47:25.046987 spapros-0.1.2/README.rst
--rw-r--r--   0        0        0     2541 2023-02-27 20:47:25.210990 spapros-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      278 2023-02-27 20:47:25.210990 spapros-0.1.2/spapros/__init__.py
--rw-r--r--   0        0        0     4756 2023-02-27 20:47:25.210990 spapros-0.1.2/spapros/__main__.py
--rw-r--r--   0        0        0        0 2023-02-27 20:47:25.210990 spapros-0.1.2/spapros/cli/__init__.py
--rw-r--r--   0        0        0     2976 2023-02-27 20:47:25.210990 spapros-0.1.2/spapros/cli/questionary.py
--rw-r--r--   0        0        0      410 2023-02-27 20:47:25.210990 spapros-0.1.2/spapros/evaluation/__init__.py
--rw-r--r--   0        0        0    92690 2023-02-27 20:47:25.210990 spapros-0.1.2/spapros/evaluation/evaluation.py
--rw-r--r--   0        0        0    13780 2023-02-27 20:47:25.210990 spapros-0.1.2/spapros/evaluation/evaluation_pipeline.py
--rw-r--r--   0        0        0    51359 2023-02-27 20:47:25.210990 spapros-0.1.2/spapros/evaluation/metrics.py
--rw-r--r--   0        0        0      912 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/plotting/__init__.py
--rw-r--r--   0        0        0    26837 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/plotting/_masked_dotplot.py
--rw-r--r--   0        0        0    61317 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/plotting/plot.py
--rw-r--r--   0        0        0        0 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/py.typed
--rw-r--r--   0        0        0      393 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/selection/__init__.py
--rw-r--r--   0        0        0     8782 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/selection/selection.py
--rw-r--r--   0        0        0    69216 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/selection/selection_methods.py
--rw-r--r--   0        0        0    99442 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/selection/selection_procedure.py
--rw-r--r--   0        0        0      371 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/util/__init__.py
--rw-r--r--   0        0        0     6874 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/util/mp_util.py
--rw-r--r--   0        0        0    28289 2023-02-27 20:47:25.214990 spapros-0.1.2/spapros/util/util.py
--rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 spapros-0.1.2/setup.py
--rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 spapros-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-10 18:28:58.030299 spapros-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3096 2023-05-10 18:28:58.034299 spapros-0.1.3/README.rst
+-rw-r--r--   0        0        0     2541 2023-05-10 18:28:58.234310 spapros-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      278 2023-05-10 18:28:58.234310 spapros-0.1.3/spapros/__init__.py
+-rw-r--r--   0        0        0     4756 2023-05-10 18:28:58.234310 spapros-0.1.3/spapros/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:28:58.234310 spapros-0.1.3/spapros/cli/__init__.py
+-rw-r--r--   0        0        0     2976 2023-05-10 18:28:58.234310 spapros-0.1.3/spapros/cli/questionary.py
+-rw-r--r--   0        0        0      410 2023-05-10 18:28:58.234310 spapros-0.1.3/spapros/evaluation/__init__.py
+-rw-r--r--   0        0        0    92904 2023-05-10 18:28:58.238310 spapros-0.1.3/spapros/evaluation/evaluation.py
+-rw-r--r--   0        0        0    13780 2023-05-10 18:28:58.238310 spapros-0.1.3/spapros/evaluation/evaluation_pipeline.py
+-rw-r--r--   0        0        0    51312 2023-05-10 18:28:58.238310 spapros-0.1.3/spapros/evaluation/metrics.py
+-rw-r--r--   0        0        0      912 2023-05-10 18:28:58.238310 spapros-0.1.3/spapros/plotting/__init__.py
+-rw-r--r--   0        0        0    26837 2023-05-10 18:28:58.238310 spapros-0.1.3/spapros/plotting/_masked_dotplot.py
+-rw-r--r--   0        0        0    61317 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/plotting/plot.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/py.typed
+-rw-r--r--   0        0        0      393 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/selection/__init__.py
+-rw-r--r--   0        0        0     8782 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/selection/selection.py
+-rw-r--r--   0        0        0    69216 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/selection/selection_methods.py
+-rw-r--r--   0        0        0    99442 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/selection/selection_procedure.py
+-rw-r--r--   0        0        0      371 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/util/__init__.py
+-rw-r--r--   0        0        0     6874 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/util/mp_util.py
+-rw-r--r--   0        0        0    28289 2023-05-10 18:28:58.242310 spapros-0.1.3/spapros/util/util.py
+-rw-r--r--   0        0        0     4704 1970-01-01 00:00:00.000000 spapros-0.1.3/PKG-INFO
```

### Comparing `spapros-0.1.2/LICENSE` & `spapros-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/README.rst` & `spapros-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/pyproject.toml` & `spapros-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spapros"
-version = "0.1.2"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.1.3"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Probe set selection for targeted spatial transcriptomics."
 authors = ["Lukas Heumos <lukas.heumos@posteo.net>", "Louis Kümmerle <louis.kuemmerle@helmholtz-muenchen.de>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/theislab/spapros"
 repository = "https://github.com/theislab/spapros"
 documentation = "https://spapros.readthedocs.io"
```

### Comparing `spapros-0.1.2/spapros/__main__.py` & `spapros-0.1.3/spapros/__main__.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/cli/questionary.py` & `spapros-0.1.3/spapros/cli/questionary.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/evaluation/evaluation.py` & `spapros-0.1.3/spapros/evaluation/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import gc
 import pickle
 import warnings
 from enum import Enum
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import Iterable
@@ -1908,14 +1909,19 @@
             extractor=pool_train_ct_tree_helper,
             show_progress_bar=False,  # verbose, # False
         )(X_train=X_train, y_train=y_train, seed=seeds[i], max_depth=max_depth, masks=masks)
         for ct in celltypes:
             ct_trees[ct].append(ct_trees_i[ct])
         if progress and verbose:
             progress.advance(forest_task)
+        # garbage collection
+        del X_train
+        del y_train
+        del cts_train
+        gc.collect()
     # Get feature importances
     importances = {
         ct: pd.DataFrame(index=a.var.index, columns=[str(i) for i in range(n_trees)], dtype="float64")
         for ct in celltypes
     }
     for i in range(n_trees):
         for ct in celltypes:
@@ -1935,14 +1941,19 @@
         ref_celltypes=ref_celltypes,
         ct_trees=ct_trees,
         X_test=X_test,
         y_test=y_test,
         cts_test=cts_test,
         masks=masks_test,
     )
+    #garbage collection
+    del X_test
+    del y_test
+    del cts_test
+    gc.collect()    
 
     # Sort results
     if sort_by_tree_performance:
         for ct in summary_metric.index:
             if (masks_test is None) or (np.sum(masks_test[ct]) > 0):
                 order = summary_metric.loc[ct].sort_values(ascending=False).index.values.copy()
                 order_int = [summary_metric.loc[ct].index.get_loc(idx) for idx in order]
```

### Comparing `spapros-0.1.2/spapros/evaluation/evaluation_pipeline.py` & `spapros-0.1.3/spapros/evaluation/evaluation_pipeline.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/evaluation/metrics.py` & `spapros-0.1.3/spapros/evaluation/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -996,26 +996,25 @@
             train_x, train_y, test_x, test_y = X[train_ix], y[train_ix], X[test_ix], y[test_ix]
             sample_weight_train = compute_sample_weight("balanced", train_y)
             sample_weight_test = compute_sample_weight("balanced", test_y)
             # Fit the classifier
             n_classes = len(np.unique(train_y))
             clf = XGBClassifier(
                 max_depth=max_depth,
-                num_class=n_classes,
+                num_class=n_classes if n_classes > 2 else None,
                 n_estimators=250,
                 objective="multi:softmax" if n_classes > 2 else "binary:logistic",
                 early_stopping_rounds=5,
-                eval_metric="mlogloss",
+                eval_metric="mlogloss" if n_classes > 2 else "logloss",
                 learning_rate=lr,
                 colsample_bytree=colsample_bytree,
                 min_child_weight=min_child_weight,
                 gamma=gamma,
                 booster="gbtree",  # TODO: compare with 'dart',rate_drop= 0.1
                 random_state=seed,
-                use_label_encoder=False,  # To get rid of deprecation warning we convert labels into ints
                 n_jobs=n_jobs,
             )
             clf.fit(
                 train_x,
                 train_y,
                 sample_weight=sample_weight_train,
                 eval_set=[(test_x, test_y)],
```

### Comparing `spapros-0.1.2/spapros/plotting/__init__.py` & `spapros-0.1.3/spapros/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/plotting/_masked_dotplot.py` & `spapros-0.1.3/spapros/plotting/_masked_dotplot.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/plotting/plot.py` & `spapros-0.1.3/spapros/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/selection/selection.py` & `spapros-0.1.3/spapros/selection/selection.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/selection/selection_methods.py` & `spapros-0.1.3/spapros/selection/selection_methods.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/selection/selection_procedure.py` & `spapros-0.1.3/spapros/selection/selection_procedure.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/util/mp_util.py` & `spapros-0.1.3/spapros/util/mp_util.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/spapros/util/util.py` & `spapros-0.1.3/spapros/util/util.py`

 * *Files identical despite different names*

### Comparing `spapros-0.1.2/PKG-INFO` & `spapros-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spapros
-Version: 0.1.2
+Version: 0.1.3
 Summary: Probe set selection for targeted spatial transcriptomics.
 Home-page: https://github.com/theislab/spapros
 License: MIT
 Author: Lukas Heumos
 Author-email: lukas.heumos@posteo.net
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
```

