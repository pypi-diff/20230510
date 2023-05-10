# Comparing `tmp/tableautransformer-0.1.6.tar.gz` & `tmp/tableautransformer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableautransformer-0.1.6.tar", last modified: Fri Feb 24 16:08:27 2023, max compression
+gzip compressed data, was "tableautransformer-1.0.0.tar", last modified: Wed May 10 14:27:38 2023, max compression
```

## Comparing `tableautransformer-0.1.6.tar` & `tableautransformer-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 16:08:27.902230 tableautransformer-0.1.6/
--rw-rw-rw-   0        0        0     1091 2022-12-21 16:48:30.000000 tableautransformer-0.1.6/LICENCE
--rw-rw-rw-   0        0        0     7617 2023-02-24 16:08:27.901229 tableautransformer-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7267 2023-02-24 16:07:26.000000 tableautransformer-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-02-24 16:08:27.903229 tableautransformer-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-02-24 16:07:37.000000 tableautransformer-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-24 16:08:27.877227 tableautransformer-0.1.6/tableautransformer/
--rw-rw-rw-   0        0        0        0 2022-12-22 15:23:56.000000 tableautransformer-0.1.6/tableautransformer/__init__.py
--rw-rw-rw-   0        0        0      189 2022-12-22 15:56:40.000000 tableautransformer-0.1.6/tableautransformer/backbone.py
--rw-rw-rw-   0        0        0     4082 2023-02-24 15:59:36.000000 tableautransformer-0.1.6/tableautransformer/datawrangling.py
-drwxrwxrwx   0        0        0        0 2023-02-24 16:08:27.899229 tableautransformer-0.1.6/tableautransformer.egg-info/
--rw-rw-rw-   0        0        0     7617 2023-02-24 16:08:27.000000 tableautransformer-0.1.6/tableautransformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-02-24 16:08:27.000000 tableautransformer-0.1.6/tableautransformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 16:08:27.000000 tableautransformer-0.1.6/tableautransformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-02-24 16:08:27.000000 tableautransformer-0.1.6/tableautransformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 14:27:38.866858 tableautransformer-1.0.0/
+-rw-rw-rw-   0        0        0     1091 2022-12-21 16:48:30.000000 tableautransformer-1.0.0/LICENCE
+-rw-rw-rw-   0        0        0     8204 2023-05-10 14:27:38.866858 tableautransformer-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7854 2023-05-10 14:18:05.000000 tableautransformer-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 14:27:38.866858 tableautransformer-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-05-10 14:18:21.000000 tableautransformer-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:27:38.826856 tableautransformer-1.0.0/tableautransformer/
+-rw-rw-rw-   0        0        0        0 2022-12-22 15:23:56.000000 tableautransformer-1.0.0/tableautransformer/__init__.py
+-rw-rw-rw-   0        0        0      189 2022-12-22 15:56:40.000000 tableautransformer-1.0.0/tableautransformer/backbone.py
+-rw-rw-rw-   0        0        0     4541 2023-05-10 13:52:34.000000 tableautransformer-1.0.0/tableautransformer/datawrangling.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:27:38.866858 tableautransformer-1.0.0/tableautransformer.egg-info/
+-rw-rw-rw-   0        0        0     8204 2023-05-10 14:27:37.000000 tableautransformer-1.0.0/tableautransformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-10 14:27:38.000000 tableautransformer-1.0.0/tableautransformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:27:37.000000 tableautransformer-1.0.0/tableautransformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-10 14:27:38.000000 tableautransformer-1.0.0/tableautransformer.egg-info/top_level.txt
```

### Comparing `tableautransformer-0.1.6/LICENCE` & `tableautransformer-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `tableautransformer-0.1.6/PKG-INFO` & `tableautransformer-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableautransformer
-Version: 0.1.6
+Version: 1.0.0
 Summary: ETL tooling for tableau seed data
 Home-page: https://pypi.org/project/tableautransformer
 Author: Josh Teixeira
 Author-email: jteixeira@cppib.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -153,14 +153,51 @@
 
 ##### Inputs
 
 > **df**: *dataframe*
 >> The DataFrame you want to loop through
 
 ***
+
+### Find_Dups()
+
+```
+find_dups(df, name)
+```
+
+##### Description
+
+Find duplicate records and print them out inside a given df, duplicates must be duplicates accross all columns.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+> **name**: *string*
+>> The name that will be printed for reference in the log
+
+***
+
+### Force_String()
+
+```
+force_string(df)
+```
+
+##### Description
+
+Force all scalar data to be strings in a given dataframe.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+***
 
 ### Is_In()
 
 ```
 is_in(df, target_col, isin_list)
 ```
```

### Comparing `tableautransformer-0.1.6/README.md` & `tableautransformer-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -141,14 +141,51 @@
 ##### Inputs
 
 > **df**: *dataframe*
 >> The DataFrame you want to loop through
 
 ***
 
+### Find_Dups()
+
+```
+find_dups(df, name)
+```
+
+##### Description
+
+Find duplicate records and print them out inside a given df, duplicates must be duplicates accross all columns.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+> **name**: *string*
+>> The name that will be printed for reference in the log
+
+***
+
+### Force_String()
+
+```
+force_string(df)
+```
+
+##### Description
+
+Force all scalar data to be strings in a given dataframe.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+***
+
 ### Is_In()
 
 ```
 is_in(df, target_col, isin_list)
 ```
 
 ##### Description
```

### Comparing `tableautransformer-0.1.6/tableautransformer/datawrangling.py` & `tableautransformer-1.0.0/tableautransformer/datawrangling.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,28 @@
     return df_basic_table
 
 def find_dtypes(df):
     for col in df.columns:
         datatypes = set(df[col].dtype for i in df[col])
         print(f'{col}: {list(datatypes)}')
 
+# this is new, add md
+def find_dups(df, name):
+    duplicated = df.duplicated(subset=df.columns)
+    print('-----------------------------------------------')
+    print(f"Your duplicated inside {name} are:")
+    print(df[duplicated])
+    print('-----------------------------------------------')
+
+# this is new, add md
+def force_string(df):
+    for col in df.columns:
+        df[col] = df[col].astype(str)
+        df[col] = df[col].replace(0,'')
+
 def is_in(df, target_col, isin_list):
     df = df[df[target_col].isin(isin_list)]
     return df
 
 def cast(df, target_col, value):
     df[target_col] = value
     return df
```

### Comparing `tableautransformer-0.1.6/tableautransformer.egg-info/PKG-INFO` & `tableautransformer-1.0.0/tableautransformer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableautransformer
-Version: 0.1.6
+Version: 1.0.0
 Summary: ETL tooling for tableau seed data
 Home-page: https://pypi.org/project/tableautransformer
 Author: Josh Teixeira
 Author-email: jteixeira@cppib.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -153,14 +153,51 @@
 
 ##### Inputs
 
 > **df**: *dataframe*
 >> The DataFrame you want to loop through
 
 ***
+
+### Find_Dups()
+
+```
+find_dups(df, name)
+```
+
+##### Description
+
+Find duplicate records and print them out inside a given df, duplicates must be duplicates accross all columns.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+> **name**: *string*
+>> The name that will be printed for reference in the log
+
+***
+
+### Force_String()
+
+```
+force_string(df)
+```
+
+##### Description
+
+Force all scalar data to be strings in a given dataframe.
+
+##### Inputs
+
+> **df**: *dataframe*
+>> The DataFrame you want to loop through
+
+***
 
 ### Is_In()
 
 ```
 is_in(df, target_col, isin_list)
 ```
```

