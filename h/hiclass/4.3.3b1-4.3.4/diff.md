# Comparing `tmp/hiclass-4.3.3b1.tar.gz` & `tmp/hiclass-4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiclass-4.3.3b1.tar", last modified: Thu Mar 16 12:48:08 2023, max compression
+gzip compressed data, was "hiclass-4.3.4.tar", last modified: Wed May 10 09:19:16 2023, max compression
```

## Comparing `hiclass-4.3.3b1.tar` & `hiclass-4.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:08.527808 hiclass-4.3.3b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-03-16 12:48:08.527808 hiclass-4.3.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14300 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:08.531808 hiclass-4.3.3b1/hiclass/
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/hiclass/BinaryPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/hiclass/ConstantClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/hiclass/HierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/hiclass/LocalClassifierPerLevel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/hiclass/LocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/hiclass/LocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/hiclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-16 12:48:08.531808 hiclass-4.3.3b1/hiclass/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/hiclass/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:08.527808 hiclass-4.3.3b1/hiclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-03-16 12:48:08.000000 hiclass-4.3.3b1/hiclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-16 12:48:08.000000 hiclass-4.3.3b1/hiclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 12:48:08.000000 hiclass-4.3.3b1/hiclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-16 12:48:08.000000 hiclass-4.3.3b1/hiclass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-16 12:48:08.000000 hiclass-4.3.3b1/hiclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 12:48:08.000000 hiclass-4.3.3b1/hiclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-16 12:48:08.531808 hiclass-4.3.3b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 12:48:08.527808 hiclass-4.3.3b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/tests/test_BinaryPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/tests/test_ConstantClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/tests/test_HierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/tests/test_LocalClassifierPerLevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/tests/test_LocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/tests/test_LocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-03-16 12:47:40.000000 hiclass-4.3.3b1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:19:16.039438 hiclass-4.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-10 09:18:52.000000 hiclass-4.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 09:18:52.000000 hiclass-4.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-05-10 09:19:16.039438 hiclass-4.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14300 2023-05-10 09:18:52.000000 hiclass-4.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:19:16.039438 hiclass-4.3.4/hiclass/
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/BinaryPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/ConstantClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/HierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/LocalClassifierPerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/LocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/LocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 09:19:16.039438 hiclass-4.3.4/hiclass/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-10 09:18:52.000000 hiclass-4.3.4/hiclass/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:19:16.039438 hiclass-4.3.4/hiclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15734 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 09:19:16.000000 hiclass-4.3.4/hiclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-10 09:19:16.039438 hiclass-4.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-10 09:18:52.000000 hiclass-4.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:19:16.039438 hiclass-4.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_BinaryPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_ConstantClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_HierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_LocalClassifierPerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_LocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_LocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-10 09:18:52.000000 hiclass-4.3.4/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-05-10 09:18:52.000000 hiclass-4.3.4/versioneer.py
```

### Comparing `hiclass-4.3.3b1/LICENSE` & `hiclass-4.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/PKG-INFO` & `hiclass-4.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclass
-Version: 4.3.3b1
+Version: 4.3.4
 Summary: Hierarchical Classification Library.
 Author: Fabio Malcher Miranda, Niklas Koehnecke
 Author-email: fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/hiclass/issues
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/hiclass
 Project-URL: Related Software, https://gitlab.com/dacs-hpi
@@ -19,14 +19,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 License-File: LICENSE
```

### Comparing `hiclass-4.3.3b1/README.md` & `hiclass-4.3.4/README.md`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/hiclass/BinaryPolicy.py` & `hiclass-4.3.4/hiclass/BinaryPolicy.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/hiclass/ConstantClassifier.py` & `hiclass-4.3.4/hiclass/ConstantClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/hiclass/HierarchicalClassifier.py` & `hiclass-4.3.4/hiclass/HierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/hiclass/LocalClassifierPerLevel.py` & `hiclass-4.3.4/hiclass/LocalClassifierPerLevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,18 @@
             separator, self.X_, self.y_[:, level], self.sample_weight_
         )
 
         unique_y = np.unique(y)
         if len(unique_y) == 1 and self.replace_classifiers:
             classifier = ConstantClassifier()
         if not self.bert:
-            classifier.fit(X, y, sample_weight)
+            try:
+                classifier.fit(X, y, sample_weight)
+            except TypeError:
+                classifier.fit(X, y)
         else:
             classifier.fit(X, y)
         return classifier
 
     @staticmethod
     def _remove_empty_leaves(separator, X, y, sample_weight):
         # Detect rows where leaves are not empty
```

### Comparing `hiclass-4.3.3b1/hiclass/LocalClassifierPerNode.py` & `hiclass-4.3.4/hiclass/LocalClassifierPerNode.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,18 @@
     def _fit_classifier(self, node):
         classifier = self.hierarchy_.nodes[node]["classifier"]
         X, y, sample_weight = self.binary_policy_.get_binary_examples(node)
         unique_y = np.unique(y)
         if len(unique_y) == 1 and self.replace_classifiers:
             classifier = ConstantClassifier()
         if not self.bert:
-            classifier.fit(X, y, sample_weight)
+            try:
+                classifier.fit(X, y, sample_weight)
+            except TypeError:
+                classifier.fit(X, y)
         else:
             classifier.fit(X, y)
         return classifier
 
     def _clean_up(self):
         super()._clean_up()
         del self.binary_policy_
```

### Comparing `hiclass-4.3.3b1/hiclass/LocalClassifierPerParentNode.py` & `hiclass-4.3.4/hiclass/LocalClassifierPerParentNode.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,15 +207,18 @@
         classifier = self.hierarchy_.nodes[node]["classifier"]
         # get children examples
         X, y, sample_weight = self._get_successors(node)
         unique_y = np.unique(y)
         if len(unique_y) == 1 and self.replace_classifiers:
             classifier = ConstantClassifier()
         if not self.bert:
-            classifier.fit(X, y, sample_weight)
+            try:
+                classifier.fit(X, y, sample_weight)
+            except TypeError:
+                classifier.fit(X, y)
         else:
             classifier.fit(X, y)
         return classifier
 
     def _fit_digraph(self, local_mode: bool = False, use_joblib: bool = False):
         self.logger_.info("Fitting local classifiers")
         nodes = self._get_parents()
```

### Comparing `hiclass-4.3.3b1/hiclass/metrics.py` & `hiclass-4.3.4/hiclass/metrics.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/hiclass.egg-info/PKG-INFO` & `hiclass-4.3.4/hiclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclass
-Version: 4.3.3b1
+Version: 4.3.4
 Summary: Hierarchical Classification Library.
 Author: Fabio Malcher Miranda, Niklas Koehnecke
 Author-email: fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/hiclass/issues
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/hiclass
 Project-URL: Related Software, https://gitlab.com/dacs-hpi
@@ -19,14 +19,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: ray
 License-File: LICENSE
```

### Comparing `hiclass-4.3.3b1/hiclass.egg-info/SOURCES.txt` & `hiclass-4.3.4/hiclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/setup.py` & `hiclass-4.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,15 @@
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
 #    # $ setup.py publish support.
 #    cmdclass={
 #        'upload': UploadCommand,
```

### Comparing `hiclass-4.3.3b1/tests/test_BinaryPolicy.py` & `hiclass-4.3.4/tests/test_BinaryPolicy.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/tests/test_ConstantClassifier.py` & `hiclass-4.3.4/tests/test_ConstantClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/tests/test_HierarchicalClassifier.py` & `hiclass-4.3.4/tests/test_HierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/tests/test_LocalClassifierPerLevel.py` & `hiclass-4.3.4/tests/test_LocalClassifierPerLevel.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import networkx as nx
 import numpy as np
 import pytest
 from numpy.testing import assert_array_equal
 from scipy.sparse import csr_matrix
 from sklearn.exceptions import NotFittedError
 from sklearn.linear_model import LogisticRegression
+from sklearn.neighbors import KNeighborsClassifier
 from sklearn.utils.estimator_checks import parametrize_with_checks
 from sklearn.utils.validation import check_is_fitted
+
 from hiclass import LocalClassifierPerLevel
 from hiclass.ConstantClassifier import ConstantClassifier
 
 
 @parametrize_with_checks([LocalClassifierPerLevel()])
 def test_sklearn_compatible_estimator(estimator, check):
     check(estimator)
@@ -181,17 +183,32 @@
         lcppn.root_,
     ]
     assert_array_equal(ground_truth, predictions)
 
 
 def test_fit_bert():
     bert = ConstantClassifier()
-    lcpn = LocalClassifierPerLevel(
+    lcpl = LocalClassifierPerLevel(
         local_classifier=bert,
         bert=True,
     )
     X = ["Text 1", "Text 2"]
     y = ["a", "a"]
-    lcpn.fit(X, y)
-    check_is_fitted(lcpn)
-    predictions = lcpn.predict(X)
+    lcpl.fit(X, y)
+    check_is_fitted(lcpl)
+    predictions = lcpl.predict(X)
     assert_array_equal(y, predictions)
+
+
+def test_knn():
+    knn = KNeighborsClassifier(
+        n_neighbors=2,
+    )
+    lcpl = LocalClassifierPerLevel(
+        local_classifier=knn,
+    )
+    y = np.array([["a", "b"], ["a", "c"]])
+    X = np.array([[1, 2], [3, 4]])
+    lcpl.fit(X, y)
+    check_is_fitted(lcpl)
+    # predictions = lcpl.predict(X)
+    # assert_array_equal(y, predictions)
```

### Comparing `hiclass-4.3.3b1/tests/test_LocalClassifierPerNode.py` & `hiclass-4.3.4/tests/test_LocalClassifierPerNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import networkx as nx
 import numpy as np
 import pytest
 from numpy.testing import assert_array_equal
 from scipy.sparse import csr_matrix
 from sklearn.exceptions import NotFittedError
 from sklearn.linear_model import LogisticRegression
+from sklearn.neighbors import KNeighborsClassifier
 from sklearn.utils.estimator_checks import parametrize_with_checks
 from sklearn.utils.validation import check_is_fitted
 
 from hiclass import LocalClassifierPerNode
 from hiclass.BinaryPolicy import ExclusivePolicy
 from hiclass.ConstantClassifier import ConstantClassifier
 
@@ -253,7 +254,22 @@
     )
     X = ["Text 1", "Text 2"]
     y = ["a", "a"]
     lcpn.fit(X, y)
     check_is_fitted(lcpn)
     predictions = lcpn.predict(X)
     assert_array_equal(y, predictions)
+
+
+def test_knn():
+    knn = KNeighborsClassifier(
+        n_neighbors=2,
+    )
+    lcpn = LocalClassifierPerNode(
+        local_classifier=knn,
+    )
+    y = np.array([["a", "b"], ["a", "c"]])
+    X = np.array([[1, 2], [3, 4]])
+    lcpn.fit(X, y)
+    check_is_fitted(lcpn)
+    # predictions = lcpn.predict(X)
+    # assert_array_equal(y, predictions)
```

### Comparing `hiclass-4.3.3b1/tests/test_LocalClassifierPerParentNode.py` & `hiclass-4.3.4/tests/test_LocalClassifierPerParentNode.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import networkx as nx
 import numpy as np
 import pytest
 from numpy.testing import assert_array_equal
 from scipy.sparse import csr_matrix
 from sklearn.exceptions import NotFittedError
 from sklearn.linear_model import LogisticRegression
+from sklearn.neighbors import KNeighborsClassifier
 from sklearn.utils.estimator_checks import parametrize_with_checks
 from sklearn.utils.validation import check_is_fitted
 
 from hiclass import LocalClassifierPerParentNode
 from hiclass.ConstantClassifier import ConstantClassifier
 
 
@@ -237,7 +238,22 @@
     )
     X = ["Text 1", "Text 2"]
     y = ["a", "a"]
     lcpn.fit(X, y)
     check_is_fitted(lcpn)
     predictions = lcpn.predict(X)
     assert_array_equal(y, predictions)
+
+
+def test_knn():
+    knn = KNeighborsClassifier(
+        n_neighbors=2,
+    )
+    lcppn = LocalClassifierPerParentNode(
+        local_classifier=knn,
+    )
+    y = np.array([["a", "b"], ["a", "c"]])
+    X = np.array([[1, 2], [3, 4]])
+    lcppn.fit(X, y)
+    check_is_fitted(lcppn)
+    # predictions = lcppn.predict(X)
+    # assert_array_equal(y, predictions)
```

### Comparing `hiclass-4.3.3b1/tests/test_metrics.py` & `hiclass-4.3.4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.3.3b1/versioneer.py` & `hiclass-4.3.4/versioneer.py`

 * *Files identical despite different names*

