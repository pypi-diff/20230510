# Comparing `tmp/dftrans-2.0.2.4.tar.gz` & `tmp/dftrans-2.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dftrans-2.0.2.4.tar", last modified: Wed May 10 12:09:08 2023, max compression
+gzip compressed data, was "dftrans-2.0.2.5.tar", last modified: Wed May 10 13:56:13 2023, max compression
```

## Comparing `dftrans-2.0.2.4.tar` & `dftrans-2.0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:09:08.534846 dftrans-2.0.2.4/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:09:08.530845 dftrans-2.0.2.4/DFTrans.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-10 12:09:08.000000 dftrans-2.0.2.4/DFTrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-05-10 12:09:08.000000 dftrans-2.0.2.4/DFTrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:09:08.000000 dftrans-2.0.2.4/DFTrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-10 12:09:08.000000 dftrans-2.0.2.4/DFTrans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-05-10 12:09:08.000000 dftrans-2.0.2.4/DFTrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       80 2023-05-10 12:09:08.000000 dftrans-2.0.2.4/DFTrans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   314986 2023-05-10 09:42:19.000000 dftrans-2.0.2.4/DFTrans_main.py
--rw-rw-rw-   0        0        0      307 2023-05-10 12:09:08.533846 dftrans-2.0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-18 13:45:30.000000 dftrans-2.0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 12:09:08.504842 dftrans-2.0.2.4/config/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:09:08.524844 dftrans-2.0.2.4/config/DFTrans/
--rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 dftrans-2.0.2.4/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2023-05-10 12:09:08.527844 dftrans-2.0.2.4/config/img/
--rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 dftrans-2.0.2.4/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 dftrans-2.0.2.4/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0   209355 2023-05-10 12:07:19.000000 dftrans-2.0.2.4/df_excel_define.py
--rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.4/df_excel_define_user.py
--rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.4/df_excel_plot.py
--rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.4/df_stock_define.py
--rw-rw-rw-   0        0        0       42 2023-05-10 12:09:08.534846 dftrans-2.0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     6380 2023-05-10 12:07:19.000000 dftrans-2.0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.637893 dftrans-2.0.2.5/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.634893 dftrans-2.0.2.5/DFTrans.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       80 2023-05-10 13:56:13.000000 dftrans-2.0.2.5/DFTrans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   315088 2023-05-10 13:54:55.000000 dftrans-2.0.2.5/DFTrans_main.py
+-rw-rw-rw-   0        0        0      307 2023-05-10 13:56:13.636892 dftrans-2.0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-18 13:45:30.000000 dftrans-2.0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.608887 dftrans-2.0.2.5/config/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.628891 dftrans-2.0.2.5/config/DFTrans/
+-rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 dftrans-2.0.2.5/config/DFTrans/DFTrans_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 13:56:13.631891 dftrans-2.0.2.5/config/img/
+-rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 dftrans-2.0.2.5/config/img/table_arrow9_transparent_256.png
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 dftrans-2.0.2.5/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0   208159 2023-05-10 13:53:28.000000 dftrans-2.0.2.5/df_excel_define.py
+-rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.5/df_excel_define_user.py
+-rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.5/df_excel_plot.py
+-rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.5/df_stock_define.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:56:13.637893 dftrans-2.0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     6380 2023-05-10 13:55:20.000000 dftrans-2.0.2.5/setup.py
```

### Comparing `dftrans-2.0.2.4/DFTrans.egg-info/SOURCES.txt` & `dftrans-2.0.2.5/DFTrans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.4/DFTrans_main.py` & `dftrans-2.0.2.5/DFTrans_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,14 +138,16 @@
 COMMAND_EXECUTED_FLAG = 0
 
 
 fileprocconfig = 'config/DFTrans/DFTrans_config.json'
 useroperatedir = 'filetrans'
 userconfigfile = 'user_operate_record.json'
 
+DFTRANS_SYSTEM_DATA_FILES = [fileprocconfig, LOCAL_SYSTEM_ICON, LOCAL_SYSTEM_IMAGE]
+
 global usecolumnnameforprocess, originfunctiondict, commanddict, commandcomment
 global commandalias, showversioninfo, ramfilesuffix
 global localusecolumnnameforprocess, localoriginfunctiondict, localcommanddict
 global commandcombolist, commandtabledictlist, commandtablekey, commandmenulist
 global currentdfnamelist, currentdfcolumnlist, commandmenudict, datatablebuttonmenuevent, datatablerightclickevent
 global specialdflist, specialdflistcopy, usermodule
 global mycommandlistfile, myinputfiles, commandfilecomment
@@ -5916,15 +5918,15 @@
 
 def initialconfig():
     global originfunctiondict, commanddict, commandcombolist
     global usecolumnnameforprocess, commandcomment, commandalias, showversioninfo, ramfilesuffix
     global useroperatedict, manualbuttonoperatedict, useroperateconfig
     # 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
     # 判断本地目录是否存在fileprocconfig
-    result = sys_config_copy(fileprocconfig)
+    result = sys_data_files_copy(DFTRANS_SYSTEM_DATA_FILES)
     if result[0] is False:
         print(result[1])
         sys.exit(-1)
 
     # 读取配置文件
     try:
         with open(fileprocconfig, 'r', encoding='utf8') as fp:
```

### Comparing `dftrans-2.0.2.4/config/DFTrans/DFTrans_config.json` & `dftrans-2.0.2.5/config/DFTrans/DFTrans_config.json`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.4/config/img/table_arrow9_transparent_256.png` & `dftrans-2.0.2.5/config/img/table_arrow9_transparent_256.png`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.4/config/img/table_arrow9_transparent_64.ico` & `dftrans-2.0.2.5/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.4/df_excel_define.py` & `dftrans-2.0.2.5/df_excel_define.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from df_stock_define import *
 DEF_FT_L = ('宋体', 10)
 DEF_PD_L = (5, 5)
 PARAM_FT = ('黑体', 10)
 DEF_PLOT_WIDTH = 12
 DEF_PLOT_HEIGHT = 8
 
-# LOCAL_SYSTEM_ICON = "./config/img/dftrans06.ico"
-LOCAL_SYSTEM_ICON = "./config/img/table_arrow9_transparent_64.ico"
-LOCAL_SYSTEM_IMAGE = "./config/img/table_arrow9_transparent_256.png"
+# LOCAL_SYSTEM_ICON = "config/img/dftrans06.ico"
+LOCAL_SYSTEM_ICON = "config/img/table_arrow9_transparent_64.ico"
+LOCAL_SYSTEM_IMAGE = "config/img/table_arrow9_transparent_256.png"
 
 HIGHLIST_SELECTED_COLOR = 'dark blue'
 ARG_PARAM_VALUE_COLOR = 'blue'
 
 TEXT_COLOR = 'black'
 TEXT_BACKGROUND_COLOR = 'white'
 INPUT_TEXT_COLOR = 'blue'
@@ -3780,27 +3780,7 @@
         tempobject = eval(object_file_name[4: 0 - (len(RAM_FILE_SUFFIX) + 1)])
     except Exception as err:
         print("读取内存虚拟对象{}失败r: {}".format(object_file_name, err))
         return None
     # 返回对象的完整拷贝，不能使用指针，否则操作实在原对象上进行
     return tempobject if useorignalmemory else copy.deepcopy(tempobject)
 
-
-# 系统初始化，判断fileprocconfig是否存在，如果不存在，尝试从系统config目录（pip，python的安装目录拷贝），系统目录也不存在则报错退出
-# 判断本地目录是否存在fileprocconfig
-def sys_config_copy(localconfigfile: str) -> list:
-    if Path(localconfigfile).is_file() is False:
-        try:
-            # 组合系统配置目录对应文件
-            sysfileprocconfig = os.path.join(sys.prefix, localconfigfile)
-            if Path(sysfileprocconfig).is_file() is False:
-                print("本地配置文件：{}及系统原始配置文件{} 均不存在！".format(localconfigfile, sysfileprocconfig))
-                sys.exit(-1)
-            else:
-                # 判断本地配置目录是否存在，如果不存在则创建目录，逐层创建
-                os.makedirs(os.path.dirname(localconfigfile))
-                # 拷贝系统配置文件到本地
-                shutil.copy(sysfileprocconfig, localconfigfile)
-        except Exception as err:
-            return [False, "拷贝系统原始配置到本地配置文件：{} 失败：{}".format(localconfigfile, err)]
-
-    return [True, ""]
```

### Comparing `dftrans-2.0.2.4/df_excel_define_user.py` & `dftrans-2.0.2.5/df_excel_define_user.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.4/df_excel_plot.py` & `dftrans-2.0.2.5/df_excel_plot.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.4/df_stock_define.py` & `dftrans-2.0.2.5/df_stock_define.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.4/setup.py` & `dftrans-2.0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 000009b0: 6e66 6967 6469 722c 205b 6f72 6769 6e63  nfigdir, [orginc
 000009c0: 6f6e 6669 6766 696c 655d 292c 0d0a 2020  onfigfile]),..  
 000009d0: 2020 2020 2020 5d0d 0a20 2020 2072 6574        ]..    ret
 000009e0: 7572 6e20 6461 7461 5f66 696c 6573 0d0a  urn data_files..
 000009f0: 0d0a 0d0a 7365 7475 7028 0d0a 2020 2020  ....setup(..    
 00000a00: 6e61 6d65 3d27 6466 7472 616e 7327 2c0d  name='dftrans',.
 00000a10: 0a20 2020 2076 6572 7369 6f6e 3d27 322e  .    version='2.
-00000a20: 302e 322e 3427 2c0d 0a20 2020 2064 6573  0.2.4',..    des
+00000a20: 302e 322e 3527 2c0d 0a20 2020 2064 6573  0.2.5',..    des
 00000a30: 6372 6970 7469 6f6e 3d27 e794 a8e4 ba8e  cription='......
 00000a40: e689 b9e9 878f e5a4 84e7 9086 6578 6365  ............exce
 00000a50: 6ce3 8081 7371 6ce6 95b0 e68d aee5 ba93  l...sql.........
 00000a60: e8a1 a8e3 8081 6a73 6f6e 6ce3 8081 6373  ......jsonl...cs
 00000a70: 76e7 ad89 e695 b0e6 8dae e6ba 90e7 9a84  v...............
 00000a80: e696 87e4 bbb6 efbc 8ce5 b9b6 e8be 93e5  ................
 00000a90: 87ba e588 b0e6 95b0 e68d aee5 ba93 e8a1  ................
```

