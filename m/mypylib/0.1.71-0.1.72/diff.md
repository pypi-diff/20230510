# Comparing `tmp/mypylib-0.1.71.tar.gz` & `tmp/mypylib-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.71.tar", last modified: Thu Apr 27 13:12:10 2023, max compression
+gzip compressed data, was "mypylib-0.1.72.tar", last modified: Wed May 10 09:28:57 2023, max compression
```

## Comparing `mypylib-0.1.71.tar` & `mypylib-0.1.72.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-27 13:12:10.191868 mypylib-0.1.71/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-04-27 13:12:10.191624 mypylib-0.1.71/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.71/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-27 13:12:10.188927 mypylib-0.1.71/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.71/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    47074 2023-04-27 13:11:20.000000 mypylib-0.1.71/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.71/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.71/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.71/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.71/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.71/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24230 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.71/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.71/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.71/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.71/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.71/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7662 2022-06-02 06:59:21.000000 mypylib-0.1.71/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-27 13:12:10.191007 mypylib-0.1.71/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.71/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.71/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.71/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.71/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.71/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-27 13:12:10.190471 mypylib-0.1.71/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-04-27 13:12:09.000000 mypylib-0.1.71/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-04-27 13:12:10.000000 mypylib-0.1.71/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-04-27 13:12:09.000000 mypylib-0.1.71/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-04-27 13:12:09.000000 mypylib-0.1.71/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-04-27 13:12:10.191966 mypylib-0.1.71/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.71/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-10 09:28:57.217402 mypylib-0.1.72/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-10 09:28:57.217126 mypylib-0.1.72/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.72/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-10 09:28:57.213919 mypylib-0.1.72/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.72/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    46777 2023-05-10 09:27:59.000000 mypylib-0.1.72/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.72/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.72/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.72/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.72/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.72/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24230 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.72/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.72/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.72/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.72/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.72/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7662 2022-06-02 06:59:21.000000 mypylib-0.1.72/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-10 09:28:57.216114 mypylib-0.1.72/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.72/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.72/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.72/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.72/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.72/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-10 09:28:57.215544 mypylib-0.1.72/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-10 09:28:56.000000 mypylib-0.1.72/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-05-10 09:28:57.000000 mypylib-0.1.72/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-05-10 09:28:56.000000 mypylib-0.1.72/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-05-10 09:28:56.000000 mypylib-0.1.72/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-05-10 09:28:57.217512 mypylib-0.1.72/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.72/setup.py
```

### Comparing `mypylib-0.1.71/README.md` & `mypylib-0.1.72/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.72/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/__init__.py` & `mypylib-0.1.72/mypylib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import requests
 
 ssl._create_default_https_context = ssl._create_unverified_context
 from termcolor import cprint
 from inspect import currentframe
 
-__version__ = '0.1.71'
+__version__ = '0.1.72'
 
 __info__ = {
     '2022/01/04: 0.1.18 加入 __info__。',
     '2022/01/04: 0.1.18 Carey修改 MVP的部分。',
     '2022/01/05: 0.1.19 add check_place_cover 預防漲停鎖住',
     '2022/01/06: 0.1.20 add get_stock_future_data(). 用來抓取每天股票期貨資料',
     '2022/01/06: 0.1.20 add get_stock_future_snapshot(). 用來抓每天股票、股票期貨漲停、跌停價格',
@@ -60,14 +60,15 @@
     '2023/02/12: 0.1.65 修改 sjtools parse timestamp的方法，以免crash',
     '2023/02/13: 0.1.66 Move toggle_btn_off and toggle_btn_on here ',
     '2023/02/23: 0.1.67 get_new_warrant_list() 元富修改網站，封鎖 read_html()',
     '2023/03/15: 0.1.68 修正一些宣告',
     '2023/04/11: 0.1.69 換成shioaji 1.0 API',
     '2023/04/18: 0.1.70 Market() 增加 ask bid information',
     '2023/04/27: 0.1.71 tplaysound 減少buffer音量以免很吵',
+    '2023/05/10: 0.1.72 改用shioaji API'
 
 }
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
@@ -132,31 +133,31 @@
 
 
 def __LINE__():
     cf = currentframe()
     return cf.f_back.f_lineno
 
 
-def get_all_stock_code_name_dict(id='PAPIUSER08', password='2222', _api=None):
+def get_all_stock_code_name_dict(_api=None):
     today = datetime.datetime.today()
 
     cache_file = f'all_stock_code-{today.strftime("%Y%m%d")}.json'
 
     if not os.path.isfile(cache_file):
 
         import shioaji as sj
 
         if _api is None:
-            def simu_login(id=id, password=password):
-                print(f'使用測試帳號 {id} {password}')
+            def login():
                 api = sj.Shioaji()
-                api.login(id, password, contracts_cb=lambda security_type: print(f"{repr(security_type)} fetch done."))
+                api.login(api_key='6Dkp67EVdMQBWE8Z6DZ5zPQAFTbvVPxEGzAEFiZ5ByhN',
+                          secret_key='2NCQAhfP73PfKYaAi8xJVHZSp4Y91mSNViiFU7zQ19T2')
                 return api
 
-            api = simu_login()
+            api = login()
         else:
             api = _api
 
         all_code_name_dir = {}
         for x in api.Contracts.Stocks.OTC:
             if len(x.code) == 4:
                 all_code_name_dir[x.code] = x.name
@@ -244,25 +245,18 @@
 
     return top_future_rank
 
 
 def get_stock_future_snapshot(filename='stock_future_snapshot.txt'):
     import shioaji as sj
 
-    def login(id='H121933940',
-              password='123',
-              ca_path="SinoPac.pfx",
-              ca_password='H121933940',
-              person_id='H121933940'):
-        print(f'使用正式帳號 {id} {password}')
+    def login():
         api = sj.Shioaji()
-        api.login(id,
-                  password,
-                  contracts_cb=lambda security_type: print(f"{repr(security_type)} fetch done.")
-                  )
+        api.login(api_key='6Dkp67EVdMQBWE8Z6DZ5zPQAFTbvVPxEGzAEFiZ5ByhN',
+                  secret_key='2NCQAhfP73PfKYaAi8xJVHZSp4Y91mSNViiFU7zQ19T2')
         return api
 
     api = login()
 
     contracts = []
 
     for x in api.Contracts.Futures:
@@ -912,16 +906,16 @@
         print(100, 6, price_ticks_offset_AB_dec(100, 6))
         print(99.8, 6, price_ticks_offset_AB_dec(99.8, 6))
         print(101.5, 6, price_ticks_offset_AB_dec(101.5, 6))
         print(50.2, 6, price_ticks_offset_AB_dec(50.2, 6))
         print(50, 6, price_ticks_offset_AB_dec(50, 6))
         print(49.9, 6, price_ticks_offset_AB_dec(49.9, 6))
 
-    if False:
-        print(get_all_stock_code_name_dict('H121933940', '123edcxzaqws'))
+    if True:
+        print(get_all_stock_code_name_dict())
 
     if False:
         ret = get_trade_days()
         print(ret)
 
         exit(0)
```

### Comparing `mypylib-0.1.71/mypylib/binance_copy_bot.py` & `mypylib-0.1.72/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.72/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/chdbif.py` & `mypylib-0.1.72/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/crypto.py` & `mypylib-0.1.72/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/finmind.py` & `mypylib-0.1.72/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/libexcel.py` & `mypylib-0.1.72/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/mvp.py` & `mypylib-0.1.72/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/mytest.py` & `mypylib-0.1.72/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/option_test.py` & `mypylib-0.1.72/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.72/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/shioaji_kline.py` & `mypylib-0.1.72/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/shioaji_ticks.py` & `mypylib-0.1.72/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/sjtools.py` & `mypylib-0.1.72/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/tLineNotify.py` & `mypylib-0.1.72/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/ti.py` & `mypylib-0.1.72/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.72/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/tplaysound.py` & `mypylib-0.1.72/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/tredis.py` & `mypylib-0.1.72/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib/warrant.py` & `mypylib-0.1.72/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.72/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.71/setup.py` & `mypylib-0.1.72/setup.py`

 * *Files identical despite different names*

