# Comparing `tmp/csv_to_dynamodb-0.2.7.tar.gz` & `tmp/csv_to_dynamodb-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_to_dynamodb-0.2.7.tar", last modified: Wed May 10 02:26:14 2023, max compression
+gzip compressed data, was "csv_to_dynamodb-0.2.8.tar", last modified: Wed May 10 02:49:39 2023, max compression
```

## Comparing `csv_to_dynamodb-0.2.7.tar` & `csv_to_dynamodb-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:26:14.401851 csv_to_dynamodb-0.2.7/
--rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.7/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 02:26:14.401253 csv_to_dynamodb-0.2.7/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.7/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:26:14.398278 csv_to_dynamodb-0.2.7/csv_to_dynamodb/
--rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6026 2023-05-10 02:26:05.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb/csv_to_dynamodb.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:26:14.400664 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       28 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 02:26:14.401975 csv_to_dynamodb-0.2.7/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      587 2023-05-10 02:25:26.000000 csv_to_dynamodb-0.2.7/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:49:39.553022 csv_to_dynamodb-0.2.8/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.8/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      516 2023-05-10 02:49:39.552523 csv_to_dynamodb-0.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.8/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:49:39.550465 csv_to_dynamodb-0.2.8/csv_to_dynamodb/
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6163 2023-05-10 02:49:16.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb/csv_to_dynamodb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:49:39.552182 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      516 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       33 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 02:49:39.000000 csv_to_dynamodb-0.2.8/csv_to_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 02:49:39.553153 csv_to_dynamodb-0.2.8/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      730 2023-05-10 02:40:21.000000 csv_to_dynamodb-0.2.8/setup.py
```

### Comparing `csv_to_dynamodb-0.2.7/LICENSE` & `csv_to_dynamodb-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.7/README.md` & `csv_to_dynamodb-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.7/csv_to_dynamodb/csv_to_dynamodb.py` & `csv_to_dynamodb-0.2.8/csv_to_dynamodb/csv_to_dynamodb.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import decimal
 import numpy as np
 import os
 import pandas as pd
 import re
 
 # Main function
-def create_table(access_key, secret_key, region, csv_path, table_name=None, hash_key=None, range_key=None):
+def create_table(access_key, secret_key, region='us-east-1', csv_path, table_name=None, hash_key=None, range_key=None):
     # Read in the CSV file and count the rows
     with open(csv_path, newline='') as csvfile:
         reader = csv.DictReader(csvfile)
         header = reader.fieldnames
         num_rows = sum(1 for row in reader)
 
     # Read in all rows if there are fewer than 100, or sample 100 rows otherwise
@@ -124,14 +124,16 @@
             print(f"The table {table.name} is not empty. Data upload stopped for this table.")
             continue
 
         chunksize = 500
         for chunk in pd.read_csv(file_path, chunksize=chunksize):
             # Replacing np.nan values with empty string
             chunk.replace(to_replace=np.nan, value="", inplace=True)
+            # Add a unique key for each record
+            chunk["UniqueID"] = [uuid.uuid4().hex for _ in range(len(chunk))]
             items = chunk.to_dict('records')
 
             # Convert data to proper format for dynamodb
             for item in items:
                 for k, v in item.items():
                     try:
                         if pd.notnull(v):
```

### Comparing `csv_to_dynamodb-0.2.7/setup.py` & `csv_to_dynamodb-0.2.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csv_to_dynamodb',
-    version='0.2.7',
+    version='0.2.8',
     author='Jason Miller',
     author_email='hackr@duck.com',
     description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
-    long_description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
+    long_description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables. The populate_table function handles floats/decimals, NaN, missing values, and create a unique Id for each row to use as a key.',
     packages=find_packages(),
     install_requires=[
         'boto3',
         'botocore',
         'numpy',
-        'pandas'
+        'pandas',
+        'uuid'
     ],
 )
```

