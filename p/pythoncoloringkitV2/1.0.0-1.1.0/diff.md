# Comparing `tmp/pythoncoloringkitV2-1.0.0.tar.gz` & `tmp/pythoncoloringkitV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythoncoloringkitV2-1.0.0.tar", last modified: Wed May 10 18:19:12 2023, max compression
+gzip compressed data, was "pythoncoloringkitV2-1.1.0.tar", last modified: Wed May 10 18:21:20 2023, max compression
```

## Comparing `pythoncoloringkitV2-1.0.0.tar` & `pythoncoloringkitV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:19:12.912666 pythoncoloringkitV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-10 18:19:12.912666 pythoncoloringkitV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:19:12.908666 pythoncoloringkitV2-1.0.0/pythoncoloringkitV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 18:19:12.000000 pythoncoloringkitV2-1.0.0/pythoncoloringkitV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:19:12.912666 pythoncoloringkitV2-1.0.0/pythoncoloringkitV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      352 2023-05-10 18:19:12.000000 pythoncoloringkitV2-1.0.0/pythoncoloringkitV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2023-05-10 18:19:12.000000 pythoncoloringkitV2-1.0.0/pythoncoloringkitV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 18:19:12.000000 pythoncoloringkitV2-1.0.0/pythoncoloringkitV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-10 18:19:12.000000 pythoncoloringkitV2-1.0.0/pythoncoloringkitV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 18:19:12.912666 pythoncoloringkitV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-10 18:19:12.000000 pythoncoloringkitV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:21:20.247302 pythoncoloringkitV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-10 18:21:20.247302 pythoncoloringkitV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:21:20.247302 pythoncoloringkitV2-1.1.0/pythoncoloringkitV2/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-10 18:21:20.000000 pythoncoloringkitV2-1.1.0/pythoncoloringkitV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:21:20.247302 pythoncoloringkitV2-1.1.0/pythoncoloringkitV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-05-10 18:21:20.000000 pythoncoloringkitV2-1.1.0/pythoncoloringkitV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-05-10 18:21:20.000000 pythoncoloringkitV2-1.1.0/pythoncoloringkitV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 18:21:20.000000 pythoncoloringkitV2-1.1.0/pythoncoloringkitV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-10 18:21:20.000000 pythoncoloringkitV2-1.1.0/pythoncoloringkitV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 18:21:20.247302 pythoncoloringkitV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-10 18:21:20.000000 pythoncoloringkitV2-1.1.0/setup.py
```

### Comparing `pythoncoloringkitV2-1.0.0/setup.py` & `pythoncoloringkitV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pythoncoloringkitV2",
     version=VERSION,
```

