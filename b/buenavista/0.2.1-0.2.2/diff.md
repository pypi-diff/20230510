# Comparing `tmp/buenavista-0.2.1.tar.gz` & `tmp/buenavista-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buenavista-0.2.1.tar", last modified: Tue Apr 25 23:03:11 2023, max compression
+gzip compressed data, was "buenavista-0.2.2.tar", last modified: Wed May 10 21:05:42 2023, max compression
```

## Comparing `buenavista-0.2.1.tar` & `buenavista-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.916820 buenavista-0.2.1/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:44.000000 buenavista-0.2.1/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)     1901 2023-04-25 23:03:11.916703 buenavista-0.2.1/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1566 2023-03-03 20:38:14.000000 buenavista-0.2.1/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.913102 buenavista-0.2.1/buenavista/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2022-12-27 19:08:41.000000 buenavista-0.2.1/buenavista/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.914506 buenavista-0.2.1/buenavista/backends/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2023-01-13 04:28:53.000000 buenavista-0.2.1/buenavista/backends/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     7478 2023-04-25 23:01:34.000000 buenavista-0.2.1/buenavista/backends/duckdb.py
--rw-r--r--   0 jwills     (501) staff       (20)     3384 2023-03-10 16:36:56.000000 buenavista-0.2.1/buenavista/backends/postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)     2486 2023-03-10 16:36:56.000000 buenavista-0.2.1/buenavista/bv_dialects.py
--rw-r--r--   0 jwills     (501) staff       (20)     3148 2023-04-25 23:01:34.000000 buenavista-0.2.1/buenavista/core.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.915330 buenavista-0.2.1/buenavista/examples/
--rw-r--r--   0 jwills     (501) staff       (20)     3540 2023-04-03 05:42:19.000000 buenavista-0.2.1/buenavista/examples/duckdb_http.py
--rw-r--r--   0 jwills     (501) staff       (20)     1218 2023-03-10 16:36:56.000000 buenavista-0.2.1/buenavista/examples/duckdb_postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)      428 2023-03-10 16:36:56.000000 buenavista-0.2.1/buenavista/examples/postgres_proxy.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.916458 buenavista-0.2.1/buenavista/http/
--rw-r--r--   0 jwills     (501) staff       (20)        0 2023-03-21 18:23:57.000000 buenavista-0.2.1/buenavista/http/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)     3247 2023-04-03 05:42:19.000000 buenavista-0.2.1/buenavista/http/context.py
--rw-r--r--   0 jwills     (501) staff       (20)     4298 2023-04-03 05:42:19.000000 buenavista-0.2.1/buenavista/http/main.py
--rw-r--r--   0 jwills     (501) staff       (20)     2227 2023-03-09 18:25:32.000000 buenavista-0.2.1/buenavista/http/schemas.py
--rw-r--r--   0 jwills     (501) staff       (20)     1709 2023-03-09 18:25:32.000000 buenavista-0.2.1/buenavista/http/type_mapping.py
--rw-r--r--   0 jwills     (501) staff       (20)    19000 2023-04-25 23:01:34.000000 buenavista-0.2.1/buenavista/postgres.py
--rw-r--r--   0 jwills     (501) staff       (20)     1840 2023-04-25 17:26:47.000000 buenavista-0.2.1/buenavista/rewrite.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-25 23:03:11.914140 buenavista-0.2.1/buenavista.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)     1901 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      652 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       83 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)       11 2023-04-25 23:03:11.000000 buenavista-0.2.1/buenavista.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-04-25 23:03:11.916856 buenavista-0.2.1/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1022 2023-04-25 23:01:34.000000 buenavista-0.2.1/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-10 21:05:42.631270 buenavista-0.2.2/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:44.000000 buenavista-0.2.2/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-05-10 21:05:42.631154 buenavista-0.2.2/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1575 2023-05-10 16:04:37.000000 buenavista-0.2.2/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-10 21:05:42.628882 buenavista-0.2.2/buenavista/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2022-12-27 19:08:41.000000 buenavista-0.2.2/buenavista/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-10 21:05:42.630067 buenavista-0.2.2/buenavista/backends/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2023-01-13 04:28:53.000000 buenavista-0.2.2/buenavista/backends/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7482 2023-05-10 21:05:33.000000 buenavista-0.2.2/buenavista/backends/duckdb.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3359 2023-05-10 21:05:33.000000 buenavista-0.2.2/buenavista/backends/postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2487 2023-05-09 19:09:29.000000 buenavista-0.2.2/buenavista/bv_dialects.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3148 2023-04-25 23:01:34.000000 buenavista-0.2.2/buenavista/core.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-10 21:05:42.630410 buenavista-0.2.2/buenavista/examples/
+-rw-r--r--   0 jwills     (501) staff       (20)     3540 2023-04-03 05:42:19.000000 buenavista-0.2.2/buenavista/examples/duckdb_http.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1472 2023-05-10 21:05:33.000000 buenavista-0.2.2/buenavista/examples/duckdb_postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)      428 2023-03-10 16:36:56.000000 buenavista-0.2.2/buenavista/examples/postgres_proxy.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-10 21:05:42.630985 buenavista-0.2.2/buenavista/http/
+-rw-r--r--   0 jwills     (501) staff       (20)        0 2023-03-21 18:23:57.000000 buenavista-0.2.2/buenavista/http/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3247 2023-04-03 05:42:19.000000 buenavista-0.2.2/buenavista/http/context.py
+-rw-r--r--   0 jwills     (501) staff       (20)     4298 2023-04-03 05:42:19.000000 buenavista-0.2.2/buenavista/http/main.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2227 2023-03-09 18:25:32.000000 buenavista-0.2.2/buenavista/http/schemas.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1709 2023-03-09 18:25:32.000000 buenavista-0.2.2/buenavista/http/type_mapping.py
+-rw-r--r--   0 jwills     (501) staff       (20)    20676 2023-05-10 16:04:37.000000 buenavista-0.2.2/buenavista/postgres.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1840 2023-04-25 17:26:47.000000 buenavista-0.2.2/buenavista/rewrite.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-10 21:05:42.629736 buenavista-0.2.2/buenavista.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-05-10 21:05:42.000000 buenavista-0.2.2/buenavista.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      652 2023-05-10 21:05:42.000000 buenavista-0.2.2/buenavista.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-10 21:05:42.000000 buenavista-0.2.2/buenavista.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       83 2023-05-10 21:05:42.000000 buenavista-0.2.2/buenavista.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       11 2023-05-10 21:05:42.000000 buenavista-0.2.2/buenavista.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-10 21:05:42.631305 buenavista-0.2.2/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1022 2023-05-10 21:05:33.000000 buenavista-0.2.2/setup.py
```

### Comparing `buenavista-0.2.1/LICENSE` & `buenavista-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/PKG-INFO` & `buenavista-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buenavista
-Version: 0.2.1
+Version: 0.2.2
 Summary: Programmable Presto and Postgres Proxies
 Home-page: https://github.com/jwills/buenavista
 Author: Josh Wills
 Author-email: joshwills+bv@gmail.com
 License: Apache
 Description-Content-Type: text/markdown
 Provides-Extra: duckdb
@@ -22,14 +22,14 @@
 with a database query tool like [DBeaver](https://dbeaver.io/) to examine the state of the database, because each DuckDB file
 may only be open by a single process at a time. The Buena Vista library makes it possible to work with a DuckDB database
 from multiple different processes over the Postgres wire protocol, and the library makes it simple enough to run an example
 that illustrates the idea locally:
 
 ```sh
 pip3 install buenavista
-python3 -m buenavista.backends.duckdb <optional_duckdb_file>
+python3 -m buenavista.examples.duckdb_postgres <optional_duckdb_file>
 ```
 
 in order to start a Postgres server on `localhost:5433` backed by the DuckDB database file that you passed in at the command line
 (or by an in-memory DuckDB database if you do not specify an argument.) You should be able to query the database via `psql` in
 another window by running `psql -h localhost -p 5433` (no database/username/password arguments required) or by using the DBeaver
 Postgres client connection.
```

### Comparing `buenavista-0.2.1/README.md` & `buenavista-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 with a database query tool like [DBeaver](https://dbeaver.io/) to examine the state of the database, because each DuckDB file
 may only be open by a single process at a time. The Buena Vista library makes it possible to work with a DuckDB database
 from multiple different processes over the Postgres wire protocol, and the library makes it simple enough to run an example
 that illustrates the idea locally:
 
 ```sh
 pip3 install buenavista
-python3 -m buenavista.backends.duckdb <optional_duckdb_file>
+python3 -m buenavista.examples.duckdb_postgres <optional_duckdb_file>
 ```
 
 in order to start a Postgres server on `localhost:5433` backed by the DuckDB database file that you passed in at the command line
 (or by an in-memory DuckDB database if you do not specify an argument.) You should be able to query the database via `psql` in
 another window by running `psql -h localhost -p 5433` (no database/username/password arguments required) or by using the DBeaver
 Postgres client connection.
```

### Comparing `buenavista-0.2.1/buenavista/backends/duckdb.py` & `buenavista-0.2.2/buenavista/backends/duckdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,17 +202,17 @@
             elif "begin" in lsql or "start transaction" in lsql:
                 return DuckDBQueryResult(status="BEGIN")
         elif "begin" in lsql or "start transaction" in lsql:
             lsql = "begin"
             self.in_txn = True
             status = "BEGIN"
 
-        logger.debug("Original SQL: ", sql)
+        logger.debug("Original SQL: %s", sql)
         sql = self.rewrite_sql(sql)
-        logger.debug("Rewritten SQL: ", sql)
+        logger.debug("Rewritten SQL: %s", sql)
         if params:
             self._cursor.execute(sql, params)
         else:
             self._cursor.execute(sql)
 
         if status:
             return DuckDBQueryResult(status=status)
```

### Comparing `buenavista-0.2.1/buenavista/backends/postgres.py` & `buenavista-0.2.2/buenavista/backends/postgres.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import io
-import logging
-import os
 import re
 from typing import Any, Dict, Iterator, List, Optional, Tuple
 
 import pandas as pd
 import psycopg
 from psycopg_pool import ConnectionPool
```

### Comparing `buenavista-0.2.1/buenavista/bv_dialects.py` & `buenavista-0.2.2/buenavista/bv_dialects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from sqlglot import exp
 from sqlglot.dialects import DuckDB, Postgres, Trino
 from sqlglot.tokens import TokenType
 
+
 # Additional expressions I need
 class ToISO8601(exp.Func):
     pass
 
 
 class BVPostgres(Postgres):
     pass
```

### Comparing `buenavista-0.2.1/buenavista/core.py` & `buenavista-0.2.2/buenavista/core.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/buenavista/examples/duckdb_http.py` & `buenavista-0.2.2/buenavista/examples/duckdb_http.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/buenavista/examples/duckdb_postgres.py` & `buenavista-0.2.2/buenavista/examples/duckdb_postgres.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import os
 import sys
+from typing import Tuple
 
 import duckdb
 
 from ..backends.duckdb import DuckDBConnection
 from .. import bv_dialects, postgres, rewrite
 
 
 class DuckDBPostgresRewriter(rewrite.Rewriter):
     def rewrite(self, sql: str) -> str:
-        if sql == "select pg_catalog.version()":
+        if sql.lower() == "select pg_catalog.version()":
             return "SELECT 'PostgreSQL 9.3' as version"
-        return super().rewrite(sql)
+        else:
+            return super().rewrite(sql)
 
 
 rewriter = DuckDBPostgresRewriter(bv_dialects.BVPostgres(), bv_dialects.BVDuckDB())
 
 
-if __name__ == "__main__":
+def create(
+    db: duckdb.DuckDBPyConnection, host_addr: Tuple[str, int], auth: dict = None
+) -> postgres.BuenaVistaServer:
+    server = postgres.BuenaVistaServer(
+        host_addr, DuckDBConnection(db), rewriter=rewriter, auth=auth
+    )
+    return server
+
 
+if __name__ == "__main__":
     if len(sys.argv) < 2:
         print("Using in-memory DuckDB database")
         db = duckdb.connect()
     else:
         print("Using DuckDB database at %s" % sys.argv[1])
         db = duckdb.connect(sys.argv[1])
 
@@ -32,16 +42,15 @@
     if "BUENAVISTA_HOST" in os.environ:
         bv_host = os.environ["BUENAVISTA_HOST"]
 
     if "BUENAVISTA_PORT" in os.environ:
         bv_port = int(os.environ["BUENAVISTA_PORT"])
 
     address = (bv_host, bv_port)
-
-    server = postgres.BuenaVistaServer(address, DuckDBConnection(db), rewriter=rewriter)
+    server = create(db, address)
     ip, port = server.server_address
     print(f"Listening on {ip}:{port}")
 
     try:
         server.serve_forever()
     finally:
         server.shutdown()
```

### Comparing `buenavista-0.2.1/buenavista/http/context.py` & `buenavista-0.2.2/buenavista/http/context.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/buenavista/http/main.py` & `buenavista-0.2.2/buenavista/http/main.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/buenavista/http/schemas.py` & `buenavista-0.2.2/buenavista/http/schemas.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/buenavista/http/type_mapping.py` & `buenavista-0.2.2/buenavista/http/type_mapping.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/buenavista/postgres.py` & `buenavista-0.2.2/buenavista/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import io
 import json
 import logging
 import os
 import random
 import socketserver
 import struct
@@ -49,14 +50,15 @@
     BIND = b"B"
     CLOSE = b"C"
     DESCRIBE = b"D"
     EXECUTE = b"E"
     FLUSH = b"H"
     QUERY = b"Q"
     PARSE = b"P"
+    PASSWORD_MESSAGE = b"p"
     SYNC = b"S"
     TERMINATE = b"X"
 
 
 PG_UNKNOWN = (705, str)
 BVTYPE_TO_PGTYPE = {
     BVType.NULL: (-1, lambda v: None),
@@ -138,31 +140,39 @@
         self.params = params
         self.process_id = random.randint(0, 2**32 - 1)
         self.secret_key = random.randint(0, 2**32 - 1)
         self.stmts = {}
         self.portals = {}
         self.result_cache = {}
         self.has_error = False
+        self.authenticated = False
+        self.salt = None
+
+    def get_hashed_password(self, auth: dict) -> str:
+        user = self.params["user"]
+        password = auth[user]
+        first = hashlib.md5(password.encode("utf-8") + user.encode("utf-8")).hexdigest()
+        return "md5" + hashlib.md5(first.encode("utf-8") + self.salt).hexdigest()
 
     def mark_error(self):
         self.has_error = True
 
     def transaction_status(self):
         if self.session.in_transaction():
             if self.has_error:
                 return TransactionStatus.IN_FAILED_TRANSACTION
             else:
                 return TransactionStatus.IN_TRANSACTION
         return TransactionStatus.IDLE
 
     def execute_sql(self, sql: str, params=None) -> QueryResult:
-        print("Input SQL: " + sql)
+        logger.info("Input SQL: " + sql)
         if self.rewriter:
             sql = self.rewriter.rewrite(sql)
-            print("Rewritten SQL: " + sql)
+            logger.info("Rewritten SQL: " + sql)
         return self.session.execute_sql(sql, params)
 
     def describe_portal(self, name: str) -> QueryResult:
         stmt, params = self.portals[name]
         sql = self.stmts[stmt]
         query_result = self.execute_sql(sql=sql, params=params)
         self.result_cache[name] = query_result
@@ -218,15 +228,20 @@
 
                 msglen = self.r.read_uint32()
                 if msglen > 4:
                     payload = self.r.read_bytes(msglen - 4)
                 else:
                     payload = None
 
-                if type_code == ClientCommand.QUERY:
+                if not ctx.authenticated:
+                    if type_code == ClientCommand.PASSWORD_MESSAGE:
+                        self.handle_md5_password(ctx, payload)
+                    else:
+                        raise Exception("Not authenticated")
+                elif type_code == ClientCommand.QUERY:
                     self.handle_query(ctx, payload)
                 elif type_code == ClientCommand.PARSE:
                     self.handle_parse(ctx, payload)
                 elif type_code == ClientCommand.BIND:
                     self.handle_bind(ctx, payload)
                 elif type_code == ClientCommand.DESCRIBE:
                     self.handle_describe(ctx, payload)
@@ -260,30 +275,62 @@
             msg = [
                 x.decode("utf-8")
                 for x in self.r.read_bytes(msglen - 4).split(NULL_BYTE)
             ]
             params = dict(zip(msg[::2], msg[1::2]))
             logger.info("Client connection params: %s", params)
             ctx = BVContext(conn.create_session(), self.server.rewriter, params)
-            self.send_authentication_ok()
-            self.send_parameter_status(conn.parameters())
-            self.send_backend_key_data(ctx)
-            self.send_ready_for_query(ctx)
+            self.send_auth_request(ctx)
             return ctx
         elif code == 80877102:  ## Cancel request
             process_id, secret_key = self.r.read_uint32(), self.r.read_uint32()
             ctx = self.server.ctxts.get(process_id)
             if ctx and ctx.secret_key == secret_key:
                 self.server.conn.close_session(ctx.session)
                 del self.server.ctxts[ctx.process_id]
                 ctx = None
             return None
         else:
             raise Exception(f"Unsupported startup message: {code}")
 
+    def send_auth_request(self, ctx: BVContext):
+        if self.server.auth is None:
+            self.send_authentication_ok()
+            self.handle_post_auth(ctx)
+        else:
+            self.send_authentication_md5(ctx)
+
+    def send_authentication_ok(self):
+        self.wfile.write(
+            struct.pack("!cii", ServerResponse.AUTHENTICATION_REQUEST, 8, 0)
+        )
+
+    def send_authentication_md5(self, ctx: BVContext):
+        ctx.salt = os.urandom(4)
+        self.wfile.write(
+            struct.pack("!cii", ServerResponse.AUTHENTICATION_REQUEST, 12, 5)
+        )
+        self.wfile.write(ctx.salt)
+
+    def handle_md5_password(self, ctx: BVContext, payload: bytes):
+        client_side = payload.decode("utf-8").rstrip("\x00")
+        server_side = ctx.get_hashed_password(self.server.auth)
+        if client_side == server_side:
+            self.send_authentication_ok()
+            self.handle_post_auth(ctx)
+        else:
+            self.send_error("Invalid password")
+
+    def handle_post_auth(self, ctx: BVContext):
+        self.send_parameter_status(self.server.conn.parameters())
+        self.send_backend_key_data(ctx)
+        self.send_ready_for_query(ctx)
+        ctx.authenticated = True
+        return
+
     def handle_query(self, ctx: BVContext, payload: bytes):
         logger.debug("Handle query")
         decoded = payload.decode("utf-8").rstrip("\x00")
         try:
             # JSON payloads signal that we should use extensions
             if req := Extension.check_json(decoded):
                 method = req.get("method")
@@ -471,19 +518,14 @@
         self.wfile.write(err_sig + out)
         if ctx:
             ctx.mark_error()
 
     def send_notice(self):
         self.wfile.write(ServerResponse.NOTICE_RESPONSE)
 
-    def send_authentication_ok(self):
-        self.wfile.write(
-            struct.pack("!cii", ServerResponse.AUTHENTICATION_REQUEST, 8, 0)
-        )
-
     def send_backend_key_data(self, ctx):
         self.wfile.write(
             struct.pack(
                 "!ciII",
                 ServerResponse.BACKEND_KEY_DATA,
                 12,
                 ctx.process_id,
@@ -532,17 +574,19 @@
     def __init__(
         self,
         server_address,
         conn: Connection,
         *,
         rewriter: Optional[Rewriter] = None,
         extensions: List[Extension] = [],
+        auth: Optional[Dict[str, str]] = None,
     ):
         super().__init__(server_address, BuenaVistaHandler)
         self.conn = conn
         self.rewriter = rewriter
         self.extensions = {e.type(): e for e in extensions}
         self.ctxts = {}
+        self.auth = auth
 
     def verify_request(self, request, client_address) -> bool:
         """Ensure all requests come from localhost until auth is in place"""
         return client_address[0] == "127.0.0.1" or "BUENAVISTA_HOST" in os.environ
```

### Comparing `buenavista-0.2.1/buenavista/rewrite.py` & `buenavista-0.2.2/buenavista/rewrite.py`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/buenavista.egg-info/PKG-INFO` & `buenavista-0.2.2/buenavista.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buenavista
-Version: 0.2.1
+Version: 0.2.2
 Summary: Programmable Presto and Postgres Proxies
 Home-page: https://github.com/jwills/buenavista
 Author: Josh Wills
 Author-email: joshwills+bv@gmail.com
 License: Apache
 Description-Content-Type: text/markdown
 Provides-Extra: duckdb
@@ -22,14 +22,14 @@
 with a database query tool like [DBeaver](https://dbeaver.io/) to examine the state of the database, because each DuckDB file
 may only be open by a single process at a time. The Buena Vista library makes it possible to work with a DuckDB database
 from multiple different processes over the Postgres wire protocol, and the library makes it simple enough to run an example
 that illustrates the idea locally:
 
 ```sh
 pip3 install buenavista
-python3 -m buenavista.backends.duckdb <optional_duckdb_file>
+python3 -m buenavista.examples.duckdb_postgres <optional_duckdb_file>
 ```
 
 in order to start a Postgres server on `localhost:5433` backed by the DuckDB database file that you passed in at the command line
 (or by an in-memory DuckDB database if you do not specify an argument.) You should be able to query the database via `psql` in
 another window by running `psql -h localhost -p 5433` (no database/username/password arguments required) or by using the DBeaver
 Postgres client connection.
```

### Comparing `buenavista-0.2.1/buenavista.egg-info/SOURCES.txt` & `buenavista-0.2.2/buenavista.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buenavista-0.2.1/setup.py` & `buenavista-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "buenavista"
-package_version = "0.2.1"
+package_version = "0.2.2"
 
 description = """Programmable Presto and Postgres Proxies"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

