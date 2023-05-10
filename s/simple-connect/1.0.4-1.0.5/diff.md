# Comparing `tmp/simple_connect-1.0.4.tar.gz` & `tmp/simple_connect-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_connect-1.0.4.tar", last modified: Mon Mar 14 16:42:26 2022, max compression
+gzip compressed data, was "simple_connect-1.0.5.tar", last modified: Wed May 10 18:38:25 2023, max compression
```

## Comparing `simple_connect-1.0.4.tar` & `simple_connect-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 saeedabdulrahim   (501) staff       (20)        0 2022-03-14 16:42:26.127478 simple_connect-1.0.4/
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)     1073 2022-01-29 11:56:08.000000 simple_connect-1.0.4/LICENSE
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)     2752 2022-03-14 16:42:26.126962 simple_connect-1.0.4/PKG-INFO
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)     2455 2022-01-30 08:00:33.000000 simple_connect-1.0.4/README.md
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)       38 2022-03-14 16:42:26.127736 simple_connect-1.0.4/setup.cfg
--rw-rw-r--   0 saeedabdulrahim   (501) staff       (20)      746 2022-03-14 16:37:28.000000 simple_connect-1.0.4/setup.py
-drwxr-xr-x   0 saeedabdulrahim   (501) staff       (20)        0 2022-03-14 16:42:26.123762 simple_connect-1.0.4/simple_connect/
--rw-rw-r--   0 saeedabdulrahim   (501) staff       (20)       21 2022-03-09 12:02:38.000000 simple_connect-1.0.4/simple_connect/__init__.py
--rw-rw-r--   0 saeedabdulrahim   (501) staff       (20)    13967 2022-03-09 12:04:04.000000 simple_connect-1.0.4/simple_connect/connect.py
-drwxr-xr-x   0 saeedabdulrahim   (501) staff       (20)        0 2022-03-14 16:42:26.126376 simple_connect-1.0.4/simple_connect.egg-info/
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)     2752 2022-03-14 16:42:25.000000 simple_connect-1.0.4/simple_connect.egg-info/PKG-INFO
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)      268 2022-03-14 16:42:25.000000 simple_connect-1.0.4/simple_connect.egg-info/SOURCES.txt
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)        1 2022-03-14 16:42:25.000000 simple_connect-1.0.4/simple_connect.egg-info/dependency_links.txt
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)      103 2022-03-14 16:42:25.000000 simple_connect-1.0.4/simple_connect.egg-info/requires.txt
--rw-r--r--   0 saeedabdulrahim   (501) staff       (20)       15 2022-03-14 16:42:25.000000 simple_connect-1.0.4/simple_connect.egg-info/top_level.txt
+drwxr-xr-x   0 saeedabdulrahim   (501) staff       (20)        0 2023-05-10 18:38:25.916870 simple_connect-1.0.5/
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)     1073 2023-05-10 18:26:35.000000 simple_connect-1.0.5/LICENSE
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)     3085 2023-05-10 18:38:25.916307 simple_connect-1.0.5/PKG-INFO
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)     2455 2023-05-10 18:26:35.000000 simple_connect-1.0.5/README.md
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)      626 2023-05-10 18:37:23.000000 simple_connect-1.0.5/pyproject.toml
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)       38 2023-05-10 18:38:25.917010 simple_connect-1.0.5/setup.cfg
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)      745 2023-05-10 18:29:50.000000 simple_connect-1.0.5/setup.py
+drwxr-xr-x   0 saeedabdulrahim   (501) staff       (20)        0 2023-05-10 18:38:25.913264 simple_connect-1.0.5/simple_connect/
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)       21 2023-05-10 18:26:35.000000 simple_connect-1.0.5/simple_connect/__init__.py
+-rw-rw-r--   0 saeedabdulrahim   (501) staff       (20)    14358 2023-05-04 09:22:57.000000 simple_connect-1.0.5/simple_connect/connect.py
+drwxr-xr-x   0 saeedabdulrahim   (501) staff       (20)        0 2023-05-10 18:38:25.915744 simple_connect-1.0.5/simple_connect.egg-info/
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)     3085 2023-05-10 18:38:25.000000 simple_connect-1.0.5/simple_connect.egg-info/PKG-INFO
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)      283 2023-05-10 18:38:25.000000 simple_connect-1.0.5/simple_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)        1 2023-05-10 18:38:25.000000 simple_connect-1.0.5/simple_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)      103 2023-05-10 18:38:25.000000 simple_connect-1.0.5/simple_connect.egg-info/requires.txt
+-rw-r--r--   0 saeedabdulrahim   (501) staff       (20)       15 2023-05-10 18:38:25.000000 simple_connect-1.0.5/simple_connect.egg-info/top_level.txt
```

### Comparing `simple_connect-1.0.4/LICENSE` & `simple_connect-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_connect-1.0.4/PKG-INFO` & `simple_connect-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: simple_connect
-Version: 1.0.4
-Summary: Simplify Connection
-Home-page: https://github.com/saeed-abdul-rahim/simple_connesct
+Version: 1.0.5
+Summary: Simplify SQL Connection for data analysis
+Home-page: https://github.com/saeed-abdul-rahim/simple_connect
 Author: Saeed
-Author-email: sae.ar2@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Saeed Abdul Rahim <sae.ar2@gmail.com>
+Project-URL: Homepage, https://github.com/saeed-abdul-rahim/simple_connect
+Project-URL: Bug Tracker, https://github.com/saeed-abdul-rahim/simple_connect/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simplify Connection to your Database
 
 Simple Connect allows you to securely access your database and it supports SSH Connection
 Currently it only supports SQL Databses.
@@ -114,9 +118,7 @@
 ```
 conn.delete_row(dataframe, 'table_name', ['columns_where_contition_applies', ...])
 ```
 Example:
 ```
 conn.delete_row(dataframe, 'sample_table', ['id', 'id_2'])
 ```
-
-
```

### Comparing `simple_connect-1.0.4/README.md` & `simple_connect-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `simple_connect-1.0.4/setup.py` & `simple_connect-1.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_connect",
-    version="1.0.4",
+    version="1.0.5",
     author="Saeed",
     author_email="sae.ar2@gmail.com",
     description="Simplify Connection",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/saeed-abdul-rahim/simple_connesct',
+    url='https://github.com/saeed-abdul-rahim/simple_connect',
     packages=setuptools.find_packages(),
     install_requires=[
         'httplib2', 'oauth2client',
         'pandas', 'pymysql', 'sqlalchemy', 'sshtunnel',
         'google-api-python-client', 'boto3', 'tqdm', 'paramiko'
     ]
 )
```

### Comparing `simple_connect-1.0.4/simple_connect/connect.py` & `simple_connect-1.0.5/simple_connect/connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,24 +52,30 @@
         dict_data = df.to_dict('records')
         dict_data=tuple(dict_data)
         set_columns=Common.create_sq_string(set_cols, ",")
         where_columns=Common.create_sq_string(where_cols, "AND")
         stmt="UPDATE "+table_name+" SET "+set_columns+" WHERE "+where_columns
         stmt=text(stmt)
         for line in tqdm(dict_data):
-              conn.execute(stmt, **line)   
+              conn.execute(stmt, **line)  
+        return self 
     
     def delete_main(self,df,conn,table_name,where_cols):
         dict_data = df.to_dict('records')
         dict_data=tuple(dict_data)
         where_columns=Common.create_sq_string(where_cols, "AND")
         stmt="DELETE FROM "+table_name+" WHERE "+where_columns
         stmt=text(stmt)
         for line in tqdm(dict_data):
-              conn.execute(stmt, **line)   
+              conn.execute(stmt, **line)
+        return self
+    
+    def _execute(self, conn, stmt):
+        conn.execute(text(stmt))
+        return self
 
 class Connect(Common):
     
     def __init__(self,credentials,database):
         cred_dir=os.path.join(os.path.expanduser('~'),'.credentials')
         cred_file=os.path.join(cred_dir,credentials)
         with open(cred_file) as f:
@@ -87,14 +93,17 @@
         return pd.read_sql_query(q, self.mydb)
     
     def update_table(self,df,table_name,set_cols,where_cols):
         self.common.update_main(df,self.mydb,table_name,set_cols,where_cols)
         
     def delete_row(self,df,table_name,where_cols):
         self.common.delete_main(df,self.mydb,table_name,where_cols)
+        
+    def execute(self, stmt):
+        self.common._execute(self.mydb, stmt)
     
 class BastionConnect(Common):
         
     def __init__(self, credentials, database, pem_path=None):
         cred_dir=os.path.join(os.path.expanduser('~'),'.credentials')
         cred_file=os.path.join(cred_dir,credentials)
         with open(cred_file) as f:
@@ -152,14 +161,20 @@
         self.server.stop()
         
     def delete_row(self,df,table_name,where_cols):
         self.server.start()
         self.start_conn()
         self.common.delete_main(df,self.mydb,table_name,where_cols)  
         self.server.stop()
+    
+    def execute(self, stmt):
+        self.server.start()
+        self.start_conn()
+        self.common._execute(self.mydb, stmt)
+        self.server.stop()
 
 
 class Gdrive:
     
     SCOPES = 'https://www.googleapis.com/auth/drive'
     
     def __init__(self, credential_file_json, SCOPES=SCOPES):
```

### Comparing `simple_connect-1.0.4/simple_connect.egg-info/PKG-INFO` & `simple_connect-1.0.5/simple_connect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: simple-connect
-Version: 1.0.4
-Summary: Simplify Connection
-Home-page: https://github.com/saeed-abdul-rahim/simple_connesct
+Version: 1.0.5
+Summary: Simplify SQL Connection for data analysis
+Home-page: https://github.com/saeed-abdul-rahim/simple_connect
 Author: Saeed
-Author-email: sae.ar2@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+Author-email: Saeed Abdul Rahim <sae.ar2@gmail.com>
+Project-URL: Homepage, https://github.com/saeed-abdul-rahim/simple_connect
+Project-URL: Bug Tracker, https://github.com/saeed-abdul-rahim/simple_connect/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simplify Connection to your Database
 
 Simple Connect allows you to securely access your database and it supports SSH Connection
 Currently it only supports SQL Databses.
@@ -114,9 +118,7 @@
 ```
 conn.delete_row(dataframe, 'table_name', ['columns_where_contition_applies', ...])
 ```
 Example:
 ```
 conn.delete_row(dataframe, 'sample_table', ['id', 'id_2'])
 ```
-
-
```

