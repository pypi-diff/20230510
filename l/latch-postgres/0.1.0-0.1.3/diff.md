# Comparing `tmp/latch_postgres-0.1.0.tar.gz` & `tmp/latch_postgres-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_postgres-0.1.0.tar", max compression
+gzip compressed data, was "latch_postgres-0.1.3.tar", max compression
```

## Comparing `latch_postgres-0.1.0.tar` & `latch_postgres-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.0/LICENSE
--rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.0/README.md
--rw-r--r--   0        0        0    23845 2023-04-27 20:58:29.910206 latch_postgres-0.1.0/latch_postgres/postgres.py
--rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.0/latch_postgres/retries.py
--rw-r--r--   0        0        0     1018 2023-04-27 21:17:17.543523 latch_postgres-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.0/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.3/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.3/README.md
+-rw-r--r--   0        0        0    24195 2023-05-10 02:58:10.102144 latch_postgres-0.1.3/latch_postgres/postgres.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.3/latch_postgres/py.typed
+-rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.3/latch_postgres/retries.py
+-rw-r--r--   0        0        0     1018 2023-05-10 02:58:27.961994 latch_postgres-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.3/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.3/PKG-INFO
```

### Comparing `latch_postgres-0.1.0/LICENSE` & `latch_postgres-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.0/latch_postgres/postgres.py` & `latch_postgres-0.1.3/latch_postgres/postgres.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     Iterable,
     ParamSpec,
     TypeVar,
     cast,
 )
 
 import psycopg.sql as sql
+from latch_config.config import DatabaseConfig, read_config
+from latch_data_validation.data_validation import JsonObject, validate
+from latch_o11y.o11y import dict_to_attrs, trace_function
 from opentelemetry.sdk.resources import Attributes
 from opentelemetry.trace import SpanKind, get_tracer
 from psycopg import AsyncConnection, AsyncCursor, IsolationLevel
 from psycopg.abc import AdaptContext, Params, Query
 from psycopg.conninfo import conninfo_to_dict, make_conninfo
 from psycopg.errors import (
     AdminShutdown,
@@ -56,23 +59,19 @@
 from psycopg.types.composite import CompositeInfo, register_composite
 from psycopg.types.enum import EnumInfo, register_enum
 from psycopg_pool import AsyncConnectionPool
 from typing_extensions import Self
 
 from latch_postgres.retries import CABackoff
 
-from latch_config.config import config
-from latch_data_validation.data_validation import JsonObject, validate
-from latch_o11y.o11y import dict_to_attrs, trace_function
-
 T = TypeVar("T")
 
 tracer = get_tracer(__name__)
 
-db_config = config.database
+db_config = read_config(DatabaseConfig)
 
 
 # todo(maximsmol): switch all the tracing attributes to otel spec
 # del span.type
 # in event names postgres -> postgresql (or to psycopg)?
 # out.host -> net.peer.name
 # out.port -> net.peer.port
@@ -481,15 +480,17 @@
         "sqlstate": x.sqlstate,
         "diagnostic": diagnostic_obj,
         "type": type(x).__name__,
     }
 
 
 def with_conn_retry(
-    f: Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]]
+    f: Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]],
+    pool: AsyncConnectionPool,
+    db_config=db_config,
 ) -> Callable[P, Awaitable[T]]:
     @functools.wraps(f)
     async def inner(*args: P.args, **kwargs: P.kwargs):
         with tracer.start_as_current_span("database session") as s:
             try:
                 retries = 0
                 accum_retry_time = 0
@@ -570,26 +571,23 @@
                         OperationalError,
                     ) as e:
                         # Connection is dead. Get a new one and retry
 
                         # todo(maximsmol): add metrics
                         retries += 1
 
-                        if (
-                            accum_retry_time
-                            > config.database.conn_retries.max_wait_time
-                        ):
+                        if accum_retry_time > db_config.conn_retries.max_wait_time:
                             raise
 
                         if retries == 1:
                             delay = 0
                         else:
                             delay = random.uniform(
-                                config.database.conn_retries.min_retry_time,
-                                config.database.conn_retries.max_retry_time,
+                                db_config.conn_retries.min_retry_time,
+                                db_config.conn_retries.max_retry_time,
                             )
 
                         s.add_event(
                             "connection retry",
                             {
                                 "db.retry.count": retries,
                                 "db.retry.accum_retry_time": str(accum_retry_time),
@@ -607,14 +605,23 @@
                 s.set_attributes(dict_to_attrs(pg_error_to_dict(e), "db.error"))
 
                 raise e
 
     return inner
 
 
+def get_with_conn_retry(
+    pool: AsyncConnectionPool, db_config=db_config
+) -> Callable[
+    [Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]]],
+    Callable[P, Awaitable[T]],
+]:
+    return functools.partial(with_conn_retry, pool=pool, db_config=db_config)
+
+
 def sqlq(x: str):
     return sql.SQL(dedent(x))
 
 
 # todo(maximsmol): conn resets appear in the startup span and make it last forever
 @trace_function(tracer)
 async def reset_conn(x: AsyncConnection[object]):
@@ -624,25 +631,26 @@
         await x.set_read_only(True)
 
     if x.isolation_level != IsolationLevel.SERIALIZABLE:
         await x.set_isolation_level(IsolationLevel.SERIALIZABLE)
 
 
 # fixme(maximsmol): use autocommit transactions
-conn_str = make_conninfo(
-    host=config.database.host,
-    port=config.database.port,
-    dbname=config.database.dbname,
-    user=config.database.user,
-    password=config.database.password,
-    application_name="latch_nucleus_data",
-)
-pool = TracedAsyncConnectionPool(
-    conn_str,
-    min_size=1,
-    max_size=config.database.pool_size,
-    timeout=timedelta(seconds=5) / timedelta(seconds=1),
-    open=False,  # tied into the server lifecycle instead
-    configure=reset_conn,
-    reset=reset_conn,
-    connection_class=LatchAsyncConnection,
-)
+def get_pool(config: DatabaseConfig) -> TracedAsyncConnectionPool:
+    conn_str = make_conninfo(
+        host=config.host,
+        port=config.port,
+        dbname=config.dbname,
+        user=config.user,
+        password=config.password,
+        application_name="latch_nucleus_data",
+    )
+    return TracedAsyncConnectionPool(
+        conn_str,
+        min_size=1,
+        max_size=config.pool_size,
+        timeout=timedelta(seconds=5) / timedelta(seconds=1),
+        open=False,  # tied into the server lifecycle instead
+        configure=reset_conn,
+        reset=reset_conn,
+        connection_class=LatchAsyncConnection,
+    )
```

### Comparing `latch_postgres-0.1.0/latch_postgres/retries.py` & `latch_postgres-0.1.3/latch_postgres/retries.py`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.0/pyproject.toml` & `latch_postgres-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "latch-postgres"
-version = "0.1.0"
+version = "0.1.3"
 description = "Postges wrapper for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_postgres"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typing-extensions = "^4.4.0"
 psycopg = { extras = ["pool", "binary"], version = "^3.1.8" }
-latch-config = "^0.1.1"
-latch-data-validation = "^0.1.0"
-latch-o11y = "^0.1.0"
+latch-config = "^0.1.4"
+latch-data-validation = "^0.1.2"
+latch-o11y = "^0.1.3"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 rich = "^13.2.0"
```

### Comparing `latch_postgres-0.1.0/setup.py` & `latch_postgres-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['latch_postgres']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['latch-config>=0.1.1,<0.2.0',
- 'latch-data-validation>=0.1.0,<0.2.0',
- 'latch-o11y>=0.1.0,<0.2.0',
+['latch-config>=0.1.4,<0.2.0',
+ 'latch-data-validation>=0.1.2,<0.2.0',
+ 'latch-o11y>=0.1.3,<0.2.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'latch-postgres',
-    'version': '0.1.0',
+    'version': '0.1.3',
     'description': 'Postges wrapper for latch python backend services',
     'long_description': '# python-postgres\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_postgres-0.1.0/PKG-INFO` & `latch_postgres-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: latch-postgres
-Version: 0.1.0
+Version: 0.1.3
 Summary: Postges wrapper for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: latch-config (>=0.1.1,<0.2.0)
-Requires-Dist: latch-data-validation (>=0.1.0,<0.2.0)
-Requires-Dist: latch-o11y (>=0.1.0,<0.2.0)
+Requires-Dist: latch-config (>=0.1.4,<0.2.0)
+Requires-Dist: latch-data-validation (>=0.1.2,<0.2.0)
+Requires-Dist: latch-o11y (>=0.1.3,<0.2.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.8,<4.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # python-postgres
```

