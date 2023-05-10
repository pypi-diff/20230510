# Comparing `tmp/pipsqlipkgV1-1.0.0.tar.gz` & `tmp/pipsqlipkgV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipsqlipkgV1-1.0.0.tar", last modified: Wed May 10 19:57:37 2023, max compression
+gzip compressed data, was "pipsqlipkgV1-1.1.0.tar", last modified: Wed May 10 19:59:44 2023, max compression
```

## Comparing `pipsqlipkgV1-1.0.0.tar` & `pipsqlipkgV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:57:37.724828 pipsqlipkgV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-10 19:57:37.720828 pipsqlipkgV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:57:37.720828 pipsqlipkgV1-1.0.0/pipsqlipkgV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 19:57:37.000000 pipsqlipkgV1-1.0.0/pipsqlipkgV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:57:37.720828 pipsqlipkgV1-1.0.0/pipsqlipkgV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-10 19:57:37.000000 pipsqlipkgV1-1.0.0/pipsqlipkgV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-10 19:57:37.000000 pipsqlipkgV1-1.0.0/pipsqlipkgV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 19:57:37.000000 pipsqlipkgV1-1.0.0/pipsqlipkgV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 19:57:37.000000 pipsqlipkgV1-1.0.0/pipsqlipkgV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:57:37.724828 pipsqlipkgV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-10 19:57:37.000000 pipsqlipkgV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:59:44.351523 pipsqlipkgV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-10 19:59:44.351523 pipsqlipkgV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:59:44.351523 pipsqlipkgV1-1.1.0/pipsqlipkgV1/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-10 19:59:44.000000 pipsqlipkgV1-1.1.0/pipsqlipkgV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:59:44.351523 pipsqlipkgV1-1.1.0/pipsqlipkgV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-05-10 19:59:44.000000 pipsqlipkgV1-1.1.0/pipsqlipkgV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-10 19:59:44.000000 pipsqlipkgV1-1.1.0/pipsqlipkgV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 19:59:44.000000 pipsqlipkgV1-1.1.0/pipsqlipkgV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-10 19:59:44.000000 pipsqlipkgV1-1.1.0/pipsqlipkgV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:59:44.351523 pipsqlipkgV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-10 19:59:44.000000 pipsqlipkgV1-1.1.0/setup.py
```

### Comparing `pipsqlipkgV1-1.0.0/setup.py` & `pipsqlipkgV1-1.1.0/setup.py`

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
     name="pipsqlipkgV1",
     version=VERSION,
```

