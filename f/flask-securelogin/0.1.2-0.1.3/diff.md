# Comparing `tmp/flask-securelogin-0.1.2.tar.gz` & `tmp/flask-securelogin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-securelogin-0.1.2.tar", last modified: Wed May 10 04:26:35 2023, max compression
+gzip compressed data, was "flask-securelogin-0.1.3.tar", last modified: Wed May 10 05:21:58 2023, max compression
```

## Comparing `flask-securelogin-0.1.2.tar` & `flask-securelogin-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 04:26:35.927049 flask-securelogin-0.1.2/
--rw-r--r--   0 qianguanghui   (501) staff       (20)    26526 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/LICENSE
--rw-r--r--   0 qianguanghui   (501) staff       (20)       16 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/MANIFEST.in
--rw-r--r--   0 qianguanghui   (501) staff       (20)    13852 2023-05-10 04:26:35.926353 flask-securelogin-0.1.2/PKG-INFO
--rw-r--r--   0 qianguanghui   (501) staff       (20)    13267 2023-05-10 04:22:20.000000 flask-securelogin-0.1.2/README.rst
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 04:26:35.906483 flask-securelogin-0.1.2/flask_securelogin/
--rw-r--r--   0 qianguanghui   (501) staff       (20)     3637 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/SecureAuth.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)       63 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/__init__.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     3846 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/account.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      661 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/errors.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      175 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/exception.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1969 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/models.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     7962 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/routes.py
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 04:26:35.924944 flask-securelogin-0.1.2/flask_securelogin/sms/
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1580 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/OTPGenerator.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      921 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/SMSBaseSender.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      306 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/SMSCall.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1342 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/SMSFactory.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     2495 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/TencentAPIClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      767 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/TwilioClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1262 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/UniSMSClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)        0 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/__init__.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      223 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/sms/models.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     5637 2023-05-09 05:09:40.000000 flask-securelogin-0.1.2/flask_securelogin/tokens.py
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 04:26:35.912536 flask-securelogin-0.1.2/flask_securelogin.egg-info/
--rw-r--r--   0 qianguanghui   (501) staff       (20)    13852 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/PKG-INFO
--rw-r--r--   0 qianguanghui   (501) staff       (20)      807 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/SOURCES.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)        1 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/dependency_links.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)      599 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/requires.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)       18 2023-05-10 04:26:35.000000 flask-securelogin-0.1.2/flask_securelogin.egg-info/top_level.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)       38 2023-05-10 04:26:35.927453 flask-securelogin-0.1.2/setup.cfg
--rw-r--r--   0 qianguanghui   (501) staff       (20)     2265 2023-05-10 04:23:04.000000 flask-securelogin-0.1.2/setup.py
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 05:21:58.489750 flask-securelogin-0.1.3/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    26526 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/LICENSE
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       16 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/MANIFEST.in
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    14043 2023-05-10 05:21:58.488240 flask-securelogin-0.1.3/PKG-INFO
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    13458 2023-05-10 05:20:29.000000 flask-securelogin-0.1.3/README.rst
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 05:21:58.465652 flask-securelogin-0.1.3/flask_securelogin/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     3637 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/SecureAuth.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       63 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/__init__.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     3846 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/account.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      661 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/errors.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      175 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/exception.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1969 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/models.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     7962 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/routes.py
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 05:21:58.486606 flask-securelogin-0.1.3/flask_securelogin/sms/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1580 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/OTPGenerator.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      921 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/SMSBaseSender.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      306 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/SMSCall.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1342 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/SMSFactory.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     2495 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/TencentAPIClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      767 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/TwilioClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1262 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/UniSMSClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)        0 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/__init__.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      223 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/sms/models.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     5637 2023-05-09 05:09:40.000000 flask-securelogin-0.1.3/flask_securelogin/tokens.py
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-10 05:21:58.472193 flask-securelogin-0.1.3/flask_securelogin.egg-info/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    14043 2023-05-10 05:21:58.000000 flask-securelogin-0.1.3/flask_securelogin.egg-info/PKG-INFO
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      807 2023-05-10 05:21:58.000000 flask-securelogin-0.1.3/flask_securelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)        1 2023-05-10 05:21:58.000000 flask-securelogin-0.1.3/flask_securelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      599 2023-05-10 05:21:58.000000 flask-securelogin-0.1.3/flask_securelogin.egg-info/requires.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       18 2023-05-10 05:21:58.000000 flask-securelogin-0.1.3/flask_securelogin.egg-info/top_level.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       38 2023-05-10 05:21:58.490922 flask-securelogin-0.1.3/setup.cfg
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     2265 2023-05-10 05:12:04.000000 flask-securelogin-0.1.3/setup.py
```

### Comparing `flask-securelogin-0.1.2/LICENSE` & `flask-securelogin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/PKG-INFO` & `flask-securelogin-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 Metadata-Version: 2.1
 Name: flask-securelogin
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.
 Home-page: https://github.com/brilliance-qian/flask-securelogin
 Author: Brilliance Qian
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
-*******************
+====================
 flask-securelogin
-*******************
+====================
 
 Description
-############
+====================
 Flask-securelogin is a library providing flask-based REST API services for account authentication with strong security protection.
 
 When developers build a service for mobile app or for web, one important thing they have to consider is to build an authentication for their customers. Most developers would choose password-based login design and session-cooke-based authentication because it is easy to implement.
 
 Unfortunately password-based authentication is a vulnerable design. Their customers could be victims of many security attacks: brutal force attack, phishing attack, password-leak if the web service didn't design their account security protection carefully. Besides, password-based authentciation is also a hassle to customers. For better security, the web service provider usually would ask their customers to have a complex password that must be 12+ charactors long and is with combination of uppercase, lowercase letters, digits and special charactors. This kind of password is usally hard to remember. Some customers might write it down somewhere, which is not a good approach on account security. Some customers might use a same password across many websites as people may have accounts on dozens of websites and it is hard to keep and remember different password per website. This is also not a good approach on account security. To enhance the security, many websites then ask their customers to provide multiple-factor-authentication (MFA), which make the system complicated and the login process less user friendly. Besides, account recovery from forget-password is also a painful process for customers.
 
 Flask-securelogin provides a SMS-based passwordless authentication. The phone number is the customer's userid. After registration, when a customer is trying to login, just enter the phone number. The flask-securelogin sends SMS/OTP code to the customer. After SMS verification, the authentication is done. No password. No worry about phishing attack, brutal force attack or password leak. No worry about forgetting password. Concise and secure.
 
 Installation
-############
+====================
 To install the latest release on `PyPI <https://pypi.org/project/flask-securelogin/>`_,
 simply run:
+
 ::
+
   pip3 install flask-securelogin
+
 Or to install the latest development version, run:
+
 ::
+
   git clone git@github.com:brilliance-qian/flask-securelogin.git
   cd flask-securelogin
   python3 setup.py install
   
 Quick Tutorial
-################
+====================
 Flask-securelogin provides a set of authentication APIs that can be seamlessly integrated to your REST API service. In your flask application, just simply add a few lines then the whole set of APIs will be ready to support account registration and login.
 
 Setup
-******
+--------
 Create the environment
+
 ::
+  
   $ mkdir sample_api
   $ cd sample_api
   $ python3 -m venv venv
   $ source venv/bin/activate
   $ pip install flask-securelogin
   $ pip freeze > requirements.txt
   $ mkdir app
   
 Source Code
-************
+------------
 Directory tree structure
+
 ::
+
     sample_api
     ├── app
     │   ├── __init__.py
     │   └── routes.py
     ├── entry.py
     ├── config.py
     └── tests
         └── test_routes.py
         
 app/__init__.py
-::
+
+.. code-block:: py
+
     from flask import Flask
     from flask_sqlalchemy import SQLAlchemy
     from flask_migrate import Migrate
     from flask_securelogin import secure_auth
     from config import Config
 
     db = SQLAlchemy()
@@ -90,37 +101,43 @@
         secure_auth.init_app(app)
 
         app.logger.setLevel(logging.INFO)
 
         return app
   
 app/routes.py
-::
+
+.. code-block:: py
+
     from flask_securelogin import routes
     from flask_securelogin import secure_auth
     from flask_securelogin.sms.TwilioClient import TwilioClient
 
     @secure_auth.create_sms_service
     def create_sms_service_instance(db, config, phone):
         return TwilioClient(db, config)
     
 entry.py
-::
+
+.. code-block:: py
+
     from app import create_app, db
     from app import routes
     from flask_securelogin.models import User
 
     app = create_app()
 
     @app.shell_context_processor
     def make_shell_context():
         return {'db': db, 'User': User}
         
 config.py, which is used to specify SMS vendor's setting
-::
+
+.. code-block:: py
+
     import os
     import traceback
     import bcrypt
     from datetime import timedelta
 
     basedir = os.path.abspath(os.path.dirname(__file__))
 
@@ -142,30 +159,36 @@
         # Twillio SID and Authe token
         TWILIO_ACCOUNT_SID = 'account_sid' # get your account sid from Twillio
         TWILIO_AUTH_TOKEN = 'auth_token'   # get your auth_token from Twillio
         TWILIO_SMS_SID = 'sms_sid'         # get your sms_sid from Twillio
         
         
 .flaskenv
-::
+
+.. code-block:: py
+
     #.flaskenv
     FLASK_APP=entry.py
     FLASK_DEBUG=1
 
 Validation
-************
+------------
 
 After the code is done, run the commands below to initialize 
+
 ::
+
     $ flask db init
     $ flask db migrate
     $ flask db upgrade
     
 Validate the auth routes
+
 ::
+
     $ flask routes
     Endpoint                        Methods  Rule
     ------------------------------  -------  -----------------------------------
     auth.change_password            POST     /api/auth/password
     auth.login                      POST     /api/auth/login_sms
     auth.login                      POST     /api/auth/login
     auth.logout                     POST     /api/auth/logout
@@ -173,23 +196,25 @@
     auth.op                         POST     /api/auth/op
     auth.op2                        POST     /api/auth/op2
     auth.refresh                    POST     /api/auth/refresh
     auth.register                   POST     /api/auth/register
     auth.verify_sms                 POST     /api/auth/verify_sms
     
 Test
-************
+------------
 Before you start to test SMS-based authentication, you need to setup configuration for calling SMS vendor. In this example, I suggest Twilio as the vendor. Twilio provides free trial account for testing purpose. After you create a free trial account on Twillio, register and verify your phone number on the free trial acount, the phone number can be used for testing without charge. Copy the Twilio account SID, auth token and SMS SID from Twilio, update the info in config.py. You are good to go.
 
-For details about how to create free trial account and get account SID, auth token and SMS SID, please refer to  https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account
+For details about how to create free trial account and get account SID, auth token and SMS SID, please refer to  `How to create your free trial account <https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account>`_
 
 After Twilio service is setup, let test the SMS-based authentication
 
 Open a terminal Run the API server
+
 ::
+
     $ cd sample_api
     $ source venv/bin/activate
     $ flask run
      * Serving Flask app 'entry.py'
      * Debug mode: on
     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
      * Running on http://127.0.0.1:5000
@@ -199,76 +224,90 @@
      * Debugger PIN: 633-717-714
 
 
 Open another terminal, try below commands
 Create a test account
 
 Registration API ``/api/auth/register``
+
 ::
+   
     $ curl -X POST -d '{ "username": "my test account", "auth_type": "PHONE", "phone": <YOUR_PHONE_NUMBER>}' -H "content-type: application/json" http://127.1:5000/api/auth/register
     {
       "message": "registered successfully",
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 Login with the test account
 
 Login API ``/api/auth/login``
+
 ::
+
     $ curl -X POST -d '{ "auth_type": "PHONE", "phone":  <YOUR_PHONE_NUMBER> }' -H "content-type: application/json" http://127.1:5000/api/auth/login
     {
       "phone":  <YOUR_PHONE_NUMBER>,
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 It receives a response with phone number and userid. Meanwhile, a SMS code is sent to your phone by Twilio. 
 
 If you didn't set Twilio settings correctly in config.py, you would receive below response
+
 ::
+
     {
       "error": "TwilioRestException",
       "exception": {
         "exception": "NoneType",
         "message": "None"
       },
       "http_code": "Bad Request",
       "message": "\n\u001b[31m\u001b[49mHTTP Error\u001b[0m \u001b[37m\u001b[49mYour request was:\u001b[0m\n\n\u001b[36m\u001b[49mPOST /Services/sms_sid/Verifications\u001b[0m\n\n\u001b[37m\u001b[49mTwilio returned the following information:\u001b[0m\n\n\u001b[34m\u001b[49mUnable to create record: Authentication Error - invalid username\u001b[0m\n\n\u001b[37m\u001b[49mMore information may be available here:\u001b[0m\n\n\u001b[34m\u001b[49mhttps://www.twilio.com/docs/errors/20003\u001b[0m\n\n"
     }
 
 Next step, enter the phone, userid and SMS token in the API below to verify SMS.
 
 Verify SMS API ``/api/auth/verify_sms``
+
 ::
+
     $ curl -X POST -d '{ "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639", "phone":  <YOUR_PHONE_NUMBER>, "token": <TOKEN> }' -H "content-type: application/json" http://127.1:5000/api/auth/verify_sms
     {
       "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6dHJ1ZSwiaWF0IjoxNjgzNjkwNzY3LCJqdGkiOiI0ZmViZTI5Zi04YjRkLTQ1ZmMtOTc5Ni1iMjFmZTA0ZmRkOTYiLCJ0eXBlIjoiYWNjZXNzIiwic3ViIjoxLCJuYmYiOjE2ODM2OTA3NjcsImV4cCI6MTY4MzY5MTM2N30.1US8-ndM3S-wrjSz8I9XOyBjvTPAjs_CVCrPZowGMeQ",
       "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MDc2NywianRpIjoiNmQ2ZjNkMmMtMDEyNC00OTA2LThjYjAtMTFjMTA5Mzg0NWU3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MDc2NywiZXhwIjoxNjg4ODc0NzY3LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.OXCMMmy9xn8-UooJVlnnCBFEd0s9MoXAx_z8q2O9RqQ",
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 Now the SMS authentication is done. You received an access token and refresh token. Access token is used to call protected operations in the API server. Refresh token is used to refresh access token if the access token is expired.
  
 Call protected operations with the access token. After you create your own operation, you can replace it by yours.
 
 Operation API ``/api/auth/op``
+
 ::
+
     $ curl -X POST -d '{}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6dHJ1ZSwiaWF0IjoxNjgzNjkwNzY3LCJqdGkiOiI0ZmViZTI5Zi04YjRkLTQ1ZmMtOTc5Ni1iMjFmZTA0ZmRkOTYiLCJ0eXBlIjoiYWNjZXNzIiwic3ViIjoxLCJuYmYiOjE2ODM2OTA3NjcsImV4cCI6MTY4MzY5MTM2N30.1US8-ndM3S-wrjSz8I9XOyBjvTPAjs_CVCrPZowGMeQ" http://127.1:5000/api/auth/op
     {
       "message": "test op successful"
     }
 
 Refresh token(please be reminded refresh token is used in Authorization header)
 
 Refresh token API ``/api/auth/refresh``
+
 ::
+
     $ curl -X POST -d '{}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MDc2NywianRpIjoiNmQ2ZjNkMmMtMDEyNC00OTA2LThjYjAtMTFjMTA5Mzg0NWU3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MDc2NywiZXhwIjoxNjg4ODc0NzY3LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.OXCMMmy9xn8-UooJVlnnCBFEd0s9MoXAx_z8q2O9RqQ" http://127.1:5000/api/auth/refresh
     {
       "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiM2QxZTMxMjUtY2RlNC00MDkzLTgxMWQtYWNjZmZmNGIzZjUxIiwidHlwZSI6ImFjY2VzcyIsInN1YiI6MSwibmJmIjoxNjgzNjkxMjk0LCJleHAiOjE2ODM2OTE4OTR9.0klw7uayU9qKh7fIEnhON6nrQdqFh1bbiF7mfnKOrJU",
       "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiNDk1ZDdmMjQtNTU0Yy00NjM3LWE5NzYtMzJmNDFlNDMzNzI3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MTI5NCwiZXhwIjoxNjg4ODc1Mjk0LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.UmNLBPuguHrGtsrJqNhp4TWgmu0OvORvEL58ittBgRc"
     }
     
 Logout API ``/api/auth/logout``
+
 ::
+
     $ curl -X POST -d '{ "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiNDk1ZDdmMjQtNTU0Yy00NjM3LWE5NzYtMzJmNDFlNDMzNzI3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MTI5NCwiZXhwIjoxNjg4ODc1Mjk0LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.UmNLBPuguHrGtsrJqNhp4TWgmu0OvORvEL58ittBgRc"}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiM2QxZTMxMjUtY2RlNC00MDkzLTgxMWQtYWNjZmZmNGIzZjUxIiwidHlwZSI6ImFjY2VzcyIsInN1YiI6MSwibmJmIjoxNjgzNjkxMjk0LCJleHAiOjE2ODM2OTE4OTR9.0klw7uayU9qKh7fIEnhON6nrQdqFh1bbiF7mfnKOrJU"  http://127.1:5000/api/auth/logout
     {
       "message": "logout successful"
     }
```

### Comparing `flask-securelogin-0.1.2/README.rst` & `flask-securelogin-0.1.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,75 @@
-*******************
+====================
 flask-securelogin
-*******************
+====================
 
 Description
-############
+====================
 Flask-securelogin is a library providing flask-based REST API services for account authentication with strong security protection.
 
 When developers build a service for mobile app or for web, one important thing they have to consider is to build an authentication for their customers. Most developers would choose password-based login design and session-cooke-based authentication because it is easy to implement.
 
 Unfortunately password-based authentication is a vulnerable design. Their customers could be victims of many security attacks: brutal force attack, phishing attack, password-leak if the web service didn't design their account security protection carefully. Besides, password-based authentciation is also a hassle to customers. For better security, the web service provider usually would ask their customers to have a complex password that must be 12+ charactors long and is with combination of uppercase, lowercase letters, digits and special charactors. This kind of password is usally hard to remember. Some customers might write it down somewhere, which is not a good approach on account security. Some customers might use a same password across many websites as people may have accounts on dozens of websites and it is hard to keep and remember different password per website. This is also not a good approach on account security. To enhance the security, many websites then ask their customers to provide multiple-factor-authentication (MFA), which make the system complicated and the login process less user friendly. Besides, account recovery from forget-password is also a painful process for customers.
 
 Flask-securelogin provides a SMS-based passwordless authentication. The phone number is the customer's userid. After registration, when a customer is trying to login, just enter the phone number. The flask-securelogin sends SMS/OTP code to the customer. After SMS verification, the authentication is done. No password. No worry about phishing attack, brutal force attack or password leak. No worry about forgetting password. Concise and secure.
 
 Installation
-############
+====================
 To install the latest release on `PyPI <https://pypi.org/project/flask-securelogin/>`_,
 simply run:
+
 ::
+
   pip3 install flask-securelogin
+
 Or to install the latest development version, run:
+
 ::
+
   git clone git@github.com:brilliance-qian/flask-securelogin.git
   cd flask-securelogin
   python3 setup.py install
   
 Quick Tutorial
-################
+====================
 Flask-securelogin provides a set of authentication APIs that can be seamlessly integrated to your REST API service. In your flask application, just simply add a few lines then the whole set of APIs will be ready to support account registration and login.
 
 Setup
-******
+--------
 Create the environment
+
 ::
+  
   $ mkdir sample_api
   $ cd sample_api
   $ python3 -m venv venv
   $ source venv/bin/activate
   $ pip install flask-securelogin
   $ pip freeze > requirements.txt
   $ mkdir app
   
 Source Code
-************
+------------
 Directory tree structure
+
 ::
+
     sample_api
     ├── app
     │   ├── __init__.py
     │   └── routes.py
     ├── entry.py
     ├── config.py
     └── tests
         └── test_routes.py
         
 app/__init__.py
-::
+
+.. code-block:: py
+
     from flask import Flask
     from flask_sqlalchemy import SQLAlchemy
     from flask_migrate import Migrate
     from flask_securelogin import secure_auth
     from config import Config
 
     db = SQLAlchemy()
@@ -75,37 +86,43 @@
         secure_auth.init_app(app)
 
         app.logger.setLevel(logging.INFO)
 
         return app
   
 app/routes.py
-::
+
+.. code-block:: py
+
     from flask_securelogin import routes
     from flask_securelogin import secure_auth
     from flask_securelogin.sms.TwilioClient import TwilioClient
 
     @secure_auth.create_sms_service
     def create_sms_service_instance(db, config, phone):
         return TwilioClient(db, config)
     
 entry.py
-::
+
+.. code-block:: py
+
     from app import create_app, db
     from app import routes
     from flask_securelogin.models import User
 
     app = create_app()
 
     @app.shell_context_processor
     def make_shell_context():
         return {'db': db, 'User': User}
         
 config.py, which is used to specify SMS vendor's setting
-::
+
+.. code-block:: py
+
     import os
     import traceback
     import bcrypt
     from datetime import timedelta
 
     basedir = os.path.abspath(os.path.dirname(__file__))
 
@@ -127,30 +144,36 @@
         # Twillio SID and Authe token
         TWILIO_ACCOUNT_SID = 'account_sid' # get your account sid from Twillio
         TWILIO_AUTH_TOKEN = 'auth_token'   # get your auth_token from Twillio
         TWILIO_SMS_SID = 'sms_sid'         # get your sms_sid from Twillio
         
         
 .flaskenv
-::
+
+.. code-block:: py
+
     #.flaskenv
     FLASK_APP=entry.py
     FLASK_DEBUG=1
 
 Validation
-************
+------------
 
 After the code is done, run the commands below to initialize 
+
 ::
+
     $ flask db init
     $ flask db migrate
     $ flask db upgrade
     
 Validate the auth routes
+
 ::
+
     $ flask routes
     Endpoint                        Methods  Rule
     ------------------------------  -------  -----------------------------------
     auth.change_password            POST     /api/auth/password
     auth.login                      POST     /api/auth/login_sms
     auth.login                      POST     /api/auth/login
     auth.logout                     POST     /api/auth/logout
@@ -158,23 +181,25 @@
     auth.op                         POST     /api/auth/op
     auth.op2                        POST     /api/auth/op2
     auth.refresh                    POST     /api/auth/refresh
     auth.register                   POST     /api/auth/register
     auth.verify_sms                 POST     /api/auth/verify_sms
     
 Test
-************
+------------
 Before you start to test SMS-based authentication, you need to setup configuration for calling SMS vendor. In this example, I suggest Twilio as the vendor. Twilio provides free trial account for testing purpose. After you create a free trial account on Twillio, register and verify your phone number on the free trial acount, the phone number can be used for testing without charge. Copy the Twilio account SID, auth token and SMS SID from Twilio, update the info in config.py. You are good to go.
 
-For details about how to create free trial account and get account SID, auth token and SMS SID, please refer to  https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account
+For details about how to create free trial account and get account SID, auth token and SMS SID, please refer to  `How to create your free trial account <https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account>`_
 
 After Twilio service is setup, let test the SMS-based authentication
 
 Open a terminal Run the API server
+
 ::
+
     $ cd sample_api
     $ source venv/bin/activate
     $ flask run
      * Serving Flask app 'entry.py'
      * Debug mode: on
     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
      * Running on http://127.0.0.1:5000
@@ -184,76 +209,90 @@
      * Debugger PIN: 633-717-714
 
 
 Open another terminal, try below commands
 Create a test account
 
 Registration API ``/api/auth/register``
+
 ::
+   
     $ curl -X POST -d '{ "username": "my test account", "auth_type": "PHONE", "phone": <YOUR_PHONE_NUMBER>}' -H "content-type: application/json" http://127.1:5000/api/auth/register
     {
       "message": "registered successfully",
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 Login with the test account
 
 Login API ``/api/auth/login``
+
 ::
+
     $ curl -X POST -d '{ "auth_type": "PHONE", "phone":  <YOUR_PHONE_NUMBER> }' -H "content-type: application/json" http://127.1:5000/api/auth/login
     {
       "phone":  <YOUR_PHONE_NUMBER>,
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 It receives a response with phone number and userid. Meanwhile, a SMS code is sent to your phone by Twilio. 
 
 If you didn't set Twilio settings correctly in config.py, you would receive below response
+
 ::
+
     {
       "error": "TwilioRestException",
       "exception": {
         "exception": "NoneType",
         "message": "None"
       },
       "http_code": "Bad Request",
       "message": "\n\u001b[31m\u001b[49mHTTP Error\u001b[0m \u001b[37m\u001b[49mYour request was:\u001b[0m\n\n\u001b[36m\u001b[49mPOST /Services/sms_sid/Verifications\u001b[0m\n\n\u001b[37m\u001b[49mTwilio returned the following information:\u001b[0m\n\n\u001b[34m\u001b[49mUnable to create record: Authentication Error - invalid username\u001b[0m\n\n\u001b[37m\u001b[49mMore information may be available here:\u001b[0m\n\n\u001b[34m\u001b[49mhttps://www.twilio.com/docs/errors/20003\u001b[0m\n\n"
     }
 
 Next step, enter the phone, userid and SMS token in the API below to verify SMS.
 
 Verify SMS API ``/api/auth/verify_sms``
+
 ::
+
     $ curl -X POST -d '{ "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639", "phone":  <YOUR_PHONE_NUMBER>, "token": <TOKEN> }' -H "content-type: application/json" http://127.1:5000/api/auth/verify_sms
     {
       "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6dHJ1ZSwiaWF0IjoxNjgzNjkwNzY3LCJqdGkiOiI0ZmViZTI5Zi04YjRkLTQ1ZmMtOTc5Ni1iMjFmZTA0ZmRkOTYiLCJ0eXBlIjoiYWNjZXNzIiwic3ViIjoxLCJuYmYiOjE2ODM2OTA3NjcsImV4cCI6MTY4MzY5MTM2N30.1US8-ndM3S-wrjSz8I9XOyBjvTPAjs_CVCrPZowGMeQ",
       "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MDc2NywianRpIjoiNmQ2ZjNkMmMtMDEyNC00OTA2LThjYjAtMTFjMTA5Mzg0NWU3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MDc2NywiZXhwIjoxNjg4ODc0NzY3LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.OXCMMmy9xn8-UooJVlnnCBFEd0s9MoXAx_z8q2O9RqQ",
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 Now the SMS authentication is done. You received an access token and refresh token. Access token is used to call protected operations in the API server. Refresh token is used to refresh access token if the access token is expired.
  
 Call protected operations with the access token. After you create your own operation, you can replace it by yours.
 
 Operation API ``/api/auth/op``
+
 ::
+
     $ curl -X POST -d '{}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6dHJ1ZSwiaWF0IjoxNjgzNjkwNzY3LCJqdGkiOiI0ZmViZTI5Zi04YjRkLTQ1ZmMtOTc5Ni1iMjFmZTA0ZmRkOTYiLCJ0eXBlIjoiYWNjZXNzIiwic3ViIjoxLCJuYmYiOjE2ODM2OTA3NjcsImV4cCI6MTY4MzY5MTM2N30.1US8-ndM3S-wrjSz8I9XOyBjvTPAjs_CVCrPZowGMeQ" http://127.1:5000/api/auth/op
     {
       "message": "test op successful"
     }
 
 Refresh token(please be reminded refresh token is used in Authorization header)
 
 Refresh token API ``/api/auth/refresh``
+
 ::
+
     $ curl -X POST -d '{}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MDc2NywianRpIjoiNmQ2ZjNkMmMtMDEyNC00OTA2LThjYjAtMTFjMTA5Mzg0NWU3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MDc2NywiZXhwIjoxNjg4ODc0NzY3LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.OXCMMmy9xn8-UooJVlnnCBFEd0s9MoXAx_z8q2O9RqQ" http://127.1:5000/api/auth/refresh
     {
       "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiM2QxZTMxMjUtY2RlNC00MDkzLTgxMWQtYWNjZmZmNGIzZjUxIiwidHlwZSI6ImFjY2VzcyIsInN1YiI6MSwibmJmIjoxNjgzNjkxMjk0LCJleHAiOjE2ODM2OTE4OTR9.0klw7uayU9qKh7fIEnhON6nrQdqFh1bbiF7mfnKOrJU",
       "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiNDk1ZDdmMjQtNTU0Yy00NjM3LWE5NzYtMzJmNDFlNDMzNzI3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MTI5NCwiZXhwIjoxNjg4ODc1Mjk0LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.UmNLBPuguHrGtsrJqNhp4TWgmu0OvORvEL58ittBgRc"
     }
     
 Logout API ``/api/auth/logout``
+
 ::
+
     $ curl -X POST -d '{ "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiNDk1ZDdmMjQtNTU0Yy00NjM3LWE5NzYtMzJmNDFlNDMzNzI3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MTI5NCwiZXhwIjoxNjg4ODc1Mjk0LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.UmNLBPuguHrGtsrJqNhp4TWgmu0OvORvEL58ittBgRc"}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiM2QxZTMxMjUtY2RlNC00MDkzLTgxMWQtYWNjZmZmNGIzZjUxIiwidHlwZSI6ImFjY2VzcyIsInN1YiI6MSwibmJmIjoxNjgzNjkxMjk0LCJleHAiOjE2ODM2OTE4OTR9.0klw7uayU9qKh7fIEnhON6nrQdqFh1bbiF7mfnKOrJU"  http://127.1:5000/api/auth/logout
     {
       "message": "logout successful"
     }
```

### Comparing `flask-securelogin-0.1.2/flask_securelogin/SecureAuth.py` & `flask-securelogin-0.1.3/flask_securelogin/SecureAuth.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/account.py` & `flask-securelogin-0.1.3/flask_securelogin/account.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/errors.py` & `flask-securelogin-0.1.3/flask_securelogin/errors.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/models.py` & `flask-securelogin-0.1.3/flask_securelogin/models.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/routes.py` & `flask-securelogin-0.1.3/flask_securelogin/routes.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/sms/OTPGenerator.py` & `flask-securelogin-0.1.3/flask_securelogin/sms/OTPGenerator.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/sms/SMSBaseSender.py` & `flask-securelogin-0.1.3/flask_securelogin/sms/SMSBaseSender.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/sms/SMSFactory.py` & `flask-securelogin-0.1.3/flask_securelogin/sms/SMSFactory.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/sms/TencentAPIClient.py` & `flask-securelogin-0.1.3/flask_securelogin/sms/TencentAPIClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/sms/TwilioClient.py` & `flask-securelogin-0.1.3/flask_securelogin/sms/TwilioClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/sms/UniSMSClient.py` & `flask-securelogin-0.1.3/flask_securelogin/sms/UniSMSClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin/tokens.py` & `flask-securelogin-0.1.3/flask_securelogin/tokens.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin.egg-info/PKG-INFO` & `flask-securelogin-0.1.3/flask_securelogin.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 Metadata-Version: 2.1
 Name: flask-securelogin
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.
 Home-page: https://github.com/brilliance-qian/flask-securelogin
 Author: Brilliance Qian
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
-*******************
+====================
 flask-securelogin
-*******************
+====================
 
 Description
-############
+====================
 Flask-securelogin is a library providing flask-based REST API services for account authentication with strong security protection.
 
 When developers build a service for mobile app or for web, one important thing they have to consider is to build an authentication for their customers. Most developers would choose password-based login design and session-cooke-based authentication because it is easy to implement.
 
 Unfortunately password-based authentication is a vulnerable design. Their customers could be victims of many security attacks: brutal force attack, phishing attack, password-leak if the web service didn't design their account security protection carefully. Besides, password-based authentciation is also a hassle to customers. For better security, the web service provider usually would ask their customers to have a complex password that must be 12+ charactors long and is with combination of uppercase, lowercase letters, digits and special charactors. This kind of password is usally hard to remember. Some customers might write it down somewhere, which is not a good approach on account security. Some customers might use a same password across many websites as people may have accounts on dozens of websites and it is hard to keep and remember different password per website. This is also not a good approach on account security. To enhance the security, many websites then ask their customers to provide multiple-factor-authentication (MFA), which make the system complicated and the login process less user friendly. Besides, account recovery from forget-password is also a painful process for customers.
 
 Flask-securelogin provides a SMS-based passwordless authentication. The phone number is the customer's userid. After registration, when a customer is trying to login, just enter the phone number. The flask-securelogin sends SMS/OTP code to the customer. After SMS verification, the authentication is done. No password. No worry about phishing attack, brutal force attack or password leak. No worry about forgetting password. Concise and secure.
 
 Installation
-############
+====================
 To install the latest release on `PyPI <https://pypi.org/project/flask-securelogin/>`_,
 simply run:
+
 ::
+
   pip3 install flask-securelogin
+
 Or to install the latest development version, run:
+
 ::
+
   git clone git@github.com:brilliance-qian/flask-securelogin.git
   cd flask-securelogin
   python3 setup.py install
   
 Quick Tutorial
-################
+====================
 Flask-securelogin provides a set of authentication APIs that can be seamlessly integrated to your REST API service. In your flask application, just simply add a few lines then the whole set of APIs will be ready to support account registration and login.
 
 Setup
-******
+--------
 Create the environment
+
 ::
+  
   $ mkdir sample_api
   $ cd sample_api
   $ python3 -m venv venv
   $ source venv/bin/activate
   $ pip install flask-securelogin
   $ pip freeze > requirements.txt
   $ mkdir app
   
 Source Code
-************
+------------
 Directory tree structure
+
 ::
+
     sample_api
     ├── app
     │   ├── __init__.py
     │   └── routes.py
     ├── entry.py
     ├── config.py
     └── tests
         └── test_routes.py
         
 app/__init__.py
-::
+
+.. code-block:: py
+
     from flask import Flask
     from flask_sqlalchemy import SQLAlchemy
     from flask_migrate import Migrate
     from flask_securelogin import secure_auth
     from config import Config
 
     db = SQLAlchemy()
@@ -90,37 +101,43 @@
         secure_auth.init_app(app)
 
         app.logger.setLevel(logging.INFO)
 
         return app
   
 app/routes.py
-::
+
+.. code-block:: py
+
     from flask_securelogin import routes
     from flask_securelogin import secure_auth
     from flask_securelogin.sms.TwilioClient import TwilioClient
 
     @secure_auth.create_sms_service
     def create_sms_service_instance(db, config, phone):
         return TwilioClient(db, config)
     
 entry.py
-::
+
+.. code-block:: py
+
     from app import create_app, db
     from app import routes
     from flask_securelogin.models import User
 
     app = create_app()
 
     @app.shell_context_processor
     def make_shell_context():
         return {'db': db, 'User': User}
         
 config.py, which is used to specify SMS vendor's setting
-::
+
+.. code-block:: py
+
     import os
     import traceback
     import bcrypt
     from datetime import timedelta
 
     basedir = os.path.abspath(os.path.dirname(__file__))
 
@@ -142,30 +159,36 @@
         # Twillio SID and Authe token
         TWILIO_ACCOUNT_SID = 'account_sid' # get your account sid from Twillio
         TWILIO_AUTH_TOKEN = 'auth_token'   # get your auth_token from Twillio
         TWILIO_SMS_SID = 'sms_sid'         # get your sms_sid from Twillio
         
         
 .flaskenv
-::
+
+.. code-block:: py
+
     #.flaskenv
     FLASK_APP=entry.py
     FLASK_DEBUG=1
 
 Validation
-************
+------------
 
 After the code is done, run the commands below to initialize 
+
 ::
+
     $ flask db init
     $ flask db migrate
     $ flask db upgrade
     
 Validate the auth routes
+
 ::
+
     $ flask routes
     Endpoint                        Methods  Rule
     ------------------------------  -------  -----------------------------------
     auth.change_password            POST     /api/auth/password
     auth.login                      POST     /api/auth/login_sms
     auth.login                      POST     /api/auth/login
     auth.logout                     POST     /api/auth/logout
@@ -173,23 +196,25 @@
     auth.op                         POST     /api/auth/op
     auth.op2                        POST     /api/auth/op2
     auth.refresh                    POST     /api/auth/refresh
     auth.register                   POST     /api/auth/register
     auth.verify_sms                 POST     /api/auth/verify_sms
     
 Test
-************
+------------
 Before you start to test SMS-based authentication, you need to setup configuration for calling SMS vendor. In this example, I suggest Twilio as the vendor. Twilio provides free trial account for testing purpose. After you create a free trial account on Twillio, register and verify your phone number on the free trial acount, the phone number can be used for testing without charge. Copy the Twilio account SID, auth token and SMS SID from Twilio, update the info in config.py. You are good to go.
 
-For details about how to create free trial account and get account SID, auth token and SMS SID, please refer to  https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account
+For details about how to create free trial account and get account SID, auth token and SMS SID, please refer to  `How to create your free trial account <https://www.twilio.com/docs/usage/tutorials/how-to-use-your-free-trial-account>`_
 
 After Twilio service is setup, let test the SMS-based authentication
 
 Open a terminal Run the API server
+
 ::
+
     $ cd sample_api
     $ source venv/bin/activate
     $ flask run
      * Serving Flask app 'entry.py'
      * Debug mode: on
     WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
      * Running on http://127.0.0.1:5000
@@ -199,76 +224,90 @@
      * Debugger PIN: 633-717-714
 
 
 Open another terminal, try below commands
 Create a test account
 
 Registration API ``/api/auth/register``
+
 ::
+   
     $ curl -X POST -d '{ "username": "my test account", "auth_type": "PHONE", "phone": <YOUR_PHONE_NUMBER>}' -H "content-type: application/json" http://127.1:5000/api/auth/register
     {
       "message": "registered successfully",
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 Login with the test account
 
 Login API ``/api/auth/login``
+
 ::
+
     $ curl -X POST -d '{ "auth_type": "PHONE", "phone":  <YOUR_PHONE_NUMBER> }' -H "content-type: application/json" http://127.1:5000/api/auth/login
     {
       "phone":  <YOUR_PHONE_NUMBER>,
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 It receives a response with phone number and userid. Meanwhile, a SMS code is sent to your phone by Twilio. 
 
 If you didn't set Twilio settings correctly in config.py, you would receive below response
+
 ::
+
     {
       "error": "TwilioRestException",
       "exception": {
         "exception": "NoneType",
         "message": "None"
       },
       "http_code": "Bad Request",
       "message": "\n\u001b[31m\u001b[49mHTTP Error\u001b[0m \u001b[37m\u001b[49mYour request was:\u001b[0m\n\n\u001b[36m\u001b[49mPOST /Services/sms_sid/Verifications\u001b[0m\n\n\u001b[37m\u001b[49mTwilio returned the following information:\u001b[0m\n\n\u001b[34m\u001b[49mUnable to create record: Authentication Error - invalid username\u001b[0m\n\n\u001b[37m\u001b[49mMore information may be available here:\u001b[0m\n\n\u001b[34m\u001b[49mhttps://www.twilio.com/docs/errors/20003\u001b[0m\n\n"
     }
 
 Next step, enter the phone, userid and SMS token in the API below to verify SMS.
 
 Verify SMS API ``/api/auth/verify_sms``
+
 ::
+
     $ curl -X POST -d '{ "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639", "phone":  <YOUR_PHONE_NUMBER>, "token": <TOKEN> }' -H "content-type: application/json" http://127.1:5000/api/auth/verify_sms
     {
       "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6dHJ1ZSwiaWF0IjoxNjgzNjkwNzY3LCJqdGkiOiI0ZmViZTI5Zi04YjRkLTQ1ZmMtOTc5Ni1iMjFmZTA0ZmRkOTYiLCJ0eXBlIjoiYWNjZXNzIiwic3ViIjoxLCJuYmYiOjE2ODM2OTA3NjcsImV4cCI6MTY4MzY5MTM2N30.1US8-ndM3S-wrjSz8I9XOyBjvTPAjs_CVCrPZowGMeQ",
       "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MDc2NywianRpIjoiNmQ2ZjNkMmMtMDEyNC00OTA2LThjYjAtMTFjMTA5Mzg0NWU3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MDc2NywiZXhwIjoxNjg4ODc0NzY3LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.OXCMMmy9xn8-UooJVlnnCBFEd0s9MoXAx_z8q2O9RqQ",
       "userid": "e5b53d55-bb32-40fb-aaeb-8ad750158639"
     }
     
 Now the SMS authentication is done. You received an access token and refresh token. Access token is used to call protected operations in the API server. Refresh token is used to refresh access token if the access token is expired.
  
 Call protected operations with the access token. After you create your own operation, you can replace it by yours.
 
 Operation API ``/api/auth/op``
+
 ::
+
     $ curl -X POST -d '{}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6dHJ1ZSwiaWF0IjoxNjgzNjkwNzY3LCJqdGkiOiI0ZmViZTI5Zi04YjRkLTQ1ZmMtOTc5Ni1iMjFmZTA0ZmRkOTYiLCJ0eXBlIjoiYWNjZXNzIiwic3ViIjoxLCJuYmYiOjE2ODM2OTA3NjcsImV4cCI6MTY4MzY5MTM2N30.1US8-ndM3S-wrjSz8I9XOyBjvTPAjs_CVCrPZowGMeQ" http://127.1:5000/api/auth/op
     {
       "message": "test op successful"
     }
 
 Refresh token(please be reminded refresh token is used in Authorization header)
 
 Refresh token API ``/api/auth/refresh``
+
 ::
+
     $ curl -X POST -d '{}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MDc2NywianRpIjoiNmQ2ZjNkMmMtMDEyNC00OTA2LThjYjAtMTFjMTA5Mzg0NWU3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MDc2NywiZXhwIjoxNjg4ODc0NzY3LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.OXCMMmy9xn8-UooJVlnnCBFEd0s9MoXAx_z8q2O9RqQ" http://127.1:5000/api/auth/refresh
     {
       "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiM2QxZTMxMjUtY2RlNC00MDkzLTgxMWQtYWNjZmZmNGIzZjUxIiwidHlwZSI6ImFjY2VzcyIsInN1YiI6MSwibmJmIjoxNjgzNjkxMjk0LCJleHAiOjE2ODM2OTE4OTR9.0klw7uayU9qKh7fIEnhON6nrQdqFh1bbiF7mfnKOrJU",
       "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiNDk1ZDdmMjQtNTU0Yy00NjM3LWE5NzYtMzJmNDFlNDMzNzI3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MTI5NCwiZXhwIjoxNjg4ODc1Mjk0LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.UmNLBPuguHrGtsrJqNhp4TWgmu0OvORvEL58ittBgRc"
     }
     
 Logout API ``/api/auth/logout``
+
 ::
+
     $ curl -X POST -d '{ "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiNDk1ZDdmMjQtNTU0Yy00NjM3LWE5NzYtMzJmNDFlNDMzNzI3IiwidHlwZSI6InJlZnJlc2giLCJzdWIiOjEsIm5iZiI6MTY4MzY5MTI5NCwiZXhwIjoxNjg4ODc1Mjk0LCJzaWQiOiI1YWUwOWViMy03NTNlLTQ5NDYtYmNhZS0yN2UzNzk4NDVlOGYifQ.UmNLBPuguHrGtsrJqNhp4TWgmu0OvORvEL58ittBgRc"}' -H "content-type: application/json" -H "Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJmcmVzaCI6ZmFsc2UsImlhdCI6MTY4MzY5MTI5NCwianRpIjoiM2QxZTMxMjUtY2RlNC00MDkzLTgxMWQtYWNjZmZmNGIzZjUxIiwidHlwZSI6ImFjY2VzcyIsInN1YiI6MSwibmJmIjoxNjgzNjkxMjk0LCJleHAiOjE2ODM2OTE4OTR9.0klw7uayU9qKh7fIEnhON6nrQdqFh1bbiF7mfnKOrJU"  http://127.1:5000/api/auth/logout
     {
       "message": "logout successful"
     }
```

### Comparing `flask-securelogin-0.1.2/flask_securelogin.egg-info/SOURCES.txt` & `flask-securelogin-0.1.3/flask_securelogin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/flask_securelogin.egg-info/requires.txt` & `flask-securelogin-0.1.3/flask_securelogin.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.2/setup.py` & `flask-securelogin-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open(file_path, "r") as fh:
         file_contents = fh.read()
     return file_contents
 
 
 setup(
     name='flask-securelogin',
-    version='0.1.2',
+    version='0.1.3',
     description='A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.',
     long_description=read_content("README.rst"),
     long_description_content_type="text/markdown",
     url='https://github.com/brilliance-qian/flask-securelogin',
     author='Brilliance Qian',
     license_files=('LICENSE.txt',),
     packages=setuptools.find_packages(),
```

