# Comparing `tmp/csv_to_dynamodb-0.2.4.tar.gz` & `tmp/csv_to_dynamodb-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/csv_to_dynamodb-0.2.4.tar", last modified: Wed May 10 01:06:19 2023, max compression
+gzip compressed data, was "csv_to_dynamodb-0.2.5.tar", last modified: Wed May 10 01:54:23 2023, max compression
```

## Comparing `csv_to_dynamodb-0.2.4.tar` & `csv_to_dynamodb-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:06:19.887728 csv_to_dynamodb-0.2.4/
--rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.4/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      433 2023-05-10 01:06:19.887400 csv_to_dynamodb-0.2.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.4/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:06:19.883931 csv_to_dynamodb-0.2.4/csv_to_dynamodb/
--rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6121 2023-05-10 01:03:16.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb/csv_to_dynamodb.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:06:19.886764 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      433 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       22 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 01:06:19.000000 csv_to_dynamodb-0.2.4/csv_to_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 01:06:19.887968 csv_to_dynamodb-0.2.4/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      570 2023-05-10 01:05:45.000000 csv_to_dynamodb-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:54:23.427577 csv_to_dynamodb-0.2.5/
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-05-09 22:19:33.000000 csv_to_dynamodb-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 01:54:23.427197 csv_to_dynamodb-0.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2302 2023-05-09 23:27:55.000000 csv_to_dynamodb-0.2.5/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:54:23.423811 csv_to_dynamodb-0.2.5/csv_to_dynamodb/
+-rw-r--r--   0 root         (0) staff       (20)       87 2023-05-09 23:00:43.000000 csv_to_dynamodb-0.2.5/csv_to_dynamodb/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6223 2023-05-10 01:52:56.000000 csv_to_dynamodb-0.2.5/csv_to_dynamodb/csv_to_dynamodb.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-10 01:54:23.426536 csv_to_dynamodb-0.2.5/csv_to_dynamodb.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      389 2023-05-10 01:54:23.000000 csv_to_dynamodb-0.2.5/csv_to_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      283 2023-05-10 01:54:23.000000 csv_to_dynamodb-0.2.5/csv_to_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-10 01:54:23.000000 csv_to_dynamodb-0.2.5/csv_to_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       22 2023-05-10 01:54:23.000000 csv_to_dynamodb-0.2.5/csv_to_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2023-05-10 01:54:23.000000 csv_to_dynamodb-0.2.5/csv_to_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-10 01:54:23.427915 csv_to_dynamodb-0.2.5/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      570 2023-05-10 01:54:20.000000 csv_to_dynamodb-0.2.5/setup.py
```

### Comparing `csv_to_dynamodb-0.2.4/LICENSE` & `csv_to_dynamodb-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.4/README.md` & `csv_to_dynamodb-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `csv_to_dynamodb-0.2.4/csv_to_dynamodb/csv_to_dynamodb.py` & `csv_to_dynamodb-0.2.5/csv_to_dynamodb/csv_to_dynamodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 
     # Wait for the table to become active
     table.wait_until_exists()
 
     return table
 
 # Data ingest
+d# Data ingest
 def populate_table(access_key, secret_key, region, csv_path, table_name=None, hash_key=None, range_key=None):
     # Handle both a single string and a list of strings for csv_path
     if isinstance(csv_path, str):
         csv_files = [csv_path]
     else:
         csv_files = csv_path
 
@@ -119,45 +120,47 @@
         except ClientError as e:
             if e.response['Error']['Code'] == "ResourceInUseException":
                 # If table already exists, just connect to it
                 table = dynamodb.Table(table_name)
             else:
                 print(f"Unexpected error: {e}")
                 continue
-                
+
         # Check if the table is empty
         if table.item_count > 0:
             print(f"The table {table.name} is not empty. Data upload stopped for this table.")
             continue
 
         # Now let's populate the table with data from the CSV file
         # We use pandas to handle large files in chunks
         chunksize = 500  # DynamoDB batch write limit
         for chunk in pd.read_csv(file_path, chunksize=chunksize):
             items = chunk.to_dict('records')
             # Convert data to proper format for dynamodb
             for item in items:
-                item = {k: decimal.Decimal(str(v)) if pd.notnull(v) and isinstance(v, (int, float)) and not pd.isna(v) else str(v) for k, v in item.items()}
-            for i in range(len(items)):
-                for k, v in items[i].items():
-                    if pd.notnull(v):
-                        if isinstance(v, float):
-                            items[i][k] = decimal.Decimal(str(v))
-                        elif isinstance(v, int):
-                            items[i][k] = decimal.Decimal(str(v))
-                        else:
-                            items[i][k] = str(v)
+                for k, v in item.items():
+                    try:
+                        if pd.notnull(v):
+                            if isinstance(v, float):
+                                item[k] = decimal.Decimal(str(v))
+                            elif isinstance(v, int):
+                                item[k] = decimal.Decimal(str(v))
+                            else:
+                                item[k] = str(v)
+                    except Exception as e:
+                        print(f"Error converting value: {v} of type {type(v)} for key: {k}")
+                        print(f"Unexpected error during conversion: {e}")
+                        continue
 
             try:
                 with table.batch_writer() as batch:
                     for item in items:
                         batch.put_item(Item=item)
 
             except NoCredentialsError:
                 print("No AWS credentials found.")
                 continue
             except Exception as e:
-                print(f"Unexpected error: {e}")
+                print(f"Unexpected error during batch writing: {e}")
                 continue
 
         print(f"Data upload completed for {file_path} to table {table.name}.")
-
```

### Comparing `csv_to_dynamodb-0.2.4/setup.py` & `csv_to_dynamodb-0.2.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='csv_to_dynamodb',
-    version='0.2.4',
+    version='0.2.5',
     author='Jason Miller',
     author_email='hackr@duck.com',
     description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     long_description='A library for automatically creating DynamoDB tables from CSV files and, optionally, automatically populating those tables.',
     packages=find_packages(),
     install_requires=[
         'boto3',
```

