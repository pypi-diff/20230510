# Comparing `tmp/dogfood_logger-0.1.7.tar.gz` & `tmp/dogfood_logger-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogfood_logger-0.1.7.tar", max compression
+gzip compressed data, was "dogfood_logger-0.1.8.tar", max compression
```

## Comparing `dogfood_logger-0.1.7.tar` & `dogfood_logger-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1087 2023-05-10 02:17:04.332370 dogfood_logger-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0      464 2023-05-10 02:17:04.332370 dogfood_logger-0.1.7/README.md
--rw-r--r--   0        0        0       21 2023-05-10 03:18:57.202008 dogfood_logger-0.1.7/dogfood_logger/__init__.py
--rw-r--r--   0        0        0     3074 2023-05-10 03:18:57.202008 dogfood_logger-0.1.7/dogfood_logger/logger.py
--rw-r--r--   0        0        0       42 2023-05-10 02:17:04.332370 dogfood_logger-0.1.7/dogfood_logger/packageData/sampleData.dat
--rw-r--r--   0        0        0     1309 2023-05-10 04:35:51.523838 dogfood_logger-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 dogfood_logger-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-10 02:17:04.332370 dogfood_logger-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0      464 2023-05-10 02:17:04.332370 dogfood_logger-0.1.8/README.md
+-rw-r--r--   0        0        0       21 2023-05-10 03:18:57.202008 dogfood_logger-0.1.8/dogfood_logger/__init__.py
+-rw-r--r--   0        0        0     2706 2023-05-10 04:36:54.116406 dogfood_logger-0.1.8/dogfood_logger/logger.py
+-rw-r--r--   0        0        0       42 2023-05-10 02:17:04.332370 dogfood_logger-0.1.8/dogfood_logger/packageData/sampleData.dat
+-rw-r--r--   0        0        0     1309 2023-05-10 04:37:00.608465 dogfood_logger-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 dogfood_logger-0.1.8/PKG-INFO
```

### Comparing `dogfood_logger-0.1.7/LICENSE.txt` & `dogfood_logger-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dogfood_logger-0.1.7/dogfood_logger/logger.py` & `dogfood_logger-0.1.8/dogfood_logger/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,28 +8,18 @@
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 from opentelemetry.sdk.trace.export import (
     BatchSpanProcessor,
     ConsoleSpanExporter,
 )
 from opentelemetry.exporter.jaeger.thrift import \
     JaegerExporter as ThriftJaegerExporter
-from constants import MANDATORY_ENV_VARS
-import os
-
-load_dotenv()  # take environment variables from .env.
-
 
 class LokiLogger:
 
     def __init__(self, app, app_name, url, log_format, env, agent_host, agent_port) -> None:
-        for var in MANDATORY_ENV_VARS:
-            if var not in os.environ or not os.environ[var]:
-                logging.error("Failed because {} is not set.".format(var))
-                raise EnvironmentError("Failed because {} is not set.".format(var))
-
         self.handler = logging_loki.LokiHandler(
             url=url,
             tags={"application": app_name},
             version="1",
         )
         self.handler.setFormatter(logging.Formatter(log_format))
         self.logger = logging.getLogger(app_name)
```

### Comparing `dogfood_logger-0.1.7/pyproject.toml` & `dogfood_logger-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dogfood-logger"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "dogfood_logger"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dogfood_logger-0.1.7/PKG-INFO` & `dogfood_logger-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogfood-logger
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

