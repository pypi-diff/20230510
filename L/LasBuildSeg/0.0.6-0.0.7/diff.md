# Comparing `tmp/LasBuildSeg-0.0.6.tar.gz` & `tmp/LasBuildSeg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.0.6.tar", last modified: Wed May 10 07:20:26 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.0.7.tar", last modified: Wed May 10 08:14:28 2023, max compression
```

## Comparing `LasBuildSeg-0.0.6.tar` & `LasBuildSeg-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 07:20:26.753909 LasBuildSeg-0.0.6/
--rw-rw-rw-   0        0        0      104 2023-05-10 07:20:02.000000 LasBuildSeg-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.6/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 07:20:26.695117 LasBuildSeg-0.0.6/LasBuildSeg/
--rw-rw-rw-   0        0        0    10755 2023-05-10 07:20:00.000000 LasBuildSeg-0.0.6/LasBuildSeg/__init__.py
--rw-rw-rw-   0        0        0    10850 2023-05-10 06:36:12.000000 LasBuildSeg-0.0.6/LasBuildSeg/all.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:20:26.747928 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0      987 2023-05-10 07:20:25.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-10 07:20:26.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 07:20:25.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-05-10 07:20:25.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 07:20:25.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       25 2022-09-19 08:00:05.000000 LasBuildSeg-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      987 2023-05-10 07:20:26.751922 LasBuildSeg-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-05-09 08:44:47.000000 LasBuildSeg-0.0.6/README.md
--rw-rw-rw-   0        0        0     1495 2023-05-10 07:20:11.000000 LasBuildSeg-0.0.6/Setup.py
--rw-rw-rw-   0        0        0      106 2023-05-10 07:11:46.000000 LasBuildSeg-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 07:20:26.754913 LasBuildSeg-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 08:14:28.396319 LasBuildSeg-0.0.7/
+-rw-rw-rw-   0        0        0      103 2023-05-10 08:04:35.000000 LasBuildSeg-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.7/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 08:14:28.339498 LasBuildSeg-0.0.7/LasBuildSeg/
+-rw-rw-rw-   0        0        0    10850 2023-05-10 08:04:56.000000 LasBuildSeg-0.0.7/LasBuildSeg/LasBuild.py
+-rw-rw-rw-   0        0        0    10663 2023-05-10 08:13:55.000000 LasBuildSeg-0.0.7/LasBuildSeg/LasBuildSeg.py
+-rw-rw-rw-   0        0        0      365 2023-05-10 08:13:43.000000 LasBuildSeg-0.0.7/LasBuildSeg/__init__.py
+-rw-rw-rw-   0        0        0    10850 2023-05-10 06:36:12.000000 LasBuildSeg-0.0.7/LasBuildSeg/all.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:14:28.390329 LasBuildSeg-0.0.7/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0      987 2023-05-10 08:14:26.000000 LasBuildSeg-0.0.7/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-05-10 08:14:27.000000 LasBuildSeg-0.0.7/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:14:26.000000 LasBuildSeg-0.0.7/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-05-10 08:14:26.000000 LasBuildSeg-0.0.7/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 08:14:26.000000 LasBuildSeg-0.0.7/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       25 2022-09-19 08:00:05.000000 LasBuildSeg-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      987 2023-05-10 08:14:28.394315 LasBuildSeg-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-05-09 08:44:47.000000 LasBuildSeg-0.0.7/README.md
+-rw-rw-rw-   0        0        0     1495 2023-05-10 08:04:41.000000 LasBuildSeg-0.0.7/Setup.py
+-rw-rw-rw-   0        0        0      106 2023-05-10 07:11:46.000000 LasBuildSeg-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:14:28.397306 LasBuildSeg-0.0.7/setup.cfg
```

### Comparing `LasBuildSeg-0.0.6/LICENSE.txt` & `LasBuildSeg-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.6/LasBuildSeg/__init__.py` & `LasBuildSeg-0.0.7/LasBuildSeg/LasBuildSeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue May  9 22:35:31 2023
-
-@author: Mertcan
-"""
 
 from rasterio.transform import from_origin
 import scipy
 from rasterio.warp import calculate_default_transform, reproject, Resampling
 
 
 import laspy
```

### Comparing `LasBuildSeg-0.0.6/LasBuildSeg/all.py` & `LasBuildSeg-0.0.7/LasBuildSeg/LasBuild.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.6/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.0.7/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.6
+Version: 0.0.7
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.0.6/PKG-INFO` & `LasBuildSeg-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.6
+Version: 0.0.7
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.0.6/Setup.py` & `LasBuildSeg-0.0.7/Setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.0.6',
+  version='0.0.7',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

