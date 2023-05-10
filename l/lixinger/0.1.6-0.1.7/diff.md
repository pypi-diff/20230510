# Comparing `tmp/lixinger-0.1.6.tar.gz` & `tmp/lixinger-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lixinger-0.1.6.tar", last modified: Wed May 10 13:04:33 2023, max compression
+gzip compressed data, was "lixinger-0.1.7.tar", last modified: Wed May 10 14:14:40 2023, max compression
```

## Comparing `lixinger-0.1.6.tar` & `lixinger-0.1.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1281 2023-05-10 13:03:59.627154 lixinger-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.6/lixinger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.6/lixinger/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.6/lixinger/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.6/lixinger/api/cn/company/__init__.py
--rw-r--r--   0        0        0     1915 2023-05-08 14:59:49.483381 lixinger-0.1.6/lixinger/api/cn/company/base.py
--rw-r--r--   0        0        0     1340 2023-05-10 12:37:08.165627 lixinger-0.1.6/lixinger/api/cn/company/block_deal.py
--rw-r--r--   0        0        0     1724 2023-05-08 14:59:49.483765 lixinger-0.1.6/lixinger/api/cn/company/candlestick.py
--rw-r--r--   0        0        0     1913 2023-05-08 14:59:49.483082 lixinger-0.1.6/lixinger/api/cn/company/dividend_and_alloment.py
--rw-r--r--   0        0        0     1284 2023-05-08 14:59:49.483153 lixinger-0.1.6/lixinger/api/cn/company/equity_change.py
--rw-r--r--   0        0        0      907 2023-05-09 12:28:21.809650 lixinger-0.1.6/lixinger/api/cn/company/indices.py
--rw-r--r--   0        0        0      916 2023-05-10 12:17:03.471765 lixinger-0.1.6/lixinger/api/cn/company/industries.py
--rw-r--r--   0        0        0     2124 2023-05-08 14:54:00.683946 lixinger-0.1.6/lixinger/api/cn/company/pledge.py
--rw-r--r--   0        0        0     1471 2023-05-07 15:02:40.594443 lixinger-0.1.6/lixinger/api/cn/company/senior_executive_shares_change.py
--rw-r--r--   0        0        0     1120 2023-05-08 14:59:49.483180 lixinger-0.1.6/lixinger/api/cn/company/shareholders_num.py
--rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.6/lixinger/api/cn/fund/__init__.py
--rw-r--r--   0        0        0     1256 2023-05-08 14:59:49.483074 lixinger-0.1.6/lixinger/api/cn/fund/exchange_traded_close_price.py
--rw-r--r--   0        0        0     1131 2023-05-08 14:59:49.483073 lixinger-0.1.6/lixinger/api/cn/fund/total_net_value.py
--rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.6/lixinger/api/cn/index/__init__.py
--rw-r--r--   0        0        0     1400 2023-05-08 14:59:49.483762 lixinger-0.1.6/lixinger/api/cn/index/candlestick.py
--rw-r--r--   0        0        0     1631 2023-05-08 14:59:49.483158 lixinger-0.1.6/lixinger/api/cn/index/fundamental.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.6/lixinger/api/hk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.6/lixinger/api/macro/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.6/lixinger/api/us/__init__.py
--rw-r--r--   0        0        0     1616 2023-05-10 12:36:30.661382 lixinger-0.1.6/lixinger/config.py
--rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.6/lixinger/py.typed
--rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.6/lixinger/settings.toml
--rw-r--r--   0        0        0     3300 2023-05-08 14:53:08.611490 lixinger-0.1.6/lixinger/utils.py
--rw-r--r--   0        0        0      912 2023-05-10 13:04:33.975708 lixinger-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.6/tests/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.6/tests/api/cn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.6/tests/api/cn/company/__init__.py
--rw-r--r--   0        0        0      127 2023-05-03 10:00:15.081563 lixinger-0.1.6/tests/api/cn/company/test_base.py
--rw-r--r--   0        0        0      164 2023-05-08 14:09:59.839924 lixinger-0.1.6/tests/api/cn/company/test_block_deal.py
--rw-r--r--   0        0        0      187 2023-05-07 03:59:49.667512 lixinger-0.1.6/tests/api/cn/company/test_candlestick.py
--rw-r--r--   0        0        0      217 2023-05-06 05:43:46.770904 lixinger-0.1.6/tests/api/cn/company/test_dividend_and_alloment.py
--rw-r--r--   0        0        0      170 2023-05-06 02:12:57.131245 lixinger-0.1.6/tests/api/cn/company/test_equity_change.py
--rw-r--r--   0        0        0      127 2023-05-09 12:28:07.598154 lixinger-0.1.6/tests/api/cn/company/test_indices.py
--rw-r--r--   0        0        0      139 2023-05-10 12:17:30.914094 lixinger-0.1.6/tests/api/cn/company/test_industries.py
--rw-r--r--   0        0        0      144 2023-05-08 14:53:32.432310 lixinger-0.1.6/tests/api/cn/company/test_pledge.py
--rw-r--r--   0        0        0      235 2023-05-07 15:03:11.303695 lixinger-0.1.6/tests/api/cn/company/test_senior_executive_shares_change.py
--rw-r--r--   0        0        0      184 2023-05-07 14:29:15.357398 lixinger-0.1.6/tests/api/cn/company/test_shareholders_num.py
--rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.6/tests/api/cn/fund/__init__.py
--rw-r--r--   0        0        0      238 2023-05-07 02:06:30.724314 lixinger-0.1.6/tests/api/cn/fund/test_exchange_traded_close_price.py
--rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.6/tests/api/cn/fund/test_total_net_value.py
--rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.6/tests/api/cn/index/__init__.py
--rw-r--r--   0        0        0      182 2023-05-07 01:58:13.309631 lixinger-0.1.6/tests/api/cn/index/test_candlestick.py
--rw-r--r--   0        0        0      270 2023-05-03 09:27:22.076125 lixinger-0.1.6/tests/api/cn/index/test_fundamental.py
--rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 lixinger-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1502 2023-05-10 14:14:08.343659 lixinger-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-01 04:05:58.277552 lixinger-0.1.7/lixinger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:33:35.225361 lixinger-0.1.7/lixinger/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:22.152169 lixinger-0.1.7/lixinger/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:36.967425 lixinger-0.1.7/lixinger/api/cn/company/__init__.py
+-rw-r--r--   0        0        0     1849 2023-05-10 13:59:47.866336 lixinger-0.1.7/lixinger/api/cn/company/base.py
+-rw-r--r--   0        0        0     1220 2023-05-10 14:14:09.173725 lixinger-0.1.7/lixinger/api/cn/company/block_deal.py
+-rw-r--r--   0        0        0     1604 2023-05-10 14:14:09.173340 lixinger-0.1.7/lixinger/api/cn/company/candlestick.py
+-rw-r--r--   0        0        0     1793 2023-05-10 14:14:09.173817 lixinger-0.1.7/lixinger/api/cn/company/dividend_and_alloment.py
+-rw-r--r--   0        0        0     1164 2023-05-10 14:14:09.173179 lixinger-0.1.7/lixinger/api/cn/company/equity_change.py
+-rw-r--r--   0        0        0      841 2023-05-10 14:14:09.108533 lixinger-0.1.7/lixinger/api/cn/company/indices.py
+-rw-r--r--   0        0        0      850 2023-05-10 14:14:09.109062 lixinger-0.1.7/lixinger/api/cn/company/industries.py
+-rw-r--r--   0        0        0     2004 2023-05-10 14:14:09.173348 lixinger-0.1.7/lixinger/api/cn/company/pledge.py
+-rw-r--r--   0        0        0     1351 2023-05-10 14:14:09.173556 lixinger-0.1.7/lixinger/api/cn/company/senior_executive_shares_change.py
+-rw-r--r--   0        0        0     1000 2023-05-10 14:14:09.173795 lixinger-0.1.7/lixinger/api/cn/company/shareholders_num.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:21:25.826889 lixinger-0.1.7/lixinger/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0     1136 2023-05-10 14:14:09.173426 lixinger-0.1.7/lixinger/api/cn/fund/exchange_traded_close_price.py
+-rw-r--r--   0        0        0     1011 2023-05-10 14:14:09.173179 lixinger-0.1.7/lixinger/api/cn/fund/total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:10:55.043163 lixinger-0.1.7/lixinger/api/cn/index/__init__.py
+-rw-r--r--   0        0        0     1280 2023-05-10 14:14:09.173306 lixinger-0.1.7/lixinger/api/cn/index/candlestick.py
+-rw-r--r--   0        0        0     1511 2023-05-10 14:14:09.173214 lixinger-0.1.7/lixinger/api/cn/index/fundamental.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:31.838744 lixinger-0.1.7/lixinger/api/hk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:09:00.179536 lixinger-0.1.7/lixinger/api/macro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:08:44.656824 lixinger-0.1.7/lixinger/api/us/__init__.py
+-rw-r--r--   0        0        0     1644 2023-05-10 14:14:18.924307 lixinger-0.1.7/lixinger/config.py
+-rw-r--r--   0        0        0        0 2023-05-03 09:27:58.212202 lixinger-0.1.7/lixinger/py.typed
+-rw-r--r--   0        0        0       75 2023-05-03 10:06:41.922780 lixinger-0.1.7/lixinger/settings.toml
+-rw-r--r--   0        0        0     5724 2023-05-10 14:14:09.115003 lixinger-0.1.7/lixinger/utils.py
+-rw-r--r--   0        0        0      912 2023-05-10 14:14:40.078071 lixinger-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:15.660305 lixinger-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:19.505533 lixinger-0.1.7/tests/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:24.536685 lixinger-0.1.7/tests/api/cn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-01 04:43:30.757795 lixinger-0.1.7/tests/api/cn/company/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-10 13:55:25.017569 lixinger-0.1.7/tests/api/cn/company/test_base.py
+-rw-r--r--   0        0        0      164 2023-05-08 14:09:59.839924 lixinger-0.1.7/tests/api/cn/company/test_block_deal.py
+-rw-r--r--   0        0        0      187 2023-05-10 14:12:30.362480 lixinger-0.1.7/tests/api/cn/company/test_candlestick.py
+-rw-r--r--   0        0        0      217 2023-05-06 05:43:46.770904 lixinger-0.1.7/tests/api/cn/company/test_dividend_and_alloment.py
+-rw-r--r--   0        0        0      170 2023-05-06 02:12:57.131245 lixinger-0.1.7/tests/api/cn/company/test_equity_change.py
+-rw-r--r--   0        0        0      127 2023-05-09 12:28:07.598154 lixinger-0.1.7/tests/api/cn/company/test_indices.py
+-rw-r--r--   0        0        0      139 2023-05-10 12:17:30.914094 lixinger-0.1.7/tests/api/cn/company/test_industries.py
+-rw-r--r--   0        0        0      144 2023-05-08 14:53:32.432310 lixinger-0.1.7/tests/api/cn/company/test_pledge.py
+-rw-r--r--   0        0        0      235 2023-05-07 15:03:11.303695 lixinger-0.1.7/tests/api/cn/company/test_senior_executive_shares_change.py
+-rw-r--r--   0        0        0      184 2023-05-07 14:29:15.357398 lixinger-0.1.7/tests/api/cn/company/test_shareholders_num.py
+-rw-r--r--   0        0        0        0 2023-05-04 14:30:00.736254 lixinger-0.1.7/tests/api/cn/fund/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-07 02:06:30.724314 lixinger-0.1.7/tests/api/cn/fund/test_exchange_traded_close_price.py
+-rw-r--r--   0        0        0      229 2023-05-04 14:32:35.703103 lixinger-0.1.7/tests/api/cn/fund/test_total_net_value.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:16:11.323717 lixinger-0.1.7/tests/api/cn/index/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-07 01:58:13.309631 lixinger-0.1.7/tests/api/cn/index/test_candlestick.py
+-rw-r--r--   0        0        0      270 2023-05-10 13:23:11.920162 lixinger-0.1.7/tests/api/cn/index/test_fundamental.py
+-rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 lixinger-0.1.7/PKG-INFO
```

### Comparing `lixinger-0.1.6/README.md` & `lixinger-0.1.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 # lixinger
 
 理杏仁 Python SDK (非官方).
 
 包含以下功能：
 
 - 自动将请求结果转换结果为 Dataframe.
-- 根据官方文档中的返回结果定义, 验证请求结果, 对缺少的列进行补齐, 对列类型进行转换.
-- 支持一次获取时间范围大于10年的数据.
+- 根据官方文档中的返回结果定义, 验证请求结果, 对缺少的列进行补齐, 对列类型进行相应转换.
+- 支持一次获取时间范围大于 10 年的数据.
+- 适当缓存请求结果，减少请求 API 次数.
 
 ## 安装
 
 ```bash
 pip install lixinger
 ```
 
 ## 用法
 
-### 设置 Token 
+### 设置 Token
 
 Token 获取地址为 [https://www.lixinger.com/open/api/token](https://www.lixinger.com/open/api/token)
 
-#### 方式1：通过环境变量来设置 Token
+#### 方式 1：通过环境变量来设置 Token
 
 ```bash
 export LIXINGER_TOKEN="你的 token"
 ```
 
-#### 方式2：通过配置文件来设置 Token
+#### 方式 2：通过配置文件来设置 Token
+
 打开配置文件（路径为 ~/.config/lixinger/settings.toml），并添加以下内容设置自己的 Token.
 
 ```toml
 [default]
 token = "你的 token"
 ```
 
 ### 调用 API
+
 使用文档请参考 [理杏仁开放平台](https://www.lixinger.com/open/api/doc)
 
+方法导入路径可以根据文档中的请求 URL 得出，例如下面代码中对应的请求 URL 为 `/api/cn/company` 则把 `/` 换成 `.` 即可.
+
 ```python
 from lixinger.api.cn.company.base import get_company
 
 # 获取股票详细信息
 company = get_company(stock_codes=["600519"])
 print(company)
 ```
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/base.py` & `lixinger-0.1.7/lixinger/api/cn/company/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 from typing import Literal, Optional
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import convert_column_list_to_str, get_response_df
+from lixinger.utils import api, convert_column_list_to_str, get_response_df
 
 
 class Output(pa.DataFrameModel):
     name: pa.typing.Series[str] = pa.Field(nullable=True)
     stock_code: pa.typing.Series[str]
     area_code: pa.typing.Series[str]
     market: pa.typing.Series[str]
@@ -19,16 +18,15 @@
     mutual_markets: Optional[pa.typing.Series[str]] = pa.Field(nullable=True)
     ipo_date: pa.typing.Series[pa.typing.DateTime] = pa.Field(nullable=True)
     delisted_date: Optional[pa.typing.Series[pa.typing.DateTime]] = pa.Field(
         nullable=True
     )
 
 
-@validate_arguments
-@pa.check_types
+@api
 def get_company(
     fs_type: Literal[
         "non_financial", "bank", "insurance", "security", "other_financial"
     ]
     | None = None,
     mutual_markets: Literal["ha"] | None = None,
     stock_codes: list[str] | None = None,
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/block_deal.py` & `lixinger-0.1.7/lixinger/api/cn/company/equity_change.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
-    trading_price: pa.typing.Series[float]
-    trading_money: pa.typing.Series[float]
-    trading_volume: pa.typing.Series[float]
-    buy_branch: pa.typing.Series[str]
-    sell_branch: pa.typing.Series[str]
-    special: pa.typing.Series[str] = pa.Field(nullable=True)
+    change_reason: pa.typing.Series[str]
+    capitalization: pa.typing.Series[int]
+    outstanding_shares_a: pa.typing.Series[int]
+    limited_shares_a: pa.typing.Series[float] = pa.Field(nullable=True)
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
-def get_block_deal(
+@api
+def get_equity_change(
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
 ) -> pa.typing.DataFrame[Output]:
-    """获取大宗交易数据.
+    """获取股本变动数据.
 
-    参考文档: https://www.lixinger.com/open/api/doc?api-key=cn/company/block-deal
+    参考文档: https://www.lixinger.com/open/api/doc?api-key=cn/company/equity-change
     """
     payload = {
         "token": settings.token,
         "startDate": start_date,
         "stockCode": stock_code,
     }
     if end_date is not None:
         payload["endDate"] = end_date
     if limit is not None:
         payload["limit"] = limit
 
     response = requests.post(
-        f"{settings.base_url}/cn/company/block-deal",
+        f"{settings.base_url}/cn/company/equity-change",
         json=payload,
     )
     df = get_response_df(response, Output)
     return df
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/candlestick.py` & `lixinger-0.1.7/lixinger/api/cn/company/candlestick.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from __future__ import annotations
 
 from typing import Literal
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     open: pa.typing.Series[float]
     high: pa.typing.Series[float]
     low: pa.typing.Series[float]
     close: pa.typing.Series[float]
     volume: pa.typing.Series[int]
     amount: pa.typing.Series[int]
     change: pa.typing.Series[float]
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
+@api
 def get_candlestick(
     type_: Literal["ex_rights", "lxr_fc_rights", "fc_rights", "bc_rights"],
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     adjust_forward_date: str | None = None,
     adjust_backward_date: str | None = None,
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/dividend_and_alloment.py` & `lixinger-0.1.7/lixinger/api/cn/company/dividend_and_alloment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import pandas as pd
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     bonus_shares_from_profit: pa.typing.Series[int]
     bonus_shares_from_capital_reserve: pa.typing.Series[int]
     dividend: pa.typing.Series[float]
@@ -19,17 +18,15 @@
     ex_date: pa.typing.Series[pa.typing.DateTime] = pa.Field(nullable=True)
     payment_date: pa.typing.Series[pa.typing.DateTime] = pa.Field(nullable=True)
     status: pa.typing.Series[str]
     original_value: pa.typing.Series[float]
     split_ratio: pa.typing.Series[float] = pa.Field(nullable=True)
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
+@api
 def get_dividend_and_alloment(
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
 ) -> pa.typing.DataFrame[Output]:
     """获取分红送配信息.
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/equity_change.py` & `lixinger-0.1.7/lixinger/api/cn/fund/exchange_traded_close_price.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
-    change_reason: pa.typing.Series[str]
-    capitalization: pa.typing.Series[int]
-    outstanding_shares_a: pa.typing.Series[int]
-    limited_shares_a: pa.typing.Series[float] = pa.Field(nullable=True)
+    open: pa.typing.Series[float]
+    high: pa.typing.Series[float]
+    low: pa.typing.Series[float]
+    close: pa.typing.Series[float]
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
-def get_equity_change(
+@api
+def get_exchange_traded_close_price(
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
 ) -> pa.typing.DataFrame[Output]:
-    """获取股本变动数据.
+    """场内基金收盘价数据.
 
-    参考文档: https://www.lixinger.com/open/api/doc?api-key=cn/company/equity-change
+    参考文档: https://www.lixinger.com/open/api/doc?api-key=cn/fund/exchange-traded-close-price
     """
     payload = {
         "token": settings.token,
         "startDate": start_date,
         "stockCode": stock_code,
     }
     if end_date is not None:
         payload["endDate"] = end_date
     if limit is not None:
         payload["limit"] = limit
 
     response = requests.post(
-        f"{settings.base_url}/cn/company/equity-change",
+        f"{settings.base_url}/cn/fund/exchange-traded-close-price",
         json=payload,
     )
     df = get_response_df(response, Output)
     return df
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/indices.py` & `lixinger-0.1.7/lixinger/api/cn/company/indices.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     area_code: pa.typing.Series[str]
     stock_code: pa.typing.Series[str]
     source: pa.typing.Series[str]
 
 
-@validate_arguments
-@pa.check_types
+@api
 def get_indices(
     stock_code: str,
     date: str | None = None,
 ) -> pa.typing.DataFrame[Output]:
     """获取股票所属指数信息.
 
     参考文档: https://www.lixinger.com/open/api/doc?api-key=cn/company/indices
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/industries.py` & `lixinger-0.1.7/lixinger/api/cn/company/industries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     area_code: pa.typing.Series[str]
     stock_code: pa.typing.Series[str]
     source: pa.typing.Series[str]
 
 
-@validate_arguments
-@pa.check_types
+@api
 def get_industries(
     stock_code: str,
     date: str | None = None,
 ) -> pa.typing.DataFrame[Output]:
     """获取股票所属行业信息.
 
     参考文档: https://www.lixinger.com/open/api/doc?api-key=cn/company/industries
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/pledge.py` & `lixinger-0.1.7/lixinger/api/cn/company/pledge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     pledgor: pa.typing.Series[str] = pa.Field(nullable=True)
     pledgee: pa.typing.Series[str] = pa.Field(nullable=True)
     pledge_matters: pa.typing.Series[str] = pa.Field(nullable=True)
@@ -25,17 +24,15 @@
     pledge_discharge_amount: pa.typing.Series[float] = pa.Field(nullable=True)
     is_pledge_repurchase_transactions: pa.typing.Series[bool] = pa.Field(nullable=True)
     accumulated_pledge_percentage_of_total_equity: pa.typing.Series[float] = pa.Field(
         nullable=True
     )
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
+@api
 def get_pledge(
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
 ) -> pa.typing.DataFrame[Output]:
     """获取股权质押数据.
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/senior_executive_shares_change.py` & `lixinger-0.1.7/lixinger/api/cn/company/senior_executive_shares_change.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     shareholder_name: pa.typing.Series[str]
     executive_name: pa.typing.Series[str]
     duty: pa.typing.Series[str]
     relation_between_e_s: pa.typing.Series[str]
     change_reason: pa.typing.Series[str]
     before_change_shares: pa.typing.Series[int]
     changed_shares: pa.typing.Series[int]
     after_change_shares: pa.typing.Series[int]
     avg_price: pa.typing.Series[float]
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
+@api
 def get_senior_executive_shares_change(
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
 ) -> pa.typing.DataFrame[Output]:
     """获取高管增减持数据.
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/company/shareholders_num.py` & `lixinger-0.1.7/lixinger/api/cn/company/shareholders_num.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     num: pa.typing.Series[int]
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
+@api
 def get_shareholders_num(
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
 ) -> pa.typing.DataFrame[Output]:
     """获取股东人数数据
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/fund/total_net_value.py` & `lixinger-0.1.7/lixinger/api/cn/fund/total_net_value.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     total_net_value: pa.typing.Series[float]
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
+@api
 def get_total_net_value(
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
 ) -> pa.typing.DataFrame[Output]:
     """获取基金累计净值数据
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/index/candlestick.py` & `lixinger-0.1.7/lixinger/api/cn/index/candlestick.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from __future__ import annotations
 
 from typing import Literal
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     open: pa.typing.Series[float]
     high: pa.typing.Series[float]
     low: pa.typing.Series[float]
     close: pa.typing.Series[float]
     volume: pa.typing.Series[int]
     amount: pa.typing.Series[int]
     change: pa.typing.Series[float]
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
+@api
 def get_candlestick(
     type_: Literal["normal", "total_return"],
     start_date: str,
     stock_code: str,
     end_date: str | None = None,
     limit: int | None = None,
 ) -> pa.typing.DataFrame[Output]:
```

### Comparing `lixinger-0.1.6/lixinger/api/cn/index/fundamental.py` & `lixinger-0.1.7/lixinger/api/cn/index/fundamental.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from __future__ import annotations
 
 import pandera as pa
 import requests
-from pydantic import validate_arguments
 
 from lixinger.config import settings
-from lixinger.utils import adjust_request_date_range, get_response_df
+from lixinger.utils import api, get_response_df
 
 
 class Output(pa.DataFrameModel):
     date: pa.typing.Series[pa.typing.DateTime]
     stock_code: pa.typing.Series[str]
 
 
-@validate_arguments
-@pa.check_types
-@adjust_request_date_range
+@api
 def get_index_fundamental(
     stock_codes: list[str],
     metrics_list: list[str],
     date: str | None = None,
     start_date: str | None = None,
     end_date: str | None = None,
     adjust_forward_date: str | None = None,
```

### Comparing `lixinger-0.1.6/lixinger/config.py` & `lixinger-0.1.7/lixinger/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import os
 import pathlib
+from typing import Callable
 
 from dynaconf import Dynaconf, Validator
 
 DEFAULT_SETTINGS_PATH: pathlib.Path = (
     pathlib.Path(__file__).resolve().parent / "settings.toml"
 )
 USER_SETTINGS_PATH: pathlib.Path = (
@@ -16,18 +17,18 @@
     .resolve()
 )
 
 
 settings_cast_map = {}
 
 
-def cast(v: str) -> callable:
+def cast(v: str) -> Callable:
     """Decorator to register cast function for a setting."""
 
-    def decorator(func) -> callable:
+    def decorator(func) -> Callable:
         settings_cast_map[v] = func
         return func
 
     return decorator
 
 
 class TypedDynaconf(Dynaconf):
```

### Comparing `lixinger-0.1.6/pyproject.toml` & `lixinger-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache/"
 addopts = "-s -p no:warnings"
 asyncio_mode = "auto"
 
 [project]
 name = "lixinger"
-version = "0.1.6"
+version = "0.1.7"
 description = "Lixinger SDK for Python (Unofficial)"
 authors = [
     { name = "Chaoying", email = "chaoying2022@gmail.com" },
 ]
 dependencies = [
     "pandera>=0.14.5",
     "pydantic>=1.10.7",
```

### Comparing `lixinger-0.1.6/PKG-INFO` & `lixinger-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lixinger
-Version: 0.1.6
+Version: 0.1.7
 Summary: Lixinger SDK for Python (Unofficial)
 Keywords: lixinger
 Author-Email: Chaoying <chaoying2022@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,46 +20,51 @@
 # lixinger
 
 理杏仁 Python SDK (非官方).
 
 包含以下功能：
 
 - 自动将请求结果转换结果为 Dataframe.
-- 根据官方文档中的返回结果定义, 验证请求结果, 对缺少的列进行补齐, 对列类型进行转换.
-- 支持一次获取时间范围大于10年的数据.
+- 根据官方文档中的返回结果定义, 验证请求结果, 对缺少的列进行补齐, 对列类型进行相应转换.
+- 支持一次获取时间范围大于 10 年的数据.
+- 适当缓存请求结果，减少请求 API 次数.
 
 ## 安装
 
 ```bash
 pip install lixinger
 ```
 
 ## 用法
 
-### 设置 Token 
+### 设置 Token
 
 Token 获取地址为 [https://www.lixinger.com/open/api/token](https://www.lixinger.com/open/api/token)
 
-#### 方式1：通过环境变量来设置 Token
+#### 方式 1：通过环境变量来设置 Token
 
 ```bash
 export LIXINGER_TOKEN="你的 token"
 ```
 
-#### 方式2：通过配置文件来设置 Token
+#### 方式 2：通过配置文件来设置 Token
+
 打开配置文件（路径为 ~/.config/lixinger/settings.toml），并添加以下内容设置自己的 Token.
 
 ```toml
 [default]
 token = "你的 token"
 ```
 
 ### 调用 API
+
 使用文档请参考 [理杏仁开放平台](https://www.lixinger.com/open/api/doc)
 
+方法导入路径可以根据文档中的请求 URL 得出，例如下面代码中对应的请求 URL 为 `/api/cn/company` 则把 `/` 换成 `.` 即可.
+
 ```python
 from lixinger.api.cn.company.base import get_company
 
 # 获取股票详细信息
 company = get_company(stock_codes=["600519"])
 print(company)
 ```
```

