# Comparing `tmp/FuzzyPySeg-0.3.tar.gz` & `tmp/FuzzyPySeg-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuzzyPySeg-0.3.tar", last modified: Wed May  3 03:59:29 2023, max compression
+gzip compressed data, was "FuzzyPySeg-1.0.tar", last modified: Wed May 10 02:09:20 2023, max compression
```

## Comparing `FuzzyPySeg-0.3.tar` & `FuzzyPySeg-1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:29.874230 FuzzyPySeg-0.3/
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:29.850054 FuzzyPySeg-0.3/FuzzyPySeg/
--rw-rw-rw-   0        0        0    25128 2023-05-03 03:02:53.000000 FuzzyPySeg-0.3/FuzzyPySeg/FuzzyPySegCode.py
--rw-rw-rw-   0        0        0       21 2023-05-03 03:56:10.000000 FuzzyPySeg-0.3/FuzzyPySeg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 03:59:29.871567 FuzzyPySeg-0.3/FuzzyPySeg.egg-info/
--rw-rw-rw-   0        0        0     1112 2023-05-03 03:59:29.000000 FuzzyPySeg-0.3/FuzzyPySeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-03 03:59:29.000000 FuzzyPySeg-0.3/FuzzyPySeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 03:59:29.000000 FuzzyPySeg-0.3/FuzzyPySeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-03 03:59:29.000000 FuzzyPySeg-0.3/FuzzyPySeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 03:59:29.000000 FuzzyPySeg-0.3/FuzzyPySeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2023-05-03 02:55:20.000000 FuzzyPySeg-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1112 2023-05-03 03:59:29.874230 FuzzyPySeg-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2488 2023-05-03 03:05:54.000000 FuzzyPySeg-0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-05-03 03:59:29.880715 FuzzyPySeg-0.3/setup.cfg
--rw-rw-rw-   0        0        0     2074 2023-05-03 03:59:09.000000 FuzzyPySeg-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:09:20.695158 FuzzyPySeg-1.0/
+drwxrwxrwx   0        0        0        0 2023-05-10 02:09:20.676527 FuzzyPySeg-1.0/FuzzyPySeg/
+-rw-rw-rw-   0        0        0    25130 2023-05-10 02:01:23.000000 FuzzyPySeg-1.0/FuzzyPySeg/FuzzyPySeg.py
+-rw-rw-rw-   0        0        0       26 2023-05-10 02:01:23.000000 FuzzyPySeg-1.0/FuzzyPySeg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:09:20.693351 FuzzyPySeg-1.0/FuzzyPySeg.egg-info/
+-rw-rw-rw-   0        0        0     1124 2023-05-10 02:09:20.000000 FuzzyPySeg-1.0/FuzzyPySeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-10 02:09:20.000000 FuzzyPySeg-1.0/FuzzyPySeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 02:09:20.000000 FuzzyPySeg-1.0/FuzzyPySeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-10 02:09:20.000000 FuzzyPySeg-1.0/FuzzyPySeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-10 02:09:20.000000 FuzzyPySeg-1.0/FuzzyPySeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1077 2023-05-10 02:01:23.000000 FuzzyPySeg-1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1124 2023-05-10 02:09:20.695158 FuzzyPySeg-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2488 2023-05-10 02:01:23.000000 FuzzyPySeg-1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-10 02:09:20.697480 FuzzyPySeg-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2023-05-10 02:08:51.000000 FuzzyPySeg-1.0/setup.py
```

### Comparing `FuzzyPySeg-0.3/FuzzyPySeg/FuzzyPySegCode.py` & `FuzzyPySeg-1.0/FuzzyPySeg/FuzzyPySeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,7 +696,8 @@
 
     images = [Image.fromarray(group.astype(np.uint8),mode="RGB") for group in copies]
 
     group_num = 0
     for image in images:
         image.save(save_to_path + "/group"+str(group_num)+"_FCM_M.jpeg")
         group_num += 1
+
```

### Comparing `FuzzyPySeg-0.3/FuzzyPySeg.egg-info/PKG-INFO` & `FuzzyPySeg-1.0/FuzzyPySeg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: FuzzyPySeg
-Version: 0.3
+Version: 1.0
 Summary: FuzzyPySeg is a package for segmenting images using Fuzzy C Means clustering with either a Euclidean or Mahalanobis distance. You may also specify a centroid initialization using the firefly algorithm, genetic algorithm, or the Biogeography-based optimization algorithm.
 Home-page: https://github.com/Danyulll/FuzzyPySeg
-Download-URL: https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v1.0.0.tar.gz
 Author: Daniel Krasnov
 Author-email: dkrasnov@student.ubc.ca
 License: MIT
 Keywords: image segmentation,clustering,fuzzy c-means,firefly algorithm,genetic algorithm,biogeography-based optimization algorithm
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `FuzzyPySeg-0.3/LICENSE.txt` & `FuzzyPySeg-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FuzzyPySeg-0.3/PKG-INFO` & `FuzzyPySeg-1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: FuzzyPySeg
-Version: 0.3
+Version: 1.0
 Summary: FuzzyPySeg is a package for segmenting images using Fuzzy C Means clustering with either a Euclidean or Mahalanobis distance. You may also specify a centroid initialization using the firefly algorithm, genetic algorithm, or the Biogeography-based optimization algorithm.
 Home-page: https://github.com/Danyulll/FuzzyPySeg
-Download-URL: https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v0.0.3.tar.gz
+Download-URL: https://github.com/Danyulll/FuzzyPySeg/archive/refs/tags/v1.0.0.tar.gz
 Author: Daniel Krasnov
 Author-email: dkrasnov@student.ubc.ca
 License: MIT
 Keywords: image segmentation,clustering,fuzzy c-means,firefly algorithm,genetic algorithm,biogeography-based optimization algorithm
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `FuzzyPySeg-0.3/README.md` & `FuzzyPySeg-1.0/README.md`

 * *Files identical despite different names*

