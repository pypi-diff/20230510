# Comparing `tmp/pg_bulk_ingest-0.0.1.tar.gz` & `tmp/pg_bulk_ingest-0.0.2.tar.gz`

## Comparing `pg_bulk_ingest-0.0.1.tar` & `pg_bulk_ingest-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.1/pg_bulk_ingest.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.1/LICENSE
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.1/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/pg_bulk_ingest.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 pg_bulk_ingest-0.0.2/PKG-INFO
```

### Comparing `pg_bulk_ingest-0.0.1/pg_bulk_ingest.py` & `pg_bulk_ingest-0.0.2/pg_bulk_ingest.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,19 +38,24 @@
         for row, table in rows:
             if table is not first_table:
                 continue
             copy.write_row(row)
 
     # Copy from that intermediate table into the main table, using
     # ON CONFLICT to update any existing rows
-    primary_keys = tuple(column.name for column in first_table.columns if column.primary_key)
-    primary_keys_fragment = sql.SQL(',').join((sql.Identifier(primary_key) for primary_key in primary_keys)) 
-    insert_fragment = sql.SQL('INSERT INTO {}.{}').format(sql.Identifier(first_table.schema), sql.Identifier(first_table.name))
-    select_fragment = sql.SQL('SELECT DISTINCT ON({}) * FROM {}.{}').format(primary_keys_fragment, sql.Identifier(first_intermediate_table.schema), sql.Identifier(first_intermediate_table.name))
-    on_conflict_fragment = sql.SQL('ON CONFLICT(') + primary_keys_fragment + sql.SQL(')')
-    do_update_fragment = sql.SQL('DO UPDATE SET') + sql.SQL(',').join(sql.SQL('{} = EXCLUDED.{}').format(sql.Identifier(column.name), sql.Identifier(column.name)) for column in first_table.columns)
-    insert_query = insert_fragment + select_fragment + on_conflict_fragment + do_update_fragment
-
+    insert_query = sql.SQL('''
+        INSERT INTO {schema}.{table}
+        SELECT DISTINCT ON({primary_keys}) * FROM {intermediate_schema}.{intermediate_table}
+        ON CONFLICT({primary_keys})
+        DO UPDATE SET {updates}
+    ''').format(
+        schema=sql.Identifier(first_table.schema),
+        table=sql.Identifier(first_table.name),
+        intermediate_schema=sql.Identifier(first_intermediate_table.schema),
+        intermediate_table=sql.Identifier(first_intermediate_table.name),      
+        primary_keys=sql.SQL(',').join((sql.Identifier(column.name) for column in first_table.columns if column.primary_key)),
+        updates=sql.SQL(',').join(sql.SQL('{} = EXCLUDED.{}').format(sql.Identifier(column.name), sql.Identifier(column.name)) for column in first_table.columns),
+    )
     conn.execute(sa.text(insert_query.as_string(conn.connection.driver_connection)))
 
     # Drop the intermediate table
     metadata.drop_all(conn, tables=intermediate_tables)
```

### Comparing `pg_bulk_ingest-0.0.1/.gitignore` & `pg_bulk_ingest-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.1/LICENSE` & `pg_bulk_ingest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.1/README.md` & `pg_bulk_ingest-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pg_bulk_ingest-0.0.1/pyproject.toml` & `pg_bulk_ingest-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-bulk-ingest"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_bulk_ingest-0.0.1/PKG-INFO` & `pg_bulk_ingest-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-bulk-ingest
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of Python utility functions for ingesting data into SQLAlchemy-defined PostgreSQL tables, automatically migrating them as needed, and minimising locking
 Project-URL: Source, https://github.com/uktrade/pg-bulk-ingest
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

