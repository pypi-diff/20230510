# Comparing `tmp/csv_to_dynamodb-0.2.3.tar.gz` & `tmp/csv_to_dynamodb-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/csv_to_dynamodb-0.2.3.tar", last modified: Wed May 10 01:04:44 2023, max compression
+gzip compressed data, was "dist/csv_to_dynamodb-0.2.4.tar", last modified: Wed May 10 01:06:19 2023, max compression
```

## Comparing `csv_to_dynamodb-0.2.3.tar` & `csv_to_dynamodb-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:04:44.427539 csv_to_dynamodb-0.2.3/
--rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.3/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      433 2023-05-10 01:04:44.427282 csv_to_dynamodb-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.3/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:04:44.424798 csv_to_dynamodb-0.2.3/csv_to_dynamodb/
--rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.3/csv_to_dynamodb/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6121 2023-05-10 01:03:16.000000 csv_to_dynamodb-0.2.3/csv_to_dynamodb/csv_to_dynamodb.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:04:44.426921 csv_to_dynamodb-0.2.3/csv_to_dynamodb.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      433 2023-05-10 01:04:44.000000 csv_to_dynamodb-0.2.3/csv_to_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 01:04:44.000000 csv_to_dynamodb-0.2.3/csv_to_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 01:04:44.000000 csv_to_dynamodb-0.2.3/csv_to_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       22 2023-05-10 01:04:44.000000 csv_to_dynamodb-0.2.3/csv_to_dynamodb.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 01:04:44.000000 csv_to_dynamodb-0.2.3/csv_to_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 01:04:44.427735 csv_to_dynamodb-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      570 2023-05-10 01:04:04.000000 csv_to_dynamodb-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:06:19.887728 csv_to_dynamodb-0.2.4/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.4/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      433 2023-05-10 01:06:19.887400 csv_to_dynamodb-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.4/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:06:19.883931 csv_to_dynamodb-0.2.4/csv_to_dynamodb/
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6121 2023-05-10 01:03:16.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb/csv_to_dynamodb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:06:19.886764 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      433 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       22 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 01:06:19.887968 csv_to_dynamodb-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      570 2023-05-10 01:05:45.000000 csv_to_dynamodb-0.2.4/setup.py
```

### Comparing `csv_to_dynamodb-0.2.3/LICENSE` & `csv_to_dynamodb-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.3/README.md` & `csv_to_dynamodb-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.3/csv_to_dynamodb/csv_to_dynamodb.py` & `csv_to_dynamodb-0.2.4/csv_to_dynamodb/csv_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.3/setup.py` & `csv_to_dynamodb-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csv_to_dynamodb',
-    version='0.2.3',
+    version='0.2.4',
     author='Jason Miller',
     author_email='hackr@duck.com',
     description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     long_description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     packages=find_packages(),
     install_requires=[
         'boto3',
```

