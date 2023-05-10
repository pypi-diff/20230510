# Comparing `tmp/brain-loop-search-0.1.1.tar.gz` & `tmp/brain-loop-search-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brain-loop-search-0.1.1.tar", last modified: Wed May 10 10:09:00 2023, max compression
+gzip compressed data, was "brain-loop-search-0.1.2.tar", last modified: Wed May 10 10:14:26 2023, max compression
```

## Comparing `brain-loop-search-0.1.1.tar` & `brain-loop-search-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:09:00.345746 brain-loop-search-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:09:00.304851 brain-loop-search-0.1.1/.github/
--rw-rw-rw-   0        0        0        6 2023-05-10 08:58:56.000000 brain-loop-search-0.1.1/.github/python-version.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:09:00.306846 brain-loop-search-0.1.1/.github/workflows/
--rw-rw-rw-   0        0        0     1447 2023-05-10 08:58:56.000000 brain-loop-search-0.1.1/.github/workflows/static.yml
--rw-rw-rw-   0        0        0     1935 2023-05-10 08:56:44.000000 brain-loop-search-0.1.1/.gitignore
--rw-rw-rw-   0        0        0     1096 2023-04-19 10:12:56.000000 brain-loop-search-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       22 2023-04-19 07:47:30.000000 brain-loop-search-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4962 2023-05-10 10:09:00.345746 brain-loop-search-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4285 2023-05-10 09:56:09.000000 brain-loop-search-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 10:09:00.316844 brain-loop-search-0.1.1/brain_loop_search/
--rw-rw-rw-   0        0        0      290 2023-05-10 05:16:54.000000 brain-loop-search-0.1.1/brain_loop_search/__init__.py
--rw-rw-rw-   0        0        0    10889 2023-05-10 09:11:32.000000 brain-loop-search-0.1.1/brain_loop_search/brain_utils.py
--rw-rw-rw-   0        0        0    13153 2023-05-03 17:31:38.000000 brain-loop-search-0.1.1/brain_loop_search/packing.py
--rw-rw-rw-   0        0        0    19645 2023-05-10 05:50:08.000000 brain-loop-search-0.1.1/brain_loop_search/search.py
--rw-rw-rw-   0        0        0    65506 2023-02-01 17:02:57.000000 brain-loop-search-0.1.1/brain_loop_search/structures.csv
-drwxrwxrwx   0        0        0        0 2023-05-10 10:09:00.326792 brain-loop-search-0.1.1/brain_loop_search.egg-info/
--rw-rw-rw-   0        0        0     4962 2023-05-10 10:09:00.000000 brain-loop-search-0.1.1/brain_loop_search.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-05-10 10:09:00.000000 brain-loop-search-0.1.1/brain_loop_search.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:09:00.000000 brain-loop-search-0.1.1/brain_loop_search.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-10 10:09:00.000000 brain-loop-search-0.1.1/brain_loop_search.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-10 10:09:00.000000 brain-loop-search-0.1.1/brain_loop_search.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      984 2023-05-10 08:55:45.000000 brain-loop-search-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 10:09:00.345746 brain-loop-search-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 10:09:00.343751 brain-loop-search-0.1.1/test/
--rw-rw-rw-   0        0        0   144508 2023-05-10 08:22:30.000000 brain-loop-search-0.1.1/test/test.png
--rw-rw-rw-   0        0        0   143835 2023-05-10 09:11:39.000000 brain-loop-search-0.1.1/test/test2.png
--rw-rw-rw-   0        0        0     1359 2023-05-10 05:50:08.000000 brain-loop-search-0.1.1/test/test_flow.py
--rw-rw-rw-   0        0        0     2818 2023-05-04 13:57:31.000000 brain-loop-search-0.1.1/test/test_graph_packing.py
--rw-rw-rw-   0        0        0     1128 2023-05-04 13:57:31.000000 brain-loop-search-0.1.1/test/test_ontology.py
--rw-rw-rw-   0        0        0     3588 2023-05-10 05:43:45.000000 brain-loop-search-0.1.1/test/test_sssp.py
--rw-rw-rw-   0        0        0     3400 2023-05-04 13:57:31.000000 brain-loop-search-0.1.1/test/test_vertex_packing.py
--rw-rw-rw-   0        0        0     1135 2023-05-10 08:35:20.000000 brain-loop-search-0.1.1/test/test_vis.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:14:26.658592 brain-loop-search-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:14:26.603197 brain-loop-search-0.1.2/.github/
+-rw-rw-rw-   0        0        0        6 2023-05-10 08:58:56.000000 brain-loop-search-0.1.2/.github/python-version.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:14:26.605193 brain-loop-search-0.1.2/.github/workflows/
+-rw-rw-rw-   0        0        0     1447 2023-05-10 08:58:56.000000 brain-loop-search-0.1.2/.github/workflows/static.yml
+-rw-rw-rw-   0        0        0     1935 2023-05-10 08:56:44.000000 brain-loop-search-0.1.2/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-04-19 10:12:56.000000 brain-loop-search-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-04-19 07:47:30.000000 brain-loop-search-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4968 2023-05-10 10:14:26.657628 brain-loop-search-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4291 2023-05-10 10:11:48.000000 brain-loop-search-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 10:14:26.612082 brain-loop-search-0.1.2/brain_loop_search/
+-rw-rw-rw-   0        0        0      290 2023-05-10 05:16:54.000000 brain-loop-search-0.1.2/brain_loop_search/__init__.py
+-rw-rw-rw-   0        0        0    10889 2023-05-10 09:11:32.000000 brain-loop-search-0.1.2/brain_loop_search/brain_utils.py
+-rw-rw-rw-   0        0        0    13153 2023-05-03 17:31:38.000000 brain-loop-search-0.1.2/brain_loop_search/packing.py
+-rw-rw-rw-   0        0        0    19645 2023-05-10 05:50:08.000000 brain-loop-search-0.1.2/brain_loop_search/search.py
+-rw-rw-rw-   0        0        0    65506 2023-02-01 17:02:57.000000 brain-loop-search-0.1.2/brain_loop_search/structures.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 10:14:26.620804 brain-loop-search-0.1.2/brain_loop_search.egg-info/
+-rw-rw-rw-   0        0        0     4968 2023-05-10 10:14:26.000000 brain-loop-search-0.1.2/brain_loop_search.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-05-10 10:14:26.000000 brain-loop-search-0.1.2/brain_loop_search.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:14:26.000000 brain-loop-search-0.1.2/brain_loop_search.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-10 10:14:26.000000 brain-loop-search-0.1.2/brain_loop_search.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-10 10:14:26.000000 brain-loop-search-0.1.2/brain_loop_search.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      984 2023-05-10 08:55:45.000000 brain-loop-search-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 10:14:26.658592 brain-loop-search-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 10:14:26.655600 brain-loop-search-0.1.2/test/
+-rw-rw-rw-   0        0        0   144508 2023-05-10 08:22:30.000000 brain-loop-search-0.1.2/test/test.png
+-rw-rw-rw-   0        0        0   143835 2023-05-10 09:11:39.000000 brain-loop-search-0.1.2/test/test2.png
+-rw-rw-rw-   0        0        0     1359 2023-05-10 05:50:08.000000 brain-loop-search-0.1.2/test/test_flow.py
+-rw-rw-rw-   0        0        0     2818 2023-05-04 13:57:31.000000 brain-loop-search-0.1.2/test/test_graph_packing.py
+-rw-rw-rw-   0        0        0     1128 2023-05-04 13:57:31.000000 brain-loop-search-0.1.2/test/test_ontology.py
+-rw-rw-rw-   0        0        0     3588 2023-05-10 05:43:45.000000 brain-loop-search-0.1.2/test/test_sssp.py
+-rw-rw-rw-   0        0        0     3400 2023-05-04 13:57:31.000000 brain-loop-search-0.1.2/test/test_vertex_packing.py
+-rw-rw-rw-   0        0        0     1135 2023-05-10 08:35:20.000000 brain-loop-search-0.1.2/test/test_vis.py
```

### Comparing `brain-loop-search-0.1.1/.github/workflows/static.yml` & `brain-loop-search-0.1.2/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/.gitignore` & `brain-loop-search-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/LICENSE` & `brain-loop-search-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/PKG-INFO` & `brain-loop-search-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: brain-loop-search
-Version: 0.1.1
+Version: 0.1.2
 Summary: Screen loops among brain structures(or any entities comprising a graph).
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/brain-loop-search
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/brain-loop-search
 Keywords: neuron-morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
-# Loop Search
+# Brain Loop Search
 Tools for screening significant loop structures in a graph, typically a
 brain structure graph with physiological or anatomical edge data.
 
 ## Installation
 
 ```shell
-$ pip install brain-loop-screen
+$ pip install brain-loop-search
 ```
 
 ## Usage
 
 ### Packing a bigger graph for regions of interest
 Packing vertices:
 ```python
```

### Comparing `brain-loop-search-0.1.1/README.md` & `brain-loop-search-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Loop Search
+# Brain Loop Search
 Tools for screening significant loop structures in a graph, typically a
 brain structure graph with physiological or anatomical edge data.
 
 ## Installation
 
 ```shell
-$ pip install brain-loop-screen
+$ pip install brain-loop-search
 ```
 
 ## Usage
 
 ### Packing a bigger graph for regions of interest
 Packing vertices:
 ```python
```

### Comparing `brain-loop-search-0.1.1/brain_loop_search/brain_utils.py` & `brain-loop-search-0.1.2/brain_loop_search/brain_utils.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/brain_loop_search/packing.py` & `brain-loop-search-0.1.2/brain_loop_search/packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/brain_loop_search/search.py` & `brain-loop-search-0.1.2/brain_loop_search/search.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/brain_loop_search/structures.csv` & `brain-loop-search-0.1.2/brain_loop_search/structures.csv`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/brain_loop_search.egg-info/PKG-INFO` & `brain-loop-search-0.1.2/brain_loop_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: brain-loop-search
-Version: 0.1.1
+Version: 0.1.2
 Summary: Screen loops among brain structures(or any entities comprising a graph).
 Author-email: Zuohan Zhao <zzhmark@126.com>
 License: MIT License
 Project-URL: GitHub Project, https://github.com/SEU-ALLEN-codebase/brain-loop-search
 Project-URL: Documentation, https://SEU-ALLEN-codebase.github.io/brain-loop-search
 Keywords: neuron-morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
-# Loop Search
+# Brain Loop Search
 Tools for screening significant loop structures in a graph, typically a
 brain structure graph with physiological or anatomical edge data.
 
 ## Installation
 
 ```shell
-$ pip install brain-loop-screen
+$ pip install brain-loop-search
 ```
 
 ## Usage
 
 ### Packing a bigger graph for regions of interest
 Packing vertices:
 ```python
```

### Comparing `brain-loop-search-0.1.1/brain_loop_search.egg-info/SOURCES.txt` & `brain-loop-search-0.1.2/brain_loop_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/pyproject.toml` & `brain-loop-search-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/test/test.png` & `brain-loop-search-0.1.2/test/test.png`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/test/test2.png` & `brain-loop-search-0.1.2/test/test2.png`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/test/test_flow.py` & `brain-loop-search-0.1.2/test/test_flow.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/test/test_graph_packing.py` & `brain-loop-search-0.1.2/test/test_graph_packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/test/test_ontology.py` & `brain-loop-search-0.1.2/test/test_ontology.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/test/test_sssp.py` & `brain-loop-search-0.1.2/test/test_sssp.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/test/test_vertex_packing.py` & `brain-loop-search-0.1.2/test/test_vertex_packing.py`

 * *Files identical despite different names*

### Comparing `brain-loop-search-0.1.1/test/test_vis.py` & `brain-loop-search-0.1.2/test/test_vis.py`

 * *Files identical despite different names*

