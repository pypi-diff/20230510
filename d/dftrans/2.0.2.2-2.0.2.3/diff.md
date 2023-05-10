# Comparing `tmp/dftrans-2.0.2.2.tar.gz` & `tmp/dftrans-2.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dftrans-2.0.2.2.tar", last modified: Wed May 10 08:51:49 2023, max compression
+gzip compressed data, was "dftrans-2.0.2.3.tar", last modified: Wed May 10 09:43:16 2023, max compression
```

## Comparing `dftrans-2.0.2.2.tar` & `dftrans-2.0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.164724 dftrans-2.0.2.2/
-drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.161723 dftrans-2.0.2.2/DFTrans.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       80 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   316033 2023-05-10 08:43:09.000000 dftrans-2.0.2.2/DFTrans_main.py
--rw-rw-rw-   0        0        0      307 2023-05-10 08:51:49.163724 dftrans-2.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-18 13:45:30.000000 dftrans-2.0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.132717 dftrans-2.0.2.2/config/
-drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.154722 dftrans-2.0.2.2/config/DFTrans/
--rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 dftrans-2.0.2.2/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.158722 dftrans-2.0.2.2/config/img/
--rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 dftrans-2.0.2.2/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 dftrans-2.0.2.2/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0   208137 2023-05-10 07:07:04.000000 dftrans-2.0.2.2/df_excel_define.py
--rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.2/df_excel_define_user.py
--rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.2/df_excel_plot.py
--rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.2/df_stock_define.py
--rw-rw-rw-   0        0        0       42 2023-05-10 08:51:49.164724 dftrans-2.0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     6380 2023-05-10 08:51:20.000000 dftrans-2.0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:16.670591 dftrans-2.0.2.3/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:16.667591 dftrans-2.0.2.3/DFTrans.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-10 09:43:16.000000 dftrans-2.0.2.3/DFTrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-05-10 09:43:16.000000 dftrans-2.0.2.3/DFTrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:43:16.000000 dftrans-2.0.2.3/DFTrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-10 09:43:16.000000 dftrans-2.0.2.3/DFTrans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-05-10 09:43:16.000000 dftrans-2.0.2.3/DFTrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       80 2023-05-10 09:43:16.000000 dftrans-2.0.2.3/DFTrans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   314986 2023-05-10 09:42:19.000000 dftrans-2.0.2.3/DFTrans_main.py
+-rw-rw-rw-   0        0        0      307 2023-05-10 09:43:16.670591 dftrans-2.0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-18 13:45:30.000000 dftrans-2.0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:16.641585 dftrans-2.0.2.3/config/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:16.661590 dftrans-2.0.2.3/config/DFTrans/
+-rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 dftrans-2.0.2.3/config/DFTrans/DFTrans_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:16.664590 dftrans-2.0.2.3/config/img/
+-rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 dftrans-2.0.2.3/config/img/table_arrow9_transparent_256.png
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 dftrans-2.0.2.3/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0   209633 2023-05-10 09:42:19.000000 dftrans-2.0.2.3/df_excel_define.py
+-rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.3/df_excel_define_user.py
+-rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.3/df_excel_plot.py
+-rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.3/df_stock_define.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:43:16.671592 dftrans-2.0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     6380 2023-05-10 09:42:51.000000 dftrans-2.0.2.3/setup.py
```

### Comparing `dftrans-2.0.2.2/DFTrans.egg-info/SOURCES.txt` & `dftrans-2.0.2.3/DFTrans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.2/DFTrans_main.py` & `dftrans-2.0.2.3/DFTrans_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -5916,34 +5916,18 @@
 
 def initialconfig():
     global originfunctiondict, commanddict, commandcombolist
     global usecolumnnameforprocess, commandcomment, commandalias, showversioninfo, ramfilesuffix
     global useroperatedict, manualbuttonoperatedict, useroperateconfig
     # 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
     # 判断本地目录是否存在fileprocconfig
-    if Path(fileprocconfig).is_file() is False:
-        try:
-            # 组合系统配置目录对应文件
-            sysfileprocconfig = os.path.join(sys.prefix, fileprocconfig)
-            if Path(sysfileprocconfig).is_file() is False:
-                print("本地配置文件：{}及系统原始配置文件{} 均不存在！".format(fileprocconfig, sysfileprocconfig))
-                sys.exit(-1)
-            else:
-                # 判断本地配置目录是否存在，如果不存在则创建目录，逐层创建
-                localconfigdirlayer = fileprocconfig.split("/")[:-1]
-                currentdir = ""
-                for currentlayer in localconfigdirlayer:
-                    currentdir = os.path.join(currentdir, currentlayer)
-                    if Path(currentdir).is_dir() is False:
-                        os.mkdir(currentdir)
-                # 拷贝系统配置文件到本地
-                shutil.copy(sysfileprocconfig, fileprocconfig)
-        except Exception as err:
-            print("拷贝系统原始配置到本地配置文件：{} 失败：{}".format(fileprocconfig, err))
-            sys.exit(-1)
+    result = sys_config_copy(fileprocconfig)
+    if result[0] is False:
+        print(result[1])
+        sys.exit(-1)
 
     # 读取配置文件
     try:
         with open(fileprocconfig, 'r', encoding='utf8') as fp:
             fileprocdic = json.load(fp)
             fp.close()
     except Exception as err:
```

### Comparing `dftrans-2.0.2.2/config/DFTrans/DFTrans_config.json` & `dftrans-2.0.2.3/config/DFTrans/DFTrans_config.json`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.2/config/img/table_arrow9_transparent_256.png` & `dftrans-2.0.2.3/config/img/table_arrow9_transparent_256.png`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.2/config/img/table_arrow9_transparent_64.ico` & `dftrans-2.0.2.3/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.2/df_excel_define.py` & `dftrans-2.0.2.3/df_excel_define.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import datacompy
 import os
 import sys
 from openpyxl import load_workbook
 from sqlalchemy import create_engine
 from sqlalchemy.sql import default_comparator           # 必须加上否则nuikta编译后，找不到模块。并且需要好安装1.4.40版本
 import shutil
+from pathlib import Path
 import time
 from datetime import datetime
 from hash_password import dftrans_simple_decrypt, dftrans_password_decrypt_str, dftrans_password_encrypt_str
 from psgspecialelements import *
 import inspect
 import PySimpleGUI as Sg
 import ast
@@ -3778,7 +3779,33 @@
     try:
         tempobject = eval(object_file_name[4: 0 - (len(RAM_FILE_SUFFIX) + 1)])
     except Exception as err:
         print("读取内存虚拟对象{}失败r: {}".format(object_file_name, err))
         return None
     # 返回对象的完整拷贝，不能使用指针，否则操作实在原对象上进行
     return tempobject if useorignalmemory else copy.deepcopy(tempobject)
+
+
+# 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
+# 判断本地目录是否存在fileprocconfig
+def sys_config_copy(localconfigfile: str) -> list:
+    if Path(localconfigfile).is_file() is False:
+        try:
+            # 组合系统配置目录对应文件
+            sysfileprocconfig = os.path.join(sys.prefix, localconfigfile)
+            if Path(sysfileprocconfig).is_file() is False:
+                print("本地配置文件：{}及系统原始配置文件{} 均不存在！".format(localconfigfile, sysfileprocconfig))
+                sys.exit(-1)
+            else:
+                # 判断本地配置目录是否存在，如果不存在则创建目录，逐层创建
+                localconfigdirlayer = localconfigfile.split("/")[:-1]
+                currentdir = ""
+                for currentlayer in localconfigdirlayer:
+                    currentdir = os.path.join(currentdir, currentlayer)
+                    if Path(currentdir).is_dir() is False:
+                        os.mkdir(currentdir)
+                # 拷贝系统配置文件到本地
+                shutil.copy(sysfileprocconfig, localconfigfile)
+        except Exception as err:
+            return [False, "拷贝系统原始配置到本地配置文件：{} 失败：{}".format(localconfigfile, err)]
+
+    return [True, ""]
```

### Comparing `dftrans-2.0.2.2/df_excel_define_user.py` & `dftrans-2.0.2.3/df_excel_define_user.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.2/df_excel_plot.py` & `dftrans-2.0.2.3/df_excel_plot.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.2/df_stock_define.py` & `dftrans-2.0.2.3/df_stock_define.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.2/setup.py` & `dftrans-2.0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 000009b0: 6e66 6967 6469 722c 205b 6f72 6769 6e63  nfigdir, [orginc
 000009c0: 6f6e 6669 6766 696c 655d 292c 0d0a 2020  onfigfile]),..  
 000009d0: 2020 2020 2020 5d0d 0a20 2020 2072 6574        ]..    ret
 000009e0: 7572 6e20 6461 7461 5f66 696c 6573 0d0a  urn data_files..
 000009f0: 0d0a 0d0a 7365 7475 7028 0d0a 2020 2020  ....setup(..    
 00000a00: 6e61 6d65 3d27 6466 7472 616e 7327 2c0d  name='dftrans',.
 00000a10: 0a20 2020 2076 6572 7369 6f6e 3d27 322e  .    version='2.
-00000a20: 302e 322e 3227 2c0d 0a20 2020 2064 6573  0.2.2',..    des
+00000a20: 302e 322e 3327 2c0d 0a20 2020 2064 6573  0.2.3',..    des
 00000a30: 6372 6970 7469 6f6e 3d27 e794 a8e4 ba8e  cription='......
 00000a40: e689 b9e9 878f e5a4 84e7 9086 6578 6365  ............exce
 00000a50: 6ce3 8081 7371 6ce6 95b0 e68d aee5 ba93  l...sql.........
 00000a60: e8a1 a8e3 8081 6a73 6f6e 6ce3 8081 6373  ......jsonl...cs
 00000a70: 76e7 ad89 e695 b0e6 8dae e6ba 90e7 9a84  v...............
 00000a80: e696 87e4 bbb6 efbc 8ce5 b9b6 e8be 93e5  ................
 00000a90: 87ba e588 b0e6 95b0 e68d aee5 ba93 e8a1  ................
```

