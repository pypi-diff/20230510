# Comparing `tmp/fyers_token_manager_v2-0.0.6.tar.gz` & `tmp/fyers_token_manager_v2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.0.6.tar", last modified: Wed May 10 05:24:24 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.0.7.tar", last modified: Wed May 10 05:36:55 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.0.6.tar` & `fyers_token_manager_v2-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.6/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:19:02.000000 fyers_token_manager_v2-0.0.6/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4523 2023-05-10 05:24:06.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2/__init__.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-10 05:23:56.000000 fyers_token_manager_v2-0.0.6/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:36:55.975710 fyers_token_manager_v2-0.0.7/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.7/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:36:55.975710 fyers_token_manager_v2-0.0.7/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:26:39.000000 fyers_token_manager_v2-0.0.7/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:36:55.971711 fyers_token_manager_v2-0.0.7/fyers_token_manager_v2/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4588 2023-05-10 05:36:04.000000 fyers_token_manager_v2-0.0.7/fyers_token_manager_v2/__init__.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:36:55.975710 fyers_token_manager_v2-0.0.7/fyers_token_manager_v2.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:36:55.000000 fyers_token_manager_v2-0.0.7/fyers_token_manager_v2.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-10 05:36:55.000000 fyers_token_manager_v2-0.0.7/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:36:55.000000 fyers_token_manager_v2-0.0.7/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-10 05:36:55.000000 fyers_token_manager_v2-0.0.7/fyers_token_manager_v2.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:36:55.000000 fyers_token_manager_v2-0.0.7/fyers_token_manager_v2.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:36:55.975710 fyers_token_manager_v2-0.0.7/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-10 05:26:27.000000 fyers_token_manager_v2-0.0.7/setup.py
```

### Comparing `fyers_token_manager_v2-0.0.6/PKG-INFO` & `fyers_token_manager_v2-0.0.7/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fyers_token_manager_v2
-Version: 0.0.6
+Name: fyers-token-manager-v2
+Version: 0.0.7
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
 
-from fyers_token_manager.v2 import FyersTokenManager
+from fyers_token_manager_v2 import FyersTokenManager
 ```
 
 #### Initialization
 
 ```
 fyersTokenManager = FyersTokenManager(config, accessToken, fyersModel, ws)
```

### Comparing `fyers_token_manager_v2-0.0.6/README.md` & `fyers_token_manager_v2-0.0.7/README.md`

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
-00000190: 616e 6167 6572 2e76 3220 696d 706f 7274  anager.v2 import
+00000190: 616e 6167 6572 5f76 3220 696d 706f 7274  anager_v2 import
 000001a0: 2046 7965 7273 546f 6b65 6e4d 616e 6167   FyersTokenManag
 000001b0: 6572 0d0a 6060 600d 0a0d 0a23 2323 2320  er..```....#### 
 000001c0: 496e 6974 6961 6c69 7a61 7469 6f6e 0d0a  Initialization..
 000001d0: 0d0a 6060 600d 0a66 7965 7273 546f 6b65  ..```..fyersToke
 000001e0: 6e4d 616e 6167 6572 203d 2046 7965 7273  nManager = Fyers
 000001f0: 546f 6b65 6e4d 616e 6167 6572 2863 6f6e  TokenManager(con
 00000200: 6669 672c 2061 6363 6573 7354 6f6b 656e  fig, accessToken
```

### Comparing `fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fyers-token-manager-v2
-Version: 0.0.6
+Name: fyers_token_manager_v2
+Version: 0.0.7
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
 
-from fyers_token_manager.v2 import FyersTokenManager
+from fyers_token_manager_v2 import FyersTokenManager
 ```
 
 #### Initialization
 
 ```
 fyersTokenManager = FyersTokenManager(config, accessToken, fyersModel, ws)
```

### Comparing `fyers_token_manager_v2-0.0.6/setup.py` & `fyers_token_manager_v2-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.0.6",
+    version="0.0.7",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

