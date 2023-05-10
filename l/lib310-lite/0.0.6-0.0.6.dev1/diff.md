# Comparing `tmp/lib310_lite-0.0.6.tar.gz` & `tmp/lib310_lite-0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib310_lite-0.0.6.tar", max compression
+gzip compressed data, was "lib310_lite-0.0.6.dev1.tar", max compression
```

## Comparing `lib310_lite-0.0.6.tar` & `lib310_lite-0.0.6.dev1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.6/lib310_lite/__init__.py
--rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.6/lib310_lite/bigquery/_functions.py
--rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.6/lib310_lite/bigquery/client.py
--rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.6/lib310_lite/bigquery/constants.py
--rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.6/lib310_lite/fucntion.py
--rw-r--r--   0        0        0     9585 2023-05-09 10:33:46.006472 lib310_lite-0.0.6/lib310_lite/mldl/mldl.py
--rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.6/lib310_lite/mldl/models/InteractionModel.py
--rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.6/lib310_lite/mldl/models/SeqLangModel.py
--rw-r--r--   0        0        0      799 2023-05-09 11:06:41.416989 lib310_lite-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 lib310_lite-0.0.6/setup.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 lib310_lite-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-03-08 14:56:22.920616 lib310_lite-0.0.6.dev1/lib310_lite/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-07 16:27:34.184530 lib310_lite-0.0.6.dev1/lib310_lite/bigquery/_functions.py
+-rw-r--r--   0        0        0     7467 2023-05-08 08:51:40.656605 lib310_lite-0.0.6.dev1/lib310_lite/bigquery/client.py
+-rw-r--r--   0        0        0      872 2023-03-07 16:14:03.813101 lib310_lite-0.0.6.dev1/lib310_lite/bigquery/constants.py
+-rw-r--r--   0        0        0       35 2023-03-07 10:52:53.179251 lib310_lite-0.0.6.dev1/lib310_lite/fucntion.py
+-rw-r--r--   0        0        0     9609 2023-05-10 11:30:32.769301 lib310_lite-0.0.6.dev1/lib310_lite/mldl/mldl.py
+-rw-r--r--   0        0        0      843 2023-05-08 09:08:49.952690 lib310_lite-0.0.6.dev1/lib310_lite/mldl/models/InteractionModel.py
+-rw-r--r--   0        0        0     2102 2023-05-08 09:07:24.596219 lib310_lite-0.0.6.dev1/lib310_lite/mldl/models/SeqLangModel.py
+-rw-r--r--   0        0        0      804 2023-05-10 11:42:56.032432 lib310_lite-0.0.6.dev1/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 lib310_lite-0.0.6.dev1/setup.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 lib310_lite-0.0.6.dev1/PKG-INFO
```

### Comparing `lib310_lite-0.0.6/lib310_lite/bigquery/client.py` & `lib310_lite-0.0.6.dev1/lib310_lite/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.6/lib310_lite/bigquery/constants.py` & `lib310_lite-0.0.6.dev1/lib310_lite/bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.6/lib310_lite/mldl/mldl.py` & `lib310_lite-0.0.6.dev1/lib310_lite/mldl/mldl.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ..bigquery.client import Client as BigQueryClient
 from ..bigquery.constants import FileFormat
 import hashlib
 
 # PGSQL
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
+from sqlalchemy.pool import NullPool
 from .models.SeqLangModel import SeqLangModel
 from .models.InteractionModel import InteractionModel
 
 
 class MLDL:
 
     __TRAIN = 'TRAIN'
@@ -25,15 +26,15 @@
     __VAL = 'VAL'
     __MAIN = 'MAIN'
     __INTERACTION = 'INTERACTION'
     __PARTS = {__INTERACTION: 1}
 
     def __init__(self, db_url: str, cache_size: int = 50, num_threads: int = 10, random_seed: int = time.time()):
         random.seed(random_seed)
-        self.engine = create_engine(db_url, pool_size=3 * (num_threads + 1), max_overflow=4 * (num_threads + 1))
+        self.engine = create_engine(db_url, poolclass=NullPool, isolation_level='READ UNCOMMITTED')
         self.Session = sessionmaker(bind=self.engine)
 
         self.bq_client = BigQueryClient()
 
         # this is the pool of samples row_id
         self.sample_cache = []
         # this is the maximum number of requests we fetch sooner from the database
```

### Comparing `lib310_lite-0.0.6/lib310_lite/mldl/models/InteractionModel.py` & `lib310_lite-0.0.6.dev1/lib310_lite/mldl/models/InteractionModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.6/lib310_lite/mldl/models/SeqLangModel.py` & `lib310_lite-0.0.6.dev1/lib310_lite/mldl/models/SeqLangModel.py`

 * *Files identical despite different names*

### Comparing `lib310_lite-0.0.6/pyproject.toml` & `lib310_lite-0.0.6.dev1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib310_lite"
-version = "0.0.6"
+version = "0.0.6.dev1"
 description = "lib310 Lite Python Package"
 authors = ["310 <info@310.ai>"]
 maintainers = ["Saman Fekri <saman@310.ai>"]
 keywords = ["biology", "AI", "genomics", "bioinforma", "machine learning", "GAN"]
 packages = [
     { include = "lib310_lite" }
 ]
```

### Comparing `lib310_lite-0.0.6/setup.py` & `lib310_lite-0.0.6.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'google-cloud-bigquery>=3.2.0',
  'google-cloud>=0.34.0',
  'numpy<1.23.0',
  'psycopg2-binary>=2.9.0']
 
 setup_kwargs = {
     'name': 'lib310-lite',
-    'version': '0.0.6',
+    'version': '0.0.6.dev1',
     'description': 'lib310 Lite Python Package',
     'long_description': 'None',
     'author': '310',
     'author_email': 'info@310.ai',
     'maintainer': 'Saman Fekri',
     'maintainer_email': 'saman@310.ai',
     'url': 'None',
```

### Comparing `lib310_lite-0.0.6/PKG-INFO` & `lib310_lite-0.0.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib310-lite
-Version: 0.0.6
+Version: 0.0.6.dev1
 Summary: lib310 Lite Python Package
 Keywords: biology,AI,genomics,bioinforma,machine learning,GAN
 Author: 310
 Author-email: info@310.ai
 Maintainer: Saman Fekri
 Maintainer-email: saman@310.ai
 Requires-Python: >=3.8
```

