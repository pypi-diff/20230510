# Comparing `tmp/django-payu-ro-1.4.2.tar.gz` & `tmp/django-payu-ro-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-payu-ro-1.4.2.tar", last modified: Wed Jan  5 09:41:07 2022, max compression
+gzip compressed data, was "django-payu-ro-1.5.0.tar", last modified: Wed May 10 07:47:08 2023, max compression
```

## Comparing `django-payu-ro-1.4.2.tar` & `django-payu-ro-1.5.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/
--rw-r--r--   0 celo      (1000) celo      (1000)     1241 2022-01-05 09:28:47.000000 django-payu-ro-1.4.2/CHANGELOG.txt
--rw-r--r--   0 celo      (1000) celo      (1000)    10143 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/LICENSE
--rw-r--r--   0 celo      (1000) celo      (1000)      116 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/MANIFEST.in
--rw-r--r--   0 celo      (1000) celo      (1000)      531 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/PKG-INFO
--rw-r--r--   0 celo      (1000) celo      (1000)      922 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/README.md
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/django_payu_ro.egg-info/
--rw-r--r--   0 celo      (1000) celo      (1000)      531 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/django_payu_ro.egg-info/PKG-INFO
--rw-r--r--   0 celo      (1000) celo      (1000)      871 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/django_payu_ro.egg-info/SOURCES.txt
--rw-r--r--   0 celo      (1000) celo      (1000)        1 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/django_payu_ro.egg-info/dependency_links.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       47 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/django_payu_ro.egg-info/requires.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       11 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/django_payu_ro.egg-info/top_level.txt
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/payu/
--rw-r--r--   0 celo      (1000) celo      (1000)      661 2022-01-05 09:28:47.000000 django-payu-ro-1.4.2/payu/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     1286 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/payu/admin.py
--rw-r--r--   0 celo      (1000) celo      (1000)     3970 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/payu/conf.py
--rw-r--r--   0 celo      (1000) celo      (1000)    10141 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/payu/forms.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/payu/management/
--rw-r--r--   0 celo      (1000) celo      (1000)      581 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/payu/management/__init__.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/payu/management/commands/
--rw-r--r--   0 celo      (1000) celo      (1000)      612 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/payu/management/commands/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     1591 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/payu/management/commands/send_idns.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/payu/migrations/
--rw-r--r--   0 celo      (1000) celo      (1000)    18324 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/payu/migrations/0001_initial.py
--rw-r--r--   0 celo      (1000) celo      (1000)      494 2021-04-14 08:06:13.000000 django-payu-ro-1.4.2/payu/migrations/0002_payutoken_token_hash.py
--rw-r--r--   0 celo      (1000) celo      (1000)      856 2021-04-14 08:06:13.000000 django-payu-ro-1.4.2/payu/migrations/0003_auto_20200820_0858.py
--rw-r--r--   0 celo      (1000) celo      (1000)    23599 2021-06-28 12:08:34.000000 django-payu-ro-1.4.2/payu/migrations/0004_auto_20210628_1208.py
--rw-r--r--   0 celo      (1000) celo      (1000)      614 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/payu/migrations/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)    22613 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/payu/models.py
--rw-r--r--   0 celo      (1000) celo      (1000)     5687 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/payu/payments.py
--rw-r--r--   0 celo      (1000) celo      (1000)      916 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/payu/signals.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/payu/templates/
--rw-r--r--   0 celo      (1000) celo      (1000)      175 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/payu/templates/custom_hidden.html
--rw-r--r--   0 celo      (1000) celo      (1000)      740 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/payu/urls.py
--rw-r--r--   0 celo      (1000) celo      (1000)     3810 2022-01-05 09:28:28.000000 django-payu-ro-1.4.2/payu/views.py
--rw-r--r--   0 celo      (1000) celo      (1000)       47 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/requirements.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       38 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/setup.cfg
--rw-r--r--   0 celo      (1000) celo      (1000)     2413 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/setup.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:41:07.000000 django-payu-ro-1.4.2/tests/
--rw-r--r--   0 celo      (1000) celo      (1000)      581 2018-06-12 13:22:04.000000 django-payu-ro-1.4.2/tests/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     1134 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/tests/conftest.py
--rw-r--r--   0 celo      (1000) celo      (1000)    10376 2018-08-14 10:36:23.000000 django-payu-ro-1.4.2/tests/test_forms.py
--rw-r--r--   0 celo      (1000) celo      (1000)     4517 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/tests/test_models.py
--rw-r--r--   0 celo      (1000) celo      (1000)     4659 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/tests/test_payments.py
--rw-r--r--   0 celo      (1000) celo      (1000)     1547 2021-06-28 10:57:49.000000 django-payu-ro-1.4.2/tests/test_send_idns_command.py
--rw-r--r--   0 celo      (1000) celo      (1000)     1777 2022-01-05 09:28:33.000000 django-payu-ro-1.4.2/tests/test_views.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 07:47:08.661826 django-payu-ro-1.5.0/
+-rw-r--r--   0 celo      (1000) celo      (1000)     1347 2023-05-09 13:00:39.000000 django-payu-ro-1.5.0/CHANGELOG.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)    10143 2022-10-05 07:17:01.000000 django-payu-ro-1.5.0/LICENSE
+-rw-r--r--   0 celo      (1000) celo      (1000)      116 2022-10-05 07:17:01.000000 django-payu-ro-1.5.0/MANIFEST.in
+-rw-r--r--   0 celo      (1000) celo      (1000)      497 2023-05-10 07:47:08.658492 django-payu-ro-1.5.0/PKG-INFO
+-rw-r--r--   0 celo      (1000) celo      (1000)      922 2022-10-05 07:17:01.000000 django-payu-ro-1.5.0/README.md
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 07:47:08.651826 django-payu-ro-1.5.0/django_payu_ro.egg-info/
+-rw-r--r--   0 celo      (1000) celo      (1000)      497 2023-05-10 07:47:08.000000 django-payu-ro-1.5.0/django_payu_ro.egg-info/PKG-INFO
+-rw-r--r--   0 celo      (1000) celo      (1000)      896 2023-05-10 07:47:08.000000 django-payu-ro-1.5.0/django_payu_ro.egg-info/SOURCES.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)        1 2023-05-10 07:47:08.000000 django-payu-ro-1.5.0/django_payu_ro.egg-info/dependency_links.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       47 2023-05-10 07:47:08.000000 django-payu-ro-1.5.0/django_payu_ro.egg-info/requires.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       11 2023-05-10 07:47:08.000000 django-payu-ro-1.5.0/django_payu_ro.egg-info/top_level.txt
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 07:47:08.655159 django-payu-ro-1.5.0/payu/
+-rw-r--r--   0 celo      (1000) celo      (1000)      661 2023-05-09 13:00:44.000000 django-payu-ro-1.5.0/payu/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     1348 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/payu/admin.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     3791 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/payu/conf.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     9834 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/payu/forms.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 07:47:08.655159 django-payu-ro-1.5.0/payu/management/
+-rw-r--r--   0 celo      (1000) celo      (1000)      580 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/payu/management/__init__.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 07:47:08.655159 django-payu-ro-1.5.0/payu/management/commands/
+-rw-r--r--   0 celo      (1000) celo      (1000)      612 2022-10-05 07:17:01.000000 django-payu-ro-1.5.0/payu/management/commands/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     1657 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/payu/management/commands/send_idns.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 07:47:08.658492 django-payu-ro-1.5.0/payu/migrations/
+-rw-r--r--   0 celo      (1000) celo      (1000)    30950 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/payu/migrations/0001_initial.py
+-rw-r--r--   0 celo      (1000) celo      (1000)      523 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/payu/migrations/0002_payutoken_token_hash.py
+-rw-r--r--   0 celo      (1000) celo      (1000)      915 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/payu/migrations/0003_auto_20200820_0858.py
+-rw-r--r--   0 celo      (1000) celo      (1000)    28528 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/payu/migrations/0004_auto_20210628_1208.py
+-rw-r--r--   0 celo      (1000) celo      (1000)      613 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/payu/migrations/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)    22661 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/payu/models.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     5781 2023-05-09 12:59:04.000000 django-payu-ro-1.5.0/payu/payments.py
+-rw-r--r--   0 celo      (1000) celo      (1000)      916 2022-10-05 07:17:01.000000 django-payu-ro-1.5.0/payu/signals.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 07:47:08.658492 django-payu-ro-1.5.0/payu/templates/
+-rw-r--r--   0 celo      (1000) celo      (1000)      175 2022-10-05 07:17:01.000000 django-payu-ro-1.5.0/payu/templates/custom_hidden.html
+-rw-r--r--   0 celo      (1000) celo      (1000)      740 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/payu/urls.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     3806 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/payu/views.py
+-rw-r--r--   0 celo      (1000) celo      (1000)       47 2022-10-05 07:17:01.000000 django-payu-ro-1.5.0/requirements.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       38 2023-05-10 07:47:08.661826 django-payu-ro-1.5.0/setup.cfg
+-rw-r--r--   0 celo      (1000) celo      (1000)     2388 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/setup.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 07:47:08.658492 django-payu-ro-1.5.0/tests/
+-rw-r--r--   0 celo      (1000) celo      (1000)      580 2023-05-08 11:34:13.000000 django-payu-ro-1.5.0/tests/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     1253 2023-05-08 11:46:49.000000 django-payu-ro-1.5.0/tests/conftest.py
+-rw-r--r--   0 celo      (1000) celo      (1000)      108 2023-05-08 11:39:31.000000 django-payu-ro-1.5.0/tests/pytest_fixtures.py
+-rw-r--r--   0 celo      (1000) celo      (1000)    12625 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/tests/test_forms.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     4981 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/tests/test_models.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     6140 2023-05-09 12:59:09.000000 django-payu-ro-1.5.0/tests/test_payments.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     1547 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/tests/test_send_idns_command.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     1790 2023-05-08 11:34:14.000000 django-payu-ro-1.5.0/tests/test_views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-payu-ro-1.4.2/CHANGELOG.txt` & `django-payu-ro-1.5.0/CHANGELOG.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+=== 1.5.0 ===
+- Send 3DS data when available (regardless whether the payment results in a token or not).
+
 === 1.4.2 ===
 - Fix IPN confirmation response.
 - Added back GET method to IPN view as a no-op, since it is used for checking the endpoint by PayU.
 
 === 1.4.1 ===
 - Added missing migrations.
```

### Comparing `django-payu-ro-1.4.2/LICENSE` & `django-payu-ro-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-payu-ro-1.4.2/README.md` & `django-payu-ro-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django-payu-ro-1.4.2/django_payu_ro.egg-info/SOURCES.txt` & `django-payu-ro-1.5.0/django_payu_ro.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -25,12 +25,13 @@
 payu/migrations/0002_payutoken_token_hash.py
 payu/migrations/0003_auto_20200820_0858.py
 payu/migrations/0004_auto_20210628_1208.py
 payu/migrations/__init__.py
 payu/templates/custom_hidden.html
 tests/__init__.py
 tests/conftest.py
+tests/pytest_fixtures.py
 tests/test_forms.py
 tests/test_models.py
 tests/test_payments.py
 tests/test_send_idns_command.py
 tests/test_views.py
```

### Comparing `django-payu-ro-1.4.2/payu/__init__.py` & `django-payu-ro-1.5.0/payu/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 
-__author__ = 'Presslabs'
-__version__ = '1.4.2'
+__author__ = "Presslabs"
+__version__ = "1.5.0"
```

### Comparing `django-payu-ro-1.4.2/payu/admin.py` & `django-payu-ro-1.5.0/payu/admin.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,24 +15,35 @@
 #    limitations under the License.
 from django.contrib import admin
 
 from payu.models import PayUIPN, PayUToken, PayUIDN
 
 
 class PayUIPNAdmin(admin.ModelAdmin):
-    list_display = ('__unicode__', 'REFNOEXT', 'ORDERSTATUS', 'flag',
-                    'flag_info', 'created_at')
-    list_filter = ('ORDERSTATUS', 'flag')
+    list_display = (
+        "__unicode__",
+        "REFNOEXT",
+        "ORDERSTATUS",
+        "flag",
+        "flag_info",
+        "created_at",
+    )
+    list_filter = ("ORDERSTATUS", "flag")
 
 
 class PayUTokenAdmin(admin.ModelAdmin):
-    list_display = ('__unicode__', 'ipn', 'IPN_CC_TOKEN', 'IPN_CC_MASK',
-                    'IPN_CC_EXP_DATE')
+    list_display = (
+        "__unicode__",
+        "ipn",
+        "IPN_CC_TOKEN",
+        "IPN_CC_MASK",
+        "IPN_CC_EXP_DATE",
+    )
 
 
 class PayUIDNAdmin(admin.ModelAdmin):
-    list_display = ('ipn', 'sent', 'success')
+    list_display = ("ipn", "sent", "success")
 
 
 admin.site.register(PayUIPN, PayUIPNAdmin)
 admin.site.register(PayUToken, PayUTokenAdmin)
 admin.site.register(PayUIDN, PayUIDNAdmin)
```

### Comparing `django-payu-ro-1.4.2/payu/forms.py` & `django-payu-ro-1.5.0/payu/forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,38 +18,45 @@
 import re
 import hmac
 from datetime import datetime
 
 from django import forms
 
 from payu.models import PayUIPN
-from payu.conf import (PAYU_MERCHANT, PAYU_MERCHANT_KEY, PAYU_TEST_TRANSACTION,
-                       PAYU_ORDER_DETAILS, PAYU_ORDER_DETAILS_DEFAULTS,
-                       PAYU_DATE_FORMATS, PAYU_CURRENCIES,
-                       PAYU_PAYMENT_METHODS, PAYU_LANGUAGES,
-                       PAYU_LU_CALLBACK)
+from payu.conf import (
+    PAYU_MERCHANT,
+    PAYU_MERCHANT_KEY,
+    PAYU_TEST_TRANSACTION,
+    PAYU_ORDER_DETAILS,
+    PAYU_ORDER_DETAILS_DEFAULTS,
+    PAYU_DATE_FORMATS,
+    PAYU_CURRENCIES,
+    PAYU_PAYMENT_METHODS,
+    PAYU_LANGUAGES,
+    PAYU_LU_CALLBACK,
+)
 
 
 class ValueHiddenInput(forms.HiddenInput):
     """
     Widget that renders only if it has a value.
     Used to remove unused fields from PayU buttons.
     """
 
-    template_name = 'custom_hidden.html'
+    template_name = "custom_hidden.html"
 
     def _get_name(self, name):
-        detail = re.match(r'^ORDER_(\d+)_(\d+)$', name)
+        detail = re.match(r"^ORDER_(\d+)_(\d+)$", name)
         if detail and int(detail.group(2)) < len(PAYU_ORDER_DETAILS):
-            name = 'ORDER_%s[]' % PAYU_ORDER_DETAILS[int(detail.group(2))]
+            name = "ORDER_%s[]" % PAYU_ORDER_DETAILS[int(detail.group(2))]
         return name
 
     def get_context(self, name, value, attrs):
         context = super(ValueHiddenInput, self).get_context(name, value, attrs)
-        context['widget']['name'] = self._get_name(context['widget']['name'])
+        context["widget"]["name"] = self._get_name(context["widget"]["name"])
         return context
 
     def render(self, name, value, *args, **kwargs):
         if value is None:
             return ""
 
         name = self._get_name(name)
@@ -60,15 +67,15 @@
 class OrderWidget(forms.MultiWidget):
     def __init__(self, attrs=None, *args, **kwargs):
         attrs = attrs or {}
         all_widgets = [ValueHiddenInput(attrs) for _ in PAYU_ORDER_DETAILS]
         super(OrderWidget, self).__init__(all_widgets, *args, **kwargs)
 
     def decompress(self, value):
-        return [value.get(detail, '') for detail in PAYU_ORDER_DETAILS]
+        return [value.get(detail, "") for detail in PAYU_ORDER_DETAILS]
 
 
 class OrderField(forms.MultiValueField):
     widget = OrderWidget
 
     def __init__(self, *args, **kwargs):
         all_fields = tuple(forms.CharField() for _ in PAYU_ORDER_DETAILS)
@@ -81,69 +88,71 @@
     def __init__(self, count, *args, **kwargs):
         all_widgets = tuple((OrderWidget()) for _ in range(count))
         super(OrdersWidget, self).__init__(all_widgets, *args, **kwargs)
 
 
 class OrdersField(forms.MultiValueField):
     def __init__(self, *args, **kwargs):
-        products = kwargs.get('initial', [])
-        kwargs['label'] = ''
+        products = kwargs.get("initial", [])
+        kwargs["label"] = ""
 
         all_fields = tuple()
         if products:
             self.widget = OrdersWidget(len(products))
             all_fields = tuple((OrderField()) for _ in products)
         super(OrdersField, self).__init__(all_fields, *args, **kwargs)
 
 
 class PayULiveUpdateForm(forms.Form):
-    MERCHANT = forms.CharField(widget=ValueHiddenInput,
-                               initial=PAYU_MERCHANT)
-    LU_ENABLE_TOKEN = forms.CharField(widget=ValueHiddenInput, initial='')
-    LU_TOKEN_TYPE = forms.CharField(widget=ValueHiddenInput, initial='')
-    ORDER_REF = forms.CharField(widget=ValueHiddenInput, initial='')
-    ORDER_DATE = forms.CharField(widget=ValueHiddenInput,
-                                 initial=datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
+    MERCHANT = forms.CharField(widget=ValueHiddenInput, initial=PAYU_MERCHANT)
+    LU_ENABLE_TOKEN = forms.CharField(widget=ValueHiddenInput, initial="")
+    LU_TOKEN_TYPE = forms.CharField(widget=ValueHiddenInput, initial="")
+    ORDER_REF = forms.CharField(widget=ValueHiddenInput, initial="")
+    ORDER_DATE = forms.CharField(
+        widget=ValueHiddenInput, initial=datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    )
 
     ORDER = OrdersField()
     ORDER_SHIPPING = forms.CharField(widget=ValueHiddenInput)
-    PRICES_CURRENCY = forms.ChoiceField(widget=ValueHiddenInput,
-                                        choices=PAYU_CURRENCIES, initial='USD')
+    PRICES_CURRENCY = forms.ChoiceField(
+        widget=ValueHiddenInput, choices=PAYU_CURRENCIES, initial="USD"
+    )
     DISCOUNT = forms.CharField(widget=ValueHiddenInput)
 
     DESTINATION_CITY = forms.CharField(widget=ValueHiddenInput)
     DESTINATION_STATE = forms.CharField(widget=ValueHiddenInput)
     DESTINATION_COUNTRY = forms.CharField(widget=ValueHiddenInput)
 
-    PAY_METHOD = forms.ChoiceField(widget=ValueHiddenInput,
-                                   choices=PAYU_PAYMENT_METHODS)
+    PAY_METHOD = forms.ChoiceField(
+        widget=ValueHiddenInput, choices=PAYU_PAYMENT_METHODS
+    )
 
-    ORDER_HASH = forms.CharField(widget=ValueHiddenInput,
-                                 initial='')
+    ORDER_HASH = forms.CharField(widget=ValueHiddenInput, initial="")
 
     BILL_FNAME = forms.CharField(widget=ValueHiddenInput)
     BILL_LNAME = forms.CharField(widget=ValueHiddenInput)
     BILL_COUNTRYCODE = forms.CharField(widget=ValueHiddenInput)
     BILL_CITY = forms.CharField(widget=ValueHiddenInput)
     BILL_PHONE = forms.CharField(widget=ValueHiddenInput)
     BILL_EMAIL = forms.CharField(widget=ValueHiddenInput)
     BILL_COMPANY = forms.CharField(widget=ValueHiddenInput)
     BILL_FISCALCODE = forms.CharField(widget=ValueHiddenInput)
 
-    CURRENCY = forms.ChoiceField(widget=ValueHiddenInput,
-                                 choices=PAYU_CURRENCIES, initial='USD')
-    AUTOMODE = forms.CharField(widget=ValueHiddenInput,
-                               initial='1')
-    LANGUAGE = forms.ChoiceField(widget=ValueHiddenInput,
-                                 choices=PAYU_LANGUAGES, initial='EN')
+    CURRENCY = forms.ChoiceField(
+        widget=ValueHiddenInput, choices=PAYU_CURRENCIES, initial="USD"
+    )
+    AUTOMODE = forms.CharField(widget=ValueHiddenInput, initial="1")
+    LANGUAGE = forms.ChoiceField(
+        widget=ValueHiddenInput, choices=PAYU_LANGUAGES, initial="EN"
+    )
     SELECTED_INSTALLMENTS_NO = forms.CharField(widget=ValueHiddenInput)
-    BACK_REF = forms.CharField(widget=ValueHiddenInput,
-                               initial=PAYU_LU_CALLBACK)
-    TESTORDER = forms.CharField(widget=ValueHiddenInput,
-                                initial=str(PAYU_TEST_TRANSACTION).upper())
+    BACK_REF = forms.CharField(widget=ValueHiddenInput, initial=PAYU_LU_CALLBACK)
+    TESTORDER = forms.CharField(
+        widget=ValueHiddenInput, initial=str(PAYU_TEST_TRANSACTION).upper()
+    )
 
     @property
     def signature(self):
         """
         Compute the ORDER_HASH of the request.
 
         The hashable string is composed by getting the values from:
@@ -173,60 +182,71 @@
         10PROD_0489110PROD_0740910PROD_0496527Extended Warranty - 5 Years8
         Dual SIM1117"Display482.371945.7545230171311220220220103RON2559
         Bucuresti9Bucuresti2RO8CCVISAMC5GROSS5GROSS5GROSS4TRUE
 
         Using this string and the MERCHANT_KEY, we compute the HMAC.
         """
 
-        hashable_fields = ['MERCHANT', 'ORDER_REF', 'ORDER_DATE',
-                           'ORDER_SHIPPING', 'PRICES_CURRENCY', 'DISCOUNT',
-                           'DESTINATION_CITY', 'DESTINATION_STATE',
-                           'DESTINATION_COUNTRY', 'PAY_METHOD',
-                           'SELECTED_INSTALLMENTS_NO', 'TESTORDER']
+        hashable_fields = [
+            "MERCHANT",
+            "ORDER_REF",
+            "ORDER_DATE",
+            "ORDER_SHIPPING",
+            "PRICES_CURRENCY",
+            "DISCOUNT",
+            "DESTINATION_CITY",
+            "DESTINATION_STATE",
+            "DESTINATION_COUNTRY",
+            "PAY_METHOD",
+            "SELECTED_INSTALLMENTS_NO",
+            "TESTORDER",
+        ]
         result = ""
 
         # We need this hack since payU is not consistent
         # with the order of fields in hash string
 
         suffix = ""
         for field in self:
-            if field.name == 'ORDER_HASH':
+            if field.name == "ORDER_HASH":
                 continue
 
             field_value = field.value()
 
             if field.name in hashable_fields and field_value:
-                encoded_value = '{length}{value}'.format(
-                    length=len(str(field_value).encode('utf-8')), value=field_value
+                encoded_value = "{length}{value}".format(
+                    length=len(str(field_value).encode("utf-8")), value=field_value
                 )
-                if field.name == 'TESTORDER' or \
-                    field.name == 'SELECTED_INSTALLMENTS_NO':
+                if (
+                    field.name == "TESTORDER"
+                    or field.name == "SELECTED_INSTALLMENTS_NO"
+                ):
                     suffix += encoded_value
                 else:
                     result += encoded_value
 
-            if field.name == 'ORDER':
+            if field.name == "ORDER":
                 for detail in PAYU_ORDER_DETAILS:
-                    if any([detail in order and order[detail]
-                            for order in field_value]):
-
+                    if any(
+                        [detail in order and order[detail] for order in field_value]
+                    ):
                         for order in field_value:
-                            value = order.get(detail, '')
+                            value = order.get(detail, "")
 
-                            item = '{length}{value}'.format(
-                                length=len(str(value).encode('utf-8')), value=value
+                            item = "{length}{value}".format(
+                                length=len(str(value).encode("utf-8")), value=value
                             )
 
-                            if detail == 'PRICE_TYPE':
+                            if detail == "PRICE_TYPE":
                                 suffix += item
                             else:
                                 result += item
 
         result += suffix
-        result = result.encode('utf-8')
+        result = result.encode("utf-8")
         return hmac.new(PAYU_MERCHANT_KEY, result, hashlib.md5).hexdigest()
 
     def _prepare_orders(self, orders):
         """
         Each order needs to have all it's details filled with default value,
         or None, in case those are not already filled.
         """
@@ -235,35 +255,34 @@
             if not any([detail in order for order in orders]):
                 for order in orders:
                     order[detail] = PAYU_ORDER_DETAILS_DEFAULTS.get(detail, None)
 
         return orders
 
     def __init__(self, **kwargs):
-        initial = kwargs.get('initial', {})
-        orders = self._prepare_orders(initial.get('ORDER', []))
+        initial = kwargs.get("initial", {})
+        orders = self._prepare_orders(initial.get("ORDER", []))
 
         super(PayULiveUpdateForm, self).__init__(**kwargs)
 
-        self.fields['ORDER'] = OrdersField(initial=orders)
-        self.fields['ORDER_HASH'].initial = self.signature
+        self.fields["ORDER"] = OrdersField(initial=orders)
+        self.fields["ORDER_HASH"].initial = self.signature
 
 
 class PayUIPNForm(forms.ModelForm):
     class Meta:
         exclude = []
         model = PayUIPN
 
     def __init__(self, data, *args, **kwargs):
         form_data = data.copy()
 
         for field in data:
             if field.endswith("[]"):
-                form_data[field[:-2]] = ",".join([value
-                                                  for value in data.getlist(field)
-                                                  if value.strip()
-                                                 ])
+                form_data[field[:-2]] = ",".join(
+                    [value for value in data.getlist(field) if value.strip()]
+                )
 
-            if field == 'IPN_DATE':
+            if field == "IPN_DATE":
                 form_data[field] = datetime.strptime(data[field], "%Y%m%d%H%M%S")
 
         super(PayUIPNForm, self).__init__(form_data)
```

### Comparing `django-payu-ro-1.4.2/payu/management/__init__.py` & `django-payu-ro-1.5.0/payu/management/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
```

### Comparing `django-payu-ro-1.4.2/payu/management/commands/__init__.py` & `django-payu-ro-1.5.0/payu/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-payu-ro-1.4.2/payu/management/commands/send_idns.py` & `django-payu-ro-1.5.0/payu/management/commands/send_idns.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,33 +19,38 @@
 
 from payu.models import PayUIDN
 
 logger = logging.getLogger(__name__)
 
 
 def string_to_list(list_as_string):
-    return list(map(int, list_as_string.strip('[] ').split(',')))
+    return list(map(int, list_as_string.strip("[] ").split(",")))
 
 
 class Command(BaseCommand):
-    help = ''
+    help = ""
 
     def add_arguments(self, parser):
         parser.add_argument(
-            '--idns',
-            help='A list of idns pks to be sent.',
-            action='store', dest='idns', type=string_to_list
+            "--idns",
+            help="A list of idns pks to be sent.",
+            action="store",
+            dest="idns",
+            type=string_to_list,
         )
 
     def handle(self, *args, **options):
         idns = PayUIDN.objects.filter(Q(sent=False) | Q(sent=True, success=False))
 
-        if options['idns']:
-            idns = idns.filter(pk__in=options['idns'])
+        if options["idns"]:
+            idns = idns.filter(pk__in=options["idns"])
 
         for idn in idns:
             idn.send()
 
             if not idn.success:
-                logger.error('Encountered exception while processing idn'
-                             'with id=%s, ex=%s.', idn.id, idn.response,
-                             exc_info=True)
+                logger.error(
+                    "Encountered exception while processing idn" "with id=%s, ex=%s.",
+                    idn.id,
+                    idn.response,
+                    exc_info=True,
+                )
```

### Comparing `django-payu-ro-1.4.2/payu/migrations/0003_auto_20200820_0858.py` & `django-payu-ro-1.5.0/payu/migrations/0003_auto_20200820_0858.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 # Generated by Django 1.11.29 on 2020-08-20 08:58
 from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('payu', '0002_payutoken_token_hash'),
+        ("payu", "0002_payutoken_token_hash"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
-            name='payutoken',
-            options={'verbose_name': 'PayU Tokens'},
+            name="payutoken",
+            options={"verbose_name": "PayU Tokens"},
         ),
         migrations.AlterField(
-            model_name='payutoken',
-            name='IPN_CC_TOKEN',
-            field=models.CharField(blank=True, max_length=9, null=True, verbose_name=b'Token (deprecated)'),
+            model_name="payutoken",
+            name="IPN_CC_TOKEN",
+            field=models.CharField(
+                blank=True, max_length=9, null=True, verbose_name=b"Token (deprecated)"
+            ),
         ),
         migrations.AlterField(
-            model_name='payutoken',
-            name='TOKEN_HASH',
-            field=models.CharField(blank=True, max_length=64, null=True, verbose_name=b'Token'),
+            model_name="payutoken",
+            name="TOKEN_HASH",
+            field=models.CharField(
+                blank=True, max_length=64, null=True, verbose_name=b"Token"
+            ),
         ),
     ]
```

### Comparing `django-payu-ro-1.4.2/payu/migrations/__init__.py` & `django-payu-ro-1.5.0/payu/migrations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
-
```

### Comparing `django-payu-ro-1.4.2/payu/models.py` & `django-payu-ro-1.5.0/payu/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,274 +21,508 @@
 import pytz
 import requests
 
 from django.db import models
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 
-from payu.signals import (payment_completed, payment_authorized,
-                          payment_flagged, alu_token_created)
-from payu.conf import (PAYU_PAYMENT_STATUS, PAYU_IDN_URL,
-                       PAYU_MERCHANT, PAYU_MERCHANT_KEY)
+from payu.signals import (
+    payment_completed,
+    payment_authorized,
+    payment_flagged,
+    alu_token_created,
+)
+from payu.conf import (
+    PAYU_PAYMENT_STATUS,
+    PAYU_IDN_URL,
+    PAYU_MERCHANT,
+    PAYU_MERCHANT_KEY,
+)
 
 
 class PayUIPN(models.Model):
-    REFNO = models.CharField(max_length=9, verbose_name='ePayment reference')
-    REFNOEXT = models.CharField(max_length=100, verbose_name='Merchant reference')
-    ORDERNO = models.CharField(max_length=6, verbose_name='Merchant order #')
-    ORDERSTATUS = models.CharField(max_length=18, choices=PAYU_PAYMENT_STATUS,
-                                   verbose_name='Status')
+    REFNO = models.CharField(max_length=9, verbose_name="ePayment reference")
+    REFNOEXT = models.CharField(max_length=100, verbose_name="Merchant reference")
+    ORDERNO = models.CharField(max_length=6, verbose_name="Merchant order #")
+    ORDERSTATUS = models.CharField(
+        max_length=18, choices=PAYU_PAYMENT_STATUS, verbose_name="Status"
+    )
     HASH = models.CharField(max_length=64)
-    PAYMETHOD_CODE = models.CharField(max_length=10,
-                                      verbose_name='Payment method code')
+    PAYMETHOD_CODE = models.CharField(max_length=10, verbose_name="Payment method code")
 
-    SALEDATE = models.DateTimeField(blank=True, null=True,
-                                    verbose_name='Sale date')
-    COMPLETE_DATE = models.DateTimeField(blank=True, null=True,
-                                         verbose_name='Complete date')
-    PAYMENTDATE = models.DateTimeField(blank=True, null=True,
-                                       verbose_name='Payment date')
-
-    PAYMETHOD = models.CharField(blank=True, null=True, max_length=100,
-                                 verbose_name='Payment method')
-    FIRSTNAME = models.CharField(blank=True, null=True, max_length=40,
-                                 help_text='Client\'s first name')
-    LASTNAME = models.CharField(blank=True, null=True, max_length=40,
-                                help_text='Client\'s last name')
-    IDENTITY_NO = models.CharField(blank=True, null=True, max_length=15,
-                                   help_text='Customer ID Card series and \
+    SALEDATE = models.DateTimeField(blank=True, null=True, verbose_name="Sale date")
+    COMPLETE_DATE = models.DateTimeField(
+        blank=True, null=True, verbose_name="Complete date"
+    )
+    PAYMENTDATE = models.DateTimeField(
+        blank=True, null=True, verbose_name="Payment date"
+    )
+
+    PAYMETHOD = models.CharField(
+        blank=True, null=True, max_length=100, verbose_name="Payment method"
+    )
+    FIRSTNAME = models.CharField(
+        blank=True, null=True, max_length=40, help_text="Client's first name"
+    )
+    LASTNAME = models.CharField(
+        blank=True, null=True, max_length=40, help_text="Client's last name"
+    )
+    IDENTITY_NO = models.CharField(
+        blank=True,
+        null=True,
+        max_length=15,
+        help_text="Customer ID Card series and \
                                    number (Series / Number - available \
-                                   only for Romanian customers)')
-    IDENTITY_ISSUER = models.CharField(blank=True, null=True, max_length=100,
-                                       help_text='IDENTITY_NO ID Card \
-                                       issuer authority ')
-    CARD_TYPE = models.CharField(blank=True, null=True, max_length=100,
-                                 help_text='Used credit card type. \
-                                 Ex: "Visa" or "MasterCard"')
-    IDENTITY_CNP = models.CharField(blank=True, null=True, max_length=13,
-                                    help_text='Customer\'s personal numeric \
-                                    code, available only for Romanian customers.')
-    COMPANY = models.CharField(blank=True, null=True, max_length=40,
-                               help_text='Company name (maximum length: \
-                                             40 characters) ')
-    REGISTRATIONNUMBER = models.CharField(blank=True, null=True, max_length=40,
-                                          help_text='Company\'s Commerce \
+                                   only for Romanian customers)",
+    )
+    IDENTITY_ISSUER = models.CharField(
+        blank=True,
+        null=True,
+        max_length=100,
+        help_text="IDENTITY_NO ID Card \
+                                       issuer authority ",
+    )
+    CARD_TYPE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=100,
+        help_text='Used credit card type. \
+                                 Ex: "Visa" or "MasterCard"',
+    )
+    IDENTITY_CNP = models.CharField(
+        blank=True,
+        null=True,
+        max_length=13,
+        help_text="Customer's personal numeric \
+                                    code, available only for Romanian customers.",
+    )
+    COMPANY = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Company name (maximum length: \
+                                             40 characters) ",
+    )
+    REGISTRATIONNUMBER = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Company's Commerce \
                                           Registry registration number \
-                                          (maximum length: 40 characters)')
-    FISCALCODE = models.CharField(blank=True, null=True, max_length=40,
-                                  help_text='Unique Registration Number / \
-                                  VAT ID (maximum length: 40 characters)')
-    CBANKNAME = models.CharField(blank=True, null=True, max_length=40,
-                                 help_text='Company\'s Bank (maximum \
-                                 length: 40 characters) ')
-    CBANKACCOUNT = models.CharField(blank=True, null=True, max_length=50,
-                                    help_text='Company\'s Bank Account \
-                                    (maximum length: 50 characters)')
-    ADDRESS1 = models.CharField(blank=True, null=True, max_length=100,
-                                help_text='Address (maximum length: 100 \
-                                characters)')
-    ADDRESS2 = models.CharField(blank=True, null=True, max_length=100,
-                                help_text='Additional Address info \
-                                (maximum length: 100 characters)')
-    CITY = models.CharField(blank=True, null=True, max_length=30,
-                            help_text='City (maximum length: 30 characters)')
-    STATE = models.CharField(blank=True, null=True, max_length=30,
-                             help_text='State/Sector/County (maximum \
-                             length: 30 characters)')
-    ZIPCODE = models.CharField(blank=True, null=True, max_length=20,
-                               help_text='ZIP/Postal Code (maximum length: \
-                               20 characters)')
-    COUNTRY = models.CharField(blank=True, null=True, max_length=50,
-                               help_text='Country (maximum length: 50 \
-                               characters)')
-    COUNTRY_CODE = models.CharField(blank=True, null=True, max_length=10,
-                                    help_text='Country (maximum length: 10 \
-                                    characters)')
-    PHONE = models.CharField(blank=True, null=True, max_length=40,
-                             help_text='Phone number (maximum length: 40 \
-                             characters)')
-    FAX = models.CharField(blank=True, null=True, max_length=40,
-                           help_text='Fax number (maximum length: 40 \
-                           characters)')
-    CUSTOMEREMAIL = models.CharField(blank=True, null=True, max_length=40,
-                                     help_text='Customer\'s e-mail address \
-                                     (maximum length: 40 characters)')
-    FIRSTNAME_D = models.CharField(blank=True, null=True, max_length=40,
-                                   help_text='First name (maximum length: \
-                                   40 characters) ')
-    LASTAME_D = models.CharField(blank=True, null=True, max_length=40,
-                                 help_text='Last Name (maximum length: 40 \
-                                 characters)')
-    COMPANY_D = models.CharField(blank=True, null=True, max_length=50,
-                                 help_text='Company (maximum length: 50 \
-                                 characters)')
-    ADDRESS1_D = models.CharField(blank=True, null=True, max_length=100,
-                                  help_text='Address (maximum length: 100 \
-                                  characters)')
-    ADDRESS2_D = models.CharField(blank=True, null=True, max_length=100,
-                                  help_text='Additional address info \
-                                  (maximum length: 100 characters)')
-    CITY_D = models.CharField(blank=True, null=True, max_length=30,
-                              help_text='City (maximum length: 30 \
-                              characters)')
-    STATE_D = models.CharField(blank=True, null=True, max_length=30,
-                               help_text='State/Sector/County (maximum \
-                               length: 30 characters)')
-    ZIPCODE_D = models.CharField(blank=True, null=True, max_length=20,
-                                 help_text='ZIP/Postal Code (maximum \
-                                 length: 20 characters)')
-    COUNTRY_D = models.CharField(blank=True, null=True, max_length=50,
-                                 help_text='Country (maximum length: 50 \
-                                 characters)')
-    COUNTRY_D_CODE = models.CharField(blank=True, null=True, max_length=10,
-                                      help_text='Country (maximum length: \
-                                      10 characters)')
-    PHONE_D = models.CharField(blank=True, null=True, max_length=40,
-                               help_text='Phone number (maximum length: 40 \
-                               characters)')
-    EMAIL_D = models.CharField(blank=True, null=True, max_length=40,
-                               help_text='E-mail (maximum length: 40 \
-                               characters)')
-    IPADDRESS = models.CharField(blank=True, null=True, max_length=250,
-                                 help_text='Client\'s IP Address (maximum \
-                                 length: 250 characters)')
-    IPCOUNTRY = models.CharField(blank=True, null=True, max_length=50,
-                                 help_text='Client\'s IP Country (maximum \
-                                 length: 50 characters)')
-    COMPLETE_DATE = models.CharField(blank=True, null=True, max_length=40,
-                                     help_text='The order completion date, \
+                                          (maximum length: 40 characters)",
+    )
+    FISCALCODE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Unique Registration Number / \
+                                  VAT ID (maximum length: 40 characters)",
+    )
+    CBANKNAME = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Company's Bank (maximum \
+                                 length: 40 characters) ",
+    )
+    CBANKACCOUNT = models.CharField(
+        blank=True,
+        null=True,
+        max_length=50,
+        help_text="Company's Bank Account \
+                                    (maximum length: 50 characters)",
+    )
+    ADDRESS1 = models.CharField(
+        blank=True,
+        null=True,
+        max_length=100,
+        help_text="Address (maximum length: 100 \
+                                characters)",
+    )
+    ADDRESS2 = models.CharField(
+        blank=True,
+        null=True,
+        max_length=100,
+        help_text="Additional Address info \
+                                (maximum length: 100 characters)",
+    )
+    CITY = models.CharField(
+        blank=True,
+        null=True,
+        max_length=30,
+        help_text="City (maximum length: 30 characters)",
+    )
+    STATE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=30,
+        help_text="State/Sector/County (maximum \
+                             length: 30 characters)",
+    )
+    ZIPCODE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=20,
+        help_text="ZIP/Postal Code (maximum length: \
+                               20 characters)",
+    )
+    COUNTRY = models.CharField(
+        blank=True,
+        null=True,
+        max_length=50,
+        help_text="Country (maximum length: 50 \
+                               characters)",
+    )
+    COUNTRY_CODE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=10,
+        help_text="Country (maximum length: 10 \
+                                    characters)",
+    )
+    PHONE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Phone number (maximum length: 40 \
+                             characters)",
+    )
+    FAX = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Fax number (maximum length: 40 \
+                           characters)",
+    )
+    CUSTOMEREMAIL = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Customer's e-mail address \
+                                     (maximum length: 40 characters)",
+    )
+    FIRSTNAME_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="First name (maximum length: \
+                                   40 characters) ",
+    )
+    LASTAME_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Last Name (maximum length: 40 \
+                                 characters)",
+    )
+    COMPANY_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=50,
+        help_text="Company (maximum length: 50 \
+                                 characters)",
+    )
+    ADDRESS1_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=100,
+        help_text="Address (maximum length: 100 \
+                                  characters)",
+    )
+    ADDRESS2_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=100,
+        help_text="Additional address info \
+                                  (maximum length: 100 characters)",
+    )
+    CITY_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=30,
+        help_text="City (maximum length: 30 \
+                              characters)",
+    )
+    STATE_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=30,
+        help_text="State/Sector/County (maximum \
+                               length: 30 characters)",
+    )
+    ZIPCODE_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=20,
+        help_text="ZIP/Postal Code (maximum \
+                                 length: 20 characters)",
+    )
+    COUNTRY_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=50,
+        help_text="Country (maximum length: 50 \
+                                 characters)",
+    )
+    COUNTRY_D_CODE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=10,
+        help_text="Country (maximum length: \
+                                      10 characters)",
+    )
+    PHONE_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Phone number (maximum length: 40 \
+                               characters)",
+    )
+    EMAIL_D = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="E-mail (maximum length: 40 \
+                               characters)",
+    )
+    IPADDRESS = models.CharField(
+        blank=True,
+        null=True,
+        max_length=250,
+        help_text="Client's IP Address (maximum \
+                                 length: 250 characters)",
+    )
+    IPCOUNTRY = models.CharField(
+        blank=True,
+        null=True,
+        max_length=50,
+        help_text="Client's IP Country (maximum \
+                                 length: 50 characters)",
+    )
+    COMPLETE_DATE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="The order completion date, \
                                      in the following format: Y-m-d H:i:s \
-                                     (2012-04-26 15:02:28) .')
-    CURRENCY = models.CharField(blank=True, null=True, max_length=10,
-                                help_text='The currency in which the order \
+                                     (2012-04-26 15:02:28) .",
+    )
+    CURRENCY = models.CharField(
+        blank=True,
+        null=True,
+        max_length=10,
+        help_text="The currency in which the order \
                                 has been processed. Possible values: RON, \
-                                USD, EUR.')
-    LANGUAGE = models.CharField(blank=True, null=True, max_length=40,
-                                help_text='The language in which the order \
+                                USD, EUR.",
+    )
+    LANGUAGE = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="The language in which the order \
                                 has been processed. Possible values: ro, \
-                                en, fr, de, it.')
+                                en, fr, de, it.",
+    )
 
-    IPN_PID = models.TextField(blank=True, null=True,
-                               help_text='Array with the ID Codes of the \
+    IPN_PID = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with the ID Codes of the \
                                ordered products, in the PayU database (PayU \
-                               reference) ')
-    IPN_PNAME = models.TextField(blank=True, null=True,
-                                 help_text='Array with product names ')
-    IPN_PCODE = models.TextField(blank=True, null=True,
-                                 help_text='Array with the product codes \
+                               reference) ",
+    )
+    IPN_PNAME = models.TextField(
+        blank=True, null=True, help_text="Array with product names "
+    )
+    IPN_PCODE = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with the product codes \
                                  assigned by the vendor in the system (vendor \
-                                 reference)')
-    IPN_INFO = models.TextField(blank=True, null=True,
-                                help_text='Array with additional \
+                                 reference)",
+    )
+    IPN_INFO = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with additional \
                                 information sent for each ordered product (if \
-                                they have been sent to PayU)')
-    IPN_QTY = models.TextField(blank=True, null=True,
-                               help_text='Array with the product quantities')
-    IPN_PRICE = models.TextField(blank=True, null=True,
-                                 help_text='Array with unit prices per \
+                                they have been sent to PayU)",
+    )
+    IPN_QTY = models.TextField(
+        blank=True, null=True, help_text="Array with the product quantities"
+    )
+    IPN_PRICE = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with unit prices per \
                                  product (without VAT), in RON, with \
                                  period/full-stop (.) as decimal place \
-                                 separator')
-    IPN_VAT = models.TextField(blank=True, null=True,
-                               help_text='Array with VAT values per \
+                                 separator",
+    )
+    IPN_VAT = models.TextField(
+        blank=True,
+        null=True,
+        help_text='Array with VAT values per \
                                product, with period "." as decimal place \
-                               separator')
-    IPN_VER = models.TextField(blank=True, null=True,
-                               help_text='Array with product versions \
-                               (maximum length: 50 characters)')
-    IPN_DISCOUNT = models.TextField(blank=True, null=True,
-                                    help_text='Array with the amounts with \
+                               separator',
+    )
+    IPN_VER = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with product versions \
+                               (maximum length: 50 characters)",
+    )
+    IPN_DISCOUNT = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with the amounts with \
                                     which there has been made a discount \
-                                    in a promotion. Including VAT. ')
-    IPN_PROMONAME = models.TextField(blank=True, null=True,
-                                     help_text='Array with the names of the \
+                                    in a promotion. Including VAT. ",
+    )
+    IPN_PROMONAME = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with the names of the \
                                      promotions in which the discounts \
-                                     specified above have been made.')
-    IPN_PROMOCODE = models.TextField(blank=True, null=True,
-                                     help_text='Array with the code of the \
+                                     specified above have been made.",
+    )
+    IPN_PROMOCODE = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with the code of the \
                                      promotions in which the discounts \
-                                     specified above have been made.')
-    IPN_ORDER_COSTS = models.TextField(blank=True, null=True,
-                                       help_text='Array with costs for each \
+                                     specified above have been made.",
+    )
+    IPN_ORDER_COSTS = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with costs for each \
                                        product from order (expressed in \
-                                       order\'s currency)')
-    IPN_REC_CURRENT_ITERATION_NO = models.TextField(blank=True, null=True,
-                                                    help_text='Current recurring \
+                                       order's currency)",
+    )
+    IPN_REC_CURRENT_ITERATION_NO = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Current recurring \
                                                                   period (avaible \
                                                                   only for recurrent \
-                                                                  payments)')
-    IPN_REC_ORIGINAL_REFNO = models.TextField(blank=True, null=True,
-                                              help_text='Array containing \
+                                                                  payments)",
+    )
+    IPN_REC_ORIGINAL_REFNO = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array containing \
                                                             the reference to \
-                                                            the original order')
-    IPN_REC_INTERVAL = models.TextField(blank=True, null=True,
-                                        help_text='Array containing \
+                                                            the original order",
+    )
+    IPN_REC_INTERVAL = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array containing \
                                                       recurring intervals \
                                                       (day/month/week) for \
-                                                      each order')
-    IPN_REC_EXPIRATION_DATE = models.TextField(blank=True, null=True,
-                                               help_text='Array with \
+                                                      each order",
+    )
+    IPN_REC_EXPIRATION_DATE = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with \
                                                              expiration dates \
                                                              for each \
-                                                             recurrence')
-    IPN_REC_MULTIPLIER = models.TextField(blank=True, null=True,
-                                          help_text='Array with reccurence \
+                                                             recurrence",
+    )
+    IPN_REC_MULTIPLIER = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with reccurence \
                                                         period (interval x \
                                                         multiplier) for each \
-                                                        product from the order')
-    IPN_DELIVEREDCODES = models.TextField(blank=True, null=True,
-                                          help_text='Array with the codes \
+                                                        product from the order",
+    )
+    IPN_DELIVEREDCODES = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Array with the codes \
                                                         delivered to the \
                                                         clients, if the PayU \
                                                         contract contains this \
                                                         feature. Each element \
                                                         in the array is \
                                                         represented by a \
                                                         string, having comma \
                                                         (,) as a separator for \
                                                         each sent code, in \
                                                         case the ordered \
                                                         quantity is greater \
-                                                        than 1.')
-    IPN_DOWNLOAD_LINK = models.CharField(blank=True, null=True, max_length=250,
-                                         help_text='Download link of the \
+                                                        than 1.",
+    )
+    IPN_DOWNLOAD_LINK = models.CharField(
+        blank=True,
+        null=True,
+        max_length=250,
+        help_text="Download link of the \
                                                        product delivered to \
-                                                       the client')
-    IPN_TOTAL = models.TextField(blank=True, null=True,
-                                 help_text='Partial total on order line \
+                                                       the client",
+    )
+    IPN_TOTAL = models.TextField(
+        blank=True,
+        null=True,
+        help_text="Partial total on order line \
                                                (including VAT), with \
                                                period/full-stop (.) as a \
-                                               decimal place separator')
-    IPN_TOTALGENERAL = models.CharField(blank=True, null=True, max_length=40,
-                                        help_text='Total transaction \
+                                               decimal place separator",
+    )
+    IPN_TOTALGENERAL = models.CharField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="Total transaction \
                                                       amount, including VAT \
                                                       costs, with \
                                                       period/full-stop (.) as \
                                                       a decimal place \
-                                                      separator')
-    IPN_SHIPPING = models.CharField(blank=True, null=True, max_length=50,
-                                    help_text='Total amount paid for \
-                                                  shippment')
-    IPN_REFERRER = models.CharField(blank=True, null=True, max_length=250,
-                                    help_text='HTTP referrer of the sale.')
-    IPN_GLOBALDISCOUNT = models.CharField(blank=True, null=True, max_length=250,
-                                          help_text='Global discount of the \
+                                                      separator",
+    )
+    IPN_SHIPPING = models.CharField(
+        blank=True,
+        null=True,
+        max_length=50,
+        help_text="Total amount paid for \
+                                                  shippment",
+    )
+    IPN_REFERRER = models.CharField(
+        blank=True, null=True, max_length=250, help_text="HTTP referrer of the sale."
+    )
+    IPN_GLOBALDISCOUNT = models.CharField(
+        blank=True,
+        null=True,
+        max_length=250,
+        help_text="Global discount of the \
                                                         sale. This field is \
                                                         option and is avaible \
                                                         only if the amount is \
-                                                        greater than zero.')
-    IPN_COMMISSION = models.CharField(blank=True, null=True, max_length=50,
-                                      help_text='Payu\'s commision in RON, \
+                                                        greater than zero.",
+    )
+    IPN_COMMISSION = models.CharField(
+        blank=True,
+        null=True,
+        max_length=50,
+        help_text="Payu's commision in RON, \
                                                     with period/full-stop (.) \
                                                     as a decimal place \
-                                                    separator.')
-    IPN_DATE = models.DateTimeField(blank=True, null=True, max_length=40,
-                                    help_text='IPN POST\'s sending date in the \
+                                                    separator.",
+    )
+    IPN_DATE = models.DateTimeField(
+        blank=True,
+        null=True,
+        max_length=40,
+        help_text="IPN POST's sending date in the \
                                                following format: YmdHMS (ex.: \
-                                               20120426145935)')
+                                               20120426145935)",
+    )
 
     response = models.TextField(blank=True)
     ip_address = models.GenericIPAddressField(blank=True, null=True)
 
     flag = models.BooleanField(default=False)
     flag_info = models.TextField(blank=True)
 
@@ -301,39 +535,39 @@
         """
 
         self.flag = True
         self.flag_info += info
 
     @property
     def is_authorized(self):
-        return self.ORDERSTATUS in ['PAYMENT_AUTHORIZED', 'PAYMENT_RECEIVED', 'TEST']
+        return self.ORDERSTATUS in ["PAYMENT_AUTHORIZED", "PAYMENT_RECEIVED", "TEST"]
 
     @property
     def is_completed(self):
-        return self.ORDERSTATUS == 'COMPLETE'
+        return self.ORDERSTATUS == "COMPLETE"
 
     def __unicode__(self):
-        return u'<IPN: %s>' % self.REFNO
+        return "<IPN: %s>" % self.REFNO
 
     class Meta:
-        verbose_name = 'PayU IPN'
-        db_table = 'payu_ipn'
-        app_label = 'payu'
+        verbose_name = "PayU IPN"
+        db_table = "payu_ipn"
+        app_label = "payu"
 
 
 class PayUIDN(models.Model):
     ipn = models.OneToOneField(PayUIPN, on_delete=models.CASCADE)
     sent = models.BooleanField(default=False)
 
     success = models.BooleanField(default=False)
     response = models.TextField(blank=True)
 
     class Meta:
-        verbose_name = 'PayU IDN'
-        app_label = 'payu'
+        verbose_name = "PayU IDN"
+        app_label = "payu"
 
     def send(self):
         payload = self._build_payload(PAYU_MERCHANT, PAYU_MERCHANT_KEY)
 
         try:
             response = requests.post(PAYU_IDN_URL, data=payload)
 
@@ -344,63 +578,81 @@
             self.success = False
 
         self.sent = True
         self.save()
 
     @classmethod
     def signature(cls, payload, merchant_key):
-        hashable_fields = ["MERCHANT", "ORDER_REF", "ORDER_AMOUNT", "ORDER_CURRENCY", "IDN_DATE",
-                           "CHARGE_AMOUNT"]
+        hashable_fields = [
+            "MERCHANT",
+            "ORDER_REF",
+            "ORDER_AMOUNT",
+            "ORDER_CURRENCY",
+            "IDN_DATE",
+            "CHARGE_AMOUNT",
+        ]
 
         hash_values = [payload[field] for field in hashable_fields if field in payload]
 
         confirmation_hash = "".join(
-            ['{length}{value}'.format(
-                    length=len(str(value).encode('utf-8')), value=value
-            ) for value in hash_values]
-        ).encode('utf-8')
+            [
+                "{length}{value}".format(
+                    length=len(str(value).encode("utf-8")), value=value
+                )
+                for value in hash_values
+            ]
+        ).encode("utf-8")
         return hmac.new(merchant_key, confirmation_hash, hashlib.md5).hexdigest()
 
     def _build_payload(self, merchant, merchant_key, now=None):
-        payload = OrderedDict([
-            ('MERCHANT', merchant),
-            ('ORDER_REF', self.ipn.REFNO or -1),
-            ('ORDER_AMOUNT', self.ipn.IPN_TOTALGENERAL or 0),
-            ('ORDER_CURRENCY', self.ipn.CURRENCY or 'RON'),
-            ('IDN_DATE', now or datetime.now(pytz.UTC).strftime('%Y-%m-%d %H:%M:%S')),
-        ])
+        payload = OrderedDict(
+            [
+                ("MERCHANT", merchant),
+                ("ORDER_REF", self.ipn.REFNO or -1),
+                ("ORDER_AMOUNT", self.ipn.IPN_TOTALGENERAL or 0),
+                ("ORDER_CURRENCY", self.ipn.CURRENCY or "RON"),
+                (
+                    "IDN_DATE",
+                    now or datetime.now(pytz.UTC).strftime("%Y-%m-%d %H:%M:%S"),
+                ),
+            ]
+        )
         payload["ORDER_HASH"] = self.signature(payload, merchant_key)
 
         return payload
 
     def __unicode__(self):
-        return u'<IDN: %s>' % self.pk
+        return "<IDN: %s>" % self.pk
 
 
 class PayUToken(models.Model):
     ipn = models.OneToOneField(PayUIPN, on_delete=models.CASCADE)
 
     # used for token/v1 api payments (same value as IPN's REFNO)
     # DEPRECATED
-    IPN_CC_TOKEN = models.CharField(max_length=9, verbose_name="Token (deprecated)", blank=True, null=True)
+    IPN_CC_TOKEN = models.CharField(
+        max_length=9, verbose_name="Token (deprecated)", blank=True, null=True
+    )
 
     # can be used for the `IPN_CC_TOKEN` field in alu/v3 token payments
-    TOKEN_HASH = models.CharField(max_length=64, verbose_name="Token", blank=True, null=True)
+    TOKEN_HASH = models.CharField(
+        max_length=64, verbose_name="Token", blank=True, null=True
+    )
 
     # documentation is unclear of the length and format of this field
     IPN_CC_MASK = models.CharField(max_length=36, verbose_name="Last 4 digits")
 
     IPN_CC_EXP_DATE = models.DateField(verbose_name="Expiration date")
 
     class Meta:
-        verbose_name = 'PayU Tokens'
-        app_label = 'payu'
+        verbose_name = "PayU Tokens"
+        app_label = "payu"
 
     def __unicode__(self):
-        return u'<Token: %s>' % (self.TOKEN_HASH or self.IPN_CC_TOKEN)
+        return "<Token: %s>" % (self.TOKEN_HASH or self.IPN_CC_TOKEN)
 
 
 @receiver(post_save, sender=PayUToken)
 def post_payu_ipn_cc_token_save(sender, instance=None, **kwargs):
     alu_token_created.send(sender=instance)
```

### Comparing `django-payu-ro-1.4.2/payu/payments.py` & `django-payu-ro-1.5.0/payu/payments.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,90 +13,100 @@
 # limitations under the License.
 import hashlib
 import hmac
 from datetime import datetime
 
 import requests
 
-from payu.conf import (PAYU_MERCHANT_KEY, PAYU_MERCHANT,
-                       PAYU_ALU_URL, PAYU_TOKENS_URL)
+from payu.conf import PAYU_MERCHANT_KEY, PAYU_MERCHANT, PAYU_ALU_URL, PAYU_TOKENS_URL
 
 
 class BasePayment(object):
-    def __init__(self, order, token, merchant_key=PAYU_MERCHANT_KEY,
-                 merchant=PAYU_MERCHANT):
-
+    def __init__(
+        self, order, token, merchant_key=PAYU_MERCHANT_KEY, merchant=PAYU_MERCHANT
+    ):
         self.order = order
         self.token = token
         self.merchant_key = merchant_key
         self.merchant = merchant
 
     def pay(self):
         raise NotImplementedError
 
     @classmethod
     def get_signature(self, payload, merchant_key):
         sorted_payload = sorted(payload.items(), key=lambda item: item[0])
         parameters = "".join(
-            ['{length}{value}'.format(
-                length=len(str(parameter[1]).encode('utf-8')), value=parameter[1]
-            ) for parameter in sorted_payload]
-        ).encode('utf-8')
+            [
+                "{length}{value}".format(
+                    length=len(str(parameter[1]).encode("utf-8")), value=parameter[1]
+                )
+                for parameter in sorted_payload
+            ]
+        ).encode("utf-8")
         return hmac.new(merchant_key, parameters, hashlib.md5).hexdigest()
 
 
 class TokenPayment(BasePayment):
     def pay(self):
-        return requests.post(PAYU_TOKENS_URL,
-                             data=self._build_payload()).content
+        return requests.post(PAYU_TOKENS_URL, data=self._build_payload()).content
 
     def _build_payload(self):
         payload = {
-            'REF_NO': self.token,
-            'METHOD': 'TOKEN_NEWSALE',
-            'MERCHANT': self.merchant,
-            'TIMESTAMP': datetime.now().strftime("%Y%m%d%H%M%S"),
+            "REF_NO": self.token,
+            "METHOD": "TOKEN_NEWSALE",
+            "MERCHANT": self.merchant,
+            "TIMESTAMP": datetime.now().strftime("%Y%m%d%H%M%S"),
         }
 
         payload.update(self.order)
 
-        payload['SIGN'] = self.get_signature(payload, self.merchant_key)
+        payload["SIGN"] = self.get_signature(payload, self.merchant_key)
 
         return payload
 
 
 class ALUPayment(BasePayment):
-    def __init__(self, *args, **kwargs):
-        self.stored_credentials_use_type = kwargs.pop("stored_credentials_use_type", None)
-        self.threeds_data = kwargs.pop("threeds_data", {})
+    def __init__(
+        self,
+        order,
+        token,
+        stored_credentials_use_type=None,
+        threeds_data: dict = None,
+        **kwargs
+    ):
+        self.stored_credentials_use_type = stored_credentials_use_type
+        self.threeds_data = threeds_data or {}
 
-        super(ALUPayment, self).__init__(*args, **kwargs)
+        super(ALUPayment, self).__init__(order, token, **kwargs)
 
     def pay(self):
-        return requests.post(PAYU_ALU_URL, data=self._build_payload()).content
+        self._request = self._build_payload()
+        self._response = requests.post(PAYU_ALU_URL, data=self._request).content
+
+        return self._response
 
     def _build_payload(self):
         order = self.order
         order["MERCHANT"] = self.merchant
         if not order.get("ORDER_DATE"):
-            order["ORDER_DATE"] = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+            order["ORDER_DATE"] = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
-        payload = self._parse_orders(order.pop('ORDER'))
-        payload['CC_TOKEN'] = self.token
-        if self.stored_credentials_use_type and payload['CC_TOKEN']:
-            payload['CC_CVV'] = ""
-            payload['STORED_CREDENTIALS_USE_TYPE'] = self.stored_credentials_use_type
-
-            if isinstance(self.threeds_data, dict):
-                payload['STRONG_CUSTOMER_AUTHENTICATION'] = "YES" if self.threeds_data else "NO"
-                payload.update(self.threeds_data)
+        payload = self._parse_orders(order.pop("ORDER"))
+        payload["CC_TOKEN"] = self.token
+        if self.stored_credentials_use_type and payload["CC_TOKEN"]:
+            payload["CC_CVV"] = ""
+            payload["STORED_CREDENTIALS_USE_TYPE"] = self.stored_credentials_use_type
+
+        if self.threeds_data and isinstance(self.threeds_data, dict):
+            payload["STRONG_CUSTOMER_AUTHENTICATION"] = "YES"
+            payload.update(self.threeds_data)
 
         payload.update(**order)
-        payload["ORDER_HASH"] = ALUPayment.get_signature(payload,
-                                                         self.merchant_key)
+        payload["ORDER_HASH"] = ALUPayment.get_signature(payload, self.merchant_key)
 
         return payload
 
     def _parse_orders(self, orders):
         r"""
         Transform orders from list objects to PHP arrays:
             [
```

### Comparing `django-payu-ro-1.4.2/payu/signals.py` & `django-payu-ro-1.5.0/payu/signals.py`

 * *Files identical despite different names*

### Comparing `django-payu-ro-1.4.2/payu/urls.py` & `django-payu-ro-1.5.0/tests/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,13 @@
+# Copyright (c) 2017 Presslabs SRL
 #
-# Copyright 2012-2016 PressLabs SRL
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#    Licensed under the Apache License, Version 2.0 (the "License");
-#    you may not use this file except in compliance with the License.
-#    You may obtain a copy of the License at
+#    http://www.apache.org/licenses/LICENSE-2.0
 #
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-#    Unless required by applicable law or agreed to in writing, software
-#    distributed under the License is distributed on an "AS IS" BASIS,
-#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    See the License for the specific language governing permissions and
-#    limitations under the License.
-#
-
-from django.conf.urls import re_path
-
-from .views import ipn
-
-urlpatterns = [
-    re_path(r'^ipn/$', ipn, name='payu-ipn'),
-]
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `django-payu-ro-1.4.2/payu/views.py` & `django-payu-ro-1.5.0/payu/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,74 +45,79 @@
     for field in PAYU_IPN_FIELDS:
         if field not in request.POST:
             continue
 
         field_value = request.POST.getlist(field)
 
         validation_hash += "".join(
-            ['{length}{value}'.format(
-                length=len(value.encode('utf-8')), value=value
-            ) for value in field_value]
+            [
+                "{length}{value}".format(length=len(value.encode("utf-8")), value=value)
+                for value in field_value
+            ]
         )
 
-    validation_hash = validation_hash.encode('utf-8')
+    validation_hash = validation_hash.encode("utf-8")
 
-    expected_hash = hmac.new(PAYU_MERCHANT_KEY, validation_hash, hashlib.md5).hexdigest()
-    request_hash = request.POST.get('HASH', '')
+    expected_hash = hmac.new(
+        PAYU_MERCHANT_KEY, validation_hash, hashlib.md5
+    ).hexdigest()
+    request_hash = request.POST.get("HASH", "")
 
     if request_hash != expected_hash:
-        error = 'Invalid hash %s. Hash string \n%s' % (request_hash, expected_hash)
+        error = "Invalid hash %s. Hash string \n%s" % (request_hash, expected_hash)
     else:
         if ipn_form.is_valid():
             try:
                 ipn_obj = ipn_form.save(commit=False)
             except Exception as exception:
                 error = "Exception while processing. (%s)" % exception
         else:
             error = "Invalid form. (%s)" % ipn_form.errors
 
     if not ipn_obj:
         ipn_obj = PayUIPN()
 
     # Set query params and sender's IP address
     ipn_obj.response = getattr(request, request.method).urlencode()
-    ipn_obj.ip_address = request.META.get('REMOTE_ADDR', '')
+    ipn_obj.ip_address = request.META.get("REMOTE_ADDR", "")
 
     if error:
         # We save errors in the error field
         ipn_obj.set_flag(error)
 
     ipn_obj.save()
 
     # Check for a token in the request and save it if found
-    IPN_CC_TOKEN = request.POST.get('IPN_CC_TOKEN')
-    TOKEN_HASH = request.POST.get('TOKEN_HASH')
-    IPN_CC_MASK = request.POST.get('IPN_CC_MASK')
-    IPN_CC_EXP_DATE = request.POST.get('IPN_CC_EXP_DATE')
+    IPN_CC_TOKEN = request.POST.get("IPN_CC_TOKEN")
+    TOKEN_HASH = request.POST.get("TOKEN_HASH")
+    IPN_CC_MASK = request.POST.get("IPN_CC_MASK")
+    IPN_CC_EXP_DATE = request.POST.get("IPN_CC_EXP_DATE")
 
     if all([(IPN_CC_TOKEN or TOKEN_HASH), IPN_CC_MASK, IPN_CC_EXP_DATE]):
         PayUToken.objects.create(
             IPN_CC_TOKEN=IPN_CC_TOKEN,
             IPN_CC_MASK=IPN_CC_MASK,
             IPN_CC_EXP_DATE=IPN_CC_EXP_DATE,
             TOKEN_HASH=TOKEN_HASH,
-            ipn=ipn_obj
+            ipn=ipn_obj,
         )
 
     PayUIDN.objects.create(ipn=ipn_obj)
 
     # Send confirmation to PayU that we received this request
-    date = datetime.now(pytz.UTC).strftime('%Y%m%d%H%M%S')
+    date = datetime.now(pytz.UTC).strftime("%Y%m%d%H%M%S")
 
     confirmation_hash = b""
     for field in ["IPN_PID[]", "IPN_PNAME[]", "IPN_DATE"]:
         field_value = request.POST.getlist(field)
 
         if not field_value:
             confirmation_hash += b"0"
         else:
             confirmation_hash += field_value
 
-    confirmation_hash = hmac.new(PAYU_MERCHANT_KEY,
-                                 b'%s14%s' % (confirmation_hash, date.encode('utf-8')),
-                                 hashlib.md5).hexdigest()
-    return HttpResponse('<EPAYMENT>%s|%s</EPAYMENT>' % (date, confirmation_hash))
+    confirmation_hash = hmac.new(
+        PAYU_MERCHANT_KEY,
+        b"%s14%s" % (confirmation_hash, date.encode("utf-8")),
+        hashlib.md5,
+    ).hexdigest()
+    return HttpResponse("<EPAYMENT>%s|%s</EPAYMENT>" % (date, confirmation_hash))
```

### Comparing `django-payu-ro-1.4.2/setup.py` & `django-payu-ro-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,29 +40,31 @@
 http://docs.python.org/2/distutils/sourcedist.html
 """
 
 from setuptools import setup, find_packages
 
 import payu
 
-install_requires = [line.strip()
-                    for line in open("requirements.txt").readlines()
-                    if not line.strip().startswith('#') and line.strip()]
+install_requires = [
+    line.strip()
+    for line in open("requirements.txt").readlines()
+    if not line.strip().startswith("#") and line.strip()
+]
 
 setup(
-    name='django-payu-ro',
+    name="django-payu-ro",
     version=payu.__version__,
-    author='Presslabs SRL',
-    author_email='support@presslabs.com',
-    url='http://github.com/PressLabs/django-payu-ro',
-    description='A pluggable Django application for integrating PayU Payments (ex. ePayment)',
+    author="Presslabs SRL",
+    author_email="support@presslabs.com",
+    url="http://github.com/PressLabs/django-payu-ro",
+    description="A pluggable Django application for integrating PayU Payments (ex. ePayment)",
     packages=find_packages(),
     include_package_data=True,
     install_requires=install_requires,
     classifiers=[
         "Framework :: Django",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
-        "Topic :: Software Development"
+        "Topic :: Software Development",
     ],
 )
```

### Comparing `django-payu-ro-1.4.2/tests/__init__.py` & `django-payu-ro-1.5.0/payu/urls.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,23 @@
-# Copyright (c) 2017 Presslabs SRL
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+# Copyright 2012-2016 PressLabs SRL
 #
-#    http://www.apache.org/licenses/LICENSE-2.0
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+#
+
+from django.conf.urls import re_path
+
+from .views import ipn
 
+urlpatterns = [
+    re_path(r"^ipn/$", ipn, name="payu-ipn"),
+]
```

### Comparing `django-payu-ro-1.4.2/tests/conftest.py` & `django-payu-ro-1.5.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,25 +16,31 @@
 
 import django
 from django.conf import settings
 
 
 settings.configure(
     DEBUG=True,
-    ROOT_URLCONF='payu.urls',
+    ROOT_URLCONF="payu.urls",
     DATABASES={
-        'default': {
-            'ENGINE': 'django.db.backends.sqlite3',
+        "default": {
+            "ENGINE": "django.db.backends.sqlite3",
         }
     },
-    PAYU_MERCHANT='PAYUDEMO',
-    PAYU_KEY='1231234567890123',
-    INSTALLED_APPS=('django.contrib.auth',
-                    'django.contrib.contenttypes',
-                    'django.contrib.sessions',
-                    'django.contrib.admin',
-                    'payu',),
-    SECRET_KEY='dummy'
+    PAYU_CALLBACK_URL="https://test.com",
+    PAYU_LU_URL="https://test.com",
+    PAYU_ALU_URL="https://test.com",
+    PAYU_IDN_URL="https://test.com",
+    PAYU_MERCHANT="PAYUDEMO",
+    PAYU_KEY="1231234567890123",
+    INSTALLED_APPS=(
+        "django.contrib.auth",
+        "django.contrib.contenttypes",
+        "django.contrib.sessions",
+        "django.contrib.admin",
+        "payu",
+    ),
+    SECRET_KEY="dummy",
 )
 
 
 django.setup()
```

### Comparing `django-payu-ro-1.4.2/tests/test_models.py` & `django-payu-ro-1.5.0/tests/test_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,104 +16,131 @@
 from mock import patch, MagicMock
 from django_dynamic_fixture import G
 
 from payu.models import PayUIPN, PayUIDN
 from payu.conf import PAYU_IDN_URL
 
 
-@pytest.mark.parametrize('flag_info, extra_info', [
-    ('', ''),
-    ('1', ''),
-    ('1', '1'),
-])
+@pytest.mark.parametrize(
+    "flag_info, extra_info",
+    [
+        ("", ""),
+        ("1", ""),
+        ("1", "1"),
+    ],
+)
 def test_payu_model_flag(flag_info, extra_info):
     model = PayUIPN(flag_info=flag_info)
     model.set_flag(extra_info)
     assert model.flag_info == flag_info + extra_info
     assert model.flag
 
 
-@pytest.mark.parametrize('order, authorized, completed', [
-    ('1', False, False),
-    ('TEST', True, False),
-    ('PAYMENT_RECEIVED', True, False),
-    ('PAYMENT_AUTHORIZED', True, False),
-    ('COMPLETE', False, True),
-    ('', False, False)
-])
+@pytest.mark.parametrize(
+    "order, authorized, completed",
+    [
+        ("1", False, False),
+        ("TEST", True, False),
+        ("PAYMENT_RECEIVED", True, False),
+        ("PAYMENT_AUTHORIZED", True, False),
+        ("COMPLETE", False, True),
+        ("", False, False),
+    ],
+)
 def test_payu_model_order_status(order, authorized, completed):
     model = PayUIPN(ORDERSTATUS=order)
     assert model.is_authorized == authorized
     assert model.is_completed == completed
 
 
 @pytest.mark.django_db
-@patch('payu.models.payment_authorized')
+@patch("payu.models.payment_authorized")
 def test_payu_model_authorized_signals(mock_authorized):
-    model = G(PayUIPN, ORDERSTATUS='TEST')
+    model = G(PayUIPN, ORDERSTATUS="TEST")
     mock_authorized.send.assert_called_once_with(sender=model)
 
 
 @pytest.mark.django_db
-@patch('payu.models.payment_completed')
+@patch("payu.models.payment_completed")
 def test_payu_model_completed_signals(mock_completed):
-    model = G(PayUIPN, ORDERSTATUS='COMPLETE')
+    model = G(PayUIPN, ORDERSTATUS="COMPLETE")
     mock_completed.send.assert_called_once_with(sender=model)
 
 
 @pytest.mark.django_db
-@patch('payu.models.payment_flagged')
+@patch("payu.models.payment_flagged")
 def test_payu_model_flagged_signals(mock_flagged):
     model = G(PayUIPN, flag=True)
     mock_flagged.send.assert_called_once_with(sender=model)
 
 
-@pytest.mark.parametrize('payload, merchant_key, signature', [
-    (
-        {}, b'0', '477f91ddbcc6839b9950045977da3530'
-    ), (
-        # example from payu docs (with actually wrong hash)
-        # check online: source b"8MERCHANT73954142539.993USD192015-05-11 14:32:08"
-        #               key b"1231234567890123"
-        {'MERCHANT': 'MERCHANT', 'ORDER_REF': 3954142, 'ORDER_AMOUNT': 39.99,
-         'ORDER_CURRENCY': 'USD', 'IDN_DATE': '2015-05-11 14:32:08'},
-        b'1231234567890123', 'e40a3d1505cbb15e34cf35f34c784bb0'
-)])
+@pytest.mark.parametrize(
+    "payload, merchant_key, signature",
+    [
+        ({}, b"0", "477f91ddbcc6839b9950045977da3530"),
+        (
+            # example from payu docs (with actually wrong hash)
+            # check online: source b"8MERCHANT73954142539.993USD192015-05-11 14:32:08"
+            #               key b"1231234567890123"
+            {
+                "MERCHANT": "MERCHANT",
+                "ORDER_REF": 3954142,
+                "ORDER_AMOUNT": 39.99,
+                "ORDER_CURRENCY": "USD",
+                "IDN_DATE": "2015-05-11 14:32:08",
+            },
+            b"1231234567890123",
+            "e40a3d1505cbb15e34cf35f34c784bb0",
+        ),
+    ],
+)
 def test_idn_signature(payload, merchant_key, signature):
     assert PayUIDN.signature(payload, merchant_key) == signature
 
 
-@pytest.mark.parametrize('payu_idn, merchant, merchant_key, now, expected_payload', [
-    (PayUIPN(REFNO=1, IPN_TOTALGENERAL=1, CURRENCY='USD'), '123', b'1', 1,
-     {
-         'MERCHANT': '123',
-         'ORDER_REF': 1,
-         'ORDER_AMOUNT': 1,
-         'ORDER_CURRENCY': 'USD',
-         'IDN_DATE': 1,
-         'ORDER_HASH': '5d275f182089bab5a5351613067b95dc'
-     }),
-    (PayUIPN(), '123', b'1', 1,
-     {
-         'MERCHANT': '123',
-         'ORDER_REF': -1,
-         'ORDER_AMOUNT': 0,
-         'ORDER_CURRENCY': 'RON',
-         'IDN_DATE': 1,
-         'ORDER_HASH': '61ff18cdfe071679176f03664b4feb72'
-     })
-
-])
+@pytest.mark.parametrize(
+    "payu_idn, merchant, merchant_key, now, expected_payload",
+    [
+        (
+            PayUIPN(REFNO=1, IPN_TOTALGENERAL=1, CURRENCY="USD"),
+            "123",
+            b"1",
+            1,
+            {
+                "MERCHANT": "123",
+                "ORDER_REF": 1,
+                "ORDER_AMOUNT": 1,
+                "ORDER_CURRENCY": "USD",
+                "IDN_DATE": 1,
+                "ORDER_HASH": "5d275f182089bab5a5351613067b95dc",
+            },
+        ),
+        (
+            PayUIPN(),
+            "123",
+            b"1",
+            1,
+            {
+                "MERCHANT": "123",
+                "ORDER_REF": -1,
+                "ORDER_AMOUNT": 0,
+                "ORDER_CURRENCY": "RON",
+                "IDN_DATE": 1,
+                "ORDER_HASH": "61ff18cdfe071679176f03664b4feb72",
+            },
+        ),
+    ],
+)
 def test_idn_payload(payu_idn, merchant, merchant_key, now, expected_payload):
     idn = PayUIDN(ipn=payu_idn)
     assert dict(**idn._build_payload(merchant, merchant_key, now)) == expected_payload
 
 
 @pytest.mark.django_db
-@patch('payu.models.requests')
+@patch("payu.models.requests")
 def test_payu_idn_send_success(mocked_requests):
     mocked_requests.post.return_value = MagicMock(status_code=200, content="ok")
 
     idn = PayUIDN(ipn=G(PayUIPN))
     idn._build_payload = MagicMock(return_value="payload")
 
     idn.send()
@@ -121,17 +148,17 @@
     mocked_requests.post.assert_called_once_with(PAYU_IDN_URL, data="payload")
     assert idn.sent
     assert idn.success
     assert idn.response == "ok"
 
 
 @pytest.mark.django_db
-@patch('payu.models.requests')
+@patch("payu.models.requests")
 def test_payu_idn_send_fail(mocked_requests):
-    mocked_requests.post.side_effect = Exception('error')
+    mocked_requests.post.side_effect = Exception("error")
 
     idn = PayUIDN(ipn=G(PayUIPN))
     idn._build_payload = MagicMock(return_value="payload")
 
     idn.send()
 
     mocked_requests.post.assert_called_once_with(PAYU_IDN_URL, data="payload")
```

### Comparing `django-payu-ro-1.4.2/tests/test_send_idns_command.py` & `django-payu-ro-1.5.0/tests/test_send_idns_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,39 +18,39 @@
 
 from django.core.management import call_command
 
 from payu.models import PayUIDN
 
 
 @pytest.mark.django_db
-@patch('payu.models.requests')
+@patch("payu.models.requests")
 def test_send_idn_payu(mocked_requests):
     mocked_requests.post().status_code = 200
     mocked_requests.post().content = "ok"
 
     idns = [G(PayUIDN) for _ in range(4)]
 
     idns_args = [str(idn.pk) for idn in idns[:2]]
-    call_command('send_idns', '--idns=%s' % ','.join(idns_args))
+    call_command("send_idns", "--idns=%s" % ",".join(idns_args))
 
     for idn in idns[:2]:
         idn.refresh_from_db()
 
         assert idn.sent
         assert idn.success
         assert idn.response == "ok"
 
 
 @pytest.mark.django_db
-@patch('payu.models.requests')
+@patch("payu.models.requests")
 def test_send_idn_payu_fail(mocked_requests):
     mocked_requests.post.side_effect = Exception("error")
 
     idn = G(PayUIDN)
 
-    call_command('send_idns')
+    call_command("send_idns")
 
     idn.refresh_from_db()
 
     assert idn.sent
     assert not idn.success
     assert idn.response == "error"
```

### Comparing `django-payu-ro-1.4.2/tests/test_views.py` & `django-payu-ro-1.5.0/tests/test_views.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,43 +18,43 @@
 from django.urls import reverse
 from freezegun import freeze_time
 
 from payu.models import PayUIPN
 
 
 @pytest.mark.django_db
-@pytest.mark.parametrize('method, status_code', [
-    ('get', 200),
-    ("post", 200),
-    ('put', 405),
-    ('patch', 405),
-    ('delete', 405)
-])
+@pytest.mark.parametrize(
+    "method, status_code",
+    [("get", 200), ("post", 200), ("put", 405), ("patch", 405), ("delete", 405)],
+)
 def test_ipn_view_methods_access(method, status_code):
     client = Client()
-    assert getattr(client, method)(reverse('payu-ipn')).status_code == status_code
+    assert getattr(client, method)(reverse("payu-ipn")).status_code == status_code
 
 
 @pytest.mark.django_db
 @freeze_time("2022-01-05 11:49:52")
 def test_ipn_view_valid_payload():
     post_data = {
-        'HASH': '30dcbb067e28aee6cfefbf45e9285d7b',
-        'REFNO': '10',
-        'REFNOEXT': '1',
-        'ORDERNO': '1',
-        'ORDERSTATUS': 'TEST',
-        'PAYMETHOD_CODE': 'CCVMC',
+        "HASH": "30dcbb067e28aee6cfefbf45e9285d7b",
+        "REFNO": "10",
+        "REFNOEXT": "1",
+        "ORDERNO": "1",
+        "ORDERSTATUS": "TEST",
+        "PAYMETHOD_CODE": "CCVMC",
     }
     client = Client()
 
-    response = client.post(reverse('payu-ipn'), post_data)
-    assert response.content == b'<EPAYMENT>20220105114952|2988b8b159454b1ed380abe25e557c9e</EPAYMENT>'
+    response = client.post(reverse("payu-ipn"), post_data)
+    assert (
+        response.content
+        == b"<EPAYMENT>20220105114952|2988b8b159454b1ed380abe25e557c9e</EPAYMENT>"
+    )
 
-    ipn = PayUIPN.objects.filter(REFNO=post_data['REFNO']).first()
+    ipn = PayUIPN.objects.filter(REFNO=post_data["REFNO"]).first()
     assert ipn
 
     for field in post_data:
         assert getattr(ipn, field) == post_data[field]
 
-    assert ipn.flag_info == ''
+    assert ipn.flag_info == ""
     assert not ipn.flag
```

