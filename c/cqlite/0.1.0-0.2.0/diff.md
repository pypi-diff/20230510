# Comparing `tmp/cqlite-0.1.0.tar.gz` & `tmp/cqlite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlite-0.1.0.tar", last modified: Wed May 10 05:22:23 2023, max compression
+gzip compressed data, was "cqlite-0.2.0.tar", last modified: Wed May 10 08:10:46 2023, max compression
```

## Comparing `cqlite-0.1.0.tar` & `cqlite-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 05:22:23.434189 cqlite-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-05-10 05:18:33.000000 cqlite-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      922 2023-05-10 05:22:23.432788 cqlite-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-05-10 05:20:21.000000 cqlite-0.1.0/README.md
--rw-rw-rw-   0        0        0      730 2023-05-10 05:20:31.000000 cqlite-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 05:22:23.434738 cqlite-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       92 2023-05-10 05:18:33.000000 cqlite-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:22:23.365852 cqlite-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 05:22:23.402082 cqlite-0.1.0/src/cqlite/
--rw-rw-rw-   0        0        0       21 2023-05-10 05:18:33.000000 cqlite-0.1.0/src/cqlite/__init__.py
--rw-rw-rw-   0        0        0     5221 2023-05-10 05:18:47.000000 cqlite-0.1.0/src/cqlite/cqlite.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:22:23.431786 cqlite-0.1.0/src/cqlite.egg-info/
--rw-rw-rw-   0        0        0      922 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 08:10:46.950084 cqlite-0.2.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-10 05:18:33.000000 cqlite-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      978 2023-05-10 08:10:46.947528 cqlite-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-05-10 08:08:23.000000 cqlite-0.2.0/README.md
+-rw-rw-rw-   0        0        0      730 2023-05-10 08:06:10.000000 cqlite-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:10:46.950147 cqlite-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       92 2023-05-10 05:18:33.000000 cqlite-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:10:46.881750 cqlite-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 08:10:46.897907 cqlite-0.2.0/src/cqlite/
+-rw-rw-rw-   0        0        0       21 2023-05-10 08:05:54.000000 cqlite-0.2.0/src/cqlite/__init__.py
+-rw-rw-rw-   0        0        0     5229 2023-05-10 08:05:11.000000 cqlite-0.2.0/src/cqlite/cqlite.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:10:46.942307 cqlite-0.2.0/src/cqlite.egg-info/
+-rw-rw-rw-   0        0        0      978 2023-05-10 08:10:46.000000 cqlite-0.2.0/src/cqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-10 08:10:46.000000 cqlite-0.2.0/src/cqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:10:46.000000 cqlite-0.2.0/src/cqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-10 08:10:46.000000 cqlite-0.2.0/src/cqlite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 08:10:46.000000 cqlite-0.2.0/src/cqlite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 08:10:46.000000 cqlite-0.2.0/src/cqlite.egg-info/top_level.txt
```

### Comparing `cqlite-0.1.0/LICENSE` & `cqlite-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cqlite-0.1.0/PKG-INFO` & `cqlite-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlite
-Version: 0.1.0
+Version: 0.2.0
 Summary: Query a CSV file from the commandline
 Author-email: Emil Kloeden <emilkloeden@gmail.com>
 Project-URL: Homepage, https://github.com/emilkloeden/cqlite
 Project-URL: Bug Tracker, https://github.com/emilkloeden/cqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,12 +30,14 @@
 
 e.g.
 
 ```sh
 cqlite fakedata.csv "SELECT * FROM csv WHERE name LIKE '%Tommy% AND date_of_birth < '1980-01-01';"
 ```
 
+(note filedata is loaded into a table called "csv").
+
 Save `<csv_file>.csv as a SQLite database (<csv_file>.db):
 
 ```sh
 cqlite <csv_file> --persist
 ```
```

### Comparing `cqlite-0.1.0/pyproject.toml` & `cqlite-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cqlite"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Emil Kloeden", email="emilkloeden@gmail.com" },
 ]
 description = "Query a CSV file from the commandline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cqlite-0.1.0/src/cqlite/cqlite.py` & `cqlite-0.2.0/src/cqlite/cqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,31 +163,32 @@
         exit(1)
     name = file_path.stem
     try:
         headers, rows = load_csv_file(file_path)
     except Exception as e:
         print(f"Unable to load {file_path}. Perhaps it is not a CSV file?")
         exit(1)
+    
     if not query and not persist:
         print("Must supply a query or specify that you want the file contents saved to a sqlite file.")
 
     if persist:
         db_path = file_path.parent / f"{name}.db"
         conn = sqlite3.connect(db_path)
     else:
         conn = sqlite3.connect(":memory:")
     # conn = sqlite3.connect("test.db")
     cur = conn.cursor()
 
-    conn, cur = populate_database(conn, cur, name, headers, rows)
+    conn, cur = populate_database(conn, cur, "csv", headers, rows)
 
     if query:
         try:
             results, result_headers = execute_query(cur, query)
-            print_results(results, result_headers, name)
+            print_results(results, result_headers, "csv")
         except sqlite3.OperationalError as e:
             print(e)
 
 def run_with_typer():
     typer.run(main)
 
 if __name__ == "__main__":
```

### Comparing `cqlite-0.1.0/src/cqlite.egg-info/PKG-INFO` & `cqlite-0.2.0/src/cqlite.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqlite
-Version: 0.1.0
+Version: 0.2.0
 Summary: Query a CSV file from the commandline
 Author-email: Emil Kloeden <emilkloeden@gmail.com>
 Project-URL: Homepage, https://github.com/emilkloeden/cqlite
 Project-URL: Bug Tracker, https://github.com/emilkloeden/cqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,12 +30,14 @@
 
 e.g.
 
 ```sh
 cqlite fakedata.csv "SELECT * FROM csv WHERE name LIKE '%Tommy% AND date_of_birth < '1980-01-01';"
 ```
 
+(note filedata is loaded into a table called "csv").
+
 Save `<csv_file>.csv as a SQLite database (<csv_file>.db):
 
 ```sh
 cqlite <csv_file> --persist
 ```
```

