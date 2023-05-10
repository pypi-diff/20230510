# Comparing `tmp/pywencai-0.7.1.tar.gz` & `tmp/pywencai-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.7.1.tar", max compression
+gzip compressed data, was "pywencai-0.8.0.tar", max compression
```

## Comparing `pywencai-0.7.1.tar` & `pywencai-0.8.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-01 04:28:42.043050 pywencai-0.7.1/LICENSE
--rw-r--r--   0        0        0     2310 2023-05-01 04:28:42.043050 pywencai-0.7.1/README.md
--rw-r--r--   0        0        0      530 2023-05-01 04:28:42.043050 pywencai-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-01 04:28:42.043050 pywencai-0.7.1/pywencai/__init__.py
--rw-r--r--   0        0        0    39677 2023-05-01 04:28:42.043050 pywencai-0.7.1/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4241 2023-05-01 04:28:42.043050 pywencai-0.7.1/pywencai/wencai.py
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 pywencai-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 05:11:57.659710 pywencai-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2446 2023-05-10 05:11:57.659710 pywencai-0.8.0/README.md
+-rw-r--r--   0        0        0      613 2023-05-10 05:11:57.659710 pywencai-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-10 05:11:57.659710 pywencai-0.8.0/pywencai/__init__.py
+-rw-r--r--   0        0        0     3559 2023-05-10 05:11:57.659710 pywencai-0.8.0/pywencai/convert.py
+-rw-r--r--   0        0        0    39677 2023-05-10 05:11:57.659710 pywencai-0.8.0/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4262 2023-05-10 05:11:57.659710 pywencai-0.8.0/pywencai/wencai.py
+-rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 pywencai-0.8.0/PKG-INFO
```

### Comparing `pywencai-0.7.1/LICENSE` & `pywencai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.7.1/README.md` & `pywencai-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,17 @@
 
 #### cookie
 
 非必填，默认为None，付费版可以尝试传入cookie，获取付费使用权限。
 
 ### 返回值
 
-该方法返回一个`pandas`的`Dataframe`
+当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
+
+当查询的是详情是，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
 
 ## 联系方式
 
 欢迎加入QQ群，分享量化技术！
 
 <img src="./qrcode.png" width=400>
```

### Comparing `pywencai-0.7.1/pyproject.toml` & `pywencai-0.8.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.7.1"
+version = "0.8.0"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
@@ -12,14 +12,18 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 PyExecJS = "^1.5.1"
 requests = "*"
 pandas = {version = "^1.5.0 || ^2.0.0"}
 fake-useragent = "^1.1.1"
+pydash = "^7.0.3"
 
 [tool.poetry.group.dev.dependencies]
 notebook = "^6.4.12"
+mypy = "^1.2.0"
+autopep8 = "^2.0.2"
+types-requests = "^2.30.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pywencai-0.7.1/pywencai/hexin-v.js` & `pywencai-0.8.0/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.7.1/pywencai/wencai.py` & `pywencai-0.8.0/pywencai/wencai.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,169 +2,159 @@
 import execjs
 import json
 import requests as rq
 import pandas as pd
 import time
 import logging
 from fake_useragent import UserAgent
+from pywencai.convert import convert_params
+import pydash as _
 
 ua = UserAgent()
 
 logging.basicConfig(
     level=logging.INFO,
     format='[pywencai] %(asctime)s - %(levelname)s - %(message)s'
 )
 
-# 获取token
+
 def get_token():
-  with open(os.path.join(os.path.dirname(__file__), 'hexin-v.js'), 'r') as f:
-    jscontent = f.read()
-  context= execjs.compile(jscontent)
-  return context.call("v")
+    '''获取token'''
+    with open(os.path.join(os.path.dirname(__file__), 'hexin-v.js'), 'r') as f:
+        jscontent = f.read()
+    context = execjs.compile(jscontent)
+    return context.call("v")
+
 
-# 获取condition
 def get_robot_data(**kwargs):
-  retry = kwargs.get('retry', 10)
-  sleep = kwargs.get('sleep', 0)
-  question = kwargs.get('query')
-  log = kwargs.get('log', False)
-  query_type = kwargs.get('query_type', 'stock')
-  cookie = kwargs.get('cookie', None)
-  data = {
-    'perpage': 10,
-    'page': 1,
-    'source': 'Ths_iwencai_Xuangu',
-    'secondary_intent': query_type,
-    'question': question
-  }
-
-  count = 0
-  log and logging.info(f'获取condition开始')
-
-  while count < retry :
-    time.sleep(sleep)
-    res = rq.request(
-      method='POST',
-      url='http://www.iwencai.com/customized/chart/get-robot-data',
-      json=data,
-      headers={
-        'hexin-v': get_token(),
-        'User-Agent': ua.random,
-        'cookie': cookie
-      }
-    )
-    result = json.loads(res.text)
-    content = result['data']['answer'][0]['txt'][0]['content']
-    if type(content) == str:
-      content = json.loads(content)
-    components0 = content['components'][0]
-    meta = components0['data']['meta']
-    params = {}
-    if meta:
-      params = {
-        'condition': components0['data']['meta']['extra']['condition'],
-        'comp_id': components0['cid'],
-        'uuid': components0['puuid']
-      }
-    else:
-      datas = components0['data']['datas']
-      params = {
-        'datas': pd.DataFrame.from_dict(datas)
-      }
-    
-    log and logging.info(f'获取get_robot_data成功')
-    return params
-  log and logging.info(f'获取get_robot_data失败')
-  return None
+    '''获取condition'''
+    retry = kwargs.get('retry', 10)
+    sleep = kwargs.get('sleep', 0)
+    question = kwargs.get('query')
+    log = kwargs.get('log', False)
+    query_type = kwargs.get('query_type', 'stock')
+    cookie = kwargs.get('cookie', None)
+    data = {
+        'perpage': 10,
+        'page': 1,
+        'source': 'Ths_iwencai_Xuangu',
+        'secondary_intent': query_type,
+        'question': question
+    }
+
+    count = 0
+    log and logging.info(f'获取condition开始')
+
+    while count < retry:
+        time.sleep(sleep)
+        res = rq.request(
+            method='POST',
+            url='http://www.iwencai.com/customized/chart/get-robot-data',
+            json=data,
+            headers={
+                'hexin-v': get_token(),
+                'User-Agent': ua.random,
+                'cookie': cookie
+            }
+        )
+        params = convert_params(res)
+        log and logging.info(f'获取get_robot_data成功')
+        return params
+    log and logging.info(f'获取get_robot_data失败')
+    return None
+
 
-# 替换key
 def replace_key(key):
+    '''替换key'''
     key_map = {
         'question': 'query',
         'sort_key': 'urp_sort_index',
         'sort_order': 'urp_sort_way'
     }
     return key_map.get(key, key)
 
 
-# 获取每页数据
 def get_page(**kwargs):
-  retry = kwargs.pop('retry', 10)
-  sleep = kwargs.pop('sleep', 0)
-  log = kwargs.pop('log', False)
-  cookie = kwargs.pop('cookie', None)
-
-  data = {
-    'perpage': 100,
-    'page': 1,
-    'source': 'Ths_iwencai_Xuangu',
-    **kwargs
-  }
-  count = 0
-  log and logging.info(f'第{data.get("page")}页开始')
-
-  while count < retry :
-    time.sleep(sleep)
-    try: 
-      res = rq.request(
-        method='POST',
-        url='http://www.iwencai.com/gateway/urp/v7/landing/getDataList',
-        data=data,
-        headers={
-          'hexin-v': get_token(),
-          'User-Agent': ua.random,
-          'cookie': cookie
-        },
-        timeout=(5, 10)
-      )
-      result = json.loads(res.text)
-      list = result['answer']['components'][0]['data']['datas']
-      log and logging.info(f'第{data.get("page")}页成功')
-      return pd.DataFrame.from_dict(list)
-    except:
-      log and logging.warning(f'{count+1}次尝试失败')
-      count+=1
-  log and logging.error(f'第{data.get("page")}页失败')
-  return pd.DataFrame.from_dict([])
-  
+    '''获取每页数据'''
+    retry = kwargs.pop('retry', 10)
+    sleep = kwargs.pop('sleep', 0)
+    log = kwargs.pop('log', False)
+    cookie = kwargs.pop('cookie', None)
+
+    data = {
+        'perpage': 100,
+        'page': 1,
+        'source': 'Ths_iwencai_Xuangu',
+        **kwargs
+    }
+    count = 0
+    log and logging.info(f'第{data.get("page")}页开始')
+
+    while count < retry:
+        time.sleep(sleep)
+        try:
+            res = rq.request(
+                method='POST',
+                url='http://www.iwencai.com/gateway/urp/v7/landing/getDataList',
+                data=data,
+                headers={
+                    'hexin-v': get_token(),
+                    'User-Agent': ua.random,
+                    'cookie': cookie
+                },
+                timeout=(5, 10)
+            )
+            result = json.loads(res.text)
+            list = result['answer']['components'][0]['data']['datas']
+            log and logging.info(f'第{data.get("page")}页成功')
+            return pd.DataFrame.from_dict(list)
+        except:
+            log and logging.warning(f'{count+1}次尝试失败')
+            count += 1
+    log and logging.error(f'第{data.get("page")}页失败')
+    return pd.DataFrame.from_dict([])
+
 
-# 是否继续循环
 def can_loop(loop, count):
-  if (loop is True):
-    return True
-  else: 
-    return count < loop
+    '''是否继续循环'''
+    if (loop is True):
+        return True
+    else:
+        return count < loop
+
 
-# 循环分页
 def loop_page(loop, **kwargs):
-  count = 0
-  resultPageLen = 1
-  result = None
-  if 'page' not in kwargs:
-    kwargs['page'] = 1
-  initPage = kwargs['page']
-
-  while resultPageLen > 0 and can_loop(loop, count):
-    kwargs['page'] = initPage + count
-    resultPage = get_page(**kwargs)
-    resultPageLen = len(resultPage)
-    count = count + 1
-    if result is None:
-      result = resultPage
-    else:
-      result = pd.concat([result, resultPage], ignore_index=True)
-  
-  return result
+    '''循环分页'''
+    count = 0
+    resultPageLen = 1
+    result = None
+    if 'page' not in kwargs:
+        kwargs['page'] = 1
+    initPage = kwargs['page']
+
+    while resultPageLen > 0 and can_loop(loop, count):
+        kwargs['page'] = initPage + count
+        resultPage = get_page(**kwargs)
+        resultPageLen = len(resultPage)
+        count = count + 1
+        if result is None:
+            result = resultPage
+        else:
+            result = pd.concat([result, resultPage], ignore_index=True)
+
+    return result
+
 
-# 获取结果
 def get(loop=False, **kwargs):
-  kwargs = {replace_key(key): value for key, value in kwargs.items()}
-  params = get_robot_data(**kwargs)
-  datas = params.get('datas', None)
-  if datas is not None:
-    return datas
-  else:
-    kwargs = {**kwargs, **params}
-    if loop:
-      return loop_page(loop, **kwargs)
+    '''获取结果'''
+    kwargs = {replace_key(key): value for key, value in kwargs.items()}
+    params = get_robot_data(**kwargs)
+    data = params.get('data')
+    condition = data.get('condition')
+    if condition is not None:
+        kwargs = {**kwargs, **data}
+        if loop:
+            return loop_page(loop, **kwargs)
+        else:
+            return get_page(**kwargs)
     else:
-      return get_page(**kwargs)
+        return data
```

### Comparing `pywencai-0.7.1/PKG-INFO` & `pywencai-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.7.1
+Version: 0.8.0
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyExecJS (>=1.5.1,<2.0.0)
 Requires-Dist: fake-useragent (>=1.1.1,<2.0.0)
 Requires-Dist: pandas (>=1.5.0,<3.0.0)
+Requires-Dist: pydash (>=7.0.3,<8.0.0)
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/pywencai.svg)](https://badge.fury.io/py/pywencai)
 [![Downloads](https://static.pepy.tech/badge/pywencai/month)](https://pepy.tech/project/pywencai)
 # pywencai
 
@@ -113,15 +114,17 @@
 
 #### cookie
 
 非必填，默认为None，付费版可以尝试传入cookie，获取付费使用权限。
 
 ### 返回值
 
-该方法返回一个`pandas`的`Dataframe`
+当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
+
+当查询的是详情是，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
 
 ## 联系方式
 
 欢迎加入QQ群，分享量化技术！
 
 <img src="./qrcode.png" width=400>
```

