# Comparing `tmp/csv_to_dynamodb-0.2.8.tar.gz` & `tmp/csv_to_dynamodb-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_to_dynamodb-0.2.8.tar", last modified: Wed May 10 02:49:39 2023, max compression
+gzip compressed data, was "csv_to_dynamodb-0.2.9.tar", last modified: Wed May 10 02:52:21 2023, max compression
```

## Comparing `csv_to_dynamodb-0.2.8.tar` & `csv_to_dynamodb-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:49:39.553022 csv_to_dynamodb-0.2.8/
--rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.8/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      516 2023-05-10 02:49:39.552523 csv_to_dynamodb-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.8/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:49:39.550465 csv_to_dynamodb-0.2.8/csv_to_dynamodb/
--rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6163 2023-05-10 02:49:16.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb/csv_to_dynamodb.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:49:39.552182 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      516 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       33 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 02:49:39.553153 csv_to_dynamodb-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      730 2023-05-10 02:40:21.000000 csv_to_dynamodb-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:52:21.826346 csv_to_dynamodb-0.2.9/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.9/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      516 2023-05-10 02:52:21.825959 csv_to_dynamodb-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.9/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:52:21.823407 csv_to_dynamodb-0.2.9/csv_to_dynamodb/
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.9/csv_to_dynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6151 2023-05-10 02:51:51.000000 csv_to_dynamodb-0.2.9/csv_to_dynamodb/csv_to_dynamodb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:52:21.825632 csv_to_dynamodb-0.2.9/csv_to_dynamodb.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      516 2023-05-10 02:52:21.000000 csv_to_dynamodb-0.2.9/csv_to_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 02:52:21.000000 csv_to_dynamodb-0.2.9/csv_to_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 02:52:21.000000 csv_to_dynamodb-0.2.9/csv_to_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       33 2023-05-10 02:52:21.000000 csv_to_dynamodb-0.2.9/csv_to_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 02:52:21.000000 csv_to_dynamodb-0.2.9/csv_to_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 02:52:21.826428 csv_to_dynamodb-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      730 2023-05-10 02:52:15.000000 csv_to_dynamodb-0.2.9/setup.py
```

### Comparing `csv_to_dynamodb-0.2.8/LICENSE` & `csv_to_dynamodb-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.8/PKG-INFO` & `csv_to_dynamodb-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1
 Name: csv_to_dynamodb
-Version: 0.2.8
+Version: 0.2.9
 Summary: A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.
 Author: Jason Miller
 Author-email: hackr@duck.com
 License-File: LICENSE
 
 A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables. The populate_table function handles floats/decimals, NaN, missing values, and create a unique Id for each row to use as a key.
```

### Comparing `csv_to_dynamodb-0.2.8/README.md` & `csv_to_dynamodb-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.8/csv_to_dynamodb/csv_to_dynamodb.py` & `csv_to_dynamodb-0.2.9/csv_to_dynamodb/csv_to_dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import decimal
 import numpy as np
 import os
 import pandas as pd
 import re
 
 # Main function
-def create_table(access_key, secret_key, region='us-east-1', csv_path, table_name=None, hash_key=None, range_key=None):
+def create_table(access_key, secret_key, region, csv_path, table_name=None, hash_key=None, range_key=None):
     # Read in the CSV file and count the rows
     with open(csv_path, newline='') as csvfile:
         reader = csv.DictReader(csvfile)
         header = reader.fieldnames
         num_rows = sum(1 for row in reader)
 
     # Read in all rows if there are fewer than 100, or sample 100 rows otherwise
```

### Comparing `csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/PKG-INFO` & `csv_to_dynamodb-0.2.9/csv_to_dynamodb.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1
 Name: csv-to-dynamodb
-Version: 0.2.8
+Version: 0.2.9
 Summary: A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.
 Author: Jason Miller
 Author-email: hackr@duck.com
 License-File: LICENSE
 
 A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables. The populate_table function handles floats/decimals, NaN, missing values, and create a unique Id for each row to use as a key.
```

### Comparing `csv_to_dynamodb-0.2.8/setup.py` & `csv_to_dynamodb-0.2.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csv_to_dynamodb',
-    version='0.2.8',
+    version='0.2.9',
     author='Jason Miller',
     author_email='hackr@duck.com',
     description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     long_description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables. The populate_table function handles floats/decimals, NaN, missing values, and create a unique Id for each row to use as a key.',
     packages=find_packages(),
     install_requires=[
         'boto3',
```

