# Comparing `tmp/csv_to_dynamodb-0.2.1.tar.gz` & `tmp/csv_to_dynamodb-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_to_dynamodb-0.2.1.tar", last modified: Tue May  9 23:36:09 2023, max compression
+gzip compressed data, was "csv_to_dynamodb-0.2.2.tar", last modified: Wed May 10 00:41:35 2023, max compression
```

## Comparing `csv_to_dynamodb-0.2.1.tar` & `csv_to_dynamodb-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:36:09.599461 csv_to_dynamodb-0.2.1/
--rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      389 2023-05-09 23:36:09.599225 csv_to_dynamodb-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.1/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:36:09.596625 csv_to_dynamodb-0.2.1/csv_to_dynamodb/
--rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5693 2023-05-09 23:21:31.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb/csv_to_dynamodb.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-09 23:36:09.598834 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      389 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      283 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       22 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       16 2023-05-09 23:36:09.000000 csv_to_dynamodb-0.2.1/csv_to_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-09 23:36:09.599680 csv_to_dynamodb-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      570 2023-05-09 23:35:16.000000 csv_to_dynamodb-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 00:41:35.197160 csv_to_dynamodb-0.2.2/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 00:41:35.196907 csv_to_dynamodb-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.2/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 00:41:35.194622 csv_to_dynamodb-0.2.2/csv_to_dynamodb/
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.2/csv_to_dynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5947 2023-05-10 00:40:04.000000 csv_to_dynamodb-0.2.2/csv_to_dynamodb/csv_to_dynamodb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 00:41:35.196519 csv_to_dynamodb-0.2.2/csv_to_dynamodb.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 00:41:35.000000 csv_to_dynamodb-0.2.2/csv_to_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 00:41:35.000000 csv_to_dynamodb-0.2.2/csv_to_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 00:41:35.000000 csv_to_dynamodb-0.2.2/csv_to_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       22 2023-05-10 00:41:35.000000 csv_to_dynamodb-0.2.2/csv_to_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 00:41:35.000000 csv_to_dynamodb-0.2.2/csv_to_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 00:41:35.197378 csv_to_dynamodb-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      570 2023-05-10 00:40:32.000000 csv_to_dynamodb-0.2.2/setup.py
```

### Comparing `csv_to_dynamodb-0.2.1/LICENSE` & `csv_to_dynamodb-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.1/README.md` & `csv_to_dynamodb-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.1/csv_to_dynamodb/csv_to_dynamodb.py` & `csv_to_dynamodb-0.2.2/csv_to_dynamodb/csv_to_dynamodb.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 
     # Wait for the table to become active
     table.wait_until_exists()
 
     return table
 
 # Data ingest
+# Data ingest
 def populate_table(access_key, secret_key, region, csv_path, table_name=None, hash_key=None, range_key=None):
     # Handle both a single string and a list of strings for csv_path
     if isinstance(csv_path, str):
         csv_files = [csv_path]
     else:
         csv_files = csv_path
 
@@ -131,24 +132,31 @@
 
         # Now let's populate the table with data from the CSV file
         # We use pandas to handle large files in chunks
         chunksize = 500  # DynamoDB batch write limit
         for chunk in pd.read_csv(file_path, chunksize=chunksize):
             items = chunk.to_dict('records')
             # Convert data to proper format for dynamodb
-            for item in items:
-                item = {k: decimal.Decimal(str(v)) if pd.notnull(v) and isinstance(v, (int, float)) else str(v) 
-                        for k, v in item.items()}
+            for i in range(len(items)):
+                for k, v in items[i].items():
+                    if pd.notnull(v):
+                        if isinstance(v, float):
+                            items[i][k] = decimal.Decimal(str(v))
+                        elif isinstance(v, int):
+                            items[i][k] = decimal.Decimal(str(v))
+                        else:
+                            items[i][k] = str(v)
 
             try:
                 with table.batch_writer() as batch:
                     for item in items:
                         batch.put_item(Item=item)
 
             except NoCredentialsError:
                 print("No AWS credentials found.")
                 continue
             except Exception as e:
                 print(f"Unexpected error: {e}")
                 continue
 
         print(f"Data upload completed for {file_path} to table {table.name}.")
+
```

### Comparing `csv_to_dynamodb-0.2.1/setup.py` & `csv_to_dynamodb-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csv_to_dynamodb',
-    version='0.2.1',
+    version='0.2.2',
     author='Jason Miller',
     author_email='hackr@duck.com',
     description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     long_description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     packages=find_packages(),
     install_requires=[
         'boto3',
```

