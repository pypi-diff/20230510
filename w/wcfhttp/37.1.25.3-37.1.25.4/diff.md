# Comparing `tmp/wcfhttp-37.1.25.3.tar.gz` & `tmp/wcfhttp-37.1.25.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-37.1.25.3.tar", last modified: Wed May 10 03:51:20 2023, max compression
+gzip compressed data, was "wcfhttp-37.1.25.4.tar", last modified: Wed May 10 05:22:21 2023, max compression
```

## Comparing `wcfhttp-37.1.25.3.tar` & `wcfhttp-37.1.25.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 03:51:20.016257 wcfhttp-37.1.25.3/
--rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1829 2023-05-10 03:51:20.016257 wcfhttp-37.1.25.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-10 03:51:20.016257 wcfhttp-37.1.25.3/setup.cfg
--rw-rw-rw-   0        0        0     1439 2023-05-08 08:39:05.000000 wcfhttp-37.1.25.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:51:20.000609 wcfhttp-37.1.25.3/wcfhttp/
--rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.3/wcfhttp/__init__.py
--rw-rw-rw-   0        0        0    14500 2023-05-10 03:51:16.000000 wcfhttp-37.1.25.3/wcfhttp/core.py
--rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.3/wcfhttp/main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:51:20.016257 wcfhttp-37.1.25.3/wcfhttp.egg-info/
--rw-rw-rw-   0        0        0     1829 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 03:51:19.000000 wcfhttp-37.1.25.3/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 05:22:21.117383 wcfhttp-37.1.25.4/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1829 2023-05-10 05:22:21.117383 wcfhttp-37.1.25.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-10 05:22:21.117383 wcfhttp-37.1.25.4/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2023-05-10 05:22:18.000000 wcfhttp-37.1.25.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:22:21.101758 wcfhttp-37.1.25.4/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.4/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    14500 2023-05-10 05:22:18.000000 wcfhttp-37.1.25.4/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.4/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:22:21.117383 wcfhttp-37.1.25.4/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1829 2023-05-10 05:22:20.000000 wcfhttp-37.1.25.4/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-10 05:22:21.000000 wcfhttp-37.1.25.4/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 05:22:20.000000 wcfhttp-37.1.25.4/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-10 05:22:20.000000 wcfhttp-37.1.25.4/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-10 05:22:20.000000 wcfhttp-37.1.25.4/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 05:22:20.000000 wcfhttp-37.1.25.4/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-37.1.25.3/PKG-INFO` & `wcfhttp-37.1.25.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 37.1.25.3
+Version: 37.1.25.4
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

### Comparing `wcfhttp-37.1.25.3/setup.py` & `wcfhttp-37.1.25.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     entry_points={
         'console_scripts': [
             'wcfhttp=wcfhttp.main:main'
         ]
     },
     install_requires=[
         "setuptools",
-        f"wcferry<={wcfhttp.core.__version__}",
         "fastapi",
-        "uvicorn[standard]"
+        "uvicorn[standard]",
+        "wcferry==37.1.25.2",
     ],
     classifiers=[
         "Environment :: Win32 (MS Windows)",
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Topic :: Communications :: Chat",
         "Operating System :: Microsoft :: Windows",
```

### Comparing `wcfhttp-37.1.25.3/wcfhttp/core.py` & `wcfhttp-37.1.25.4/wcfhttp/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 import requests
 from fastapi import Body, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "37.1.25.3"
+__version__ = "37.1.25.4"
 
 
 class Msg(BaseModel):
     id: str
     type: int
     xml: str
     sender: str
```

### Comparing `wcfhttp-37.1.25.3/wcfhttp/main.py` & `wcfhttp-37.1.25.4/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-37.1.25.3/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-37.1.25.4/wcfhttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 37.1.25.3
+Version: 37.1.25.4
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

