# Comparing `tmp/macrometa-source-mongo-0.0.35.tar.gz` & `tmp/macrometa-source-mongo-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.35.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.36.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.35.tar` & `macrometa-source-mongo-0.0.36.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/LICENSE
--rw-r--r--   0        0        0    21337 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6470 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0     1151 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     8097 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     6267 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-05-09 10:12:47.249009 macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-05-09 10:12:47.493013 macrometa-source-mongo-0.0.35/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.35/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/LICENSE
+-rw-r--r--   0        0        0    21341 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6470 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0     1151 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     8097 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     6267 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-05-10 04:22:49.571824 macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-05-10 04:22:49.851829 macrometa-source-mongo-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.36/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.36/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.35/LICENSE` & `macrometa-source-mongo-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.35/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.36/macrometa_source_mongo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,20 +203,20 @@
     def get_config(integration: dict) -> dict:
         try:
             return {
                 # Required config keys
                 'host': integration['host'],
                 'user': integration['user'],
                 'password': integration['password'],
-                'port': integration['port'],
                 'database': integration['database'],
                 'auth_database': integration['auth_database'],
                 'source_collection': integration['source_collection'],
                 # Optional config keys
                 'srv': integration.get('srv', False),
+                'port': integration.get('port'),
                 'replica_set': integration.get('replica_set'),
                 'ssl': integration.get('ssl', False),
                 'verify_mode': integration.get('verify_mode', True),
                 'direct_connection': integration.get('direct_connection', False),
                 'await_time_ms': integration.get('await_time_ms', 900000),
                 'tls_ca_file': integration.get('tls_ca_file'),
                 'tls_certificate_key_file': integration.get('tls_certificate_key_file'),
```

### Comparing `macrometa-source-mongo-0.0.35/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.36/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.35/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.36/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.35/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.36/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.35/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.36/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.35/pyproject.toml` & `macrometa-source-mongo-0.0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.35'
+version='0.0.36'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.35/setup.py` & `macrometa-source-mongo-0.0.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.35',
+    'version': '0.0.36',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.35/PKG-INFO` & `macrometa-source-mongo-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.35
+Version: 0.0.36
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

