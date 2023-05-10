# Comparing `tmp/silver-payu-0.6.0.tar.gz` & `tmp/silver-payu-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silver-payu-0.6.0.tar", last modified: Wed May 10 08:39:06 2023, max compression
+gzip compressed data, was "silver-payu-0.6.1.tar", last modified: Wed May 10 09:29:48 2023, max compression
```

## Comparing `silver-payu-0.6.0.tar` & `silver-payu-0.6.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/
--rw-r--r--   0 celo      (1000) celo      (1000)    11357 2022-10-05 07:17:22.000000 silver-payu-0.6.0/LICENSE
--rw-r--r--   0 celo      (1000) celo      (1000)      189 2022-10-05 07:17:22.000000 silver-payu-0.6.0/MANIFEST.in
--rw-r--r--   0 celo      (1000) celo      (1000)      758 2023-05-10 08:39:06.972860 silver-payu-0.6.0/PKG-INFO
--rw-r--r--   0 celo      (1000) celo      (1000)      190 2022-10-05 07:17:22.000000 silver-payu-0.6.0/README.md
--rw-r--r--   0 celo      (1000) celo      (1000)      188 2023-05-09 07:56:34.000000 silver-payu-0.6.0/requirements.test.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       63 2023-05-10 08:37:14.000000 silver-payu-0.6.0/requirements.txt
--rw-r--r--   0 celo      (1000) celo      (1000)      117 2023-05-10 08:39:06.976194 silver-payu-0.6.0/setup.cfg
--rw-r--r--   0 celo      (1000) celo      (1000)     1704 2023-05-09 07:45:10.000000 silver-payu-0.6.0/setup.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/
--rw-r--r--   0 celo      (1000) celo      (1000)      661 2023-05-10 08:37:34.000000 silver-payu-0.6.0/silver_payu/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     6880 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/errors.py
--rw-r--r--   0 celo      (1000) celo      (1000)     3878 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/forms.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/migrations/
--rw-r--r--   0 celo      (1000) celo      (1000)      464 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/migrations/0001_initial.py
--rw-r--r--   0 celo      (1000) celo      (1000)        0 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/migrations/__init__.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/models/
--rw-r--r--   0 celo      (1000) celo      (1000)      628 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/models/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     1616 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/models/payment_methods.py
--rw-r--r--   0 celo      (1000) celo      (1000)    13274 2023-05-10 08:32:28.000000 silver-payu-0.6.0/silver_payu/payment_processors.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.969527 silver-payu-0.6.0/silver_payu/templates/
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.969527 silver-payu-0.6.0/silver_payu/templates/forms/
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/templates/forms/payu_manual/
--rw-r--r--   0 celo      (1000) celo      (1000)       43 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/forms/payu_manual/transaction_form.html
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/templates/forms/payu_triggered/
--rw-r--r--   0 celo      (1000) celo      (1000)       43 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/forms/payu_triggered/transaction_form.html
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/templates/payu/
--rw-r--r--   0 celo      (1000) celo      (1000)     2433 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/payu/3ds_form.html
--rw-r--r--   0 celo      (1000) celo      (1000)      164 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/payu/get_billing_details_form.html
--rw-r--r--   0 celo      (1000) celo      (1000)      364 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/payu/payu_lu_form.html
--rw-r--r--   0 celo      (1000) celo      (1000)      644 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/payu/transaction_form.html
--rw-r--r--   0 celo      (1000) celo      (1000)     1188 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/urls.py
--rw-r--r--   0 celo      (1000) celo      (1000)     2831 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/views.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu.egg-info/
--rw-r--r--   0 celo      (1000) celo      (1000)      758 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/PKG-INFO
--rw-r--r--   0 celo      (1000) celo      (1000)      979 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/SOURCES.txt
--rw-r--r--   0 celo      (1000) celo      (1000)        1 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/dependency_links.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       43 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/requires.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       18 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/top_level.txt
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/tests/
--rw-r--r--   0 celo      (1000) celo      (1000)        0 2022-10-05 07:17:22.000000 silver-payu-0.6.0/tests/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     2159 2023-05-09 07:54:40.000000 silver-payu-0.6.0/tests/conftest.py
--rw-r--r--   0 celo      (1000) celo      (1000)      510 2023-05-09 07:45:10.000000 silver-payu-0.6.0/tests/factories.py
--rw-r--r--   0 celo      (1000) celo      (1000)     2794 2023-05-10 08:26:50.000000 silver-payu-0.6.0/tests/fixtures.py
--rw-r--r--   0 celo      (1000) celo      (1000)     2991 2023-05-09 07:45:10.000000 silver-payu-0.6.0/tests/test_forms.py
--rw-r--r--   0 celo      (1000) celo      (1000)    10780 2023-05-10 08:25:09.000000 silver-payu-0.6.0/tests/test_models.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/
+-rw-r--r--   0 celo      (1000) celo      (1000)    11357 2022-10-05 07:17:22.000000 silver-payu-0.6.1/LICENSE
+-rw-r--r--   0 celo      (1000) celo      (1000)      189 2022-10-05 07:17:22.000000 silver-payu-0.6.1/MANIFEST.in
+-rw-r--r--   0 celo      (1000) celo      (1000)      758 2023-05-10 09:29:48.239147 silver-payu-0.6.1/PKG-INFO
+-rw-r--r--   0 celo      (1000) celo      (1000)      190 2022-10-05 07:17:22.000000 silver-payu-0.6.1/README.md
+-rw-r--r--   0 celo      (1000) celo      (1000)      188 2023-05-09 07:56:34.000000 silver-payu-0.6.1/requirements.test.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       63 2023-05-10 08:37:14.000000 silver-payu-0.6.1/requirements.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)      117 2023-05-10 09:29:48.239147 silver-payu-0.6.1/setup.cfg
+-rw-r--r--   0 celo      (1000) celo      (1000)     1704 2023-05-09 07:45:10.000000 silver-payu-0.6.1/setup.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/silver_payu/
+-rw-r--r--   0 celo      (1000) celo      (1000)      661 2023-05-10 09:28:32.000000 silver-payu-0.6.1/silver_payu/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     6880 2023-05-09 07:45:10.000000 silver-payu-0.6.1/silver_payu/errors.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     3878 2023-05-09 07:45:10.000000 silver-payu-0.6.1/silver_payu/forms.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/silver_payu/migrations/
+-rw-r--r--   0 celo      (1000) celo      (1000)      464 2023-05-09 07:45:10.000000 silver-payu-0.6.1/silver_payu/migrations/0001_initial.py
+-rw-r--r--   0 celo      (1000) celo      (1000)        0 2022-10-05 07:17:22.000000 silver-payu-0.6.1/silver_payu/migrations/__init__.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/silver_payu/models/
+-rw-r--r--   0 celo      (1000) celo      (1000)      628 2022-10-05 07:17:22.000000 silver-payu-0.6.1/silver_payu/models/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     1616 2023-05-09 07:45:10.000000 silver-payu-0.6.1/silver_payu/models/payment_methods.py
+-rw-r--r--   0 celo      (1000) celo      (1000)    13335 2023-05-10 09:28:10.000000 silver-payu-0.6.1/silver_payu/payment_processors.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.235813 silver-payu-0.6.1/silver_payu/templates/
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.235813 silver-payu-0.6.1/silver_payu/templates/forms/
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/silver_payu/templates/forms/payu_manual/
+-rw-r--r--   0 celo      (1000) celo      (1000)       43 2022-10-05 07:17:22.000000 silver-payu-0.6.1/silver_payu/templates/forms/payu_manual/transaction_form.html
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/silver_payu/templates/forms/payu_triggered/
+-rw-r--r--   0 celo      (1000) celo      (1000)       43 2022-10-05 07:17:22.000000 silver-payu-0.6.1/silver_payu/templates/forms/payu_triggered/transaction_form.html
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/silver_payu/templates/payu/
+-rw-r--r--   0 celo      (1000) celo      (1000)     2433 2022-10-05 07:17:22.000000 silver-payu-0.6.1/silver_payu/templates/payu/3ds_form.html
+-rw-r--r--   0 celo      (1000) celo      (1000)      164 2022-10-05 07:17:22.000000 silver-payu-0.6.1/silver_payu/templates/payu/get_billing_details_form.html
+-rw-r--r--   0 celo      (1000) celo      (1000)      364 2022-10-05 07:17:22.000000 silver-payu-0.6.1/silver_payu/templates/payu/payu_lu_form.html
+-rw-r--r--   0 celo      (1000) celo      (1000)      644 2022-10-05 07:17:22.000000 silver-payu-0.6.1/silver_payu/templates/payu/transaction_form.html
+-rw-r--r--   0 celo      (1000) celo      (1000)     1188 2023-05-09 07:45:10.000000 silver-payu-0.6.1/silver_payu/urls.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     2831 2023-05-09 07:45:10.000000 silver-payu-0.6.1/silver_payu/views.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/silver_payu.egg-info/
+-rw-r--r--   0 celo      (1000) celo      (1000)      758 2023-05-10 09:29:48.000000 silver-payu-0.6.1/silver_payu.egg-info/PKG-INFO
+-rw-r--r--   0 celo      (1000) celo      (1000)      979 2023-05-10 09:29:48.000000 silver-payu-0.6.1/silver_payu.egg-info/SOURCES.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)        1 2023-05-10 09:29:48.000000 silver-payu-0.6.1/silver_payu.egg-info/dependency_links.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       43 2023-05-10 09:29:48.000000 silver-payu-0.6.1/silver_payu.egg-info/requires.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       18 2023-05-10 09:29:48.000000 silver-payu-0.6.1/silver_payu.egg-info/top_level.txt
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 09:29:48.239147 silver-payu-0.6.1/tests/
+-rw-r--r--   0 celo      (1000) celo      (1000)        0 2022-10-05 07:17:22.000000 silver-payu-0.6.1/tests/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     2159 2023-05-09 07:54:40.000000 silver-payu-0.6.1/tests/conftest.py
+-rw-r--r--   0 celo      (1000) celo      (1000)      510 2023-05-09 07:45:10.000000 silver-payu-0.6.1/tests/factories.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     2794 2023-05-10 08:26:50.000000 silver-payu-0.6.1/tests/fixtures.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     2991 2023-05-09 07:45:10.000000 silver-payu-0.6.1/tests/test_forms.py
+-rw-r--r--   0 celo      (1000) celo      (1000)    12571 2023-05-10 09:28:13.000000 silver-payu-0.6.1/tests/test_models.py
```

### Comparing `silver-payu-0.6.0/LICENSE` & `silver-payu-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/PKG-INFO` & `silver-payu-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silver-payu
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/silverapp/silver-payu
 Author: Presslabs
 Author-email: ping@presslabs.com
 License: Apache 2.0
 Keywords: django,app,reusable,billing,invoicing,api
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `silver-payu-0.6.0/setup.py` & `silver-payu-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu/__init__.py` & `silver-payu-0.6.1/silver_payu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 
 __author__ = "Presslabs"
-__version__ = "0.6.0"
+__version__ = "0.6.1"
```

### Comparing `silver-payu-0.6.0/silver_payu/errors.py` & `silver-payu-0.6.1/silver_payu/errors.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu/forms.py` & `silver-payu-0.6.1/silver_payu/forms.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu/models/__init__.py` & `silver-payu-0.6.1/silver_payu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu/models/payment_methods.py` & `silver-payu-0.6.1/silver_payu/models/payment_methods.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu/payment_processors.py` & `silver-payu-0.6.1/silver_payu/payment_processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,32 +296,33 @@
                 "BILL_EMAIL",
             ]
 
         for field in redacted_fields:
             if request.get(field):
                 request[field] = "[REDACTED]"
 
-        response = getattr(payment, "_response", "")
-        if isinstance(response, bytes):
-            response = response.decode("utf-8")
-
-        transaction.data.update(
-            {
-                "_request": str(request),
-                "_response": str(response),
-            }
-        )
+        transaction.data["_request"] = str(request)
+
+        if transaction.state == Transaction.States.Failed:
+            response = getattr(payment, "_response", "")
+            if isinstance(response, bytes):
+                response = response.decode("utf-8")
+
+            transaction.data["_response"] = str(response)
 
     def _parse_result(self, transaction, result, payment=None):
         try:
             element = ElementTree.fromstring(result)
             status = element.find("STATUS").text
             return_code = element.find("RETURN_CODE").text
 
             if status == "SUCCESS":
+                self._log_request_response(transaction, payment)
+                transaction.save()
+
                 return True
 
             error_code, error_reason = self._parse_response_error(return_code)
             transaction.data.update(
                 {
                     "status": status,
                     "message": error_reason,
@@ -329,20 +330,19 @@
                 }
             )
 
             return_message = element.find("RETURN_MESSAGE")
             if return_message is not None:
                 transaction.data["return_message"] = return_message.text
 
-            self._log_request_response(transaction, payment)
             transaction.fail(fail_code=error_code, fail_reason=error_reason)
         except ValueError as error:
-            self._log_request_response(transaction, payment)
             transaction.fail(fail_reason=str(error))
 
+        self._log_request_response(transaction, payment)
         transaction.save()
 
         return False
 
     def _parse_response_error(self, return_code):
         if str(return_code) in ALU_ERROR_CODES:
             error = ALU_ERROR_CODES[str(return_code)]
```

### Comparing `silver-payu-0.6.0/silver_payu/templates/payu/3ds_form.html` & `silver-payu-0.6.1/silver_payu/templates/payu/3ds_form.html`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu/templates/payu/transaction_form.html` & `silver-payu-0.6.1/silver_payu/templates/payu/transaction_form.html`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu/urls.py` & `silver-payu-0.6.1/silver_payu/urls.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu/views.py` & `silver-payu-0.6.1/silver_payu/views.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/silver_payu.egg-info/PKG-INFO` & `silver-payu-0.6.1/silver_payu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silver-payu
-Version: 0.6.0
+Version: 0.6.1
 Home-page: https://github.com/silverapp/silver-payu
 Author: Presslabs
 Author-email: ping@presslabs.com
 License: Apache 2.0
 Keywords: django,app,reusable,billing,invoicing,api
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `silver-payu-0.6.0/silver_payu.egg-info/SOURCES.txt` & `silver-payu-0.6.1/silver_payu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/tests/conftest.py` & `silver-payu-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/tests/fixtures.py` & `silver-payu-0.6.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/tests/test_forms.py` & `silver-payu-0.6.1/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.6.0/tests/test_models.py` & `silver-payu-0.6.1/tests/test_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,21 +42,75 @@
     transaction_triggered = MagicMock(
         payment_processor=payment_processor_triggered, state=Transaction.States.Settled
     )
     assert not payment_processor_triggered.execute_transaction(transaction_triggered)
 
 
 @pytest.mark.django_db
-def test_execute_transaction_happy_path(payment_processor_triggered):
-    payment_processor_triggered._charge_transaction = lambda x: True
+def test_execute_transaction_happy_path(
+    payment_method_triggered_v2,
+    payment_processor_triggered_v2,
+    transaction_triggered_v2,
+):
+    response = """<?xml version="1.0"?>
+    <EPAYMENT>
+        <REFNO>123456789</REFNO>
+        <ALIAS>9592b7736c9e277fea8cc79c2e5b5a23</ALIAS>
+        <STATUS>SUCCESS</STATUS>
+        <RETURN_CODE>AUTHORIZED</RETURN_CODE>
+        <RETURN_MESSAGE>Successfull authorized</RETURN_MESSAGE>
+        <DATE>2012-11-06 20:52:20</DATE>
+        <ORDER_REF>7305</ORDER_REF>
+        <AUTH_CODE>13157TUlA15117</AUTH_CODE>
+        <HASH>b560a38e2b3e7bcbac328bbd6218bc60</HASH>
+    </EPAYMENT>
+    """
 
-    transaction_triggered = MagicMock(
-        payment_processor=payment_processor_triggered, state=Transaction.States.Pending
+    responses.add(
+        responses.POST,
+        settings.PAYU_ALU_URL,
+        body=response,
+        status=200,
+    )
+
+    payment_method_triggered_v2.archived_customer = {
+        "BILL_ADDRESS": faker.address(),
+        "BILL_CITY": faker.city(),
+        "BILL_EMAIL": faker.email(),
+        "BILL_FNAME": faker.first_name(),
+        "BILL_LNAME": faker.last_name(),
+        "BILL_PHONE": faker.phone_number(),
+    }
+    payment_method_triggered_v2.threeds_data = {
+        "BROWSER_IP": "111.1.11.111",
+        "BROWSER_ACCEPT_HEADER": "*/*",
+        "BROWSER_JAVA_ENABLED": "NO",
+        "BROWSER_LANGUAGE": "en-US",
+        "BROWSER_COLOR_DEPTH": "32",
+        "BROWSER_SCREEN_HEIGHT": "1024",
+        "BROWSER_SCREEN_WIDTH": "768",
+        "BROWSER_TIMEZONE": "180",
+        "BROWSER_USER_AGENT": "Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:47.0) Gecko/20100101 Firefox/47.0",
+    }
+    payment_method_triggered_v2.save()
+
+    assert payment_processor_triggered_v2.process_transaction(transaction_triggered_v2)
+
+    transaction_triggered_v2.refresh_from_db()
+    assert transaction_triggered_v2.state == Transaction.States.Pending
+
+    assert (
+        "'STRONG_CUSTOMER_AUTHENTICATION': 'YES'"
+        in transaction_triggered_v2.data["_request"]
+    )
+    assert "'BROWSER_IP': '111.1.11.111'" in transaction_triggered_v2.data["_request"]
+    assert (
+        f"'BILL_FNAME': '{payment_method_triggered_v2.archived_customer['BILL_FNAME']}'"
+        in transaction_triggered_v2.data["_request"]
     )
-    assert payment_processor_triggered.execute_transaction(transaction_triggered)
 
 
 @pytest.mark.django_db
 def test_execute_transaction_authorization_failed(
     payment_method_triggered_v2,
     payment_processor_triggered_v2,
     transaction_triggered_v2,
```

