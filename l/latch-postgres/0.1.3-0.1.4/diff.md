# Comparing `tmp/latch_postgres-0.1.3.tar.gz` & `tmp/latch_postgres-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_postgres-0.1.3.tar", max compression
+gzip compressed data, was "latch_postgres-0.1.4.tar", max compression
```

## Comparing `latch_postgres-0.1.3.tar` & `latch_postgres-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.3/LICENSE
--rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.3/README.md
--rw-r--r--   0        0        0    24195 2023-05-10 02:58:10.102144 latch_postgres-0.1.3/latch_postgres/postgres.py
--rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.3/latch_postgres/py.typed
--rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.3/latch_postgres/retries.py
--rw-r--r--   0        0        0     1018 2023-05-10 02:58:27.961994 latch_postgres-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.3/setup.py
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 18:09:35.301064 latch_postgres-0.1.4/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-27 18:34:23.535053 latch_postgres-0.1.4/README.md
+-rw-r--r--   0        0        0    24224 2023-05-10 14:55:28.970229 latch_postgres-0.1.4/latch_postgres/postgres.py
+-rw-r--r--   0        0        0        0 2023-05-09 21:55:58.985422 latch_postgres-0.1.4/latch_postgres/py.typed
+-rw-r--r--   0        0        0     1308 2023-04-27 18:36:31.699816 latch_postgres-0.1.4/latch_postgres/retries.py
+-rw-r--r--   0        0        0     1018 2023-05-10 14:56:07.895949 latch_postgres-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 latch_postgres-0.1.4/setup.py
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 latch_postgres-0.1.4/PKG-INFO
```

### Comparing `latch_postgres-0.1.3/LICENSE` & `latch_postgres-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.3/latch_postgres/postgres.py` & `latch_postgres-0.1.4/latch_postgres/postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,22 +631,25 @@
         await x.set_read_only(True)
 
     if x.isolation_level != IsolationLevel.SERIALIZABLE:
         await x.set_isolation_level(IsolationLevel.SERIALIZABLE)
 
 
 # fixme(maximsmol): use autocommit transactions
-def get_pool(config: DatabaseConfig) -> TracedAsyncConnectionPool:
+def get_pool(
+    config: DatabaseConfig,
+    application_name: str
+) -> TracedAsyncConnectionPool:
     conn_str = make_conninfo(
         host=config.host,
         port=config.port,
         dbname=config.dbname,
         user=config.user,
         password=config.password,
-        application_name="latch_nucleus_data",
+        application_name=application_name,
     )
     return TracedAsyncConnectionPool(
         conn_str,
         min_size=1,
         max_size=config.pool_size,
         timeout=timedelta(seconds=5) / timedelta(seconds=1),
         open=False,  # tied into the server lifecycle instead
```

### Comparing `latch_postgres-0.1.3/latch_postgres/retries.py` & `latch_postgres-0.1.4/latch_postgres/retries.py`

 * *Files identical despite different names*

### Comparing `latch_postgres-0.1.3/pyproject.toml` & `latch_postgres-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-postgres"
-version = "0.1.3"
+version = "0.1.4"
 description = "Postges wrapper for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_postgres"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_postgres-0.1.3/setup.py` & `latch_postgres-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'latch-postgres',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Postges wrapper for latch python backend services',
     'long_description': '# python-postgres\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_postgres-0.1.3/PKG-INFO` & `latch_postgres-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-postgres
-Version: 0.1.3
+Version: 0.1.4
 Summary: Postges wrapper for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

