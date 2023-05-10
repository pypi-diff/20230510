# Comparing `tmp/servicex_did_finder_lib-1.3.1.tar.gz` & `tmp/servicex_did_finder_lib-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicex_did_finder_lib-1.3.1.tar", max compression
+gzip compressed data, was "servicex_did_finder_lib-1.4.tar", max compression
```

## Comparing `servicex_did_finder_lib-1.3.1.tar` & `servicex_did_finder_lib-1.4.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11324 2022-11-01 21:21:37.172452 servicex_did_finder_lib-1.3.1/LICENSE
--rw-r--r--   0        0        0      506 2022-11-01 21:21:51.064684 servicex_did_finder_lib-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      113 2022-11-01 21:21:37.172452 servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/__init__.py
--rw-r--r--   0        0        0    10214 2022-11-01 21:21:37.172452 servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/communication.py
--rw-r--r--   0        0        0     1537 2022-11-01 21:21:37.172452 servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/did_logging.py
--rw-r--r--   0        0        0     3558 2022-11-01 21:21:37.172452 servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/did_summary.py
--rw-r--r--   0        0        0     6684 2022-11-01 21:21:37.172452 servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/servicex_adaptor.py
--rw-r--r--   0        0        0     1817 2022-11-01 21:21:37.172452 servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/util_uri.py
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 servicex_did_finder_lib-1.3.1/setup.py
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 servicex_did_finder_lib-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11324 2023-05-10 12:16:48.138715 servicex_did_finder_lib-1.4/LICENSE
+-rw-r--r--   0        0        0      504 2023-05-10 12:17:07.571406 servicex_did_finder_lib-1.4/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-05-10 12:16:48.138715 servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/__init__.py
+-rw-r--r--   0        0        0    10217 2023-05-10 12:16:48.138715 servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/communication.py
+-rw-r--r--   0        0        0     1537 2023-05-10 12:16:48.138715 servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/did_logging.py
+-rw-r--r--   0        0        0     3558 2023-05-10 12:16:48.138715 servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/did_summary.py
+-rw-r--r--   0        0        0     6879 2023-05-10 12:16:48.138715 servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/servicex_adaptor.py
+-rw-r--r--   0        0        0     1817 2023-05-10 12:16:48.138715 servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/util_uri.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 servicex_did_finder_lib-1.4/PKG-INFO
```

### Comparing `servicex_did_finder_lib-1.3.1/LICENSE` & `servicex_did_finder_lib-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/communication.py` & `servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/communication.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,46 +126,46 @@
     Args:
         channel ([type]): RabbitMQ channel
         method ([type]): Delivery method
         properties ([type]): Properties of the message
         body ([type]): The body (json for us) of the message
         file_prefix([str]): Prefix to put in front of file paths to enable use of Cache service
     """
-    request_id = None  # set this in case we get an exception while loading request
+    dataset_id = None  # set this in case we get an exception while loading request
     try:
         # Unpack the message. Really bad if we fail up here!
         did_request = json.loads(body)
         did = did_request["did"]
-        request_id = did_request["request_id"]
+        dataset_id = did_request["dataset_id"]
         __logging.info(
-            f"Received DID request {did_request}", extra={"requestId": request_id}
+            f"Received DID request {did_request}", extra={"dataset_id": dataset_id}
         )
         servicex = ServiceXAdapter(did_request["service-endpoint"], file_prefix)
         servicex.post_status_update("DID Request received")
 
         info = {
-            "request-id": request_id,
+            "dataset-id": dataset_id,
         }
 
         # Process the request and resolve the DID
         try:
             make_sync(run_file_fetch_loop)(did, servicex, info, user_callback)
 
         except Exception as e:
             _, exec_value, _ = sys.exc_info()
-            __logging.exception("DID Request Failed", extra={"requestId": request_id})
+            __logging.exception("DID Request Failed", extra={"dataset_id": dataset_id})
             servicex.post_status_update(
-                f"DID Request Failed for id {request_id}: " f"{str(e)} - {exec_value}",
+                f"DID Request Failed for id {dataset_id}: " f"{str(e)} - {exec_value}",
                 severity="fatal",
             )
             raise
 
     except Exception as e:
         __logging.exception(
-            f"DID request failed {str(e)}", extra={"requestId": request_id}
+            f"DID request failed {str(e)}", extra={"dataset_id": dataset_id}
         )
 
     finally:
         channel.basic_ack(delivery_tag=method.delivery_tag)
 
 
 def init_rabbit_mq(
```

### Comparing `servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/did_logging.py` & `servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/did_logging.py`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/did_summary.py` & `servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/did_summary.py`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/servicex_adaptor.py` & `servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/servicex_adaptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,16 @@
                 self.logger.exception(f'Connection error to ServiceX App. Will retry '
                                       f'(try {attempts} out of {MAX_RETRIES}')
                 attempts += 1
         if not success:
             self.logger.error(f'After {attempts} tries, failed to send ServiceX App a status '
                               f'message: {str(status_msg)} - Ignoring error.')
 
+    # not needed anymore
+    # ????
     def _prefix_file(self, file_path):
         return file_path if not self.file_prefix else self.file_prefix+file_path
 
     def _create_json(self, file_info):
         return {
             "timestamp": datetime.now().isoformat(),
             "paths": [self._prefix_file(fp) for fp in file_info['paths']],
@@ -110,14 +112,17 @@
                     self.logger.exception(f'Connection error to ServiceX App. Will retry '
                                           f'(try {attempts} out of {MAX_RETRIES}')
                     attempts += 1
             if not success:
                 self.logger.error(f'After {attempts} tries, failed to send ServiceX App '
                                   f'a put_file_bulk message: {mesg} - Ignoring error.')
 
+    # should be removed...
+    # transforms can start as soon as request has been made. No need to wait for this.
+    # whole endpoint '/start' is not needed.
     def post_transform_start(self):
         success = False
         attempts = 0
         while not success and attempts < MAX_RETRIES:
             try:
                 requests.post(self.endpoint + "/start")
                 success = True
```

### Comparing `servicex_did_finder_lib-1.3.1/src/servicex_did_finder_lib/util_uri.py` & `servicex_did_finder_lib-1.4/src/servicex_did_finder_lib/util_uri.py`

 * *Files identical despite different names*

### Comparing `servicex_did_finder_lib-1.3.1/PKG-INFO` & `servicex_did_finder_lib-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicex-did-finder-lib
-Version: 1.3.1
+Version: 1.4
 Summary: ServiceX DID Library Routines
 Author: Gordon Watts
 Author-email: gwatts@uw.edu
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

