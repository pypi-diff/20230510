# Comparing `tmp/equal-odds-0.0.5.tar.gz` & `tmp/equal-odds-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equal-odds-0.0.5.tar", last modified: Tue May  9 09:11:31 2023, max compression
+gzip compressed data, was "equal-odds-0.0.6.tar", last modified: Wed May 10 15:07:58 2023, max compression
```

## Comparing `equal-odds-0.0.5.tar` & `equal-odds-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:11:31.006971 equal-odds-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-09 09:11:19.000000 equal-odds-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 09:11:19.000000 equal-odds-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-09 09:11:31.006971 equal-odds-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-09 09:11:19.000000 equal-odds-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:11:31.002971 equal-odds-0.0.5/equal_odds/
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-05-09 09:11:19.000000 equal-odds-0.0.5/equal_odds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-09 09:11:19.000000 equal-odds-0.0.5/equal_odds/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-05-09 09:11:19.000000 equal-odds-0.0.5/equal_odds/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-05-09 09:11:19.000000 equal-odds-0.0.5/equal_odds/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-05-09 09:11:19.000000 equal-odds-0.0.5/equal_odds/equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-09 09:11:19.000000 equal-odds-0.0.5/equal_odds/roc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:11:31.002971 equal-odds-0.0.5/equal_odds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-09 09:11:30.000000 equal-odds-0.0.5/equal_odds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 09:11:30.000000 equal-odds-0.0.5/equal_odds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:11:30.000000 equal-odds-0.0.5/equal_odds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 09:11:30.000000 equal-odds-0.0.5/equal_odds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 09:11:30.000000 equal-odds-0.0.5/equal_odds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:11:31.006971 equal-odds-0.0.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 09:11:19.000000 equal-odds-0.0.5/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 09:11:19.000000 equal-odds-0.0.5/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 09:11:19.000000 equal-odds-0.0.5/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:11:31.006971 equal-odds-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-09 09:11:19.000000 equal-odds-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:07:58.629537 equal-odds-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 15:07:45.000000 equal-odds-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 15:07:45.000000 equal-odds-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-10 15:07:58.629537 equal-odds-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-10 15:07:45.000000 equal-odds-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:07:58.625537 equal-odds-0.0.6/equal_odds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/equal_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-10 15:07:45.000000 equal-odds-0.0.6/equal_odds/roc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:07:58.625537 equal-odds-0.0.6/equal_odds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 15:07:58.000000 equal-odds-0.0.6/equal_odds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:07:58.629537 equal-odds-0.0.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 15:07:45.000000 equal-odds-0.0.6/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 15:07:45.000000 equal-odds-0.0.6/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 15:07:45.000000 equal-odds-0.0.6/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:07:58.629537 equal-odds-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-10 15:07:45.000000 equal-odds-0.0.6/setup.py
```

### Comparing `equal-odds-0.0.5/LICENSE` & `equal-odds-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.5/PKG-INFO` & `equal-odds-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equal-odds
-Version: 0.0.5
+Version: 0.0.6
 Summary: _PACKAGE UNDER CONSTRUCTION_
 Home-page: https://github.com/AndreFCruz/equal-odds
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `equal-odds-0.0.5/README.md` & `equal-odds-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.5/equal_odds/classifiers.py` & `equal-odds-0.0.6/equal_odds/classifiers.py`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.5/equal_odds/cvxpy_utils.py` & `equal-odds-0.0.6/equal_odds/cvxpy_utils.py`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.5/equal_odds/equal_odds.py` & `equal-odds-0.0.6/equal_odds/equal_odds.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,27 +174,29 @@
             f"group={groupA} (p={self.groupwise_roc_points[groupA]}) and "
             f"group={groupB} (p={self.groupwise_roc_points[groupB]});"
         )
 
         return max_violation
 
 
-    def fit(self, X: np.ndarray, y: np.ndarray, group: np.ndarray):
+    def fit(self, X: np.ndarray, y: np.ndarray, group: np.ndarray, y_scores: np.ndarray = None):
         """Fit this predictor to achieve the (possibly relaxed) equal odds 
         constraint on the provided data.
 
         Parameters
         ----------
         X : np.ndarray
             The input features.
         y : np.ndarray
             The input labels.
         group : np.ndarray
             The group membership of each sample.
             Assumes groups are numbered [0, 1, ..., num_groups-1].
+        y_scores : np.ndarray, optional
+            The pre-computed model predictions on this data.
         
         Returns
         -------
         callable
             Returns self.
         """
 
@@ -220,15 +222,16 @@
         assert np.sum(group_sizes_label_neg) + np.sum(group_sizes_label_pos) == len(y)
 
         # Convert to relative sizes
         group_sizes_label_neg = group_sizes_label_neg.astype(float) / np.sum(group_sizes_label_neg)
         group_sizes_label_pos = group_sizes_label_pos.astype(float) / np.sum(group_sizes_label_pos)
 
         # Compute group-wise ROC curves
-        y_scores = self.predictor(X)
+        if y_scores is None:
+            y_scores = self.predictor(X)
 
         self._all_roc_data = dict()
         for g in unique_groups:
             group_filter = group == g
 
             roc_curve_data = roc_curve(
                 y[group_filter],
```

### Comparing `equal-odds-0.0.5/equal_odds/roc_utils.py` & `equal-odds-0.0.6/equal_odds/roc_utils.py`

 * *Files identical despite different names*

### Comparing `equal-odds-0.0.5/equal_odds.egg-info/PKG-INFO` & `equal-odds-0.0.6/equal_odds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: equal-odds
-Version: 0.0.5
+Version: 0.0.6
 Summary: _PACKAGE UNDER CONSTRUCTION_
 Home-page: https://github.com/AndreFCruz/equal-odds
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `equal-odds-0.0.5/setup.py` & `equal-odds-0.0.6/setup.py`

 * *Files identical despite different names*

