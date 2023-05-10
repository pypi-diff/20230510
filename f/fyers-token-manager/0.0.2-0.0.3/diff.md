# Comparing `tmp/fyers-token-manager-0.0.2.tar.gz` & `tmp/fyers-token-manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers-token-manager-0.0.2.tar", last modified: Sun Feb 12 05:44:05 2023, max compression
+gzip compressed data, was "fyers-token-manager-0.0.3.tar", last modified: Wed May 10 02:54:44 2023, max compression
```

## Comparing `fyers-token-manager-0.0.2.tar` & `fyers-token-manager-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-02-12 05:44:05.903499 fyers-token-manager-0.0.2/
--rw-rw-rw-   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers-token-manager-0.0.2/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1070 2023-02-12 05:44:05.903499 fyers-token-manager-0.0.2/PKG-INFO
--rw-rw-rw-   0 krunaldodiya  (1000) krunaldodiya  (1000)      694 2023-02-12 04:33:59.000000 fyers-token-manager-0.0.2/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-02-12 05:44:05.903499 fyers-token-manager-0.0.2/fyers_token_manager/
--rw-rw-rw-   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-01-08 04:29:16.000000 fyers-token-manager-0.0.2/fyers_token_manager/__init__.py
--rw-rw-rw-   0 krunaldodiya  (1000) krunaldodiya  (1000)     4113 2023-02-12 05:38:19.000000 fyers-token-manager-0.0.2/fyers_token_manager/main.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-02-12 05:44:05.903499 fyers-token-manager-0.0.2/fyers_token_manager.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1070 2023-02-12 05:44:05.000000 fyers-token-manager-0.0.2/fyers_token_manager.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      310 2023-02-12 05:44:05.000000 fyers-token-manager-0.0.2/fyers_token_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-02-12 05:44:05.000000 fyers-token-manager-0.0.2/fyers_token_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-02-12 05:44:05.000000 fyers-token-manager-0.0.2/fyers_token_manager.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       20 2023-02-12 05:44:05.000000 fyers-token-manager-0.0.2/fyers_token_manager.egg-info/top_level.txt
--rw-rw-rw-   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-02-12 05:44:05.903499 fyers-token-manager-0.0.2/setup.cfg
--rw-rw-rw-   0 krunaldodiya  (1000) krunaldodiya  (1000)      687 2023-02-12 05:37:42.000000 fyers-token-manager-0.0.2/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 02:54:44.799402 fyers-token-manager-0.0.3/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers-token-manager-0.0.3/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1070 2023-05-10 02:54:44.799402 fyers-token-manager-0.0.3/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      694 2023-02-12 04:33:59.000000 fyers-token-manager-0.0.3/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 02:54:44.799402 fyers-token-manager-0.0.3/fyers_token_manager/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-01-08 04:29:16.000000 fyers-token-manager-0.0.3/fyers_token_manager/__init__.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4633 2023-05-10 02:53:13.000000 fyers-token-manager-0.0.3/fyers_token_manager/main.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 02:54:44.799402 fyers-token-manager-0.0.3/fyers_token_manager.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1070 2023-05-10 02:54:44.000000 fyers-token-manager-0.0.3/fyers_token_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      310 2023-05-10 02:54:44.000000 fyers-token-manager-0.0.3/fyers_token_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 02:54:44.000000 fyers-token-manager-0.0.3/fyers_token_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-10 02:54:44.000000 fyers-token-manager-0.0.3/fyers_token_manager.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       20 2023-05-10 02:54:44.000000 fyers-token-manager-0.0.3/fyers_token_manager.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 02:54:44.799402 fyers-token-manager-0.0.3/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      687 2023-05-10 02:54:15.000000 fyers-token-manager-0.0.3/setup.py
```

### Comparing `fyers-token-manager-0.0.2/PKG-INFO` & `fyers-token-manager-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers-token-manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fyers-token-manager-0.0.2/README.md` & `fyers-token-manager-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fyers-token-manager-0.0.2/fyers_token_manager/main.py` & `fyers-token-manager-0.0.3/fyers_token_manager/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 import os
 from datetime import datetime
 from urllib.parse import parse_qs, urlparse
-
+import base64
 import requests
 
 current_directory = os.path.dirname(os.path.realpath(__file__))
 
 data_path = os.path.join(current_directory, "data")
 data_file = datetime.now().strftime("%Y-%m-%d")
 fyers_access_token_path = os.path.join(data_path, data_file)
 
 log_path = os.path.join(current_directory, "logs")
 
 
-class FyersBrokerConfig:
-    def __init__(self, config):
+class FyersTokenManager:
+    def __init__(self, config, accessToken, fyersModel, ws):
         self.username = config["username"]
-        self.password = config["password"]
+        self.totp_key = config["totp_key"]
         self.pin = config["pin"]
         self.client_id = config["client_id"]
         self.secret_key = config["secret_key"]
         self.redirect_uri = config["redirect_uri"]
 
-
-class FyersTokenManager:
-    def __init__(self, config, accessToken, fyersModel, ws):
-        self.__config = FyersBrokerConfig(config)
         self.__accessToken = accessToken
         self.__fyersModel = fyersModel
         self.__ws = ws
 
         self.__generate_folders_if_not_exists()
-
         self.__initialize()
 
     def __generate_folders_if_not_exists(self):
         if not os.path.exists(data_path):
             os.makedirs(data_path)
 
         if not os.path.exists(log_path):
             os.makedirs(log_path)
 
     def __set_initial_values(self, token):
         self.http_access_token = token
+
+        self.ws_access_token = f"{self.client_id}:{self.http_access_token}"
+
         self.http_client = self.__fyersModel.FyersModel(
-            client_id=self.__config.client_id, token=token, log_path=log_path
+            client_id=self.client_id, token=token, log_path=log_path
         )
 
-        self.ws_access_token = f"{self.__config.client_id}:{self.http_access_token}"
         self.ws_client = self.__ws.FyersSocket(
             access_token=self.ws_access_token, run_background=False, log_path=log_path
         )
 
     def __initialize(self):
         try:
             token = self.__read_file()
@@ -59,49 +56,69 @@
         except FileNotFoundError:
             token = self.__setup()
             self.__set_initial_values(token)
 
     def __read_file(self):
         with open(f"{fyers_access_token_path}", "r") as f:
             token = f.read()
+
         return token
 
     def __write_file(self, token):
         with open(f"{fyers_access_token_path}", "w") as f:
             f.write(token)
 
-    def __setup(self):
+    def __get_token(self):
+        headers = {
+            "Accept": "application/json",
+            "Accept-Language": "en-US,en;q=0.9",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
+        }
+
         s = requests.Session()
+        s.headers.update(headers)
 
-        data1 = f'{{"fy_id":"{self.__config.username}","password":"{self.__config.password}","app_id":"2","imei":"","recaptcha_token":""}}'
-        r1 = s.post("https://api.fyers.in/vagator/v1/login", data=data1)
+        data1 = f'{{"fy_id":"{base64.b64encode(f"{self.username}".encode()).decode()}","app_id":"2"}}'
+        r1 = s.post("https://api-t2.fyers.in/vagator/v2/send_login_otp_v2", data=data1)
         assert r1.status_code == 200, f"Error in r1:\n {r1.json()}"
 
         request_key = r1.json()["request_key"]
-        data2 = f'{{"request_key":"{request_key}","identity_type":"pin","identifier":"{self.__config.pin}","recaptcha_token":""}}'
-        r2 = s.post("https://api.fyers.in/vagator/v1/verify_pin", data=data2)
-        assert r2.status_code == 200, f"Error in r2:\n {r2.json()}"
+        data2 = (
+            f'{{"request_key":"{request_key}","otp":{pyotp.TOTP(self.totp_key).now()}}}'
+        )
+        r2 = s.post("https://api-t2.fyers.in/vagator/v2/verify_otp", data=data2)
+        assert r2.status_code == 200, f"Error in r2:\n {r2.text}"
+
+        request_key = r2.json()["request_key"]
+        data3 = f'{{"request_key":"{request_key}","identity_type":"pin","identifier":"{base64.b64encode(f"{self.pin}".encode()).decode()}"}}'
+        r3 = s.post("https://api-t2.fyers.in/vagator/v2/verify_pin_v2", data=data3)
+        assert r3.status_code == 200, f"Error in r3:\n {r3.json()}"
 
         headers = {
-            "authorization": f"Bearer {r2.json()['data']['access_token']}",
+            "authorization": f"Bearer {r3.json()['data']['access_token']}",
             "content-type": "application/json; charset=UTF-8",
         }
-        data3 = f'{{"fyers_id":"{self.__config.username}","app_id":"{self.__config.client_id[:-4]}","redirect_uri":"{self.__config.redirect_uri}","appType":"100","code_challenge":"","state":"abcdefg","scope":"","nonce":"","response_type":"code","create_cookie":true}}'
-        r3 = s.post("https://api.fyers.in/api/v2/token", headers=headers, data=data3)
-        assert r3.status_code == 308, f"Error in r3:\n {r3.json()}"
+        data4 = f'{{"fyers_id":"{self.username}","app_id":"{self.client_id[:-4]}","redirect_uri":"{self.redirect_uri}","appType":"100","code_challenge":"","state":"abcdefg","scope":"","nonce":"","response_type":"code","create_cookie":true}}'
+        r4 = s.post("https://api.fyers.in/api/v2/token", headers=headers, data=data4)
+        assert r4.status_code == 308, f"Error in r4:\n {r4.json()}"
 
-        parsed = urlparse(r3.json()["Url"])
+        parsed = urlparse(r4.json()["Url"])
         auth_code = parse_qs(parsed.query)["auth_code"][0]
 
         session = self.__accessToken.SessionModel(
-            client_id=self.__config.client_id,
-            secret_key=self.__config.secret_key,
-            redirect_uri=self.__config.redirect_uri,
+            client_id=self.client_id,
+            secret_key=self.secret_key,
+            redirect_uri=self.redirect_uri,
             response_type="code",
             grant_type="authorization_code",
         )
+
         session.set_token(auth_code)
         response = session.generate_token()
-        token = response["access_token"]
+
+        return response["access_token"]
+
+    def __setup(self):
+        token = self.__get_token()
         self.__write_file(token)
 
         return token
```

### Comparing `fyers-token-manager-0.0.2/fyers_token_manager.egg-info/PKG-INFO` & `fyers-token-manager-0.0.3/fyers_token_manager.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers-token-manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fyers-token-manager-0.0.2/setup.py` & `fyers-token-manager-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers-token-manager",
-    version="0.0.2",
+    version="0.0.3",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers-token-manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

