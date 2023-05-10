# Comparing `tmp/LasBuildSeg-0.0.3.tar.gz` & `tmp/LasBuildSeg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LasBuildSeg-0.0.3.tar", last modified: Wed May 10 07:04:19 2023, max compression
+gzip compressed data, was "LasBuildSeg-0.0.4.tar", last modified: Wed May 10 07:08:16 2023, max compression
```

## Comparing `LasBuildSeg-0.0.3.tar` & `LasBuildSeg-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:19.534964 LasBuildSeg-0.0.3/
--rw-rw-rw-   0        0        0      104 2023-05-10 07:03:57.000000 LasBuildSeg-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.3/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:19.477153 LasBuildSeg-0.0.3/LasBuildSeg/
--rw-rw-rw-   0        0        0       91 2023-05-09 19:12:51.000000 LasBuildSeg-0.0.3/LasBuildSeg/__init__.py
--rw-rw-rw-   0        0        0    10850 2023-05-10 06:36:12.000000 LasBuildSeg-0.0.3/LasBuildSeg/all.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:19.528981 LasBuildSeg-0.0.3/LasBuildSeg.egg-info/
--rw-rw-rw-   0        0        0      987 2023-05-10 07:04:18.000000 LasBuildSeg-0.0.3/LasBuildSeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-10 07:04:18.000000 LasBuildSeg-0.0.3/LasBuildSeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 07:04:18.000000 LasBuildSeg-0.0.3/LasBuildSeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-05-10 07:04:18.000000 LasBuildSeg-0.0.3/LasBuildSeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 07:04:18.000000 LasBuildSeg-0.0.3/LasBuildSeg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       25 2022-09-19 08:00:05.000000 LasBuildSeg-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      987 2023-05-10 07:04:19.531967 LasBuildSeg-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-05-09 08:44:47.000000 LasBuildSeg-0.0.3/README.md
--rw-rw-rw-   0        0        0     1495 2023-05-10 07:03:42.000000 LasBuildSeg-0.0.3/Setup.py
--rw-rw-rw-   0        0        0      103 2023-05-10 07:03:22.000000 LasBuildSeg-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 07:04:19.534964 LasBuildSeg-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 07:08:16.093452 LasBuildSeg-0.0.4/
+-rw-rw-rw-   0        0        0      104 2023-05-10 07:03:57.000000 LasBuildSeg-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    18092 2023-05-10 06:27:14.000000 LasBuildSeg-0.0.4/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 07:08:16.028137 LasBuildSeg-0.0.4/LasBuildSeg/
+-rw-rw-rw-   0        0        0       91 2023-05-09 19:12:51.000000 LasBuildSeg-0.0.4/LasBuildSeg/__init__.py
+-rw-rw-rw-   0        0        0    10850 2023-05-10 06:36:12.000000 LasBuildSeg-0.0.4/LasBuildSeg/all.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:08:16.087473 LasBuildSeg-0.0.4/LasBuildSeg.egg-info/
+-rw-rw-rw-   0        0        0      987 2023-05-10 07:08:14.000000 LasBuildSeg-0.0.4/LasBuildSeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-10 07:08:15.000000 LasBuildSeg-0.0.4/LasBuildSeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 07:08:14.000000 LasBuildSeg-0.0.4/LasBuildSeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-05-10 07:08:14.000000 LasBuildSeg-0.0.4/LasBuildSeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 07:08:14.000000 LasBuildSeg-0.0.4/LasBuildSeg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       25 2022-09-19 08:00:05.000000 LasBuildSeg-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      987 2023-05-10 07:08:16.090461 LasBuildSeg-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-05-09 08:44:47.000000 LasBuildSeg-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1495 2023-05-10 07:07:15.000000 LasBuildSeg-0.0.4/Setup.py
+-rw-rw-rw-   0        0        0      107 2023-05-10 07:07:03.000000 LasBuildSeg-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 07:08:16.093452 LasBuildSeg-0.0.4/setup.cfg
```

### Comparing `LasBuildSeg-0.0.3/LICENSE.txt` & `LasBuildSeg-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.3/LasBuildSeg/all.py` & `LasBuildSeg-0.0.4/LasBuildSeg/all.py`

 * *Files identical despite different names*

### Comparing `LasBuildSeg-0.0.3/LasBuildSeg.egg-info/PKG-INFO` & `LasBuildSeg-0.0.4/LasBuildSeg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.3
+Version: 0.0.4
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.0.3/PKG-INFO` & `LasBuildSeg-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LasBuildSeg
-Version: 0.0.3
+Version: 0.0.4
 Summary: Building Footrprint Extraction from Aerial LiDAR data
 Home-page: 
 Author: MertcanErdem
 Author-email: merak908@gmail.com
 License: GNU General Public License v2.0
 Keywords: Building,Lidar
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `LasBuildSeg-0.0.3/Setup.py` & `LasBuildSeg-0.0.4/Setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     INSTALL_REQUIRES = []
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
         
 setup(
   name='LasBuildSeg',
-  version='0.0.3',
+  version='0.0.4',
   description='Building Footrprint Extraction from Aerial LiDAR data',
   long_description=long_description,
   long_description_content_type='text/markdown',  
   url='',  
   author='MertcanErdem',
   author_email='merak908@gmail.com',
   license='GNU General Public License v2.0',
```

