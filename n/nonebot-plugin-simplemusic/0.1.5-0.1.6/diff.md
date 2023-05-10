# Comparing `tmp/nonebot_plugin_simplemusic-0.1.5.tar.gz` & `tmp/nonebot_plugin_simplemusic-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_simplemusic-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_simplemusic-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_simplemusic-0.1.5.tar` & `nonebot_plugin_simplemusic-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1063 2022-06-20 14:22:23.630000 nonebot_plugin_simplemusic-0.1.5/LICENSE
--rw-r--r--   0        0        0      588 2022-06-20 14:22:23.630000 nonebot_plugin_simplemusic-0.1.5/README.md
--rw-r--r--   0        0        0     2526 2022-12-01 04:17:58.003239 nonebot_plugin_simplemusic-0.1.5/nonebot_plugin_simplemusic/__init__.py
--rw-r--r--   0        0        0     7412 2022-12-01 04:16:58.823237 nonebot_plugin_simplemusic-0.1.5/nonebot_plugin_simplemusic/data_source.py
--rw-r--r--   0        0        0      629 2022-12-01 04:17:48.903239 nonebot_plugin_simplemusic-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1391 2022-12-01 04:19:01.805536 nonebot_plugin_simplemusic-0.1.5/setup.py
--rw-r--r--   0        0        0     1373 2022-12-01 04:19:01.805711 nonebot_plugin_simplemusic-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-09 02:58:24.119753 nonebot_plugin_simplemusic-0.1.6/LICENSE
+-rw-r--r--   0        0        0      588 2023-05-09 02:58:24.119753 nonebot_plugin_simplemusic-0.1.6/README.md
+-rw-r--r--   0        0        0     2526 2023-05-09 02:58:24.119753 nonebot_plugin_simplemusic-0.1.6/nonebot_plugin_simplemusic/__init__.py
+-rw-r--r--   0        0        0     7950 2023-05-09 02:58:24.119753 nonebot_plugin_simplemusic-0.1.6/nonebot_plugin_simplemusic/data_source.py
+-rw-r--r--   0        0        0      629 2023-05-09 02:58:24.123753 nonebot_plugin_simplemusic-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 nonebot_plugin_simplemusic-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_simplemusic-0.1.5/LICENSE` & `nonebot_plugin_simplemusic-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simplemusic-0.1.5/README.md` & `nonebot_plugin_simplemusic-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simplemusic-0.1.5/nonebot_plugin_simplemusic/__init__.py` & `nonebot_plugin_simplemusic-0.1.6/nonebot_plugin_simplemusic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import asyncio
 import traceback
 
 from nonebot import on_command
+from nonebot.adapters.onebot.v11 import Message
 from nonebot.log import logger
 from nonebot.matcher import Matcher
-from nonebot.typing import T_Handler
 from nonebot.params import CommandArg
 from nonebot.plugin import PluginMetadata
-from nonebot.adapters.onebot.v11 import Message
+from nonebot.typing import T_Handler
 
 from .data_source import Func, Source, sources
 
 __plugin_meta__ = PluginMetadata(
     name="点歌",
     description="点歌，支持qq、网易云等来源",
     usage="点歌/qq点歌/网易点歌/酷我点歌/酷狗点歌/咪咕点歌/b站点歌 + 关键词",
     extra={
         "unique_name": "simplemusic",
         "example": "点歌 万古生香",
         "author": "meetwq <meetwq@gmail.com>",
-        "version": "0.1.5",
+        "version": "0.1.6",
     },
 )
 
 
 def retry(func: Func, count=3, sleep=3):
     async def wrapper(*args, **kwargs):
         for i in range(count):
```

### Comparing `nonebot_plugin_simplemusic-0.1.5/nonebot_plugin_simplemusic/data_source.py` & `nonebot_plugin_simplemusic-0.1.6/nonebot_plugin_simplemusic/data_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import httpx
 from dataclasses import dataclass
 from difflib import SequenceMatcher
-from typing import Any, Dict, List, Protocol, Optional, Tuple
+from typing import Any, Dict, List, Optional, Protocol, Tuple
 
+import httpx
 from nonebot.adapters.onebot.v11 import MessageSegment
 
 
 async def search_qq(keyword: str) -> Optional[MessageSegment]:
     url = "https://c.y.qq.com/splcloud/fcgi-bin/smartbox_new.fcg"
     params = {
         "format": "json",
@@ -76,24 +76,24 @@
             resp = httpx.get(song_url, params=params)
             result = resp.json()
 
             if info := result["data"]["songinfo"]:
                 play_url = "https://kuwo.cn/api/v1/www/music/playUrl"
                 params = {"mid": rid, "type": "music", "httpsStatus": 1}
                 resp = httpx.get(play_url, params=params)
-                result = resp.json()
+                result: Dict = resp.json()
 
-                if data := result["data"]:
+                if result.get("data", None) and (data := result["data"]):
                     return MessageSegment(
                         "music",
                         {
                             "type": "custom",
                             "subtype": "kuwo",
                             "url": f"https://kuwo.cn/play_detail/{rid}",
-                            "audio": data["url"],
+                            "voice": data["url"],
                             "title": info["songName"],
                             "content": info["artist"],
                             "image": info["pic"],
                         },
                     )
 
 
@@ -126,15 +126,15 @@
             if info := resp.json():
                 return MessageSegment(
                     "music",
                     {
                         "type": "custom",
                         "subtype": "kugou",
                         "url": f"https://www.kugou.com/song/#hash={hash}&album_id={album_id}",
-                        "audio": info["url"],
+                        "voice": info["url"],
                         "title": info["songName"],
                         "content": info["author_name"],
                         "image": str(info["imgUrl"]).format(size=240),
                     },
                 )
 
 
@@ -154,15 +154,15 @@
         info = songs[0]
         return MessageSegment(
             "music",
             {
                 "type": "custom",
                 "subtype": "migu",
                 "url": f"https://music.migu.cn/v3/music/song/{info['copyrightId']}",
-                "audio": info["mp3"],
+                "voice": info["mp3"],
                 "title": info["title"],
                 "content": info["singerName"],
                 "image": info["cover"],
             },
         )
 
 
@@ -175,20 +175,34 @@
     songs: List[Dict[str, Any]] = result["data"]["result"]
     if songs:
         songs.sort(
             key=lambda x: SequenceMatcher(None, keyword, x["title"]).ratio(),
             reverse=True,
         )
         info = songs[0]
-        return MessageSegment.share(
-            url=f"https://www.bilibili.com/audio/au{info['id']}",
-            title=info["title"],
-            content=info["author"],
-            image=info["cover"],
-        )
+        return MessageSegment.text(f"https://www.bilibili.com/audio/au{info['id']}")
+
+        # return MessageSegment.share(
+        #     url=f"https://www.bilibili.com/audio/au{info['id']}",
+        #     title=info["title"],
+        #     content=info["author"],
+        #     image=info["cover"],
+        # )
+
+        """https://github.com/Mrs4s/go-cqhttp/issues/1495"""
+        # return MessageSegment(
+        #     "music",
+        #     {
+        #         "type": "custom",
+        #         "url": f"https://www.bilibili.com/audio/au{info['id']}",
+        #         "title": info["title"],
+        #         "content": info["author"],
+        #         "image": info["cover"],
+        #     },
+        # )
 
 
 class Func(Protocol):
     async def __call__(self, keyword: str) -> Optional[MessageSegment]:
         ...
```

### Comparing `nonebot_plugin_simplemusic-0.1.5/pyproject.toml` & `nonebot_plugin_simplemusic-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_simplemusic"
-version = "0.1.5"
+version = "0.1.6"
 description = "适用于 Nonebot2 的点歌插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-simplemusic"
 repository = "https://github.com/noneplugin/nonebot-plugin-simplemusic"
```

### Comparing `nonebot_plugin_simplemusic-0.1.5/PKG-INFO` & `nonebot_plugin_simplemusic-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-simplemusic
-Version: 0.1.5
+Version: 0.1.6
 Summary: 适用于 Nonebot2 的点歌插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-simplemusic
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.19.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-simplemusic
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-simplemusic
```

