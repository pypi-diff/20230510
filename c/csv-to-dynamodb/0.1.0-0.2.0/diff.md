# Comparing `tmp/csv_to_dynamodb-0.1.0.tar.gz` & `tmp/csv_to_dynamodb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/csv_to_dynamodb-0.1.0.tar", last modified: Mon May  8 01:57:05 2023, max compression
+gzip compressed data, was "csv_to_dynamodb-0.2.0.tar", last modified: Tue May  9 23:30:42 2023, max compression
```

## Comparing `csv_to_dynamodb-0.1.0.tar` & `csv_to_dynamodb-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-08 01:57:05.738741 csv_to_dynamodb-0.1.0/
--rw-r--r--   0 user       (501) staff       (20)      262 2023-05-08 01:57:05.738338 csv_to_dynamodb-0.1.0/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     1437 2023-05-08 01:55:57.000000 csv_to_dynamodb-0.1.0/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-08 01:57:05.734961 csv_to_dynamodb-0.1.0/csv_to_dynamodb/
--rw-r--r--   0 user       (501) staff       (20)       43 2023-05-08 01:28:47.000000 csv_to_dynamodb-0.1.0/csv_to_dynamodb/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     2741 2023-05-08 01:48:07.000000 csv_to_dynamodb-0.1.0/csv_to_dynamodb/csv_to_dynamodb.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-08 01:57:05.737893 csv_to_dynamodb-0.1.0/csv_to_dynamodb.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      262 2023-05-08 01:57:05.000000 csv_to_dynamodb-0.1.0/csv_to_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      275 2023-05-08 01:57:05.000000 csv_to_dynamodb-0.1.0/csv_to_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-08 01:57:05.000000 csv_to_dynamodb-0.1.0/csv_to_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        6 2023-05-08 01:57:05.000000 csv_to_dynamodb-0.1.0/csv_to_dynamodb.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       16 2023-05-08 01:57:05.000000 csv_to_dynamodb-0.1.0/csv_to_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-08 01:57:05.738857 csv_to_dynamodb-0.1.0/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      330 2023-05-08 00:06:44.000000 csv_to_dynamodb-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:30:42.778212 csv_to_dynamodb-0.2.0/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-05-09 23:30:42.777858 csv_to_dynamodb-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.0/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:30:42.774973 csv_to_dynamodb-0.2.0/csv_to_dynamodb/
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5693 2023-05-09 23:21:31.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb/csv_to_dynamodb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:30:42.777445 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       22 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-05-09 23:30:42.000000 csv_to_dynamodb-0.2.0/csv_to_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-09 23:30:42.778566 csv_to_dynamodb-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      422 2023-05-09 23:29:59.000000 csv_to_dynamodb-0.2.0/setup.py
```

### Comparing `csv_to_dynamodb-0.1.0/README.md` & `csv_to_dynamodb-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,67 @@
 # csv-to-dynamodb
 
-A Python library to create a DynamoDB table from a CSV file.
+A Python library to create a DynamoDB table from a CSV file. Optionally, these tables can be populated with populate_table, which also supports directories and lists of CSVs as inputs.
 
 ## Installation
 
-pip install csv-to-dynamodb
+Available on PyPI (and therefore via pip, pip3, etc). 
 
+https://pypi.org/project/csv-to-dynamodb/0.1.0/
+
+```python
+pip3 install csv-to-dynamodb
+```
+
+## Dependencies
+
+This library uses boto3, botocore, and pandas. They are included in the requirements.txt and the setup.py files.
 
 ## Usage
 
+The `create_table` method can be used to create tables as follows:
+
 ```python
 import csv_to_dynamodb
 
 # Required:
 access_key = "your_aws_access_key"
 secret_key = "your_aws_secret_key"
-region = "your_aws_region"
-csv_path = "/path/to/your/csv_file.csv"
+region     = "your_aws_region"
+csv_path   = "/path/to/your/csv_file.csv"
 
 # Optional:
 table_name = "your_table_name"
-hash_key = "your_hash_key"
-range_key = "your_range_key"
+hash_key   = "your_hash_key"
+range_key  = "your_range_key"
 
+# Invocation:
 table = csv_to_dynamodb.create_table(
-    access_key=access_key,
-    secret_key=secret_key,
-    region=region,
-    csv_path=csv_path,
-    table_name=table_name,
-    hash_key=hash_key,
-    range_key=range_key
+    access_key = access_key,
+    secret_key = secret_key,
+    region     = region,
+    csv_path   = csv_path
+)
+```
+
+`populate_table` creates the table if it's not already created and populates it. It will populate an existing but empty table of the same name if the columns and data types match.
+
+```
+populate_table(
+    access_key = access_key,
+    secret_key = secret_key,
+    region     = region,
+    csv_path   = csv_path,
+    table_name = table_name,
+    hash_key   = hash_key,
+    range_key  = range_key
 )
 ```
 
+See sample_usage.py and sample_usage2.py for more examples.
 
 ## Arguments:
 
 - access_key (required): Your AWS access key.
 - secret_key (required): Your AWS secret key.
 - region (required): The AWS region you want to create the table in.
 - csv_path (required): The path to your CSV file.
```

