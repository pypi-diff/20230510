# Comparing `tmp/pycolouringsV1-1.0.0.tar.gz` & `tmp/pycolouringsV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolouringsV1-1.0.0.tar", last modified: Tue May  9 22:11:02 2023, max compression
+gzip compressed data, was "pycolouringsV1-1.1.0.tar", last modified: Tue May  9 22:13:09 2023, max compression
```

## Comparing `pycolouringsV1-1.0.0.tar` & `pycolouringsV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:11:02.385599 pycolouringsV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-09 22:11:02.385599 pycolouringsV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:11:02.385599 pycolouringsV1-1.0.0/pycolouringsV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-09 22:11:02.000000 pycolouringsV1-1.0.0/pycolouringsV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:11:02.385599 pycolouringsV1-1.0.0/pycolouringsV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-09 22:11:02.000000 pycolouringsV1-1.0.0/pycolouringsV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-09 22:11:02.000000 pycolouringsV1-1.0.0/pycolouringsV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 22:11:02.000000 pycolouringsV1-1.0.0/pycolouringsV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-09 22:11:02.000000 pycolouringsV1-1.0.0/pycolouringsV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 22:11:02.385599 pycolouringsV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-09 22:11:02.000000 pycolouringsV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:13:09.164236 pycolouringsV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-09 22:13:09.164236 pycolouringsV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:13:09.160236 pycolouringsV1-1.1.0/pycolouringsV1/
+-rw-r--r--   0 root         (0) root         (0)    97161 2023-05-09 22:13:08.000000 pycolouringsV1-1.1.0/pycolouringsV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:13:09.164236 pycolouringsV1-1.1.0/pycolouringsV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-09 22:13:09.000000 pycolouringsV1-1.1.0/pycolouringsV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-09 22:13:09.000000 pycolouringsV1-1.1.0/pycolouringsV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 22:13:09.000000 pycolouringsV1-1.1.0/pycolouringsV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-09 22:13:09.000000 pycolouringsV1-1.1.0/pycolouringsV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 22:13:09.164236 pycolouringsV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-09 22:13:08.000000 pycolouringsV1-1.1.0/setup.py
```

### Comparing `pycolouringsV1-1.0.0/setup.py` & `pycolouringsV1-1.1.0/setup.py`

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
     name="pycolouringsV1",
     version=VERSION,
```

