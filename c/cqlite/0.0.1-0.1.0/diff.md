# Comparing `tmp/cqlite-0.0.1.tar.gz` & `tmp/cqlite-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlite-0.0.1.tar", last modified: Wed May 10 04:49:03 2023, max compression
+gzip compressed data, was "cqlite-0.1.0.tar", last modified: Wed May 10 05:22:23 2023, max compression
```

## Comparing `cqlite-0.0.1.tar` & `cqlite-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 04:49:03.000628 cqlite-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-05-10 02:37:30.000000 cqlite-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      637 2023-05-10 04:49:02.999121 cqlite-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      110 2023-05-10 02:37:30.000000 cqlite-0.0.1/README.md
--rw-rw-rw-   0        0        0      730 2023-05-10 02:54:39.000000 cqlite-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 04:49:03.001129 cqlite-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       92 2023-05-10 02:37:30.000000 cqlite-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 04:49:02.949032 cqlite-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 04:49:02.971921 cqlite-0.0.1/src/cqlite/
--rw-rw-rw-   0        0        0       21 2023-05-10 02:37:30.000000 cqlite-0.0.1/src/cqlite/__init__.py
--rw-rw-rw-   0        0        0     5089 2023-05-10 04:44:01.000000 cqlite-0.0.1/src/cqlite/cqlite.py
-drwxrwxrwx   0        0        0        0 2023-05-10 04:49:02.997642 cqlite-0.0.1/src/cqlite.egg-info/
--rw-rw-rw-   0        0        0      637 2023-05-10 04:49:02.000000 cqlite-0.0.1/src/cqlite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-10 04:49:02.000000 cqlite-0.0.1/src/cqlite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 04:49:02.000000 cqlite-0.0.1/src/cqlite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-10 04:49:02.000000 cqlite-0.0.1/src/cqlite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-05-10 04:49:02.000000 cqlite-0.0.1/src/cqlite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 04:49:02.000000 cqlite-0.0.1/src/cqlite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 05:22:23.434189 cqlite-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-10 05:18:33.000000 cqlite-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      922 2023-05-10 05:22:23.432788 cqlite-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-10 05:20:21.000000 cqlite-0.1.0/README.md
+-rw-rw-rw-   0        0        0      730 2023-05-10 05:20:31.000000 cqlite-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 05:22:23.434738 cqlite-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       92 2023-05-10 05:18:33.000000 cqlite-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:22:23.365852 cqlite-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 05:22:23.402082 cqlite-0.1.0/src/cqlite/
+-rw-rw-rw-   0        0        0       21 2023-05-10 05:18:33.000000 cqlite-0.1.0/src/cqlite/__init__.py
+-rw-rw-rw-   0        0        0     5221 2023-05-10 05:18:47.000000 cqlite-0.1.0/src/cqlite/cqlite.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:22:23.431786 cqlite-0.1.0/src/cqlite.egg-info/
+-rw-rw-rw-   0        0        0      922 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 05:22:23.000000 cqlite-0.1.0/src/cqlite.egg-info/top_level.txt
```

### Comparing `cqlite-0.0.1/LICENSE` & `cqlite-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cqlite-0.0.1/pyproject.toml` & `cqlite-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cqlite"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="Emil Kloeden", email="emilkloeden@gmail.com" },
 ]
 description = "Query a CSV file from the commandline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cqlite-0.0.1/src/cqlite/cqlite.py` & `cqlite-0.1.0/src/cqlite/cqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         ]
         rows = list(csvreader)
         cols = rotate_n_rows(rows, 8)
         types = guess_types(cols)
         headers = list(zip(header_names, types))
         return headers, rows
 
-
 def populate_database(conn, cur, name, headers, rows):
     cur.execute(f"DROP TABLE IF EXISTS {name};")
     conn.commit()
     try:
         stmt = construct_create_table_stmt(name, headers)
         cur.execute(stmt)
         conn.commit()
@@ -159,16 +158,19 @@
     persist: bool = typer.Option(False, help="Save input to sqlite file."),
 ):
     file_path = Path(path_to_csv)
     if not file_path.exists():
         print(f"No such file: '{file_path}'")
         exit(1)
     name = file_path.stem
-    headers, rows = load_csv_file(file_path)
-
+    try:
+        headers, rows = load_csv_file(file_path)
+    except Exception as e:
+        print(f"Unable to load {file_path}. Perhaps it is not a CSV file?")
+        exit(1)
     if not query and not persist:
         print("Must supply a query or specify that you want the file contents saved to a sqlite file.")
 
     if persist:
         db_path = file_path.parent / f"{name}.db"
         conn = sqlite3.connect(db_path)
     else:
```

