# Comparing `tmp/Lab93DatabaseSystem-0.0.2.tar.gz` & `tmp/Lab93DatabaseSystem-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lab93DatabaseSystem-0.0.2.tar", last modified: Mon May  8 13:06:35 2023, max compression
+gzip compressed data, was "Lab93DatabaseSystem-0.0.3.tar", last modified: Wed May 10 00:38:37 2023, max compression
```

## Comparing `Lab93DatabaseSystem-0.0.2.tar` & `Lab93DatabaseSystem-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.596242 Lab93DatabaseSystem-0.0.2/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2505 2023-05-08 13:06:35.596242 Lab93DatabaseSystem-0.0.2/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      652 2023-05-08 13:03:57.000000 Lab93DatabaseSystem-0.0.2/pyproject.toml
--rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)     1950 2023-04-19 18:29:25.000000 Lab93DatabaseSystem-0.0.2/readme.md
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-05-08 13:06:35.596242 Lab93DatabaseSystem-0.0.2/setup.cfg
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.582907 Lab93DatabaseSystem-0.0.2/src/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.586241 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     5722 2023-05-08 12:36:38.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.592908 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.596242 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     7444 2023-05-08 12:55:53.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-08 12:54:50.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-04-21 17:54:30.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 12:40:34.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-08 13:06:35.589574 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/
--rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)     2505 2023-05-08 13:06:35.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/PKG-INFO
--rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-05-08 13:06:35.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
--rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-05-08 13:06:35.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
--rw-rw-r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-05-08 13:06:35.000000 Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.738439 Lab93DatabaseSystem-0.0.3/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      941 2023-05-10 00:38:37.738439 Lab93DatabaseSystem-0.0.3/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      652 2023-05-10 00:38:00.000000 Lab93DatabaseSystem-0.0.3/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      386 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.3/readme.md
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-05-10 00:38:37.738439 Lab93DatabaseSystem-0.0.3/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.718437 Lab93DatabaseSystem-0.0.3/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.725104 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     5661 2023-05-10 00:02:51.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.735105 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.738439 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     8087 2023-05-10 00:37:15.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      928 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-09 21:37:42.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-05-10 00:38:37.731772 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      941 2023-05-10 00:38:37.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      469 2023-05-10 00:38:37.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-05-10 00:38:37.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       20 2023-05-10 00:38:37.000000 Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem.egg-info/top_level.txt
```

### Comparing `Lab93DatabaseSystem-0.0.2/pyproject.toml` & `Lab93DatabaseSystem-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Lab93DatabaseSystem"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 
 description = "An API for interfacing with SQLite3 databases from the command line."
 readme = "readme.md"
 requires-python = ">=3.10"
```

### Comparing `Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/__init__.py` & `Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,10 +121,7 @@
                 column_type = config[table]["columns"][column]
                 SQLite3.newColumn( database,
                                    table=str(table),
                                    column=str(column),
                                    column_type=column_type, ); print(
                     f"    --{str(column).title()} column created."
                 )
-
-if __name__ == "__main__":
-    buildAdministratorDatabase()
```

### Comparing `Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py` & `Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/SQLite3.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,17 @@
     'queryColumnExistence': "SELECT COUNT(*) FROM pragma_table_info('{}') WHERE name='{}';",
 
     # Enumerate a list of tables within the master record.
     'queryTableList': "SELECT name FROM sqlite_schema WHERE type='table' ORDER BY name;",
 
     # Curate a list of headers for a given table.
     'queryHeaderList': "SELECT name FROM sqlite_master WHERE type='table'",
+
+    # Add a new row to a specific table.
+    'createNewRow': "INSERT OR IGNORE INTO {}({}) VALUES({});",
 }
 
 
 def newColumn( database,
                table: str="test_table_one",
                column: str="test_column_one",
                column_type: str="UNIQUE PRIMARY TEXT" ) -> None:
@@ -198,7 +201,25 @@
     """
     database = databaseConnection(database)
     return database.cursor\
                    .execute( statements['queryColumnExistence']\
                                  .format( table.lower(),
                                           column.lower() )            )\
                    .fetchall()[0][0]
+
+
+def newRow( database,
+            table: str="test_table_one",
+            columns: str="test_column_one, test_column_two",
+            values: str="test_value_one, test_value_two" ):
+    """
+    """
+
+    database = databaseConnection(database)
+    database.cursor\
+            .execute( statements['createNewRow']\
+                          .format( table.lower(),
+                                   columns.lower(),
+                                   values.lower() )  )
+
+    return database.connection\
+                   .commit()
```

### Comparing `Lab93DatabaseSystem-0.0.2/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py` & `Lab93DatabaseSystem-0.0.3/src/Lab93DatabaseSystem/submodules/DatabaseAPI/Shelve.py`

 * *Files identical despite different names*

