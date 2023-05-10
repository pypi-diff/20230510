# Comparing `tmp/frequency_feature_map_visualization-0.2.0.tar.gz` & `tmp/frequency_feature_map_visualization-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequency_feature_map_visualization-0.2.0.tar", last modified: Wed May 10 15:12:33 2023, max compression
+gzip compressed data, was "frequency_feature_map_visualization-0.3.0.tar", last modified: Wed May 10 15:36:21 2023, max compression
```

## Comparing `frequency_feature_map_visualization-0.2.0.tar` & `frequency_feature_map_visualization-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-10 15:12:33.458702 frequency_feature_map_visualization-0.2.0/
--rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-10 15:12:33.458515 frequency_feature_map_visualization-0.2.0/PKG-INFO
-drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-10 15:12:33.458310 frequency_feature_map_visualization-0.2.0/frequency_feature_map_visualization.egg-info/
--rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-10 15:12:33.000000 frequency_feature_map_visualization-0.2.0/frequency_feature_map_visualization.egg-info/PKG-INFO
--rw-r--r--   0 fuguanghui   (501) staff       (20)      302 2023-05-10 15:12:33.000000 frequency_feature_map_visualization-0.2.0/frequency_feature_map_visualization.egg-info/SOURCES.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)        1 2023-05-10 15:12:33.000000 frequency_feature_map_visualization-0.2.0/frequency_feature_map_visualization.egg-info/dependency_links.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)       23 2023-05-10 15:12:33.000000 frequency_feature_map_visualization-0.2.0/frequency_feature_map_visualization.egg-info/requires.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)        1 2023-05-10 15:12:33.000000 frequency_feature_map_visualization-0.2.0/frequency_feature_map_visualization.egg-info/top_level.txt
--rw-r--r--   0 fuguanghui   (501) staff       (20)       38 2023-05-10 15:12:33.458746 frequency_feature_map_visualization-0.2.0/setup.cfg
--rw-rw-r--   0 fuguanghui   (501) staff       (20)      689 2023-05-10 15:10:33.000000 frequency_feature_map_visualization-0.2.0/setup.py
+drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-10 15:36:21.336923 frequency_feature_map_visualization-0.3.0/
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-10 15:36:21.336715 frequency_feature_map_visualization-0.3.0/PKG-INFO
+drwxr-xr-x   0 fuguanghui   (501) staff       (20)        0 2023-05-10 15:36:21.336495 frequency_feature_map_visualization-0.3.0/frequency_feature_map_visualization.egg-info/
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      530 2023-05-10 15:36:21.000000 frequency_feature_map_visualization-0.3.0/frequency_feature_map_visualization.egg-info/PKG-INFO
+-rw-r--r--   0 fuguanghui   (501) staff       (20)      302 2023-05-10 15:36:21.000000 frequency_feature_map_visualization-0.3.0/frequency_feature_map_visualization.egg-info/SOURCES.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)        1 2023-05-10 15:36:21.000000 frequency_feature_map_visualization-0.3.0/frequency_feature_map_visualization.egg-info/dependency_links.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)       23 2023-05-10 15:36:21.000000 frequency_feature_map_visualization-0.3.0/frequency_feature_map_visualization.egg-info/requires.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)        1 2023-05-10 15:36:21.000000 frequency_feature_map_visualization-0.3.0/frequency_feature_map_visualization.egg-info/top_level.txt
+-rw-r--r--   0 fuguanghui   (501) staff       (20)       38 2023-05-10 15:36:21.336970 frequency_feature_map_visualization-0.3.0/setup.cfg
+-rw-rw-r--   0 fuguanghui   (501) staff       (20)      689 2023-05-10 15:36:17.000000 frequency_feature_map_visualization-0.3.0/setup.py
```

### Comparing `frequency_feature_map_visualization-0.2.0/PKG-INFO` & `frequency_feature_map_visualization-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequency_feature_map_visualization
-Version: 0.2.0
+Version: 0.3.0
 Summary: This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.
 Home-page: UNKNOWN
 Author: Guanghui FU
 Author-email: aslanfu123@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `frequency_feature_map_visualization-0.2.0/frequency_feature_map_visualization.egg-info/PKG-INFO` & `frequency_feature_map_visualization-0.3.0/frequency_feature_map_visualization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequency-feature-map-visualization
-Version: 0.2.0
+Version: 0.3.0
 Summary: This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.
 Home-page: UNKNOWN
 Author: Guanghui FU
 Author-email: aslanfu123@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `frequency_feature_map_visualization-0.2.0/setup.py` & `frequency_feature_map_visualization-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="frequency_feature_map_visualization",
-    version="0.2.0",
+    version="0.3.0",
     description="This code is designed to visualize and save the feature maps of 3D and 2D models. The feature maps can be viewed in the image domain and frequency domain, and saved as .npy files.",
     author="Guanghui FU",
     author_email="aslanfu123@gmail.com",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "torch",
```

