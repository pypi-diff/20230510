# Comparing `tmp/dython-0.7.3.tar.gz` & `tmp/dython-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dython-0.7.3.tar", last modified: Tue Dec 13 21:46:43 2022, max compression
+gzip compressed data, was "dython-0.7.4.tar", last modified: Wed May 10 07:38:24 2023, max compression
```

## Comparing `dython-0.7.3.tar` & `dython-0.7.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 21:46:43.318421 dython-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2022-12-13 21:46:34.000000 dython-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-13 21:46:34.000000 dython-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2022-12-13 21:46:43.318421 dython-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2022-12-13 21:46:34.000000 dython-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-13 21:46:34.000000 dython-0.7.3/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 21:46:43.318421 dython-0.7.3/dython/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-13 21:46:34.000000 dython-0.7.3/dython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2022-12-13 21:46:34.000000 dython-0.7.3/dython/_private.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2022-12-13 21:46:34.000000 dython-0.7.3/dython/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2022-12-13 21:46:34.000000 dython-0.7.3/dython/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2022-12-13 21:46:34.000000 dython-0.7.3/dython/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46792 2022-12-13 21:46:34.000000 dython-0.7.3/dython/nominal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2022-12-13 21:46:34.000000 dython-0.7.3/dython/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 21:46:43.318421 dython-0.7.3/dython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2022-12-13 21:46:43.000000 dython-0.7.3/dython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2022-12-13 21:46:43.000000 dython-0.7.3/dython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 21:46:43.000000 dython-0.7.3/dython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-13 21:46:43.000000 dython-0.7.3/dython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-13 21:46:43.000000 dython-0.7.3/dython.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-13 21:46:34.000000 dython-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-13 21:46:34.000000 dython-0.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 21:46:43.318421 dython-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2022-12-13 21:46:34.000000 dython-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:38:24.301157 dython-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-10 07:38:14.000000 dython-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 07:38:14.000000 dython-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-10 07:38:24.301157 dython-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-10 07:38:14.000000 dython-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 07:38:14.000000 dython-0.7.4/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:38:24.301157 dython-0.7.4/dython/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-10 07:38:14.000000 dython-0.7.4/dython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-10 07:38:14.000000 dython-0.7.4/dython/_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-10 07:38:14.000000 dython-0.7.4/dython/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-10 07:38:14.000000 dython-0.7.4/dython/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-05-10 07:38:14.000000 dython-0.7.4/dython/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46815 2023-05-10 07:38:14.000000 dython-0.7.4/dython/nominal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-10 07:38:14.000000 dython-0.7.4/dython/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:38:24.301157 dython-0.7.4/dython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-10 07:38:24.000000 dython-0.7.4/dython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 07:38:24.000000 dython-0.7.4/dython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:38:24.000000 dython-0.7.4/dython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-10 07:38:24.000000 dython-0.7.4/dython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 07:38:24.000000 dython-0.7.4/dython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 07:38:14.000000 dython-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-10 07:38:14.000000 dython-0.7.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 07:38:24.301157 dython-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-10 07:38:14.000000 dython-0.7.4/setup.py
```

### Comparing `dython-0.7.3/LICENSE` & `dython-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dython-0.7.3/PKG-INFO` & `dython-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dython
-Version: 0.7.3
+Version: 0.7.4
 Summary: A set of data tools in Python
 Home-page: http://shakedzy.xyz/dython
 Download-URL: https://pypi.org/project/dython/
 Author: Shaked Zychlinski
 Author-email: shakedzy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dython-0.7.3/README.md` & `dython-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dython-0.7.3/dython/data_utils.py` & `dython-0.7.4/dython/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
-from ._private import convert
+from ._private import convert, plot_or_not
 
 
 __all__ = [
     "identify_columns_by_type",
     "identify_columns_with_na",
     "one_hot_encode",
     "split_hist",
@@ -109,16 +109,15 @@
         plt.xlabel(xlabel)
     if title is not None:
         if title == "":
             title = values + " by " + split_by
         plt.title(title)
     plt.ylabel(ylabel)
     ax = plt.gca()
-    if plot:
-        plt.show()
+    plot_or_not(plot)
     return ax
 
 
 def identify_columns_by_type(dataset, include):
     """
     Given a dataset, identify columns of the types requested.
```

### Comparing `dython-0.7.3/dython/examples.py` & `dython-0.7.4/dython/examples.py`

 * *Files identical despite different names*

### Comparing `dython-0.7.3/dython/model_utils.py` & `dython-0.7.4/dython/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn.metrics import roc_curve, precision_recall_curve, auc
 from scikitplot.helpers import binary_ks_curve
-from ._private import convert
+from ._private import convert, plot_or_not
 
 __all__ = ["random_forest_feature_importance", "metric_graph", "ks_abc"]
 
 _ROC_PLOT_COLORS = ["b", "g", "r", "c", "m", "y", "k", "darkorange"]
 
 
 def _display_metric_plot(
@@ -24,16 +24,15 @@
         ax.set_xlabel("Recall")
         ax.set_ylabel("Precision")
         ax.set_title(title or "Precision-Recall Curve")
     if legend:
         ax.legend(loc=legend)
     if filename:
         plt.savefig(filename)
-    if plot:
-        plt.show()
+    plot_or_not(plot)
     return ax
 
 
 def _draw_estimated_optimal_threshold_mark(
     metric, x_axis, y_axis, thresholds, color, ms, fmt, ax
 ):
     annotation_offset = (-0.027, 0.03)
@@ -512,15 +511,14 @@
             t=title or "KS Statistic Plot", a=abc, fmt=fmt
         )
     )
     if legend:
         ax.legend(loc=legend)
     if filename:
         plt.savefig(filename)
-    if plot:
-        plt.show()
+    plot_or_not(plot)
     return {
         "abc": abc,
         "ks_stat": ks_statistic,
         "eopt": max_distance_at,
         "ax": ax,
     }
```

### Comparing `dython-0.7.3/dython/nominal.py` & `dython-0.7.4/dython/nominal.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 import numpy as np
 import pandas as pd
 import scipy.cluster.hierarchy as sch
 import scipy.stats as ss
 import seaborn as sns
 from psutil import cpu_count
 
-from ._private import convert, remove_incomplete_samples, replace_nan_with_value
+from ._private import (
+    convert,
+    remove_incomplete_samples,
+    replace_nan_with_value,
+    plot_or_not,
+)
 from .data_utils import identify_columns_by_type
 
 __all__ = [
     "associations",
     "cluster_correlations",
     "conditional_entropy",
     "correlation_ratio",
@@ -513,15 +518,14 @@
         else:
             nominal_columns = [
                 c for c in dataset.columns if c not in numerical_columns
             ]
 
     # handling NaN values in data
     if nan_strategy == _REPLACE:
-
         # handling pandas categorical
         dataset = _handling_category_for_nan_imputation(
             dataset, nan_replace_value
         )
 
         dataset.fillna(nan_replace_value, inplace=True)
     elif nan_strategy == _DROP_SAMPLES:
@@ -916,16 +920,15 @@
         mask=mask,
         ax=ax,
         cbar=cbar,
     )
     plt.title(title)
     if filename:
         plt.savefig(filename)
-    if plot:
-        plt.show()
+    plot_or_not(plot)
     return ax
 
 
 def _handling_category_for_nan_imputation(dataset, nan_replace_value):
     pd_categorical_columns = identify_columns_by_type(
         dataset, include=["category"]
     )
```

### Comparing `dython-0.7.3/dython/sampling.py` & `dython-0.7.4/dython/sampling.py`

 * *Files identical despite different names*

### Comparing `dython-0.7.3/dython.egg-info/PKG-INFO` & `dython-0.7.4/dython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dython
-Version: 0.7.3
+Version: 0.7.4
 Summary: A set of data tools in Python
 Home-page: http://shakedzy.xyz/dython
 Download-URL: https://pypi.org/project/dython/
 Author: Shaked Zychlinski
 Author-email: shakedzy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dython-0.7.3/setup.py` & `dython-0.7.4/setup.py`

 * *Files identical despite different names*

