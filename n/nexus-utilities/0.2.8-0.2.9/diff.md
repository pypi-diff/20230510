# Comparing `tmp/nexus-utilities-0.2.8.tar.gz` & `tmp/nexus-utilities-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.2.8.tar", last modified: Wed May 10 15:58:39 2023, max compression
+gzip compressed data, was "nexus-utilities-0.2.9.tar", last modified: Wed May 10 16:25:55 2023, max compression
```

## Comparing `nexus-utilities-0.2.8.tar` & `nexus-utilities-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:58:39.095232 nexus-utilities-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 15:58:39.095232 nexus-utilities-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:58:39.091232 nexus-utilities-0.2.8/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 15:58:38.000000 nexus-utilities-0.2.8/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-10 15:58:39.000000 nexus-utilities-0.2.8/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:58:38.000000 nexus-utilities-0.2.8/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 15:58:38.000000 nexus-utilities-0.2.8/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 15:58:38.000000 nexus-utilities-0.2.8/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:58:39.095232 nexus-utilities-0.2.8/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:58:39.095232 nexus-utilities-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-10 15:58:27.000000 nexus-utilities-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:55.483606 nexus-utilities-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 16:25:55.483606 nexus-utilities-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:55.479606 nexus-utilities-0.2.9/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 16:25:55.000000 nexus-utilities-0.2.9/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:55.479606 nexus-utilities-0.2.9/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:25:55.483606 nexus-utilities-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-10 16:25:44.000000 nexus-utilities-0.2.9/setup.py
```

### Comparing `nexus-utilities-0.2.8/LICENSE.txt` & `nexus-utilities-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.8/PKG-INFO` & `nexus-utilities-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.2.8
+Version: 0.2.9
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.2.8/README.md` & `nexus-utilities-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - [datetime\_utils.py](#datetime_utilspy)
   - [**get\_current\_timestamp()**](#get_current_timestamp)
   - [**getDuration(then, now=datetime.datetime.now())**](#getdurationthen-nowdatetimedatetimenow)
 - [package\_utils.py](#package_utilspy)
   - [**add\_package\_to\_path()**](#add_package_to_path)
   - [**import\_relative(package\_root\_name, module\_path, import\_name, alias=None)**](#import_relativepackage_root_name-module_path-import_name-aliasnone)
 - [password\_utils.py](#password_utilspy)
-  - [**get\_password(password\_method, password\_key, account\_name=None, access\_key=None, secret\_key=None, endpoint\_url=None, password\_path=None, encoding='utf-8')**](#get_passwordpassword_method-password_key-account_namenone-access_keynone-secret_keynone-endpoint_urlnone-password_pathnone-encodingutf-8)
+  - [**get\_password(password\_method, password\_key, account\_name=None, access\_key=None, secret\_key=None, endpoint\_url=None, region\_name=None, password\_path=None, encoding='utf-8')**](#get_passwordpassword_method-password_key-account_namenone-access_keynone-secret_keynone-endpoint_urlnone-region_namenone-password_pathnone-encodingutf-8)
 - [About the Author](#about-the-author)
 
 ---
 
 ## Installation
 
 ```python
@@ -152,26 +152,27 @@
 
 ---
 
 ## password_utils.py
 
 This module contains functions for working with passwords and other sensitive information.
 
-### **get_password(password_method, password_key, account_name=None, access_key=None, secret_key=None, endpoint_url=None, password_path=None, encoding='utf-8')**
+### **get_password(password_method, password_key, account_name=None, access_key=None, secret_key=None, endpoint_url=None, region_name=None, password_path=None, encoding='utf-8')**
 
 Arguments:
  * ***password_method (str):*** Desired password method.  Options include:
      * keyring:  Use the "keyring" python library
      * ssm:  Use the AWS Parameter Store method
      * secretsmanager:  Use the AWS Secrets Manager method
  * ***password_key (str):*** Unique identifier of the password or secret
  * ***account_name (str):*** Account name associated with the password (primarily used by keyring)
  * ***access_key (str):*** AWS access key
  * ***secret_key (str):*** AWS secret key
  * ***endpoint_url (str):*** AWS endpoint url
+ * ***region_name (str):*** AWS region name
  * ***password_path (str):*** AWS path to secret (primarily used by AWS Parameter Store)
  * ***encoding (str):*** Password encoding.  Supports the following, but uses utf-8 as the default: 'utf-8', 'ascii', 'latin-1', 'utf-16'
 
 Returns:
  * ***secret_value (str):*** Secret in plain text
 
 Allows multiple methods of retrieving sensitive information.
@@ -179,20 +180,22 @@
 Note:  If you prefer to use environment variables instead of passing the sensitive information directly, you can use the below.  They will be used in place of the function arguments when present:
 
 ```python
 AWS Parameter Store:
 access_key = 'AWS_SSM_ACCESS_KEY_ID'
 secret_key = 'AWS_SSM_SECRETACCESS_KEY_ID'
 endpoint_url = 'AWS_SSM_ENDPOINT_URL'
+region_name = 'AWS_SSM_REGION_NAME'
 password_path = 'AWS_SSM_PASSWORD_PATH'
 
 AWS Secrets Manager:
 access_key = 'AWS_SM_SECRET_ACCESS_KEY'
 secret_key = 'AWS_SM_ACCESS_KEY_ID'
 endpoint_url = 'AWS_SM_ENDPOINT_URL'
+region_name = 'AWS_SM_REGION_NAME'
 password_key = 'AWS_SM_PASSWORD_KEY'
 ```
 
 ---
 
 ## About the Author
```

### Comparing `nexus-utilities-0.2.8/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.2.9/nexus_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.2.8
+Version: 0.2.9
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.2.8/nexus_utils/config_utils.py` & `nexus-utilities-0.2.9/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.8/nexus_utils/database_utils.py` & `nexus-utilities-0.2.9/nexus_utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.8/nexus_utils/datetime_utils.py` & `nexus-utilities-0.2.9/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.8/nexus_utils/package_utils.py` & `nexus-utilities-0.2.9/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.2.8/nexus_utils/password_utils.py` & `nexus-utilities-0.2.9/nexus_utils/password_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Password-related utilities"""
 import boto3
 import os
 from botocore.exceptions import ClientError
 import keyring
 
-def get_password(password_method, password_key, account_name=None, access_key=None, secret_key=None, endpoint_url=None, password_path=None, encoding='utf-8'):
+def get_password(password_method, password_key, account_name=None, access_key=None, secret_key=None, endpoint_url=None, region_name=None, password_path=None, encoding='utf-8'):
     """Retrieve password based on method provided"""
     if password_method == 'keyring':
         try:
             response = keyring.get_password(account_name, password_key)
         except Exception as e:
             print(f"Error retrieving secret: {e}")
             return None
@@ -16,30 +16,32 @@
             secret_value = response
             return secret_value
         
     elif password_method == 'ssm':
         access_key = os.environ.get('AWS_SSM_ACCESS_KEY_ID') or access_key
         secret_key = os.environ.get('AWS_SSM_SECRETACCESS_KEY_ID') or secret_key
         ssm_endpoint_url = os.environ.get('AWS_SSM_ENDPOINT_URL') or endpoint_url
+        ssm_region_name = os.environ.get('AWS_SSM_REGION_NAME') or region_name
         ssm_password_path = os.environ.get('AWS_SSM_PASSWORD_PATH') or password_path
 
-        if not all([access_key, secret_key, ssm_endpoint_url, ssm_password_path]):
+        if not all([access_key, secret_key, ssm_endpoint_url, ssm_region_name, ssm_password_path]):
             raise ValueError('One or more required environment variables is not set')
 
         sts_client = boto3.client('sts', aws_access_key_id=access_key, aws_secret_access_key=secret_key)
 
         response = sts_client.get_session_token()
         access_key_id = response['Credentials']['AccessKeyId']
         secret_access_key = response['Credentials']['SecretAccessKey']
         session_token = response['Credentials']['SessionToken']
 
         client = boto3.client(
             'ssm',
             # endpoint_url='https://ssm.us-west-1.amazonaws.com',
             # region_name='us-west-1',
+            region_name=ssm_region_name,
             endpoint_url=ssm_endpoint_url,
             aws_access_key_id=access_key_id,
             aws_secret_access_key=secret_access_key,
             aws_session_token=session_token
         )
 
         # password_path = '/flat_file_loader/passwords/dev'
@@ -65,29 +67,31 @@
         
         return secret_value
     
     elif password_method == 'secretsmanager':
         access_key = os.environ.get('AWS_SM_SECRET_ACCESS_KEY') or access_key
         secret_key = os.environ.get('AWS_SM_ACCESS_KEY_ID') or secret_key
         sm_endpoint_url = os.environ.get('AWS_SM_ENDPOINT_URL') or endpoint_url
+        sm_region_name = os.environ.get('AWS_SM_REGION_NAME') or region_name
         password_key = os.environ.get('AWS_SM_PASSWORD_KEY') or password_key
 
-        if not all([access_key, secret_key, sm_endpoint_url, password_key]):
+        if not all([access_key, secret_key, sm_endpoint_url, sm_region_name, password_key]):
             raise ValueError('One or more required environment variables is not set')
 
         sts_client = boto3.client('sts', aws_access_key_id=access_key, aws_secret_access_key=secret_key)
 
         response = sts_client.get_session_token()
         access_key_id = response['Credentials']['AccessKeyId']
         secret_access_key = response['Credentials']['SecretAccessKey']
         session_token = response['Credentials']['SessionToken']
 
         client = boto3.client(
             'secretsmanager',
             endpoint_url=sm_endpoint_url,
+            region_name=sm_region_name,
             aws_access_key_id=access_key_id,
             aws_secret_access_key=secret_access_key,
             aws_session_token=session_token
         )
 
         if password_key is not None and password_key != '':
             secret_name = password_key
```

### Comparing `nexus-utilities-0.2.8/setup.py` & `nexus-utilities-0.2.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.2.8',
+    version='0.2.9',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

