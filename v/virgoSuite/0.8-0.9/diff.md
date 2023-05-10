# Comparing `tmp/virgoSuite-0.8.tar.gz` & `tmp/virgoSuite-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgoSuite-0.8.tar", last modified: Wed May 10 12:27:02 2023, max compression
+gzip compressed data, was "virgoSuite-0.9.tar", last modified: Wed May 10 12:37:10 2023, max compression
```

## Comparing `virgoSuite-0.8.tar` & `virgoSuite-0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:27:02.902916 virgoSuite-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 12:26:48.000000 virgoSuite-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 12:27:02.902916 virgoSuite-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 12:26:48.000000 virgoSuite-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:27:02.902916 virgoSuite-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 12:26:48.000000 virgoSuite-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:27:02.902916 virgoSuite-0.8/virgoSuite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 12:27:02.000000 virgoSuite-0.8/virgoSuite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 12:27:02.000000 virgoSuite-0.8/virgoSuite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:27:02.000000 virgoSuite-0.8/virgoSuite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:27:02.000000 virgoSuite-0.8/virgoSuite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:37:10.848439 virgoSuite-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 12:36:51.000000 virgoSuite-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 12:37:10.848439 virgoSuite-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 12:36:51.000000 virgoSuite-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:37:10.848439 virgoSuite-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 12:36:51.000000 virgoSuite-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:37:10.848439 virgoSuite-0.9/virgoSuite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 12:37:10.000000 virgoSuite-0.9/virgoSuite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 12:37:10.000000 virgoSuite-0.9/virgoSuite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:37:10.000000 virgoSuite-0.9/virgoSuite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:37:10.000000 virgoSuite-0.9/virgoSuite.egg-info/top_level.txt
```

### Comparing `virgoSuite-0.8/LICENSE` & `virgoSuite-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `virgoSuite-0.8/setup.py` & `virgoSuite-0.9/setup.py`

 * *Files identical despite different names*

