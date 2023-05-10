# Comparing `tmp/pytextclassifier-1.3.5.tar.gz` & `tmp/pytextclassifier-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytextclassifier-1.3.5.tar", last modified: Mon Apr  3 12:39:16 2023, max compression
+gzip compressed data, was "pytextclassifier-1.3.6.tar", last modified: Wed May 10 03:36:52 2023, max compression
```

## Comparing `pytextclassifier-1.3.5.tar` & `pytextclassifier-1.3.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-03 12:39:16.051075 pytextclassifier-1.3.5/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:50.000000 pytextclassifier-1.3.5/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    26374 2023-04-03 12:39:16.051595 pytextclassifier-1.3.5/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    21249 2023-01-03 08:17:05.000000 pytextclassifier-1.3.5/README.md
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-03 12:39:16.046539 pytextclassifier-1.3.5/examples/
--rw-r--r--   0 xuming     (501) staff       (20)   616465 2022-03-29 07:45:47.000000 pytextclassifier-1.3.5/examples/thucnews_train_1w.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-03 12:39:16.042865 pytextclassifier-1.3.5/pytextclassifier/
--rw-r--r--   0 xuming     (501) staff       (20)      640 2023-04-03 12:38:48.000000 pytextclassifier-1.3.5/pytextclassifier/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     2467 2022-12-27 14:58:33.000000 pytextclassifier-1.3.5/pytextclassifier/base_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    39046 2023-03-02 03:38:43.000000 pytextclassifier-1.3.5/pytextclassifier/bert_classfication_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    87482 2023-04-03 12:04:45.000000 pytextclassifier-1.3.5/pytextclassifier/bert_classification_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10856 2022-12-28 09:00:19.000000 pytextclassifier-1.3.5/pytextclassifier/bert_classifier.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    30020 2023-01-06 02:12:44.000000 pytextclassifier-1.3.5/pytextclassifier/bert_multi_label_classification_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10789 2022-12-27 15:02:35.000000 pytextclassifier-1.3.5/pytextclassifier/classic_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)     1329 2022-04-12 03:46:17.000000 pytextclassifier-1.3.5/pytextclassifier/data_helper.py
--rw-r--r--   0 xuming     (501) staff       (20)    21016 2022-12-27 15:02:35.000000 pytextclassifier-1.3.5/pytextclassifier/fasttext_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 pytextclassifier-1.3.5/pytextclassifier/stopwords.txt
--rw-r--r--   0 xuming     (501) staff       (20)     7245 2022-04-12 07:49:32.000000 pytextclassifier-1.3.5/pytextclassifier/textcluster.py
--rw-r--r--   0 xuming     (501) staff       (20)    18971 2022-12-27 15:02:35.000000 pytextclassifier-1.3.5/pytextclassifier/textcnn_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)    19431 2022-12-27 15:02:35.000000 pytextclassifier-1.3.5/pytextclassifier/textrnn_classifier.py
--rw-r--r--   0 xuming     (501) staff       (20)      852 2022-04-12 06:51:36.000000 pytextclassifier-1.3.5/pytextclassifier/time_util.py
--rw-r--r--   0 xuming     (501) staff       (20)     2330 2022-11-25 09:11:54.000000 pytextclassifier-1.3.5/pytextclassifier/tokenizer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-03 12:39:16.046143 pytextclassifier-1.3.5/pytextclassifier.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    26374 2023-04-03 12:39:15.000000 pytextclassifier-1.3.5/pytextclassifier.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      848 2023-04-03 12:39:15.000000 pytextclassifier-1.3.5/pytextclassifier.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-03 12:39:15.000000 pytextclassifier-1.3.5/pytextclassifier.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)       52 2023-04-03 12:39:15.000000 pytextclassifier-1.3.5/pytextclassifier.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       17 2023-04-03 12:39:15.000000 pytextclassifier-1.3.5/pytextclassifier.egg-info/top_level.txt
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-03 12:39:16.052621 pytextclassifier-1.3.5/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1444 2023-04-03 12:38:48.000000 pytextclassifier-1.3.5/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-10 03:36:52.892834 pytextclassifier-1.3.6/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:50.000000 pytextclassifier-1.3.6/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    27150 2023-05-10 03:36:52.893785 pytextclassifier-1.3.6/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    21977 2023-05-09 09:17:58.000000 pytextclassifier-1.3.6/README.md
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-10 03:36:52.885107 pytextclassifier-1.3.6/examples/
+-rw-r--r--   0 xuming     (501) staff       (20)   616465 2022-03-29 07:45:47.000000 pytextclassifier-1.3.6/examples/thucnews_train_1w.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-10 03:36:52.880046 pytextclassifier-1.3.6/pytextclassifier/
+-rw-r--r--   0 xuming     (501) staff       (20)      640 2023-05-09 08:59:46.000000 pytextclassifier-1.3.6/pytextclassifier/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2467 2022-12-27 14:58:33.000000 pytextclassifier-1.3.6/pytextclassifier/base_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    39043 2023-05-09 08:58:29.000000 pytextclassifier-1.3.6/pytextclassifier/bert_classfication_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    87482 2023-04-03 12:04:45.000000 pytextclassifier-1.3.6/pytextclassifier/bert_classification_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    11106 2023-05-09 08:58:29.000000 pytextclassifier-1.3.6/pytextclassifier/bert_classifier.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    29987 2023-05-09 08:58:29.000000 pytextclassifier-1.3.6/pytextclassifier/bert_multi_label_classification_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10892 2023-05-09 08:47:54.000000 pytextclassifier-1.3.6/pytextclassifier/classic_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1329 2022-04-12 03:46:17.000000 pytextclassifier-1.3.6/pytextclassifier/data_helper.py
+-rw-r--r--   0 xuming     (501) staff       (20)    21111 2023-05-09 08:44:44.000000 pytextclassifier-1.3.6/pytextclassifier/fasttext_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 pytextclassifier-1.3.6/pytextclassifier/stopwords.txt
+-rw-r--r--   0 xuming     (501) staff       (20)     7304 2023-05-09 08:44:44.000000 pytextclassifier-1.3.6/pytextclassifier/textcluster.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18996 2023-05-09 08:42:39.000000 pytextclassifier-1.3.6/pytextclassifier/textcnn_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19633 2023-05-09 08:42:39.000000 pytextclassifier-1.3.6/pytextclassifier/textrnn_classifier.py
+-rw-r--r--   0 xuming     (501) staff       (20)      852 2022-04-12 06:51:36.000000 pytextclassifier-1.3.6/pytextclassifier/time_util.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2330 2022-11-25 09:11:54.000000 pytextclassifier-1.3.6/pytextclassifier/tokenizer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-10 03:36:52.884399 pytextclassifier-1.3.6/pytextclassifier.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    27150 2023-05-10 03:36:52.000000 pytextclassifier-1.3.6/pytextclassifier.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      848 2023-05-10 03:36:52.000000 pytextclassifier-1.3.6/pytextclassifier.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-05-10 03:36:52.000000 pytextclassifier-1.3.6/pytextclassifier.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       52 2023-05-10 03:36:52.000000 pytextclassifier-1.3.6/pytextclassifier.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       17 2023-05-10 03:36:52.000000 pytextclassifier-1.3.6/pytextclassifier.egg-info/top_level.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-05-10 03:36:52.895355 pytextclassifier-1.3.6/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1444 2023-05-09 08:59:46.000000 pytextclassifier-1.3.6/setup.py
```

### Comparing `pytextclassifier-1.3.5/LICENSE` & `pytextclassifier-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/PKG-INFO` & `pytextclassifier-1.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,1649 +1,1697 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7465  : 2.1.Name: pyte
 00000020: 7874 636c 6173 7369 6669 6572 0a56 6572  xtclassifier.Ver
-00000030: 7369 6f6e 3a20 312e 332e 350a 5375 6d6d  sion: 1.3.5.Summ
+00000030: 7369 6f6e 3a20 312e 332e 360a 5375 6d6d  sion: 1.3.6.Summ
 00000040: 6172 793a 2054 6578 7420 436c 6173 7369  ary: Text Classi
 00000050: 6669 6572 2c20 5465 7874 2043 6c61 7373  fier, Text Class
 00000060: 6966 6963 6174 696f 6e0a 486f 6d65 2d70  ification.Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
 00000090: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
 000000a0: 6965 720a 4175 7468 6f72 3a20 5875 4d69  ier.Author: XuMi
 000000b0: 6e67 0a41 7574 686f 722d 656d 6169 6c3a  ng.Author-email:
 000000c0: 2078 756d 696e 6736 3234 4071 712e 636f   xuming624@qq.co
 000000d0: 6d0a 4c69 6365 6e73 653a 2041 7061 6368  m.License: Apach
 000000e0: 6520 322e 300a 4465 7363 7269 7074 696f  e 2.0.Descriptio
-000000f0: 6e3a 205b 215b 5079 5049 2076 6572 7369  n: [![PyPI versi
-00000100: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
-00000110: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
-00000120: 6578 7463 6c61 7373 6966 6965 722e 7376  extclassifier.sv
-00000130: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
-00000140: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
-00000150: 6578 7463 6c61 7373 6966 6965 7229 0a20  extclassifier). 
-00000160: 2020 2020 2020 205b 215b 446f 776e 6c6f         [![Downlo
-00000170: 6164 735d 2868 7474 7073 3a2f 2f70 6570  ads](https://pep
-00000180: 792e 7465 6368 2f62 6164 6765 2f70 7974  y.tech/badge/pyt
-00000190: 6578 7463 6c61 7373 6966 6965 7229 5d28  extclassifier)](
-000001a0: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
-000001b0: 682f 7072 6f6a 6563 742f 7079 7465 7874  h/project/pytext
-000001c0: 636c 6173 7369 6669 6572 290a 2020 2020  classifier).    
-000001d0: 2020 2020 5b21 5b43 6f6e 7472 6962 7574      [![Contribut
-000001e0: 696f 6e73 2077 656c 636f 6d65 5d28 6874  ions welcome](ht
-000001f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000200: 732e 696f 2f62 6164 6765 2f63 6f6e 7472  s.io/badge/contr
-00000210: 6962 7574 696f 6e73 2d77 656c 636f 6d65  ibutions-welcome
-00000220: 2d62 7269 6768 7467 7265 656e 2e73 7667  -brightgreen.svg
-00000230: 295d 2843 4f4e 5452 4942 5554 494e 472e  )](CONTRIBUTING.
-00000240: 6d64 290a 2020 2020 2020 2020 5b21 5b47  md).        [![G
-00000250: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
-00000260: 7273 5d28 6874 7470 733a 2f2f 696d 672e  rs](https://img.
-00000270: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000280: 622f 636f 6e74 7269 6275 746f 7273 2f73  b/contributors/s
-00000290: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
-000002a0: 636c 6173 7369 6669 6572 2e73 7667 295d  classifier.svg)]
-000002b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000002c0: 636f 6d2f 7368 6962 696e 6736 3234 2f70  com/shibing624/p
-000002d0: 7974 6578 7463 6c61 7373 6966 6965 722f  ytextclassifier/
-000002e0: 6772 6170 6873 2f63 6f6e 7472 6962 7574  graphs/contribut
-000002f0: 6f72 7329 0a20 2020 2020 2020 205b 215b  ors).        [![
-00000300: 4c69 6365 6e73 6520 4170 6163 6865 2032  License Apache 2
-00000310: 2e30 5d28 6874 7470 733a 2f2f 696d 672e  .0](https://img.
-00000320: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000330: 2f6c 6963 656e 7365 2d41 7061 6368 6525  /license-Apache%
-00000340: 3230 322e 302d 626c 7565 2e73 7667 295d  202.0-blue.svg)]
-00000350: 284c 4943 454e 5345 290a 2020 2020 2020  (LICENSE).      
-00000360: 2020 5b21 5b70 7974 686f 6e5f 7665 7369    [![python_vesi
-00000370: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-00000380: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000390: 2f50 7974 686f 6e2d 332e 3525 3242 2d67  /Python-3.5%2B-g
-000003a0: 7265 656e 2e73 7667 295d 2872 6571 7569  reen.svg)](requi
-000003b0: 7265 6d65 6e74 732e 7478 7429 0a20 2020  rements.txt).   
-000003c0: 2020 2020 205b 215b 4769 7448 7562 2069       [![GitHub i
-000003d0: 7373 7565 735d 2868 7474 7073 3a2f 2f69  ssues](https://i
-000003e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-000003f0: 7468 7562 2f69 7373 7565 732f 7368 6962  thub/issues/shib
-00000400: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
-00000410: 7373 6966 6965 722e 7376 6729 5d28 6874  ssifier.svg)](ht
-00000420: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000430: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
-00000440: 7874 636c 6173 7369 6669 6572 2f69 7373  xtclassifier/iss
-00000450: 7565 7329 0a20 2020 2020 2020 205b 215b  ues).        [![
-00000460: 5765 6368 6174 2047 726f 7570 5d28 6874  Wechat Group](ht
-00000470: 7470 3a2f 2f76 6c6f 672e 7366 7963 2e6c  tp://vlog.sfyc.l
-00000480: 7464 2f77 6563 6861 745f 6576 6572 7964  td/wechat_everyd
-00000490: 6179 2f77 7867 726f 7570 5f6c 6f67 6f2e  ay/wxgroup_logo.
-000004a0: 706e 673f 696d 6167 6556 6965 7732 2f30  png?imageView2/0
-000004b0: 2f77 2f36 302f 682f 3230 295d 2823 436f  /w/60/h/20)](#Co
-000004c0: 6e74 6163 7429 0a20 2020 2020 2020 200a  ntact).        .
-000004d0: 2020 2020 2020 2020 2320 5079 5465 7874          # PyText
-000004e0: 436c 6173 7369 6669 6572 0a20 2020 2020  Classifier.     
-000004f0: 2020 2050 7954 6578 7443 6c61 7373 6966     PyTextClassif
-00000500: 6965 722c 2050 7974 686f 6e20 5465 7874  ier, Python Text
-00000510: 2043 6c61 7373 6966 6965 722e 2049 7420   Classifier. It 
-00000520: 6361 6e20 6265 2061 7070 6c69 6564 2074  can be applied t
-00000530: 6f20 7468 6520 6669 656c 6473 206f 6620  o the fields of 
-00000540: 7365 6e74 696d 656e 7420 706f 6c61 7269  sentiment polari
-00000550: 7479 2061 6e61 6c79 7369 732c 2074 6578  ty analysis, tex
-00000560: 7420 7269 736b 2063 6c61 7373 6966 6963  t risk classific
-00000570: 6174 696f 6e20 616e 6420 736f 206f 6e2c  ation and so on,
-00000580: 0a20 2020 2020 2020 2061 6e64 2069 7420  .        and it 
-00000590: 7375 7070 6f72 7473 206d 756c 7469 706c  supports multipl
-000005a0: 6520 636c 6173 7369 6669 6361 7469 6f6e  e classification
-000005b0: 2061 6c67 6f72 6974 686d 7320 616e 6420   algorithms and 
-000005c0: 636c 7573 7465 7269 6e67 2061 6c67 6f72  clustering algor
-000005d0: 6974 686d 732e 0a20 2020 2020 2020 200a  ithms..        .
-000005e0: 2020 2020 2020 2020 e696 87e6 9cac e588          ........
-000005f0: 86e7 b1bb e599 a8ef bc8c e68f 90e4 be9b  ................
-00000600: e5a4 9ae7 a78d e696 87e6 9cac e588 86e7  ................
-00000610: b1bb e592 8ce8 819a e7b1 bbe7 ae97 e6b3  ................
-00000620: 95ef bc8c e694 afe6 8c81 e58f a5e5 ad90  ................
-00000630: e592 8ce6 9687 e6a1 a3e7 baa7 e79a 84e6  ................
-00000640: 9687 e69c ace5 8886 e7b1 bbe4 bbbb e58a  ................
-00000650: a1ef bc8c e694 afe6 8c81 e4ba 8ce5 8886  ................
-00000660: e7b1 bbe3 8081 e5a4 9ae5 8886 e7b1 bbe3  ................
-00000670: 8081 e5a4 9ae6 a087 e7ad bee5 8886 e7b1  ................
-00000680: bbe3 8081 e5a4 9ae5 b182 e7ba a7e5 8886  ................
-00000690: e7b1 bbe5 928c 4b6d 6561 6e73 e881 9ae7  ......Kmeans....
-000006a0: b1bb efbc 8ce5 bc80 e7ae b1e5 8db3 e794  ................
-000006b0: a8e3 8082 7079 7468 6f6e 33e5 bc80 e58f  ....python3.....
-000006c0: 91e3 8082 0a20 2020 2020 2020 200a 2020  .....        .  
-000006d0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-000006e0: 2a47 7569 6465 2a2a 0a20 2020 2020 2020  *Guide**.       
-000006f0: 200a 2020 2020 2020 2020 2d20 5b46 6561   .        - [Fea
-00000700: 7475 7265 5d28 2346 6561 7475 7265 290a  ture](#Feature).
-00000710: 2020 2020 2020 2020 2d20 5b49 6e73 7461          - [Insta
-00000720: 6c6c 5d28 2369 6e73 7461 6c6c 290a 2020  ll](#install).  
-00000730: 2020 2020 2020 2d20 5b55 7361 6765 5d28        - [Usage](
-00000740: 2375 7361 6765 290a 2020 2020 2020 2020  #usage).        
-00000750: 2d20 5b44 6174 6173 6574 5d28 2344 6174  - [Dataset](#Dat
-00000760: 6173 6574 290a 2020 2020 2020 2020 2d20  aset).        - 
-00000770: 5b43 6f6e 7461 6374 5d28 2343 6f6e 7461  [Contact](#Conta
-00000780: 6374 290a 2020 2020 2020 2020 2d20 5b43  ct).        - [C
-00000790: 6974 6174 696f 6e5d 2823 4369 7461 7469  itation](#Citati
-000007a0: 6f6e 290a 2020 2020 2020 2020 2d20 5b52  on).        - [R
-000007b0: 6566 6572 656e 6365 5d28 2372 6566 6572  eference](#refer
-000007c0: 656e 6365 290a 2020 2020 2020 2020 0a20  ence).        . 
-000007d0: 2020 2020 2020 2023 2046 6561 7475 7265         # Feature
-000007e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000007f0: 2020 2a2a 7079 7465 7874 636c 6173 7369    **pytextclassi
-00000800: 6669 6572 2a2a 2069 7320 6120 7079 7468  fier** is a pyth
-00000810: 6f6e 204f 7065 6e20 536f 7572 6365 2054  on Open Source T
-00000820: 6f6f 6c6b 6974 2066 6f72 2074 6578 7420  oolkit for text 
-00000830: 636c 6173 7369 6669 6361 7469 6f6e 2e20  classification. 
-00000840: 5468 6520 676f 616c 2069 7320 746f 2069  The goal is to i
-00000850: 6d70 6c65 6d65 6e74 0a20 2020 2020 2020  mplement.       
-00000860: 2074 6578 7420 616e 616c 7973 6973 2061   text analysis a
-00000870: 6c67 6f72 6974 686d 2c20 736f 2061 7320  lgorithm, so as 
-00000880: 746f 2061 6368 6965 7665 2074 6865 2075  to achieve the u
-00000890: 7365 2069 6e20 7468 6520 7072 6f64 7563  se in the produc
-000008a0: 7469 6f6e 2065 6e76 6972 6f6e 6d65 6e74  tion environment
-000008b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000008c0: 2020 202a 2a70 7974 6578 7463 6c61 7373     **pytextclass
-000008d0: 6966 6965 722a 2a20 6861 7320 7468 6520  ifier** has the 
-000008e0: 6368 6172 6163 7465 7269 7374 6963 730a  characteristics.
-000008f0: 2020 2020 2020 2020 6f66 2063 6c65 6172          of clear
-00000900: 2061 6c67 6f72 6974 686d 2c20 6869 6768   algorithm, high
-00000910: 2070 6572 666f 726d 616e 6365 2061 6e64   performance and
-00000920: 2063 7573 746f 6d69 7a61 626c 6520 636f   customizable co
-00000930: 7270 7573 2e0a 2020 2020 2020 2020 0a20  rpus..        . 
-00000940: 2020 2020 2020 2046 756e 6374 696f 6e73         Functions
-00000950: efbc 9a0a 2020 2020 2020 2020 2323 2320  ....        ### 
-00000960: 436c 6173 7369 6669 6572 0a20 2020 2020  Classifier.     
-00000970: 2020 2020 202d 205b 785d 204c 6f67 6973       - [x] Logis
-00000980: 7469 6352 6567 7265 7373 696f 6e0a 2020  ticRegression.  
-00000990: 2020 2020 2020 2020 2d20 5b78 5d20 5261          - [x] Ra
-000009a0: 6e64 6f6d 2046 6f72 6573 740a 2020 2020  ndom Forest.    
-000009b0: 2020 2020 2020 2d20 5b78 5d20 4465 6369        - [x] Deci
-000009c0: 7369 6f6e 2054 7265 650a 2020 2020 2020  sion Tree.      
-000009d0: 2020 2020 2d20 5b78 5d20 4b2d 4e65 6172      - [x] K-Near
-000009e0: 6573 7420 4e65 6967 6862 6f75 7273 0a20  est Neighbours. 
-000009f0: 2020 2020 2020 2020 202d 205b 785d 204e           - [x] N
-00000a00: 6169 7665 2062 6179 6573 0a20 2020 2020  aive bayes.     
-00000a10: 2020 2020 202d 205b 785d 2058 6762 6f6f       - [x] Xgboo
-00000a20: 7374 0a20 2020 2020 2020 2020 202d 205b  st.          - [
-00000a30: 785d 2053 7570 706f 7274 2056 6563 746f  x] Support Vecto
-00000a40: 7220 4d61 6368 696e 6528 5356 4d29 0a20  r Machine(SVM). 
-00000a50: 2020 2020 2020 2020 202d 205b 785d 2054           - [x] T
-00000a60: 6578 7443 4e4e 0a20 2020 2020 2020 2020  extCNN.         
-00000a70: 202d 205b 785d 2054 6578 7452 4e4e 0a20   - [x] TextRNN. 
-00000a80: 2020 2020 2020 2020 202d 205b 785d 2046           - [x] F
-00000a90: 6173 7474 6578 740a 2020 2020 2020 2020  asttext.        
-00000aa0: 2020 2d20 5b78 5d20 4245 5254 0a20 2020    - [x] BERT.   
-00000ab0: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000ac0: 2320 436c 7573 7465 720a 2020 2020 2020  # Cluster.      
-00000ad0: 2020 2020 2d20 5b78 5d20 4d69 6e69 4261      - [x] MiniBa
-00000ae0: 7463 684b 6d65 616e 730a 2020 2020 2020  tchKmeans.      
-00000af0: 2020 0a20 2020 2020 2020 2057 6869 6c65    .        While
-00000b00: 2070 726f 7669 6469 6e67 2072 6963 6820   providing rich 
-00000b10: 6675 6e63 7469 6f6e 732c 202a 2a70 7974  functions, **pyt
-00000b20: 6578 7463 6c61 7373 6966 6965 722a 2a20  extclassifier** 
-00000b30: 696e 7465 726e 616c 206d 6f64 756c 6573  internal modules
-00000b40: 2061 6468 6572 6520 746f 206c 6f77 2063   adhere to low c
-00000b50: 6f75 706c 696e 672c 206d 6f64 656c 2061  oupling, model a
-00000b60: 6468 6572 656e 6365 2074 6f20 696e 6572  dherence to iner
-00000b70: 7420 6c6f 6164 696e 672c 2064 6963 7469  t loading, dicti
-00000b80: 6f6e 6172 7920 7075 626c 6963 6174 696f  onary publicatio
-00000b90: 6e2c 2061 6e64 2065 6173 7920 746f 2075  n, and easy to u
-00000ba0: 7365 2e0a 2020 2020 2020 2020 0a20 2020  se..        .   
-00000bb0: 2020 2020 2023 2049 6e73 7461 6c6c 0a20       # Install. 
-00000bc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000bd0: 2d20 5265 7175 6972 656d 656e 7473 2061  - Requirements a
-00000be0: 6e64 2049 6e73 7461 6c6c 6174 696f 6e0a  nd Installation.
-00000bf0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000c00: 2060 6060 0a20 2020 2020 2020 2070 6970   ```.        pip
-00000c10: 3320 696e 7374 616c 6c20 746f 7263 6820  3 install torch 
-00000c20: 2320 636f 6e64 6120 696e 7374 616c 6c20  # conda install 
-00000c30: 7079 746f 7263 680a 2020 2020 2020 2020  pytorch.        
-00000c40: 7069 7033 2069 6e73 7461 6c6c 2070 7974  pip3 install pyt
-00000c50: 6578 7463 6c61 7373 6966 6965 720a 2020  extclassifier.  
-00000c60: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00000c70: 2020 0a20 2020 2020 2020 206f 720a 2020    .        or.  
-00000c80: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
-00000c90: 6060 0a20 2020 2020 2020 2067 6974 2063  ``.        git c
-00000ca0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-00000cb0: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
-00000cc0: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
-00000cd0: 6965 722e 6769 740a 2020 2020 2020 2020  ier.git.        
-00000ce0: 6364 2070 7974 6578 7463 6c61 7373 6966  cd pytextclassif
-00000cf0: 6965 720a 2020 2020 2020 2020 7079 7468  ier.        pyth
-00000d00: 6f6e 3320 7365 7475 702e 7079 2069 6e73  on3 setup.py ins
-00000d10: 7461 6c6c 0a20 2020 2020 2020 2060 6060  tall.        ```
-00000d20: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000d30: 2020 0a20 2020 2020 2020 2023 2055 7361    .        # Usa
-00000d40: 6765 0a20 2020 2020 2020 2023 2054 6578  ge.        # Tex
-00000d50: 7420 436c 6173 7369 6669 6572 0a20 2020  t Classifier.   
-00000d60: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000d70: 2045 6e67 6c69 7368 2054 6578 7420 436c   English Text Cl
-00000d80: 6173 7369 6669 6572 0a20 2020 2020 2020  assifier.       
-00000d90: 200a 2020 2020 2020 2020 496e 636c 7564   .        Includ
-00000da0: 696e 6720 6d6f 6465 6c20 7472 6169 6e69  ing model traini
-00000db0: 6e67 2c20 7361 7669 6e67 2c20 7072 6564  ng, saving, pred
-00000dc0: 6963 742c 2065 7661 6c75 6174 652c 2066  ict, evaluate, f
-00000dd0: 6f72 2065 7861 6d70 6c65 205b 6578 616d  or example [exam
-00000de0: 706c 6573 2f6c 725f 656e 5f63 6c61 7373  ples/lr_en_class
-00000df0: 6966 6963 6174 696f 6e5f 6465 6d6f 2e70  ification_demo.p
-00000e00: 795d 2865 7861 6d70 6c65 732f 6c72 5f65  y](examples/lr_e
-00000e10: 6e5f 636c 6173 7369 6669 6361 7469 6f6e  n_classification
-00000e20: 5f64 656d 6f2e 7079 293a 0a20 2020 2020  _demo.py):.     
-00000e30: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00000e40: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00000e50: 2020 2020 2020 2069 6d70 6f72 7420 7379         import sy
-00000e60: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-00000e70: 2020 2073 7973 2e70 6174 682e 6170 7065     sys.path.appe
-00000e80: 6e64 2827 2e2e 2729 0a20 2020 2020 2020  nd('..').       
-00000e90: 2066 726f 6d20 7079 7465 7874 636c 6173   from pytextclas
-00000ea0: 7369 6669 6572 2069 6d70 6f72 7420 436c  sifier import Cl
-00000eb0: 6173 7369 6343 6c61 7373 6966 6965 720a  assicClassifier.
-00000ec0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000ed0: 2069 6620 5f5f 6e61 6d65 5f5f 203d 3d20   if __name__ == 
-00000ee0: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
-00000ef0: 2020 2020 2020 2020 6d20 3d20 436c 6173          m = Clas
-00000f00: 7369 6343 6c61 7373 6966 6965 7228 6d6f  sicClassifier(mo
-00000f10: 6465 6c5f 6469 723d 276d 6f64 656c 732f  del_dir='models/
-00000f20: 6c72 272c 206d 6f64 656c 5f6e 616d 655f  lr', model_name_
-00000f30: 6f72 5f6d 6f64 656c 3d27 6c72 2729 0a20  or_model='lr'). 
-00000f40: 2020 2020 2020 2020 2020 2023 2043 6c61             # Cla
-00000f50: 7373 6963 436c 6173 7369 6669 6572 2073  ssicClassifier s
-00000f60: 7570 706f 7274 206d 6f64 656c 5f6e 616d  upport model_nam
-00000f70: 65ef bc9a 6c72 2c20 7261 6e64 6f6d 5f66  e...lr, random_f
-00000f80: 6f72 6573 742c 2064 6563 6973 696f 6e5f  orest, decision_
-00000f90: 7472 6565 2c20 6b6e 6e2c 2062 6179 6573  tree, knn, bayes
-00000fa0: 2c20 7376 6d2c 2078 6762 6f6f 7374 0a20  , svm, xgboost. 
-00000fb0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00000fc0: 286d 290a 2020 2020 2020 2020 2020 2020  (m).            
-00000fd0: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00000fe0: 2020 2020 2020 2020 2028 2765 6475 6361           ('educa
-00000ff0: 7469 6f6e 272c 2027 5374 7564 656e 7420  tion', 'Student 
-00001000: 6465 6274 2074 6f20 636f 7374 2042 7269  debt to cost Bri
-00001010: 7461 696e 2062 696c 6c69 6f6e 7320 7769  tain billions wi
-00001020: 7468 696e 2064 6563 6164 6573 2729 2c0a  thin decades'),.
-00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001040: 2827 6564 7563 6174 696f 6e27 2c20 2743  ('education', 'C
-00001050: 6869 6e65 7365 2065 6475 6361 7469 6f6e  hinese education
-00001060: 2066 6f72 2054 5620 6578 7065 7269 6d65   for TV experime
-00001070: 6e74 2729 2c0a 2020 2020 2020 2020 2020  nt'),.          
-00001080: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00001090: 2027 4d69 6464 6c65 2045 6173 7420 616e   'Middle East an
-000010a0: 6420 4173 6961 2062 6f6f 7374 2069 6e76  d Asia boost inv
-000010b0: 6573 746d 656e 7420 696e 2074 6f70 206c  estment in top l
-000010c0: 6576 656c 2073 706f 7274 7327 292c 0a20  evel sports'),. 
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000010e0: 2773 706f 7274 7327 2c20 2753 756d 6d69  'sports', 'Summi
-000010f0: 7420 5365 7269 6573 206c 6f6f 6b20 6c61  t Series look la
-00001100: 756e 6368 6573 2048 424f 2043 616e 6164  unches HBO Canad
-00001110: 6120 7370 6f72 7473 2064 6f63 2073 6572  a sports doc ser
-00001120: 6965 733a 204d 7564 6861 7227 290a 2020  ies: Mudhar').  
-00001130: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00001140: 2020 2020 2020 2020 2320 7472 6169 6e20          # train 
-00001150: 616e 6420 7361 7665 2062 6573 7420 6d6f  and save best mo
-00001160: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
-00001170: 6d2e 7472 6169 6e28 6461 7461 290a 2020  m.train(data).  
-00001180: 2020 2020 2020 2020 2020 2320 6c6f 6164            # load
-00001190: 2062 6573 7420 6d6f 6465 6c20 6672 6f6d   best model from
-000011a0: 206d 6f64 656c 5f64 6972 0a20 2020 2020   model_dir.     
-000011b0: 2020 2020 2020 206d 2e6c 6f61 645f 6d6f         m.load_mo
-000011c0: 6465 6c28 290a 2020 2020 2020 2020 2020  del().          
-000011d0: 2020 7072 6564 6963 745f 6c61 6265 6c2c    predict_label,
-000011e0: 2070 7265 6469 6374 5f70 726f 6261 203d   predict_proba =
-000011f0: 206d 2e70 7265 6469 6374 285b 0a20 2020   m.predict([.   
-00001200: 2020 2020 2020 2020 2020 2020 2027 4162               'Ab
-00001210: 626f 7474 2067 6f76 6572 6e6d 656e 7420  bott government 
-00001220: 7370 656e 6473 2024 3820 6d69 6c6c 696f  spends $8 millio
-00001230: 6e20 6f6e 2068 6967 6865 7220 6564 7563  n on higher educ
-00001240: 6174 696f 6e20 6d65 6469 6120 626c 6974  ation media blit
-00001250: 7a27 5d29 0a20 2020 2020 2020 2020 2020  z']).           
-00001260: 2070 7269 6e74 2866 2770 7265 6469 6374   print(f'predict
-00001270: 5f6c 6162 656c 3a20 7b70 7265 6469 6374  _label: {predict
-00001280: 5f6c 6162 656c 7d2c 2070 7265 6469 6374  _label}, predict
-00001290: 5f70 726f 6261 3a20 7b70 7265 6469 6374  _proba: {predict
-000012a0: 5f70 726f 6261 7d27 290a 2020 2020 2020  _proba}').      
-000012b0: 2020 0a20 2020 2020 2020 2020 2020 2074    .            t
-000012c0: 6573 745f 6461 7461 203d 205b 0a20 2020  est_data = [.   
-000012d0: 2020 2020 2020 2020 2020 2020 2028 2765               ('e
-000012e0: 6475 6361 7469 6f6e 272c 2027 4162 626f  ducation', 'Abbo
-000012f0: 7474 2067 6f76 6572 6e6d 656e 7420 7370  tt government sp
-00001300: 656e 6473 2024 3820 6d69 6c6c 696f 6e20  ends $8 million 
-00001310: 6f6e 2068 6967 6865 7220 6564 7563 6174  on higher educat
-00001320: 696f 6e20 6d65 6469 6120 626c 6974 7a27  ion media blitz'
-00001330: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00001340: 2020 2028 2773 706f 7274 7327 2c20 274d     ('sports', 'M
-00001350: 6964 646c 6520 4561 7374 2061 6e64 2041  iddle East and A
-00001360: 7369 6120 626f 6f73 7420 696e 7665 7374  sia boost invest
-00001370: 6d65 6e74 2069 6e20 746f 7020 6c65 7665  ment in top leve
-00001380: 6c20 7370 6f72 7473 2729 2c0a 2020 2020  l sports'),.    
-00001390: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000013a0: 2020 2020 2020 6163 635f 7363 6f72 6520        acc_score 
-000013b0: 3d20 6d2e 6576 616c 7561 7465 5f6d 6f64  = m.evaluate_mod
-000013c0: 656c 2874 6573 745f 6461 7461 290a 2020  el(test_data).  
-000013d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000013e0: 6627 6163 635f 7363 6f72 653a 207b 6163  f'acc_score: {ac
-000013f0: 635f 7363 6f72 657d 2729 0a20 2020 2020  c_score}').     
-00001400: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
-00001410: 2020 2020 2020 2020 6f75 7470 7574 3a0a          output:.
-00001420: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001430: 2060 6060 0a20 2020 2020 2020 2043 6c61   ```.        Cla
-00001440: 7373 6963 436c 6173 7369 6669 6572 2069  ssicClassifier i
-00001450: 6e73 7461 6e63 6520 284c 6f67 6973 7469  nstance (Logisti
-00001460: 6352 6567 7265 7373 696f 6e28 6669 745f  cRegression(fit_
-00001470: 696e 7465 7263 6570 743d 4661 6c73 6529  intercept=False)
-00001480: 2c20 7374 6f70 776f 7264 7320 7369 7a65  , stopwords size
-00001490: 3a20 3234 3338 290a 2020 2020 2020 2020  : 2438).        
-000014a0: 7072 6564 6963 745f 6c61 6265 6c3a 205b  predict_label: [
-000014b0: 2765 6475 6361 7469 6f6e 275d 2c20 7072  'education'], pr
-000014c0: 6564 6963 745f 7072 6f62 613a 205b 302e  edict_proba: [0.
-000014d0: 3533 3738 3233 3633 3538 3439 3231 3132  5378236358492112
-000014e0: 5d0a 2020 2020 2020 2020 6163 635f 7363  ].        acc_sc
-000014f0: 6f72 653a 2031 2e30 0a20 2020 2020 2020  ore: 1.0.       
-00001500: 2060 6060 0a20 2020 2020 2020 200a 2020   ```.        .  
-00001510: 2020 2020 2020 2323 2043 6869 6e65 7365        ## Chinese
-00001520: 2054 6578 7420 436c 6173 7369 6669 6572   Text Classifier
-00001530: 28e4 b8ad e696 87e6 9687 e69c ace5 8886  (...............
-00001540: e7b1 bb29 0a20 2020 2020 2020 200a 2020  ...).        .  
-00001550: 2020 2020 2020 5465 7874 2063 6c61 7373        Text class
-00001560: 6966 6963 6174 696f 6e20 636f 6d70 6174  ification compat
-00001570: 6962 6c65 2077 6974 6820 4368 696e 6573  ible with Chines
-00001580: 6520 616e 6420 456e 676c 6973 6820 636f  e and English co
-00001590: 7270 6f72 612e 0a20 2020 2020 2020 200a  rpora..        .
-000015a0: 2020 2020 2020 2020 6578 616d 706c 6520          example 
-000015b0: 5b65 7861 6d70 6c65 732f 6c72 5f63 6c61  [examples/lr_cla
-000015c0: 7373 6966 6963 6174 696f 6e5f 6465 6d6f  ssification_demo
-000015d0: 2e70 795d 2865 7861 6d70 6c65 732f 6c72  .py](examples/lr
-000015e0: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
-000015f0: 6465 6d6f 2e70 7929 0a20 2020 2020 2020  demo.py).       
-00001600: 200a 2020 2020 2020 2020 6060 6070 7974   .        ```pyt
-00001610: 686f 6e0a 2020 2020 2020 2020 696d 706f  hon.        impo
-00001620: 7274 2073 7973 0a20 2020 2020 2020 200a  rt sys.        .
-00001630: 2020 2020 2020 2020 7379 732e 7061 7468          sys.path
-00001640: 2e61 7070 656e 6428 272e 2e27 290a 2020  .append('..').  
-00001650: 2020 2020 2020 6672 6f6d 2070 7974 6578        from pytex
-00001660: 7463 6c61 7373 6966 6965 7220 696d 706f  tclassifier impo
-00001670: 7274 2043 6c61 7373 6963 436c 6173 7369  rt ClassicClassi
-00001680: 6669 6572 0a20 2020 2020 2020 200a 2020  fier.        .  
-00001690: 2020 2020 2020 6966 205f 5f6e 616d 655f        if __name_
-000016a0: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
-000016b0: 0a20 2020 2020 2020 2020 2020 206d 203d  .            m =
-000016c0: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
-000016d0: 6572 286d 6f64 656c 5f64 6972 3d27 6d6f  er(model_dir='mo
-000016e0: 6465 6c73 2f6c 722d 746f 7927 2c20 6d6f  dels/lr-toy', mo
-000016f0: 6465 6c5f 6e61 6d65 5f6f 725f 6d6f 6465  del_name_or_mode
-00001700: 6c3d 276c 7227 290a 2020 2020 2020 2020  l='lr').        
-00001710: 2020 2020 2320 e7bb 8fe5 85b8 e588 86e7      # ..........
-00001720: b1bb e696 b9e6 b395 efbc 8ce6 94af e68c  ................
-00001730: 81e7 9a84 e6a8 a1e5 9e8b e58c 85e6 8bac  ................
-00001740: efbc 9a6c 722c 2072 616e 646f 6d5f 666f  ...lr, random_fo
-00001750: 7265 7374 2c20 6465 6369 7369 6f6e 5f74  rest, decision_t
-00001760: 7265 652c 206b 6e6e 2c20 6261 7965 732c  ree, knn, bayes,
-00001770: 2073 766d 2c20 7867 626f 6f73 740a 2020   svm, xgboost.  
-00001780: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00001790: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000017a0: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
-000017b0: 2027 e590 8de5 b888 e68c 87e5 afbc e689   '..............
-000017c0: 98e7 a68f e8af ade6 b395 e68a 80e5 b7a7  ................
-000017d0: efbc 9ae5 908d e8af 8de7 9a84 e5a4 8de6  ................
-000017e0: 95b0 e5bd a2e5 bc8f 2729 2c0a 2020 2020  ........'),.    
-000017f0: 2020 2020 2020 2020 2020 2020 2827 6564              ('ed
-00001800: 7563 6174 696f 6e27 2c20 27e4 b8ad e59b  ucation', '.....
-00001810: bde9 ab98 e880 83e6 8890 e7bb a9e6 b5b7  ................
-00001820: e5a4 96e8 aea4 e58f af20 e698 afe2 809c  ......... ......
-00001830: e78b bce6 9da5 e4ba 86e2 809d e590 97ef  ................
-00001840: bc9f 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00001850: 2020 2020 2020 2827 6564 7563 6174 696f        ('educatio
-00001860: 6e27 2c20 27e5 85ac e58a a1e5 9198 e880  n', '...........
-00001870: 83e8 9991 e8b6 8ae6 9da5 e8b6 8ae5 9083  ................
-00001880: e9a6 99ef bc8c e8bf 99e6 98af e680 8ee4  ................
-00001890: b988 e59b 9ee4 ba8b efbc 9f27 292c 0a20  ...........'),. 
-000018a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000018b0: 2773 706f 7274 7327 2c20 27e5 9bbe e696  'sports', '.....
-000018c0: 87ef bc9a e6b3 95e7 bd91 e5ad 9fe8 8fb2  ................
-000018d0: e5b0 94e6 96af e88b a6e6 8898 e8bf 9b31  ...............1
-000018e0: 36e5 bcba 20e5 ad9f e88f b2e5 b094 e696  6... ...........
-000018f0: afe6 8092 e590 bc27 292c 0a20 2020 2020  .......'),.     
-00001900: 2020 2020 2020 2020 2020 2028 2773 706f             ('spo
-00001910: 7274 7327 2c20 27e5 9b9b e5b7 9de4 b8b9  rts', '.........
-00001920: e6a3 b1e4 b8be e8a1 8ce5 85a8 e59b bde9  ................
-00001930: 95bf e8b7 9de7 99bb e5b1 b1e6 8c91 e688  ................
-00001940: 98e8 b59b 20e8 bf91 e4b8 87e4 baba e58f  .... ...........
-00001950: 82e4 b88e 2729 2c0a 2020 2020 2020 2020  ....'),.        
-00001960: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
-00001970: 272c 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba  ', '............
-00001980: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
-00001990: 3130 e5b9 b4e8 bf9e e883 9c27 292c 0a20  10.........'),. 
-000019a0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-000019b0: 2020 2020 2020 2020 206d 2e74 7261 696e           m.train
-000019c0: 2864 6174 6129 0a20 2020 2020 2020 2020  (data).         
-000019d0: 2020 2070 7269 6e74 286d 290a 2020 2020     print(m).    
-000019e0: 2020 2020 2020 2020 2320 6c6f 6164 2062          # load b
-000019f0: 6573 7420 6d6f 6465 6c20 6672 6f6d 206d  est model from m
-00001a00: 6f64 656c 5f64 6972 0a20 2020 2020 2020  odel_dir.       
-00001a10: 2020 2020 206d 2e6c 6f61 645f 6d6f 6465       m.load_mode
-00001a20: 6c28 290a 2020 2020 2020 2020 2020 2020  l().            
-00001a30: 7072 6564 6963 745f 6c61 6265 6c2c 2070  predict_label, p
-00001a40: 7265 6469 6374 5f70 726f 6261 203d 206d  redict_proba = m
-00001a50: 2e70 7265 6469 6374 285b 27e7 a68f e5bb  .predict(['.....
-00001a60: bae6 98a5 e5ad a3e5 85ac e58a a1e5 9198  ................
-00001a70: e880 83e8 af95 e68a a5e5 908d 3138 e697  ............18..
-00001a80: a5e6 88aa e6ad a220 32e6 9c88 36e6 97a5  ....... 2...6...
-00001a90: e880 83e8 af95 272c 0a20 2020 2020 2020  ......',.       
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001ad0: e684 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8  ................
-00001ae0: b59b e4ba a4e6 8898 e8ae b0e5 bd95 3ae7  ..............:.
-00001af0: b1b3 e585 b0e5 aea2 e59c ba38 e688 98e4  ...........8....
-00001b00: b88d e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4  ...........10...
-00001b10: e8bf 9ee8 839c 275d 290a 2020 2020 2020  ......']).      
-00001b20: 2020 2020 2020 7072 696e 7428 6627 7072        print(f'pr
-00001b30: 6564 6963 745f 6c61 6265 6c3a 207b 7072  edict_label: {pr
-00001b40: 6564 6963 745f 6c61 6265 6c7d 2c20 7072  edict_label}, pr
-00001b50: 6564 6963 745f 7072 6f62 613a 207b 7072  edict_proba: {pr
-00001b60: 6564 6963 745f 7072 6f62 617d 2729 0a20  edict_proba}'). 
-00001b70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001b80: 2020 2020 7465 7374 5f64 6174 6120 3d20      test_data = 
-00001b90: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00001ba0: 2020 2827 6564 7563 6174 696f 6e27 2c20    ('education', 
-00001bb0: 27e7 a68f e5bb bae6 98a5 e5ad a3e5 85ac  '...............
-00001bc0: e58a a1e5 9198 e880 83e8 af95 e68a a5e5  ................
-00001bd0: 908d 3138 e697 a5e6 88aa e6ad a220 32e6  ..18......... 2.
-00001be0: 9c88 36e6 97a5 e880 83e8 af95 2729 2c0a  ..6.........'),.
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2827 7370 6f72 7473 272c 2027 e684 8fe7  ('sports', '....
-00001c10: 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b e4ba  ................
-00001c20: a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3 e585  ..........:.....
-00001c30: b0e5 aea2 e59c ba38 e688 98e4 b88d e8b4  .......8........
-00001c40: a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8  .......10.......
-00001c50: 839c 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00001c60: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-00001c70: 6163 635f 7363 6f72 6520 3d20 6d2e 6576  acc_score = m.ev
-00001c80: 616c 7561 7465 5f6d 6f64 656c 2874 6573  aluate_model(tes
-00001c90: 745f 6461 7461 290a 2020 2020 2020 2020  t_data).        
-00001ca0: 2020 2020 7072 696e 7428 6627 6163 635f      print(f'acc_
-00001cb0: 7363 6f72 653a 207b 6163 635f 7363 6f72  score: {acc_scor
-00001cc0: 657d 2729 2020 2320 312e 300a 2020 2020  e}')  # 1.0.    
-00001cd0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00001ce0: 2023 2323 2320 7472 6169 6e20 6d6f 6465   #### train mode
-00001cf0: 6c20 7769 7468 2031 7720 6461 7461 0a20  l with 1w data. 
-00001d00: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00001d10: 2827 2d27 202a 2034 3229 0a20 2020 2020  ('-' * 42).     
-00001d20: 2020 2020 2020 206d 203d 2043 6c61 7373         m = Class
-00001d30: 6963 436c 6173 7369 6669 6572 286d 6f64  icClassifier(mod
-00001d40: 656c 5f64 6972 3d27 6d6f 6465 6c73 2f6c  el_dir='models/l
-00001d50: 7227 2c20 6d6f 6465 6c5f 6e61 6d65 5f6f  r', model_name_o
-00001d60: 725f 6d6f 6465 6c3d 276c 7227 290a 2020  r_model='lr').  
-00001d70: 2020 2020 2020 2020 2020 6461 7461 5f66            data_f
-00001d80: 696c 6520 3d20 2774 6875 636e 6577 735f  ile = 'thucnews_
-00001d90: 7472 6169 6e5f 3177 2e74 7874 270a 2020  train_1w.txt'.  
-00001da0: 2020 2020 2020 2020 2020 6d2e 7472 6169            m.trai
-00001db0: 6e28 6461 7461 5f66 696c 6529 0a20 2020  n(data_file).   
-00001dc0: 2020 2020 2020 2020 206d 2e6c 6f61 645f           m.load_
-00001dd0: 6d6f 6465 6c28 290a 2020 2020 2020 2020  model().        
-00001de0: 2020 2020 7072 6564 6963 745f 6c61 6265      predict_labe
-00001df0: 6c2c 2070 7265 6469 6374 5f70 726f 6261  l, predict_proba
-00001e00: 203d 206d 2e70 7265 6469 6374 280a 2020   = m.predict(.  
-00001e10: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
-00001e20: e9a1 bae4 b989 e58c 97e4 baac e88b 8fe6  ................
-00001e30: b4bb 3838 e5b9 b3e7 b1b3 e8b5 b7e7 b2be  ..88............
-00001e40: e8a3 85e6 88bf e59c a8e5 94ae 272c 0a20  ............',. 
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e60: 27e7 be8e 4542 2d35 e9a1 b9e7 9bae e280  '...EB-5........
-00001e70: 9c31 35e6 97a5 e5bf abe9 809f e7a7 bbe6  .15.............
-00001e80: b091 e280 9de5 b086 e68e a8e8 bf9f 275d  ..............']
-00001e90: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00001ea0: 696e 7428 6627 7072 6564 6963 745f 6c61  int(f'predict_la
-00001eb0: 6265 6c3a 207b 7072 6564 6963 745f 6c61  bel: {predict_la
-00001ec0: 6265 6c7d 2c20 7072 6564 6963 745f 7072  bel}, predict_pr
-00001ed0: 6f62 613a 207b 7072 6564 6963 745f 7072  oba: {predict_pr
-00001ee0: 6f62 617d 2729 0a20 2020 2020 2020 2060  oba}').        `
-00001ef0: 6060 0a20 2020 2020 2020 200a 2020 2020  ``.        .    
-00001f00: 2020 2020 6f75 7470 7574 3a0a 2020 2020      output:.    
-00001f10: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-00001f20: 0a20 2020 2020 2020 2043 6c61 7373 6963  .        Classic
-00001f30: 436c 6173 7369 6669 6572 2069 6e73 7461  Classifier insta
-00001f40: 6e63 6520 284c 6f67 6973 7469 6352 6567  nce (LogisticReg
-00001f50: 7265 7373 696f 6e28 6669 745f 696e 7465  ression(fit_inte
-00001f60: 7263 6570 743d 4661 6c73 6529 2c20 7374  rcept=False), st
-00001f70: 6f70 776f 7264 7320 7369 7a65 3a20 3234  opwords size: 24
-00001f80: 3338 290a 2020 2020 2020 2020 7072 6564  38).        pred
-00001f90: 6963 745f 6c61 6265 6c3a 205b 2765 6475  ict_label: ['edu
-00001fa0: 6361 7469 6f6e 2720 2773 706f 7274 7327  cation' 'sports'
-00001fb0: 5d2c 2070 7265 6469 6374 5f70 726f 6261  ], predict_proba
-00001fc0: 3a20 5b30 2e35 2c20 302e 3539 3839 3431  : [0.5, 0.598941
-00001fd0: 3830 3637 3431 3533 345d 0a20 2020 2020  806741534].     
-00001fe0: 2020 2061 6363 5f73 636f 7265 3a20 312e     acc_score: 1.
-00001ff0: 300a 2020 2020 2020 2020 2d2d 2d2d 2d2d  0.        ------
-00002000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002020: 2d2d 2d2d 0a20 2020 2020 2020 2070 7265  ----.        pre
-00002030: 6469 6374 5f6c 6162 656c 3a20 5b27 7265  dict_label: ['re
-00002040: 616c 7479 2720 2765 6475 6361 7469 6f6e  alty' 'education
-00002050: 275d 2c20 7072 6564 6963 745f 7072 6f62  '], predict_prob
-00002060: 613a 205b 302e 3733 3032 3935 3639 3233  a: [0.7302956923
-00002070: 3631 3733 3732 2c20 302e 3235 3635 3030  617372, 0.256500
-00002080: 3534 3435 3332 3239 3233 5d0a 2020 2020  5445322923].    
-00002090: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-000020a0: 0a20 2020 2020 2020 2023 2320 5669 7375  .        ## Visu
-000020b0: 616c 2046 6561 7475 7265 2049 6d70 6f72  al Feature Impor
-000020c0: 7461 6e63 650a 2020 2020 2020 2020 0a20  tance.        . 
-000020d0: 2020 2020 2020 2053 686f 7720 6665 6174         Show feat
-000020e0: 7572 6520 7765 6967 6874 7320 6f66 206d  ure weights of m
-000020f0: 6f64 656c 2c20 616e 6420 7072 6564 6963  odel, and predic
-00002100: 7469 6f6e 2077 6f72 6420 7765 6967 6874  tion word weight
-00002110: 2c20 666f 7220 6578 616d 706c 6520 5b65  , for example [e
-00002120: 7861 6d70 6c65 732f 7669 7375 616c 5f66  xamples/visual_f
-00002130: 6561 7475 7265 5f69 6d70 6f72 7461 6e63  eature_importanc
-00002140: 652e 6970 796e 625d 2865 7861 6d70 6c65  e.ipynb](example
-00002150: 732f 7669 7375 616c 5f66 6561 7475 7265  s/visual_feature
-00002160: 5f69 6d70 6f72 7461 6e63 652e 6970 796e  _importance.ipyn
-00002170: 6229 0a20 2020 2020 2020 2060 6060 7079  b).        ```py
-00002180: 7468 6f6e 0a20 2020 2020 2020 2069 6d70  thon.        imp
-00002190: 6f72 7420 7379 730a 2020 2020 2020 2020  ort sys.        
-000021a0: 0a20 2020 2020 2020 2073 7973 2e70 6174  .        sys.pat
-000021b0: 682e 6170 7065 6e64 2827 2e2e 2729 0a20  h.append('..'). 
-000021c0: 2020 2020 2020 2066 726f 6d20 7079 7465         from pyte
-000021d0: 7874 636c 6173 7369 6669 6572 2069 6d70  xtclassifier imp
-000021e0: 6f72 7420 436c 6173 7369 6343 6c61 7373  ort ClassicClass
-000021f0: 6966 6965 720a 2020 2020 2020 2020 696d  ifier.        im
-00002200: 706f 7274 206a 6965 6261 0a20 2020 2020  port jieba.     
-00002210: 2020 200a 2020 2020 2020 2020 7463 203d     .        tc =
-00002220: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
-00002230: 6572 286d 6f64 656c 5f64 6972 3d27 6d6f  er(model_dir='mo
-00002240: 6465 6c73 2f6c 722d 746f 7927 2c20 6d6f  dels/lr-toy', mo
-00002250: 6465 6c5f 6e61 6d65 5f6f 725f 6d6f 6465  del_name_or_mode
-00002260: 6c3d 276c 7227 290a 2020 2020 2020 2020  l='lr').        
-00002270: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00002280: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
-00002290: 272c 2027 e590 8de5 b888 e68c 87e5 afbc  ', '............
-000022a0: e689 98e7 a68f e8af ade6 b395 e68a 80e5  ................
-000022b0: b7a7 efbc 9ae5 908d e8af 8de7 9a84 e5a4  ................
-000022c0: 8de6 95b0 e5bd a2e5 bc8f 2729 2c0a 2020  ..........'),.  
-000022d0: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-000022e0: 6174 696f 6e27 2c20 27e4 b8ad e59b bde9  ation', '.......
-000022f0: ab98 e880 83e6 8890 e7bb a9e6 b5b7 e5a4  ................
-00002300: 96e8 aea4 e58f af20 e698 afe2 809c e78b  ....... ........
-00002310: bce6 9da5 e4ba 86e2 809d e590 97ef bc9f  ................
-00002320: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00002330: 2827 7370 6f72 7473 272c 2027 e59b bee6  ('sports', '....
-00002340: 9687 efbc 9ae6 b395 e7bd 91e5 ad9f e88f  ................
-00002350: b2e5 b094 e696 afe8 8ba6 e688 98e8 bf9b  ................
-00002360: 3136 e5bc ba20 e5ad 9fe8 8fb2 e5b0 94e6  16... ..........
-00002370: 96af e680 92e5 90bc 2729 2c0a 2020 2020  ........'),.    
-00002380: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
-00002390: 272c 2027 e59b 9be5 b79d e4b8 b9e6 a3b1  ', '............
-000023a0: e4b8 bee8 a18c e585 a8e5 9bbd e995 bfe8  ................
-000023b0: b79d e799 bbe5 b1b1 e68c 91e6 8898 e8b5  ................
-000023c0: 9b20 e8bf 91e4 b887 e4ba bae5 8f82 e4b8  . ..............
-000023d0: 8e27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
-000023e0: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
-000023f0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
-00002400: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
-00002410: 9ee8 839c 2729 0a20 2020 2020 2020 205d  ....').        ]
-00002420: 0a20 2020 2020 2020 2074 632e 7472 6169  .        tc.trai
-00002430: 6e28 6461 7461 290a 2020 2020 2020 2020  n(data).        
-00002440: 696d 706f 7274 2065 6c69 350a 2020 2020  import eli5.    
-00002450: 2020 2020 696e 6665 725f 6461 7461 203d      infer_data =
-00002460: 205b 27e9 ab98 e880 83e6 8c87 e5af bce6   ['.............
-00002470: 8998 e7a6 8fe8 afad e6b3 95e6 8a80 e5b7  ................
-00002480: a7e5 9bbd e999 85e8 aea4 e58f af27 2c0a  .............',.
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2020 27e6 848f e794 b2e9 a696        '.........
-000024b0: e8bd aee8 a1a5 e8b5 9be4 baa4 e688 98e8  ................
-000024c0: aeb0 e5bd 953a e7b1 b3e5 85b0 e5ae a2e5  .....:..........
-000024d0: 9cba 38e6 8898 e4b8 8de8 b4a5 e59b bde7  ..8.............
-000024e0: b1b3 3130 e5b9 b4e8 bf9e e883 9c27 5d0a  ..10.........'].
-000024f0: 2020 2020 2020 2020 656c 6935 2e73 686f          eli5.sho
-00002500: 775f 7765 6967 6874 7328 7463 2e6d 6f64  w_weights(tc.mod
-00002510: 656c 2c20 7665 633d 7463 2e66 6561 7475  el, vec=tc.featu
-00002520: 7265 290a 2020 2020 2020 2020 7365 675f  re).        seg_
-00002530: 696e 6665 725f 6461 7461 203d 205b 2720  infer_data = [' 
-00002540: 272e 6a6f 696e 286a 6965 6261 2e6c 6375  '.join(jieba.lcu
-00002550: 7428 6929 2920 666f 7220 6920 696e 2069  t(i)) for i in i
-00002560: 6e66 6572 5f64 6174 615d 0a20 2020 2020  nfer_data].     
-00002570: 2020 2065 6c69 352e 7368 6f77 5f70 7265     eli5.show_pre
-00002580: 6469 6374 696f 6e28 7463 2e6d 6f64 656c  diction(tc.model
-00002590: 2c20 7365 675f 696e 6665 725f 6461 7461  , seg_infer_data
-000025a0: 5b30 5d2c 2076 6563 3d74 632e 6665 6174  [0], vec=tc.feat
-000025b0: 7572 652c 0a20 2020 2020 2020 2020 2020  ure,.           
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 2020 7461 7267 6574 5f6e 616d 6573 3d5b    target_names=[
-000025e0: 2765 6475 6361 7469 6f6e 272c 2027 7370  'education', 'sp
-000025f0: 6f72 7473 275d 290a 2020 2020 2020 2020  orts']).        
-00002600: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00002610: 2020 2020 206f 7574 7075 743a 0a20 2020       output:.   
-00002620: 2020 2020 200a 2020 2020 2020 2020 215b       .        ![
-00002630: 696d 672e 706e 675d 2864 6f63 732f 696d  img.png](docs/im
-00002640: 672e 706e 6729 0a20 2020 2020 2020 200a  g.png).        .
-00002650: 2020 2020 2020 2020 2323 2044 6565 7020          ## Deep 
-00002660: 436c 6173 7369 6669 6361 7469 6f6e 206d  Classification m
-00002670: 6f64 656c 0a20 2020 2020 2020 200a 2020  odel.        .  
-00002680: 2020 2020 2020 e69c ace9 a1b9 e79b aee6        ..........
-00002690: 94af e68c 81e4 bba5 e4b8 8be6 b7b1 e5ba  ................
-000026a0: a6e5 8886 e7b1 bbe6 a8a1 e59e 8bef bc9a  ................
-000026b0: 4661 7374 5465 7874 e380 8154 6578 7443  FastText...TextC
-000026c0: 4e4e e380 8154 6578 7452 4e4e e380 8142  NN...TextRNN...B
-000026d0: 6572 74e6 a8a1 e59e 8bef bc8c 6069 6d70  ert.........`imp
-000026e0: 6f72 7460 e6a8 a1e5 9e8b e5af b9e5 ba94  ort`............
-000026f0: e79a 84e6 96b9 e6b3 95e6 9da5 e8b0 83e7  ................
-00002700: 94a8 efbc 9a0a 2020 2020 2020 2020 6060  ......        ``
-00002710: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-00002720: 6672 6f6d 2070 7974 6578 7463 6c61 7373  from pytextclass
-00002730: 6966 6965 7220 696d 706f 7274 2046 6173  ifier import Fas
-00002740: 7454 6578 7443 6c61 7373 6966 6965 722c  tTextClassifier,
-00002750: 2054 6578 7443 4e4e 436c 6173 7369 6669   TextCNNClassifi
-00002760: 6572 2c20 5465 7874 524e 4e43 6c61 7373  er, TextRNNClass
-00002770: 6966 6965 722c 2042 6572 7443 6c61 7373  ifier, BertClass
-00002780: 6966 6965 720a 2020 2020 2020 2020 6060  ifier.        ``
-00002790: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-000027a0: 2020 20e4 b88b e99d a2e4 bba5 4661 7374     .........Fast
-000027b0: 5465 7874 e6a8 a1e5 9e8b e4b8 bae7 a4ba  Text............
-000027c0: e4be 8bef bc8c e585 b6e4 bb96 e6a8 a1e5  ................
-000027d0: 9e8b e79a 84e4 bdbf e794 a8e6 96b9 e6b3  ................
-000027e0: 95e7 b1bb e4bc bce3 8082 0a20 2020 2020  ...........     
-000027f0: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
-00002800: 4661 7374 5465 7874 20e6 a8a1 e59e 8b0a  FastText .......
-00002810: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002820: 20e8 aead e7bb 83e5 928c e9a2 84e6 b58b   ...............
-00002830: 6046 6173 7454 6578 7460 e6a8 a1e5 9e8b  `FastText`......
-00002840: e7a4 bae4 be8b 5b65 7861 6d70 6c65 732f  ......[examples/
-00002850: 6661 7374 7465 7874 5f63 6c61 7373 6966  fasttext_classif
-00002860: 6963 6174 696f 6e5f 6465 6d6f 2e70 795d  ication_demo.py]
-00002870: 2865 7861 6d70 6c65 732f 6661 7374 7465  (examples/fastte
-00002880: 7874 5f63 6c61 7373 6966 6963 6174 696f  xt_classificatio
-00002890: 6e5f 6465 6d6f 2e70 7929 0a20 2020 2020  n_demo.py).     
-000028a0: 2020 200a 2020 2020 2020 2020 6060 6070     .        ```p
-000028b0: 7974 686f 6e0a 2020 2020 2020 2020 696d  ython.        im
-000028c0: 706f 7274 2073 7973 0a20 2020 2020 2020  port sys.       
-000028d0: 200a 2020 2020 2020 2020 7379 732e 7061   .        sys.pa
-000028e0: 7468 2e61 7070 656e 6428 272e 2e27 290a  th.append('..').
-000028f0: 2020 2020 2020 2020 6672 6f6d 2070 7974          from pyt
-00002900: 6578 7463 6c61 7373 6966 6965 7220 696d  extclassifier im
-00002910: 706f 7274 2046 6173 7454 6578 7443 6c61  port FastTextCla
-00002920: 7373 6966 6965 722c 206c 6f61 645f 6461  ssifier, load_da
-00002930: 7461 0a20 2020 2020 2020 200a 2020 2020  ta.        .    
-00002940: 2020 2020 6966 205f 5f6e 616d 655f 5f20      if __name__ 
-00002950: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
-00002960: 2020 2020 2020 2020 2020 206d 203d 2046             m = F
-00002970: 6173 7454 6578 7443 6c61 7373 6966 6965  astTextClassifie
-00002980: 7228 6d6f 6465 6c5f 6469 723d 276d 6f64  r(model_dir='mod
-00002990: 656c 732f 6661 7374 7465 7874 2d74 6f79  els/fasttext-toy
-000029a0: 2729 0a20 2020 2020 2020 2020 2020 2064  ').            d
-000029b0: 6174 6120 3d20 5b0a 2020 2020 2020 2020  ata = [.        
-000029c0: 2020 2020 2020 2020 2827 6564 7563 6174          ('educat
-000029d0: 696f 6e27 2c20 27e5 908d e5b8 88e6 8c87  ion', '.........
-000029e0: e5af bce6 8998 e7a6 8fe8 afad e6b3 95e6  ................
-000029f0: 8a80 e5b7 a7ef bc9a e590 8de8 af8d e79a  ................
-00002a00: 84e5 a48d e695 b0e5 bda2 e5bc 8f27 292c  .............'),
-00002a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a20: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
-00002a30: e4b8 ade5 9bbd e9ab 98e8 8083 e688 90e7  ................
-00002a40: bba9 e6b5 b7e5 a496 e8ae a4e5 8faf 20e6  .............. .
-00002a50: 98af e280 9ce7 8bbc e69d a5e4 ba86 e280  ................
-00002a60: 9de5 9097 efbc 9f27 292c 0a20 2020 2020  .......'),.     
-00002a70: 2020 2020 2020 2020 2020 2028 2765 6475             ('edu
-00002a80: 6361 7469 6f6e 272c 2027 e585 ace5 8aa1  cation', '......
-00002a90: e591 98e8 8083 e899 91e8 b68a e69d a5e8  ................
-00002aa0: b68a e590 83e9 a699 efbc 8ce8 bf99 e698  ................
-00002ab0: afe6 808e e4b9 88e5 9b9e e4ba 8bef bc9f  ................
-00002ac0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00002ad0: 2020 2020 2827 7370 6f72 7473 272c 2027      ('sports', '
-00002ae0: e59b bee6 9687 efbc 9ae6 b395 e7bd 91e5  ................
-00002af0: ad9f e88f b2e5 b094 e696 afe8 8ba6 e688  ................
-00002b00: 98e8 bf9b 3136 e5bc ba20 e5ad 9fe8 8fb2  ....16... ......
-00002b10: e5b0 94e6 96af e680 92e5 90bc 2729 2c0a  ............'),.
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2827 7370 6f72 7473 272c 2027 e59b 9be5  ('sports', '....
-00002b40: b79d e4b8 b9e6 a3b1 e4b8 bee8 a18c e585  ................
-00002b50: a8e5 9bbd e995 bfe8 b79d e799 bbe5 b1b1  ................
-00002b60: e68c 91e6 8898 e8b5 9b20 e8bf 91e4 b887  ......... ......
-00002b70: e4ba bae5 8f82 e4b8 8e27 292c 0a20 2020  .........'),.   
-00002b80: 2020 2020 2020 2020 2020 2020 2028 2773               ('s
-00002b90: 706f 7274 7327 2c20 27e7 b1b3 e585 b0e5  ports', '.......
-00002ba0: aea2 e59c ba38 e688 98e4 b88d e8b4 a5e4  .....8..........
-00002bb0: bf9d e68c 81e8 bf9e e883 9c27 292c 0a20  ...........'),. 
-00002bc0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-00002bd0: 2020 2020 2020 2020 206d 2e74 7261 696e           m.train
-00002be0: 2864 6174 612c 206e 756d 5f65 706f 6368  (data, num_epoch
-00002bf0: 733d 3329 0a20 2020 2020 2020 2020 2020  s=3).           
-00002c00: 2070 7269 6e74 286d 290a 2020 2020 2020   print(m).      
-00002c10: 2020 2020 2020 2320 6c6f 6164 2074 7261        # load tra
-00002c20: 696e 6564 2062 6573 7420 6d6f 6465 6c0a  ined best model.
-00002c30: 2020 2020 2020 2020 2020 2020 6d2e 6c6f              m.lo
-00002c40: 6164 5f6d 6f64 656c 2829 0a20 2020 2020  ad_model().     
-00002c50: 2020 2020 2020 2070 7265 6469 6374 5f6c         predict_l
-00002c60: 6162 656c 2c20 7072 6564 6963 745f 7072  abel, predict_pr
-00002c70: 6f62 6120 3d20 6d2e 7072 6564 6963 7428  oba = m.predict(
-00002c80: 5b27 e7a6 8fe5 bbba e698 a5e5 ada3 e585  ['..............
-00002c90: ace5 8aa1 e591 98e8 8083 e8af 95e6 8aa5  ................
-00002ca0: e590 8d31 38e6 97a5 e688 aae6 ada2 2032  ...18......... 2
-00002cb0: e69c 8836 e697 a5e8 8083 e8af 9527 2c0a  ...6.........',.
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cf0: 2020 2020 2020 27e6 848f e794 b2e9 a696        '.........
-00002d00: e8bd aee8 a1a5 e8b5 9be4 baa4 e688 98e8  ................
-00002d10: aeb0 e5bd 953a e7b1 b3e5 85b0 e5ae a2e5  .....:..........
-00002d20: 9cba 38e6 8898 e4b8 8de8 b4a5 e59b bde7  ..8.............
-00002d30: b1b3 3130 e5b9 b4e8 bf9e e883 9c27 5d29  ..10.........'])
-00002d40: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00002d50: 6e74 2866 2770 7265 6469 6374 5f6c 6162  nt(f'predict_lab
-00002d60: 656c 3a20 7b70 7265 6469 6374 5f6c 6162  el: {predict_lab
-00002d70: 656c 7d2c 2070 7265 6469 6374 5f70 726f  el}, predict_pro
-00002d80: 6261 3a20 7b70 7265 6469 6374 5f70 726f  ba: {predict_pro
-00002d90: 6261 7d27 290a 2020 2020 2020 2020 2020  ba}').          
-00002da0: 2020 7465 7374 5f64 6174 6120 3d20 5b0a    test_data = [.
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2827 6564 7563 6174 696f 6e27 2c20 27e7  ('education', '.
-00002dd0: a68f e5bb bae6 98a5 e5ad a3e5 85ac e58a  ................
-00002de0: a1e5 9198 e880 83e8 af95 e68a a5e5 908d  ................
-00002df0: 3138 e697 a5e6 88aa e6ad a220 32e6 9c88  18......... 2...
-00002e00: 36e6 97a5 e880 83e8 af95 2729 2c0a 2020  6.........'),.  
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00002e20: 7370 6f72 7473 272c 2027 e684 8fe7 94b2  sports', '......
-00002e30: e9a6 96e8 bdae e8a1 a5e8 b59b e4ba a4e6  ................
-00002e40: 8898 e8ae b0e5 bd95 3ae7 b1b3 e585 b0e5  ........:.......
-00002e50: aea2 e59c ba38 e688 98e4 b88d e8b4 a5e5  .....8..........
-00002e60: 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8 839c  .....10.........
-00002e70: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00002e80: 5d0a 2020 2020 2020 2020 2020 2020 6163  ].            ac
-00002e90: 635f 7363 6f72 6520 3d20 6d2e 6576 616c  c_score = m.eval
-00002ea0: 7561 7465 5f6d 6f64 656c 2874 6573 745f  uate_model(test_
-00002eb0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00002ec0: 2020 7072 696e 7428 6627 6163 635f 7363    print(f'acc_sc
-00002ed0: 6f72 653a 207b 6163 635f 7363 6f72 657d  ore: {acc_score}
-00002ee0: 2729 2020 2320 312e 300a 2020 2020 2020  ')  # 1.0.      
-00002ef0: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
-00002f00: 2323 2320 7472 6169 6e20 6d6f 6465 6c20  ### train model 
-00002f10: 7769 7468 2031 7720 6461 7461 0a20 2020  with 1w data.   
-00002f20: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00002f30: 2d27 202a 2034 3229 0a20 2020 2020 2020  -' * 42).       
-00002f40: 2020 2020 2064 6174 615f 6669 6c65 203d       data_file =
-00002f50: 2027 7468 7563 6e65 7773 5f74 7261 696e   'thucnews_train
-00002f60: 5f31 772e 7478 7427 0a20 2020 2020 2020  _1w.txt'.       
-00002f70: 2020 2020 206d 203d 2046 6173 7454 6578       m = FastTex
-00002f80: 7443 6c61 7373 6966 6965 7228 6d6f 6465  tClassifier(mode
-00002f90: 6c5f 6469 723d 276d 6f64 656c 732f 6661  l_dir='models/fa
-00002fa0: 7374 7465 7874 2729 0a20 2020 2020 2020  sttext').       
-00002fb0: 2020 2020 206d 2e74 7261 696e 2864 6174       m.train(dat
-00002fc0: 615f 6669 6c65 2c20 6e61 6d65 733d 2827  a_file, names=('
-00002fd0: 6c61 6265 6c73 272c 2027 7465 7874 2729  labels', 'text')
-00002fe0: 2c20 6e75 6d5f 6570 6f63 6873 3d33 290a  , num_epochs=3).
-00002ff0: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
-00003000: 6164 2062 6573 7420 7472 6169 6e65 6420  ad best trained 
-00003010: 6d6f 6465 6c20 6672 6f6d 206d 6f64 656c  model from model
-00003020: 5f64 6972 0a20 2020 2020 2020 2020 2020  _dir.           
-00003030: 206d 2e6c 6f61 645f 6d6f 6465 6c28 290a   m.load_model().
-00003040: 2020 2020 2020 2020 2020 2020 7072 6564              pred
-00003050: 6963 745f 6c61 6265 6c2c 2070 7265 6469  ict_label, predi
-00003060: 6374 5f70 726f 6261 203d 206d 2e70 7265  ct_proba = m.pre
-00003070: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-00003080: 2020 2020 2020 5b27 e9a1 bae4 b989 e58c        ['........
-00003090: 97e4 baac e88b 8fe6 b4bb 3838 e5b9 b3e7  ..........88....
-000030a0: b1b3 e8b5 b7e7 b2be e8a3 85e6 88bf e59c  ................
-000030b0: a8e5 94ae 272c 0a20 2020 2020 2020 2020  ....',.         
-000030c0: 2020 2020 2020 2020 27e7 be8e 4542 2d35          '...EB-5
-000030d0: e9a1 b9e7 9bae e280 9c31 35e6 97a5 e5bf  .........15.....
-000030e0: abe9 809f e7a7 bbe6 b091 e280 9de5 b086  ................
-000030f0: e68e a8e8 bf9f 275d 0a20 2020 2020 2020  ......'].       
-00003100: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00003110: 2020 2070 7269 6e74 2866 2770 7265 6469     print(f'predi
-00003120: 6374 5f6c 6162 656c 3a20 7b70 7265 6469  ct_label: {predi
-00003130: 6374 5f6c 6162 656c 7d2c 2070 7265 6469  ct_label}, predi
-00003140: 6374 5f70 726f 6261 3a20 7b70 7265 6469  ct_proba: {predi
-00003150: 6374 5f70 726f 6261 7d27 290a 2020 2020  ct_proba}').    
-00003160: 2020 2020 2020 2020 782c 2079 2c20 6466          x, y, df
-00003170: 203d 206c 6f61 645f 6461 7461 2864 6174   = load_data(dat
-00003180: 615f 6669 6c65 290a 2020 2020 2020 2020  a_file).        
-00003190: 2020 2020 7465 7374 5f64 6174 6120 3d20      test_data = 
-000031a0: 6466 5b3a 3130 305d 0a20 2020 2020 2020  df[:100].       
-000031b0: 2020 2020 2061 6363 5f73 636f 7265 203d       acc_score =
-000031c0: 206d 2e65 7661 6c75 6174 655f 6d6f 6465   m.evaluate_mode
-000031d0: 6c28 7465 7374 5f64 6174 6129 0a20 2020  l(test_data).   
-000031e0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-000031f0: 2761 6363 5f73 636f 7265 3a20 7b61 6363  'acc_score: {acc
-00003200: 5f73 636f 7265 7d27 290a 2020 2020 2020  _score}').      
-00003210: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
-00003220: 2020 2020 2020 2023 2323 2042 4552 5420         ### BERT 
-00003230: e7b1 bbe6 a8a1 e59e 8b0a 2020 2020 2020  ..........      
-00003240: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
-00003250: e5a4 9ae5 8886 e7b1 bbe6 a8a1 e59e 8b0a  ................
-00003260: 2020 2020 2020 2020 e8ae ade7 bb83 e592          ........
-00003270: 8ce9 a284 e6b5 8b60 4245 5254 60e5 a49a  .......`BERT`...
-00003280: e588 86e7 b1bb e6a8 a1e5 9e8b efbc 8ce7  ................
-00003290: a4ba e4be 8b5b 6578 616d 706c 6573 2f62  .....[examples/b
-000032a0: 6572 745f 636c 6173 7369 6669 6361 7469  ert_classificati
-000032b0: 6f6e 5f7a 685f 6465 6d6f 2e70 795d 2865  on_zh_demo.py](e
-000032c0: 7861 6d70 6c65 732f 6265 7274 5f63 6c61  xamples/bert_cla
-000032d0: 7373 6966 6963 6174 696f 6e5f 7a68 5f64  ssification_zh_d
-000032e0: 656d 6f2e 7079 290a 2020 2020 2020 2020  emo.py).        
-000032f0: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
-00003300: 6f6e 0a20 2020 2020 2020 2069 6d70 6f72  on.        impor
-00003310: 7420 7379 730a 2020 2020 2020 2020 0a20  t sys.        . 
-00003320: 2020 2020 2020 2073 7973 2e70 6174 682e         sys.path.
-00003330: 6170 7065 6e64 2827 2e2e 2729 0a20 2020  append('..').   
-00003340: 2020 2020 2066 726f 6d20 7079 7465 7874       from pytext
-00003350: 636c 6173 7369 6669 6572 2069 6d70 6f72  classifier impor
-00003360: 7420 4265 7274 436c 6173 7369 6669 6572  t BertClassifier
-00003370: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003380: 2020 6966 205f 5f6e 616d 655f 5f20 3d3d    if __name__ ==
-00003390: 2027 5f5f 6d61 696e 5f5f 273a 0a20 2020   '__main__':.   
-000033a0: 2020 2020 2020 2020 206d 203d 2042 6572           m = Ber
-000033b0: 7443 6c61 7373 6966 6965 7228 6d6f 6465  tClassifier(mode
-000033c0: 6c5f 6469 723d 276d 6f64 656c 732f 6265  l_dir='models/be
-000033d0: 7274 2d63 6869 6e65 7365 2d74 6f79 272c  rt-chinese-toy',
-000033e0: 206e 756d 5f63 6c61 7373 6573 3d32 2c0a   num_classes=2,.
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00003410: 6f64 656c 5f74 7970 653d 2762 6572 7427  odel_type='bert'
-00003420: 2c20 6d6f 6465 6c5f 6e61 6d65 3d27 6265  , model_name='be
-00003430: 7274 2d62 6173 652d 6368 696e 6573 6527  rt-base-chinese'
-00003440: 2c20 6e75 6d5f 6570 6f63 6873 3d32 290a  , num_epochs=2).
-00003450: 2020 2020 2020 2020 2020 2020 2320 6d6f              # mo
-00003460: 6465 6c5f 7479 7065 3a20 7375 7070 6f72  del_type: suppor
-00003470: 7420 2762 6572 7427 2c20 2761 6c62 6572  t 'bert', 'alber
-00003480: 7427 2c20 2772 6f62 6572 7461 272c 2027  t', 'roberta', '
-00003490: 786c 6e65 7427 0a20 2020 2020 2020 2020  xlnet'.         
-000034a0: 2020 2023 206d 6f64 656c 5f6e 616d 653a     # model_name:
-000034b0: 2073 7570 706f 7274 2027 6265 7274 2d62   support 'bert-b
-000034c0: 6173 652d 6368 696e 6573 6527 2c20 2762  ase-chinese', 'b
-000034d0: 6572 742d 6261 7365 2d63 6173 6564 272c  ert-base-cased',
-000034e0: 2027 6265 7274 2d62 6173 652d 6d75 6c74   'bert-base-mult
-000034f0: 696c 696e 6775 616c 2d63 6173 6564 2720  ilingual-cased' 
-00003500: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00003510: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00003520: 2020 2020 2020 2020 2028 2765 6475 6361           ('educa
-00003530: 7469 6f6e 272c 2027 e590 8de5 b888 e68c  tion', '........
-00003540: 87e5 afbc e689 98e7 a68f e8af ade6 b395  ................
-00003550: e68a 80e5 b7a7 efbc 9ae5 908d e8af 8de7  ................
-00003560: 9a84 e5a4 8de6 95b0 e5bd a2e5 bc8f 2729  ..............')
-00003570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003580: 2020 2827 6564 7563 6174 696f 6e27 2c20    ('education', 
-00003590: 27e4 b8ad e59b bde9 ab98 e880 83e6 8890  '...............
-000035a0: e7bb a9e6 b5b7 e5a4 96e8 aea4 e58f af20  ............... 
-000035b0: e698 afe2 809c e78b bce6 9da5 e4ba 86e2  ................
-000035c0: 809d e590 97ef bc9f 2729 2c0a 2020 2020  ........'),.    
-000035d0: 2020 2020 2020 2020 2020 2020 2827 6564              ('ed
-000035e0: 7563 6174 696f 6e27 2c20 27e5 85ac e58a  ucation', '.....
-000035f0: a1e5 9198 e880 83e8 9991 e8b6 8ae6 9da5  ................
-00003600: e8b6 8ae5 9083 e9a6 99ef bc8c e8bf 99e6  ................
-00003610: 98af e680 8ee4 b988 e59b 9ee4 ba8b efbc  ................
-00003620: 9f27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
-00003630: 2020 2020 2028 2773 706f 7274 7327 2c20       ('sports', 
-00003640: 27e5 9bbe e696 87ef bc9a e6b3 95e7 bd91  '...............
-00003650: e5ad 9fe8 8fb2 e5b0 94e6 96af e88b a6e6  ................
-00003660: 8898 e8bf 9b31 36e5 bcba 20e5 ad9f e88f  .....16... .....
-00003670: b2e5 b094 e696 afe6 8092 e590 bc27 292c  .............'),
+000000f0: 6e3a 203c 6469 7620 616c 6967 6e3d 2263  n: <div align="c
+00000100: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
+00000110: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000120: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+00000130: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
+00000140: 6c61 7373 6966 6965 7222 3e0a 2020 2020  lassifier">.    
+00000150: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000160: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000170: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
+00000180: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00000190: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
+000001a0: 732f 6c6f 676f 2e70 6e67 2220 616c 743d  s/logo.png" alt=
+000001b0: 224c 6f67 6f22 2068 6569 6768 743d 2231  "Logo" height="1
+000001c0: 3536 223e 0a20 2020 2020 2020 2020 203c  56">.          <
+000001d0: 2f61 3e0a 2020 2020 2020 2020 3c2f 6469  /a>.        </di
+000001e0: 763e 0a20 2020 2020 2020 200a 2020 2020  v>.        .    
+000001f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00000200: 2d2d 2d2d 2d0a 2020 2020 2020 2020 0a20  -----.        . 
+00000210: 2020 2020 2020 2023 2050 7954 6578 7443         # PyTextC
+00000220: 6c61 7373 6966 6965 723a 2050 7974 686f  lassifier: Pytho
+00000230: 6e20 5465 7874 2043 6c61 7373 6966 6965  n Text Classifie
+00000240: 720a 2020 2020 2020 2020 5b21 5b50 7950  r.        [![PyP
+00000250: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
+00000260: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+00000270: 2f70 792f 7079 7465 7874 636c 6173 7369  /py/pytextclassi
+00000280: 6669 6572 2e73 7667 295d 2868 7474 7073  fier.svg)](https
+00000290: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+000002a0: 2f70 792f 7079 7465 7874 636c 6173 7369  /py/pytextclassi
+000002b0: 6669 6572 290a 2020 2020 2020 2020 5b21  fier).        [!
+000002c0: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
+000002d0: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
+000002e0: 6467 652f 7079 7465 7874 636c 6173 7369  dge/pytextclassi
+000002f0: 6669 6572 295d 2868 7474 7073 3a2f 2f70  fier)](https://p
+00000300: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+00000310: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+00000320: 7229 0a20 2020 2020 2020 205b 215b 436f  r).        [![Co
+00000330: 6e74 7269 6275 7469 6f6e 7320 7765 6c63  ntributions welc
+00000340: 6f6d 655d 2868 7474 7073 3a2f 2f69 6d67  ome](https://img
+00000350: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000360: 652f 636f 6e74 7269 6275 7469 6f6e 732d  e/contributions-
+00000370: 7765 6c63 6f6d 652d 6272 6967 6874 6772  welcome-brightgr
+00000380: 6565 6e2e 7376 6729 5d28 434f 4e54 5249  een.svg)](CONTRI
+00000390: 4255 5449 4e47 2e6d 6429 0a20 2020 2020  BUTING.md).     
+000003a0: 2020 205b 215b 4769 7448 7562 2063 6f6e     [![GitHub con
+000003b0: 7472 6962 7574 6f72 735d 2868 7474 7073  tributors](https
+000003c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000003d0: 6f2f 6769 7468 7562 2f63 6f6e 7472 6962  o/github/contrib
+000003e0: 7574 6f72 732f 7368 6962 696e 6736 3234  utors/shibing624
+000003f0: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+00000400: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
+00000410: 6769 7468 7562 2e63 6f6d 2f73 6869 6269  github.com/shibi
+00000420: 6e67 3632 342f 7079 7465 7874 636c 6173  ng624/pytextclas
+00000430: 7369 6669 6572 2f67 7261 7068 732f 636f  sifier/graphs/co
+00000440: 6e74 7269 6275 746f 7273 290a 2020 2020  ntributors).    
+00000450: 2020 2020 5b21 5b4c 6963 656e 7365 2041      [![License A
+00000460: 7061 6368 6520 322e 305d 2868 7474 7073  pache 2.0](https
+00000470: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000480: 6f2f 6261 6467 652f 6c69 6365 6e73 652d  o/badge/license-
+00000490: 4170 6163 6865 2532 3032 2e30 2d62 6c75  Apache%202.0-blu
+000004a0: 652e 7376 6729 5d28 4c49 4345 4e53 4529  e.svg)](LICENSE)
+000004b0: 0a20 2020 2020 2020 205b 215b 7079 7468  .        [![pyth
+000004c0: 6f6e 5f76 6573 696f 6e5d 2868 7474 7073  on_vesion](https
+000004d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004e0: 6f2f 6261 6467 652f 5079 7468 6f6e 2d33  o/badge/Python-3
+000004f0: 2e35 2532 422d 6772 6565 6e2e 7376 6729  .5%2B-green.svg)
+00000500: 5d28 7265 7175 6972 656d 656e 7473 2e74  ](requirements.t
+00000510: 7874 290a 2020 2020 2020 2020 5b21 5b47  xt).        [![G
+00000520: 6974 4875 6220 6973 7375 6573 5d28 6874  itHub issues](ht
+00000530: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000540: 732e 696f 2f67 6974 6875 622f 6973 7375  s.io/github/issu
+00000550: 6573 2f73 6869 6269 6e67 3632 342f 7079  es/shibing624/py
+00000560: 7465 7874 636c 6173 7369 6669 6572 2e73  textclassifier.s
+00000570: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000580: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
+00000590: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
+000005a0: 6965 722f 6973 7375 6573 290a 2020 2020  ier/issues).    
+000005b0: 2020 2020 5b21 5b57 6563 6861 7420 4772      [![Wechat Gr
+000005c0: 6f75 705d 2868 7474 703a 2f2f 766c 6f67  oup](http://vlog
+000005d0: 2e73 6679 632e 6c74 642f 7765 6368 6174  .sfyc.ltd/wechat
+000005e0: 5f65 7665 7279 6461 792f 7778 6772 6f75  _everyday/wxgrou
+000005f0: 705f 6c6f 676f 2e70 6e67 3f69 6d61 6765  p_logo.png?image
+00000600: 5669 6577 322f 302f 772f 3630 2f68 2f32  View2/0/w/60/h/2
+00000610: 3029 5d28 2343 6f6e 7461 6374 290a 2020  0)](#Contact).  
+00000620: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
+00000630: 2020 2020 2020 2020 2323 2049 6e74 726f          ## Intro
+00000640: 6475 6374 696f 6e0a 2020 2020 2020 2020  duction.        
+00000650: 5079 5465 7874 436c 6173 7369 6669 6572  PyTextClassifier
+00000660: 3a20 5079 7468 6f6e 2054 6578 7420 436c  : Python Text Cl
+00000670: 6173 7369 6669 6572 2e20 4974 2063 616e  assifier. It can
+00000680: 2062 6520 6170 706c 6965 6420 746f 2074   be applied to t
+00000690: 6865 2066 6965 6c64 7320 6f66 2073 656e  he fields of sen
+000006a0: 7469 6d65 6e74 2070 6f6c 6172 6974 7920  timent polarity 
+000006b0: 616e 616c 7973 6973 2c20 7465 7874 2072  analysis, text r
+000006c0: 6973 6b20 636c 6173 7369 6669 6361 7469  isk classificati
+000006d0: 6f6e 2061 6e64 2073 6f20 6f6e 2c0a 2020  on and so on,.  
+000006e0: 2020 2020 2020 616e 6420 6974 2073 7570        and it sup
+000006f0: 706f 7274 7320 6d75 6c74 6970 6c65 2063  ports multiple c
+00000700: 6c61 7373 6966 6963 6174 696f 6e20 616c  lassification al
+00000710: 676f 7269 7468 6d73 2061 6e64 2063 6c75  gorithms and clu
+00000720: 7374 6572 696e 6720 616c 676f 7269 7468  stering algorith
+00000730: 6d73 2e0a 2020 2020 2020 2020 0a20 2020  ms..        .   
+00000740: 2020 2020 202a 2a70 7974 6578 7463 6c61       **pytextcla
+00000750: 7373 6966 6965 722a 2a20 6973 2061 2070  ssifier** is a p
+00000760: 7974 686f 6e20 4f70 656e 2053 6f75 7263  ython Open Sourc
+00000770: 6520 546f 6f6c 6b69 7420 666f 7220 7465  e Toolkit for te
+00000780: 7874 2063 6c61 7373 6966 6963 6174 696f  xt classificatio
+00000790: 6e2e 2054 6865 2067 6f61 6c20 6973 2074  n. The goal is t
+000007a0: 6f20 696d 706c 656d 656e 740a 2020 2020  o implement.    
+000007b0: 2020 2020 7465 7874 2061 6e61 6c79 7369      text analysi
+000007c0: 7320 616c 676f 7269 7468 6d2c 2073 6f20  s algorithm, so 
+000007d0: 746f 2061 6368 6965 7665 2074 6865 2075  to achieve the u
+000007e0: 7365 2069 6e20 7468 6520 7072 6f64 7563  se in the produc
+000007f0: 7469 6f6e 2065 6e76 6972 6f6e 6d65 6e74  tion environment
+00000800: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00000810: 2020 20e6 9687 e69c ace5 8886 e7b1 bbe5     .............
+00000820: 99a8 efbc 8ce6 8f90 e4be 9be5 a49a e7a7  ................
+00000830: 8de6 9687 e69c ace5 8886 e7b1 bbe5 928c  ................
+00000840: e881 9ae7 b1bb e7ae 97e6 b395 efbc 8ce6  ................
+00000850: 94af e68c 81e5 8fa5 e5ad 90e5 928c e696  ................
+00000860: 87e6 a1a3 e7ba a7e7 9a84 e696 87e6 9cac  ................
+00000870: e588 86e7 b1bb e4bb bbe5 8aa1 efbc 8ce6  ................
+00000880: 94af e68c 81e4 ba8c e588 86e7 b1bb e380  ................
+00000890: 81e5 a49a e588 86e7 b1bb e380 81e5 a49a  ................
+000008a0: e6a0 87e7 adbe e588 86e7 b1bb e380 81e5  ................
+000008b0: a49a e5b1 82e7 baa7 e588 86e7 b1bb e592  ................
+000008c0: 8c4b 6d65 616e 73e8 819a e7b1 bbef bc8c  .Kmeans.........
+000008d0: e5bc 80e7 aeb1 e58d b3e7 94a8 e380 8270  ...............p
+000008e0: 7974 686f 6e33 e5bc 80e5 8f91 e380 820a  ython3..........
+000008f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000900: 202a 2a47 7569 6465 2a2a 0a20 2020 2020   **Guide**.     
+00000910: 2020 200a 2020 2020 2020 2020 2d20 5b46     .        - [F
+00000920: 6561 7475 7265 5d28 2346 6561 7475 7265  eature](#Feature
+00000930: 290a 2020 2020 2020 2020 2d20 5b49 6e73  ).        - [Ins
+00000940: 7461 6c6c 5d28 2369 6e73 7461 6c6c 290a  tall](#install).
+00000950: 2020 2020 2020 2020 2d20 5b55 7361 6765          - [Usage
+00000960: 5d28 2375 7361 6765 290a 2020 2020 2020  ](#usage).      
+00000970: 2020 2d20 5b44 6174 6173 6574 5d28 2344    - [Dataset](#D
+00000980: 6174 6173 6574 290a 2020 2020 2020 2020  ataset).        
+00000990: 2d20 5b43 6f6e 7461 6374 5d28 2343 6f6e  - [Contact](#Con
+000009a0: 7461 6374 290a 2020 2020 2020 2020 2d20  tact).        - 
+000009b0: 5b43 6974 6174 696f 6e5d 2823 4369 7461  [Citation](#Cita
+000009c0: 7469 6f6e 290a 2020 2020 2020 2020 2d20  tion).        - 
+000009d0: 5b52 6566 6572 656e 6365 5d28 2372 6566  [Reference](#ref
+000009e0: 6572 656e 6365 290a 2020 2020 2020 2020  erence).        
+000009f0: 0a20 2020 2020 2020 2023 2320 4665 6174  .        ## Feat
+00000a00: 7572 650a 2020 2020 2020 2020 0a20 2020  ure.        .   
+00000a10: 2020 2020 202a 2a70 7974 6578 7463 6c61       **pytextcla
+00000a20: 7373 6966 6965 722a 2a20 6861 7320 7468  ssifier** has th
+00000a30: 6520 6368 6172 6163 7465 7269 7374 6963  e characteristic
+00000a40: 730a 2020 2020 2020 2020 6f66 2063 6c65  s.        of cle
+00000a50: 6172 2061 6c67 6f72 6974 686d 2c20 6869  ar algorithm, hi
+00000a60: 6768 2070 6572 666f 726d 616e 6365 2061  gh performance a
+00000a70: 6e64 2063 7573 746f 6d69 7a61 626c 6520  nd customizable 
+00000a80: 636f 7270 7573 2e0a 2020 2020 2020 2020  corpus..        
+00000a90: 0a20 2020 2020 2020 2046 756e 6374 696f  .        Functio
+00000aa0: 6e73 efbc 9a0a 2020 2020 2020 2020 2323  ns....        ##
+00000ab0: 2320 436c 6173 7369 6669 6572 0a20 2020  # Classifier.   
+00000ac0: 2020 2020 2020 202d 205b 785d 204c 6f67         - [x] Log
+00000ad0: 6973 7469 6352 6567 7265 7373 696f 6e0a  isticRegression.
+00000ae0: 2020 2020 2020 2020 2020 2d20 5b78 5d20            - [x] 
+00000af0: 5261 6e64 6f6d 2046 6f72 6573 740a 2020  Random Forest.  
+00000b00: 2020 2020 2020 2020 2d20 5b78 5d20 4465          - [x] De
+00000b10: 6369 7369 6f6e 2054 7265 650a 2020 2020  cision Tree.    
+00000b20: 2020 2020 2020 2d20 5b78 5d20 4b2d 4e65        - [x] K-Ne
+00000b30: 6172 6573 7420 4e65 6967 6862 6f75 7273  arest Neighbours
+00000b40: 0a20 2020 2020 2020 2020 202d 205b 785d  .          - [x]
+00000b50: 204e 6169 7665 2062 6179 6573 0a20 2020   Naive bayes.   
+00000b60: 2020 2020 2020 202d 205b 785d 2058 6762         - [x] Xgb
+00000b70: 6f6f 7374 0a20 2020 2020 2020 2020 202d  oost.          -
+00000b80: 205b 785d 2053 7570 706f 7274 2056 6563   [x] Support Vec
+00000b90: 746f 7220 4d61 6368 696e 6528 5356 4d29  tor Machine(SVM)
+00000ba0: 0a20 2020 2020 2020 2020 202d 205b 785d  .          - [x]
+00000bb0: 2054 6578 7443 4e4e 0a20 2020 2020 2020   TextCNN.       
+00000bc0: 2020 202d 205b 785d 2054 6578 7452 4e4e     - [x] TextRNN
+00000bd0: 0a20 2020 2020 2020 2020 202d 205b 785d  .          - [x]
+00000be0: 2046 6173 7474 6578 740a 2020 2020 2020   Fasttext.      
+00000bf0: 2020 2020 2d20 5b78 5d20 4245 5254 0a20      - [x] BERT. 
+00000c00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000c10: 2323 2320 436c 7573 7465 720a 2020 2020  ### Cluster.    
+00000c20: 2020 2020 2020 2d20 5b78 5d20 4d69 6e69        - [x] Mini
+00000c30: 4261 7463 684b 6d65 616e 730a 2020 2020  BatchKmeans.    
+00000c40: 2020 2020 0a20 2020 2020 2020 2057 6869      .        Whi
+00000c50: 6c65 2070 726f 7669 6469 6e67 2072 6963  le providing ric
+00000c60: 6820 6675 6e63 7469 6f6e 732c 202a 2a70  h functions, **p
+00000c70: 7974 6578 7463 6c61 7373 6966 6965 722a  ytextclassifier*
+00000c80: 2a20 696e 7465 726e 616c 206d 6f64 756c  * internal modul
+00000c90: 6573 2061 6468 6572 6520 746f 206c 6f77  es adhere to low
+00000ca0: 2063 6f75 706c 696e 672c 206d 6f64 656c   coupling, model
+00000cb0: 2061 6468 6572 656e 6365 2074 6f20 696e   adherence to in
+00000cc0: 6572 7420 6c6f 6164 696e 672c 2064 6963  ert loading, dic
+00000cd0: 7469 6f6e 6172 7920 7075 626c 6963 6174  tionary publicat
+00000ce0: 696f 6e2c 2061 6e64 2065 6173 7920 746f  ion, and easy to
+00000cf0: 2075 7365 2e0a 2020 2020 2020 2020 0a20   use..        . 
+00000d00: 2020 2020 2020 2023 2320 496e 7374 616c         ## Instal
+00000d10: 6c0a 2020 2020 2020 2020 0a20 2020 2020  l.        .     
+00000d20: 2020 202d 2052 6571 7569 7265 6d65 6e74     - Requirement
+00000d30: 7320 616e 6420 496e 7374 616c 6c61 7469  s and Installati
+00000d40: 6f6e 0a20 2020 2020 2020 200a 2020 2020  on.        .    
+00000d50: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00000d60: 7069 7033 2069 6e73 7461 6c6c 2074 6f72  pip3 install tor
+00000d70: 6368 2023 2063 6f6e 6461 2069 6e73 7461  ch # conda insta
+00000d80: 6c6c 2070 7974 6f72 6368 0a20 2020 2020  ll pytorch.     
+00000d90: 2020 2070 6970 3320 696e 7374 616c 6c20     pip3 install 
+00000da0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00000db0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00000dc0: 2020 2020 200a 2020 2020 2020 2020 6f72       .        or
+00000dd0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000de0: 2020 6060 600a 2020 2020 2020 2020 6769    ```.        gi
+00000df0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00000e00: 6769 7468 7562 2e63 6f6d 2f73 6869 6269  github.com/shibi
+00000e10: 6e67 3632 342f 7079 7465 7874 636c 6173  ng624/pytextclas
+00000e20: 7369 6669 6572 2e67 6974 0a20 2020 2020  sifier.git.     
+00000e30: 2020 2063 6420 7079 7465 7874 636c 6173     cd pytextclas
+00000e40: 7369 6669 6572 0a20 2020 2020 2020 2070  sifier.        p
+00000e50: 7974 686f 6e33 2073 6574 7570 2e70 7920  ython3 setup.py 
+00000e60: 696e 7374 616c 6c0a 2020 2020 2020 2020  install.        
+00000e70: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
+00000e80: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00000e90: 2055 7361 6765 0a20 2020 2020 2020 2023   Usage.        #
+00000ea0: 2323 2054 6578 7420 436c 6173 7369 6669  ## Text Classifi
+00000eb0: 6572 0a20 2020 2020 2020 200a 2020 2020  er.        .    
+00000ec0: 2020 2020 2323 2320 456e 676c 6973 6820      ### English 
+00000ed0: 5465 7874 2043 6c61 7373 6966 6965 720a  Text Classifier.
+00000ee0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000ef0: 2049 6e63 6c75 6469 6e67 206d 6f64 656c   Including model
+00000f00: 2074 7261 696e 696e 672c 2073 6176 696e   training, savin
+00000f10: 672c 2070 7265 6469 6374 2c20 6576 616c  g, predict, eval
+00000f20: 7561 7465 2c20 666f 7220 6578 616d 706c  uate, for exampl
+00000f30: 6520 5b65 7861 6d70 6c65 732f 6c72 5f65  e [examples/lr_e
+00000f40: 6e5f 636c 6173 7369 6669 6361 7469 6f6e  n_classification
+00000f50: 5f64 656d 6f2e 7079 5d28 6874 7470 733a  _demo.py](https:
+00000f60: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6869  //github.com/shi
+00000f70: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
+00000f80: 6173 7369 6669 6572 2f62 6c6f 622f 6d61  assifier/blob/ma
+00000f90: 7374 6572 2f65 7861 6d70 6c65 732f 6c72  ster/examples/lr
+00000fa0: 5f65 6e5f 636c 6173 7369 6669 6361 7469  _en_classificati
+00000fb0: 6f6e 5f64 656d 6f2e 7079 293a 0a20 2020  on_demo.py):.   
+00000fc0: 2020 2020 200a 2020 2020 2020 2020 6060       .        ``
+00000fd0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00000fe0: 696d 706f 7274 2073 7973 0a20 2020 2020  import sys.     
+00000ff0: 2020 200a 2020 2020 2020 2020 7379 732e     .        sys.
+00001000: 7061 7468 2e61 7070 656e 6428 272e 2e27  path.append('..'
+00001010: 290a 2020 2020 2020 2020 6672 6f6d 2070  ).        from p
+00001020: 7974 6578 7463 6c61 7373 6966 6965 7220  ytextclassifier 
+00001030: 696d 706f 7274 2043 6c61 7373 6963 436c  import ClassicCl
+00001040: 6173 7369 6669 6572 0a20 2020 2020 2020  assifier.       
+00001050: 200a 2020 2020 2020 2020 6966 205f 5f6e   .        if __n
+00001060: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
+00001070: 5f5f 273a 0a20 2020 2020 2020 2020 2020  __':.           
+00001080: 206d 203d 2043 6c61 7373 6963 436c 6173   m = ClassicClas
+00001090: 7369 6669 6572 286f 7574 7075 745f 6469  sifier(output_di
+000010a0: 723d 276d 6f64 656c 732f 6c72 272c 206d  r='models/lr', m
+000010b0: 6f64 656c 5f6e 616d 655f 6f72 5f6d 6f64  odel_name_or_mod
+000010c0: 656c 3d27 6c72 2729 0a20 2020 2020 2020  el='lr').       
+000010d0: 2020 2020 2023 2043 6c61 7373 6963 436c       # ClassicCl
+000010e0: 6173 7369 6669 6572 2073 7570 706f 7274  assifier support
+000010f0: 206d 6f64 656c 5f6e 616d 65ef bc9a 6c72   model_name...lr
+00001100: 2c20 7261 6e64 6f6d 5f66 6f72 6573 742c  , random_forest,
+00001110: 2064 6563 6973 696f 6e5f 7472 6565 2c20   decision_tree, 
+00001120: 6b6e 6e2c 2062 6179 6573 2c20 7376 6d2c  knn, bayes, svm,
+00001130: 2078 6762 6f6f 7374 0a20 2020 2020 2020   xgboost.       
+00001140: 2020 2020 2070 7269 6e74 286d 290a 2020       print(m).  
+00001150: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00001160: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00001170: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+00001180: 2027 5374 7564 656e 7420 6465 6274 2074   'Student debt t
+00001190: 6f20 636f 7374 2042 7269 7461 696e 2062  o cost Britain b
+000011a0: 696c 6c69 6f6e 7320 7769 7468 696e 2064  illions within d
+000011b0: 6563 6164 6573 2729 2c0a 2020 2020 2020  ecades'),.      
+000011c0: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
+000011d0: 6174 696f 6e27 2c20 2743 6869 6e65 7365  ation', 'Chinese
+000011e0: 2065 6475 6361 7469 6f6e 2066 6f72 2054   education for T
+000011f0: 5620 6578 7065 7269 6d65 6e74 2729 2c0a  V experiment'),.
+00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001210: 2827 7370 6f72 7473 272c 2027 4d69 6464  ('sports', 'Midd
+00001220: 6c65 2045 6173 7420 616e 6420 4173 6961  le East and Asia
+00001230: 2062 6f6f 7374 2069 6e76 6573 746d 656e   boost investmen
+00001240: 7420 696e 2074 6f70 206c 6576 656c 2073  t in top level s
+00001250: 706f 7274 7327 292c 0a20 2020 2020 2020  ports'),.       
+00001260: 2020 2020 2020 2020 2028 2773 706f 7274           ('sport
+00001270: 7327 2c20 2753 756d 6d69 7420 5365 7269  s', 'Summit Seri
+00001280: 6573 206c 6f6f 6b20 6c61 756e 6368 6573  es look launches
+00001290: 2048 424f 2043 616e 6164 6120 7370 6f72   HBO Canada spor
+000012a0: 7473 2064 6f63 2073 6572 6965 733a 204d  ts doc series: M
+000012b0: 7564 6861 7227 290a 2020 2020 2020 2020  udhar').        
+000012c0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+000012d0: 2020 2320 7472 6169 6e20 616e 6420 7361    # train and sa
+000012e0: 7665 2062 6573 7420 6d6f 6465 6c0a 2020  ve best model.  
+000012f0: 2020 2020 2020 2020 2020 6d2e 7472 6169            m.trai
+00001300: 6e28 6461 7461 290a 2020 2020 2020 2020  n(data).        
+00001310: 2020 2020 2320 6c6f 6164 2062 6573 7420      # load best 
+00001320: 6d6f 6465 6c20 6672 6f6d 206d 6f64 656c  model from model
+00001330: 5f64 6972 0a20 2020 2020 2020 2020 2020  _dir.           
+00001340: 206d 2e6c 6f61 645f 6d6f 6465 6c28 290a   m.load_model().
+00001350: 2020 2020 2020 2020 2020 2020 7072 6564              pred
+00001360: 6963 745f 6c61 6265 6c2c 2070 7265 6469  ict_label, predi
+00001370: 6374 5f70 726f 6261 203d 206d 2e70 7265  ct_proba = m.pre
+00001380: 6469 6374 285b 0a20 2020 2020 2020 2020  dict([.         
+00001390: 2020 2020 2020 2027 4162 626f 7474 2067         'Abbott g
+000013a0: 6f76 6572 6e6d 656e 7420 7370 656e 6473  overnment spends
+000013b0: 2024 3820 6d69 6c6c 696f 6e20 6f6e 2068   $8 million on h
+000013c0: 6967 6865 7220 6564 7563 6174 696f 6e20  igher education 
+000013d0: 6d65 6469 6120 626c 6974 7a27 5d29 0a20  media blitz']). 
+000013e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000013f0: 2866 2770 7265 6469 6374 5f6c 6162 656c  (f'predict_label
+00001400: 3a20 7b70 7265 6469 6374 5f6c 6162 656c  : {predict_label
+00001410: 7d2c 2070 7265 6469 6374 5f70 726f 6261  }, predict_proba
+00001420: 3a20 7b70 7265 6469 6374 5f70 726f 6261  : {predict_proba
+00001430: 7d27 290a 2020 2020 2020 2020 0a20 2020  }').        .   
+00001440: 2020 2020 2020 2020 2074 6573 745f 6461           test_da
+00001450: 7461 203d 205b 0a20 2020 2020 2020 2020  ta = [.         
+00001460: 2020 2020 2020 2028 2765 6475 6361 7469         ('educati
+00001470: 6f6e 272c 2027 4162 626f 7474 2067 6f76  on', 'Abbott gov
+00001480: 6572 6e6d 656e 7420 7370 656e 6473 2024  ernment spends $
+00001490: 3820 6d69 6c6c 696f 6e20 6f6e 2068 6967  8 million on hig
+000014a0: 6865 7220 6564 7563 6174 696f 6e20 6d65  her education me
+000014b0: 6469 6120 626c 6974 7a27 292c 0a20 2020  dia blitz'),.   
+000014c0: 2020 2020 2020 2020 2020 2020 2028 2773               ('s
+000014d0: 706f 7274 7327 2c20 274d 6964 646c 6520  ports', 'Middle 
+000014e0: 4561 7374 2061 6e64 2041 7369 6120 626f  East and Asia bo
+000014f0: 6f73 7420 696e 7665 7374 6d65 6e74 2069  ost investment i
+00001500: 6e20 746f 7020 6c65 7665 6c20 7370 6f72  n top level spor
+00001510: 7473 2729 2c0a 2020 2020 2020 2020 2020  ts'),.          
+00001520: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00001530: 6163 635f 7363 6f72 6520 3d20 6d2e 6576  acc_score = m.ev
+00001540: 616c 7561 7465 5f6d 6f64 656c 2874 6573  aluate_model(tes
+00001550: 745f 6461 7461 290a 2020 2020 2020 2020  t_data).        
+00001560: 2020 2020 7072 696e 7428 6627 6163 635f      print(f'acc_
+00001570: 7363 6f72 653a 207b 6163 635f 7363 6f72  score: {acc_scor
+00001580: 657d 2729 0a20 2020 2020 2020 2060 6060  e}').        ```
+00001590: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000015a0: 2020 6f75 7470 7574 3a0a 2020 2020 2020    output:.      
+000015b0: 2020 0a20 2020 2020 2020 2060 6060 0a20    .        ```. 
+000015c0: 2020 2020 2020 2043 6c61 7373 6963 436c         ClassicCl
+000015d0: 6173 7369 6669 6572 2069 6e73 7461 6e63  assifier instanc
+000015e0: 6520 284c 6f67 6973 7469 6352 6567 7265  e (LogisticRegre
+000015f0: 7373 696f 6e28 6669 745f 696e 7465 7263  ssion(fit_interc
+00001600: 6570 743d 4661 6c73 6529 2c20 7374 6f70  ept=False), stop
+00001610: 776f 7264 7320 7369 7a65 3a20 3234 3338  words size: 2438
+00001620: 290a 2020 2020 2020 2020 7072 6564 6963  ).        predic
+00001630: 745f 6c61 6265 6c3a 205b 2765 6475 6361  t_label: ['educa
+00001640: 7469 6f6e 275d 2c20 7072 6564 6963 745f  tion'], predict_
+00001650: 7072 6f62 613a 205b 302e 3533 3738 3233  proba: [0.537823
+00001660: 3633 3538 3439 3231 3132 5d0a 2020 2020  6358492112].    
+00001670: 2020 2020 6163 635f 7363 6f72 653a 2031      acc_score: 1
+00001680: 2e30 0a20 2020 2020 2020 2060 6060 0a20  .0.        ```. 
+00001690: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000016a0: 2323 2320 4368 696e 6573 6520 5465 7874  ### Chinese Text
+000016b0: 2043 6c61 7373 6966 6965 7228 e4b8 ade6   Classifier(....
+000016c0: 9687 e696 87e6 9cac e588 86e7 b1bb 290a  ..............).
+000016d0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000016e0: 2054 6578 7420 636c 6173 7369 6669 6361   Text classifica
+000016f0: 7469 6f6e 2063 6f6d 7061 7469 626c 6520  tion compatible 
+00001700: 7769 7468 2043 6869 6e65 7365 2061 6e64  with Chinese and
+00001710: 2045 6e67 6c69 7368 2063 6f72 706f 7261   English corpora
+00001720: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00001730: 2020 2065 7861 6d70 6c65 205b 6578 616d     example [exam
+00001740: 706c 6573 2f6c 725f 636c 6173 7369 6669  ples/lr_classifi
+00001750: 6361 7469 6f6e 5f64 656d 6f2e 7079 5d28  cation_demo.py](
+00001760: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001770: 6f6d 2f73 6869 6269 6e67 3632 342f 7079  om/shibing624/py
+00001780: 7465 7874 636c 6173 7369 6669 6572 2f62  textclassifier/b
+00001790: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
+000017a0: 6c65 732f 6c72 5f63 6c61 7373 6966 6963  les/lr_classific
+000017b0: 6174 696f 6e5f 6465 6d6f 2e70 7929 0a20  ation_demo.py). 
+000017c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000017d0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+000017e0: 2020 696d 706f 7274 2073 7973 0a20 2020    import sys.   
+000017f0: 2020 2020 200a 2020 2020 2020 2020 7379       .        sy
+00001800: 732e 7061 7468 2e61 7070 656e 6428 272e  s.path.append('.
+00001810: 2e27 290a 2020 2020 2020 2020 6672 6f6d  .').        from
+00001820: 2070 7974 6578 7463 6c61 7373 6966 6965   pytextclassifie
+00001830: 7220 696d 706f 7274 2043 6c61 7373 6963  r import Classic
+00001840: 436c 6173 7369 6669 6572 0a20 2020 2020  Classifier.     
+00001850: 2020 200a 2020 2020 2020 2020 6966 205f     .        if _
+00001860: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00001870: 696e 5f5f 273a 0a20 2020 2020 2020 2020  in__':.         
+00001880: 2020 206d 203d 2043 6c61 7373 6963 436c     m = ClassicCl
+00001890: 6173 7369 6669 6572 286f 7574 7075 745f  assifier(output_
+000018a0: 6469 723d 276d 6f64 656c 732f 6c72 2d74  dir='models/lr-t
+000018b0: 6f79 272c 206d 6f64 656c 5f6e 616d 655f  oy', model_name_
+000018c0: 6f72 5f6d 6f64 656c 3d27 6c72 2729 0a20  or_model='lr'). 
+000018d0: 2020 2020 2020 2020 2020 2023 20e7 bb8f             # ...
+000018e0: e585 b8e5 8886 e7b1 bbe6 96b9 e6b3 95ef  ................
+000018f0: bc8c e694 afe6 8c81 e79a 84e6 a8a1 e59e  ................
+00001900: 8be5 8c85 e68b acef bc9a 6c72 2c20 7261  ..........lr, ra
+00001910: 6e64 6f6d 5f66 6f72 6573 742c 2064 6563  ndom_forest, dec
+00001920: 6973 696f 6e5f 7472 6565 2c20 6b6e 6e2c  ision_tree, knn,
+00001930: 2062 6179 6573 2c20 7376 6d2c 2078 6762   bayes, svm, xgb
+00001940: 6f6f 7374 0a20 2020 2020 2020 2020 2020  oost.           
+00001950: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
+00001960: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
+00001970: 6174 696f 6e27 2c20 27e5 908d e5b8 88e6  ation', '.......
+00001980: 8c87 e5af bce6 8998 e7a6 8fe8 afad e6b3  ................
+00001990: 95e6 8a80 e5b7 a7ef bc9a e590 8de8 af8d  ................
+000019a0: e79a 84e5 a48d e695 b0e5 bda2 e5bc 8f27  ...............'
+000019b0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000019c0: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+000019d0: 2027 e4b8 ade5 9bbd e9ab 98e8 8083 e688   '..............
+000019e0: 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5 8faf  ................
+000019f0: 20e6 98af e280 9ce7 8bbc e69d a5e4 ba86   ...............
+00001a00: e280 9de5 9097 efbc 9f27 292c 0a20 2020  .........'),.   
+00001a10: 2020 2020 2020 2020 2020 2020 2028 2765               ('e
+00001a20: 6475 6361 7469 6f6e 272c 2027 e585 ace5  ducation', '....
+00001a30: 8aa1 e591 98e8 8083 e899 91e8 b68a e69d  ................
+00001a40: a5e8 b68a e590 83e9 a699 efbc 8ce8 bf99  ................
+00001a50: e698 afe6 808e e4b9 88e5 9b9e e4ba 8bef  ................
+00001a60: bc9f 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
+00001a70: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
+00001a80: 2027 e59b bee6 9687 efbc 9ae6 b395 e7bd   '..............
+00001a90: 91e5 ad9f e88f b2e5 b094 e696 afe8 8ba6  ................
+00001aa0: e688 98e8 bf9b 3136 e5bc ba20 e5ad 9fe8  ......16... ....
+00001ab0: 8fb2 e5b0 94e6 96af e680 92e5 90bc 2729  ..............')
+00001ac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001ad0: 2020 2827 7370 6f72 7473 272c 2027 e59b    ('sports', '..
+00001ae0: 9be5 b79d e4b8 b9e6 a3b1 e4b8 bee8 a18c  ................
+00001af0: e585 a8e5 9bbd e995 bfe8 b79d e799 bbe5  ................
+00001b00: b1b1 e68c 91e6 8898 e8b5 9b20 e8bf 91e4  ........... ....
+00001b10: b887 e4ba bae5 8f82 e4b8 8e27 292c 0a20  ...........'),. 
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00001b30: 2773 706f 7274 7327 2c20 27e7 b1b3 e585  'sports', '.....
+00001b40: b0e5 aea2 e59c ba38 e688 98e4 b88d e8b4  .......8........
+00001b50: a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8  .......10.......
+00001b60: 839c 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
+00001b70: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00001b80: 6d2e 7472 6169 6e28 6461 7461 290a 2020  m.train(data).  
+00001b90: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00001ba0: 6d29 0a20 2020 2020 2020 2020 2020 2023  m).            #
+00001bb0: 206c 6f61 6420 6265 7374 206d 6f64 656c   load best model
+00001bc0: 2066 726f 6d20 6d6f 6465 6c5f 6469 720a   from model_dir.
+00001bd0: 2020 2020 2020 2020 2020 2020 6d2e 6c6f              m.lo
+00001be0: 6164 5f6d 6f64 656c 2829 0a20 2020 2020  ad_model().     
+00001bf0: 2020 2020 2020 2070 7265 6469 6374 5f6c         predict_l
+00001c00: 6162 656c 2c20 7072 6564 6963 745f 7072  abel, predict_pr
+00001c10: 6f62 6120 3d20 6d2e 7072 6564 6963 7428  oba = m.predict(
+00001c20: 5b27 e7a6 8fe5 bbba e698 a5e5 ada3 e585  ['..............
+00001c30: ace5 8aa1 e591 98e8 8083 e8af 95e6 8aa5  ................
+00001c40: e590 8d31 38e6 97a5 e688 aae6 ada2 2032  ...18......... 2
+00001c50: e69c 8836 e697 a5e8 8083 e8af 9527 2c0a  ...6.........',.
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 27e6 848f e794 b2e9 a696        '.........
+00001ca0: e8bd aee8 a1a5 e8b5 9be4 baa4 e688 98e8  ................
+00001cb0: aeb0 e5bd 953a e7b1 b3e5 85b0 e5ae a2e5  .....:..........
+00001cc0: 9cba 38e6 8898 e4b8 8de8 b4a5 e59b bde7  ..8.............
+00001cd0: b1b3 3130 e5b9 b4e8 bf9e e883 9c27 5d29  ..10.........'])
+00001ce0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00001cf0: 6e74 2866 2770 7265 6469 6374 5f6c 6162  nt(f'predict_lab
+00001d00: 656c 3a20 7b70 7265 6469 6374 5f6c 6162  el: {predict_lab
+00001d10: 656c 7d2c 2070 7265 6469 6374 5f70 726f  el}, predict_pro
+00001d20: 6261 3a20 7b70 7265 6469 6374 5f70 726f  ba: {predict_pro
+00001d30: 6261 7d27 290a 2020 2020 2020 2020 0a20  ba}').        . 
+00001d40: 2020 2020 2020 2020 2020 2074 6573 745f             test_
+00001d50: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
+00001d60: 2020 2020 2020 2020 2028 2765 6475 6361           ('educa
+00001d70: 7469 6f6e 272c 2027 e7a6 8fe5 bbba e698  tion', '........
+00001d80: a5e5 ada3 e585 ace5 8aa1 e591 98e8 8083  ................
+00001d90: e8af 95e6 8aa5 e590 8d31 38e6 97a5 e688  .........18.....
+00001da0: aae6 ada2 2032 e69c 8836 e697 a5e8 8083  .... 2...6......
+00001db0: e8af 9527 292c 0a20 2020 2020 2020 2020  ...'),.         
+00001dc0: 2020 2020 2020 2028 2773 706f 7274 7327         ('sports'
+00001dd0: 2c20 27e6 848f e794 b2e9 a696 e8bd aee8  , '.............
+00001de0: a1a5 e8b5 9be4 baa4 e688 98e8 aeb0 e5bd  ................
+00001df0: 953a e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6  .:............8.
+00001e00: 8898 e4b8 8de8 b4a5 e59b bde7 b1b3 3130  ..............10
+00001e10: e5b9 b4e8 bf9e e883 9c27 292c 0a20 2020  .........'),.   
+00001e20: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00001e30: 2020 2020 2020 2061 6363 5f73 636f 7265         acc_score
+00001e40: 203d 206d 2e65 7661 6c75 6174 655f 6d6f   = m.evaluate_mo
+00001e50: 6465 6c28 7465 7374 5f64 6174 6129 0a20  del(test_data). 
+00001e60: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00001e70: 2866 2761 6363 5f73 636f 7265 3a20 7b61  (f'acc_score: {a
+00001e80: 6363 5f73 636f 7265 7d27 2920 2023 2031  cc_score}')  # 1
+00001e90: 2e30 0a20 2020 2020 2020 200a 2020 2020  .0.        .    
+00001ea0: 2020 2020 2020 2020 2323 2323 2074 7261          #### tra
+00001eb0: 696e 206d 6f64 656c 2077 6974 6820 3177  in model with 1w
+00001ec0: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+00001ed0: 2020 7072 696e 7428 272d 2720 2a20 3432    print('-' * 42
+00001ee0: 290a 2020 2020 2020 2020 2020 2020 6d20  ).            m 
+00001ef0: 3d20 436c 6173 7369 6343 6c61 7373 6966  = ClassicClassif
+00001f00: 6965 7228 6f75 7470 7574 5f64 6972 3d27  ier(output_dir='
+00001f10: 6d6f 6465 6c73 2f6c 7227 2c20 6d6f 6465  models/lr', mode
+00001f20: 6c5f 6e61 6d65 5f6f 725f 6d6f 6465 6c3d  l_name_or_model=
+00001f30: 276c 7227 290a 2020 2020 2020 2020 2020  'lr').          
+00001f40: 2020 6461 7461 5f66 696c 6520 3d20 2774    data_file = 't
+00001f50: 6875 636e 6577 735f 7472 6169 6e5f 3177  hucnews_train_1w
+00001f60: 2e74 7874 270a 2020 2020 2020 2020 2020  .txt'.          
+00001f70: 2020 6d2e 7472 6169 6e28 6461 7461 5f66    m.train(data_f
+00001f80: 696c 6529 0a20 2020 2020 2020 2020 2020  ile).           
+00001f90: 206d 2e6c 6f61 645f 6d6f 6465 6c28 290a   m.load_model().
+00001fa0: 2020 2020 2020 2020 2020 2020 7072 6564              pred
+00001fb0: 6963 745f 6c61 6265 6c2c 2070 7265 6469  ict_label, predi
+00001fc0: 6374 5f70 726f 6261 203d 206d 2e70 7265  ct_proba = m.pre
+00001fd0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
+00001fe0: 2020 2020 2020 5b27 e9a1 bae4 b989 e58c        ['........
+00001ff0: 97e4 baac e88b 8fe6 b4bb 3838 e5b9 b3e7  ..........88....
+00002000: b1b3 e8b5 b7e7 b2be e8a3 85e6 88bf e59c  ................
+00002010: a8e5 94ae 272c 0a20 2020 2020 2020 2020  ....',.         
+00002020: 2020 2020 2020 2020 27e7 be8e 4542 2d35          '...EB-5
+00002030: e9a1 b9e7 9bae e280 9c31 35e6 97a5 e5bf  .........15.....
+00002040: abe9 809f e7a7 bbe6 b091 e280 9de5 b086  ................
+00002050: e68e a8e8 bf9f 275d 290a 2020 2020 2020  ......']).      
+00002060: 2020 2020 2020 7072 696e 7428 6627 7072        print(f'pr
+00002070: 6564 6963 745f 6c61 6265 6c3a 207b 7072  edict_label: {pr
+00002080: 6564 6963 745f 6c61 6265 6c7d 2c20 7072  edict_label}, pr
+00002090: 6564 6963 745f 7072 6f62 613a 207b 7072  edict_proba: {pr
+000020a0: 6564 6963 745f 7072 6f62 617d 2729 0a20  edict_proba}'). 
+000020b0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+000020c0: 2020 200a 2020 2020 2020 2020 6f75 7470     .        outp
+000020d0: 7574 3a0a 2020 2020 2020 2020 0a20 2020  ut:.        .   
+000020e0: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+000020f0: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
+00002100: 6572 2069 6e73 7461 6e63 6520 284c 6f67  er instance (Log
+00002110: 6973 7469 6352 6567 7265 7373 696f 6e28  isticRegression(
+00002120: 6669 745f 696e 7465 7263 6570 743d 4661  fit_intercept=Fa
+00002130: 6c73 6529 2c20 7374 6f70 776f 7264 7320  lse), stopwords 
+00002140: 7369 7a65 3a20 3234 3338 290a 2020 2020  size: 2438).    
+00002150: 2020 2020 7072 6564 6963 745f 6c61 6265      predict_labe
+00002160: 6c3a 205b 2765 6475 6361 7469 6f6e 2720  l: ['education' 
+00002170: 2773 706f 7274 7327 5d2c 2070 7265 6469  'sports'], predi
+00002180: 6374 5f70 726f 6261 3a20 5b30 2e35 2c20  ct_proba: [0.5, 
+00002190: 302e 3539 3839 3431 3830 3637 3431 3533  0.59894180674153
+000021a0: 345d 0a20 2020 2020 2020 2061 6363 5f73  4].        acc_s
+000021b0: 636f 7265 3a20 312e 300a 2020 2020 2020  core: 1.0.      
+000021c0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+000021d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000021e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+000021f0: 2020 2020 2070 7265 6469 6374 5f6c 6162       predict_lab
+00002200: 656c 3a20 5b27 7265 616c 7479 2720 2765  el: ['realty' 'e
+00002210: 6475 6361 7469 6f6e 275d 2c20 7072 6564  ducation'], pred
+00002220: 6963 745f 7072 6f62 613a 205b 302e 3733  ict_proba: [0.73
+00002230: 3032 3935 3639 3233 3631 3733 3732 2c20  02956923617372, 
+00002240: 302e 3235 3635 3030 3534 3435 3332 3239  0.25650054453229
+00002250: 3233 5d0a 2020 2020 2020 2020 6060 600a  23].        ```.
+00002260: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00002270: 2023 2323 2056 6973 7561 6c20 4665 6174   ### Visual Feat
+00002280: 7572 6520 496d 706f 7274 616e 6365 0a20  ure Importance. 
+00002290: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000022a0: 5368 6f77 2066 6561 7475 7265 2077 6569  Show feature wei
+000022b0: 6768 7473 206f 6620 6d6f 6465 6c2c 2061  ghts of model, a
+000022c0: 6e64 2070 7265 6469 6374 696f 6e20 776f  nd prediction wo
+000022d0: 7264 2077 6569 6768 742c 2066 6f72 2065  rd weight, for e
+000022e0: 7861 6d70 6c65 205b 6578 616d 706c 6573  xample [examples
+000022f0: 2f76 6973 7561 6c5f 6665 6174 7572 655f  /visual_feature_
+00002300: 696d 706f 7274 616e 6365 2e69 7079 6e62  importance.ipynb
+00002310: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002320: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
+00002330: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00002340: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00002350: 6d70 6c65 732f 7669 7375 616c 5f66 6561  mples/visual_fea
+00002360: 7475 7265 5f69 6d70 6f72 7461 6e63 652e  ture_importance.
+00002370: 6970 796e 6229 0a20 2020 2020 2020 200a  ipynb).        .
+00002380: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00002390: 6e0a 2020 2020 2020 2020 696d 706f 7274  n.        import
+000023a0: 2073 7973 0a20 2020 2020 2020 200a 2020   sys.        .  
+000023b0: 2020 2020 2020 7379 732e 7061 7468 2e61        sys.path.a
+000023c0: 7070 656e 6428 272e 2e27 290a 2020 2020  ppend('..').    
+000023d0: 2020 2020 6672 6f6d 2070 7974 6578 7463      from pytextc
+000023e0: 6c61 7373 6966 6965 7220 696d 706f 7274  lassifier import
+000023f0: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
+00002400: 6572 0a20 2020 2020 2020 2069 6d70 6f72  er.        impor
+00002410: 7420 6a69 6562 610a 2020 2020 2020 2020  t jieba.        
+00002420: 0a20 2020 2020 2020 2074 6320 3d20 436c  .        tc = Cl
+00002430: 6173 7369 6343 6c61 7373 6966 6965 7228  assicClassifier(
+00002440: 6f75 7470 7574 5f64 6972 3d27 6d6f 6465  output_dir='mode
+00002450: 6c73 2f6c 722d 746f 7927 2c20 6d6f 6465  ls/lr-toy', mode
+00002460: 6c5f 6e61 6d65 5f6f 725f 6d6f 6465 6c3d  l_name_or_model=
+00002470: 276c 7227 290a 2020 2020 2020 2020 6461  'lr').        da
+00002480: 7461 203d 205b 0a20 2020 2020 2020 2020  ta = [.         
+00002490: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+000024a0: 2027 e590 8de5 b888 e68c 87e5 afbc e689   '..............
+000024b0: 98e7 a68f e8af ade6 b395 e68a 80e5 b7a7  ................
+000024c0: efbc 9ae5 908d e8af 8de7 9a84 e5a4 8de6  ................
+000024d0: 95b0 e5bd a2e5 bc8f 2729 2c0a 2020 2020  ........'),.    
+000024e0: 2020 2020 2020 2020 2827 6564 7563 6174          ('educat
+000024f0: 696f 6e27 2c20 27e4 b8ad e59b bde9 ab98  ion', '.........
+00002500: e880 83e6 8890 e7bb a9e6 b5b7 e5a4 96e8  ................
+00002510: aea4 e58f af20 e698 afe2 809c e78b bce6  ..... ..........
+00002520: 9da5 e4ba 86e2 809d e590 97ef bc9f 2729  ..............')
+00002530: 2c0a 2020 2020 2020 2020 2020 2020 2827  ,.            ('
+00002540: 7370 6f72 7473 272c 2027 e59b bee6 9687  sports', '......
+00002550: efbc 9ae6 b395 e7bd 91e5 ad9f e88f b2e5  ................
+00002560: b094 e696 afe8 8ba6 e688 98e8 bf9b 3136  ..............16
+00002570: e5bc ba20 e5ad 9fe8 8fb2 e5b0 94e6 96af  ... ............
+00002580: e680 92e5 90bc 2729 2c0a 2020 2020 2020  ......'),.      
+00002590: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
+000025a0: 2027 e59b 9be5 b79d e4b8 b9e6 a3b1 e4b8   '..............
+000025b0: bee8 a18c e585 a8e5 9bbd e995 bfe8 b79d  ................
+000025c0: e799 bbe5 b1b1 e68c 91e6 8898 e8b5 9b20  ............... 
+000025d0: e8bf 91e4 b887 e4ba bae5 8f82 e4b8 8e27  ...............'
+000025e0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+000025f0: 2773 706f 7274 7327 2c20 27e7 b1b3 e585  'sports', '.....
+00002600: b0e5 aea2 e59c ba38 e688 98e4 b88d e8b4  .......8........
+00002610: a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8  .......10.......
+00002620: 839c 2729 0a20 2020 2020 2020 205d 0a20  ..').        ]. 
+00002630: 2020 2020 2020 2074 632e 7472 6169 6e28         tc.train(
+00002640: 6461 7461 290a 2020 2020 2020 2020 696d  data).        im
+00002650: 706f 7274 2065 6c69 350a 2020 2020 2020  port eli5.      
+00002660: 2020 0a20 2020 2020 2020 2069 6e66 6572    .        infer
+00002670: 5f64 6174 6120 3d20 5b27 e9ab 98e8 8083  _data = ['......
+00002680: e68c 87e5 afbc e689 98e7 a68f e8af ade6  ................
+00002690: b395 e68a 80e5 b7a7 e59b bde9 9985 e8ae  ................
+000026a0: a4e5 8faf 272c 0a20 2020 2020 2020 2020  ....',.         
+000026b0: 2020 2020 2020 2020 2020 2020 2027 e684               '..
+000026c0: 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b  ................
+000026d0: e4ba a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3  ............:...
+000026e0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+000026f0: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+00002700: 9ee8 839c 275d 0a20 2020 2020 2020 2065  ....'].        e
+00002710: 6c69 352e 7368 6f77 5f77 6569 6768 7473  li5.show_weights
+00002720: 2874 632e 6d6f 6465 6c2c 2076 6563 3d74  (tc.model, vec=t
+00002730: 632e 6665 6174 7572 6529 0a20 2020 2020  c.feature).     
+00002740: 2020 2073 6567 5f69 6e66 6572 5f64 6174     seg_infer_dat
+00002750: 6120 3d20 5b27 2027 2e6a 6f69 6e28 6a69  a = [' '.join(ji
+00002760: 6562 612e 6c63 7574 2869 2929 2066 6f72  eba.lcut(i)) for
+00002770: 2069 2069 6e20 696e 6665 725f 6461 7461   i in infer_data
+00002780: 5d0a 2020 2020 2020 2020 656c 6935 2e73  ].        eli5.s
+00002790: 686f 775f 7072 6564 6963 7469 6f6e 2874  how_prediction(t
+000027a0: 632e 6d6f 6465 6c2c 2073 6567 5f69 6e66  c.model, seg_inf
+000027b0: 6572 5f64 6174 615b 305d 2c20 7665 633d  er_data[0], vec=
+000027c0: 7463 2e66 6561 7475 7265 2c0a 2020 2020  tc.feature,.    
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027e0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+000027f0: 6e61 6d65 733d 5b27 6564 7563 6174 696f  names=['educatio
+00002800: 6e27 2c20 2773 706f 7274 7327 5d29 0a20  n', 'sports']). 
+00002810: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00002820: 2020 200a 2020 2020 2020 2020 6f75 7470     .        outp
+00002830: 7574 3a0a 2020 2020 2020 2020 0a20 2020  ut:.        .   
+00002840: 2020 2020 2021 5b69 6d67 2e70 6e67 5d28       ![img.png](
+00002850: 646f 6373 2f69 6d67 2e70 6e67 290a 2020  docs/img.png).  
+00002860: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00002870: 2323 2044 6565 7020 436c 6173 7369 6669  ## Deep Classifi
+00002880: 6361 7469 6f6e 206d 6f64 656c 0a20 2020  cation model.   
+00002890: 2020 2020 200a 2020 2020 2020 2020 e69c       .        ..
+000028a0: ace9 a1b9 e79b aee6 94af e68c 81e4 bba5  ................
+000028b0: e4b8 8be6 b7b1 e5ba a6e5 8886 e7b1 bbe6  ................
+000028c0: a8a1 e59e 8bef bc9a 4661 7374 5465 7874  ........FastText
+000028d0: e380 8154 6578 7443 4e4e e380 8154 6578  ...TextCNN...Tex
+000028e0: 7452 4e4e e380 8142 6572 74e6 a8a1 e59e  tRNN...Bert.....
+000028f0: 8bef bc8c 6069 6d70 6f72 7460 e6a8 a1e5  ....`import`....
+00002900: 9e8b e5af b9e5 ba94 e79a 84e6 96b9 e6b3  ................
+00002910: 95e6 9da5 e8b0 83e7 94a8 efbc 9a0a 2020  ..............  
+00002920: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00002930: 2020 2020 2020 2020 6672 6f6d 2070 7974          from pyt
+00002940: 6578 7463 6c61 7373 6966 6965 7220 696d  extclassifier im
+00002950: 706f 7274 2046 6173 7454 6578 7443 6c61  port FastTextCla
+00002960: 7373 6966 6965 722c 2054 6578 7443 4e4e  ssifier, TextCNN
+00002970: 436c 6173 7369 6669 6572 2c20 5465 7874  Classifier, Text
+00002980: 524e 4e43 6c61 7373 6966 6965 722c 2042  RNNClassifier, B
+00002990: 6572 7443 6c61 7373 6966 6965 720a 2020  ertClassifier.  
+000029a0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+000029b0: 2020 0a20 2020 2020 2020 20e4 b88b e99d    .        .....
+000029c0: a2e4 bba5 4661 7374 5465 7874 e6a8 a1e5  ....FastText....
+000029d0: 9e8b e4b8 bae7 a4ba e4be 8bef bc8c e585  ................
+000029e0: b6e4 bb96 e6a8 a1e5 9e8b e79a 84e4 bdbf  ................
+000029f0: e794 a8e6 96b9 e6b3 95e7 b1bb e4bc bce3  ................
+00002a00: 8082 0a20 2020 2020 2020 200a 2020 2020  ...        .    
+00002a10: 2020 2020 2323 2320 4661 7374 5465 7874      ### FastText
+00002a20: 20e6 a8a1 e59e 8b0a 2020 2020 2020 2020   .......        
+00002a30: 0a20 2020 2020 2020 20e8 aead e7bb 83e5  .        .......
+00002a40: 928c e9a2 84e6 b58b 6046 6173 7454 6578  ........`FastTex
+00002a50: 7460 e6a8 a1e5 9e8b e7a4 bae4 be8b 5b65  t`............[e
+00002a60: 7861 6d70 6c65 732f 6661 7374 7465 7874  xamples/fasttext
+00002a70: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
+00002a80: 6465 6d6f 2e70 795d 2868 7474 7073 3a2f  demo.py](https:/
+00002a90: 2f67 6974 6875 622e 636f 6d2f 7368 6962  /github.com/shib
+00002aa0: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
+00002ab0: 7373 6966 6965 722f 626c 6f62 2f6d 6173  ssifier/blob/mas
+00002ac0: 7465 722f 6578 616d 706c 6573 2f66 6173  ter/examples/fas
+00002ad0: 7474 6578 745f 636c 6173 7369 6669 6361  ttext_classifica
+00002ae0: 7469 6f6e 5f64 656d 6f2e 7079 290a 2020  tion_demo.py).  
+00002af0: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
+00002b00: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
+00002b10: 2069 6d70 6f72 7420 7379 730a 2020 2020   import sys.    
+00002b20: 2020 2020 0a20 2020 2020 2020 2073 7973      .        sys
+00002b30: 2e70 6174 682e 6170 7065 6e64 2827 2e2e  .path.append('..
+00002b40: 2729 0a20 2020 2020 2020 2066 726f 6d20  ').        from 
+00002b50: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00002b60: 2069 6d70 6f72 7420 4661 7374 5465 7874   import FastText
+00002b70: 436c 6173 7369 6669 6572 2c20 6c6f 6164  Classifier, load
+00002b80: 5f64 6174 610a 2020 2020 2020 2020 0a20  _data.        . 
+00002b90: 2020 2020 2020 2069 6620 5f5f 6e61 6d65         if __name
+00002ba0: 5f5f 203d 3d20 275f 5f6d 6169 6e5f 5f27  __ == '__main__'
+00002bb0: 3a0a 2020 2020 2020 2020 2020 2020 6d20  :.            m 
+00002bc0: 3d20 4661 7374 5465 7874 436c 6173 7369  = FastTextClassi
+00002bd0: 6669 6572 286f 7574 7075 745f 6469 723d  fier(output_dir=
+00002be0: 276d 6f64 656c 732f 6661 7374 7465 7874  'models/fasttext
+00002bf0: 2d74 6f79 2729 0a20 2020 2020 2020 2020  -toy').         
+00002c00: 2020 2064 6174 6120 3d20 5b0a 2020 2020     data = [.    
+00002c10: 2020 2020 2020 2020 2020 2020 2827 6564              ('ed
+00002c20: 7563 6174 696f 6e27 2c20 27e5 908d e5b8  ucation', '.....
+00002c30: 88e6 8c87 e5af bce6 8998 e7a6 8fe8 afad  ................
+00002c40: e6b3 95e6 8a80 e5b7 a7ef bc9a e590 8de8  ................
+00002c50: af8d e79a 84e5 a48d e695 b0e5 bda2 e5bc  ................
+00002c60: 8f27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
+00002c70: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
+00002c80: 272c 2027 e4b8 ade5 9bbd e9ab 98e8 8083  ', '............
+00002c90: e688 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5  ................
+00002ca0: 8faf 20e6 98af e280 9ce7 8bbc e69d a5e4  .. .............
+00002cb0: ba86 e280 9de5 9097 efbc 9f27 292c 0a20  ...........'),. 
+00002cc0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00002cd0: 2765 6475 6361 7469 6f6e 272c 2027 e585  'education', '..
+00002ce0: ace5 8aa1 e591 98e8 8083 e899 91e8 b68a  ................
+00002cf0: e69d a5e8 b68a e590 83e9 a699 efbc 8ce8  ................
+00002d00: bf99 e698 afe6 808e e4b9 88e5 9b9e e4ba  ................
+00002d10: 8bef bc9f 2729 2c0a 2020 2020 2020 2020  ....'),.        
+00002d20: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
+00002d30: 272c 2027 e59b bee6 9687 efbc 9ae6 b395  ', '............
+00002d40: e7bd 91e5 ad9f e88f b2e5 b094 e696 afe8  ................
+00002d50: 8ba6 e688 98e8 bf9b 3136 e5bc ba20 e5ad  ........16... ..
+00002d60: 9fe8 8fb2 e5b0 94e6 96af e680 92e5 90bc  ................
+00002d70: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00002d80: 2020 2020 2827 7370 6f72 7473 272c 2027      ('sports', '
+00002d90: e59b 9be5 b79d e4b8 b9e6 a3b1 e4b8 bee8  ................
+00002da0: a18c e585 a8e5 9bbd e995 bfe8 b79d e799  ................
+00002db0: bbe5 b1b1 e68c 91e6 8898 e8b5 9b20 e8bf  ............. ..
+00002dc0: 91e4 b887 e4ba bae5 8f82 e4b8 8e27 292c  .............'),
+00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002de0: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
+00002df0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+00002e00: e8b4 a5e4 bf9d e68c 81e8 bf9e e883 9c27  ...............'
+00002e10: 292c 0a20 2020 2020 2020 2020 2020 205d  ),.            ]
+00002e20: 0a20 2020 2020 2020 2020 2020 206d 2e74  .            m.t
+00002e30: 7261 696e 2864 6174 612c 206e 756d 5f65  rain(data, num_e
+00002e40: 706f 6368 733d 3329 0a20 2020 2020 2020  pochs=3).       
+00002e50: 2020 2020 2070 7269 6e74 286d 290a 2020       print(m).  
+00002e60: 2020 2020 2020 2020 2020 2320 6c6f 6164            # load
+00002e70: 2074 7261 696e 6564 2062 6573 7420 6d6f   trained best mo
+00002e80: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
+00002e90: 6d2e 6c6f 6164 5f6d 6f64 656c 2829 0a20  m.load_model(). 
+00002ea0: 2020 2020 2020 2020 2020 2070 7265 6469             predi
+00002eb0: 6374 5f6c 6162 656c 2c20 7072 6564 6963  ct_label, predic
+00002ec0: 745f 7072 6f62 6120 3d20 6d2e 7072 6564  t_proba = m.pred
+00002ed0: 6963 7428 5b27 e7a6 8fe5 bbba e698 a5e5  ict(['..........
+00002ee0: ada3 e585 ace5 8aa1 e591 98e8 8083 e8af  ................
+00002ef0: 95e6 8aa5 e590 8d31 38e6 97a5 e688 aae6  .......18.......
+00002f00: ada2 2032 e69c 8836 e697 a5e8 8083 e8af  .. 2...6........
+00002f10: 9527 2c0a 2020 2020 2020 2020 2020 2020  .',.            
+00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f40: 2020 2020 2020 2020 2020 27e6 848f e794            '.....
+00002f50: b2e9 a696 e8bd aee8 a1a5 e8b5 9be4 baa4  ................
+00002f60: e688 98e8 aeb0 e5bd 953a e7b1 b3e5 85b0  .........:......
+00002f70: e5ae a2e5 9cba 38e6 8898 e4b8 8de8 b4a5  ......8.........
+00002f80: e59b bde7 b1b3 3130 e5b9 b4e8 bf9e e883  ......10........
+00002f90: 9c27 5d29 0a20 2020 2020 2020 2020 2020  .']).           
+00002fa0: 2070 7269 6e74 2866 2770 7265 6469 6374   print(f'predict
+00002fb0: 5f6c 6162 656c 3a20 7b70 7265 6469 6374  _label: {predict
+00002fc0: 5f6c 6162 656c 7d2c 2070 7265 6469 6374  _label}, predict
+00002fd0: 5f70 726f 6261 3a20 7b70 7265 6469 6374  _proba: {predict
+00002fe0: 5f70 726f 6261 7d27 290a 2020 2020 2020  _proba}').      
+00002ff0: 2020 2020 2020 7465 7374 5f64 6174 6120        test_data 
+00003000: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00003010: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
+00003020: 2c20 27e7 a68f e5bb bae6 98a5 e5ad a3e5  , '.............
+00003030: 85ac e58a a1e5 9198 e880 83e8 af95 e68a  ................
+00003040: a5e5 908d 3138 e697 a5e6 88aa e6ad a220  ....18......... 
+00003050: 32e6 9c88 36e6 97a5 e880 83e8 af95 2729  2...6.........')
+00003060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003070: 2020 2827 7370 6f72 7473 272c 2027 e684    ('sports', '..
+00003080: 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b  ................
+00003090: e4ba a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3  ............:...
+000030a0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+000030b0: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+000030c0: 9ee8 839c 2729 2c0a 2020 2020 2020 2020  ....'),.        
+000030d0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+000030e0: 2020 6163 635f 7363 6f72 6520 3d20 6d2e    acc_score = m.
+000030f0: 6576 616c 7561 7465 5f6d 6f64 656c 2874  evaluate_model(t
+00003100: 6573 745f 6461 7461 290a 2020 2020 2020  est_data).      
+00003110: 2020 2020 2020 7072 696e 7428 6627 6163        print(f'ac
+00003120: 635f 7363 6f72 653a 207b 6163 635f 7363  c_score: {acc_sc
+00003130: 6f72 657d 2729 2020 2320 312e 300a 2020  ore}')  # 1.0.  
+00003140: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00003150: 2020 2023 2323 2320 7472 6169 6e20 6d6f     #### train mo
+00003160: 6465 6c20 7769 7468 2031 7720 6461 7461  del with 1w data
+00003170: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00003180: 6e74 2827 2d27 202a 2034 3229 0a20 2020  nt('-' * 42).   
+00003190: 2020 2020 2020 2020 2064 6174 615f 6669           data_fi
+000031a0: 6c65 203d 2027 7468 7563 6e65 7773 5f74  le = 'thucnews_t
+000031b0: 7261 696e 5f31 772e 7478 7427 0a20 2020  rain_1w.txt'.   
+000031c0: 2020 2020 2020 2020 206d 203d 2046 6173           m = Fas
+000031d0: 7454 6578 7443 6c61 7373 6966 6965 7228  tTextClassifier(
+000031e0: 6f75 7470 7574 5f64 6972 3d27 6d6f 6465  output_dir='mode
+000031f0: 6c73 2f66 6173 7474 6578 7427 290a 2020  ls/fasttext').  
+00003200: 2020 2020 2020 2020 2020 6d2e 7472 6169            m.trai
+00003210: 6e28 6461 7461 5f66 696c 652c 206e 616d  n(data_file, nam
+00003220: 6573 3d28 276c 6162 656c 7327 2c20 2774  es=('labels', 't
+00003230: 6578 7427 292c 206e 756d 5f65 706f 6368  ext'), num_epoch
+00003240: 733d 3329 0a20 2020 2020 2020 2020 2020  s=3).           
+00003250: 2023 206c 6f61 6420 6265 7374 2074 7261   # load best tra
+00003260: 696e 6564 206d 6f64 656c 2066 726f 6d20  ined model from 
+00003270: 6d6f 6465 6c5f 6469 720a 2020 2020 2020  model_dir.      
+00003280: 2020 2020 2020 6d2e 6c6f 6164 5f6d 6f64        m.load_mod
+00003290: 656c 2829 0a20 2020 2020 2020 2020 2020  el().           
+000032a0: 2070 7265 6469 6374 5f6c 6162 656c 2c20   predict_label, 
+000032b0: 7072 6564 6963 745f 7072 6f62 6120 3d20  predict_proba = 
+000032c0: 6d2e 7072 6564 6963 7428 0a20 2020 2020  m.predict(.     
+000032d0: 2020 2020 2020 2020 2020 205b 27e9 a1ba             ['...
+000032e0: e4b9 89e5 8c97 e4ba ace8 8b8f e6b4 bb38  ...............8
+000032f0: 38e5 b9b3 e7b1 b3e8 b5b7 e7b2 bee8 a385  8...............
+00003300: e688 bfe5 9ca8 e594 ae27 2c0a 2020 2020  .........',.    
+00003310: 2020 2020 2020 2020 2020 2020 2027 e7be               '..
+00003320: 8e45 422d 35e9 a1b9 e79b aee2 809c 3135  .EB-5.........15
+00003330: e697 a5e5 bfab e980 9fe7 a7bb e6b0 91e2  ................
+00003340: 809d e5b0 86e6 8ea8 e8bf 9f27 5d0a 2020  ...........'].  
+00003350: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00003360: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00003370: 7072 6564 6963 745f 6c61 6265 6c3a 207b  predict_label: {
+00003380: 7072 6564 6963 745f 6c61 6265 6c7d 2c20  predict_label}, 
+00003390: 7072 6564 6963 745f 7072 6f62 613a 207b  predict_proba: {
+000033a0: 7072 6564 6963 745f 7072 6f62 617d 2729  predict_proba}')
+000033b0: 0a20 2020 2020 2020 2020 2020 2078 2c20  .            x, 
+000033c0: 792c 2064 6620 3d20 6c6f 6164 5f64 6174  y, df = load_dat
+000033d0: 6128 6461 7461 5f66 696c 6529 0a20 2020  a(data_file).   
+000033e0: 2020 2020 2020 2020 2074 6573 745f 6461           test_da
+000033f0: 7461 203d 2064 665b 3a31 3030 5d0a 2020  ta = df[:100].  
+00003400: 2020 2020 2020 2020 2020 6163 635f 7363            acc_sc
+00003410: 6f72 6520 3d20 6d2e 6576 616c 7561 7465  ore = m.evaluate
+00003420: 5f6d 6f64 656c 2874 6573 745f 6461 7461  _model(test_data
+00003430: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00003440: 696e 7428 6627 6163 635f 7363 6f72 653a  int(f'acc_score:
+00003450: 207b 6163 635f 7363 6f72 657d 2729 0a20   {acc_score}'). 
+00003460: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00003470: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
+00003480: 4245 5254 20e7 b1bb e6a8 a1e5 9e8b 0a20  BERT .......... 
+00003490: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000034a0: 2323 2323 20e5 a49a e588 86e7 b1bb e6a8  #### ...........
+000034b0: a1e5 9e8b 0a20 2020 2020 2020 20e8 aead  .....        ...
+000034c0: e7bb 83e5 928c e9a2 84e6 b58b 6042 4552  ............`BER
+000034d0: 5460 e5a4 9ae5 8886 e7b1 bbe6 a8a1 e59e  T`..............
+000034e0: 8bef bc8c e7a4 bae4 be8b 5b65 7861 6d70  ..........[examp
+000034f0: 6c65 732f 6265 7274 5f63 6c61 7373 6966  les/bert_classif
+00003500: 6963 6174 696f 6e5f 7a68 5f64 656d 6f2e  ication_zh_demo.
+00003510: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
+00003520: 7562 2e63 6f6d 2f73 6869 6269 6e67 3632  ub.com/shibing62
+00003530: 342f 7079 7465 7874 636c 6173 7369 6669  4/pytextclassifi
+00003540: 6572 2f62 6c6f 622f 6d61 7374 6572 2f65  er/blob/master/e
+00003550: 7861 6d70 6c65 732f 6265 7274 5f63 6c61  xamples/bert_cla
+00003560: 7373 6966 6963 6174 696f 6e5f 7a68 5f64  ssification_zh_d
+00003570: 656d 6f2e 7079 290a 2020 2020 2020 2020  emo.py).        
+00003580: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
+00003590: 6f6e 0a20 2020 2020 2020 2069 6d70 6f72  on.        impor
+000035a0: 7420 7379 730a 2020 2020 2020 2020 0a20  t sys.        . 
+000035b0: 2020 2020 2020 2073 7973 2e70 6174 682e         sys.path.
+000035c0: 6170 7065 6e64 2827 2e2e 2729 0a20 2020  append('..').   
+000035d0: 2020 2020 2066 726f 6d20 7079 7465 7874       from pytext
+000035e0: 636c 6173 7369 6669 6572 2069 6d70 6f72  classifier impor
+000035f0: 7420 4265 7274 436c 6173 7369 6669 6572  t BertClassifier
+00003600: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00003610: 2020 6966 205f 5f6e 616d 655f 5f20 3d3d    if __name__ ==
+00003620: 2027 5f5f 6d61 696e 5f5f 273a 0a20 2020   '__main__':.   
+00003630: 2020 2020 2020 2020 206d 203d 2042 6572           m = Ber
+00003640: 7443 6c61 7373 6966 6965 7228 6f75 7470  tClassifier(outp
+00003650: 7574 5f64 6972 3d27 6d6f 6465 6c73 2f62  ut_dir='models/b
+00003660: 6572 742d 6368 696e 6573 652d 746f 7927  ert-chinese-toy'
+00003670: 2c20 6e75 6d5f 636c 6173 7365 733d 322c  , num_classes=2,
 00003680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003690: 2028 2773 706f 7274 7327 2c20 27e5 9b9b   ('sports', '...
-000036a0: e5b7 9de4 b8b9 e6a3 b1e4 b8be e8a1 8ce5  ................
-000036b0: 85a8 e59b bde9 95bf e8b7 9de7 99bb e5b1  ................
-000036c0: b1e6 8c91 e688 98e8 b59b 20e8 bf91 e4b8  .......... .....
-000036d0: 87e4 baba e58f 82e4 b88e 2729 2c0a 2020  ..........'),.  
-000036e0: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-000036f0: 7370 6f72 7473 272c 2027 e7b1 b3e5 85b0  sports', '......
-00003700: e5ae a2e5 9cba 38e6 8898 e4b8 8de8 b4a5  ......8.........
-00003710: e59b bde7 b1b3 3130 e5b9 b4e8 bf9e e883  ......10........
-00003720: 9c27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
-00003730: 205d 0a20 2020 2020 2020 2020 2020 206d   ].            m
-00003740: 2e74 7261 696e 2864 6174 6129 0a20 2020  .train(data).   
-00003750: 2020 2020 2020 2020 2070 7269 6e74 286d           print(m
-00003760: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-00003770: 6c6f 6164 2074 7261 696e 6564 2062 6573  load trained bes
-00003780: 7420 6d6f 6465 6c20 6672 6f6d 206d 6f64  t model from mod
-00003790: 656c 5f64 6972 0a20 2020 2020 2020 2020  el_dir.         
-000037a0: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
-000037b0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-000037c0: 6564 6963 745f 6c61 6265 6c2c 2070 7265  edict_label, pre
-000037d0: 6469 6374 5f70 726f 6261 203d 206d 2e70  dict_proba = m.p
-000037e0: 7265 6469 6374 285b 27e7 a68f e5bb bae6  redict(['.......
-000037f0: 98a5 e5ad a3e5 85ac e58a a1e5 9198 e880  ................
-00003800: 83e8 af95 e68a a5e5 908d 3138 e697 a5e6  ..........18....
-00003810: 88aa e6ad a220 32e6 9c88 36e6 97a5 e880  ..... 2...6.....
-00003820: 83e8 af95 272c 0a20 2020 2020 2020 2020  ....',.         
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 2020 2020 2020 2020 2020 2027 e684               '..
-00003860: 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b  ................
-00003870: e4ba a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3  ............:...
-00003880: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
-00003890: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
-000038a0: 9ee8 839c 275d 290a 2020 2020 2020 2020  ....']).        
-000038b0: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
-000038c0: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
-000038d0: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
-000038e0: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
-000038f0: 6963 745f 7072 6f62 617d 2729 0a20 2020  ict_proba}').   
-00003900: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00003910: 2020 7465 7374 5f64 6174 6120 3d20 5b0a    test_data = [.
-00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003930: 2827 6564 7563 6174 696f 6e27 2c20 27e7  ('education', '.
-00003940: a68f e5bb bae6 98a5 e5ad a3e5 85ac e58a  ................
-00003950: a1e5 9198 e880 83e8 af95 e68a a5e5 908d  ................
-00003960: 3138 e697 a5e6 88aa e6ad a220 32e6 9c88  18......... 2...
-00003970: 36e6 97a5 e880 83e8 af95 2729 2c0a 2020  6.........'),.  
-00003980: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00003990: 7370 6f72 7473 272c 2027 e684 8fe7 94b2  sports', '......
-000039a0: e9a6 96e8 bdae e8a1 a5e8 b59b e4ba a4e6  ................
-000039b0: 8898 e8ae b0e5 bd95 3ae7 b1b3 e585 b0e5  ........:.......
-000039c0: aea2 e59c ba38 e688 98e4 b88d e8b4 a5e5  .....8..........
-000039d0: 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8 839c  .....10.........
-000039e0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-000039f0: 5d0a 2020 2020 2020 2020 2020 2020 6163  ].            ac
-00003a00: 635f 7363 6f72 6520 3d20 6d2e 6576 616c  c_score = m.eval
-00003a10: 7561 7465 5f6d 6f64 656c 2874 6573 745f  uate_model(test_
-00003a20: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00003a30: 2020 7072 696e 7428 6627 6163 635f 7363    print(f'acc_sc
-00003a40: 6f72 653a 207b 6163 635f 7363 6f72 657d  ore: {acc_score}
-00003a50: 2729 0a20 2020 2020 2020 2020 2020 200a  ').            .
-00003a60: 2020 2020 2020 2020 2020 2020 2320 7472              # tr
-00003a70: 6169 6e20 6d6f 6465 6c20 7769 7468 2031  ain model with 1
-00003a80: 7720 6461 7461 2066 696c 6520 616e 6420  w data file and 
-00003a90: 3130 2063 6c61 7373 6573 0a20 2020 2020  10 classes.     
-00003aa0: 2020 2020 2020 2070 7269 6e74 2827 2d27         print('-'
-00003ab0: 202a 2034 3229 0a20 2020 2020 2020 2020   * 42).         
-00003ac0: 2020 206d 203d 2042 6572 7443 6c61 7373     m = BertClass
-00003ad0: 6966 6965 7228 6d6f 6465 6c5f 6469 723d  ifier(model_dir=
-00003ae0: 276d 6f64 656c 732f 6265 7274 2d63 6869  'models/bert-chi
-00003af0: 6e65 7365 272c 206e 756d 5f63 6c61 7373  nese', num_class
-00003b00: 6573 3d31 302c 0a20 2020 2020 2020 2020  es=10,.         
-00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b20: 2020 2020 2020 6d6f 6465 6c5f 7479 7065        model_type
-00003b30: 3d27 6265 7274 272c 206d 6f64 656c 5f6e  ='bert', model_n
-00003b40: 616d 653d 2762 6572 742d 6261 7365 2d63  ame='bert-base-c
-00003b50: 6869 6e65 7365 272c 206e 756d 5f65 706f  hinese', num_epo
-00003b60: 6368 733d 322c 0a20 2020 2020 2020 2020  chs=2,.         
-00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 2020 2020 2020 6172 6773 3d7b 226e 6f5f        args={"no_
-00003b90: 6361 6368 6522 3a20 5472 7565 2c20 226c  cache": True, "l
-00003ba0: 617a 795f 6c6f 6164 696e 6722 3a20 5472  azy_loading": Tr
-00003bb0: 7565 2c20 226c 617a 795f 7465 7874 5f63  ue, "lazy_text_c
-00003bc0: 6f6c 756d 6e22 3a20 312c 2022 6c61 7a79  olumn": 1, "lazy
-00003bd0: 5f6c 6162 656c 735f 636f 6c75 6d6e 223a  _labels_column":
-00003be0: 2030 2c20 7d29 0a20 2020 2020 2020 2020   0, }).         
-00003bf0: 2020 2064 6174 615f 6669 6c65 203d 2027     data_file = '
-00003c00: 7468 7563 6e65 7773 5f74 7261 696e 5f31  thucnews_train_1
-00003c10: 772e 7478 7427 0a20 2020 2020 2020 2020  w.txt'.         
-00003c20: 2020 2023 20e5 a682 e69e 9ce8 aead e7bb     # ...........
-00003c30: 83e6 95b0 e68d aee8 b685 e8bf 87e7 99be  ................
-00003c40: e4b8 87e6 9da1 efbc 8ce5 bbba e8ae aee4  ................
-00003c50: bdbf e794 a86c 617a 795f 6c6f 6164 696e  .....lazy_loadin
-00003c60: 67e6 a8a1 e5bc 8fef bc8c e587 8fe5 b091  g...............
-00003c70: e586 85e5 ad98 e58d a0e7 94a8 0a20 2020  .............   
-00003c80: 2020 2020 2020 2020 206d 2e74 7261 696e           m.train
-00003c90: 2864 6174 615f 6669 6c65 2c20 7465 7374  (data_file, test
-00003ca0: 5f73 697a 653d 302c 206e 616d 6573 3d28  _size=0, names=(
-00003cb0: 276c 6162 656c 7327 2c20 2774 6578 7427  'labels', 'text'
-00003cc0: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
-00003cd0: 2e6c 6f61 645f 6d6f 6465 6c28 290a 2020  .load_model().  
-00003ce0: 2020 2020 2020 2020 2020 7072 6564 6963            predic
-00003cf0: 745f 6c61 6265 6c2c 2070 7265 6469 6374  t_label, predict
-00003d00: 5f70 726f 6261 203d 206d 2e70 7265 6469  _proba = m.predi
-00003d10: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-00003d20: 2020 2020 5b27 e9a1 bae4 b989 e58c 97e4      ['..........
-00003d30: baac e88b 8fe6 b4bb 3838 e5b9 b3e7 b1b3  ........88......
-00003d40: e8b5 b7e7 b2be e8a3 85e6 88bf e59c a8e5  ................
-00003d50: 94ae 272c 0a20 2020 2020 2020 2020 2020  ..',.           
-00003d60: 2020 2020 2020 27e7 be8e 4542 2d35 e9a1        '...EB-5..
-00003d70: b9e7 9bae e280 9c31 35e6 97a5 e5bf abe9  .......15.......
-00003d80: 809f e7a7 bbe6 b091 e280 9de5 b086 e68e  ................
-00003d90: a8e8 bf9f 272c 0a20 2020 2020 2020 2020  ....',.         
-00003da0: 2020 2020 2020 2020 27e6 8192 e794 9f41          '......A
-00003db0: 48e6 baa2 e68c 87e6 94b6 e5b9 b320 41e8  H............ A.
-00003dc0: 82a1 e5af b948 e882 a1e6 8a98 e4bb b731  .....H.........1
-00003dd0: 2e39 3525 275d 290a 2020 2020 2020 2020  .95%']).        
-00003de0: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
-00003df0: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
-00003e00: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
-00003e10: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
-00003e20: 6963 745f 7072 6f62 617d 2729 0a20 2020  ict_proba}').   
-00003e30: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
-00003e40: 2050 53ef bc9a e5a6 82e6 9e9c e8ae ade7   PS.............
-00003e50: bb83 e695 b0e6 8dae e8b6 85e8 bf87 e799  ................
-00003e60: bee4 b887 e69d a1ef bc8c e5bb bae8 aeae  ................
-00003e70: e4bd bfe7 94a8 6c61 7a79 5f6c 6f61 6469  ......lazy_loadi
-00003e80: 6e67 e6a8 a1e5 bc8f efbc 8ce5 878f e5b0  ng..............
-00003e90: 91e5 8685 e5ad 98e5 8da0 e794 a80a 2020  ..............  
-00003ea0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00003eb0: 2323 2320 e5a4 9ae6 a087 e7ad bee5 8886  ### ............
-00003ec0: e7b1 bbe6 a8a1 e59e 8b0a 2020 2020 2020  ..........      
-00003ed0: 2020 e588 86e7 b1bb e58f afe4 bba5 e588    ..............
-00003ee0: 86e4 b8ba e5a4 9ae5 8886 e7b1 bbe5 928c  ................
-00003ef0: e5a4 9ae6 a087 e7ad bee5 8886 e7b1 bbe3  ................
-00003f00: 8082 e5a4 9ae5 8886 e7b1 bbe7 9a84 e6a0  ................
-00003f10: 87e7 adbe e698 afe6 8e92 e4bb 96e7 9a84  ................
-00003f20: efbc 8ce8 808c e5a4 9ae6 a087 e7ad bee5  ................
-00003f30: 8886 e7b1 bbe7 9a84 e689 80e6 9c89 e6a0  ................
-00003f40: 87e7 adbe e698 afe4 b88d e68e 92e4 bb96  ................
-00003f50: e79a 84e3 8082 0a20 2020 2020 2020 200a  .......        .
-00003f60: 2020 2020 2020 2020 e5a4 9ae6 a087 e7ad          ........
-00003f70: bee5 8886 e7b1 bbe6 af94 e8be 83e7 9bb4  ................
-00003f80: e8a7 82e7 9a84 e790 86e8 a7a3 e698 afef  ................
-00003f90: bc8c e4b8 80e4 b8aa e6a0 b7e6 9cac e58f  ................
-00003fa0: afe4 bba5 e590 8ce6 97b6 e68b a5e6 9c89  ................
-00003fb0: e587 a0e4 b8aa e7b1 bbe5 88ab e6a0 87e7  ................
-00003fc0: adbe efbc 8c0a 2020 2020 2020 2020 e6af  ......        ..
-00003fd0: 94e5 a682 e4b8 80e9 a696 e6ad 8ce7 9a84  ................
-00003fe0: e6a0 87e7 adbe e58f afe4 bba5 e698 afe6  ................
-00003ff0: b581 e8a1 8ce3 8081 e8bd bbe5 bfab efbc  ................
-00004000: 8ce4 b880 e983 a8e7 94b5 e5bd b1e7 9a84  ................
-00004010: e6a0 87e7 adbe e58f afe4 bba5 e698 afe5  ................
-00004020: 8aa8 e4bd 9ce3 8081 e596 9ce5 89a7 e380  ................
-00004030: 81e6 909e e7ac 91e7 ad89 efbc 8ce8 bf99  ................
-00004040: e983 bde6 98af e5a4 9ae6 a087 e7ad bee5  ................
-00004050: 8886 e7b1 bbe7 9a84 e683 85e5 86b5 e380  ................
-00004060: 820a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00004070: 2020 20e8 aead e7bb 83e5 928c e9a2 84e6     .............
-00004080: b58b 6042 4552 5460 e5a4 9ae6 a087 e7ad  ..`BERT`........
-00004090: bee5 8886 e7b1 bbe6 a8a1 e59e 8bef bc8c  ................
-000040a0: e7a4 bae4 be8b 5b65 7861 6d70 6c65 732f  ......[examples/
-000040b0: 6265 7274 5f6d 756c 7469 6c61 6265 6c5f  bert_multilabel_
-000040c0: 636c 6173 7369 6669 6361 7469 6f6e 5f7a  classification_z
-000040d0: 685f 6465 6d6f 2e70 792e 7079 5d28 6874  h_demo.py.py](ht
-000040e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000040f0: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
-00004100: 7874 636c 6173 7369 6669 6572 2f62 6c6f  xtclassifier/blo
-00004110: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
-00004120: 732f 6265 7274 5f6d 756c 7469 6c61 6265  s/bert_multilabe
-00004130: 6c5f 636c 6173 7369 6669 6361 7469 6f6e  l_classification
-00004140: 5f7a 685f 6465 6d6f 2e70 7929 0a20 2020  _zh_demo.py).   
-00004150: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
-00004160: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-00004170: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00004180: 7379 730a 2020 2020 2020 2020 696d 706f  sys.        impo
-00004190: 7274 2070 616e 6461 7320 6173 2070 640a  rt pandas as pd.
-000041a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000041b0: 2073 7973 2e70 6174 682e 6170 7065 6e64   sys.path.append
-000041c0: 2827 2e2e 2729 0a20 2020 2020 2020 2066  ('..').        f
-000041d0: 726f 6d20 7079 7465 7874 636c 6173 7369  rom pytextclassi
-000041e0: 6669 6572 2069 6d70 6f72 7420 4265 7274  fier import Bert
-000041f0: 436c 6173 7369 6669 6572 0a20 2020 2020  Classifier.     
-00004200: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00004210: 2020 2020 2064 6566 206c 6f61 645f 6a64       def load_jd
-00004220: 5f64 6174 6128 6669 6c65 5f70 6174 6829  _data(file_path)
-00004230: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
-00004240: 220a 2020 2020 2020 2020 2020 2020 4c6f  ".            Lo
-00004250: 6164 206a 6420 6461 7461 2066 726f 6d20  ad jd data from 
-00004260: 6669 6c65 2e0a 2020 2020 2020 2020 2020  file..          
-00004270: 2020 4070 6172 616d 2066 696c 655f 7061    @param file_pa
-00004280: 7468 3a20 0a20 2020 2020 2020 2020 2020  th: .           
-00004290: 2020 2020 2066 6f72 6d61 743a 2063 6f6e       format: con
-000042a0: 7465 6e74 2ce5 85b6 e4bb 962c e4ba 92e8  tent,......,....
-000042b0: 8194 e4ba 92e9 809a 2ce4 baa7 e593 81e5  ........,.......
-000042c0: 8a9f e880 972c e6bb 91e8 bdae e68f 90e6  .....,..........
-000042d0: 898b 2ce5 a3b0 e99f b32c 4150 50e6 938d  ..,......,APP...
-000042e0: e68e a7e6 80a7 2ce5 91bc e590 b8e7 81af  ......,.........
-000042f0: 2ce5 a496 e8a7 822c e5ba 95e5 baa7 2ce5  ,......,......,.
-00004300: 88b6 e783 ade8 8c83 e59b b42c e981 a5e6  ...........,....
-00004310: 8ea7 e599 a8e7 94b5 e6b1 a02c e591 b3e9  ...........,....
-00004320: 8193 2ce5 88b6 e783 ade6 9588 e69e 9c2c  ..,............,
-00004330: e8a1 a3e7 89a9 e783 98e5 b9b2 2ce4 bd93  ............,...
-00004340: e7a7 afe5 a4a7 e5b0 8f0a 2020 2020 2020  ..........      
-00004350: 2020 2020 2020 4072 6574 7572 6e3a 200a        @return: .
-00004360: 2020 2020 2020 2020 2020 2020 2222 220a              """.
-00004370: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00004380: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-00004390: 2020 7769 7468 206f 7065 6e28 6669 6c65    with open(file
-000043a0: 5f70 6174 682c 2027 7227 2c20 656e 636f  _path, 'r', enco
-000043b0: 6469 6e67 3d27 7574 662d 3827 2920 6173  ding='utf-8') as
-000043c0: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
-000043d0: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-000043e0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-000043f0: 2020 2020 2020 206c 696e 6520 3d20 6c69         line = li
-00004400: 6e65 2e73 7472 6970 2829 0a20 2020 2020  ne.strip().     
-00004410: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004420: 6620 6c69 6e65 2e73 7461 7274 7377 6974  f line.startswit
-00004430: 6828 2723 2729 3a0a 2020 2020 2020 2020  h('#'):.        
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00004460: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004470: 6e6f 7420 6c69 6e65 3a0a 2020 2020 2020  not line:.      
-00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-000044a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000044b0: 6572 6d73 203d 206c 696e 652e 7370 6c69  erms = line.spli
-000044c0: 7428 272c 2729 0a20 2020 2020 2020 2020  t(',').         
-000044d0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-000044e0: 6e28 7465 726d 7329 2021 3d20 3136 3a0a  n(terms) != 16:.
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00004510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004520: 2020 2020 2076 616c 203d 205b 696e 7428       val = [int(
-00004530: 6929 2066 6f72 2069 2069 6e20 7465 726d  i) for i in term
-00004540: 735b 313a 5d5d 0a20 2020 2020 2020 2020  s[1:]].         
-00004550: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-00004560: 6170 7065 6e64 285b 7465 726d 735b 305d  append([terms[0]
-00004570: 2c20 7661 6c5d 290a 2020 2020 2020 2020  , val]).        
-00004580: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
-00004590: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000045a0: 200a 2020 2020 2020 2020 6966 205f 5f6e   .        if __n
-000045b0: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-000045c0: 5f5f 273a 0a20 2020 2020 2020 2020 2020  __':.           
-000045d0: 2023 206d 6f64 656c 5f74 7970 653a 2073   # model_type: s
-000045e0: 7570 706f 7274 2027 6265 7274 272c 2027  upport 'bert', '
-000045f0: 616c 6265 7274 272c 2027 726f 6265 7274  albert', 'robert
-00004600: 6127 2c20 2778 6c6e 6574 270a 2020 2020  a', 'xlnet'.    
-00004610: 2020 2020 2020 2020 2320 6d6f 6465 6c5f          # model_
-00004620: 6e61 6d65 3a20 7375 7070 6f72 7420 2762  name: support 'b
-00004630: 6572 742d 6261 7365 2d63 6869 6e65 7365  ert-base-chinese
-00004640: 272c 2027 6265 7274 2d62 6173 652d 6361  ', 'bert-base-ca
-00004650: 7365 6427 2c20 2762 6572 742d 6261 7365  sed', 'bert-base
-00004660: 2d6d 756c 7469 6c69 6e67 7561 6c2d 6361  -multilingual-ca
-00004670: 7365 6427 202e 2e2e 0a20 2020 2020 2020  sed' ....       
-00004680: 2020 2020 206d 203d 2042 6572 7443 6c61       m = BertCla
-00004690: 7373 6966 6965 7228 6d6f 6465 6c5f 6469  ssifier(model_di
-000046a0: 723d 276d 6f64 656c 732f 6d75 6c74 696c  r='models/multil
-000046b0: 6162 656c 2d62 6572 742d 7a68 2d6d 6f64  abel-bert-zh-mod
-000046c0: 656c 272c 206e 756d 5f63 6c61 7373 6573  el', num_classes
-000046d0: 3d31 352c 0a20 2020 2020 2020 2020 2020  =15,.           
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 6d6f 6465 6c5f 7479 7065 3d27 6265 7274  model_type='bert
+000036b0: 272c 206d 6f64 656c 5f6e 616d 653d 2762  ', model_name='b
+000036c0: 6572 742d 6261 7365 2d63 6869 6e65 7365  ert-base-chinese
+000036d0: 272c 206e 756d 5f65 706f 6368 733d 3229  ', num_epochs=2)
+000036e0: 0a20 2020 2020 2020 2020 2020 2023 206d  .            # m
+000036f0: 6f64 656c 5f74 7970 653a 2073 7570 706f  odel_type: suppo
+00003700: 7274 2027 6265 7274 272c 2027 616c 6265  rt 'bert', 'albe
+00003710: 7274 272c 2027 726f 6265 7274 6127 2c20  rt', 'roberta', 
+00003720: 2778 6c6e 6574 270a 2020 2020 2020 2020  'xlnet'.        
+00003730: 2020 2020 2320 6d6f 6465 6c5f 6e61 6d65      # model_name
+00003740: 3a20 7375 7070 6f72 7420 2762 6572 742d  : support 'bert-
+00003750: 6261 7365 2d63 6869 6e65 7365 272c 2027  base-chinese', '
+00003760: 6265 7274 2d62 6173 652d 6361 7365 6427  bert-base-cased'
+00003770: 2c20 2762 6572 742d 6261 7365 2d6d 756c  , 'bert-base-mul
+00003780: 7469 6c69 6e67 7561 6c2d 6361 7365 6427  tilingual-cased'
+00003790: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+000037a0: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
+000037b0: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
+000037c0: 6174 696f 6e27 2c20 27e5 908d e5b8 88e6  ation', '.......
+000037d0: 8c87 e5af bce6 8998 e7a6 8fe8 afad e6b3  ................
+000037e0: 95e6 8a80 e5b7 a7ef bc9a e590 8de8 af8d  ................
+000037f0: e79a 84e5 a48d e695 b0e5 bda2 e5bc 8f27  ...............'
+00003800: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00003810: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+00003820: 2027 e4b8 ade5 9bbd e9ab 98e8 8083 e688   '..............
+00003830: 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5 8faf  ................
+00003840: 20e6 98af e280 9ce7 8bbc e69d a5e4 ba86   ...............
+00003850: e280 9de5 9097 efbc 9f27 292c 0a20 2020  .........'),.   
+00003860: 2020 2020 2020 2020 2020 2020 2028 2765               ('e
+00003870: 6475 6361 7469 6f6e 272c 2027 e585 ace5  ducation', '....
+00003880: 8aa1 e591 98e8 8083 e899 91e8 b68a e69d  ................
+00003890: a5e8 b68a e590 83e9 a699 efbc 8ce8 bf99  ................
+000038a0: e698 afe6 808e e4b9 88e5 9b9e e4ba 8bef  ................
+000038b0: bc9f 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
+000038c0: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
+000038d0: 2027 e59b bee6 9687 efbc 9ae6 b395 e7bd   '..............
+000038e0: 91e5 ad9f e88f b2e5 b094 e696 afe8 8ba6  ................
+000038f0: e688 98e8 bf9b 3136 e5bc ba20 e5ad 9fe8  ......16... ....
+00003900: 8fb2 e5b0 94e6 96af e680 92e5 90bc 2729  ..............')
+00003910: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003920: 2020 2827 7370 6f72 7473 272c 2027 e59b    ('sports', '..
+00003930: 9be5 b79d e4b8 b9e6 a3b1 e4b8 bee8 a18c  ................
+00003940: e585 a8e5 9bbd e995 bfe8 b79d e799 bbe5  ................
+00003950: b1b1 e68c 91e6 8898 e8b5 9b20 e8bf 91e4  ........... ....
+00003960: b887 e4ba bae5 8f82 e4b8 8e27 292c 0a20  ...........'),. 
+00003970: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00003980: 2773 706f 7274 7327 2c20 27e7 b1b3 e585  'sports', '.....
+00003990: b0e5 aea2 e59c ba38 e688 98e4 b88d e8b4  .......8........
+000039a0: a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8  .......10.......
+000039b0: 839c 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
+000039c0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+000039d0: 6d2e 7472 6169 6e28 6461 7461 290a 2020  m.train(data).  
+000039e0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000039f0: 6d29 0a20 2020 2020 2020 2020 2020 2023  m).            #
+00003a00: 206c 6f61 6420 7472 6169 6e65 6420 6265   load trained be
+00003a10: 7374 206d 6f64 656c 2066 726f 6d20 6d6f  st model from mo
+00003a20: 6465 6c5f 6469 720a 2020 2020 2020 2020  del_dir.        
+00003a30: 2020 2020 6d2e 6c6f 6164 5f6d 6f64 656c      m.load_model
+00003a40: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+00003a50: 7265 6469 6374 5f6c 6162 656c 2c20 7072  redict_label, pr
+00003a60: 6564 6963 745f 7072 6f62 6120 3d20 6d2e  edict_proba = m.
+00003a70: 7072 6564 6963 7428 5b27 e7a6 8fe5 bbba  predict(['......
+00003a80: e698 a5e5 ada3 e585 ace5 8aa1 e591 98e8  ................
+00003a90: 8083 e8af 95e6 8aa5 e590 8d31 38e6 97a5  ...........18...
+00003aa0: e688 aae6 ada2 2032 e69c 8836 e697 a5e8  ...... 2...6....
+00003ab0: 8083 e8af 9527 2c0a 2020 2020 2020 2020  .....',.        
+00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 27e6                '.
+00003af0: 848f e794 b2e9 a696 e8bd aee8 a1a5 e8b5  ................
+00003b00: 9be4 baa4 e688 98e8 aeb0 e5bd 953a e7b1  .............:..
+00003b10: b3e5 85b0 e5ae a2e5 9cba 38e6 8898 e4b8  ..........8.....
+00003b20: 8de8 b4a5 e59b bde7 b1b3 3130 e5b9 b4e8  ..........10....
+00003b30: bf9e e883 9c27 5d29 0a20 2020 2020 2020  .....']).       
+00003b40: 2020 2020 2070 7269 6e74 2866 2770 7265       print(f'pre
+00003b50: 6469 6374 5f6c 6162 656c 3a20 7b70 7265  dict_label: {pre
+00003b60: 6469 6374 5f6c 6162 656c 7d2c 2070 7265  dict_label}, pre
+00003b70: 6469 6374 5f70 726f 6261 3a20 7b70 7265  dict_proba: {pre
+00003b80: 6469 6374 5f70 726f 6261 7d27 290a 2020  dict_proba}').  
+00003b90: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00003ba0: 2020 2074 6573 745f 6461 7461 203d 205b     test_data = [
+00003bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003bc0: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
+00003bd0: e7a6 8fe5 bbba e698 a5e5 ada3 e585 ace5  ................
+00003be0: 8aa1 e591 98e8 8083 e8af 95e6 8aa5 e590  ................
+00003bf0: 8d31 38e6 97a5 e688 aae6 ada2 2032 e69c  .18......... 2..
+00003c00: 8836 e697 a5e8 8083 e8af 9527 292c 0a20  .6.........'),. 
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00003c20: 2773 706f 7274 7327 2c20 27e6 848f e794  'sports', '.....
+00003c30: b2e9 a696 e8bd aee8 a1a5 e8b5 9be4 baa4  ................
+00003c40: e688 98e8 aeb0 e5bd 953a e7b1 b3e5 85b0  .........:......
+00003c50: e5ae a2e5 9cba 38e6 8898 e4b8 8de8 b4a5  ......8.........
+00003c60: e59b bde7 b1b3 3130 e5b9 b4e8 bf9e e883  ......10........
+00003c70: 9c27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
+00003c80: 205d 0a20 2020 2020 2020 2020 2020 2061   ].            a
+00003c90: 6363 5f73 636f 7265 203d 206d 2e65 7661  cc_score = m.eva
+00003ca0: 6c75 6174 655f 6d6f 6465 6c28 7465 7374  luate_model(test
+00003cb0: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
+00003cc0: 2020 2070 7269 6e74 2866 2761 6363 5f73     print(f'acc_s
+00003cd0: 636f 7265 3a20 7b61 6363 5f73 636f 7265  core: {acc_score
+00003ce0: 7d27 290a 2020 2020 2020 2020 0a20 2020  }').        .   
+00003cf0: 2020 2020 2020 2020 2023 2074 7261 696e           # train
+00003d00: 206d 6f64 656c 2077 6974 6820 3177 2064   model with 1w d
+00003d10: 6174 6120 6669 6c65 2061 6e64 2031 3020  ata file and 10 
+00003d20: 636c 6173 7365 730a 2020 2020 2020 2020  classes.        
+00003d30: 2020 2020 7072 696e 7428 272d 2720 2a20      print('-' * 
+00003d40: 3432 290a 2020 2020 2020 2020 2020 2020  42).            
+00003d50: 6d20 3d20 4265 7274 436c 6173 7369 6669  m = BertClassifi
+00003d60: 6572 286f 7574 7075 745f 6469 723d 276d  er(output_dir='m
+00003d70: 6f64 656c 732f 6265 7274 2d63 6869 6e65  odels/bert-chine
+00003d80: 7365 272c 206e 756d 5f63 6c61 7373 6573  se', num_classes
+00003d90: 3d31 302c 0a20 2020 2020 2020 2020 2020  =10,.           
+00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003db0: 2020 2020 6d6f 6465 6c5f 7479 7065 3d27      model_type='
+00003dc0: 6265 7274 272c 206d 6f64 656c 5f6e 616d  bert', model_nam
+00003dd0: 653d 2762 6572 742d 6261 7365 2d63 6869  e='bert-base-chi
+00003de0: 6e65 7365 272c 206e 756d 5f65 706f 6368  nese', num_epoch
+00003df0: 733d 322c 0a20 2020 2020 2020 2020 2020  s=2,.           
+00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e10: 2020 2020 6172 6773 3d7b 226e 6f5f 6361      args={"no_ca
+00003e20: 6368 6522 3a20 5472 7565 2c20 226c 617a  che": True, "laz
+00003e30: 795f 6c6f 6164 696e 6722 3a20 5472 7565  y_loading": True
+00003e40: 2c20 226c 617a 795f 7465 7874 5f63 6f6c  , "lazy_text_col
+00003e50: 756d 6e22 3a20 312c 2022 6c61 7a79 5f6c  umn": 1, "lazy_l
+00003e60: 6162 656c 735f 636f 6c75 6d6e 223a 2030  abels_column": 0
+00003e70: 2c20 7d29 0a20 2020 2020 2020 2020 2020  , }).           
+00003e80: 2064 6174 615f 6669 6c65 203d 2027 7468   data_file = 'th
+00003e90: 7563 6e65 7773 5f74 7261 696e 5f31 772e  ucnews_train_1w.
+00003ea0: 7478 7427 0a20 2020 2020 2020 2020 2020  txt'.           
+00003eb0: 2023 20e5 a682 e69e 9ce8 aead e7bb 83e6   # .............
+00003ec0: 95b0 e68d aee8 b685 e8bf 87e7 99be e4b8  ................
+00003ed0: 87e6 9da1 efbc 8ce5 bbba e8ae aee4 bdbf  ................
+00003ee0: e794 a86c 617a 795f 6c6f 6164 696e 67e6  ...lazy_loading.
+00003ef0: a8a1 e5bc 8fef bc8c e587 8fe5 b091 e586  ................
+00003f00: 85e5 ad98 e58d a0e7 94a8 0a20 2020 2020  ...........     
+00003f10: 2020 2020 2020 206d 2e74 7261 696e 2864         m.train(d
+00003f20: 6174 615f 6669 6c65 2c20 7465 7374 5f73  ata_file, test_s
+00003f30: 697a 653d 302c 206e 616d 6573 3d28 276c  ize=0, names=('l
+00003f40: 6162 656c 7327 2c20 2774 6578 7427 2929  abels', 'text'))
+00003f50: 0a20 2020 2020 2020 2020 2020 206d 2e6c  .            m.l
+00003f60: 6f61 645f 6d6f 6465 6c28 290a 2020 2020  oad_model().    
+00003f70: 2020 2020 2020 2020 7072 6564 6963 745f          predict_
+00003f80: 6c61 6265 6c2c 2070 7265 6469 6374 5f70  label, predict_p
+00003f90: 726f 6261 203d 206d 2e70 7265 6469 6374  roba = m.predict
+00003fa0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00003fb0: 2020 5b27 e9a1 bae4 b989 e58c 97e4 baac    ['............
+00003fc0: e88b 8fe6 b4bb 3838 e5b9 b3e7 b1b3 e8b5  ......88........
+00003fd0: b7e7 b2be e8a3 85e6 88bf e59c a8e5 94ae  ................
+00003fe0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00003ff0: 2020 2020 27e7 be8e 4542 2d35 e9a1 b9e7      '...EB-5....
+00004000: 9bae e280 9c31 35e6 97a5 e5bf abe9 809f  .....15.........
+00004010: e7a7 bbe6 b091 e280 9de5 b086 e68e a8e8  ................
+00004020: bf9f 272c 0a20 2020 2020 2020 2020 2020  ..',.           
+00004030: 2020 2020 2020 27e6 8192 e794 9f41 48e6        '......AH.
+00004040: baa2 e68c 87e6 94b6 e5b9 b320 41e8 82a1  ........... A...
+00004050: e5af b948 e882 a1e6 8a98 e4bb b731 2e39  ...H.........1.9
+00004060: 3525 275d 290a 2020 2020 2020 2020 2020  5%']).          
+00004070: 2020 7072 696e 7428 6627 7072 6564 6963    print(f'predic
+00004080: 745f 6c61 6265 6c3a 207b 7072 6564 6963  t_label: {predic
+00004090: 745f 6c61 6265 6c7d 2c20 7072 6564 6963  t_label}, predic
+000040a0: 745f 7072 6f62 613a 207b 7072 6564 6963  t_proba: {predic
+000040b0: 745f 7072 6f62 617d 2729 0a20 2020 2020  t_proba}').     
+000040c0: 2020 2060 6060 0a20 2020 2020 2020 2050     ```.        P
+000040d0: 53ef bc9a e5a6 82e6 9e9c e8ae ade7 bb83  S...............
+000040e0: e695 b0e6 8dae e8b6 85e8 bf87 e799 bee4  ................
+000040f0: b887 e69d a1ef bc8c e5bb bae8 aeae e4bd  ................
+00004100: bfe7 94a8 6c61 7a79 5f6c 6f61 6469 6e67  ....lazy_loading
+00004110: e6a8 a1e5 bc8f efbc 8ce5 878f e5b0 91e5  ................
+00004120: 8685 e5ad 98e5 8da0 e794 a80a 2020 2020  ............    
+00004130: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00004140: 2320 e5a4 9ae6 a087 e7ad bee5 8886 e7b1  # ..............
+00004150: bbe6 a8a1 e59e 8b0a 2020 2020 2020 2020  ........        
+00004160: e588 86e7 b1bb e58f afe4 bba5 e588 86e4  ................
+00004170: b8ba e5a4 9ae5 8886 e7b1 bbe5 928c e5a4  ................
+00004180: 9ae6 a087 e7ad bee5 8886 e7b1 bbe3 8082  ................
+00004190: e5a4 9ae5 8886 e7b1 bbe7 9a84 e6a0 87e7  ................
+000041a0: adbe e698 afe6 8e92 e4bb 96e7 9a84 efbc  ................
+000041b0: 8ce8 808c e5a4 9ae6 a087 e7ad bee5 8886  ................
+000041c0: e7b1 bbe7 9a84 e689 80e6 9c89 e6a0 87e7  ................
+000041d0: adbe e698 afe4 b88d e68e 92e4 bb96 e79a  ................
+000041e0: 84e3 8082 0a20 2020 2020 2020 200a 2020  .....        .  
+000041f0: 2020 2020 2020 e5a4 9ae6 a087 e7ad bee5        ..........
+00004200: 8886 e7b1 bbe6 af94 e8be 83e7 9bb4 e8a7  ................
+00004210: 82e7 9a84 e790 86e8 a7a3 e698 afef bc8c  ................
+00004220: e4b8 80e4 b8aa e6a0 b7e6 9cac e58f afe4  ................
+00004230: bba5 e590 8ce6 97b6 e68b a5e6 9c89 e587  ................
+00004240: a0e4 b8aa e7b1 bbe5 88ab e6a0 87e7 adbe  ................
+00004250: efbc 8c0a 2020 2020 2020 2020 e6af 94e5  ....        ....
+00004260: a682 e4b8 80e9 a696 e6ad 8ce7 9a84 e6a0  ................
+00004270: 87e7 adbe e58f afe4 bba5 e698 afe6 b581  ................
+00004280: e8a1 8ce3 8081 e8bd bbe5 bfab efbc 8ce4  ................
+00004290: b880 e983 a8e7 94b5 e5bd b1e7 9a84 e6a0  ................
+000042a0: 87e7 adbe e58f afe4 bba5 e698 afe5 8aa8  ................
+000042b0: e4bd 9ce3 8081 e596 9ce5 89a7 e380 81e6  ................
+000042c0: 909e e7ac 91e7 ad89 efbc 8ce8 bf99 e983  ................
+000042d0: bde6 98af e5a4 9ae6 a087 e7ad bee5 8886  ................
+000042e0: e7b1 bbe7 9a84 e683 85e5 86b5 e380 820a  ................
+000042f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004300: 20e8 aead e7bb 83e5 928c e9a2 84e6 b58b   ...............
+00004310: 6042 4552 5460 e5a4 9ae6 a087 e7ad bee5  `BERT`..........
+00004320: 8886 e7b1 bbe6 a8a1 e59e 8bef bc8c e7a4  ................
+00004330: bae4 be8b 5b65 7861 6d70 6c65 732f 6265  ....[examples/be
+00004340: 7274 5f6d 756c 7469 6c61 6265 6c5f 636c  rt_multilabel_cl
+00004350: 6173 7369 6669 6361 7469 6f6e 5f7a 685f  assification_zh_
+00004360: 6465 6d6f 2e70 792e 7079 5d28 6874 7470  demo.py.py](http
+00004370: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00004380: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
+00004390: 636c 6173 7369 6669 6572 2f62 6c6f 622f  classifier/blob/
+000043a0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+000043b0: 6265 7274 5f6d 756c 7469 6c61 6265 6c5f  bert_multilabel_
+000043c0: 636c 6173 7369 6669 6361 7469 6f6e 5f7a  classification_z
+000043d0: 685f 6465 6d6f 2e70 7929 0a20 2020 2020  h_demo.py).     
+000043e0: 2020 200a 2020 2020 2020 2020 6060 6070     .        ```p
+000043f0: 7974 686f 6e0a 2020 2020 2020 2020 696d  ython.        im
+00004400: 706f 7274 2073 7973 0a20 2020 2020 2020  port sys.       
+00004410: 2069 6d70 6f72 7420 7061 6e64 6173 2061   import pandas a
+00004420: 7320 7064 0a20 2020 2020 2020 200a 2020  s pd.        .  
+00004430: 2020 2020 2020 7379 732e 7061 7468 2e61        sys.path.a
+00004440: 7070 656e 6428 272e 2e27 290a 2020 2020  ppend('..').    
+00004450: 2020 2020 6672 6f6d 2070 7974 6578 7463      from pytextc
+00004460: 6c61 7373 6966 6965 7220 696d 706f 7274  lassifier import
+00004470: 2042 6572 7443 6c61 7373 6966 6965 720a   BertClassifier.
+00004480: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004490: 200a 2020 2020 2020 2020 6465 6620 6c6f   .        def lo
+000044a0: 6164 5f6a 645f 6461 7461 2866 696c 655f  ad_jd_data(file_
+000044b0: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
+000044c0: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
+000044d0: 2020 204c 6f61 6420 6a64 2064 6174 6120     Load jd data 
+000044e0: 6672 6f6d 2066 696c 652e 0a20 2020 2020  from file..     
+000044f0: 2020 2020 2020 2040 7061 7261 6d20 6669         @param fi
+00004500: 6c65 5f70 6174 683a 200a 2020 2020 2020  le_path: .      
+00004510: 2020 2020 2020 2020 2020 666f 726d 6174            format
+00004520: 3a20 636f 6e74 656e 742c e585 b6e4 bb96  : content,......
+00004530: 2ce4 ba92 e881 94e4 ba92 e980 9a2c e4ba  ,............,..
+00004540: a7e5 9381 e58a 9fe8 8097 2ce6 bb91 e8bd  ..........,.....
+00004550: aee6 8f90 e689 8b2c e5a3 b0e9 9fb3 2c41  .......,......,A
+00004560: 5050 e693 8de6 8ea7 e680 a72c e591 bce5  PP.........,....
+00004570: 90b8 e781 af2c e5a4 96e8 a782 2ce5 ba95  .....,......,...
+00004580: e5ba a72c e588 b6e7 83ad e88c 83e5 9bb4  ...,............
+00004590: 2ce9 81a5 e68e a7e5 99a8 e794 b5e6 b1a0  ,...............
+000045a0: 2ce5 91b3 e981 932c e588 b6e7 83ad e695  ,......,........
+000045b0: 88e6 9e9c 2ce8 a1a3 e789 a9e7 8398 e5b9  ....,...........
+000045c0: b22c e4bd 93e7 a7af e5a4 a7e5 b08f 0a20  .,............. 
+000045d0: 2020 2020 2020 2020 2020 2040 7265 7475             @retu
+000045e0: 726e 3a20 0a20 2020 2020 2020 2020 2020  rn: .           
+000045f0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
+00004600: 2064 6174 6120 3d20 5b5d 0a20 2020 2020   data = [].     
+00004610: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00004620: 2866 696c 655f 7061 7468 2c20 2772 272c  (file_path, 'r',
+00004630: 2065 6e63 6f64 696e 673d 2775 7466 2d38   encoding='utf-8
+00004640: 2729 2061 7320 663a 0a20 2020 2020 2020  ') as f:.       
+00004650: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
+00004660: 6520 696e 2066 3a0a 2020 2020 2020 2020  e in f:.        
+00004670: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00004680: 203d 206c 696e 652e 7374 7269 7028 290a   = line.strip().
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2020 6966 206c 696e 652e 7374 6172      if line.star
+000046b0: 7473 7769 7468 2827 2327 293a 0a20 2020  tswith('#'):.   
+000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046d0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
 000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2020 6d6f 6465 6c5f 7479 7065 3d27      model_type='
-00004700: 6265 7274 272c 206d 6f64 656c 5f6e 616d  bert', model_nam
-00004710: 653d 2762 6572 742d 6261 7365 2d63 6869  e='bert-base-chi
-00004720: 6e65 7365 272c 206e 756d 5f65 706f 6368  nese', num_epoch
-00004730: 733d 322c 206d 756c 7469 5f6c 6162 656c  s=2, multi_label
-00004740: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00004750: 2020 2023 2054 7261 696e 2061 6e64 2045     # Train and E
-00004760: 7661 6c75 6174 696f 6e20 6461 7461 206e  valuation data n
-00004770: 6565 6473 2074 6f20 6265 2069 6e20 6120  eeds to be in a 
-00004780: 5061 6e64 6173 2044 6174 6166 7261 6d65  Pandas Dataframe
-00004790: 2063 6f6e 7461 696e 696e 6720 6174 206c   containing at l
-000047a0: 6561 7374 2074 776f 2063 6f6c 756d 6e73  east two columns
-000047b0: 2c20 6120 2774 6578 7427 2061 6e64 2061  , a 'text' and a
-000047c0: 2027 6c61 6265 6c73 2720 636f 6c75 6d6e   'labels' column
-000047d0: 2e20 5468 6520 606c 6162 656c 7360 2063  . The `labels` c
-000047e0: 6f6c 756d 6e20 7368 6f75 6c64 2063 6f6e  olumn should con
-000047f0: 7461 696e 206d 756c 7469 2d68 6f74 2065  tain multi-hot e
-00004800: 6e63 6f64 6564 206c 6973 7473 2e0a 2020  ncoded lists..  
-00004810: 2020 2020 2020 2020 2020 7472 6169 6e5f            train_
-00004820: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00004830: 2020 2020 2020 2020 205b 22e4 b880 e4b8           [".....
-00004840: aae5 b08f e697 b6e6 88bf e997 b4e4 bb8d  ................
-00004850: e784 b6e6 b2a1 e69a 96e5 928c 222c 205b  ............", [
-00004860: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00004870: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00004880: 2030 2c20 312c 2030 2c20 305d 5d2c 0a20   0, 1, 0, 0]],. 
-00004890: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000048a0: 22e8 8097 e794 b5e6 8385 e586 b5ef bc9a  "...............
-000048b0: e8bf 99e4 b8aa e6b2 a1e6 9c89 e6b3 a8e6  ................
-000048c0: 848f 222c 205b 302c 2030 2c20 312c 2030  ..", [0, 0, 1, 0
-000048d0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-000048e0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
-000048f0: 305d 5d2c 0a20 2020 2020 2020 2020 2020  0]],.           
-00004900: 205d 0a20 2020 2020 2020 2020 2020 2064   ].            d
-00004910: 6174 6120 3d20 6c6f 6164 5f6a 645f 6461  ata = load_jd_da
-00004920: 7461 2827 6d75 6c74 696c 6162 656c 5f6a  ta('multilabel_j
-00004930: 645f 636f 6d6d 656e 7473 2e63 7376 2729  d_comments.csv')
-00004940: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00004950: 696e 5f64 6174 612e 6578 7465 6e64 2864  in_data.extend(d
-00004960: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-00004970: 2070 7269 6e74 2874 7261 696e 5f64 6174   print(train_dat
-00004980: 615b 3a35 5d29 0a20 2020 2020 2020 2020  a[:5]).         
-00004990: 2020 2074 7261 696e 5f64 6620 3d20 7064     train_df = pd
-000049a0: 2e44 6174 6146 7261 6d65 2874 7261 696e  .DataFrame(train
-000049b0: 5f64 6174 612c 2063 6f6c 756d 6e73 3d5b  _data, columns=[
-000049c0: 2274 6578 7422 2c20 226c 6162 656c 7322  "text", "labels"
-000049d0: 5d29 0a20 2020 2020 2020 200a 2020 2020  ]).        .    
-000049e0: 2020 2020 2020 2020 7072 696e 7428 7472          print(tr
-000049f0: 6169 6e5f 6466 2e68 6561 6428 2929 0a20  ain_df.head()). 
-00004a00: 2020 2020 2020 2020 2020 206d 2e74 7261             m.tra
-00004a10: 696e 2874 7261 696e 5f64 6629 0a20 2020  in(train_df).   
-00004a20: 2020 2020 2020 2020 2070 7269 6e74 286d           print(m
-00004a30: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-00004a40: 4576 616c 7561 7465 2074 6865 206d 6f64  Evaluate the mod
-00004a50: 656c 0a20 2020 2020 2020 2020 2020 2061  el.            a
-00004a60: 6363 5f73 636f 7265 203d 206d 2e65 7661  cc_score = m.eva
-00004a70: 6c75 6174 655f 6d6f 6465 6c28 7472 6169  luate_model(trai
-00004a80: 6e5f 6466 5b3a 3230 5d29 0a20 2020 2020  n_df[:20]).     
-00004a90: 2020 2020 2020 2070 7269 6e74 2866 2761         print(f'a
-00004aa0: 6363 5f73 636f 7265 3a20 7b61 6363 5f73  cc_score: {acc_s
-00004ab0: 636f 7265 7d27 290a 2020 2020 2020 2020  core}').        
-00004ac0: 0a20 2020 2020 2020 2020 2020 2023 206c  .            # l
-00004ad0: 6f61 6420 7472 6169 6e65 6420 6265 7374  oad trained best
-00004ae0: 206d 6f64 656c 2066 726f 6d20 6d6f 6465   model from mode
-00004af0: 6c5f 6469 720a 2020 2020 2020 2020 2020  l_dir.          
-00004b00: 2020 6d2e 6c6f 6164 5f6d 6f64 656c 2829    m.load_model()
-00004b10: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
-00004b20: 6469 6374 5f6c 6162 656c 2c20 7072 6564  dict_label, pred
-00004b30: 6963 745f 7072 6f62 6120 3d20 6d2e 7072  ict_proba = m.pr
-00004b40: 6564 6963 7428 5b27 e4b8 80e4 b8aa e5b0  edict(['........
-00004b50: 8fe6 97b6 e688 bfe9 97b4 e4bb 8de7 84b6  ................
-00004b60: e6b2 a1e6 9a96 e592 8c27 2c20 27e8 8097  .........', '...
-00004b70: e794 b5e6 8385 e586 b5ef bc9a e8bf 99e4  ................
-00004b80: b8aa e6b2 a1e6 9c89 e6b3 a8e6 848f 275d  ..............']
-00004b90: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00004ba0: 696e 7428 6627 7072 6564 6963 745f 6c61  int(f'predict_la
-00004bb0: 6265 6c3a 207b 7072 6564 6963 745f 6c61  bel: {predict_la
-00004bc0: 6265 6c7d 2c20 7072 6564 6963 745f 7072  bel}, predict_pr
-00004bd0: 6f62 613a 207b 7072 6564 6963 745f 7072  oba: {predict_pr
-00004be0: 6f62 617d 2729 0a20 2020 2020 2020 2060  oba}').        `
-00004bf0: 6060 0a20 2020 2020 2020 200a 2020 2020  ``.        .    
-00004c00: 2020 2020 2323 2045 7661 6c75 6174 696f      ## Evaluatio
-00004c10: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
-00004c20: 2020 2023 2323 2044 6174 6173 6574 0a20     ### Dataset. 
-00004c30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004c40: 312e 2054 4855 434e 6577 73e4 b8ad e696  1. THUCNews.....
-00004c50: 87e6 9687 e69c ace6 95b0 e68d aee9 9b86  ................
-00004c60: efbc 8831 2e35 3647 42ef bc89 efbc 9ae5  ...1.56GB.......
-00004c70: ae98 e696 b95b e4b8 8be8 bdbd e59c b0e5  .....[..........
-00004c80: 9d80 5d28 6874 7470 3a2f 2f74 6875 6374  ..](http://thuct
-00004c90: 632e 7468 756e 6c70 2e6f 7267 2f29 efbc  c.thunlp.org/)..
-00004ca0: 8ce6 8abd e6a0 b7e4 ba86 3130 e4b8 87e6  ..........10....
-00004cb0: 9da1 5448 5543 4e65 7773 e4b8 ade6 9687  ..THUCNews......
-00004cc0: e696 87e6 9cac 3130 e588 86e7 b1bb e695  ......10........
-00004cd0: b0e6 8dae e99b 86ef bc88 364d 42ef bc89  ..........6MB...
-00004ce0: efbc 8ce5 9cb0 e59d 80ef bc9a 5b65 7861  ............[exa
-00004cf0: 6d70 6c65 732f 7468 7563 6e65 7773 5f74  mples/thucnews_t
-00004d00: 7261 696e 5f31 3077 2e74 7874 5d28 6578  rain_10w.txt](ex
-00004d10: 616d 706c 6573 2f74 6875 636e 6577 735f  amples/thucnews_
-00004d20: 7472 6169 6e5f 3130 772e 7478 7429 e380  train_10w.txt)..
-00004d30: 820a 2020 2020 2020 2020 322e 2054 4e45  ..        2. TNE
-00004d40: 5753 e4bb 8ae6 97a5 e5a4 b4e6 9da1 e4b8  WS..............
-00004d50: ade6 9687 e696 b0e9 97bb efbc 88e7 9fad  ................
-00004d60: e696 87e6 9cac efbc 89e5 8886 e7b1 bb20  ............... 
-00004d70: 5368 6f72 7420 5465 7874 2043 6c61 7373  Short Text Class
-00004d80: 6966 6963 6169 746f 6e20 666f 7220 4e65  ificaiton for Ne
-00004d90: 7773 efbc 8ce8 afa5 e695 b0e6 8dae e99b  ws..............
-00004da0: 8628 352e 314d 4229 e69d a5e8 87aa e4bb  .(5.1MB)........
-00004db0: 8ae6 97a5 e5a4 b4e6 9da1 e79a 84e6 96b0  ................
-00004dc0: e997 bbe7 8988 e59d 97ef bc8c e585 b1e6  ................
-00004dd0: 8f90 e58f 96e4 ba86 3135 e4b8 aae7 b1bb  ........15......
-00004de0: e588 abe7 9a84 e696 b0e9 97bb efbc 8ce5  ................
-00004df0: 8c85 e68b ace6 9785 e6b8 b8ef bc8c e695  ................
-00004e00: 99e8 82b2 efbc 8ce9 8791 e89e 8def bc8c  ................
-00004e10: e586 9be4 ba8b e7ad 89ef bc8c e59c b0e5  ................
-00004e20: 9d80 efbc 9a5b 746e 6577 735f 7075 626c  .....[tnews_publ
-00004e30: 6963 2e7a 6970 5d28 6874 7470 733a 2f2f  ic.zip](https://
-00004e40: 7374 6f72 6167 652e 676f 6f67 6c65 6170  storage.googleap
-00004e50: 6973 2e63 6f6d 2f63 6c75 6562 656e 6368  is.com/cluebench
-00004e60: 6d61 726b 2f74 6173 6b73 2f74 6e65 7773  mark/tasks/tnews
-00004e70: 5f70 7562 6c69 632e 7a69 7029 0a20 2020  _public.zip).   
-00004e80: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00004e90: 2320 4576 616c 7561 7469 6f6e 2052 6573  # Evaluation Res
-00004ea0: 756c 740a 2020 2020 2020 2020 e59c a854  ult.        ...T
-00004eb0: 4855 434e 6577 73e4 b8ad e696 87e6 9687  HUCNews.........
-00004ec0: e69c ac31 30e5 8886 e7b1 bbe6 95b0 e68d  ...10...........
-00004ed0: aee9 9b86 efbc 8836 4d42 efbc 89e4 b88a  .......6MB......
-00004ee0: e8af 84e4 bcb0 efbc 8ce6 a8a1 e59e 8be5  ................
-00004ef0: 9ca8 e6b5 8be8 af95 e99b 8628 7465 7374  ...........(test
-00004f00: 29e8 af84 e6b5 8be6 9588 e69e 9ce5 a682  )...............
-00004f10: e4b8 8bef bc9a 0a20 2020 2020 2020 200a  .......        .
-00004f20: 2020 2020 2020 2020 e6a8 a1e5 9e8b 7c61          ......|a
-00004f30: 6363 7ce8 afb4 e698 8e0a 2020 2020 2020  cc|.......      
-00004f40: 2020 2d2d 7c2d 2d7c 2d2d 0a20 2020 2020    --|--|--.     
-00004f50: 2020 204c 527c 302e 3838 3033 7ce9 80bb     LR|0.8803|...
-00004f60: e8be 91e5 9b9e e5bd 924c 6f67 6973 7469  .........Logisti
-00004f70: 6373 2052 6567 7265 7373 696f 6e0a 2020  cs Regression.  
-00004f80: 2020 2020 2020 5465 7874 434e 4e7c 302e        TextCNN|0.
-00004f90: 3838 3039 7c4b 696d 2032 3031 3420 e7bb  8809|Kim 2014 ..
-00004fa0: 8fe5 85b8 e79a 8443 4e4e e696 87e6 9cac  .......CNN......
-00004fb0: e588 86e7 b1bb 0a20 2020 2020 2020 2054  .......        T
-00004fc0: 6578 7452 4e4e 5f41 7474 7c30 2e39 3032  extRNN_Att|0.902
-00004fd0: 327c 4269 4c53 544d 2b41 7474 656e 7469  2|BiLSTM+Attenti
-00004fe0: 6f6e 0a20 2020 2020 2020 2046 6173 7454  on.        FastT
-00004ff0: 6578 747c 302e 3931 3737 7c62 6f77 2b62  ext|0.9177|bow+b
-00005000: 6967 7261 6d2b 7472 6967 7261 6def bc8c  igram+trigram...
-00005010: 20e6 9588 e69e 9ce5 87ba e5a5 87e7 9a84   ...............
-00005020: e5a5 bd0a 2020 2020 2020 2020 4450 434e  ....        DPCN
-00005030: 4e7c 302e 3931 3235 7ce6 b7b1 e5b1 82e9  N|0.9125|.......
-00005040: 8791 e5ad 97e5 a194 434e 4e0a 2020 2020  ........CNN.    
-00005050: 2020 2020 5472 616e 7366 6f72 6d65 727c      Transformer|
-00005060: 302e 3839 3931 7ce6 9588 e69e 9ce8 be83  0.8991|.........
-00005070: e5b7 ae0a 2020 2020 2020 2020 4245 5254  ....        BERT
-00005080: 2d62 6173 657c 2a2a 302e 3934 3833 2a2a  -base|**0.9483**
-00005090: 7c62 6572 7420 2b20 6663 0a20 2020 2020  |bert + fc.     
-000050a0: 2020 2045 524e 4945 7c30 2e39 3436 317c     ERNIE|0.9461|
-000050b0: e6af 9462 6572 74e7 95a5 e5b7 ae0a 2020  ...bert.......  
-000050c0: 2020 2020 2020 0a20 2020 2020 2020 20e5        .        .
-000050d0: 9ca8 e4b8 ade6 9687 e696 b0e9 97bb e79f  ................
-000050e0: ade6 9687 e69c ace5 8886 e7b1 bbe6 95b0  ................
-000050f0: e68d aee9 9b86 544e 4557 53e4 b88a e8af  ......TNEWS.....
-00005100: 84e4 bcb0 efbc 8ce6 a8a1 e59e 8be5 9ca8  ................
-00005110: e5bc 80e5 8f91 e99b 8628 6465 7629 e8af  .........(dev)..
-00005120: 84e6 b58b e695 88e6 9e9c e5a6 82e4 b88b  ................
-00005130: efbc 9a0a 2020 2020 2020 2020 0a20 2020  ....        .   
-00005140: 2020 2020 20e6 a8a1 e59e 8b7c 6163 637c       ......|acc|
-00005150: e8af b4e6 988e 0a20 2020 2020 2020 202d  .......        -
-00005160: 2d7c 2d2d 7c2d 2d0a 2020 2020 2020 2020  -|--|--.        
-00005170: 4245 5254 2d62 6173 657c 2a2a 302e 3536  BERT-base|**0.56
-00005180: 3630 2a2a 7ce6 9cac e9a1 b9e7 9bae e5ae  60**|...........
-00005190: 9ee7 8eb0 0a20 2020 2020 2020 2042 4552  .....        BER
-000051a0: 542d 6261 7365 7c30 2e35 3630 397c 434c  T-base|0.5609|CL
-000051b0: 5545 2042 656e 6368 6d61 726b 204c 6561  UE Benchmark Lea
-000051c0: 6465 7262 6f61 7264 e7bb 93e6 9e9c 205b  derboard...... [
-000051d0: 434c 5545 6265 6e63 686d 6172 6b5d 2868  CLUEbenchmark](h
-000051e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000051f0: 6d2f 434c 5545 6265 6e63 686d 6172 6b2f  m/CLUEbenchmark/
-00005200: 434c 5545 290a 2020 2020 2020 2020 0a20  CLUE).        . 
-00005210: 2020 2020 2020 202d 20e4 bba5 e4b8 8ae7         - .......
-00005220: bb93 e69e 9ce5 9d87 e4b8 bae5 8886 e7b1  ................
-00005230: bbe7 9a84 e587 86e7 a1ae e78e 87ef bc88  ................
-00005240: 6163 6375 7261 6379 efbc 89e7 bb93 e69e  accuracy........
-00005250: 9c0a 2020 2020 2020 2020 2d20 5448 5543  ..        - THUC
-00005260: 4e65 7773 e695 b0e6 8dae e99b 86e8 af84  News............
-00005270: e6b5 8be7 bb93 e69e 9ce5 8faf e4bb a5e5  ................
-00005280: 9fba e4ba 8e60 6578 616d 706c 6573 2f74  .....`examples/t
-00005290: 6875 636e 6577 735f 7472 6169 6e5f 3130  hucnews_train_10
-000052a0: 772e 7478 7460 e695 b0e6 8dae e794 a860  w.txt`.........`
-000052b0: 6578 616d 706c 6573 60e4 b88b e79a 84e5  examples`.......
-000052c0: 9084 e6a8 a1e5 9e8b 6465 6d6f e5a4 8de7  ........demo....
-000052d0: 8eb0 0a20 2020 2020 2020 202d 2054 4e45  ...        - TNE
-000052e0: 5753 e695 b0e6 8dae e99b 86e8 af84 e6b5  WS..............
-000052f0: 8be7 bb93 e69e 9ce5 8faf e4bb a5e4 b88b  ................
-00005300: e8bd bd54 4e45 5753 e695 b0e6 8dae e99b  ...TNEWS........
-00005310: 86ef bc8c e8bf 90e8 a18c 6065 7861 6d70  ..........`examp
-00005320: 6c65 732f 6265 7274 5f63 6c61 7373 6966  les/bert_classif
-00005330: 6963 6174 696f 6e5f 746e 6577 735f 6465  ication_tnews_de
-00005340: 6d6f 2e70 7960 e5a4 8de7 8eb0 0a20 2020  mo.py`.......   
-00005350: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00005360: 2320 e6a8 a1e5 9e8b e8b0 83e7 a094 0a20  # ............. 
-00005370: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00005380: e68f 90e4 be9b e588 86e7 b1bb e6a8 a1e5  ................
-00005390: 9e8b e5bf abe9 809f e8b0 83e7 a094 e5b7  ................
-000053a0: a5e5 85b7 efbc 8ce6 9687 e4bb b6e6 a091  ................
-000053b0: efbc 9a0a 2020 2020 2020 2020 6060 6062  ....        ```b
-000053c0: 6173 680a 2020 2020 2020 2020 7079 7465  ash.        pyte
-000053d0: 7874 636c 6173 7369 6669 6572 0a20 2020  xtclassifier.   
-000053e0: 2020 2020 20e2 949c e294 80e2 9480 2062       ......... b
-000053f0: 6572 745f 636c 6173 7369 6669 6572 2e70  ert_classifier.p
-00005400: 790a 2020 2020 2020 2020 e294 9ce2 9480  y.        ......
-00005410: e294 8020 6661 7374 7465 7874 5f63 6c61  ... fasttext_cla
-00005420: 7373 6966 6965 722e 7079 0a20 2020 2020  ssifier.py.     
-00005430: 2020 20e2 949c e294 80e2 9480 2063 6c61     ......... cla
-00005440: 7373 6963 5f63 6c61 7373 6966 6965 722e  ssic_classifier.
-00005450: 7079 0a20 2020 2020 2020 20e2 949c e294  py.        .....
-00005460: 80e2 9480 2074 6578 7463 6e6e 5f63 6c61  .... textcnn_cla
-00005470: 7373 6966 6965 722e 7079 0a20 2020 2020  ssifier.py.     
-00005480: 2020 20e2 9494 e294 80e2 9480 2074 6578     ......... tex
-00005490: 7472 6e6e 5f63 6c61 7373 6966 6965 722e  trnn_classifier.
-000054a0: 7079 0a20 2020 2020 2020 2060 6060 0a20  py.        ```. 
-000054b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000054c0: e6af 8fe4 b8aa e696 87e4 bbb6 e5af b9e5  ................
-000054d0: ba94 e4b8 80e4 b8aa e6a8 a1e5 9e8b efbc  ................
-000054e0: 8ce5 9084 e6a8 a1e5 9e8b e5ae 8ce5 85a8  ................
-000054f0: e78b ace7 ab8b efbc 8ce5 8faf e4bb a5e7  ................
-00005500: 9bb4 e68e a5e8 bf90 e8a1 8cef bc8c e4b9  ................
-00005510: 9fe6 96b9 e4be bfe4 bfae e694 b9ef bc8c  ................
-00005520: e694 afe6 8c81 e980 9ae8 bf87 6061 7267  ............`arg
-00005530: 7061 7273 6560 20e4 bfae e694 b960 2d2d  parse` ......`--
-00005540: 6461 7461 5f70 6174 6860 e7ad 89e5 8f82  data_path`......
-00005550: e695 b0e3 8082 0a20 2020 2020 2020 200a  .......        .
-00005560: 2020 2020 2020 2020 e79b b4e6 8ea5 e59c          ........
-00005570: a8e7 bb88 e7ab afe8 b083 e794 a866 6173  .............fas
-00005580: 7474 6578 74e6 a8a1 e59e 8be8 aead e7bb  ttext...........
-00005590: 83ef bc9a 0a20 2020 2020 2020 2060 6060  .....        ```
-000055a0: 6261 7368 0a20 2020 2020 2020 2070 7974  bash.        pyt
-000055b0: 686f 6e20 2d6d 2070 7974 6578 7463 6c61  hon -m pytextcla
-000055c0: 7373 6966 6965 722e 6661 7374 7465 7874  ssifier.fasttext
-000055d0: 5f63 6c61 7373 6966 6965 7220 2d68 0a20  _classifier -h. 
-000055e0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-000055f0: 2020 200a 2020 2020 2020 2020 2323 2054     .        ## T
-00005600: 6578 7420 436c 7573 7465 720a 2020 2020  ext Cluster.    
-00005610: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
-00005620: 2020 2020 2020 5465 7874 2063 6c75 7374        Text clust
-00005630: 6572 696e 672c 2066 6f72 2065 7861 6d70  ering, for examp
-00005640: 6c65 205b 6578 616d 706c 6573 2f63 6c75  le [examples/clu
-00005650: 7374 6572 5f64 656d 6f2e 7079 5d28 6578  ster_demo.py](ex
-00005660: 616d 706c 6573 2f63 6c75 7374 6572 5f64  amples/cluster_d
-00005670: 656d 6f2e 7079 290a 2020 2020 2020 2020  emo.py).        
-00005680: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00005690: 2020 696d 706f 7274 2073 7973 0a20 2020    import sys.   
-000056a0: 2020 2020 200a 2020 2020 2020 2020 7379       .        sy
-000056b0: 732e 7061 7468 2e61 7070 656e 6428 272e  s.path.append('.
-000056c0: 2e27 290a 2020 2020 2020 2020 6672 6f6d  .').        from
-000056d0: 2070 7974 6578 7463 6c61 7373 6966 6965   pytextclassifie
-000056e0: 722e 7465 7874 636c 7573 7465 7220 696d  r.textcluster im
-000056f0: 706f 7274 2054 6578 7443 6c75 7374 6572  port TextCluster
-00005700: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005710: 2020 6966 205f 5f6e 616d 655f 5f20 3d3d    if __name__ ==
-00005720: 2027 5f5f 6d61 696e 5f5f 273a 0a20 2020   '__main__':.   
-00005730: 2020 2020 2020 2020 206d 203d 2054 6578           m = Tex
-00005740: 7443 6c75 7374 6572 286d 6f64 656c 5f64  tCluster(model_d
-00005750: 6972 3d27 6d6f 6465 6c73 2f63 6c75 7374  ir='models/clust
-00005760: 6572 2d74 6f79 272c 206e 5f63 6c75 7374  er-toy', n_clust
-00005770: 6572 733d 3229 0a20 2020 2020 2020 2020  ers=2).         
-00005780: 2020 2070 7269 6e74 286d 290a 2020 2020     print(m).    
-00005790: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-000057a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057b0: 2027 5374 7564 656e 7420 6465 6274 2074   'Student debt t
-000057c0: 6f20 636f 7374 2042 7269 7461 696e 2062  o cost Britain b
-000057d0: 696c 6c69 6f6e 7320 7769 7468 696e 2064  illions within d
-000057e0: 6563 6164 6573 272c 0a20 2020 2020 2020  ecades',.       
-000057f0: 2020 2020 2020 2020 2027 4368 696e 6573           'Chines
-00005800: 6520 6564 7563 6174 696f 6e20 666f 7220  e education for 
-00005810: 5456 2065 7870 6572 696d 656e 7427 2c0a  TV experiment',.
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 2741 6262 6f74 7420 676f 7665 726e 6d65  'Abbott governme
-00005840: 6e74 2073 7065 6e64 7320 2438 206d 696c  nt spends $8 mil
-00005850: 6c69 6f6e 206f 6e20 6869 6768 6572 2065  lion on higher e
-00005860: 6475 6361 7469 6f6e 272c 0a20 2020 2020  ducation',.     
-00005870: 2020 2020 2020 2020 2020 2027 4d69 6464             'Midd
-00005880: 6c65 2045 6173 7420 616e 6420 4173 6961  le East and Asia
-00005890: 2062 6f6f 7374 2069 6e76 6573 746d 656e   boost investmen
-000058a0: 7420 696e 2074 6f70 206c 6576 656c 2073  t in top level s
-000058b0: 706f 7274 7327 2c0a 2020 2020 2020 2020  ports',.        
-000058c0: 2020 2020 2020 2020 2753 756d 6d69 7420          'Summit 
-000058d0: 5365 7269 6573 206c 6f6f 6b20 6c61 756e  Series look laun
-000058e0: 6368 6573 2048 424f 2043 616e 6164 6120  ches HBO Canada 
-000058f0: 7370 6f72 7473 2064 6f63 2073 6572 6965  sports doc serie
-00005900: 733a 204d 7564 6861 7227 0a20 2020 2020  s: Mudhar'.     
-00005910: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00005920: 2020 2020 206d 2e74 7261 696e 2864 6174       m.train(dat
-00005930: 6129 0a20 2020 2020 2020 2020 2020 206d  a).            m
-00005940: 2e6c 6f61 645f 6d6f 6465 6c28 290a 2020  .load_model().  
-00005950: 2020 2020 2020 2020 2020 7220 3d20 6d2e            r = m.
-00005960: 7072 6564 6963 7428 5b27 4162 626f 7474  predict(['Abbott
-00005970: 2067 6f76 6572 6e6d 656e 7420 7370 656e   government spen
-00005980: 6473 2024 3820 6d69 6c6c 696f 6e20 6f6e  ds $8 million on
-00005990: 2068 6967 6865 7220 6564 7563 6174 696f   higher educatio
-000059a0: 6e20 6d65 6469 6120 626c 6974 7a27 2c0a  n media blitz',.
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2020 2020 2020 2020 2020 2027 4d69 6464             'Midd
-000059d0: 6c65 2045 6173 7420 616e 6420 4173 6961  le East and Asia
-000059e0: 2062 6f6f 7374 2069 6e76 6573 746d 656e   boost investmen
-000059f0: 7420 696e 2074 6f70 206c 6576 656c 2073  t in top level s
-00005a00: 706f 7274 7327 5d29 0a20 2020 2020 2020  ports']).       
-00005a10: 2020 2020 2070 7269 6e74 2872 290a 2020       print(r).  
-00005a20: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00005a30: 2020 2023 2323 2323 2323 2323 2323 206c     ########### l
-00005a40: 6f61 6420 6368 696e 6573 6520 7472 6169  oad chinese trai
-00005a50: 6e20 6461 7461 2066 726f 6d20 3177 2064  n data from 1w d
-00005a60: 6174 6120 6669 6c65 0a20 2020 2020 2020  ata file.       
-00005a70: 2020 2020 2066 726f 6d20 736b 6c65 6172       from sklear
-00005a80: 6e2e 6665 6174 7572 655f 6578 7472 6163  n.feature_extrac
-00005a90: 7469 6f6e 2e74 6578 7420 696d 706f 7274  tion.text import
-00005aa0: 2054 6669 6466 5665 6374 6f72 697a 6572   TfidfVectorizer
-00005ab0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005ac0: 2020 2020 2020 7463 6c75 7374 6572 203d        tcluster =
-00005ad0: 2054 6578 7443 6c75 7374 6572 286d 6f64   TextCluster(mod
-00005ae0: 656c 5f64 6972 3d27 6d6f 6465 6c73 2f63  el_dir='models/c
-00005af0: 6c75 7374 6572 272c 2066 6561 7475 7265  luster', feature
-00005b00: 3d54 6669 6466 5665 6374 6f72 697a 6572  =TfidfVectorizer
-00005b10: 286e 6772 616d 5f72 616e 6765 3d28 312c  (ngram_range=(1,
-00005b20: 2032 2929 2c20 6e5f 636c 7573 7465 7273   2)), n_clusters
-00005b30: 3d31 3029 0a20 2020 2020 2020 2020 2020  =10).           
-00005b40: 2064 6174 6120 3d20 7463 6c75 7374 6572   data = tcluster
-00005b50: 2e6c 6f61 645f 6669 6c65 5f64 6174 6128  .load_file_data(
-00005b60: 2774 6875 636e 6577 735f 7472 6169 6e5f  'thucnews_train_
-00005b70: 3177 2e74 7874 272c 2073 6570 3d27 5c74  1w.txt', sep='\t
-00005b80: 272c 2075 7365 5f63 6f6c 3d31 290a 2020  ', use_col=1).  
-00005b90: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-00005ba0: 652c 206c 6162 656c 7320 3d20 7463 6c75  e, labels = tclu
-00005bb0: 7374 6572 2e74 7261 696e 2864 6174 615b  ster.train(data[
-00005bc0: 3a35 3030 305d 290a 2020 2020 2020 2020  :5000]).        
-00005bd0: 2020 2020 7463 6c75 7374 6572 2e73 686f      tcluster.sho
-00005be0: 775f 636c 7573 7465 7273 2866 6561 7475  w_clusters(featu
-00005bf0: 7265 2c20 6c61 6265 6c73 2c20 276d 6f64  re, labels, 'mod
-00005c00: 656c 732f 636c 7573 7465 722f 636c 7573  els/cluster/clus
-00005c10: 7465 725f 7472 6169 6e5f 7365 675f 7361  ter_train_seg_sa
-00005c20: 6d70 6c65 732e 706e 6727 290a 2020 2020  mples.png').    
-00005c30: 2020 2020 2020 2020 7220 3d20 7463 6c75          r = tclu
-00005c40: 7374 6572 2e70 7265 6469 6374 2864 6174  ster.predict(dat
-00005c50: 615b 3a33 305d 290a 2020 2020 2020 2020  a[:30]).        
-00005c60: 2020 2020 7072 696e 7428 7229 0a20 2020      print(r).   
-00005c70: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
-00005c80: 200a 2020 2020 2020 2020 6f75 7470 7574   .        output
-00005c90: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
-00005ca0: 2020 2060 6060 0a20 2020 2020 2020 2054     ```.        T
-00005cb0: 6578 7443 6c75 7374 6572 2069 6e73 7461  extCluster insta
-00005cc0: 6e63 6520 284d 696e 6942 6174 6368 4b4d  nce (MiniBatchKM
-00005cd0: 6561 6e73 286e 5f63 6c75 7374 6572 733d  eans(n_clusters=
-00005ce0: 322c 206e 5f69 6e69 743d 3130 292c 203c  2, n_init=10), <
-00005cf0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00005d00: 2e75 7469 6c73 2e74 6f6b 656e 697a 6572  .utils.tokenizer
-00005d10: 2e54 6f6b 656e 697a 6572 206f 626a 6563  .Tokenizer objec
-00005d20: 7420 6174 2030 7837 6638 3062 6434 3638  t at 0x7f80bd468
-00005d30: 3262 303e 2c20 5466 6964 6656 6563 746f  2b0>, TfidfVecto
-00005d40: 7269 7a65 7228 6e67 7261 6d5f 7261 6e67  rizer(ngram_rang
-00005d50: 653d 2831 2c20 3229 2929 0a20 2020 2020  e=(1, 2))).     
-00005d60: 2020 205b 3120 3120 3120 3120 3120 3120     [1 1 1 1 1 1 
-00005d70: 3120 3120 3120 3120 3120 3820 3120 3120  1 1 1 1 1 8 1 1 
-00005d80: 3120 3120 3120 3120 3120 3120 3120 3120  1 1 1 1 1 1 1 1 
-00005d90: 3920 3120 3120 3820 3120 3120 3920 315d  9 1 1 8 1 1 9 1]
-00005da0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00005db0: 2020 2020 2063 6c75 7374 6572 696e 6720       clustering 
-00005dc0: 706c 6f74 2069 6d61 6765 3a0a 2020 2020  plot image:.    
-00005dd0: 2020 2020 0a20 2020 2020 2020 2021 5b63      .        ![c
-00005de0: 6c75 7374 6572 5f69 6d61 6765 5d28 646f  luster_image](do
-00005df0: 6373 2f63 6c75 7374 6572 5f74 7261 696e  cs/cluster_train
-00005e00: 5f73 6567 5f73 616d 706c 6573 2e70 6e67  _seg_samples.png
-00005e10: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00005e20: 2020 200a 2020 2020 2020 2020 2320 436f     .        # Co
-00005e30: 6e74 6163 740a 2020 2020 2020 2020 0a20  ntact.        . 
-00005e40: 2020 2020 2020 202d 2049 7373 7565 28e5         - Issue(.
-00005e50: bbba e8ae ae29 efbc 9a5b 215b 4769 7448  .....)...[![GitH
-00005e60: 7562 2069 7373 7565 735d 2868 7474 7073  ub issues](https
-00005e70: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00005e80: 6f2f 6769 7468 7562 2f69 7373 7565 732f  o/github/issues/
-00005e90: 7368 6962 696e 6736 3234 2f70 7974 6578  shibing624/pytex
-00005ea0: 7463 6c61 7373 6966 6965 722e 7376 6729  tclassifier.svg)
-00005eb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005ec0: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
-00005ed0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00005ee0: 2f69 7373 7565 7329 0a20 2020 2020 2020  /issues).       
-00005ef0: 202d 20e9 82ae e4bb b6e6 8891 efbc 9a78   - ............x
-00005f00: 756d 696e 673a 2078 756d 696e 6736 3234  uming: xuming624
-00005f10: 4071 712e 636f 6d0a 2020 2020 2020 2020  @qq.com.        
-00005f20: 2d20 e5be aee4 bfa1 e688 91ef bc9a e58a  - ..............
-00005f30: a0e6 8891 2ae5 beae e4bf a1e5 8fb7 efbc  ....*...........
-00005f40: 9a78 756d 696e 6736 3234 2a2c 20e8 bf9b  .xuming624*, ...
-00005f50: 5079 7468 6f6e 2d4e 4c50 e4ba a4e6 b581  Python-NLP......
-00005f60: e7be a4ef bc8c e5a4 87e6 b3a8 efbc 9a2a  ...............*
-00005f70: e5a7 93e5 908d 2de5 85ac e58f b8e5 908d  ......-.........
-00005f80: 2d4e 4c50 2a0a 2020 2020 2020 2020 3c69  -NLP*.        <i
-00005f90: 6d67 2073 7263 3d22 646f 6373 2f77 6563  mg src="docs/wec
-00005fa0: 6861 742e 6a70 6567 2220 7769 6474 683d  hat.jpeg" width=
-00005fb0: 2232 3030 2220 2f3e 0a20 2020 2020 2020  "200" />.       
-00005fc0: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-00005fd0: 2020 2023 2043 6974 6174 696f 6e0a 2020     # Citation.  
-00005fe0: 2020 2020 2020 0a20 2020 2020 2020 20e5        .        .
-00005ff0: a682 e69e 9ce4 bda0 e59c a8e7 a094 e7a9  ................
-00006000: b6e4 b8ad e4bd bfe7 94a8 e4ba 8670 7974  .............pyt
-00006010: 6578 7463 6c61 7373 6966 6965 72ef bc8c  extclassifier...
-00006020: e8af b7e6 8c89 e5a6 82e4 b88b e6a0 bce5  ................
-00006030: bc8f e5bc 95e7 94a8 efbc 9a0a 2020 2020  ............    
-00006040: 2020 2020 0a20 2020 2020 2020 2041 5041      .        APA
-00006050: 3a0a 2020 2020 2020 2020 6060 606c 6174  :.        ```lat
-00006060: 6578 0a20 2020 2020 2020 2058 752c 204d  ex.        Xu, M
-00006070: 2e20 5079 7465 7874 636c 6173 7369 6669  . Pytextclassifi
-00006080: 6572 3a20 5465 7874 2063 6c61 7373 6966  er: Text classif
-00006090: 6965 7220 746f 6f6c 6b69 7420 666f 7220  ier toolkit for 
-000060a0: 4e4c 5020 2856 6572 7369 6f6e 2031 2e32  NLP (Version 1.2
-000060b0: 2e30 2920 5b43 6f6d 7075 7465 7220 736f  .0) [Computer so
-000060c0: 6674 7761 7265 5d2e 2068 7474 7073 3a2f  ftware]. https:/
-000060d0: 2f67 6974 6875 622e 636f 6d2f 7368 6962  /github.com/shib
-000060e0: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
-000060f0: 7373 6966 6965 720a 2020 2020 2020 2020  ssifier.        
-00006100: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00006110: 2020 2020 2042 6962 5465 583a 0a20 2020       BibTeX:.   
-00006120: 2020 2020 2060 6060 6c61 7465 780a 2020       ```latex.  
-00006130: 2020 2020 2020 406d 6973 637b 5079 7465        @misc{Pyte
-00006140: 7874 636c 6173 7369 6669 6572 2c0a 2020  xtclassifier,.  
-00006150: 2020 2020 2020 2020 7469 746c 653d 7b50          title={P
-00006160: 7974 6578 7463 6c61 7373 6966 6965 723a  ytextclassifier:
-00006170: 2054 6578 7420 636c 6173 7369 6669 6572   Text classifier
-00006180: 2074 6f6f 6c6b 6974 2066 6f72 204e 4c50   toolkit for NLP
-00006190: 7d2c 0a20 2020 2020 2020 2020 2061 7574  },.          aut
-000061a0: 686f 723d 7b58 7520 4d69 6e67 7d2c 0a20  hor={Xu Ming},. 
-000061b0: 2020 2020 2020 2020 2079 6561 723d 7b32           year={2
-000061c0: 3032 327d 2c0a 2020 2020 2020 2020 2020  022},.          
-000061d0: 686f 7770 7562 6c69 7368 6564 3d7b 5c75  howpublished={\u
-000061e0: 726c 7b68 7474 7073 3a2f 2f67 6974 6875  rl{https://githu
-000061f0: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
-00006200: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
-00006210: 727d 7d2c 0a20 2020 2020 2020 207d 0a20  r}},.        }. 
-00006220: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00006230: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00006240: 2020 2020 2023 204c 6963 656e 7365 0a20       # License. 
-00006250: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006260: 0a20 2020 2020 2020 20e6 8e88 e69d 83e5  .        .......
-00006270: 8d8f e8ae aee4 b8ba 205b 5468 6520 4170  ........ [The Ap
-00006280: 6163 6865 204c 6963 656e 7365 2032 2e30  ache License 2.0
-00006290: 5d28 4c49 4345 4e53 4529 efbc 8ce5 8faf  ](LICENSE)......
-000062a0: e585 8de8 b4b9 e794 a8e5 819a e595 86e4  ................
-000062b0: b89a e794 a8e9 8094 e380 82e8 afb7 e59c  ................
-000062c0: a8e4 baa7 e593 81e8 afb4 e698 8ee4 b8ad  ................
-000062d0: e999 84e5 8aa0 2a2a 7079 7465 7874 636c  ......**pytextcl
-000062e0: 6173 7369 6669 6572 2a2a e79a 84e9 93be  assifier**......
-000062f0: e68e a5e5 928c e68e 88e6 9d83 e58d 8fe8  ................
-00006300: aeae e380 820a 2020 2020 2020 2020 0a20  ......        . 
-00006310: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006320: 2320 436f 6e74 7269 6275 7465 0a20 2020  # Contribute.   
-00006330: 2020 2020 20e9 a1b9 e79b aee4 bba3 e7a0       ...........
-00006340: 81e8 bf98 e5be 88e7 b297 e7b3 99ef bc8c  ................
-00006350: e5a6 82e6 9e9c e5a4 a7e5 aeb6 e5af b9e4  ................
-00006360: bba3 e7a0 81e6 9c89 e689 80e6 94b9 e8bf  ................
-00006370: 9bef bc8c e6ac a2e8 bf8e e68f 90e4 baa4  ................
-00006380: e59b 9ee6 9cac e9a1 b9e7 9bae efbc 8ce5  ................
-00006390: 9ca8 e68f 90e4 baa4 e4b9 8be5 898d efbc  ................
-000063a0: 8ce6 b3a8 e684 8fe4 bba5 e4b8 8be4 b8a4  ................
-000063b0: e782 b9ef bc9a 0a20 2020 2020 2020 200a  .......        .
-000063c0: 2020 2020 2020 2020 202d 20e5 9ca8 6074           - ...`t
-000063d0: 6573 7473 60e6 b7bb e58a a0e7 9bb8 e5ba  ests`...........
-000063e0: 94e7 9a84 e58d 95e5 8583 e6b5 8be8 af95  ................
-000063f0: 0a20 2020 2020 2020 2020 2d20 e4bd bfe7  .         - ....
-00006400: 94a8 6070 7974 686f 6e20 7365 7475 702e  ..`python setup.
-00006410: 7079 2074 6573 7460 e69d a5e8 bf90 e8a1  py test`........
-00006420: 8ce6 8980 e69c 89e5 8d95 e585 83e6 b58b  ................
-00006430: e8af 95ef bc8c e7a1 aee4 bf9d e689 80e6  ................
-00006440: 9c89 e58d 95e6 b58b e983 bde6 98af e980  ................
-00006450: 9ae8 bf87 e79a 840a 2020 2020 2020 2020  ........        
-00006460: 0a20 2020 2020 2020 20e4 b98b e590 8ee5  .        .......
-00006470: 8db3 e58f afe6 8f90 e4ba a450 52e3 8082  ...........PR...
-00006480: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006490: 2020 0a20 2020 2020 2020 2023 2052 6566    .        # Ref
-000064a0: 6572 656e 6365 0a20 2020 2020 2020 200a  erence.        .
-000064b0: 2020 2020 2020 2020 2d20 5365 6e74 696d          - Sentim
-000064c0: 656e 7450 6f6c 6172 6974 7941 6e61 6c79  entPolarityAnaly
-000064d0: 7369 730a 2020 2020 2020 2020 0a4b 6579  sis.        .Key
-000064e0: 776f 7264 733a 2070 7974 6578 7463 6c61  words: pytextcla
-000064f0: 7373 6966 6965 722c 7465 7874 636c 6173  ssifier,textclas
-00006500: 7369 6669 6572 2c63 6c61 7373 6966 6965  sifier,classifie
-00006510: 722c 7465 7874 636c 6173 7369 6669 6361  r,textclassifica
-00006520: 7469 6f6e 0a50 6c61 7466 6f72 6d3a 2055  tion.Platform: U
-00006530: 4e4b 4e4f 574e 0a43 6c61 7373 6966 6965  NKNOWN.Classifie
-00006540: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00006550: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
-00006560: 5265 7365 6172 6368 0a43 6c61 7373 6966  Research.Classif
-00006570: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00006580: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00006590: 7065 6e64 656e 740a 436c 6173 7369 6669  pendent.Classifi
-000065a0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-000065b0: 5349 2041 7070 726f 7665 6420 3a3a 2041  SI Approved :: A
-000065c0: 7061 6368 6520 536f 6674 7761 7265 204c  pache Software L
-000065d0: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
-000065e0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000065f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00006600: 6e0a 436c 6173 7369 6669 6572 3a20 5072  n.Classifier: Pr
-00006610: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00006620: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00006630: 322e 370a 436c 6173 7369 6669 6572 3a20  2.7.Classifier: 
-00006640: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00006650: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00006660: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-00006670: 546f 7069 6320 3a3a 2054 6578 7420 5072  Topic :: Text Pr
-00006680: 6f63 6573 7369 6e67 203a 3a20 4c69 6e67  ocessing :: Ling
-00006690: 7569 7374 6963 0a43 6c61 7373 6966 6965  uistic.Classifie
-000066a0: 723a 2054 6f70 6963 203a 3a20 5363 6965  r: Topic :: Scie
-000066b0: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-000066c0: 6e67 203a 3a20 4172 7469 6669 6369 616c  ng :: Artificial
-000066d0: 2049 6e74 656c 6c69 6765 6e63 650a 4465   Intelligence.De
-000066e0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-000066f0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00006700: 6b64 6f77 6e0a                           kdown.
+000046f0: 2020 6966 206e 6f74 206c 696e 653a 0a20    if not line:. 
+00004700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004710: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004730: 2020 2020 7465 726d 7320 3d20 6c69 6e65      terms = line
+00004740: 2e73 706c 6974 2827 2c27 290a 2020 2020  .split(',').    
+00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004760: 6966 206c 656e 2874 6572 6d73 2920 213d  if len(terms) !=
+00004770: 2031 363a 0a20 2020 2020 2020 2020 2020   16:.           
+00004780: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00004790: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+000047a0: 2020 2020 2020 2020 2020 7661 6c20 3d20            val = 
+000047b0: 5b69 6e74 2869 2920 666f 7220 6920 696e  [int(i) for i in
+000047c0: 2074 6572 6d73 5b31 3a5d 5d0a 2020 2020   terms[1:]].    
+000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047e0: 6461 7461 2e61 7070 656e 6428 5b74 6572  data.append([ter
+000047f0: 6d73 5b30 5d2c 2076 616c 5d29 0a20 2020  ms[0], val]).   
+00004800: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004810: 6461 7461 0a20 2020 2020 2020 200a 2020  data.        .  
+00004820: 2020 2020 2020 0a20 2020 2020 2020 2069        .        i
+00004830: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 275f  f __name__ == '_
+00004840: 5f6d 6169 6e5f 5f27 3a0a 2020 2020 2020  _main__':.      
+00004850: 2020 2020 2020 2320 6d6f 6465 6c5f 7479        # model_ty
+00004860: 7065 3a20 7375 7070 6f72 7420 2762 6572  pe: support 'ber
+00004870: 7427 2c20 2761 6c62 6572 7427 2c20 2772  t', 'albert', 'r
+00004880: 6f62 6572 7461 272c 2027 786c 6e65 7427  oberta', 'xlnet'
+00004890: 0a20 2020 2020 2020 2020 2020 2023 206d  .            # m
+000048a0: 6f64 656c 5f6e 616d 653a 2073 7570 706f  odel_name: suppo
+000048b0: 7274 2027 6265 7274 2d62 6173 652d 6368  rt 'bert-base-ch
+000048c0: 696e 6573 6527 2c20 2762 6572 742d 6261  inese', 'bert-ba
+000048d0: 7365 2d63 6173 6564 272c 2027 6265 7274  se-cased', 'bert
+000048e0: 2d62 6173 652d 6d75 6c74 696c 696e 6775  -base-multilingu
+000048f0: 616c 2d63 6173 6564 2720 2e2e 2e0a 2020  al-cased' ....  
+00004900: 2020 2020 2020 2020 2020 6d20 3d20 4265            m = Be
+00004910: 7274 436c 6173 7369 6669 6572 286f 7574  rtClassifier(out
+00004920: 7075 745f 6469 723d 276d 6f64 656c 732f  put_dir='models/
+00004930: 6d75 6c74 696c 6162 656c 2d62 6572 742d  multilabel-bert-
+00004940: 7a68 2d6d 6f64 656c 272c 206e 756d 5f63  zh-model', num_c
+00004950: 6c61 7373 6573 3d31 352c 0a20 2020 2020  lasses=15,.     
+00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004970: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+00004980: 7479 7065 3d27 6265 7274 272c 206d 6f64  type='bert', mod
+00004990: 656c 5f6e 616d 653d 2762 6572 742d 6261  el_name='bert-ba
+000049a0: 7365 2d63 6869 6e65 7365 272c 206e 756d  se-chinese', num
+000049b0: 5f65 706f 6368 733d 322c 206d 756c 7469  _epochs=2, multi
+000049c0: 5f6c 6162 656c 3d54 7275 6529 0a20 2020  _label=True).   
+000049d0: 2020 2020 2020 2020 2023 2054 7261 696e           # Train
+000049e0: 2061 6e64 2045 7661 6c75 6174 696f 6e20   and Evaluation 
+000049f0: 6461 7461 206e 6565 6473 2074 6f20 6265  data needs to be
+00004a00: 2069 6e20 6120 5061 6e64 6173 2044 6174   in a Pandas Dat
+00004a10: 6166 7261 6d65 2063 6f6e 7461 696e 696e  aframe containin
+00004a20: 6720 6174 206c 6561 7374 2074 776f 2063  g at least two c
+00004a30: 6f6c 756d 6e73 2c20 6120 2774 6578 7427  olumns, a 'text'
+00004a40: 2061 6e64 2061 2027 6c61 6265 6c73 2720   and a 'labels' 
+00004a50: 636f 6c75 6d6e 2e20 5468 6520 606c 6162  column. The `lab
+00004a60: 656c 7360 2063 6f6c 756d 6e20 7368 6f75  els` column shou
+00004a70: 6c64 2063 6f6e 7461 696e 206d 756c 7469  ld contain multi
+00004a80: 2d68 6f74 2065 6e63 6f64 6564 206c 6973  -hot encoded lis
+00004a90: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+00004aa0: 7472 6169 6e5f 6461 7461 203d 205b 0a20  train_data = [. 
+00004ab0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00004ac0: 22e4 b880 e4b8 aae5 b08f e697 b6e6 88bf  "...............
+00004ad0: e997 b4e4 bb8d e784 b6e6 b2a1 e69a 96e5  ................
+00004ae0: 928c 222c 205b 302c 2030 2c20 302c 2030  ..", [0, 0, 0, 0
+00004af0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00004b00: 2030 2c20 302c 2030 2c20 312c 2030 2c20   0, 0, 0, 1, 0, 
+00004b10: 305d 5d2c 0a20 2020 2020 2020 2020 2020  0]],.           
+00004b20: 2020 2020 205b 22e8 8097 e794 b5e6 8385       [".........
+00004b30: e586 b5ef bc9a e8bf 99e4 b8aa e6b2 a1e6  ................
+00004b40: 9c89 e6b3 a8e6 848f 222c 205b 302c 2030  ........", [0, 0
+00004b50: 2c20 312c 2030 2c20 302c 2030 2c20 302c  , 1, 0, 0, 0, 0,
+00004b60: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00004b70: 302c 2030 2c20 305d 5d2c 0a20 2020 2020  0, 0, 0]],.     
+00004b80: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00004b90: 2020 2020 2064 6174 6120 3d20 6c6f 6164       data = load
+00004ba0: 5f6a 645f 6461 7461 2827 6d75 6c74 696c  _jd_data('multil
+00004bb0: 6162 656c 5f6a 645f 636f 6d6d 656e 7473  abel_jd_comments
+00004bc0: 2e63 7376 2729 0a20 2020 2020 2020 2020  .csv').         
+00004bd0: 2020 2074 7261 696e 5f64 6174 612e 6578     train_data.ex
+00004be0: 7465 6e64 2864 6174 6129 0a20 2020 2020  tend(data).     
+00004bf0: 2020 2020 2020 2070 7269 6e74 2874 7261         print(tra
+00004c00: 696e 5f64 6174 615b 3a35 5d29 0a20 2020  in_data[:5]).   
+00004c10: 2020 2020 2020 2020 2074 7261 696e 5f64           train_d
+00004c20: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+00004c30: 2874 7261 696e 5f64 6174 612c 2063 6f6c  (train_data, col
+00004c40: 756d 6e73 3d5b 2274 6578 7422 2c20 226c  umns=["text", "l
+00004c50: 6162 656c 7322 5d29 0a20 2020 2020 2020  abels"]).       
+00004c60: 200a 2020 2020 2020 2020 2020 2020 7072   .            pr
+00004c70: 696e 7428 7472 6169 6e5f 6466 2e68 6561  int(train_df.hea
+00004c80: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
+00004c90: 206d 2e74 7261 696e 2874 7261 696e 5f64   m.train(train_d
+00004ca0: 6629 0a20 2020 2020 2020 2020 2020 2070  f).            p
+00004cb0: 7269 6e74 286d 290a 2020 2020 2020 2020  rint(m).        
+00004cc0: 2020 2020 2320 4576 616c 7561 7465 2074      # Evaluate t
+00004cd0: 6865 206d 6f64 656c 0a20 2020 2020 2020  he model.       
+00004ce0: 2020 2020 2061 6363 5f73 636f 7265 203d       acc_score =
+00004cf0: 206d 2e65 7661 6c75 6174 655f 6d6f 6465   m.evaluate_mode
+00004d00: 6c28 7472 6169 6e5f 6466 5b3a 3230 5d29  l(train_df[:20])
+00004d10: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00004d20: 6e74 2866 2761 6363 5f73 636f 7265 3a20  nt(f'acc_score: 
+00004d30: 7b61 6363 5f73 636f 7265 7d27 290a 2020  {acc_score}').  
+00004d40: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00004d50: 2020 2023 206c 6f61 6420 7472 6169 6e65     # load traine
+00004d60: 6420 6265 7374 206d 6f64 656c 2066 726f  d best model fro
+00004d70: 6d20 6d6f 6465 6c5f 6469 720a 2020 2020  m model_dir.    
+00004d80: 2020 2020 2020 2020 6d2e 6c6f 6164 5f6d          m.load_m
+00004d90: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
+00004da0: 2020 2070 7265 6469 6374 5f6c 6162 656c     predict_label
+00004db0: 2c20 7072 6564 6963 745f 7072 6f62 6120  , predict_proba 
+00004dc0: 3d20 6d2e 7072 6564 6963 7428 5b27 e4b8  = m.predict(['..
+00004dd0: 80e4 b8aa e5b0 8fe6 97b6 e688 bfe9 97b4  ................
+00004de0: e4bb 8de7 84b6 e6b2 a1e6 9a96 e592 8c27  ...............'
+00004df0: 2c20 27e8 8097 e794 b5e6 8385 e586 b5ef  , '.............
+00004e00: bc9a e8bf 99e4 b8aa e6b2 a1e6 9c89 e6b3  ................
+00004e10: a8e6 848f 275d 290a 2020 2020 2020 2020  ....']).        
+00004e20: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
+00004e30: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
+00004e40: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
+00004e50: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
+00004e60: 6963 745f 7072 6f62 617d 2729 0a20 2020  ict_proba}').   
+00004e70: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+00004e80: 200a 2020 2020 2020 2020 2323 2045 7661   .        ## Eva
+00004e90: 6c75 6174 696f 6e0a 2020 2020 2020 2020  luation.        
+00004ea0: 0a20 2020 2020 2020 2023 2323 2044 6174  .        ### Dat
+00004eb0: 6173 6574 0a20 2020 2020 2020 200a 2020  aset.        .  
+00004ec0: 2020 2020 2020 312e 2054 4855 434e 6577        1. THUCNew
+00004ed0: 73e4 b8ad e696 87e6 9687 e69c ace6 95b0  s...............
+00004ee0: e68d aee9 9b86 efbc 8831 2e35 3647 42ef  .........1.56GB.
+00004ef0: bc89 efbc 9ae5 ae98 e696 b95b e4b8 8be8  ...........[....
+00004f00: bdbd e59c b0e5 9d80 5d28 6874 7470 3a2f  ........](http:/
+00004f10: 2f74 6875 6374 632e 7468 756e 6c70 2e6f  /thuctc.thunlp.o
+00004f20: 7267 2f29 efbc 8ce6 8abd e6a0 b7e4 ba86  rg/)............
+00004f30: 3130 e4b8 87e6 9da1 5448 5543 4e65 7773  10......THUCNews
+00004f40: e4b8 ade6 9687 e696 87e6 9cac 3130 e588  ............10..
+00004f50: 86e7 b1bb e695 b0e6 8dae e99b 86ef bc88  ................
+00004f60: 364d 42ef bc89 efbc 8ce5 9cb0 e59d 80ef  6MB.............
+00004f70: bc9a 5b65 7861 6d70 6c65 732f 7468 7563  ..[examples/thuc
+00004f80: 6e65 7773 5f74 7261 696e 5f31 3077 2e74  news_train_10w.t
+00004f90: 7874 5d28 6874 7470 733a 2f2f 6769 7468  xt](https://gith
+00004fa0: 7562 2e63 6f6d 2f73 6869 6269 6e67 3632  ub.com/shibing62
+00004fb0: 342f 7079 7465 7874 636c 6173 7369 6669  4/pytextclassifi
+00004fc0: 6572 2f62 6c6f 622f 6d61 7374 6572 2f65  er/blob/master/e
+00004fd0: 7861 6d70 6c65 732f 7468 7563 6e65 7773  xamples/thucnews
+00004fe0: 5f74 7261 696e 5f31 3077 2e74 7874 29e3  _train_10w.txt).
+00004ff0: 8082 0a20 2020 2020 2020 2032 2e20 544e  ...        2. TN
+00005000: 4557 53e4 bb8a e697 a5e5 a4b4 e69d a1e4  EWS.............
+00005010: b8ad e696 87e6 96b0 e997 bbef bc88 e79f  ................
+00005020: ade6 9687 e69c acef bc89 e588 86e7 b1bb  ................
+00005030: 2053 686f 7274 2054 6578 7420 436c 6173   Short Text Clas
+00005040: 7369 6669 6361 6974 6f6e 2066 6f72 204e  sificaiton for N
+00005050: 6577 73ef bc8c e8af a5e6 95b0 e68d aee9  ews.............
+00005060: 9b86 2835 2e31 4d42 29e6 9da5 e887 aae4  ..(5.1MB).......
+00005070: bb8a e697 a5e5 a4b4 e69d a1e7 9a84 e696  ................
+00005080: b0e9 97bb e789 88e5 9d97 efbc 8ce5 85b1  ................
+00005090: e68f 90e5 8f96 e4ba 8631 35e4 b8aa e7b1  .........15.....
+000050a0: bbe5 88ab e79a 84e6 96b0 e997 bbef bc8c  ................
+000050b0: e58c 85e6 8bac e697 85e6 b8b8 efbc 8ce6  ................
+000050c0: 9599 e882 b2ef bc8c e987 91e8 9e8d efbc  ................
+000050d0: 8ce5 869b e4ba 8be7 ad89 efbc 8ce5 9cb0  ................
+000050e0: e59d 80ef bc9a 5b74 6e65 7773 5f70 7562  ......[tnews_pub
+000050f0: 6c69 632e 7a69 705d 2868 7474 7073 3a2f  lic.zip](https:/
+00005100: 2f73 746f 7261 6765 2e67 6f6f 676c 6561  /storage.googlea
+00005110: 7069 732e 636f 6d2f 636c 7565 6265 6e63  pis.com/cluebenc
+00005120: 686d 6172 6b2f 7461 736b 732f 746e 6577  hmark/tasks/tnew
+00005130: 735f 7075 626c 6963 2e7a 6970 290a 2020  s_public.zip).  
+00005140: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00005150: 2323 2045 7661 6c75 6174 696f 6e20 5265  ## Evaluation Re
+00005160: 7375 6c74 0a20 2020 2020 2020 20e5 9ca8  sult.        ...
+00005170: 5448 5543 4e65 7773 e4b8 ade6 9687 e696  THUCNews........
+00005180: 87e6 9cac 3130 e588 86e7 b1bb e695 b0e6  ....10..........
+00005190: 8dae e99b 86ef bc88 364d 42ef bc89 e4b8  ........6MB.....
+000051a0: 8ae8 af84 e4bc b0ef bc8c e6a8 a1e5 9e8b  ................
+000051b0: e59c a8e6 b58b e8af 95e9 9b86 2874 6573  ............(tes
+000051c0: 7429 e8af 84e6 b58b e695 88e6 9e9c e5a6  t)..............
+000051d0: 82e4 b88b efbc 9a0a 2020 2020 2020 2020  ........        
+000051e0: 0a20 2020 2020 2020 20e6 a8a1 e59e 8b7c  .        ......|
+000051f0: 6163 637c e8af b4e6 988e 0a20 2020 2020  acc|.......     
+00005200: 2020 202d 2d7c 2d2d 7c2d 2d0a 2020 2020     --|--|--.    
+00005210: 2020 2020 4c52 7c30 2e38 3830 337c e980      LR|0.8803|..
+00005220: bbe8 be91 e59b 9ee5 bd92 4c6f 6769 7374  ..........Logist
+00005230: 6963 7320 5265 6772 6573 7369 6f6e 0a20  ics Regression. 
+00005240: 2020 2020 2020 2054 6578 7443 4e4e 7c30         TextCNN|0
+00005250: 2e38 3830 397c 4b69 6d20 3230 3134 20e7  .8809|Kim 2014 .
+00005260: bb8f e585 b8e7 9a84 434e 4ee6 9687 e69c  ........CNN.....
+00005270: ace5 8886 e7b1 bb0a 2020 2020 2020 2020  ........        
+00005280: 5465 7874 524e 4e5f 4174 747c 302e 3930  TextRNN_Att|0.90
+00005290: 3232 7c42 694c 5354 4d2b 4174 7465 6e74  22|BiLSTM+Attent
+000052a0: 696f 6e0a 2020 2020 2020 2020 4661 7374  ion.        Fast
+000052b0: 5465 7874 7c30 2e39 3137 377c 626f 772b  Text|0.9177|bow+
+000052c0: 6269 6772 616d 2b74 7269 6772 616d efbc  bigram+trigram..
+000052d0: 8c20 e695 88e6 9e9c e587 bae5 a587 e79a  . ..............
+000052e0: 84e5 a5bd 0a20 2020 2020 2020 2044 5043  .....        DPC
+000052f0: 4e4e 7c30 2e39 3132 357c e6b7 b1e5 b182  NN|0.9125|......
+00005300: e987 91e5 ad97 e5a1 9443 4e4e 0a20 2020  .........CNN.   
+00005310: 2020 2020 2054 7261 6e73 666f 726d 6572       Transformer
+00005320: 7c30 2e38 3939 317c e695 88e6 9e9c e8be  |0.8991|........
+00005330: 83e5 b7ae 0a20 2020 2020 2020 2042 4552  .....        BER
+00005340: 542d 6261 7365 7c2a 2a30 2e39 3438 332a  T-base|**0.9483*
+00005350: 2a7c 6265 7274 202b 2066 630a 2020 2020  *|bert + fc.    
+00005360: 2020 2020 4552 4e49 457c 302e 3934 3631      ERNIE|0.9461
+00005370: 7ce6 af94 6265 7274 e795 a5e5 b7ae 0a20  |...bert....... 
+00005380: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005390: e59c a8e4 b8ad e696 87e6 96b0 e997 bbe7  ................
+000053a0: 9fad e696 87e6 9cac e588 86e7 b1bb e695  ................
+000053b0: b0e6 8dae e99b 8654 4e45 5753 e4b8 8ae8  .......TNEWS....
+000053c0: af84 e4bc b0ef bc8c e6a8 a1e5 9e8b e59c  ................
+000053d0: a8e5 bc80 e58f 91e9 9b86 2864 6576 29e8  ..........(dev).
+000053e0: af84 e6b5 8be6 9588 e69e 9ce5 a682 e4b8  ................
+000053f0: 8bef bc9a 0a20 2020 2020 2020 200a 2020  .....        .  
+00005400: 2020 2020 2020 e6a8 a1e5 9e8b 7c61 6363        ......|acc
+00005410: 7ce8 afb4 e698 8e0a 2020 2020 2020 2020  |.......        
+00005420: 2d2d 7c2d 2d7c 2d2d 0a20 2020 2020 2020  --|--|--.       
+00005430: 2042 4552 542d 6261 7365 7c2a 2a30 2e35   BERT-base|**0.5
+00005440: 3636 302a 2a7c e69c ace9 a1b9 e79b aee5  660**|..........
+00005450: ae9e e78e b00a 2020 2020 2020 2020 4245  ......        BE
+00005460: 5254 2d62 6173 657c 302e 3536 3039 7c43  RT-base|0.5609|C
+00005470: 4c55 4520 4265 6e63 686d 6172 6b20 4c65  LUE Benchmark Le
+00005480: 6164 6572 626f 6172 64e7 bb93 e69e 9c20  aderboard...... 
+00005490: 5b43 4c55 4562 656e 6368 6d61 726b 5d28  [CLUEbenchmark](
+000054a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000054b0: 6f6d 2f43 4c55 4562 656e 6368 6d61 726b  om/CLUEbenchmark
+000054c0: 2f43 4c55 4529 0a20 2020 2020 2020 200a  /CLUE).        .
+000054d0: 2020 2020 2020 2020 2d20 e4bb a5e4 b88a          - ......
+000054e0: e7bb 93e6 9e9c e59d 87e4 b8ba e588 86e7  ................
+000054f0: b1bb e79a 84e5 8786 e7a1 aee7 8e87 efbc  ................
+00005500: 8861 6363 7572 6163 79ef bc89 e7bb 93e6  .accuracy.......
+00005510: 9e9c 0a20 2020 2020 2020 202d 2054 4855  ...        - THU
+00005520: 434e 6577 73e6 95b0 e68d aee9 9b86 e8af  CNews...........
+00005530: 84e6 b58b e7bb 93e6 9e9c e58f afe4 bba5  ................
+00005540: e59f bae4 ba8e 6065 7861 6d70 6c65 732f  ......`examples/
+00005550: 7468 7563 6e65 7773 5f74 7261 696e 5f31  thucnews_train_1
+00005560: 3077 2e74 7874 60e6 95b0 e68d aee7 94a8  0w.txt`.........
+00005570: 6065 7861 6d70 6c65 7360 e4b8 8be7 9a84  `examples`......
+00005580: e590 84e6 a8a1 e59e 8b64 656d 6fe5 a48d  .........demo...
+00005590: e78e b00a 2020 2020 2020 2020 2d20 544e  ....        - TN
+000055a0: 4557 53e6 95b0 e68d aee9 9b86 e8af 84e6  EWS.............
+000055b0: b58b e7bb 93e6 9e9c e58f afe4 bba5 e4b8  ................
+000055c0: 8be8 bdbd 544e 4557 53e6 95b0 e68d aee9  ....TNEWS.......
+000055d0: 9b86 efbc 8ce8 bf90 e8a1 8c60 6578 616d  ...........`exam
+000055e0: 706c 6573 2f62 6572 745f 636c 6173 7369  ples/bert_classi
+000055f0: 6669 6361 7469 6f6e 5f74 6e65 7773 5f64  fication_tnews_d
+00005600: 656d 6f2e 7079 60e5 a48d e78e b00a 2020  emo.py`.......  
+00005610: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00005620: 2323 20e5 91bd e4bb a4e8 a18c e8b0 83e7  ## .............
+00005630: 94a8 0a20 2020 2020 2020 200a 2020 2020  ...        .    
+00005640: 2020 2020 e68f 90e4 be9b e588 86e7 b1bb      ............
+00005650: e6a8 a1e5 9e8b e591 bde4 bba4 e8a1 8ce8  ................
+00005660: b083 e794 a8e8 849a e69c acef bc8c e696  ................
+00005670: 87e4 bbb6 e6a0 91ef bc9a 0a20 2020 2020  ...........     
+00005680: 2020 2060 6060 6261 7368 0a20 2020 2020     ```bash.     
+00005690: 2020 2070 7974 6578 7463 6c61 7373 6966     pytextclassif
+000056a0: 6965 720a 2020 2020 2020 2020 e294 9ce2  ier.        ....
+000056b0: 9480 e294 8020 6265 7274 5f63 6c61 7373  ..... bert_class
+000056c0: 6966 6965 722e 7079 0a20 2020 2020 2020  ifier.py.       
+000056d0: 20e2 949c e294 80e2 9480 2066 6173 7474   ......... fastt
+000056e0: 6578 745f 636c 6173 7369 6669 6572 2e70  ext_classifier.p
+000056f0: 790a 2020 2020 2020 2020 e294 9ce2 9480  y.        ......
+00005700: e294 8020 636c 6173 7369 635f 636c 6173  ... classic_clas
+00005710: 7369 6669 6572 2e70 790a 2020 2020 2020  sifier.py.      
+00005720: 2020 e294 9ce2 9480 e294 8020 7465 7874    ......... text
+00005730: 636e 6e5f 636c 6173 7369 6669 6572 2e70  cnn_classifier.p
+00005740: 790a 2020 2020 2020 2020 e294 94e2 9480  y.        ......
+00005750: e294 8020 7465 7874 726e 6e5f 636c 6173  ... textrnn_clas
+00005760: 7369 6669 6572 2e70 790a 2020 2020 2020  sifier.py.      
+00005770: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
+00005780: 2020 2020 2020 20e6 af8f e4b8 aae6 9687         .........
+00005790: e4bb b6e5 afb9 e5ba 94e4 b880 e4b8 aae6  ................
+000057a0: a8a1 e59e 8be6 96b9 e6b3 95ef bc8c e590  ................
+000057b0: 84e6 a8a1 e59e 8be5 ae8c e585 a8e7 8bac  ................
+000057c0: e7ab 8bef bc8c e58f afe4 bba5 e79b b4e6  ................
+000057d0: 8ea5 e8bf 90e8 a18c efbc 8ce4 b99f e696  ................
+000057e0: b9e4 bebf e4bf aee6 94b9 efbc 8ce6 94af  ................
+000057f0: e68c 81e9 809a e8bf 8760 6172 6770 6172  .........`argpar
+00005800: 7365 6020 e4bf aee6 94b9 602d 2d64 6174  se` ......`--dat
+00005810: 615f 7061 7468 60e7 ad89 e58f 82e6 95b0  a_path`.........
+00005820: e380 820a 2020 2020 2020 2020 0a20 2020  ....        .   
+00005830: 2020 2020 20e7 9bb4 e68e a5e5 9ca8 e7bb       ...........
+00005840: 88e7 abaf e8b0 83e7 94a8 6661 7374 7465  ..........fastte
+00005850: 7874 e6a8 a1e5 9e8b e8ae ade7 bb83 efbc  xt..............
+00005860: 9a0a 2020 2020 2020 2020 6060 6062 6173  ..        ```bas
+00005870: 680a 2020 2020 2020 2020 7079 7468 6f6e  h.        python
+00005880: 202d 6d20 7079 7465 7874 636c 6173 7369   -m pytextclassi
+00005890: 6669 6572 2e66 6173 7474 6578 745f 636c  fier.fasttext_cl
+000058a0: 6173 7369 6669 6572 202d 680a 2020 2020  assifier -h.    
+000058b0: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+000058c0: 0a20 2020 2020 2020 2023 2320 5465 7874  .        ## Text
+000058d0: 2043 6c75 7374 6572 0a20 2020 2020 2020   Cluster.       
+000058e0: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
+000058f0: 2020 2054 6578 7420 636c 7573 7465 7269     Text clusteri
+00005900: 6e67 2c20 666f 7220 6578 616d 706c 6520  ng, for example 
+00005910: 5b65 7861 6d70 6c65 732f 636c 7573 7465  [examples/cluste
+00005920: 725f 6465 6d6f 2e70 795d 2868 7474 7073  r_demo.py](https
+00005930: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+00005940: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
+00005950: 6c61 7373 6966 6965 722f 626c 6f62 2f6d  lassifier/blob/m
+00005960: 6173 7465 722f 6578 616d 706c 6573 2f63  aster/examples/c
+00005970: 6c75 7374 6572 5f64 656d 6f2e 7079 290a  luster_demo.py).
+00005980: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005990: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+000059a0: 2020 2069 6d70 6f72 7420 7379 730a 2020     import sys.  
+000059b0: 2020 2020 2020 0a20 2020 2020 2020 2073        .        s
+000059c0: 7973 2e70 6174 682e 6170 7065 6e64 2827  ys.path.append('
+000059d0: 2e2e 2729 0a20 2020 2020 2020 2066 726f  ..').        fro
+000059e0: 6d20 7079 7465 7874 636c 6173 7369 6669  m pytextclassifi
+000059f0: 6572 2e74 6578 7463 6c75 7374 6572 2069  er.textcluster i
+00005a00: 6d70 6f72 7420 5465 7874 436c 7573 7465  mport TextCluste
+00005a10: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
+00005a20: 2020 2069 6620 5f5f 6e61 6d65 5f5f 203d     if __name__ =
+00005a30: 3d20 275f 5f6d 6169 6e5f 5f27 3a0a 2020  = '__main__':.  
+00005a40: 2020 2020 2020 2020 2020 6d20 3d20 5465            m = Te
+00005a50: 7874 436c 7573 7465 7228 6f75 7470 7574  xtCluster(output
+00005a60: 5f64 6972 3d27 6d6f 6465 6c73 2f63 6c75  _dir='models/clu
+00005a70: 7374 6572 2d74 6f79 272c 206e 5f63 6c75  ster-toy', n_clu
+00005a80: 7374 6572 733d 3229 0a20 2020 2020 2020  sters=2).       
+00005a90: 2020 2020 2070 7269 6e74 286d 290a 2020       print(m).  
+00005aa0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00005ab0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00005ac0: 2020 2027 5374 7564 656e 7420 6465 6274     'Student debt
+00005ad0: 2074 6f20 636f 7374 2042 7269 7461 696e   to cost Britain
+00005ae0: 2062 696c 6c69 6f6e 7320 7769 7468 696e   billions within
+00005af0: 2064 6563 6164 6573 272c 0a20 2020 2020   decades',.     
+00005b00: 2020 2020 2020 2020 2020 2027 4368 696e             'Chin
+00005b10: 6573 6520 6564 7563 6174 696f 6e20 666f  ese education fo
+00005b20: 7220 5456 2065 7870 6572 696d 656e 7427  r TV experiment'
+00005b30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005b40: 2020 2741 6262 6f74 7420 676f 7665 726e    'Abbott govern
+00005b50: 6d65 6e74 2073 7065 6e64 7320 2438 206d  ment spends $8 m
+00005b60: 696c 6c69 6f6e 206f 6e20 6869 6768 6572  illion on higher
+00005b70: 2065 6475 6361 7469 6f6e 272c 0a20 2020   education',.   
+00005b80: 2020 2020 2020 2020 2020 2020 2027 4d69               'Mi
+00005b90: 6464 6c65 2045 6173 7420 616e 6420 4173  ddle East and As
+00005ba0: 6961 2062 6f6f 7374 2069 6e76 6573 746d  ia boost investm
+00005bb0: 656e 7420 696e 2074 6f70 206c 6576 656c  ent in top level
+00005bc0: 2073 706f 7274 7327 2c0a 2020 2020 2020   sports',.      
+00005bd0: 2020 2020 2020 2020 2020 2753 756d 6d69            'Summi
+00005be0: 7420 5365 7269 6573 206c 6f6f 6b20 6c61  t Series look la
+00005bf0: 756e 6368 6573 2048 424f 2043 616e 6164  unches HBO Canad
+00005c00: 6120 7370 6f72 7473 2064 6f63 2073 6572  a sports doc ser
+00005c10: 6965 733a 204d 7564 6861 7227 0a20 2020  ies: Mudhar'.   
+00005c20: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00005c30: 2020 2020 2020 206d 2e74 7261 696e 2864         m.train(d
+00005c40: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
+00005c50: 206d 2e6c 6f61 645f 6d6f 6465 6c28 290a   m.load_model().
+00005c60: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
+00005c70: 6d2e 7072 6564 6963 7428 5b27 4162 626f  m.predict(['Abbo
+00005c80: 7474 2067 6f76 6572 6e6d 656e 7420 7370  tt government sp
+00005c90: 656e 6473 2024 3820 6d69 6c6c 696f 6e20  ends $8 million 
+00005ca0: 6f6e 2068 6967 6865 7220 6564 7563 6174  on higher educat
+00005cb0: 696f 6e20 6d65 6469 6120 626c 6974 7a27  ion media blitz'
+00005cc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005cd0: 2020 2020 2020 2020 2020 2020 2027 4d69               'Mi
+00005ce0: 6464 6c65 2045 6173 7420 616e 6420 4173  ddle East and As
+00005cf0: 6961 2062 6f6f 7374 2069 6e76 6573 746d  ia boost investm
+00005d00: 656e 7420 696e 2074 6f70 206c 6576 656c  ent in top level
+00005d10: 2073 706f 7274 7327 5d29 0a20 2020 2020   sports']).     
+00005d20: 2020 2020 2020 2070 7269 6e74 2872 290a         print(r).
+00005d30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005d40: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+00005d50: 206c 6f61 6420 6368 696e 6573 6520 7472   load chinese tr
+00005d60: 6169 6e20 6461 7461 2066 726f 6d20 3177  ain data from 1w
+00005d70: 2064 6174 6120 6669 6c65 0a20 2020 2020   data file.     
+00005d80: 2020 2020 2020 2066 726f 6d20 736b 6c65         from skle
+00005d90: 6172 6e2e 6665 6174 7572 655f 6578 7472  arn.feature_extr
+00005da0: 6163 7469 6f6e 2e74 6578 7420 696d 706f  action.text impo
+00005db0: 7274 2054 6669 6466 5665 6374 6f72 697a  rt TfidfVectoriz
+00005dc0: 6572 0a20 2020 2020 2020 200a 2020 2020  er.        .    
+00005dd0: 2020 2020 2020 2020 7463 6c75 7374 6572          tcluster
+00005de0: 203d 2054 6578 7443 6c75 7374 6572 286f   = TextCluster(o
+00005df0: 7574 7075 745f 6469 723d 276d 6f64 656c  utput_dir='model
+00005e00: 732f 636c 7573 7465 7227 2c20 6665 6174  s/cluster', feat
+00005e10: 7572 653d 5466 6964 6656 6563 746f 7269  ure=TfidfVectori
+00005e20: 7a65 7228 6e67 7261 6d5f 7261 6e67 653d  zer(ngram_range=
+00005e30: 2831 2c20 3229 292c 206e 5f63 6c75 7374  (1, 2)), n_clust
+00005e40: 6572 733d 3130 290a 2020 2020 2020 2020  ers=10).        
+00005e50: 2020 2020 6461 7461 203d 2074 636c 7573      data = tclus
+00005e60: 7465 722e 6c6f 6164 5f66 696c 655f 6461  ter.load_file_da
+00005e70: 7461 2827 7468 7563 6e65 7773 5f74 7261  ta('thucnews_tra
+00005e80: 696e 5f31 772e 7478 7427 2c20 7365 703d  in_1w.txt', sep=
+00005e90: 275c 7427 2c20 7573 655f 636f 6c3d 3129  '\t', use_col=1)
+00005ea0: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
+00005eb0: 7475 7265 2c20 6c61 6265 6c73 203d 2074  ture, labels = t
+00005ec0: 636c 7573 7465 722e 7472 6169 6e28 6461  cluster.train(da
+00005ed0: 7461 5b3a 3530 3030 5d29 0a20 2020 2020  ta[:5000]).     
+00005ee0: 2020 2020 2020 2074 636c 7573 7465 722e         tcluster.
+00005ef0: 7368 6f77 5f63 6c75 7374 6572 7328 6665  show_clusters(fe
+00005f00: 6174 7572 652c 206c 6162 656c 732c 2027  ature, labels, '
+00005f10: 6d6f 6465 6c73 2f63 6c75 7374 6572 2f63  models/cluster/c
+00005f20: 6c75 7374 6572 5f74 7261 696e 5f73 6567  luster_train_seg
+00005f30: 5f73 616d 706c 6573 2e70 6e67 2729 0a20  _samples.png'). 
+00005f40: 2020 2020 2020 2020 2020 2072 203d 2074             r = t
+00005f50: 636c 7573 7465 722e 7072 6564 6963 7428  cluster.predict(
+00005f60: 6461 7461 5b3a 3330 5d29 0a20 2020 2020  data[:30]).     
+00005f70: 2020 2020 2020 2070 7269 6e74 2872 290a         print(r).
+00005f80: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+00005f90: 2020 2020 0a20 2020 2020 2020 206f 7574      .        out
+00005fa0: 7075 743a 0a20 2020 2020 2020 200a 2020  put:.        .  
+00005fb0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00005fc0: 2020 5465 7874 436c 7573 7465 7220 696e    TextCluster in
+00005fd0: 7374 616e 6365 2028 4d69 6e69 4261 7463  stance (MiniBatc
+00005fe0: 684b 4d65 616e 7328 6e5f 636c 7573 7465  hKMeans(n_cluste
+00005ff0: 7273 3d32 2c20 6e5f 696e 6974 3d31 3029  rs=2, n_init=10)
+00006000: 2c20 3c70 7974 6578 7463 6c61 7373 6966  , <pytextclassif
+00006010: 6965 722e 7574 696c 732e 746f 6b65 6e69  ier.utils.tokeni
+00006020: 7a65 722e 546f 6b65 6e69 7a65 7220 6f62  zer.Tokenizer ob
+00006030: 6a65 6374 2061 7420 3078 3766 3830 6264  ject at 0x7f80bd
+00006040: 3436 3832 6230 3e2c 2054 6669 6466 5665  4682b0>, TfidfVe
+00006050: 6374 6f72 697a 6572 286e 6772 616d 5f72  ctorizer(ngram_r
+00006060: 616e 6765 3d28 312c 2032 2929 290a 2020  ange=(1, 2))).  
+00006070: 2020 2020 2020 5b31 2031 2031 2031 2031        [1 1 1 1 1
+00006080: 2031 2031 2031 2031 2031 2031 2038 2031   1 1 1 1 1 1 8 1
+00006090: 2031 2031 2031 2031 2031 2031 2031 2031   1 1 1 1 1 1 1 1
+000060a0: 2031 2039 2031 2031 2038 2031 2031 2039   1 9 1 1 8 1 1 9
+000060b0: 2031 5d0a 2020 2020 2020 2020 6060 600a   1].        ```.
+000060c0: 2020 2020 2020 2020 636c 7573 7465 7269          clusteri
+000060d0: 6e67 2070 6c6f 7420 696d 6167 653a 0a20  ng plot image:. 
+000060e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000060f0: 215b 636c 7573 7465 725f 696d 6167 655d  ![cluster_image]
+00006100: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006110: 636f 6d2f 7368 6962 696e 6736 3234 2f70  com/shibing624/p
+00006120: 7974 6578 7463 6c61 7373 6966 6965 722f  ytextclassifier/
+00006130: 626c 6f62 2f6d 6173 7465 722f 646f 6373  blob/master/docs
+00006140: 2f63 6c75 7374 6572 5f74 7261 696e 5f73  /cluster_train_s
+00006150: 6567 5f73 616d 706c 6573 2e70 6e67 290a  eg_samples.png).
+00006160: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006170: 200a 2020 2020 2020 2020 2323 2043 6f6e   .        ## Con
+00006180: 7461 6374 0a20 2020 2020 2020 200a 2020  tact.        .  
+00006190: 2020 2020 2020 2d20 4973 7375 6528 e5bb        - Issue(..
+000061a0: bae8 aeae 29ef bc9a 5b21 5b47 6974 4875  ....)...[![GitHu
+000061b0: 6220 6973 7375 6573 5d28 6874 7470 733a  b issues](https:
+000061c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000061d0: 2f67 6974 6875 622f 6973 7375 6573 2f73  /github/issues/s
+000061e0: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
+000061f0: 636c 6173 7369 6669 6572 2e73 7667 295d  classifier.svg)]
+00006200: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006210: 636f 6d2f 7368 6962 696e 6736 3234 2f70  com/shibing624/p
+00006220: 7974 6578 7463 6c61 7373 6966 6965 722f  ytextclassifier/
+00006230: 6973 7375 6573 290a 2020 2020 2020 2020  issues).        
+00006240: 2d20 e982 aee4 bbb6 e688 91ef bc9a 7875  - ............xu
+00006250: 6d69 6e67 3a20 7875 6d69 6e67 3632 3440  ming: xuming624@
+00006260: 7171 2e63 6f6d 0a20 2020 2020 2020 202d  qq.com.        -
+00006270: 20e5 beae e4bf a1e6 8891 efbc 9ae5 8aa0   ...............
+00006280: e688 912a e5be aee4 bfa1 e58f b7ef bc9a  ...*............
+00006290: 7875 6d69 6e67 3632 342a 2c20 e8bf 9b50  xuming624*, ...P
+000062a0: 7974 686f 6e2d 4e4c 50e4 baa4 e6b5 81e7  ython-NLP.......
+000062b0: bea4 efbc 8ce5 a487 e6b3 a8ef bc9a 2ae5  ..............*.
+000062c0: a793 e590 8d2d e585 ace5 8fb8 e590 8d2d  .....-.........-
+000062d0: 4e4c 502a 0a20 2020 2020 2020 203c 696d  NLP*.        <im
+000062e0: 6720 7372 633d 2264 6f63 732f 7765 6368  g src="docs/wech
+000062f0: 6174 2e6a 7065 6722 2077 6964 7468 3d22  at.jpeg" width="
+00006300: 3230 3022 202f 3e0a 2020 2020 2020 2020  200" />.        
+00006310: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006320: 2020 2323 2043 6974 6174 696f 6e0a 2020    ## Citation.  
+00006330: 2020 2020 2020 0a20 2020 2020 2020 20e5        .        .
+00006340: a682 e69e 9ce4 bda0 e59c a8e7 a094 e7a9  ................
+00006350: b6e4 b8ad e4bd bfe7 94a8 e4ba 8670 7974  .............pyt
+00006360: 6578 7463 6c61 7373 6966 6965 72ef bc8c  extclassifier...
+00006370: e8af b7e6 8c89 e5a6 82e4 b88b e6a0 bce5  ................
+00006380: bc8f e5bc 95e7 94a8 efbc 9a0a 2020 2020  ............    
+00006390: 2020 2020 0a20 2020 2020 2020 2041 5041      .        APA
+000063a0: 3a0a 2020 2020 2020 2020 6060 606c 6174  :.        ```lat
+000063b0: 6578 0a20 2020 2020 2020 2058 752c 204d  ex.        Xu, M
+000063c0: 2e20 5079 7465 7874 636c 6173 7369 6669  . Pytextclassifi
+000063d0: 6572 3a20 5465 7874 2063 6c61 7373 6966  er: Text classif
+000063e0: 6965 7220 746f 6f6c 6b69 7420 666f 7220  ier toolkit for 
+000063f0: 4e4c 5020 2856 6572 7369 6f6e 2031 2e32  NLP (Version 1.2
+00006400: 2e30 2920 5b43 6f6d 7075 7465 7220 736f  .0) [Computer so
+00006410: 6674 7761 7265 5d2e 2068 7474 7073 3a2f  ftware]. https:/
+00006420: 2f67 6974 6875 622e 636f 6d2f 7368 6962  /github.com/shib
+00006430: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
+00006440: 7373 6966 6965 720a 2020 2020 2020 2020  ssifier.        
+00006450: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
+00006460: 2020 2020 2042 6962 5465 583a 0a20 2020       BibTeX:.   
+00006470: 2020 2020 2060 6060 6c61 7465 780a 2020       ```latex.  
+00006480: 2020 2020 2020 406d 6973 637b 5079 7465        @misc{Pyte
+00006490: 7874 636c 6173 7369 6669 6572 2c0a 2020  xtclassifier,.  
+000064a0: 2020 2020 2020 2020 7469 746c 653d 7b50          title={P
+000064b0: 7974 6578 7463 6c61 7373 6966 6965 723a  ytextclassifier:
+000064c0: 2054 6578 7420 636c 6173 7369 6669 6572   Text classifier
+000064d0: 2074 6f6f 6c6b 6974 2066 6f72 204e 4c50   toolkit for NLP
+000064e0: 7d2c 0a20 2020 2020 2020 2020 2061 7574  },.          aut
+000064f0: 686f 723d 7b58 7520 4d69 6e67 7d2c 0a20  hor={Xu Ming},. 
+00006500: 2020 2020 2020 2020 2079 6561 723d 7b32           year={2
+00006510: 3032 327d 2c0a 2020 2020 2020 2020 2020  022},.          
+00006520: 686f 7770 7562 6c69 7368 6564 3d7b 5c75  howpublished={\u
+00006530: 726c 7b68 7474 7073 3a2f 2f67 6974 6875  rl{https://githu
+00006540: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
+00006550: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+00006560: 727d 7d2c 0a20 2020 2020 2020 207d 0a20  r}},.        }. 
+00006570: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00006580: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+00006590: 2020 2020 2023 2320 4c69 6365 6e73 650a       ## License.
+000065a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000065b0: 200a 2020 2020 2020 2020 e68e 88e6 9d83   .        ......
+000065c0: e58d 8fe8 aeae e4b8 ba20 5b54 6865 2041  ......... [The A
+000065d0: 7061 6368 6520 4c69 6365 6e73 6520 322e  pache License 2.
+000065e0: 305d 284c 4943 454e 5345 29ef bc8c e58f  0](LICENSE).....
+000065f0: afe5 858d e8b4 b9e7 94a8 e581 9ae5 9586  ................
+00006600: e4b8 9ae7 94a8 e980 94e3 8082 e8af b7e5  ................
+00006610: 9ca8 e4ba a7e5 9381 e8af b4e6 988e e4b8  ................
+00006620: ade9 9984 e58a a02a 2a70 7974 6578 7463  .......**pytextc
+00006630: 6c61 7373 6966 6965 722a 2ae7 9a84 e993  lassifier**.....
+00006640: bee6 8ea5 e592 8ce6 8e88 e69d 83e5 8d8f  ................
+00006650: e8ae aee3 8082 0a20 2020 2020 2020 200a  .......        .
+00006660: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006670: 2023 2320 436f 6e74 7269 6275 7465 0a20   ## Contribute. 
+00006680: 2020 2020 2020 20e9 a1b9 e79b aee4 bba3         .........
+00006690: e7a0 81e8 bf98 e5be 88e7 b297 e7b3 99ef  ................
+000066a0: bc8c e5a6 82e6 9e9c e5a4 a7e5 aeb6 e5af  ................
+000066b0: b9e4 bba3 e7a0 81e6 9c89 e689 80e6 94b9  ................
+000066c0: e8bf 9bef bc8c e6ac a2e8 bf8e e68f 90e4  ................
+000066d0: baa4 e59b 9ee6 9cac e9a1 b9e7 9bae efbc  ................
+000066e0: 8ce5 9ca8 e68f 90e4 baa4 e4b9 8be5 898d  ................
+000066f0: efbc 8ce6 b3a8 e684 8fe4 bba5 e4b8 8be4  ................
+00006700: b8a4 e782 b9ef bc9a 0a20 2020 2020 2020  .........       
+00006710: 200a 2020 2020 2020 2020 202d 20e5 9ca8   .         - ...
+00006720: 6074 6573 7473 60e6 b7bb e58a a0e7 9bb8  `tests`.........
+00006730: e5ba 94e7 9a84 e58d 95e5 8583 e6b5 8be8  ................
+00006740: af95 0a20 2020 2020 2020 2020 2d20 e4bd  ...         - ..
+00006750: bfe7 94a8 6070 7974 686f 6e20 7365 7475  ....`python setu
+00006760: 702e 7079 2074 6573 7460 e69d a5e8 bf90  p.py test`......
+00006770: e8a1 8ce6 8980 e69c 89e5 8d95 e585 83e6  ................
+00006780: b58b e8af 95ef bc8c e7a1 aee4 bf9d e689  ................
+00006790: 80e6 9c89 e58d 95e6 b58b e983 bde6 98af  ................
+000067a0: e980 9ae8 bf87 e79a 840a 2020 2020 2020  ..........      
+000067b0: 2020 0a20 2020 2020 2020 20e4 b98b e590    .        .....
+000067c0: 8ee5 8db3 e58f afe6 8f90 e4ba a450 52e3  .............PR.
+000067d0: 8082 0a20 2020 2020 2020 200a 2020 2020  ...        .    
+000067e0: 2020 2020 0a4b 6579 776f 7264 733a 2070      .Keywords: p
+000067f0: 7974 6578 7463 6c61 7373 6966 6965 722c  ytextclassifier,
+00006800: 7465 7874 636c 6173 7369 6669 6572 2c63  textclassifier,c
+00006810: 6c61 7373 6966 6965 722c 7465 7874 636c  lassifier,textcl
+00006820: 6173 7369 6669 6361 7469 6f6e 0a50 6c61  assification.Pla
+00006830: 7466 6f72 6d3a 2055 4e4b 4e4f 574e 0a43  tform: UNKNOWN.C
+00006840: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00006850: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00006860: 5363 6965 6e63 652f 5265 7365 6172 6368  Science/Research
+00006870: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00006880: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00006890: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+000068a0: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
+000068b0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000068c0: 7665 6420 3a3a 2041 7061 6368 6520 536f  ved :: Apache So
+000068d0: 6674 7761 7265 204c 6963 656e 7365 0a43  ftware License.C
+000068e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000068f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00006900: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
+00006910: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00006920: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00006930: 7468 6f6e 203a 3a20 322e 370a 436c 6173  thon :: 2.7.Clas
+00006940: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00006950: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00006960: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
+00006970: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00006980: 2054 6578 7420 5072 6f63 6573 7369 6e67   Text Processing
+00006990: 203a 3a20 4c69 6e67 7569 7374 6963 0a43   :: Linguistic.C
+000069a0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+000069b0: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
+000069c0: 6e67 696e 6565 7269 6e67 203a 3a20 4172  ngineering :: Ar
+000069d0: 7469 6669 6369 616c 2049 6e74 656c 6c69  tificial Intelli
+000069e0: 6765 6e63 650a 4465 7363 7269 7074 696f  gence.Descriptio
+000069f0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00006a00: 7465 7874 2f6d 6172 6b64 6f77 6e0a       text/markdown.
```

### Comparing `pytextclassifier-1.3.5/README.md` & `pytextclassifier-1.3.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,46 @@
+<div align="center">
+  <a href="https://github.com/shibing624/pytextclassifier">
+    <img src="https://github.com/shibing624/pytextclassifier/blob/master/docs/logo.png" alt="Logo" height="156">
+  </a>
+</div>
+
+-----------------
+
+# PyTextClassifier: Python Text Classifier
 [![PyPI version](https://badge.fury.io/py/pytextclassifier.svg)](https://badge.fury.io/py/pytextclassifier)
 [![Downloads](https://pepy.tech/badge/pytextclassifier)](https://pepy.tech/project/pytextclassifier)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
 [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/pytextclassifier.svg)](https://github.com/shibing624/pytextclassifier/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
 [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/pytextclassifier.svg)](https://github.com/shibing624/pytextclassifier/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
-# PyTextClassifier
-PyTextClassifier, Python Text Classifier. It can be applied to the fields of sentiment polarity analysis, text risk classification and so on,
+
+## Introduction
+PyTextClassifier: Python Text Classifier. It can be applied to the fields of sentiment polarity analysis, text risk classification and so on,
 and it supports multiple classification algorithms and clustering algorithms.
 
-文本分类器，提供多种文本分类和聚类算法，支持句子和文档级的文本分类任务，支持二分类、多分类、多标签分类、多层级分类和Kmeans聚类，开箱即用。python3开发。
+**pytextclassifier** is a python Open Source Toolkit for text classification. The goal is to implement
+text analysis algorithm, so to achieve the use in the production environment.
 
+文本分类器，提供多种文本分类和聚类算法，支持句子和文档级的文本分类任务，支持二分类、多分类、多标签分类、多层级分类和Kmeans聚类，开箱即用。python3开发。
 
 **Guide**
 
 - [Feature](#Feature)
 - [Install](#install)
 - [Usage](#usage)
 - [Dataset](#Dataset)
 - [Contact](#Contact)
 - [Citation](#Citation)
 - [Reference](#reference)
 
-# Feature
-
-**pytextclassifier** is a python Open Source Toolkit for text classification. The goal is to implement
-text analysis algorithm, so as to achieve the use in the production environment.
+## Feature
 
 **pytextclassifier** has the characteristics
 of clear algorithm, high performance and customizable corpus.
 
 Functions：
 ### Classifier
   - [x] LogisticRegression
@@ -47,15 +56,15 @@
   - [x] BERT
 
 ### Cluster
   - [x] MiniBatchKmeans
 
 While providing rich functions, **pytextclassifier** internal modules adhere to low coupling, model adherence to inert loading, dictionary publication, and easy to use.
 
-# Install
+## Install
 
 - Requirements and Installation
 
 ```
 pip3 install torch # conda install pytorch
 pip3 install pytextclassifier
 ```
@@ -65,30 +74,29 @@
 ```
 git clone https://github.com/shibing624/pytextclassifier.git
 cd pytextclassifier
 python3 setup.py install
 ```
 
 
-# Usage
-# Text Classifier
+## Usage
+### Text Classifier
 
-## English Text Classifier
-
-Including model training, saving, predict, evaluate, for example [examples/lr_en_classification_demo.py](examples/lr_en_classification_demo.py):
+### English Text Classifier
 
+Including model training, saving, predict, evaluate, for example [examples/lr_en_classification_demo.py](https://github.com/shibing624/pytextclassifier/blob/master/examples/lr_en_classification_demo.py):
 
 ```python
 import sys
 
 sys.path.append('..')
 from pytextclassifier import ClassicClassifier
 
 if __name__ == '__main__':
-    m = ClassicClassifier(model_dir='models/lr', model_name_or_model='lr')
+    m = ClassicClassifier(output_dir='models/lr', model_name_or_model='lr')
     # ClassicClassifier support model_name：lr, random_forest, decision_tree, knn, bayes, svm, xgboost
     print(m)
     data = [
         ('education', 'Student debt to cost Britain billions within decades'),
         ('education', 'Chinese education for TV experiment'),
         ('sports', 'Middle East and Asia boost investment in top level sports'),
         ('sports', 'Summit Series look launches HBO Canada sports doc series: Mudhar')
@@ -113,28 +121,28 @@
 
 ```
 ClassicClassifier instance (LogisticRegression(fit_intercept=False), stopwords size: 2438)
 predict_label: ['education'], predict_proba: [0.5378236358492112]
 acc_score: 1.0
 ```
 
-## Chinese Text Classifier(中文文本分类)
+### Chinese Text Classifier(中文文本分类)
 
 Text classification compatible with Chinese and English corpora.
 
-example [examples/lr_classification_demo.py](examples/lr_classification_demo.py)
+example [examples/lr_classification_demo.py](https://github.com/shibing624/pytextclassifier/blob/master/examples/lr_classification_demo.py)
 
 ```python
 import sys
 
 sys.path.append('..')
 from pytextclassifier import ClassicClassifier
 
 if __name__ == '__main__':
-    m = ClassicClassifier(model_dir='models/lr-toy', model_name_or_model='lr')
+    m = ClassicClassifier(output_dir='models/lr-toy', model_name_or_model='lr')
     # 经典分类方法，支持的模型包括：lr, random_forest, decision_tree, knn, bayes, svm, xgboost
     data = [
         ('education', '名师指导托福语法技巧：名词的复数形式'),
         ('education', '中国高考成绩海外认可 是“狼来了”吗？'),
         ('education', '公务员考虑越来越吃香，这是怎么回事？'),
         ('sports', '图文：法网孟菲尔斯苦战进16强 孟菲尔斯怒吼'),
         ('sports', '四川丹棱举行全国长距登山挑战赛 近万人参与'),
@@ -153,15 +161,15 @@
         ('sports', '意甲首轮补赛交战记录:米兰客场8战不败国米10年连胜'),
     ]
     acc_score = m.evaluate_model(test_data)
     print(f'acc_score: {acc_score}')  # 1.0
 
     #### train model with 1w data
     print('-' * 42)
-    m = ClassicClassifier(model_dir='models/lr', model_name_or_model='lr')
+    m = ClassicClassifier(output_dir='models/lr', model_name_or_model='lr')
     data_file = 'thucnews_train_1w.txt'
     m.train(data_file)
     m.load_model()
     predict_label, predict_proba = m.predict(
         ['顺义北京苏活88平米起精装房在售',
          '美EB-5项目“15日快速移民”将推迟'])
     print(f'predict_label: {predict_label}, predict_proba: {predict_proba}')
@@ -173,67 +181,69 @@
 ClassicClassifier instance (LogisticRegression(fit_intercept=False), stopwords size: 2438)
 predict_label: ['education' 'sports'], predict_proba: [0.5, 0.598941806741534]
 acc_score: 1.0
 ------------------------------------------
 predict_label: ['realty' 'education'], predict_proba: [0.7302956923617372, 0.2565005445322923]
 ```
 
-## Visual Feature Importance
+### Visual Feature Importance
+
+Show feature weights of model, and prediction word weight, for example [examples/visual_feature_importance.ipynb](https://github.com/shibing624/pytextclassifier/blob/master/examples/visual_feature_importance.ipynb)
 
-Show feature weights of model, and prediction word weight, for example [examples/visual_feature_importance.ipynb](examples/visual_feature_importance.ipynb)
 ```python
 import sys
 
 sys.path.append('..')
 from pytextclassifier import ClassicClassifier
 import jieba
 
-tc = ClassicClassifier(model_dir='models/lr-toy', model_name_or_model='lr')
+tc = ClassicClassifier(output_dir='models/lr-toy', model_name_or_model='lr')
 data = [
     ('education', '名师指导托福语法技巧：名词的复数形式'),
     ('education', '中国高考成绩海外认可 是“狼来了”吗？'),
     ('sports', '图文：法网孟菲尔斯苦战进16强 孟菲尔斯怒吼'),
     ('sports', '四川丹棱举行全国长距登山挑战赛 近万人参与'),
     ('sports', '米兰客场8战不败国米10年连胜')
 ]
 tc.train(data)
 import eli5
+
 infer_data = ['高考指导托福语法技巧国际认可',
               '意甲首轮补赛交战记录:米兰客场8战不败国米10年连胜']
 eli5.show_weights(tc.model, vec=tc.feature)
 seg_infer_data = [' '.join(jieba.lcut(i)) for i in infer_data]
 eli5.show_prediction(tc.model, seg_infer_data[0], vec=tc.feature,
                      target_names=['education', 'sports'])
 ```
 
 output:
 
 ![img.png](docs/img.png)
 
-## Deep Classification model
+### Deep Classification model
 
 本项目支持以下深度分类模型：FastText、TextCNN、TextRNN、Bert模型，`import`模型对应的方法来调用：
 ```python
 from pytextclassifier import FastTextClassifier, TextCNNClassifier, TextRNNClassifier, BertClassifier
 ```
 
 下面以FastText模型为示例，其他模型的使用方法类似。
 
 ### FastText 模型
 
-训练和预测`FastText`模型示例[examples/fasttext_classification_demo.py](examples/fasttext_classification_demo.py)
+训练和预测`FastText`模型示例[examples/fasttext_classification_demo.py](https://github.com/shibing624/pytextclassifier/blob/master/examples/fasttext_classification_demo.py)
 
 ```python
 import sys
 
 sys.path.append('..')
 from pytextclassifier import FastTextClassifier, load_data
 
 if __name__ == '__main__':
-    m = FastTextClassifier(model_dir='models/fasttext-toy')
+    m = FastTextClassifier(output_dir='models/fasttext-toy')
     data = [
         ('education', '名师指导托福语法技巧：名词的复数形式'),
         ('education', '中国高考成绩海外认可 是“狼来了”吗？'),
         ('education', '公务员考虑越来越吃香，这是怎么回事？'),
         ('sports', '图文：法网孟菲尔斯苦战进16强 孟菲尔斯怒吼'),
         ('sports', '四川丹棱举行全国长距登山挑战赛 近万人参与'),
         ('sports', '米兰客场8战不败保持连胜'),
@@ -251,15 +261,15 @@
     ]
     acc_score = m.evaluate_model(test_data)
     print(f'acc_score: {acc_score}')  # 1.0
 
     #### train model with 1w data
     print('-' * 42)
     data_file = 'thucnews_train_1w.txt'
-    m = FastTextClassifier(model_dir='models/fasttext')
+    m = FastTextClassifier(output_dir='models/fasttext')
     m.train(data_file, names=('labels', 'text'), num_epochs=3)
     # load best trained model from model_dir
     m.load_model()
     predict_label, predict_proba = m.predict(
         ['顺义北京苏活88平米起精装房在售',
          '美EB-5项目“15日快速移民”将推迟']
     )
@@ -269,24 +279,24 @@
     acc_score = m.evaluate_model(test_data)
     print(f'acc_score: {acc_score}')
 ```
 
 ### BERT 类模型
 
 #### 多分类模型
-训练和预测`BERT`多分类模型，示例[examples/bert_classification_zh_demo.py](examples/bert_classification_zh_demo.py)
+训练和预测`BERT`多分类模型，示例[examples/bert_classification_zh_demo.py](https://github.com/shibing624/pytextclassifier/blob/master/examples/bert_classification_zh_demo.py)
 
 ```python
 import sys
 
 sys.path.append('..')
 from pytextclassifier import BertClassifier
 
 if __name__ == '__main__':
-    m = BertClassifier(model_dir='models/bert-chinese-toy', num_classes=2,
+    m = BertClassifier(output_dir='models/bert-chinese-toy', num_classes=2,
                        model_type='bert', model_name='bert-base-chinese', num_epochs=2)
     # model_type: support 'bert', 'albert', 'roberta', 'xlnet'
     # model_name: support 'bert-base-chinese', 'bert-base-cased', 'bert-base-multilingual-cased' ...
     data = [
         ('education', '名师指导托福语法技巧：名词的复数形式'),
         ('education', '中国高考成绩海外认可 是“狼来了”吗？'),
         ('education', '公务员考虑越来越吃香，这是怎么回事？'),
@@ -304,18 +314,18 @@
 
     test_data = [
         ('education', '福建春季公务员考试报名18日截止 2月6日考试'),
         ('sports', '意甲首轮补赛交战记录:米兰客场8战不败国米10年连胜'),
     ]
     acc_score = m.evaluate_model(test_data)
     print(f'acc_score: {acc_score}')
-    
+
     # train model with 1w data file and 10 classes
     print('-' * 42)
-    m = BertClassifier(model_dir='models/bert-chinese', num_classes=10,
+    m = BertClassifier(output_dir='models/bert-chinese', num_classes=10,
                        model_type='bert', model_name='bert-base-chinese', num_epochs=2,
                        args={"no_cache": True, "lazy_loading": True, "lazy_text_column": 1, "lazy_labels_column": 0, })
     data_file = 'thucnews_train_1w.txt'
     # 如果训练数据超过百万条，建议使用lazy_loading模式，减少内存占用
     m.train(data_file, test_size=0, names=('labels', 'text'))
     m.load_model()
     predict_label, predict_proba = m.predict(
@@ -330,15 +340,14 @@
 分类可以分为多分类和多标签分类。多分类的标签是排他的，而多标签分类的所有标签是不排他的。
 
 多标签分类比较直观的理解是，一个样本可以同时拥有几个类别标签，
 比如一首歌的标签可以是流行、轻快，一部电影的标签可以是动作、喜剧、搞笑等，这都是多标签分类的情况。
 
 训练和预测`BERT`多标签分类模型，示例[examples/bert_multilabel_classification_zh_demo.py.py](https://github.com/shibing624/pytextclassifier/blob/master/examples/bert_multilabel_classification_zh_demo.py)
 
-
 ```python
 import sys
 import pandas as pd
 
 sys.path.append('..')
 from pytextclassifier import BertClassifier
 
@@ -365,15 +374,15 @@
             data.append([terms[0], val])
     return data
 
 
 if __name__ == '__main__':
     # model_type: support 'bert', 'albert', 'roberta', 'xlnet'
     # model_name: support 'bert-base-chinese', 'bert-base-cased', 'bert-base-multilingual-cased' ...
-    m = BertClassifier(model_dir='models/multilabel-bert-zh-model', num_classes=15,
+    m = BertClassifier(output_dir='models/multilabel-bert-zh-model', num_classes=15,
                        model_type='bert', model_name='bert-base-chinese', num_epochs=2, multi_label=True)
     # Train and Evaluation data needs to be in a Pandas Dataframe containing at least two columns, a 'text' and a 'labels' column. The `labels` column should contain multi-hot encoded lists.
     train_data = [
         ["一个小时房间仍然没暖和", [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0]],
         ["耗电情况：这个没有注意", [0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]],
     ]
     data = load_jd_data('multilabel_jd_comments.csv')
@@ -394,15 +403,15 @@
     print(f'predict_label: {predict_label}, predict_proba: {predict_proba}')
 ```
 
 ## Evaluation
 
 ### Dataset
 
-1. THUCNews中文文本数据集（1.56GB）：官方[下载地址](http://thuctc.thunlp.org/)，抽样了10万条THUCNews中文文本10分类数据集（6MB），地址：[examples/thucnews_train_10w.txt](examples/thucnews_train_10w.txt)。
+1. THUCNews中文文本数据集（1.56GB）：官方[下载地址](http://thuctc.thunlp.org/)，抽样了10万条THUCNews中文文本10分类数据集（6MB），地址：[examples/thucnews_train_10w.txt](https://github.com/shibing624/pytextclassifier/blob/master/examples/thucnews_train_10w.txt)。
 2. TNEWS今日头条中文新闻（短文本）分类 Short Text Classificaiton for News，该数据集(5.1MB)来自今日头条的新闻版块，共提取了15个类别的新闻，包括旅游，教育，金融，军事等，地址：[tnews_public.zip](https://storage.googleapis.com/cluebenchmark/tasks/tnews_public.zip)
 
 ### Evaluation Result
 在THUCNews中文文本10分类数据集（6MB）上评估，模型在测试集(test)评测效果如下：
 
 模型|acc|说明
 --|--|--
@@ -422,45 +431,46 @@
 BERT-base|**0.5660**|本项目实现
 BERT-base|0.5609|CLUE Benchmark Leaderboard结果 [CLUEbenchmark](https://github.com/CLUEbenchmark/CLUE)
 
 - 以上结果均为分类的准确率（accuracy）结果
 - THUCNews数据集评测结果可以基于`examples/thucnews_train_10w.txt`数据用`examples`下的各模型demo复现
 - TNEWS数据集评测结果可以下载TNEWS数据集，运行`examples/bert_classification_tnews_demo.py`复现
 
-### 模型调研
+### 命令行调用
 
-提供分类模型快速调研工具，文件树：
+提供分类模型命令行调用脚本，文件树：
 ```bash
 pytextclassifier
 ├── bert_classifier.py
 ├── fasttext_classifier.py
 ├── classic_classifier.py
 ├── textcnn_classifier.py
 └── textrnn_classifier.py
 ```
 
-每个文件对应一个模型，各模型完全独立，可以直接运行，也方便修改，支持通过`argparse` 修改`--data_path`等参数。
+每个文件对应一个模型方法，各模型完全独立，可以直接运行，也方便修改，支持通过`argparse` 修改`--data_path`等参数。
 
 直接在终端调用fasttext模型训练：
 ```bash
 python -m pytextclassifier.fasttext_classifier -h
 ```
 
 ## Text Cluster
 
 
-Text clustering, for example [examples/cluster_demo.py](examples/cluster_demo.py)
+Text clustering, for example [examples/cluster_demo.py](https://github.com/shibing624/pytextclassifier/blob/master/examples/cluster_demo.py)
+
 ```python
 import sys
 
 sys.path.append('..')
 from pytextclassifier.textcluster import TextCluster
 
 if __name__ == '__main__':
-    m = TextCluster(model_dir='models/cluster-toy', n_clusters=2)
+    m = TextCluster(output_dir='models/cluster-toy', n_clusters=2)
     print(m)
     data = [
         'Student debt to cost Britain billions within decades',
         'Chinese education for TV experiment',
         'Abbott government spends $8 million on higher education',
         'Middle East and Asia boost investment in top level sports',
         'Summit Series look launches HBO Canada sports doc series: Mudhar'
@@ -470,15 +480,15 @@
     r = m.predict(['Abbott government spends $8 million on higher education media blitz',
                    'Middle East and Asia boost investment in top level sports'])
     print(r)
 
     ########### load chinese train data from 1w data file
     from sklearn.feature_extraction.text import TfidfVectorizer
 
-    tcluster = TextCluster(model_dir='models/cluster', feature=TfidfVectorizer(ngram_range=(1, 2)), n_clusters=10)
+    tcluster = TextCluster(output_dir='models/cluster', feature=TfidfVectorizer(ngram_range=(1, 2)), n_clusters=10)
     data = tcluster.load_file_data('thucnews_train_1w.txt', sep='\t', use_col=1)
     feature, labels = tcluster.train(data[:5000])
     tcluster.show_clusters(feature, labels, 'models/cluster/cluster_train_seg_samples.png')
     r = tcluster.predict(data[:30])
     print(r)
 ```
 
@@ -486,26 +496,26 @@
 
 ```
 TextCluster instance (MiniBatchKMeans(n_clusters=2, n_init=10), <pytextclassifier.utils.tokenizer.Tokenizer object at 0x7f80bd4682b0>, TfidfVectorizer(ngram_range=(1, 2)))
 [1 1 1 1 1 1 1 1 1 1 1 8 1 1 1 1 1 1 1 1 1 1 9 1 1 8 1 1 9 1]
 ```
 clustering plot image:
 
-![cluster_image](docs/cluster_train_seg_samples.png)
+![cluster_image](https://github.com/shibing624/pytextclassifier/blob/master/docs/cluster_train_seg_samples.png)
 
 
-# Contact
+## Contact
 
 - Issue(建议)：[![GitHub issues](https://img.shields.io/github/issues/shibing624/pytextclassifier.svg)](https://github.com/shibing624/pytextclassifier/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我：加我*微信号：xuming624*, 进Python-NLP交流群，备注：*姓名-公司名-NLP*
 <img src="docs/wechat.jpeg" width="200" />
 
 
-# Citation
+## Citation
 
 如果你在研究中使用了pytextclassifier，请按如下格式引用：
 
 APA:
 ```latex
 Xu, M. Pytextclassifier: Text classifier toolkit for NLP (Version 1.2.0) [Computer software]. https://github.com/shibing624/pytextclassifier
 ```
@@ -517,25 +527,21 @@
   author={Xu Ming},
   year={2022},
   howpublished={\url{https://github.com/shibing624/pytextclassifier}},
 }
 ```
 
 
-# License
+## License
 
 
 授权协议为 [The Apache License 2.0](LICENSE)，可免费用做商业用途。请在产品说明中附加**pytextclassifier**的链接和授权协议。
 
 
-# Contribute
+## Contribute
 项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
 
  - 在`tests`添加相应的单元测试
  - 使用`python setup.py test`来运行所有单元测试，确保所有单测都是通过的
 
 之后即可提交PR。
 
-
-# Reference
-
-- SentimentPolarityAnalysis
```

### Comparing `pytextclassifier-1.3.5/examples/thucnews_train_1w.txt` & `pytextclassifier-1.3.6/examples/thucnews_train_1w.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/pytextclassifier/__init__.py` & `pytextclassifier-1.3.6/pytextclassifier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
-__version__ = '1.3.5'
+__version__ = '1.3.6'
 
 from pytextclassifier.classic_classifier import ClassicClassifier
 from pytextclassifier.fasttext_classifier import FastTextClassifier
 from pytextclassifier.textcnn_classifier import TextCNNClassifier
 from pytextclassifier.textrnn_classifier import TextRNNClassifier
 from pytextclassifier.bert_classifier import BertClassifier
 from pytextclassifier.base_classifier import load_data
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/base_classifier.py` & `pytextclassifier-1.3.6/pytextclassifier/base_classifier.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/pytextclassifier/bert_classfication_utils.py` & `pytextclassifier-1.3.6/pytextclassifier/bert_classfication_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
     # sequence or the second sequence. The embedding vectors for `type=0` and
     # `type=1` were learned during pre-training and are added to the wordpiece
     # embedding vector (and position vector). This is not *strictly* necessary
     # since the [SEP] token unambiguously separates the sequences, but it makes
     # it easier for the model to learn the concept of sequences.
     #
     # For classification tasks, the first vector (corresponding to [CLS]) is
-    # used as as the "sentence vector". Note that this only makes sense because
+    # used as the "sentence vector". Note that this only makes sense because
     # the entire model is fine-tuned.
     tokens = tokens_a + [sep_token]
     segment_ids = [sequence_a_segment_id] * len(tokens)
 
     if tokens_b:
         if sep_token_extra:
             tokens += [sep_token]
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/bert_classification_model.py` & `pytextclassifier-1.3.6/pytextclassifier/bert_classification_model.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/pytextclassifier/bert_classifier.py` & `pytextclassifier-1.3.6/pytextclassifier/bert_classifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,44 +23,45 @@
 use_cuda = torch.cuda.is_available()
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 
 class BertClassifier(ClassifierABC):
     def __init__(
             self,
-            model_dir,
             num_classes,
+            output_dir="outputs",
             model_type='bert',
             model_name='bert-base-chinese',
             num_epochs=3,
             batch_size=64,
             max_seq_length=128,
             multi_label=False,
             labels_sep=',',
             args=None,
     ):
+
         """
         Init classification model
-        @param model_dir: str, model dir
+        @param output_dir: output model dir
         @param model_type: support 'bert', 'albert', 'roberta', 'xlnet'
         @param model_name:
         @param num_classes:
         @param num_epochs:
         @param batch_size:
         @param max_seq_length:
         @param multi_label:
         @param labels_sep:
         @param args:
         """
         default_args = {
-            "output_dir": model_dir,
+            "output_dir": output_dir,
             "max_seq_length": max_seq_length,
             "num_train_epochs": num_epochs,
             "train_batch_size": batch_size,
-            "best_model_dir": os.path.join(model_dir, 'best_model'),
+            "best_model_dir": os.path.join(output_dir, 'best_model'),
             "labels_sep": labels_sep,
         }
         train_args = BertClassificationArgs()
         if args and isinstance(args, dict):
             train_args.update_from_dict(args)
         train_args.update_from_dict(default_args)
 
@@ -68,25 +69,25 @@
             model_type=model_type,
             model_name=model_name,
             num_labels=num_classes,
             multi_label=multi_label,
             args=train_args,
             use_cuda=use_cuda,
         )
-        self.model_dir = model_dir
+        self.output_dir = output_dir
         self.model_type = model_type
         self.num_classes = num_classes
         self.batch_size = batch_size
         self.max_seq_length = max_seq_length
         self.num_epochs = num_epochs
         self.train_args = train_args
         self.use_cuda = use_cuda
         self.multi_label = multi_label
         self.labels_sep = labels_sep
-        self.label_vocab_path = os.path.join(self.model_dir, 'label_vocab.json')
+        self.label_vocab_path = os.path.join(self.output_dir, 'label_vocab.json')
         self.is_trained = False
 
     def __str__(self):
         return f'BertClassifier instance ({self.model})'
 
     def train(
             self,
@@ -94,31 +95,31 @@
             dev_data_list_or_path=None,
             header=None,
             names=('labels', 'text'),
             delimiter='\t',
             test_size=0.1,
     ):
         """
-        Train model with data_list_or_path and save model to model_dir
+        Train model with data_list_or_path and save model to output_dir
         @param data_list_or_path:
         @param dev_data_list_or_path:
         @param header:
         @param names:
         @param delimiter:
         @param test_size:
         @return:
         """
         logger.debug('train model ...')
         SEED = 1
         set_seed(SEED)
         # load data
         X, y, data_df = load_data(data_list_or_path, header=header, names=names, delimiter=delimiter,
                                   labels_sep=self.labels_sep, is_train=True)
-        if self.model_dir:
-            os.makedirs(self.model_dir, exist_ok=True)
+        if self.output_dir:
+            os.makedirs(self.output_dir, exist_ok=True)
         labels_map = self.build_labels_map(y, self.label_vocab_path, self.multi_label, self.labels_sep)
         labels_list = sorted(list(labels_map.keys()))
         if dev_data_list_or_path is not None:
             dev_X, dev_y, dev_df = load_data(dev_data_list_or_path, header=header, names=names,
                                              delimiter=delimiter, labels_sep=self.labels_sep,
                                              is_train=False)
             train_data = data_df
@@ -167,43 +168,52 @@
             # predict probability
             predict_probs = [1 - np.exp(-np.max(raw_output)) for raw_output, prediction in
                              zip(raw_outputs, predictions)]
             return predictions, predict_probs
 
     def evaluate_model(self, data_list_or_path, header=None,
                        names=('labels', 'text'), delimiter='\t', **kwargs):
+        """
+        Evaluate model with data_list_or_path
+        @param data_list_or_path:
+        @param header:
+        @param names:
+        @param delimiter:
+        @param kwargs:
+        @return:
+        """
         if self.train_args.lazy_loading:
             eval_df = data_list_or_path
         else:
             X_test, y_test, eval_df = load_data(data_list_or_path, header=header, names=names, delimiter=delimiter,
-                                            labels_sep=self.labels_sep)
+                                                labels_sep=self.labels_sep)
         if not self.is_trained:
             self.load_model()
         result, model_outputs, wrong_predictions = self.model.eval_model(
             eval_df,
-            output_dir=self.model_dir,
+            output_dir=self.output_dir,
             **kwargs,
         )
         return result
 
     def load_model(self):
         """
-        Load model from model_dir
+        Load model from output_dir
         @return:
         """
-        model_path = os.path.join(self.model_dir, 'pytorch_model.bin')
+        model_path = os.path.join(self.output_dir, 'pytorch_model.bin')
         if os.path.exists(model_path):
             labels_map = json.load(open(self.label_vocab_path, 'r', encoding='utf-8'))
             labels_list = sorted(list(labels_map.keys()))
             num_classes = len(labels_map)
             assert num_classes == self.num_classes, f'num_classes not match, {num_classes} != {self.num_classes}'
             self.train_args.update_from_dict({'labels_map': labels_map, 'labels_list': labels_list})
             self.model = BertClassificationModel(
                 model_type=self.model_type,
-                model_name=self.model_dir,
+                model_name=self.output_dir,
                 num_labels=self.num_classes,
                 multi_label=self.multi_label,
                 args=self.train_args,
                 use_cuda=self.use_cuda,
             )
             self.is_trained = True
         else:
@@ -242,37 +252,37 @@
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Bert Text Classification')
     parser.add_argument('--pretrain_model_type', default='bert', type=str,
                         help='pretrained huggingface model type')
     parser.add_argument('--pretrain_model_name', default='bert-base-chinese', type=str,
                         help='pretrained huggingface model name')
-    parser.add_argument('--model_dir', default='models/bert', type=str, help='save model dir')
+    parser.add_argument('--output_dir', default='models/bert', type=str, help='save model dir')
     parser.add_argument('--data_path', default=os.path.join(pwd_path, '../examples/thucnews_train_1w.txt'),
                         type=str, help='sample data file path')
-    parser.add_argument('--num_classes', default=10, type=int, help='number of classes')
+    parser.add_argument('--num_classes', default=10, type=int, help='number of label classes')
     parser.add_argument('--num_epochs', default=3, type=int, help='train epochs')
     parser.add_argument('--batch_size', default=64, type=int, help='train batch size')
     parser.add_argument('--max_seq_length', default=128, type=int, help='max seq length, trim longer sentence.')
     args = parser.parse_args()
     print(args)
     # create model
     m = BertClassifier(
-        model_dir=args.model_dir,
         num_classes=args.num_classes,
+        output_dir=args.output_dir,
         model_type=args.pretrain_model_type,
         model_name=args.pretrain_model_name,
         num_epochs=args.num_epochs,
         batch_size=args.batch_size,
         max_seq_length=args.max_seq_length,
         multi_label=False,
     )
     # train model
     m.train(data_list_or_path=args.data_path)
-    # load trained best model and predict
+    # load trained model and predict
     m.load_model()
     print('best model loaded from file, and predict')
     X, y, _ = load_data(args.data_path)
     X = X[:5]
     y = y[:5]
     predict_labels, predict_probs = m.predict(X)
     for text, pred_label, pred_prob, y_truth in zip(X, predict_labels, predict_probs, y):
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/bert_multi_label_classification_model.py` & `pytextclassifier-1.3.6/pytextclassifier/bert_multi_label_classification_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description:
 """
-
-import sys
-from abc import ABC
-
 import torch
 from torch import nn
 from torch.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 from transformers import (
     BertModel,
     BertPreTrainedModel,
     DistilBertModel,
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/classic_classifier.py` & `pytextclassifier-1.3.6/pytextclassifier/classic_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,31 @@
 from pytextclassifier.tokenizer import Tokenizer
 
 pwd_path = os.path.abspath(os.path.dirname(__file__))
 default_stopwords_path = os.path.join(pwd_path, 'stopwords.txt')
 
 
 class ClassicClassifier(ClassifierABC):
-    def __init__(self, model_dir, model_name_or_model='lr', feature_name_or_feature='tfidf',
-                 stopwords_path=default_stopwords_path, tokenizer=None):
+    def __init__(
+            self,
+            output_dir="outputs",
+            model_name_or_model='lr',
+            feature_name_or_feature='tfidf',
+            stopwords_path=default_stopwords_path,
+            tokenizer=None
+    ):
         """
         经典机器学习分类模型，支持lr, random_forest, decision_tree, knn, bayes, svm, xgboost
-        @param model_dir: 模型保存路径
+        @param output_dir: 模型保存路径
         @param model_name_or_model:
         @param feature_name_or_feature:
         @param stopwords_path:
         @param tokenizer: 切词器，默认为jieba切词
         """
-        self.model_dir = model_dir
+        self.output_dir = output_dir
         if isinstance(model_name_or_model, str):
             model_name = model_name_or_model.lower()
             if model_name not in ['lr', 'random_forest', 'decision_tree', 'knn', 'bayes', 'xgboost', 'svm']:
                 raise ValueError('model_name not found.')
             logger.debug(f'model_name: {model_name}')
             self.model = self.get_model(model_name)
         elif hasattr(model_name_or_model, 'fit'):
@@ -127,15 +133,15 @@
             return
         if pkl_path:
             with open(pkl_path, 'wb') as f:
                 pickle.dump(vocab, f, protocol=pickle.HIGHEST_PROTOCOL)  # python3
 
     def train(self, data_list_or_path, header=None, names=('labels', 'text'), delimiter='\t', test_size=0.1):
         """
-        Train model with data_list_or_path and save model to model_dir
+        Train model with data_list_or_path and save model to output_dir
         @param data_list_or_path:
         @param header:
         @param names:
         @param delimiter:
         @param test_size:
         @return:
         """
@@ -195,58 +201,58 @@
         # evaluate the model
         y_pred, _ = self.predict(X_test)
         acc_score = metrics.accuracy_score(y_test, y_pred)
         return acc_score
 
     def load_model(self):
         """
-        Load model from model_dir
+        Load model from output_dir
         @return:
         """
-        model_path = os.path.join(self.model_dir, 'classifier_model.pkl')
+        model_path = os.path.join(self.output_dir, 'classifier_model.pkl')
         if os.path.exists(model_path):
             self.model = self.load_pkl(model_path)
-            feature_path = os.path.join(self.model_dir, 'classifier_feature.pkl')
+            feature_path = os.path.join(self.output_dir, 'classifier_feature.pkl')
             self.feature = self.load_pkl(feature_path)
             logger.info(f'Loaded model: {model_path}.')
             self.is_trained = True
         else:
             logger.error(f'{model_path} not exists.')
             self.is_trained = False
         return self.is_trained
 
     def save_model(self):
         """
-        Save model to model_dir
+        Save model to output_dir
         @return:
         """
-        if self.model_dir:
-            os.makedirs(self.model_dir, exist_ok=True)
+        if self.output_dir:
+            os.makedirs(self.output_dir, exist_ok=True)
         if self.is_trained:
-            feature_path = os.path.join(self.model_dir, 'classifier_feature.pkl')
+            feature_path = os.path.join(self.output_dir, 'classifier_feature.pkl')
             self.save_pkl(self.feature, feature_path)
-            model_path = os.path.join(self.model_dir, 'classifier_model.pkl')
+            model_path = os.path.join(self.output_dir, 'classifier_model.pkl')
             self.save_pkl(self.model, model_path)
             logger.info(f'Saved model: {model_path}, feature_path: {feature_path}')
         else:
             logger.error('model is not trained, please train model first')
         return self.model, self.feature
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Text Classification')
     parser.add_argument('--model_name', default='lr', type=str, help='model name')
-    parser.add_argument('--model_dir', default='models/lr', type=str, help='model dir')
+    parser.add_argument('--output_dir', default='models/lr', type=str, help='saved model dir')
     parser.add_argument('--feature_name', default='tfidf', type=str, help='feature name')
     parser.add_argument('--data_path', default=os.path.join(pwd_path, '../examples/thucnews_train_1w.txt'),
                         type=str, help='sample data file path')
     args = parser.parse_args()
     print(args)
     # create model
-    m = ClassicClassifier(args.model_dir, model_name_or_model=args.model_name,
+    m = ClassicClassifier(output_dir=args.output_dir, model_name_or_model=args.model_name,
                           feature_name_or_feature=args.feature_name)
     # train model
     m.train(args.data_path)
     # load best trained model and predict
     m.load_model()
     X, y, _ = load_data(args.data_path)
     X = X[:5]
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/data_helper.py` & `pytextclassifier-1.3.6/pytextclassifier/data_helper.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/pytextclassifier/fasttext_classifier.py` & `pytextclassifier-1.3.6/pytextclassifier/fasttext_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,15 +145,21 @@
     return DatasetIterater(dataset, device, batch_size)
 
 
 class FastTextModel(nn.Module):
     """Bag of Tricks for Efficient Text Classification"""
 
     def __init__(
-            self, vocab_size, num_classes, embed_size=200, n_gram_vocab=250499, hidden_size=256, dropout_rate=0.5
+            self,
+            vocab_size,
+            num_classes,
+            embed_size=200,
+            n_gram_vocab=250499,
+            hidden_size=256,
+            dropout_rate=0.5
     ):
         super().__init__()
         self.embedding = nn.Embedding(vocab_size, embed_size, padding_idx=vocab_size - 1)
         self.embedding_ngram2 = nn.Embedding(n_gram_vocab, embed_size)
         self.embedding_ngram3 = nn.Embedding(n_gram_vocab, embed_size)
         self.dropout = nn.Dropout(dropout_rate)
         self.fc1 = nn.Linear(embed_size * 3, hidden_size)
@@ -172,37 +178,37 @@
         out = self.fc2(out)
         return out
 
 
 class FastTextClassifier(ClassifierABC):
     def __init__(
             self,
-            model_dir,
+            output_dir="outputs",
             dropout_rate=0.5, batch_size=64, max_seq_length=128,
             embed_size=200, hidden_size=256, n_gram_vocab=250499,
             max_vocab_size=10000, unk_token='[UNK]', pad_token='[PAD]',
             tokenizer=None,
             enable_ngram=True,
     ):
         """
         初始化
-        @param model_dir: 模型的保存路径
+        @param output_dir: 模型的保存路径
         @param dropout_rate: 随机失活
         @param batch_size: mini-batch大小
         @param max_seq_length: 每句话处理成的长度(短填长切)
         @param embed_size: 字向量维度
         @param hidden_size: 隐藏层大小
         @param n_gram_vocab: ngram 词表大小
         @param max_vocab_size: 词表长度限制
         @param unk_token: 未知字
         @param pad_token: padding符号
         @param tokenizer: 切词器
         @param enable_ngram: 是否使用ngram
         """
-        self.model_dir = model_dir
+        self.output_dir = output_dir
         self.is_trained = False
         self.model = None
         logger.debug(f'device: {device}')
         self.dropout_rate = dropout_rate
         self.batch_size = batch_size
         self.max_seq_length = max_seq_length
         self.embed_size = embed_size
@@ -221,15 +227,15 @@
             self,
             data_list_or_path,
             header=None, names=('labels', 'text'), delimiter='\t', test_size=0.1,
             num_epochs=20, learning_rate=1e-3,
             require_improvement=1000, evaluate_during_training_steps=100
     ):
         """
-        Train model with data_list_or_path and save model to model_dir
+        Train model with data_list_or_path and save model to output_dir
         @param data_list_or_path:
         @param header:
         @param names:
         @param delimiter:
         @param test_size:
         @param num_epochs: epoch数
         @param learning_rate: 学习率
@@ -238,20 +244,20 @@
         @return:
         """
         logger.debug('train model...')
         SEED = 1
         set_seed(SEED)
         # load data
         X, y, data_df = load_data(data_list_or_path, header=header, names=names, delimiter=delimiter, is_train=True)
-        model_dir = self.model_dir
-        if model_dir:
-            os.makedirs(model_dir, exist_ok=True)
-        word_vocab_path = os.path.join(model_dir, 'word_vocab.json')
-        label_vocab_path = os.path.join(model_dir, 'label_vocab.json')
-        save_model_path = os.path.join(model_dir, 'model.pth')
+        output_dir = self.output_dir
+        if output_dir:
+            os.makedirs(output_dir, exist_ok=True)
+        word_vocab_path = os.path.join(output_dir, 'word_vocab.json')
+        label_vocab_path = os.path.join(output_dir, 'label_vocab.json')
+        save_model_path = os.path.join(output_dir, 'model.pth')
 
         dataset, self.word_id_map, self.label_id_map = build_dataset(
             self.tokenizer, X, y, word_vocab_path,
             label_vocab_path,
             max_vocab_size=self.max_vocab_size,
             max_seq_length=self.max_seq_length,
             unk_token=self.unk_token,
@@ -454,21 +460,21 @@
                 predict_all = np.append(predict_all, predic)
             logger.debug(f"evaluate, last batch, y_true: {labels}, y_pred: {predic}")
         acc = metrics.accuracy_score(labels_all, predict_all)
         return acc, loss_total / len(data_iter)
 
     def load_model(self):
         """
-        Load model from model_dir
+        Load model from output_dir
         @return:
         """
-        model_path = os.path.join(self.model_dir, 'model.pth')
+        model_path = os.path.join(self.output_dir, 'model.pth')
         if os.path.exists(model_path):
-            self.word_vocab_path = os.path.join(self.model_dir, 'word_vocab.json')
-            self.label_vocab_path = os.path.join(self.model_dir, 'label_vocab.json')
+            self.word_vocab_path = os.path.join(self.output_dir, 'word_vocab.json')
+            self.label_vocab_path = os.path.join(self.output_dir, 'label_vocab.json')
             self.word_id_map = load_vocab(self.word_vocab_path)
             self.label_id_map = load_vocab(self.label_vocab_path)
             vocab_size = len(self.word_id_map)
             num_classes = len(self.label_id_map)
             self.model = FastTextModel(
                 vocab_size, num_classes, self.embed_size, self.n_gram_vocab, self.hidden_size,
                 self.dropout_rate
@@ -480,24 +486,24 @@
             logger.error(f'{model_path} not exists.')
             self.is_trained = False
         return self.is_trained
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Text Classification')
-    parser.add_argument('--model_dir', default='models/fasttext', type=str, help='save model dir')
+    parser.add_argument('--output_dir', default='models/fasttext', type=str, help='save model dir')
     parser.add_argument('--data_path', default=os.path.join(pwd_path, '../examples/thucnews_train_1w.txt'),
                         type=str, help='sample data file path')
     args = parser.parse_args()
     print(args)
     # create model
-    m = FastTextClassifier(args.model_dir)
+    m = FastTextClassifier(args.output_dir)
     # train model
     m.train(data_list_or_path=args.data_path, num_epochs=3)
-    # load trained best model and predict
+    # load trained model and predict
     m.load_model()
     print('best model loaded from file, and predict')
     X, y, _ = load_data(args.data_path)
     X = X[:5]
     y = y[:5]
     predict_labels, predict_probs = m.predict(X)
     for text, pred_label, pred_prob, y_truth in zip(X, predict_labels, predict_probs, y):
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/stopwords.txt` & `pytextclassifier-1.3.6/pytextclassifier/stopwords.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/pytextclassifier/textcluster.py` & `pytextclassifier-1.3.6/pytextclassifier/textcluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 import os
+import sys
 from codecs import open
 import pickle
 from sklearn.cluster import MiniBatchKMeans
 from sklearn.feature_extraction.text import TfidfVectorizer
 from loguru import logger
+
+sys.path.append('..')
 from pytextclassifier.tokenizer import Tokenizer
 
 pwd_path = os.path.abspath(os.path.dirname(__file__))
 default_stopwords_path = os.path.join(pwd_path, 'stopwords.txt')
 
 
 class TextCluster(object):
     def __init__(
             self,
-            model_dir,
+            output_dir="outputs",
             model=None, tokenizer=None, feature=None,
             stopwords_path=default_stopwords_path,
             n_clusters=3, n_init=10, ngram_range=(1, 2), **kwargs
     ):
-        self.model_dir = model_dir
+        self.output_dir = output_dir
         self.model = model if model else MiniBatchKMeans(n_clusters=n_clusters, n_init=n_init)
         self.tokenizer = tokenizer if tokenizer else Tokenizer()
         self.feature = feature if feature else TfidfVectorizer(ngram_range=ngram_range, **kwargs)
         self.stopwords = set(self.load_list(stopwords_path)) if stopwords_path and os.path.exists(
             stopwords_path) else set()
         self.is_trained = False
 
@@ -130,20 +133,20 @@
         X_tokens = self.tokenize_sentences(sentences)
         logger.debug('data tokens top 1: {}'.format(X_tokens[:1]))
         feature = self.feature.fit_transform(X_tokens)
         # fit cluster
         self.model.fit(feature)
         labels = self.model.labels_
         logger.debug('cluster labels:{}'.format(labels))
-        model_dir = self.model_dir
-        if model_dir:
-            os.makedirs(model_dir, exist_ok=True)
-        feature_path = os.path.join(model_dir, 'cluster_feature.pkl')
+        output_dir = self.output_dir
+        if output_dir:
+            os.makedirs(output_dir, exist_ok=True)
+        feature_path = os.path.join(output_dir, 'cluster_feature.pkl')
         self.save_pkl(self.feature, feature_path)
-        model_path = os.path.join(model_dir, 'cluster_model.pkl')
+        model_path = os.path.join(output_dir, 'cluster_model.pkl')
         self.save_pkl(self.model, model_path)
         logger.info('save done. feature path: {}, model path: {}'.format(feature_path, model_path))
 
         self.is_trained = True
         return feature, labels
 
     def predict(self, X):
@@ -170,31 +173,31 @@
         """
         if not self.is_trained:
             raise ValueError('model is None, run train first.')
         self.show_plt(feature_matrix, labels, image_file)
 
     def load_model(self):
         """
-        Load model from model_dir
-        :param model_dir: path
+        Load model from output_dir
+        :param output_dir: path
         :return: None
         """
-        model_path = os.path.join(self.model_dir, 'cluster_model.pkl')
+        model_path = os.path.join(self.output_dir, 'cluster_model.pkl')
         if not os.path.exists(model_path):
             raise ValueError("model is not found. please train and save model first.")
         self.model = self.load_pkl(model_path)
-        feature_path = os.path.join(self.model_dir, 'cluster_feature.pkl')
+        feature_path = os.path.join(self.output_dir, 'cluster_feature.pkl')
         self.feature = self.load_pkl(feature_path)
         self.is_trained = True
-        logger.info('model loaded {}'.format(self.model_dir))
+        logger.info('model loaded {}'.format(self.output_dir))
         return self.is_trained
 
 
 if __name__ == '__main__':
-    m = TextCluster(model_dir='models/cluster', n_clusters=2)
+    m = TextCluster(output_dir='models/cluster', n_clusters=2)
     print(m)
     data = [
         'Student debt to cost Britain billions within decades',
         'Chinese education for TV experiment',
         'Abbott government spends $8 million on higher education',
         'Middle East and Asia boost investment in top level sports',
         'Summit Series look launches HBO Canada sports doc series: Mudhar'
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/textcnn_classifier.py` & `pytextclassifier-1.3.6/pytextclassifier/textcnn_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,35 +154,35 @@
         out = self.fc(out)
         return out
 
 
 class TextCNNClassifier(ClassifierABC):
     def __init__(
             self,
-            model_dir,
+            output_dir="outputs",
             filter_sizes=(2, 3, 4), num_filters=256,
             dropout_rate=0.5, batch_size=64, max_seq_length=128,
             embed_size=200, max_vocab_size=10000,
             unk_token='[UNK]', pad_token='[PAD]', tokenizer=None,
     ):
         """
         Init the TextCNNClassifier
-        @param model_dir: 模型保存路径
+        @param output_dir: 模型保存路径
         @param filter_sizes: 卷积核尺寸
         @param num_filters: 卷积核数量(channels数)
         @param dropout_rate:
         @param batch_size:
         @param max_seq_length:
         @param embed_size:
         @param max_vocab_size:
         @param unk_token:
         @param pad_token:
         @param tokenizer: 切词器，默认为字粒度切分
         """
-        self.model_dir = model_dir
+        self.output_dir = output_dir
         self.is_trained = False
         self.model = None
         logger.debug(f'device: {device}')
         self.filter_sizes = filter_sizes
         self.num_filters = num_filters
         self.dropout_rate = dropout_rate
         self.batch_size = batch_size
@@ -200,17 +200,17 @@
             self,
             data_list_or_path,
             header=None, names=('labels', 'text'), delimiter='\t', test_size=0.1,
             num_epochs=20, learning_rate=1e-3,
             require_improvement=1000, evaluate_during_training_steps=100
     ):
         """
-        Train model with data_list_or_path and save model to model_dir
+        Train model with data_list_or_path and save model to output_dir
         @param data_list_or_path:
-        @param model_dir:
+        @param output_dir:
         @param header:
         @param names:
         @param delimiter:
         @param test_size:
         @param num_epochs: epoch数
         @param learning_rate: 学习率
         @param require_improvement: 若超过1000batch效果还没提升，则提前结束训练
@@ -218,20 +218,20 @@
         @return:
         """
         logger.debug('train model...')
         SEED = 1
         set_seed(SEED)
         # load data
         X, y, data_df = load_data(data_list_or_path, header=header, names=names, delimiter=delimiter, is_train=True)
-        model_dir = self.model_dir
-        if model_dir:
-            os.makedirs(model_dir, exist_ok=True)
-        word_vocab_path = os.path.join(model_dir, 'word_vocab.json')
-        label_vocab_path = os.path.join(model_dir, 'label_vocab.json')
-        save_model_path = os.path.join(model_dir, 'model.pth')
+        output_dir = self.output_dir
+        if output_dir:
+            os.makedirs(output_dir, exist_ok=True)
+        word_vocab_path = os.path.join(output_dir, 'word_vocab.json')
+        label_vocab_path = os.path.join(output_dir, 'label_vocab.json')
+        save_model_path = os.path.join(output_dir, 'model.pth')
 
         dataset, self.word_id_map, self.label_id_map = build_dataset(
             self.tokenizer, X, y,
             word_vocab_path,
             label_vocab_path,
             max_vocab_size=self.max_vocab_size,
             max_seq_length=self.max_seq_length,
@@ -406,21 +406,21 @@
                 predict_all = np.append(predict_all, predic)
             logger.debug(f"evaluate, last batch, y_true: {labels}, y_pred: {predic}")
         acc = metrics.accuracy_score(labels_all, predict_all)
         return acc, loss_total / len(data_iter)
 
     def load_model(self):
         """
-        Load model from model_dir
+        Load model from output_dir
         @return:
         """
-        model_path = os.path.join(self.model_dir, 'model.pth')
+        model_path = os.path.join(self.output_dir, 'model.pth')
         if os.path.exists(model_path):
-            self.word_vocab_path = os.path.join(self.model_dir, 'word_vocab.json')
-            self.label_vocab_path = os.path.join(self.model_dir, 'label_vocab.json')
+            self.word_vocab_path = os.path.join(self.output_dir, 'word_vocab.json')
+            self.label_vocab_path = os.path.join(self.output_dir, 'label_vocab.json')
             self.word_id_map = load_vocab(self.word_vocab_path)
             self.label_id_map = load_vocab(self.label_vocab_path)
             vocab_size = len(self.word_id_map)
             num_classes = len(self.label_id_map)
             self.model = TextCNNModel(
                 vocab_size, num_classes,
                 embed_size=self.embed_size,
@@ -435,24 +435,24 @@
             logger.error(f'{model_path} not exists.')
             self.is_trained = False
         return self.is_trained
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Text Classification')
-    parser.add_argument('--model_dir', default='models/textcnn', type=str, help='save model dir')
+    parser.add_argument('--output_dir', default='models/textcnn', type=str, help='save model dir')
     parser.add_argument('--data_path', default=os.path.join(pwd_path, '../examples/thucnews_train_1w.txt'),
                         type=str, help='sample data file path')
     args = parser.parse_args()
     print(args)
     # create model
-    m = TextCNNClassifier(model_dir=args.model_dir)
+    m = TextCNNClassifier(output_dir=args.output_dir)
     # train model
     m.train(data_list_or_path=args.data_path, num_epochs=3)
-    # load trained best model and predict
+    # load trained model and predict
     m.load_model()
     print('best model loaded from file, and predict')
     X, y, _ = load_data(args.data_path)
     X = X[:5]
     y = y[:5]
     predict_labels, predict_probs = m.predict(X)
     for text, pred_label, pred_prob, y_truth in zip(X, predict_labels, predict_probs, y):
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/textrnn_classifier.py` & `pytextclassifier-1.3.6/pytextclassifier/textrnn_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,36 +162,36 @@
         out = self.fc2(out)  # [128, 64]
         return out
 
 
 class TextRNNClassifier(ClassifierABC):
     def __init__(
             self,
-            model_dir,
+            output_dir="outputs",
             hidden_size=128,
             num_layers=2,
             dropout_rate=0.5, batch_size=64, max_seq_length=128,
             embed_size=200, max_vocab_size=10000, unk_token='[UNK]',
             pad_token='[PAD]', tokenizer=None,
     ):
         """
         Init the TextRNNClassifier
-        @param model_dir: 模型保存路径
+        @param output_dir: 模型保存路径
         @param hidden_size: lstm隐藏层
         @param num_layers: lstm层数
         @param dropout_rate:
         @param batch_size:
         @param max_seq_length:
         @param embed_size:
         @param max_vocab_size:
         @param unk_token:
         @param pad_token:
         @param tokenizer: 切词器，默认为字粒度切分
         """
-        self.model_dir = model_dir
+        self.output_dir = output_dir
         self.is_trained = False
         self.model = None
         logger.debug(f'device: {device}')
         self.hidden_size = hidden_size
         self.num_layers = num_layers
         self.dropout_rate = dropout_rate
         self.batch_size = batch_size
@@ -209,15 +209,15 @@
             self,
             data_list_or_path,
             header=None, names=('labels', 'text'), delimiter='\t', test_size=0.1,
             num_epochs=20, learning_rate=1e-3,
             require_improvement=1000, evaluate_during_training_steps=100
     ):
         """
-        Train model with data_list_or_path and save model to model_dir
+        Train model with data_list_or_path and save model to output_dir
         @param data_list_or_path:
         @param header:
         @param names:
         @param delimiter:
         @param test_size:
         @param num_epochs: epoch数
         @param learning_rate: 学习率
@@ -226,20 +226,20 @@
         @return:
         """
         logger.debug('train model...')
         SEED = 1
         set_seed(SEED)
         # load data
         X, y, data_df = load_data(data_list_or_path, header=header, names=names, delimiter=delimiter, is_train=True)
-        model_dir = self.model_dir
-        if model_dir:
-            os.makedirs(model_dir, exist_ok=True)
-        word_vocab_path = os.path.join(model_dir, 'word_vocab.json')
-        label_vocab_path = os.path.join(model_dir, 'label_vocab.json')
-        save_model_path = os.path.join(model_dir, 'model.pth')
+        output_dir = self.output_dir
+        if output_dir:
+            os.makedirs(output_dir, exist_ok=True)
+        word_vocab_path = os.path.join(output_dir, 'word_vocab.json')
+        label_vocab_path = os.path.join(output_dir, 'label_vocab.json')
+        save_model_path = os.path.join(output_dir, 'model.pth')
 
         dataset, self.word_id_map, self.label_id_map = build_dataset(
             self.tokenizer, X, y,
             word_vocab_path,
             label_vocab_path,
             max_vocab_size=self.max_vocab_size,
             max_seq_length=self.max_seq_length,
@@ -373,14 +373,22 @@
         id_label_map = {v: k for k, v in self.label_id_map.items()}
         predict_labels = [id_label_map.get(i) for i in predict_all]
         predict_probs = proba_all.tolist()
         return predict_labels, predict_probs
 
     def evaluate_model(self, data_list_or_path, header=None,
                        names=('labels', 'text'), delimiter='\t'):
+        """
+        Evaluate model.
+        @param data_list_or_path:
+        @param header:
+        @param names:
+        @param delimiter:
+        @return:
+        """
         X_test, y_test, df = load_data(data_list_or_path, header=header, names=names, delimiter=delimiter)
         self.load_model()
         data, word_id_map, label_id_map = build_dataset(
             self.tokenizer, X_test, y_test,
             self.word_vocab_path,
             self.label_vocab_path,
             max_vocab_size=self.max_vocab_size,
@@ -414,21 +422,21 @@
                 predict_all = np.append(predict_all, predic)
             logger.debug(f"evaluate, last batch, y_true: {labels}, y_pred: {predic}")
         acc = metrics.accuracy_score(labels_all, predict_all)
         return acc, loss_total / len(data_iter)
 
     def load_model(self):
         """
-        Load model from model_dir
+        Load model from output_dir
         @return:
         """
-        model_path = os.path.join(self.model_dir, 'model.pth')
+        model_path = os.path.join(self.output_dir, 'model.pth')
         if os.path.exists(model_path):
-            self.word_vocab_path = os.path.join(self.model_dir, 'word_vocab.json')
-            self.label_vocab_path = os.path.join(self.model_dir, 'label_vocab.json')
+            self.word_vocab_path = os.path.join(self.output_dir, 'word_vocab.json')
+            self.label_vocab_path = os.path.join(self.output_dir, 'label_vocab.json')
             self.word_id_map = load_vocab(self.word_vocab_path)
             self.label_id_map = load_vocab(self.label_vocab_path)
             vocab_size = len(self.word_id_map)
             num_classes = len(self.label_id_map)
             self.model = TextRNNAttModel(
                 vocab_size, num_classes,
                 embed_size=self.embed_size,
@@ -443,24 +451,24 @@
             logger.error(f'{model_path} not exists.')
             self.is_trained = False
         return self.is_trained
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Text Classification')
-    parser.add_argument('--model_dir', default='models/textrnn', type=str, help='save model dir')
+    parser.add_argument('--output_dir', default='models/textrnn', type=str, help='save model dir')
     parser.add_argument('--data_path', default=os.path.join(pwd_path, '../examples/thucnews_train_1w.txt'),
                         type=str, help='sample data file path')
     args = parser.parse_args()
     print(args)
     # create model
-    m = TextRNNClassifier(args.model_dir)
+    m = TextRNNClassifier(args.output_dir)
     # train model
     m.train(data_list_or_path=args.data_path, num_epochs=3)
-    # load trained best model and predict
+    # load trained the best model and predict
     m.load_model()
     print('best model loaded from file, and predict')
     X, y, _ = load_data(args.data_path)
     X = X[:5]
     y = y[:5]
     predict_labels, predict_probs = m.predict(X)
     for text, pred_label, pred_prob, y_truth in zip(X, predict_labels, predict_probs, y):
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier/time_util.py` & `pytextclassifier-1.3.6/pytextclassifier/time_util.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/pytextclassifier/tokenizer.py` & `pytextclassifier-1.3.6/pytextclassifier/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/pytextclassifier.egg-info/PKG-INFO` & `pytextclassifier-1.3.6/pytextclassifier.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,1649 +1,1697 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 7465  : 2.1.Name: pyte
 00000020: 7874 636c 6173 7369 6669 6572 0a56 6572  xtclassifier.Ver
-00000030: 7369 6f6e 3a20 312e 332e 350a 5375 6d6d  sion: 1.3.5.Summ
+00000030: 7369 6f6e 3a20 312e 332e 360a 5375 6d6d  sion: 1.3.6.Summ
 00000040: 6172 793a 2054 6578 7420 436c 6173 7369  ary: Text Classi
 00000050: 6669 6572 2c20 5465 7874 2043 6c61 7373  fier, Text Class
 00000060: 6966 6963 6174 696f 6e0a 486f 6d65 2d70  ification.Home-p
 00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
 00000080: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
 00000090: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
 000000a0: 6965 720a 4175 7468 6f72 3a20 5875 4d69  ier.Author: XuMi
 000000b0: 6e67 0a41 7574 686f 722d 656d 6169 6c3a  ng.Author-email:
 000000c0: 2078 756d 696e 6736 3234 4071 712e 636f   xuming624@qq.co
 000000d0: 6d0a 4c69 6365 6e73 653a 2041 7061 6368  m.License: Apach
 000000e0: 6520 322e 300a 4465 7363 7269 7074 696f  e 2.0.Descriptio
-000000f0: 6e3a 205b 215b 5079 5049 2076 6572 7369  n: [![PyPI versi
-00000100: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
-00000110: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
-00000120: 6578 7463 6c61 7373 6966 6965 722e 7376  extclassifier.sv
-00000130: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
-00000140: 652e 6675 7279 2e69 6f2f 7079 2f70 7974  e.fury.io/py/pyt
-00000150: 6578 7463 6c61 7373 6966 6965 7229 0a20  extclassifier). 
-00000160: 2020 2020 2020 205b 215b 446f 776e 6c6f         [![Downlo
-00000170: 6164 735d 2868 7474 7073 3a2f 2f70 6570  ads](https://pep
-00000180: 792e 7465 6368 2f62 6164 6765 2f70 7974  y.tech/badge/pyt
-00000190: 6578 7463 6c61 7373 6966 6965 7229 5d28  extclassifier)](
-000001a0: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
-000001b0: 682f 7072 6f6a 6563 742f 7079 7465 7874  h/project/pytext
-000001c0: 636c 6173 7369 6669 6572 290a 2020 2020  classifier).    
-000001d0: 2020 2020 5b21 5b43 6f6e 7472 6962 7574      [![Contribut
-000001e0: 696f 6e73 2077 656c 636f 6d65 5d28 6874  ions welcome](ht
-000001f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000200: 732e 696f 2f62 6164 6765 2f63 6f6e 7472  s.io/badge/contr
-00000210: 6962 7574 696f 6e73 2d77 656c 636f 6d65  ibutions-welcome
-00000220: 2d62 7269 6768 7467 7265 656e 2e73 7667  -brightgreen.svg
-00000230: 295d 2843 4f4e 5452 4942 5554 494e 472e  )](CONTRIBUTING.
-00000240: 6d64 290a 2020 2020 2020 2020 5b21 5b47  md).        [![G
-00000250: 6974 4875 6220 636f 6e74 7269 6275 746f  itHub contributo
-00000260: 7273 5d28 6874 7470 733a 2f2f 696d 672e  rs](https://img.
-00000270: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00000280: 622f 636f 6e74 7269 6275 746f 7273 2f73  b/contributors/s
-00000290: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
-000002a0: 636c 6173 7369 6669 6572 2e73 7667 295d  classifier.svg)]
-000002b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000002c0: 636f 6d2f 7368 6962 696e 6736 3234 2f70  com/shibing624/p
-000002d0: 7974 6578 7463 6c61 7373 6966 6965 722f  ytextclassifier/
-000002e0: 6772 6170 6873 2f63 6f6e 7472 6962 7574  graphs/contribut
-000002f0: 6f72 7329 0a20 2020 2020 2020 205b 215b  ors).        [![
-00000300: 4c69 6365 6e73 6520 4170 6163 6865 2032  License Apache 2
-00000310: 2e30 5d28 6874 7470 733a 2f2f 696d 672e  .0](https://img.
-00000320: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000330: 2f6c 6963 656e 7365 2d41 7061 6368 6525  /license-Apache%
-00000340: 3230 322e 302d 626c 7565 2e73 7667 295d  202.0-blue.svg)]
-00000350: 284c 4943 454e 5345 290a 2020 2020 2020  (LICENSE).      
-00000360: 2020 5b21 5b70 7974 686f 6e5f 7665 7369    [![python_vesi
-00000370: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-00000380: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000390: 2f50 7974 686f 6e2d 332e 3525 3242 2d67  /Python-3.5%2B-g
-000003a0: 7265 656e 2e73 7667 295d 2872 6571 7569  reen.svg)](requi
-000003b0: 7265 6d65 6e74 732e 7478 7429 0a20 2020  rements.txt).   
-000003c0: 2020 2020 205b 215b 4769 7448 7562 2069       [![GitHub i
-000003d0: 7373 7565 735d 2868 7474 7073 3a2f 2f69  ssues](https://i
-000003e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-000003f0: 7468 7562 2f69 7373 7565 732f 7368 6962  thub/issues/shib
-00000400: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
-00000410: 7373 6966 6965 722e 7376 6729 5d28 6874  ssifier.svg)](ht
-00000420: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000430: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
-00000440: 7874 636c 6173 7369 6669 6572 2f69 7373  xtclassifier/iss
-00000450: 7565 7329 0a20 2020 2020 2020 205b 215b  ues).        [![
-00000460: 5765 6368 6174 2047 726f 7570 5d28 6874  Wechat Group](ht
-00000470: 7470 3a2f 2f76 6c6f 672e 7366 7963 2e6c  tp://vlog.sfyc.l
-00000480: 7464 2f77 6563 6861 745f 6576 6572 7964  td/wechat_everyd
-00000490: 6179 2f77 7867 726f 7570 5f6c 6f67 6f2e  ay/wxgroup_logo.
-000004a0: 706e 673f 696d 6167 6556 6965 7732 2f30  png?imageView2/0
-000004b0: 2f77 2f36 302f 682f 3230 295d 2823 436f  /w/60/h/20)](#Co
-000004c0: 6e74 6163 7429 0a20 2020 2020 2020 200a  ntact).        .
-000004d0: 2020 2020 2020 2020 2320 5079 5465 7874          # PyText
-000004e0: 436c 6173 7369 6669 6572 0a20 2020 2020  Classifier.     
-000004f0: 2020 2050 7954 6578 7443 6c61 7373 6966     PyTextClassif
-00000500: 6965 722c 2050 7974 686f 6e20 5465 7874  ier, Python Text
-00000510: 2043 6c61 7373 6966 6965 722e 2049 7420   Classifier. It 
-00000520: 6361 6e20 6265 2061 7070 6c69 6564 2074  can be applied t
-00000530: 6f20 7468 6520 6669 656c 6473 206f 6620  o the fields of 
-00000540: 7365 6e74 696d 656e 7420 706f 6c61 7269  sentiment polari
-00000550: 7479 2061 6e61 6c79 7369 732c 2074 6578  ty analysis, tex
-00000560: 7420 7269 736b 2063 6c61 7373 6966 6963  t risk classific
-00000570: 6174 696f 6e20 616e 6420 736f 206f 6e2c  ation and so on,
-00000580: 0a20 2020 2020 2020 2061 6e64 2069 7420  .        and it 
-00000590: 7375 7070 6f72 7473 206d 756c 7469 706c  supports multipl
-000005a0: 6520 636c 6173 7369 6669 6361 7469 6f6e  e classification
-000005b0: 2061 6c67 6f72 6974 686d 7320 616e 6420   algorithms and 
-000005c0: 636c 7573 7465 7269 6e67 2061 6c67 6f72  clustering algor
-000005d0: 6974 686d 732e 0a20 2020 2020 2020 200a  ithms..        .
-000005e0: 2020 2020 2020 2020 e696 87e6 9cac e588          ........
-000005f0: 86e7 b1bb e599 a8ef bc8c e68f 90e4 be9b  ................
-00000600: e5a4 9ae7 a78d e696 87e6 9cac e588 86e7  ................
-00000610: b1bb e592 8ce8 819a e7b1 bbe7 ae97 e6b3  ................
-00000620: 95ef bc8c e694 afe6 8c81 e58f a5e5 ad90  ................
-00000630: e592 8ce6 9687 e6a1 a3e7 baa7 e79a 84e6  ................
-00000640: 9687 e69c ace5 8886 e7b1 bbe4 bbbb e58a  ................
-00000650: a1ef bc8c e694 afe6 8c81 e4ba 8ce5 8886  ................
-00000660: e7b1 bbe3 8081 e5a4 9ae5 8886 e7b1 bbe3  ................
-00000670: 8081 e5a4 9ae6 a087 e7ad bee5 8886 e7b1  ................
-00000680: bbe3 8081 e5a4 9ae5 b182 e7ba a7e5 8886  ................
-00000690: e7b1 bbe5 928c 4b6d 6561 6e73 e881 9ae7  ......Kmeans....
-000006a0: b1bb efbc 8ce5 bc80 e7ae b1e5 8db3 e794  ................
-000006b0: a8e3 8082 7079 7468 6f6e 33e5 bc80 e58f  ....python3.....
-000006c0: 91e3 8082 0a20 2020 2020 2020 200a 2020  .....        .  
-000006d0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-000006e0: 2a47 7569 6465 2a2a 0a20 2020 2020 2020  *Guide**.       
-000006f0: 200a 2020 2020 2020 2020 2d20 5b46 6561   .        - [Fea
-00000700: 7475 7265 5d28 2346 6561 7475 7265 290a  ture](#Feature).
-00000710: 2020 2020 2020 2020 2d20 5b49 6e73 7461          - [Insta
-00000720: 6c6c 5d28 2369 6e73 7461 6c6c 290a 2020  ll](#install).  
-00000730: 2020 2020 2020 2d20 5b55 7361 6765 5d28        - [Usage](
-00000740: 2375 7361 6765 290a 2020 2020 2020 2020  #usage).        
-00000750: 2d20 5b44 6174 6173 6574 5d28 2344 6174  - [Dataset](#Dat
-00000760: 6173 6574 290a 2020 2020 2020 2020 2d20  aset).        - 
-00000770: 5b43 6f6e 7461 6374 5d28 2343 6f6e 7461  [Contact](#Conta
-00000780: 6374 290a 2020 2020 2020 2020 2d20 5b43  ct).        - [C
-00000790: 6974 6174 696f 6e5d 2823 4369 7461 7469  itation](#Citati
-000007a0: 6f6e 290a 2020 2020 2020 2020 2d20 5b52  on).        - [R
-000007b0: 6566 6572 656e 6365 5d28 2372 6566 6572  eference](#refer
-000007c0: 656e 6365 290a 2020 2020 2020 2020 0a20  ence).        . 
-000007d0: 2020 2020 2020 2023 2046 6561 7475 7265         # Feature
-000007e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000007f0: 2020 2a2a 7079 7465 7874 636c 6173 7369    **pytextclassi
-00000800: 6669 6572 2a2a 2069 7320 6120 7079 7468  fier** is a pyth
-00000810: 6f6e 204f 7065 6e20 536f 7572 6365 2054  on Open Source T
-00000820: 6f6f 6c6b 6974 2066 6f72 2074 6578 7420  oolkit for text 
-00000830: 636c 6173 7369 6669 6361 7469 6f6e 2e20  classification. 
-00000840: 5468 6520 676f 616c 2069 7320 746f 2069  The goal is to i
-00000850: 6d70 6c65 6d65 6e74 0a20 2020 2020 2020  mplement.       
-00000860: 2074 6578 7420 616e 616c 7973 6973 2061   text analysis a
-00000870: 6c67 6f72 6974 686d 2c20 736f 2061 7320  lgorithm, so as 
-00000880: 746f 2061 6368 6965 7665 2074 6865 2075  to achieve the u
-00000890: 7365 2069 6e20 7468 6520 7072 6f64 7563  se in the produc
-000008a0: 7469 6f6e 2065 6e76 6972 6f6e 6d65 6e74  tion environment
-000008b0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-000008c0: 2020 202a 2a70 7974 6578 7463 6c61 7373     **pytextclass
-000008d0: 6966 6965 722a 2a20 6861 7320 7468 6520  ifier** has the 
-000008e0: 6368 6172 6163 7465 7269 7374 6963 730a  characteristics.
-000008f0: 2020 2020 2020 2020 6f66 2063 6c65 6172          of clear
-00000900: 2061 6c67 6f72 6974 686d 2c20 6869 6768   algorithm, high
-00000910: 2070 6572 666f 726d 616e 6365 2061 6e64   performance and
-00000920: 2063 7573 746f 6d69 7a61 626c 6520 636f   customizable co
-00000930: 7270 7573 2e0a 2020 2020 2020 2020 0a20  rpus..        . 
-00000940: 2020 2020 2020 2046 756e 6374 696f 6e73         Functions
-00000950: efbc 9a0a 2020 2020 2020 2020 2323 2320  ....        ### 
-00000960: 436c 6173 7369 6669 6572 0a20 2020 2020  Classifier.     
-00000970: 2020 2020 202d 205b 785d 204c 6f67 6973       - [x] Logis
-00000980: 7469 6352 6567 7265 7373 696f 6e0a 2020  ticRegression.  
-00000990: 2020 2020 2020 2020 2d20 5b78 5d20 5261          - [x] Ra
-000009a0: 6e64 6f6d 2046 6f72 6573 740a 2020 2020  ndom Forest.    
-000009b0: 2020 2020 2020 2d20 5b78 5d20 4465 6369        - [x] Deci
-000009c0: 7369 6f6e 2054 7265 650a 2020 2020 2020  sion Tree.      
-000009d0: 2020 2020 2d20 5b78 5d20 4b2d 4e65 6172      - [x] K-Near
-000009e0: 6573 7420 4e65 6967 6862 6f75 7273 0a20  est Neighbours. 
-000009f0: 2020 2020 2020 2020 202d 205b 785d 204e           - [x] N
-00000a00: 6169 7665 2062 6179 6573 0a20 2020 2020  aive bayes.     
-00000a10: 2020 2020 202d 205b 785d 2058 6762 6f6f       - [x] Xgboo
-00000a20: 7374 0a20 2020 2020 2020 2020 202d 205b  st.          - [
-00000a30: 785d 2053 7570 706f 7274 2056 6563 746f  x] Support Vecto
-00000a40: 7220 4d61 6368 696e 6528 5356 4d29 0a20  r Machine(SVM). 
-00000a50: 2020 2020 2020 2020 202d 205b 785d 2054           - [x] T
-00000a60: 6578 7443 4e4e 0a20 2020 2020 2020 2020  extCNN.         
-00000a70: 202d 205b 785d 2054 6578 7452 4e4e 0a20   - [x] TextRNN. 
-00000a80: 2020 2020 2020 2020 202d 205b 785d 2046           - [x] F
-00000a90: 6173 7474 6578 740a 2020 2020 2020 2020  asttext.        
-00000aa0: 2020 2d20 5b78 5d20 4245 5254 0a20 2020    - [x] BERT.   
-00000ab0: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000ac0: 2320 436c 7573 7465 720a 2020 2020 2020  # Cluster.      
-00000ad0: 2020 2020 2d20 5b78 5d20 4d69 6e69 4261      - [x] MiniBa
-00000ae0: 7463 684b 6d65 616e 730a 2020 2020 2020  tchKmeans.      
-00000af0: 2020 0a20 2020 2020 2020 2057 6869 6c65    .        While
-00000b00: 2070 726f 7669 6469 6e67 2072 6963 6820   providing rich 
-00000b10: 6675 6e63 7469 6f6e 732c 202a 2a70 7974  functions, **pyt
-00000b20: 6578 7463 6c61 7373 6966 6965 722a 2a20  extclassifier** 
-00000b30: 696e 7465 726e 616c 206d 6f64 756c 6573  internal modules
-00000b40: 2061 6468 6572 6520 746f 206c 6f77 2063   adhere to low c
-00000b50: 6f75 706c 696e 672c 206d 6f64 656c 2061  oupling, model a
-00000b60: 6468 6572 656e 6365 2074 6f20 696e 6572  dherence to iner
-00000b70: 7420 6c6f 6164 696e 672c 2064 6963 7469  t loading, dicti
-00000b80: 6f6e 6172 7920 7075 626c 6963 6174 696f  onary publicatio
-00000b90: 6e2c 2061 6e64 2065 6173 7920 746f 2075  n, and easy to u
-00000ba0: 7365 2e0a 2020 2020 2020 2020 0a20 2020  se..        .   
-00000bb0: 2020 2020 2023 2049 6e73 7461 6c6c 0a20       # Install. 
-00000bc0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00000bd0: 2d20 5265 7175 6972 656d 656e 7473 2061  - Requirements a
-00000be0: 6e64 2049 6e73 7461 6c6c 6174 696f 6e0a  nd Installation.
-00000bf0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000c00: 2060 6060 0a20 2020 2020 2020 2070 6970   ```.        pip
-00000c10: 3320 696e 7374 616c 6c20 746f 7263 6820  3 install torch 
-00000c20: 2320 636f 6e64 6120 696e 7374 616c 6c20  # conda install 
-00000c30: 7079 746f 7263 680a 2020 2020 2020 2020  pytorch.        
-00000c40: 7069 7033 2069 6e73 7461 6c6c 2070 7974  pip3 install pyt
-00000c50: 6578 7463 6c61 7373 6966 6965 720a 2020  extclassifier.  
-00000c60: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00000c70: 2020 0a20 2020 2020 2020 206f 720a 2020    .        or.  
-00000c80: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
-00000c90: 6060 0a20 2020 2020 2020 2067 6974 2063  ``.        git c
-00000ca0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-00000cb0: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
-00000cc0: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
-00000cd0: 6965 722e 6769 740a 2020 2020 2020 2020  ier.git.        
-00000ce0: 6364 2070 7974 6578 7463 6c61 7373 6966  cd pytextclassif
-00000cf0: 6965 720a 2020 2020 2020 2020 7079 7468  ier.        pyth
-00000d00: 6f6e 3320 7365 7475 702e 7079 2069 6e73  on3 setup.py ins
-00000d10: 7461 6c6c 0a20 2020 2020 2020 2060 6060  tall.        ```
-00000d20: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000d30: 2020 0a20 2020 2020 2020 2023 2055 7361    .        # Usa
-00000d40: 6765 0a20 2020 2020 2020 2023 2054 6578  ge.        # Tex
-00000d50: 7420 436c 6173 7369 6669 6572 0a20 2020  t Classifier.   
-00000d60: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00000d70: 2045 6e67 6c69 7368 2054 6578 7420 436c   English Text Cl
-00000d80: 6173 7369 6669 6572 0a20 2020 2020 2020  assifier.       
-00000d90: 200a 2020 2020 2020 2020 496e 636c 7564   .        Includ
-00000da0: 696e 6720 6d6f 6465 6c20 7472 6169 6e69  ing model traini
-00000db0: 6e67 2c20 7361 7669 6e67 2c20 7072 6564  ng, saving, pred
-00000dc0: 6963 742c 2065 7661 6c75 6174 652c 2066  ict, evaluate, f
-00000dd0: 6f72 2065 7861 6d70 6c65 205b 6578 616d  or example [exam
-00000de0: 706c 6573 2f6c 725f 656e 5f63 6c61 7373  ples/lr_en_class
-00000df0: 6966 6963 6174 696f 6e5f 6465 6d6f 2e70  ification_demo.p
-00000e00: 795d 2865 7861 6d70 6c65 732f 6c72 5f65  y](examples/lr_e
-00000e10: 6e5f 636c 6173 7369 6669 6361 7469 6f6e  n_classification
-00000e20: 5f64 656d 6f2e 7079 293a 0a20 2020 2020  _demo.py):.     
-00000e30: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00000e40: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00000e50: 2020 2020 2020 2069 6d70 6f72 7420 7379         import sy
-00000e60: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
-00000e70: 2020 2073 7973 2e70 6174 682e 6170 7065     sys.path.appe
-00000e80: 6e64 2827 2e2e 2729 0a20 2020 2020 2020  nd('..').       
-00000e90: 2066 726f 6d20 7079 7465 7874 636c 6173   from pytextclas
-00000ea0: 7369 6669 6572 2069 6d70 6f72 7420 436c  sifier import Cl
-00000eb0: 6173 7369 6343 6c61 7373 6966 6965 720a  assicClassifier.
-00000ec0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000ed0: 2069 6620 5f5f 6e61 6d65 5f5f 203d 3d20   if __name__ == 
-00000ee0: 275f 5f6d 6169 6e5f 5f27 3a0a 2020 2020  '__main__':.    
-00000ef0: 2020 2020 2020 2020 6d20 3d20 436c 6173          m = Clas
-00000f00: 7369 6343 6c61 7373 6966 6965 7228 6d6f  sicClassifier(mo
-00000f10: 6465 6c5f 6469 723d 276d 6f64 656c 732f  del_dir='models/
-00000f20: 6c72 272c 206d 6f64 656c 5f6e 616d 655f  lr', model_name_
-00000f30: 6f72 5f6d 6f64 656c 3d27 6c72 2729 0a20  or_model='lr'). 
-00000f40: 2020 2020 2020 2020 2020 2023 2043 6c61             # Cla
-00000f50: 7373 6963 436c 6173 7369 6669 6572 2073  ssicClassifier s
-00000f60: 7570 706f 7274 206d 6f64 656c 5f6e 616d  upport model_nam
-00000f70: 65ef bc9a 6c72 2c20 7261 6e64 6f6d 5f66  e...lr, random_f
-00000f80: 6f72 6573 742c 2064 6563 6973 696f 6e5f  orest, decision_
-00000f90: 7472 6565 2c20 6b6e 6e2c 2062 6179 6573  tree, knn, bayes
-00000fa0: 2c20 7376 6d2c 2078 6762 6f6f 7374 0a20  , svm, xgboost. 
-00000fb0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00000fc0: 286d 290a 2020 2020 2020 2020 2020 2020  (m).            
-00000fd0: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00000fe0: 2020 2020 2020 2020 2028 2765 6475 6361           ('educa
-00000ff0: 7469 6f6e 272c 2027 5374 7564 656e 7420  tion', 'Student 
-00001000: 6465 6274 2074 6f20 636f 7374 2042 7269  debt to cost Bri
-00001010: 7461 696e 2062 696c 6c69 6f6e 7320 7769  tain billions wi
-00001020: 7468 696e 2064 6563 6164 6573 2729 2c0a  thin decades'),.
-00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001040: 2827 6564 7563 6174 696f 6e27 2c20 2743  ('education', 'C
-00001050: 6869 6e65 7365 2065 6475 6361 7469 6f6e  hinese education
-00001060: 2066 6f72 2054 5620 6578 7065 7269 6d65   for TV experime
-00001070: 6e74 2729 2c0a 2020 2020 2020 2020 2020  nt'),.          
-00001080: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
-00001090: 2027 4d69 6464 6c65 2045 6173 7420 616e   'Middle East an
-000010a0: 6420 4173 6961 2062 6f6f 7374 2069 6e76  d Asia boost inv
-000010b0: 6573 746d 656e 7420 696e 2074 6f70 206c  estment in top l
-000010c0: 6576 656c 2073 706f 7274 7327 292c 0a20  evel sports'),. 
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000010e0: 2773 706f 7274 7327 2c20 2753 756d 6d69  'sports', 'Summi
-000010f0: 7420 5365 7269 6573 206c 6f6f 6b20 6c61  t Series look la
-00001100: 756e 6368 6573 2048 424f 2043 616e 6164  unches HBO Canad
-00001110: 6120 7370 6f72 7473 2064 6f63 2073 6572  a sports doc ser
-00001120: 6965 733a 204d 7564 6861 7227 290a 2020  ies: Mudhar').  
-00001130: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00001140: 2020 2020 2020 2020 2320 7472 6169 6e20          # train 
-00001150: 616e 6420 7361 7665 2062 6573 7420 6d6f  and save best mo
-00001160: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
-00001170: 6d2e 7472 6169 6e28 6461 7461 290a 2020  m.train(data).  
-00001180: 2020 2020 2020 2020 2020 2320 6c6f 6164            # load
-00001190: 2062 6573 7420 6d6f 6465 6c20 6672 6f6d   best model from
-000011a0: 206d 6f64 656c 5f64 6972 0a20 2020 2020   model_dir.     
-000011b0: 2020 2020 2020 206d 2e6c 6f61 645f 6d6f         m.load_mo
-000011c0: 6465 6c28 290a 2020 2020 2020 2020 2020  del().          
-000011d0: 2020 7072 6564 6963 745f 6c61 6265 6c2c    predict_label,
-000011e0: 2070 7265 6469 6374 5f70 726f 6261 203d   predict_proba =
-000011f0: 206d 2e70 7265 6469 6374 285b 0a20 2020   m.predict([.   
-00001200: 2020 2020 2020 2020 2020 2020 2027 4162               'Ab
-00001210: 626f 7474 2067 6f76 6572 6e6d 656e 7420  bott government 
-00001220: 7370 656e 6473 2024 3820 6d69 6c6c 696f  spends $8 millio
-00001230: 6e20 6f6e 2068 6967 6865 7220 6564 7563  n on higher educ
-00001240: 6174 696f 6e20 6d65 6469 6120 626c 6974  ation media blit
-00001250: 7a27 5d29 0a20 2020 2020 2020 2020 2020  z']).           
-00001260: 2070 7269 6e74 2866 2770 7265 6469 6374   print(f'predict
-00001270: 5f6c 6162 656c 3a20 7b70 7265 6469 6374  _label: {predict
-00001280: 5f6c 6162 656c 7d2c 2070 7265 6469 6374  _label}, predict
-00001290: 5f70 726f 6261 3a20 7b70 7265 6469 6374  _proba: {predict
-000012a0: 5f70 726f 6261 7d27 290a 2020 2020 2020  _proba}').      
-000012b0: 2020 0a20 2020 2020 2020 2020 2020 2074    .            t
-000012c0: 6573 745f 6461 7461 203d 205b 0a20 2020  est_data = [.   
-000012d0: 2020 2020 2020 2020 2020 2020 2028 2765               ('e
-000012e0: 6475 6361 7469 6f6e 272c 2027 4162 626f  ducation', 'Abbo
-000012f0: 7474 2067 6f76 6572 6e6d 656e 7420 7370  tt government sp
-00001300: 656e 6473 2024 3820 6d69 6c6c 696f 6e20  ends $8 million 
-00001310: 6f6e 2068 6967 6865 7220 6564 7563 6174  on higher educat
-00001320: 696f 6e20 6d65 6469 6120 626c 6974 7a27  ion media blitz'
-00001330: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00001340: 2020 2028 2773 706f 7274 7327 2c20 274d     ('sports', 'M
-00001350: 6964 646c 6520 4561 7374 2061 6e64 2041  iddle East and A
-00001360: 7369 6120 626f 6f73 7420 696e 7665 7374  sia boost invest
-00001370: 6d65 6e74 2069 6e20 746f 7020 6c65 7665  ment in top leve
-00001380: 6c20 7370 6f72 7473 2729 2c0a 2020 2020  l sports'),.    
-00001390: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000013a0: 2020 2020 2020 6163 635f 7363 6f72 6520        acc_score 
-000013b0: 3d20 6d2e 6576 616c 7561 7465 5f6d 6f64  = m.evaluate_mod
-000013c0: 656c 2874 6573 745f 6461 7461 290a 2020  el(test_data).  
-000013d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000013e0: 6627 6163 635f 7363 6f72 653a 207b 6163  f'acc_score: {ac
-000013f0: 635f 7363 6f72 657d 2729 0a20 2020 2020  c_score}').     
-00001400: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
-00001410: 2020 2020 2020 2020 6f75 7470 7574 3a0a          output:.
-00001420: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001430: 2060 6060 0a20 2020 2020 2020 2043 6c61   ```.        Cla
-00001440: 7373 6963 436c 6173 7369 6669 6572 2069  ssicClassifier i
-00001450: 6e73 7461 6e63 6520 284c 6f67 6973 7469  nstance (Logisti
-00001460: 6352 6567 7265 7373 696f 6e28 6669 745f  cRegression(fit_
-00001470: 696e 7465 7263 6570 743d 4661 6c73 6529  intercept=False)
-00001480: 2c20 7374 6f70 776f 7264 7320 7369 7a65  , stopwords size
-00001490: 3a20 3234 3338 290a 2020 2020 2020 2020  : 2438).        
-000014a0: 7072 6564 6963 745f 6c61 6265 6c3a 205b  predict_label: [
-000014b0: 2765 6475 6361 7469 6f6e 275d 2c20 7072  'education'], pr
-000014c0: 6564 6963 745f 7072 6f62 613a 205b 302e  edict_proba: [0.
-000014d0: 3533 3738 3233 3633 3538 3439 3231 3132  5378236358492112
-000014e0: 5d0a 2020 2020 2020 2020 6163 635f 7363  ].        acc_sc
-000014f0: 6f72 653a 2031 2e30 0a20 2020 2020 2020  ore: 1.0.       
-00001500: 2060 6060 0a20 2020 2020 2020 200a 2020   ```.        .  
-00001510: 2020 2020 2020 2323 2043 6869 6e65 7365        ## Chinese
-00001520: 2054 6578 7420 436c 6173 7369 6669 6572   Text Classifier
-00001530: 28e4 b8ad e696 87e6 9687 e69c ace5 8886  (...............
-00001540: e7b1 bb29 0a20 2020 2020 2020 200a 2020  ...).        .  
-00001550: 2020 2020 2020 5465 7874 2063 6c61 7373        Text class
-00001560: 6966 6963 6174 696f 6e20 636f 6d70 6174  ification compat
-00001570: 6962 6c65 2077 6974 6820 4368 696e 6573  ible with Chines
-00001580: 6520 616e 6420 456e 676c 6973 6820 636f  e and English co
-00001590: 7270 6f72 612e 0a20 2020 2020 2020 200a  rpora..        .
-000015a0: 2020 2020 2020 2020 6578 616d 706c 6520          example 
-000015b0: 5b65 7861 6d70 6c65 732f 6c72 5f63 6c61  [examples/lr_cla
-000015c0: 7373 6966 6963 6174 696f 6e5f 6465 6d6f  ssification_demo
-000015d0: 2e70 795d 2865 7861 6d70 6c65 732f 6c72  .py](examples/lr
-000015e0: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
-000015f0: 6465 6d6f 2e70 7929 0a20 2020 2020 2020  demo.py).       
-00001600: 200a 2020 2020 2020 2020 6060 6070 7974   .        ```pyt
-00001610: 686f 6e0a 2020 2020 2020 2020 696d 706f  hon.        impo
-00001620: 7274 2073 7973 0a20 2020 2020 2020 200a  rt sys.        .
-00001630: 2020 2020 2020 2020 7379 732e 7061 7468          sys.path
-00001640: 2e61 7070 656e 6428 272e 2e27 290a 2020  .append('..').  
-00001650: 2020 2020 2020 6672 6f6d 2070 7974 6578        from pytex
-00001660: 7463 6c61 7373 6966 6965 7220 696d 706f  tclassifier impo
-00001670: 7274 2043 6c61 7373 6963 436c 6173 7369  rt ClassicClassi
-00001680: 6669 6572 0a20 2020 2020 2020 200a 2020  fier.        .  
-00001690: 2020 2020 2020 6966 205f 5f6e 616d 655f        if __name_
-000016a0: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
-000016b0: 0a20 2020 2020 2020 2020 2020 206d 203d  .            m =
-000016c0: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
-000016d0: 6572 286d 6f64 656c 5f64 6972 3d27 6d6f  er(model_dir='mo
-000016e0: 6465 6c73 2f6c 722d 746f 7927 2c20 6d6f  dels/lr-toy', mo
-000016f0: 6465 6c5f 6e61 6d65 5f6f 725f 6d6f 6465  del_name_or_mode
-00001700: 6c3d 276c 7227 290a 2020 2020 2020 2020  l='lr').        
-00001710: 2020 2020 2320 e7bb 8fe5 85b8 e588 86e7      # ..........
-00001720: b1bb e696 b9e6 b395 efbc 8ce6 94af e68c  ................
-00001730: 81e7 9a84 e6a8 a1e5 9e8b e58c 85e6 8bac  ................
-00001740: efbc 9a6c 722c 2072 616e 646f 6d5f 666f  ...lr, random_fo
-00001750: 7265 7374 2c20 6465 6369 7369 6f6e 5f74  rest, decision_t
-00001760: 7265 652c 206b 6e6e 2c20 6261 7965 732c  ree, knn, bayes,
-00001770: 2073 766d 2c20 7867 626f 6f73 740a 2020   svm, xgboost.  
-00001780: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00001790: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000017a0: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
-000017b0: 2027 e590 8de5 b888 e68c 87e5 afbc e689   '..............
-000017c0: 98e7 a68f e8af ade6 b395 e68a 80e5 b7a7  ................
-000017d0: efbc 9ae5 908d e8af 8de7 9a84 e5a4 8de6  ................
-000017e0: 95b0 e5bd a2e5 bc8f 2729 2c0a 2020 2020  ........'),.    
-000017f0: 2020 2020 2020 2020 2020 2020 2827 6564              ('ed
-00001800: 7563 6174 696f 6e27 2c20 27e4 b8ad e59b  ucation', '.....
-00001810: bde9 ab98 e880 83e6 8890 e7bb a9e6 b5b7  ................
-00001820: e5a4 96e8 aea4 e58f af20 e698 afe2 809c  ......... ......
-00001830: e78b bce6 9da5 e4ba 86e2 809d e590 97ef  ................
-00001840: bc9f 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00001850: 2020 2020 2020 2827 6564 7563 6174 696f        ('educatio
-00001860: 6e27 2c20 27e5 85ac e58a a1e5 9198 e880  n', '...........
-00001870: 83e8 9991 e8b6 8ae6 9da5 e8b6 8ae5 9083  ................
-00001880: e9a6 99ef bc8c e8bf 99e6 98af e680 8ee4  ................
-00001890: b988 e59b 9ee4 ba8b efbc 9f27 292c 0a20  ...........'),. 
-000018a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000018b0: 2773 706f 7274 7327 2c20 27e5 9bbe e696  'sports', '.....
-000018c0: 87ef bc9a e6b3 95e7 bd91 e5ad 9fe8 8fb2  ................
-000018d0: e5b0 94e6 96af e88b a6e6 8898 e8bf 9b31  ...............1
-000018e0: 36e5 bcba 20e5 ad9f e88f b2e5 b094 e696  6... ...........
-000018f0: afe6 8092 e590 bc27 292c 0a20 2020 2020  .......'),.     
-00001900: 2020 2020 2020 2020 2020 2028 2773 706f             ('spo
-00001910: 7274 7327 2c20 27e5 9b9b e5b7 9de4 b8b9  rts', '.........
-00001920: e6a3 b1e4 b8be e8a1 8ce5 85a8 e59b bde9  ................
-00001930: 95bf e8b7 9de7 99bb e5b1 b1e6 8c91 e688  ................
-00001940: 98e8 b59b 20e8 bf91 e4b8 87e4 baba e58f  .... ...........
-00001950: 82e4 b88e 2729 2c0a 2020 2020 2020 2020  ....'),.        
-00001960: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
-00001970: 272c 2027 e7b1 b3e5 85b0 e5ae a2e5 9cba  ', '............
-00001980: 38e6 8898 e4b8 8de8 b4a5 e59b bde7 b1b3  8...............
-00001990: 3130 e5b9 b4e8 bf9e e883 9c27 292c 0a20  10.........'),. 
-000019a0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-000019b0: 2020 2020 2020 2020 206d 2e74 7261 696e           m.train
-000019c0: 2864 6174 6129 0a20 2020 2020 2020 2020  (data).         
-000019d0: 2020 2070 7269 6e74 286d 290a 2020 2020     print(m).    
-000019e0: 2020 2020 2020 2020 2320 6c6f 6164 2062          # load b
-000019f0: 6573 7420 6d6f 6465 6c20 6672 6f6d 206d  est model from m
-00001a00: 6f64 656c 5f64 6972 0a20 2020 2020 2020  odel_dir.       
-00001a10: 2020 2020 206d 2e6c 6f61 645f 6d6f 6465       m.load_mode
-00001a20: 6c28 290a 2020 2020 2020 2020 2020 2020  l().            
-00001a30: 7072 6564 6963 745f 6c61 6265 6c2c 2070  predict_label, p
-00001a40: 7265 6469 6374 5f70 726f 6261 203d 206d  redict_proba = m
-00001a50: 2e70 7265 6469 6374 285b 27e7 a68f e5bb  .predict(['.....
-00001a60: bae6 98a5 e5ad a3e5 85ac e58a a1e5 9198  ................
-00001a70: e880 83e8 af95 e68a a5e5 908d 3138 e697  ............18..
-00001a80: a5e6 88aa e6ad a220 32e6 9c88 36e6 97a5  ....... 2...6...
-00001a90: e880 83e8 af95 272c 0a20 2020 2020 2020  ......',.       
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ac0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001ad0: e684 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8  ................
-00001ae0: b59b e4ba a4e6 8898 e8ae b0e5 bd95 3ae7  ..............:.
-00001af0: b1b3 e585 b0e5 aea2 e59c ba38 e688 98e4  ...........8....
-00001b00: b88d e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4  ...........10...
-00001b10: e8bf 9ee8 839c 275d 290a 2020 2020 2020  ......']).      
-00001b20: 2020 2020 2020 7072 696e 7428 6627 7072        print(f'pr
-00001b30: 6564 6963 745f 6c61 6265 6c3a 207b 7072  edict_label: {pr
-00001b40: 6564 6963 745f 6c61 6265 6c7d 2c20 7072  edict_label}, pr
-00001b50: 6564 6963 745f 7072 6f62 613a 207b 7072  edict_proba: {pr
-00001b60: 6564 6963 745f 7072 6f62 617d 2729 0a20  edict_proba}'). 
-00001b70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001b80: 2020 2020 7465 7374 5f64 6174 6120 3d20      test_data = 
-00001b90: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00001ba0: 2020 2827 6564 7563 6174 696f 6e27 2c20    ('education', 
-00001bb0: 27e7 a68f e5bb bae6 98a5 e5ad a3e5 85ac  '...............
-00001bc0: e58a a1e5 9198 e880 83e8 af95 e68a a5e5  ................
-00001bd0: 908d 3138 e697 a5e6 88aa e6ad a220 32e6  ..18......... 2.
-00001be0: 9c88 36e6 97a5 e880 83e8 af95 2729 2c0a  ..6.........'),.
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2827 7370 6f72 7473 272c 2027 e684 8fe7  ('sports', '....
-00001c10: 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b e4ba  ................
-00001c20: a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3 e585  ..........:.....
-00001c30: b0e5 aea2 e59c ba38 e688 98e4 b88d e8b4  .......8........
-00001c40: a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8  .......10.......
-00001c50: 839c 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
-00001c60: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-00001c70: 6163 635f 7363 6f72 6520 3d20 6d2e 6576  acc_score = m.ev
-00001c80: 616c 7561 7465 5f6d 6f64 656c 2874 6573  aluate_model(tes
-00001c90: 745f 6461 7461 290a 2020 2020 2020 2020  t_data).        
-00001ca0: 2020 2020 7072 696e 7428 6627 6163 635f      print(f'acc_
-00001cb0: 7363 6f72 653a 207b 6163 635f 7363 6f72  score: {acc_scor
-00001cc0: 657d 2729 2020 2320 312e 300a 2020 2020  e}')  # 1.0.    
-00001cd0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00001ce0: 2023 2323 2320 7472 6169 6e20 6d6f 6465   #### train mode
-00001cf0: 6c20 7769 7468 2031 7720 6461 7461 0a20  l with 1w data. 
-00001d00: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00001d10: 2827 2d27 202a 2034 3229 0a20 2020 2020  ('-' * 42).     
-00001d20: 2020 2020 2020 206d 203d 2043 6c61 7373         m = Class
-00001d30: 6963 436c 6173 7369 6669 6572 286d 6f64  icClassifier(mod
-00001d40: 656c 5f64 6972 3d27 6d6f 6465 6c73 2f6c  el_dir='models/l
-00001d50: 7227 2c20 6d6f 6465 6c5f 6e61 6d65 5f6f  r', model_name_o
-00001d60: 725f 6d6f 6465 6c3d 276c 7227 290a 2020  r_model='lr').  
-00001d70: 2020 2020 2020 2020 2020 6461 7461 5f66            data_f
-00001d80: 696c 6520 3d20 2774 6875 636e 6577 735f  ile = 'thucnews_
-00001d90: 7472 6169 6e5f 3177 2e74 7874 270a 2020  train_1w.txt'.  
-00001da0: 2020 2020 2020 2020 2020 6d2e 7472 6169            m.trai
-00001db0: 6e28 6461 7461 5f66 696c 6529 0a20 2020  n(data_file).   
-00001dc0: 2020 2020 2020 2020 206d 2e6c 6f61 645f           m.load_
-00001dd0: 6d6f 6465 6c28 290a 2020 2020 2020 2020  model().        
-00001de0: 2020 2020 7072 6564 6963 745f 6c61 6265      predict_labe
-00001df0: 6c2c 2070 7265 6469 6374 5f70 726f 6261  l, predict_proba
-00001e00: 203d 206d 2e70 7265 6469 6374 280a 2020   = m.predict(.  
-00001e10: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
-00001e20: e9a1 bae4 b989 e58c 97e4 baac e88b 8fe6  ................
-00001e30: b4bb 3838 e5b9 b3e7 b1b3 e8b5 b7e7 b2be  ..88............
-00001e40: e8a3 85e6 88bf e59c a8e5 94ae 272c 0a20  ............',. 
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e60: 27e7 be8e 4542 2d35 e9a1 b9e7 9bae e280  '...EB-5........
-00001e70: 9c31 35e6 97a5 e5bf abe9 809f e7a7 bbe6  .15.............
-00001e80: b091 e280 9de5 b086 e68e a8e8 bf9f 275d  ..............']
-00001e90: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00001ea0: 696e 7428 6627 7072 6564 6963 745f 6c61  int(f'predict_la
-00001eb0: 6265 6c3a 207b 7072 6564 6963 745f 6c61  bel: {predict_la
-00001ec0: 6265 6c7d 2c20 7072 6564 6963 745f 7072  bel}, predict_pr
-00001ed0: 6f62 613a 207b 7072 6564 6963 745f 7072  oba: {predict_pr
-00001ee0: 6f62 617d 2729 0a20 2020 2020 2020 2060  oba}').        `
-00001ef0: 6060 0a20 2020 2020 2020 200a 2020 2020  ``.        .    
-00001f00: 2020 2020 6f75 7470 7574 3a0a 2020 2020      output:.    
-00001f10: 2020 2020 0a20 2020 2020 2020 2060 6060      .        ```
-00001f20: 0a20 2020 2020 2020 2043 6c61 7373 6963  .        Classic
-00001f30: 436c 6173 7369 6669 6572 2069 6e73 7461  Classifier insta
-00001f40: 6e63 6520 284c 6f67 6973 7469 6352 6567  nce (LogisticReg
-00001f50: 7265 7373 696f 6e28 6669 745f 696e 7465  ression(fit_inte
-00001f60: 7263 6570 743d 4661 6c73 6529 2c20 7374  rcept=False), st
-00001f70: 6f70 776f 7264 7320 7369 7a65 3a20 3234  opwords size: 24
-00001f80: 3338 290a 2020 2020 2020 2020 7072 6564  38).        pred
-00001f90: 6963 745f 6c61 6265 6c3a 205b 2765 6475  ict_label: ['edu
-00001fa0: 6361 7469 6f6e 2720 2773 706f 7274 7327  cation' 'sports'
-00001fb0: 5d2c 2070 7265 6469 6374 5f70 726f 6261  ], predict_proba
-00001fc0: 3a20 5b30 2e35 2c20 302e 3539 3839 3431  : [0.5, 0.598941
-00001fd0: 3830 3637 3431 3533 345d 0a20 2020 2020  806741534].     
-00001fe0: 2020 2061 6363 5f73 636f 7265 3a20 312e     acc_score: 1.
-00001ff0: 300a 2020 2020 2020 2020 2d2d 2d2d 2d2d  0.        ------
-00002000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002020: 2d2d 2d2d 0a20 2020 2020 2020 2070 7265  ----.        pre
-00002030: 6469 6374 5f6c 6162 656c 3a20 5b27 7265  dict_label: ['re
-00002040: 616c 7479 2720 2765 6475 6361 7469 6f6e  alty' 'education
-00002050: 275d 2c20 7072 6564 6963 745f 7072 6f62  '], predict_prob
-00002060: 613a 205b 302e 3733 3032 3935 3639 3233  a: [0.7302956923
-00002070: 3631 3733 3732 2c20 302e 3235 3635 3030  617372, 0.256500
-00002080: 3534 3435 3332 3239 3233 5d0a 2020 2020  5445322923].    
-00002090: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-000020a0: 0a20 2020 2020 2020 2023 2320 5669 7375  .        ## Visu
-000020b0: 616c 2046 6561 7475 7265 2049 6d70 6f72  al Feature Impor
-000020c0: 7461 6e63 650a 2020 2020 2020 2020 0a20  tance.        . 
-000020d0: 2020 2020 2020 2053 686f 7720 6665 6174         Show feat
-000020e0: 7572 6520 7765 6967 6874 7320 6f66 206d  ure weights of m
-000020f0: 6f64 656c 2c20 616e 6420 7072 6564 6963  odel, and predic
-00002100: 7469 6f6e 2077 6f72 6420 7765 6967 6874  tion word weight
-00002110: 2c20 666f 7220 6578 616d 706c 6520 5b65  , for example [e
-00002120: 7861 6d70 6c65 732f 7669 7375 616c 5f66  xamples/visual_f
-00002130: 6561 7475 7265 5f69 6d70 6f72 7461 6e63  eature_importanc
-00002140: 652e 6970 796e 625d 2865 7861 6d70 6c65  e.ipynb](example
-00002150: 732f 7669 7375 616c 5f66 6561 7475 7265  s/visual_feature
-00002160: 5f69 6d70 6f72 7461 6e63 652e 6970 796e  _importance.ipyn
-00002170: 6229 0a20 2020 2020 2020 2060 6060 7079  b).        ```py
-00002180: 7468 6f6e 0a20 2020 2020 2020 2069 6d70  thon.        imp
-00002190: 6f72 7420 7379 730a 2020 2020 2020 2020  ort sys.        
-000021a0: 0a20 2020 2020 2020 2073 7973 2e70 6174  .        sys.pat
-000021b0: 682e 6170 7065 6e64 2827 2e2e 2729 0a20  h.append('..'). 
-000021c0: 2020 2020 2020 2066 726f 6d20 7079 7465         from pyte
-000021d0: 7874 636c 6173 7369 6669 6572 2069 6d70  xtclassifier imp
-000021e0: 6f72 7420 436c 6173 7369 6343 6c61 7373  ort ClassicClass
-000021f0: 6966 6965 720a 2020 2020 2020 2020 696d  ifier.        im
-00002200: 706f 7274 206a 6965 6261 0a20 2020 2020  port jieba.     
-00002210: 2020 200a 2020 2020 2020 2020 7463 203d     .        tc =
-00002220: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
-00002230: 6572 286d 6f64 656c 5f64 6972 3d27 6d6f  er(model_dir='mo
-00002240: 6465 6c73 2f6c 722d 746f 7927 2c20 6d6f  dels/lr-toy', mo
-00002250: 6465 6c5f 6e61 6d65 5f6f 725f 6d6f 6465  del_name_or_mode
-00002260: 6c3d 276c 7227 290a 2020 2020 2020 2020  l='lr').        
-00002270: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00002280: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
-00002290: 272c 2027 e590 8de5 b888 e68c 87e5 afbc  ', '............
-000022a0: e689 98e7 a68f e8af ade6 b395 e68a 80e5  ................
-000022b0: b7a7 efbc 9ae5 908d e8af 8de7 9a84 e5a4  ................
-000022c0: 8de6 95b0 e5bd a2e5 bc8f 2729 2c0a 2020  ..........'),.  
-000022d0: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
-000022e0: 6174 696f 6e27 2c20 27e4 b8ad e59b bde9  ation', '.......
-000022f0: ab98 e880 83e6 8890 e7bb a9e6 b5b7 e5a4  ................
-00002300: 96e8 aea4 e58f af20 e698 afe2 809c e78b  ....... ........
-00002310: bce6 9da5 e4ba 86e2 809d e590 97ef bc9f  ................
-00002320: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00002330: 2827 7370 6f72 7473 272c 2027 e59b bee6  ('sports', '....
-00002340: 9687 efbc 9ae6 b395 e7bd 91e5 ad9f e88f  ................
-00002350: b2e5 b094 e696 afe8 8ba6 e688 98e8 bf9b  ................
-00002360: 3136 e5bc ba20 e5ad 9fe8 8fb2 e5b0 94e6  16... ..........
-00002370: 96af e680 92e5 90bc 2729 2c0a 2020 2020  ........'),.    
-00002380: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
-00002390: 272c 2027 e59b 9be5 b79d e4b8 b9e6 a3b1  ', '............
-000023a0: e4b8 bee8 a18c e585 a8e5 9bbd e995 bfe8  ................
-000023b0: b79d e799 bbe5 b1b1 e68c 91e6 8898 e8b5  ................
-000023c0: 9b20 e8bf 91e4 b887 e4ba bae5 8f82 e4b8  . ..............
-000023d0: 8e27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
-000023e0: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
-000023f0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
-00002400: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
-00002410: 9ee8 839c 2729 0a20 2020 2020 2020 205d  ....').        ]
-00002420: 0a20 2020 2020 2020 2074 632e 7472 6169  .        tc.trai
-00002430: 6e28 6461 7461 290a 2020 2020 2020 2020  n(data).        
-00002440: 696d 706f 7274 2065 6c69 350a 2020 2020  import eli5.    
-00002450: 2020 2020 696e 6665 725f 6461 7461 203d      infer_data =
-00002460: 205b 27e9 ab98 e880 83e6 8c87 e5af bce6   ['.............
-00002470: 8998 e7a6 8fe8 afad e6b3 95e6 8a80 e5b7  ................
-00002480: a7e5 9bbd e999 85e8 aea4 e58f af27 2c0a  .............',.
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2020 27e6 848f e794 b2e9 a696        '.........
-000024b0: e8bd aee8 a1a5 e8b5 9be4 baa4 e688 98e8  ................
-000024c0: aeb0 e5bd 953a e7b1 b3e5 85b0 e5ae a2e5  .....:..........
-000024d0: 9cba 38e6 8898 e4b8 8de8 b4a5 e59b bde7  ..8.............
-000024e0: b1b3 3130 e5b9 b4e8 bf9e e883 9c27 5d0a  ..10.........'].
-000024f0: 2020 2020 2020 2020 656c 6935 2e73 686f          eli5.sho
-00002500: 775f 7765 6967 6874 7328 7463 2e6d 6f64  w_weights(tc.mod
-00002510: 656c 2c20 7665 633d 7463 2e66 6561 7475  el, vec=tc.featu
-00002520: 7265 290a 2020 2020 2020 2020 7365 675f  re).        seg_
-00002530: 696e 6665 725f 6461 7461 203d 205b 2720  infer_data = [' 
-00002540: 272e 6a6f 696e 286a 6965 6261 2e6c 6375  '.join(jieba.lcu
-00002550: 7428 6929 2920 666f 7220 6920 696e 2069  t(i)) for i in i
-00002560: 6e66 6572 5f64 6174 615d 0a20 2020 2020  nfer_data].     
-00002570: 2020 2065 6c69 352e 7368 6f77 5f70 7265     eli5.show_pre
-00002580: 6469 6374 696f 6e28 7463 2e6d 6f64 656c  diction(tc.model
-00002590: 2c20 7365 675f 696e 6665 725f 6461 7461  , seg_infer_data
-000025a0: 5b30 5d2c 2076 6563 3d74 632e 6665 6174  [0], vec=tc.feat
-000025b0: 7572 652c 0a20 2020 2020 2020 2020 2020  ure,.           
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 2020 7461 7267 6574 5f6e 616d 6573 3d5b    target_names=[
-000025e0: 2765 6475 6361 7469 6f6e 272c 2027 7370  'education', 'sp
-000025f0: 6f72 7473 275d 290a 2020 2020 2020 2020  orts']).        
-00002600: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00002610: 2020 2020 206f 7574 7075 743a 0a20 2020       output:.   
-00002620: 2020 2020 200a 2020 2020 2020 2020 215b       .        ![
-00002630: 696d 672e 706e 675d 2864 6f63 732f 696d  img.png](docs/im
-00002640: 672e 706e 6729 0a20 2020 2020 2020 200a  g.png).        .
-00002650: 2020 2020 2020 2020 2323 2044 6565 7020          ## Deep 
-00002660: 436c 6173 7369 6669 6361 7469 6f6e 206d  Classification m
-00002670: 6f64 656c 0a20 2020 2020 2020 200a 2020  odel.        .  
-00002680: 2020 2020 2020 e69c ace9 a1b9 e79b aee6        ..........
-00002690: 94af e68c 81e4 bba5 e4b8 8be6 b7b1 e5ba  ................
-000026a0: a6e5 8886 e7b1 bbe6 a8a1 e59e 8bef bc9a  ................
-000026b0: 4661 7374 5465 7874 e380 8154 6578 7443  FastText...TextC
-000026c0: 4e4e e380 8154 6578 7452 4e4e e380 8142  NN...TextRNN...B
-000026d0: 6572 74e6 a8a1 e59e 8bef bc8c 6069 6d70  ert.........`imp
-000026e0: 6f72 7460 e6a8 a1e5 9e8b e5af b9e5 ba94  ort`............
-000026f0: e79a 84e6 96b9 e6b3 95e6 9da5 e8b0 83e7  ................
-00002700: 94a8 efbc 9a0a 2020 2020 2020 2020 6060  ......        ``
-00002710: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-00002720: 6672 6f6d 2070 7974 6578 7463 6c61 7373  from pytextclass
-00002730: 6966 6965 7220 696d 706f 7274 2046 6173  ifier import Fas
-00002740: 7454 6578 7443 6c61 7373 6966 6965 722c  tTextClassifier,
-00002750: 2054 6578 7443 4e4e 436c 6173 7369 6669   TextCNNClassifi
-00002760: 6572 2c20 5465 7874 524e 4e43 6c61 7373  er, TextRNNClass
-00002770: 6966 6965 722c 2042 6572 7443 6c61 7373  ifier, BertClass
-00002780: 6966 6965 720a 2020 2020 2020 2020 6060  ifier.        ``
-00002790: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
-000027a0: 2020 20e4 b88b e99d a2e4 bba5 4661 7374     .........Fast
-000027b0: 5465 7874 e6a8 a1e5 9e8b e4b8 bae7 a4ba  Text............
-000027c0: e4be 8bef bc8c e585 b6e4 bb96 e6a8 a1e5  ................
-000027d0: 9e8b e79a 84e4 bdbf e794 a8e6 96b9 e6b3  ................
-000027e0: 95e7 b1bb e4bc bce3 8082 0a20 2020 2020  ...........     
-000027f0: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
-00002800: 4661 7374 5465 7874 20e6 a8a1 e59e 8b0a  FastText .......
-00002810: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002820: 20e8 aead e7bb 83e5 928c e9a2 84e6 b58b   ...............
-00002830: 6046 6173 7454 6578 7460 e6a8 a1e5 9e8b  `FastText`......
-00002840: e7a4 bae4 be8b 5b65 7861 6d70 6c65 732f  ......[examples/
-00002850: 6661 7374 7465 7874 5f63 6c61 7373 6966  fasttext_classif
-00002860: 6963 6174 696f 6e5f 6465 6d6f 2e70 795d  ication_demo.py]
-00002870: 2865 7861 6d70 6c65 732f 6661 7374 7465  (examples/fastte
-00002880: 7874 5f63 6c61 7373 6966 6963 6174 696f  xt_classificatio
-00002890: 6e5f 6465 6d6f 2e70 7929 0a20 2020 2020  n_demo.py).     
-000028a0: 2020 200a 2020 2020 2020 2020 6060 6070     .        ```p
-000028b0: 7974 686f 6e0a 2020 2020 2020 2020 696d  ython.        im
-000028c0: 706f 7274 2073 7973 0a20 2020 2020 2020  port sys.       
-000028d0: 200a 2020 2020 2020 2020 7379 732e 7061   .        sys.pa
-000028e0: 7468 2e61 7070 656e 6428 272e 2e27 290a  th.append('..').
-000028f0: 2020 2020 2020 2020 6672 6f6d 2070 7974          from pyt
-00002900: 6578 7463 6c61 7373 6966 6965 7220 696d  extclassifier im
-00002910: 706f 7274 2046 6173 7454 6578 7443 6c61  port FastTextCla
-00002920: 7373 6966 6965 722c 206c 6f61 645f 6461  ssifier, load_da
-00002930: 7461 0a20 2020 2020 2020 200a 2020 2020  ta.        .    
-00002940: 2020 2020 6966 205f 5f6e 616d 655f 5f20      if __name__ 
-00002950: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
-00002960: 2020 2020 2020 2020 2020 206d 203d 2046             m = F
-00002970: 6173 7454 6578 7443 6c61 7373 6966 6965  astTextClassifie
-00002980: 7228 6d6f 6465 6c5f 6469 723d 276d 6f64  r(model_dir='mod
-00002990: 656c 732f 6661 7374 7465 7874 2d74 6f79  els/fasttext-toy
-000029a0: 2729 0a20 2020 2020 2020 2020 2020 2064  ').            d
-000029b0: 6174 6120 3d20 5b0a 2020 2020 2020 2020  ata = [.        
-000029c0: 2020 2020 2020 2020 2827 6564 7563 6174          ('educat
-000029d0: 696f 6e27 2c20 27e5 908d e5b8 88e6 8c87  ion', '.........
-000029e0: e5af bce6 8998 e7a6 8fe8 afad e6b3 95e6  ................
-000029f0: 8a80 e5b7 a7ef bc9a e590 8de8 af8d e79a  ................
-00002a00: 84e5 a48d e695 b0e5 bda2 e5bc 8f27 292c  .............'),
-00002a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a20: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
-00002a30: e4b8 ade5 9bbd e9ab 98e8 8083 e688 90e7  ................
-00002a40: bba9 e6b5 b7e5 a496 e8ae a4e5 8faf 20e6  .............. .
-00002a50: 98af e280 9ce7 8bbc e69d a5e4 ba86 e280  ................
-00002a60: 9de5 9097 efbc 9f27 292c 0a20 2020 2020  .......'),.     
-00002a70: 2020 2020 2020 2020 2020 2028 2765 6475             ('edu
-00002a80: 6361 7469 6f6e 272c 2027 e585 ace5 8aa1  cation', '......
-00002a90: e591 98e8 8083 e899 91e8 b68a e69d a5e8  ................
-00002aa0: b68a e590 83e9 a699 efbc 8ce8 bf99 e698  ................
-00002ab0: afe6 808e e4b9 88e5 9b9e e4ba 8bef bc9f  ................
-00002ac0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00002ad0: 2020 2020 2827 7370 6f72 7473 272c 2027      ('sports', '
-00002ae0: e59b bee6 9687 efbc 9ae6 b395 e7bd 91e5  ................
-00002af0: ad9f e88f b2e5 b094 e696 afe8 8ba6 e688  ................
-00002b00: 98e8 bf9b 3136 e5bc ba20 e5ad 9fe8 8fb2  ....16... ......
-00002b10: e5b0 94e6 96af e680 92e5 90bc 2729 2c0a  ............'),.
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2827 7370 6f72 7473 272c 2027 e59b 9be5  ('sports', '....
-00002b40: b79d e4b8 b9e6 a3b1 e4b8 bee8 a18c e585  ................
-00002b50: a8e5 9bbd e995 bfe8 b79d e799 bbe5 b1b1  ................
-00002b60: e68c 91e6 8898 e8b5 9b20 e8bf 91e4 b887  ......... ......
-00002b70: e4ba bae5 8f82 e4b8 8e27 292c 0a20 2020  .........'),.   
-00002b80: 2020 2020 2020 2020 2020 2020 2028 2773               ('s
-00002b90: 706f 7274 7327 2c20 27e7 b1b3 e585 b0e5  ports', '.......
-00002ba0: aea2 e59c ba38 e688 98e4 b88d e8b4 a5e4  .....8..........
-00002bb0: bf9d e68c 81e8 bf9e e883 9c27 292c 0a20  ...........'),. 
-00002bc0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-00002bd0: 2020 2020 2020 2020 206d 2e74 7261 696e           m.train
-00002be0: 2864 6174 612c 206e 756d 5f65 706f 6368  (data, num_epoch
-00002bf0: 733d 3329 0a20 2020 2020 2020 2020 2020  s=3).           
-00002c00: 2070 7269 6e74 286d 290a 2020 2020 2020   print(m).      
-00002c10: 2020 2020 2020 2320 6c6f 6164 2074 7261        # load tra
-00002c20: 696e 6564 2062 6573 7420 6d6f 6465 6c0a  ined best model.
-00002c30: 2020 2020 2020 2020 2020 2020 6d2e 6c6f              m.lo
-00002c40: 6164 5f6d 6f64 656c 2829 0a20 2020 2020  ad_model().     
-00002c50: 2020 2020 2020 2070 7265 6469 6374 5f6c         predict_l
-00002c60: 6162 656c 2c20 7072 6564 6963 745f 7072  abel, predict_pr
-00002c70: 6f62 6120 3d20 6d2e 7072 6564 6963 7428  oba = m.predict(
-00002c80: 5b27 e7a6 8fe5 bbba e698 a5e5 ada3 e585  ['..............
-00002c90: ace5 8aa1 e591 98e8 8083 e8af 95e6 8aa5  ................
-00002ca0: e590 8d31 38e6 97a5 e688 aae6 ada2 2032  ...18......... 2
-00002cb0: e69c 8836 e697 a5e8 8083 e8af 9527 2c0a  ...6.........',.
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cf0: 2020 2020 2020 27e6 848f e794 b2e9 a696        '.........
-00002d00: e8bd aee8 a1a5 e8b5 9be4 baa4 e688 98e8  ................
-00002d10: aeb0 e5bd 953a e7b1 b3e5 85b0 e5ae a2e5  .....:..........
-00002d20: 9cba 38e6 8898 e4b8 8de8 b4a5 e59b bde7  ..8.............
-00002d30: b1b3 3130 e5b9 b4e8 bf9e e883 9c27 5d29  ..10.........'])
-00002d40: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00002d50: 6e74 2866 2770 7265 6469 6374 5f6c 6162  nt(f'predict_lab
-00002d60: 656c 3a20 7b70 7265 6469 6374 5f6c 6162  el: {predict_lab
-00002d70: 656c 7d2c 2070 7265 6469 6374 5f70 726f  el}, predict_pro
-00002d80: 6261 3a20 7b70 7265 6469 6374 5f70 726f  ba: {predict_pro
-00002d90: 6261 7d27 290a 2020 2020 2020 2020 2020  ba}').          
-00002da0: 2020 7465 7374 5f64 6174 6120 3d20 5b0a    test_data = [.
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2827 6564 7563 6174 696f 6e27 2c20 27e7  ('education', '.
-00002dd0: a68f e5bb bae6 98a5 e5ad a3e5 85ac e58a  ................
-00002de0: a1e5 9198 e880 83e8 af95 e68a a5e5 908d  ................
-00002df0: 3138 e697 a5e6 88aa e6ad a220 32e6 9c88  18......... 2...
-00002e00: 36e6 97a5 e880 83e8 af95 2729 2c0a 2020  6.........'),.  
-00002e10: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00002e20: 7370 6f72 7473 272c 2027 e684 8fe7 94b2  sports', '......
-00002e30: e9a6 96e8 bdae e8a1 a5e8 b59b e4ba a4e6  ................
-00002e40: 8898 e8ae b0e5 bd95 3ae7 b1b3 e585 b0e5  ........:.......
-00002e50: aea2 e59c ba38 e688 98e4 b88d e8b4 a5e5  .....8..........
-00002e60: 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8 839c  .....10.........
-00002e70: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00002e80: 5d0a 2020 2020 2020 2020 2020 2020 6163  ].            ac
-00002e90: 635f 7363 6f72 6520 3d20 6d2e 6576 616c  c_score = m.eval
-00002ea0: 7561 7465 5f6d 6f64 656c 2874 6573 745f  uate_model(test_
-00002eb0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00002ec0: 2020 7072 696e 7428 6627 6163 635f 7363    print(f'acc_sc
-00002ed0: 6f72 653a 207b 6163 635f 7363 6f72 657d  ore: {acc_score}
-00002ee0: 2729 2020 2320 312e 300a 2020 2020 2020  ')  # 1.0.      
-00002ef0: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
-00002f00: 2323 2320 7472 6169 6e20 6d6f 6465 6c20  ### train model 
-00002f10: 7769 7468 2031 7720 6461 7461 0a20 2020  with 1w data.   
-00002f20: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
-00002f30: 2d27 202a 2034 3229 0a20 2020 2020 2020  -' * 42).       
-00002f40: 2020 2020 2064 6174 615f 6669 6c65 203d       data_file =
-00002f50: 2027 7468 7563 6e65 7773 5f74 7261 696e   'thucnews_train
-00002f60: 5f31 772e 7478 7427 0a20 2020 2020 2020  _1w.txt'.       
-00002f70: 2020 2020 206d 203d 2046 6173 7454 6578       m = FastTex
-00002f80: 7443 6c61 7373 6966 6965 7228 6d6f 6465  tClassifier(mode
-00002f90: 6c5f 6469 723d 276d 6f64 656c 732f 6661  l_dir='models/fa
-00002fa0: 7374 7465 7874 2729 0a20 2020 2020 2020  sttext').       
-00002fb0: 2020 2020 206d 2e74 7261 696e 2864 6174       m.train(dat
-00002fc0: 615f 6669 6c65 2c20 6e61 6d65 733d 2827  a_file, names=('
-00002fd0: 6c61 6265 6c73 272c 2027 7465 7874 2729  labels', 'text')
-00002fe0: 2c20 6e75 6d5f 6570 6f63 6873 3d33 290a  , num_epochs=3).
-00002ff0: 2020 2020 2020 2020 2020 2020 2320 6c6f              # lo
-00003000: 6164 2062 6573 7420 7472 6169 6e65 6420  ad best trained 
-00003010: 6d6f 6465 6c20 6672 6f6d 206d 6f64 656c  model from model
-00003020: 5f64 6972 0a20 2020 2020 2020 2020 2020  _dir.           
-00003030: 206d 2e6c 6f61 645f 6d6f 6465 6c28 290a   m.load_model().
-00003040: 2020 2020 2020 2020 2020 2020 7072 6564              pred
-00003050: 6963 745f 6c61 6265 6c2c 2070 7265 6469  ict_label, predi
-00003060: 6374 5f70 726f 6261 203d 206d 2e70 7265  ct_proba = m.pre
-00003070: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-00003080: 2020 2020 2020 5b27 e9a1 bae4 b989 e58c        ['........
-00003090: 97e4 baac e88b 8fe6 b4bb 3838 e5b9 b3e7  ..........88....
-000030a0: b1b3 e8b5 b7e7 b2be e8a3 85e6 88bf e59c  ................
-000030b0: a8e5 94ae 272c 0a20 2020 2020 2020 2020  ....',.         
-000030c0: 2020 2020 2020 2020 27e7 be8e 4542 2d35          '...EB-5
-000030d0: e9a1 b9e7 9bae e280 9c31 35e6 97a5 e5bf  .........15.....
-000030e0: abe9 809f e7a7 bbe6 b091 e280 9de5 b086  ................
-000030f0: e68e a8e8 bf9f 275d 0a20 2020 2020 2020  ......'].       
-00003100: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00003110: 2020 2070 7269 6e74 2866 2770 7265 6469     print(f'predi
-00003120: 6374 5f6c 6162 656c 3a20 7b70 7265 6469  ct_label: {predi
-00003130: 6374 5f6c 6162 656c 7d2c 2070 7265 6469  ct_label}, predi
-00003140: 6374 5f70 726f 6261 3a20 7b70 7265 6469  ct_proba: {predi
-00003150: 6374 5f70 726f 6261 7d27 290a 2020 2020  ct_proba}').    
-00003160: 2020 2020 2020 2020 782c 2079 2c20 6466          x, y, df
-00003170: 203d 206c 6f61 645f 6461 7461 2864 6174   = load_data(dat
-00003180: 615f 6669 6c65 290a 2020 2020 2020 2020  a_file).        
-00003190: 2020 2020 7465 7374 5f64 6174 6120 3d20      test_data = 
-000031a0: 6466 5b3a 3130 305d 0a20 2020 2020 2020  df[:100].       
-000031b0: 2020 2020 2061 6363 5f73 636f 7265 203d       acc_score =
-000031c0: 206d 2e65 7661 6c75 6174 655f 6d6f 6465   m.evaluate_mode
-000031d0: 6c28 7465 7374 5f64 6174 6129 0a20 2020  l(test_data).   
-000031e0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-000031f0: 2761 6363 5f73 636f 7265 3a20 7b61 6363  'acc_score: {acc
-00003200: 5f73 636f 7265 7d27 290a 2020 2020 2020  _score}').      
-00003210: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
-00003220: 2020 2020 2020 2023 2323 2042 4552 5420         ### BERT 
-00003230: e7b1 bbe6 a8a1 e59e 8b0a 2020 2020 2020  ..........      
-00003240: 2020 0a20 2020 2020 2020 2023 2323 2320    .        #### 
-00003250: e5a4 9ae5 8886 e7b1 bbe6 a8a1 e59e 8b0a  ................
-00003260: 2020 2020 2020 2020 e8ae ade7 bb83 e592          ........
-00003270: 8ce9 a284 e6b5 8b60 4245 5254 60e5 a49a  .......`BERT`...
-00003280: e588 86e7 b1bb e6a8 a1e5 9e8b efbc 8ce7  ................
-00003290: a4ba e4be 8b5b 6578 616d 706c 6573 2f62  .....[examples/b
-000032a0: 6572 745f 636c 6173 7369 6669 6361 7469  ert_classificati
-000032b0: 6f6e 5f7a 685f 6465 6d6f 2e70 795d 2865  on_zh_demo.py](e
-000032c0: 7861 6d70 6c65 732f 6265 7274 5f63 6c61  xamples/bert_cla
-000032d0: 7373 6966 6963 6174 696f 6e5f 7a68 5f64  ssification_zh_d
-000032e0: 656d 6f2e 7079 290a 2020 2020 2020 2020  emo.py).        
-000032f0: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
-00003300: 6f6e 0a20 2020 2020 2020 2069 6d70 6f72  on.        impor
-00003310: 7420 7379 730a 2020 2020 2020 2020 0a20  t sys.        . 
-00003320: 2020 2020 2020 2073 7973 2e70 6174 682e         sys.path.
-00003330: 6170 7065 6e64 2827 2e2e 2729 0a20 2020  append('..').   
-00003340: 2020 2020 2066 726f 6d20 7079 7465 7874       from pytext
-00003350: 636c 6173 7369 6669 6572 2069 6d70 6f72  classifier impor
-00003360: 7420 4265 7274 436c 6173 7369 6669 6572  t BertClassifier
-00003370: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003380: 2020 6966 205f 5f6e 616d 655f 5f20 3d3d    if __name__ ==
-00003390: 2027 5f5f 6d61 696e 5f5f 273a 0a20 2020   '__main__':.   
-000033a0: 2020 2020 2020 2020 206d 203d 2042 6572           m = Ber
-000033b0: 7443 6c61 7373 6966 6965 7228 6d6f 6465  tClassifier(mode
-000033c0: 6c5f 6469 723d 276d 6f64 656c 732f 6265  l_dir='models/be
-000033d0: 7274 2d63 6869 6e65 7365 2d74 6f79 272c  rt-chinese-toy',
-000033e0: 206e 756d 5f63 6c61 7373 6573 3d32 2c0a   num_classes=2,.
-000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003400: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00003410: 6f64 656c 5f74 7970 653d 2762 6572 7427  odel_type='bert'
-00003420: 2c20 6d6f 6465 6c5f 6e61 6d65 3d27 6265  , model_name='be
-00003430: 7274 2d62 6173 652d 6368 696e 6573 6527  rt-base-chinese'
-00003440: 2c20 6e75 6d5f 6570 6f63 6873 3d32 290a  , num_epochs=2).
-00003450: 2020 2020 2020 2020 2020 2020 2320 6d6f              # mo
-00003460: 6465 6c5f 7479 7065 3a20 7375 7070 6f72  del_type: suppor
-00003470: 7420 2762 6572 7427 2c20 2761 6c62 6572  t 'bert', 'alber
-00003480: 7427 2c20 2772 6f62 6572 7461 272c 2027  t', 'roberta', '
-00003490: 786c 6e65 7427 0a20 2020 2020 2020 2020  xlnet'.         
-000034a0: 2020 2023 206d 6f64 656c 5f6e 616d 653a     # model_name:
-000034b0: 2073 7570 706f 7274 2027 6265 7274 2d62   support 'bert-b
-000034c0: 6173 652d 6368 696e 6573 6527 2c20 2762  ase-chinese', 'b
-000034d0: 6572 742d 6261 7365 2d63 6173 6564 272c  ert-base-cased',
-000034e0: 2027 6265 7274 2d62 6173 652d 6d75 6c74   'bert-base-mult
-000034f0: 696c 696e 6775 616c 2d63 6173 6564 2720  ilingual-cased' 
-00003500: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00003510: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00003520: 2020 2020 2020 2020 2028 2765 6475 6361           ('educa
-00003530: 7469 6f6e 272c 2027 e590 8de5 b888 e68c  tion', '........
-00003540: 87e5 afbc e689 98e7 a68f e8af ade6 b395  ................
-00003550: e68a 80e5 b7a7 efbc 9ae5 908d e8af 8de7  ................
-00003560: 9a84 e5a4 8de6 95b0 e5bd a2e5 bc8f 2729  ..............')
-00003570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003580: 2020 2827 6564 7563 6174 696f 6e27 2c20    ('education', 
-00003590: 27e4 b8ad e59b bde9 ab98 e880 83e6 8890  '...............
-000035a0: e7bb a9e6 b5b7 e5a4 96e8 aea4 e58f af20  ............... 
-000035b0: e698 afe2 809c e78b bce6 9da5 e4ba 86e2  ................
-000035c0: 809d e590 97ef bc9f 2729 2c0a 2020 2020  ........'),.    
-000035d0: 2020 2020 2020 2020 2020 2020 2827 6564              ('ed
-000035e0: 7563 6174 696f 6e27 2c20 27e5 85ac e58a  ucation', '.....
-000035f0: a1e5 9198 e880 83e8 9991 e8b6 8ae6 9da5  ................
-00003600: e8b6 8ae5 9083 e9a6 99ef bc8c e8bf 99e6  ................
-00003610: 98af e680 8ee4 b988 e59b 9ee4 ba8b efbc  ................
-00003620: 9f27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
-00003630: 2020 2020 2028 2773 706f 7274 7327 2c20       ('sports', 
-00003640: 27e5 9bbe e696 87ef bc9a e6b3 95e7 bd91  '...............
-00003650: e5ad 9fe8 8fb2 e5b0 94e6 96af e88b a6e6  ................
-00003660: 8898 e8bf 9b31 36e5 bcba 20e5 ad9f e88f  .....16... .....
-00003670: b2e5 b094 e696 afe6 8092 e590 bc27 292c  .............'),
+000000f0: 6e3a 203c 6469 7620 616c 6967 6e3d 2263  n: <div align="c
+00000100: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
+00000110: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000120: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+00000130: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
+00000140: 6c61 7373 6966 6965 7222 3e0a 2020 2020  lassifier">.    
+00000150: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+00000160: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000170: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
+00000180: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00000190: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
+000001a0: 732f 6c6f 676f 2e70 6e67 2220 616c 743d  s/logo.png" alt=
+000001b0: 224c 6f67 6f22 2068 6569 6768 743d 2231  "Logo" height="1
+000001c0: 3536 223e 0a20 2020 2020 2020 2020 203c  56">.          <
+000001d0: 2f61 3e0a 2020 2020 2020 2020 3c2f 6469  /a>.        </di
+000001e0: 763e 0a20 2020 2020 2020 200a 2020 2020  v>.        .    
+000001f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00000200: 2d2d 2d2d 2d0a 2020 2020 2020 2020 0a20  -----.        . 
+00000210: 2020 2020 2020 2023 2050 7954 6578 7443         # PyTextC
+00000220: 6c61 7373 6966 6965 723a 2050 7974 686f  lassifier: Pytho
+00000230: 6e20 5465 7874 2043 6c61 7373 6966 6965  n Text Classifie
+00000240: 720a 2020 2020 2020 2020 5b21 5b50 7950  r.        [![PyP
+00000250: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
+00000260: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+00000270: 2f70 792f 7079 7465 7874 636c 6173 7369  /py/pytextclassi
+00000280: 6669 6572 2e73 7667 295d 2868 7474 7073  fier.svg)](https
+00000290: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+000002a0: 2f70 792f 7079 7465 7874 636c 6173 7369  /py/pytextclassi
+000002b0: 6669 6572 290a 2020 2020 2020 2020 5b21  fier).        [!
+000002c0: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
+000002d0: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
+000002e0: 6467 652f 7079 7465 7874 636c 6173 7369  dge/pytextclassi
+000002f0: 6669 6572 295d 2868 7474 7073 3a2f 2f70  fier)](https://p
+00000300: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+00000310: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+00000320: 7229 0a20 2020 2020 2020 205b 215b 436f  r).        [![Co
+00000330: 6e74 7269 6275 7469 6f6e 7320 7765 6c63  ntributions welc
+00000340: 6f6d 655d 2868 7474 7073 3a2f 2f69 6d67  ome](https://img
+00000350: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000360: 652f 636f 6e74 7269 6275 7469 6f6e 732d  e/contributions-
+00000370: 7765 6c63 6f6d 652d 6272 6967 6874 6772  welcome-brightgr
+00000380: 6565 6e2e 7376 6729 5d28 434f 4e54 5249  een.svg)](CONTRI
+00000390: 4255 5449 4e47 2e6d 6429 0a20 2020 2020  BUTING.md).     
+000003a0: 2020 205b 215b 4769 7448 7562 2063 6f6e     [![GitHub con
+000003b0: 7472 6962 7574 6f72 735d 2868 7474 7073  tributors](https
+000003c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000003d0: 6f2f 6769 7468 7562 2f63 6f6e 7472 6962  o/github/contrib
+000003e0: 7574 6f72 732f 7368 6962 696e 6736 3234  utors/shibing624
+000003f0: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+00000400: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
+00000410: 6769 7468 7562 2e63 6f6d 2f73 6869 6269  github.com/shibi
+00000420: 6e67 3632 342f 7079 7465 7874 636c 6173  ng624/pytextclas
+00000430: 7369 6669 6572 2f67 7261 7068 732f 636f  sifier/graphs/co
+00000440: 6e74 7269 6275 746f 7273 290a 2020 2020  ntributors).    
+00000450: 2020 2020 5b21 5b4c 6963 656e 7365 2041      [![License A
+00000460: 7061 6368 6520 322e 305d 2868 7474 7073  pache 2.0](https
+00000470: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000480: 6f2f 6261 6467 652f 6c69 6365 6e73 652d  o/badge/license-
+00000490: 4170 6163 6865 2532 3032 2e30 2d62 6c75  Apache%202.0-blu
+000004a0: 652e 7376 6729 5d28 4c49 4345 4e53 4529  e.svg)](LICENSE)
+000004b0: 0a20 2020 2020 2020 205b 215b 7079 7468  .        [![pyth
+000004c0: 6f6e 5f76 6573 696f 6e5d 2868 7474 7073  on_vesion](https
+000004d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000004e0: 6f2f 6261 6467 652f 5079 7468 6f6e 2d33  o/badge/Python-3
+000004f0: 2e35 2532 422d 6772 6565 6e2e 7376 6729  .5%2B-green.svg)
+00000500: 5d28 7265 7175 6972 656d 656e 7473 2e74  ](requirements.t
+00000510: 7874 290a 2020 2020 2020 2020 5b21 5b47  xt).        [![G
+00000520: 6974 4875 6220 6973 7375 6573 5d28 6874  itHub issues](ht
+00000530: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000540: 732e 696f 2f67 6974 6875 622f 6973 7375  s.io/github/issu
+00000550: 6573 2f73 6869 6269 6e67 3632 342f 7079  es/shibing624/py
+00000560: 7465 7874 636c 6173 7369 6669 6572 2e73  textclassifier.s
+00000570: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000580: 6875 622e 636f 6d2f 7368 6962 696e 6736  hub.com/shibing6
+00000590: 3234 2f70 7974 6578 7463 6c61 7373 6966  24/pytextclassif
+000005a0: 6965 722f 6973 7375 6573 290a 2020 2020  ier/issues).    
+000005b0: 2020 2020 5b21 5b57 6563 6861 7420 4772      [![Wechat Gr
+000005c0: 6f75 705d 2868 7474 703a 2f2f 766c 6f67  oup](http://vlog
+000005d0: 2e73 6679 632e 6c74 642f 7765 6368 6174  .sfyc.ltd/wechat
+000005e0: 5f65 7665 7279 6461 792f 7778 6772 6f75  _everyday/wxgrou
+000005f0: 705f 6c6f 676f 2e70 6e67 3f69 6d61 6765  p_logo.png?image
+00000600: 5669 6577 322f 302f 772f 3630 2f68 2f32  View2/0/w/60/h/2
+00000610: 3029 5d28 2343 6f6e 7461 6374 290a 2020  0)](#Contact).  
+00000620: 2020 2020 2020 0a20 2020 2020 2020 200a        .        .
+00000630: 2020 2020 2020 2020 2323 2049 6e74 726f          ## Intro
+00000640: 6475 6374 696f 6e0a 2020 2020 2020 2020  duction.        
+00000650: 5079 5465 7874 436c 6173 7369 6669 6572  PyTextClassifier
+00000660: 3a20 5079 7468 6f6e 2054 6578 7420 436c  : Python Text Cl
+00000670: 6173 7369 6669 6572 2e20 4974 2063 616e  assifier. It can
+00000680: 2062 6520 6170 706c 6965 6420 746f 2074   be applied to t
+00000690: 6865 2066 6965 6c64 7320 6f66 2073 656e  he fields of sen
+000006a0: 7469 6d65 6e74 2070 6f6c 6172 6974 7920  timent polarity 
+000006b0: 616e 616c 7973 6973 2c20 7465 7874 2072  analysis, text r
+000006c0: 6973 6b20 636c 6173 7369 6669 6361 7469  isk classificati
+000006d0: 6f6e 2061 6e64 2073 6f20 6f6e 2c0a 2020  on and so on,.  
+000006e0: 2020 2020 2020 616e 6420 6974 2073 7570        and it sup
+000006f0: 706f 7274 7320 6d75 6c74 6970 6c65 2063  ports multiple c
+00000700: 6c61 7373 6966 6963 6174 696f 6e20 616c  lassification al
+00000710: 676f 7269 7468 6d73 2061 6e64 2063 6c75  gorithms and clu
+00000720: 7374 6572 696e 6720 616c 676f 7269 7468  stering algorith
+00000730: 6d73 2e0a 2020 2020 2020 2020 0a20 2020  ms..        .   
+00000740: 2020 2020 202a 2a70 7974 6578 7463 6c61       **pytextcla
+00000750: 7373 6966 6965 722a 2a20 6973 2061 2070  ssifier** is a p
+00000760: 7974 686f 6e20 4f70 656e 2053 6f75 7263  ython Open Sourc
+00000770: 6520 546f 6f6c 6b69 7420 666f 7220 7465  e Toolkit for te
+00000780: 7874 2063 6c61 7373 6966 6963 6174 696f  xt classificatio
+00000790: 6e2e 2054 6865 2067 6f61 6c20 6973 2074  n. The goal is t
+000007a0: 6f20 696d 706c 656d 656e 740a 2020 2020  o implement.    
+000007b0: 2020 2020 7465 7874 2061 6e61 6c79 7369      text analysi
+000007c0: 7320 616c 676f 7269 7468 6d2c 2073 6f20  s algorithm, so 
+000007d0: 746f 2061 6368 6965 7665 2074 6865 2075  to achieve the u
+000007e0: 7365 2069 6e20 7468 6520 7072 6f64 7563  se in the produc
+000007f0: 7469 6f6e 2065 6e76 6972 6f6e 6d65 6e74  tion environment
+00000800: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00000810: 2020 20e6 9687 e69c ace5 8886 e7b1 bbe5     .............
+00000820: 99a8 efbc 8ce6 8f90 e4be 9be5 a49a e7a7  ................
+00000830: 8de6 9687 e69c ace5 8886 e7b1 bbe5 928c  ................
+00000840: e881 9ae7 b1bb e7ae 97e6 b395 efbc 8ce6  ................
+00000850: 94af e68c 81e5 8fa5 e5ad 90e5 928c e696  ................
+00000860: 87e6 a1a3 e7ba a7e7 9a84 e696 87e6 9cac  ................
+00000870: e588 86e7 b1bb e4bb bbe5 8aa1 efbc 8ce6  ................
+00000880: 94af e68c 81e4 ba8c e588 86e7 b1bb e380  ................
+00000890: 81e5 a49a e588 86e7 b1bb e380 81e5 a49a  ................
+000008a0: e6a0 87e7 adbe e588 86e7 b1bb e380 81e5  ................
+000008b0: a49a e5b1 82e7 baa7 e588 86e7 b1bb e592  ................
+000008c0: 8c4b 6d65 616e 73e8 819a e7b1 bbef bc8c  .Kmeans.........
+000008d0: e5bc 80e7 aeb1 e58d b3e7 94a8 e380 8270  ...............p
+000008e0: 7974 686f 6e33 e5bc 80e5 8f91 e380 820a  ython3..........
+000008f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000900: 202a 2a47 7569 6465 2a2a 0a20 2020 2020   **Guide**.     
+00000910: 2020 200a 2020 2020 2020 2020 2d20 5b46     .        - [F
+00000920: 6561 7475 7265 5d28 2346 6561 7475 7265  eature](#Feature
+00000930: 290a 2020 2020 2020 2020 2d20 5b49 6e73  ).        - [Ins
+00000940: 7461 6c6c 5d28 2369 6e73 7461 6c6c 290a  tall](#install).
+00000950: 2020 2020 2020 2020 2d20 5b55 7361 6765          - [Usage
+00000960: 5d28 2375 7361 6765 290a 2020 2020 2020  ](#usage).      
+00000970: 2020 2d20 5b44 6174 6173 6574 5d28 2344    - [Dataset](#D
+00000980: 6174 6173 6574 290a 2020 2020 2020 2020  ataset).        
+00000990: 2d20 5b43 6f6e 7461 6374 5d28 2343 6f6e  - [Contact](#Con
+000009a0: 7461 6374 290a 2020 2020 2020 2020 2d20  tact).        - 
+000009b0: 5b43 6974 6174 696f 6e5d 2823 4369 7461  [Citation](#Cita
+000009c0: 7469 6f6e 290a 2020 2020 2020 2020 2d20  tion).        - 
+000009d0: 5b52 6566 6572 656e 6365 5d28 2372 6566  [Reference](#ref
+000009e0: 6572 656e 6365 290a 2020 2020 2020 2020  erence).        
+000009f0: 0a20 2020 2020 2020 2023 2320 4665 6174  .        ## Feat
+00000a00: 7572 650a 2020 2020 2020 2020 0a20 2020  ure.        .   
+00000a10: 2020 2020 202a 2a70 7974 6578 7463 6c61       **pytextcla
+00000a20: 7373 6966 6965 722a 2a20 6861 7320 7468  ssifier** has th
+00000a30: 6520 6368 6172 6163 7465 7269 7374 6963  e characteristic
+00000a40: 730a 2020 2020 2020 2020 6f66 2063 6c65  s.        of cle
+00000a50: 6172 2061 6c67 6f72 6974 686d 2c20 6869  ar algorithm, hi
+00000a60: 6768 2070 6572 666f 726d 616e 6365 2061  gh performance a
+00000a70: 6e64 2063 7573 746f 6d69 7a61 626c 6520  nd customizable 
+00000a80: 636f 7270 7573 2e0a 2020 2020 2020 2020  corpus..        
+00000a90: 0a20 2020 2020 2020 2046 756e 6374 696f  .        Functio
+00000aa0: 6e73 efbc 9a0a 2020 2020 2020 2020 2323  ns....        ##
+00000ab0: 2320 436c 6173 7369 6669 6572 0a20 2020  # Classifier.   
+00000ac0: 2020 2020 2020 202d 205b 785d 204c 6f67         - [x] Log
+00000ad0: 6973 7469 6352 6567 7265 7373 696f 6e0a  isticRegression.
+00000ae0: 2020 2020 2020 2020 2020 2d20 5b78 5d20            - [x] 
+00000af0: 5261 6e64 6f6d 2046 6f72 6573 740a 2020  Random Forest.  
+00000b00: 2020 2020 2020 2020 2d20 5b78 5d20 4465          - [x] De
+00000b10: 6369 7369 6f6e 2054 7265 650a 2020 2020  cision Tree.    
+00000b20: 2020 2020 2020 2d20 5b78 5d20 4b2d 4e65        - [x] K-Ne
+00000b30: 6172 6573 7420 4e65 6967 6862 6f75 7273  arest Neighbours
+00000b40: 0a20 2020 2020 2020 2020 202d 205b 785d  .          - [x]
+00000b50: 204e 6169 7665 2062 6179 6573 0a20 2020   Naive bayes.   
+00000b60: 2020 2020 2020 202d 205b 785d 2058 6762         - [x] Xgb
+00000b70: 6f6f 7374 0a20 2020 2020 2020 2020 202d  oost.          -
+00000b80: 205b 785d 2053 7570 706f 7274 2056 6563   [x] Support Vec
+00000b90: 746f 7220 4d61 6368 696e 6528 5356 4d29  tor Machine(SVM)
+00000ba0: 0a20 2020 2020 2020 2020 202d 205b 785d  .          - [x]
+00000bb0: 2054 6578 7443 4e4e 0a20 2020 2020 2020   TextCNN.       
+00000bc0: 2020 202d 205b 785d 2054 6578 7452 4e4e     - [x] TextRNN
+00000bd0: 0a20 2020 2020 2020 2020 202d 205b 785d  .          - [x]
+00000be0: 2046 6173 7474 6578 740a 2020 2020 2020   Fasttext.      
+00000bf0: 2020 2020 2d20 5b78 5d20 4245 5254 0a20      - [x] BERT. 
+00000c00: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000c10: 2323 2320 436c 7573 7465 720a 2020 2020  ### Cluster.    
+00000c20: 2020 2020 2020 2d20 5b78 5d20 4d69 6e69        - [x] Mini
+00000c30: 4261 7463 684b 6d65 616e 730a 2020 2020  BatchKmeans.    
+00000c40: 2020 2020 0a20 2020 2020 2020 2057 6869      .        Whi
+00000c50: 6c65 2070 726f 7669 6469 6e67 2072 6963  le providing ric
+00000c60: 6820 6675 6e63 7469 6f6e 732c 202a 2a70  h functions, **p
+00000c70: 7974 6578 7463 6c61 7373 6966 6965 722a  ytextclassifier*
+00000c80: 2a20 696e 7465 726e 616c 206d 6f64 756c  * internal modul
+00000c90: 6573 2061 6468 6572 6520 746f 206c 6f77  es adhere to low
+00000ca0: 2063 6f75 706c 696e 672c 206d 6f64 656c   coupling, model
+00000cb0: 2061 6468 6572 656e 6365 2074 6f20 696e   adherence to in
+00000cc0: 6572 7420 6c6f 6164 696e 672c 2064 6963  ert loading, dic
+00000cd0: 7469 6f6e 6172 7920 7075 626c 6963 6174  tionary publicat
+00000ce0: 696f 6e2c 2061 6e64 2065 6173 7920 746f  ion, and easy to
+00000cf0: 2075 7365 2e0a 2020 2020 2020 2020 0a20   use..        . 
+00000d00: 2020 2020 2020 2023 2320 496e 7374 616c         ## Instal
+00000d10: 6c0a 2020 2020 2020 2020 0a20 2020 2020  l.        .     
+00000d20: 2020 202d 2052 6571 7569 7265 6d65 6e74     - Requirement
+00000d30: 7320 616e 6420 496e 7374 616c 6c61 7469  s and Installati
+00000d40: 6f6e 0a20 2020 2020 2020 200a 2020 2020  on.        .    
+00000d50: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+00000d60: 7069 7033 2069 6e73 7461 6c6c 2074 6f72  pip3 install tor
+00000d70: 6368 2023 2063 6f6e 6461 2069 6e73 7461  ch # conda insta
+00000d80: 6c6c 2070 7974 6f72 6368 0a20 2020 2020  ll pytorch.     
+00000d90: 2020 2070 6970 3320 696e 7374 616c 6c20     pip3 install 
+00000da0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00000db0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00000dc0: 2020 2020 200a 2020 2020 2020 2020 6f72       .        or
+00000dd0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000de0: 2020 6060 600a 2020 2020 2020 2020 6769    ```.        gi
+00000df0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00000e00: 6769 7468 7562 2e63 6f6d 2f73 6869 6269  github.com/shibi
+00000e10: 6e67 3632 342f 7079 7465 7874 636c 6173  ng624/pytextclas
+00000e20: 7369 6669 6572 2e67 6974 0a20 2020 2020  sifier.git.     
+00000e30: 2020 2063 6420 7079 7465 7874 636c 6173     cd pytextclas
+00000e40: 7369 6669 6572 0a20 2020 2020 2020 2070  sifier.        p
+00000e50: 7974 686f 6e33 2073 6574 7570 2e70 7920  ython3 setup.py 
+00000e60: 696e 7374 616c 6c0a 2020 2020 2020 2020  install.        
+00000e70: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
+00000e80: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00000e90: 2055 7361 6765 0a20 2020 2020 2020 2023   Usage.        #
+00000ea0: 2323 2054 6578 7420 436c 6173 7369 6669  ## Text Classifi
+00000eb0: 6572 0a20 2020 2020 2020 200a 2020 2020  er.        .    
+00000ec0: 2020 2020 2323 2320 456e 676c 6973 6820      ### English 
+00000ed0: 5465 7874 2043 6c61 7373 6966 6965 720a  Text Classifier.
+00000ee0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000ef0: 2049 6e63 6c75 6469 6e67 206d 6f64 656c   Including model
+00000f00: 2074 7261 696e 696e 672c 2073 6176 696e   training, savin
+00000f10: 672c 2070 7265 6469 6374 2c20 6576 616c  g, predict, eval
+00000f20: 7561 7465 2c20 666f 7220 6578 616d 706c  uate, for exampl
+00000f30: 6520 5b65 7861 6d70 6c65 732f 6c72 5f65  e [examples/lr_e
+00000f40: 6e5f 636c 6173 7369 6669 6361 7469 6f6e  n_classification
+00000f50: 5f64 656d 6f2e 7079 5d28 6874 7470 733a  _demo.py](https:
+00000f60: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6869  //github.com/shi
+00000f70: 6269 6e67 3632 342f 7079 7465 7874 636c  bing624/pytextcl
+00000f80: 6173 7369 6669 6572 2f62 6c6f 622f 6d61  assifier/blob/ma
+00000f90: 7374 6572 2f65 7861 6d70 6c65 732f 6c72  ster/examples/lr
+00000fa0: 5f65 6e5f 636c 6173 7369 6669 6361 7469  _en_classificati
+00000fb0: 6f6e 5f64 656d 6f2e 7079 293a 0a20 2020  on_demo.py):.   
+00000fc0: 2020 2020 200a 2020 2020 2020 2020 6060       .        ``
+00000fd0: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00000fe0: 696d 706f 7274 2073 7973 0a20 2020 2020  import sys.     
+00000ff0: 2020 200a 2020 2020 2020 2020 7379 732e     .        sys.
+00001000: 7061 7468 2e61 7070 656e 6428 272e 2e27  path.append('..'
+00001010: 290a 2020 2020 2020 2020 6672 6f6d 2070  ).        from p
+00001020: 7974 6578 7463 6c61 7373 6966 6965 7220  ytextclassifier 
+00001030: 696d 706f 7274 2043 6c61 7373 6963 436c  import ClassicCl
+00001040: 6173 7369 6669 6572 0a20 2020 2020 2020  assifier.       
+00001050: 200a 2020 2020 2020 2020 6966 205f 5f6e   .        if __n
+00001060: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
+00001070: 5f5f 273a 0a20 2020 2020 2020 2020 2020  __':.           
+00001080: 206d 203d 2043 6c61 7373 6963 436c 6173   m = ClassicClas
+00001090: 7369 6669 6572 286f 7574 7075 745f 6469  sifier(output_di
+000010a0: 723d 276d 6f64 656c 732f 6c72 272c 206d  r='models/lr', m
+000010b0: 6f64 656c 5f6e 616d 655f 6f72 5f6d 6f64  odel_name_or_mod
+000010c0: 656c 3d27 6c72 2729 0a20 2020 2020 2020  el='lr').       
+000010d0: 2020 2020 2023 2043 6c61 7373 6963 436c       # ClassicCl
+000010e0: 6173 7369 6669 6572 2073 7570 706f 7274  assifier support
+000010f0: 206d 6f64 656c 5f6e 616d 65ef bc9a 6c72   model_name...lr
+00001100: 2c20 7261 6e64 6f6d 5f66 6f72 6573 742c  , random_forest,
+00001110: 2064 6563 6973 696f 6e5f 7472 6565 2c20   decision_tree, 
+00001120: 6b6e 6e2c 2062 6179 6573 2c20 7376 6d2c  knn, bayes, svm,
+00001130: 2078 6762 6f6f 7374 0a20 2020 2020 2020   xgboost.       
+00001140: 2020 2020 2070 7269 6e74 286d 290a 2020       print(m).  
+00001150: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00001160: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00001170: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+00001180: 2027 5374 7564 656e 7420 6465 6274 2074   'Student debt t
+00001190: 6f20 636f 7374 2042 7269 7461 696e 2062  o cost Britain b
+000011a0: 696c 6c69 6f6e 7320 7769 7468 696e 2064  illions within d
+000011b0: 6563 6164 6573 2729 2c0a 2020 2020 2020  ecades'),.      
+000011c0: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
+000011d0: 6174 696f 6e27 2c20 2743 6869 6e65 7365  ation', 'Chinese
+000011e0: 2065 6475 6361 7469 6f6e 2066 6f72 2054   education for T
+000011f0: 5620 6578 7065 7269 6d65 6e74 2729 2c0a  V experiment'),.
+00001200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001210: 2827 7370 6f72 7473 272c 2027 4d69 6464  ('sports', 'Midd
+00001220: 6c65 2045 6173 7420 616e 6420 4173 6961  le East and Asia
+00001230: 2062 6f6f 7374 2069 6e76 6573 746d 656e   boost investmen
+00001240: 7420 696e 2074 6f70 206c 6576 656c 2073  t in top level s
+00001250: 706f 7274 7327 292c 0a20 2020 2020 2020  ports'),.       
+00001260: 2020 2020 2020 2020 2028 2773 706f 7274           ('sport
+00001270: 7327 2c20 2753 756d 6d69 7420 5365 7269  s', 'Summit Seri
+00001280: 6573 206c 6f6f 6b20 6c61 756e 6368 6573  es look launches
+00001290: 2048 424f 2043 616e 6164 6120 7370 6f72   HBO Canada spor
+000012a0: 7473 2064 6f63 2073 6572 6965 733a 204d  ts doc series: M
+000012b0: 7564 6861 7227 290a 2020 2020 2020 2020  udhar').        
+000012c0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+000012d0: 2020 2320 7472 6169 6e20 616e 6420 7361    # train and sa
+000012e0: 7665 2062 6573 7420 6d6f 6465 6c0a 2020  ve best model.  
+000012f0: 2020 2020 2020 2020 2020 6d2e 7472 6169            m.trai
+00001300: 6e28 6461 7461 290a 2020 2020 2020 2020  n(data).        
+00001310: 2020 2020 2320 6c6f 6164 2062 6573 7420      # load best 
+00001320: 6d6f 6465 6c20 6672 6f6d 206d 6f64 656c  model from model
+00001330: 5f64 6972 0a20 2020 2020 2020 2020 2020  _dir.           
+00001340: 206d 2e6c 6f61 645f 6d6f 6465 6c28 290a   m.load_model().
+00001350: 2020 2020 2020 2020 2020 2020 7072 6564              pred
+00001360: 6963 745f 6c61 6265 6c2c 2070 7265 6469  ict_label, predi
+00001370: 6374 5f70 726f 6261 203d 206d 2e70 7265  ct_proba = m.pre
+00001380: 6469 6374 285b 0a20 2020 2020 2020 2020  dict([.         
+00001390: 2020 2020 2020 2027 4162 626f 7474 2067         'Abbott g
+000013a0: 6f76 6572 6e6d 656e 7420 7370 656e 6473  overnment spends
+000013b0: 2024 3820 6d69 6c6c 696f 6e20 6f6e 2068   $8 million on h
+000013c0: 6967 6865 7220 6564 7563 6174 696f 6e20  igher education 
+000013d0: 6d65 6469 6120 626c 6974 7a27 5d29 0a20  media blitz']). 
+000013e0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000013f0: 2866 2770 7265 6469 6374 5f6c 6162 656c  (f'predict_label
+00001400: 3a20 7b70 7265 6469 6374 5f6c 6162 656c  : {predict_label
+00001410: 7d2c 2070 7265 6469 6374 5f70 726f 6261  }, predict_proba
+00001420: 3a20 7b70 7265 6469 6374 5f70 726f 6261  : {predict_proba
+00001430: 7d27 290a 2020 2020 2020 2020 0a20 2020  }').        .   
+00001440: 2020 2020 2020 2020 2074 6573 745f 6461           test_da
+00001450: 7461 203d 205b 0a20 2020 2020 2020 2020  ta = [.         
+00001460: 2020 2020 2020 2028 2765 6475 6361 7469         ('educati
+00001470: 6f6e 272c 2027 4162 626f 7474 2067 6f76  on', 'Abbott gov
+00001480: 6572 6e6d 656e 7420 7370 656e 6473 2024  ernment spends $
+00001490: 3820 6d69 6c6c 696f 6e20 6f6e 2068 6967  8 million on hig
+000014a0: 6865 7220 6564 7563 6174 696f 6e20 6d65  her education me
+000014b0: 6469 6120 626c 6974 7a27 292c 0a20 2020  dia blitz'),.   
+000014c0: 2020 2020 2020 2020 2020 2020 2028 2773               ('s
+000014d0: 706f 7274 7327 2c20 274d 6964 646c 6520  ports', 'Middle 
+000014e0: 4561 7374 2061 6e64 2041 7369 6120 626f  East and Asia bo
+000014f0: 6f73 7420 696e 7665 7374 6d65 6e74 2069  ost investment i
+00001500: 6e20 746f 7020 6c65 7665 6c20 7370 6f72  n top level spor
+00001510: 7473 2729 2c0a 2020 2020 2020 2020 2020  ts'),.          
+00001520: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00001530: 6163 635f 7363 6f72 6520 3d20 6d2e 6576  acc_score = m.ev
+00001540: 616c 7561 7465 5f6d 6f64 656c 2874 6573  aluate_model(tes
+00001550: 745f 6461 7461 290a 2020 2020 2020 2020  t_data).        
+00001560: 2020 2020 7072 696e 7428 6627 6163 635f      print(f'acc_
+00001570: 7363 6f72 653a 207b 6163 635f 7363 6f72  score: {acc_scor
+00001580: 657d 2729 0a20 2020 2020 2020 2060 6060  e}').        ```
+00001590: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+000015a0: 2020 6f75 7470 7574 3a0a 2020 2020 2020    output:.      
+000015b0: 2020 0a20 2020 2020 2020 2060 6060 0a20    .        ```. 
+000015c0: 2020 2020 2020 2043 6c61 7373 6963 436c         ClassicCl
+000015d0: 6173 7369 6669 6572 2069 6e73 7461 6e63  assifier instanc
+000015e0: 6520 284c 6f67 6973 7469 6352 6567 7265  e (LogisticRegre
+000015f0: 7373 696f 6e28 6669 745f 696e 7465 7263  ssion(fit_interc
+00001600: 6570 743d 4661 6c73 6529 2c20 7374 6f70  ept=False), stop
+00001610: 776f 7264 7320 7369 7a65 3a20 3234 3338  words size: 2438
+00001620: 290a 2020 2020 2020 2020 7072 6564 6963  ).        predic
+00001630: 745f 6c61 6265 6c3a 205b 2765 6475 6361  t_label: ['educa
+00001640: 7469 6f6e 275d 2c20 7072 6564 6963 745f  tion'], predict_
+00001650: 7072 6f62 613a 205b 302e 3533 3738 3233  proba: [0.537823
+00001660: 3633 3538 3439 3231 3132 5d0a 2020 2020  6358492112].    
+00001670: 2020 2020 6163 635f 7363 6f72 653a 2031      acc_score: 1
+00001680: 2e30 0a20 2020 2020 2020 2060 6060 0a20  .0.        ```. 
+00001690: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000016a0: 2323 2320 4368 696e 6573 6520 5465 7874  ### Chinese Text
+000016b0: 2043 6c61 7373 6966 6965 7228 e4b8 ade6   Classifier(....
+000016c0: 9687 e696 87e6 9cac e588 86e7 b1bb 290a  ..............).
+000016d0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000016e0: 2054 6578 7420 636c 6173 7369 6669 6361   Text classifica
+000016f0: 7469 6f6e 2063 6f6d 7061 7469 626c 6520  tion compatible 
+00001700: 7769 7468 2043 6869 6e65 7365 2061 6e64  with Chinese and
+00001710: 2045 6e67 6c69 7368 2063 6f72 706f 7261   English corpora
+00001720: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00001730: 2020 2065 7861 6d70 6c65 205b 6578 616d     example [exam
+00001740: 706c 6573 2f6c 725f 636c 6173 7369 6669  ples/lr_classifi
+00001750: 6361 7469 6f6e 5f64 656d 6f2e 7079 5d28  cation_demo.py](
+00001760: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001770: 6f6d 2f73 6869 6269 6e67 3632 342f 7079  om/shibing624/py
+00001780: 7465 7874 636c 6173 7369 6669 6572 2f62  textclassifier/b
+00001790: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
+000017a0: 6c65 732f 6c72 5f63 6c61 7373 6966 6963  les/lr_classific
+000017b0: 6174 696f 6e5f 6465 6d6f 2e70 7929 0a20  ation_demo.py). 
+000017c0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000017d0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
+000017e0: 2020 696d 706f 7274 2073 7973 0a20 2020    import sys.   
+000017f0: 2020 2020 200a 2020 2020 2020 2020 7379       .        sy
+00001800: 732e 7061 7468 2e61 7070 656e 6428 272e  s.path.append('.
+00001810: 2e27 290a 2020 2020 2020 2020 6672 6f6d  .').        from
+00001820: 2070 7974 6578 7463 6c61 7373 6966 6965   pytextclassifie
+00001830: 7220 696d 706f 7274 2043 6c61 7373 6963  r import Classic
+00001840: 436c 6173 7369 6669 6572 0a20 2020 2020  Classifier.     
+00001850: 2020 200a 2020 2020 2020 2020 6966 205f     .        if _
+00001860: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00001870: 696e 5f5f 273a 0a20 2020 2020 2020 2020  in__':.         
+00001880: 2020 206d 203d 2043 6c61 7373 6963 436c     m = ClassicCl
+00001890: 6173 7369 6669 6572 286f 7574 7075 745f  assifier(output_
+000018a0: 6469 723d 276d 6f64 656c 732f 6c72 2d74  dir='models/lr-t
+000018b0: 6f79 272c 206d 6f64 656c 5f6e 616d 655f  oy', model_name_
+000018c0: 6f72 5f6d 6f64 656c 3d27 6c72 2729 0a20  or_model='lr'). 
+000018d0: 2020 2020 2020 2020 2020 2023 20e7 bb8f             # ...
+000018e0: e585 b8e5 8886 e7b1 bbe6 96b9 e6b3 95ef  ................
+000018f0: bc8c e694 afe6 8c81 e79a 84e6 a8a1 e59e  ................
+00001900: 8be5 8c85 e68b acef bc9a 6c72 2c20 7261  ..........lr, ra
+00001910: 6e64 6f6d 5f66 6f72 6573 742c 2064 6563  ndom_forest, dec
+00001920: 6973 696f 6e5f 7472 6565 2c20 6b6e 6e2c  ision_tree, knn,
+00001930: 2062 6179 6573 2c20 7376 6d2c 2078 6762   bayes, svm, xgb
+00001940: 6f6f 7374 0a20 2020 2020 2020 2020 2020  oost.           
+00001950: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
+00001960: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
+00001970: 6174 696f 6e27 2c20 27e5 908d e5b8 88e6  ation', '.......
+00001980: 8c87 e5af bce6 8998 e7a6 8fe8 afad e6b3  ................
+00001990: 95e6 8a80 e5b7 a7ef bc9a e590 8de8 af8d  ................
+000019a0: e79a 84e5 a48d e695 b0e5 bda2 e5bc 8f27  ...............'
+000019b0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000019c0: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+000019d0: 2027 e4b8 ade5 9bbd e9ab 98e8 8083 e688   '..............
+000019e0: 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5 8faf  ................
+000019f0: 20e6 98af e280 9ce7 8bbc e69d a5e4 ba86   ...............
+00001a00: e280 9de5 9097 efbc 9f27 292c 0a20 2020  .........'),.   
+00001a10: 2020 2020 2020 2020 2020 2020 2028 2765               ('e
+00001a20: 6475 6361 7469 6f6e 272c 2027 e585 ace5  ducation', '....
+00001a30: 8aa1 e591 98e8 8083 e899 91e8 b68a e69d  ................
+00001a40: a5e8 b68a e590 83e9 a699 efbc 8ce8 bf99  ................
+00001a50: e698 afe6 808e e4b9 88e5 9b9e e4ba 8bef  ................
+00001a60: bc9f 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
+00001a70: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
+00001a80: 2027 e59b bee6 9687 efbc 9ae6 b395 e7bd   '..............
+00001a90: 91e5 ad9f e88f b2e5 b094 e696 afe8 8ba6  ................
+00001aa0: e688 98e8 bf9b 3136 e5bc ba20 e5ad 9fe8  ......16... ....
+00001ab0: 8fb2 e5b0 94e6 96af e680 92e5 90bc 2729  ..............')
+00001ac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001ad0: 2020 2827 7370 6f72 7473 272c 2027 e59b    ('sports', '..
+00001ae0: 9be5 b79d e4b8 b9e6 a3b1 e4b8 bee8 a18c  ................
+00001af0: e585 a8e5 9bbd e995 bfe8 b79d e799 bbe5  ................
+00001b00: b1b1 e68c 91e6 8898 e8b5 9b20 e8bf 91e4  ........... ....
+00001b10: b887 e4ba bae5 8f82 e4b8 8e27 292c 0a20  ...........'),. 
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00001b30: 2773 706f 7274 7327 2c20 27e7 b1b3 e585  'sports', '.....
+00001b40: b0e5 aea2 e59c ba38 e688 98e4 b88d e8b4  .......8........
+00001b50: a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8  .......10.......
+00001b60: 839c 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
+00001b70: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+00001b80: 6d2e 7472 6169 6e28 6461 7461 290a 2020  m.train(data).  
+00001b90: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00001ba0: 6d29 0a20 2020 2020 2020 2020 2020 2023  m).            #
+00001bb0: 206c 6f61 6420 6265 7374 206d 6f64 656c   load best model
+00001bc0: 2066 726f 6d20 6d6f 6465 6c5f 6469 720a   from model_dir.
+00001bd0: 2020 2020 2020 2020 2020 2020 6d2e 6c6f              m.lo
+00001be0: 6164 5f6d 6f64 656c 2829 0a20 2020 2020  ad_model().     
+00001bf0: 2020 2020 2020 2070 7265 6469 6374 5f6c         predict_l
+00001c00: 6162 656c 2c20 7072 6564 6963 745f 7072  abel, predict_pr
+00001c10: 6f62 6120 3d20 6d2e 7072 6564 6963 7428  oba = m.predict(
+00001c20: 5b27 e7a6 8fe5 bbba e698 a5e5 ada3 e585  ['..............
+00001c30: ace5 8aa1 e591 98e8 8083 e8af 95e6 8aa5  ................
+00001c40: e590 8d31 38e6 97a5 e688 aae6 ada2 2032  ...18......... 2
+00001c50: e69c 8836 e697 a5e8 8083 e8af 9527 2c0a  ...6.........',.
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 27e6 848f e794 b2e9 a696        '.........
+00001ca0: e8bd aee8 a1a5 e8b5 9be4 baa4 e688 98e8  ................
+00001cb0: aeb0 e5bd 953a e7b1 b3e5 85b0 e5ae a2e5  .....:..........
+00001cc0: 9cba 38e6 8898 e4b8 8de8 b4a5 e59b bde7  ..8.............
+00001cd0: b1b3 3130 e5b9 b4e8 bf9e e883 9c27 5d29  ..10.........'])
+00001ce0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00001cf0: 6e74 2866 2770 7265 6469 6374 5f6c 6162  nt(f'predict_lab
+00001d00: 656c 3a20 7b70 7265 6469 6374 5f6c 6162  el: {predict_lab
+00001d10: 656c 7d2c 2070 7265 6469 6374 5f70 726f  el}, predict_pro
+00001d20: 6261 3a20 7b70 7265 6469 6374 5f70 726f  ba: {predict_pro
+00001d30: 6261 7d27 290a 2020 2020 2020 2020 0a20  ba}').        . 
+00001d40: 2020 2020 2020 2020 2020 2074 6573 745f             test_
+00001d50: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
+00001d60: 2020 2020 2020 2020 2028 2765 6475 6361           ('educa
+00001d70: 7469 6f6e 272c 2027 e7a6 8fe5 bbba e698  tion', '........
+00001d80: a5e5 ada3 e585 ace5 8aa1 e591 98e8 8083  ................
+00001d90: e8af 95e6 8aa5 e590 8d31 38e6 97a5 e688  .........18.....
+00001da0: aae6 ada2 2032 e69c 8836 e697 a5e8 8083  .... 2...6......
+00001db0: e8af 9527 292c 0a20 2020 2020 2020 2020  ...'),.         
+00001dc0: 2020 2020 2020 2028 2773 706f 7274 7327         ('sports'
+00001dd0: 2c20 27e6 848f e794 b2e9 a696 e8bd aee8  , '.............
+00001de0: a1a5 e8b5 9be4 baa4 e688 98e8 aeb0 e5bd  ................
+00001df0: 953a e7b1 b3e5 85b0 e5ae a2e5 9cba 38e6  .:............8.
+00001e00: 8898 e4b8 8de8 b4a5 e59b bde7 b1b3 3130  ..............10
+00001e10: e5b9 b4e8 bf9e e883 9c27 292c 0a20 2020  .........'),.   
+00001e20: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00001e30: 2020 2020 2020 2061 6363 5f73 636f 7265         acc_score
+00001e40: 203d 206d 2e65 7661 6c75 6174 655f 6d6f   = m.evaluate_mo
+00001e50: 6465 6c28 7465 7374 5f64 6174 6129 0a20  del(test_data). 
+00001e60: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00001e70: 2866 2761 6363 5f73 636f 7265 3a20 7b61  (f'acc_score: {a
+00001e80: 6363 5f73 636f 7265 7d27 2920 2023 2031  cc_score}')  # 1
+00001e90: 2e30 0a20 2020 2020 2020 200a 2020 2020  .0.        .    
+00001ea0: 2020 2020 2020 2020 2323 2323 2074 7261          #### tra
+00001eb0: 696e 206d 6f64 656c 2077 6974 6820 3177  in model with 1w
+00001ec0: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+00001ed0: 2020 7072 696e 7428 272d 2720 2a20 3432    print('-' * 42
+00001ee0: 290a 2020 2020 2020 2020 2020 2020 6d20  ).            m 
+00001ef0: 3d20 436c 6173 7369 6343 6c61 7373 6966  = ClassicClassif
+00001f00: 6965 7228 6f75 7470 7574 5f64 6972 3d27  ier(output_dir='
+00001f10: 6d6f 6465 6c73 2f6c 7227 2c20 6d6f 6465  models/lr', mode
+00001f20: 6c5f 6e61 6d65 5f6f 725f 6d6f 6465 6c3d  l_name_or_model=
+00001f30: 276c 7227 290a 2020 2020 2020 2020 2020  'lr').          
+00001f40: 2020 6461 7461 5f66 696c 6520 3d20 2774    data_file = 't
+00001f50: 6875 636e 6577 735f 7472 6169 6e5f 3177  hucnews_train_1w
+00001f60: 2e74 7874 270a 2020 2020 2020 2020 2020  .txt'.          
+00001f70: 2020 6d2e 7472 6169 6e28 6461 7461 5f66    m.train(data_f
+00001f80: 696c 6529 0a20 2020 2020 2020 2020 2020  ile).           
+00001f90: 206d 2e6c 6f61 645f 6d6f 6465 6c28 290a   m.load_model().
+00001fa0: 2020 2020 2020 2020 2020 2020 7072 6564              pred
+00001fb0: 6963 745f 6c61 6265 6c2c 2070 7265 6469  ict_label, predi
+00001fc0: 6374 5f70 726f 6261 203d 206d 2e70 7265  ct_proba = m.pre
+00001fd0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
+00001fe0: 2020 2020 2020 5b27 e9a1 bae4 b989 e58c        ['........
+00001ff0: 97e4 baac e88b 8fe6 b4bb 3838 e5b9 b3e7  ..........88....
+00002000: b1b3 e8b5 b7e7 b2be e8a3 85e6 88bf e59c  ................
+00002010: a8e5 94ae 272c 0a20 2020 2020 2020 2020  ....',.         
+00002020: 2020 2020 2020 2020 27e7 be8e 4542 2d35          '...EB-5
+00002030: e9a1 b9e7 9bae e280 9c31 35e6 97a5 e5bf  .........15.....
+00002040: abe9 809f e7a7 bbe6 b091 e280 9de5 b086  ................
+00002050: e68e a8e8 bf9f 275d 290a 2020 2020 2020  ......']).      
+00002060: 2020 2020 2020 7072 696e 7428 6627 7072        print(f'pr
+00002070: 6564 6963 745f 6c61 6265 6c3a 207b 7072  edict_label: {pr
+00002080: 6564 6963 745f 6c61 6265 6c7d 2c20 7072  edict_label}, pr
+00002090: 6564 6963 745f 7072 6f62 613a 207b 7072  edict_proba: {pr
+000020a0: 6564 6963 745f 7072 6f62 617d 2729 0a20  edict_proba}'). 
+000020b0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+000020c0: 2020 200a 2020 2020 2020 2020 6f75 7470     .        outp
+000020d0: 7574 3a0a 2020 2020 2020 2020 0a20 2020  ut:.        .   
+000020e0: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+000020f0: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
+00002100: 6572 2069 6e73 7461 6e63 6520 284c 6f67  er instance (Log
+00002110: 6973 7469 6352 6567 7265 7373 696f 6e28  isticRegression(
+00002120: 6669 745f 696e 7465 7263 6570 743d 4661  fit_intercept=Fa
+00002130: 6c73 6529 2c20 7374 6f70 776f 7264 7320  lse), stopwords 
+00002140: 7369 7a65 3a20 3234 3338 290a 2020 2020  size: 2438).    
+00002150: 2020 2020 7072 6564 6963 745f 6c61 6265      predict_labe
+00002160: 6c3a 205b 2765 6475 6361 7469 6f6e 2720  l: ['education' 
+00002170: 2773 706f 7274 7327 5d2c 2070 7265 6469  'sports'], predi
+00002180: 6374 5f70 726f 6261 3a20 5b30 2e35 2c20  ct_proba: [0.5, 
+00002190: 302e 3539 3839 3431 3830 3637 3431 3533  0.59894180674153
+000021a0: 345d 0a20 2020 2020 2020 2061 6363 5f73  4].        acc_s
+000021b0: 636f 7265 3a20 312e 300a 2020 2020 2020  core: 1.0.      
+000021c0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+000021d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000021e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+000021f0: 2020 2020 2070 7265 6469 6374 5f6c 6162       predict_lab
+00002200: 656c 3a20 5b27 7265 616c 7479 2720 2765  el: ['realty' 'e
+00002210: 6475 6361 7469 6f6e 275d 2c20 7072 6564  ducation'], pred
+00002220: 6963 745f 7072 6f62 613a 205b 302e 3733  ict_proba: [0.73
+00002230: 3032 3935 3639 3233 3631 3733 3732 2c20  02956923617372, 
+00002240: 302e 3235 3635 3030 3534 3435 3332 3239  0.25650054453229
+00002250: 3233 5d0a 2020 2020 2020 2020 6060 600a  23].        ```.
+00002260: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00002270: 2023 2323 2056 6973 7561 6c20 4665 6174   ### Visual Feat
+00002280: 7572 6520 496d 706f 7274 616e 6365 0a20  ure Importance. 
+00002290: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000022a0: 5368 6f77 2066 6561 7475 7265 2077 6569  Show feature wei
+000022b0: 6768 7473 206f 6620 6d6f 6465 6c2c 2061  ghts of model, a
+000022c0: 6e64 2070 7265 6469 6374 696f 6e20 776f  nd prediction wo
+000022d0: 7264 2077 6569 6768 742c 2066 6f72 2065  rd weight, for e
+000022e0: 7861 6d70 6c65 205b 6578 616d 706c 6573  xample [examples
+000022f0: 2f76 6973 7561 6c5f 6665 6174 7572 655f  /visual_feature_
+00002300: 696d 706f 7274 616e 6365 2e69 7079 6e62  importance.ipynb
+00002310: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002320: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
+00002330: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00002340: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00002350: 6d70 6c65 732f 7669 7375 616c 5f66 6561  mples/visual_fea
+00002360: 7475 7265 5f69 6d70 6f72 7461 6e63 652e  ture_importance.
+00002370: 6970 796e 6229 0a20 2020 2020 2020 200a  ipynb).        .
+00002380: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00002390: 6e0a 2020 2020 2020 2020 696d 706f 7274  n.        import
+000023a0: 2073 7973 0a20 2020 2020 2020 200a 2020   sys.        .  
+000023b0: 2020 2020 2020 7379 732e 7061 7468 2e61        sys.path.a
+000023c0: 7070 656e 6428 272e 2e27 290a 2020 2020  ppend('..').    
+000023d0: 2020 2020 6672 6f6d 2070 7974 6578 7463      from pytextc
+000023e0: 6c61 7373 6966 6965 7220 696d 706f 7274  lassifier import
+000023f0: 2043 6c61 7373 6963 436c 6173 7369 6669   ClassicClassifi
+00002400: 6572 0a20 2020 2020 2020 2069 6d70 6f72  er.        impor
+00002410: 7420 6a69 6562 610a 2020 2020 2020 2020  t jieba.        
+00002420: 0a20 2020 2020 2020 2074 6320 3d20 436c  .        tc = Cl
+00002430: 6173 7369 6343 6c61 7373 6966 6965 7228  assicClassifier(
+00002440: 6f75 7470 7574 5f64 6972 3d27 6d6f 6465  output_dir='mode
+00002450: 6c73 2f6c 722d 746f 7927 2c20 6d6f 6465  ls/lr-toy', mode
+00002460: 6c5f 6e61 6d65 5f6f 725f 6d6f 6465 6c3d  l_name_or_model=
+00002470: 276c 7227 290a 2020 2020 2020 2020 6461  'lr').        da
+00002480: 7461 203d 205b 0a20 2020 2020 2020 2020  ta = [.         
+00002490: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+000024a0: 2027 e590 8de5 b888 e68c 87e5 afbc e689   '..............
+000024b0: 98e7 a68f e8af ade6 b395 e68a 80e5 b7a7  ................
+000024c0: efbc 9ae5 908d e8af 8de7 9a84 e5a4 8de6  ................
+000024d0: 95b0 e5bd a2e5 bc8f 2729 2c0a 2020 2020  ........'),.    
+000024e0: 2020 2020 2020 2020 2827 6564 7563 6174          ('educat
+000024f0: 696f 6e27 2c20 27e4 b8ad e59b bde9 ab98  ion', '.........
+00002500: e880 83e6 8890 e7bb a9e6 b5b7 e5a4 96e8  ................
+00002510: aea4 e58f af20 e698 afe2 809c e78b bce6  ..... ..........
+00002520: 9da5 e4ba 86e2 809d e590 97ef bc9f 2729  ..............')
+00002530: 2c0a 2020 2020 2020 2020 2020 2020 2827  ,.            ('
+00002540: 7370 6f72 7473 272c 2027 e59b bee6 9687  sports', '......
+00002550: efbc 9ae6 b395 e7bd 91e5 ad9f e88f b2e5  ................
+00002560: b094 e696 afe8 8ba6 e688 98e8 bf9b 3136  ..............16
+00002570: e5bc ba20 e5ad 9fe8 8fb2 e5b0 94e6 96af  ... ............
+00002580: e680 92e5 90bc 2729 2c0a 2020 2020 2020  ......'),.      
+00002590: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
+000025a0: 2027 e59b 9be5 b79d e4b8 b9e6 a3b1 e4b8   '..............
+000025b0: bee8 a18c e585 a8e5 9bbd e995 bfe8 b79d  ................
+000025c0: e799 bbe5 b1b1 e68c 91e6 8898 e8b5 9b20  ............... 
+000025d0: e8bf 91e4 b887 e4ba bae5 8f82 e4b8 8e27  ...............'
+000025e0: 292c 0a20 2020 2020 2020 2020 2020 2028  ),.            (
+000025f0: 2773 706f 7274 7327 2c20 27e7 b1b3 e585  'sports', '.....
+00002600: b0e5 aea2 e59c ba38 e688 98e4 b88d e8b4  .......8........
+00002610: a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8  .......10.......
+00002620: 839c 2729 0a20 2020 2020 2020 205d 0a20  ..').        ]. 
+00002630: 2020 2020 2020 2074 632e 7472 6169 6e28         tc.train(
+00002640: 6461 7461 290a 2020 2020 2020 2020 696d  data).        im
+00002650: 706f 7274 2065 6c69 350a 2020 2020 2020  port eli5.      
+00002660: 2020 0a20 2020 2020 2020 2069 6e66 6572    .        infer
+00002670: 5f64 6174 6120 3d20 5b27 e9ab 98e8 8083  _data = ['......
+00002680: e68c 87e5 afbc e689 98e7 a68f e8af ade6  ................
+00002690: b395 e68a 80e5 b7a7 e59b bde9 9985 e8ae  ................
+000026a0: a4e5 8faf 272c 0a20 2020 2020 2020 2020  ....',.         
+000026b0: 2020 2020 2020 2020 2020 2020 2027 e684               '..
+000026c0: 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b  ................
+000026d0: e4ba a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3  ............:...
+000026e0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+000026f0: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+00002700: 9ee8 839c 275d 0a20 2020 2020 2020 2065  ....'].        e
+00002710: 6c69 352e 7368 6f77 5f77 6569 6768 7473  li5.show_weights
+00002720: 2874 632e 6d6f 6465 6c2c 2076 6563 3d74  (tc.model, vec=t
+00002730: 632e 6665 6174 7572 6529 0a20 2020 2020  c.feature).     
+00002740: 2020 2073 6567 5f69 6e66 6572 5f64 6174     seg_infer_dat
+00002750: 6120 3d20 5b27 2027 2e6a 6f69 6e28 6a69  a = [' '.join(ji
+00002760: 6562 612e 6c63 7574 2869 2929 2066 6f72  eba.lcut(i)) for
+00002770: 2069 2069 6e20 696e 6665 725f 6461 7461   i in infer_data
+00002780: 5d0a 2020 2020 2020 2020 656c 6935 2e73  ].        eli5.s
+00002790: 686f 775f 7072 6564 6963 7469 6f6e 2874  how_prediction(t
+000027a0: 632e 6d6f 6465 6c2c 2073 6567 5f69 6e66  c.model, seg_inf
+000027b0: 6572 5f64 6174 615b 305d 2c20 7665 633d  er_data[0], vec=
+000027c0: 7463 2e66 6561 7475 7265 2c0a 2020 2020  tc.feature,.    
+000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027e0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+000027f0: 6e61 6d65 733d 5b27 6564 7563 6174 696f  names=['educatio
+00002800: 6e27 2c20 2773 706f 7274 7327 5d29 0a20  n', 'sports']). 
+00002810: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00002820: 2020 200a 2020 2020 2020 2020 6f75 7470     .        outp
+00002830: 7574 3a0a 2020 2020 2020 2020 0a20 2020  ut:.        .   
+00002840: 2020 2020 2021 5b69 6d67 2e70 6e67 5d28       ![img.png](
+00002850: 646f 6373 2f69 6d67 2e70 6e67 290a 2020  docs/img.png).  
+00002860: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00002870: 2323 2044 6565 7020 436c 6173 7369 6669  ## Deep Classifi
+00002880: 6361 7469 6f6e 206d 6f64 656c 0a20 2020  cation model.   
+00002890: 2020 2020 200a 2020 2020 2020 2020 e69c       .        ..
+000028a0: ace9 a1b9 e79b aee6 94af e68c 81e4 bba5  ................
+000028b0: e4b8 8be6 b7b1 e5ba a6e5 8886 e7b1 bbe6  ................
+000028c0: a8a1 e59e 8bef bc9a 4661 7374 5465 7874  ........FastText
+000028d0: e380 8154 6578 7443 4e4e e380 8154 6578  ...TextCNN...Tex
+000028e0: 7452 4e4e e380 8142 6572 74e6 a8a1 e59e  tRNN...Bert.....
+000028f0: 8bef bc8c 6069 6d70 6f72 7460 e6a8 a1e5  ....`import`....
+00002900: 9e8b e5af b9e5 ba94 e79a 84e6 96b9 e6b3  ................
+00002910: 95e6 9da5 e8b0 83e7 94a8 efbc 9a0a 2020  ..............  
+00002920: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00002930: 2020 2020 2020 2020 6672 6f6d 2070 7974          from pyt
+00002940: 6578 7463 6c61 7373 6966 6965 7220 696d  extclassifier im
+00002950: 706f 7274 2046 6173 7454 6578 7443 6c61  port FastTextCla
+00002960: 7373 6966 6965 722c 2054 6578 7443 4e4e  ssifier, TextCNN
+00002970: 436c 6173 7369 6669 6572 2c20 5465 7874  Classifier, Text
+00002980: 524e 4e43 6c61 7373 6966 6965 722c 2042  RNNClassifier, B
+00002990: 6572 7443 6c61 7373 6966 6965 720a 2020  ertClassifier.  
+000029a0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+000029b0: 2020 0a20 2020 2020 2020 20e4 b88b e99d    .        .....
+000029c0: a2e4 bba5 4661 7374 5465 7874 e6a8 a1e5  ....FastText....
+000029d0: 9e8b e4b8 bae7 a4ba e4be 8bef bc8c e585  ................
+000029e0: b6e4 bb96 e6a8 a1e5 9e8b e79a 84e4 bdbf  ................
+000029f0: e794 a8e6 96b9 e6b3 95e7 b1bb e4bc bce3  ................
+00002a00: 8082 0a20 2020 2020 2020 200a 2020 2020  ...        .    
+00002a10: 2020 2020 2323 2320 4661 7374 5465 7874      ### FastText
+00002a20: 20e6 a8a1 e59e 8b0a 2020 2020 2020 2020   .......        
+00002a30: 0a20 2020 2020 2020 20e8 aead e7bb 83e5  .        .......
+00002a40: 928c e9a2 84e6 b58b 6046 6173 7454 6578  ........`FastTex
+00002a50: 7460 e6a8 a1e5 9e8b e7a4 bae4 be8b 5b65  t`............[e
+00002a60: 7861 6d70 6c65 732f 6661 7374 7465 7874  xamples/fasttext
+00002a70: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
+00002a80: 6465 6d6f 2e70 795d 2868 7474 7073 3a2f  demo.py](https:/
+00002a90: 2f67 6974 6875 622e 636f 6d2f 7368 6962  /github.com/shib
+00002aa0: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
+00002ab0: 7373 6966 6965 722f 626c 6f62 2f6d 6173  ssifier/blob/mas
+00002ac0: 7465 722f 6578 616d 706c 6573 2f66 6173  ter/examples/fas
+00002ad0: 7474 6578 745f 636c 6173 7369 6669 6361  ttext_classifica
+00002ae0: 7469 6f6e 5f64 656d 6f2e 7079 290a 2020  tion_demo.py).  
+00002af0: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
+00002b00: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
+00002b10: 2069 6d70 6f72 7420 7379 730a 2020 2020   import sys.    
+00002b20: 2020 2020 0a20 2020 2020 2020 2073 7973      .        sys
+00002b30: 2e70 6174 682e 6170 7065 6e64 2827 2e2e  .path.append('..
+00002b40: 2729 0a20 2020 2020 2020 2066 726f 6d20  ').        from 
+00002b50: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
+00002b60: 2069 6d70 6f72 7420 4661 7374 5465 7874   import FastText
+00002b70: 436c 6173 7369 6669 6572 2c20 6c6f 6164  Classifier, load
+00002b80: 5f64 6174 610a 2020 2020 2020 2020 0a20  _data.        . 
+00002b90: 2020 2020 2020 2069 6620 5f5f 6e61 6d65         if __name
+00002ba0: 5f5f 203d 3d20 275f 5f6d 6169 6e5f 5f27  __ == '__main__'
+00002bb0: 3a0a 2020 2020 2020 2020 2020 2020 6d20  :.            m 
+00002bc0: 3d20 4661 7374 5465 7874 436c 6173 7369  = FastTextClassi
+00002bd0: 6669 6572 286f 7574 7075 745f 6469 723d  fier(output_dir=
+00002be0: 276d 6f64 656c 732f 6661 7374 7465 7874  'models/fasttext
+00002bf0: 2d74 6f79 2729 0a20 2020 2020 2020 2020  -toy').         
+00002c00: 2020 2064 6174 6120 3d20 5b0a 2020 2020     data = [.    
+00002c10: 2020 2020 2020 2020 2020 2020 2827 6564              ('ed
+00002c20: 7563 6174 696f 6e27 2c20 27e5 908d e5b8  ucation', '.....
+00002c30: 88e6 8c87 e5af bce6 8998 e7a6 8fe8 afad  ................
+00002c40: e6b3 95e6 8a80 e5b7 a7ef bc9a e590 8de8  ................
+00002c50: af8d e79a 84e5 a48d e695 b0e5 bda2 e5bc  ................
+00002c60: 8f27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
+00002c70: 2020 2020 2028 2765 6475 6361 7469 6f6e       ('education
+00002c80: 272c 2027 e4b8 ade5 9bbd e9ab 98e8 8083  ', '............
+00002c90: e688 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5  ................
+00002ca0: 8faf 20e6 98af e280 9ce7 8bbc e69d a5e4  .. .............
+00002cb0: ba86 e280 9de5 9097 efbc 9f27 292c 0a20  ...........'),. 
+00002cc0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00002cd0: 2765 6475 6361 7469 6f6e 272c 2027 e585  'education', '..
+00002ce0: ace5 8aa1 e591 98e8 8083 e899 91e8 b68a  ................
+00002cf0: e69d a5e8 b68a e590 83e9 a699 efbc 8ce8  ................
+00002d00: bf99 e698 afe6 808e e4b9 88e5 9b9e e4ba  ................
+00002d10: 8bef bc9f 2729 2c0a 2020 2020 2020 2020  ....'),.        
+00002d20: 2020 2020 2020 2020 2827 7370 6f72 7473          ('sports
+00002d30: 272c 2027 e59b bee6 9687 efbc 9ae6 b395  ', '............
+00002d40: e7bd 91e5 ad9f e88f b2e5 b094 e696 afe8  ................
+00002d50: 8ba6 e688 98e8 bf9b 3136 e5bc ba20 e5ad  ........16... ..
+00002d60: 9fe8 8fb2 e5b0 94e6 96af e680 92e5 90bc  ................
+00002d70: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00002d80: 2020 2020 2827 7370 6f72 7473 272c 2027      ('sports', '
+00002d90: e59b 9be5 b79d e4b8 b9e6 a3b1 e4b8 bee8  ................
+00002da0: a18c e585 a8e5 9bbd e995 bfe8 b79d e799  ................
+00002db0: bbe5 b1b1 e68c 91e6 8898 e8b5 9b20 e8bf  ............. ..
+00002dc0: 91e4 b887 e4ba bae5 8f82 e4b8 8e27 292c  .............'),
+00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002de0: 2028 2773 706f 7274 7327 2c20 27e7 b1b3   ('sports', '...
+00002df0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+00002e00: e8b4 a5e4 bf9d e68c 81e8 bf9e e883 9c27  ...............'
+00002e10: 292c 0a20 2020 2020 2020 2020 2020 205d  ),.            ]
+00002e20: 0a20 2020 2020 2020 2020 2020 206d 2e74  .            m.t
+00002e30: 7261 696e 2864 6174 612c 206e 756d 5f65  rain(data, num_e
+00002e40: 706f 6368 733d 3329 0a20 2020 2020 2020  pochs=3).       
+00002e50: 2020 2020 2070 7269 6e74 286d 290a 2020       print(m).  
+00002e60: 2020 2020 2020 2020 2020 2320 6c6f 6164            # load
+00002e70: 2074 7261 696e 6564 2062 6573 7420 6d6f   trained best mo
+00002e80: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
+00002e90: 6d2e 6c6f 6164 5f6d 6f64 656c 2829 0a20  m.load_model(). 
+00002ea0: 2020 2020 2020 2020 2020 2070 7265 6469             predi
+00002eb0: 6374 5f6c 6162 656c 2c20 7072 6564 6963  ct_label, predic
+00002ec0: 745f 7072 6f62 6120 3d20 6d2e 7072 6564  t_proba = m.pred
+00002ed0: 6963 7428 5b27 e7a6 8fe5 bbba e698 a5e5  ict(['..........
+00002ee0: ada3 e585 ace5 8aa1 e591 98e8 8083 e8af  ................
+00002ef0: 95e6 8aa5 e590 8d31 38e6 97a5 e688 aae6  .......18.......
+00002f00: ada2 2032 e69c 8836 e697 a5e8 8083 e8af  .. 2...6........
+00002f10: 9527 2c0a 2020 2020 2020 2020 2020 2020  .',.            
+00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f40: 2020 2020 2020 2020 2020 27e6 848f e794            '.....
+00002f50: b2e9 a696 e8bd aee8 a1a5 e8b5 9be4 baa4  ................
+00002f60: e688 98e8 aeb0 e5bd 953a e7b1 b3e5 85b0  .........:......
+00002f70: e5ae a2e5 9cba 38e6 8898 e4b8 8de8 b4a5  ......8.........
+00002f80: e59b bde7 b1b3 3130 e5b9 b4e8 bf9e e883  ......10........
+00002f90: 9c27 5d29 0a20 2020 2020 2020 2020 2020  .']).           
+00002fa0: 2070 7269 6e74 2866 2770 7265 6469 6374   print(f'predict
+00002fb0: 5f6c 6162 656c 3a20 7b70 7265 6469 6374  _label: {predict
+00002fc0: 5f6c 6162 656c 7d2c 2070 7265 6469 6374  _label}, predict
+00002fd0: 5f70 726f 6261 3a20 7b70 7265 6469 6374  _proba: {predict
+00002fe0: 5f70 726f 6261 7d27 290a 2020 2020 2020  _proba}').      
+00002ff0: 2020 2020 2020 7465 7374 5f64 6174 6120        test_data 
+00003000: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00003010: 2020 2020 2827 6564 7563 6174 696f 6e27      ('education'
+00003020: 2c20 27e7 a68f e5bb bae6 98a5 e5ad a3e5  , '.............
+00003030: 85ac e58a a1e5 9198 e880 83e8 af95 e68a  ................
+00003040: a5e5 908d 3138 e697 a5e6 88aa e6ad a220  ....18......... 
+00003050: 32e6 9c88 36e6 97a5 e880 83e8 af95 2729  2...6.........')
+00003060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003070: 2020 2827 7370 6f72 7473 272c 2027 e684    ('sports', '..
+00003080: 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b  ................
+00003090: e4ba a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3  ............:...
+000030a0: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
+000030b0: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
+000030c0: 9ee8 839c 2729 2c0a 2020 2020 2020 2020  ....'),.        
+000030d0: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+000030e0: 2020 6163 635f 7363 6f72 6520 3d20 6d2e    acc_score = m.
+000030f0: 6576 616c 7561 7465 5f6d 6f64 656c 2874  evaluate_model(t
+00003100: 6573 745f 6461 7461 290a 2020 2020 2020  est_data).      
+00003110: 2020 2020 2020 7072 696e 7428 6627 6163        print(f'ac
+00003120: 635f 7363 6f72 653a 207b 6163 635f 7363  c_score: {acc_sc
+00003130: 6f72 657d 2729 2020 2320 312e 300a 2020  ore}')  # 1.0.  
+00003140: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00003150: 2020 2023 2323 2320 7472 6169 6e20 6d6f     #### train mo
+00003160: 6465 6c20 7769 7468 2031 7720 6461 7461  del with 1w data
+00003170: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00003180: 6e74 2827 2d27 202a 2034 3229 0a20 2020  nt('-' * 42).   
+00003190: 2020 2020 2020 2020 2064 6174 615f 6669           data_fi
+000031a0: 6c65 203d 2027 7468 7563 6e65 7773 5f74  le = 'thucnews_t
+000031b0: 7261 696e 5f31 772e 7478 7427 0a20 2020  rain_1w.txt'.   
+000031c0: 2020 2020 2020 2020 206d 203d 2046 6173           m = Fas
+000031d0: 7454 6578 7443 6c61 7373 6966 6965 7228  tTextClassifier(
+000031e0: 6f75 7470 7574 5f64 6972 3d27 6d6f 6465  output_dir='mode
+000031f0: 6c73 2f66 6173 7474 6578 7427 290a 2020  ls/fasttext').  
+00003200: 2020 2020 2020 2020 2020 6d2e 7472 6169            m.trai
+00003210: 6e28 6461 7461 5f66 696c 652c 206e 616d  n(data_file, nam
+00003220: 6573 3d28 276c 6162 656c 7327 2c20 2774  es=('labels', 't
+00003230: 6578 7427 292c 206e 756d 5f65 706f 6368  ext'), num_epoch
+00003240: 733d 3329 0a20 2020 2020 2020 2020 2020  s=3).           
+00003250: 2023 206c 6f61 6420 6265 7374 2074 7261   # load best tra
+00003260: 696e 6564 206d 6f64 656c 2066 726f 6d20  ined model from 
+00003270: 6d6f 6465 6c5f 6469 720a 2020 2020 2020  model_dir.      
+00003280: 2020 2020 2020 6d2e 6c6f 6164 5f6d 6f64        m.load_mod
+00003290: 656c 2829 0a20 2020 2020 2020 2020 2020  el().           
+000032a0: 2070 7265 6469 6374 5f6c 6162 656c 2c20   predict_label, 
+000032b0: 7072 6564 6963 745f 7072 6f62 6120 3d20  predict_proba = 
+000032c0: 6d2e 7072 6564 6963 7428 0a20 2020 2020  m.predict(.     
+000032d0: 2020 2020 2020 2020 2020 205b 27e9 a1ba             ['...
+000032e0: e4b9 89e5 8c97 e4ba ace8 8b8f e6b4 bb38  ...............8
+000032f0: 38e5 b9b3 e7b1 b3e8 b5b7 e7b2 bee8 a385  8...............
+00003300: e688 bfe5 9ca8 e594 ae27 2c0a 2020 2020  .........',.    
+00003310: 2020 2020 2020 2020 2020 2020 2027 e7be               '..
+00003320: 8e45 422d 35e9 a1b9 e79b aee2 809c 3135  .EB-5.........15
+00003330: e697 a5e5 bfab e980 9fe7 a7bb e6b0 91e2  ................
+00003340: 809d e5b0 86e6 8ea8 e8bf 9f27 5d0a 2020  ...........'].  
+00003350: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00003360: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00003370: 7072 6564 6963 745f 6c61 6265 6c3a 207b  predict_label: {
+00003380: 7072 6564 6963 745f 6c61 6265 6c7d 2c20  predict_label}, 
+00003390: 7072 6564 6963 745f 7072 6f62 613a 207b  predict_proba: {
+000033a0: 7072 6564 6963 745f 7072 6f62 617d 2729  predict_proba}')
+000033b0: 0a20 2020 2020 2020 2020 2020 2078 2c20  .            x, 
+000033c0: 792c 2064 6620 3d20 6c6f 6164 5f64 6174  y, df = load_dat
+000033d0: 6128 6461 7461 5f66 696c 6529 0a20 2020  a(data_file).   
+000033e0: 2020 2020 2020 2020 2074 6573 745f 6461           test_da
+000033f0: 7461 203d 2064 665b 3a31 3030 5d0a 2020  ta = df[:100].  
+00003400: 2020 2020 2020 2020 2020 6163 635f 7363            acc_sc
+00003410: 6f72 6520 3d20 6d2e 6576 616c 7561 7465  ore = m.evaluate
+00003420: 5f6d 6f64 656c 2874 6573 745f 6461 7461  _model(test_data
+00003430: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00003440: 696e 7428 6627 6163 635f 7363 6f72 653a  int(f'acc_score:
+00003450: 207b 6163 635f 7363 6f72 657d 2729 0a20   {acc_score}'). 
+00003460: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00003470: 2020 200a 2020 2020 2020 2020 2323 2320     .        ### 
+00003480: 4245 5254 20e7 b1bb e6a8 a1e5 9e8b 0a20  BERT .......... 
+00003490: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000034a0: 2323 2323 20e5 a49a e588 86e7 b1bb e6a8  #### ...........
+000034b0: a1e5 9e8b 0a20 2020 2020 2020 20e8 aead  .....        ...
+000034c0: e7bb 83e5 928c e9a2 84e6 b58b 6042 4552  ............`BER
+000034d0: 5460 e5a4 9ae5 8886 e7b1 bbe6 a8a1 e59e  T`..............
+000034e0: 8bef bc8c e7a4 bae4 be8b 5b65 7861 6d70  ..........[examp
+000034f0: 6c65 732f 6265 7274 5f63 6c61 7373 6966  les/bert_classif
+00003500: 6963 6174 696f 6e5f 7a68 5f64 656d 6f2e  ication_zh_demo.
+00003510: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
+00003520: 7562 2e63 6f6d 2f73 6869 6269 6e67 3632  ub.com/shibing62
+00003530: 342f 7079 7465 7874 636c 6173 7369 6669  4/pytextclassifi
+00003540: 6572 2f62 6c6f 622f 6d61 7374 6572 2f65  er/blob/master/e
+00003550: 7861 6d70 6c65 732f 6265 7274 5f63 6c61  xamples/bert_cla
+00003560: 7373 6966 6963 6174 696f 6e5f 7a68 5f64  ssification_zh_d
+00003570: 656d 6f2e 7079 290a 2020 2020 2020 2020  emo.py).        
+00003580: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
+00003590: 6f6e 0a20 2020 2020 2020 2069 6d70 6f72  on.        impor
+000035a0: 7420 7379 730a 2020 2020 2020 2020 0a20  t sys.        . 
+000035b0: 2020 2020 2020 2073 7973 2e70 6174 682e         sys.path.
+000035c0: 6170 7065 6e64 2827 2e2e 2729 0a20 2020  append('..').   
+000035d0: 2020 2020 2066 726f 6d20 7079 7465 7874       from pytext
+000035e0: 636c 6173 7369 6669 6572 2069 6d70 6f72  classifier impor
+000035f0: 7420 4265 7274 436c 6173 7369 6669 6572  t BertClassifier
+00003600: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00003610: 2020 6966 205f 5f6e 616d 655f 5f20 3d3d    if __name__ ==
+00003620: 2027 5f5f 6d61 696e 5f5f 273a 0a20 2020   '__main__':.   
+00003630: 2020 2020 2020 2020 206d 203d 2042 6572           m = Ber
+00003640: 7443 6c61 7373 6966 6965 7228 6f75 7470  tClassifier(outp
+00003650: 7574 5f64 6972 3d27 6d6f 6465 6c73 2f62  ut_dir='models/b
+00003660: 6572 742d 6368 696e 6573 652d 746f 7927  ert-chinese-toy'
+00003670: 2c20 6e75 6d5f 636c 6173 7365 733d 322c  , num_classes=2,
 00003680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003690: 2028 2773 706f 7274 7327 2c20 27e5 9b9b   ('sports', '...
-000036a0: e5b7 9de4 b8b9 e6a3 b1e4 b8be e8a1 8ce5  ................
-000036b0: 85a8 e59b bde9 95bf e8b7 9de7 99bb e5b1  ................
-000036c0: b1e6 8c91 e688 98e8 b59b 20e8 bf91 e4b8  .......... .....
-000036d0: 87e4 baba e58f 82e4 b88e 2729 2c0a 2020  ..........'),.  
-000036e0: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-000036f0: 7370 6f72 7473 272c 2027 e7b1 b3e5 85b0  sports', '......
-00003700: e5ae a2e5 9cba 38e6 8898 e4b8 8de8 b4a5  ......8.........
-00003710: e59b bde7 b1b3 3130 e5b9 b4e8 bf9e e883  ......10........
-00003720: 9c27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
-00003730: 205d 0a20 2020 2020 2020 2020 2020 206d   ].            m
-00003740: 2e74 7261 696e 2864 6174 6129 0a20 2020  .train(data).   
-00003750: 2020 2020 2020 2020 2070 7269 6e74 286d           print(m
-00003760: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-00003770: 6c6f 6164 2074 7261 696e 6564 2062 6573  load trained bes
-00003780: 7420 6d6f 6465 6c20 6672 6f6d 206d 6f64  t model from mod
-00003790: 656c 5f64 6972 0a20 2020 2020 2020 2020  el_dir.         
-000037a0: 2020 206d 2e6c 6f61 645f 6d6f 6465 6c28     m.load_model(
-000037b0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-000037c0: 6564 6963 745f 6c61 6265 6c2c 2070 7265  edict_label, pre
-000037d0: 6469 6374 5f70 726f 6261 203d 206d 2e70  dict_proba = m.p
-000037e0: 7265 6469 6374 285b 27e7 a68f e5bb bae6  redict(['.......
-000037f0: 98a5 e5ad a3e5 85ac e58a a1e5 9198 e880  ................
-00003800: 83e8 af95 e68a a5e5 908d 3138 e697 a5e6  ..........18....
-00003810: 88aa e6ad a220 32e6 9c88 36e6 97a5 e880  ..... 2...6.....
-00003820: 83e8 af95 272c 0a20 2020 2020 2020 2020  ....',.         
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 2020 2020 2020 2020 2020 2027 e684               '..
-00003860: 8fe7 94b2 e9a6 96e8 bdae e8a1 a5e8 b59b  ................
-00003870: e4ba a4e6 8898 e8ae b0e5 bd95 3ae7 b1b3  ............:...
-00003880: e585 b0e5 aea2 e59c ba38 e688 98e4 b88d  .........8......
-00003890: e8b4 a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf  .........10.....
-000038a0: 9ee8 839c 275d 290a 2020 2020 2020 2020  ....']).        
-000038b0: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
-000038c0: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
-000038d0: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
-000038e0: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
-000038f0: 6963 745f 7072 6f62 617d 2729 0a20 2020  ict_proba}').   
-00003900: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00003910: 2020 7465 7374 5f64 6174 6120 3d20 5b0a    test_data = [.
-00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003930: 2827 6564 7563 6174 696f 6e27 2c20 27e7  ('education', '.
-00003940: a68f e5bb bae6 98a5 e5ad a3e5 85ac e58a  ................
-00003950: a1e5 9198 e880 83e8 af95 e68a a5e5 908d  ................
-00003960: 3138 e697 a5e6 88aa e6ad a220 32e6 9c88  18......... 2...
-00003970: 36e6 97a5 e880 83e8 af95 2729 2c0a 2020  6.........'),.  
-00003980: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-00003990: 7370 6f72 7473 272c 2027 e684 8fe7 94b2  sports', '......
-000039a0: e9a6 96e8 bdae e8a1 a5e8 b59b e4ba a4e6  ................
-000039b0: 8898 e8ae b0e5 bd95 3ae7 b1b3 e585 b0e5  ........:.......
-000039c0: aea2 e59c ba38 e688 98e4 b88d e8b4 a5e5  .....8..........
-000039d0: 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8 839c  .....10.........
-000039e0: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-000039f0: 5d0a 2020 2020 2020 2020 2020 2020 6163  ].            ac
-00003a00: 635f 7363 6f72 6520 3d20 6d2e 6576 616c  c_score = m.eval
-00003a10: 7561 7465 5f6d 6f64 656c 2874 6573 745f  uate_model(test_
-00003a20: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00003a30: 2020 7072 696e 7428 6627 6163 635f 7363    print(f'acc_sc
-00003a40: 6f72 653a 207b 6163 635f 7363 6f72 657d  ore: {acc_score}
-00003a50: 2729 0a20 2020 2020 2020 2020 2020 200a  ').            .
-00003a60: 2020 2020 2020 2020 2020 2020 2320 7472              # tr
-00003a70: 6169 6e20 6d6f 6465 6c20 7769 7468 2031  ain model with 1
-00003a80: 7720 6461 7461 2066 696c 6520 616e 6420  w data file and 
-00003a90: 3130 2063 6c61 7373 6573 0a20 2020 2020  10 classes.     
-00003aa0: 2020 2020 2020 2070 7269 6e74 2827 2d27         print('-'
-00003ab0: 202a 2034 3229 0a20 2020 2020 2020 2020   * 42).         
-00003ac0: 2020 206d 203d 2042 6572 7443 6c61 7373     m = BertClass
-00003ad0: 6966 6965 7228 6d6f 6465 6c5f 6469 723d  ifier(model_dir=
-00003ae0: 276d 6f64 656c 732f 6265 7274 2d63 6869  'models/bert-chi
-00003af0: 6e65 7365 272c 206e 756d 5f63 6c61 7373  nese', num_class
-00003b00: 6573 3d31 302c 0a20 2020 2020 2020 2020  es=10,.         
-00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b20: 2020 2020 2020 6d6f 6465 6c5f 7479 7065        model_type
-00003b30: 3d27 6265 7274 272c 206d 6f64 656c 5f6e  ='bert', model_n
-00003b40: 616d 653d 2762 6572 742d 6261 7365 2d63  ame='bert-base-c
-00003b50: 6869 6e65 7365 272c 206e 756d 5f65 706f  hinese', num_epo
-00003b60: 6368 733d 322c 0a20 2020 2020 2020 2020  chs=2,.         
-00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 2020 2020 2020 6172 6773 3d7b 226e 6f5f        args={"no_
-00003b90: 6361 6368 6522 3a20 5472 7565 2c20 226c  cache": True, "l
-00003ba0: 617a 795f 6c6f 6164 696e 6722 3a20 5472  azy_loading": Tr
-00003bb0: 7565 2c20 226c 617a 795f 7465 7874 5f63  ue, "lazy_text_c
-00003bc0: 6f6c 756d 6e22 3a20 312c 2022 6c61 7a79  olumn": 1, "lazy
-00003bd0: 5f6c 6162 656c 735f 636f 6c75 6d6e 223a  _labels_column":
-00003be0: 2030 2c20 7d29 0a20 2020 2020 2020 2020   0, }).         
-00003bf0: 2020 2064 6174 615f 6669 6c65 203d 2027     data_file = '
-00003c00: 7468 7563 6e65 7773 5f74 7261 696e 5f31  thucnews_train_1
-00003c10: 772e 7478 7427 0a20 2020 2020 2020 2020  w.txt'.         
-00003c20: 2020 2023 20e5 a682 e69e 9ce8 aead e7bb     # ...........
-00003c30: 83e6 95b0 e68d aee8 b685 e8bf 87e7 99be  ................
-00003c40: e4b8 87e6 9da1 efbc 8ce5 bbba e8ae aee4  ................
-00003c50: bdbf e794 a86c 617a 795f 6c6f 6164 696e  .....lazy_loadin
-00003c60: 67e6 a8a1 e5bc 8fef bc8c e587 8fe5 b091  g...............
-00003c70: e586 85e5 ad98 e58d a0e7 94a8 0a20 2020  .............   
-00003c80: 2020 2020 2020 2020 206d 2e74 7261 696e           m.train
-00003c90: 2864 6174 615f 6669 6c65 2c20 7465 7374  (data_file, test
-00003ca0: 5f73 697a 653d 302c 206e 616d 6573 3d28  _size=0, names=(
-00003cb0: 276c 6162 656c 7327 2c20 2774 6578 7427  'labels', 'text'
-00003cc0: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
-00003cd0: 2e6c 6f61 645f 6d6f 6465 6c28 290a 2020  .load_model().  
-00003ce0: 2020 2020 2020 2020 2020 7072 6564 6963            predic
-00003cf0: 745f 6c61 6265 6c2c 2070 7265 6469 6374  t_label, predict
-00003d00: 5f70 726f 6261 203d 206d 2e70 7265 6469  _proba = m.predi
-00003d10: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-00003d20: 2020 2020 5b27 e9a1 bae4 b989 e58c 97e4      ['..........
-00003d30: baac e88b 8fe6 b4bb 3838 e5b9 b3e7 b1b3  ........88......
-00003d40: e8b5 b7e7 b2be e8a3 85e6 88bf e59c a8e5  ................
-00003d50: 94ae 272c 0a20 2020 2020 2020 2020 2020  ..',.           
-00003d60: 2020 2020 2020 27e7 be8e 4542 2d35 e9a1        '...EB-5..
-00003d70: b9e7 9bae e280 9c31 35e6 97a5 e5bf abe9  .......15.......
-00003d80: 809f e7a7 bbe6 b091 e280 9de5 b086 e68e  ................
-00003d90: a8e8 bf9f 272c 0a20 2020 2020 2020 2020  ....',.         
-00003da0: 2020 2020 2020 2020 27e6 8192 e794 9f41          '......A
-00003db0: 48e6 baa2 e68c 87e6 94b6 e5b9 b320 41e8  H............ A.
-00003dc0: 82a1 e5af b948 e882 a1e6 8a98 e4bb b731  .....H.........1
-00003dd0: 2e39 3525 275d 290a 2020 2020 2020 2020  .95%']).        
-00003de0: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
-00003df0: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
-00003e00: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
-00003e10: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
-00003e20: 6963 745f 7072 6f62 617d 2729 0a20 2020  ict_proba}').   
-00003e30: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
-00003e40: 2050 53ef bc9a e5a6 82e6 9e9c e8ae ade7   PS.............
-00003e50: bb83 e695 b0e6 8dae e8b6 85e8 bf87 e799  ................
-00003e60: bee4 b887 e69d a1ef bc8c e5bb bae8 aeae  ................
-00003e70: e4bd bfe7 94a8 6c61 7a79 5f6c 6f61 6469  ......lazy_loadi
-00003e80: 6e67 e6a8 a1e5 bc8f efbc 8ce5 878f e5b0  ng..............
-00003e90: 91e5 8685 e5ad 98e5 8da0 e794 a80a 2020  ..............  
-00003ea0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00003eb0: 2323 2320 e5a4 9ae6 a087 e7ad bee5 8886  ### ............
-00003ec0: e7b1 bbe6 a8a1 e59e 8b0a 2020 2020 2020  ..........      
-00003ed0: 2020 e588 86e7 b1bb e58f afe4 bba5 e588    ..............
-00003ee0: 86e4 b8ba e5a4 9ae5 8886 e7b1 bbe5 928c  ................
-00003ef0: e5a4 9ae6 a087 e7ad bee5 8886 e7b1 bbe3  ................
-00003f00: 8082 e5a4 9ae5 8886 e7b1 bbe7 9a84 e6a0  ................
-00003f10: 87e7 adbe e698 afe6 8e92 e4bb 96e7 9a84  ................
-00003f20: efbc 8ce8 808c e5a4 9ae6 a087 e7ad bee5  ................
-00003f30: 8886 e7b1 bbe7 9a84 e689 80e6 9c89 e6a0  ................
-00003f40: 87e7 adbe e698 afe4 b88d e68e 92e4 bb96  ................
-00003f50: e79a 84e3 8082 0a20 2020 2020 2020 200a  .......        .
-00003f60: 2020 2020 2020 2020 e5a4 9ae6 a087 e7ad          ........
-00003f70: bee5 8886 e7b1 bbe6 af94 e8be 83e7 9bb4  ................
-00003f80: e8a7 82e7 9a84 e790 86e8 a7a3 e698 afef  ................
-00003f90: bc8c e4b8 80e4 b8aa e6a0 b7e6 9cac e58f  ................
-00003fa0: afe4 bba5 e590 8ce6 97b6 e68b a5e6 9c89  ................
-00003fb0: e587 a0e4 b8aa e7b1 bbe5 88ab e6a0 87e7  ................
-00003fc0: adbe efbc 8c0a 2020 2020 2020 2020 e6af  ......        ..
-00003fd0: 94e5 a682 e4b8 80e9 a696 e6ad 8ce7 9a84  ................
-00003fe0: e6a0 87e7 adbe e58f afe4 bba5 e698 afe6  ................
-00003ff0: b581 e8a1 8ce3 8081 e8bd bbe5 bfab efbc  ................
-00004000: 8ce4 b880 e983 a8e7 94b5 e5bd b1e7 9a84  ................
-00004010: e6a0 87e7 adbe e58f afe4 bba5 e698 afe5  ................
-00004020: 8aa8 e4bd 9ce3 8081 e596 9ce5 89a7 e380  ................
-00004030: 81e6 909e e7ac 91e7 ad89 efbc 8ce8 bf99  ................
-00004040: e983 bde6 98af e5a4 9ae6 a087 e7ad bee5  ................
-00004050: 8886 e7b1 bbe7 9a84 e683 85e5 86b5 e380  ................
-00004060: 820a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00004070: 2020 20e8 aead e7bb 83e5 928c e9a2 84e6     .............
-00004080: b58b 6042 4552 5460 e5a4 9ae6 a087 e7ad  ..`BERT`........
-00004090: bee5 8886 e7b1 bbe6 a8a1 e59e 8bef bc8c  ................
-000040a0: e7a4 bae4 be8b 5b65 7861 6d70 6c65 732f  ......[examples/
-000040b0: 6265 7274 5f6d 756c 7469 6c61 6265 6c5f  bert_multilabel_
-000040c0: 636c 6173 7369 6669 6361 7469 6f6e 5f7a  classification_z
-000040d0: 685f 6465 6d6f 2e70 792e 7079 5d28 6874  h_demo.py.py](ht
-000040e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000040f0: 2f73 6869 6269 6e67 3632 342f 7079 7465  /shibing624/pyte
-00004100: 7874 636c 6173 7369 6669 6572 2f62 6c6f  xtclassifier/blo
-00004110: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
-00004120: 732f 6265 7274 5f6d 756c 7469 6c61 6265  s/bert_multilabe
-00004130: 6c5f 636c 6173 7369 6669 6361 7469 6f6e  l_classification
-00004140: 5f7a 685f 6465 6d6f 2e70 7929 0a20 2020  _zh_demo.py).   
-00004150: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
-00004160: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-00004170: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00004180: 7379 730a 2020 2020 2020 2020 696d 706f  sys.        impo
-00004190: 7274 2070 616e 6461 7320 6173 2070 640a  rt pandas as pd.
-000041a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000041b0: 2073 7973 2e70 6174 682e 6170 7065 6e64   sys.path.append
-000041c0: 2827 2e2e 2729 0a20 2020 2020 2020 2066  ('..').        f
-000041d0: 726f 6d20 7079 7465 7874 636c 6173 7369  rom pytextclassi
-000041e0: 6669 6572 2069 6d70 6f72 7420 4265 7274  fier import Bert
-000041f0: 436c 6173 7369 6669 6572 0a20 2020 2020  Classifier.     
-00004200: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00004210: 2020 2020 2064 6566 206c 6f61 645f 6a64       def load_jd
-00004220: 5f64 6174 6128 6669 6c65 5f70 6174 6829  _data(file_path)
-00004230: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
-00004240: 220a 2020 2020 2020 2020 2020 2020 4c6f  ".            Lo
-00004250: 6164 206a 6420 6461 7461 2066 726f 6d20  ad jd data from 
-00004260: 6669 6c65 2e0a 2020 2020 2020 2020 2020  file..          
-00004270: 2020 4070 6172 616d 2066 696c 655f 7061    @param file_pa
-00004280: 7468 3a20 0a20 2020 2020 2020 2020 2020  th: .           
-00004290: 2020 2020 2066 6f72 6d61 743a 2063 6f6e       format: con
-000042a0: 7465 6e74 2ce5 85b6 e4bb 962c e4ba 92e8  tent,......,....
-000042b0: 8194 e4ba 92e9 809a 2ce4 baa7 e593 81e5  ........,.......
-000042c0: 8a9f e880 972c e6bb 91e8 bdae e68f 90e6  .....,..........
-000042d0: 898b 2ce5 a3b0 e99f b32c 4150 50e6 938d  ..,......,APP...
-000042e0: e68e a7e6 80a7 2ce5 91bc e590 b8e7 81af  ......,.........
-000042f0: 2ce5 a496 e8a7 822c e5ba 95e5 baa7 2ce5  ,......,......,.
-00004300: 88b6 e783 ade8 8c83 e59b b42c e981 a5e6  ...........,....
-00004310: 8ea7 e599 a8e7 94b5 e6b1 a02c e591 b3e9  ...........,....
-00004320: 8193 2ce5 88b6 e783 ade6 9588 e69e 9c2c  ..,............,
-00004330: e8a1 a3e7 89a9 e783 98e5 b9b2 2ce4 bd93  ............,...
-00004340: e7a7 afe5 a4a7 e5b0 8f0a 2020 2020 2020  ..........      
-00004350: 2020 2020 2020 4072 6574 7572 6e3a 200a        @return: .
-00004360: 2020 2020 2020 2020 2020 2020 2222 220a              """.
-00004370: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00004380: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-00004390: 2020 7769 7468 206f 7065 6e28 6669 6c65    with open(file
-000043a0: 5f70 6174 682c 2027 7227 2c20 656e 636f  _path, 'r', enco
-000043b0: 6469 6e67 3d27 7574 662d 3827 2920 6173  ding='utf-8') as
-000043c0: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
-000043d0: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-000043e0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-000043f0: 2020 2020 2020 206c 696e 6520 3d20 6c69         line = li
-00004400: 6e65 2e73 7472 6970 2829 0a20 2020 2020  ne.strip().     
-00004410: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004420: 6620 6c69 6e65 2e73 7461 7274 7377 6974  f line.startswit
-00004430: 6828 2723 2729 3a0a 2020 2020 2020 2020  h('#'):.        
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00004460: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004470: 6e6f 7420 6c69 6e65 3a0a 2020 2020 2020  not line:.      
-00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-000044a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000044b0: 6572 6d73 203d 206c 696e 652e 7370 6c69  erms = line.spli
-000044c0: 7428 272c 2729 0a20 2020 2020 2020 2020  t(',').         
-000044d0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-000044e0: 6e28 7465 726d 7329 2021 3d20 3136 3a0a  n(terms) != 16:.
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00004510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004520: 2020 2020 2076 616c 203d 205b 696e 7428       val = [int(
-00004530: 6929 2066 6f72 2069 2069 6e20 7465 726d  i) for i in term
-00004540: 735b 313a 5d5d 0a20 2020 2020 2020 2020  s[1:]].         
-00004550: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-00004560: 6170 7065 6e64 285b 7465 726d 735b 305d  append([terms[0]
-00004570: 2c20 7661 6c5d 290a 2020 2020 2020 2020  , val]).        
-00004580: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
-00004590: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000045a0: 200a 2020 2020 2020 2020 6966 205f 5f6e   .        if __n
-000045b0: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-000045c0: 5f5f 273a 0a20 2020 2020 2020 2020 2020  __':.           
-000045d0: 2023 206d 6f64 656c 5f74 7970 653a 2073   # model_type: s
-000045e0: 7570 706f 7274 2027 6265 7274 272c 2027  upport 'bert', '
-000045f0: 616c 6265 7274 272c 2027 726f 6265 7274  albert', 'robert
-00004600: 6127 2c20 2778 6c6e 6574 270a 2020 2020  a', 'xlnet'.    
-00004610: 2020 2020 2020 2020 2320 6d6f 6465 6c5f          # model_
-00004620: 6e61 6d65 3a20 7375 7070 6f72 7420 2762  name: support 'b
-00004630: 6572 742d 6261 7365 2d63 6869 6e65 7365  ert-base-chinese
-00004640: 272c 2027 6265 7274 2d62 6173 652d 6361  ', 'bert-base-ca
-00004650: 7365 6427 2c20 2762 6572 742d 6261 7365  sed', 'bert-base
-00004660: 2d6d 756c 7469 6c69 6e67 7561 6c2d 6361  -multilingual-ca
-00004670: 7365 6427 202e 2e2e 0a20 2020 2020 2020  sed' ....       
-00004680: 2020 2020 206d 203d 2042 6572 7443 6c61       m = BertCla
-00004690: 7373 6966 6965 7228 6d6f 6465 6c5f 6469  ssifier(model_di
-000046a0: 723d 276d 6f64 656c 732f 6d75 6c74 696c  r='models/multil
-000046b0: 6162 656c 2d62 6572 742d 7a68 2d6d 6f64  abel-bert-zh-mod
-000046c0: 656c 272c 206e 756d 5f63 6c61 7373 6573  el', num_classes
-000046d0: 3d31 352c 0a20 2020 2020 2020 2020 2020  =15,.           
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 6d6f 6465 6c5f 7479 7065 3d27 6265 7274  model_type='bert
+000036b0: 272c 206d 6f64 656c 5f6e 616d 653d 2762  ', model_name='b
+000036c0: 6572 742d 6261 7365 2d63 6869 6e65 7365  ert-base-chinese
+000036d0: 272c 206e 756d 5f65 706f 6368 733d 3229  ', num_epochs=2)
+000036e0: 0a20 2020 2020 2020 2020 2020 2023 206d  .            # m
+000036f0: 6f64 656c 5f74 7970 653a 2073 7570 706f  odel_type: suppo
+00003700: 7274 2027 6265 7274 272c 2027 616c 6265  rt 'bert', 'albe
+00003710: 7274 272c 2027 726f 6265 7274 6127 2c20  rt', 'roberta', 
+00003720: 2778 6c6e 6574 270a 2020 2020 2020 2020  'xlnet'.        
+00003730: 2020 2020 2320 6d6f 6465 6c5f 6e61 6d65      # model_name
+00003740: 3a20 7375 7070 6f72 7420 2762 6572 742d  : support 'bert-
+00003750: 6261 7365 2d63 6869 6e65 7365 272c 2027  base-chinese', '
+00003760: 6265 7274 2d62 6173 652d 6361 7365 6427  bert-base-cased'
+00003770: 2c20 2762 6572 742d 6261 7365 2d6d 756c  , 'bert-base-mul
+00003780: 7469 6c69 6e67 7561 6c2d 6361 7365 6427  tilingual-cased'
+00003790: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+000037a0: 2064 6174 6120 3d20 5b0a 2020 2020 2020   data = [.      
+000037b0: 2020 2020 2020 2020 2020 2827 6564 7563            ('educ
+000037c0: 6174 696f 6e27 2c20 27e5 908d e5b8 88e6  ation', '.......
+000037d0: 8c87 e5af bce6 8998 e7a6 8fe8 afad e6b3  ................
+000037e0: 95e6 8a80 e5b7 a7ef bc9a e590 8de8 af8d  ................
+000037f0: e79a 84e5 a48d e695 b0e5 bda2 e5bc 8f27  ...............'
+00003800: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00003810: 2020 2028 2765 6475 6361 7469 6f6e 272c     ('education',
+00003820: 2027 e4b8 ade5 9bbd e9ab 98e8 8083 e688   '..............
+00003830: 90e7 bba9 e6b5 b7e5 a496 e8ae a4e5 8faf  ................
+00003840: 20e6 98af e280 9ce7 8bbc e69d a5e4 ba86   ...............
+00003850: e280 9de5 9097 efbc 9f27 292c 0a20 2020  .........'),.   
+00003860: 2020 2020 2020 2020 2020 2020 2028 2765               ('e
+00003870: 6475 6361 7469 6f6e 272c 2027 e585 ace5  ducation', '....
+00003880: 8aa1 e591 98e8 8083 e899 91e8 b68a e69d  ................
+00003890: a5e8 b68a e590 83e9 a699 efbc 8ce8 bf99  ................
+000038a0: e698 afe6 808e e4b9 88e5 9b9e e4ba 8bef  ................
+000038b0: bc9f 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
+000038c0: 2020 2020 2020 2827 7370 6f72 7473 272c        ('sports',
+000038d0: 2027 e59b bee6 9687 efbc 9ae6 b395 e7bd   '..............
+000038e0: 91e5 ad9f e88f b2e5 b094 e696 afe8 8ba6  ................
+000038f0: e688 98e8 bf9b 3136 e5bc ba20 e5ad 9fe8  ......16... ....
+00003900: 8fb2 e5b0 94e6 96af e680 92e5 90bc 2729  ..............')
+00003910: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003920: 2020 2827 7370 6f72 7473 272c 2027 e59b    ('sports', '..
+00003930: 9be5 b79d e4b8 b9e6 a3b1 e4b8 bee8 a18c  ................
+00003940: e585 a8e5 9bbd e995 bfe8 b79d e799 bbe5  ................
+00003950: b1b1 e68c 91e6 8898 e8b5 9b20 e8bf 91e4  ........... ....
+00003960: b887 e4ba bae5 8f82 e4b8 8e27 292c 0a20  ...........'),. 
+00003970: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00003980: 2773 706f 7274 7327 2c20 27e7 b1b3 e585  'sports', '.....
+00003990: b0e5 aea2 e59c ba38 e688 98e4 b88d e8b4  .......8........
+000039a0: a5e5 9bbd e7b1 b331 30e5 b9b4 e8bf 9ee8  .......10.......
+000039b0: 839c 2729 2c0a 2020 2020 2020 2020 2020  ..'),.          
+000039c0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+000039d0: 6d2e 7472 6169 6e28 6461 7461 290a 2020  m.train(data).  
+000039e0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000039f0: 6d29 0a20 2020 2020 2020 2020 2020 2023  m).            #
+00003a00: 206c 6f61 6420 7472 6169 6e65 6420 6265   load trained be
+00003a10: 7374 206d 6f64 656c 2066 726f 6d20 6d6f  st model from mo
+00003a20: 6465 6c5f 6469 720a 2020 2020 2020 2020  del_dir.        
+00003a30: 2020 2020 6d2e 6c6f 6164 5f6d 6f64 656c      m.load_model
+00003a40: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+00003a50: 7265 6469 6374 5f6c 6162 656c 2c20 7072  redict_label, pr
+00003a60: 6564 6963 745f 7072 6f62 6120 3d20 6d2e  edict_proba = m.
+00003a70: 7072 6564 6963 7428 5b27 e7a6 8fe5 bbba  predict(['......
+00003a80: e698 a5e5 ada3 e585 ace5 8aa1 e591 98e8  ................
+00003a90: 8083 e8af 95e6 8aa5 e590 8d31 38e6 97a5  ...........18...
+00003aa0: e688 aae6 ada2 2032 e69c 8836 e697 a5e8  ...... 2...6....
+00003ab0: 8083 e8af 9527 2c0a 2020 2020 2020 2020  .....',.        
+00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 27e6                '.
+00003af0: 848f e794 b2e9 a696 e8bd aee8 a1a5 e8b5  ................
+00003b00: 9be4 baa4 e688 98e8 aeb0 e5bd 953a e7b1  .............:..
+00003b10: b3e5 85b0 e5ae a2e5 9cba 38e6 8898 e4b8  ..........8.....
+00003b20: 8de8 b4a5 e59b bde7 b1b3 3130 e5b9 b4e8  ..........10....
+00003b30: bf9e e883 9c27 5d29 0a20 2020 2020 2020  .....']).       
+00003b40: 2020 2020 2070 7269 6e74 2866 2770 7265       print(f'pre
+00003b50: 6469 6374 5f6c 6162 656c 3a20 7b70 7265  dict_label: {pre
+00003b60: 6469 6374 5f6c 6162 656c 7d2c 2070 7265  dict_label}, pre
+00003b70: 6469 6374 5f70 726f 6261 3a20 7b70 7265  dict_proba: {pre
+00003b80: 6469 6374 5f70 726f 6261 7d27 290a 2020  dict_proba}').  
+00003b90: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00003ba0: 2020 2074 6573 745f 6461 7461 203d 205b     test_data = [
+00003bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003bc0: 2028 2765 6475 6361 7469 6f6e 272c 2027   ('education', '
+00003bd0: e7a6 8fe5 bbba e698 a5e5 ada3 e585 ace5  ................
+00003be0: 8aa1 e591 98e8 8083 e8af 95e6 8aa5 e590  ................
+00003bf0: 8d31 38e6 97a5 e688 aae6 ada2 2032 e69c  .18......... 2..
+00003c00: 8836 e697 a5e8 8083 e8af 9527 292c 0a20  .6.........'),. 
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00003c20: 2773 706f 7274 7327 2c20 27e6 848f e794  'sports', '.....
+00003c30: b2e9 a696 e8bd aee8 a1a5 e8b5 9be4 baa4  ................
+00003c40: e688 98e8 aeb0 e5bd 953a e7b1 b3e5 85b0  .........:......
+00003c50: e5ae a2e5 9cba 38e6 8898 e4b8 8de8 b4a5  ......8.........
+00003c60: e59b bde7 b1b3 3130 e5b9 b4e8 bf9e e883  ......10........
+00003c70: 9c27 292c 0a20 2020 2020 2020 2020 2020  .'),.           
+00003c80: 205d 0a20 2020 2020 2020 2020 2020 2061   ].            a
+00003c90: 6363 5f73 636f 7265 203d 206d 2e65 7661  cc_score = m.eva
+00003ca0: 6c75 6174 655f 6d6f 6465 6c28 7465 7374  luate_model(test
+00003cb0: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
+00003cc0: 2020 2070 7269 6e74 2866 2761 6363 5f73     print(f'acc_s
+00003cd0: 636f 7265 3a20 7b61 6363 5f73 636f 7265  core: {acc_score
+00003ce0: 7d27 290a 2020 2020 2020 2020 0a20 2020  }').        .   
+00003cf0: 2020 2020 2020 2020 2023 2074 7261 696e           # train
+00003d00: 206d 6f64 656c 2077 6974 6820 3177 2064   model with 1w d
+00003d10: 6174 6120 6669 6c65 2061 6e64 2031 3020  ata file and 10 
+00003d20: 636c 6173 7365 730a 2020 2020 2020 2020  classes.        
+00003d30: 2020 2020 7072 696e 7428 272d 2720 2a20      print('-' * 
+00003d40: 3432 290a 2020 2020 2020 2020 2020 2020  42).            
+00003d50: 6d20 3d20 4265 7274 436c 6173 7369 6669  m = BertClassifi
+00003d60: 6572 286f 7574 7075 745f 6469 723d 276d  er(output_dir='m
+00003d70: 6f64 656c 732f 6265 7274 2d63 6869 6e65  odels/bert-chine
+00003d80: 7365 272c 206e 756d 5f63 6c61 7373 6573  se', num_classes
+00003d90: 3d31 302c 0a20 2020 2020 2020 2020 2020  =10,.           
+00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003db0: 2020 2020 6d6f 6465 6c5f 7479 7065 3d27      model_type='
+00003dc0: 6265 7274 272c 206d 6f64 656c 5f6e 616d  bert', model_nam
+00003dd0: 653d 2762 6572 742d 6261 7365 2d63 6869  e='bert-base-chi
+00003de0: 6e65 7365 272c 206e 756d 5f65 706f 6368  nese', num_epoch
+00003df0: 733d 322c 0a20 2020 2020 2020 2020 2020  s=2,.           
+00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e10: 2020 2020 6172 6773 3d7b 226e 6f5f 6361      args={"no_ca
+00003e20: 6368 6522 3a20 5472 7565 2c20 226c 617a  che": True, "laz
+00003e30: 795f 6c6f 6164 696e 6722 3a20 5472 7565  y_loading": True
+00003e40: 2c20 226c 617a 795f 7465 7874 5f63 6f6c  , "lazy_text_col
+00003e50: 756d 6e22 3a20 312c 2022 6c61 7a79 5f6c  umn": 1, "lazy_l
+00003e60: 6162 656c 735f 636f 6c75 6d6e 223a 2030  abels_column": 0
+00003e70: 2c20 7d29 0a20 2020 2020 2020 2020 2020  , }).           
+00003e80: 2064 6174 615f 6669 6c65 203d 2027 7468   data_file = 'th
+00003e90: 7563 6e65 7773 5f74 7261 696e 5f31 772e  ucnews_train_1w.
+00003ea0: 7478 7427 0a20 2020 2020 2020 2020 2020  txt'.           
+00003eb0: 2023 20e5 a682 e69e 9ce8 aead e7bb 83e6   # .............
+00003ec0: 95b0 e68d aee8 b685 e8bf 87e7 99be e4b8  ................
+00003ed0: 87e6 9da1 efbc 8ce5 bbba e8ae aee4 bdbf  ................
+00003ee0: e794 a86c 617a 795f 6c6f 6164 696e 67e6  ...lazy_loading.
+00003ef0: a8a1 e5bc 8fef bc8c e587 8fe5 b091 e586  ................
+00003f00: 85e5 ad98 e58d a0e7 94a8 0a20 2020 2020  ...........     
+00003f10: 2020 2020 2020 206d 2e74 7261 696e 2864         m.train(d
+00003f20: 6174 615f 6669 6c65 2c20 7465 7374 5f73  ata_file, test_s
+00003f30: 697a 653d 302c 206e 616d 6573 3d28 276c  ize=0, names=('l
+00003f40: 6162 656c 7327 2c20 2774 6578 7427 2929  abels', 'text'))
+00003f50: 0a20 2020 2020 2020 2020 2020 206d 2e6c  .            m.l
+00003f60: 6f61 645f 6d6f 6465 6c28 290a 2020 2020  oad_model().    
+00003f70: 2020 2020 2020 2020 7072 6564 6963 745f          predict_
+00003f80: 6c61 6265 6c2c 2070 7265 6469 6374 5f70  label, predict_p
+00003f90: 726f 6261 203d 206d 2e70 7265 6469 6374  roba = m.predict
+00003fa0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00003fb0: 2020 5b27 e9a1 bae4 b989 e58c 97e4 baac    ['............
+00003fc0: e88b 8fe6 b4bb 3838 e5b9 b3e7 b1b3 e8b5  ......88........
+00003fd0: b7e7 b2be e8a3 85e6 88bf e59c a8e5 94ae  ................
+00003fe0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00003ff0: 2020 2020 27e7 be8e 4542 2d35 e9a1 b9e7      '...EB-5....
+00004000: 9bae e280 9c31 35e6 97a5 e5bf abe9 809f  .....15.........
+00004010: e7a7 bbe6 b091 e280 9de5 b086 e68e a8e8  ................
+00004020: bf9f 272c 0a20 2020 2020 2020 2020 2020  ..',.           
+00004030: 2020 2020 2020 27e6 8192 e794 9f41 48e6        '......AH.
+00004040: baa2 e68c 87e6 94b6 e5b9 b320 41e8 82a1  ........... A...
+00004050: e5af b948 e882 a1e6 8a98 e4bb b731 2e39  ...H.........1.9
+00004060: 3525 275d 290a 2020 2020 2020 2020 2020  5%']).          
+00004070: 2020 7072 696e 7428 6627 7072 6564 6963    print(f'predic
+00004080: 745f 6c61 6265 6c3a 207b 7072 6564 6963  t_label: {predic
+00004090: 745f 6c61 6265 6c7d 2c20 7072 6564 6963  t_label}, predic
+000040a0: 745f 7072 6f62 613a 207b 7072 6564 6963  t_proba: {predic
+000040b0: 745f 7072 6f62 617d 2729 0a20 2020 2020  t_proba}').     
+000040c0: 2020 2060 6060 0a20 2020 2020 2020 2050     ```.        P
+000040d0: 53ef bc9a e5a6 82e6 9e9c e8ae ade7 bb83  S...............
+000040e0: e695 b0e6 8dae e8b6 85e8 bf87 e799 bee4  ................
+000040f0: b887 e69d a1ef bc8c e5bb bae8 aeae e4bd  ................
+00004100: bfe7 94a8 6c61 7a79 5f6c 6f61 6469 6e67  ....lazy_loading
+00004110: e6a8 a1e5 bc8f efbc 8ce5 878f e5b0 91e5  ................
+00004120: 8685 e5ad 98e5 8da0 e794 a80a 2020 2020  ............    
+00004130: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00004140: 2320 e5a4 9ae6 a087 e7ad bee5 8886 e7b1  # ..............
+00004150: bbe6 a8a1 e59e 8b0a 2020 2020 2020 2020  ........        
+00004160: e588 86e7 b1bb e58f afe4 bba5 e588 86e4  ................
+00004170: b8ba e5a4 9ae5 8886 e7b1 bbe5 928c e5a4  ................
+00004180: 9ae6 a087 e7ad bee5 8886 e7b1 bbe3 8082  ................
+00004190: e5a4 9ae5 8886 e7b1 bbe7 9a84 e6a0 87e7  ................
+000041a0: adbe e698 afe6 8e92 e4bb 96e7 9a84 efbc  ................
+000041b0: 8ce8 808c e5a4 9ae6 a087 e7ad bee5 8886  ................
+000041c0: e7b1 bbe7 9a84 e689 80e6 9c89 e6a0 87e7  ................
+000041d0: adbe e698 afe4 b88d e68e 92e4 bb96 e79a  ................
+000041e0: 84e3 8082 0a20 2020 2020 2020 200a 2020  .....        .  
+000041f0: 2020 2020 2020 e5a4 9ae6 a087 e7ad bee5        ..........
+00004200: 8886 e7b1 bbe6 af94 e8be 83e7 9bb4 e8a7  ................
+00004210: 82e7 9a84 e790 86e8 a7a3 e698 afef bc8c  ................
+00004220: e4b8 80e4 b8aa e6a0 b7e6 9cac e58f afe4  ................
+00004230: bba5 e590 8ce6 97b6 e68b a5e6 9c89 e587  ................
+00004240: a0e4 b8aa e7b1 bbe5 88ab e6a0 87e7 adbe  ................
+00004250: efbc 8c0a 2020 2020 2020 2020 e6af 94e5  ....        ....
+00004260: a682 e4b8 80e9 a696 e6ad 8ce7 9a84 e6a0  ................
+00004270: 87e7 adbe e58f afe4 bba5 e698 afe6 b581  ................
+00004280: e8a1 8ce3 8081 e8bd bbe5 bfab efbc 8ce4  ................
+00004290: b880 e983 a8e7 94b5 e5bd b1e7 9a84 e6a0  ................
+000042a0: 87e7 adbe e58f afe4 bba5 e698 afe5 8aa8  ................
+000042b0: e4bd 9ce3 8081 e596 9ce5 89a7 e380 81e6  ................
+000042c0: 909e e7ac 91e7 ad89 efbc 8ce8 bf99 e983  ................
+000042d0: bde6 98af e5a4 9ae6 a087 e7ad bee5 8886  ................
+000042e0: e7b1 bbe7 9a84 e683 85e5 86b5 e380 820a  ................
+000042f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004300: 20e8 aead e7bb 83e5 928c e9a2 84e6 b58b   ...............
+00004310: 6042 4552 5460 e5a4 9ae6 a087 e7ad bee5  `BERT`..........
+00004320: 8886 e7b1 bbe6 a8a1 e59e 8bef bc8c e7a4  ................
+00004330: bae4 be8b 5b65 7861 6d70 6c65 732f 6265  ....[examples/be
+00004340: 7274 5f6d 756c 7469 6c61 6265 6c5f 636c  rt_multilabel_cl
+00004350: 6173 7369 6669 6361 7469 6f6e 5f7a 685f  assification_zh_
+00004360: 6465 6d6f 2e70 792e 7079 5d28 6874 7470  demo.py.py](http
+00004370: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00004380: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
+00004390: 636c 6173 7369 6669 6572 2f62 6c6f 622f  classifier/blob/
+000043a0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+000043b0: 6265 7274 5f6d 756c 7469 6c61 6265 6c5f  bert_multilabel_
+000043c0: 636c 6173 7369 6669 6361 7469 6f6e 5f7a  classification_z
+000043d0: 685f 6465 6d6f 2e70 7929 0a20 2020 2020  h_demo.py).     
+000043e0: 2020 200a 2020 2020 2020 2020 6060 6070     .        ```p
+000043f0: 7974 686f 6e0a 2020 2020 2020 2020 696d  ython.        im
+00004400: 706f 7274 2073 7973 0a20 2020 2020 2020  port sys.       
+00004410: 2069 6d70 6f72 7420 7061 6e64 6173 2061   import pandas a
+00004420: 7320 7064 0a20 2020 2020 2020 200a 2020  s pd.        .  
+00004430: 2020 2020 2020 7379 732e 7061 7468 2e61        sys.path.a
+00004440: 7070 656e 6428 272e 2e27 290a 2020 2020  ppend('..').    
+00004450: 2020 2020 6672 6f6d 2070 7974 6578 7463      from pytextc
+00004460: 6c61 7373 6966 6965 7220 696d 706f 7274  lassifier import
+00004470: 2042 6572 7443 6c61 7373 6966 6965 720a   BertClassifier.
+00004480: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00004490: 200a 2020 2020 2020 2020 6465 6620 6c6f   .        def lo
+000044a0: 6164 5f6a 645f 6461 7461 2866 696c 655f  ad_jd_data(file_
+000044b0: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
+000044c0: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
+000044d0: 2020 204c 6f61 6420 6a64 2064 6174 6120     Load jd data 
+000044e0: 6672 6f6d 2066 696c 652e 0a20 2020 2020  from file..     
+000044f0: 2020 2020 2020 2040 7061 7261 6d20 6669         @param fi
+00004500: 6c65 5f70 6174 683a 200a 2020 2020 2020  le_path: .      
+00004510: 2020 2020 2020 2020 2020 666f 726d 6174            format
+00004520: 3a20 636f 6e74 656e 742c e585 b6e4 bb96  : content,......
+00004530: 2ce4 ba92 e881 94e4 ba92 e980 9a2c e4ba  ,............,..
+00004540: a7e5 9381 e58a 9fe8 8097 2ce6 bb91 e8bd  ..........,.....
+00004550: aee6 8f90 e689 8b2c e5a3 b0e9 9fb3 2c41  .......,......,A
+00004560: 5050 e693 8de6 8ea7 e680 a72c e591 bce5  PP.........,....
+00004570: 90b8 e781 af2c e5a4 96e8 a782 2ce5 ba95  .....,......,...
+00004580: e5ba a72c e588 b6e7 83ad e88c 83e5 9bb4  ...,............
+00004590: 2ce9 81a5 e68e a7e5 99a8 e794 b5e6 b1a0  ,...............
+000045a0: 2ce5 91b3 e981 932c e588 b6e7 83ad e695  ,......,........
+000045b0: 88e6 9e9c 2ce8 a1a3 e789 a9e7 8398 e5b9  ....,...........
+000045c0: b22c e4bd 93e7 a7af e5a4 a7e5 b08f 0a20  .,............. 
+000045d0: 2020 2020 2020 2020 2020 2040 7265 7475             @retu
+000045e0: 726e 3a20 0a20 2020 2020 2020 2020 2020  rn: .           
+000045f0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
+00004600: 2064 6174 6120 3d20 5b5d 0a20 2020 2020   data = [].     
+00004610: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00004620: 2866 696c 655f 7061 7468 2c20 2772 272c  (file_path, 'r',
+00004630: 2065 6e63 6f64 696e 673d 2775 7466 2d38   encoding='utf-8
+00004640: 2729 2061 7320 663a 0a20 2020 2020 2020  ') as f:.       
+00004650: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
+00004660: 6520 696e 2066 3a0a 2020 2020 2020 2020  e in f:.        
+00004670: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00004680: 203d 206c 696e 652e 7374 7269 7028 290a   = line.strip().
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2020 6966 206c 696e 652e 7374 6172      if line.star
+000046b0: 7473 7769 7468 2827 2327 293a 0a20 2020  tswith('#'):.   
+000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046d0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
 000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2020 6d6f 6465 6c5f 7479 7065 3d27      model_type='
-00004700: 6265 7274 272c 206d 6f64 656c 5f6e 616d  bert', model_nam
-00004710: 653d 2762 6572 742d 6261 7365 2d63 6869  e='bert-base-chi
-00004720: 6e65 7365 272c 206e 756d 5f65 706f 6368  nese', num_epoch
-00004730: 733d 322c 206d 756c 7469 5f6c 6162 656c  s=2, multi_label
-00004740: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00004750: 2020 2023 2054 7261 696e 2061 6e64 2045     # Train and E
-00004760: 7661 6c75 6174 696f 6e20 6461 7461 206e  valuation data n
-00004770: 6565 6473 2074 6f20 6265 2069 6e20 6120  eeds to be in a 
-00004780: 5061 6e64 6173 2044 6174 6166 7261 6d65  Pandas Dataframe
-00004790: 2063 6f6e 7461 696e 696e 6720 6174 206c   containing at l
-000047a0: 6561 7374 2074 776f 2063 6f6c 756d 6e73  east two columns
-000047b0: 2c20 6120 2774 6578 7427 2061 6e64 2061  , a 'text' and a
-000047c0: 2027 6c61 6265 6c73 2720 636f 6c75 6d6e   'labels' column
-000047d0: 2e20 5468 6520 606c 6162 656c 7360 2063  . The `labels` c
-000047e0: 6f6c 756d 6e20 7368 6f75 6c64 2063 6f6e  olumn should con
-000047f0: 7461 696e 206d 756c 7469 2d68 6f74 2065  tain multi-hot e
-00004800: 6e63 6f64 6564 206c 6973 7473 2e0a 2020  ncoded lists..  
-00004810: 2020 2020 2020 2020 2020 7472 6169 6e5f            train_
-00004820: 6461 7461 203d 205b 0a20 2020 2020 2020  data = [.       
-00004830: 2020 2020 2020 2020 205b 22e4 b880 e4b8           [".....
-00004840: aae5 b08f e697 b6e6 88bf e997 b4e4 bb8d  ................
-00004850: e784 b6e6 b2a1 e69a 96e5 928c 222c 205b  ............", [
-00004860: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00004870: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00004880: 2030 2c20 312c 2030 2c20 305d 5d2c 0a20   0, 1, 0, 0]],. 
-00004890: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-000048a0: 22e8 8097 e794 b5e6 8385 e586 b5ef bc9a  "...............
-000048b0: e8bf 99e4 b8aa e6b2 a1e6 9c89 e6b3 a8e6  ................
-000048c0: 848f 222c 205b 302c 2030 2c20 312c 2030  ..", [0, 0, 1, 0
-000048d0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-000048e0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
-000048f0: 305d 5d2c 0a20 2020 2020 2020 2020 2020  0]],.           
-00004900: 205d 0a20 2020 2020 2020 2020 2020 2064   ].            d
-00004910: 6174 6120 3d20 6c6f 6164 5f6a 645f 6461  ata = load_jd_da
-00004920: 7461 2827 6d75 6c74 696c 6162 656c 5f6a  ta('multilabel_j
-00004930: 645f 636f 6d6d 656e 7473 2e63 7376 2729  d_comments.csv')
-00004940: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
-00004950: 696e 5f64 6174 612e 6578 7465 6e64 2864  in_data.extend(d
-00004960: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-00004970: 2070 7269 6e74 2874 7261 696e 5f64 6174   print(train_dat
-00004980: 615b 3a35 5d29 0a20 2020 2020 2020 2020  a[:5]).         
-00004990: 2020 2074 7261 696e 5f64 6620 3d20 7064     train_df = pd
-000049a0: 2e44 6174 6146 7261 6d65 2874 7261 696e  .DataFrame(train
-000049b0: 5f64 6174 612c 2063 6f6c 756d 6e73 3d5b  _data, columns=[
-000049c0: 2274 6578 7422 2c20 226c 6162 656c 7322  "text", "labels"
-000049d0: 5d29 0a20 2020 2020 2020 200a 2020 2020  ]).        .    
-000049e0: 2020 2020 2020 2020 7072 696e 7428 7472          print(tr
-000049f0: 6169 6e5f 6466 2e68 6561 6428 2929 0a20  ain_df.head()). 
-00004a00: 2020 2020 2020 2020 2020 206d 2e74 7261             m.tra
-00004a10: 696e 2874 7261 696e 5f64 6629 0a20 2020  in(train_df).   
-00004a20: 2020 2020 2020 2020 2070 7269 6e74 286d           print(m
-00004a30: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-00004a40: 4576 616c 7561 7465 2074 6865 206d 6f64  Evaluate the mod
-00004a50: 656c 0a20 2020 2020 2020 2020 2020 2061  el.            a
-00004a60: 6363 5f73 636f 7265 203d 206d 2e65 7661  cc_score = m.eva
-00004a70: 6c75 6174 655f 6d6f 6465 6c28 7472 6169  luate_model(trai
-00004a80: 6e5f 6466 5b3a 3230 5d29 0a20 2020 2020  n_df[:20]).     
-00004a90: 2020 2020 2020 2070 7269 6e74 2866 2761         print(f'a
-00004aa0: 6363 5f73 636f 7265 3a20 7b61 6363 5f73  cc_score: {acc_s
-00004ab0: 636f 7265 7d27 290a 2020 2020 2020 2020  core}').        
-00004ac0: 0a20 2020 2020 2020 2020 2020 2023 206c  .            # l
-00004ad0: 6f61 6420 7472 6169 6e65 6420 6265 7374  oad trained best
-00004ae0: 206d 6f64 656c 2066 726f 6d20 6d6f 6465   model from mode
-00004af0: 6c5f 6469 720a 2020 2020 2020 2020 2020  l_dir.          
-00004b00: 2020 6d2e 6c6f 6164 5f6d 6f64 656c 2829    m.load_model()
-00004b10: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
-00004b20: 6469 6374 5f6c 6162 656c 2c20 7072 6564  dict_label, pred
-00004b30: 6963 745f 7072 6f62 6120 3d20 6d2e 7072  ict_proba = m.pr
-00004b40: 6564 6963 7428 5b27 e4b8 80e4 b8aa e5b0  edict(['........
-00004b50: 8fe6 97b6 e688 bfe9 97b4 e4bb 8de7 84b6  ................
-00004b60: e6b2 a1e6 9a96 e592 8c27 2c20 27e8 8097  .........', '...
-00004b70: e794 b5e6 8385 e586 b5ef bc9a e8bf 99e4  ................
-00004b80: b8aa e6b2 a1e6 9c89 e6b3 a8e6 848f 275d  ..............']
-00004b90: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00004ba0: 696e 7428 6627 7072 6564 6963 745f 6c61  int(f'predict_la
-00004bb0: 6265 6c3a 207b 7072 6564 6963 745f 6c61  bel: {predict_la
-00004bc0: 6265 6c7d 2c20 7072 6564 6963 745f 7072  bel}, predict_pr
-00004bd0: 6f62 613a 207b 7072 6564 6963 745f 7072  oba: {predict_pr
-00004be0: 6f62 617d 2729 0a20 2020 2020 2020 2060  oba}').        `
-00004bf0: 6060 0a20 2020 2020 2020 200a 2020 2020  ``.        .    
-00004c00: 2020 2020 2323 2045 7661 6c75 6174 696f      ## Evaluatio
-00004c10: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
-00004c20: 2020 2023 2323 2044 6174 6173 6574 0a20     ### Dataset. 
-00004c30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004c40: 312e 2054 4855 434e 6577 73e4 b8ad e696  1. THUCNews.....
-00004c50: 87e6 9687 e69c ace6 95b0 e68d aee9 9b86  ................
-00004c60: efbc 8831 2e35 3647 42ef bc89 efbc 9ae5  ...1.56GB.......
-00004c70: ae98 e696 b95b e4b8 8be8 bdbd e59c b0e5  .....[..........
-00004c80: 9d80 5d28 6874 7470 3a2f 2f74 6875 6374  ..](http://thuct
-00004c90: 632e 7468 756e 6c70 2e6f 7267 2f29 efbc  c.thunlp.org/)..
-00004ca0: 8ce6 8abd e6a0 b7e4 ba86 3130 e4b8 87e6  ..........10....
-00004cb0: 9da1 5448 5543 4e65 7773 e4b8 ade6 9687  ..THUCNews......
-00004cc0: e696 87e6 9cac 3130 e588 86e7 b1bb e695  ......10........
-00004cd0: b0e6 8dae e99b 86ef bc88 364d 42ef bc89  ..........6MB...
-00004ce0: efbc 8ce5 9cb0 e59d 80ef bc9a 5b65 7861  ............[exa
-00004cf0: 6d70 6c65 732f 7468 7563 6e65 7773 5f74  mples/thucnews_t
-00004d00: 7261 696e 5f31 3077 2e74 7874 5d28 6578  rain_10w.txt](ex
-00004d10: 616d 706c 6573 2f74 6875 636e 6577 735f  amples/thucnews_
-00004d20: 7472 6169 6e5f 3130 772e 7478 7429 e380  train_10w.txt)..
-00004d30: 820a 2020 2020 2020 2020 322e 2054 4e45  ..        2. TNE
-00004d40: 5753 e4bb 8ae6 97a5 e5a4 b4e6 9da1 e4b8  WS..............
-00004d50: ade6 9687 e696 b0e9 97bb efbc 88e7 9fad  ................
-00004d60: e696 87e6 9cac efbc 89e5 8886 e7b1 bb20  ............... 
-00004d70: 5368 6f72 7420 5465 7874 2043 6c61 7373  Short Text Class
-00004d80: 6966 6963 6169 746f 6e20 666f 7220 4e65  ificaiton for Ne
-00004d90: 7773 efbc 8ce8 afa5 e695 b0e6 8dae e99b  ws..............
-00004da0: 8628 352e 314d 4229 e69d a5e8 87aa e4bb  .(5.1MB)........
-00004db0: 8ae6 97a5 e5a4 b4e6 9da1 e79a 84e6 96b0  ................
-00004dc0: e997 bbe7 8988 e59d 97ef bc8c e585 b1e6  ................
-00004dd0: 8f90 e58f 96e4 ba86 3135 e4b8 aae7 b1bb  ........15......
-00004de0: e588 abe7 9a84 e696 b0e9 97bb efbc 8ce5  ................
-00004df0: 8c85 e68b ace6 9785 e6b8 b8ef bc8c e695  ................
-00004e00: 99e8 82b2 efbc 8ce9 8791 e89e 8def bc8c  ................
-00004e10: e586 9be4 ba8b e7ad 89ef bc8c e59c b0e5  ................
-00004e20: 9d80 efbc 9a5b 746e 6577 735f 7075 626c  .....[tnews_publ
-00004e30: 6963 2e7a 6970 5d28 6874 7470 733a 2f2f  ic.zip](https://
-00004e40: 7374 6f72 6167 652e 676f 6f67 6c65 6170  storage.googleap
-00004e50: 6973 2e63 6f6d 2f63 6c75 6562 656e 6368  is.com/cluebench
-00004e60: 6d61 726b 2f74 6173 6b73 2f74 6e65 7773  mark/tasks/tnews
-00004e70: 5f70 7562 6c69 632e 7a69 7029 0a20 2020  _public.zip).   
-00004e80: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00004e90: 2320 4576 616c 7561 7469 6f6e 2052 6573  # Evaluation Res
-00004ea0: 756c 740a 2020 2020 2020 2020 e59c a854  ult.        ...T
-00004eb0: 4855 434e 6577 73e4 b8ad e696 87e6 9687  HUCNews.........
-00004ec0: e69c ac31 30e5 8886 e7b1 bbe6 95b0 e68d  ...10...........
-00004ed0: aee9 9b86 efbc 8836 4d42 efbc 89e4 b88a  .......6MB......
-00004ee0: e8af 84e4 bcb0 efbc 8ce6 a8a1 e59e 8be5  ................
-00004ef0: 9ca8 e6b5 8be8 af95 e99b 8628 7465 7374  ...........(test
-00004f00: 29e8 af84 e6b5 8be6 9588 e69e 9ce5 a682  )...............
-00004f10: e4b8 8bef bc9a 0a20 2020 2020 2020 200a  .......        .
-00004f20: 2020 2020 2020 2020 e6a8 a1e5 9e8b 7c61          ......|a
-00004f30: 6363 7ce8 afb4 e698 8e0a 2020 2020 2020  cc|.......      
-00004f40: 2020 2d2d 7c2d 2d7c 2d2d 0a20 2020 2020    --|--|--.     
-00004f50: 2020 204c 527c 302e 3838 3033 7ce9 80bb     LR|0.8803|...
-00004f60: e8be 91e5 9b9e e5bd 924c 6f67 6973 7469  .........Logisti
-00004f70: 6373 2052 6567 7265 7373 696f 6e0a 2020  cs Regression.  
-00004f80: 2020 2020 2020 5465 7874 434e 4e7c 302e        TextCNN|0.
-00004f90: 3838 3039 7c4b 696d 2032 3031 3420 e7bb  8809|Kim 2014 ..
-00004fa0: 8fe5 85b8 e79a 8443 4e4e e696 87e6 9cac  .......CNN......
-00004fb0: e588 86e7 b1bb 0a20 2020 2020 2020 2054  .......        T
-00004fc0: 6578 7452 4e4e 5f41 7474 7c30 2e39 3032  extRNN_Att|0.902
-00004fd0: 327c 4269 4c53 544d 2b41 7474 656e 7469  2|BiLSTM+Attenti
-00004fe0: 6f6e 0a20 2020 2020 2020 2046 6173 7454  on.        FastT
-00004ff0: 6578 747c 302e 3931 3737 7c62 6f77 2b62  ext|0.9177|bow+b
-00005000: 6967 7261 6d2b 7472 6967 7261 6def bc8c  igram+trigram...
-00005010: 20e6 9588 e69e 9ce5 87ba e5a5 87e7 9a84   ...............
-00005020: e5a5 bd0a 2020 2020 2020 2020 4450 434e  ....        DPCN
-00005030: 4e7c 302e 3931 3235 7ce6 b7b1 e5b1 82e9  N|0.9125|.......
-00005040: 8791 e5ad 97e5 a194 434e 4e0a 2020 2020  ........CNN.    
-00005050: 2020 2020 5472 616e 7366 6f72 6d65 727c      Transformer|
-00005060: 302e 3839 3931 7ce6 9588 e69e 9ce8 be83  0.8991|.........
-00005070: e5b7 ae0a 2020 2020 2020 2020 4245 5254  ....        BERT
-00005080: 2d62 6173 657c 2a2a 302e 3934 3833 2a2a  -base|**0.9483**
-00005090: 7c62 6572 7420 2b20 6663 0a20 2020 2020  |bert + fc.     
-000050a0: 2020 2045 524e 4945 7c30 2e39 3436 317c     ERNIE|0.9461|
-000050b0: e6af 9462 6572 74e7 95a5 e5b7 ae0a 2020  ...bert.......  
-000050c0: 2020 2020 2020 0a20 2020 2020 2020 20e5        .        .
-000050d0: 9ca8 e4b8 ade6 9687 e696 b0e9 97bb e79f  ................
-000050e0: ade6 9687 e69c ace5 8886 e7b1 bbe6 95b0  ................
-000050f0: e68d aee9 9b86 544e 4557 53e4 b88a e8af  ......TNEWS.....
-00005100: 84e4 bcb0 efbc 8ce6 a8a1 e59e 8be5 9ca8  ................
-00005110: e5bc 80e5 8f91 e99b 8628 6465 7629 e8af  .........(dev)..
-00005120: 84e6 b58b e695 88e6 9e9c e5a6 82e4 b88b  ................
-00005130: efbc 9a0a 2020 2020 2020 2020 0a20 2020  ....        .   
-00005140: 2020 2020 20e6 a8a1 e59e 8b7c 6163 637c       ......|acc|
-00005150: e8af b4e6 988e 0a20 2020 2020 2020 202d  .......        -
-00005160: 2d7c 2d2d 7c2d 2d0a 2020 2020 2020 2020  -|--|--.        
-00005170: 4245 5254 2d62 6173 657c 2a2a 302e 3536  BERT-base|**0.56
-00005180: 3630 2a2a 7ce6 9cac e9a1 b9e7 9bae e5ae  60**|...........
-00005190: 9ee7 8eb0 0a20 2020 2020 2020 2042 4552  .....        BER
-000051a0: 542d 6261 7365 7c30 2e35 3630 397c 434c  T-base|0.5609|CL
-000051b0: 5545 2042 656e 6368 6d61 726b 204c 6561  UE Benchmark Lea
-000051c0: 6465 7262 6f61 7264 e7bb 93e6 9e9c 205b  derboard...... [
-000051d0: 434c 5545 6265 6e63 686d 6172 6b5d 2868  CLUEbenchmark](h
-000051e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000051f0: 6d2f 434c 5545 6265 6e63 686d 6172 6b2f  m/CLUEbenchmark/
-00005200: 434c 5545 290a 2020 2020 2020 2020 0a20  CLUE).        . 
-00005210: 2020 2020 2020 202d 20e4 bba5 e4b8 8ae7         - .......
-00005220: bb93 e69e 9ce5 9d87 e4b8 bae5 8886 e7b1  ................
-00005230: bbe7 9a84 e587 86e7 a1ae e78e 87ef bc88  ................
-00005240: 6163 6375 7261 6379 efbc 89e7 bb93 e69e  accuracy........
-00005250: 9c0a 2020 2020 2020 2020 2d20 5448 5543  ..        - THUC
-00005260: 4e65 7773 e695 b0e6 8dae e99b 86e8 af84  News............
-00005270: e6b5 8be7 bb93 e69e 9ce5 8faf e4bb a5e5  ................
-00005280: 9fba e4ba 8e60 6578 616d 706c 6573 2f74  .....`examples/t
-00005290: 6875 636e 6577 735f 7472 6169 6e5f 3130  hucnews_train_10
-000052a0: 772e 7478 7460 e695 b0e6 8dae e794 a860  w.txt`.........`
-000052b0: 6578 616d 706c 6573 60e4 b88b e79a 84e5  examples`.......
-000052c0: 9084 e6a8 a1e5 9e8b 6465 6d6f e5a4 8de7  ........demo....
-000052d0: 8eb0 0a20 2020 2020 2020 202d 2054 4e45  ...        - TNE
-000052e0: 5753 e695 b0e6 8dae e99b 86e8 af84 e6b5  WS..............
-000052f0: 8be7 bb93 e69e 9ce5 8faf e4bb a5e4 b88b  ................
-00005300: e8bd bd54 4e45 5753 e695 b0e6 8dae e99b  ...TNEWS........
-00005310: 86ef bc8c e8bf 90e8 a18c 6065 7861 6d70  ..........`examp
-00005320: 6c65 732f 6265 7274 5f63 6c61 7373 6966  les/bert_classif
-00005330: 6963 6174 696f 6e5f 746e 6577 735f 6465  ication_tnews_de
-00005340: 6d6f 2e70 7960 e5a4 8de7 8eb0 0a20 2020  mo.py`.......   
-00005350: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
-00005360: 2320 e6a8 a1e5 9e8b e8b0 83e7 a094 0a20  # ............. 
-00005370: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00005380: e68f 90e4 be9b e588 86e7 b1bb e6a8 a1e5  ................
-00005390: 9e8b e5bf abe9 809f e8b0 83e7 a094 e5b7  ................
-000053a0: a5e5 85b7 efbc 8ce6 9687 e4bb b6e6 a091  ................
-000053b0: efbc 9a0a 2020 2020 2020 2020 6060 6062  ....        ```b
-000053c0: 6173 680a 2020 2020 2020 2020 7079 7465  ash.        pyte
-000053d0: 7874 636c 6173 7369 6669 6572 0a20 2020  xtclassifier.   
-000053e0: 2020 2020 20e2 949c e294 80e2 9480 2062       ......... b
-000053f0: 6572 745f 636c 6173 7369 6669 6572 2e70  ert_classifier.p
-00005400: 790a 2020 2020 2020 2020 e294 9ce2 9480  y.        ......
-00005410: e294 8020 6661 7374 7465 7874 5f63 6c61  ... fasttext_cla
-00005420: 7373 6966 6965 722e 7079 0a20 2020 2020  ssifier.py.     
-00005430: 2020 20e2 949c e294 80e2 9480 2063 6c61     ......... cla
-00005440: 7373 6963 5f63 6c61 7373 6966 6965 722e  ssic_classifier.
-00005450: 7079 0a20 2020 2020 2020 20e2 949c e294  py.        .....
-00005460: 80e2 9480 2074 6578 7463 6e6e 5f63 6c61  .... textcnn_cla
-00005470: 7373 6966 6965 722e 7079 0a20 2020 2020  ssifier.py.     
-00005480: 2020 20e2 9494 e294 80e2 9480 2074 6578     ......... tex
-00005490: 7472 6e6e 5f63 6c61 7373 6966 6965 722e  trnn_classifier.
-000054a0: 7079 0a20 2020 2020 2020 2060 6060 0a20  py.        ```. 
-000054b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000054c0: e6af 8fe4 b8aa e696 87e4 bbb6 e5af b9e5  ................
-000054d0: ba94 e4b8 80e4 b8aa e6a8 a1e5 9e8b efbc  ................
-000054e0: 8ce5 9084 e6a8 a1e5 9e8b e5ae 8ce5 85a8  ................
-000054f0: e78b ace7 ab8b efbc 8ce5 8faf e4bb a5e7  ................
-00005500: 9bb4 e68e a5e8 bf90 e8a1 8cef bc8c e4b9  ................
-00005510: 9fe6 96b9 e4be bfe4 bfae e694 b9ef bc8c  ................
-00005520: e694 afe6 8c81 e980 9ae8 bf87 6061 7267  ............`arg
-00005530: 7061 7273 6560 20e4 bfae e694 b960 2d2d  parse` ......`--
-00005540: 6461 7461 5f70 6174 6860 e7ad 89e5 8f82  data_path`......
-00005550: e695 b0e3 8082 0a20 2020 2020 2020 200a  .......        .
-00005560: 2020 2020 2020 2020 e79b b4e6 8ea5 e59c          ........
-00005570: a8e7 bb88 e7ab afe8 b083 e794 a866 6173  .............fas
-00005580: 7474 6578 74e6 a8a1 e59e 8be8 aead e7bb  ttext...........
-00005590: 83ef bc9a 0a20 2020 2020 2020 2060 6060  .....        ```
-000055a0: 6261 7368 0a20 2020 2020 2020 2070 7974  bash.        pyt
-000055b0: 686f 6e20 2d6d 2070 7974 6578 7463 6c61  hon -m pytextcla
-000055c0: 7373 6966 6965 722e 6661 7374 7465 7874  ssifier.fasttext
-000055d0: 5f63 6c61 7373 6966 6965 7220 2d68 0a20  _classifier -h. 
-000055e0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-000055f0: 2020 200a 2020 2020 2020 2020 2323 2054     .        ## T
-00005600: 6578 7420 436c 7573 7465 720a 2020 2020  ext Cluster.    
-00005610: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
-00005620: 2020 2020 2020 5465 7874 2063 6c75 7374        Text clust
-00005630: 6572 696e 672c 2066 6f72 2065 7861 6d70  ering, for examp
-00005640: 6c65 205b 6578 616d 706c 6573 2f63 6c75  le [examples/clu
-00005650: 7374 6572 5f64 656d 6f2e 7079 5d28 6578  ster_demo.py](ex
-00005660: 616d 706c 6573 2f63 6c75 7374 6572 5f64  amples/cluster_d
-00005670: 656d 6f2e 7079 290a 2020 2020 2020 2020  emo.py).        
-00005680: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00005690: 2020 696d 706f 7274 2073 7973 0a20 2020    import sys.   
-000056a0: 2020 2020 200a 2020 2020 2020 2020 7379       .        sy
-000056b0: 732e 7061 7468 2e61 7070 656e 6428 272e  s.path.append('.
-000056c0: 2e27 290a 2020 2020 2020 2020 6672 6f6d  .').        from
-000056d0: 2070 7974 6578 7463 6c61 7373 6966 6965   pytextclassifie
-000056e0: 722e 7465 7874 636c 7573 7465 7220 696d  r.textcluster im
-000056f0: 706f 7274 2054 6578 7443 6c75 7374 6572  port TextCluster
-00005700: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005710: 2020 6966 205f 5f6e 616d 655f 5f20 3d3d    if __name__ ==
-00005720: 2027 5f5f 6d61 696e 5f5f 273a 0a20 2020   '__main__':.   
-00005730: 2020 2020 2020 2020 206d 203d 2054 6578           m = Tex
-00005740: 7443 6c75 7374 6572 286d 6f64 656c 5f64  tCluster(model_d
-00005750: 6972 3d27 6d6f 6465 6c73 2f63 6c75 7374  ir='models/clust
-00005760: 6572 2d74 6f79 272c 206e 5f63 6c75 7374  er-toy', n_clust
-00005770: 6572 733d 3229 0a20 2020 2020 2020 2020  ers=2).         
-00005780: 2020 2070 7269 6e74 286d 290a 2020 2020     print(m).    
-00005790: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
-000057a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057b0: 2027 5374 7564 656e 7420 6465 6274 2074   'Student debt t
-000057c0: 6f20 636f 7374 2042 7269 7461 696e 2062  o cost Britain b
-000057d0: 696c 6c69 6f6e 7320 7769 7468 696e 2064  illions within d
-000057e0: 6563 6164 6573 272c 0a20 2020 2020 2020  ecades',.       
-000057f0: 2020 2020 2020 2020 2027 4368 696e 6573           'Chines
-00005800: 6520 6564 7563 6174 696f 6e20 666f 7220  e education for 
-00005810: 5456 2065 7870 6572 696d 656e 7427 2c0a  TV experiment',.
-00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005830: 2741 6262 6f74 7420 676f 7665 726e 6d65  'Abbott governme
-00005840: 6e74 2073 7065 6e64 7320 2438 206d 696c  nt spends $8 mil
-00005850: 6c69 6f6e 206f 6e20 6869 6768 6572 2065  lion on higher e
-00005860: 6475 6361 7469 6f6e 272c 0a20 2020 2020  ducation',.     
-00005870: 2020 2020 2020 2020 2020 2027 4d69 6464             'Midd
-00005880: 6c65 2045 6173 7420 616e 6420 4173 6961  le East and Asia
-00005890: 2062 6f6f 7374 2069 6e76 6573 746d 656e   boost investmen
-000058a0: 7420 696e 2074 6f70 206c 6576 656c 2073  t in top level s
-000058b0: 706f 7274 7327 2c0a 2020 2020 2020 2020  ports',.        
-000058c0: 2020 2020 2020 2020 2753 756d 6d69 7420          'Summit 
-000058d0: 5365 7269 6573 206c 6f6f 6b20 6c61 756e  Series look laun
-000058e0: 6368 6573 2048 424f 2043 616e 6164 6120  ches HBO Canada 
-000058f0: 7370 6f72 7473 2064 6f63 2073 6572 6965  sports doc serie
-00005900: 733a 204d 7564 6861 7227 0a20 2020 2020  s: Mudhar'.     
-00005910: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00005920: 2020 2020 206d 2e74 7261 696e 2864 6174       m.train(dat
-00005930: 6129 0a20 2020 2020 2020 2020 2020 206d  a).            m
-00005940: 2e6c 6f61 645f 6d6f 6465 6c28 290a 2020  .load_model().  
-00005950: 2020 2020 2020 2020 2020 7220 3d20 6d2e            r = m.
-00005960: 7072 6564 6963 7428 5b27 4162 626f 7474  predict(['Abbott
-00005970: 2067 6f76 6572 6e6d 656e 7420 7370 656e   government spen
-00005980: 6473 2024 3820 6d69 6c6c 696f 6e20 6f6e  ds $8 million on
-00005990: 2068 6967 6865 7220 6564 7563 6174 696f   higher educatio
-000059a0: 6e20 6d65 6469 6120 626c 6974 7a27 2c0a  n media blitz',.
-000059b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059c0: 2020 2020 2020 2020 2020 2027 4d69 6464             'Midd
-000059d0: 6c65 2045 6173 7420 616e 6420 4173 6961  le East and Asia
-000059e0: 2062 6f6f 7374 2069 6e76 6573 746d 656e   boost investmen
-000059f0: 7420 696e 2074 6f70 206c 6576 656c 2073  t in top level s
-00005a00: 706f 7274 7327 5d29 0a20 2020 2020 2020  ports']).       
-00005a10: 2020 2020 2070 7269 6e74 2872 290a 2020       print(r).  
-00005a20: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00005a30: 2020 2023 2323 2323 2323 2323 2323 206c     ########### l
-00005a40: 6f61 6420 6368 696e 6573 6520 7472 6169  oad chinese trai
-00005a50: 6e20 6461 7461 2066 726f 6d20 3177 2064  n data from 1w d
-00005a60: 6174 6120 6669 6c65 0a20 2020 2020 2020  ata file.       
-00005a70: 2020 2020 2066 726f 6d20 736b 6c65 6172       from sklear
-00005a80: 6e2e 6665 6174 7572 655f 6578 7472 6163  n.feature_extrac
-00005a90: 7469 6f6e 2e74 6578 7420 696d 706f 7274  tion.text import
-00005aa0: 2054 6669 6466 5665 6374 6f72 697a 6572   TfidfVectorizer
-00005ab0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00005ac0: 2020 2020 2020 7463 6c75 7374 6572 203d        tcluster =
-00005ad0: 2054 6578 7443 6c75 7374 6572 286d 6f64   TextCluster(mod
-00005ae0: 656c 5f64 6972 3d27 6d6f 6465 6c73 2f63  el_dir='models/c
-00005af0: 6c75 7374 6572 272c 2066 6561 7475 7265  luster', feature
-00005b00: 3d54 6669 6466 5665 6374 6f72 697a 6572  =TfidfVectorizer
-00005b10: 286e 6772 616d 5f72 616e 6765 3d28 312c  (ngram_range=(1,
-00005b20: 2032 2929 2c20 6e5f 636c 7573 7465 7273   2)), n_clusters
-00005b30: 3d31 3029 0a20 2020 2020 2020 2020 2020  =10).           
-00005b40: 2064 6174 6120 3d20 7463 6c75 7374 6572   data = tcluster
-00005b50: 2e6c 6f61 645f 6669 6c65 5f64 6174 6128  .load_file_data(
-00005b60: 2774 6875 636e 6577 735f 7472 6169 6e5f  'thucnews_train_
-00005b70: 3177 2e74 7874 272c 2073 6570 3d27 5c74  1w.txt', sep='\t
-00005b80: 272c 2075 7365 5f63 6f6c 3d31 290a 2020  ', use_col=1).  
-00005b90: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-00005ba0: 652c 206c 6162 656c 7320 3d20 7463 6c75  e, labels = tclu
-00005bb0: 7374 6572 2e74 7261 696e 2864 6174 615b  ster.train(data[
-00005bc0: 3a35 3030 305d 290a 2020 2020 2020 2020  :5000]).        
-00005bd0: 2020 2020 7463 6c75 7374 6572 2e73 686f      tcluster.sho
-00005be0: 775f 636c 7573 7465 7273 2866 6561 7475  w_clusters(featu
-00005bf0: 7265 2c20 6c61 6265 6c73 2c20 276d 6f64  re, labels, 'mod
-00005c00: 656c 732f 636c 7573 7465 722f 636c 7573  els/cluster/clus
-00005c10: 7465 725f 7472 6169 6e5f 7365 675f 7361  ter_train_seg_sa
-00005c20: 6d70 6c65 732e 706e 6727 290a 2020 2020  mples.png').    
-00005c30: 2020 2020 2020 2020 7220 3d20 7463 6c75          r = tclu
-00005c40: 7374 6572 2e70 7265 6469 6374 2864 6174  ster.predict(dat
-00005c50: 615b 3a33 305d 290a 2020 2020 2020 2020  a[:30]).        
-00005c60: 2020 2020 7072 696e 7428 7229 0a20 2020      print(r).   
-00005c70: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
-00005c80: 200a 2020 2020 2020 2020 6f75 7470 7574   .        output
-00005c90: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
-00005ca0: 2020 2060 6060 0a20 2020 2020 2020 2054     ```.        T
-00005cb0: 6578 7443 6c75 7374 6572 2069 6e73 7461  extCluster insta
-00005cc0: 6e63 6520 284d 696e 6942 6174 6368 4b4d  nce (MiniBatchKM
-00005cd0: 6561 6e73 286e 5f63 6c75 7374 6572 733d  eans(n_clusters=
-00005ce0: 322c 206e 5f69 6e69 743d 3130 292c 203c  2, n_init=10), <
-00005cf0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00005d00: 2e75 7469 6c73 2e74 6f6b 656e 697a 6572  .utils.tokenizer
-00005d10: 2e54 6f6b 656e 697a 6572 206f 626a 6563  .Tokenizer objec
-00005d20: 7420 6174 2030 7837 6638 3062 6434 3638  t at 0x7f80bd468
-00005d30: 3262 303e 2c20 5466 6964 6656 6563 746f  2b0>, TfidfVecto
-00005d40: 7269 7a65 7228 6e67 7261 6d5f 7261 6e67  rizer(ngram_rang
-00005d50: 653d 2831 2c20 3229 2929 0a20 2020 2020  e=(1, 2))).     
-00005d60: 2020 205b 3120 3120 3120 3120 3120 3120     [1 1 1 1 1 1 
-00005d70: 3120 3120 3120 3120 3120 3820 3120 3120  1 1 1 1 1 8 1 1 
-00005d80: 3120 3120 3120 3120 3120 3120 3120 3120  1 1 1 1 1 1 1 1 
-00005d90: 3920 3120 3120 3820 3120 3120 3920 315d  9 1 1 8 1 1 9 1]
-00005da0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00005db0: 2020 2020 2063 6c75 7374 6572 696e 6720       clustering 
-00005dc0: 706c 6f74 2069 6d61 6765 3a0a 2020 2020  plot image:.    
-00005dd0: 2020 2020 0a20 2020 2020 2020 2021 5b63      .        ![c
-00005de0: 6c75 7374 6572 5f69 6d61 6765 5d28 646f  luster_image](do
-00005df0: 6373 2f63 6c75 7374 6572 5f74 7261 696e  cs/cluster_train
-00005e00: 5f73 6567 5f73 616d 706c 6573 2e70 6e67  _seg_samples.png
-00005e10: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-00005e20: 2020 200a 2020 2020 2020 2020 2320 436f     .        # Co
-00005e30: 6e74 6163 740a 2020 2020 2020 2020 0a20  ntact.        . 
-00005e40: 2020 2020 2020 202d 2049 7373 7565 28e5         - Issue(.
-00005e50: bbba e8ae ae29 efbc 9a5b 215b 4769 7448  .....)...[![GitH
-00005e60: 7562 2069 7373 7565 735d 2868 7474 7073  ub issues](https
-00005e70: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00005e80: 6f2f 6769 7468 7562 2f69 7373 7565 732f  o/github/issues/
-00005e90: 7368 6962 696e 6736 3234 2f70 7974 6578  shibing624/pytex
-00005ea0: 7463 6c61 7373 6966 6965 722e 7376 6729  tclassifier.svg)
-00005eb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00005ec0: 2e63 6f6d 2f73 6869 6269 6e67 3632 342f  .com/shibing624/
-00005ed0: 7079 7465 7874 636c 6173 7369 6669 6572  pytextclassifier
-00005ee0: 2f69 7373 7565 7329 0a20 2020 2020 2020  /issues).       
-00005ef0: 202d 20e9 82ae e4bb b6e6 8891 efbc 9a78   - ............x
-00005f00: 756d 696e 673a 2078 756d 696e 6736 3234  uming: xuming624
-00005f10: 4071 712e 636f 6d0a 2020 2020 2020 2020  @qq.com.        
-00005f20: 2d20 e5be aee4 bfa1 e688 91ef bc9a e58a  - ..............
-00005f30: a0e6 8891 2ae5 beae e4bf a1e5 8fb7 efbc  ....*...........
-00005f40: 9a78 756d 696e 6736 3234 2a2c 20e8 bf9b  .xuming624*, ...
-00005f50: 5079 7468 6f6e 2d4e 4c50 e4ba a4e6 b581  Python-NLP......
-00005f60: e7be a4ef bc8c e5a4 87e6 b3a8 efbc 9a2a  ...............*
-00005f70: e5a7 93e5 908d 2de5 85ac e58f b8e5 908d  ......-.........
-00005f80: 2d4e 4c50 2a0a 2020 2020 2020 2020 3c69  -NLP*.        <i
-00005f90: 6d67 2073 7263 3d22 646f 6373 2f77 6563  mg src="docs/wec
-00005fa0: 6861 742e 6a70 6567 2220 7769 6474 683d  hat.jpeg" width=
-00005fb0: 2232 3030 2220 2f3e 0a20 2020 2020 2020  "200" />.       
-00005fc0: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
-00005fd0: 2020 2023 2043 6974 6174 696f 6e0a 2020     # Citation.  
-00005fe0: 2020 2020 2020 0a20 2020 2020 2020 20e5        .        .
-00005ff0: a682 e69e 9ce4 bda0 e59c a8e7 a094 e7a9  ................
-00006000: b6e4 b8ad e4bd bfe7 94a8 e4ba 8670 7974  .............pyt
-00006010: 6578 7463 6c61 7373 6966 6965 72ef bc8c  extclassifier...
-00006020: e8af b7e6 8c89 e5a6 82e4 b88b e6a0 bce5  ................
-00006030: bc8f e5bc 95e7 94a8 efbc 9a0a 2020 2020  ............    
-00006040: 2020 2020 0a20 2020 2020 2020 2041 5041      .        APA
-00006050: 3a0a 2020 2020 2020 2020 6060 606c 6174  :.        ```lat
-00006060: 6578 0a20 2020 2020 2020 2058 752c 204d  ex.        Xu, M
-00006070: 2e20 5079 7465 7874 636c 6173 7369 6669  . Pytextclassifi
-00006080: 6572 3a20 5465 7874 2063 6c61 7373 6966  er: Text classif
-00006090: 6965 7220 746f 6f6c 6b69 7420 666f 7220  ier toolkit for 
-000060a0: 4e4c 5020 2856 6572 7369 6f6e 2031 2e32  NLP (Version 1.2
-000060b0: 2e30 2920 5b43 6f6d 7075 7465 7220 736f  .0) [Computer so
-000060c0: 6674 7761 7265 5d2e 2068 7474 7073 3a2f  ftware]. https:/
-000060d0: 2f67 6974 6875 622e 636f 6d2f 7368 6962  /github.com/shib
-000060e0: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
-000060f0: 7373 6966 6965 720a 2020 2020 2020 2020  ssifier.        
-00006100: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
-00006110: 2020 2020 2042 6962 5465 583a 0a20 2020       BibTeX:.   
-00006120: 2020 2020 2060 6060 6c61 7465 780a 2020       ```latex.  
-00006130: 2020 2020 2020 406d 6973 637b 5079 7465        @misc{Pyte
-00006140: 7874 636c 6173 7369 6669 6572 2c0a 2020  xtclassifier,.  
-00006150: 2020 2020 2020 2020 7469 746c 653d 7b50          title={P
-00006160: 7974 6578 7463 6c61 7373 6966 6965 723a  ytextclassifier:
-00006170: 2054 6578 7420 636c 6173 7369 6669 6572   Text classifier
-00006180: 2074 6f6f 6c6b 6974 2066 6f72 204e 4c50   toolkit for NLP
-00006190: 7d2c 0a20 2020 2020 2020 2020 2061 7574  },.          aut
-000061a0: 686f 723d 7b58 7520 4d69 6e67 7d2c 0a20  hor={Xu Ming},. 
-000061b0: 2020 2020 2020 2020 2079 6561 723d 7b32           year={2
-000061c0: 3032 327d 2c0a 2020 2020 2020 2020 2020  022},.          
-000061d0: 686f 7770 7562 6c69 7368 6564 3d7b 5c75  howpublished={\u
-000061e0: 726c 7b68 7474 7073 3a2f 2f67 6974 6875  rl{https://githu
-000061f0: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
-00006200: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
-00006210: 727d 7d2c 0a20 2020 2020 2020 207d 0a20  r}},.        }. 
-00006220: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00006230: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00006240: 2020 2020 2023 204c 6963 656e 7365 0a20       # License. 
-00006250: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006260: 0a20 2020 2020 2020 20e6 8e88 e69d 83e5  .        .......
-00006270: 8d8f e8ae aee4 b8ba 205b 5468 6520 4170  ........ [The Ap
-00006280: 6163 6865 204c 6963 656e 7365 2032 2e30  ache License 2.0
-00006290: 5d28 4c49 4345 4e53 4529 efbc 8ce5 8faf  ](LICENSE)......
-000062a0: e585 8de8 b4b9 e794 a8e5 819a e595 86e4  ................
-000062b0: b89a e794 a8e9 8094 e380 82e8 afb7 e59c  ................
-000062c0: a8e4 baa7 e593 81e8 afb4 e698 8ee4 b8ad  ................
-000062d0: e999 84e5 8aa0 2a2a 7079 7465 7874 636c  ......**pytextcl
-000062e0: 6173 7369 6669 6572 2a2a e79a 84e9 93be  assifier**......
-000062f0: e68e a5e5 928c e68e 88e6 9d83 e58d 8fe8  ................
-00006300: aeae e380 820a 2020 2020 2020 2020 0a20  ......        . 
-00006310: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006320: 2320 436f 6e74 7269 6275 7465 0a20 2020  # Contribute.   
-00006330: 2020 2020 20e9 a1b9 e79b aee4 bba3 e7a0       ...........
-00006340: 81e8 bf98 e5be 88e7 b297 e7b3 99ef bc8c  ................
-00006350: e5a6 82e6 9e9c e5a4 a7e5 aeb6 e5af b9e4  ................
-00006360: bba3 e7a0 81e6 9c89 e689 80e6 94b9 e8bf  ................
-00006370: 9bef bc8c e6ac a2e8 bf8e e68f 90e4 baa4  ................
-00006380: e59b 9ee6 9cac e9a1 b9e7 9bae efbc 8ce5  ................
-00006390: 9ca8 e68f 90e4 baa4 e4b9 8be5 898d efbc  ................
-000063a0: 8ce6 b3a8 e684 8fe4 bba5 e4b8 8be4 b8a4  ................
-000063b0: e782 b9ef bc9a 0a20 2020 2020 2020 200a  .......        .
-000063c0: 2020 2020 2020 2020 202d 20e5 9ca8 6074           - ...`t
-000063d0: 6573 7473 60e6 b7bb e58a a0e7 9bb8 e5ba  ests`...........
-000063e0: 94e7 9a84 e58d 95e5 8583 e6b5 8be8 af95  ................
-000063f0: 0a20 2020 2020 2020 2020 2d20 e4bd bfe7  .         - ....
-00006400: 94a8 6070 7974 686f 6e20 7365 7475 702e  ..`python setup.
-00006410: 7079 2074 6573 7460 e69d a5e8 bf90 e8a1  py test`........
-00006420: 8ce6 8980 e69c 89e5 8d95 e585 83e6 b58b  ................
-00006430: e8af 95ef bc8c e7a1 aee4 bf9d e689 80e6  ................
-00006440: 9c89 e58d 95e6 b58b e983 bde6 98af e980  ................
-00006450: 9ae8 bf87 e79a 840a 2020 2020 2020 2020  ........        
-00006460: 0a20 2020 2020 2020 20e4 b98b e590 8ee5  .        .......
-00006470: 8db3 e58f afe6 8f90 e4ba a450 52e3 8082  ...........PR...
-00006480: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006490: 2020 0a20 2020 2020 2020 2023 2052 6566    .        # Ref
-000064a0: 6572 656e 6365 0a20 2020 2020 2020 200a  erence.        .
-000064b0: 2020 2020 2020 2020 2d20 5365 6e74 696d          - Sentim
-000064c0: 656e 7450 6f6c 6172 6974 7941 6e61 6c79  entPolarityAnaly
-000064d0: 7369 730a 2020 2020 2020 2020 0a4b 6579  sis.        .Key
-000064e0: 776f 7264 733a 2070 7974 6578 7463 6c61  words: pytextcla
-000064f0: 7373 6966 6965 722c 7465 7874 636c 6173  ssifier,textclas
-00006500: 7369 6669 6572 2c63 6c61 7373 6966 6965  sifier,classifie
-00006510: 722c 7465 7874 636c 6173 7369 6669 6361  r,textclassifica
-00006520: 7469 6f6e 0a50 6c61 7466 6f72 6d3a 2055  tion.Platform: U
-00006530: 4e4b 4e4f 574e 0a43 6c61 7373 6966 6965  NKNOWN.Classifie
-00006540: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00006550: 656e 6365 203a 3a20 5363 6965 6e63 652f  ence :: Science/
-00006560: 5265 7365 6172 6368 0a43 6c61 7373 6966  Research.Classif
-00006570: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-00006580: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00006590: 7065 6e64 656e 740a 436c 6173 7369 6669  pendent.Classifi
-000065a0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-000065b0: 5349 2041 7070 726f 7665 6420 3a3a 2041  SI Approved :: A
-000065c0: 7061 6368 6520 536f 6674 7761 7265 204c  pache Software L
-000065d0: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
-000065e0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000065f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00006600: 6e0a 436c 6173 7369 6669 6572 3a20 5072  n.Classifier: Pr
-00006610: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00006620: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00006630: 322e 370a 436c 6173 7369 6669 6572 3a20  2.7.Classifier: 
-00006640: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00006650: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00006660: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
-00006670: 546f 7069 6320 3a3a 2054 6578 7420 5072  Topic :: Text Pr
-00006680: 6f63 6573 7369 6e67 203a 3a20 4c69 6e67  ocessing :: Ling
-00006690: 7569 7374 6963 0a43 6c61 7373 6966 6965  uistic.Classifie
-000066a0: 723a 2054 6f70 6963 203a 3a20 5363 6965  r: Topic :: Scie
-000066b0: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
-000066c0: 6e67 203a 3a20 4172 7469 6669 6369 616c  ng :: Artificial
-000066d0: 2049 6e74 656c 6c69 6765 6e63 650a 4465   Intelligence.De
-000066e0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-000066f0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00006700: 6b64 6f77 6e0a                           kdown.
+000046f0: 2020 6966 206e 6f74 206c 696e 653a 0a20    if not line:. 
+00004700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004710: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004730: 2020 2020 7465 726d 7320 3d20 6c69 6e65      terms = line
+00004740: 2e73 706c 6974 2827 2c27 290a 2020 2020  .split(',').    
+00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004760: 6966 206c 656e 2874 6572 6d73 2920 213d  if len(terms) !=
+00004770: 2031 363a 0a20 2020 2020 2020 2020 2020   16:.           
+00004780: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00004790: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+000047a0: 2020 2020 2020 2020 2020 7661 6c20 3d20            val = 
+000047b0: 5b69 6e74 2869 2920 666f 7220 6920 696e  [int(i) for i in
+000047c0: 2074 6572 6d73 5b31 3a5d 5d0a 2020 2020   terms[1:]].    
+000047d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047e0: 6461 7461 2e61 7070 656e 6428 5b74 6572  data.append([ter
+000047f0: 6d73 5b30 5d2c 2076 616c 5d29 0a20 2020  ms[0], val]).   
+00004800: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004810: 6461 7461 0a20 2020 2020 2020 200a 2020  data.        .  
+00004820: 2020 2020 2020 0a20 2020 2020 2020 2069        .        i
+00004830: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 275f  f __name__ == '_
+00004840: 5f6d 6169 6e5f 5f27 3a0a 2020 2020 2020  _main__':.      
+00004850: 2020 2020 2020 2320 6d6f 6465 6c5f 7479        # model_ty
+00004860: 7065 3a20 7375 7070 6f72 7420 2762 6572  pe: support 'ber
+00004870: 7427 2c20 2761 6c62 6572 7427 2c20 2772  t', 'albert', 'r
+00004880: 6f62 6572 7461 272c 2027 786c 6e65 7427  oberta', 'xlnet'
+00004890: 0a20 2020 2020 2020 2020 2020 2023 206d  .            # m
+000048a0: 6f64 656c 5f6e 616d 653a 2073 7570 706f  odel_name: suppo
+000048b0: 7274 2027 6265 7274 2d62 6173 652d 6368  rt 'bert-base-ch
+000048c0: 696e 6573 6527 2c20 2762 6572 742d 6261  inese', 'bert-ba
+000048d0: 7365 2d63 6173 6564 272c 2027 6265 7274  se-cased', 'bert
+000048e0: 2d62 6173 652d 6d75 6c74 696c 696e 6775  -base-multilingu
+000048f0: 616c 2d63 6173 6564 2720 2e2e 2e0a 2020  al-cased' ....  
+00004900: 2020 2020 2020 2020 2020 6d20 3d20 4265            m = Be
+00004910: 7274 436c 6173 7369 6669 6572 286f 7574  rtClassifier(out
+00004920: 7075 745f 6469 723d 276d 6f64 656c 732f  put_dir='models/
+00004930: 6d75 6c74 696c 6162 656c 2d62 6572 742d  multilabel-bert-
+00004940: 7a68 2d6d 6f64 656c 272c 206e 756d 5f63  zh-model', num_c
+00004950: 6c61 7373 6573 3d31 352c 0a20 2020 2020  lasses=15,.     
+00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004970: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+00004980: 7479 7065 3d27 6265 7274 272c 206d 6f64  type='bert', mod
+00004990: 656c 5f6e 616d 653d 2762 6572 742d 6261  el_name='bert-ba
+000049a0: 7365 2d63 6869 6e65 7365 272c 206e 756d  se-chinese', num
+000049b0: 5f65 706f 6368 733d 322c 206d 756c 7469  _epochs=2, multi
+000049c0: 5f6c 6162 656c 3d54 7275 6529 0a20 2020  _label=True).   
+000049d0: 2020 2020 2020 2020 2023 2054 7261 696e           # Train
+000049e0: 2061 6e64 2045 7661 6c75 6174 696f 6e20   and Evaluation 
+000049f0: 6461 7461 206e 6565 6473 2074 6f20 6265  data needs to be
+00004a00: 2069 6e20 6120 5061 6e64 6173 2044 6174   in a Pandas Dat
+00004a10: 6166 7261 6d65 2063 6f6e 7461 696e 696e  aframe containin
+00004a20: 6720 6174 206c 6561 7374 2074 776f 2063  g at least two c
+00004a30: 6f6c 756d 6e73 2c20 6120 2774 6578 7427  olumns, a 'text'
+00004a40: 2061 6e64 2061 2027 6c61 6265 6c73 2720   and a 'labels' 
+00004a50: 636f 6c75 6d6e 2e20 5468 6520 606c 6162  column. The `lab
+00004a60: 656c 7360 2063 6f6c 756d 6e20 7368 6f75  els` column shou
+00004a70: 6c64 2063 6f6e 7461 696e 206d 756c 7469  ld contain multi
+00004a80: 2d68 6f74 2065 6e63 6f64 6564 206c 6973  -hot encoded lis
+00004a90: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
+00004aa0: 7472 6169 6e5f 6461 7461 203d 205b 0a20  train_data = [. 
+00004ab0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00004ac0: 22e4 b880 e4b8 aae5 b08f e697 b6e6 88bf  "...............
+00004ad0: e997 b4e4 bb8d e784 b6e6 b2a1 e69a 96e5  ................
+00004ae0: 928c 222c 205b 302c 2030 2c20 302c 2030  ..", [0, 0, 0, 0
+00004af0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00004b00: 2030 2c20 302c 2030 2c20 312c 2030 2c20   0, 0, 0, 1, 0, 
+00004b10: 305d 5d2c 0a20 2020 2020 2020 2020 2020  0]],.           
+00004b20: 2020 2020 205b 22e8 8097 e794 b5e6 8385       [".........
+00004b30: e586 b5ef bc9a e8bf 99e4 b8aa e6b2 a1e6  ................
+00004b40: 9c89 e6b3 a8e6 848f 222c 205b 302c 2030  ........", [0, 0
+00004b50: 2c20 312c 2030 2c20 302c 2030 2c20 302c  , 1, 0, 0, 0, 0,
+00004b60: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00004b70: 302c 2030 2c20 305d 5d2c 0a20 2020 2020  0, 0, 0]],.     
+00004b80: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00004b90: 2020 2020 2064 6174 6120 3d20 6c6f 6164       data = load
+00004ba0: 5f6a 645f 6461 7461 2827 6d75 6c74 696c  _jd_data('multil
+00004bb0: 6162 656c 5f6a 645f 636f 6d6d 656e 7473  abel_jd_comments
+00004bc0: 2e63 7376 2729 0a20 2020 2020 2020 2020  .csv').         
+00004bd0: 2020 2074 7261 696e 5f64 6174 612e 6578     train_data.ex
+00004be0: 7465 6e64 2864 6174 6129 0a20 2020 2020  tend(data).     
+00004bf0: 2020 2020 2020 2070 7269 6e74 2874 7261         print(tra
+00004c00: 696e 5f64 6174 615b 3a35 5d29 0a20 2020  in_data[:5]).   
+00004c10: 2020 2020 2020 2020 2074 7261 696e 5f64           train_d
+00004c20: 6620 3d20 7064 2e44 6174 6146 7261 6d65  f = pd.DataFrame
+00004c30: 2874 7261 696e 5f64 6174 612c 2063 6f6c  (train_data, col
+00004c40: 756d 6e73 3d5b 2274 6578 7422 2c20 226c  umns=["text", "l
+00004c50: 6162 656c 7322 5d29 0a20 2020 2020 2020  abels"]).       
+00004c60: 200a 2020 2020 2020 2020 2020 2020 7072   .            pr
+00004c70: 696e 7428 7472 6169 6e5f 6466 2e68 6561  int(train_df.hea
+00004c80: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
+00004c90: 206d 2e74 7261 696e 2874 7261 696e 5f64   m.train(train_d
+00004ca0: 6629 0a20 2020 2020 2020 2020 2020 2070  f).            p
+00004cb0: 7269 6e74 286d 290a 2020 2020 2020 2020  rint(m).        
+00004cc0: 2020 2020 2320 4576 616c 7561 7465 2074      # Evaluate t
+00004cd0: 6865 206d 6f64 656c 0a20 2020 2020 2020  he model.       
+00004ce0: 2020 2020 2061 6363 5f73 636f 7265 203d       acc_score =
+00004cf0: 206d 2e65 7661 6c75 6174 655f 6d6f 6465   m.evaluate_mode
+00004d00: 6c28 7472 6169 6e5f 6466 5b3a 3230 5d29  l(train_df[:20])
+00004d10: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00004d20: 6e74 2866 2761 6363 5f73 636f 7265 3a20  nt(f'acc_score: 
+00004d30: 7b61 6363 5f73 636f 7265 7d27 290a 2020  {acc_score}').  
+00004d40: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00004d50: 2020 2023 206c 6f61 6420 7472 6169 6e65     # load traine
+00004d60: 6420 6265 7374 206d 6f64 656c 2066 726f  d best model fro
+00004d70: 6d20 6d6f 6465 6c5f 6469 720a 2020 2020  m model_dir.    
+00004d80: 2020 2020 2020 2020 6d2e 6c6f 6164 5f6d          m.load_m
+00004d90: 6f64 656c 2829 0a20 2020 2020 2020 2020  odel().         
+00004da0: 2020 2070 7265 6469 6374 5f6c 6162 656c     predict_label
+00004db0: 2c20 7072 6564 6963 745f 7072 6f62 6120  , predict_proba 
+00004dc0: 3d20 6d2e 7072 6564 6963 7428 5b27 e4b8  = m.predict(['..
+00004dd0: 80e4 b8aa e5b0 8fe6 97b6 e688 bfe9 97b4  ................
+00004de0: e4bb 8de7 84b6 e6b2 a1e6 9a96 e592 8c27  ...............'
+00004df0: 2c20 27e8 8097 e794 b5e6 8385 e586 b5ef  , '.............
+00004e00: bc9a e8bf 99e4 b8aa e6b2 a1e6 9c89 e6b3  ................
+00004e10: a8e6 848f 275d 290a 2020 2020 2020 2020  ....']).        
+00004e20: 2020 2020 7072 696e 7428 6627 7072 6564      print(f'pred
+00004e30: 6963 745f 6c61 6265 6c3a 207b 7072 6564  ict_label: {pred
+00004e40: 6963 745f 6c61 6265 6c7d 2c20 7072 6564  ict_label}, pred
+00004e50: 6963 745f 7072 6f62 613a 207b 7072 6564  ict_proba: {pred
+00004e60: 6963 745f 7072 6f62 617d 2729 0a20 2020  ict_proba}').   
+00004e70: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+00004e80: 200a 2020 2020 2020 2020 2323 2045 7661   .        ## Eva
+00004e90: 6c75 6174 696f 6e0a 2020 2020 2020 2020  luation.        
+00004ea0: 0a20 2020 2020 2020 2023 2323 2044 6174  .        ### Dat
+00004eb0: 6173 6574 0a20 2020 2020 2020 200a 2020  aset.        .  
+00004ec0: 2020 2020 2020 312e 2054 4855 434e 6577        1. THUCNew
+00004ed0: 73e4 b8ad e696 87e6 9687 e69c ace6 95b0  s...............
+00004ee0: e68d aee9 9b86 efbc 8831 2e35 3647 42ef  .........1.56GB.
+00004ef0: bc89 efbc 9ae5 ae98 e696 b95b e4b8 8be8  ...........[....
+00004f00: bdbd e59c b0e5 9d80 5d28 6874 7470 3a2f  ........](http:/
+00004f10: 2f74 6875 6374 632e 7468 756e 6c70 2e6f  /thuctc.thunlp.o
+00004f20: 7267 2f29 efbc 8ce6 8abd e6a0 b7e4 ba86  rg/)............
+00004f30: 3130 e4b8 87e6 9da1 5448 5543 4e65 7773  10......THUCNews
+00004f40: e4b8 ade6 9687 e696 87e6 9cac 3130 e588  ............10..
+00004f50: 86e7 b1bb e695 b0e6 8dae e99b 86ef bc88  ................
+00004f60: 364d 42ef bc89 efbc 8ce5 9cb0 e59d 80ef  6MB.............
+00004f70: bc9a 5b65 7861 6d70 6c65 732f 7468 7563  ..[examples/thuc
+00004f80: 6e65 7773 5f74 7261 696e 5f31 3077 2e74  news_train_10w.t
+00004f90: 7874 5d28 6874 7470 733a 2f2f 6769 7468  xt](https://gith
+00004fa0: 7562 2e63 6f6d 2f73 6869 6269 6e67 3632  ub.com/shibing62
+00004fb0: 342f 7079 7465 7874 636c 6173 7369 6669  4/pytextclassifi
+00004fc0: 6572 2f62 6c6f 622f 6d61 7374 6572 2f65  er/blob/master/e
+00004fd0: 7861 6d70 6c65 732f 7468 7563 6e65 7773  xamples/thucnews
+00004fe0: 5f74 7261 696e 5f31 3077 2e74 7874 29e3  _train_10w.txt).
+00004ff0: 8082 0a20 2020 2020 2020 2032 2e20 544e  ...        2. TN
+00005000: 4557 53e4 bb8a e697 a5e5 a4b4 e69d a1e4  EWS.............
+00005010: b8ad e696 87e6 96b0 e997 bbef bc88 e79f  ................
+00005020: ade6 9687 e69c acef bc89 e588 86e7 b1bb  ................
+00005030: 2053 686f 7274 2054 6578 7420 436c 6173   Short Text Clas
+00005040: 7369 6669 6361 6974 6f6e 2066 6f72 204e  sificaiton for N
+00005050: 6577 73ef bc8c e8af a5e6 95b0 e68d aee9  ews.............
+00005060: 9b86 2835 2e31 4d42 29e6 9da5 e887 aae4  ..(5.1MB).......
+00005070: bb8a e697 a5e5 a4b4 e69d a1e7 9a84 e696  ................
+00005080: b0e9 97bb e789 88e5 9d97 efbc 8ce5 85b1  ................
+00005090: e68f 90e5 8f96 e4ba 8631 35e4 b8aa e7b1  .........15.....
+000050a0: bbe5 88ab e79a 84e6 96b0 e997 bbef bc8c  ................
+000050b0: e58c 85e6 8bac e697 85e6 b8b8 efbc 8ce6  ................
+000050c0: 9599 e882 b2ef bc8c e987 91e8 9e8d efbc  ................
+000050d0: 8ce5 869b e4ba 8be7 ad89 efbc 8ce5 9cb0  ................
+000050e0: e59d 80ef bc9a 5b74 6e65 7773 5f70 7562  ......[tnews_pub
+000050f0: 6c69 632e 7a69 705d 2868 7474 7073 3a2f  lic.zip](https:/
+00005100: 2f73 746f 7261 6765 2e67 6f6f 676c 6561  /storage.googlea
+00005110: 7069 732e 636f 6d2f 636c 7565 6265 6e63  pis.com/cluebenc
+00005120: 686d 6172 6b2f 7461 736b 732f 746e 6577  hmark/tasks/tnew
+00005130: 735f 7075 626c 6963 2e7a 6970 290a 2020  s_public.zip).  
+00005140: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00005150: 2323 2045 7661 6c75 6174 696f 6e20 5265  ## Evaluation Re
+00005160: 7375 6c74 0a20 2020 2020 2020 20e5 9ca8  sult.        ...
+00005170: 5448 5543 4e65 7773 e4b8 ade6 9687 e696  THUCNews........
+00005180: 87e6 9cac 3130 e588 86e7 b1bb e695 b0e6  ....10..........
+00005190: 8dae e99b 86ef bc88 364d 42ef bc89 e4b8  ........6MB.....
+000051a0: 8ae8 af84 e4bc b0ef bc8c e6a8 a1e5 9e8b  ................
+000051b0: e59c a8e6 b58b e8af 95e9 9b86 2874 6573  ............(tes
+000051c0: 7429 e8af 84e6 b58b e695 88e6 9e9c e5a6  t)..............
+000051d0: 82e4 b88b efbc 9a0a 2020 2020 2020 2020  ........        
+000051e0: 0a20 2020 2020 2020 20e6 a8a1 e59e 8b7c  .        ......|
+000051f0: 6163 637c e8af b4e6 988e 0a20 2020 2020  acc|.......     
+00005200: 2020 202d 2d7c 2d2d 7c2d 2d0a 2020 2020     --|--|--.    
+00005210: 2020 2020 4c52 7c30 2e38 3830 337c e980      LR|0.8803|..
+00005220: bbe8 be91 e59b 9ee5 bd92 4c6f 6769 7374  ..........Logist
+00005230: 6963 7320 5265 6772 6573 7369 6f6e 0a20  ics Regression. 
+00005240: 2020 2020 2020 2054 6578 7443 4e4e 7c30         TextCNN|0
+00005250: 2e38 3830 397c 4b69 6d20 3230 3134 20e7  .8809|Kim 2014 .
+00005260: bb8f e585 b8e7 9a84 434e 4ee6 9687 e69c  ........CNN.....
+00005270: ace5 8886 e7b1 bb0a 2020 2020 2020 2020  ........        
+00005280: 5465 7874 524e 4e5f 4174 747c 302e 3930  TextRNN_Att|0.90
+00005290: 3232 7c42 694c 5354 4d2b 4174 7465 6e74  22|BiLSTM+Attent
+000052a0: 696f 6e0a 2020 2020 2020 2020 4661 7374  ion.        Fast
+000052b0: 5465 7874 7c30 2e39 3137 377c 626f 772b  Text|0.9177|bow+
+000052c0: 6269 6772 616d 2b74 7269 6772 616d efbc  bigram+trigram..
+000052d0: 8c20 e695 88e6 9e9c e587 bae5 a587 e79a  . ..............
+000052e0: 84e5 a5bd 0a20 2020 2020 2020 2044 5043  .....        DPC
+000052f0: 4e4e 7c30 2e39 3132 357c e6b7 b1e5 b182  NN|0.9125|......
+00005300: e987 91e5 ad97 e5a1 9443 4e4e 0a20 2020  .........CNN.   
+00005310: 2020 2020 2054 7261 6e73 666f 726d 6572       Transformer
+00005320: 7c30 2e38 3939 317c e695 88e6 9e9c e8be  |0.8991|........
+00005330: 83e5 b7ae 0a20 2020 2020 2020 2042 4552  .....        BER
+00005340: 542d 6261 7365 7c2a 2a30 2e39 3438 332a  T-base|**0.9483*
+00005350: 2a7c 6265 7274 202b 2066 630a 2020 2020  *|bert + fc.    
+00005360: 2020 2020 4552 4e49 457c 302e 3934 3631      ERNIE|0.9461
+00005370: 7ce6 af94 6265 7274 e795 a5e5 b7ae 0a20  |...bert....... 
+00005380: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00005390: e59c a8e4 b8ad e696 87e6 96b0 e997 bbe7  ................
+000053a0: 9fad e696 87e6 9cac e588 86e7 b1bb e695  ................
+000053b0: b0e6 8dae e99b 8654 4e45 5753 e4b8 8ae8  .......TNEWS....
+000053c0: af84 e4bc b0ef bc8c e6a8 a1e5 9e8b e59c  ................
+000053d0: a8e5 bc80 e58f 91e9 9b86 2864 6576 29e8  ..........(dev).
+000053e0: af84 e6b5 8be6 9588 e69e 9ce5 a682 e4b8  ................
+000053f0: 8bef bc9a 0a20 2020 2020 2020 200a 2020  .....        .  
+00005400: 2020 2020 2020 e6a8 a1e5 9e8b 7c61 6363        ......|acc
+00005410: 7ce8 afb4 e698 8e0a 2020 2020 2020 2020  |.......        
+00005420: 2d2d 7c2d 2d7c 2d2d 0a20 2020 2020 2020  --|--|--.       
+00005430: 2042 4552 542d 6261 7365 7c2a 2a30 2e35   BERT-base|**0.5
+00005440: 3636 302a 2a7c e69c ace9 a1b9 e79b aee5  660**|..........
+00005450: ae9e e78e b00a 2020 2020 2020 2020 4245  ......        BE
+00005460: 5254 2d62 6173 657c 302e 3536 3039 7c43  RT-base|0.5609|C
+00005470: 4c55 4520 4265 6e63 686d 6172 6b20 4c65  LUE Benchmark Le
+00005480: 6164 6572 626f 6172 64e7 bb93 e69e 9c20  aderboard...... 
+00005490: 5b43 4c55 4562 656e 6368 6d61 726b 5d28  [CLUEbenchmark](
+000054a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000054b0: 6f6d 2f43 4c55 4562 656e 6368 6d61 726b  om/CLUEbenchmark
+000054c0: 2f43 4c55 4529 0a20 2020 2020 2020 200a  /CLUE).        .
+000054d0: 2020 2020 2020 2020 2d20 e4bb a5e4 b88a          - ......
+000054e0: e7bb 93e6 9e9c e59d 87e4 b8ba e588 86e7  ................
+000054f0: b1bb e79a 84e5 8786 e7a1 aee7 8e87 efbc  ................
+00005500: 8861 6363 7572 6163 79ef bc89 e7bb 93e6  .accuracy.......
+00005510: 9e9c 0a20 2020 2020 2020 202d 2054 4855  ...        - THU
+00005520: 434e 6577 73e6 95b0 e68d aee9 9b86 e8af  CNews...........
+00005530: 84e6 b58b e7bb 93e6 9e9c e58f afe4 bba5  ................
+00005540: e59f bae4 ba8e 6065 7861 6d70 6c65 732f  ......`examples/
+00005550: 7468 7563 6e65 7773 5f74 7261 696e 5f31  thucnews_train_1
+00005560: 3077 2e74 7874 60e6 95b0 e68d aee7 94a8  0w.txt`.........
+00005570: 6065 7861 6d70 6c65 7360 e4b8 8be7 9a84  `examples`......
+00005580: e590 84e6 a8a1 e59e 8b64 656d 6fe5 a48d  .........demo...
+00005590: e78e b00a 2020 2020 2020 2020 2d20 544e  ....        - TN
+000055a0: 4557 53e6 95b0 e68d aee9 9b86 e8af 84e6  EWS.............
+000055b0: b58b e7bb 93e6 9e9c e58f afe4 bba5 e4b8  ................
+000055c0: 8be8 bdbd 544e 4557 53e6 95b0 e68d aee9  ....TNEWS.......
+000055d0: 9b86 efbc 8ce8 bf90 e8a1 8c60 6578 616d  ...........`exam
+000055e0: 706c 6573 2f62 6572 745f 636c 6173 7369  ples/bert_classi
+000055f0: 6669 6361 7469 6f6e 5f74 6e65 7773 5f64  fication_tnews_d
+00005600: 656d 6f2e 7079 60e5 a48d e78e b00a 2020  emo.py`.......  
+00005610: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
+00005620: 2323 20e5 91bd e4bb a4e8 a18c e8b0 83e7  ## .............
+00005630: 94a8 0a20 2020 2020 2020 200a 2020 2020  ...        .    
+00005640: 2020 2020 e68f 90e4 be9b e588 86e7 b1bb      ............
+00005650: e6a8 a1e5 9e8b e591 bde4 bba4 e8a1 8ce8  ................
+00005660: b083 e794 a8e8 849a e69c acef bc8c e696  ................
+00005670: 87e4 bbb6 e6a0 91ef bc9a 0a20 2020 2020  ...........     
+00005680: 2020 2060 6060 6261 7368 0a20 2020 2020     ```bash.     
+00005690: 2020 2070 7974 6578 7463 6c61 7373 6966     pytextclassif
+000056a0: 6965 720a 2020 2020 2020 2020 e294 9ce2  ier.        ....
+000056b0: 9480 e294 8020 6265 7274 5f63 6c61 7373  ..... bert_class
+000056c0: 6966 6965 722e 7079 0a20 2020 2020 2020  ifier.py.       
+000056d0: 20e2 949c e294 80e2 9480 2066 6173 7474   ......... fastt
+000056e0: 6578 745f 636c 6173 7369 6669 6572 2e70  ext_classifier.p
+000056f0: 790a 2020 2020 2020 2020 e294 9ce2 9480  y.        ......
+00005700: e294 8020 636c 6173 7369 635f 636c 6173  ... classic_clas
+00005710: 7369 6669 6572 2e70 790a 2020 2020 2020  sifier.py.      
+00005720: 2020 e294 9ce2 9480 e294 8020 7465 7874    ......... text
+00005730: 636e 6e5f 636c 6173 7369 6669 6572 2e70  cnn_classifier.p
+00005740: 790a 2020 2020 2020 2020 e294 94e2 9480  y.        ......
+00005750: e294 8020 7465 7874 726e 6e5f 636c 6173  ... textrnn_clas
+00005760: 7369 6669 6572 2e70 790a 2020 2020 2020  sifier.py.      
+00005770: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
+00005780: 2020 2020 2020 20e6 af8f e4b8 aae6 9687         .........
+00005790: e4bb b6e5 afb9 e5ba 94e4 b880 e4b8 aae6  ................
+000057a0: a8a1 e59e 8be6 96b9 e6b3 95ef bc8c e590  ................
+000057b0: 84e6 a8a1 e59e 8be5 ae8c e585 a8e7 8bac  ................
+000057c0: e7ab 8bef bc8c e58f afe4 bba5 e79b b4e6  ................
+000057d0: 8ea5 e8bf 90e8 a18c efbc 8ce4 b99f e696  ................
+000057e0: b9e4 bebf e4bf aee6 94b9 efbc 8ce6 94af  ................
+000057f0: e68c 81e9 809a e8bf 8760 6172 6770 6172  .........`argpar
+00005800: 7365 6020 e4bf aee6 94b9 602d 2d64 6174  se` ......`--dat
+00005810: 615f 7061 7468 60e7 ad89 e58f 82e6 95b0  a_path`.........
+00005820: e380 820a 2020 2020 2020 2020 0a20 2020  ....        .   
+00005830: 2020 2020 20e7 9bb4 e68e a5e5 9ca8 e7bb       ...........
+00005840: 88e7 abaf e8b0 83e7 94a8 6661 7374 7465  ..........fastte
+00005850: 7874 e6a8 a1e5 9e8b e8ae ade7 bb83 efbc  xt..............
+00005860: 9a0a 2020 2020 2020 2020 6060 6062 6173  ..        ```bas
+00005870: 680a 2020 2020 2020 2020 7079 7468 6f6e  h.        python
+00005880: 202d 6d20 7079 7465 7874 636c 6173 7369   -m pytextclassi
+00005890: 6669 6572 2e66 6173 7474 6578 745f 636c  fier.fasttext_cl
+000058a0: 6173 7369 6669 6572 202d 680a 2020 2020  assifier -h.    
+000058b0: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
+000058c0: 0a20 2020 2020 2020 2023 2320 5465 7874  .        ## Text
+000058d0: 2043 6c75 7374 6572 0a20 2020 2020 2020   Cluster.       
+000058e0: 200a 2020 2020 2020 2020 0a20 2020 2020   .        .     
+000058f0: 2020 2054 6578 7420 636c 7573 7465 7269     Text clusteri
+00005900: 6e67 2c20 666f 7220 6578 616d 706c 6520  ng, for example 
+00005910: 5b65 7861 6d70 6c65 732f 636c 7573 7465  [examples/cluste
+00005920: 725f 6465 6d6f 2e70 795d 2868 7474 7073  r_demo.py](https
+00005930: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
+00005940: 6962 696e 6736 3234 2f70 7974 6578 7463  ibing624/pytextc
+00005950: 6c61 7373 6966 6965 722f 626c 6f62 2f6d  lassifier/blob/m
+00005960: 6173 7465 722f 6578 616d 706c 6573 2f63  aster/examples/c
+00005970: 6c75 7374 6572 5f64 656d 6f2e 7079 290a  luster_demo.py).
+00005980: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005990: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+000059a0: 2020 2069 6d70 6f72 7420 7379 730a 2020     import sys.  
+000059b0: 2020 2020 2020 0a20 2020 2020 2020 2073        .        s
+000059c0: 7973 2e70 6174 682e 6170 7065 6e64 2827  ys.path.append('
+000059d0: 2e2e 2729 0a20 2020 2020 2020 2066 726f  ..').        fro
+000059e0: 6d20 7079 7465 7874 636c 6173 7369 6669  m pytextclassifi
+000059f0: 6572 2e74 6578 7463 6c75 7374 6572 2069  er.textcluster i
+00005a00: 6d70 6f72 7420 5465 7874 436c 7573 7465  mport TextCluste
+00005a10: 720a 2020 2020 2020 2020 0a20 2020 2020  r.        .     
+00005a20: 2020 2069 6620 5f5f 6e61 6d65 5f5f 203d     if __name__ =
+00005a30: 3d20 275f 5f6d 6169 6e5f 5f27 3a0a 2020  = '__main__':.  
+00005a40: 2020 2020 2020 2020 2020 6d20 3d20 5465            m = Te
+00005a50: 7874 436c 7573 7465 7228 6f75 7470 7574  xtCluster(output
+00005a60: 5f64 6972 3d27 6d6f 6465 6c73 2f63 6c75  _dir='models/clu
+00005a70: 7374 6572 2d74 6f79 272c 206e 5f63 6c75  ster-toy', n_clu
+00005a80: 7374 6572 733d 3229 0a20 2020 2020 2020  sters=2).       
+00005a90: 2020 2020 2070 7269 6e74 286d 290a 2020       print(m).  
+00005aa0: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00005ab0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00005ac0: 2020 2027 5374 7564 656e 7420 6465 6274     'Student debt
+00005ad0: 2074 6f20 636f 7374 2042 7269 7461 696e   to cost Britain
+00005ae0: 2062 696c 6c69 6f6e 7320 7769 7468 696e   billions within
+00005af0: 2064 6563 6164 6573 272c 0a20 2020 2020   decades',.     
+00005b00: 2020 2020 2020 2020 2020 2027 4368 696e             'Chin
+00005b10: 6573 6520 6564 7563 6174 696f 6e20 666f  ese education fo
+00005b20: 7220 5456 2065 7870 6572 696d 656e 7427  r TV experiment'
+00005b30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005b40: 2020 2741 6262 6f74 7420 676f 7665 726e    'Abbott govern
+00005b50: 6d65 6e74 2073 7065 6e64 7320 2438 206d  ment spends $8 m
+00005b60: 696c 6c69 6f6e 206f 6e20 6869 6768 6572  illion on higher
+00005b70: 2065 6475 6361 7469 6f6e 272c 0a20 2020   education',.   
+00005b80: 2020 2020 2020 2020 2020 2020 2027 4d69               'Mi
+00005b90: 6464 6c65 2045 6173 7420 616e 6420 4173  ddle East and As
+00005ba0: 6961 2062 6f6f 7374 2069 6e76 6573 746d  ia boost investm
+00005bb0: 656e 7420 696e 2074 6f70 206c 6576 656c  ent in top level
+00005bc0: 2073 706f 7274 7327 2c0a 2020 2020 2020   sports',.      
+00005bd0: 2020 2020 2020 2020 2020 2753 756d 6d69            'Summi
+00005be0: 7420 5365 7269 6573 206c 6f6f 6b20 6c61  t Series look la
+00005bf0: 756e 6368 6573 2048 424f 2043 616e 6164  unches HBO Canad
+00005c00: 6120 7370 6f72 7473 2064 6f63 2073 6572  a sports doc ser
+00005c10: 6965 733a 204d 7564 6861 7227 0a20 2020  ies: Mudhar'.   
+00005c20: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00005c30: 2020 2020 2020 206d 2e74 7261 696e 2864         m.train(d
+00005c40: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
+00005c50: 206d 2e6c 6f61 645f 6d6f 6465 6c28 290a   m.load_model().
+00005c60: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
+00005c70: 6d2e 7072 6564 6963 7428 5b27 4162 626f  m.predict(['Abbo
+00005c80: 7474 2067 6f76 6572 6e6d 656e 7420 7370  tt government sp
+00005c90: 656e 6473 2024 3820 6d69 6c6c 696f 6e20  ends $8 million 
+00005ca0: 6f6e 2068 6967 6865 7220 6564 7563 6174  on higher educat
+00005cb0: 696f 6e20 6d65 6469 6120 626c 6974 7a27  ion media blitz'
+00005cc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005cd0: 2020 2020 2020 2020 2020 2020 2027 4d69               'Mi
+00005ce0: 6464 6c65 2045 6173 7420 616e 6420 4173  ddle East and As
+00005cf0: 6961 2062 6f6f 7374 2069 6e76 6573 746d  ia boost investm
+00005d00: 656e 7420 696e 2074 6f70 206c 6576 656c  ent in top level
+00005d10: 2073 706f 7274 7327 5d29 0a20 2020 2020   sports']).     
+00005d20: 2020 2020 2020 2070 7269 6e74 2872 290a         print(r).
+00005d30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00005d40: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+00005d50: 206c 6f61 6420 6368 696e 6573 6520 7472   load chinese tr
+00005d60: 6169 6e20 6461 7461 2066 726f 6d20 3177  ain data from 1w
+00005d70: 2064 6174 6120 6669 6c65 0a20 2020 2020   data file.     
+00005d80: 2020 2020 2020 2066 726f 6d20 736b 6c65         from skle
+00005d90: 6172 6e2e 6665 6174 7572 655f 6578 7472  arn.feature_extr
+00005da0: 6163 7469 6f6e 2e74 6578 7420 696d 706f  action.text impo
+00005db0: 7274 2054 6669 6466 5665 6374 6f72 697a  rt TfidfVectoriz
+00005dc0: 6572 0a20 2020 2020 2020 200a 2020 2020  er.        .    
+00005dd0: 2020 2020 2020 2020 7463 6c75 7374 6572          tcluster
+00005de0: 203d 2054 6578 7443 6c75 7374 6572 286f   = TextCluster(o
+00005df0: 7574 7075 745f 6469 723d 276d 6f64 656c  utput_dir='model
+00005e00: 732f 636c 7573 7465 7227 2c20 6665 6174  s/cluster', feat
+00005e10: 7572 653d 5466 6964 6656 6563 746f 7269  ure=TfidfVectori
+00005e20: 7a65 7228 6e67 7261 6d5f 7261 6e67 653d  zer(ngram_range=
+00005e30: 2831 2c20 3229 292c 206e 5f63 6c75 7374  (1, 2)), n_clust
+00005e40: 6572 733d 3130 290a 2020 2020 2020 2020  ers=10).        
+00005e50: 2020 2020 6461 7461 203d 2074 636c 7573      data = tclus
+00005e60: 7465 722e 6c6f 6164 5f66 696c 655f 6461  ter.load_file_da
+00005e70: 7461 2827 7468 7563 6e65 7773 5f74 7261  ta('thucnews_tra
+00005e80: 696e 5f31 772e 7478 7427 2c20 7365 703d  in_1w.txt', sep=
+00005e90: 275c 7427 2c20 7573 655f 636f 6c3d 3129  '\t', use_col=1)
+00005ea0: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
+00005eb0: 7475 7265 2c20 6c61 6265 6c73 203d 2074  ture, labels = t
+00005ec0: 636c 7573 7465 722e 7472 6169 6e28 6461  cluster.train(da
+00005ed0: 7461 5b3a 3530 3030 5d29 0a20 2020 2020  ta[:5000]).     
+00005ee0: 2020 2020 2020 2074 636c 7573 7465 722e         tcluster.
+00005ef0: 7368 6f77 5f63 6c75 7374 6572 7328 6665  show_clusters(fe
+00005f00: 6174 7572 652c 206c 6162 656c 732c 2027  ature, labels, '
+00005f10: 6d6f 6465 6c73 2f63 6c75 7374 6572 2f63  models/cluster/c
+00005f20: 6c75 7374 6572 5f74 7261 696e 5f73 6567  luster_train_seg
+00005f30: 5f73 616d 706c 6573 2e70 6e67 2729 0a20  _samples.png'). 
+00005f40: 2020 2020 2020 2020 2020 2072 203d 2074             r = t
+00005f50: 636c 7573 7465 722e 7072 6564 6963 7428  cluster.predict(
+00005f60: 6461 7461 5b3a 3330 5d29 0a20 2020 2020  data[:30]).     
+00005f70: 2020 2020 2020 2070 7269 6e74 2872 290a         print(r).
+00005f80: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+00005f90: 2020 2020 0a20 2020 2020 2020 206f 7574      .        out
+00005fa0: 7075 743a 0a20 2020 2020 2020 200a 2020  put:.        .  
+00005fb0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00005fc0: 2020 5465 7874 436c 7573 7465 7220 696e    TextCluster in
+00005fd0: 7374 616e 6365 2028 4d69 6e69 4261 7463  stance (MiniBatc
+00005fe0: 684b 4d65 616e 7328 6e5f 636c 7573 7465  hKMeans(n_cluste
+00005ff0: 7273 3d32 2c20 6e5f 696e 6974 3d31 3029  rs=2, n_init=10)
+00006000: 2c20 3c70 7974 6578 7463 6c61 7373 6966  , <pytextclassif
+00006010: 6965 722e 7574 696c 732e 746f 6b65 6e69  ier.utils.tokeni
+00006020: 7a65 722e 546f 6b65 6e69 7a65 7220 6f62  zer.Tokenizer ob
+00006030: 6a65 6374 2061 7420 3078 3766 3830 6264  ject at 0x7f80bd
+00006040: 3436 3832 6230 3e2c 2054 6669 6466 5665  4682b0>, TfidfVe
+00006050: 6374 6f72 697a 6572 286e 6772 616d 5f72  ctorizer(ngram_r
+00006060: 616e 6765 3d28 312c 2032 2929 290a 2020  ange=(1, 2))).  
+00006070: 2020 2020 2020 5b31 2031 2031 2031 2031        [1 1 1 1 1
+00006080: 2031 2031 2031 2031 2031 2031 2038 2031   1 1 1 1 1 1 8 1
+00006090: 2031 2031 2031 2031 2031 2031 2031 2031   1 1 1 1 1 1 1 1
+000060a0: 2031 2039 2031 2031 2038 2031 2031 2039   1 9 1 1 8 1 1 9
+000060b0: 2031 5d0a 2020 2020 2020 2020 6060 600a   1].        ```.
+000060c0: 2020 2020 2020 2020 636c 7573 7465 7269          clusteri
+000060d0: 6e67 2070 6c6f 7420 696d 6167 653a 0a20  ng plot image:. 
+000060e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000060f0: 215b 636c 7573 7465 725f 696d 6167 655d  ![cluster_image]
+00006100: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006110: 636f 6d2f 7368 6962 696e 6736 3234 2f70  com/shibing624/p
+00006120: 7974 6578 7463 6c61 7373 6966 6965 722f  ytextclassifier/
+00006130: 626c 6f62 2f6d 6173 7465 722f 646f 6373  blob/master/docs
+00006140: 2f63 6c75 7374 6572 5f74 7261 696e 5f73  /cluster_train_s
+00006150: 6567 5f73 616d 706c 6573 2e70 6e67 290a  eg_samples.png).
+00006160: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006170: 200a 2020 2020 2020 2020 2323 2043 6f6e   .        ## Con
+00006180: 7461 6374 0a20 2020 2020 2020 200a 2020  tact.        .  
+00006190: 2020 2020 2020 2d20 4973 7375 6528 e5bb        - Issue(..
+000061a0: bae8 aeae 29ef bc9a 5b21 5b47 6974 4875  ....)...[![GitHu
+000061b0: 6220 6973 7375 6573 5d28 6874 7470 733a  b issues](https:
+000061c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000061d0: 2f67 6974 6875 622f 6973 7375 6573 2f73  /github/issues/s
+000061e0: 6869 6269 6e67 3632 342f 7079 7465 7874  hibing624/pytext
+000061f0: 636c 6173 7369 6669 6572 2e73 7667 295d  classifier.svg)]
+00006200: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00006210: 636f 6d2f 7368 6962 696e 6736 3234 2f70  com/shibing624/p
+00006220: 7974 6578 7463 6c61 7373 6966 6965 722f  ytextclassifier/
+00006230: 6973 7375 6573 290a 2020 2020 2020 2020  issues).        
+00006240: 2d20 e982 aee4 bbb6 e688 91ef bc9a 7875  - ............xu
+00006250: 6d69 6e67 3a20 7875 6d69 6e67 3632 3440  ming: xuming624@
+00006260: 7171 2e63 6f6d 0a20 2020 2020 2020 202d  qq.com.        -
+00006270: 20e5 beae e4bf a1e6 8891 efbc 9ae5 8aa0   ...............
+00006280: e688 912a e5be aee4 bfa1 e58f b7ef bc9a  ...*............
+00006290: 7875 6d69 6e67 3632 342a 2c20 e8bf 9b50  xuming624*, ...P
+000062a0: 7974 686f 6e2d 4e4c 50e4 baa4 e6b5 81e7  ython-NLP.......
+000062b0: bea4 efbc 8ce5 a487 e6b3 a8ef bc9a 2ae5  ..............*.
+000062c0: a793 e590 8d2d e585 ace5 8fb8 e590 8d2d  .....-.........-
+000062d0: 4e4c 502a 0a20 2020 2020 2020 203c 696d  NLP*.        <im
+000062e0: 6720 7372 633d 2264 6f63 732f 7765 6368  g src="docs/wech
+000062f0: 6174 2e6a 7065 6722 2077 6964 7468 3d22  at.jpeg" width="
+00006300: 3230 3022 202f 3e0a 2020 2020 2020 2020  200" />.        
+00006310: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006320: 2020 2323 2043 6974 6174 696f 6e0a 2020    ## Citation.  
+00006330: 2020 2020 2020 0a20 2020 2020 2020 20e5        .        .
+00006340: a682 e69e 9ce4 bda0 e59c a8e7 a094 e7a9  ................
+00006350: b6e4 b8ad e4bd bfe7 94a8 e4ba 8670 7974  .............pyt
+00006360: 6578 7463 6c61 7373 6966 6965 72ef bc8c  extclassifier...
+00006370: e8af b7e6 8c89 e5a6 82e4 b88b e6a0 bce5  ................
+00006380: bc8f e5bc 95e7 94a8 efbc 9a0a 2020 2020  ............    
+00006390: 2020 2020 0a20 2020 2020 2020 2041 5041      .        APA
+000063a0: 3a0a 2020 2020 2020 2020 6060 606c 6174  :.        ```lat
+000063b0: 6578 0a20 2020 2020 2020 2058 752c 204d  ex.        Xu, M
+000063c0: 2e20 5079 7465 7874 636c 6173 7369 6669  . Pytextclassifi
+000063d0: 6572 3a20 5465 7874 2063 6c61 7373 6966  er: Text classif
+000063e0: 6965 7220 746f 6f6c 6b69 7420 666f 7220  ier toolkit for 
+000063f0: 4e4c 5020 2856 6572 7369 6f6e 2031 2e32  NLP (Version 1.2
+00006400: 2e30 2920 5b43 6f6d 7075 7465 7220 736f  .0) [Computer so
+00006410: 6674 7761 7265 5d2e 2068 7474 7073 3a2f  ftware]. https:/
+00006420: 2f67 6974 6875 622e 636f 6d2f 7368 6962  /github.com/shib
+00006430: 696e 6736 3234 2f70 7974 6578 7463 6c61  ing624/pytextcla
+00006440: 7373 6966 6965 720a 2020 2020 2020 2020  ssifier.        
+00006450: 6060 600a 2020 2020 2020 2020 0a20 2020  ```.        .   
+00006460: 2020 2020 2042 6962 5465 583a 0a20 2020       BibTeX:.   
+00006470: 2020 2020 2060 6060 6c61 7465 780a 2020       ```latex.  
+00006480: 2020 2020 2020 406d 6973 637b 5079 7465        @misc{Pyte
+00006490: 7874 636c 6173 7369 6669 6572 2c0a 2020  xtclassifier,.  
+000064a0: 2020 2020 2020 2020 7469 746c 653d 7b50          title={P
+000064b0: 7974 6578 7463 6c61 7373 6966 6965 723a  ytextclassifier:
+000064c0: 2054 6578 7420 636c 6173 7369 6669 6572   Text classifier
+000064d0: 2074 6f6f 6c6b 6974 2066 6f72 204e 4c50   toolkit for NLP
+000064e0: 7d2c 0a20 2020 2020 2020 2020 2061 7574  },.          aut
+000064f0: 686f 723d 7b58 7520 4d69 6e67 7d2c 0a20  hor={Xu Ming},. 
+00006500: 2020 2020 2020 2020 2079 6561 723d 7b32           year={2
+00006510: 3032 327d 2c0a 2020 2020 2020 2020 2020  022},.          
+00006520: 686f 7770 7562 6c69 7368 6564 3d7b 5c75  howpublished={\u
+00006530: 726c 7b68 7474 7073 3a2f 2f67 6974 6875  rl{https://githu
+00006540: 622e 636f 6d2f 7368 6962 696e 6736 3234  b.com/shibing624
+00006550: 2f70 7974 6578 7463 6c61 7373 6966 6965  /pytextclassifie
+00006560: 727d 7d2c 0a20 2020 2020 2020 207d 0a20  r}},.        }. 
+00006570: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00006580: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+00006590: 2020 2020 2023 2320 4c69 6365 6e73 650a       ## License.
+000065a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000065b0: 200a 2020 2020 2020 2020 e68e 88e6 9d83   .        ......
+000065c0: e58d 8fe8 aeae e4b8 ba20 5b54 6865 2041  ......... [The A
+000065d0: 7061 6368 6520 4c69 6365 6e73 6520 322e  pache License 2.
+000065e0: 305d 284c 4943 454e 5345 29ef bc8c e58f  0](LICENSE).....
+000065f0: afe5 858d e8b4 b9e7 94a8 e581 9ae5 9586  ................
+00006600: e4b8 9ae7 94a8 e980 94e3 8082 e8af b7e5  ................
+00006610: 9ca8 e4ba a7e5 9381 e8af b4e6 988e e4b8  ................
+00006620: ade9 9984 e58a a02a 2a70 7974 6578 7463  .......**pytextc
+00006630: 6c61 7373 6966 6965 722a 2ae7 9a84 e993  lassifier**.....
+00006640: bee6 8ea5 e592 8ce6 8e88 e69d 83e5 8d8f  ................
+00006650: e8ae aee3 8082 0a20 2020 2020 2020 200a  .......        .
+00006660: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006670: 2023 2320 436f 6e74 7269 6275 7465 0a20   ## Contribute. 
+00006680: 2020 2020 2020 20e9 a1b9 e79b aee4 bba3         .........
+00006690: e7a0 81e8 bf98 e5be 88e7 b297 e7b3 99ef  ................
+000066a0: bc8c e5a6 82e6 9e9c e5a4 a7e5 aeb6 e5af  ................
+000066b0: b9e4 bba3 e7a0 81e6 9c89 e689 80e6 94b9  ................
+000066c0: e8bf 9bef bc8c e6ac a2e8 bf8e e68f 90e4  ................
+000066d0: baa4 e59b 9ee6 9cac e9a1 b9e7 9bae efbc  ................
+000066e0: 8ce5 9ca8 e68f 90e4 baa4 e4b9 8be5 898d  ................
+000066f0: efbc 8ce6 b3a8 e684 8fe4 bba5 e4b8 8be4  ................
+00006700: b8a4 e782 b9ef bc9a 0a20 2020 2020 2020  .........       
+00006710: 200a 2020 2020 2020 2020 202d 20e5 9ca8   .         - ...
+00006720: 6074 6573 7473 60e6 b7bb e58a a0e7 9bb8  `tests`.........
+00006730: e5ba 94e7 9a84 e58d 95e5 8583 e6b5 8be8  ................
+00006740: af95 0a20 2020 2020 2020 2020 2d20 e4bd  ...         - ..
+00006750: bfe7 94a8 6070 7974 686f 6e20 7365 7475  ....`python setu
+00006760: 702e 7079 2074 6573 7460 e69d a5e8 bf90  p.py test`......
+00006770: e8a1 8ce6 8980 e69c 89e5 8d95 e585 83e6  ................
+00006780: b58b e8af 95ef bc8c e7a1 aee4 bf9d e689  ................
+00006790: 80e6 9c89 e58d 95e6 b58b e983 bde6 98af  ................
+000067a0: e980 9ae8 bf87 e79a 840a 2020 2020 2020  ..........      
+000067b0: 2020 0a20 2020 2020 2020 20e4 b98b e590    .        .....
+000067c0: 8ee5 8db3 e58f afe6 8f90 e4ba a450 52e3  .............PR.
+000067d0: 8082 0a20 2020 2020 2020 200a 2020 2020  ...        .    
+000067e0: 2020 2020 0a4b 6579 776f 7264 733a 2070      .Keywords: p
+000067f0: 7974 6578 7463 6c61 7373 6966 6965 722c  ytextclassifier,
+00006800: 7465 7874 636c 6173 7369 6669 6572 2c63  textclassifier,c
+00006810: 6c61 7373 6966 6965 722c 7465 7874 636c  lassifier,textcl
+00006820: 6173 7369 6669 6361 7469 6f6e 0a50 6c61  assification.Pla
+00006830: 7466 6f72 6d3a 2055 4e4b 4e4f 574e 0a43  tform: UNKNOWN.C
+00006840: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00006850: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00006860: 5363 6965 6e63 652f 5265 7365 6172 6368  Science/Research
+00006870: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00006880: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00006890: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+000068a0: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
+000068b0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000068c0: 7665 6420 3a3a 2041 7061 6368 6520 536f  ved :: Apache So
+000068d0: 6674 7761 7265 204c 6963 656e 7365 0a43  ftware License.C
+000068e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000068f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00006900: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
+00006910: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00006920: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00006930: 7468 6f6e 203a 3a20 322e 370a 436c 6173  thon :: 2.7.Clas
+00006940: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00006950: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00006960: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
+00006970: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00006980: 2054 6578 7420 5072 6f63 6573 7369 6e67   Text Processing
+00006990: 203a 3a20 4c69 6e67 7569 7374 6963 0a43   :: Linguistic.C
+000069a0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
+000069b0: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
+000069c0: 6e67 696e 6565 7269 6e67 203a 3a20 4172  ngineering :: Ar
+000069d0: 7469 6669 6369 616c 2049 6e74 656c 6c69  tificial Intelli
+000069e0: 6765 6e63 650a 4465 7363 7269 7074 696f  gence.Descriptio
+000069f0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00006a00: 7465 7874 2f6d 6172 6b64 6f77 6e0a       text/markdown.
```

### Comparing `pytextclassifier-1.3.5/pytextclassifier.egg-info/SOURCES.txt` & `pytextclassifier-1.3.6/pytextclassifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytextclassifier-1.3.5/setup.py` & `pytextclassifier-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 from setuptools import setup, find_packages
 
-__version__ = '1.3.5'
+__version__ = '1.3.6'
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='pytextclassifier',
     version=__version__,
```

