# Comparing `tmp/cefeste-1.1.1.tar.gz` & `tmp/cefeste-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefeste-1.1.1.tar", last modified: Tue May  9 13:07:09 2023, max compression
+gzip compressed data, was "cefeste-1.1.2.tar", last modified: Wed May 10 10:23:59 2023, max compression
```

## Comparing `cefeste-1.1.1.tar` & `cefeste-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.057908 cefeste-1.1.1/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.1/LICENCE
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-05-09 13:07:09.057908 cefeste-1.1.1/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1558 2023-05-05 08:25:33.000000 cefeste-1.1.1/README.md
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-05-09 12:58:02.000000 cefeste-1.1.1/pyproject.toml
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-09 13:07:09.057908 cefeste-1.1.1/setup.cfg
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      997 2023-05-09 12:58:02.000000 cefeste-1.1.1/setup.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.049908 cefeste-1.1.1/src/
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.053908 cefeste-1.1.1/src/cefeste/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/config.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.053908 cefeste-1.1.1/src/cefeste/elimination/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15368 2023-05-09 12:58:02.000000 cefeste-1.1.1/src/cefeste/elimination/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25816 2023-05-09 13:05:39.000000 cefeste-1.1.1/src/cefeste/elimination/shap_rfe.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.057908 cefeste-1.1.1/src/cefeste/selection/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/selection/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/selection/explanatory.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/selection/multivariate.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/selection/univariate.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.057908 cefeste-1.1.1/src/cefeste/transform/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-05-05 08:25:33.000000 cefeste-1.1.1/src/cefeste/transform/__init__.py
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-05 08:25:52.000000 cefeste-1.1.1/src/cefeste/utils.py
-drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-09 13:07:09.053908 cefeste-1.1.1/src/cefeste.egg-info/
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2074 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)      129 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-09 13:07:09.000000 cefeste-1.1.1/src/cefeste.egg-info/top_level.txt
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.880164 cefeste-1.1.2/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1073 2023-05-05 08:25:33.000000 cefeste-1.1.2/LICENCE
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2076 2023-05-10 10:23:59.880164 cefeste-1.1.2/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1560 2023-05-10 10:23:33.000000 cefeste-1.1.2/README.md
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      544 2023-05-10 10:23:33.000000 cefeste-1.1.2/pyproject.toml
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)       38 2023-05-10 10:23:59.880164 cefeste-1.1.2/setup.cfg
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      997 2023-05-10 10:23:33.000000 cefeste-1.1.2/setup.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.772162 cefeste-1.1.2/src/
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.824163 cefeste-1.1.2/src/cefeste/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     3364 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      444 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/config.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.824163 cefeste-1.1.2/src/cefeste/elimination/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    15368 2023-05-10 10:23:33.000000 cefeste-1.1.2/src/cefeste/elimination/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    25817 2023-05-10 10:23:33.000000 cefeste-1.1.2/src/cefeste/elimination/shap_rfe.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.844163 cefeste-1.1.2/src/cefeste/selection/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    27726 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/selection/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10558 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/selection/explanatory.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    21561 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/selection/multivariate.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)    10122 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/selection/univariate.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.852163 cefeste-1.1.2/src/cefeste/transform/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     1003 2023-05-05 08:25:33.000000 cefeste-1.1.2/src/cefeste/transform/__init__.py
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2434 2023-05-10 10:23:33.000000 cefeste-1.1.2/src/cefeste/utils.py
+drwxr-xr-x   0 jupyter   (1000) jupyter   (1001)        0 2023-05-10 10:23:59.824163 cefeste-1.1.2/src/cefeste.egg-info/
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)     2076 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      533 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        1 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)      129 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/requires.txt
+-rw-r--r--   0 jupyter   (1000) jupyter   (1001)        8 2023-05-10 10:23:59.000000 cefeste-1.1.2/src/cefeste.egg-info/top_level.txt
```

### Comparing `cefeste-1.1.1/LICENCE` & `cefeste-1.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/PKG-INFO` & `cefeste-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.1
+Version: 1.1.2
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# **C**redito **E**miliano -  Fe**ature **S**election, **T**ransformation and **E**limination (CE - FeSTE)
+# **C**redito **E**miliano -  **Fe**ature **S**election, **T**ransformation and **E**limination (CE - FeSTE)
 
 This repo contains the 'FeSTE' python package which helps in the features management from the pre-filtering to the pre-processing and feature elimination.
 
 # Installation
 
 To install it:
```

### Comparing `cefeste-1.1.1/README.md` & `cefeste-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# **C**redito **E**miliano -  Fe**ature **S**election, **T**ransformation and **E**limination (CE - FeSTE)
+# **C**redito **E**miliano -  **Fe**ature **S**election, **T**ransformation and **E**limination (CE - FeSTE)
 
 This repo contains the 'FeSTE' python package which helps in the features management from the pre-filtering to the pre-processing and feature elimination.
 
 # Installation
 
 To install it:
```

### Comparing `cefeste-1.1.1/pyproject.toml` & `cefeste-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cefeste"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="DAT - Mattia Centurelli", email="mcenturelli@credem.it" },
 ]
 description = "Feature Selection and Elimination"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cefeste-1.1.1/setup.py` & `cefeste-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ce-feste",
-    version="1.1.1",
+    version="1.1.2",
     description="Package for Feature Selection, Transformation, Elimination",
     author="DAT/Mattia Centurelli",
     author_email="mcenturelli@credem.it",
     url="https://dev.azure.com/credem-data/DAT/_git/ce-feste",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `cefeste-1.1.1/src/cefeste/__init__.py` & `cefeste-1.1.2/src/cefeste/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/src/cefeste/elimination/__init__.py` & `cefeste-1.1.2/src/cefeste/elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/src/cefeste/elimination/shap_rfe.py` & `cefeste-1.1.2/src/cefeste/elimination/shap_rfe.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
         pd.DataFrame: Shap DataFrame.
     """
     if categorical_feature is None:
         categorical_feature = []
 
     # Get Shap
     feature_names = X_train.columns
-    using_features_imporance = False
+    using_features_importance = False
     try:
         shap_values = shap.TreeExplainer(model).shap_values(X_train)
     except Exception:
         try:
             # For Support Vector Machine and other no-Tree Algorithms
             n_clusters = max(10, min(1000, int(X_train.shape[0] / 100)))
             model.fit(X_train.values, y_train.values)
```

### Comparing `cefeste-1.1.1/src/cefeste/selection/__init__.py` & `cefeste-1.1.2/src/cefeste/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/src/cefeste/selection/explanatory.py` & `cefeste-1.1.2/src/cefeste/selection/explanatory.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/src/cefeste/selection/multivariate.py` & `cefeste-1.1.2/src/cefeste/selection/multivariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/src/cefeste/selection/univariate.py` & `cefeste-1.1.2/src/cefeste/selection/univariate.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/src/cefeste/transform/__init__.py` & `cefeste-1.1.2/src/cefeste/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/src/cefeste/utils.py` & `cefeste-1.1.2/src/cefeste/utils.py`

 * *Files identical despite different names*

### Comparing `cefeste-1.1.1/src/cefeste.egg-info/PKG-INFO` & `cefeste-1.1.2/src/cefeste.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cefeste
-Version: 1.1.1
+Version: 1.1.2
 Summary: Feature Selection and Elimination
 Home-page: https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Author: DAT/Mattia Centurelli
 Author-email: DAT - Mattia Centurelli <mcenturelli@credem.it>
 Project-URL: Homepage, https://dev.azure.com/credem-data/DAT/_git/ce-feste
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
-# **C**redito **E**miliano -  Fe**ature **S**election, **T**ransformation and **E**limination (CE - FeSTE)
+# **C**redito **E**miliano -  **Fe**ature **S**election, **T**ransformation and **E**limination (CE - FeSTE)
 
 This repo contains the 'FeSTE' python package which helps in the features management from the pre-filtering to the pre-processing and feature elimination.
 
 # Installation
 
 To install it:
```

### Comparing `cefeste-1.1.1/src/cefeste.egg-info/SOURCES.txt` & `cefeste-1.1.2/src/cefeste.egg-info/SOURCES.txt`

 * *Files identical despite different names*

