# Comparing `tmp/batframes-1.0.0.3.tar.gz` & `tmp/batframes-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batframes-1.0.0.3.tar", last modified: Wed May 10 08:57:03 2023, max compression
+gzip compressed data, was "batframes-1.0.0.4.tar", last modified: Wed May 10 09:49:29 2023, max compression
```

## Comparing `batframes-1.0.0.3.tar` & `batframes-1.0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:57:03.321685 batframes-1.0.0.3/
--rw-rw-rw-   0        0        0      330 2023-05-10 08:57:03.320683 batframes-1.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-04-06 11:08:10.000000 batframes-1.0.0.3/README.md
--rw-rw-rw-   0        0        0     9590 2023-04-07 22:32:48.000000 batframes-1.0.0.3/bat_function_call_define.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:57:03.301679 batframes-1.0.0.3/bat_inner_module/
--rw-rw-rw-   0        0        0      227 2023-04-07 22:37:37.000000 batframes-1.0.0.3/bat_inner_module/inner_demo.py
--rw-rw-rw-   0        0        0      143 2023-04-07 15:30:40.000000 batframes-1.0.0.3/bat_inner_module/inner_demo1.py
--rw-rw-rw-   0        0        0      173 2023-04-07 10:56:05.000000 batframes-1.0.0.3/bat_inner_module/readme_for_inner.md
--rw-rw-rw-   0        0        0    68212 2023-04-08 01:59:23.000000 batframes-1.0.0.3/bat_menu_auto.py
--rw-rw-rw-   0        0        0    43797 2023-05-10 08:56:03.000000 batframes-1.0.0.3/batframe_main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:57:03.309681 batframes-1.0.0.3/batframes.egg-info/
--rw-rw-rw-   0        0        0      330 2023-05-10 08:57:03.000000 batframes-1.0.0.3/batframes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-05-10 08:57:03.000000 batframes-1.0.0.3/batframes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:57:03.000000 batframes-1.0.0.3/batframes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-10 08:57:03.000000 batframes-1.0.0.3/batframes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      308 2023-05-10 08:57:03.000000 batframes-1.0.0.3/batframes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       77 2023-05-10 08:57:03.000000 batframes-1.0.0.3/batframes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 08:57:03.288676 batframes-1.0.0.3/config/
-drwxrwxrwx   0        0        0        0 2023-05-10 08:57:03.310680 batframes-1.0.0.3/config/DFTrans/
--rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 batframes-1.0.0.3/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 08:57:03.312682 batframes-1.0.0.3/config/batframe/
--rw-rw-rw-   0        0        0     2816 2023-04-11 01:59:57.000000 batframes-1.0.0.3/config/batframe/bat_tools_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 08:57:03.319683 batframes-1.0.0.3/config/img/
--rw-rw-rw-   0        0        0     7631 2023-04-06 08:06:16.000000 batframes-1.0.0.3/config/img/Excel.png
--rw-rw-rw-   0        0        0     1962 2023-04-06 08:06:16.000000 batframes-1.0.0.3/config/img/excel.gif
--rw-rw-rw-   0        0        0    10200 2023-04-06 08:06:16.000000 batframes-1.0.0.3/config/img/little_bear.png
--rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 batframes-1.0.0.3/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 batframes-1.0.0.3/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0      585 2023-04-08 00:42:18.000000 batframes-1.0.0.3/nuitka_dependency_files.py
--rw-rw-rw-   0        0        0       42 2023-05-10 08:57:03.321685 batframes-1.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     6956 2023-05-10 08:56:27.000000 batframes-1.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:49:29.682104 batframes-1.0.0.4/
+-rw-rw-rw-   0        0        0      330 2023-05-10 09:49:29.682104 batframes-1.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2023-04-06 11:08:10.000000 batframes-1.0.0.4/README.md
+-rw-rw-rw-   0        0        0     9590 2023-04-07 22:32:48.000000 batframes-1.0.0.4/bat_function_call_define.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:49:29.659099 batframes-1.0.0.4/bat_inner_module/
+-rw-rw-rw-   0        0        0      227 2023-04-07 22:37:37.000000 batframes-1.0.0.4/bat_inner_module/inner_demo.py
+-rw-rw-rw-   0        0        0      143 2023-04-07 15:30:40.000000 batframes-1.0.0.4/bat_inner_module/inner_demo1.py
+-rw-rw-rw-   0        0        0      173 2023-04-07 10:56:05.000000 batframes-1.0.0.4/bat_inner_module/readme_for_inner.md
+-rw-rw-rw-   0        0        0    68212 2023-04-08 01:59:23.000000 batframes-1.0.0.4/bat_menu_auto.py
+-rw-rw-rw-   0        0        0    42689 2023-05-10 09:48:33.000000 batframes-1.0.0.4/batframe_main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:49:29.669101 batframes-1.0.0.4/batframes.egg-info/
+-rw-rw-rw-   0        0        0      330 2023-05-10 09:49:29.000000 batframes-1.0.0.4/batframes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-05-10 09:49:29.000000 batframes-1.0.0.4/batframes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:49:29.000000 batframes-1.0.0.4/batframes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-10 09:49:29.000000 batframes-1.0.0.4/batframes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      308 2023-05-10 09:49:29.000000 batframes-1.0.0.4/batframes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       77 2023-05-10 09:49:29.000000 batframes-1.0.0.4/batframes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 09:49:29.644096 batframes-1.0.0.4/config/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:49:29.670102 batframes-1.0.0.4/config/DFTrans/
+-rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 batframes-1.0.0.4/config/DFTrans/DFTrans_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 09:49:29.672102 batframes-1.0.0.4/config/batframe/
+-rw-rw-rw-   0        0        0     2816 2023-04-11 01:59:57.000000 batframes-1.0.0.4/config/batframe/bat_tools_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 09:49:29.680104 batframes-1.0.0.4/config/img/
+-rw-rw-rw-   0        0        0     7631 2023-04-06 08:06:16.000000 batframes-1.0.0.4/config/img/Excel.png
+-rw-rw-rw-   0        0        0     1962 2023-04-06 08:06:16.000000 batframes-1.0.0.4/config/img/excel.gif
+-rw-rw-rw-   0        0        0    10200 2023-04-06 08:06:16.000000 batframes-1.0.0.4/config/img/little_bear.png
+-rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 batframes-1.0.0.4/config/img/table_arrow9_transparent_256.png
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 batframes-1.0.0.4/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0      585 2023-04-08 00:42:18.000000 batframes-1.0.0.4/nuitka_dependency_files.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:49:29.682104 batframes-1.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     6956 2023-05-10 09:49:00.000000 batframes-1.0.0.4/setup.py
```

### Comparing `batframes-1.0.0.3/bat_function_call_define.py` & `batframes-1.0.0.4/bat_function_call_define.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/bat_menu_auto.py` & `batframes-1.0.0.4/bat_menu_auto.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/batframe_main.py` & `batframes-1.0.0.4/batframe_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*-
+bat# -*- coding: utf-8 -*-
 # !/usr/bin/env python
 """
 ###############################################################################################################
 # BAT工具集成框架
 # 用于集成相关的配套工具
 # 可以通过配置文件增加工具
 # Version 1.0.0
@@ -828,34 +828,18 @@
 
         debugswitchdefault = 'n'
 
         fileprocconfig = battoolsconfig
 
         # 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
         # 判断本地目录是否存在fileprocconfig
-        if Path(fileprocconfig).is_file() is False:
-            try:
-                # 组合系统配置目录对应文件
-                sysfileprocconfig = os.path.join(sys.prefix, fileprocconfig)
-                if Path(sysfileprocconfig).is_file() is False:
-                    print("本地配置文件：{}及系统原始配置文件{} 均不存在！".format(fileprocconfig, sysfileprocconfig))
-                    sys.exit(-1)
-                else:
-                    # 判断本地配置目录是否存在，如果不存在则创建目录，逐层创建
-                    localconfigdirlayer = fileprocconfig.split("/")[:-1]
-                    currentdir = ""
-                    for currentlayer in localconfigdirlayer:
-                        currentdir = os.path.join(currentdir, currentlayer)
-                        if Path(currentdir).is_dir() is False:
-                            os.mkdir(currentdir)
-                    # 拷贝系统配置文件到本地
-                    shutil.copy(sysfileprocconfig, fileprocconfig)
-            except Exception as err:
-                print("拷贝系统原始配置到本地配置文件：{} 失败：{}".format(fileprocconfig, err))
-                sys.exit(-1)
+        result = sys_config_copy(fileprocconfig)
+        if result[0] is False:
+            print(result[1])
+            sys.exit(-1)
 
         # 读取配置文件
         try:
             with open(battoolsconfig, 'r', encoding='utf8') as fp:
                 configdic = json.load(fp)
                 fp.close()
         except Exception as err:
```

### Comparing `batframes-1.0.0.3/batframes.egg-info/SOURCES.txt` & `batframes-1.0.0.4/batframes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/config/DFTrans/DFTrans_config.json` & `batframes-1.0.0.4/config/DFTrans/DFTrans_config.json`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/config/batframe/bat_tools_config.json` & `batframes-1.0.0.4/config/batframe/bat_tools_config.json`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/config/img/Excel.png` & `batframes-1.0.0.4/config/img/Excel.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/config/img/excel.gif` & `batframes-1.0.0.4/config/img/excel.gif`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/config/img/little_bear.png` & `batframes-1.0.0.4/config/img/little_bear.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/config/img/table_arrow9_transparent_256.png` & `batframes-1.0.0.4/config/img/table_arrow9_transparent_256.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/config/img/table_arrow9_transparent_64.ico` & `batframes-1.0.0.4/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/nuitka_dependency_files.py` & `batframes-1.0.0.4/nuitka_dependency_files.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.3/setup.py` & `batframes-1.0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 00000b60: 6f6e 6669 6764 6972 2c20 5b6f 7267 696e  onfigdir, [orgin
 00000b70: 636f 6e66 6967 6669 6c65 5d29 2c0d 0a20  configfile]),.. 
 00000b80: 2020 2020 2020 205d 0d0a 2020 2020 7265         ]..    re
 00000b90: 7475 726e 2064 6174 615f 6669 6c65 730d  turn data_files.
 00000ba0: 0a0d 0a0d 0a73 6574 7570 280d 0a20 2020  .....setup(..   
 00000bb0: 206e 616d 653d 2762 6174 6672 616d 6573   name='batframes
 00000bc0: 272c 0d0a 2020 2020 7665 7273 696f 6e3d  ',..    version=
-00000bd0: 2731 2e30 2e30 2e33 272c 0d0a 2020 2020  '1.0.0.3',..    
+00000bd0: 2731 2e30 2e30 2e34 272c 0d0a 2020 2020  '1.0.0.4',..    
 00000be0: 6465 7363 7269 7074 696f 6e3d 27e5 8faf  description='...
 00000bf0: e4bb a5e9 858d e7bd aee5 b086 e5a4 9ae4  ................
 00000c00: b8aa e58f afe6 89a7 e8a1 8ce6 9687 e4bb  ................
 00000c10: b6e5 928c e586 85e9 83a8 e591 bde4 bba4  ................
 00000c20: e4b8 b2e6 8ea5 e688 90e4 b880 e4b8 aae5  ................
 00000c30: ae8c e695 b4e5 91bd e4bb a4e6 89a7 e8a1  ................
 00000c40: 8ce7 9a84 e6a1 86e6 9eb6 e5b7 a5e5 85b7  ................
```

