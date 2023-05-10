# Comparing `tmp/fyers-token-manager-0.0.4.tar.gz` & `tmp/fyers-token-manager-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers-token-manager-0.0.4.tar", last modified: Wed May 10 03:14:59 2023, max compression
+gzip compressed data, was "fyers-token-manager-0.0.5.tar", last modified: Wed May 10 03:21:50 2023, max compression
```

## Comparing `fyers-token-manager-0.0.4.tar` & `fyers-token-manager-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:14:59.475846 fyers-token-manager-0.0.4/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers-token-manager-0.0.4/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1033 2023-05-10 03:14:59.475846 fyers-token-manager-0.0.4/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      694 2023-02-12 04:33:59.000000 fyers-token-manager-0.0.4/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:14:59.475846 fyers-token-manager-0.0.4/fyers_token_manager/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-01-08 04:29:16.000000 fyers-token-manager-0.0.4/fyers_token_manager/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4574 2023-05-10 03:12:17.000000 fyers-token-manager-0.0.4/fyers_token_manager/main.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:14:59.475846 fyers-token-manager-0.0.4/fyers_token_manager.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1033 2023-05-10 03:14:59.000000 fyers-token-manager-0.0.4/fyers_token_manager.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      325 2023-05-10 03:14:59.000000 fyers-token-manager-0.0.4/fyers_token_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 03:14:59.000000 fyers-token-manager-0.0.4/fyers_token_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-10 03:14:59.000000 fyers-token-manager-0.0.4/fyers_token_manager.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       20 2023-05-10 03:14:59.000000 fyers-token-manager-0.0.4/fyers_token_manager.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      406 2023-05-10 03:14:57.000000 fyers-token-manager-0.0.4/pyproject.toml
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 03:14:59.475846 fyers-token-manager-0.0.4/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      687 2023-05-10 03:07:49.000000 fyers-token-manager-0.0.4/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:21:50.916078 fyers-token-manager-0.0.5/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers-token-manager-0.0.5/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1033 2023-05-10 03:21:50.916078 fyers-token-manager-0.0.5/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      694 2023-02-12 04:33:59.000000 fyers-token-manager-0.0.5/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:21:50.916078 fyers-token-manager-0.0.5/fyers_token_manager/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-01-08 04:29:16.000000 fyers-token-manager-0.0.5/fyers_token_manager/__init__.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4647 2023-05-10 03:21:33.000000 fyers-token-manager-0.0.5/fyers_token_manager/main.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:21:50.916078 fyers-token-manager-0.0.5/fyers_token_manager.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1033 2023-05-10 03:21:50.000000 fyers-token-manager-0.0.5/fyers_token_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      325 2023-05-10 03:21:50.000000 fyers-token-manager-0.0.5/fyers_token_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 03:21:50.000000 fyers-token-manager-0.0.5/fyers_token_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-10 03:21:50.000000 fyers-token-manager-0.0.5/fyers_token_manager.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       20 2023-05-10 03:21:50.000000 fyers-token-manager-0.0.5/fyers_token_manager.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      406 2023-05-10 03:14:57.000000 fyers-token-manager-0.0.5/pyproject.toml
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 03:21:50.916078 fyers-token-manager-0.0.5/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      687 2023-05-10 03:21:02.000000 fyers-token-manager-0.0.5/setup.py
```

### Comparing `fyers-token-manager-0.0.4/PKG-INFO` & `fyers-token-manager-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers-token-manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers-token-manager-0.0.4/README.md` & `fyers-token-manager-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fyers-token-manager-0.0.4/fyers_token_manager/main.py` & `fyers-token-manager-0.0.5/fyers_token_manager/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import os
 from datetime import datetime
 from urllib.parse import parse_qs, urlparse
 import base64
 import pyotp
 import requests
 
-from fyers_api import accessToken, fyersModel
-from fyers_api.Websocket import ws
-
 current_directory = os.path.dirname(os.path.realpath(__file__))
 
 data_path = os.path.join(current_directory, "data")
 data_file = datetime.now().strftime("%Y-%m-%d")
 fyers_access_token_path = os.path.join(data_path, data_file)
 
 log_path = os.path.join(current_directory, "logs")
 
 
 class FyersTokenManager:
-    def __init__(self, config):
+    def __init__(self, config, accessToken, fyersModel, ws):
         self.username = config["username"]
         self.totp_key = config["totp_key"]
         self.pin = config["pin"]
         self.client_id = config["client_id"]
         self.secret_key = config["secret_key"]
         self.redirect_uri = config["redirect_uri"]
 
+        self.__accessToken = accessToken
+        self.__fyersModel = fyersModel
+        self.__ws = ws
+
         self.__generate_folders_if_not_exists()
         self.__initialize()
 
     def __generate_folders_if_not_exists(self):
         if not os.path.exists(data_path):
             os.makedirs(data_path)
 
@@ -37,19 +38,19 @@
             os.makedirs(log_path)
 
     def __set_initial_values(self, token):
         self.http_access_token = token
 
         self.ws_access_token = f"{self.client_id}:{self.http_access_token}"
 
-        self.http_client = fyersModel.FyersModel(
+        self.http_client = self.__fyersModel.FyersModel(
             client_id=self.client_id, token=token, log_path=log_path
         )
 
-        self.ws_client = ws.FyersSocket(
+        self.ws_client = self.__ws.FyersSocket(
             access_token=self.ws_access_token, run_background=False, log_path=log_path
         )
 
     def __initialize(self):
         try:
             token = self.__read_file()
             self.__set_initial_values(token)
@@ -100,15 +101,15 @@
         data4 = f'{{"fyers_id":"{self.username}","app_id":"{self.client_id[:-4]}","redirect_uri":"{self.redirect_uri}","appType":"100","code_challenge":"","state":"abcdefg","scope":"","nonce":"","response_type":"code","create_cookie":true}}'
         r4 = s.post("https://api.fyers.in/api/v2/token", headers=headers, data=data4)
         assert r4.status_code == 308, f"Error in r4:\n {r4.json()}"
 
         parsed = urlparse(r4.json()["Url"])
         auth_code = parse_qs(parsed.query)["auth_code"][0]
 
-        session = accessToken.SessionModel(
+        session = self.__accessToken.SessionModel(
             client_id=self.client_id,
             secret_key=self.secret_key,
             redirect_uri=self.redirect_uri,
             response_type="code",
             grant_type="authorization_code",
         )
```

### Comparing `fyers-token-manager-0.0.4/fyers_token_manager.egg-info/PKG-INFO` & `fyers-token-manager-0.0.5/fyers_token_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers-token-manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers-token-manager-0.0.4/setup.py` & `fyers-token-manager-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers-token-manager",
-    version="0.0.4",
+    version="0.0.5",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers-token-manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

