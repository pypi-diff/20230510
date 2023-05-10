# Comparing `tmp/musegan-0.1.1.tar.gz` & `tmp/musegan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musegan-0.1.1.tar", last modified: Wed May 10 11:57:30 2023, max compression
+gzip compressed data, was "musegan-0.1.2.tar", last modified: Wed May 10 12:15:49 2023, max compression
```

## Comparing `musegan-0.1.1.tar` & `musegan-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:57:30.656185 musegan-0.1.1/
--rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2828 2023-05-10 11:57:30.656185 musegan-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-05-10 06:38:22.000000 musegan-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 11:57:30.624464 musegan-0.1.1/musegan/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:57:30.640159 musegan-0.1.1/musegan/musegan/
--rw-rw-rw-   0        0        0      420 2023-05-08 14:02:00.000000 musegan-0.1.1/musegan/musegan/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-09 08:17:02.000000 musegan-0.1.1/musegan/musegan/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:57:30.656185 musegan-0.1.1/musegan/musegan/archs/
--rw-rw-rw-   0        0        0      376 2023-04-25 08:04:27.000000 musegan-0.1.1/musegan/musegan/archs/__init__.py
--rw-rw-rw-   0        0        0     3686 2023-04-25 08:06:16.000000 musegan-0.1.1/musegan/musegan/archs/bar_generator.py
--rw-rw-rw-   0        0        0     3590 2023-04-25 05:46:28.000000 musegan-0.1.1/musegan/musegan/archs/critic.py
--rw-rw-rw-   0        0        0     3659 2023-04-26 07:29:58.000000 musegan-0.1.1/musegan/musegan/archs/generator.py
--rw-rw-rw-   0        0        0     1909 2023-05-04 06:26:35.000000 musegan-0.1.1/musegan/musegan/archs/temp_network.py
--rw-rw-rw-   0        0        0     1342 2023-04-28 09:57:42.000000 musegan-0.1.1/musegan/musegan/archs/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:57:30.656185 musegan-0.1.1/musegan/musegan/dataset/
--rw-rw-rw-   0        0        0      174 2023-04-28 12:56:56.000000 musegan-0.1.1/musegan/musegan/dataset/__init__.py
--rw-rw-rw-   0        0        0     5443 2023-05-03 06:12:36.000000 musegan-0.1.1/musegan/musegan/dataset/data_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:57:30.656185 musegan-0.1.1/musegan/musegan/trainner/
--rw-rw-rw-   0        0        0      188 2023-04-26 07:13:54.000000 musegan-0.1.1/musegan/musegan/trainner/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-04-25 05:46:28.000000 musegan-0.1.1/musegan/musegan/trainner/criterion.py
--rw-rw-rw-   0        0        0    10398 2023-05-03 11:42:28.000000 musegan-0.1.1/musegan/musegan/trainner/trainer.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:57:30.646671 musegan-0.1.1/musegan/musegan.egg-info/
--rw-rw-rw-   0        0        0     2828 2023-05-10 11:57:30.000000 musegan-0.1.1/musegan/musegan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-05-10 11:57:30.000000 musegan-0.1.1/musegan/musegan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:57:30.000000 musegan-0.1.1/musegan/musegan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 11:57:30.000000 musegan-0.1.1/musegan/musegan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-09 06:31:55.000000 musegan-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      780 2023-05-10 11:57:30.671825 musegan-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 12:15:49.310585 musegan-0.1.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2828 2023-05-10 12:15:49.310585 musegan-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-05-10 06:38:22.000000 musegan-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 12:15:49.264040 musegan-0.1.2/musegan/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:15:49.278800 musegan-0.1.2/musegan/musegan/
+-rw-rw-rw-   0        0        0      420 2023-05-08 14:02:00.000000 musegan-0.1.2/musegan/musegan/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-09 08:17:02.000000 musegan-0.1.2/musegan/musegan/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:15:49.299029 musegan-0.1.2/musegan/musegan/archs/
+-rw-rw-rw-   0        0        0      376 2023-04-25 08:04:27.000000 musegan-0.1.2/musegan/musegan/archs/__init__.py
+-rw-rw-rw-   0        0        0     3686 2023-04-25 08:06:16.000000 musegan-0.1.2/musegan/musegan/archs/bar_generator.py
+-rw-rw-rw-   0        0        0     3590 2023-04-25 05:46:28.000000 musegan-0.1.2/musegan/musegan/archs/critic.py
+-rw-rw-rw-   0        0        0     3659 2023-04-26 07:29:58.000000 musegan-0.1.2/musegan/musegan/archs/generator.py
+-rw-rw-rw-   0        0        0     1909 2023-05-04 06:26:35.000000 musegan-0.1.2/musegan/musegan/archs/temp_network.py
+-rw-rw-rw-   0        0        0     1342 2023-04-28 09:57:42.000000 musegan-0.1.2/musegan/musegan/archs/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:15:49.303058 musegan-0.1.2/musegan/musegan/dataset/
+-rw-rw-rw-   0        0        0      174 2023-04-28 12:56:56.000000 musegan-0.1.2/musegan/musegan/dataset/__init__.py
+-rw-rw-rw-   0        0        0     5443 2023-05-03 06:12:36.000000 musegan-0.1.2/musegan/musegan/dataset/data_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:15:49.308544 musegan-0.1.2/musegan/musegan/trainner/
+-rw-rw-rw-   0        0        0      188 2023-04-26 07:13:54.000000 musegan-0.1.2/musegan/musegan/trainner/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-04-25 05:46:28.000000 musegan-0.1.2/musegan/musegan/trainner/criterion.py
+-rw-rw-rw-   0        0        0    10398 2023-05-03 11:42:28.000000 musegan-0.1.2/musegan/musegan/trainner/trainer.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:15:49.287326 musegan-0.1.2/musegan/musegan.egg-info/
+-rw-rw-rw-   0        0        0     2828 2023-05-10 12:15:49.000000 musegan-0.1.2/musegan/musegan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-05-10 12:15:49.000000 musegan-0.1.2/musegan/musegan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:15:49.000000 musegan-0.1.2/musegan/musegan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 12:15:49.000000 musegan-0.1.2/musegan/musegan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-09 06:31:55.000000 musegan-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      775 2023-05-10 12:15:49.312544 musegan-0.1.2/setup.cfg
```

### Comparing `musegan-0.1.1/LICENSE` & `musegan-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/PKG-INFO` & `musegan-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pytorch implementation of musegan
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `musegan-0.1.1/README.md` & `musegan-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan/archs/bar_generator.py` & `musegan-0.1.2/musegan/musegan/archs/bar_generator.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan/archs/critic.py` & `musegan-0.1.2/musegan/musegan/archs/critic.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan/archs/generator.py` & `musegan-0.1.2/musegan/musegan/archs/generator.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan/archs/temp_network.py` & `musegan-0.1.2/musegan/musegan/archs/temp_network.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan/archs/utils.py` & `musegan-0.1.2/musegan/musegan/archs/utils.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan/dataset/data_utils.py` & `musegan-0.1.2/musegan/musegan/dataset/data_utils.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan/trainner/criterion.py` & `musegan-0.1.2/musegan/musegan/trainner/criterion.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan/trainner/trainer.py` & `musegan-0.1.2/musegan/musegan/trainner/trainer.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/musegan/musegan.egg-info/PKG-INFO` & `musegan-0.1.2/musegan/musegan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.1.1
+Version: 0.1.2
 Summary: A pytorch implementation of musegan
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `musegan-0.1.1/musegan/musegan.egg-info/SOURCES.txt` & `musegan-0.1.2/musegan/musegan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musegan-0.1.1/setup.cfg` & `musegan-0.1.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7573 6567 616e 0d0a 7665 7273   = musegan..vers
-00000020: 696f 6e20 3d20 302e 312e 310d 0a61 7574  ion = 0.1.1..aut
+00000020: 696f 6e20 3d20 302e 312e 320d 0a61 7574  ion = 0.1.2..aut
 00000030: 686f 7220 3d20 436c 6966 666f 7264 204e  hor = Clifford N
 00000040: 6a6f 726f 6765 0d0a 6175 7468 6f72 5f65  joroge..author_e
 00000050: 6d61 696c 203d 2063 6e6a 6f72 6f67 6540  mail = cnjoroge@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 2070 7974 6f72  iption = A pytor
 00000080: 6368 2069 6d70 6c65 6d65 6e74 6174 696f  ch implementatio
 00000090: 6e20 6f66 206d 7573 6567 616e 0d0a 6c6f  n of musegan..lo
@@ -14,36 +14,36 @@
 000000d0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 000000e0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
 000000f0: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
 00000100: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000110: 7562 2e63 6f6d 2f63 6c69 6666 6f72 646b  ub.com/cliffordk
 00000120: 6c65 696e 7372 2f6d 7573 6567 616e 2d70  leinsr/musegan-p
 00000130: 7974 6f72 6368 0d0a 696e 7374 616c 6c5f  ytorch..install_
-00000140: 7265 7175 6972 6573 203d 205b 0d0a 096d  requires = [...m
-00000150: 7573 6963 3231 0d0a 096e 756d 7079 0d0a  usic21...numpy..
-00000160: 095d 0d0a 636c 6173 7369 6669 6572 7320  .]..classifiers 
-00000170: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
-00000180: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000190: 686f 6e20 3a3a 2033 0d0a 0950 726f 6772  hon :: 3...Progr
-000001a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
-000001c0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000001d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001e0: 6e20 3a3a 2033 2e38 0d0a 0950 726f 6772  n :: 3.8...Progr
-000001f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000200: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-00000210: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000220: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000230: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-00000240: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000250: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-00000260: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
-00000270: 6b61 6765 5f64 6972 203d 200d 0a09 3d20  kage_dir = ...= 
-00000280: 6d75 7365 6761 6e0d 0a70 6163 6b61 6765  musegan..package
-00000290: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-000002a0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000002b0: 2e39 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .9....[options.p
-000002c0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-000002d0: 6865 7265 203d 206d 7573 6567 616e 0d0a  here = musegan..
-000002e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000300: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000140: 7265 7175 6972 6573 203d 200d 0a09 6d75  requires = ...mu
+00000150: 7369 6332 310d 0a09 6e75 6d70 790d 0a63  sic21...numpy..c
+00000160: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+00000170: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000180: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000190: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
+000001a0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001b0: 7468 6f6e 203a 3a20 332e 370d 0a09 5072  thon :: 3.7...Pr
+000001c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001e0: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
+000001f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000200: 7468 6f6e 203a 3a20 332e 390d 0a09 4c69  thon :: 3.9...Li
+00000210: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000220: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
+00000230: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
+00000240: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
+00000250: 6465 7065 6e64 656e 740d 0a0d 0a5b 6f70  dependent....[op
+00000260: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
+00000270: 6469 7220 3d20 0d0a 093d 206d 7573 6567  dir = ...= museg
+00000280: 616e 0d0a 7061 636b 6167 6573 203d 2066  an..packages = f
+00000290: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
+000002a0: 7569 7265 7320 3d20 3e3d 332e 390d 0a0d  uires = >=3.9...
+000002b0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+000002c0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+000002d0: 3d20 6d75 7365 6761 6e0d 0a0d 0a5b 6567  = musegan....[eg
+000002e0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000002f0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000300: 3d20 300d 0a0d 0a                        = 0....
```

