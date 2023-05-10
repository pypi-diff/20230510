# Comparing `tmp/batframes-1.0.0.1.tar.gz` & `tmp/batframes-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batframes-1.0.0.1.tar", last modified: Tue May  9 08:37:42 2023, max compression
+gzip compressed data, was "batframes-1.0.0.2.tar", last modified: Tue May  9 14:17:12 2023, max compression
```

## Comparing `batframes-1.0.0.1.tar` & `batframes-1.0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:37:42.978578 batframes-1.0.0.1/
--rw-rw-rw-   0        0        0      330 2023-05-09 08:37:42.977578 batframes-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-04-06 11:08:10.000000 batframes-1.0.0.1/README.md
--rw-rw-rw-   0        0        0     9590 2023-04-07 22:32:48.000000 batframes-1.0.0.1/bat_function_call_define.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:37:42.956574 batframes-1.0.0.1/bat_inner_module/
--rw-rw-rw-   0        0        0      227 2023-04-07 22:37:37.000000 batframes-1.0.0.1/bat_inner_module/inner_demo.py
--rw-rw-rw-   0        0        0      143 2023-04-07 15:30:40.000000 batframes-1.0.0.1/bat_inner_module/inner_demo1.py
--rw-rw-rw-   0        0        0      173 2023-04-07 10:56:05.000000 batframes-1.0.0.1/bat_inner_module/readme_for_inner.md
--rw-rw-rw-   0        0        0    68212 2023-04-08 01:59:23.000000 batframes-1.0.0.1/bat_menu_auto.py
--rw-rw-rw-   0        0        0    42258 2023-04-18 03:27:51.000000 batframes-1.0.0.1/batframe_main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:37:42.965575 batframes-1.0.0.1/batframes.egg-info/
--rw-rw-rw-   0        0        0      330 2023-05-09 08:37:42.000000 batframes-1.0.0.1/batframes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-05-09 08:37:42.000000 batframes-1.0.0.1/batframes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:37:42.000000 batframes-1.0.0.1/batframes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-09 08:37:42.000000 batframes-1.0.0.1/batframes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      308 2023-05-09 08:37:42.000000 batframes-1.0.0.1/batframes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       77 2023-05-09 08:37:42.000000 batframes-1.0.0.1/batframes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 08:37:42.942570 batframes-1.0.0.1/config/
-drwxrwxrwx   0        0        0        0 2023-05-09 08:37:42.966576 batframes-1.0.0.1/config/DFTrans/
--rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 batframes-1.0.0.1/config/DFTrans/DFTrans_config.json
-drwxrwxrwx   0        0        0        0 2023-05-09 08:37:42.968576 batframes-1.0.0.1/config/batframe/
--rw-rw-rw-   0        0        0     2816 2023-04-11 01:59:57.000000 batframes-1.0.0.1/config/batframe/bat_tools_config.json
-drwxrwxrwx   0        0        0        0 2023-05-09 08:37:42.976578 batframes-1.0.0.1/config/img/
--rw-rw-rw-   0        0        0     7631 2023-04-06 08:06:16.000000 batframes-1.0.0.1/config/img/Excel.png
--rw-rw-rw-   0        0        0     1962 2023-04-06 08:06:16.000000 batframes-1.0.0.1/config/img/excel.gif
--rw-rw-rw-   0        0        0    10200 2023-04-06 08:06:16.000000 batframes-1.0.0.1/config/img/little_bear.png
--rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 batframes-1.0.0.1/config/img/table_arrow9_transparent_256.png
--rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 batframes-1.0.0.1/config/img/table_arrow9_transparent_64.ico
--rw-rw-rw-   0        0        0      585 2023-04-08 00:42:18.000000 batframes-1.0.0.1/nuitka_dependency_files.py
--rw-rw-rw-   0        0        0       42 2023-05-09 08:37:42.978578 batframes-1.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     6956 2023-05-09 08:37:05.000000 batframes-1.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:17:12.217241 batframes-1.0.0.2/
+-rw-rw-rw-   0        0        0      330 2023-05-09 14:17:12.217241 batframes-1.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2023-04-06 11:08:10.000000 batframes-1.0.0.2/README.md
+-rw-rw-rw-   0        0        0     9590 2023-04-07 22:32:48.000000 batframes-1.0.0.2/bat_function_call_define.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:17:12.194236 batframes-1.0.0.2/bat_inner_module/
+-rw-rw-rw-   0        0        0      227 2023-04-07 22:37:37.000000 batframes-1.0.0.2/bat_inner_module/inner_demo.py
+-rw-rw-rw-   0        0        0      143 2023-04-07 15:30:40.000000 batframes-1.0.0.2/bat_inner_module/inner_demo1.py
+-rw-rw-rw-   0        0        0      173 2023-04-07 10:56:05.000000 batframes-1.0.0.2/bat_inner_module/readme_for_inner.md
+-rw-rw-rw-   0        0        0    68212 2023-04-08 01:59:23.000000 batframes-1.0.0.2/bat_menu_auto.py
+-rw-rw-rw-   0        0        0    42258 2023-04-18 03:27:51.000000 batframes-1.0.0.2/batframe_main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:17:12.203237 batframes-1.0.0.2/batframes.egg-info/
+-rw-rw-rw-   0        0        0      330 2023-05-09 14:17:12.000000 batframes-1.0.0.2/batframes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-05-09 14:17:12.000000 batframes-1.0.0.2/batframes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:17:12.000000 batframes-1.0.0.2/batframes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-09 14:17:12.000000 batframes-1.0.0.2/batframes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      308 2023-05-09 14:17:12.000000 batframes-1.0.0.2/batframes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       77 2023-05-09 14:17:12.000000 batframes-1.0.0.2/batframes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 14:17:12.180232 batframes-1.0.0.2/config/
+drwxrwxrwx   0        0        0        0 2023-05-09 14:17:12.205238 batframes-1.0.0.2/config/DFTrans/
+-rw-rw-rw-   0        0        0   162264 2023-04-18 13:07:06.000000 batframes-1.0.0.2/config/DFTrans/DFTrans_config.json
+drwxrwxrwx   0        0        0        0 2023-05-09 14:17:12.207238 batframes-1.0.0.2/config/batframe/
+-rw-rw-rw-   0        0        0     2816 2023-04-11 01:59:57.000000 batframes-1.0.0.2/config/batframe/bat_tools_config.json
+drwxrwxrwx   0        0        0        0 2023-05-09 14:17:12.215240 batframes-1.0.0.2/config/img/
+-rw-rw-rw-   0        0        0     7631 2023-04-06 08:06:16.000000 batframes-1.0.0.2/config/img/Excel.png
+-rw-rw-rw-   0        0        0     1962 2023-04-06 08:06:16.000000 batframes-1.0.0.2/config/img/excel.gif
+-rw-rw-rw-   0        0        0    10200 2023-04-06 08:06:16.000000 batframes-1.0.0.2/config/img/little_bear.png
+-rw-rw-rw-   0        0        0    42148 2023-03-08 01:46:58.000000 batframes-1.0.0.2/config/img/table_arrow9_transparent_256.png
+-rw-rw-rw-   0        0        0    16958 2023-03-08 01:46:58.000000 batframes-1.0.0.2/config/img/table_arrow9_transparent_64.ico
+-rw-rw-rw-   0        0        0      585 2023-04-08 00:42:18.000000 batframes-1.0.0.2/nuitka_dependency_files.py
+-rw-rw-rw-   0        0        0       42 2023-05-09 14:17:12.218241 batframes-1.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     6956 2023-05-09 14:14:44.000000 batframes-1.0.0.2/setup.py
```

### Comparing `batframes-1.0.0.1/bat_function_call_define.py` & `batframes-1.0.0.2/bat_function_call_define.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/bat_menu_auto.py` & `batframes-1.0.0.2/bat_menu_auto.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/batframe_main.py` & `batframes-1.0.0.2/batframe_main.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/batframes.egg-info/SOURCES.txt` & `batframes-1.0.0.2/batframes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/config/DFTrans/DFTrans_config.json` & `batframes-1.0.0.2/config/DFTrans/DFTrans_config.json`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/config/batframe/bat_tools_config.json` & `batframes-1.0.0.2/config/batframe/bat_tools_config.json`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/config/img/Excel.png` & `batframes-1.0.0.2/config/img/Excel.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/config/img/excel.gif` & `batframes-1.0.0.2/config/img/excel.gif`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/config/img/little_bear.png` & `batframes-1.0.0.2/config/img/little_bear.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/config/img/table_arrow9_transparent_256.png` & `batframes-1.0.0.2/config/img/table_arrow9_transparent_256.png`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/config/img/table_arrow9_transparent_64.ico` & `batframes-1.0.0.2/config/img/table_arrow9_transparent_64.ico`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/nuitka_dependency_files.py` & `batframes-1.0.0.2/nuitka_dependency_files.py`

 * *Files identical despite different names*

### Comparing `batframes-1.0.0.1/setup.py` & `batframes-1.0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 00000b60: 6f6e 6669 6764 6972 2c20 5b6f 7267 696e  onfigdir, [orgin
 00000b70: 636f 6e66 6967 6669 6c65 5d29 2c0d 0a20  configfile]),.. 
 00000b80: 2020 2020 2020 205d 0d0a 2020 2020 7265         ]..    re
 00000b90: 7475 726e 2064 6174 615f 6669 6c65 730d  turn data_files.
 00000ba0: 0a0d 0a0d 0a73 6574 7570 280d 0a20 2020  .....setup(..   
 00000bb0: 206e 616d 653d 2762 6174 6672 616d 6573   name='batframes
 00000bc0: 272c 0d0a 2020 2020 7665 7273 696f 6e3d  ',..    version=
-00000bd0: 2731 2e30 2e30 2e31 272c 0d0a 2020 2020  '1.0.0.1',..    
+00000bd0: 2731 2e30 2e30 2e32 272c 0d0a 2020 2020  '1.0.0.2',..    
 00000be0: 6465 7363 7269 7074 696f 6e3d 27e5 8faf  description='...
 00000bf0: e4bb a5e9 858d e7bd aee5 b086 e5a4 9ae4  ................
 00000c00: b8aa e58f afe6 89a7 e8a1 8ce6 9687 e4bb  ................
 00000c10: b6e5 928c e586 85e9 83a8 e591 bde4 bba4  ................
 00000c20: e4b8 b2e6 8ea5 e688 90e4 b880 e4b8 aae5  ................
 00000c30: ae8c e695 b4e5 91bd e4bb a4e6 89a7 e8a1  ................
 00000c40: 8ce7 9a84 e6a1 86e6 9eb6 e5b7 a5e5 85b7  ................
@@ -206,15 +206,15 @@
 00000cd0: 636b 6167 6573 2829 2c20 2020 2020 2020  ckages(),       
 00000ce0: 2023 20e8 a1a8 e7a4 bae4 bda0 e8a6 81e5   # .............
 00000cf0: b081 e8a3 85e7 9a84 e58c 85ef bc8c 6669  ..............fi
 00000d00: 6e64 5f70 6163 6b61 6765 73e7 94a8 e4ba  nd_packages.....
 00000d10: 8ee7 b3bb e7bb 9fe8 87aa e58a a8e4 bb8e  ................
 00000d20: e5bd 93e5 898d e79b aee5 bd95 e5bc 80e5  ................
 00000d30: a78b e689 bee5 8c85 0d0a 2020 2020 6c69  ..........    li
-00000d40: 6365 6e73 653d 2242 5344 222c 0d0a 2020  cense="BSD",..  
+00000d40: 6365 6e73 653d 224d 4954 222c 0d0a 2020  cense="MIT",..  
 00000d50: 2020 7079 5f6d 6f64 756c 6573 3d5b 2762    py_modules=['b
 00000d60: 6174 6672 616d 655f 6d61 696e 272c 2027  atframe_main', '
 00000d70: 6261 745f 6d65 6e75 5f61 7574 6f27 2c20  bat_menu_auto', 
 00000d80: 2762 6174 5f66 756e 6374 696f 6e5f 6361  'bat_function_ca
 00000d90: 6c6c 5f64 6566 696e 6527 2c20 276e 7569  ll_define', 'nui
 00000da0: 746b 615f 6465 7065 6e64 656e 6379 5f66  tka_dependency_f
 00000db0: 696c 6573 275d 2c0d 0a20 2020 2069 6e73  iles'],..    ins
```

