# Comparing `tmp/wcfhttp-37.1.25.2.tar.gz` & `tmp/wcfhttp-37.1.25.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-37.1.25.2.tar", last modified: Mon May  8 09:01:04 2023, max compression
+gzip compressed data, was "wcfhttp-37.1.25.3.tar", last modified: Wed May 10 03:51:20 2023, max compression
```

## Comparing `wcfhttp-37.1.25.2.tar` & `wcfhttp-37.1.25.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 09:01:04.493223 wcfhttp-37.1.25.2/
--rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1829 2023-05-08 09:01:04.493223 wcfhttp-37.1.25.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-08 09:01:04.493223 wcfhttp-37.1.25.2/setup.cfg
--rw-rw-rw-   0        0        0     1439 2023-05-08 08:39:05.000000 wcfhttp-37.1.25.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:01:04.477599 wcfhttp-37.1.25.2/wcfhttp/
--rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.2/wcfhttp/__init__.py
--rw-rw-rw-   0        0        0    14482 2023-05-08 08:59:43.000000 wcfhttp-37.1.25.2/wcfhttp/core.py
--rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.2/wcfhttp/main.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:01:04.493223 wcfhttp-37.1.25.2/wcfhttp.egg-info/
--rw-rw-rw-   0        0        0     1829 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 03:51:20.016257 wcfhttp-37.1.25.3/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1829 2023-05-10 03:51:20.016257 wcfhttp-37.1.25.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-10 03:51:20.016257 wcfhttp-37.1.25.3/setup.cfg
+-rw-rw-rw-   0        0        0     1439 2023-05-08 08:39:05.000000 wcfhttp-37.1.25.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:51:20.000609 wcfhttp-37.1.25.3/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.3/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    14500 2023-05-10 03:51:16.000000 wcfhttp-37.1.25.3/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.3/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:51:20.016257 wcfhttp-37.1.25.3/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1829 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-37.1.25.2/PKG-INFO` & `wcfhttp-37.1.25.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 37.1.25.2
+Version: 37.1.25.3
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

### Comparing `wcfhttp-37.1.25.2/setup.py` & `wcfhttp-37.1.25.3/setup.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-37.1.25.2/wcfhttp/core.py` & `wcfhttp-37.1.25.3/wcfhttp/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 import requests
 from fastapi import Body, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "37.1.25.2"
+__version__ = "37.1.25.3"
 
 
 class Msg(BaseModel):
     id: str
     type: int
     xml: str
     sender: str
@@ -65,15 +65,15 @@
             data["type"] = msg.type
             data["xml"] = msg.xml
             data["sender"] = msg.sender
             data["roomid"] = msg.roomid
             data["content"] = msg.content
             data["thumb"] = msg.thumb
             data["extra"] = msg.extra
-            data["is_at"] = msg.is_at()
+            data["is_at"] = msg.is_at(self.wcf.self_wxid)
             data["is_self"] = msg.from_self()
             data["is_group"] = msg.from_group()
 
             try:
                 rsp = requests.post(url=cb, json=data)
                 if rsp.status_code != 200:
                     self.LOG.error(f"消息转发失败，HTTP 状态码为: {rsp.status_code}")
```

### Comparing `wcfhttp-37.1.25.2/wcfhttp/main.py` & `wcfhttp-37.1.25.3/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-37.1.25.2/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-37.1.25.3/wcfhttp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 37.1.25.2
+Version: 37.1.25.3
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

