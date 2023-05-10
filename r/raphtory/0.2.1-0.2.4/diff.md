# Comparing `tmp/raphtory-0.2.1-cp39-none-win_amd64.whl.zip` & `tmp/raphtory-0.2.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2846821 bytes, number of entries: 7
--rw-r--r--  4.6 unx     9743 b- defN 23-May-09 16:35 raphtory-0.2.1.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-May-09 16:35 raphtory-0.2.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     2052 b- defN 23-May-09 16:35 raphtory/nullmodels.py
--rw-r--r--  4.6 unx     7531 b- defN 23-May-09 16:35 raphtory/vis.py
--rw-r--r--  4.6 unx      537 b- defN 23-May-09 16:35 raphtory/__init__.py
--rwxr-xr-x  4.6 unx  8145920 b- defN 23-May-09 16:35 raphtory/raphtory.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      532 b- defN 23-May-09 16:35 raphtory-0.2.1.dist-info/RECORD
-7 files, 8166410 bytes uncompressed, 2845893 bytes compressed:  65.2%
+Zip file size: 2847832 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     9743 b- defN 23-May-10 10:25 raphtory-0.2.4.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-May-10 10:25 raphtory-0.2.4.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2052 b- defN 23-May-10 10:25 raphtory/nullmodels.py
+-rw-r--r--  4.6 unx     7531 b- defN 23-May-10 10:25 raphtory/vis.py
+-rw-r--r--  4.6 unx      537 b- defN 23-May-10 10:25 raphtory/__init__.py
+-rwxr-xr-x  4.6 unx  8151040 b- defN 23-May-10 10:25 raphtory/raphtory.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      532 b- defN 23-May-10 10:25 raphtory-0.2.4.dist-info/RECORD
+7 files, 8171530 bytes uncompressed, 2846904 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: raphtory-0.2.1.dist-info/METADATA
+Filename: raphtory-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: raphtory-0.2.1.dist-info/WHEEL
+Filename: raphtory-0.2.4.dist-info/WHEEL
 Comment: 
 
 Filename: raphtory/nullmodels.py
 Comment: 
 
 Filename: raphtory/vis.py
 Comment: 
 
 Filename: raphtory/__init__.py
 Comment: 
 
 Filename: raphtory/raphtory.cp39-win_amd64.pyd
 Comment: 
 
-Filename: raphtory-0.2.1.dist-info/RECORD
+Filename: raphtory-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `raphtory-0.2.1.dist-info/METADATA` & `raphtory-0.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raphtory
-Version: 0.2.1
+Version: 0.2.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=1.3.3
 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
 Requires-Dist: networkx >=2.6.3 ; extra == 'vis'
 Requires-Dist: matplotlib >=3.4.3 ; extra == 'vis'
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: raphtory Version: 0.2.1 Classifier: Programming
+Metadata-Version: 2.1 Name: raphtory Version: 0.2.4 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=1.3.3 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
 Requires-Dist: networkx >=2.6.3 ; extra == 'vis' Requires-Dist: matplotlib
 >=3.4.3 ; extra == 'vis' Requires-Dist: seaborn >=0.11.2 ; extra == 'vis'
 Provides-Extra: vis Summary: Python package for raphtory, a temporal graph
 library Keywords: graph,temporal-graph,temporal Home-Page: https://github.com/
```

