# Comparing `tmp/latch_postgres-0.1.5.tar.gz` & `tmp/latch_postgres-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_postgres-0.1.5.tar", max compression
+gzip compressed data, was "latch_postgres-0.1.6.tar", max compression
```

## Comparing `latch_postgres-0.1.5.tar` & `latch_postgres-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.5/LICENSE
--rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-10 16:20:18.720567 latch_postgres-0.1.5/latch_postgres/__init__.py
--rw-r--r--   0        0        0    24224 2023-05-10 14:55:28.970229 latch_postgres-0.1.5/latch_postgres/postgres.py
--rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.5/latch_postgres/py.typed
--rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.5/latch_postgres/retries.py
--rw-r--r--   0        0        0     1018 2023-05-10 16:20:12.226724 latch_postgres-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.5/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.6/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 16:20:18.720567 latch_postgres-0.1.6/latch_postgres/__init__.py
+-rw-r--r--   0        0        0    24177 2023-05-10 17:24:58.509088 latch_postgres-0.1.6/latch_postgres/postgres.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.6/latch_postgres/py.typed
+-rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.6/latch_postgres/retries.py
+-rw-r--r--   0        0        0     1018 2023-05-10 17:24:55.837956 latch_postgres-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.6/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.6/PKG-INFO
```

### Comparing `latch_postgres-0.1.5/LICENSE` & `latch_postgres-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.5/latch_postgres/postgres.py` & `latch_postgres-0.1.6/latch_postgres/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Iterable,
     ParamSpec,
     TypeVar,
     cast,
 )
 
 import psycopg.sql as sql
-from latch_config.config import DatabaseConfig, read_config
+from latch_config.config import DatabaseConfig
 from latch_data_validation.data_validation import JsonObject, validate
 from latch_o11y.o11y import dict_to_attrs, trace_function
 from opentelemetry.sdk.resources import Attributes
 from opentelemetry.trace import SpanKind, get_tracer
 from psycopg import AsyncConnection, AsyncCursor, IsolationLevel
 from psycopg.abc import AdaptContext, Params, Query
 from psycopg.conninfo import conninfo_to_dict, make_conninfo
@@ -63,17 +63,14 @@
 
 from latch_postgres.retries import CABackoff
 
 T = TypeVar("T")
 
 tracer = get_tracer(__name__)
 
-db_config = read_config(DatabaseConfig)
-
-
 # todo(maximsmol): switch all the tracing attributes to otel spec
 # del span.type
 # in event names postgres -> postgresql (or to psycopg)?
 # out.host -> net.peer.name
 # out.port -> net.peer.port
 # sql.query -> db.statement
 # del resource.name
@@ -482,15 +479,15 @@
         "type": type(x).__name__,
     }
 
 
 def with_conn_retry(
     f: Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]],
     pool: AsyncConnectionPool,
-    db_config=db_config,
+    db_config: DatabaseConfig,
 ) -> Callable[P, Awaitable[T]]:
     @functools.wraps(f)
     async def inner(*args: P.args, **kwargs: P.kwargs):
         with tracer.start_as_current_span("database session") as s:
             try:
                 retries = 0
                 accum_retry_time = 0
@@ -606,15 +603,15 @@
 
                 raise e
 
     return inner
 
 
 def get_with_conn_retry(
-    pool: AsyncConnectionPool, db_config=db_config
+    pool: AsyncConnectionPool, db_config: DatabaseConfig
 ) -> Callable[
     [Callable[Concatenate[LatchAsyncConnection[Any], P], Awaitable[T]]],
     Callable[P, Awaitable[T]],
 ]:
     return functools.partial(with_conn_retry, pool=pool, db_config=db_config)
 
 
@@ -632,16 +629,15 @@
 
     if x.isolation_level != IsolationLevel.SERIALIZABLE:
         await x.set_isolation_level(IsolationLevel.SERIALIZABLE)
 
 
 # fixme(maximsmol): use autocommit transactions
 def get_pool(
-    config: DatabaseConfig,
-    application_name: str
+    config: DatabaseConfig, application_name: str
 ) -> TracedAsyncConnectionPool:
     conn_str = make_conninfo(
         host=config.host,
         port=config.port,
         dbname=config.dbname,
         user=config.user,
         password=config.password,
```

### Comparing `latch_postgres-0.1.5/latch_postgres/retries.py` & `latch_postgres-0.1.6/latch_postgres/retries.py`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.5/pyproject.toml` & `latch_postgres-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-postgres"
-version = "0.1.5"
+version = "0.1.6"
 description = "Postges wrapper for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_postgres"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_postgres-0.1.5/setup.py` & `latch_postgres-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'latch-postgres',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Postges wrapper for latch python backend services',
     'long_description': '# python-postgres\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_postgres-0.1.5/PKG-INFO` & `latch_postgres-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-postgres
-Version: 0.1.5
+Version: 0.1.6
 Summary: Postges wrapper for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

