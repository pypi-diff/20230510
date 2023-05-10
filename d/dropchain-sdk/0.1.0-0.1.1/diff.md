# Comparing `tmp/dropchain-sdk-0.1.0.tar.gz` & `tmp/dropchain-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dropchain-sdk-0.1.0.tar", last modified: Wed Apr  5 02:15:43 2023, max compression
+gzip compressed data, was "dist/dropchain-sdk-0.1.1.tar", last modified: Wed May 10 20:58:47 2023, max compression
```

## Comparing `dropchain-sdk-0.1.0.tar` & `dropchain-sdk-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/
--rw-r--r--   0 crazink    (501) staff       (20)      935 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 crazink    (501) staff       (20)     1069 2023-03-03 02:58:53.000000 dropchain-sdk-0.1.0/LICENSE.md
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/dropchain_sdk/
--rw-r--r--   0 crazink    (501) staff       (20)    22820 2023-04-05 02:08:09.000000 dropchain-sdk-0.1.0/dropchain_sdk/__init__.py
--rw-r--r--   0 crazink    (501) staff       (20)      436 2023-03-04 00:06:46.000000 dropchain-sdk-0.1.0/README.md
--rw-r--r--   0 crazink    (501) staff       (20)      580 2023-04-05 02:11:15.000000 dropchain-sdk-0.1.0/setup.py
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/dropchain_sdk.egg-info/
--rw-r--r--   0 crazink    (501) staff       (20)      935 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/dropchain_sdk.egg-info/PKG-INFO
--rw-r--r--   0 crazink    (501) staff       (20)      239 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/dropchain_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 crazink    (501) staff       (20)        9 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/dropchain_sdk.egg-info/requires.txt
--rw-r--r--   0 crazink    (501) staff       (20)       14 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/dropchain_sdk.egg-info/top_level.txt
--rw-r--r--   0 crazink    (501) staff       (20)        1 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/dropchain_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 crazink    (501) staff       (20)       38 2023-04-05 02:15:43.000000 dropchain-sdk-0.1.0/setup.cfg
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/
+-rw-r--r--   0 crazink    (501) staff       (20)      935 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 crazink    (501) staff       (20)     1069 2023-03-03 02:58:53.000000 dropchain-sdk-0.1.1/LICENSE.md
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/dropchain_sdk/
+-rw-r--r--   0 crazink    (501) staff       (20)    23896 2023-05-10 20:57:53.000000 dropchain-sdk-0.1.1/dropchain_sdk/__init__.py
+-rw-r--r--   0 crazink    (501) staff       (20)      436 2023-03-04 00:06:46.000000 dropchain-sdk-0.1.1/README.md
+-rw-r--r--   0 crazink    (501) staff       (20)      580 2023-05-10 20:58:22.000000 dropchain-sdk-0.1.1/setup.py
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/dropchain_sdk.egg-info/
+-rw-r--r--   0 crazink    (501) staff       (20)      935 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/dropchain_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 crazink    (501) staff       (20)      239 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/dropchain_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 crazink    (501) staff       (20)        9 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/dropchain_sdk.egg-info/requires.txt
+-rw-r--r--   0 crazink    (501) staff       (20)       14 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/dropchain_sdk.egg-info/top_level.txt
+-rw-r--r--   0 crazink    (501) staff       (20)        1 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/dropchain_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 crazink    (501) staff       (20)       38 2023-05-10 20:58:47.000000 dropchain-sdk-0.1.1/setup.cfg
```

### Comparing `dropchain-sdk-0.1.0/PKG-INFO` & `dropchain-sdk-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropchain-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build robust web3 applications seamlessly using Python with existing frameworks.
 Home-page: https://github.com/cRazink/py_dropchain_sdk
 Author: DropChain Inc
 Author-email: carter@dropchain.network
 License: MIT
 Description: # Python DropChain SDK
```

### Comparing `dropchain-sdk-0.1.0/LICENSE.md` & `dropchain-sdk-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dropchain-sdk-0.1.0/dropchain_sdk/__init__.py` & `dropchain-sdk-0.1.1/dropchain_sdk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -348,27 +348,59 @@
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
+    def asset_indexer_lookup_testnet(self, receiver1_uid, session1_token, user1_uid):
+        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_indexer_lookup_testnet"
+
+        payload = {
+            "app_id": self.app_id,
+            "user1_uid": user1_uid,
+            "receiver1_uid": receiver1_uid
+        }
+
+        if session1_token is not None:
+            payload["session1_token"] = session1_token
+
+        response = requests.post(url, json=payload, headers=self.headers, timeout=30)
+
+        return response.json()
+
     def asset_indexer_dropnet(self, session1_token, user1_uid):
         url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_indexer_dropnet"
 
         payload = {
             "app_id": self.app_id,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
+        return response.json()
+
+    def asset_indexer_lookup_dropnet(self, receiver1_uid, session1_token, user1_uid):
+        url = "https://dropchain1.p.rapidapi.com/dropchain/v1/asset_indexer_lookup_dropnet"
+
+        payload = {
+            "app_id": self.app_id,
+            "user1_uid": user1_uid,
+            "receiver1_uid": receiver1_uid
+        }
+
+        if session1_token is not None:
+            payload["session1_token"] = session1_token
+
+        response = requests.post(url, json=payload, headers=self.headers, timeout=30)
+
         return response.json()
 
     def atomic_swap_testnet(self, asset1_amount_int, asset1_id, asset2_amount_int, asset2_id, receiver1_uid, receiver2_uid, transaction1_note, transaction2_note, session1_token, session2_token, user1_uid, user2_uid):
         url = "https://dropchain1.p.rapidapi.com/dropchain/v1/atomic_swap_testnet"
 
         payload = {
             "app_id": self.app_id,
```

### Comparing `dropchain-sdk-0.1.0/setup.py` & `dropchain-sdk-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setuptools.setup(
     name="dropchain-sdk",
-    version="0.1.0",
+    version="0.1.1",
     author="DropChain Inc",
     author_email="carter@dropchain.network",
     packages=["dropchain_sdk"],
     description="Build robust web3 applications seamlessly using Python with existing frameworks.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/cRazink/py_dropchain_sdk",
```

### Comparing `dropchain-sdk-0.1.0/dropchain_sdk.egg-info/PKG-INFO` & `dropchain-sdk-0.1.1/dropchain_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropchain-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Build robust web3 applications seamlessly using Python with existing frameworks.
 Home-page: https://github.com/cRazink/py_dropchain_sdk
 Author: DropChain Inc
 Author-email: carter@dropchain.network
 License: MIT
 Description: # Python DropChain SDK
```

