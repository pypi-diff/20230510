# Comparing `tmp/latch_o11y-0.1.3.tar.gz` & `tmp/latch_o11y-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_o11y-0.1.3.tar", max compression
+gzip compressed data, was "latch_o11y-0.1.4.tar", max compression
```

## Comparing `latch_o11y-0.1.3.tar` & `latch_o11y-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     7052 2023-04-27 17:53:53.729206 latch_o11y-0.1.3/LICENSE
--rw-r--r--   0        0        0       14 2023-04-27 17:54:11.934983 latch_o11y-0.1.3/README.md
--rw-r--r--   0        0        0     7048 2023-05-09 21:34:27.276447 latch_o11y-0.1.3/latch_o11y/o11y.py
--rw-r--r--   0        0        0        0 2023-05-09 17:04:17.188957 latch_o11y-0.1.3/latch_o11y/py.typed
--rw-r--r--   0        0        0     1257 2023-05-09 21:34:50.312612 latch_o11y-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 latch_o11y-0.1.3/setup.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 latch_o11y-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 17:53:53.729206 latch_o11y-0.1.4/LICENSE
+-rw-r--r--   0        0        0       14 2023-04-27 17:54:11.934983 latch_o11y-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 16:18:11.991042 latch_o11y-0.1.4/latch_o11y/__init__.py
+-rw-r--r--   0        0        0     7048 2023-05-09 21:34:27.276447 latch_o11y-0.1.4/latch_o11y/o11y.py
+-rw-r--r--   0        0        0        0 2023-05-09 17:04:17.188957 latch_o11y-0.1.4/latch_o11y/py.typed
+-rw-r--r--   0        0        0     1257 2023-05-10 16:19:01.224331 latch_o11y-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 latch_o11y-0.1.4/setup.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 latch_o11y-0.1.4/PKG-INFO
```

### Comparing `latch_o11y-0.1.3/LICENSE` & `latch_o11y-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_o11y-0.1.3/latch_o11y/o11y.py` & `latch_o11y-0.1.4/latch_o11y/o11y.py`

 * *Files identical despite different names*

### Comparing `latch_o11y-0.1.3/pyproject.toml` & `latch_o11y-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "latch-o11y"
-version = "0.1.3"
+version = "0.1.4"
 description = "Observability for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_o11y"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-latch-config = "^0.1.4"
+latch-config = "^0.1.5"
 opentelemetry-api = "^1.15.0"
 opentelemetry-sdk = "^1.15.0"
 opentelemetry-exporter-otlp-proto-grpc = "^1.15.0"
 orjson = "^3.8.5"
 structlog = "^22.3.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `latch_o11y-0.1.3/setup.py` & `latch_o11y-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 packages = \
 ['latch_o11y']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['latch-config>=0.1.4,<0.2.0',
+['latch-config>=0.1.5,<0.2.0',
  'opentelemetry-api>=1.15.0,<2.0.0',
  'opentelemetry-exporter-otlp-proto-grpc>=1.15.0,<2.0.0',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'orjson>=3.8.5,<4.0.0',
  'structlog>=22.3.0,<23.0.0']
 
 setup_kwargs = {
     'name': 'latch-o11y',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Observability for latch python backend services',
     'long_description': '# python-o11y\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_o11y-0.1.3/PKG-INFO` & `latch_o11y-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: latch-o11y
-Version: 0.1.3
+Version: 0.1.4
 Summary: Observability for latch python backend services
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: latch-config (>=0.1.4,<0.2.0)
+Requires-Dist: latch-config (>=0.1.5,<0.2.0)
 Requires-Dist: opentelemetry-api (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (>=1.15.0,<2.0.0)
 Requires-Dist: opentelemetry-sdk (>=1.15.0,<2.0.0)
 Requires-Dist: orjson (>=3.8.5,<4.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Description-Content-Type: text/markdown
```

