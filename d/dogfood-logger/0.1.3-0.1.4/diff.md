# Comparing `tmp/dogfood-logger-0.1.3.tar.gz` & `tmp/dogfood_logger-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogfood-logger-0.1.3.tar", last modified: Wed May 10 03:44:24 2023, max compression
+gzip compressed data, was "dogfood_logger-0.1.4.tar", max compression
```

## Comparing `dogfood-logger-0.1.3.tar` & `dogfood_logger-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,7 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1087 2023-05-10 02:17:04.000000 dogfood-logger-0.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 02:17:04.000000 dogfood-logger-0.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-10 02:17:04.000000 dogfood-logger-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/dogfood_logger/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 03:18:57.000000 dogfood-logger-0.1.3/dogfood_logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-05-10 03:18:57.000000 dogfood-logger-0.1.3/dogfood_logger/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/dogfood_logger.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 03:44:24.000000 dogfood-logger-0.1.3/dogfood_logger.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      339 2023-05-10 03:43:18.000000 dogfood-logger-0.1.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-10 03:43:18.000000 dogfood-logger-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 03:44:24.599807 dogfood-logger-0.1.3/tests/
--rw-r--r--   0 root         (0) root         (0)      143 2023-05-10 02:20:45.000000 dogfood-logger-0.1.3/tests/test.py
+-rw-r--r--   0        0        0     1087 2023-05-10 02:17:04.332370 dogfood_logger-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      464 2023-05-10 02:17:04.332370 dogfood_logger-0.1.4/README.md
+-rw-r--r--   0        0        0       21 2023-05-10 03:18:57.202008 dogfood_logger-0.1.4/dogfood_logger/__init__.py
+-rw-r--r--   0        0        0     3074 2023-05-10 03:18:57.202008 dogfood_logger-0.1.4/dogfood_logger/logger.py
+-rw-r--r--   0        0        0       42 2023-05-10 02:17:04.332370 dogfood_logger-0.1.4/dogfood_logger/packageData/sampleData.dat
+-rw-r--r--   0        0        0      370 2023-05-10 03:55:15.557701 dogfood_logger-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 dogfood_logger-0.1.4/PKG-INFO
```

### Comparing `dogfood-logger-0.1.3/LICENSE.txt` & `dogfood_logger-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dogfood-logger-0.1.3/dogfood_logger/logger.py` & `dogfood_logger-0.1.4/dogfood_logger/logger.py`

 * *Files identical despite different names*

