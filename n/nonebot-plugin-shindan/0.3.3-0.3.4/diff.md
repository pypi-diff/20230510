# Comparing `tmp/nonebot_plugin_shindan-0.3.3.tar.gz` & `tmp/nonebot_plugin_shindan-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_shindan-0.3.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_shindan-0.3.4.tar", max compression
```

## Comparing `nonebot_plugin_shindan-0.3.3.tar` & `nonebot_plugin_shindan-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/LICENSE
--rw-r--r--   0        0        0     1626 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/README.md
--rw-r--r--   0        0        0     8442 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/__init__.py
--rw-r--r--   0        0        0      119 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/config.py
--rw-r--r--   0        0        0     2374 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/manager.py
--rw-r--r--   0        0        0     3393 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py
--rw-r--r--   0        0        0      530 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/model.py
--rw-r--r--   0        0        0     4526 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/shindanmaker.py
--rw-r--r--   0        0        0   180778 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/app.css
--rw-r--r--   0        0        0   247324 2023-05-09 01:51:52.212255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/app.js
--rw-r--r--   0        0        0   477118 2023-05-09 01:51:52.216255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/chart.js
--rw-r--r--   0        0        0      339 2023-05-09 01:51:52.216255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/shindan.html
--rw-r--r--   0        0        0     1965 2023-05-09 01:51:52.216255 nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/shindan_list.html
--rw-r--r--   0        0        0      843 2023-05-09 01:51:52.216255 nonebot_plugin_shindan-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 nonebot_plugin_shindan-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1746 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/README.md
+-rw-r--r--   0        0        0     8442 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/config.py
+-rw-r--r--   0        0        0     2374 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/manager.py
+-rw-r--r--   0        0        0     3393 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py
+-rw-r--r--   0        0        0      530 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/model.py
+-rw-r--r--   0        0        0     4707 2023-05-10 02:37:27.583660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/shindanmaker.py
+-rw-r--r--   0        0        0   180778 2023-05-10 02:37:27.587660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/app.css
+-rw-r--r--   0        0        0   247324 2023-05-10 02:37:27.587660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/app.js
+-rw-r--r--   0        0        0   477118 2023-05-10 02:37:27.591660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/chart.js
+-rw-r--r--   0        0        0      339 2023-05-10 02:37:27.591660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/shindan.html
+-rw-r--r--   0        0        0     1965 2023-05-10 02:37:27.591660 nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/shindan_list.html
+-rw-r--r--   0        0        0      843 2023-05-10 02:37:27.591660 nonebot_plugin_shindan-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 nonebot_plugin_shindan-0.3.4/PKG-INFO
```

### Comparing `nonebot_plugin_shindan-0.3.3/LICENSE` & `nonebot_plugin_shindan-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.3/README.md` & `nonebot_plugin_shindan-0.3.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 - 英灵召唤 (595068)
 - 卖萌 (360578)
 
 发送 “占卜指令 名字” 即可，如：`人设生成 小Q`
 
 发送 “/占卜列表” 可以查看上述列表；
 
-超级用户可以发送 “/添加占卜 id 指令”、“/删除占卜 id” 增删占卜列表，可以发送 “/设置占卜 id image/text”设置输出形式
+**超级用户** 可以发送 “/添加占卜 id 指令”、“/删除占卜 id” 增删占卜列表，可以发送 “/设置占卜 id image/text”设置输出形式
+
+超级用户设置方式：[Nonebot 超级用户配置](https://v2.nonebot.dev/docs/appendices/config#superusers)
 
 对于需要登录推特的占卜，可以在 `.env.xxx` 文件中添加 ShindanMaker cookie：
 
 ```
 shindanmaker_cookie=xxx
 ```
```

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/__init__.py` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     description="使用ShindanMaker网站的趣味占卜",
     usage="发送“占卜列表”查看可用占卜\n发送“{占卜名} {名字}”使用占卜",
     config=Config,
     extra={
         "unique_name": "shindan",
         "example": "人设生成 小Q",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.3.3",
+        "version": "0.3.4",
     },
 )
 
 add_usage = """Usage:
 添加占卜 {id} {指令}
 如：添加占卜 917962 人设生成"""
```

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/manager.py` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/migrations/02bb36c59899_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/model.py` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/shindanmaker.py` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/shindanmaker.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,20 +74,23 @@
 
 async def make_shindan(id: str, name: str, mode="image") -> Union[str, bytes]:
     url = f"https://shindanmaker.com/{id}"
     seed = time.strftime("%y%m%d", time.localtime())
     async with httpx.AsyncClient() as client:
         resp = await get(client, url)
         dom = BeautifulSoup(resp.text, "lxml")
-        token = dom.find("form", {"id": "shindanForm"}).find("input")["value"]  # type: ignore
+        form = dom.find("form", {"id": "shindanForm"})
+        _token = form.find("input", {"name": "_token"})["value"]  # type: ignore
+        shindan_token = form.find("input", {"name": "shindan_token"})["value"]  # type: ignore
         payload = {
-            "_token": token,
+            "_token": _token,
             "shindanName": name + seed,
             "hiddenName": "名無しのR",
             "type": "name",
+            "shindan_token": shindan_token,
         }
         resp = await post(client, url, json=payload)
 
     content = resp.text
     if mode == "image":
         html, has_chart = await render_html(content)
         html = html.replace(seed, "")
```

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/app.css` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/app.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/app.js` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/app.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/chart.js` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/chart.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.3/nonebot_plugin_shindan/templates/shindan_list.html` & `nonebot_plugin_shindan-0.3.4/nonebot_plugin_shindan/templates/shindan_list.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shindan-0.3.3/pyproject.toml` & `nonebot_plugin_shindan-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_shindan"
-version = "0.3.3"
+version = "0.3.4"
 description = "Nonebot2 plugin for using ShindanMaker"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-shindan"
 repository = "https://github.com/noneplugin/nonebot-plugin-shindan"
```

### Comparing `nonebot_plugin_shindan-0.3.3/PKG-INFO` & `nonebot_plugin_shindan-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-shindan
-Version: 0.3.3
+Version: 0.3.4
 Summary: Nonebot2 plugin for using ShindanMaker
 Home-page: https://github.com/noneplugin/nonebot-plugin-shindan
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -62,15 +62,17 @@
 - 英灵召唤 (595068)
 - 卖萌 (360578)
 
 发送 “占卜指令 名字” 即可，如：`人设生成 小Q`
 
 发送 “/占卜列表” 可以查看上述列表；
 
-超级用户可以发送 “/添加占卜 id 指令”、“/删除占卜 id” 增删占卜列表，可以发送 “/设置占卜 id image/text”设置输出形式
+**超级用户** 可以发送 “/添加占卜 id 指令”、“/删除占卜 id” 增删占卜列表，可以发送 “/设置占卜 id image/text”设置输出形式
+
+超级用户设置方式：[Nonebot 超级用户配置](https://v2.nonebot.dev/docs/appendices/config#superusers)
 
 对于需要登录推特的占卜，可以在 `.env.xxx` 文件中添加 ShindanMaker cookie：
 
 ```
 shindanmaker_cookie=xxx
 ```
```

