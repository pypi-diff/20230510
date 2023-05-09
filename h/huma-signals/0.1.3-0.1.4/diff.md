# Comparing `tmp/huma_signals-0.1.3.tar.gz` & `tmp/huma_signals-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_signals-0.1.3.tar", max compression
+gzip compressed data, was "huma_signals-0.1.4.tar", max compression
```

## Comparing `huma_signals-0.1.3.tar` & `huma_signals-0.1.4.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0    34523 2023-05-06 00:10:02.616918 huma_signals-0.1.3/LICENSE
--rw-r--r--   0        0        0     2173 2023-05-06 00:10:02.617080 huma_signals-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617555 huma_signals-0.1.3/huma_signals/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617626 huma_signals-0.1.3/huma_signals/api/__init__.py
--rw-r--r--   0        0        0     1187 2023-05-06 00:10:02.617701 huma_signals-0.1.3/huma_signals/api/exception_handlers.py
--rw-r--r--   0        0        0      997 2023-05-06 00:10:02.617769 huma_signals-0.1.3/huma_signals/api/main.py
--rw-r--r--   0        0        0      289 2023-05-06 00:10:02.617834 huma_signals-0.1.3/huma_signals/api/models.py
--rw-r--r--   0        0        0     1114 2023-05-06 00:10:02.617904 huma_signals-0.1.3/huma_signals/api/views.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617961 huma_signals-0.1.3/huma_signals/commons/__init__.py
--rw-r--r--   0        0        0      812 2023-05-06 00:10:02.618029 huma_signals-0.1.3/huma_signals/commons/chains.py
--rw-r--r--   0        0        0      330 2023-05-06 00:10:02.618090 huma_signals-0.1.3/huma_signals/commons/datetime_utils.py
--rw-r--r--   0        0        0      227 2023-05-06 00:10:02.618146 huma_signals-0.1.3/huma_signals/commons/pydantic_utils.py
--rw-r--r--   0        0        0      569 2023-05-06 00:10:02.618202 huma_signals-0.1.3/huma_signals/commons/string_utils.py
--rw-r--r--   0        0        0     1309 2023-05-06 00:10:02.618262 huma_signals-0.1.3/huma_signals/commons/tokens.py
--rw-r--r--   0        0        0     1078 2023-05-06 00:10:02.618330 huma_signals-0.1.3/huma_signals/commons/web3_utils.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618388 huma_signals-0.1.3/huma_signals/domain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618462 huma_signals-0.1.3/huma_signals/domain/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618534 huma_signals-0.1.3/huma_signals/domain/adapters/allowlist/__init__.py
--rw-r--r--   0        0        0     1755 2023-05-06 00:10:02.618617 huma_signals-0.1.3/huma_signals/domain/adapters/allowlist/adapter.py
--rw-r--r--   0        0        0      589 2023-05-06 00:10:02.618719 huma_signals-0.1.3/huma_signals/domain/adapters/ethereum_wallet/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618750 huma_signals-0.1.3/huma_signals/domain/adapters/ethereum_wallet/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-09 22:56:01.650045 huma_signals-0.1.3/huma_signals/domain/adapters/ethereum_wallet/adapter.py
--rw-r--r--   0        0        0      186 2023-05-09 22:56:01.650122 huma_signals-0.1.3/huma_signals/domain/adapters/ethereum_wallet/settings.py
--rw-r--r--   0        0        0      589 2023-05-06 00:10:02.618984 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.619013 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/__init__.py
--rw-r--r--   0        0        0    23699 2023-05-06 00:10:02.619139 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/abi/BaseCreditPool.json
--rw-r--r--   0        0        0    30632 2023-05-06 00:10:02.619304 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/abi/BasePoolConfig.json
--rw-r--r--   0        0        0    32155 2023-05-06 00:10:02.619389 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/abi/ReceivableFactoringPool.json
--rw-r--r--   0        0        0    30290 2023-05-06 00:10:02.619495 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/abi/SuperfluidFactoringPool.json
--rw-r--r--   0        0        0     4740 2023-05-09 22:56:01.650261 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/adapter.py
--rw-r--r--   0        0        0     1938 2023-05-06 00:10:02.619635 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/registry.py
--rw-r--r--   0        0        0      158 2023-05-09 22:56:01.650357 huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/settings.py
--rw-r--r--   0        0        0      582 2023-05-06 00:10:02.619763 huma_signals-0.1.3/huma_signals/domain/adapters/models.py
--rw-r--r--   0        0        0      594 2023-05-06 00:10:02.619844 huma_signals-0.1.3/huma_signals/domain/adapters/polygon_wallet/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.619871 huma_signals-0.1.3/huma_signals/domain/adapters/polygon_wallet/__init__.py
--rw-r--r--   0        0        0     3427 2023-05-09 22:56:01.650473 huma_signals-0.1.3/huma_signals/domain/adapters/polygon_wallet/adapter.py
--rw-r--r--   0        0        0      222 2023-05-09 22:56:01.650540 huma_signals-0.1.3/huma_signals/domain/adapters/polygon_wallet/settings.py
--rw-r--r--   0        0        0     2791 2023-05-06 00:10:02.620043 huma_signals-0.1.3/huma_signals/domain/adapters/registry.py
--rw-r--r--   0        0        0      579 2023-05-06 00:10:02.620132 huma_signals-0.1.3/huma_signals/domain/adapters/request_network/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620159 huma_signals-0.1.3/huma_signals/domain/adapters/request_network/__init__.py
--rw-r--r--   0        0        0     4372 2023-05-06 00:10:02.620235 huma_signals-0.1.3/huma_signals/domain/adapters/request_network/models.py
--rw-r--r--   0        0        0     5949 2023-05-09 22:56:01.650686 huma_signals-0.1.3/huma_signals/domain/adapters/request_network/request_invoice_adapter.py
--rw-r--r--   0        0        0     5262 2023-05-09 22:56:01.650791 huma_signals-0.1.3/huma_signals/domain/adapters/request_network/request_transaction_adapter.py
--rw-r--r--   0        0        0      284 2023-05-09 22:56:01.650850 huma_signals-0.1.3/huma_signals/domain/adapters/request_network/settings.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620495 huma_signals-0.1.3/huma_signals/domain/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620556 huma_signals-0.1.3/huma_signals/domain/clients/eth_client/__init__.py
--rw-r--r--   0        0        0     1434 2023-05-09 22:56:01.650971 huma_signals-0.1.3/huma_signals/domain/clients/eth_client/eth_client.py
--rw-r--r--   0        0        0      673 2023-05-06 00:10:02.620677 huma_signals-0.1.3/huma_signals/domain/clients/eth_client/eth_types.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620728 huma_signals-0.1.3/huma_signals/domain/clients/polygon_client/__init__.py
--rw-r--r--   0        0        0     1510 2023-05-09 22:56:01.651074 huma_signals-0.1.3/huma_signals/domain/clients/polygon_client/polygon_client.py
--rw-r--r--   0        0        0      685 2023-05-06 00:10:02.620830 huma_signals-0.1.3/huma_signals/domain/clients/polygon_client/polygon_types.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620885 huma_signals-0.1.3/huma_signals/domain/clients/request_client/__init__.py
--rw-r--r--   0        0        0     8136 2023-05-09 22:56:01.651238 huma_signals-0.1.3/huma_signals/domain/clients/request_client/request_client.py
--rw-r--r--   0        0        0      900 2023-05-06 00:10:02.621033 huma_signals-0.1.3/huma_signals/domain/clients/request_client/request_types.py
--rw-r--r--   0        0        0      499 2023-05-06 00:10:02.621121 huma_signals-0.1.3/huma_signals/dotenv/example.env
--rw-r--r--   0        0        0      946 2023-05-06 00:10:02.621175 huma_signals-0.1.3/huma_signals/exceptions.py
--rw-r--r--   0        0        0      322 2023-05-06 00:10:02.621231 huma_signals-0.1.3/huma_signals/models.py
--rw-r--r--   0        0        0     1563 2023-05-06 00:10:02.621293 huma_signals-0.1.3/huma_signals/settings.py
--rw-r--r--   0        0        0     2703 2023-05-09 22:56:40.688139 huma_signals-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 huma_signals-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-06 00:10:02.616918 huma_signals-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2173 2023-05-06 00:10:02.617080 huma_signals-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617555 huma_signals-0.1.4/huma_signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617626 huma_signals-0.1.4/huma_signals/api/__init__.py
+-rw-r--r--   0        0        0     1187 2023-05-06 00:10:02.617701 huma_signals-0.1.4/huma_signals/api/exception_handlers.py
+-rw-r--r--   0        0        0      997 2023-05-06 00:10:02.617769 huma_signals-0.1.4/huma_signals/api/main.py
+-rw-r--r--   0        0        0      289 2023-05-06 00:10:02.617834 huma_signals-0.1.4/huma_signals/api/models.py
+-rw-r--r--   0        0        0     1114 2023-05-06 00:10:02.617904 huma_signals-0.1.4/huma_signals/api/views.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617961 huma_signals-0.1.4/huma_signals/commons/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-06 00:10:02.618029 huma_signals-0.1.4/huma_signals/commons/chains.py
+-rw-r--r--   0        0        0      330 2023-05-06 00:10:02.618090 huma_signals-0.1.4/huma_signals/commons/datetime_utils.py
+-rw-r--r--   0        0        0      227 2023-05-06 00:10:02.618146 huma_signals-0.1.4/huma_signals/commons/pydantic_utils.py
+-rw-r--r--   0        0        0      569 2023-05-06 00:10:02.618202 huma_signals-0.1.4/huma_signals/commons/string_utils.py
+-rw-r--r--   0        0        0     1309 2023-05-06 00:10:02.618262 huma_signals-0.1.4/huma_signals/commons/tokens.py
+-rw-r--r--   0        0        0     1078 2023-05-06 00:10:02.618330 huma_signals-0.1.4/huma_signals/commons/web3_utils.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618388 huma_signals-0.1.4/huma_signals/domain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618462 huma_signals-0.1.4/huma_signals/domain/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618534 huma_signals-0.1.4/huma_signals/domain/adapters/allowlist/__init__.py
+-rw-r--r--   0        0        0     1755 2023-05-06 00:10:02.618617 huma_signals-0.1.4/huma_signals/domain/adapters/allowlist/adapter.py
+-rw-r--r--   0        0        0      589 2023-05-06 00:10:02.618719 huma_signals-0.1.4/huma_signals/domain/adapters/ethereum_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.618750 huma_signals-0.1.4/huma_signals/domain/adapters/ethereum_wallet/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-09 22:56:01.650045 huma_signals-0.1.4/huma_signals/domain/adapters/ethereum_wallet/adapter.py
+-rw-r--r--   0        0        0      186 2023-05-09 22:56:01.650122 huma_signals-0.1.4/huma_signals/domain/adapters/ethereum_wallet/settings.py
+-rw-r--r--   0        0        0      589 2023-05-06 00:10:02.618984 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.619013 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/__init__.py
+-rw-r--r--   0        0        0    23699 2023-05-06 00:10:02.619139 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/abi/BaseCreditPool.json
+-rw-r--r--   0        0        0    30632 2023-05-06 00:10:02.619304 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/abi/BasePoolConfig.json
+-rw-r--r--   0        0        0    32155 2023-05-06 00:10:02.619389 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/abi/ReceivableFactoringPool.json
+-rw-r--r--   0        0        0    30290 2023-05-06 00:10:02.619495 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/abi/SuperfluidFactoringPool.json
+-rw-r--r--   0        0        0     4740 2023-05-09 22:56:01.650261 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/adapter.py
+-rw-r--r--   0        0        0     1938 2023-05-06 00:10:02.619635 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/registry.py
+-rw-r--r--   0        0        0      158 2023-05-09 22:56:01.650357 huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/settings.py
+-rw-r--r--   0        0        0      582 2023-05-06 00:10:02.619763 huma_signals-0.1.4/huma_signals/domain/adapters/models.py
+-rw-r--r--   0        0        0      594 2023-05-06 00:10:02.619844 huma_signals-0.1.4/huma_signals/domain/adapters/polygon_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.619871 huma_signals-0.1.4/huma_signals/domain/adapters/polygon_wallet/__init__.py
+-rw-r--r--   0        0        0     3427 2023-05-09 22:56:01.650473 huma_signals-0.1.4/huma_signals/domain/adapters/polygon_wallet/adapter.py
+-rw-r--r--   0        0        0      222 2023-05-09 22:56:01.650540 huma_signals-0.1.4/huma_signals/domain/adapters/polygon_wallet/settings.py
+-rw-r--r--   0        0        0     2791 2023-05-06 00:10:02.620043 huma_signals-0.1.4/huma_signals/domain/adapters/registry.py
+-rw-r--r--   0        0        0      579 2023-05-06 00:10:02.620132 huma_signals-0.1.4/huma_signals/domain/adapters/request_network/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620159 huma_signals-0.1.4/huma_signals/domain/adapters/request_network/__init__.py
+-rw-r--r--   0        0        0     4372 2023-05-06 00:10:02.620235 huma_signals-0.1.4/huma_signals/domain/adapters/request_network/models.py
+-rw-r--r--   0        0        0     5949 2023-05-09 22:56:01.650686 huma_signals-0.1.4/huma_signals/domain/adapters/request_network/request_invoice_adapter.py
+-rw-r--r--   0        0        0     5262 2023-05-09 22:56:01.650791 huma_signals-0.1.4/huma_signals/domain/adapters/request_network/request_transaction_adapter.py
+-rw-r--r--   0        0        0      284 2023-05-09 22:56:01.650850 huma_signals-0.1.4/huma_signals/domain/adapters/request_network/settings.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620495 huma_signals-0.1.4/huma_signals/domain/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620556 huma_signals-0.1.4/huma_signals/domain/clients/eth_client/__init__.py
+-rw-r--r--   0        0        0     1434 2023-05-09 22:56:01.650971 huma_signals-0.1.4/huma_signals/domain/clients/eth_client/eth_client.py
+-rw-r--r--   0        0        0      673 2023-05-06 00:10:02.620677 huma_signals-0.1.4/huma_signals/domain/clients/eth_client/eth_types.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620728 huma_signals-0.1.4/huma_signals/domain/clients/polygon_client/__init__.py
+-rw-r--r--   0        0        0     1510 2023-05-09 22:56:01.651074 huma_signals-0.1.4/huma_signals/domain/clients/polygon_client/polygon_client.py
+-rw-r--r--   0        0        0      685 2023-05-06 00:10:02.620830 huma_signals-0.1.4/huma_signals/domain/clients/polygon_client/polygon_types.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.620885 huma_signals-0.1.4/huma_signals/domain/clients/request_client/__init__.py
+-rw-r--r--   0        0        0     8136 2023-05-09 22:56:01.651238 huma_signals-0.1.4/huma_signals/domain/clients/request_client/request_client.py
+-rw-r--r--   0        0        0      900 2023-05-06 00:10:02.621033 huma_signals-0.1.4/huma_signals/domain/clients/request_client/request_types.py
+-rw-r--r--   0        0        0      499 2023-05-06 00:10:02.621121 huma_signals-0.1.4/huma_signals/dotenv/example.env
+-rw-r--r--   0        0        0      946 2023-05-06 00:10:02.621175 huma_signals-0.1.4/huma_signals/exceptions.py
+-rw-r--r--   0        0        0      322 2023-05-06 00:10:02.621231 huma_signals-0.1.4/huma_signals/models.py
+-rw-r--r--   0        0        0        0 2023-05-09 22:56:04.974259 huma_signals-0.1.4/huma_signals/py.typed
+-rw-r--r--   0        0        0     1563 2023-05-06 00:10:02.621293 huma_signals-0.1.4/huma_signals/settings.py
+-rw-r--r--   0        0        0     2703 2023-05-09 23:06:11.492776 huma_signals-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 huma_signals-0.1.4/PKG-INFO
```

### Comparing `huma_signals-0.1.3/LICENSE` & `huma_signals-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/README.md` & `huma_signals-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/api/exception_handlers.py` & `huma_signals-0.1.4/huma_signals/api/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/api/main.py` & `huma_signals-0.1.4/huma_signals/api/main.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/api/views.py` & `huma_signals-0.1.4/huma_signals/api/views.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/commons/chains.py` & `huma_signals-0.1.4/huma_signals/commons/chains.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/commons/string_utils.py` & `huma_signals-0.1.4/huma_signals/commons/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/commons/tokens.py` & `huma_signals-0.1.4/huma_signals/commons/tokens.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/commons/web3_utils.py` & `huma_signals-0.1.4/huma_signals/commons/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/allowlist/adapter.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/allowlist/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/ethereum_wallet/README.md` & `huma_signals-0.1.4/huma_signals/domain/adapters/ethereum_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/ethereum_wallet/adapter.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/ethereum_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/README.md` & `huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/abi/BaseCreditPool.json` & `huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/abi/BaseCreditPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/abi/BasePoolConfig.json` & `huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/abi/BasePoolConfig.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/abi/ReceivableFactoringPool.json` & `huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/abi/ReceivableFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/abi/SuperfluidFactoringPool.json` & `huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/abi/SuperfluidFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/adapter.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/lending_pools/registry.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/lending_pools/registry.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/models.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/polygon_wallet/README.md` & `huma_signals-0.1.4/huma_signals/domain/adapters/polygon_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/polygon_wallet/adapter.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/polygon_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/registry.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/request_network/README.md` & `huma_signals-0.1.4/huma_signals/domain/adapters/request_network/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/request_network/models.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/request_network/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/request_network/request_invoice_adapter.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/request_network/request_invoice_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/adapters/request_network/request_transaction_adapter.py` & `huma_signals-0.1.4/huma_signals/domain/adapters/request_network/request_transaction_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/clients/eth_client/eth_client.py` & `huma_signals-0.1.4/huma_signals/domain/clients/eth_client/eth_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/clients/eth_client/eth_types.py` & `huma_signals-0.1.4/huma_signals/domain/clients/eth_client/eth_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/clients/polygon_client/polygon_client.py` & `huma_signals-0.1.4/huma_signals/domain/clients/polygon_client/polygon_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/clients/polygon_client/polygon_types.py` & `huma_signals-0.1.4/huma_signals/domain/clients/polygon_client/polygon_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/clients/request_client/request_client.py` & `huma_signals-0.1.4/huma_signals/domain/clients/request_client/request_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/domain/clients/request_client/request_types.py` & `huma_signals-0.1.4/huma_signals/domain/clients/request_client/request_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/exceptions.py` & `huma_signals-0.1.4/huma_signals/exceptions.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/huma_signals/settings.py` & `huma_signals-0.1.4/huma_signals/settings.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.1.3/pyproject.toml` & `huma_signals-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-signals"
-version = "0.1.3"
+version = "0.1.4"
 description = "Enables access to high-quality signals about a borrower's income, assets, and liabilities."
 authors = ["Jiatu Liu <jiatu@huma.finance>", "Ji Peng <ji@huma.finance>"]
 license = "AGPL v3"
 readme = "README.md"
 packages = [{include = "huma_signals"}]
 
 [tool.poetry.dependencies]
```

### Comparing `huma_signals-0.1.3/PKG-INFO` & `huma_signals-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huma-signals
-Version: 0.1.3
+Version: 0.1.4
 Summary: Enables access to high-quality signals about a borrower's income, assets, and liabilities.
 License: AGPL v3
 Author: Jiatu Liu
 Author-email: jiatu@huma.finance
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: huma-signals Version: 0.1.3 Summary: Enables access
+Metadata-Version: 2.1 Name: huma-signals Version: 0.1.4 Summary: Enables access
 to high-quality signals about a borrower's income, assets, and liabilities.
 License: AGPL v3 Author: Jiatu Liu Author-email: jiatu@huma.finance Requires-
 Python: >=3.10,<3.11 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-
 Dist: datadog (>=0.44.0,<0.45.0) Requires-Dist: ddtrace[opentracing]
 (>=1.7.5,<2.0.0) Requires-Dist: fastapi (>=0.95.1,<0.96.0) Requires-Dist: httpx
```

