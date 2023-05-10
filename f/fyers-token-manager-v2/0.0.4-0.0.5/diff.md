# Comparing `tmp/fyers_token_manager_v2-0.0.4.tar.gz` & `tmp/fyers_token_manager_v2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.0.4.tar", last modified: Wed May 10 05:10:53 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.0.5.tar", last modified: Wed May 10 05:20:42 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.0.4.tar` & `fyers_token_manager_v2-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:10:53.951569 fyers_token_manager_v2-0.0.4/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.4/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:10:53.951569 fyers_token_manager_v2-0.0.4/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 04:19:57.000000 fyers_token_manager_v2-0.0.4/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:10:53.947569 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4868 2023-05-10 05:10:03.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2/__init__.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:10:53.947569 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:10:53.951569 fyers_token_manager_v2-0.0.4/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-10 05:10:45.000000 fyers_token_manager_v2-0.0.4/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.5/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:19:02.000000 fyers_token_manager_v2-0.0.5/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:18:24.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2/__init__.py
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4523 2023-05-10 05:18:34.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2/v2.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      319 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-10 05:20:32.000000 fyers_token_manager_v2-0.0.5/setup.py
```

### Comparing `fyers_token_manager_v2-0.0.4/PKG-INFO` & `fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fyers_token_manager_v2
-Version: 0.0.4
+Name: fyers-token-manager-v2
+Version: 0.0.5
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -29,15 +29,15 @@
 
 ## Fyers Token Generator
 
 ```
 from fyers_api import accessToken, fyersModel
 from fyers_api.Websocket import ws
 
-from fyers_token_manager_v2 import FyersTokenManager
+from fyers_token_manager.v2 import FyersTokenManager
 ```
 
 #### Initialization
 
 ```
 fyersTokenManager = FyersTokenManager(config, accessToken, fyersModel, ws)
```

### Comparing `fyers_token_manager_v2-0.0.4/README.md` & `fyers_token_manager_v2-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 00000120: 0d0a 0d0a 6060 600d 0a66 726f 6d20 6679  ....```..from fy
 00000130: 6572 735f 6170 6920 696d 706f 7274 2061  ers_api import a
 00000140: 6363 6573 7354 6f6b 656e 2c20 6679 6572  ccessToken, fyer
 00000150: 734d 6f64 656c 0d0a 6672 6f6d 2066 7965  sModel..from fye
 00000160: 7273 5f61 7069 2e57 6562 736f 636b 6574  rs_api.Websocket
 00000170: 2069 6d70 6f72 7420 7773 0d0a 0d0a 6672   import ws....fr
 00000180: 6f6d 2066 7965 7273 5f74 6f6b 656e 5f6d  om fyers_token_m
-00000190: 616e 6167 6572 5f76 3220 696d 706f 7274  anager_v2 import
+00000190: 616e 6167 6572 2e76 3220 696d 706f 7274  anager.v2 import
 000001a0: 2046 7965 7273 546f 6b65 6e4d 616e 6167   FyersTokenManag
 000001b0: 6572 0d0a 6060 600d 0a0d 0a23 2323 2320  er..```....#### 
 000001c0: 496e 6974 6961 6c69 7a61 7469 6f6e 0d0a  Initialization..
 000001d0: 0d0a 6060 600d 0a66 7965 7273 546f 6b65  ..```..fyersToke
 000001e0: 6e4d 616e 6167 6572 203d 2046 7965 7273  nManager = Fyers
 000001f0: 546f 6b65 6e4d 616e 6167 6572 2863 6f6e  TokenManager(con
 00000200: 6669 672c 2061 6363 6573 7354 6f6b 656e  fig, accessToken
```

### Comparing `fyers_token_manager_v2-0.0.4/fyers_token_manager_v2/__init__.py` & `fyers_token_manager_v2-0.0.5/fyers_token_manager_v2/v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,25 +66,14 @@
         return token
 
     def __write_file(self, token):
         with open(f"{fyers_access_token_path}", "w") as f:
             f.write(token)
 
     def __get_token(self):
-        session = self.__accessToken.SessionModel(
-            client_id=self.client_id,
-            secret_key=self.secret_key,
-            redirect_uri=self.redirect_uri,
-            response_type="code",
-        )
-
-        auth_code = session.generate_authcode()
-
-        print(f"if app is not activated, you can activate using", auth_code)
-
         headers = {
             "Accept": "application/json",
             "Accept-Language": "en-US,en;q=0.9",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
         }
 
         s = requests.Session()
```

### Comparing `fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fyers-token-manager-v2
-Version: 0.0.4
+Name: fyers_token_manager_v2
+Version: 0.0.5
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -29,15 +29,15 @@
 
 ## Fyers Token Generator
 
 ```
 from fyers_api import accessToken, fyersModel
 from fyers_api.Websocket import ws
 
-from fyers_token_manager_v2 import FyersTokenManager
+from fyers_token_manager.v2 import FyersTokenManager
 ```
 
 #### Initialization
 
 ```
 fyersTokenManager = FyersTokenManager(config, accessToken, fyersModel, ws)
```

### Comparing `fyers_token_manager_v2-0.0.4/setup.py` & `fyers_token_manager_v2-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.0.4",
+    version="0.0.5",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

