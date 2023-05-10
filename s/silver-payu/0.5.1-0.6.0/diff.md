# Comparing `tmp/silver-payu-0.5.1.tar.gz` & `tmp/silver-payu-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/silver-payu-0.5.1.tar", last modified: Wed Jan  5 09:47:29 2022, max compression
+gzip compressed data, was "silver-payu-0.6.0.tar", last modified: Wed May 10 08:39:06 2023, max compression
```

## Comparing `silver-payu-0.5.1.tar` & `silver-payu-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/
--rw-r--r--   0 celo      (1000) celo      (1000)    11357 2017-12-04 10:18:00.000000 silver-payu-0.5.1/LICENSE
--rw-r--r--   0 celo      (1000) celo      (1000)      189 2021-06-28 13:54:58.000000 silver-payu-0.5.1/MANIFEST.in
--rw-r--r--   0 celo      (1000) celo      (1000)      790 2022-01-05 09:47:29.000000 silver-payu-0.5.1/PKG-INFO
--rw-r--r--   0 celo      (1000) celo      (1000)      190 2017-12-04 10:18:00.000000 silver-payu-0.5.1/README.md
--rw-r--r--   0 celo      (1000) celo      (1000)      145 2021-06-28 13:54:58.000000 silver-payu-0.5.1/requirements.test.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       63 2022-01-05 09:34:33.000000 silver-payu-0.5.1/requirements.txt
--rw-r--r--   0 celo      (1000) celo      (1000)      117 2022-01-05 09:47:29.000000 silver-payu-0.5.1/setup.cfg
--rw-r--r--   0 celo      (1000) celo      (1000)     1711 2021-06-28 13:54:58.000000 silver-payu-0.5.1/setup.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu/
--rw-r--r--   0 celo      (1000) celo      (1000)      661 2022-01-05 09:34:33.000000 silver-payu-0.5.1/silver_payu/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     6909 2020-08-17 09:47:05.000000 silver-payu-0.5.1/silver_payu/errors.py
--rw-r--r--   0 celo      (1000) celo      (1000)     3874 2021-06-28 13:54:58.000000 silver-payu-0.5.1/silver_payu/forms.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu/migrations/
--rw-r--r--   0 celo      (1000) celo      (1000)      478 2017-12-04 10:18:00.000000 silver-payu-0.5.1/silver_payu/migrations/0001_initial.py
--rw-r--r--   0 celo      (1000) celo      (1000)        0 2017-12-04 10:18:00.000000 silver-payu-0.5.1/silver_payu/migrations/__init__.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu/models/
--rw-r--r--   0 celo      (1000) celo      (1000)      628 2017-12-04 10:18:00.000000 silver-payu-0.5.1/silver_payu/models/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     1616 2021-02-05 11:47:55.000000 silver-payu-0.5.1/silver_payu/models/payment_methods.py
--rw-r--r--   0 celo      (1000) celo      (1000)    12100 2021-06-28 13:54:58.000000 silver-payu-0.5.1/silver_payu/payment_processors.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu/templates/
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu/templates/forms/
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu/templates/forms/payu_manual/
--rw-r--r--   0 celo      (1000) celo      (1000)       43 2017-12-04 10:18:00.000000 silver-payu-0.5.1/silver_payu/templates/forms/payu_manual/transaction_form.html
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu/templates/forms/payu_triggered/
--rw-r--r--   0 celo      (1000) celo      (1000)       43 2017-12-04 10:18:00.000000 silver-payu-0.5.1/silver_payu/templates/forms/payu_triggered/transaction_form.html
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu/templates/payu/
--rw-r--r--   0 celo      (1000) celo      (1000)     2433 2021-06-28 13:54:58.000000 silver-payu-0.5.1/silver_payu/templates/payu/3ds_form.html
--rw-r--r--   0 celo      (1000) celo      (1000)      164 2017-12-04 10:18:00.000000 silver-payu-0.5.1/silver_payu/templates/payu/get_billing_details_form.html
--rw-r--r--   0 celo      (1000) celo      (1000)      364 2021-06-28 13:54:58.000000 silver-payu-0.5.1/silver_payu/templates/payu/payu_lu_form.html
--rw-r--r--   0 celo      (1000) celo      (1000)      644 2021-06-28 13:54:58.000000 silver-payu-0.5.1/silver_payu/templates/payu/transaction_form.html
--rw-r--r--   0 celo      (1000) celo      (1000)     1163 2021-06-28 13:54:58.000000 silver-payu-0.5.1/silver_payu/urls.py
--rw-r--r--   0 celo      (1000) celo      (1000)     2808 2021-02-05 11:41:31.000000 silver-payu-0.5.1/silver_payu/views.py
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu.egg-info/
--rw-r--r--   0 celo      (1000) celo      (1000)      790 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu.egg-info/PKG-INFO
--rw-r--r--   0 celo      (1000) celo      (1000)      979 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu.egg-info/SOURCES.txt
--rw-r--r--   0 celo      (1000) celo      (1000)        1 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu.egg-info/dependency_links.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       43 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu.egg-info/requires.txt
--rw-r--r--   0 celo      (1000) celo      (1000)       18 2022-01-05 09:47:29.000000 silver-payu-0.5.1/silver_payu.egg-info/top_level.txt
-drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2022-01-05 09:47:29.000000 silver-payu-0.5.1/tests/
--rw-r--r--   0 celo      (1000) celo      (1000)        0 2017-12-04 10:18:00.000000 silver-payu-0.5.1/tests/__init__.py
--rw-r--r--   0 celo      (1000) celo      (1000)     2105 2021-06-28 13:54:58.000000 silver-payu-0.5.1/tests/conftest.py
--rw-r--r--   0 celo      (1000) celo      (1000)      510 2021-06-28 13:54:58.000000 silver-payu-0.5.1/tests/factories.py
--rw-r--r--   0 celo      (1000) celo      (1000)     2722 2021-06-28 13:54:58.000000 silver-payu-0.5.1/tests/fixtures.py
--rw-r--r--   0 celo      (1000) celo      (1000)     2683 2018-10-01 09:24:05.000000 silver-payu-0.5.1/tests/test_forms.py
--rw-r--r--   0 celo      (1000) celo      (1000)     5855 2021-06-28 13:54:58.000000 silver-payu-0.5.1/tests/test_models.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/
+-rw-r--r--   0 celo      (1000) celo      (1000)    11357 2022-10-05 07:17:22.000000 silver-payu-0.6.0/LICENSE
+-rw-r--r--   0 celo      (1000) celo      (1000)      189 2022-10-05 07:17:22.000000 silver-payu-0.6.0/MANIFEST.in
+-rw-r--r--   0 celo      (1000) celo      (1000)      758 2023-05-10 08:39:06.972860 silver-payu-0.6.0/PKG-INFO
+-rw-r--r--   0 celo      (1000) celo      (1000)      190 2022-10-05 07:17:22.000000 silver-payu-0.6.0/README.md
+-rw-r--r--   0 celo      (1000) celo      (1000)      188 2023-05-09 07:56:34.000000 silver-payu-0.6.0/requirements.test.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       63 2023-05-10 08:37:14.000000 silver-payu-0.6.0/requirements.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)      117 2023-05-10 08:39:06.976194 silver-payu-0.6.0/setup.cfg
+-rw-r--r--   0 celo      (1000) celo      (1000)     1704 2023-05-09 07:45:10.000000 silver-payu-0.6.0/setup.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/
+-rw-r--r--   0 celo      (1000) celo      (1000)      661 2023-05-10 08:37:34.000000 silver-payu-0.6.0/silver_payu/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     6880 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/errors.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     3878 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/forms.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/migrations/
+-rw-r--r--   0 celo      (1000) celo      (1000)      464 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/migrations/0001_initial.py
+-rw-r--r--   0 celo      (1000) celo      (1000)        0 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/migrations/__init__.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/models/
+-rw-r--r--   0 celo      (1000) celo      (1000)      628 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/models/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     1616 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/models/payment_methods.py
+-rw-r--r--   0 celo      (1000) celo      (1000)    13274 2023-05-10 08:32:28.000000 silver-payu-0.6.0/silver_payu/payment_processors.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.969527 silver-payu-0.6.0/silver_payu/templates/
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.969527 silver-payu-0.6.0/silver_payu/templates/forms/
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/templates/forms/payu_manual/
+-rw-r--r--   0 celo      (1000) celo      (1000)       43 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/forms/payu_manual/transaction_form.html
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/templates/forms/payu_triggered/
+-rw-r--r--   0 celo      (1000) celo      (1000)       43 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/forms/payu_triggered/transaction_form.html
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu/templates/payu/
+-rw-r--r--   0 celo      (1000) celo      (1000)     2433 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/payu/3ds_form.html
+-rw-r--r--   0 celo      (1000) celo      (1000)      164 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/payu/get_billing_details_form.html
+-rw-r--r--   0 celo      (1000) celo      (1000)      364 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/payu/payu_lu_form.html
+-rw-r--r--   0 celo      (1000) celo      (1000)      644 2022-10-05 07:17:22.000000 silver-payu-0.6.0/silver_payu/templates/payu/transaction_form.html
+-rw-r--r--   0 celo      (1000) celo      (1000)     1188 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/urls.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     2831 2023-05-09 07:45:10.000000 silver-payu-0.6.0/silver_payu/views.py
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/silver_payu.egg-info/
+-rw-r--r--   0 celo      (1000) celo      (1000)      758 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/PKG-INFO
+-rw-r--r--   0 celo      (1000) celo      (1000)      979 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/SOURCES.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)        1 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/dependency_links.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       43 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/requires.txt
+-rw-r--r--   0 celo      (1000) celo      (1000)       18 2023-05-10 08:39:06.000000 silver-payu-0.6.0/silver_payu.egg-info/top_level.txt
+drwxr-xr-x   0 celo      (1000) celo      (1000)        0 2023-05-10 08:39:06.972860 silver-payu-0.6.0/tests/
+-rw-r--r--   0 celo      (1000) celo      (1000)        0 2022-10-05 07:17:22.000000 silver-payu-0.6.0/tests/__init__.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     2159 2023-05-09 07:54:40.000000 silver-payu-0.6.0/tests/conftest.py
+-rw-r--r--   0 celo      (1000) celo      (1000)      510 2023-05-09 07:45:10.000000 silver-payu-0.6.0/tests/factories.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     2794 2023-05-10 08:26:50.000000 silver-payu-0.6.0/tests/fixtures.py
+-rw-r--r--   0 celo      (1000) celo      (1000)     2991 2023-05-09 07:45:10.000000 silver-payu-0.6.0/tests/test_forms.py
+-rw-r--r--   0 celo      (1000) celo      (1000)    10780 2023-05-10 08:25:09.000000 silver-payu-0.6.0/tests/test_models.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `silver-payu-0.5.1/LICENSE` & `silver-payu-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `silver-payu-0.5.1/PKG-INFO` & `silver-payu-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: silver-payu
-Version: 0.5.1
-Summary: UNKNOWN
+Version: 0.6.0
 Home-page: https://github.com/silverapp/silver-payu
 Author: Presslabs
 Author-email: ping@presslabs.com
 License: Apache 2.0
-Description: # silver-payu [![Build Status](https://travis-ci.org/silverapp/silver-payu.svg?branch=master)](https://travis-ci.org/silverapp/silver-payu)
-        
-        PayU Payment Processor implementation for silver
-        
 Keywords: django,app,reusable,billing,invoicing,api
 Platform: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+# silver-payu [![Build Status](https://travis-ci.org/silverapp/silver-payu.svg?branch=master)](https://travis-ci.org/silverapp/silver-payu)
+
+PayU Payment Processor implementation for silver
```

### Comparing `silver-payu-0.5.1/setup.py` & `silver-payu-0.6.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,42 +18,40 @@
 import os
 
 from setuptools import setup, find_packages
 
 from silver_payu import __version__ as version
 
 
-install_requires = [
-    'django-payu-ro>=1.4.1',
-    'django-ipware>=3.0.2'
-]
+install_requires = ["django-payu-ro>=1.4.1", "django-ipware>=3.0.2"]
 
 
 def read(fname):
     try:
         return open(os.path.join(os.path.dirname(__file__), fname)).read()
     except IOError:
-        return ''
+        return ""
+
 
 setup(
     name="silver-payu",
     version=version,
-    description=read('DESCRIPTION'),
-    long_description=read('README.md'),
-    license='Apache 2.0',
-    platforms=['OS Independent'],
-    keywords='django, app, reusable, billing, invoicing, api',
-    author='Presslabs',
-    author_email='ping@presslabs.com',
-    url='https://github.com/silverapp/silver-payu',
+    description=read("DESCRIPTION"),
+    long_description=read("README.md"),
+    license="Apache 2.0",
+    platforms=["OS Independent"],
+    keywords="django, app, reusable, billing, invoicing, api",
+    author="Presslabs",
+    author_email="ping@presslabs.com",
+    url="https://github.com/silverapp/silver-payu",
     packages=find_packages(),
     include_package_data=True,
     install_requires=install_requires,
     classifiers=[
-        'Environment :: Web Environment',
-        'Framework :: Django :: 3.1',
-        'Framework :: Django :: 3.2',
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.7'
-    ]
+        "Environment :: Web Environment",
+        "Framework :: Django :: 3.1",
+        "Framework :: Django :: 3.2",
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3.7",
+    ],
 )
```

### Comparing `silver-payu-0.5.1/silver_payu/__init__.py` & `silver-payu-0.6.0/silver_payu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 #
 
-__author__ = 'Presslabs'
-__version__ = '0.5.1'
+__author__ = "Presslabs"
+__version__ = "0.6.0"
```

### Comparing `silver-payu-0.5.1/silver_payu/errors.py` & `silver-payu-0.6.0/silver_payu/errors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,248 +1,209 @@
 TOKEN_ERROR_CODES = {
-    '300': {
-        'silver_code': 'default',
-        'reason': 'The REF_NO specified is not a valid transaction',
+    "300": {
+        "silver_code": "default",
+        "reason": "The REF_NO specified is not a valid transaction",
     },
-
-    '400': {
-        'silver_code': 'default',
-        'reason': 'The METHOD variable needs to have one of the following values:TOKEN_NEWSALE, TOKEN_CANCEL, TOKEN_GETINFO',
+    "400": {
+        "silver_code": "default",
+        "reason": "The METHOD variable needs to have one of the following values:TOKEN_NEWSALE, TOKEN_CANCEL, TOKEN_GETINFO",
     },
-
-    '500': {
-        'silver_code': 'default',
-        'reason': 'The value of TIMESTAMP differs too much from the current time. Check your system clock and ensure that TIMESTAMP is in UTC timezone.',
+    "500": {
+        "silver_code": "default",
+        "reason": "The value of TIMESTAMP differs too much from the current time. Check your system clock and ensure that TIMESTAMP is in UTC timezone.",
     },
-
-    '600': {
-        'silver_code': 'default',
-        'reason': 'Make sure that your MerchantID is the same one found in yourPayU Control Panel',
+    "600": {
+        "silver_code": "default",
+        "reason": "Make sure that your MerchantID is the same one found in yourPayU Control Panel",
     },
-
-    '601': {
-        'silver_code': 'insufficient_funds',
-        'reason': 'The credit card used has insufficient funds available.',
+    "601": {
+        "silver_code": "insufficient_funds",
+        "reason": "The credit card used has insufficient funds available.",
     },
-
-    '602': {
-        'silver_code': 'expired_card',
-        'reason': 'The credit card used is expired',
+    "602": {
+        "silver_code": "expired_card",
+        "reason": "The credit card used is expired",
     },
-
-    '603': {
-        'silver_code': 'default',
-        'reason': 'Temporary processing error. Retrying after a few minutes should work.',
+    "603": {
+        "silver_code": "default",
+        "reason": "Temporary processing error. Retrying after a few minutes should work.",
     },
-
-    '604': {
-        'silver_code': 'invalid_card',
-        'reason': 'The credit card used is invalid.',
+    "604": {
+        "silver_code": "invalid_card",
+        "reason": "The credit card used is invalid.",
     },
-
-    '605': {
-        'silver_code': 'default',
-        'reason': 'General system error. Retrying after a few minutes should work but if it\'s not please contact our support team.',
+    "605": {
+        "silver_code": "default",
+        "reason": "General system error. Retrying after a few minutes should work but if it's not please contact our support team.",
     },
-
-    '606': {
-        'silver_code': 'transaction_declined_by_bank',
-        'reason': 'Invalid Transaction error specified by the credit card company.',
+    "606": {
+        "silver_code": "transaction_declined_by_bank",
+        "reason": "Invalid Transaction error specified by the credit card company.",
     },
-
-    '607': {
-        'silver_code': 'default',
-        'reason': 'The bank is still processing the transaction, check order status using IOS webservice.',
+    "607": {
+        "silver_code": "default",
+        "reason": "The bank is still processing the transaction, check order status using IOS webservice.",
     },
-
-    '1200': {
-        'silver_code': 'default',
-        'reason': 'There is a problem with your SIGN variable. Please check your code.',
+    "1200": {
+        "silver_code": "default",
+        "reason": "There is a problem with your SIGN variable. Please check your code.",
     },
-
-    '1300': {
-        'silver_code': 'default',
-        'reason': 'The REF_NO you have specified is not valid. Please check the value.',
+    "1300": {
+        "silver_code": "default",
+        "reason": "The REF_NO you have specified is not valid. Please check the value.",
     },
-
-    '1500': {
-        'silver_code': 'default',
-        'reason': 'Invalid Token command for the REF_NO you have specified.',
+    "1500": {
+        "silver_code": "default",
+        "reason": "Invalid Token command for the REF_NO you have specified.",
     },
-
-    '1600': {
-        'silver_code': 'default',
-        'reason': 'Invalid External Ref No',
+    "1600": {
+        "silver_code": "default",
+        "reason": "Invalid External Ref No",
     },
-
-    '1900': {
-        'silver_code': 'default',
-        'reason': 'The AMOUNT value should be a positive number, either integer or a float.',
+    "1900": {
+        "silver_code": "default",
+        "reason": "The AMOUNT value should be a positive number, either integer or a float.",
     },
-
-    '2000': {
-        'silver_code': 'default',
-        'reason': 'You have exceeded the maximum amount limit for your terminal. Please try again in a few minutes.',
+    "2000": {
+        "silver_code": "default",
+        "reason": "You have exceeded the maximum amount limit for your terminal. Please try again in a few minutes.",
     },
-
-    '2100': {
-        'silver_code': 'default',
-        'reason': 'CURRENCY variable has an unsupported or invalid value.',
+    "2100": {
+        "silver_code": "default",
+        "reason": "CURRENCY variable has an unsupported or invalid value.",
     },
-
-    '2200': {
-        'silver_code': 'expired_payment_method',
-        'reason': 'Operation was not performed because the token has expired.',
+    "2200": {
+        "silver_code": "expired_payment_method",
+        "reason": "Operation was not performed because the token has expired.",
     },
-
-    '2300': {
-        'silver_code': 'expired_payment_method',
-        'reason': 'Operation was not performed because the token has expired.',
+    "2300": {
+        "silver_code": "expired_payment_method",
+        "reason": "Operation was not performed because the token has expired.",
     },
-
-    '2401': {
-        'silver_code': 'default',
-        'reason': 'BILL_LNAME field is mandatory',
+    "2401": {
+        "silver_code": "default",
+        "reason": "BILL_LNAME field is mandatory",
     },
-
-    '2402': {
-        'silver_code': 'default',
-        'reason': 'BILL_FNAME field is mandatory',
+    "2402": {
+        "silver_code": "default",
+        "reason": "BILL_FNAME field is mandatory",
     },
-
-    '2403': {
-        'silver_code': 'default',
-        'reason': 'BILL_EMAIL field is mandatory',
+    "2403": {
+        "silver_code": "default",
+        "reason": "BILL_EMAIL field is mandatory",
     },
-
-    '2404': {
-        'silver_code': 'default',
-        'reason': 'BILL_EMAIL field is not a valid e-mail',
+    "2404": {
+        "silver_code": "default",
+        "reason": "BILL_EMAIL field is not a valid e-mail",
     },
-
-    '2405': {
-        'silver_code': 'default',
-        'reason': 'BILL_PHONE field is mandatory',
+    "2405": {
+        "silver_code": "default",
+        "reason": "BILL_PHONE field is mandatory",
     },
-
-    '2406': {
-        'silver_code': 'default',
-        'reason': 'BILL_ADDRESS field is mandatory',
+    "2406": {
+        "silver_code": "default",
+        "reason": "BILL_ADDRESS field is mandatory",
     },
-
-    '2407': {
-        'silver_code': 'default',
-        'reason': 'BILL_CITY field is mandatory',
+    "2407": {
+        "silver_code": "default",
+        "reason": "BILL_CITY field is mandatory",
     },
-
-    '2408': {
-        'silver_code': 'default',
-        'reason': 'DELIVERY_LNAME field is mandatory',
+    "2408": {
+        "silver_code": "default",
+        "reason": "DELIVERY_LNAME field is mandatory",
     },
-
-    '2409': {
-        'silver_code': 'default',
-        'reason': 'DELIVERY_FNAME field is mandatory',
+    "2409": {
+        "silver_code": "default",
+        "reason": "DELIVERY_FNAME field is mandatory",
     },
-
-    '2410': {
-        'silver_code': 'default',
-        'reason': 'DELIVERY_PHONE field is mandatory',
+    "2410": {
+        "silver_code": "default",
+        "reason": "DELIVERY_PHONE field is mandatory",
     },
-
-    '2411': {
-        'silver_code': 'default',
-        'reason': 'DELIVERY_ADDRESS field is mandatory',
+    "2411": {
+        "silver_code": "default",
+        "reason": "DELIVERY_ADDRESS field is mandatory",
     },
-
-    '2412': {
-        'silver_code': 'default',
-        'reason': 'DELIVERY_CITY field is mandatory',
+    "2412": {
+        "silver_code": "default",
+        "reason": "DELIVERY_CITY field is mandatory",
     },
-
-    '2413': {
-        'silver_code': 'default',
-        'reason': 'DELIVERY_EMAIL field is not a valid e-mail',
+    "2413": {
+        "silver_code": "default",
+        "reason": "DELIVERY_EMAIL field is not a valid e-mail",
     },
-
-    '2414': {
-        'silver_code': 'default',
-        'reason': 'BILL_COUNTRYCODE field is not a valid ISO 3166-1 alpha-2country code',
+    "2414": {
+        "silver_code": "default",
+        "reason": "BILL_COUNTRYCODE field is not a valid ISO 3166-1 alpha-2country code",
     },
-
-    '2415': {
-        'silver_code': 'default',
-        'reason': 'DELIVERY_COUNTRYCODE field is not a valid ISO 3166-1 alpha-2country code',
+    "2415": {
+        "silver_code": "default",
+        "reason": "DELIVERY_COUNTRYCODE field is not a valid ISO 3166-1 alpha-2country code",
     },
-
-    '3000': {
-        'silver_code': 'default',
-        'reason': 'Invalid number of installments selected',
+    "3000": {
+        "silver_code": "default",
+        "reason": "Invalid number of installments selected",
     },
-
-    '3100': {
-        'silver_code': 'default',
-        'reason': 'Token is already persistent',
+    "3100": {
+        "silver_code": "default",
+        "reason": "Token is already persistent",
     },
-
-    '3101': {
-        'silver_code': 'expired_payment_method',
-        'reason': 'Token has expired',
+    "3101": {
+        "silver_code": "expired_payment_method",
+        "reason": "Token has expired",
     },
-
-    '3200': {
-        'silver_code': 'default',
-        'reason': 'Token usage on marketplace orders is restricted on this protocol',
+    "3200": {
+        "silver_code": "default",
+        "reason": "Token usage on marketplace orders is restricted on this protocol",
     },
-
-    '4000': {
-        'silver_code': 'default',
-        'reason': 'Please check if the card scheme used to make the original transaction is still enabled for that merchant.',
+    "4000": {
+        "silver_code": "default",
+        "reason": "Please check if the card scheme used to make the original transaction is still enabled for that merchant.",
     },
 }
 
 ALU_ERROR_CODES = {
     "ALREADY_AUTHORIZED": {
         "silver_code": "default",
-        "reason": "Tried to place a new order with the same ORDER_REF and HASH as previous one."
+        "reason": "Tried to place a new order with the same ORDER_REF and HASH as previous one.",
     },
     "AUTHORIZATION_FAILED": {
         "silver_code": "default",
-        "reason": "The payment was not authorized."
+        "reason": "The payment was not authorized.",
     },
     "INVALID_CUSTOMER_INFO": {
         "silver_code": "default",
-        "reason": "Required data from the Shopper is missing or is malformed."
+        "reason": "Required data from the Shopper is missing or is malformed.",
     },
     "INVALID_PAYMENT_INFO": {
         "silver_code": "default",
-        "reason": "Card data is not correct."
+        "reason": "Card data is not correct.",
     },
     "INVALID_ACCOUNT": {
         "silver_code": "default",
-        "reason": "The Merchant name is not correct."
+        "reason": "The Merchant name is not correct.",
     },
     "INVALID_PAYMENT_METHOD_CODE": {
         "silver_code": "default",
-        "reason": "Payment method code is NOT recognized."
+        "reason": "Payment method code is NOT recognized.",
     },
     "INVALID_CURRENCY": {
         "silver_code": "default",
-        "reason": "Payment currency is not recognized."
+        "reason": "Payment currency is not recognized.",
     },
     "REQUEST_EXPIRED": {
         "silver_code": "default",
-        "reason": "The request has expired based on provided ORDER_DATE."
+        "reason": "The request has expired based on provided ORDER_DATE.",
     },
     "HASH_MISMATCH": {
         "silver_code": "default",
-        "reason": "Hash sent by the Merchant does not match the hash calculated by PayU."
+        "reason": "Hash sent by the Merchant does not match the hash calculated by PayU.",
     },
     "WRONG_VERSION": {
         "silver_code": "default",
-        "reason": "ALU version sent by the Merchant does not exist."
+        "reason": "ALU version sent by the Merchant does not exist.",
     },
     "INVALID_CC_TOKEN": {
         "silver_code": "default",
-        "reason": "CC_TOKEN sent by the Merchant is not valid."
+        "reason": "CC_TOKEN sent by the Merchant is not valid.",
     },
 }
```

### Comparing `silver-payu-0.5.1/silver_payu/forms.py` & `silver-payu-0.6.0/silver_payu/forms.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,108 +9,119 @@
 
 from silver.payment_processors.forms import GenericTransactionForm
 from silver.utils.payments import get_payment_complete_url
 from silver.utils.international import countries
 
 
 class PayUTransactionFormBase(GenericTransactionForm, PayULiveUpdateForm):
-    def __init__(self, payment_method, transaction, billing_details,
-                 request=None, *args, **kwargs):
+    def __init__(
+        self,
+        payment_method,
+        transaction,
+        billing_details,
+        request=None,
+        *args,
+        **kwargs,
+    ):
+        kwargs["initial"] = self._build_form_body(transaction, request)
+        kwargs["initial"].update(billing_details)
 
-        kwargs['initial'] = self._build_form_body(transaction, request)
-        kwargs['initial'].update(billing_details)
-
-        super(PayUTransactionFormBase, self).__init__(payment_method,
-                                                      transaction,
-                                                      request, **kwargs)
+        super(PayUTransactionFormBase, self).__init__(
+            payment_method, transaction, request, **kwargs
+        )
 
     def _build_form_body(self, transaction, request) -> Dict[str, str]:
         return {
-            'ORDER_REF': str(transaction.uuid),
-            'ORDER_DATE':  datetime.now(pytz.UTC).strftime('%Y-%m-%d %H:%M:%S'),
-            'PRICES_CURRENCY': transaction.currency,
-            'CURRENCY': transaction.currency,
-            'PAY_METHOD': 'CCVISAMC',
-            'AUTOMODE': '1',
-            'BACK_REF': get_payment_complete_url(transaction, request),
-            'ORDER': self._get_order(transaction)
+            "ORDER_REF": str(transaction.uuid),
+            "ORDER_DATE": datetime.now(pytz.UTC).strftime("%Y-%m-%d %H:%M:%S"),
+            "PRICES_CURRENCY": transaction.currency,
+            "CURRENCY": transaction.currency,
+            "PAY_METHOD": "CCVISAMC",
+            "AUTOMODE": "1",
+            "BACK_REF": get_payment_complete_url(transaction, request),
+            "ORDER": self._get_order(transaction),
         }
 
     def _get_order(self, transaction) -> List[Dict[str, str]]:
         document = transaction.document
-        product_name = f'Payment for {document.kind} {document.series}-{document.number}'
+        product_name = (
+            f"Payment for {document.kind} {document.series}-{document.number}"
+        )
 
-        return [{
-            'PNAME': product_name,
-            'PCODE': f'{document.series}-{document.number}',
-            'PRICE': str(transaction.amount),
-            'PRICE_TYPE': 'GROSS',
-            'VAT': str(document.sales_tax_percent or '0')
-        }]
+        return [
+            {
+                "PNAME": product_name,
+                "PCODE": f"{document.series}-{document.number}",
+                "PRICE": str(transaction.amount),
+                "PRICE_TYPE": "GROSS",
+                "VAT": str(document.sales_tax_percent or "0"),
+            }
+        ]
 
 
 class PayUTransactionFormManual(PayUTransactionFormBase):
     pass
 
 
 class PayUTransactionFormTriggered(PayUTransactionFormBase):
     def _build_form_body(self, transaction, request):
         form_body = super(PayUTransactionFormTriggered, self)._build_form_body(
             transaction, request
         )
 
-        form_body['LU_ENABLE_TOKEN'] = '1'
+        form_body["LU_ENABLE_TOKEN"] = "1"
 
         return form_body
 
 
 class PayUTransactionFormTriggeredV2(PayUTransactionFormBase):
     def _build_form_body(self, transaction, request):
         form_body = super(PayUTransactionFormTriggeredV2, self)._build_form_body(
             transaction, request
         )
 
-        form_body['LU_ENABLE_TOKEN'] = '1'
-        form_body['LU_TOKEN_TYPE'] = 'PAY_ON_TIME'
+        form_body["LU_ENABLE_TOKEN"] = "1"
+        form_body["LU_TOKEN_TYPE"] = "PAY_ON_TIME"
 
         return form_body
 
 
 class PayUBillingForm(GenericTransactionForm):
     email = forms.EmailField()
     first_name = forms.CharField()
     last_name = forms.CharField()
     phone = forms.CharField()
     city = forms.CharField()
     country = forms.ChoiceField(choices=countries)
 
-    def __init__(self, payment_method, transaction,
-                 request=None, data=None, *args, **kwargs):
-
+    def __init__(
+        self, payment_method, transaction, request=None, data=None, *args, **kwargs
+    ):
         if not data:
             data = self._build_form_body(payment_method.customer)
 
-        super(PayUBillingForm, self).__init__(payment_method, transaction,
-                                              request, data, **kwargs)
+        super(PayUBillingForm, self).__init__(
+            payment_method, transaction, request, data, **kwargs
+        )
 
     def to_payu_billing(self):
         data = self.cleaned_data
         return {
-            'BILL_FNAME': data['first_name'],
-            'BILL_LNAME': data['last_name'],
-            'BILL_EMAIL': data['email'],
-            'BILL_PHONE': data['phone'],
-            'BILL_CITY': data['city'],
-            'BILL_COUNTRYCODE': data['country']
+            "BILL_FNAME": data["first_name"],
+            "BILL_LNAME": data["last_name"],
+            "BILL_EMAIL": data["email"],
+            "BILL_PHONE": data["phone"],
+            "BILL_CITY": data["city"],
+            "BILL_COUNTRYCODE": data["country"],
         }
 
     def _build_form_body(self, customer):
         form_body = {
-            'first_name': customer.first_name,
-            'last_name': customer.last_name,
-            'email': customer.email,
-            'phone': customer.phone or '',
-            'country': customer.country,
-            'city': customer.city
+            "first_name": customer.first_name,
+            "last_name": customer.last_name,
+            "email": customer.email,
+            "phone": customer.phone or "",
+            "country": customer.country,
+            "city": customer.city,
         }
 
         return form_body
```

### Comparing `silver-payu-0.5.1/silver_payu/models/__init__.py` & `silver-payu-0.6.0/silver_payu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `silver-payu-0.5.1/silver_payu/models/payment_methods.py` & `silver-payu-0.6.0/silver_payu/models/payment_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,32 +20,32 @@
 
 class PayUPaymentMethod(PaymentMethod):
     class Meta:
         proxy = True
 
     @property
     def token(self):
-        return self.decrypt_data(self.data.get('token'))
+        return self.decrypt_data(self.data.get("token"))
 
     @token.setter
     def token(self, value):
-        self.data['token'] = self.encrypt_data(value)
+        self.data["token"] = self.encrypt_data(value)
 
     @property
     def archived_customer(self):
-        raw_customer = self.data.get('archived_customer', '')
-        return json.loads(self.decrypt_data(raw_customer) or '{}')
+        raw_customer = self.data.get("archived_customer", "")
+        return json.loads(self.decrypt_data(raw_customer) or "{}")
 
     @archived_customer.setter
     def archived_customer(self, value):
         raw_customer = json.dumps(value)
-        self.data['archived_customer'] = self.encrypt_data(raw_customer)
+        self.data["archived_customer"] = self.encrypt_data(raw_customer)
 
     @property
     def threeds_data(self):
-        raw_data = self.data.get('3ds_data', '')
-        return json.loads(self.decrypt_data(raw_data) or '{}')
+        raw_data = self.data.get("3ds_data", "")
+        return json.loads(self.decrypt_data(raw_data) or "{}")
 
     @threeds_data.setter
     def threeds_data(self, value):
         raw_data = json.dumps(value)
-        self.data['3ds_data'] = self.encrypt_data(raw_data)
+        self.data["3ds_data"] = self.encrypt_data(raw_data)
```

### Comparing `silver-payu-0.5.1/silver_payu/payment_processors.py` & `silver-payu-0.6.0/silver_payu/payment_processors.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,58 +10,70 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import json
 from xml.etree import ElementTree
 
+from django.conf import settings
 from django.db import transaction as django_transaction
 from django.dispatch import receiver
 from django_fsm import TransitionNotAllowed
 from payu.payments import ALUPayment, TokenPayment
 from payu.signals import payment_authorized, alu_token_created, payment_completed
 from silver.models import Transaction
 from silver.payment_processors import PaymentProcessorBase
-from silver.payment_processors.mixins import (TriggeredProcessorMixin,
-                                              ManualProcessorMixin)
+from silver.payment_processors.mixins import (
+    TriggeredProcessorMixin,
+    ManualProcessorMixin,
+)
 
 from silver_payu.errors import TOKEN_ERROR_CODES, ALU_ERROR_CODES
-from silver_payu.forms import (PayUTransactionFormManual,
-                               PayUTransactionFormTriggered, PayUBillingForm,
-                               PayUTransactionFormTriggeredV2)
+from silver_payu.forms import (
+    PayUTransactionFormManual,
+    PayUTransactionFormTriggered,
+    PayUBillingForm,
+    PayUTransactionFormTriggeredV2,
+)
 from silver_payu.models import PayUPaymentMethod
 from silver_payu.views import PayUTransactionView
 
 
 class PayUBase(PaymentProcessorBase):
     payment_method_class = PayUPaymentMethod
     transaction_view_class = PayUTransactionView
-    allowed_currencies = ('RON', 'USD', 'EUR')
+    allowed_currencies = ("RON", "USD", "EUR")
 
     _has_been_setup = False
 
     def get_form(self, transaction, request):
-        form = PayUBillingForm(payment_method=transaction.payment_method,
-                               transaction=transaction, request=request,
-                               data=request.POST)
+        form = PayUBillingForm(
+            payment_method=transaction.payment_method,
+            transaction=transaction,
+            request=request,
+            data=request.POST,
+        )
 
         if form.is_valid():
             if not transaction.payment_method.archived_customer:
                 customer = transaction.document.customer
                 address = f"{customer.address_1} {customer.address_2}"
 
                 archived_customer = form.to_payu_billing()
-                archived_customer['BILL_ADDRESS'] = address
+                archived_customer["BILL_ADDRESS"] = address
 
                 transaction.payment_method.archived_customer = archived_customer
                 transaction.payment_method.save()
 
-            form = self.form_class(payment_method=transaction.payment_method,
-                                   transaction=transaction, request=request,
-                                   billing_details=form.to_payu_billing())
+            form = self.form_class(
+                payment_method=transaction.payment_method,
+                transaction=transaction,
+                request=request,
+                billing_details=form.to_payu_billing(),
+            )
 
         return form
 
     def refund_transaction(self, transaction, payment_method=None):
         pass
 
     def void_transaction(self, transaction, payment_method=None):
@@ -69,36 +81,37 @@
 
     def handle_transaction_response(self, transaction, request):
         with django_transaction.atomic():
             Transaction.objects.select_for_update().filter(pk=transaction.pk).get()
             transaction.refresh_from_db()
 
             try:
-                if request.GET.get('ctrl', None):
-                    transaction.data['ctrl'] = request.GET['ctrl']
+                if request.GET.get("ctrl", None):
+                    transaction.data["ctrl"] = request.GET["ctrl"]
                     transaction.process()
                 else:
-                    error = request.GET.get('err', None) or 'Unknown error'
+                    error = request.GET.get("err", None) or "Unknown error"
                     transaction.fail(fail_reason=error)
             except TransitionNotAllowed:
                 pass
 
             transaction.save()
 
 
 class PayUManual(PayUBase, ManualProcessorMixin):
-    template_slug = 'payu_manual'
+    template_slug = "payu_manual"
     form_class = PayUTransactionFormManual
 
 
 class PayUTriggered(PayUBase, TriggeredProcessorMixin):
     """
     Uses TokenV1 API for recurrent payments.
     """
-    template_slug = 'payu_triggered'
+
+    template_slug = "payu_triggered"
     form_class = PayUTransactionFormTriggered
 
     def execute_transaction(self, transaction):
         """
         :param transaction: A PayU transaction in Initial or Pending state.
         :return: True on success, False on failure.
         """
@@ -115,25 +128,25 @@
         try:
             delivery_details = {
                 "DELIVERY_ADDRESS": billing_details["BILL_ADDRESS"],
                 "DELIVERY_CITY": billing_details["BILL_CITY"],
                 "DELIVERY_EMAIL": billing_details["BILL_EMAIL"],
                 "DELIVERY_FNAME": billing_details["BILL_FNAME"],
                 "DELIVERY_LNAME": billing_details["BILL_LNAME"],
-                "DELIVERY_PHONE": billing_details["BILL_PHONE"]
+                "DELIVERY_PHONE": billing_details["BILL_PHONE"],
             }
         except KeyError as error:
-            transaction.fail(fail_reason=f'Invalid customer details. [{error}]')
+            transaction.fail(fail_reason=f"Invalid customer details. [{error}]")
             transaction.save()
             return False
 
         payment_details = {
             "AMOUNT": str(transaction.amount),
             "CURRENCY": str(transaction.currency),
-            "EXTERNAL_REF": str(transaction.uuid)
+            "EXTERNAL_REF": str(transaction.uuid),
         }
         payment_details.update(billing_details)
         payment_details.update(delivery_details)
 
         payment = TokenPayment(payment_details, token)
 
         try:
@@ -158,29 +171,30 @@
             transaction.fail(fail_reason=str(error))
 
         transaction.save()
 
         return False
 
     def _parse_response_error(self, payu_response):
-        if not isinstance(payu_response, dict) or 'code' not in payu_response:
-            return 'default', f'Missing payu error code.({payu_response})'
+        if not isinstance(payu_response, dict) or "code" not in payu_response:
+            return "default", f"Missing payu error code.({payu_response})"
 
-        if str(payu_response['code']) in TOKEN_ERROR_CODES:
-            error = TOKEN_ERROR_CODES[str(payu_response['code'])]
-            return error['silver_code'], error['reason']
+        if str(payu_response["code"]) in TOKEN_ERROR_CODES:
+            error = TOKEN_ERROR_CODES[str(payu_response["code"])]
+            return error["silver_code"], error["reason"]
 
-        return 'default', f'Unknown error code {payu_response["code"]}'
+        return "default", f'Unknown error code {payu_response["code"]}'
 
 
 class PayUTriggeredV2(PayUBase, TriggeredProcessorMixin):
     """
     Uses ALUPaymentV3 API for recurrent payments.
     """
-    template_slug = 'payu_triggered'
+
+    template_slug = "payu_triggered"
     form_class = PayUTransactionFormTriggeredV2
 
     def execute_transaction(self, transaction):
         """
         :param transaction: A PayU transaction in Initial or Pending state.
         :return: True on success, False on failure.
         """
@@ -198,104 +212,147 @@
         try:
             delivery_details = {
                 "DELIVERY_ADDRESS": customer_details["BILL_ADDRESS"],
                 "DELIVERY_CITY": customer_details["BILL_CITY"],
                 "DELIVERY_EMAIL": customer_details["BILL_EMAIL"],
                 "DELIVERY_FNAME": customer_details["BILL_FNAME"],
                 "DELIVERY_LNAME": customer_details["BILL_LNAME"],
-                "DELIVERY_PHONE": customer_details["BILL_PHONE"]
+                "DELIVERY_PHONE": customer_details["BILL_PHONE"],
             }
         except KeyError as error:
-            transaction.fail(fail_reason=f'Invalid customer details. [{error}]')
+            transaction.fail(fail_reason=f"Invalid customer details. [{error}]")
             transaction.save()
             return False
 
         payment_details = {
             "PRICES_CURRENCY": str(transaction.currency),
             "ORDER_REF": str(transaction.uuid),
             "PAY_METHOD": "CCVISAMC",
         }
 
         if transaction.document:
             pname = "{provider} {doc_type} {doc_number}".format(
                 doc_type=transaction.document.kind,
                 doc_number=transaction.document.series_number,
-                provider=transaction.provider.name
+                provider=transaction.provider.name,
             )
 
             vat = str(int(transaction.document.sales_tax_percent or 0))
             price_type = "GROSS"  # (VAT included)
         else:
             pname = f"Payment for {transaction.provider.name}"
 
             vat = "0"
             price_type = "NET"  # (VAT will be added by PayU)
 
         order_details = [
             {
-                'PNAME': pname,
-                'PCODE': str(transaction.uuid),
-                'PRICE': str(transaction.amount),
-                'VAT': vat,
-                'PRICE_TYPE': price_type,
-                'QTY': '1',
+                "PNAME": pname,
+                "PCODE": str(transaction.uuid),
+                "PRICE": str(transaction.amount),
+                "VAT": vat,
+                "PRICE_TYPE": price_type,
+                "QTY": "1",
             }
         ]
 
         payment_details.update(customer_details)
         payment_details.update(delivery_details)
         payment_details["ORDER"] = order_details
 
-        payment = ALUPayment(payment_details, token,
-                             stored_credentials_use_type="merchant",
-                             threeds_data=payment_method.threeds_data)
+        payment = ALUPayment(
+            payment_details,
+            token,
+            stored_credentials_use_type="merchant",
+            threeds_data=payment_method.threeds_data,
+        )
 
         try:
             result = payment.pay()
         except Exception as error:
             transaction.fail(fail_reason=str(error))
+            self._log_request_response(transaction, payment)
+
             transaction.save()
+
             return False
 
-        return self._parse_result(transaction, result)
+        return self._parse_result(transaction, result, payment)
 
-    def _parse_result(self, transaction, result):
+    def _log_request_response(self, transaction, payment):
+        if not payment:
+            return
+
+        request = getattr(payment, "_request", {})
+        redacted_fields = ["CC_TOKEN", "CC_CVV"]
+
+        if getattr(settings, "SILVER_PAYU_REDACT_PII", False):
+            redacted_fields += [
+                "BROWSER_IP",
+                "BILL_ADDRESS",
+                "BILL_CITY",
+                "BILL_PHONE",
+                "BILL_FNAME",
+                "BILL_LNAME",
+                "BILL_EMAIL",
+            ]
+
+        for field in redacted_fields:
+            if request.get(field):
+                request[field] = "[REDACTED]"
+
+        response = getattr(payment, "_response", "")
+        if isinstance(response, bytes):
+            response = response.decode("utf-8")
+
+        transaction.data.update(
+            {
+                "_request": str(request),
+                "_response": str(response),
+            }
+        )
+
+    def _parse_result(self, transaction, result, payment=None):
         try:
             element = ElementTree.fromstring(result)
             status = element.find("STATUS").text
-            return_code = element.find('RETURN_CODE').text
+            return_code = element.find("RETURN_CODE").text
 
             if status == "SUCCESS":
                 return True
 
             error_code, error_reason = self._parse_response_error(return_code)
-            transaction.data = {
-                "status": status,
-                "message": error_reason,
-                "return_code": return_code,
-            }
+            transaction.data.update(
+                {
+                    "status": status,
+                    "message": error_reason,
+                    "return_code": return_code,
+                }
+            )
 
             return_message = element.find("RETURN_MESSAGE")
             if return_message is not None:
                 transaction.data["return_message"] = return_message.text
 
+            self._log_request_response(transaction, payment)
             transaction.fail(fail_code=error_code, fail_reason=error_reason)
         except ValueError as error:
+            self._log_request_response(transaction, payment)
             transaction.fail(fail_reason=str(error))
 
         transaction.save()
 
         return False
 
     def _parse_response_error(self, return_code):
         if str(return_code) in ALU_ERROR_CODES:
             error = ALU_ERROR_CODES[str(return_code)]
-            return error['silver_code'], error['reason']
+            return error["silver_code"], error["reason"]
 
-        return 'default', f'Unknown error code {return_code}'
+        return "default", f"Unknown error code {return_code}"
 
 
 @receiver([payment_authorized, payment_completed])
 def payu_ipn_received(sender, **kwargs):
     transaction = Transaction.objects.get(uuid=sender.REFNOEXT)
 
     try:
```

### Comparing `silver-payu-0.5.1/silver_payu/templates/payu/3ds_form.html` & `silver-payu-0.6.0/silver_payu/templates/payu/3ds_form.html`

 * *Files identical despite different names*

### Comparing `silver-payu-0.5.1/silver_payu/templates/payu/transaction_form.html` & `silver-payu-0.6.0/silver_payu/templates/payu/transaction_form.html`

 * *Files identical despite different names*

### Comparing `silver-payu-0.5.1/silver_payu/views.py` & `silver-payu-0.6.0/silver_payu/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,25 @@
         return data
 
     def post(self, request):
         return HttpResponse(self.render_template())
 
 
 def threeds_data_url(transaction, request):
-    kwargs = {'token': _get_jwt_token(transaction)}
-    return reverse('silver-payu-payment-complete', kwargs=kwargs, request=request)
+    kwargs = {"token": _get_jwt_token(transaction)}
+    return reverse("silver-payu-payment-complete", kwargs=kwargs, request=request)
 
 
 @csrf_exempt
 @get_transaction_from_token
 def threeds_data_view(request, transaction, expired=None):
-    if transaction.state not in [Transaction.States.Initial, Transaction.States.Pending]:
+    if transaction.state not in [
+        Transaction.States.Initial,
+        Transaction.States.Pending,
+    ]:
         return HttpResponseNotAllowed()
 
     payment_method = transaction.payment_method
     if not payment_method:
         return HttpResponseNotAllowed()
 
     if payment_method.verified or payment_method.canceled:
@@ -55,21 +58,21 @@
 
     client_ip, _ = get_client_ip(request)
     if not client_ip:
         return HttpResponseServerError()
 
     threeds_data = {
         "BROWSER_IP": client_ip,
-        "BROWSER_ACCEPT_HEADER": request.META.get('HTTP_ACCEPT'),
-        "BROWSER_JAVA_ENABLED": request.POST.get('browser-java-enabled'),
-        "BROWSER_LANGUAGE": request.POST.get('browser-language'),
-        "BROWSER_COLOR_DEPTH": request.POST.get('browser-color-depth'),
-        "BROWSER_SCREEN_HEIGHT": request.POST.get('browser-screen-height'),
-        "BROWSER_SCREEN_WIDTH": request.POST.get('browser-screen-width'),
-        "BROWSER_TIMEZONE": request.POST.get('browser-timezone'),
-        "BROWSER_USER_AGENT": request.META.get('HTTP_USER_AGENT'),
+        "BROWSER_ACCEPT_HEADER": request.META.get("HTTP_ACCEPT"),
+        "BROWSER_JAVA_ENABLED": request.POST.get("browser-java-enabled"),
+        "BROWSER_LANGUAGE": request.POST.get("browser-language"),
+        "BROWSER_COLOR_DEPTH": request.POST.get("browser-color-depth"),
+        "BROWSER_SCREEN_HEIGHT": request.POST.get("browser-screen-height"),
+        "BROWSER_SCREEN_WIDTH": request.POST.get("browser-screen-width"),
+        "BROWSER_TIMEZONE": request.POST.get("browser-timezone"),
+        "BROWSER_USER_AGENT": request.META.get("HTTP_USER_AGENT"),
     }
 
     payment_method.threeds_data = threeds_data
     payment_method.save()
 
     return HttpResponse()
```

### Comparing `silver-payu-0.5.1/silver_payu.egg-info/PKG-INFO` & `silver-payu-0.6.0/silver_payu.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: silver-payu
-Version: 0.5.1
-Summary: UNKNOWN
+Version: 0.6.0
 Home-page: https://github.com/silverapp/silver-payu
 Author: Presslabs
 Author-email: ping@presslabs.com
 License: Apache 2.0
-Description: # silver-payu [![Build Status](https://travis-ci.org/silverapp/silver-payu.svg?branch=master)](https://travis-ci.org/silverapp/silver-payu)
-        
-        PayU Payment Processor implementation for silver
-        
 Keywords: django,app,reusable,billing,invoicing,api
 Platform: OS Independent
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+# silver-payu [![Build Status](https://travis-ci.org/silverapp/silver-payu.svg?branch=master)](https://travis-ci.org/silverapp/silver-payu)
+
+PayU Payment Processor implementation for silver
```

### Comparing `silver-payu-0.5.1/silver_payu.egg-info/SOURCES.txt` & `silver-payu-0.6.0/silver_payu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silver-payu-0.5.1/tests/fixtures.py` & `silver-payu-0.6.0/tests/fixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,106 +1,111 @@
 import pytest
+import responses
 
 from silver import payment_processors
-from silver.fixtures.factories import CustomerFactory, ProformaFactory, InvoiceFactory, \
-    TransactionFactory
+from silver.fixtures.factories import (
+    CustomerFactory,
+    ProformaFactory,
+    InvoiceFactory,
+    TransactionFactory,
+)
 from silver.models import Invoice
 
 from tests.factories import PayUPaymentMethodFactory
 
 
+@pytest.fixture(autouse=True)
+def reset_responses():
+    responses.reset()
+
+
 @pytest.fixture()
 def customer():
     return CustomerFactory.create(
-        address_1=u"Zalaegerszegi utca 65.\nH-5484 ligetv\xc3\xa1r", address_2='9'
+        address_1="Zalaegerszegi utca 65.\nH-5484 ligetv\xc3\xa1r", address_2="9"
     )
 
 
 @pytest.fixture()
 def payment_processor():
-    return payment_processors.get_instance('payu_manual')
+    return payment_processors.get_instance("payu_manual")
 
 
 @pytest.fixture()
 def payment_processor_triggered():
-    return payment_processors.get_instance('payu_triggered')
+    return payment_processors.get_instance("payu_triggered")
 
 
 @pytest.fixture()
 def payment_processor_triggered_v2():
-    return payment_processors.get_instance('payu_triggered_v2')
+    return payment_processors.get_instance("payu_triggered_v2")
 
 
 @pytest.fixture()
 def payment_method(customer, payment_processor):
     return PayUPaymentMethodFactory.create(
-        customer=customer,
-        payment_processor=payment_processor.name
+        customer=customer, payment_processor=payment_processor.name
     )
 
 
 @pytest.fixture()
 def payment_method_triggered(customer, payment_processor_triggered):
     return PayUPaymentMethodFactory.create(
-        customer=customer,
-        payment_processor=payment_processor_triggered.name
+        customer=customer, payment_processor=payment_processor_triggered.name
     )
 
 
 @pytest.fixture()
 def payment_method_triggered_v2(customer, payment_processor_triggered_v2):
     return PayUPaymentMethodFactory.create(
-        customer=customer,
-        payment_processor=payment_processor_triggered_v2.name
+        customer=customer, payment_processor=payment_processor_triggered_v2.name
     )
 
 
 @pytest.fixture()
 def proforma(customer):
     return ProformaFactory.create(
-        state=Invoice.STATES.ISSUED,
-        customer=customer,
-        transaction_currency='RON'
+        state=Invoice.STATES.ISSUED, customer=customer, transaction_currency="RON"
     )
 
 
 @pytest.fixture()
 def invoice(customer, proforma):
     return InvoiceFactory.create(
         related_document=proforma,
         state=Invoice.STATES.ISSUED,
         customer=customer,
-        transaction_currency='RON'
+        transaction_currency="RON",
     )
 
 
 @pytest.fixture()
 def transaction(db, customer, payment_processor, payment_method, proforma, invoice):
     return TransactionFactory.create(
         invoice=invoice,
         proforma=proforma,
-        currency='RON',
+        currency="RON",
         amount=invoice.total,
-        payment_method=payment_method
+        payment_method=payment_method,
     )
 
 
 @pytest.fixture()
 def transaction_triggered(customer, payment_method_triggered, proforma, invoice):
     return TransactionFactory.create(
         invoice=invoice,
         proforma=proforma,
-        currency='RON',
+        currency="RON",
         amount=invoice.total,
-        payment_method=payment_method_triggered
+        payment_method=payment_method_triggered,
     )
 
 
 @pytest.fixture()
 def transaction_triggered_v2(customer, payment_method_triggered_v2, proforma, invoice):
     return TransactionFactory.create(
         invoice=invoice,
         proforma=proforma,
-        currency='RON',
+        currency="RON",
         amount=invoice.total,
-        payment_method=payment_method_triggered_v2
+        payment_method=payment_method_triggered_v2,
     )
```

### Comparing `silver-payu-0.5.1/tests/test_forms.py` & `silver-payu-0.6.0/tests/test_forms.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,68 +6,87 @@
 
 from .fixtures import *
 
 
 faker = Faker()
 
 
-@patch('silver_payu.forms.datetime')
+@patch("silver_payu.forms.datetime")
 def test_payu_transaction_form_build_body(mocked_datetime, transaction, payment_method):
-    mocked_datetime.now.return_value.strftime.return_value = 'order_date'
+    mocked_datetime.now.return_value.strftime.return_value = "order_date"
 
-    with patch('silver.utils.payments._get_jwt_token') as mocked_token:
-        mocked_token.return_value = 'token'
+    with patch("silver.utils.payments._get_jwt_token") as mocked_token:
+        mocked_token.return_value = "token"
 
         form = PayUTransactionFormBase(payment_method, transaction, {})
 
         assert form._build_form_body(transaction, None) == {
-            'AUTOMODE': '1',
-            'BACK_REF': '/pay/token/complete',
-            'CURRENCY': 'RON',
-            'ORDER': [{'PCODE': '%s-%s' % (transaction.document.series,
-                                           transaction.document.number),
-                       'PNAME': 'Payment for %s %s-%s' % (transaction.document.kind,
-                                                          transaction.document.series,
-                                                          transaction.document.number),
-                       'PRICE': str(transaction.amount),
-                       'PRICE_TYPE': 'GROSS',
-                       'VAT': str(transaction.document.sales_tax_percent)}],
-            'ORDER_DATE': 'order_date',
-            'ORDER_REF': '%s' % transaction.uuid,
-            'PAY_METHOD': 'CCVISAMC',
-            'PRICES_CURRENCY': 'RON'
+            "AUTOMODE": "1",
+            "BACK_REF": "/pay/token/complete",
+            "CURRENCY": "RON",
+            "ORDER": [
+                {
+                    "PCODE": "%s-%s"
+                    % (transaction.document.series, transaction.document.number),
+                    "PNAME": "Payment for %s %s-%s"
+                    % (
+                        transaction.document.kind,
+                        transaction.document.series,
+                        transaction.document.number,
+                    ),
+                    "PRICE": str(transaction.amount),
+                    "PRICE_TYPE": "GROSS",
+                    "VAT": str(transaction.document.sales_tax_percent),
+                }
+            ],
+            "ORDER_DATE": "order_date",
+            "ORDER_REF": "%s" % transaction.uuid,
+            "PAY_METHOD": "CCVISAMC",
+            "PRICES_CURRENCY": "RON",
         }
 
 
-@pytest.mark.parametrize('data, form_class, archived_customer', [
-    ({
-        'email': faker.email(),
-        'first_name': faker.first_name(),
-        'last_name': faker.last_name(),
-        'phone': faker.phone_number(),
-        'country': '',
-        'fiscal_code': ''
-    }, PayUBillingForm, {}),
-    ({
-        'email': 'john@acme.com',
-        'first_name': 'John',
-        'last_name': 'Doe',
-        'phone': '+40000000000',
-        'country': 'RO',
-        'city': 'Timisoara',
-        'fiscal_code': ''
-    }, PayUTransactionFormBase, {
-        'BILL_ADDRESS': u"Zalaegerszegi utca 65.\nH-5484 ligetv\xc3\xa1r 9",
-        'BILL_CITY': 'Timisoara',
-        'BILL_COUNTRYCODE': 'RO',
-        'BILL_EMAIL': 'john@acme.com',
-        'BILL_FNAME': 'John',
-        'BILL_LNAME': 'Doe',
-        'BILL_PHONE': '+40000000000'
-    })
-])
-def test_payment_processor_get_form(payment_processor, transaction, data,
-                                    form_class, archived_customer):
+@pytest.mark.parametrize(
+    "data, form_class, archived_customer",
+    [
+        (
+            {
+                "email": faker.email(),
+                "first_name": faker.first_name(),
+                "last_name": faker.last_name(),
+                "phone": faker.phone_number(),
+                "country": "",
+                "fiscal_code": "",
+            },
+            PayUBillingForm,
+            {},
+        ),
+        (
+            {
+                "email": "john@acme.com",
+                "first_name": "John",
+                "last_name": "Doe",
+                "phone": "+40000000000",
+                "country": "RO",
+                "city": "Timisoara",
+                "fiscal_code": "",
+            },
+            PayUTransactionFormBase,
+            {
+                "BILL_ADDRESS": "Zalaegerszegi utca 65.\nH-5484 ligetv\xc3\xa1r 9",
+                "BILL_CITY": "Timisoara",
+                "BILL_COUNTRYCODE": "RO",
+                "BILL_EMAIL": "john@acme.com",
+                "BILL_FNAME": "John",
+                "BILL_LNAME": "Doe",
+                "BILL_PHONE": "+40000000000",
+            },
+        ),
+    ],
+)
+def test_payment_processor_get_form(
+    payment_processor, transaction, data, form_class, archived_customer
+):
     form = payment_processor.get_form(transaction, MagicMock(POST=data))
 
     assert isinstance(form, form_class)
     assert transaction.payment_method.archived_customer == archived_customer
```

