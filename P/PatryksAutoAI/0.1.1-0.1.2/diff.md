# Comparing `tmp/PatryksAutoAI-0.1.1.tar.gz` & `tmp/PatryksAutoAI-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.1.1.tar", last modified: Wed May 10 17:07:56 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.1.2.tar", last modified: Wed May 10 17:50:34 2023, max compression
```

## Comparing `PatryksAutoAI-0.1.1.tar` & `PatryksAutoAI-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:07:56.658593 PatryksAutoAI-0.1.1/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:07:56.650593 PatryksAutoAI-0.1.1/Machine_Learning_Classes/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 16:58:56.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:07:56.650593 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       49 2023-05-10 16:59:16.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:07:56.650593 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 17:06:32.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7918 2023-04-26 14:31:57.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6282 2023-04-26 15:22:54.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5247 2023-04-18 06:48:02.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5918 2023-04-18 06:48:25.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2214 2023-04-18 06:48:31.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7243 2023-04-18 19:39:52.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2310 2023-04-18 09:55:03.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4835 2023-04-18 08:17:03.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6313 2023-04-26 15:24:02.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-04-18 19:40:03.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2264 2023-04-18 06:49:08.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5713 2023-04-18 08:16:37.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:07:56.654593 PatryksAutoAI-0.1.1/Machine_Learning_Classes/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        0 2023-05-10 16:59:50.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/model_data/metrics.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/model_data/metrics_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:07:56.654593 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       49 2023-05-10 16:59:21.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:07:56.654593 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      175 2023-05-10 17:07:35.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5972 2023-05-09 14:10:43.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2730 2023-05-09 14:36:47.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6078 2023-05-08 20:02:01.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2638 2023-05-09 14:36:46.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5445 2023-05-09 13:38:03.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2928 2023-05-09 14:26:13.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2762 2023-05-09 14:37:34.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7207 2023-05-09 13:52:06.000000 PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 17:07:56.658593 PatryksAutoAI-0.1.1/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:07:56.658593 PatryksAutoAI-0.1.1/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 17:07:56.000000 PatryksAutoAI-0.1.1/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1852 2023-05-10 17:07:56.000000 PatryksAutoAI-0.1.1/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 17:07:56.000000 PatryksAutoAI-0.1.1/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 17:07:56.000000 PatryksAutoAI-0.1.1/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 17:07:56.000000 PatryksAutoAI-0.1.1/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 17:07:56.658593 PatryksAutoAI-0.1.1/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 17:07:41.000000 PatryksAutoAI-0.1.1/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:50:34.211282 PatryksAutoAI-0.1.2/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:50:34.183282 PatryksAutoAI-0.1.2/Machine_Learning_Classes/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      153 2023-05-10 16:58:56.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:50:34.183282 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       49 2023-05-10 16:59:16.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:50:34.199282 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 17:06:32.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7918 2023-04-26 14:31:57.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6282 2023-04-26 15:22:54.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5247 2023-04-18 06:48:02.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5918 2023-04-18 06:48:25.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2214 2023-04-18 06:48:31.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7243 2023-04-18 19:39:52.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2310 2023-04-18 09:55:03.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4835 2023-04-18 08:17:03.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6313 2023-04-26 15:24:02.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2320 2023-04-18 19:40:03.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2264 2023-04-18 06:49:08.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5713 2023-04-18 08:16:37.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:50:34.203282 PatryksAutoAI-0.1.2/Machine_Learning_Classes/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       82 2023-05-10 17:49:51.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/model_data/metrics.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/model_data/metrics_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:50:34.203282 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       49 2023-05-10 16:59:21.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:50:34.207282 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      175 2023-05-10 17:07:35.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5972 2023-05-09 14:10:43.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2730 2023-05-09 14:36:47.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6078 2023-05-08 20:02:01.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2638 2023-05-09 14:36:46.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5445 2023-05-09 13:38:03.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2928 2023-05-09 14:26:13.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2762 2023-05-09 14:37:34.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7207 2023-05-09 13:52:06.000000 PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 17:50:34.211282 PatryksAutoAI-0.1.2/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-10 17:50:34.211282 PatryksAutoAI-0.1.2/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      602 2023-05-10 17:50:34.000000 PatryksAutoAI-0.1.2/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1852 2023-05-10 17:50:34.000000 PatryksAutoAI-0.1.2/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-10 17:50:34.000000 PatryksAutoAI-0.1.2/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      162 2023-05-10 17:50:34.000000 PatryksAutoAI-0.1.2/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       25 2023-05-10 17:50:34.000000 PatryksAutoAI-0.1.2/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-10 17:50:34.211282 PatryksAutoAI-0.1.2/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1062 2023-05-10 17:49:56.000000 PatryksAutoAI-0.1.2/setup.py
```

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/cat.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/extra_trees.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/hist_gradient.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/kneighbours.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/light_lgb.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/linear_svc.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/logistic_regression.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/random_forest.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/svc.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/classification/models/xgb.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/helper_function.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/model_data/metrics.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/model_data/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/model_data/metrics_regression.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/model_data/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/model_data/model_data.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/cat.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/elastic_net.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/lasso.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/lgb.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/sgd.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/svr.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/Machine_Learning_Classes/regression/models/xgb.py` & `PatryksAutoAI-0.1.2/Machine_Learning_Classes/regression/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/PKG-INFO` & `PatryksAutoAI-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.1.1
+Version: 0.1.2
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.1.1/PatryksAutoAI.egg-info/PKG-INFO` & `PatryksAutoAI-0.1.2/PatryksAutoAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PatryksAutoAI
-Version: 0.1.1
+Version: 0.1.2
 Summary: Auto_AI_patryk
 Home-page: UNKNOWN
 Author: patryk
 Author-email: lyczkopatryk1@gmail.com
 License: UNKNOWN
 Keywords: python,machine_learning,auto
 Platform: UNKNOWN
```

### Comparing `PatryksAutoAI-0.1.1/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.1.2/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.1.1/setup.py` & `PatryksAutoAI-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./Machine_Learning_Classes/requirements.txt') as f:
     requirements = f.read().splitlines()
```

