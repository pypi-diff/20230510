# Comparing `tmp/sqlflat-1.0.tar.gz` & `tmp/sqlflat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlflat-1.0.tar", last modified: Wed May 10 13:26:25 2023, max compression
+gzip compressed data, was "sqlflat-1.0.1.tar", last modified: Wed May 10 13:47:27 2023, max compression
```

## Comparing `sqlflat-1.0.tar` & `sqlflat-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 timothee  (1000) timothee  (1000)        0 2023-05-10 13:26:25.698845 sqlflat-1.0/
--rw-rw-r--   0 timothee  (1000) timothee  (1000)     1075 2023-05-10 12:26:06.000000 sqlflat-1.0/LICENSE.md
--rw-rw-r--   0 timothee  (1000) timothee  (1000)      311 2023-05-10 13:26:25.698845 sqlflat-1.0/PKG-INFO
--rw-rw-r--   0 timothee  (1000) timothee  (1000)     1911 2023-05-10 13:14:54.000000 sqlflat-1.0/README.md
--rw-rw-r--   0 timothee  (1000) timothee  (1000)       38 2023-05-10 13:26:25.698845 sqlflat-1.0/setup.cfg
--rw-rw-r--   0 timothee  (1000) timothee  (1000)      529 2023-05-10 13:09:25.000000 sqlflat-1.0/setup.py
-drwxrwxr-x   0 timothee  (1000) timothee  (1000)        0 2023-05-10 13:26:25.698845 sqlflat-1.0/sqlflat.egg-info/
--rw-rw-r--   0 timothee  (1000) timothee  (1000)      311 2023-05-10 13:26:25.000000 sqlflat-1.0/sqlflat.egg-info/PKG-INFO
--rw-rw-r--   0 timothee  (1000) timothee  (1000)      217 2023-05-10 13:26:25.000000 sqlflat-1.0/sqlflat.egg-info/SOURCES.txt
--rw-rw-r--   0 timothee  (1000) timothee  (1000)        1 2023-05-10 13:26:25.000000 sqlflat-1.0/sqlflat.egg-info/dependency_links.txt
--rw-rw-r--   0 timothee  (1000) timothee  (1000)       49 2023-05-10 13:26:25.000000 sqlflat-1.0/sqlflat.egg-info/entry_points.txt
--rw-rw-r--   0 timothee  (1000) timothee  (1000)       17 2023-05-10 13:26:25.000000 sqlflat-1.0/sqlflat.egg-info/requires.txt
--rw-rw-r--   0 timothee  (1000) timothee  (1000)        1 2023-05-10 13:26:25.000000 sqlflat-1.0/sqlflat.egg-info/top_level.txt
+drwxrwxr-x   0 timothee  (1000) timothee  (1000)        0 2023-05-10 13:47:27.587839 sqlflat-1.0.1/
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)     1075 2023-05-10 12:26:06.000000 sqlflat-1.0.1/LICENSE.md
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)     2566 2023-05-10 13:47:27.587839 sqlflat-1.0.1/PKG-INFO
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)     1911 2023-05-10 13:14:54.000000 sqlflat-1.0.1/README.md
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)     2054 2023-05-10 13:36:28.000000 sqlflat-1.0.1/README.rst
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)       38 2023-05-10 13:47:27.587839 sqlflat-1.0.1/setup.cfg
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)      885 2023-05-10 13:47:23.000000 sqlflat-1.0.1/setup.py
+drwxrwxr-x   0 timothee  (1000) timothee  (1000)        0 2023-05-10 13:47:27.587839 sqlflat-1.0.1/sqlflat.egg-info/
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)     2566 2023-05-10 13:47:27.000000 sqlflat-1.0.1/sqlflat.egg-info/PKG-INFO
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)      228 2023-05-10 13:47:27.000000 sqlflat-1.0.1/sqlflat.egg-info/SOURCES.txt
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)        1 2023-05-10 13:47:27.000000 sqlflat-1.0.1/sqlflat.egg-info/dependency_links.txt
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)       49 2023-05-10 13:47:27.000000 sqlflat-1.0.1/sqlflat.egg-info/entry_points.txt
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)       17 2023-05-10 13:47:27.000000 sqlflat-1.0.1/sqlflat.egg-info/requires.txt
+-rw-rw-r--   0 timothee  (1000) timothee  (1000)        1 2023-05-10 13:47:27.000000 sqlflat-1.0.1/sqlflat.egg-info/top_level.txt
```

### Comparing `sqlflat-1.0/LICENSE.md` & `sqlflat-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlflat-1.0/README.md` & `sqlflat-1.0.1/README.md`

 * *Files identical despite different names*

