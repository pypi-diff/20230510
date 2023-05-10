# Comparing `tmp/csv_to_dynamodb-0.2.6.tar.gz` & `tmp/csv_to_dynamodb-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_to_dynamodb-0.2.6.tar", last modified: Wed May 10 02:14:34 2023, max compression
+gzip compressed data, was "csv_to_dynamodb-0.2.7.tar", last modified: Wed May 10 02:26:14 2023, max compression
```

## Comparing `csv_to_dynamodb-0.2.6.tar` & `csv_to_dynamodb-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:14:34.293667 csv_to_dynamodb-0.2.6/
--rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.6/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 02:14:34.293303 csv_to_dynamodb-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.6/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:14:34.289223 csv_to_dynamodb-0.2.6/csv_to_dynamodb/
--rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.6/csv_to_dynamodb/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6208 2023-05-10 02:07:50.000000 csv_to_dynamodb-0.2.6/csv_to_dynamodb/csv_to_dynamodb.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:14:34.292682 csv_to_dynamodb-0.2.6/csv_to_dynamodb.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 02:14:34.000000 csv_to_dynamodb-0.2.6/csv_to_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 02:14:34.000000 csv_to_dynamodb-0.2.6/csv_to_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 02:14:34.000000 csv_to_dynamodb-0.2.6/csv_to_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       22 2023-05-10 02:14:34.000000 csv_to_dynamodb-0.2.6/csv_to_dynamodb.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 02:14:34.000000 csv_to_dynamodb-0.2.6/csv_to_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 02:14:34.293944 csv_to_dynamodb-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      570 2023-05-10 02:08:43.000000 csv_to_dynamodb-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:26:14.401851 csv_to_dynamodb-0.2.7/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 02:26:14.401253 csv_to_dynamodb-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.7/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:26:14.398278 csv_to_dynamodb-0.2.7/csv_to_dynamodb/
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6026 2023-05-10 02:26:05.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb/csv_to_dynamodb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 02:26:14.400664 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       28 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 02:26:14.000000 csv_to_dynamodb-0.2.7/csv_to_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 02:26:14.401975 csv_to_dynamodb-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      587 2023-05-10 02:25:26.000000 csv_to_dynamodb-0.2.7/setup.py
```

### Comparing `csv_to_dynamodb-0.2.6/LICENSE` & `csv_to_dynamodb-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.6/README.md` & `csv_to_dynamodb-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.6/csv_to_dynamodb/csv_to_dynamodb.py` & `csv_to_dynamodb-0.2.7/csv_to_dynamodb/csv_to_dynamodb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Libs
 from botocore.exceptions import ClientError
 from botocore.exceptions import NoCredentialsError
+from math import isnan, isinf
 
 import csv
 import boto3
 import decimal
+import numpy as np
 import os
 import pandas as pd
 import re
 
 # Main function
 def create_table(access_key, secret_key, region, csv_path, table_name=None, hash_key=None, range_key=None):
     # Read in the CSV file and count the rows
@@ -83,68 +85,65 @@
     # Wait for the table to become active
     table.wait_until_exists()
 
     return table
 
 # Data ingest
 def populate_table(access_key, secret_key, region, csv_path, table_name=None, hash_key=None, range_key=None):
-    # Handle both a single string and a list of strings for csv_path
     if isinstance(csv_path, str):
         csv_files = [csv_path]
     else:
         csv_files = csv_path
 
     for file_path in csv_files:
-        # Define table_name inside the loop
         if table_name is None:
             table_name = re.sub(r'\W+', '_', os.path.basename(file_path).split('.')[0])
 
         if os.path.isdir(file_path):
-            # If the path is a directory, get all CSV files in the directory
             csv_files_in_dir = [os.path.join(file_path, f) for f in os.listdir(file_path) if f.endswith('.csv')]
             csv_files.extend(csv_files_in_dir)
             continue
 
-        # Connect to the DynamoDB table
         session = boto3.Session(
             aws_access_key_id=access_key,
             aws_secret_access_key=secret_key,
             region_name=region
         )
         dynamodb = session.resource('dynamodb')
 
         try:
-            # Create the table first
             table = create_table(access_key, secret_key, region, file_path, table_name, hash_key, range_key)
-            table = dynamodb.Table(table.name)  # Get the table object
+            table = dynamodb.Table(table.name)
         except ClientError as e:
             if e.response['Error']['Code'] == "ResourceInUseException":
-                # If table already exists, just connect to it
                 table = dynamodb.Table(table_name)
             else:
                 print(f"Unexpected error: {e}")
                 continue
-
-        # Check if the table is empty
+                
         if table.item_count > 0:
             print(f"The table {table.name} is not empty. Data upload stopped for this table.")
             continue
 
-        # Now let's populate the table with data from the CSV file
-        # We use pandas to handle large files in chunks
-        chunksize = 500  # DynamoDB batch write limit
+        chunksize = 500
         for chunk in pd.read_csv(file_path, chunksize=chunksize):
+            # Replacing np.nan values with empty string
+            chunk.replace(to_replace=np.nan, value="", inplace=True)
             items = chunk.to_dict('records')
+
             # Convert data to proper format for dynamodb
             for item in items:
                 for k, v in item.items():
                     try:
                         if pd.notnull(v):
                             if isinstance(v, float):
-                                item[k] = decimal.Decimal(str(v))
+                                if isnan(v) or isinf(v):
+                                    item[k] = None  # Or replace with a value of your choice
+                                else:
+                                    item[k] = decimal.Decimal(str(v))
                             elif isinstance(v, int):
                                 item[k] = decimal.Decimal(str(v))
                             else:
                                 item[k] = str(v)
                     except Exception as e:
                         print(f"Error converting value: {v} of type {type(v)} for key: {k}")
                         print(f"Unexpected error during conversion: {e}")
@@ -155,11 +154,11 @@
                     for item in items:
                         batch.put_item(Item=item)
 
             except NoCredentialsError:
                 print("No AWS credentials found.")
                 continue
             except Exception as e:
-                print(f"Unexpected error during batch writing: {e}")
+                print(f"Unexpected error: {e}")
                 continue
 
         print(f"Data upload completed for {file_path} to table {table.name}.")
```

### Comparing `csv_to_dynamodb-0.2.6/setup.py` & `csv_to_dynamodb-0.2.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csv_to_dynamodb',
-    version='0.2.6',
+    version='0.2.7',
     author='Jason Miller',
     author_email='hackr@duck.com',
     description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     long_description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     packages=find_packages(),
     install_requires=[
         'boto3',
         'botocore',
+        'numpy',
         'pandas'
     ],
 )
```

