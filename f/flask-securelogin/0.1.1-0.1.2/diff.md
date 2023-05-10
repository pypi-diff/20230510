# Comparing `tmp/flask-securelogin-0.1.1.tar.gz` & `tmp/flask-securelogin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-securelogin-0.1.1.tar", last modified: Tue May  9 01:49:07 2023, max compression
+gzip compressed data, was "flask-securelogin-0.1.2.tar", last modified: Wed May 10 04:26:35 2023, max compression
```

## Comparing `flask-securelogin-0.1.1.tar` & `flask-securelogin-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/
--rw-r--r--   0 qianguanghui   (501) staff       (20)    26526 2023-05-06 20:49:31.000000 flask-securelogin-0.1.1/LICENSE
--rw-r--r--   0 qianguanghui   (501) staff       (20)       16 2023-05-07 01:00:18.000000 flask-securelogin-0.1.1/MANIFEST.in
--rw-r--r--   0 qianguanghui   (501) staff       (20)      769 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/PKG-INFO
--rw-r--r--   0 qianguanghui   (501) staff       (20)       99 2023-05-07 00:31:50.000000 flask-securelogin-0.1.1/README.rst
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin/
--rw-r--r--   0 qianguanghui   (501) staff       (20)      432 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/SecureAuth.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)       63 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/__init__.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     3846 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/account.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      661 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/errors.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      175 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/exception.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1969 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/models.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     7962 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/routes.py
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin/sms/
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1580 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/OTPGenerator.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      921 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/SMSBaseSender.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      306 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/SMSCall.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1025 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/SMSFactory.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     2495 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/TencentAPIClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      767 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/TwilioClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1262 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/UniSMSClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)        0 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/__init__.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      223 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/models.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     5497 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/tokens.py
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/
--rw-r--r--   0 qianguanghui   (501) staff       (20)      769 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/PKG-INFO
--rw-r--r--   0 qianguanghui   (501) staff       (20)      807 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/SOURCES.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)        1 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/dependency_links.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)      599 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/requires.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)       18 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/top_level.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)       38 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/setup.cfg
--rw-r--r--   0 qianguanghui   (501) staff       (20)     2264 2023-05-09 01:48:52.000000 flask-securelogin-0.1.1/setup.py
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 04:26:35.927049 flask-securelogin-0.1.2/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    26526 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/LICENSE
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       16 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/MANIFEST.in
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    13852 2023-05-10 04:26:35.926353 flask-securelogin-0.1.2/PKG-INFO
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    13267 2023-05-10 04:22:20.000000 flask-securelogin-0.1.2/README.rst
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 04:26:35.906483 flask-securelogin-0.1.2/flask_securelogin/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     3637 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/SecureAuth.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       63 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/__init__.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     3846 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/account.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      661 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/errors.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      175 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/exception.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1969 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/models.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     7962 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/routes.py
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 04:26:35.924944 flask-securelogin-0.1.2/flask_securelogin/sms/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1580 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/OTPGenerator.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      921 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/SMSBaseSender.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      306 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/SMSCall.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1342 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/SMSFactory.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     2495 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/TencentAPIClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      767 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/TwilioClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1262 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/UniSMSClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)        0 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/__init__.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      223 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/models.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     5637 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/tokens.py
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 04:26:35.912536 flask-securelogin-0.1.2/flask_securelogin.egg-info/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    13852 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/PKG-INFO
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      807 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)        1 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      599 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/requires.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       18 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/top_level.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       38 2023-05-10 04:26:35.927453 flask-securelogin-0.1.2/setup.cfg
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     2265 2023-05-10 04:23:04.000000 flask-securelogin-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flask-securelogin-0.1.1/LICENSE` & `flask-securelogin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/account.py` & `flask-securelogin-0.1.2/flask_securelogin/account.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/errors.py` & `flask-securelogin-0.1.2/flask_securelogin/errors.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/models.py` & `flask-securelogin-0.1.2/flask_securelogin/models.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/routes.py` & `flask-securelogin-0.1.2/flask_securelogin/routes.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/sms/OTPGenerator.py` & `flask-securelogin-0.1.2/flask_securelogin/sms/OTPGenerator.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/sms/SMSBaseSender.py` & `flask-securelogin-0.1.2/flask_securelogin/sms/SMSBaseSender.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/sms/SMSFactory.py` & `flask-securelogin-0.1.2/flask_securelogin/sms/SMSFactory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from flask_securelogin.sms.TwilioClient import TwilioClient
 from flask_securelogin.sms.UniSMSClient import UniSMSClient
 from flask_securelogin.sms.TencentAPIClient import TencentAPIClient
+from flask_securelogin import secure_auth
 
 
 class SMSFactory():
     def get_vendor(config, phone):
         vendor = config['SMS_VENDOR']       # default setting
 
         # SMS vendor routing
@@ -14,14 +15,21 @@
             vendor = 'uni-sms'
         elif phone.find('+1') == 0:			# US phone number
             vendor = 'tencent'
 
         return vendor.lower()
 
     def create_instance(db, config, phone):
+        handler = secure_auth.get_create_sms_service_handler()
+        if handler is None:
+            return SMSFactory.create_default_service(db, config, phone)
+        else:
+            return handler(db, config, phone)
+
+    def create_default_service(db, config, phone):
         vendor = SMSFactory.get_vendor(config, phone)
 
         if vendor == 'twillio':
             return TwilioClient(db, config)
         elif vendor == 'uni-sms':
             return UniSMSClient(db, config)
         elif vendor == 'tencent':
```

### Comparing `flask-securelogin-0.1.1/flask_securelogin/sms/TencentAPIClient.py` & `flask-securelogin-0.1.2/flask_securelogin/sms/TencentAPIClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/sms/TwilioClient.py` & `flask-securelogin-0.1.2/flask_securelogin/sms/TwilioClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/sms/UniSMSClient.py` & `flask-securelogin-0.1.2/flask_securelogin/sms/UniSMSClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin/tokens.py` & `flask-securelogin-0.1.2/flask_securelogin/tokens.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from flask_securelogin.exception import AppException
 from flask_securelogin.models import UserActiveToken
+from flask_securelogin import secure_auth
 
 from flask_jwt_extended import (
     create_access_token,
     create_refresh_token,
     decode_token,
 )
 
@@ -118,16 +119,18 @@
 
         active_token.active = False
         self._db.session.commit()
 
     def check_if_token_revoked(self, token_jwt):
         token_type = token_jwt['type']
         if token_type != 'refresh':
-            # access token, skip check
-            # future: check the token against cache
+            handler = secure_auth.get_check_if_access_token_revoked_handler()
+            if handler is not None:
+                jti = token_jwt['jti']
+                return handler(jti)
             return False
 
         jti = token_jwt['jti']
         sid = token_jwt['sid']
 
         active_token = UserActiveToken.query.filter_by(sessionid=sid).first()
         if active_token is None:
```

### Comparing `flask-securelogin-0.1.1/flask_securelogin.egg-info/SOURCES.txt` & `flask-securelogin-0.1.2/flask_securelogin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/flask_securelogin.egg-info/requires.txt` & `flask-securelogin-0.1.2/flask_securelogin.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.1/setup.py` & `flask-securelogin-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     with open(file_path, "r") as fh:
         file_contents = fh.read()
     return file_contents
 
 
 setup(
     name='flask-securelogin',
-    version='0.1.1',
+    version='0.1.2',
     description='A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.',
-    long_description=read_content("README.md"),
+    long_description=read_content("README.rst"),
     long_description_content_type="text/markdown",
     url='https://github.com/brilliance-qian/flask-securelogin',
     author='Brilliance Qian',
     license_files=('LICENSE.txt',),
     packages=setuptools.find_packages(),
     install_requires=[
         'aiohttp',
```

