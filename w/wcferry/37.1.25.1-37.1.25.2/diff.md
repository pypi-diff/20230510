# Comparing `tmp/wcferry-37.1.25.1.tar.gz` & `tmp/wcferry-37.1.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcferry-37.1.25.1.tar", last modified: Wed May 10 03:15:41 2023, max compression
+gzip compressed data, was "wcferry-37.1.25.2.tar", last modified: Wed May 10 03:44:15 2023, max compression
```

## Comparing `wcferry-37.1.25.1.tar` & `wcferry-37.1.25.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 03:15:41.507879 wcferry-37.1.25.1/
--rw-rw-rw-   0        0        0       46 2023-03-10 16:21:28.000000 wcferry-37.1.25.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6361 2023-05-10 03:15:41.507879 wcferry-37.1.25.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-10 03:15:41.507879 wcferry-37.1.25.1/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-05-10 03:10:59.000000 wcferry-37.1.25.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:15:41.492253 wcferry-37.1.25.1/wcferry/
--rw-rw-rw-   0        0        0      105 2023-05-04 13:34:55.000000 wcferry-37.1.25.1/wcferry/__init__.py
--rw-rw-rw-   0        0        0    19045 2023-05-10 03:10:59.000000 wcferry-37.1.25.1/wcferry/client.py
--rw-rw-rw-   0        0        0   629760 2023-05-08 04:08:05.000000 wcferry-37.1.25.1/wcferry/spy.dll
--rw-rw-rw-   0        0        0  1150976 2023-05-08 04:06:58.000000 wcferry-37.1.25.1/wcferry/spy_debug.dll
--rwxrwxrwx   0        0        0   370688 2023-05-05 06:24:34.000000 wcferry-37.1.25.1/wcferry/wcf.exe
--rw-rw-rw-   0        0        0     7175 2023-04-19 11:01:25.000000 wcferry-37.1.25.1/wcferry/wcf_pb2.py
--rw-rw-rw-   0        0        0     1874 2023-05-10 03:10:59.000000 wcferry-37.1.25.1/wcferry/wxmsg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:15:41.507879 wcferry-37.1.25.1/wcferry.egg-info/
--rw-rw-rw-   0        0        0     6361 2023-05-10 03:15:41.000000 wcferry-37.1.25.1/wcferry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-10 03:15:41.000000 wcferry-37.1.25.1/wcferry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 03:15:41.000000 wcferry-37.1.25.1/wcferry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-10 03:15:41.000000 wcferry-37.1.25.1/wcferry.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 03:15:41.000000 wcferry-37.1.25.1/wcferry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 03:44:15.974803 wcferry-37.1.25.2/
+-rw-rw-rw-   0        0        0       46 2023-03-10 16:21:28.000000 wcferry-37.1.25.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6361 2023-05-10 03:44:15.974803 wcferry-37.1.25.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-10 03:44:15.974803 wcferry-37.1.25.2/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-05-10 03:10:59.000000 wcferry-37.1.25.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:44:15.959179 wcferry-37.1.25.2/wcferry/
+-rw-rw-rw-   0        0        0      105 2023-05-04 13:34:55.000000 wcferry-37.1.25.2/wcferry/__init__.py
+-rw-rw-rw-   0        0        0    19045 2023-05-10 03:43:35.000000 wcferry-37.1.25.2/wcferry/client.py
+-rw-rw-rw-   0        0        0   629760 2023-05-08 04:08:05.000000 wcferry-37.1.25.2/wcferry/spy.dll
+-rw-rw-rw-   0        0        0  1150976 2023-05-08 04:06:58.000000 wcferry-37.1.25.2/wcferry/spy_debug.dll
+-rwxrwxrwx   0        0        0   370688 2023-05-05 06:24:34.000000 wcferry-37.1.25.2/wcferry/wcf.exe
+-rw-rw-rw-   0        0        0     7175 2023-04-19 11:01:25.000000 wcferry-37.1.25.2/wcferry/wcf_pb2.py
+-rw-rw-rw-   0        0        0     2055 2023-05-10 03:43:35.000000 wcferry-37.1.25.2/wcferry/wxmsg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:44:15.974803 wcferry-37.1.25.2/wcferry.egg-info/
+-rw-rw-rw-   0        0        0     6361 2023-05-10 03:44:15.000000 wcferry-37.1.25.2/wcferry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-10 03:44:15.000000 wcferry-37.1.25.2/wcferry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 03:44:15.000000 wcferry-37.1.25.2/wcferry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-10 03:44:15.000000 wcferry-37.1.25.2/wcferry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 03:44:15.000000 wcferry-37.1.25.2/wcferry.egg-info/top_level.txt
```

### Comparing `wcferry-37.1.25.1/PKG-INFO` & `wcferry-37.1.25.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcferry
-Version: 37.1.25.1
+Version: 37.1.25.2
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

### Comparing `wcferry-37.1.25.1/setup.py` & `wcferry-37.1.25.2/setup.py`

 * *Files identical despite different names*

### Comparing `wcferry-37.1.25.1/wcferry/client.py` & `wcferry-37.1.25.2/wcferry/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-__version__ = "37.1.25.1"
+__version__ = "37.1.25.2"
 
 import atexit
 import base64
 import logging
 import os
 import re
 import sys
```

### Comparing `wcferry-37.1.25.1/wcferry/spy.dll` & `wcferry-37.1.25.2/wcferry/spy.dll`

 * *Files identical despite different names*

### Comparing `wcferry-37.1.25.1/wcferry/spy_debug.dll` & `wcferry-37.1.25.2/wcferry/spy_debug.dll`

 * *Files identical despite different names*

### Comparing `wcferry-37.1.25.1/wcferry/wcf.exe` & `wcferry-37.1.25.2/wcferry/wcf.exe`

 * *Files identical despite different names*

### Comparing `wcferry-37.1.25.1/wcferry/wcf_pb2.py` & `wcferry-37.1.25.2/wcferry/wcf_pb2.py`

 * *Files identical despite different names*

### Comparing `wcferry-37.1.25.1/wcferry/wxmsg.py` & `wcferry-37.1.25.2/wcferry/wxmsg.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,13 +45,21 @@
 
     def from_group(self) -> bool:
         """是否群聊消息"""
         return self._is_group
 
     def is_at(self, wxid) -> bool:
         """是否被 @：群消息，在 @ 名单里，并且不是 @ 所有人"""
-        return self.from_group() and re.findall(
-            f"<atuserlist>.*({wxid}).*</atuserlist>", self.xml) and not re.findall(r"@(?:所有人|all|All)", self.content)
+        if not self.from_group():
+            return False  # 只有群消息才能 @
+
+        if not re.findall(f"<atuserlist>.*({wxid}).*</atuserlist>", self.xml):
+            return False  # 不在 @ 清单里
+
+        if re.findall(r"@(?:所有人|all|All)", self.content):
+            return False  # 排除 @ 所有人
+
+        return True
 
     def is_text(self) -> bool:
         """是否文本消息"""
         return self.type == 1
```

### Comparing `wcferry-37.1.25.1/wcferry.egg-info/PKG-INFO` & `wcferry-37.1.25.2/wcferry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcferry
-Version: 37.1.25.1
+Version: 37.1.25.2
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

