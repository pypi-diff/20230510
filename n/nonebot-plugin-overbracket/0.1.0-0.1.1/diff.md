# Comparing `tmp/nonebot-plugin-overbracket-0.1.0.tar.gz` & `tmp/nonebot-plugin-overbracket-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-overbracket-0.1.0.tar", last modified: Sun Mar 26 12:14:23 2023, max compression
+gzip compressed data, was "nonebot-plugin-overbracket-0.1.1.tar", last modified: Wed May 10 16:32:59 2023, max compression
```

## Comparing `nonebot-plugin-overbracket-0.1.0.tar` & `nonebot-plugin-overbracket-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:14:23.271551 nonebot-plugin-overbracket-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-26 12:14:07.000000 nonebot-plugin-overbracket-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-26 12:14:23.271551 nonebot-plugin-overbracket-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-26 12:14:07.000000 nonebot-plugin-overbracket-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:14:23.267551 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-26 12:14:07.000000 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-26 12:14:07.000000 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 12:14:23.271551 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-26 12:14:23.000000 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-26 12:14:23.000000 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 12:14:23.000000 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-26 12:14:23.000000 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-26 12:14:23.000000 nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-26 12:14:07.000000 nonebot-plugin-overbracket-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 12:14:23.271551 nonebot-plugin-overbracket-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:32:59.375301 nonebot-plugin-overbracket-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 16:32:45.000000 nonebot-plugin-overbracket-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-10 16:32:59.375301 nonebot-plugin-overbracket-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-10 16:32:45.000000 nonebot-plugin-overbracket-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:32:59.375301 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-10 16:32:45.000000 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-10 16:32:45.000000 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:32:59.375301 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-10 16:32:59.000000 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-10 16:32:59.000000 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:32:59.000000 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 16:32:59.000000 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 16:32:59.000000 nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-10 16:32:45.000000 nonebot-plugin-overbracket-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:32:59.375301 nonebot-plugin-overbracket-0.1.1/setup.cfg
```

### Comparing `nonebot-plugin-overbracket-0.1.0/LICENSE` & `nonebot-plugin-overbracket-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-overbracket-0.1.0/PKG-INFO` & `nonebot-plugin-overbracket-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-overbracket
-Version: 0.1.0
+Version: 0.1.1
 Summary: NoneBot2 插件 通括膨胀——泛滥的括号
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-overbracket
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-overbracket
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-overbracket Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-overbracket Version: 0.1.1 Summary:
 NoneBot2 æä»¶ éæ¬è¨èââæ³æ»¥çæ¬å· Author-email: HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-overbracket Project-URL: Repository, https://github.com/NCBM/nonebot-
 plugin-overbracket Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE
    # nonebot-plugin-overbracket _â¨ éæ¬è¨èââæ³æ»¥çæ¬å· â¨_
                            [license] [pypi] [python]
```

### Comparing `nonebot-plugin-overbracket-0.1.0/README.md` & `nonebot-plugin-overbracket-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket/__init__.py` & `nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 import random
 from nonebot import on_message, get_driver
 from nonebot.adapters import Event
+from nonebot.plugin import PluginMetadata
 from .config import Config
 
+__plugin_meta__ = PluginMetadata(
+    name="通括膨胀",
+    description="让你的机器人随机发括号",
+    usage="[请查阅插件介绍文档]",
+    config=Config
+)
+
 global_config = get_driver().config
 parsed_config = Config.parse_obj(global_config)
 
 obr = on_message(priority=25, block=False)
 
 
 @obr.handle()
 async def make_lbracket(event: Event):
     msg = event.get_message().extract_plain_text()
+    
+    if len(msg) < 1:
+        return None
+    
     last = msg[-1]
     if parsed_config.overbracket_nohalfsize and last in "([{":
         text = "半角异端！"
         chance = parsed_config.overbracket_purpose_chance
     elif last in parsed_config.overbracket_brackets:
         text = last
         chance = parsed_config.overbracket_purpose_chance
```

### Comparing `nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket/config.py` & `nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-overbracket-0.1.0/nonebot_plugin_overbracket.egg-info/PKG-INFO` & `nonebot-plugin-overbracket-0.1.1/nonebot_plugin_overbracket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-overbracket
-Version: 0.1.0
+Version: 0.1.1
 Summary: NoneBot2 插件 通括膨胀——泛滥的括号
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/NCBM/nonebot-plugin-overbracket
 Project-URL: Repository, https://github.com/NCBM/nonebot-plugin-overbracket
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-overbracket Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-overbracket Version: 0.1.1 Summary:
 NoneBot2 æä»¶ éæ¬è¨èââæ³æ»¥çæ¬å· Author-email: HivertMoZara
 163.com> License: MIT Project-URL: Homepage, https://github.com/NCBM/nonebot-
 plugin-overbracket Project-URL: Repository, https://github.com/NCBM/nonebot-
 plugin-overbracket Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE
    # nonebot-plugin-overbracket _â¨ éæ¬è¨èââæ³æ»¥çæ¬å· â¨_
                            [license] [pypi] [python]
```

