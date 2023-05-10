# Comparing `tmp/dxsp-2.2.1.tar.gz` & `tmp/dxsp-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.2.1.tar", max compression
+gzip compressed data, was "dxsp-2.2.2.tar", max compression
```

## Comparing `dxsp-2.2.1.tar` & `dxsp-2.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-10 10:32:15.868295 dxsp-2.2.1/LICENSE
--rw-r--r--   0        0        0     2605 2023-05-10 10:32:15.868295 dxsp-2.2.1/README.md
--rw-r--r--   0        0        0       86 2023-05-10 10:32:16.544314 dxsp-2.2.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/config.py
--rw-r--r--   0        0        0     3432 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28843 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-10 10:32:16.544314 dxsp-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 11:05:15.055733 dxsp-2.2.2/LICENSE
+-rw-r--r--   0        0        0     2605 2023-05-10 11:05:15.055733 dxsp-2.2.2/README.md
+-rw-r--r--   0        0        0       86 2023-05-10 11:05:15.703731 dxsp-2.2.2/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/config.py
+-rw-r--r--   0        0        0     3432 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    29162 2023-05-10 11:05:15.055733 dxsp-2.2.2/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-10 11:05:15.703731 dxsp-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.2.2/PKG-INFO
```

### Comparing `dxsp-2.2.1/LICENSE` & `dxsp-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.1/README.md` & `dxsp-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.1/dxsp/assets/blockchains.py` & `dxsp-2.2.2/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.1/dxsp/default_settings.toml` & `dxsp-2.2.2/dxsp/default_settings.toml`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 [chain_56]
 dex_chain_id = 56
 dex_rpc = "https://rpc.ankr.com/bsc"
 dex_block_explorer_url = "https://api.bscscan.com/api?"
 dex_block_explorer_api =  ""
 dex_protocol_type = "uniswap_v2"
-dex_router_contract_addr = "0xca143ce32fe78f1f7019d7d551a6402fc5350c73" #pancakeswap V2
+dex_router_contract_addr = "0x10ED43C718714eb63d5aA57B78B54704E256024E" #pancakeswap V2
 dex_0x_url = "https://bsc.api.0x.org/"
 
 [chain_97]
 loglevel = "DEBUG"
 dex_chain_id = 97
 dex_rpc = "https://rpc.ankr.com/bsc_testnet_chapel"
 dex_block_explorer_url = "https://api-testnet.bscscan.com/api?"
```

### Comparing `dxsp-2.2.1/dxsp/main.py` & `dxsp-2.2.2/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,16 +375,17 @@
         except Exception as e:
             self.logger.error("get_approve %s", e)
             return None
 
     async def get_sign(self, order):
 
         try:
-            if not isinstance(order, dict):
-                raise ValueError("Transaction must be a dictionary")
+            # if not isinstance(order, dict):
+            #     raise ValueError("Transaction must be a dictionary")
+            self.logger.debug("get_sign: order %s", order)
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 order_params = {
                             'from': self.wallet_address,
                             'gas': await self.get_gas(order),
                             'gasPrice': await self.get_gasPrice(order),
                             'nonce': self.w3.eth.get_transaction_count(
                                 self.wallet_address),
@@ -544,23 +545,23 @@
 # uniswap v2 🦄
     async def get_quote_uniswap_v2(
         self,
         asset_in_address,
         asset_out_address,
         amount=1
     ):
+        self.logger.debug("get_quote_uniswap_v2")
         try:
             order_path_dex = [asset_out_address, asset_in_address]
             router_instance = await self.router()
-            order_min_amount = int(
-                router_instance.functions.getAmountsOut(
-                    amount,
-                    order_path_dex)
-                .call()[1])
-            return order_min_amount
+            get_amount = router_instance.functions.getAmountsOut(
+                amount,
+                order_path_dex).call()
+            self.logger.debug("get_amount: %s", get_amount)
+            return get_amount[1]
         except Exception as e:
             self.logger.error("get_quote_uniswap_v2 %s", e)
             return
 
     async def get_approve_uniswap(self, asset_out_address):
 
         try:
@@ -569,21 +570,24 @@
                 address=asset_out_address,
                 abi=asset_out_abi)
             approval_check = asset_out_contract.functions.allowance(
                             self.w3.to_checksum_address(self.wallet_address),
                             self.w3.to_checksum_address(
                                 settings.dex_router_contract_addr)
                             ).call()
+            self.logger.debug("approval_check %s", approval_check)
             if (approval_check == 0):
                 approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
                 approval_TX = asset_out_contract.functions.approve(
                                 self.w3.to_checksum_address(
                                     settings.dex_router_contract_addr),
                                 approved_amount)
+                self.logger.debug("approval_TX %s", approval_TX)
                 approval_txHash = await self.get_sign(approval_TX)
+                self.logger.debug("approval_txHash %s", approval_txHash)
                 approval_txHash_complete = (
                     self.w3.eth.wait_for_transaction_receipt(
                         approval_txHash,
                         timeout=120,
                         poll_latency=0.1))
                 return approval_txHash_complete
         except Exception as e:
```

### Comparing `dxsp-2.2.1/pyproject.toml` & `dxsp-2.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.2.1"
+version = "2.2.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.2.1/PKG-INFO` & `dxsp-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.2.1
+Version: 2.2.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

