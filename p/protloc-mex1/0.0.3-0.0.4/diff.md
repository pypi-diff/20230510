# Comparing `tmp/protloc_mex1-0.0.3.tar.gz` & `tmp/protloc_mex1-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex1-0.0.3.tar", last modified: Sat Apr 29 13:44:59 2023, max compression
+gzip compressed data, was "protloc_mex1-0.0.4.tar", last modified: Wed May 10 07:39:21 2023, max compression
```

## Comparing `protloc_mex1-0.0.3.tar` & `protloc_mex1-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 13:44:59.512865 protloc_mex1-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1143 2023-04-29 13:44:59.511358 protloc_mex1-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-04-26 08:22:56.000000 protloc_mex1-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 13:44:59.478536 protloc_mex1-0.0.3/protloc_mex1/
--rw-rw-rw-   0        0        0    12015 2023-04-25 09:31:12.000000 protloc_mex1-0.0.3/protloc_mex1/AA_count.py
--rw-rw-rw-   0        0        0     8014 2023-04-29 12:40:52.000000 protloc_mex1-0.0.3/protloc_mex1/GO_count.py
--rw-rw-rw-   0        0        0    10510 2023-04-28 13:10:04.000000 protloc_mex1-0.0.3/protloc_mex1/SHAP_conduct.py
--rw-rw-rw-   0        0        0    28926 2023-04-29 13:10:06.000000 protloc_mex1-0.0.3/protloc_mex1/SHAP_plus.py
--rw-rw-rw-   0        0        0       39 2023-04-29 12:25:34.000000 protloc_mex1-0.0.3/protloc_mex1/__init__.py
--rw-rw-rw-   0        0        0    11146 2023-04-29 13:23:26.000000 protloc_mex1-0.0.3/protloc_mex1/classifier_evalute.py
-drwxrwxrwx   0        0        0        0 2023-04-29 13:44:59.507950 protloc_mex1-0.0.3/protloc_mex1.egg-info/
--rw-rw-rw-   0        0        0     1143 2023-04-29 13:44:59.000000 protloc_mex1-0.0.3/protloc_mex1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-04-29 13:44:59.000000 protloc_mex1-0.0.3/protloc_mex1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 13:44:59.000000 protloc_mex1-0.0.3/protloc_mex1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-04-29 13:44:59.000000 protloc_mex1-0.0.3/protloc_mex1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-29 13:44:59.000000 protloc_mex1-0.0.3/protloc_mex1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      859 2023-04-29 13:37:35.000000 protloc_mex1-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 13:44:59.512865 protloc_mex1-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 07:39:21.666519 protloc_mex1-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1143 2023-05-10 07:39:21.666519 protloc_mex1-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-04-26 08:22:56.000000 protloc_mex1-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 07:39:21.622341 protloc_mex1-0.0.4/protloc_mex1/
+-rw-rw-rw-   0        0        0    14385 2023-05-08 13:54:14.000000 protloc_mex1-0.0.4/protloc_mex1/AA_count.py
+-rw-rw-rw-   0        0        0     8014 2023-04-29 12:40:52.000000 protloc_mex1-0.0.4/protloc_mex1/GO_count.py
+-rw-rw-rw-   0        0        0    10510 2023-04-28 13:10:04.000000 protloc_mex1-0.0.4/protloc_mex1/SHAP_conduct.py
+-rw-rw-rw-   0        0        0    28926 2023-04-29 13:10:06.000000 protloc_mex1-0.0.4/protloc_mex1/SHAP_plus.py
+-rw-rw-rw-   0        0        0       39 2023-04-29 12:25:34.000000 protloc_mex1-0.0.4/protloc_mex1/__init__.py
+-rw-rw-rw-   0        0        0    10886 2023-05-09 03:16:02.000000 protloc_mex1-0.0.4/protloc_mex1/classifier_evalute.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:39:21.662513 protloc_mex1-0.0.4/protloc_mex1.egg-info/
+-rw-rw-rw-   0        0        0     1143 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      859 2023-05-10 07:30:07.000000 protloc_mex1-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 07:39:21.666519 protloc_mex1-0.0.4/setup.cfg
```

### Comparing `protloc_mex1-0.0.3/LICENSE.txt` & `protloc_mex1-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.3/PKG-INFO` & `protloc_mex1-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc_mex1
-Version: 0.0.3
+Version: 0.0.4
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `protloc_mex1-0.0.3/README.md` & `protloc_mex1-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.3/protloc_mex1/AA_count.py` & `protloc_mex1-0.0.4/protloc_mex1/AA_count.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,59 @@
 
 from Bio.SeqUtils.ProtParam import ProteinAnalysis
 
 import numpy as np
 
 import re
 
-
+def dna_sequence_conduct(df):
+    
+    elements = {'C': {'A': 5, 'T': 5, 'C': 4, 'G': 5},
+                'H': {'A': 5, 'T': 6, 'C': 5, 'G': 5},
+                'N': {'A': 5, 'T': 2, 'C': 3, 'G': 5},
+                'O': {'A': 0, 'T': 2, 'C': 1, 'G': 1}}
+
+    # 过滤所有非法碱基
+    df['gene_seq'] = df['gene_seq'].apply(lambda x: ''.join([base for base in x if base in {'A', 'T', 'C', 'G'}]))
+    # 计算元素的频率
+    df['Carbon']   = df['gene_seq'].apply(lambda x: sum([elements['C'][base] for base in x]) / len(x))
+    df['Hydrogen'] = df['gene_seq'].apply(lambda x: sum([elements['H'][base] for base in x]) / len(x))
+    df['Nitrogen'] = df['gene_seq'].apply(lambda x: sum([elements['N'][base] for base in x]) / len(x))
+    df['Oxygen']   = df['gene_seq'].apply(lambda x: sum([elements['O'][base] for base in x]) / len(x))
+    # 计算碱基频率
+    df['A'] = df['gene_seq'].apply(lambda x: x.count('A') / len(x))
+    df['T'] = df['gene_seq'].apply(lambda x: x.count('T') / len(x))
+    df['G'] = df['gene_seq'].apply(lambda x: x.count('G') / len(x))
+    df['C'] = df['gene_seq'].apply(lambda x: x.count('C') / len(x))
+    
+    
+    return df
+
+def rna_sequence_conduct(df):
+    
+    elements = {'C': {'A': 5, 'U': 4, 'C': 4, 'G': 5},
+                'H': {'A': 5, 'U': 4, 'C': 5, 'G': 5},
+                'N': {'A': 5, 'U': 2, 'C': 3, 'G': 5},
+                'O': {'A': 0, 'U': 2, 'C': 1, 'G': 1}}
+
+    # 过滤所有非法碱基
+    df['gene_seq'] = df['gene_seq'].apply(lambda x: ''.join([base for base in x if base in {'A', 'U', 'C', 'G'}]))
+    # 计算元素的频率
+    df['Carbon']   = df['gene_seq'].apply(lambda x: sum([elements['C'][base] for base in x]) / len(x))
+    df['Hydrogen'] = df['gene_seq'].apply(lambda x: sum([elements['H'][base] for base in x]) / len(x))
+    df['Nitrogen'] = df['gene_seq'].apply(lambda x: sum([elements['N'][base] for base in x]) / len(x))
+    df['Oxygen']   = df['gene_seq'].apply(lambda x: sum([elements['O'][base] for base in x]) / len(x))
+    # 计算碱基频率
+    df['A'] = df['gene_seq'].apply(lambda x: x.count('A') / len(x))
+    df['U'] = df['gene_seq'].apply(lambda x: x.count('U') / len(x))
+    df['G'] = df['gene_seq'].apply(lambda x: x.count('G') / len(x))
+    df['C'] = df['gene_seq'].apply(lambda x: x.count('C') / len(x))
+    
+    
+    return df
 
 def protein_sequence_conduct(file_data, sequence_name="Sequence"):
     """
     Conduct protein sequence analysis and add relevant protein properties to an input pandas dataframe.
 
     Parameters
     ----------
```

### Comparing `protloc_mex1-0.0.3/protloc_mex1/GO_count.py` & `protloc_mex1-0.0.4/protloc_mex1/GO_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.3/protloc_mex1/SHAP_conduct.py` & `protloc_mex1-0.0.4/protloc_mex1/SHAP_conduct.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.3/protloc_mex1/SHAP_plus.py` & `protloc_mex1-0.0.4/protloc_mex1/SHAP_plus.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.3/protloc_mex1/classifier_evalute.py` & `protloc_mex1-0.0.4/protloc_mex1/classifier_evalute.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,38 +8,25 @@
 import logging
 
 from packaging import version
 import warnings
 
 try:
     import sklearn
-    sklearn_exists = True
+    if version.parse(sklearn.__version__) < version.parse('1.0.2'):
+        warnings.warn("Your sklearn version is older than 1.0.2 and may not operate correctly.")
+    from sklearn.metrics import roc_curve, auc, confusion_matrix
+    from sklearn.metrics import classification_report, accuracy_score, roc_auc_score
 except ImportError:
-    sklearn_exists = False
+    warnings.warn("Sklearn not found. Some functions will not be available.")
 
-try: 
+try:
     import mglearn
-    mglearn_exists = True 
 except ImportError:
-    mglearn_exists = False
-    
-if sklearn_exists:
-    if version.parse(sklearn.__version__) < version.parse('1.0.2'):
-        warnings.warn("Your sklearn version is older than 1.0.2  +\
-                      and may be not operation correct.")
-    from sklearn.metrics import roc_curve, auc, confusion_matrix
-    from sklearn.metrics import classification_report,accuracy_score,roc_auc_score    
-    
-else:
-    warnings.warn("Sklearn not found. Some functions will not be available.") 
-
-if mglearn_exists:
-    pass  # mglearn已导入,可以使用  
-else:
-    warnings.warn("Mglearn not found. Some functions will not be available.")  
+    warnings.warn("Mglearn not found. Some functions will not be available.")
 
     
 class ClassifierEvaluator:
     """
     A class for evaluating the performance of a classifier model.
     
     Attributes:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `protloc_mex1-0.0.3/protloc_mex1.egg-info/PKG-INFO` & `protloc_mex1-0.0.4/protloc_mex1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc-mex1
-Version: 0.0.3
+Version: 0.0.4
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `protloc_mex1-0.0.3/pyproject.toml` & `protloc_mex1-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "protloc_mex1"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ze Yu Luo", email="1024226968@qq.com" },
 ]
 description = "..."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

