# Comparing `tmp/afex-sso-0.0.42.tar.gz` & `tmp/afex-sso-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-sso-0.0.42.tar", last modified: Fri May  5 12:15:58 2023, max compression
+gzip compressed data, was "afex-sso-0.0.43.tar", last modified: Wed May 10 09:17:38 2023, max compression
```

## Comparing `afex-sso-0.0.42.tar` & `afex-sso-0.0.43.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.201666 afex-sso-0.0.42/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-03-04 00:13:16.000000 afex-sso-0.0.42/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     1356 2023-05-05 12:15:58.201758 afex-sso-0.0.42/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      911 2023-03-27 13:13:14.000000 afex-sso-0.0.42/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.199004 afex-sso-0.0.42/app/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.200139 afex-sso-0.0.42/app/AFEX_SSO/
--rw-r--r--   0 mac        (501) staff       (20)       33 2023-03-20 23:30:24.000000 afex-sso-0.0.42/app/AFEX_SSO/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.200633 afex-sso-0.0.42/app/AFEX_SSO/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-03-20 23:17:21.000000 afex-sso-0.0.42/app/AFEX_SSO/src/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1184 2023-05-05 11:28:13.000000 afex-sso-0.0.42/app/AFEX_SSO/src/sso.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.201405 afex-sso-0.0.42/app/afex_sso.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1356 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      308 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       61 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        9 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)      134 2023-03-15 21:51:52.000000 afex-sso-0.0.42/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)      474 2023-05-05 12:15:58.202039 afex-sso-0.0.42/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      802 2023-05-05 12:15:04.000000 afex-sso-0.0.42/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.131185 afex-sso-0.0.43/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-03-04 00:13:16.000000 afex-sso-0.0.43/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)     1615 2023-05-10 09:17:38.131260 afex-sso-0.0.43/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1170 2023-05-10 08:31:16.000000 afex-sso-0.0.43/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.128414 afex-sso-0.0.43/app/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.129661 afex-sso-0.0.43/app/AFEX_SSO/
+-rw-r--r--   0 mac        (501) staff       (20)       33 2023-03-20 23:30:24.000000 afex-sso-0.0.43/app/AFEX_SSO/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.130359 afex-sso-0.0.43/app/AFEX_SSO/src/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-03-20 23:17:21.000000 afex-sso-0.0.43/app/AFEX_SSO/src/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1706 2023-05-10 08:17:42.000000 afex-sso-0.0.43/app/AFEX_SSO/src/sso.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.131055 afex-sso-0.0.43/app/afex_sso.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1615 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      308 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       61 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        9 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)      134 2023-03-15 21:51:52.000000 afex-sso-0.0.43/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)      474 2023-05-10 09:17:38.131556 afex-sso-0.0.43/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      802 2023-05-10 09:05:27.000000 afex-sso-0.0.43/setup.py
```

### Comparing `afex-sso-0.0.42/LICENSE` & `afex-sso-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.42/PKG-INFO` & `afex-sso-0.0.43/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.42
+Version: 0.0.43
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -23,18 +23,27 @@
 
 ## simple integration (usage)
 
 instantiate the SSO class
 
 
       from AFEX_SSO import SSO
-      validate = SSO(sp_api_key, sp_hash_key, session_key)
+      sso = SSO()
 
       def get_user_details(View):
-        get_user = validate()['data'].get('user')
+        sso_instance = sso.check_credentials(sp_api_key, sp_hash_key, session_key)
+        get_user = sso_instance['data'].get('user')
+        '''
+            # other codes
+        '''
+      
+       def logout(View):
+           # get user email
+            email = " "
+            signout = sso.sign_out(sp_api_key, sp_hash_key, session_key, email)
         '''
             # other codes
         '''
 
 ## Keys
     
 - sp_api_key: service provider api key
@@ -60,7 +69,8 @@
 
     "message": "Successfully Retrieved"
 
     }
 
 
 
+
```

### Comparing `afex-sso-0.0.42/app/AFEX_SSO/src/sso.py` & `afex-sso-0.0.43/app/AFEX_SSO/src/sso.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,59 @@
-
 import time
 import json
 import requests
 from django.conf import settings as app_settings
 
 URL = app_settings.SSO_URL
 
+
 # settings.configure()
 # os.environ.setdefault("DJANGO_SETTINGS_MODULE", "SSO.settings")
 
 
 class SSO:
     """_summary_
     SSO CLASS
     """
 
-    def __init__(self, sp_api_key, sp_hash_key, session_key) -> None:
-        self.api = sp_api_key
-        self.hash = sp_hash_key
-        self.session = session_key
-
-    def __call__(self):
-        return self.check_credentials(self.api, self.hash, self.session)
-
-    @staticmethod
-    def check_credentials(api_key: str, hash_key: str, session_key: str):
-        """_summary_
-            checks the session and returns session status
-        """
+    # def __init__(self, sp_api_key, sp_hash_key, session_key) -> None:
+    #     self.api = sp_api_key
+    #     self.hash = sp_hash_key
+    #     self.session = session_key
+
+    # def __call__(self):
+    #     return self.check_credentials(self.api, self.hash, self.session)
+
+
+    def check_credentials(self, sp_api_key, sp_hash_key, session_key):
+        try:
+            headers = {
+                "api-key": sp_api_key,
+                "hash-key":  sp_hash_key,
+                "request-ts": session_key
+            }
+            response = requests.get(
+                f"{URL}/v1/api/verify_sp/{self.session}", headers=headers)
+            data = json.loads(response.text)
+            return data
+
+        except Exception as e:
+            return f"Something went wrong, please confirm the credentials and try again: {e}"
+
+    def sign_out(self, sp_api_key, sp_hash_key, session_key, email: str):
         try:
             headers = {
-                "api-key": api_key,
-                "hash-key":  hash_key,
+                "api-key": sp_api_key,
+                "hash-key": sp_hash_key,
                 "request-ts": session_key
             }
+            data = {
+                email: email
+            }
             response = requests.get(
-                f"{URL}/v1/api/verify_sp/{session_key}", headers=headers)
+                f"{URL}/v1/api/signout", headers=headers, data=data)
             data = json.loads(response.text)
             return data
 
         except Exception as e:
             return f"Something went wrong, please confirm the credentials and try again: {e}"
+
```

### Comparing `afex-sso-0.0.42/app/afex_sso.egg-info/PKG-INFO` & `afex-sso-0.0.43/app/afex_sso.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.42
+Version: 0.0.43
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -23,18 +23,27 @@
 
 ## simple integration (usage)
 
 instantiate the SSO class
 
 
       from AFEX_SSO import SSO
-      validate = SSO(sp_api_key, sp_hash_key, session_key)
+      sso = SSO()
 
       def get_user_details(View):
-        get_user = validate()['data'].get('user')
+        sso_instance = sso.check_credentials(sp_api_key, sp_hash_key, session_key)
+        get_user = sso_instance['data'].get('user')
+        '''
+            # other codes
+        '''
+      
+       def logout(View):
+           # get user email
+            email = " "
+            signout = sso.sign_out(sp_api_key, sp_hash_key, session_key, email)
         '''
             # other codes
         '''
 
 ## Keys
     
 - sp_api_key: service provider api key
@@ -60,7 +69,8 @@
 
     "message": "Successfully Retrieved"
 
     }
 
 
 
+
```

### Comparing `afex-sso-0.0.42/setup.py` & `afex-sso-0.0.43/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="afex-sso",
-    version="0.0.42",
+    version="0.0.43",
     description="For integrating sso",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="AFEX NIGERIA",
     author_email="it@africaexchange.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
-    install_requires=["requests >= 2.28.2", "django>=4.1"],
+    install_requires=["requests >= 2.28.2", "django>=3.2"],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires=">=3.7",
 )
```

