# Comparing `tmp/pipcolouringskits-1.0.0.tar.gz` & `tmp/pipcolouringskits-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcolouringskits-1.0.0.tar", last modified: Wed May 10 19:44:54 2023, max compression
+gzip compressed data, was "pipcolouringskits-1.1.0.tar", last modified: Wed May 10 19:47:02 2023, max compression
```

## Comparing `pipcolouringskits-1.0.0.tar` & `pipcolouringskits-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:44:54.012524 pipcolouringskits-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-10 19:44:54.012524 pipcolouringskits-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:44:54.012524 pipcolouringskits-1.0.0/pipcolouringskits/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 19:44:53.000000 pipcolouringskits-1.0.0/pipcolouringskits/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:44:54.012524 pipcolouringskits-1.0.0/pipcolouringskits.egg-info/
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-10 19:44:53.000000 pipcolouringskits-1.0.0/pipcolouringskits.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-10 19:44:53.000000 pipcolouringskits-1.0.0/pipcolouringskits.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 19:44:53.000000 pipcolouringskits-1.0.0/pipcolouringskits.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-10 19:44:53.000000 pipcolouringskits-1.0.0/pipcolouringskits.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:44:54.012524 pipcolouringskits-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      563 2023-05-10 19:44:53.000000 pipcolouringskits-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:47:02.187266 pipcolouringskits-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-10 19:47:02.187266 pipcolouringskits-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:47:02.187266 pipcolouringskits-1.1.0/pipcolouringskits/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-10 19:47:01.000000 pipcolouringskits-1.1.0/pipcolouringskits/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:47:02.187266 pipcolouringskits-1.1.0/pipcolouringskits.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-10 19:47:02.000000 pipcolouringskits-1.1.0/pipcolouringskits.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-10 19:47:02.000000 pipcolouringskits-1.1.0/pipcolouringskits.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 19:47:02.000000 pipcolouringskits-1.1.0/pipcolouringskits.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-10 19:47:02.000000 pipcolouringskits-1.1.0/pipcolouringskits.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:47:02.187266 pipcolouringskits-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      563 2023-05-10 19:47:01.000000 pipcolouringskits-1.1.0/setup.py
```

### Comparing `pipcolouringskits-1.0.0/setup.py` & `pipcolouringskits-1.1.0/setup.py`

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
     name="pipcolouringskits",
     version=VERSION,
```

