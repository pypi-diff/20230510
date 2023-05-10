# Comparing `tmp/cefeste-1.1.0.tar.gz` & `tmp/cefeste-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.1.0.tar", last modified: Fri May  5 08:29:51 2023, max compression
+gzip compressed data, was "cefeste-1.1.1.tar", last modified: Tue May  9 13:07:09 2023, max compression
```

## Comparing `cefeste-1.1.0.tar` & `cefeste-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.014606 cefeste-1.1.0/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.0/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-05-05 08:29:51.010606 cefeste-1.1.0/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1558 2023-05-05 08:25:33.000000 cefeste-1.1.0/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-05-05 08:25:52.000000 cefeste-1.1.0/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-05 08:29:51.014606 cefeste-1.1.0/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      997 2023-05-05 08:25:52.000000 cefeste-1.1.0/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.002606 cefeste-1.1.0/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.006605 cefeste-1.1.0/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.010606 cefeste-1.1.0/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    13908 2023-05-05 08:25:52.000000 cefeste-1.1.0/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25190 2023-05-05 08:25:52.000000 cefeste-1.1.0/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.010606 cefeste-1.1.0/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.010606 cefeste-1.1.0/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-05-05 08:25:33.000000 cefeste-1.1.0/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-05 08:25:52.000000 cefeste-1.1.0/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-05 08:29:51.010606 cefeste-1.1.0/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-05-05 08:29:50.000000 cefeste-1.1.0/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-05 08:29:51.000000 cefeste-1.1.0/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-05 08:29:50.000000 cefeste-1.1.0/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      129 2023-05-05 08:29:50.000000 cefeste-1.1.0/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-05 08:29:50.000000 cefeste-1.1.0/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.057908 cefeste-1.1.1/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.1/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-05-09 13:07:09.057908 cefeste-1.1.1/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1558 2023-05-05 08:25:33.000000 cefeste-1.1.1/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-05-09 12:58:02.000000 cefeste-1.1.1/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-09 13:07:09.057908 cefeste-1.1.1/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      997 2023-05-09 12:58:02.000000 cefeste-1.1.1/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.049908 cefeste-1.1.1/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.053908 cefeste-1.1.1/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.053908 cefeste-1.1.1/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15368 2023-05-09 12:58:02.000000 cefeste-1.1.1/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25816 2023-05-09 13:05:39.000000 cefeste-1.1.1/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.057908 cefeste-1.1.1/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.057908 cefeste-1.1.1/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-05 08:25:52.000000 cefeste-1.1.1/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.053908 cefeste-1.1.1/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      129 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.1.0/LICENCE` & `cefeste-1.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/PKG-INFO` & `cefeste-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.0
+Version: 1.1.1
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cefeste-1.1.0/README.md` & `cefeste-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/pyproject.toml` & `cefeste-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="DAT - Mattia Centurelli", email="mcenturelli@credem.it" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cefeste-1.1.0/setup.py` & `cefeste-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.1.0",
+    version="1.1.1",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT/Mattia Centurelli",
     author_email="mcenturelli@credem.it",
     url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `cefeste-1.1.0/src/cefeste/__init__.py` & `cefeste-1.1.1/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/src/cefeste/elimination/__init__.py` & `cefeste-1.1.1/src/cefeste/elimination/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -221,30 +221,34 @@
         if self.report is not None:
             self.report.plot(
                 x="n_feat", y=["train_score", "valid_score"], xlim=(max(self.report.n_feat), min(self.report.n_feat))
             )
         else:
             raise ValueError("Missing report, run .make_report() first")
 
-    def extract_features(self, selection_rule="decrease_perf", number_feat_rep=None, gap=0.1):
+    def extract_features(self, selection_rule="decrease_perf", number_feat_rep=None, gap=0.1, alpha=0.5):
         """Extract survived features after SHAP RFE.
 
         Args:
-            selection_rule (str, optional): "decrease_perf", "best_valid", "num_feat", describes the rule for which the features after shap are chosen. Defaults to 'decrease_perf'.
+            selection_rule (str, optional): "decrease_perf", "best_valid", "num_feat", "robust_tradeoff" describes the rule for which the features after shap are chosen. Defaults to 'decrease_perf'.
             number_feat_rep (int, optional): valid only for the selection_rule "num_feat", determines the number of features to be extracted according to the report. Defaults to None.
             gap(float, optional): valid only for the selection_rule "decrease_perf", identifies the maximum gap over which the decrease in performance is not acceptable.
+            alpha(float, optional): valid only fot the selection_rule "robust_tradeoff", determines which term is preferred betweeen robustness and average performances in the formula 
+            α * Average_Perf - (1-α) * Gap_Robust
         Returns:
             list: list of features extracted after SHAP RFE according to the selection_rule.
         """
         self.selection_rule = selection_rule
         self.number_feat_rep = number_feat_rep
+        self.gap = gap
+        self.alpha = alpha
         # Check the target var and set the algo type
-        if selection_rule not in ["decrease_perf", "best_valid", "num_feat"]:
+        if selection_rule not in ["decrease_perf", "best_valid", "num_feat","robust_tradeoff"]:
             raise ValueError(
-                f"{selection_rule} is not a valid selection_rule. It should be one of the following:\n ['decrease_perf', 'best_valid', 'num_feat']"
+                f"{selection_rule} is not a valid selection_rule. It should be one of the following:\n ['decrease_perf', 'best_valid', 'num_feat', 'robust_tradeoff']"
             )
 
         if self.report is not None:
             if selection_rule == "decrease_perf":
                 # Define n_feat: the first time the validation score decreases of more than 10%
                 cutoff = (
                     self.report[["n_feat", "valid_score"]]
@@ -270,15 +274,28 @@
 
             elif selection_rule == "best_valid":
                 # Define n_feat: best validation score iteration
                 n_min_feat = self.report.loc[
                     self.report["valid_score"] == self.report["valid_score"].max(), "n_feat"
                 ].min()
                 self.final_feat = list(self.report.loc[self.report["n_feat"] == n_min_feat, "feat_used"])[0]
-
+            
+            elif selection_rule == "robust_tradeoff":
+                # Define n_feat: best score of the formula α * Average_Perf - (1-α) * Gap_Robust
+                adding_report = (
+                    self.report[["n_feat","train_score","valid_score"]]
+                    .assign(average_scoring=lambda x: (x.train_score + x.valid_score)/2)
+                    .assign(gap_ratio=lambda x: abs(x.train_score - x.valid_score))
+                    .assign(average_scoring=lambda x: (x.average_scoring - x.average_scoring.mean())/x.average_scoring.std())
+                    .assign(gap_ratio=lambda x: (x.gap_ratio - x.gap_ratio.mean())/x.gap_ratio.std())
+                    .assign(tradeoff_robust_average_scoring=lambda x: (alpha * x.average_scoring - (1 - alpha) * x.gap_ratio))
+                )
+                n_min_feat = adding_report.loc[adding_report.tradeoff_robust_average_scoring == adding_report.tradeoff_robust_average_scoring.max(),"n_feat"].min()
+                self.final_feat = list(self.report.loc[self.report["n_feat"] == n_min_feat, "feat_used"])[0]
+                
             else:
                 # Define n_feat: the user choose the features to use according to number of features to be used
                 if number_feat_rep is not None:
                     try:
                         self.final_feat = list(self.report.loc[self.report["n_feat"] == number_feat_rep, "feat_used"])[
                             0
                         ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cefeste-1.1.0/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.1.1/src/cefeste/elimination/shap_rfe.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from sklearn.metrics import roc_auc_score, r2_score, balanced_accuracy_score
 from sklearn.model_selection import RandomizedSearchCV, StratifiedKFold, GroupKFold
 from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder
 from sklearn.compose import ColumnTransformer
 import re
 from cefeste.utils import remove_features, time_step, get_categorical_features
 from functools import reduce
+import warnings
 
 
 @time_step
 def Shap_RFE_full(
     X_train,
     y_train,
     model,
@@ -312,40 +313,51 @@
         pd.DataFrame: Shap DataFrame.
     """
     if categorical_feature is None:
         categorical_feature = []
 
     # Get Shap
     feature_names = X_train.columns
+    using_features_imporance = False
     try:
         shap_values = shap.TreeExplainer(model).shap_values(X_train)
     except Exception:
-        # For Support Vector Machine and other no-Tree Algorithms
-        n_clusters = max(10, min(1000, int(X_train.shape[0] / 100)))
-        model.fit(X_train.values, y_train.values)
-        shap_values = shap.KernelExplainer(model.predict, shap.kmeans(X_train, n_clusters)).shap_values(X_train)
-    # For (multi) classification
-    if isinstance(shap_values, list):
-        db_list = list()
-        for i in range(len(shap_values)):
-            db_list.append(
-                pd.DataFrame(
-                    {"feature": feature_names, "shap_importance_" + str(i): np.abs(shap_values[i]).mean(axis=0)}
+        try:
+            # For Support Vector Machine and other no-Tree Algorithms
+            n_clusters = max(10, min(1000, int(X_train.shape[0] / 100)))
+            model.fit(X_train.values, y_train.values)
+            shap_values = shap.KernelExplainer(model.predict, shap.kmeans(X_train, n_clusters)).shap_values(X_train)
+        except Exception:
+            warnings.warn('shap inconsistent with this numpy version. Using feature_importance_ attribute')
+            # For computing features importance due to numpy version issues
+            feature_importances = model.feature_importances_
+            using_features_importance = True
+    
+    if using_features_importance:
+        shap_importance = pd.DataFrame({"feature": feature_names, "shap_importance": feature_importances})
+    else:
+        # For (multi) classification
+        if isinstance(shap_values, list):
+            db_list = list()
+            for i in range(len(shap_values)):
+                db_list.append(
+                    pd.DataFrame(
+                        {"feature": feature_names, "shap_importance_" + str(i): np.abs(shap_values[i]).mean(axis=0)}
+                    )
                 )
+            shap_importance = (
+                reduce(lambda left, right: pd.merge(left, right, how="outer", on="feature"), db_list)
+                .set_index("feature")
+                .assign(shap_importance=lambda x: x.sum(axis=1))
+                .loc[:, "shap_importance"]
+                .reset_index()
             )
-        shap_importance = (
-            reduce(lambda left, right: pd.merge(left, right, how="outer", on="feature"), db_list)
-            .set_index("feature")
-            .assign(shap_importance=lambda x: x.sum(axis=1))
-            .loc[:, "shap_importance"]
-            .reset_index()
-        )
-    # For regression and (some - depending on the classifier) binary classification
-    elif isinstance(shap_values, np.ndarray):
-        shap_importance = pd.DataFrame({"feature": feature_names, "shap_importance": np.abs(shap_values).mean(axis=0)})
+        # For regression and (some - depending on the classifier) binary classification
+        elif isinstance(shap_values, np.ndarray):
+            shap_importance = pd.DataFrame({"feature": feature_names, "shap_importance": np.abs(shap_values).mean(axis=0)})
 
     # For categorical features one-hot-encoded sum the shap values referring the same pivot feature
     if categorical_shap_ohe:
         for i in categorical_feature:
             shap_importance.loc[shap_importance.feature.str.startswith(i)] = shap_importance.loc[
                 shap_importance.feature.str.startswith(i)
             ].assign(
@@ -521,15 +533,15 @@
         feat_names = [re.sub(r"((remainder)|(cat))__", "", x) for x in feat_names]
         X_train_tsf = pd.DataFrame(preprocessor.transform(X_train_tsf), columns=feat_names)
         categorical_shap_ohe = True
 
     else:
         X_train_tsf[X_train_tsf.select_dtypes(['object']).columns] = X_train_tsf.select_dtypes(['object']).apply(lambda x: x.astype('category'))
 
-        CVSel_algo.fit(X_train_tsf, y_train)
+    CVSel_algo.fit(X_train_tsf, y_train)
 
     model = CVSel_algo.best_estimator_
     # Get Balanced Accuracy
     train_model_score = balanced_accuracy_score(y_train, CVSel_algo.predict(X_train_tsf))
     valid_model_score = CVSel_algo.best_score_
 
     # Get Shap
```

### Comparing `cefeste-1.1.0/src/cefeste/selection/__init__.py` & `cefeste-1.1.1/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/src/cefeste/selection/explanatory.py` & `cefeste-1.1.1/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/src/cefeste/selection/multivariate.py` & `cefeste-1.1.1/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/src/cefeste/selection/univariate.py` & `cefeste-1.1.1/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/src/cefeste/transform/__init__.py` & `cefeste-1.1.1/src/cefeste/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/src/cefeste/utils.py` & `cefeste-1.1.1/src/cefeste/utils.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.0/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.1.1/src/cefeste.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.0
+Version: 1.1.1
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cefeste-1.1.0/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.1.1/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

