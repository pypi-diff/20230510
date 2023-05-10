# Comparing `tmp/LasBuildSeg-0.0.5.tar.gz` & `tmp/LasBuildSeg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.0.5.tar", last modified: Wed May 10 07:12:34 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.0.6.tar", last modified: Wed May 10 07:20:26 2023, max compression
```

## Comparing `LasBuildSeg-0.0.5.tar` & `LasBuildSeg-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 07:12:34.805476 LasBuildSeg-0.0.5/
--rw-rw-rw-   0        0        0      104 2023-05-10 07:03:57.000000 LasBuildSeg-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.5/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 07:12:34.745669 LasBuildSeg-0.0.5/LasBuildSeg/
--rw-rw-rw-   0        0        0       91 2023-05-09 19:12:51.000000 LasBuildSeg-0.0.5/LasBuildSeg/__init__.py
--rw-rw-rw-   0        0        0    10850 2023-05-10 06:36:12.000000 LasBuildSeg-0.0.5/LasBuildSeg/all.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:12:34.799489 LasBuildSeg-0.0.5/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0      987 2023-05-10 07:12:33.000000 LasBuildSeg-0.0.5/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-10 07:12:34.000000 LasBuildSeg-0.0.5/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 07:12:33.000000 LasBuildSeg-0.0.5/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-05-10 07:12:33.000000 LasBuildSeg-0.0.5/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 07:12:33.000000 LasBuildSeg-0.0.5/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       25 2022-09-19 08:00:05.000000 LasBuildSeg-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      987 2023-05-10 07:12:34.803489 LasBuildSeg-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-05-09 08:44:47.000000 LasBuildSeg-0.0.5/README.md
--rw-rw-rw-   0        0        0     1495 2023-05-10 07:11:59.000000 LasBuildSeg-0.0.5/Setup.py
--rw-rw-rw-   0        0        0      106 2023-05-10 07:11:46.000000 LasBuildSeg-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 07:12:34.805476 LasBuildSeg-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 07:20:26.753909 LasBuildSeg-0.0.6/
+-rw-rw-rw-   0        0        0      104 2023-05-10 07:20:02.000000 LasBuildSeg-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.6/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 07:20:26.695117 LasBuildSeg-0.0.6/LasBuildSeg/
+-rw-rw-rw-   0        0        0    10755 2023-05-10 07:20:00.000000 LasBuildSeg-0.0.6/LasBuildSeg/__init__.py
+-rw-rw-rw-   0        0        0    10850 2023-05-10 06:36:12.000000 LasBuildSeg-0.0.6/LasBuildSeg/all.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:20:26.747928 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0      987 2023-05-10 07:20:25.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-10 07:20:26.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 07:20:25.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-05-10 07:20:25.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 07:20:25.000000 LasBuildSeg-0.0.6/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       25 2022-09-19 08:00:05.000000 LasBuildSeg-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      987 2023-05-10 07:20:26.751922 LasBuildSeg-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-05-09 08:44:47.000000 LasBuildSeg-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1495 2023-05-10 07:20:11.000000 LasBuildSeg-0.0.6/Setup.py
+-rw-rw-rw-   0        0        0      106 2023-05-10 07:11:46.000000 LasBuildSeg-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 07:20:26.754913 LasBuildSeg-0.0.6/setup.cfg
```

### Comparing `LasBuildSeg-0.0.5/LICENSE.txt` & `LasBuildSeg-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.5/LasBuildSeg/all.py` & `LasBuildSeg-0.0.6/LasBuildSeg/all.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.5/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.0.6/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.5
+Version: 0.0.6
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.0.5/PKG-INFO` & `LasBuildSeg-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.5
+Version: 0.0.6
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.0.5/Setup.py` & `LasBuildSeg-0.0.6/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.0.5',
+  version='0.0.6',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

