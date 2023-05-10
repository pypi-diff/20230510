# Comparing `tmp/apitest_ezgo-2.0.1-py2.py3-none-any.whl.zip` & `tmp/apitest_ezgo-2.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 14004 bytes, number of entries: 15
+Zip file size: 14315 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     5287 b- defN 23-Apr-23 02:33 apitest_ezgo/Compare.py
--rw-rw-rw-  2.0 fat    10011 b- defN 23-Apr-23 07:34 apitest_ezgo/DbHelper.py
--rw-rw-rw-  2.0 fat     4035 b- defN 23-Apr-10 07:13 apitest_ezgo/FastRequest.py
--rw-rw-rw-  2.0 fat      237 b- defN 23-Apr-23 06:32 apitest_ezgo/__about__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Feb-09 11:57 apitest_ezgo/__init__.py
+-rw-rw-rw-  2.0 fat    10168 b- defN 23-May-09 06:52 apitest_ezgo/DbHelper.py
+-rw-rw-rw-  2.0 fat     4629 b- defN 23-May-09 08:19 apitest_ezgo/FastRequest.py
+-rw-rw-rw-  2.0 fat      237 b- defN 23-May-10 02:12 apitest_ezgo/__about__.py
+-rw-rw-rw-  2.0 fat      160 b- defN 23-Apr-26 07:00 apitest_ezgo/__init__.py
 -rw-rw-rw-  2.0 fat      901 b- defN 23-Apr-21 09:59 apitest_ezgo/compat.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-16 03:14 apitest_ezgo/Har2Template/__init__.py
 -rw-rw-rw-  2.0 fat     1844 b- defN 23-Apr-23 06:27 apitest_ezgo/Har2Template/cli.py
 -rw-rw-rw-  2.0 fat     6466 b- defN 23-Apr-21 09:44 apitest_ezgo/Har2Template/core.py
 -rw-rw-rw-  2.0 fat     3506 b- defN 23-Apr-21 09:44 apitest_ezgo/Har2Template/utils.py
--rw-rw-rw-  2.0 fat      501 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       69 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1263 b- defN 23-Apr-23 07:37 apitest_ezgo-2.0.1.dist-info/RECORD
-15 files, 34296 bytes uncompressed, 11894 bytes compressed:  65.3%
+-rw-rw-rw-  2.0 fat      501 b- defN 23-May-10 02:13 apitest_ezgo-2.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-10 02:13 apitest_ezgo-2.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       69 b- defN 23-May-10 02:13 apitest_ezgo-2.0.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-May-10 02:13 apitest_ezgo-2.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1264 b- defN 23-May-10 02:13 apitest_ezgo-2.0.3.dist-info/RECORD
+15 files, 35155 bytes uncompressed, 12205 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: apitest_ezgo/Har2Template/core.py
 Comment: 
 
 Filename: apitest_ezgo/Har2Template/utils.py
 Comment: 
 
-Filename: apitest_ezgo-2.0.1.dist-info/METADATA
+Filename: apitest_ezgo-2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: apitest_ezgo-2.0.1.dist-info/WHEEL
+Filename: apitest_ezgo-2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: apitest_ezgo-2.0.1.dist-info/entry_points.txt
+Filename: apitest_ezgo-2.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: apitest_ezgo-2.0.1.dist-info/top_level.txt
+Filename: apitest_ezgo-2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: apitest_ezgo-2.0.1.dist-info/RECORD
+Filename: apitest_ezgo-2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## apitest_ezgo/DbHelper.py

```diff
@@ -1,14 +1,15 @@
 # coding:utf-8
 """
 @date: 2023/2/23
 @author: mawengang
 """
-from DBUtils.PooledDB import PooledDB
+import traceback
 from robot.api import logger
+from DBUtils.PooledDB import PooledDB
 
 
 class Config():
     # 数据库连接编码
     # DB_CHARSET = "utf-8"
 
     # mincached : 启动时开启的闲置连接数量(缺省值 0 开始时不创建连接)
@@ -132,15 +133,16 @@
                 count = cursor.execute(sql, param)
             else:
                 count = cursor.execute(sql)
             conn.commit()
             if autoclose:
                 self.close(cursor, conn)
         except Exception as e:
-            pass
+            traceback.print_exc()
+            # logger.warn(traceback.format_exc(e))
         return cursor, conn, count
 
     # 执行多条命令
     def executemany(self, lis):
         """
         :param lis: 是一个列表，里面放的是每个sql的字典'[{"sql":"xxx","param":"xx"}....]'
         :return:
@@ -158,14 +160,15 @@
                 else:
                     cursor.execute(sql)
             conn.commit()
             self.close(cursor, conn)
             return True
         except Exception as e:
             print(e)
+            traceback.print_exc()
             conn.rollback()
             self.close(cursor, conn)
             return False
 
     # 释放连接
     def close(self, cursor, conn):
         """释放连接归还给连接池"""
@@ -179,14 +182,15 @@
             res = cursor.fetchall()
             print(res)
             if self.cursor_factory and res:
                 res = [dict(i) for i in res]
             return [] if res == 0 else res
         except Exception as e:
             print(e)
+            traceback.print_exc()
             self.close(cursor, conn)
             return [] if self.cursor_factory else count
 
     # 查询单条
     def select_one(self, sql, param=None):
         cursor, conn, count = self.execute(sql, param)
         try:
```

## apitest_ezgo/FastRequest.py

```diff
@@ -3,14 +3,15 @@
 @date: 2023/2/9
 @author: mawengang
 """
 
 import logging
 import os
 import json
+import random
 import requests
 import jsonpath_ng
 from jsonpath import jsonpath
 from requests.adapters import HTTPAdapter
 
 
 def update_req_info(replace_dict, req_info):
@@ -32,15 +33,15 @@
 
     # 删除请求参数为{REMOVE}的
     parser = jsonpath_ng.parse("$..*")
     parser.filter(lambda x: x == '{REMOVE}', req_info)
 
 
 def load_req_info(file_path):
-    with open(file_path, "r") as f:
+    with open(file_path, "r", encoding="utf-8") as f:
         return json.load(f)
 
 
 class FastRequest(object):
     def __init__(self, template_path="", base_url="", session=None):
         """
         Http对象
@@ -55,21 +56,22 @@
         # http适配器，自动重试次数3
         adapter = HTTPAdapter(max_retries=3, pool_connections=3, pool_maxsize=5)
         # http和https都适用适配器
         self.session.mount('http://', adapter)
         self.session.mount('https://', adapter)
         # @TODO session管理器
 
-    def fast_request(self, request_name, file_path='', resp_jpath=None, session=None, **replace_dict):
+    def fast_request(self, request_name, file_path='', resp_jpath=None, session=None, index=0, **replace_dict):
         """
         支持各类请求方式各类content-type的请求入口
         @param file_path: json文件路径，可为相对于template_path的相对路径，不传时template_path需要到文件
         @param request_name: json文件中请求的名称，即字典名称
         @param resp_jpath: 需要提取响应数据的jsonpath
         @param session: 支持临时session请求，不传默认使用实例session
+        @param index: 返回数据的索引，默认为0， 只能传入数字或 random； random表示从列表中随机抽取一个
         @param replace_dict:需要更新请求参数，传入对应jpath 和 值，如果需要将某个参数从请求中删除，将值更新为{REMOVE}
                             例如{"$.headers.User-Agent": "new agent", "$..sec-ch-ua": '{REMOVE}'}
         @return: 传入resp_jpath取对应数据，默认返回响应对象
         """
         path = os.path.join(self.template_path, file_path) if (self.template_path and file_path) \
             else (file_path if file_path else self.template_path)
         req_info = load_req_info(path).get(request_name)
@@ -86,10 +88,20 @@
         logging.info(u"请求信息：\n %s" % req_info)
         if session:
             resp = session.request(url=url, **req_info)
         else:
             resp = self.session.request(url=url, **req_info)
         msg = u"请求status_code： %s" % resp.status_code
         logging.info(msg) if resp.status_code == 200 else logging.warning(msg)
-        return jsonpath(resp.json(), resp_jpath)[0] if resp_jpath else resp
+        if resp_jpath:
+            if index is None:
+                return jsonpath(resp.json(), resp_jpath)
+            elif str(index).lower() == 'random':
+                return random.choice(jsonpath(resp.json(), resp_jpath))
+            elif isinstance(index, int):
+                return jsonpath(resp.json(), resp_jpath)[index]
+            else:
+                raise ValueError("index 参数只能为 None、 random 或 整数数字")
+        else:
+            return resp
```

## apitest_ezgo/__about__.py

```diff
@@ -1,8 +1,8 @@
 __title__ = 'apitest_ezgo'
 __description__ = 'easy http interface test frame'
 __url__ = ''
-__version__ = '2.0.1'
+__version__ = '2.0.3'
 __author__ = 'Gawen'
 __author_email__ = '502286126@qq.com'
 __license__ = 'Apache-2.0'
 __copyright__ = 'Copyright 2022 Gawen'
```

## apitest_ezgo/__init__.py

```diff
@@ -1,3 +1,5 @@
 # coding=utf-8
 
-from .Compare import compare_json
+from apitest_ezgo.Compare import compare_json
+from apitest_ezgo.DbHelper import SqLHelper
+from apitest_ezgo.FastRequest import FastRequest
```

## Comparing `apitest_ezgo-2.0.1.dist-info/RECORD` & `apitest_ezgo-2.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 apitest_ezgo/Compare.py,sha256=cXD4UFvHFTKnj_eMo9qD-AgsShPMorVQsw4mwhSDtuU,5287
-apitest_ezgo/DbHelper.py,sha256=vSyy4clGU2hG1JtNiyE85M9iUY9F7jS81rBxppJ29nA,10011
-apitest_ezgo/FastRequest.py,sha256=dJURPhlq_7npDkEY2VrRy9s04aQ51qV5hIGZL-6-qYA,4035
-apitest_ezgo/__about__.py,sha256=F3aPnxqfgI_fw1DG8tK8Tn5htsBskh8tt4kZXJMYstM,237
-apitest_ezgo/__init__.py,sha256=uM6HTTSwSziyZus-ubqZ-VKNG3KKd4kBHOlj7lR2OhQ,53
+apitest_ezgo/DbHelper.py,sha256=5YMx7sdweoSg6ylJT1aHlkY34bye6MIgGNL8E_AsCbo,10168
+apitest_ezgo/FastRequest.py,sha256=D1dlCC_tpwE8DqKjDMyuG9vWgHxDDE65o9FGOGb2dUs,4629
+apitest_ezgo/__about__.py,sha256=SkOh7pYbAQXc7JAgXJAk_NttFtSpDUyDqU81DdJvyW8,237
+apitest_ezgo/__init__.py,sha256=6FS67m6oJLc2WokQ1Y-uWVOoIOlNMEB3_uPEmrFzevk,160
 apitest_ezgo/compat.py,sha256=U6y6S0jiigCV76iOZZoU26EYuxaIhnvT1nZr3v-nSCA,901
 apitest_ezgo/Har2Template/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 apitest_ezgo/Har2Template/cli.py,sha256=zXDmePVyKb7mRE__8bZQRI74Fjw8VKMVWYHHgBU2uGo,1844
 apitest_ezgo/Har2Template/core.py,sha256=ib7X-miBSHbxFAhDq24bgXlJA4jK2y3YdS0nukk4OSg,6466
 apitest_ezgo/Har2Template/utils.py,sha256=6bdbmru4nCCXK4J9xYMh-00IcZFZj6zw1wFQjbMH5VM,3506
-apitest_ezgo-2.0.1.dist-info/METADATA,sha256=wL4P2DgIDuVxc_MESjX6b9UY0K0tBy1dv9Tw3PbRDiY,501
-apitest_ezgo-2.0.1.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-apitest_ezgo-2.0.1.dist-info/entry_points.txt,sha256=aiep-Pjj130COhWjsCumlAgLfs_UrCKNLiW0rCprSHM,69
-apitest_ezgo-2.0.1.dist-info/top_level.txt,sha256=XZrZdozvAJVSlCHruFoGsK7hTau52-om-M9nnxTqOXE,13
-apitest_ezgo-2.0.1.dist-info/RECORD,,
+apitest_ezgo-2.0.3.dist-info/METADATA,sha256=hvEfPe6v959rP_oiqbRGXc3OYSuOryxZFtL13KQtV98,501
+apitest_ezgo-2.0.3.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+apitest_ezgo-2.0.3.dist-info/entry_points.txt,sha256=aiep-Pjj130COhWjsCumlAgLfs_UrCKNLiW0rCprSHM,69
+apitest_ezgo-2.0.3.dist-info/top_level.txt,sha256=XZrZdozvAJVSlCHruFoGsK7hTau52-om-M9nnxTqOXE,13
+apitest_ezgo-2.0.3.dist-info/RECORD,,
```

