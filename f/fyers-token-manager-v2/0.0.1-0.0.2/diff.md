# Comparing `tmp/fyers_token_manager_v2-0.0.1.tar.gz` & `tmp/fyers_token_manager_v2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.0.1.tar", last modified: Wed May 10 03:53:55 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.0.2.tar", last modified: Wed May 10 04:44:46 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.0.1.tar` & `fyers_token_manager_v2-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:53:55.263932 fyers_token_manager_v2-0.0.1/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.1/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1066 2023-05-10 03:53:55.263932 fyers_token_manager_v2-0.0.1/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      726 2023-05-10 03:36:13.000000 fyers_token_manager_v2-0.0.1/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:53:55.263932 fyers_token_manager_v2-0.0.1/fyers_token_manager/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:47:58.000000 fyers_token_manager_v2-0.0.1/fyers_token_manager/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4647 2023-05-10 03:47:58.000000 fyers_token_manager_v2-0.0.1/fyers_token_manager/main.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 03:53:55.263932 fyers_token_manager_v2-0.0.1/fyers_token_manager_v2.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1066 2023-05-10 03:53:55.000000 fyers_token_manager_v2-0.0.1/fyers_token_manager_v2.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      330 2023-05-10 03:53:55.000000 fyers_token_manager_v2-0.0.1/fyers_token_manager_v2.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 03:53:55.000000 fyers_token_manager_v2-0.0.1/fyers_token_manager_v2.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-10 03:53:55.000000 fyers_token_manager_v2-0.0.1/fyers_token_manager_v2.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       20 2023-05-10 03:53:55.000000 fyers_token_manager_v2-0.0.1/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      366 2023-05-10 03:49:19.000000 fyers_token_manager_v2-0.0.1/pyproject.toml
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 03:53:55.263932 fyers_token_manager_v2-0.0.1/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      690 2023-05-10 03:53:52.000000 fyers_token_manager_v2-0.0.1/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.2/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 04:19:57.000000 fyers_token_manager_v2-0.0.2/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4523 2023-05-10 04:19:45.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2/__init__.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      305 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      383 2023-05-10 04:19:38.000000 fyers_token_manager_v2-0.0.2/pyproject.toml
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      690 2023-05-10 04:20:08.000000 fyers_token_manager_v2-0.0.2/setup.py
```

### Comparing `fyers_token_manager_v2-0.0.1/PKG-INFO` & `fyers_token_manager_v2-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_token_manager_v2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -17,21 +17,27 @@
   "pin": "<PIN>",
   "client_id": "<CLIENT_ID>",
   "secret_key": "<SECRET_KEY>",
   "redirect_uri": <REDIRECT_URL>
 }
 ```
 
+## Install
+
+```
+pip install fyers-token-manager-v2
+```
+
 ## Fyers Token Generator
 
 ```
 from fyers_api import accessToken, fyersModel
 from fyers_api.Websocket import ws
 
-from fyers_token_manager.main import FyersTokenManager
+from fyers_token_manager_v2 import FyersTokenManager
 ```
 
 #### Initialization
 
 ```
 fyersTokenManager = FyersTokenManager(config, accessToken, fyersModel, ws)
```

### Comparing `fyers_token_manager_v2-0.0.1/README.md` & `fyers_token_manager_v2-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,41 +6,45 @@
 00000050: 6e22 3a20 223c 5049 4e3e 222c 0d0a 2020  n": "<PIN>",..  
 00000060: 2263 6c69 656e 745f 6964 223a 2022 3c43  "client_id": "<C
 00000070: 4c49 454e 545f 4944 3e22 2c0d 0a20 2022  LIENT_ID>",..  "
 00000080: 7365 6372 6574 5f6b 6579 223a 2022 3c53  secret_key": "<S
 00000090: 4543 5245 545f 4b45 593e 222c 0d0a 2020  ECRET_KEY>",..  
 000000a0: 2272 6564 6972 6563 745f 7572 6922 3a20  "redirect_uri": 
 000000b0: 3c52 4544 4952 4543 545f 5552 4c3e 0d0a  <REDIRECT_URL>..
-000000c0: 7d0d 0a60 6060 0d0a 0d0a 2323 2046 7965  }..```....## Fye
-000000d0: 7273 2054 6f6b 656e 2047 656e 6572 6174  rs Token Generat
-000000e0: 6f72 0d0a 0d0a 6060 600d 0a66 726f 6d20  or....```..from 
-000000f0: 6679 6572 735f 6170 6920 696d 706f 7274  fyers_api import
-00000100: 2061 6363 6573 7354 6f6b 656e 2c20 6679   accessToken, fy
-00000110: 6572 734d 6f64 656c 0d0a 6672 6f6d 2066  ersModel..from f
-00000120: 7965 7273 5f61 7069 2e57 6562 736f 636b  yers_api.Websock
-00000130: 6574 2069 6d70 6f72 7420 7773 0d0a 0d0a  et import ws....
-00000140: 6672 6f6d 2066 7965 7273 5f74 6f6b 656e  from fyers_token
-00000150: 5f6d 616e 6167 6572 2e6d 6169 6e20 696d  _manager.main im
-00000160: 706f 7274 2046 7965 7273 546f 6b65 6e4d  port FyersTokenM
-00000170: 616e 6167 6572 0d0a 6060 600d 0a0d 0a23  anager..```....#
-00000180: 2323 2320 496e 6974 6961 6c69 7a61 7469  ### Initializati
-00000190: 6f6e 0d0a 0d0a 6060 600d 0a66 7965 7273  on....```..fyers
-000001a0: 546f 6b65 6e4d 616e 6167 6572 203d 2046  TokenManager = F
-000001b0: 7965 7273 546f 6b65 6e4d 616e 6167 6572  yersTokenManager
-000001c0: 2863 6f6e 6669 672c 2061 6363 6573 7354  (config, accessT
-000001d0: 6f6b 656e 2c20 6679 6572 734d 6f64 656c  oken, fyersModel
-000001e0: 2c20 7773 290d 0a0d 0a70 7269 6e74 2866  , ws)....print(f
-000001f0: 7965 7273 546f 6b65 6e4d 616e 6167 6572  yersTokenManager
-00000200: 2e68 7474 705f 6163 6365 7373 5f74 6f6b  .http_access_tok
-00000210: 656e 290d 0a70 7269 6e74 2866 7965 7273  en)..print(fyers
-00000220: 546f 6b65 6e4d 616e 6167 6572 2e77 735f  TokenManager.ws_
-00000230: 6163 6365 7373 5f74 6f6b 656e 290d 0a60  access_token)..`
-00000240: 6060 0d0a 0d0a 2323 2323 2048 5454 5020  ``....#### HTTP 
-00000250: 436c 6965 6e74 0d0a 0d0a 2d20 6679 6572  Client....- fyer
-00000260: 7354 6f6b 656e 4d61 6e61 6765 722e 6874  sTokenManager.ht
-00000270: 7470 5f63 6c69 656e 742e 6765 745f 7072  tp_client.get_pr
-00000280: 6f66 696c 6528 290d 0a0d 0a23 2323 2320  ofile()....#### 
-00000290: 5765 6253 6f63 6b65 7420 436c 6965 6e74  WebSocket Client
-000002a0: 0d0a 0d0a 2d20 6679 6572 7354 6f6b 656e  ....- fyersToken
-000002b0: 4d61 6e61 6765 722e 7773 5f63 6c69 656e  Manager.ws_clien
-000002c0: 742e 7375 6273 6372 6962 6528 7061 796c  t.subscribe(payl
-000002d0: 6f61 6429 0d0a                           oad)..
+000000c0: 7d0d 0a60 6060 0d0a 0d0a 2323 2049 6e73  }..```....## Ins
+000000d0: 7461 6c6c 0d0a 0d0a 6060 600d 0a70 6970  tall....```..pip
+000000e0: 2069 6e73 7461 6c6c 2066 7965 7273 2d74   install fyers-t
+000000f0: 6f6b 656e 2d6d 616e 6167 6572 2d76 320d  oken-manager-v2.
+00000100: 0a60 6060 0d0a 0d0a 2323 2046 7965 7273  .```....## Fyers
+00000110: 2054 6f6b 656e 2047 656e 6572 6174 6f72   Token Generator
+00000120: 0d0a 0d0a 6060 600d 0a66 726f 6d20 6679  ....```..from fy
+00000130: 6572 735f 6170 6920 696d 706f 7274 2061  ers_api import a
+00000140: 6363 6573 7354 6f6b 656e 2c20 6679 6572  ccessToken, fyer
+00000150: 734d 6f64 656c 0d0a 6672 6f6d 2066 7965  sModel..from fye
+00000160: 7273 5f61 7069 2e57 6562 736f 636b 6574  rs_api.Websocket
+00000170: 2069 6d70 6f72 7420 7773 0d0a 0d0a 6672   import ws....fr
+00000180: 6f6d 2066 7965 7273 5f74 6f6b 656e 5f6d  om fyers_token_m
+00000190: 616e 6167 6572 5f76 3220 696d 706f 7274  anager_v2 import
+000001a0: 2046 7965 7273 546f 6b65 6e4d 616e 6167   FyersTokenManag
+000001b0: 6572 0d0a 6060 600d 0a0d 0a23 2323 2320  er..```....#### 
+000001c0: 496e 6974 6961 6c69 7a61 7469 6f6e 0d0a  Initialization..
+000001d0: 0d0a 6060 600d 0a66 7965 7273 546f 6b65  ..```..fyersToke
+000001e0: 6e4d 616e 6167 6572 203d 2046 7965 7273  nManager = Fyers
+000001f0: 546f 6b65 6e4d 616e 6167 6572 2863 6f6e  TokenManager(con
+00000200: 6669 672c 2061 6363 6573 7354 6f6b 656e  fig, accessToken
+00000210: 2c20 6679 6572 734d 6f64 656c 2c20 7773  , fyersModel, ws
+00000220: 290d 0a0d 0a70 7269 6e74 2866 7965 7273  )....print(fyers
+00000230: 546f 6b65 6e4d 616e 6167 6572 2e68 7474  TokenManager.htt
+00000240: 705f 6163 6365 7373 5f74 6f6b 656e 290d  p_access_token).
+00000250: 0a70 7269 6e74 2866 7965 7273 546f 6b65  .print(fyersToke
+00000260: 6e4d 616e 6167 6572 2e77 735f 6163 6365  nManager.ws_acce
+00000270: 7373 5f74 6f6b 656e 290d 0a60 6060 0d0a  ss_token)..```..
+00000280: 0d0a 2323 2323 2048 5454 5020 436c 6965  ..#### HTTP Clie
+00000290: 6e74 0d0a 0d0a 2d20 6679 6572 7354 6f6b  nt....- fyersTok
+000002a0: 656e 4d61 6e61 6765 722e 6874 7470 5f63  enManager.http_c
+000002b0: 6c69 656e 742e 6765 745f 7072 6f66 696c  lient.get_profil
+000002c0: 6528 290d 0a0d 0a23 2323 2320 5765 6253  e()....#### WebS
+000002d0: 6f63 6b65 7420 436c 6965 6e74 0d0a 0d0a  ocket Client....
+000002e0: 2d20 6679 6572 7354 6f6b 656e 4d61 6e61  - fyersTokenMana
+000002f0: 6765 722e 7773 5f63 6c69 656e 742e 7375  ger.ws_client.su
+00000300: 6273 6372 6962 6528 7061 796c 6f61 6429  bscribe(payload)
+00000310: 0d0a                                     ..
```

### Comparing `fyers_token_manager_v2-0.0.1/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager-v2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -17,21 +17,27 @@
   "pin": "<PIN>",
   "client_id": "<CLIENT_ID>",
   "secret_key": "<SECRET_KEY>",
   "redirect_uri": <REDIRECT_URL>
 }
 ```
 
+## Install
+
+```
+pip install fyers-token-manager-v2
+```
+
 ## Fyers Token Generator
 
 ```
 from fyers_api import accessToken, fyersModel
 from fyers_api.Websocket import ws
 
-from fyers_token_manager.main import FyersTokenManager
+from fyers_token_manager_v2 import FyersTokenManager
 ```
 
 #### Initialization
 
 ```
 fyersTokenManager = FyersTokenManager(config, accessToken, fyersModel, ws)
```

### Comparing `fyers_token_manager_v2-0.0.1/setup.py` & `fyers_token_manager_v2-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.0.1",
+    version="0.0.2",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

