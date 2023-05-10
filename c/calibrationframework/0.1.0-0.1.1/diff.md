# Comparing `tmp/calibrationframework-0.1.0.tar.gz` & `tmp/calibrationframework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibrationframework-0.1.0.tar", last modified: Wed May 10 17:18:19 2023, max compression
+gzip compressed data, was "calibrationframework-0.1.1.tar", last modified: Wed May 10 18:28:54 2023, max compression
```

## Comparing `calibrationframework-0.1.0.tar` & `calibrationframework-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:18:19.935220 calibrationframework-0.1.0/
--rw-rw-rw-   0        0        0     1095 2023-05-10 16:56:58.000000 calibrationframework-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      313 2023-05-10 17:18:19.935220 calibrationframework-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2023-05-10 16:56:58.000000 calibrationframework-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 17:18:19.935220 calibrationframework-0.1.0/calfram/
--rw-rw-rw-   0        0        0        2 2023-05-10 16:56:58.000000 calibrationframework-0.1.0/calfram/__init__.py
--rw-rw-rw-   0        0        0    16390 2023-05-10 16:56:58.000000 calibrationframework-0.1.0/calfram/calibrationframework.py
--rw-rw-rw-   0        0        0     3856 2023-05-10 16:56:58.000000 calibrationframework-0.1.0/calfram/ece.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:18:19.935220 calibrationframework-0.1.0/calibrationframework.egg-info/
--rw-rw-rw-   0        0        0      313 2023-05-10 17:18:19.000000 calibrationframework-0.1.0/calibrationframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-05-10 17:18:19.000000 calibrationframework-0.1.0/calibrationframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:18:19.000000 calibrationframework-0.1.0/calibrationframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 17:18:19.000000 calibrationframework-0.1.0/calibrationframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 17:18:19.000000 calibrationframework-0.1.0/calibrationframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 17:18:19.935220 calibrationframework-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-05-10 17:17:07.000000 calibrationframework-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:28:54.806103 calibrationframework-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2023-05-10 16:56:58.000000 calibrationframework-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      313 2023-05-10 18:28:54.806103 calibrationframework-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4812 2023-05-10 18:27:43.000000 calibrationframework-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 18:28:54.799597 calibrationframework-0.1.1/calfram/
+-rw-rw-rw-   0        0        0        2 2023-05-10 16:56:58.000000 calibrationframework-0.1.1/calfram/__init__.py
+-rw-rw-rw-   0        0        0    16568 2023-05-10 18:27:43.000000 calibrationframework-0.1.1/calfram/calibrationframework.py
+-rw-rw-rw-   0        0        0     3856 2023-05-10 16:56:58.000000 calibrationframework-0.1.1/calfram/ece.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:28:54.806103 calibrationframework-0.1.1/calibrationframework.egg-info/
+-rw-rw-rw-   0        0        0      313 2023-05-10 18:28:54.000000 calibrationframework-0.1.1/calibrationframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-05-10 18:28:54.000000 calibrationframework-0.1.1/calibrationframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:28:54.000000 calibrationframework-0.1.1/calibrationframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:28:54.000000 calibrationframework-0.1.1/calibrationframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 18:28:54.000000 calibrationframework-0.1.1/calibrationframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:28:54.806103 calibrationframework-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-05-10 18:28:13.000000 calibrationframework-0.1.1/setup.py
```

### Comparing `calibrationframework-0.1.0/LICENSE` & `calibrationframework-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calibrationframework-0.1.0/calfram/calibrationframework.py` & `calibrationframework-0.1.1/calfram/calibrationframework.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from ece import compute_eces
 from sklearn.preprocessing import OneHotEncoder
 import random
+from sklearn.metrics import brier_score_loss
 
 def end_points(x,y):
     #check coordinates (0,0) and (1,1)
     points = np.concatenate([x.reshape(x.shape[0], 1), y.reshape(y.shape[0], 1)], axis = 1)
     # if not np.all(points[0,:] == [0,0]):
     points = np.concatenate([np.array([[0,0]]), points], axis = 0)
     # else:
@@ -377,26 +378,29 @@
             elif up_weight is None and below_weight is not None:
                 fcc_dir = np.average(below_dist, weights=below_weight)
             elif up_weight is not None and below_weight is None:
                 fcc_dir = -np.average(up_dist, weights=up_weight)
             else:
                 fcc_dir = np.nan
 
+                
             ece = compute_eces(classes_scores[i]['y_one_hot_nclass'], classes_scores[i]['y_prob_one_hotnclass'],
                             classes_scores[i]['y_pred_one_hotnclass'], bins_dict['binids'],
                             bins_dict['bins'],'fp',int(i))
             ece_acc = compute_eces(classes_scores[i]['y_one_hot_nclass'], classes_scores[i]['y_prob_one_hotnclass'],
                             classes_scores[i]['y_pred_one_hotnclass'], bins_dict['binids'],  bins_dict['bins'],'acc',int(i))
-
+            brierloss = brier_score_loss(classes_scores[i]['y'], classes_scores[i]['proba'][:,1])
+        
             dict_msr = {'ece_acc': ece_acc, 'ece_fp':ece, 'ec_g': fcc_g, 'ec_under': 1-up_dist,'under_fr': up_weight, 'ec_over': 1-below_dist, 
-                        'over_fr': below_weight,'ec_underconf': fcc_underconf,'ec_overconf': fcc_overconf, 
-                        'ec_dir': fcc_dir, 'over_pts': below_pts, 'under_pts': up_pts, 
-                        'ec_l_all': 1-pts_distance_norm, 'where': where_are,
-                        'relative-freq': bins_dict['binfr'], 'x': x, 'y' :y
-                        }
+                    'over_fr': below_weight,'ec_underconf': fcc_underconf,'ec_overconf': fcc_overconf, 
+                    'ec_dir': fcc_dir, 'brier_loss': brierloss, 'over_pts': below_pts, 'under_pts': up_pts, 
+                    'ec_l_all': 1-pts_distance_norm, 'where': where_are,
+                    'relative-freq': bins_dict['binfr'], 'x': x, 'y' :y
+                    }
+
 
         measures['{}'.format(i)] = dict_msr
         binning_dict['{}'.format(i)] = bins_dict
 
             # ece, mce = mcece(prob, n_bins, y_test, predictions)
 
     return measures, binning_dict
```

### Comparing `calibrationframework-0.1.0/calfram/ece.py` & `calibrationframework-0.1.1/calfram/ece.py`

 * *Files identical despite different names*

