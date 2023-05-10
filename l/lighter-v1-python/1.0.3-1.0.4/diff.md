# Comparing `tmp/lighter-v1-python-1.0.3.tar.gz` & `tmp/lighter-v1-python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lighter-v1-python-1.0.3.tar", last modified: Thu Mar 23 12:49:09 2023, max compression
+gzip compressed data, was "lighter-v1-python-1.0.4.tar", last modified: Wed May 10 17:47:00 2023, max compression
```

## Comparing `lighter-v1-python-1.0.3.tar` & `lighter-v1-python-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-03-23 12:49:09.526596 lighter-v1-python-1.0.3/
--rw-r--r--   0 ahmetavci   (501) staff       (20)    11357 2023-02-16 12:31:17.000000 lighter-v1-python-1.0.3/LICENSE
--rw-r--r--   0 ahmetavci   (501) staff       (20)     6233 2023-03-23 12:49:09.526464 lighter-v1-python-1.0.3/PKG-INFO
--rw-r--r--   0 ahmetavci   (501) staff       (20)     5419 2023-03-23 12:25:53.000000 lighter-v1-python-1.0.3/README.md
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-03-23 12:49:09.524467 lighter-v1-python-1.0.3/lighter/
--rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.3/lighter/__init__.py
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-03-23 12:49:09.524925 lighter-v1-python-1.0.3/lighter/abi/
--rw-r--r--   0 ahmetavci   (501) staff       (20)     4841 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.3/lighter/abi/erc20.json
--rw-r--r--   0 ahmetavci   (501) staff       (20)     5643 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.3/lighter/abi/factory.json
--rw-r--r--   0 ahmetavci   (501) staff       (20)    11602 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.3/lighter/abi/orderbook.json
--rw-r--r--   0 ahmetavci   (501) staff       (20)     9730 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.3/lighter/abi/router.json
--rw-r--r--   0 ahmetavci   (501) staff       (20)     1181 2023-02-16 12:32:00.000000 lighter-v1-python-1.0.3/lighter/constants.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)      869 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.3/lighter/errors.py
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-03-23 12:49:09.525117 lighter-v1-python-1.0.3/lighter/helpers/
--rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.3/lighter/helpers/__init__.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)      413 2023-03-22 12:52:18.000000 lighter-v1-python-1.0.3/lighter/helpers/request_helpers.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)     5322 2023-03-23 12:19:17.000000 lighter-v1-python-1.0.3/lighter/lighter_client.py
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-03-23 12:49:09.525428 lighter-v1-python-1.0.3/lighter/modules/
--rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.3/lighter/modules/__init__.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)     9492 2023-03-22 12:51:32.000000 lighter-v1-python-1.0.3/lighter/modules/api.py
--rw-r--r--   0 ahmetavci   (501) staff       (20)    58598 2023-03-22 17:06:48.000000 lighter-v1-python-1.0.3/lighter/modules/blockchain.py
-drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-03-23 12:49:09.526301 lighter-v1-python-1.0.3/lighter_v1_python.egg-info/
--rw-r--r--   0 ahmetavci   (501) staff       (20)     6233 2023-03-23 12:49:09.000000 lighter-v1-python-1.0.3/lighter_v1_python.egg-info/PKG-INFO
--rw-r--r--   0 ahmetavci   (501) staff       (20)      558 2023-03-23 12:49:09.000000 lighter-v1-python-1.0.3/lighter_v1_python.egg-info/SOURCES.txt
--rw-r--r--   0 ahmetavci   (501) staff       (20)        1 2023-03-23 12:49:09.000000 lighter-v1-python-1.0.3/lighter_v1_python.egg-info/dependency_links.txt
--rw-r--r--   0 ahmetavci   (501) staff       (20)      194 2023-03-23 12:49:09.000000 lighter-v1-python-1.0.3/lighter_v1_python.egg-info/requires.txt
--rw-r--r--   0 ahmetavci   (501) staff       (20)        8 2023-03-23 12:49:09.000000 lighter-v1-python-1.0.3/lighter_v1_python.egg-info/top_level.txt
--rw-r--r--   0 ahmetavci   (501) staff       (20)       38 2023-03-23 12:49:09.526638 lighter-v1-python-1.0.3/setup.cfg
--rw-r--r--   0 ahmetavci   (501) staff       (20)     1426 2023-03-23 12:27:44.000000 lighter-v1-python-1.0.3/setup.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.294110 lighter-v1-python-1.0.4/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)    11357 2023-02-16 12:31:17.000000 lighter-v1-python-1.0.4/LICENSE
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     6233 2023-05-10 17:47:00.293979 lighter-v1-python-1.0.4/PKG-INFO
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     5419 2023-03-27 10:20:02.000000 lighter-v1-python-1.0.4/README.md
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.292082 lighter-v1-python-1.0.4/lighter/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/__init__.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.292571 lighter-v1-python-1.0.4/lighter/abi/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     4841 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/abi/erc20.json
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     5643 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/abi/factory.json
+-rw-r--r--   0 ahmetavci   (501) staff       (20)    11602 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/abi/orderbook.json
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     9730 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/abi/router.json
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     1158 2023-05-10 17:43:58.000000 lighter-v1-python-1.0.4/lighter/constants.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)      869 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/errors.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.292779 lighter-v1-python-1.0.4/lighter/helpers/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/helpers/__init__.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)      413 2023-03-27 10:20:02.000000 lighter-v1-python-1.0.4/lighter/helpers/request_helpers.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     5319 2023-05-10 17:43:58.000000 lighter-v1-python-1.0.4/lighter/lighter_client.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.293119 lighter-v1-python-1.0.4/lighter/modules/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        0 2023-02-03 14:27:54.000000 lighter-v1-python-1.0.4/lighter/modules/__init__.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     9492 2023-03-27 10:20:02.000000 lighter-v1-python-1.0.4/lighter/modules/api.py
+-rw-r--r--   0 ahmetavci   (501) staff       (20)    58421 2023-05-10 17:43:58.000000 lighter-v1-python-1.0.4/lighter/modules/blockchain.py
+drwxr-xr-x   0 ahmetavci   (501) staff       (20)        0 2023-05-10 17:47:00.293822 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     6233 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/PKG-INFO
+-rw-r--r--   0 ahmetavci   (501) staff       (20)      558 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        1 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmetavci   (501) staff       (20)      194 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/requires.txt
+-rw-r--r--   0 ahmetavci   (501) staff       (20)        8 2023-05-10 17:47:00.000000 lighter-v1-python-1.0.4/lighter_v1_python.egg-info/top_level.txt
+-rw-r--r--   0 ahmetavci   (501) staff       (20)       38 2023-05-10 17:47:00.294149 lighter-v1-python-1.0.4/setup.cfg
+-rw-r--r--   0 ahmetavci   (501) staff       (20)     1426 2023-05-10 17:46:45.000000 lighter-v1-python-1.0.4/setup.py
```

### Comparing `lighter-v1-python-1.0.3/LICENSE` & `lighter-v1-python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/PKG-INFO` & `lighter-v1-python-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighter-v1-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: lighter Python rest api and blockchain interactions for Limit Orders
 Home-page: https://github.com/elliottech/lighter-v1-python
 Author: Elliot
 Author-email: ahmet@elliot.ai
 License: Apache 2.0
 Keywords: lighter exchange rest api defi ethereum optimism l2 eth
 Classifier: Intended Audience :: Developers
```

### Comparing `lighter-v1-python-1.0.3/README.md` & `lighter-v1-python-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/lighter/abi/erc20.json` & `lighter-v1-python-1.0.4/lighter/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/lighter/abi/factory.json` & `lighter-v1-python-1.0.4/lighter/abi/factory.json`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/lighter/abi/orderbook.json` & `lighter-v1-python-1.0.4/lighter/abi/orderbook.json`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/lighter/abi/router.json` & `lighter-v1-python-1.0.4/lighter/abi/router.json`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/lighter/constants.py` & `lighter-v1-python-1.0.4/lighter/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,16 @@
 
 # ------------ Order Types -------------------
 ORDER_TYPE_LIMIT = "limit"
 ORDER_TYPE_MARKET = "market"
 
 
 # ------------ Ethereum Transactions ------------
-DEFAULT_GAS_AMOUNT = 250000
+DEFAULT_GAS_AMOUNT = 4000000
 DEFAULT_GAS_MULTIPLIER = 1.2
 DEFAULT_GAS_PRICE = 4000000000
 DEFAULT_MAX_FEE_PER_GAS = 2000000000
 DEFAULT_MAX_PRIORITY_FEE_PER_GAS = 0
-MAX_GAS_LIMIT = 4000000
 MAX_SOLIDITY_UINT = (
     115792089237316195423570985008687907853269984665640564039457584007913129639935
 )
 DEFAULT_API_TIMEOUT = 3000
```

### Comparing `lighter-v1-python-1.0.3/lighter/errors.py` & `lighter-v1-python-1.0.4/lighter/errors.py`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/lighter/lighter_client.py` & `lighter-v1-python-1.0.4/lighter/lighter_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         api_auth: str,
         web3_provider_url: str,
         private_key: Optional[str] = None,
         host: Optional[str] = None,
         send_options: Optional[dict] = {},
         api_timeout: Optional[int] = None,
     ):
-
         self.host = host or HOST
 
         if self.host.endswith("/"):
             self.host = self.host[:-1]
 
         self.private_key = private_key
         self.api_timeout = api_timeout or DEFAULT_API_TIMEOUT
@@ -72,15 +71,14 @@
     def blockchain(self):
         """
         Get the blockchain module, used for interracting with contracts.
         """
 
         if not self._blockchain:
             if self.web3 and self.private_key:
-
                 orderbooks: List[Orderbook] = self.api.get_orderbook_meta()[
                     "orderbookmetas"
                 ]
 
                 chains = self.api.get_blockchains()["blockchains"]
 
                 chain = next(
@@ -120,15 +118,14 @@
     def async_blockchain(self) -> AsyncBlockchain:
         """
         Get the blockchain module, used for interracting with contracts.
         """
 
         if not self._async_blockchain:
             if self.async_web3 and self.private_key:
-
                 orderbooks: List[Orderbook] = self.api.get_orderbook_meta()[
                     "orderbookmetas"
                 ]
 
                 chains = self.api.get_blockchains()["blockchains"]
 
                 chain = next(
```

### Comparing `lighter-v1-python-1.0.3/lighter/modules/api.py` & `lighter-v1-python-1.0.4/lighter/modules/api.py`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/lighter/modules/blockchain.py` & `lighter-v1-python-1.0.4/lighter/modules/blockchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from eth_account.datastructures import SignedTransaction
 from decimal import Decimal
 from web3.logs import DISCARD
 import asyncio
 import nest_asyncio
 
 from lighter.constants import DEFAULT_GAS_AMOUNT
-from lighter.constants import MAX_GAS_LIMIT
 from lighter.constants import DEFAULT_MAX_PRIORITY_FEE_PER_GAS
 from lighter.constants import DEFAULT_GAS_MULTIPLIER
 from lighter.constants import DEFAULT_MAX_FEE_PER_GAS
 from lighter.constants import MAX_SOLIDITY_UINT
 from lighter.errors import TransactionReverted
 from collections.abc import Iterable
 
@@ -621,18 +620,14 @@
             options["value"] = 0
         gas_multiplier = options.pop("gasMultiplier", DEFAULT_GAS_MULTIPLIER)
         options["maxFeePerGas"] = DEFAULT_MAX_FEE_PER_GAS
         options["maxPriorityFeePerGas"] = DEFAULT_MAX_PRIORITY_FEE_PER_GAS
         if "gas" not in options and method:
             try:
                 options["gas"] = int(method.estimate_gas(options) * gas_multiplier)
-                if options["gas"] > MAX_GAS_LIMIT:
-                    raise ValueError(
-                        "Gas limit exceeded, try with less number of operations in a batch transaction."
-                    )
             except Exception:
                 options["gas"] = DEFAULT_GAS_AMOUNT
 
         signed = await self._sign_tx(method, options)
         try:
             tx_hash = await self.web3.eth.send_raw_transaction(signed.rawTransaction)
         except ValueError as error:
@@ -853,14 +848,15 @@
     # -----------------------------------------------------------
     async def create_limit_order_batch(
         self,
         orderbook_symbol: str,
         human_readable_sizes: List[str],
         human_readable_prices: List[str],
         sides: List[OrderSide],
+        options: Dict[str, Any] = {},
     ) -> HexBytes:
         if not all(isinstance(x, str) for x in human_readable_sizes):
             raise ValueError("Invalid size, size should be string")
         if not all(isinstance(x, str) for x in human_readable_prices):
             raise ValueError("Invalid price, price should be string")
 
         self._tick_check(human_readable_sizes, human_readable_prices, orderbook_symbol)
@@ -892,28 +888,27 @@
                 amount_bases, price_bases, sides, hint_ids
             )
         )
 
         data = "0x01{:02x}{:02x}{}".format(orderbook["id"], len(sizes), orders_data)
 
         options = dict(
-            to=(await self.router_contract).address,
-            data=data,
-            gas=4000000,
+            to=(await self.router_contract).address, data=data, **(options or {})
         )
 
         return await self._send_eth_transaction(options=options)
 
     async def update_limit_order_batch(
         self,
         orderbook_symbol: str,
         order_ids: List[int],
         human_readable_sizes: List[str],
         human_readable_prices: List[str],
         old_sides: List[OrderSide],
+        options: Dict[str, Any] = {},
     ) -> HexBytes:
         if not all(isinstance(x, str) for x in human_readable_sizes):
             raise ValueError("Invalid size, size should be string")
         if not all(isinstance(x, str) for x in human_readable_prices):
             raise ValueError("Invalid price, price should be string")
 
         self._tick_check(human_readable_sizes, human_readable_prices, orderbook_symbol)
@@ -946,44 +941,41 @@
                 order_ids, amount_bases, price_bases, hint_ids
             )
         )
 
         data = "0x02{:02x}{:02x}{}".format(orderbook["id"], len(sizes), orders_data)
 
         options = dict(
-            to=(await self.router_contract).address,
-            data=data,
-            gas=4000000,
+            to=(await self.router_contract).address, data=data, **(options or {})
         )
 
         return await self._send_eth_transaction(options=options)
 
     async def cancel_limit_order_batch(
-        self, orderbook_symbol: str, order_ids: List[int]
+        self, orderbook_symbol: str, order_ids: List[int], options: Dict[str, Any] = {}
     ) -> HexBytes:
         orderbook = self._get_orderbook(orderbook_symbol)
 
         orders_data = "".join("{:08x}".format(order_id) for order_id in order_ids)
 
         data = "0x03{:02x}{:02x}{}".format(orderbook["id"], len(order_ids), orders_data)
 
         options = dict(
-            to=(await self.router_contract).address,
-            data=data,
-            gas=4000000,
+            to=(await self.router_contract).address, data=data, **(options or {})
         )
 
         return await self._send_eth_transaction(options=options)
 
     async def create_market_order(
         self,
         orderbook_symbol: str,
         human_readable_size: str,
         human_readable_price: str,
         side: OrderSide,
+        options: Dict[str, Any] = {},
     ) -> HexBytes:
         self._tick_check(
             [human_readable_size], [human_readable_price], orderbook_symbol
         )
         orderbook = self._get_orderbook(orderbook_symbol)
 
         size = self._get_amount_from_human_readable(
@@ -999,17 +991,15 @@
         orders_data = "{:016x}{:016x}{:02x}".format(
             amount_base, price_base, side == OrderSide.SELL
         )
 
         data = "0x04{:02x}{}".format(orderbook["id"], orders_data)
 
         options = dict(
-            to=(await self.router_contract).address,
-            data=data,
-            gas=4000000,
+            to=(await self.router_contract).address, data=data, **(options or {})
         )
 
         return await self._send_eth_transaction(options=options)
 
     async def set_token_max_allowance(
         self,
         spender: str,
@@ -1266,28 +1256,31 @@
                 "options['from'] is not set, and no default address is set",
             )
         auto_detect_nonce = "nonce" not in options
         if auto_detect_nonce:
             options["nonce"] = self._get_next_nonce(options["from"])
         if "value" not in options:
             options["value"] = 0
+
         gas_multiplier = options.pop("gasMultiplier", DEFAULT_GAS_MULTIPLIER)
-        options["maxFeePerGas"] = DEFAULT_MAX_FEE_PER_GAS
-        options["maxPriorityFeePerGas"] = DEFAULT_MAX_PRIORITY_FEE_PER_GAS
-        if "gas" not in options and method:
-            try:
-                options["gas"] = int(method.estimate_gas(options) * gas_multiplier)
-                if options["gas"] > MAX_GAS_LIMIT:
-                    raise ValueError(
-                        "Gas limit exceeded, try with less number of operations in a batch transaction."
-                    )
-            except Exception:
+        if "maxFeePerGas" not in options:
+            options["maxFeePerGas"] = DEFAULT_MAX_FEE_PER_GAS
+        if "maxPriorityFeePerGas" not in options:
+            options["maxPriorityFeePerGas"] = DEFAULT_MAX_PRIORITY_FEE_PER_GAS
+        if "gas" not in options:
+            if not method:
                 options["gas"] = DEFAULT_GAS_AMOUNT
+            else:
+                try:
+                    options["gas"] = int(method.estimate_gas(options) * gas_multiplier)
+                except Exception:
+                    options["gas"] = DEFAULT_GAS_AMOUNT
 
         signed = self._sign_tx(method, options)
+
         try:
             tx_hash = self.web3.eth.send_raw_transaction(signed.rawTransaction)
         except ValueError as error:
             retry_count = 0
             while retry_count < 3:
                 if auto_detect_nonce and (
                     "nonce too low" in str(error)
@@ -1504,14 +1497,15 @@
     # -----------------------------------------------------------
     def create_limit_order_batch(
         self,
         orderbook_symbol: str,
         human_readable_sizes: List[str],
         human_readable_prices: List[str],
         sides: List[OrderSide],
+        options: Dict[str, Any] = {},
     ) -> HexBytes:
         if not all(isinstance(x, str) for x in human_readable_sizes):
             raise ValueError("Invalid size, size should be string")
         if not all(isinstance(x, str) for x in human_readable_prices):
             raise ValueError("Invalid price, price should be string")
 
         self._tick_check(human_readable_sizes, human_readable_prices, orderbook_symbol)
@@ -1540,29 +1534,26 @@
             for amount_base, price_base, side, hint_id in zip(
                 amount_bases, price_bases, sides, hint_ids
             )
         )
 
         data = "0x01{:02x}{:02x}{}".format(orderbook["id"], len(sizes), orders_data)
 
-        options = dict(
-            to=self.router_contract.address,
-            data=data,
-            gas=4000000,
-        )
+        options = dict(to=self.router_contract.address, data=data, **(options or {}))
 
         return self._send_eth_transaction(options=options)
 
     def update_limit_order_batch(
         self,
         orderbook_symbol: str,
         order_ids: List[int],
         human_readable_sizes: List[str],
         human_readable_prices: List[str],
         old_sides: List[OrderSide],
+        options: Dict[str, Any] = {},
     ) -> HexBytes:
         if not all(isinstance(x, str) for x in human_readable_sizes):
             raise ValueError("Invalid size, size should be string")
         if not all(isinstance(x, str) for x in human_readable_prices):
             raise ValueError("Invalid price, price should be string")
 
         self._tick_check(human_readable_sizes, human_readable_prices, orderbook_symbol)
@@ -1594,45 +1585,42 @@
             for order_id, amount_base, price_base, hint_id in zip(
                 order_ids, amount_bases, price_bases, hint_ids
             )
         )
 
         data = "0x02{:02x}{:02x}{}".format(orderbook["id"], len(sizes), orders_data)
 
-        options = dict(
-            to=self.router_contract.address,
-            data=data,
-            gas=4000000,
-        )
+        options = dict(to=self.router_contract.address, data=data, **(options or {}))
 
         return self._send_eth_transaction(options=options)
 
     def cancel_limit_order_batch(
-        self, orderbook_symbol: str, order_ids: List[int]
+        self, orderbook_symbol: str, order_ids: List[int], options: Dict[str, Any] = {}
     ) -> HexBytes:
         orderbook = self._get_orderbook(orderbook_symbol)
 
         orders_data = "".join("{:08x}".format(order_id) for order_id in order_ids)
 
         data = "0x03{:02x}{:02x}{}".format(orderbook["id"], len(order_ids), orders_data)
 
         options = dict(
             to=self.router_contract.address,
             data=data,
-            gas=4000000,
+            **(options or {}),
         )
 
         return self._send_eth_transaction(options=options)
 
     def create_market_order(
         self,
         orderbook_symbol: str,
         human_readable_size: str,
         human_readable_price: str,
         side: OrderSide,
+        options: Dict[str, Any] = {},
     ) -> HexBytes:
         self._tick_check(
             [human_readable_size], [human_readable_price], orderbook_symbol
         )
         orderbook = self._get_orderbook(orderbook_symbol)
 
         size = self._get_amount_from_human_readable(
@@ -1647,19 +1635,15 @@
 
         orders_data = "{:016x}{:016x}{:02x}".format(
             amount_base, price_base, side == OrderSide.SELL
         )
 
         data = "0x04{:02x}{}".format(orderbook["id"], orders_data)
 
-        options = dict(
-            to=self.router_contract.address,
-            data=data,
-            gas=4000000,
-        )
+        options = dict(to=self.router_contract.address, data=data, **(options or {}))
 
         return self._send_eth_transaction(options=options)
 
     def set_token_max_allowance(
         self,
         spender: str,
         token: str,
```

### Comparing `lighter-v1-python-1.0.3/lighter_v1_python.egg-info/PKG-INFO` & `lighter-v1-python-1.0.4/lighter_v1_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lighter-v1-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: lighter Python rest api and blockchain interactions for Limit Orders
 Home-page: https://github.com/elliottech/lighter-v1-python
 Author: Elliot
 Author-email: ahmet@elliot.ai
 License: Apache 2.0
 Keywords: lighter exchange rest api defi ethereum optimism l2 eth
 Classifier: Intended Audience :: Developers
```

### Comparing `lighter-v1-python-1.0.3/lighter_v1_python.egg-info/SOURCES.txt` & `lighter-v1-python-1.0.4/lighter_v1_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lighter-v1-python-1.0.3/setup.py` & `lighter-v1-python-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "dateparser>=1.0.0",
     "nest-asyncio>=1.5.6",
     "pytest-asyncio>=0.21.0",
 ]
 
 setup(
     name="lighter-v1-python",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     package_data={
         "lighter": [
             "abi/*.json",
         ],
     },
     description="lighter Python rest api and blockchain interactions for Limit Orders",
```

