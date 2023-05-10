# Comparing `tmp/dxsp-2.2.0.tar.gz` & `tmp/dxsp-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.2.0.tar", max compression
+gzip compressed data, was "dxsp-2.2.1.tar", max compression
```

## Comparing `dxsp-2.2.0.tar` & `dxsp-2.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-10 10:23:33.435868 dxsp-2.2.0/LICENSE
--rw-r--r--   0        0        0     2605 2023-05-10 10:23:33.435868 dxsp-2.2.0/README.md
--rw-r--r--   0        0        0       86 2023-05-10 10:23:34.087875 dxsp-2.2.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-10 10:23:33.435868 dxsp-2.2.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-10 10:23:33.435868 dxsp-2.2.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-10 10:23:33.435868 dxsp-2.2.0/dxsp/config.py
--rw-r--r--   0        0        0     3432 2023-05-10 10:23:33.435868 dxsp-2.2.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28870 2023-05-10 10:23:33.435868 dxsp-2.2.0/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-10 10:23:34.087875 dxsp-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 10:32:15.868295 dxsp-2.2.1/LICENSE
+-rw-r--r--   0        0        0     2605 2023-05-10 10:32:15.868295 dxsp-2.2.1/README.md
+-rw-r--r--   0        0        0       86 2023-05-10 10:32:16.544314 dxsp-2.2.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/config.py
+-rw-r--r--   0        0        0     3432 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28843 2023-05-10 10:32:15.868295 dxsp-2.2.1/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-10 10:32:16.544314 dxsp-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 dxsp-2.2.1/PKG-INFO
```

### Comparing `dxsp-2.2.0/LICENSE` & `dxsp-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.0/README.md` & `dxsp-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.0/dxsp/assets/blockchains.py` & `dxsp-2.2.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.0/dxsp/default_settings.toml` & `dxsp-2.2.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.2.0/dxsp/main.py` & `dxsp-2.2.1/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,24 @@
 
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         # USER
         self.wallet_address = settings.dex_wallet_address
         self.private_key = settings.dex_private_key
 
-        # COINGECKO
+        # COINGECKO 🦎
         try:
             self.cg = CoinGeckoAPI()
             assetplatform = self.cg.get_asset_platforms()
             output_dict = [x for x in assetplatform if x['chain_identifier']
                            == int(self.chain_id)]
             self.cg_platform = output_dict[0]['id']
             self.logger.debug("cg_platform %s", self.cg_platform)
         except Exception as e:
-            self.logger.error("CoinGecko: %s", e)
-            return
+            self.logger.error("CG🦎: %s", e)
 
     async def get_quote(
                 self,
                 symbol
             ):
         self.logger.debug("get_quote")
         asset_in_address = await self.search_contract(symbol)
@@ -272,15 +271,15 @@
                 return self.w3.to_checksum_address(token_contract)
             self.logger.info("no contract found for %s", token)
         except Exception as e:
             self.logger.error("search_contract %s", e)
             return
 
     async def search_cg(self, token):
-        """🦎 search coingecko"""
+        """search coingecko"""
         try:
             search_results = self.cg.search(query=token)
             search_dict = search_results['coins']
             filtered_dict = [x for x in search_dict if
                              x['symbol'] == token.upper()]
             api_dict = [sub['api_symbol'] for sub in filtered_dict]
             for i in api_dict:
@@ -291,15 +290,15 @@
                 except KeyError:
                     pass
         except Exception as e:
             self.logger.error("search_cg %s", e)
             return
 
     async def search_cg_contract(self, token):
-        """🦎 search coingecko contract"""
+        """search coingecko contract"""
         try:
             coin_info = await self.search_cg(token)
             if coin_info is not None:
                 return coin_info['platforms'][f'{self.cg_platform}']
         except Exception as e:
             self.logger.error(" search_cg_contract: %s", e)
             return
```

### Comparing `dxsp-2.2.0/pyproject.toml` & `dxsp-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.2.0"
+version = "2.2.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.2.0/PKG-INFO` & `dxsp-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.2.0
+Version: 2.2.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

