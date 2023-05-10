# Comparing `tmp/pg_force_execute-0.0.7.tar.gz` & `tmp/pg_force_execute-0.0.8.tar.gz`

## Comparing `pg_force_execute-0.0.7.tar` & `pg_force_execute-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/pg_force_execute.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/LICENSE
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/README.md
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 pg_force_execute-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pg_force_execute-0.0.8/pg_force_execute.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pg_force_execute-0.0.8/README.md
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pg_force_execute-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pg_force_execute-0.0.8/PKG-INFO
```

### Comparing `pg_force_execute-0.0.7/pg_force_execute.py` & `pg_force_execute-0.0.8/pg_force_execute.py`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.7/.gitignore` & `pg_force_execute-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.7/LICENSE` & `pg_force_execute-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.7/README.md` & `pg_force_execute-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 query = 'SELECT 1'  # A more realistic example would be something that needs an exclusive lock on a table
 
 with \
         engine.begin() as conn, \
         pg_force_execute(
-            conn,           # SQLAlchemy connection to run the query
+            conn,                                 # SQLAlchemy connection to run the query
             delay=datetime.timedelta(minutes=5),  # Amount of time to wait before cancelling queries
         ):
 
     results = conn.execute(sa.text(query))
     print(results.fetchall())
 ```
```

### Comparing `pg_force_execute-0.0.7/pyproject.toml` & `pg_force_execute-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-force-execute"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that block them"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_force_execute-0.0.7/PKG-INFO` & `pg_force_execute-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-force-execute
-Version: 0.0.7
+Version: 0.0.8
 Summary: Context manager to run PostgreSQL queries with SQLAlchemy, terminating any other clients that block them
 Project-URL: Source, https://github.com/uktrade/pg-force-execute
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,15 @@
 
 engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 query = 'SELECT 1'  # A more realistic example would be something that needs an exclusive lock on a table
 
 with \
         engine.begin() as conn, \
         pg_force_execute(
-            conn,           # SQLAlchemy connection to run the query
+            conn,                                 # SQLAlchemy connection to run the query
             delay=datetime.timedelta(minutes=5),  # Amount of time to wait before cancelling queries
         ):
 
     results = conn.execute(sa.text(query))
     print(results.fetchall())
 ```
```

