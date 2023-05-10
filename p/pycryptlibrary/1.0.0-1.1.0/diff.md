# Comparing `tmp/pycryptlibrary-1.0.0.tar.gz` & `tmp/pycryptlibrary-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycryptlibrary-1.0.0.tar", last modified: Wed May 10 18:16:34 2023, max compression
+gzip compressed data, was "pycryptlibrary-1.1.0.tar", last modified: Wed May 10 18:18:40 2023, max compression
```

## Comparing `pycryptlibrary-1.0.0.tar` & `pycryptlibrary-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:16:34.194368 pycryptlibrary-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-10 18:16:34.194368 pycryptlibrary-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:16:34.194368 pycryptlibrary-1.0.0/pycryptlibrary/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 18:16:33.000000 pycryptlibrary-1.0.0/pycryptlibrary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:16:34.194368 pycryptlibrary-1.0.0/pycryptlibrary.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-10 18:16:34.000000 pycryptlibrary-1.0.0/pycryptlibrary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-10 18:16:34.000000 pycryptlibrary-1.0.0/pycryptlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 18:16:34.000000 pycryptlibrary-1.0.0/pycryptlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 18:16:34.000000 pycryptlibrary-1.0.0/pycryptlibrary.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 18:16:34.194368 pycryptlibrary-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-10 18:16:33.000000 pycryptlibrary-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:18:40.921008 pycryptlibrary-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-10 18:18:40.921008 pycryptlibrary-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:18:40.921008 pycryptlibrary-1.1.0/pycryptlibrary/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-10 18:18:40.000000 pycryptlibrary-1.1.0/pycryptlibrary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:18:40.921008 pycryptlibrary-1.1.0/pycryptlibrary.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-10 18:18:40.000000 pycryptlibrary-1.1.0/pycryptlibrary.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-10 18:18:40.000000 pycryptlibrary-1.1.0/pycryptlibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 18:18:40.000000 pycryptlibrary-1.1.0/pycryptlibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 18:18:40.000000 pycryptlibrary-1.1.0/pycryptlibrary.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 18:18:40.921008 pycryptlibrary-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-10 18:18:40.000000 pycryptlibrary-1.1.0/setup.py
```

### Comparing `pycryptlibrary-1.0.0/setup.py` & `pycryptlibrary-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pycryptlibrary",
     version=VERSION,
```

