# Comparing `tmp/PatryksAutoAI-0.1.3.tar.gz` & `tmp/PatryksAutoAI-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.1.3.tar", last modified: Wed May 10 17:53:11 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.1.4.tar", last modified: Wed May 10 18:03:28 2023, max compression
```

## Comparing `PatryksAutoAI-0.1.3.tar` & `PatryksAutoAI-0.1.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:53:11.580723 PatryksAutoAI-0.1.3/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:53:11.564723 PatryksAutoAI-0.1.3/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 17:52:56.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:53:11.564723 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       49 2023-05-10 16:59:16.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:53:11.572723 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 17:06:32.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7918 2023-04-26 14:31:57.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6282 2023-04-26 15:22:54.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5247 2023-04-18 06:48:02.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5918 2023-04-18 06:48:25.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2214 2023-04-18 06:48:31.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7243 2023-04-18 19:39:52.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2310 2023-04-18 09:55:03.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4835 2023-04-18 08:17:03.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6313 2023-04-26 15:24:02.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-04-18 19:40:03.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2264 2023-04-18 06:49:08.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5713 2023-04-18 08:16:37.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:53:11.572723 PatryksAutoAI-0.1.3/Machine_Learning_Classes/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       82 2023-05-10 17:49:51.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/model_data/metrics.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/model_data/metrics_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:53:11.572723 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       49 2023-05-10 17:52:37.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:53:11.576723 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      175 2023-05-10 17:52:36.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5972 2023-05-09 14:10:43.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2730 2023-05-09 14:36:47.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6078 2023-05-08 20:02:01.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2638 2023-05-09 14:36:46.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5445 2023-05-09 13:38:03.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2928 2023-05-09 14:26:13.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2762 2023-05-09 14:37:34.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7207 2023-05-09 13:52:06.000000 PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 17:53:11.576723 PatryksAutoAI-0.1.3/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:53:11.576723 PatryksAutoAI-0.1.3/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 17:53:11.000000 PatryksAutoAI-0.1.3/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1852 2023-05-10 17:53:11.000000 PatryksAutoAI-0.1.3/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 17:53:11.000000 PatryksAutoAI-0.1.3/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 17:53:11.000000 PatryksAutoAI-0.1.3/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 17:53:11.000000 PatryksAutoAI-0.1.3/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 17:53:11.580723 PatryksAutoAI-0.1.3/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 17:52:59.000000 PatryksAutoAI-0.1.3/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:03:28.785850 PatryksAutoAI-0.1.4/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:03:28.757850 PatryksAutoAI-0.1.4/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 17:52:56.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:03:28.757850 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:03:28.773850 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7947 2023-05-10 18:02:26.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6311 2023-05-10 18:02:28.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5276 2023-05-10 18:02:20.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5947 2023-05-10 18:02:52.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2243 2023-05-10 18:02:51.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7272 2023-05-10 18:02:49.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2339 2023-05-10 18:02:48.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4864 2023-05-10 18:02:47.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6342 2023-05-10 18:02:46.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2349 2023-05-10 18:02:45.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2293 2023-05-10 18:02:44.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5742 2023-05-10 18:02:41.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:03:28.777850 PatryksAutoAI-0.1.4/Machine_Learning_Classes/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:03:28.777850 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       83 2023-05-10 18:02:07.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:03:28.781850 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      175 2023-05-10 17:52:36.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5997 2023-05-10 18:02:14.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2755 2023-05-10 18:02:16.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6103 2023-05-10 18:02:37.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2663 2023-05-10 18:02:36.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5470 2023-05-10 18:02:35.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2953 2023-05-10 18:02:34.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2787 2023-05-10 18:02:33.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7232 2023-05-10 18:02:30.000000 PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 18:03:28.781850 PatryksAutoAI-0.1.4/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 18:03:28.781850 PatryksAutoAI-0.1.4/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 18:03:28.000000 PatryksAutoAI-0.1.4/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1856 2023-05-10 18:03:28.000000 PatryksAutoAI-0.1.4/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 18:03:28.000000 PatryksAutoAI-0.1.4/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 18:03:28.000000 PatryksAutoAI-0.1.4/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 18:03:28.000000 PatryksAutoAI-0.1.4/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 18:03:28.785850 PatryksAutoAI-0.1.4/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 18:03:02.000000 PatryksAutoAI-0.1.4/setup.py
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/cat.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/cat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sklearn.model_selection import train_test_split, GridSearchCV, KFold
 from sklearn.preprocessing import OneHotEncoder
 from catboost import CatBoostClassifier
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.metrics import accuracy_score, roc_auc_score, log_loss
 import pandas as pd
 import numpy as np
 import optuna
 
 class Cat(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/extra_trees.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/extra_trees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import train_test_split, GridSearchCV, KFold
 from sklearn.ensemble import ExtraTreesClassifier
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.metrics import accuracy_score, roc_auc_score
 import pandas as pd
 import numpy as np
 import optuna
 from sklearn.preprocessing import OneHotEncoder
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/gradient_boosting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import train_test_split, GridSearchCV, KFold
 from sklearn.ensemble import GradientBoostingClassifier
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.metrics import accuracy_score, roc_auc_score
 import numpy as np
 import optuna
 
 
 class GradientBoosting(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/hist_gradient.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/hist_gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import train_test_split, GridSearchCV, KFold
 from sklearn.ensemble import HistGradientBoostingClassifier
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.metrics import accuracy_score, roc_auc_score
 import numpy as np
 import optuna
 
 
 class HistGradient(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/kneighbours.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/kneighbours.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, KFold
 from sklearn.metrics import roc_auc_score
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.neighbors import KNeighborsClassifier
 import numpy as np
 
 
 class Kneighbours(Metrics):
     def __init__(self):
         self.metric = Metrics()
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/light_lgb.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/light_lgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import train_test_split, GridSearchCV, KFold
 import optuna.integration.lightgbm as lgb
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.metrics import accuracy_score, roc_auc_score
 import numpy as np
 import optuna
 
 class LightLGB(Metrics):
     def __init__(self):
         self.metric = Metrics()
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/linear_svc.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/sgd_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from sklearn.model_selection import GridSearchCV, KFold
 from sklearn.metrics import roc_auc_score
-from model_data.metrics import Metrics
-from sklearn.svm import LinearSVC
+from Machine_Learning_Classes.classification.metrics import Metrics
+from sklearn.svm import SGDClassifier
 import numpy as np
 
-class SVC(Metrics):
+
+class SGD(Metrics):
     def __init__(self):
         self.metric = Metrics()
         self.model = None
         self.parameters = None
-    
-    def create(self,X,y, params=None,cv=3):
-        params_columns = ["C", "penalty", "verbose", 
-                          "random_state","max_iter"]
-        params_basic = {'C': [0.1,1,10],
-                'penalty': ['l2','l1'],
-                'verbose': [0],
-                'random_state': [42],
-                'max_iter': [100, 600]}
-        
+
+    def create(self, X, y, params=None, cv=3):
+        params_columns = ["loss", "penalty","alpha","max_iter"]
+        params_basic = {
+            'loss': ['hinge', 'log_loss', 'modified_huber','perceptron'],
+            'penalty': ['l2', 'l1', 'elasticnet'],
+            'alpha': [0.001, 0.01, 0.1,0.5],
+            'max_iter': [1000, 5000]
+            }
         if params == None:
             params = params_basic
         else:
             for parameter in params_columns:
                 if parameter not in params.keys():
                     params[parameter] = params_basic[parameter]
 
-        svc = LinearSVC()
-        grid_search = GridSearchCV(svc, params, cv=cv)
+        sgd = SGDClassifier()
+        grid_search = GridSearchCV(sgd, params, cv=cv)
         grid_search.fit(X, y)
         best_params = grid_search.best_params_
         self.model = grid_search.best_estimator_
         self.parameters = best_params
 
     def score(self,X,y):
         preds = np.round(self.model.predict(X))
@@ -49,21 +49,21 @@
         kfold = KFold(n_splits=n_splits, shuffle=True, random_state=42)
         predictions = np.zeros(df_test.shape[0])
         roc = []
         n=0
 
         for i, (train_index, valid_index) in enumerate(kfold.split(X,y)):
             X_train, X_test = X.iloc[train_index], X.iloc[valid_index]
-            y_train, y_test = X.iloc[train_index], y.iloc[valid_index]
+            y_train, y_test = y.iloc[train_index], y.iloc[valid_index]
 
             self.create(X_train,y_train,params=params)
             predictions += self.predict(df_test)/n_splits
             val_pred = self.predict(X_test)
             roc.append(roc_auc_score(y_test,val_pred))
 
             print(f"{i} Fold scored: {roc[i]}")
 
         print(f"Mean roc score {np.mean(roc)}")
         return predictions
     
     def get_parameters(self):
-        return self.parameters
+        return self.parameters
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/logistic_regression.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/logistic_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import train_test_split,GridSearchCV, KFold
 from sklearn.linear_model import LogisticRegression
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.metrics import accuracy_score, roc_auc_score
 import numpy as np
 import optuna
 
 ## Logistic Regression
 class LR(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/random_forest.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/random_forest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import train_test_split, GridSearchCV, KFold
 from sklearn.ensemble import RandomForestClassifier
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.metrics import accuracy_score, roc_auc_score
 import pandas as pd
 import numpy as np
 import optuna
 from sklearn.preprocessing import OneHotEncoder
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/linear_svc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from sklearn.model_selection import GridSearchCV, KFold
 from sklearn.metrics import roc_auc_score
-from model_data.metrics import Metrics
-from sklearn.svm import SGDClassifier
+from Machine_Learning_Classes.classification.metrics import Metrics
+from sklearn.svm import LinearSVC
 import numpy as np
 
-
-class SGD(Metrics):
+class SVC(Metrics):
     def __init__(self):
         self.metric = Metrics()
         self.model = None
         self.parameters = None
-
-    def create(self, X, y, params=None, cv=3):
-        params_columns = ["loss", "penalty","alpha","max_iter"]
-        params_basic = {
-            'loss': ['hinge', 'log_loss', 'modified_huber','perceptron'],
-            'penalty': ['l2', 'l1', 'elasticnet'],
-            'alpha': [0.001, 0.01, 0.1,0.5],
-            'max_iter': [1000, 5000]
-            }
+    
+    def create(self,X,y, params=None,cv=3):
+        params_columns = ["C", "penalty", "verbose", 
+                          "random_state","max_iter"]
+        params_basic = {'C': [0.1,1,10],
+                'penalty': ['l2','l1'],
+                'verbose': [0],
+                'random_state': [42],
+                'max_iter': [100, 600]}
+        
         if params == None:
             params = params_basic
         else:
             for parameter in params_columns:
                 if parameter not in params.keys():
                     params[parameter] = params_basic[parameter]
 
-        sgd = SGDClassifier()
-        grid_search = GridSearchCV(sgd, params, cv=cv)
+        svc = LinearSVC()
+        grid_search = GridSearchCV(svc, params, cv=cv)
         grid_search.fit(X, y)
         best_params = grid_search.best_params_
         self.model = grid_search.best_estimator_
         self.parameters = best_params
 
     def score(self,X,y):
         preds = np.round(self.model.predict(X))
@@ -49,21 +49,21 @@
         kfold = KFold(n_splits=n_splits, shuffle=True, random_state=42)
         predictions = np.zeros(df_test.shape[0])
         roc = []
         n=0
 
         for i, (train_index, valid_index) in enumerate(kfold.split(X,y)):
             X_train, X_test = X.iloc[train_index], X.iloc[valid_index]
-            y_train, y_test = y.iloc[train_index], y.iloc[valid_index]
+            y_train, y_test = X.iloc[train_index], y.iloc[valid_index]
 
             self.create(X_train,y_train,params=params)
             predictions += self.predict(df_test)/n_splits
             val_pred = self.predict(X_test)
             roc.append(roc_auc_score(y_test,val_pred))
 
             print(f"{i} Fold scored: {roc[i]}")
 
         print(f"Mean roc score {np.mean(roc)}")
         return predictions
     
     def get_parameters(self):
-        return self.parameters
+        return self.parameters
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/svc.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/svc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, KFold
 from sklearn.metrics import roc_auc_score
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.svm import SVC
 import numpy as np
 
 
 class SVCModel(Metrics):
     def __init__(self):
         self.metric = Metrics()
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/classification/models/xgb.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/models/xgb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
  
 from sklearn.model_selection import train_test_split,GridSearchCV,KFold
-from model_data.metrics import Metrics
+from Machine_Learning_Classes.classification.metrics import Metrics
 from sklearn.metrics import log_loss, roc_auc_score
 import numpy as np
 import xgboost as xgb
 import optuna
 
 
 class XGB(Metrics):
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/model_data/metrics.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/model_data/metrics_regression.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/model_data/model_data.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/cat.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/cat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split
 from sklearn.metrics import mean_squared_error,KFold
-from model_data.metrics_regression import Metrics
+from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from catboost import CatBoostRegressor
 import numpy as np
 import optuna
 
 
 class Cat(Metrics):
     def __init__(self):
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/elastic_net.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/elastic_net.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split
 from sklearn.metrics import mean_squared_error,KFold
-from model_data.metrics_regression import Metrics
+from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from sklearn.linear_model import ElasticNet
 import numpy as np
 
 class ElasticNetM(Metrics):
     def __init__(self):
         self.model = None
         self.parameters = None
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/gradient_boosting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sklearn.metrics import mean_squared_error,KFold
 from sklearn.ensemble import GradientBoostingRegressor
 from sklearn.model_selection import GridSearchCV, train_test_split
-from model_data.metrics_regression import Metrics
+from Machine_Learning_Classes.regression.metrics_regression import Metrics
 import numpy as np
 import optuna
 
 
 class GradientBoosting(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/lasso.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/lasso.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split
 from sklearn.metrics import mean_squared_error,KFold
-from model_data.metrics_regression import Metrics
+from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from sklearn.linear_model import Lasso
 import numpy as np
 
 class LassoM(Metrics):
     def __init__(self):
         self.model = None
         self.parameters = None
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/lgb.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/lgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split
 from sklearn.metrics import mean_squared_error,KFold
-from model_data.metrics_regression import Metrics
+from Machine_Learning_Classes.regression.metrics_regression import Metrics
 import lightgbm as lgb
 import numpy as np
 import optuna
 
 class LGB(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/sgd.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/sgd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split
 from sklearn.metrics import mean_squared_error,KFold
-from model_data.metrics_regression import Metrics
+from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from sklearn.linear_model import SGDRegressor
 import numpy as np
 
 class SGD(Metrics):
     def __init__(self):
         self.model = None
         self.parameters = None
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/svr.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/svr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split
 from sklearn.metrics import mean_squared_error,KFold
-from model_data.metrics_regression import Metrics
+from Machine_Learning_Classes.regression.metrics_regression import Metrics
 from sklearn.svm import SVR
 import numpy as np
 
 
 class SVRM(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.3/Machine_Learning_Classes/regression/models/xgb.py` & `PatryksAutoAI-0.1.4/Machine_Learning_Classes/regression/models/xgb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sklearn.model_selection import GridSearchCV, train_test_split
 from sklearn.metrics import mean_squared_error,KFold
-from model_data.metrics_regression import Metrics
+from Machine_Learning_Classes.regression.metrics_regression import Metrics
 import xgboost as xgb
 import numpy as np
 import optuna
 
 class XGB(Metrics):
     def __init__(self):
         self.model = None
```

### Comparing `PatryksAutoAI-0.1.3/PKG-INFO` & `PatryksAutoAI-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.1.3
+Version: 0.1.4
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.1.3/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.1.4/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.1.3
+Version: 0.1.4
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.1.3/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.1.4/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 setup.py
 Machine_Learning_Classes/__init__.py
 Machine_Learning_Classes/helper_function.py
 Machine_Learning_Classes/classification/__init__.py
+Machine_Learning_Classes/classification/metrics.py
 Machine_Learning_Classes/classification/models/__init__.py
 Machine_Learning_Classes/classification/models/cat.py
 Machine_Learning_Classes/classification/models/extra_trees.py
 Machine_Learning_Classes/classification/models/gradient_boosting.py
 Machine_Learning_Classes/classification/models/hist_gradient.py
 Machine_Learning_Classes/classification/models/kneighbours.py
 Machine_Learning_Classes/classification/models/light_lgb.py
 Machine_Learning_Classes/classification/models/linear_svc.py
 Machine_Learning_Classes/classification/models/logistic_regression.py
 Machine_Learning_Classes/classification/models/random_forest.py
 Machine_Learning_Classes/classification/models/sgd_classifier.py
 Machine_Learning_Classes/classification/models/svc.py
 Machine_Learning_Classes/classification/models/xgb.py
 Machine_Learning_Classes/model_data/__init__.py
-Machine_Learning_Classes/model_data/metrics.py
-Machine_Learning_Classes/model_data/metrics_regression.py
 Machine_Learning_Classes/model_data/model_data.py
 Machine_Learning_Classes/regression/__init__.py
+Machine_Learning_Classes/regression/metrics_regression.py
 Machine_Learning_Classes/regression/models/__init__.py
 Machine_Learning_Classes/regression/models/cat.py
 Machine_Learning_Classes/regression/models/elastic_net.py
 Machine_Learning_Classes/regression/models/gradient_boosting.py
 Machine_Learning_Classes/regression/models/lasso.py
 Machine_Learning_Classes/regression/models/lgb.py
 Machine_Learning_Classes/regression/models/sgd.py
```

### Comparing `PatryksAutoAI-0.1.3/setup.py` & `PatryksAutoAI-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./Machine_Learning_Classes/requirements.txt') as f:
     requirements = f.read().splitlines()
```

