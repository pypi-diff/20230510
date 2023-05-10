# Comparing `tmp/lixinger-0.1.5.tar.gz` & `tmp/lixinger-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixinger-0.1.5.tar", last modified: Mon May  8 15:00:03 2023, max compression
+gzip compressed data, was "lixinger-0.1.6.tar", last modified: Wed May 10 13:04:33 2023, max compression
```

## Comparing `lixinger-0.1.5.tar` & `lixinger-0.1.6.tar`

### file list

```diff
@@ -1,46 +1,50 @@
--rw-r--r--   0        0        0      705 2023-05-03 10:11:52.615764 lixinger-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.5/lixinger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.5/lixinger/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.5/lixinger/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.5/lixinger/api/cn/company/__init__.py
--rw-r--r--   0        0        0     1915 2023-05-08 14:59:49.483381 lixinger-0.1.5/lixinger/api/cn/company/base.py
--rw-r--r--   0        0        0     1340 2023-05-08 14:59:49.483210 lixinger-0.1.5/lixinger/api/cn/company/block_deal.py
--rw-r--r--   0        0        0     1724 2023-05-08 14:59:49.483765 lixinger-0.1.5/lixinger/api/cn/company/candlestick.py
--rw-r--r--   0        0        0     1913 2023-05-08 14:59:49.483082 lixinger-0.1.5/lixinger/api/cn/company/dividend_and_alloment.py
--rw-r--r--   0        0        0     1284 2023-05-08 14:59:49.483153 lixinger-0.1.5/lixinger/api/cn/company/equity_change.py
--rw-r--r--   0        0        0     2124 2023-05-08 14:54:00.683946 lixinger-0.1.5/lixinger/api/cn/company/pledge.py
--rw-r--r--   0        0        0     1471 2023-05-07 15:02:40.594443 lixinger-0.1.5/lixinger/api/cn/company/senior_executive_shares_change.py
--rw-r--r--   0        0        0     1120 2023-05-08 14:59:49.483180 lixinger-0.1.5/lixinger/api/cn/company/shareholders_num.py
--rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.5/lixinger/api/cn/fund/__init__.py
--rw-r--r--   0        0        0     1256 2023-05-08 14:59:49.483074 lixinger-0.1.5/lixinger/api/cn/fund/exchange_traded_close_price.py
--rw-r--r--   0        0        0     1131 2023-05-08 14:59:49.483073 lixinger-0.1.5/lixinger/api/cn/fund/total_net_value.py
--rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.5/lixinger/api/cn/index/__init__.py
--rw-r--r--   0        0        0     1400 2023-05-08 14:59:49.483762 lixinger-0.1.5/lixinger/api/cn/index/candlestick.py
--rw-r--r--   0        0        0     1631 2023-05-08 14:59:49.483158 lixinger-0.1.5/lixinger/api/cn/index/fundamental.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.5/lixinger/api/hk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.5/lixinger/api/macro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.5/lixinger/api/us/__init__.py
--rw-r--r--   0        0        0     1582 2023-05-04 10:40:12.141591 lixinger-0.1.5/lixinger/config.py
--rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.5/lixinger/py.typed
--rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.5/lixinger/settings.toml
--rw-r--r--   0        0        0     3300 2023-05-08 14:53:08.611490 lixinger-0.1.5/lixinger/utils.py
--rw-r--r--   0        0        0      912 2023-05-08 15:00:03.040767 lixinger-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.5/tests/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.5/tests/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.5/tests/api/cn/company/__init__.py
--rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.5/tests/api/cn/company/test_base.py
--rw-r--r--   0        0        0      164 2023-05-08 14:09:59.839924 lixinger-0.1.5/tests/api/cn/company/test_block_deal.py
--rw-r--r--   0        0        0      187 2023-05-07 03:59:49.667512 lixinger-0.1.5/tests/api/cn/company/test_candlestick.py
--rw-r--r--   0        0        0      217 2023-05-06 05:43:46.770904 lixinger-0.1.5/tests/api/cn/company/test_dividend_and_alloment.py
--rw-r--r--   0        0        0      170 2023-05-06 02:12:57.131245 lixinger-0.1.5/tests/api/cn/company/test_equity_change.py
--rw-r--r--   0        0        0      144 2023-05-08 14:53:32.432310 lixinger-0.1.5/tests/api/cn/company/test_pledge.py
--rw-r--r--   0        0        0      235 2023-05-07 15:03:11.303695 lixinger-0.1.5/tests/api/cn/company/test_senior_executive_shares_change.py
--rw-r--r--   0        0        0      184 2023-05-07 14:29:15.357398 lixinger-0.1.5/tests/api/cn/company/test_shareholders_num.py
--rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.5/tests/api/cn/fund/__init__.py
--rw-r--r--   0        0        0      238 2023-05-07 02:06:30.724314 lixinger-0.1.5/tests/api/cn/fund/test_exchange_traded_close_price.py
--rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.5/tests/api/cn/fund/test_total_net_value.py
--rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.5/tests/api/cn/index/__init__.py
--rw-r--r--   0        0        0      182 2023-05-07 01:58:13.309631 lixinger-0.1.5/tests/api/cn/index/test_candlestick.py
--rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.5/tests/api/cn/index/test_fundamental.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 lixinger-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1281 2023-05-10 13:03:59.627154 lixinger-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.6/lixinger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.6/lixinger/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.6/lixinger/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.6/lixinger/api/cn/company/__init__.py
+-rw-r--r--   0        0        0     1915 2023-05-08 14:59:49.483381 lixinger-0.1.6/lixinger/api/cn/company/base.py
+-rw-r--r--   0        0        0     1340 2023-05-10 12:37:08.165627 lixinger-0.1.6/lixinger/api/cn/company/block_deal.py
+-rw-r--r--   0        0        0     1724 2023-05-08 14:59:49.483765 lixinger-0.1.6/lixinger/api/cn/company/candlestick.py
+-rw-r--r--   0        0        0     1913 2023-05-08 14:59:49.483082 lixinger-0.1.6/lixinger/api/cn/company/dividend_and_alloment.py
+-rw-r--r--   0        0        0     1284 2023-05-08 14:59:49.483153 lixinger-0.1.6/lixinger/api/cn/company/equity_change.py
+-rw-r--r--   0        0        0      907 2023-05-09 12:28:21.809650 lixinger-0.1.6/lixinger/api/cn/company/indices.py
+-rw-r--r--   0        0        0      916 2023-05-10 12:17:03.471765 lixinger-0.1.6/lixinger/api/cn/company/industries.py
+-rw-r--r--   0        0        0     2124 2023-05-08 14:54:00.683946 lixinger-0.1.6/lixinger/api/cn/company/pledge.py
+-rw-r--r--   0        0        0     1471 2023-05-07 15:02:40.594443 lixinger-0.1.6/lixinger/api/cn/company/senior_executive_shares_change.py
+-rw-r--r--   0        0        0     1120 2023-05-08 14:59:49.483180 lixinger-0.1.6/lixinger/api/cn/company/shareholders_num.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.6/lixinger/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0     1256 2023-05-08 14:59:49.483074 lixinger-0.1.6/lixinger/api/cn/fund/exchange_traded_close_price.py
+-rw-r--r--   0        0        0     1131 2023-05-08 14:59:49.483073 lixinger-0.1.6/lixinger/api/cn/fund/total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.6/lixinger/api/cn/index/__init__.py
+-rw-r--r--   0        0        0     1400 2023-05-08 14:59:49.483762 lixinger-0.1.6/lixinger/api/cn/index/candlestick.py
+-rw-r--r--   0        0        0     1631 2023-05-08 14:59:49.483158 lixinger-0.1.6/lixinger/api/cn/index/fundamental.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.6/lixinger/api/hk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.6/lixinger/api/macro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.6/lixinger/api/us/__init__.py
+-rw-r--r--   0        0        0     1616 2023-05-10 12:36:30.661382 lixinger-0.1.6/lixinger/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.6/lixinger/py.typed
+-rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.6/lixinger/settings.toml
+-rw-r--r--   0        0        0     3300 2023-05-08 14:53:08.611490 lixinger-0.1.6/lixinger/utils.py
+-rw-r--r--   0        0        0      912 2023-05-10 13:04:33.975708 lixinger-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.6/tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.6/tests/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.6/tests/api/cn/company/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.6/tests/api/cn/company/test_base.py
+-rw-r--r--   0        0        0      164 2023-05-08 14:09:59.839924 lixinger-0.1.6/tests/api/cn/company/test_block_deal.py
+-rw-r--r--   0        0        0      187 2023-05-07 03:59:49.667512 lixinger-0.1.6/tests/api/cn/company/test_candlestick.py
+-rw-r--r--   0        0        0      217 2023-05-06 05:43:46.770904 lixinger-0.1.6/tests/api/cn/company/test_dividend_and_alloment.py
+-rw-r--r--   0        0        0      170 2023-05-06 02:12:57.131245 lixinger-0.1.6/tests/api/cn/company/test_equity_change.py
+-rw-r--r--   0        0        0      127 2023-05-09 12:28:07.598154 lixinger-0.1.6/tests/api/cn/company/test_indices.py
+-rw-r--r--   0        0        0      139 2023-05-10 12:17:30.914094 lixinger-0.1.6/tests/api/cn/company/test_industries.py
+-rw-r--r--   0        0        0      144 2023-05-08 14:53:32.432310 lixinger-0.1.6/tests/api/cn/company/test_pledge.py
+-rw-r--r--   0        0        0      235 2023-05-07 15:03:11.303695 lixinger-0.1.6/tests/api/cn/company/test_senior_executive_shares_change.py
+-rw-r--r--   0        0        0      184 2023-05-07 14:29:15.357398 lixinger-0.1.6/tests/api/cn/company/test_shareholders_num.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.6/tests/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-07 02:06:30.724314 lixinger-0.1.6/tests/api/cn/fund/test_exchange_traded_close_price.py
+-rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.6/tests/api/cn/fund/test_total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.6/tests/api/cn/index/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-07 01:58:13.309631 lixinger-0.1.6/tests/api/cn/index/test_candlestick.py
+-rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.6/tests/api/cn/index/test_fundamental.py
+-rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 lixinger-0.1.6/PKG-INFO
```

### Comparing `lixinger-0.1.5/lixinger/api/cn/company/base.py` & `lixinger-0.1.6/lixinger/api/cn/company/base.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/company/block_deal.py` & `lixinger-0.1.6/lixinger/api/cn/company/block_deal.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/company/candlestick.py` & `lixinger-0.1.6/lixinger/api/cn/company/candlestick.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/company/dividend_and_alloment.py` & `lixinger-0.1.6/lixinger/api/cn/company/dividend_and_alloment.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/company/equity_change.py` & `lixinger-0.1.6/lixinger/api/cn/company/equity_change.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/company/pledge.py` & `lixinger-0.1.6/lixinger/api/cn/company/pledge.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/company/senior_executive_shares_change.py` & `lixinger-0.1.6/lixinger/api/cn/company/senior_executive_shares_change.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/company/shareholders_num.py` & `lixinger-0.1.6/lixinger/api/cn/company/shareholders_num.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/fund/exchange_traded_close_price.py` & `lixinger-0.1.6/lixinger/api/cn/fund/exchange_traded_close_price.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/fund/total_net_value.py` & `lixinger-0.1.6/lixinger/api/cn/fund/total_net_value.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/index/candlestick.py` & `lixinger-0.1.6/lixinger/api/cn/index/candlestick.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/api/cn/index/fundamental.py` & `lixinger-0.1.6/lixinger/api/cn/index/fundamental.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/lixinger/config.py` & `lixinger-0.1.6/lixinger/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,12 +57,13 @@
     )
     default_settings = TypedDynaconf(
         settings_files=settings_files,
         merge_enabled=True,
         environments=True,
         validators=get_validators(),
         validate=True,
+        envvar_prefix="LIXINGER",
     )
     return default_settings
 
 
 settings = load_settings()
```

### Comparing `lixinger-0.1.5/lixinger/utils.py` & `lixinger-0.1.6/lixinger/utils.py`

 * *Files identical despite different names*

### Comparing `lixinger-0.1.5/pyproject.toml` & `lixinger-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache/"
 addopts = "-s -p no:warnings"
 asyncio_mode = "auto"
 
 [project]
 name = "lixinger"
-version = "0.1.5"
+version = "0.1.6"
 description = "Lixinger SDK for Python (Unofficial)"
 authors = [
     { name = "Chaoying", email = "chaoying2022@gmail.com" },
 ]
 dependencies = [
     "pandera>=0.14.5",
     "pydantic>=1.10.7",
```

