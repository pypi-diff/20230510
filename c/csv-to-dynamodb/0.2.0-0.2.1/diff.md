# Comparing `tmp/csv_to_dynamodb-0.2.0.tar.gz` & `tmp/csv_to_dynamodb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_to_dynamodb-0.2.0.tar", last modified: Tue May  9 23:30:42 2023, max compression
+gzip compressed data, was "csv_to_dynamodb-0.2.1.tar", last modified: Tue May  9 23:36:09 2023, max compression
```

## Comparing `csv_to_dynamodb-0.2.0.tar` & `csv_to_dynamodb-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:30:42.778212 csv_to_dynamodb-0.2.0/
--rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      264 2023-05-09 23:30:42.777858 csv_to_dynamodb-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.0/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:30:42.774973 csv_to_dynamodb-0.2.0/csv_to_dynamodb/
--rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5693 2023-05-09 23:21:31.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb/csv_to_dynamodb.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:30:42.777445 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      264 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      283 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       22 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       16 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-09 23:30:42.778566 csv_to_dynamodb-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      422 2023-05-09 23:29:59.000000 csv_to_dynamodb-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:36:09.599461 csv_to_dynamodb-0.2.1/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      389 2023-05-09 23:36:09.599225 csv_to_dynamodb-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.1/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:36:09.596625 csv_to_dynamodb-0.2.1/csv_to_dynamodb/
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5693 2023-05-09 23:21:31.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb/csv_to_dynamodb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:36:09.598834 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      389 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       22 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-09 23:36:09.599680 csv_to_dynamodb-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      570 2023-05-09 23:35:16.000000 csv_to_dynamodb-0.2.1/setup.py
```

### Comparing `csv_to_dynamodb-0.2.0/LICENSE` & `csv_to_dynamodb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.0/README.md` & `csv_to_dynamodb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.0/csv_to_dynamodb/csv_to_dynamodb.py` & `csv_to_dynamodb-0.2.1/csv_to_dynamodb/csv_to_dynamodb.py`

 * *Files identical despite different names*

