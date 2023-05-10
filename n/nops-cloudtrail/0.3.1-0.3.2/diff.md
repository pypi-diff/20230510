# Comparing `tmp/nops-cloudtrail-0.3.1.tar.gz` & `tmp/nops_cloudtrail-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nops-cloudtrail-0.3.1.tar", max compression
+gzip compressed data, was "nops_cloudtrail-0.3.2.tar", max compression
```

## Comparing `nops-cloudtrail-0.3.1.tar` & `nops_cloudtrail-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2022-05-28 17:43:44.460528 nops-cloudtrail-0.3.1/nops_cloudtrail/__init__.py
--rw-r--r--   0        0        0     6237 2022-06-07 16:55:47.458838 nops-cloudtrail-0.3.1/nops_cloudtrail/bucket.py
--rw-r--r--   0        0        0     1698 2022-06-02 09:43:29.081825 nops-cloudtrail-0.3.1/nops_cloudtrail/data_types.py
--rw-r--r--   0        0        0      208 2022-06-06 11:02:49.720911 nops-cloudtrail-0.3.1/nops_cloudtrail/exceptions.py
--rw-r--r--   0        0        0     4082 2022-06-07 16:55:47.459354 nops-cloudtrail-0.3.1/nops_cloudtrail/fetcher.py
--rw-r--r--   0        0        0        0 2022-05-28 14:50:10.705210 nops-cloudtrail-0.3.1/nops_cloudtrail/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-05-28 14:50:24.815232 nops-cloudtrail-0.3.1/nops_cloudtrail/tests/conftest.py
--rw-r--r--   0        0        0     2330 2022-06-06 11:03:07.966476 nops-cloudtrail-0.3.1/nops_cloudtrail/tests/test_fetcher.py
--rw-r--r--   0        0        0      794 2022-06-02 17:12:20.388899 nops-cloudtrail-0.3.1/nops_cloudtrail/tests/test_utils.py
--rw-r--r--   0        0        0     3544 2022-06-07 16:55:47.459809 nops-cloudtrail-0.3.1/nops_cloudtrail/utils.py
--rw-r--r--   0        0        0      680 2022-06-07 16:55:47.460295 nops-cloudtrail-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      715 2022-06-07 16:55:55.808823 nops-cloudtrail-0.3.1/setup.py
--rw-r--r--   0        0        0      858 2022-06-07 16:55:55.808963 nops-cloudtrail-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       39 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/__init__.py
+-rw-r--r--   0        0        0     6237 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/bucket.py
+-rw-r--r--   0        0        0     1698 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/data_types.py
+-rw-r--r--   0        0        0      208 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/exceptions.py
+-rw-r--r--   0        0        0     4082 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/fetcher.py
+-rw-r--r--   0        0        0        0 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/tests/conftest.py
+-rw-r--r--   0        0        0     2330 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/tests/test_fetcher.py
+-rw-r--r--   0        0        0      794 2023-05-10 12:57:11.740499 nops_cloudtrail-0.3.2/nops_cloudtrail/tests/test_utils.py
+-rw-r--r--   0        0        0     3637 2023-05-10 12:57:30.380930 nops_cloudtrail-0.3.2/nops_cloudtrail/utils.py
+-rw-r--r--   0        0        0      680 2023-05-10 12:57:43.873242 nops_cloudtrail-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 nops_cloudtrail-0.3.2/setup.py
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 nops_cloudtrail-0.3.2/PKG-INFO
```

### Comparing `nops-cloudtrail-0.3.1/nops_cloudtrail/bucket.py` & `nops_cloudtrail-0.3.2/nops_cloudtrail/bucket.py`

 * *Files identical despite different names*

### Comparing `nops-cloudtrail-0.3.1/nops_cloudtrail/data_types.py` & `nops_cloudtrail-0.3.2/nops_cloudtrail/data_types.py`

 * *Files identical despite different names*

### Comparing `nops-cloudtrail-0.3.1/nops_cloudtrail/fetcher.py` & `nops_cloudtrail-0.3.2/nops_cloudtrail/fetcher.py`

 * *Files identical despite different names*

### Comparing `nops-cloudtrail-0.3.1/nops_cloudtrail/tests/test_fetcher.py` & `nops_cloudtrail-0.3.2/nops_cloudtrail/tests/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `nops-cloudtrail-0.3.1/nops_cloudtrail/tests/test_utils.py` & `nops_cloudtrail-0.3.2/nops_cloudtrail/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nops-cloudtrail-0.3.1/nops_cloudtrail/utils.py` & `nops_cloudtrail-0.3.2/nops_cloudtrail/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import json
 import decimal
+import json
 import logging
 from datetime import datetime
 from datetime import timedelta
 from typing import Iterator
 
 import dateutil.parser as dparser
 import orjson
@@ -16,19 +16,21 @@
             "ResourceType": resource.get("type", ""),
             "ResourceName": resource["ARN"],
         }
         output.append(output_resource)
 
     return output
 
+
 def json_default(obj):
     if isinstance(obj, decimal.Decimal):
         return str(obj)
     raise TypeError
 
+
 def convert_to_boto3(event):
     """
     Function to provide compatibility between Boto3 CT output from `.lookup_events()` and events
     fetched from the S3 bucket.
     """
     response = {}
 
@@ -57,14 +59,16 @@
         response["Username"] = "root"
     elif "userName" in identity:
         response["Username"] = identity["userName"]
     elif "arn" in identity:
         response["Username"] = identity["arn"]
     elif "roleSessionName" in event.get("requestParameters") or {}:
         response["Username"] = event["requestParameters"]["roleSessionName"]
+    elif "anonymous" == identity["accountId"]:
+        response["Username"] = "anonymous"
     else:
         logging.critical(f"Not handled event username {identity}")
 
     return response
 
 
 def day_chunks(start: datetime, end: datetime) -> Iterator[list[datetime]]:
@@ -97,8 +101,8 @@
             chunk_start = current_date + timedelta(microseconds=1)
             chunk_end = (
                 datetime.combine(chunk_start.date(), datetime.min.time(), tzinfo=current_date.tzinfo)
                 + timedelta(days=1)
                 - timedelta(microseconds=1)
             )
             yield [chunk_start, chunk_end]
-            current_date = chunk_end
+            current_date = chunk_end
```

### Comparing `nops-cloudtrail-0.3.1/pyproject.toml` & `nops_cloudtrail-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nops-cloudtrail"
-version = "0.3.1"
+version = "0.3.2"
 description = "Pull cloudtrail logs from S3 bucket."
 authors = ["nOps Engineers <eng@nops.io>"]
 
 [tool.poetry.dependencies]
 boto3 = ">=1.17.102"
 pyrsistent = ">=0.17.3"
 pydantic = ">=1.8.0"
```

### Comparing `nops-cloudtrail-0.3.1/PKG-INFO` & `nops_cloudtrail-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nops-cloudtrail
-Version: 0.3.1
+Version: 0.3.2
 Summary: Pull cloudtrail logs from S3 bucket.
 Author: nOps Engineers
 Author-email: eng@nops.io
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.17.102)
 Requires-Dist: ijson (>=3.1)
 Requires-Dist: orjson (>=3.6.9)
 Requires-Dist: pydantic (>=1.8.0)
 Requires-Dist: pyrsistent (>=0.17.3)
 Requires-Dist: python-dateutil (>=2.8.2)
```

