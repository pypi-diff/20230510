# Comparing `tmp/flask_securelogin-0.1.5-py3-none-any.whl.zip` & `tmp/flask_securelogin-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 19181 bytes, number of entries: 21
+Zip file size: 19183 bytes, number of entries: 21
 -rw-r--r--  2.0 unx     3637 b- defN 23-May-09 05:09 flask_securelogin/SecureAuth.py
 -rw-r--r--  2.0 unx       63 b- defN 23-May-09 05:09 flask_securelogin/__init__.py
 -rw-r--r--  2.0 unx     3846 b- defN 23-May-09 05:09 flask_securelogin/account.py
 -rw-r--r--  2.0 unx      661 b- defN 23-May-09 05:09 flask_securelogin/errors.py
 -rw-r--r--  2.0 unx      175 b- defN 23-May-09 05:09 flask_securelogin/exception.py
 -rw-r--r--  2.0 unx     1969 b- defN 23-May-09 05:09 flask_securelogin/models.py
 -rw-r--r--  2.0 unx     7962 b- defN 23-May-09 05:09 flask_securelogin/routes.py
@@ -12,12 +12,12 @@
 -rw-r--r--  2.0 unx      306 b- defN 23-May-09 05:09 flask_securelogin/sms/SMSCall.py
 -rw-r--r--  2.0 unx     1342 b- defN 23-May-09 05:09 flask_securelogin/sms/SMSFactory.py
 -rw-r--r--  2.0 unx     2495 b- defN 23-May-09 05:09 flask_securelogin/sms/TencentAPIClient.py
 -rw-r--r--  2.0 unx      767 b- defN 23-May-09 05:09 flask_securelogin/sms/TwilioClient.py
 -rw-r--r--  2.0 unx     1262 b- defN 23-May-09 05:09 flask_securelogin/sms/UniSMSClient.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 05:09 flask_securelogin/sms/__init__.py
 -rw-r--r--  2.0 unx      223 b- defN 23-May-09 05:09 flask_securelogin/sms/models.py
--rw-r--r--  2.0 unx    15764 b- defN 23-May-10 05:54 flask_securelogin-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 05:54 flask_securelogin-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-10 05:54 flask_securelogin-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1844 b- defN 23-May-10 05:54 flask_securelogin-0.1.5.dist-info/RECORD
-21 files, 50564 bytes uncompressed, 16133 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx    15762 b- defN 23-May-10 06:01 flask_securelogin-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 06:01 flask_securelogin-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-10 06:01 flask_securelogin-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1844 b- defN 23-May-10 06:01 flask_securelogin-0.1.6.dist-info/RECORD
+21 files, 50562 bytes uncompressed, 16135 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: flask_securelogin/sms/__init__.py
 Comment: 
 
 Filename: flask_securelogin/sms/models.py
 Comment: 
 
-Filename: flask_securelogin-0.1.5.dist-info/METADATA
+Filename: flask_securelogin-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: flask_securelogin-0.1.5.dist-info/WHEEL
+Filename: flask_securelogin-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: flask_securelogin-0.1.5.dist-info/top_level.txt
+Filename: flask_securelogin-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_securelogin-0.1.5.dist-info/RECORD
+Filename: flask_securelogin-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `flask_securelogin-0.1.5.dist-info/METADATA` & `flask_securelogin-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-securelogin
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.
 Home-page: https://github.com/brilliance-qian/flask-securelogin
 Author: Brilliance Qian
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -82,21 +82,19 @@
 Flask-securelogin provides a SMS-based passwordless authentication. The phone number is the customer's userid. After registration, when a customer is trying to login, just enter the phone number. The flask-securelogin sends SMS/OTP code to the customer. After SMS verification, the authentication is done. No password. No worry about phishing attack, brutal force attack or password leak. No worry about forgetting password. Concise and secure.
 
 Installation
 ====================
 To install the latest release on `PyPI <https://pypi.org/project/flask-securelogin>`_ 
 
 simply run:
-
 .. code:: text
 
   pip3 install flask-securelogin
 
 Or to install the latest development version, run:
-
 .. code:: text
 
   git clone git@github.com:brilliance-qian/flask-securelogin.git
   cd flask-securelogin
   python3 setup.py install
   
 Quick Tutorial
```

## Comparing `flask_securelogin-0.1.5.dist-info/RECORD` & `flask_securelogin-0.1.6.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 flask_securelogin/sms/SMSCall.py,sha256=kS0CZkOpthmEUlZEduzQVjeMSlnJQKNitHv5tRVmmFk,306
 flask_securelogin/sms/SMSFactory.py,sha256=wpTLAzwE3GnPf6x-KiCJto-JNkOJIoSw8vWoy_WZU5o,1342
 flask_securelogin/sms/TencentAPIClient.py,sha256=bRDcAdLP69ngMEqM8MbQQj03rY4p353GvIwnFtdtcdE,2495
 flask_securelogin/sms/TwilioClient.py,sha256=KgSs4HORa40XxCO2aT8VC7Mz-0pekebGZmX7j_EYmOc,767
 flask_securelogin/sms/UniSMSClient.py,sha256=69Zv5nBU3KtVbhnkEwHHpMdM8Hf6YYP5DgoOQ_JTBTU,1262
 flask_securelogin/sms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 flask_securelogin/sms/models.py,sha256=BxsS341SY9Uz_pa2NOISeTCAHCNa1Yz-ZkavzCnCsso,223
-flask_securelogin-0.1.5.dist-info/METADATA,sha256=C16UIsdzQMel1kdTizTfUTh-UtNuGPO57L6U12gbiGQ,15764
-flask_securelogin-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-flask_securelogin-0.1.5.dist-info/top_level.txt,sha256=ncrbn4YMf1gvrYn_AI0qi6DtcgZxKbv_8dqVCkbSVjs,18
-flask_securelogin-0.1.5.dist-info/RECORD,,
+flask_securelogin-0.1.6.dist-info/METADATA,sha256=OgqwsKRHZKCKxGoGR2T6kgF6YSE8ZaE0J4nZMSvLXl8,15762
+flask_securelogin-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+flask_securelogin-0.1.6.dist-info/top_level.txt,sha256=ncrbn4YMf1gvrYn_AI0qi6DtcgZxKbv_8dqVCkbSVjs,18
+flask_securelogin-0.1.6.dist-info/RECORD,,
```

