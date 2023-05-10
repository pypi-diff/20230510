# Comparing `tmp/dftrans-2.0.2.1.tar.gz` & `tmp/dftrans-2.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dftrans-2.0.2.1.tar", last modified: Tue May  9 08:22:00 2023, max compression
+gzip compressed data, was "dftrans-2.0.2.2.tar", last modified: Wed May 10 08:51:49 2023, max compression
```

## Comparing `dftrans-2.0.2.1.tar` & `dftrans-2.0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:22:00.771848 dftrans-2.0.2.1/
-drwxrwxrwx   0        0        0        0 2023-05-09 08:22:00.768847 dftrans-2.0.2.1/DFTrans.egg-info/
--rw-rw-rw-   0        0        0      307 2023-05-09 08:22:00.000000 dftrans-2.0.2.1/DFTrans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-05-09 08:22:00.000000 dftrans-2.0.2.1/DFTrans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:22:00.000000 dftrans-2.0.2.1/DFTrans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-09 08:22:00.000000 dftrans-2.0.2.1/DFTrans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-05-09 08:22:00.000000 dftrans-2.0.2.1/DFTrans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       80 2023-05-09 08:22:00.000000 dftrans-2.0.2.1/DFTrans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   314625 2023-04-18 10:56:03.000000 dftrans-2.0.2.1/DFTrans_main.py
--rw-rw-rw-   0        0        0      307 2023-05-09 08:22:00.771848 dftrans-2.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-04-18 13:45:30.000000 dftrans-2.0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 08:22:00.740841 dftrans-2.0.2.1/config/
-drwxrwxrwx   0        0        0        0 2023-05-09 08:22:00.761846 dftrans-2.0.2.1/config/DFTrans/
--rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 dftrans-2.0.2.1/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2023-05-09 08:22:00.765847 dftrans-2.0.2.1/config/img/
--rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 dftrans-2.0.2.1/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 dftrans-2.0.2.1/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0   208131 2023-04-18 14:53:50.000000 dftrans-2.0.2.1/df_excel_define.py
--rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.1/df_excel_define_user.py
--rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.1/df_excel_plot.py
--rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.1/df_stock_define.py
--rw-rw-rw-   0        0        0       42 2023-05-09 08:22:00.771848 dftrans-2.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     6380 2023-05-09 08:21:29.000000 dftrans-2.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.164724 dftrans-2.0.2.2/
+drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.161723 dftrans-2.0.2.2/DFTrans.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       80 2023-05-10 08:51:49.000000 dftrans-2.0.2.2/DFTrans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   316033 2023-05-10 08:43:09.000000 dftrans-2.0.2.2/DFTrans_main.py
+-rw-rw-rw-   0        0        0      307 2023-05-10 08:51:49.163724 dftrans-2.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-04-18 13:45:30.000000 dftrans-2.0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.132717 dftrans-2.0.2.2/config/
+drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.154722 dftrans-2.0.2.2/config/DFTrans/
+-rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 dftrans-2.0.2.2/config/DFTrans/DFTrans_config.json
+drwxrwxrwx   0        0        0        0 2023-05-10 08:51:49.158722 dftrans-2.0.2.2/config/img/
+-rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 dftrans-2.0.2.2/config/img/table_arrow9_transparent_256.png
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 dftrans-2.0.2.2/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0   208137 2023-05-10 07:07:04.000000 dftrans-2.0.2.2/df_excel_define.py
+-rw-rw-rw-   0        0        0     3418 2023-04-06 04:23:37.000000 dftrans-2.0.2.2/df_excel_define_user.py
+-rw-rw-rw-   0        0        0    17037 2023-04-18 14:54:25.000000 dftrans-2.0.2.2/df_excel_plot.py
+-rw-rw-rw-   0        0        0     7706 2023-04-18 13:30:39.000000 dftrans-2.0.2.2/df_stock_define.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:51:49.164724 dftrans-2.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     6380 2023-05-10 08:51:20.000000 dftrans-2.0.2.2/setup.py
```

### Comparing `dftrans-2.0.2.1/DFTrans.egg-info/SOURCES.txt` & `dftrans-2.0.2.2/DFTrans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.1/DFTrans_main.py` & `dftrans-2.0.2.2/DFTrans_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 TO_CURRENT_RUN = 1
 ALL_RUN = 2
 
 # 命令是否已经运行标记
 COMMAND_EXECUTED_FLAG = 0
 
 
-fileprocconfig = './config/DFTrans/DFTrans_config.json'
+fileprocconfig = 'config/DFTrans/DFTrans_config.json'
 useroperatedir = 'filetrans'
 userconfigfile = 'user_operate_record.json'
 
 global usecolumnnameforprocess, originfunctiondict, commanddict, commandcomment
 global commandalias, showversioninfo, ramfilesuffix
 global localusecolumnnameforprocess, localoriginfunctiondict, localcommanddict
 global commandcombolist, commandtabledictlist, commandtablekey, commandmenulist
@@ -5914,14 +5914,37 @@
                                    background_color='dark blue')
 
 
 def initialconfig():
     global originfunctiondict, commanddict, commandcombolist
     global usecolumnnameforprocess, commandcomment, commandalias, showversioninfo, ramfilesuffix
     global useroperatedict, manualbuttonoperatedict, useroperateconfig
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
     # 读取配置文件
     try:
         with open(fileprocconfig, 'r', encoding='utf8') as fp:
             fileprocdic = json.load(fp)
             fp.close()
     except Exception as err:
         print("读取配置文件：{}失败：{}".format(fileprocconfig, err))
```

### Comparing `dftrans-2.0.2.1/config/DFTrans/DFTrans_config.json` & `dftrans-2.0.2.2/config/DFTrans/DFTrans_config.json`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.1/config/img/table_arrow9_transparent_256.png` & `dftrans-2.0.2.2/config/img/table_arrow9_transparent_256.png`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.1/config/img/table_arrow9_transparent_64.ico` & `dftrans-2.0.2.2/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.1/df_excel_define.py` & `dftrans-2.0.2.2/df_excel_define.py`

 * *Files 0% similar despite different names*

```diff
@@ -3617,14 +3617,17 @@
             break
         elif event == "_save_":
             filetemp = Sg.popup_get_file('选择文件',
                                          save_as=True,
                                          file_types=(('png文件', '*.png'), ),
                                          initial_folder="d:/temp/",
                                          default_path="figure.png",
+
+
+
                                          history_setting_filename="d:/temp/figure.png",
                                          keep_on_top=True, modal=True,
                                          no_window=True, icon=LOCAL_SYSTEM_ICON)
             print(filetemp)
             if dfplot:
                 dfplot.save_figure(filetemp)
             continue
```

### Comparing `dftrans-2.0.2.1/df_excel_define_user.py` & `dftrans-2.0.2.2/df_excel_define_user.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.1/df_excel_plot.py` & `dftrans-2.0.2.2/df_excel_plot.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.1/df_stock_define.py` & `dftrans-2.0.2.2/df_stock_define.py`

 * *Files identical despite different names*

### Comparing `dftrans-2.0.2.1/setup.py` & `dftrans-2.0.2.2/setup.py`

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
-00000a20: 302e 322e 3127 2c0d 0a20 2020 2064 6573  0.2.1',..    des
+00000a20: 302e 322e 3227 2c0d 0a20 2020 2064 6573  0.2.2',..    des
 00000a30: 6372 6970 7469 6f6e 3d27 e794 a8e4 ba8e  cription='......
 00000a40: e689 b9e9 878f e5a4 84e7 9086 6578 6365  ............exce
 00000a50: 6ce3 8081 7371 6ce6 95b0 e68d aee5 ba93  l...sql.........
 00000a60: e8a1 a8e3 8081 6a73 6f6e 6ce3 8081 6373  ......jsonl...cs
 00000a70: 76e7 ad89 e695 b0e6 8dae e6ba 90e7 9a84  v...............
 00000a80: e696 87e4 bbb6 efbc 8ce5 b9b6 e8be 93e5  ................
 00000a90: 87ba e588 b0e6 95b0 e68d aee5 ba93 e8a1  ................
```

