# Comparing `tmp/dxsp-2.1.5.tar.gz` & `tmp/dxsp-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.1.5.tar", max compression
+gzip compressed data, was "dxsp-2.1.6.tar", max compression
```

## Comparing `dxsp-2.1.5.tar` & `dxsp-2.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-10 09:25:19.421315 dxsp-2.1.5/LICENSE
--rw-r--r--   0        0        0     2605 2023-05-10 09:25:19.421315 dxsp-2.1.5/README.md
--rw-r--r--   0        0        0       86 2023-05-10 09:25:20.217363 dxsp-2.1.5/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-10 09:25:19.421315 dxsp-2.1.5/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-10 09:25:19.421315 dxsp-2.1.5/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-10 09:25:19.421315 dxsp-2.1.5/dxsp/config.py
--rw-r--r--   0        0        0     3365 2023-05-10 09:25:19.425315 dxsp-2.1.5/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28027 2023-05-10 09:25:19.425315 dxsp-2.1.5/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-10 09:25:20.217363 dxsp-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 09:59:58.534048 dxsp-2.1.6/LICENSE
+-rw-r--r--   0        0        0     2605 2023-05-10 09:59:58.534048 dxsp-2.1.6/README.md
+-rw-r--r--   0        0        0       86 2023-05-10 09:59:59.370071 dxsp-2.1.6/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-10 09:59:58.534048 dxsp-2.1.6/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-10 09:59:58.534048 dxsp-2.1.6/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-10 09:59:58.534048 dxsp-2.1.6/dxsp/config.py
+-rw-r--r--   0        0        0     3365 2023-05-10 09:59:58.534048 dxsp-2.1.6/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28043 2023-05-10 09:59:58.534048 dxsp-2.1.6/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-10 09:59:59.370071 dxsp-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.1.6/PKG-INFO
```

### Comparing `dxsp-2.1.5/LICENSE` & `dxsp-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.5/README.md` & `dxsp-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.5/dxsp/assets/blockchains.py` & `dxsp-2.1.6/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.5/dxsp/default_settings.toml` & `dxsp-2.1.6/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.5/dxsp/main.py` & `dxsp-2.1.6/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,17 +351,17 @@
             self.logger.error("_get: %s", e)
 
     async def router(self):
         try:
             router_abi = await self.get_abi(settings.dex_router_contract_addr)
             self.logger.debug("router_abi: %s", router_abi)
             router = self.w3.eth.contract(
-                self.w3.to_checksum_address(
+                address=self.w3.to_checksum_address(
                     settings.dex_router_contract_addr),
-                router_abi)
+                abi=router_abi)
             return router
         except Exception as e:
             self.logger.error("router setup: %s", e)
 
     async def get_approve(self, asset_out_address):
 
         try:
@@ -570,15 +570,15 @@
                             self.w3.to_checksum_address(
                                 settings.dex_router_contract_addr)
                             ).call()
             if (approval_check == 0):
                 approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
                 approval_TX = asset_out_contract.functions.approve(
                                 self.w3.to_checksum_address(
-                                    settings.router_contract_addr),
+                                    settings.dex_router_contract_addr),
                                 approved_amount)
                 approval_txHash = await self.get_sign(approval_TX)
                 approval_txHash_complete = (
                     self.w3.eth.wait_for_transaction_receipt(
                         approval_txHash,
                         timeout=120,
                         poll_latency=0.1))
```

### Comparing `dxsp-2.1.5/pyproject.toml` & `dxsp-2.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.1.5"
+version = "2.1.6"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.1.5/PKG-INFO` & `dxsp-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.1.5
+Version: 2.1.6
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

