# Comparing `tmp/PicsToPdfs-0.3.5.tar.gz` & `tmp/PicsToPdfs-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PicsToPdfs-0.3.5.tar", last modified: Sat May  6 08:10:28 2023, max compression
+gzip compressed data, was "PicsToPdfs-0.3.6.tar", last modified: Wed May 10 01:37:30 2023, max compression
```

## Comparing `PicsToPdfs-0.3.5.tar` & `PicsToPdfs-0.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.534897 PicsToPdfs-0.3.5/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0      387 2023-05-06 08:10:28.534897 PicsToPdfs-0.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.519895 PicsToPdfs-0.3.5/PicsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.528898 PicsToPdfs-0.3.5/PicsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.5/PicsToPdfs/Function/__init__.py
--rw-rw-rw-   0        0        0    59904 2023-04-28 06:28:35.000000 PicsToPdfs-0.3.5/PicsToPdfs/Function/imgToPdf.pyd
--rw-rw-rw-   0        0        0   110592 2023-05-06 08:08:30.000000 PicsToPdfs-0.3.5/PicsToPdfs/PicsToPdfs.pyd
-drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.533938 PicsToPdfs-0.3.5/PicsToPdfs/Ui/
--rw-rw-rw-   0        0        0    79360 2023-04-28 06:28:53.000000 PicsToPdfs-0.3.5/PicsToPdfs/Ui/PicToPdfUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.5/PicsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.5/PicsToPdfs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:10:28.524895 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      387 2023-05-06 08:10:28.000000 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-06 08:10:28.000000 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 08:10:28.000000 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 08:10:28.000000 PicsToPdfs-0.3.5/PicsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.5/README.md
--rw-rw-rw-   0        0        0      135 2023-05-06 08:10:28.535894 PicsToPdfs-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-06 08:10:19.000000 PicsToPdfs-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:37:30.814199 PicsToPdfs-0.3.6/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      387 2023-05-10 01:37:30.814339 PicsToPdfs-0.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 01:37:30.769400 PicsToPdfs-0.3.6/PicsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-05-10 01:37:30.802340 PicsToPdfs-0.3.6/PicsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.6/PicsToPdfs/Function/__init__.py
+-rw-rw-rw-   0        0        0    59904 2023-04-28 06:28:35.000000 PicsToPdfs-0.3.6/PicsToPdfs/Function/imgToPdf.pyd
+-rw-rw-rw-   0        0        0   110592 2023-05-10 01:29:00.000000 PicsToPdfs-0.3.6/PicsToPdfs/PicsToPdfs.pyd
+drwxrwxrwx   0        0        0        0 2023-05-10 01:37:30.810341 PicsToPdfs-0.3.6/PicsToPdfs/Ui/
+-rw-rw-rw-   0        0        0    79360 2023-04-28 06:28:53.000000 PicsToPdfs-0.3.6/PicsToPdfs/Ui/PicToPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.6/PicsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.6/PicsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:37:30.793346 PicsToPdfs-0.3.6/PicsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      387 2023-05-10 01:37:30.000000 PicsToPdfs-0.3.6/PicsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-05-10 01:37:30.000000 PicsToPdfs-0.3.6/PicsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:37:30.000000 PicsToPdfs-0.3.6/PicsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-10 01:37:30.000000 PicsToPdfs-0.3.6/PicsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.6/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-10 01:37:30.816345 PicsToPdfs-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-10 01:35:49.000000 PicsToPdfs-0.3.6/setup.py
```

### Comparing `PicsToPdfs-0.3.5/LICENSE.txt` & `PicsToPdfs-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PicsToPdfs-0.3.5/setup.py` & `PicsToPdfs-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 5
+PATCH = 6
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "PicsToPdfs",
```

