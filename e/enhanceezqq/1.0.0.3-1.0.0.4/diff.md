# Comparing `tmp/enhanceezqq-1.0.0.3.tar.gz` & `tmp/enhanceezqq-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhanceezqq-1.0.0.3.tar", last modified: Tue May  9 14:25:53 2023, max compression
+gzip compressed data, was "enhanceezqq-1.0.0.4.tar", last modified: Wed May 10 08:52:38 2023, max compression
```

## Comparing `enhanceezqq-1.0.0.3.tar` & `enhanceezqq-1.0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 14:25:52.999842 enhanceezqq-1.0.0.3/
--rw-rw-rw-   0        0        0      307 2023-05-09 14:25:52.998841 enhanceezqq-1.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2696 2023-04-16 04:39:07.000000 enhanceezqq-1.0.0.3/akpack.py
--rw-rw-rw-   0        0        0     5179 2023-04-15 07:50:36.000000 enhanceezqq-1.0.0.3/basefund.py
-drwxrwxrwx   0        0        0        0 2023-05-09 14:25:52.980839 enhanceezqq-1.0.0.3/config/
-drwxrwxrwx   0        0        0        0 2023-05-09 14:25:52.989839 enhanceezqq-1.0.0.3/config/enhanceezqq/
--rw-rw-rw-   0        0        0      394 2023-04-15 01:21:04.000000 enhanceezqq-1.0.0.3/config/enhanceezqq/enhanceezqq_config.json
-drwxrwxrwx   0        0        0        0 2023-05-09 14:25:52.997841 enhanceezqq-1.0.0.3/enhanceezqq.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-09 14:25:52.000000 enhanceezqq-1.0.0.3/enhanceezqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-09 14:25:52.000000 enhanceezqq-1.0.0.3/enhanceezqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 14:25:52.000000 enhanceezqq-1.0.0.3/enhanceezqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-09 14:25:52.000000 enhanceezqq-1.0.0.3/enhanceezqq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      299 2023-05-09 14:25:52.000000 enhanceezqq-1.0.0.3/enhanceezqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-05-09 14:25:52.000000 enhanceezqq-1.0.0.3/enhanceezqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17684 2023-05-09 12:51:24.000000 enhanceezqq-1.0.0.3/enhanceezqq.py
--rw-rw-rw-   0        0        0       42 2023-05-09 14:25:52.999842 enhanceezqq-1.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     6270 2023-05-09 14:25:36.000000 enhanceezqq-1.0.0.3/setup.py
--rw-rw-rw-   0        0        0     5674 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.3/ths.py
--rw-rw-rw-   0        0        0     5690 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.3/ttjj.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:52:38.132028 enhanceezqq-1.0.0.4/
+-rw-rw-rw-   0        0        0      307 2023-05-10 08:52:38.131028 enhanceezqq-1.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2696 2023-04-16 04:39:07.000000 enhanceezqq-1.0.0.4/akpack.py
+-rw-rw-rw-   0        0        0     5179 2023-04-15 07:50:36.000000 enhanceezqq-1.0.0.4/basefund.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:52:38.109023 enhanceezqq-1.0.0.4/config/
+drwxrwxrwx   0        0        0        0 2023-05-10 08:52:38.120025 enhanceezqq-1.0.0.4/config/enhanceezqq/
+-rw-rw-rw-   0        0        0      394 2023-04-15 01:21:04.000000 enhanceezqq-1.0.0.4/config/enhanceezqq/enhanceezqq_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 08:52:38.129027 enhanceezqq-1.0.0.4/enhanceezqq.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-10 08:52:38.000000 enhanceezqq-1.0.0.4/enhanceezqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-10 08:52:38.000000 enhanceezqq-1.0.0.4/enhanceezqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:52:38.000000 enhanceezqq-1.0.0.4/enhanceezqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-10 08:52:38.000000 enhanceezqq-1.0.0.4/enhanceezqq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      299 2023-05-10 08:52:38.000000 enhanceezqq-1.0.0.4/enhanceezqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-05-10 08:52:38.000000 enhanceezqq-1.0.0.4/enhanceezqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19168 2023-05-10 08:48:19.000000 enhanceezqq-1.0.0.4/enhanceezqq.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:52:38.132028 enhanceezqq-1.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     6270 2023-05-10 08:51:02.000000 enhanceezqq-1.0.0.4/setup.py
+-rw-rw-rw-   0        0        0     5674 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.4/ths.py
+-rw-rw-rw-   0        0        0     5690 2023-04-15 05:59:20.000000 enhanceezqq-1.0.0.4/ttjj.py
```

### Comparing `enhanceezqq-1.0.0.3/akpack.py` & `enhanceezqq-1.0.0.4/akpack.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.3/basefund.py` & `enhanceezqq-1.0.0.4/basefund.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.3/enhanceezqq.py` & `enhanceezqq-1.0.0.4/enhanceezqq.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import warnings
 import json
 import pandas as pd
 import easyquotation as ezqtt
 import ast
 import re
 import requests
+from pathlib import Path
 from df_excel_define import is_mem_virtual_file_name, save_object_to_virtual_file
 
 # 本程序调试时使用
 
 # 外部调用是使用
 import os
 import ttjj
@@ -132,14 +133,40 @@
     # 是否从网络股票代码信息
     getcodesflag = 'n'
     getcodechoice = ['real', 'local']
     # 输出结果配置文件
     resultconfigfile = 'nan'
     # 默认输出文件名
     resultfile = 'd:/temp/equotation_result.xlsx'
+    fileprocconfig = STOCK_RESEARCH_CONFIG
+
+    # 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
+    # 判断本地目录是否存在fileprocconfig
+    if Path(fileprocconfig).is_file() is False:
+        try:
+            # 组合系统配置目录对应文件
+            sysfileprocconfig = os.path.join(sys.prefix, fileprocconfig)
+            if Path(sysfileprocconfig).is_file() is False:
+                print("本地配置文件：{}及系统原始配置文件{} 均不存在！".format(fileprocconfig, sysfileprocconfig))
+                sys.exit(-1)
+            else:
+                # 判断本地配置目录是否存在，如果不存在则创建目录，逐层创建
+                localconfigdirlayer = fileprocconfig.split("/")[:-1]
+                currentdir = ""
+                for currentlayer in localconfigdirlayer:
+                    currentdir = os.path.join(currentdir, currentlayer)
+                    if Path(currentdir).is_dir() is False:
+                        os.mkdir(currentdir)
+                # 拷贝系统配置文件到本地
+                shutil.copy(sysfileprocconfig, fileprocconfig)
+        except Exception as err:
+            print("拷贝系统原始配置到本地配置文件：{} 失败：{}".format(fileprocconfig, err))
+            sys.exit(-1)
+
+
 
     try:
         with open(STOCK_RESEARCH_CONFIG, "r", encoding="utf-8") as fp:
             configdic = json.load(fp)
             databaseinfo = configdic["database"]
             fp.close()
     except Exception as err:
```

### Comparing `enhanceezqq-1.0.0.3/setup.py` & `enhanceezqq-1.0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 00000940: 7269 6769 6e63 6f6e 6669 6764 6972 2c20  riginconfigdir, 
 00000950: 5b6f 7267 696e 636f 6e66 6967 6669 6c65  [orginconfigfile
 00000960: 5d29 2c0d 0a20 2020 2020 2020 205d 0d0a  ]),..        ]..
 00000970: 2020 2020 7265 7475 726e 2064 6174 615f      return data_
 00000980: 6669 6c65 730d 0a0d 0a0d 0a73 6574 7570  files......setup
 00000990: 280d 0a20 2020 206e 616d 653d 2765 6e68  (..    name='enh
 000009a0: 616e 6365 657a 7171 272c 0d0a 2020 2020  anceezqq',..    
-000009b0: 7665 7273 696f 6e3d 2731 2e30 2e30 2e33  version='1.0.0.3
+000009b0: 7665 7273 696f 6e3d 2731 2e30 2e30 2e34  version='1.0.0.4
 000009c0: 272c 0d0a 2020 2020 6465 7363 7269 7074  ',..    descript
 000009d0: 696f 6e3d 27e7 94a8 e4ba 8ee5 afb9 657a  ion='.........ez
 000009e0: 7171 e6a8 a1e5 9d97 e5a2 9ee5 bcba e58a  qq..............
 000009f0: 9fe8 83bd efbc 8ce8 83bd e5a4 9fe8 8eb7  ................
 00000a00: e58f 96e5 8e86 e58f b2e6 95b0 e68d aee4  ................
 00000a10: bf9d e5ad 98e5 88b0 e695 b0e6 8dae e5ba  ................
 00000a20: 93ef bc8c e5b9 b6e4 bb8e e695 b0e6 8dae  ................
```

### Comparing `enhanceezqq-1.0.0.3/ths.py` & `enhanceezqq-1.0.0.4/ths.py`

 * *Files identical despite different names*

### Comparing `enhanceezqq-1.0.0.3/ttjj.py` & `enhanceezqq-1.0.0.4/ttjj.py`

 * *Files identical despite different names*

