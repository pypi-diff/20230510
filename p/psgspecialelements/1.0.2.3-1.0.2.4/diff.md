# Comparing `tmp/psgspecialelements-1.0.2.3.tar.gz` & `tmp/psgspecialelements-1.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgspecialelements-1.0.2.3.tar", last modified: Tue May  9 08:15:28 2023, max compression
+gzip compressed data, was "psgspecialelements-1.0.2.4.tar", last modified: Wed May 10 13:47:15 2023, max compression
```

## Comparing `psgspecialelements-1.0.2.3.tar` & `psgspecialelements-1.0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:15:28.466161 psgspecialelements-1.0.2.3/
--rw-rw-rw-   0        0        0      255 2023-05-09 08:15:28.465161 psgspecialelements-1.0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1525 2023-04-21 00:40:07.000000 psgspecialelements-1.0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 08:15:28.445156 psgspecialelements-1.0.2.3/config/
-drwxrwxrwx   0        0        0        0 2023-05-09 08:15:28.454158 psgspecialelements-1.0.2.3/config/img/
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 psgspecialelements-1.0.2.3/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0    34392 2023-04-06 03:13:05.000000 psgspecialelements-1.0.2.3/hash_password.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:15:28.463160 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/
--rw-rw-rw-   0        0        0      255 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-05-09 08:15:28.000000 psgspecialelements-1.0.2.3/psgspecialelements.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   239428 2023-05-09 08:11:32.000000 psgspecialelements-1.0.2.3/psgspecialelements.py
--rw-rw-rw-   0        0        0       42 2023-05-09 08:15:28.466161 psgspecialelements-1.0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2782 2023-05-09 08:15:08.000000 psgspecialelements-1.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:47:15.348108 psgspecialelements-1.0.2.4/
+-rw-rw-rw-   0        0        0      255 2023-05-10 13:47:15.347107 psgspecialelements-1.0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1525 2023-04-21 00:40:07.000000 psgspecialelements-1.0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 13:47:15.325102 psgspecialelements-1.0.2.4/config/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:47:15.334103 psgspecialelements-1.0.2.4/config/img/
+-rw-rw-rw-   0        0        0    16958 2023-05-10 13:46:04.000000 psgspecialelements-1.0.2.4/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0    34392 2023-04-06 03:13:05.000000 psgspecialelements-1.0.2.4/hash_password.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:47:15.345106 psgspecialelements-1.0.2.4/psgspecialelements.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-05-10 13:47:15.000000 psgspecialelements-1.0.2.4/psgspecialelements.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-05-10 13:47:15.000000 psgspecialelements-1.0.2.4/psgspecialelements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:47:15.000000 psgspecialelements-1.0.2.4/psgspecialelements.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-10 13:47:15.000000 psgspecialelements-1.0.2.4/psgspecialelements.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2023-05-10 13:47:15.000000 psgspecialelements-1.0.2.4/psgspecialelements.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-05-10 13:47:15.000000 psgspecialelements-1.0.2.4/psgspecialelements.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   241263 2023-05-10 13:46:51.000000 psgspecialelements-1.0.2.4/psgspecialelements.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:47:15.348108 psgspecialelements-1.0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2782 2023-05-10 13:46:51.000000 psgspecialelements-1.0.2.4/setup.py
```

### Comparing `psgspecialelements-1.0.2.3/README.md` & `psgspecialelements-1.0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.3/config/img/table_arrow9_transparent_64.ico` & `psgspecialelements-1.0.2.4/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.3/hash_password.py` & `psgspecialelements-1.0.2.4/hash_password.py`

 * *Files identical despite different names*

### Comparing `psgspecialelements-1.0.2.3/psgspecialelements.py` & `psgspecialelements-1.0.2.4/psgspecialelements.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 import ast
 
 import PySimpleGUI as Sg
 import pandas as pd
 import numpy as np
 import copy
 import os
+import sys
+import shutil
+from pathlib import Path
 from openpyxl import load_workbook
 import inspect
 from dataclasses import dataclass
 
-SYSTEM_ICON = './config/img/table_arrow9_transparent_64.ico'
-
+SYSTEM_ICON = 'config/img/table_arrow9_transparent_64.ico'
+SYSTEM_DATA_FILES = [SYSTEM_ICON]
 INPUTFILE_SRTING_COLUMNS = '-string-columns'
 OUTPUTFILE_RENAME_KEY = '-output'
 
 # 表格tab中的最大阈值，表格数及每张表格的最大列数
 MAX_TABLE_NUMBER = 15  # 最大配置，大于18运行错误
 MAX_TABLE_SHOW_COLUMNS = 20
 
@@ -3672,14 +3675,46 @@
         """
         if attribute is None:
             return self.currenttable
         else:
             return super().get(attribute=attribute, **kwargs)
 
 
+# 根据系统配置拷贝相应的数据文件和配置文件到本地目录
+def sys_data_files_copy(sysdatafiles: list) -> list:
+    for file in sysdatafiles:
+        result = sys_config_copy(file)
+        if result[0] is False:
+            return result
+    return [True, ""]
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
+                localdir = os.path.dirname(localconfigfile)
+                if Path(localdir).is_dir() is False:
+                    os.makedirs(os.path.dirname(localdir))
+                # 拷贝系统配置文件到本地
+                shutil.copy(sysfileprocconfig, localconfigfile)
+        except Exception as err:
+            return [False, "拷贝系统原始配置到本地配置文件：{} 失败：{}".format(localconfigfile, err)]
+
+    return [True, ""]
+
+
 def main_test():
     from PySimpleGUI import THEME_CLAM, THEME_DEFAULT, THEME_ALT, THEME_CLASSIC
     Sg.set_options(ttk_theme=THEME_DEFAULT)
     dfdata1 = pd.DataFrame(
         ["数据{}-{}".format(x, y) for y in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
         for x in range(MAX_SPECIAL_TABLE_ROWS * MAX_SPECIAL_TABLE_ROWS - 10))
     dfdata2 = pd.DataFrame(
@@ -3762,14 +3797,20 @@
         None,
         [],  # 菜单配置文件
         ['是', '否'],
         commandtypelist,  # 命令类型
         []  # 图标文件
     ]
 
+    # 拷贝系统文件
+    result = sys_data_files_copy(SYSTEM_DATA_FILES)
+    if result[0] is False:
+        print(result[1])
+        sys.exit(-1)
+
     tablegroupkey = '_table_group_'
     headings1 = ["数据列{}".format(x) for x in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
     headings2 = ["测试列{}".format(x) for x in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
     headings3 = ["新数据列{}".format(x) for x in range(MAX_SPECIAL_TABLE_COLUMNS * 2)]
     dfdata1.columns = headings1
     dfdata2.columns = headings2
     dfdata3.columns = headings3
```

### Comparing `psgspecialelements-1.0.2.3/setup.py` & `psgspecialelements-1.0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
 00000010: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
 00000020: 6669 6e64 5f70 6163 6b61 6765 730d 0a0d  find_packages...
 00000030: 0a73 6574 7570 280d 0a20 2020 206e 616d  .setup(..    nam
 00000040: 653d 2770 7367 7370 6563 6961 6c65 6c65  e='psgspecialele
 00000050: 6d65 6e74 7327 2c0d 0a20 2020 2076 6572  ments',..    ver
-00000060: 7369 6f6e 3d27 312e 302e 322e 3327 2c0d  sion='1.0.2.3',.
+00000060: 7369 6f6e 3d27 312e 302e 322e 3427 2c0d  sion='1.0.2.4',.
 00000070: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
 00000080: 3d27 7370 6563 6961 6c20 656c 656d 656e  ='special elemen
 00000090: 7473 2062 6173 6564 206f 6e20 7079 7369  ts based on pysi
 000000a0: 6d70 6c65 6775 6920 656c 656d 656e 7473  mplegui elements
 000000b0: 272c 0d0a 2020 2020 6175 7468 6f72 3d27  ',..    author='
 000000c0: 4672 616e 6b20 476f 6e67 272c 0d0a 2020  Frank Gong',..  
 000000d0: 2020 6175 7468 6f72 5f65 6d61 696c 3d27    author_email='
```

