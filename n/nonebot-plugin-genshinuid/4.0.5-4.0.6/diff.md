# Comparing `tmp/nonebot_plugin_genshinuid-4.0.5.tar.gz` & `tmp/nonebot_plugin_genshinuid-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshinuid-4.0.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshinuid-4.0.6.tar", max compression
```

## Comparing `nonebot_plugin_genshinuid-4.0.5.tar` & `nonebot_plugin_genshinuid-4.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    15002 2023-04-18 16:20:25.532575 nonebot_plugin_genshinuid-4.0.5/GenshinUID/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-18 16:20:25.533580 nonebot_plugin_genshinuid-4.0.5/GenshinUID/auto_install.py
--rw-r--r--   0        0        0    23544 2023-04-22 04:43:39.377571 nonebot_plugin_genshinuid-4.0.5/GenshinUID/client.py
--rw-r--r--   0        0        0     1004 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.5/GenshinUID/models.py
--rw-r--r--   0        0        0      336 2023-04-18 16:20:25.609922 nonebot_plugin_genshinuid-4.0.5/GenshinUID/path.py
--rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.5/LICENSE
--rw-r--r--   0        0        0     1652 2023-04-22 04:44:38.967953 nonebot_plugin_genshinuid-4.0.5/pyproject.toml
--rw-r--r--   0        0        0     3318 2023-04-18 16:20:25.696204 nonebot_plugin_genshinuid-4.0.5/README.md
--rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.5/PKG-INFO
+-rw-r--r--   0        0        0    15060 2023-05-10 19:02:42.499695 nonebot_plugin_genshinuid-4.0.6/GenshinUID/__init__.py
+-rw-r--r--   0        0        0     1227 2023-05-06 15:31:52.460341 nonebot_plugin_genshinuid-4.0.6/GenshinUID/auto_install.py
+-rw-r--r--   0        0        0    23544 2023-05-06 15:31:52.639881 nonebot_plugin_genshinuid-4.0.6/GenshinUID/client.py
+-rw-r--r--   0        0        0     1004 2023-04-14 17:44:32.923572 nonebot_plugin_genshinuid-4.0.6/GenshinUID/models.py
+-rw-r--r--   0        0        0      336 2023-05-06 15:31:52.641883 nonebot_plugin_genshinuid-4.0.6/GenshinUID/path.py
+-rw-r--r--   0        0        0    35823 2023-03-31 16:54:56.436943 nonebot_plugin_genshinuid-4.0.6/LICENSE
+-rw-r--r--   0        0        0     1652 2023-05-10 19:03:36.939635 nonebot_plugin_genshinuid-4.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3318 2023-05-06 15:31:52.719678 nonebot_plugin_genshinuid-4.0.6/README.md
+-rw-r--r--   0        0        0     4482 1970-01-01 00:00:00.000000 nonebot_plugin_genshinuid-4.0.6/PKG-INFO
```

### Comparing `nonebot_plugin_genshinuid-4.0.5/GenshinUID/__init__.py` & `nonebot_plugin_genshinuid-4.0.6/GenshinUID/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import asyncio
 from pathlib import Path
+from copy import deepcopy
 from base64 import b64encode
 from typing import Any, List, Union, Optional
 
 import aiofiles
 from nonebot.log import logger
 from nonebot.adapters import Bot
 from nonebot.matcher import Matcher
@@ -27,15 +28,16 @@
 install_core = on_fullmatch('gs一键安装', permission=SUPERUSER, block=True)
 start_core = on_fullmatch('启动core', permission=SUPERUSER, block=True)
 connect_core = on_fullmatch(
     ('连接core', '链接core'), permission=SUPERUSER, block=True
 )
 
 gsclient: Optional[GsClient] = None
-command_start = driver.config.command_start
+command_start = deepcopy(driver.config.command_start)
+command_start.discard('')
 
 if hasattr(driver.config, 'gsuid_core_repeat'):
     is_repeat = True
 else:
     is_repeat = False
 
 
@@ -420,18 +422,20 @@
 
 
 def convert_message(_msg: Any, message: List[Message], index: int):
     if _msg.type == 'text':
         data: str = (
             _msg.data['text'] if 'text' in _msg.data else _msg.data['content']
         )
+
         if index == 0:
-            if data.startswith(tuple(command_start)):
-                for word in command_start:
-                    data = data.replace(word, '', 1)
+            for word in command_start:
+                if data.startswith(word):
+                    data = data[len(word) :]  # noqa:E203
+                    break
         message.append(Message('text', data))
     elif _msg.type == 'image':
         file_id = _msg.data.get('file_id')
         if file_id in _msg.data.values():
             message.append(Message('image', _msg.data['file_id']))
             logger.debug('[OB12图片]', _msg.data['file_id'])
         else:
@@ -451,15 +455,14 @@
 
 
 # 读取文件为base64
 async def convert_file(
     content: Union[Path, str, bytes], file_name: str
 ) -> Message:
     if isinstance(content, Path):
-        print(content)
         async with aiofiles.open(str(content), 'rb') as fp:
             file = await fp.read()
     elif isinstance(content, bytes):
         file = content
     else:
         async with aiofiles.open(content, 'rb') as fp:
             file = await fp.read()
```

### Comparing `nonebot_plugin_genshinuid-4.0.5/GenshinUID/auto_install.py` & `nonebot_plugin_genshinuid-4.0.6/GenshinUID/auto_install.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.5/GenshinUID/client.py` & `nonebot_plugin_genshinuid-4.0.6/GenshinUID/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.5/GenshinUID/models.py` & `nonebot_plugin_genshinuid-4.0.6/GenshinUID/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.5/LICENSE` & `nonebot_plugin_genshinuid-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.5/pyproject.toml` & `nonebot_plugin_genshinuid-4.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nonebot-plugin-genshinuid"
-version = "4.0.5"
+version = "4.0.6"
 description = "支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件"
 authors = ["KimigaiiWuyi <444835641@qq.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2"
 repository = "https://github.com/KimigaiiWuyi/GenshinUID"
 documentation = "https://docs.gsuid.gbots.work/#/"
```

### Comparing `nonebot_plugin_genshinuid-4.0.5/README.md` & `nonebot_plugin_genshinuid-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshinuid-4.0.5/PKG-INFO` & `nonebot_plugin_genshinuid-4.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshinuid
-Version: 4.0.5
+Version: 4.0.6
 Summary: 支持OneBot(QQ)、OneBotV12、QQ频道、微信、KOOK（开黑啦）、Telegram（电报）、FeiShu（飞书）的全功能NoneBot2原神插件
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later
 Author: KimigaiiWuyi
 Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshinuid Version: 4.0.6 Summary:
 æ¯æOneBot
 (QQ)ãOneBotV12ãQQé¢éãå¾®ä¿¡ãKOOKï¼å¼é»å¦ï¼ãTelegramï¼çµæ¥ï¼ãFeiShuï¼é£ä¹¦ï¼çå¨åè½NoneBot2åç¥æä»¶
 Home-page: https://github.com/KimigaiiWuyi/GenshinUID/tree/v4.0-nonebot2
 License: GPL-3.0-or-later Author: KimigaiiWuyi Author-email: 444835641@qq.com
 Requires-Python: >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: GNU
 General Public License v3 or later (GPLv3+) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

