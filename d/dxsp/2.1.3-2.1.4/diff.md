# Comparing `tmp/dxsp-2.1.3.tar.gz` & `tmp/dxsp-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.1.3.tar", max compression
+gzip compressed data, was "dxsp-2.1.4.tar", max compression
```

## Comparing `dxsp-2.1.3.tar` & `dxsp-2.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-09 21:06:58.236220 dxsp-2.1.3/LICENSE
--rw-r--r--   0        0        0     2595 2023-05-09 21:06:58.236220 dxsp-2.1.3/README.md
--rw-r--r--   0        0        0       86 2023-05-09 21:06:58.956220 dxsp-2.1.3/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-09 21:06:58.236220 dxsp-2.1.3/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-09 21:06:58.236220 dxsp-2.1.3/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-09 21:06:58.236220 dxsp-2.1.3/dxsp/config.py
--rw-r--r--   0        0        0     3337 2023-05-09 21:06:58.236220 dxsp-2.1.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26060 2023-05-09 21:06:58.236220 dxsp-2.1.3/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-09 21:06:58.956220 dxsp-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 dxsp-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 08:12:35.286986 dxsp-2.1.4/LICENSE
+-rw-r--r--   0        0        0     2605 2023-05-10 08:12:35.286986 dxsp-2.1.4/README.md
+-rw-r--r--   0        0        0       86 2023-05-10 08:12:36.186998 dxsp-2.1.4/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-10 08:12:35.286986 dxsp-2.1.4/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-10 08:12:35.286986 dxsp-2.1.4/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-10 08:12:35.286986 dxsp-2.1.4/dxsp/config.py
+-rw-r--r--   0        0        0     3337 2023-05-10 08:12:35.286986 dxsp-2.1.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28019 2023-05-10 08:12:35.286986 dxsp-2.1.4/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-10 08:12:36.186998 dxsp-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.1.4/PKG-INFO
```

### Comparing `dxsp-2.1.3/LICENSE` & `dxsp-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.3/README.md` & `dxsp-2.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 # DXSP (DeX SwaP)
 
-
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy. |
 | ------------- | ------------- |
 |[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
-
-
 Key features:
 
 - Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
 - 2 swap protocol type supported:
-	- 1inch API v5
-	- Uniswap version 2 router protocol type
+  - Uniswap version 2 router protocol type
+  - 1inch API v5
 
 Other features:
-- Translate token symbol to contract address via user defined tokenlist format or coingecko api 
-- Connect to web3 if no web3 object or no rpc provided
-- Able to approve contract and sign transaction
-- Quote for a given token
-- Use Base symbol like stablecoin
-- Settings to use the modile for your own tool/bot
 
+- Translate token symbol to contract address via user defined tokenlist format or coingecko api
+- Connect to web3 automatically (optionn to provide a web3 object)
+- Approve contract and sign transaction
+- Quote a given token
+- Use Base trading symbol like stablecoin
+- Settings to use the module for your own setup
 
 # Install
+
 `pip install dxsp`
 
 # How to use it
+
 ```
 from dxsp import DexSwap
 
-	dex = DexSwap()
-	#BUY 10 USDC to SWAP with BITCOIN
-	demo_tx = await dex.get_swap('USDT','wBTC',10)
-	print("demo_tx ", demo_tx)
+ dex = DexSwap()
+ #BUY 10 USDC to SWAP with BITCOIN
+ demo_tx = await dex.get_swap('USDT','wBTC',10)
+ print("demo_tx ", demo_tx)
 ```
+
 ## Example
+
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
 
 ## Real use case
-[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
+[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
 # Documentation
-https://github.com/mraniki/dxsp/wiki
+
+<https://github.com/mraniki/dxsp/wiki>
 
 ## 🚧 Roadmap
 
 [🚧 Roadmap](https://github.com/mraniki/dxsp/milestones)
 
-## Questions? Want to help? 
+## Questions? Want to help?
+
 [![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
 [![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
```

### Comparing `dxsp-2.1.3/dxsp/assets/blockchains.py` & `dxsp-2.1.4/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.1.3/dxsp/default_settings.toml` & `dxsp-2.1.4/dxsp/default_settings.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 
 #protocol specific
 #🦄1inch
 dex_1inch_url = "https://api.1inch.exchange/v5.0/"
 dex_1inch_limit_url = "https://limit-orders.1inch.io/v3.0/"
 #0️⃣0x
 dex_0x_url = "https://api.0x.org/mainnet/"
-dex_0x_limit_url = ""
+dex_0x_api_key = "" 
+
 #🪐apollo
 apollo_spot_api_key = ""
 apollo_spot_api_secret = ""
 apollo_future_api_key = ""
 apollo_future_api_secret = ""
 
 [chain_1]
```

### Comparing `dxsp-2.1.3/dxsp/main.py` & `dxsp-2.1.4/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,178 +42,48 @@
                            == int(self.chain_id)]
             self.cg_platform = output_dict[0]['id']
             self.logger.debug("cg_platform %s", self.cg_platform)
         except Exception as e:
             self.logger.error("CoinGecko: %s", e)
             return
 
-    async def _get(
-        self,
-        url,
-        params=None,
-        headers=None
-            ):
-        try:
-            self.logger.debug("url: %s", url)
-            self.logger.debug("_header: %s", settings.headers)
-            response = requests.get(
-                url,
-                params=params,
-                headers=settings.headers,
-                #headers={'User-Agent': 'Mozilla/5.0'},
-                timeout=10)
-            self.logger.debug("_response: %s", response)
-            if response:
-                #self.logger.debug("_json: %s", response.json())
-                return response.json()
-
-        except Exception as e:
-            self.logger.error("_get: %s", e)
-
-    async def router(self):
-        try:
-            router_abi = await self.get_abi(settings.dex_router_contract_addr)
-            self.logger.debug("router_abi: %s", router_abi)
-            router = self.w3.eth.contract(
-                self.w3.to_checksum_address(
-                    settings.dex_router_contract_addr),
-                router_abi)
-            return router
-        except Exception as e:
-            self.logger.error("router setup: %s", e)
-
     async def get_quote(
                 self,
                 symbol
             ):
         self.logger.debug("get_quote")
         asset_in_address = await self.search_contract(symbol)
         asset_out_symbol = settings.trading_quote_ccy
         asset_out_address = await self.search_contract(asset_out_symbol)
         if asset_out_address is None:
             self.logger.warning("No Valid Contract")
             return
         try:
             if self.protocol_type in ["1inch", "1inch_limit"]:
                 self.logger.debug("1inch getquote")
-                await self.oneinch_quote(
+                await self.get_quote_1inch(
                     asset_in_address,
                     asset_out_address)
             if self.protocol_type == "uniswap_v2":
                 self.logger.debug("uniswap_v2 getquote")
-                await self.uniswap_v2_quote(
+                await self.get_quote_uniswap_v2(
                     asset_in_address,
                     asset_out_address)
+            if self.protocol_type == "0x":
+                await self.get_quote_0x(
+                    symbol,
+                    asset_out_symbol,)
             if self.protocol_type == "uniswap_v3":
-                await self.uniswap_v3_quote(
+                await self.get_quote_uniswap_v3(
                     asset_in_address,
                     asset_out_address)
         except Exception as e:
             self.logger.error("get_quote %s", e)
             return
 
-    async def oneinch_quote(
-        self,
-        asset_in_address,
-        asset_out_address,
-        amount=1
-    ):
-        try:
-            asset_out_amount = self.w3.to_wei(amount, 'ether')
-            quote_url = (
-                settings.dex_1inch_url
-                + str(self.chain_id)
-                + "/quote?fromTokenAddress="
-                + str(asset_in_address)
-                + "&toTokenAddress="
-                + str(asset_out_address)
-                + "&amount="
-                + str(asset_out_amount))
-            quote_response = await self._get(quote_url)
-            self.logger.debug("quote_response %s", quote_response)
-            if quote_response:
-                quote_amount = quote_response['toTokenAmount']
-                self.logger.debug("quote_amount %s", quote_amount)
-                # quote_decimals = quote_response['fromToken']['decimals']
-                quote = self.w3.from_wei(int(quote_amount), 'ether')
-                # /(10 ** quote_decimals))
-                return round(quote, 2)
-        except Exception as e:
-            self.logger.error("oneinch_quote %s", e)
-
-    async def uniswap_v2_quote(
-        self,
-        asset_in_address,
-        asset_out_address,
-        amount=1
-    ):
-        try:
-            order_path_dex = [asset_out_address, asset_in_address]
-            router_instance = await self.router()
-            order_min_amount = int(
-                router_instance.functions.getAmountsOut(
-                    amount,
-                    order_path_dex)
-                .call()[1])
-            return order_min_amount
-        except Exception as e:
-            self.logger.error("uniswap_v2_quote %s", e)
-            return
-
-    async def uniswap_v3_quote(
-        self,
-        asset_in_address,
-        asset_out_address,
-        amount=1
-    ):
-        return
-
-    async def execute_order(self, order_params):
-        """execute swap function"""
-        action = order_params.get('action')
-        instrument = order_params.get('instrument')
-        quantity = order_params.get('quantity', 1)
-
-        try:
-            asset_out_symbol = (
-                settings.trading_quote_ccy if
-                action == "BUY" else instrument)
-            asset_in_symbol = (
-                instrument if action == "BUY"
-                else settings.trading_quote_ccy)
-            try:
-                asset_out_contract = await self.get_token_contract(
-                    asset_out_symbol)
-                asset_out_decimals = (
-                    asset_out_contract.functions.decimals().call()
-                    or 18)
-            except Exception as e:
-                self.logger.error("execute_order decimals: %s", e)
-                asset_out_decimals = 18
-            asset_out_balance = await self.get_token_balance(asset_out_symbol)
-
-            #  Amount to risk percentage - DEFAULT OPTION is 10%
-            asset_out_amount = (
-                (asset_out_balance) /
-                (settings.trading_risk_amount
-                 ** asset_out_decimals)
-                )*(float(quantity)/100)
-
-            order = await self.get_swap(
-                    asset_out_symbol,
-                    asset_in_symbol,
-                    asset_out_amount
-                    )
-            if order:
-                return order['confirmation']
-
-        except Exception as e:
-            self.logger.debug("error execute_order %s", e)
-            return "error processing order in DXSP"
-
     async def get_swap(
                 self,
                 asset_out_symbol: str,
                 asset_in_symbol: str,
                 amount: int,
                 ):
         """main swap function"""
@@ -250,32 +120,37 @@
                  (settings.trading_slippage/100)))
             self.logger.debug("order_amount %s", order_amount)
 
             # VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
             if (await self.get_approve(asset_out_address)) is None:
                 return
 
-            # 1INCH
-            if self.protocol_type in ["1inch"]:
-                swap_order = await self.oneinch_swap(
+            # UNISWAP V2
+            if self.protocol_type in ["uniswap_v2"]:
+                swap_order = await self.get_swap_uniswap_v2(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
-            # UNISWAP V2
-            if self.protocol_type in ["uniswap_v2"]:
-                swap_order = await self.uniswap_v2_swap(
+            # 0x
+            if self.protocol_type == "0x":
+                swap_order = await self.get_quote_0x(
+                    asset_in_symbol,
+                    asset_out_symbol,)
+                await self.get_sign(swap_order)
+
+            # 1INCH
+            if self.protocol_type in ["1inch"]:
+                swap_order = await self.get_swap_1inch(
                     asset_out_address,
                     asset_in_address,
                     order_amount)
-            # 1INCH LIMIT
-            if self.protocol_type in ["1inch_limit"]:
-                return
             # UNISWAP V3
             if self.protocol_type in ['uniswap_v3']:
-                swap_order = await self.uniswap_v3_swap()
+                swap_order = await self.get_swap_uniswap_v3()
+
             if swap_order:
                 self.logger.debug("swap_order %s", swap_order)
                 signed_order = await self.get_sign(swap_order)
                 order_hash = str(self.w3.to_hex(signed_order))
                 order_hash_details = self.w3.wait_for_transaction_receipt(
                                         order_hash,
                                         timeout=120,
@@ -287,65 +162,14 @@
                         asset_out_symbol,
                         asset_out_address,
                         order_amount,)
         except Exception as e:
             self.logger.error("get_swap %s", e)
             return
 
-    async def oneinch_swap(
-        self,
-        asset_out_address,
-        asset_in_address,
-        amount
-    ):
-        swap_url = (
-            settings.dex_1inch_url
-            + str(self.chain_id)
-            + "/swap?fromTokenAddress="
-            + asset_out_address
-            + "&toTokenAddress="
-            + asset_in_address
-            + "&amount="
-            + amount
-            + "&fromAddress="
-            + self.wallet_address
-            + "&slippage="
-            + settings.trading_slippage
-            )
-        swap_order = await self._get(swap_url)
-        swap_order_status = swap_order['statusCode']
-        if swap_order_status != 200:
-            return
-        return swap_order
-
-    async def uniswap_v2_swap(
-        self,
-        asset_out_address,
-        asset_in_address,
-        amount
-    ):
-        order_path_dex = [asset_out_address, asset_in_address]
-
-        deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
-        order_min_amount = self.uniswap_v2_quote(
-            asset_in_address,
-            asset_out_address)
-        router_instance = await self.router()
-        swap_order = router_instance.functions.swapExactTokensForTokens(
-                        amount,
-                        order_min_amount,
-                        order_path_dex,
-                        self.wallet_address,
-                        deadline)
-        return swap_order
-
-    async def uniswap_v3_swap(self):
-        self.logger.warning("Not available")
-        return
-
     async def get_confirmation(self,
                                order_hash,
                                order_hash_details,
                                asset_out_symbol,
                                asset_out_address,
                                order_amount,
                                ):
@@ -369,30 +193,58 @@
             trade['confirmation'] += f"🗓️ {trade['datetime']}"
             self.logger.info("trade %s", trade)
             return trade
         except Exception as e:
             self.logger.error("get_confirmation %s", e)
             return
 
-    async def get_block_explorer_status(self, txHash):
+    async def execute_order(self, order_params):
+        """execute swap function"""
+        action = order_params.get('action')
+        instrument = order_params.get('instrument')
+        quantity = order_params.get('quantity', 1)
+
         try:
-            if settings.block_explorer_api:
-                checkTransactionSuccessURL = (
-                    settings.block_explorer_url
-                    + "?module=transaction&action=gettxreceiptstatus&txhash="
-                    + str(txHash)
-                    + "&apikey="
-                    + str(settings.block_explorer_api))
-                checkTransactionRequest = self._get(checkTransactionSuccessURL)
-                return checkTransactionRequest['status']
+            asset_out_symbol = (
+                settings.trading_quote_ccy if
+                action == "BUY" else instrument)
+            asset_in_symbol = (
+                instrument if action == "BUY"
+                else settings.trading_quote_ccy)
+            try:
+                asset_out_contract = await self.get_token_contract(
+                    asset_out_symbol)
+                asset_out_decimals = (
+                    asset_out_contract.functions.decimals().call()
+                    or 18)
+            except Exception as e:
+                self.logger.error("execute_order decimals: %s", e)
+                asset_out_decimals = 18
+            asset_out_balance = await self.get_token_balance(asset_out_symbol)
+
+            #  Amount to risk percentage - DEFAULT OPTION is 10%
+            asset_out_amount = (
+                (asset_out_balance) /
+                (settings.trading_risk_amount
+                 ** asset_out_decimals)
+                )*(float(quantity)/100)
+
+            order = await self.get_swap(
+                    asset_out_symbol,
+                    asset_in_symbol,
+                    asset_out_amount
+                    )
+            if order:
+                return order['confirmation']
+
         except Exception as e:
-            self.logger.error("get_block_explorer_status %s", e)
-            return
+            self.logger.debug("error execute_order %s", e)
+            return "error processing order in DXSP"
 
-# ###CONTRACT SEARCH
+# 📝CONTRACT SEARCH
     async def search_contract(
                             self,
                             token
                             ):
         """search a contract function"""
         self.logger.debug("search_contract")
 
@@ -444,114 +296,88 @@
             coin_info = await self.search_cg(token)
             if coin_info is not None:
                 return coin_info['platforms'][f'{self.cg_platform}']
         except Exception as e:
             self.logger.error(" search_cg_contract: %s", e)
             return
 
-    async def get_contract_address(
-                            self,
-                            token_list_url,
-                            symbol
-                        ):
+    async def get_contract_address(self, token_list_url, symbol):
         """Given a token symbol and json tokenlist, get token address"""
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and
                    keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug("get_contract_address %s", e)
             return
 
-    async def get_token_contract(
-                                self,
-                                token
-                            ):
+    async def get_token_contract(self, token):
         """Given a token symbol, returns a contract object. """
         self.logger.debug("get_token_contract %s", token)
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(
                 address=token_address,
                 abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s", e)
             return
 
-# W3 UTILS
-    async def get_approve(self, asset_out_address):
+# 🛠️ W3 UTILS
+    async def _get(
+        self,
+        url,
+        params=None,
+        headers=None
+            ):
         try:
-            if self.protocol_type in ["1inch", "1inch_limit"]:
-                await self.get_approve_1inch(asset_out_address)
-            elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
-                await self.get_approve_uniswap(asset_out_address)
+            self.logger.debug("url: %s", url)
+            self.logger.debug("_header: %s", settings.headers)
+            response = requests.get(
+                url,
+                params=params,
+                headers=headers,
+                # headers={'User-Agent': 'Mozilla/5.0'},
+                timeout=10)
+            self.logger.debug("_response: %s", response)
+            if response:
+                # self.logger.debug("_json: %s", response.json())
+                return response.json()
+
         except Exception as e:
-            self.logger.error("get_approve %s", e)
-            return None
+            self.logger.error("_get: %s", e)
 
-    async def get_approve_1inch(self, asset_out_address):
+    async def router(self):
         try:
-            approval_check_URL = (
-                settings.dex_1inch_url
-                + str(self.chain_id)
-                + "/approve/allowance?tokenAddress="
-                + str(asset_out_address)
-                + "&walletAddress="
-                + str(self.wallet_address))
-            approval_response = await self._get(approval_check_URL)
-            approval_check = approval_response['allowance']
-            if (approval_check == 0):
-                approval_URL = (
-                    settings.dex_1inch_url
-                    + str(self.chain_id)
-                    + "/approve/transaction?tokenAddress="
-                    + str(asset_out_address))
-                approval_response = await self._get(approval_URL)
-                return approval_response
+            router_abi = await self.get_abi(settings.dex_router_contract_addr)
+            self.logger.debug("router_abi: %s", router_abi)
+            router = self.w3.eth.contract(
+                self.w3.to_checksum_address(
+                    settings.dex_router_contract_addr),
+                router_abi)
+            return router
         except Exception as e:
-            self.logger.error("get_approve_uniswap %s", e)
-            return None
+            self.logger.error("router setup: %s", e)
 
-    async def get_approve_uniswap(self, asset_out_address):
+    async def get_approve(self, asset_out_address):
 
         try:
-            asset_out_abi = await self.get_abi(asset_out_address)
-            asset_out_contract = self.w3.eth.contract(
-                address=asset_out_address,
-                abi=asset_out_abi)
-            approval_check = asset_out_contract.functions.allowance(
-                            self.w3.to_checksum_address(self.wallet_address),
-                            self.w3.to_checksum_address(
-                                settings.dex_router_contract_addr)
-                            ).call()
-            if (approval_check == 0):
-                approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
-                approval_TX = asset_out_contract.functions.approve(
-                                self.w3.to_checksum_address(
-                                    settings.router_contract_addr),
-                                approved_amount)
-                approval_txHash = await self.get_sign(approval_TX)
-                approval_txHash_complete = (
-                    self.w3.eth.wait_for_transaction_receipt(
-                        approval_txHash,
-                        timeout=120,
-                        poll_latency=0.1))
-                return approval_txHash_complete
+            if self.protocol_type in ["1inch", "1inch_limit"]:
+                await self.get_approve_1inch(asset_out_address)
+            elif self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
+                await self.get_approve_uniswap(asset_out_address)
         except Exception as e:
-            self.logger.error("get_approve_uniswap %s", e)
+            self.logger.error("get_approve %s", e)
             return None
 
-    async def get_sign(
-        self,
-        order
-         ):
+    async def get_sign(self, order):
 
         try:
             if not isinstance(order, dict):
                 raise ValueError("Transaction must be a dictionary")
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 order_params = {
                             'from': self.wallet_address,
@@ -628,15 +454,29 @@
                 self.logger.error("get_abi %s", e)
                 return None
         else:
             # If no block_explorer_api is set, log a warning
             self.logger.warning("No block_explorer_api.")
             return
 
-# USER BALANCE AND POSITION RELATED
+    async def get_block_explorer_status(self, txHash):
+        try:
+            if settings.block_explorer_api:
+                checkTransactionSuccessURL = (
+                    settings.block_explorer_url
+                    + "?module=transaction&action=gettxreceiptstatus&txhash="
+                    + str(txHash)
+                    + "&apikey="
+                    + str(settings.block_explorer_api))
+                checkTransactionRequest = self._get(checkTransactionSuccessURL)
+                return checkTransactionRequest['status']
+        except Exception as e:
+            self.logger.error("get_block_explorer_status %s", e)
+            return
+# 🔒 USER RELATED
 
     async def get_token_balance(
         self,
         token
          ):
 
         try:
@@ -692,7 +532,227 @@
 
         try:
             self.logger.debug("get_account_position")
             return
         except Exception as e:
             self.logger.error("get_account_position: %s", e)
             return 0
+
+# PROTOCOL SPECIFIC
+# uniswap v2 🦄
+    async def get_quote_uniswap_v2(
+        self,
+        asset_in_address,
+        asset_out_address,
+        amount=1
+    ):
+        try:
+            order_path_dex = [asset_out_address, asset_in_address]
+            router_instance = await self.router()
+            order_min_amount = int(
+                router_instance.functions.getAmountsOut(
+                    amount,
+                    order_path_dex)
+                .call()[1])
+            return order_min_amount
+        except Exception as e:
+            self.logger.error("get_quote_uniswap_v2 %s", e)
+            return
+
+    async def get_approve_uniswap(self, asset_out_address):
+
+        try:
+            asset_out_abi = await self.get_abi(asset_out_address)
+            asset_out_contract = self.w3.eth.contract(
+                address=asset_out_address,
+                abi=asset_out_abi)
+            approval_check = asset_out_contract.functions.allowance(
+                            self.w3.to_checksum_address(self.wallet_address),
+                            self.w3.to_checksum_address(
+                                settings.dex_router_contract_addr)
+                            ).call()
+            if (approval_check == 0):
+                approved_amount = (self.w3.to_wei(2**64-1, 'ether'))
+                approval_TX = asset_out_contract.functions.approve(
+                                self.w3.to_checksum_address(
+                                    settings.router_contract_addr),
+                                approved_amount)
+                approval_txHash = await self.get_sign(approval_TX)
+                approval_txHash_complete = (
+                    self.w3.eth.wait_for_transaction_receipt(
+                        approval_txHash,
+                        timeout=120,
+                        poll_latency=0.1))
+                return approval_txHash_complete
+        except Exception as e:
+            self.logger.error("get_approve_uniswap %s", e)
+            return None
+
+    async def get_swap_uniswap_v2(
+        self,
+        asset_out_address,
+        asset_in_address,
+        amount
+    ):
+        order_path_dex = [asset_out_address, asset_in_address]
+
+        deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
+        order_min_amount = self.get_quote_uniswap_v2(
+            asset_in_address,
+            asset_out_address)
+        router_instance = await self.router()
+        swap_order = router_instance.functions.swapExactTokensForTokens(
+                        amount,
+                        order_min_amount,
+                        order_path_dex,
+                        self.wallet_address,
+                        deadline)
+        return swap_order
+
+# uniswap v3 🦄
+    async def get_quote_uniswap_v3(
+        self,
+        asset_in_address,
+        asset_out_address,
+        amount=1
+    ):
+        return
+
+    async def get_swap_uniswap_v3(self):
+        self.logger.warning("Not available")
+        return
+
+# 0️⃣x
+    async def get_quote_0x(
+        self,
+        asset_in_address,
+        asset_out_address,
+        amount=1
+    ):
+        try:
+            asset_out_amount = self.w3.to_wei(amount, 'ether')
+
+            quote_url = (
+                settings.dex_0x_url
+                + "/swap/v1/quote?buyToken="
+                + str(asset_in_address)
+                + "&sellToken="
+                + str(asset_out_address)
+                + "&sellAmount="
+                + str(asset_out_amount))
+            quote_response = await self._get(
+                quote_url,
+                params=None,
+                headers={"0x-api-key": settings.dex_0x_api_key}
+                )
+            self.logger.debug("quote_response %s", quote_response)
+            if quote_response:
+                quote_amount = quote_response['guaranteedPrice']
+                self.logger.debug("quote_amount %s", quote_amount)
+                # quote_decimals = quote_response['fromToken']['decimals']
+                quote = self.w3.from_wei(int(quote_amount), 'ether')
+                # /(10 ** quote_decimals))
+                return round(quote, 2)
+        except Exception as e:
+            self.logger.error("get_quote_0x %s", e)
+
+# 1inch 🦄
+    async def get_quote_1inch(
+        self,
+        asset_in_address,
+        asset_out_address,
+        amount=1
+    ):
+        try:
+            asset_out_amount = self.w3.to_wei(amount, 'ether')
+            quote_url = (
+                settings.dex_1inch_url
+                + str(self.chain_id)
+                + "/quote?fromTokenAddress="
+                + str(asset_in_address)
+                + "&toTokenAddress="
+                + str(asset_out_address)
+                + "&amount="
+                + str(asset_out_amount))
+            quote_response = await self._get(
+                url=quote_url,
+                params=None,
+                headers=settings.headers)
+            self.logger.debug("quote_response %s", quote_response)
+            if quote_response:
+                quote_amount = quote_response['toTokenAmount']
+                self.logger.debug("quote_amount %s", quote_amount)
+                # quote_decimals = quote_response['fromToken']['decimals']
+                quote = self.w3.from_wei(int(quote_amount), 'ether')
+                # /(10 ** quote_decimals))
+                return round(quote, 2)
+        except Exception as e:
+            self.logger.error("get_quote_1inch %s", e)
+
+    async def get_approve_1inch(self, asset_out_address):
+        try:
+            approval_check_URL = (
+                settings.dex_1inch_url
+                + str(self.chain_id)
+                + "/approve/allowance?tokenAddress="
+                + str(asset_out_address)
+                + "&walletAddress="
+                + str(self.wallet_address))
+            approval_response = await self._get(
+                url=approval_check_URL,
+                params=None,
+                headers=settings.headers)
+            approval_check = approval_response['allowance']
+            if (approval_check == 0):
+                approval_URL = (
+                    settings.dex_1inch_url
+                    + str(self.chain_id)
+                    + "/approve/transaction?tokenAddress="
+                    + str(asset_out_address))
+                approval_response = await self._get(approval_URL)
+                return approval_response
+        except Exception as e:
+            self.logger.error("get_approve_1inch %s", e)
+            return None
+
+    async def get_swap_1inch(
+        self,
+        asset_out_address,
+        asset_in_address,
+        amount
+    ):
+        swap_url = (
+            settings.dex_1inch_url
+            + str(self.chain_id)
+            + "/swap?fromTokenAddress="
+            + asset_out_address
+            + "&toTokenAddress="
+            + asset_in_address
+            + "&amount="
+            + amount
+            + "&fromAddress="
+            + self.wallet_address
+            + "&slippage="
+            + settings.trading_slippage
+            )
+        swap_order = await self._get(
+            url=swap_url,
+            params=None,
+            headers=settings.headers  # headers={'User-Agent': 'Mozilla/5.0'},
+            )
+        swap_order_status = swap_order['statusCode']
+        if swap_order_status != 200:
+            return
+        return swap_order
+
+# apollo finance
+    async def get_quote_apollo(
+        self,
+        asset_in_address,
+        asset_out_address,
+        amount=1
+    ):
+        return
+
+    async def get_swap_apolllo(self):
+        self.logger.warning("Not available")
+        return
```

### Comparing `dxsp-2.1.3/pyproject.toml` & `dxsp-2.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.1.3"
+version = "2.1.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.1.3/PKG-INFO` & `dxsp-2.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.1.3
+Version: 2.1.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,60 +16,63 @@
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
 
-
 |<img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/231213427-63ea2752-13d5-4993-aee2-90671b57fc6e.png">  | A python defi swap helper package. Swap made easy. |
 | ------------- | ------------- |
 |[![Pypi](https://badgen.net/badge/icon/dxsp?icon=pypi&label)](https://pypi.org/project/dxsp/) ![Version](https://img.shields.io/pypi/v/dxsp)<br>  ![Pypi](https://img.shields.io/pypi/dm/dxsp) [![Docker Pulls](https://badgen.net/docker/pulls/mraniki/dxsp)](https://hub.docker.com/r/mraniki/dxsp)<br>[![✨Flow](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml/badge.svg)](https://github.com/mraniki/dxsp/actions/workflows/%E2%9C%A8Flow.yml) [![codecov](https://codecov.io/gh/mraniki/dxsp/branch/main/graph/badge.svg?token=39ED0ZA6IH)](https://codecov.io/gh/mraniki/dxsp) <br>![](https://healthchecks.io/badge/227be4cc-702a-4ac8-b37b-d3d5a3/UcTrNrys-2/dxsp.svg)<br>[![Web3](https://badgen.net/badge/icon/web3/black?icon=libraries&label)](https://github.com/ethereum/web3.py) [![coingecko](https://badgen.net/badge/icon/coingecko/black?icon=libraries&label)](https://github.com/coingecko)|24 blockchains (ETH, BSC, ARB, MATIC, OPT...)<br>2 swap protocol (1inch API, UniV2 router)
 
-
-
 Key features:
 
 - Any blockchains mainnet or testnet supported by web3py, 1inch or uniswap type router.
 - 2 swap protocol type supported:
-	- 1inch API v5
-	- Uniswap version 2 router protocol type
+  - Uniswap version 2 router protocol type
+  - 1inch API v5
 
 Other features:
-- Translate token symbol to contract address via user defined tokenlist format or coingecko api 
-- Connect to web3 if no web3 object or no rpc provided
-- Able to approve contract and sign transaction
-- Quote for a given token
-- Use Base symbol like stablecoin
-- Settings to use the modile for your own tool/bot
 
+- Translate token symbol to contract address via user defined tokenlist format or coingecko api
+- Connect to web3 automatically (optionn to provide a web3 object)
+- Approve contract and sign transaction
+- Quote a given token
+- Use Base trading symbol like stablecoin
+- Settings to use the module for your own setup
 
 # Install
+
 `pip install dxsp`
 
 # How to use it
+
 ```
 from dxsp import DexSwap
 
-	dex = DexSwap()
-	#BUY 10 USDC to SWAP with BITCOIN
-	demo_tx = await dex.get_swap('USDT','wBTC',10)
-	print("demo_tx ", demo_tx)
+ dex = DexSwap()
+ #BUY 10 USDC to SWAP with BITCOIN
+ demo_tx = await dex.get_swap('USDT','wBTC',10)
+ print("demo_tx ", demo_tx)
 ```
+
 ## Example
+
 [example](https://github.com/mraniki/dxsp/blob/main/examples/example.py)
 
 ## Real use case
-[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
+[TalkyTrader, submit trading order to CEX & DEX with messaging platform (Telegram, Matrix and Discord)](https://github.com/mraniki/tt)
 
 # Documentation
-https://github.com/mraniki/dxsp/wiki
+
+<https://github.com/mraniki/dxsp/wiki>
 
 ## 🚧 Roadmap
 
 [🚧 Roadmap](https://github.com/mraniki/dxsp/milestones)
 
-## Questions? Want to help? 
+## Questions? Want to help?
+
 [![discord](https://badgen.net/badge/icon/discord/purple?icon=discord&label)](https://discord.gg/vegJQGrRRa)
 [![telegram](https://badgen.net/badge/icon/telegram?icon=telegram&label)](https://t.me/TTTalkyTraderChat/1)
```

