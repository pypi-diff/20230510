# Comparing `tmp/anypay-1.1.2.tar.gz` & `tmp/anypay-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anypay-1.1.2.tar", last modified: Fri Mar 31 14:10:41 2023, max compression
+gzip compressed data, was "anypay-1.1.3.tar", last modified: Wed May 10 13:15:13 2023, max compression
```

## Comparing `anypay-1.1.2.tar` & `anypay-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-03-31 14:10:41.270301 anypay-1.1.2/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1210 2023-02-01 21:00:44.000000 anypay-1.1.2/LICENSE
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2817 2023-03-31 14:10:41.270301 anypay-1.1.2/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2051 2023-03-30 17:49:45.000000 anypay-1.1.2/README.md
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-03-31 14:10:41.270301 anypay-1.1.2/anypay/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      245 2023-02-01 20:28:21.000000 anypay-1.1.2/anypay/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)    15611 2023-03-31 14:10:29.000000 anypay-1.1.2/anypay/api.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      612 2023-03-30 10:03:25.000000 anypay-1.1.2/anypay/exceptions.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-03-31 14:10:41.270301 anypay-1.1.2/anypay/models/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      174 2023-02-01 20:20:14.000000 anypay-1.1.2/anypay/models/__init__.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      408 2023-03-30 10:02:29.000000 anypay-1.1.2/anypay/models/bill.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      547 2023-03-30 10:02:12.000000 anypay-1.1.2/anypay/models/payment.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      660 2023-03-30 10:02:48.000000 anypay-1.1.2/anypay/models/payout.py
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      229 2023-02-04 08:28:53.000000 anypay-1.1.2/anypay/models/rates.py
-drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-03-31 14:10:41.270301 anypay-1.1.2/anypay.egg-info/
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     2817 2023-03-31 14:10:41.000000 anypay-1.1.2/anypay.egg-info/PKG-INFO
--rw-rw-r--   0 bifle     (1000) bifle     (1000)      349 2023-03-31 14:10:41.000000 anypay-1.1.2/anypay.egg-info/SOURCES.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-03-31 14:10:41.000000 anypay-1.1.2/anypay.egg-info/dependency_links.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       15 2023-03-31 14:10:41.000000 anypay-1.1.2/anypay.egg-info/requires.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)        7 2023-03-31 14:10:41.000000 anypay-1.1.2/anypay.egg-info/top_level.txt
--rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-03-31 14:10:41.270301 anypay-1.1.2/setup.cfg
--rw-rw-r--   0 bifle     (1000) bifle     (1000)     1242 2023-03-31 14:10:36.000000 anypay-1.1.2/setup.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-10 13:15:13.296982 anypay-1.1.3/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1210 2023-02-01 21:00:44.000000 anypay-1.1.3/LICENSE
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2817 2023-05-10 13:15:13.296982 anypay-1.1.3/PKG-INFO
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2051 2023-03-30 17:49:45.000000 anypay-1.1.3/README.md
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-10 13:15:13.296982 anypay-1.1.3/anypay/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      245 2023-02-01 20:28:21.000000 anypay-1.1.3/anypay/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)    15585 2023-05-10 13:13:50.000000 anypay-1.1.3/anypay/api.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      612 2023-03-30 10:03:25.000000 anypay-1.1.3/anypay/exceptions.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-10 13:15:13.296982 anypay-1.1.3/anypay/models/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      174 2023-02-01 20:20:14.000000 anypay-1.1.3/anypay/models/__init__.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      408 2023-03-30 10:02:29.000000 anypay-1.1.3/anypay/models/bill.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      547 2023-03-30 10:02:12.000000 anypay-1.1.3/anypay/models/payment.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      660 2023-03-30 10:02:48.000000 anypay-1.1.3/anypay/models/payout.py
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      229 2023-02-04 08:28:53.000000 anypay-1.1.3/anypay/models/rates.py
+drwxrwxr-x   0 bifle     (1000) bifle     (1000)        0 2023-05-10 13:15:13.296982 anypay-1.1.3/anypay.egg-info/
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     2817 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/PKG-INFO
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)      349 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/SOURCES.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)        1 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/dependency_links.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       15 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/requires.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)        7 2023-05-10 13:15:13.000000 anypay-1.1.3/anypay.egg-info/top_level.txt
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)       38 2023-05-10 13:15:13.296982 anypay-1.1.3/setup.cfg
+-rw-rw-r--   0 bifle     (1000) bifle     (1000)     1242 2023-05-10 13:14:24.000000 anypay-1.1.3/setup.py
```

### Comparing `anypay-1.1.2/LICENSE` & `anypay-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anypay-1.1.2/PKG-INFO` & `anypay-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anypay
-Version: 1.1.2
+Version: 1.1.3
 Summary: Asynchronous AnyPay API wrapper
 Home-page: https://github.com/nikitalm8/anypay
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/anypay
 Project-URL: Bug Tracker, https://github.com/nikitalm8/anypay/issues
 Project-URL: API Docs, https://anypay.io/doc/api
```

### Comparing `anypay-1.1.2/README.md` & `anypay-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `anypay-1.1.2/anypay/api.py` & `anypay-1.1.3/anypay/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,14 @@
         :param lang: Bill page language.
         
         :return: Payout object.
         :raises: AnyPayAPIError
         """
 
         result = await self._make_request_async(
-            self.API_URL,
             'create-payment',
             '%(project_id)s%(amount)s%(currency)s%(desc)s%(method)s',
             project_id=project_id or self.project_id,
             pay_id=pay_id,
             amount=amount,
             currency=currency,
             desc=desc,
```

### Comparing `anypay-1.1.2/anypay/exceptions.py` & `anypay-1.1.3/anypay/exceptions.py`

 * *Files identical despite different names*

### Comparing `anypay-1.1.2/anypay/models/payment.py` & `anypay-1.1.3/anypay/models/payment.py`

 * *Files identical despite different names*

### Comparing `anypay-1.1.2/anypay/models/payout.py` & `anypay-1.1.3/anypay/models/payout.py`

 * *Files identical despite different names*

### Comparing `anypay-1.1.2/anypay.egg-info/PKG-INFO` & `anypay-1.1.3/anypay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anypay
-Version: 1.1.2
+Version: 1.1.3
 Summary: Asynchronous AnyPay API wrapper
 Home-page: https://github.com/nikitalm8/anypay
 Author: Nikita Minaev
 Author-email: <nikita@minaev.su>
 Project-URL: Homepage, https://github.com/nikitalm8/anypay
 Project-URL: Bug Tracker, https://github.com/nikitalm8/anypay/issues
 Project-URL: API Docs, https://anypay.io/doc/api
```

### Comparing `anypay-1.1.2/setup.py` & `anypay-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as file:
 
     long_description = "\n" + file.read()
 
-VERSION = '1.1.2'
+VERSION = '1.1.3'
 DESCRIPTION = 'Asynchronous AnyPay API wrapper'
 
 setup(
     name="anypay",
     version=VERSION,
     author="Nikita Minaev",
     author_email="<nikita@minaev.su>",
```

