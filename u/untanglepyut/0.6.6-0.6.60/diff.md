# Comparing `tmp/untanglepyut-0.6.6.tar.gz` & `tmp/untanglepyut-0.6.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "untanglepyut-0.6.6.tar", last modified: Thu Jan 26 21:36:58 2023, max compression
+gzip compressed data, was "untanglepyut-0.6.60.tar", last modified: Wed May 10 17:25:46 2023, max compression
```

## Comparing `untanglepyut-0.6.6.tar` & `untanglepyut-0.6.60.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-26 21:36:58.929210 untanglepyut-0.6.6/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-0.6.6/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2844 2023-01-26 21:36:58.929078 untanglepyut-0.6.6/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2593 2023-01-12 22:24:26.000000 untanglepyut-0.6.6/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-01-26 21:36:58.929246 untanglepyut-0.6.6/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      685 2023-01-26 21:15:26.000000 untanglepyut-0.6.6/setup.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-26 21:36:58.928199 untanglepyut-0.6.6/untanglepyut/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      886 2023-01-03 16:20:29.000000 untanglepyut-0.6.6/untanglepyut/BaseUnTangle.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1774 2022-08-29 19:49:16.000000 untanglepyut-0.6.6/untanglepyut/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2022-10-13 01:16:21.000000 untanglepyut-0.6.6/untanglepyut/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15593 2022-11-15 02:56:29.000000 untanglepyut-0.6.6/untanglepyut/UnTangleOglLinks.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13941 2023-01-26 21:34:58.000000 untanglepyut-0.6.6/untanglepyut/UnTanglePyut.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4154 2022-08-23 19:21:04.000000 untanglepyut-0.6.6/untanglepyut/UnTangleUseCaseDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    12818 2023-01-02 13:59:28.000000 untanglepyut-0.6.6/untanglepyut/UnTangler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3958 2022-10-14 00:36:17.000000 untanglepyut-0.6.6/untanglepyut/UntangleSequenceDiagram.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2022-06-24 19:59:25.000000 untanglepyut-0.6.6/untanglepyut/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-25 14:46:48.000000 untanglepyut-0.6.6/untanglepyut/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-01-26 21:36:58.928913 untanglepyut-0.6.6/untanglepyut.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2844 2023-01-26 21:36:58.000000 untanglepyut-0.6.6/untanglepyut.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      493 2023-01-26 21:36:58.000000 untanglepyut-0.6.6/untanglepyut.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-01-26 21:36:58.000000 untanglepyut-0.6.6/untanglepyut.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       29 2023-01-26 21:36:58.000000 untanglepyut-0.6.6/untanglepyut.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-01-26 21:36:58.000000 untanglepyut-0.6.6/untanglepyut.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-10 17:25:46.215013 untanglepyut-0.6.60/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-08-15 19:41:01.000000 untanglepyut-0.6.60/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3478 2023-05-10 17:25:46.214886 untanglepyut-0.6.60/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3226 2023-04-13 20:32:39.000000 untanglepyut-0.6.60/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-10 17:25:46.215051 untanglepyut-0.6.60/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      750 2023-05-10 15:26:37.000000 untanglepyut-0.6.60/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-10 17:25:46.214165 untanglepyut-0.6.60/untanglepyut/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      886 2023-01-03 16:20:29.000000 untanglepyut-0.6.60/untanglepyut/BaseUnTangle.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1774 2022-08-29 19:49:16.000000 untanglepyut-0.6.60/untanglepyut/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1078 2022-10-13 01:16:21.000000 untanglepyut-0.6.60/untanglepyut/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    15843 2023-03-19 16:02:08.000000 untanglepyut-0.6.60/untanglepyut/UnTangleOglLinks.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14445 2023-05-08 16:55:26.000000 untanglepyut-0.6.60/untanglepyut/UnTanglePyut.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4154 2022-08-23 19:21:04.000000 untanglepyut-0.6.60/untanglepyut/UnTangleUseCaseDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    13009 2023-05-10 17:16:32.000000 untanglepyut-0.6.60/untanglepyut/UnTangler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3918 2023-01-31 19:27:38.000000 untanglepyut-0.6.60/untanglepyut/UntangleSequenceDiagram.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2022-06-24 19:59:25.000000 untanglepyut-0.6.60/untanglepyut/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-06-25 14:46:48.000000 untanglepyut-0.6.60/untanglepyut/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-10 17:25:46.214727 untanglepyut-0.6.60/untanglepyut.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3478 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      493 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       84 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-05-10 17:25:46.000000 untanglepyut-0.6.60/untanglepyut.egg-info/top_level.txt
```

### Comparing `untanglepyut-0.6.6/LICENSE` & `untanglepyut-0.6.60/LICENSE`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.6/PKG-INFO` & `untanglepyut-0.6.60/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,178 +1,202 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 756e 7461  : 2.1.Name: unta
-00000020: 6e67 6c65 7079 7574 0a56 6572 7369 6f6e  nglepyut.Version
-00000030: 3a20 302e 362e 360a 5375 6d6d 6172 793a  : 0.6.6.Summary:
-00000040: 2058 4d4c 2074 6f20 4f67 6c20 4f62 6a65   XML to Ogl Obje
-00000050: 6374 204d 6f64 656c 0a48 6f6d 652d 7061  ct Model.Home-pa
-00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000070: 7562 2e63 6f6d 2f68 6173 6969 3230 3131  ub.com/hasii2011
-00000080: 2f75 6e74 616e 676c 6570 7975 740a 4175  /untanglepyut.Au
-00000090: 7468 6f72 2d65 6d61 696c 3a20 4875 6d62  thor-email: Humb
-000000a0: 6572 746f 2e41 2e53 616e 6368 657a 2e49  erto.A.Sanchez.I
-000000b0: 4940 676d 6169 6c2e 636f 6d0a 4465 7363  I@gmail.com.Desc
-000000c0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-000000d0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-000000e0: 6f77 6e0a 4c69 6365 6e73 652d 4669 6c65  own.License-File
-000000f0: 3a20 4c49 4345 4e53 450a 0a3c 696d 6720  : LICENSE..<img 
-00000100: 7372 633d 222e 2f64 6f63 732f 6167 706c  src="./docs/agpl
-00000110: 2d6c 6963 656e 7365 2d77 6562 2d62 6164  -license-web-bad
-00000120: 6765 2d76 6572 7369 6f6e 2d32 2d32 3536  ge-version-2-256
-00000130: 7834 382e 706e 6722 2f3e 0a0a 5b21 5b4d  x48.png"/>..[![M
-00000140: 6169 6e74 656e 616e 6365 5d28 6874 7470  aintenance](http
-00000150: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000160: 696f 2f62 6164 6765 2f4d 6169 6e74 6169  io/badge/Maintai
-00000170: 6e65 6425 3346 2d79 6573 2d67 7265 656e  ned%3F-yes-green
-00000180: 2e73 7667 295d 2868 7474 7073 3a2f 2f47  .svg)](https://G
-00000190: 6974 4875 622e 636f 6d2f 4e61 6572 6565  itHub.com/Naeree
-000001a0: 6e2f 5374 7261 7044 6f77 6e2e 6a73 2f67  n/StrapDown.js/g
-000001b0: 7261 7068 732f 636f 6d6d 6974 2d61 6374  raphs/commit-act
-000001c0: 6976 6974 7929 0a5b 215b 4369 7263 6c65  ivity).[![Circle
-000001d0: 4349 5d28 6874 7470 733a 2f2f 646c 2e63  CI](https://dl.c
-000001e0: 6972 636c 6563 692e 636f 6d2f 7374 6174  ircleci.com/stat
-000001f0: 7573 2d62 6164 6765 2f69 6d67 2f67 682f  us-badge/img/gh/
-00000200: 6861 7369 6932 3031 312f 756e 7461 6e67  hasii2011/untang
-00000210: 6c65 7079 7574 2f74 7265 652f 6d61 7374  lepyut/tree/mast
-00000220: 6572 2e73 7667 3f73 7479 6c65 3d73 6869  er.svg?style=shi
-00000230: 656c 6429 5d28 6874 7470 733a 2f2f 646c  eld)](https://dl
-00000240: 2e63 6972 636c 6563 692e 636f 6d2f 7374  .circleci.com/st
-00000250: 6174 7573 2d62 6164 6765 2f72 6564 6972  atus-badge/redir
-00000260: 6563 742f 6768 2f68 6173 6969 3230 3131  ect/gh/hasii2011
-00000270: 2f75 6e74 616e 676c 6570 7975 742f 7472  /untanglepyut/tr
-00000280: 6565 2f6d 6173 7465 7229 0a5b 215b 6d61  ee/master).[![ma
-00000290: 634f 535d 2868 7474 7073 3a2f 2f73 7667  cOS](https://svg
-000002a0: 7368 6172 652e 636f 6d2f 692f 5a6a 502e  share.com/i/ZjP.
-000002b0: 7376 6729 5d28 6874 7470 733a 2f2f 7376  svg)](https://sv
-000002c0: 6773 6861 7265 2e63 6f6d 2f69 2f5a 6a50  gshare.com/i/ZjP
-000002d0: 2e73 7667 290a 0a5b 215b 666f 7274 6865  .svg)..[![forthe
-000002e0: 6261 6467 6520 6d61 6465 2d77 6974 682d  badge made-with-
-000002f0: 7079 7468 6f6e 5d28 6874 7470 3a2f 2f46  python](http://F
-00000300: 6f72 5468 6542 6164 6765 2e63 6f6d 2f69  orTheBadge.com/i
-00000310: 6d61 6765 732f 6261 6467 6573 2f6d 6164  mages/badges/mad
-00000320: 652d 7769 7468 2d70 7974 686f 6e2e 7376  e-with-python.sv
-00000330: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
-00000340: 7079 7468 6f6e 2e6f 7267 2f29 0a0a 5468  python.org/)..Th
-00000350: 6973 2070 726f 6a65 6374 2069 7320 696e  is project is in
-00000360: 7465 6e64 6564 2074 6f20 6265 2075 7365  tended to be use
-00000370: 6420 6279 205b 5079 7574 2050 6c75 6769  d by [Pyut Plugi
-00000380: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
-00000390: 622e 636f 6d2f 6861 7369 6932 3031 312f  b.com/hasii2011/
-000003a0: 7079 7574 706c 7567 696e 636f 7265 2920  pyutplugincore) 
-000003b0: 6465 7665 6c6f 7065 7273 2074 6f20 636f  developers to co
-000003c0: 6e76 6572 7420 5b50 7975 745d 2868 7474  nvert [Pyut](htt
-000003d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000003e0: 6861 7369 6932 3031 312f 5079 5574 2920  hasii2011/PyUt) 
-000003f0: 584d 4c20 6669 6c65 7320 746f 2074 6865  XML files to the
-00000400: 205b 4f67 6c20 4d6f 6465 6c5d 2868 7474   [Ogl Model](htt
-00000410: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000420: 6861 7369 6932 3031 312f 6f67 6c29 2063  hasii2011/ogl) c
-00000430: 6c61 7373 6573 2e20 2054 6865 7365 206d  lasses.  These m
-00000440: 6f64 656c 2063 6c61 7373 6573 2063 616e  odel classes can
-00000450: 2074 6865 6e20 6265 2075 7365 6420 6279   then be used by
-00000460: 2074 6865 2050 7975 7420 5549 2074 6f20   the Pyut UI to 
-00000470: 6469 7370 6c61 7920 6173 2055 4d4c 2044  display as UML D
-00000480: 6961 6772 616d 732e 0a0a 2d2d 2d2d 2d2d  iagrams...------
-00000490: 0a0a 5573 6520 6173 2066 6f6c 6c6f 7773  ..Use as follows
-000004a0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-000004b0: 6d20 756e 7461 6e67 6c65 7079 7574 2e55  m untanglepyut.U
-000004c0: 6e54 616e 676c 6572 2069 6d70 6f72 7420  nTangler import 
-000004d0: 446f 6375 6d65 6e74 0a66 726f 6d20 756e  Document.from un
-000004e0: 7461 6e67 6c65 7079 7574 2e55 6e54 616e  tanglepyut.UnTan
-000004f0: 676c 6572 2069 6d70 6f72 7420 556e 5461  gler import UnTa
-00000500: 6e67 6c65 720a 0a66 726f 6d20 756e 7461  ngler..from unta
-00000510: 6e67 6c65 7079 7574 2e54 7970 6573 2069  nglepyut.Types i
-00000520: 6d70 6f72 7420 556e 7461 6e67 6c65 644f  mport UntangledO
-00000530: 676c 436c 6173 7365 730a 6672 6f6d 2075  glClasses.from u
-00000540: 6e74 616e 676c 6570 7975 742e 5479 7065  ntanglepyut.Type
-00000550: 7320 696d 706f 7274 2055 6e74 616e 676c  s import Untangl
-00000560: 6564 4f67 6c4c 696e 6b73 0a66 726f 6d20  edOglLinks.from 
-00000570: 756e 7461 6e67 6c65 7079 7574 2e54 7970  untanglepyut.Typ
-00000580: 6573 2069 6d70 6f72 7420 556e 7461 6e67  es import Untang
-00000590: 6c65 644f 676c 4e6f 7465 730a 6672 6f6d  ledOglNotes.from
-000005a0: 2075 6e74 616e 676c 6570 7975 742e 5479   untanglepyut.Ty
-000005b0: 7065 7320 696d 706f 7274 2055 6e74 616e  pes import Untan
-000005c0: 676c 6564 4f67 6c54 6578 7473 0a0a 756e  gledOglTexts..un
-000005d0: 7461 6e67 6c65 723a 2055 6e54 616e 676c  tangler: UnTangl
-000005e0: 6572 203d 2055 6e54 616e 676c 6572 2866  er = UnTangler(f
-000005f0: 7146 696c 654e 616d 653d 274d 756c 7469  qFileName='Multi
-00000600: 446f 6375 6d65 6e74 5072 6f6a 6563 742e  DocumentProject.
-00000610: 786d 6c27 290a 0a64 6f63 756d 656e 743a  xml')..document:
-00000620: 2044 6f63 756d 656e 7420 3d20 756e 7461   Document = unta
-00000630: 6e67 6c65 722e 646f 6375 6d65 6e74 735b  ngler.documents[
-00000640: 2744 6961 6772 616d 2d31 275d 0a0a 6f67  'Diagram-1']..og
-00000650: 6c43 6c61 7373 6573 3a20 556e 7461 6e67  lClasses: Untang
-00000660: 6c65 644f 676c 436c 6173 7365 7320 3d20  ledOglClasses = 
-00000670: 646f 6375 6d65 6e74 2e6f 676c 436c 6173  document.oglClas
-00000680: 7365 730a 6f67 6c4c 696e 6b73 3a20 2020  ses.oglLinks:   
-00000690: 556e 7461 6e67 6c65 644f 676c 4c69 6e6b  UntangledOglLink
-000006a0: 7320 2020 3d20 646f 6375 6d65 6e74 2e6f  s   = document.o
-000006b0: 676c 4c69 6e6b 730a 6f67 6c4e 6f74 6573  glLinks.oglNotes
-000006c0: 3a20 2020 556e 7461 6e67 6c65 644f 676c  :   UntangledOgl
-000006d0: 4e6f 7465 7320 2020 3d20 646f 6375 6d65  Notes   = docume
-000006e0: 6e74 2e6f 676c 4e6f 7465 730a 6f67 6c54  nt.oglNotes.oglT
-000006f0: 6578 7473 3a20 2020 556e 7461 6e67 6c65  exts:   Untangle
-00000700: 644f 676c 5465 7874 7320 2020 3d20 646f  dOglTexts   = do
-00000710: 6375 6d65 6e74 2e6f 676c 5465 7874 730a  cument.oglTexts.
-00000720: 0a60 6060 0a0a 0a0a 5468 6520 666f 6c6c  .```....The foll
-00000730: 6f77 696e 6720 6973 2074 6865 2055 4d4c  owing is the UML
-00000740: 2064 6961 6772 616d 2066 6f72 2074 6865   diagram for the
-00000750: 2050 7975 7420 556e 7461 6e67 6c65 720a   Pyut Untangler.
-00000760: 0a21 5b55 6e74 616e 676c 6550 7975 745d  .![UntanglePyut]
-00000770: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000780: 636f 6d2f 6861 7369 6932 3031 312f 756e  com/hasii2011/un
-00000790: 7461 6e67 6c65 7079 7574 2f62 6c6f 622f  tanglepyut/blob/
-000007a0: 6d61 7374 6572 2f64 6f63 732f 556e 7461  master/docs/Unta
-000007b0: 6e67 6c65 5079 7574 2e70 6e67 290a 0a0a  nglePyut.png)...
-000007c0: 0a2d 2d2d 2d2d 2d0a 0a0a 215b 4875 6d62  .------...![Humb
-000007d0: 6572 746f 2773 204d 6f64 6966 6965 6420  erto's Modified 
-000007e0: 4c6f 676f 5d28 6874 7470 733a 2f2f 7261  Logo](https://ra
-000007f0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000800: 656e 742e 636f 6d2f 7769 6b69 2f68 6173  ent.com/wiki/has
-00000810: 6969 3230 3131 2f67 6974 746f 646f 6973  ii2011/gittodois
-00000820: 7463 6c6f 6e65 2f69 6d61 6765 732f 5369  tclone/images/Si
-00000830: 6c6c 7947 6974 4875 622e 706e 6729 0a0a  llyGitHub.png)..
-00000840: 4920 616d 2063 6f6e 6365 726e 6564 2061  I am concerned a
-00000850: 626f 7574 2047 6974 4875 6227 7320 436f  bout GitHub's Co
-00000860: 7069 6c6f 7420 7072 6f6a 6563 740a 0a0a  pilot project...
-00000870: 0a49 2075 7267 6520 796f 7520 746f 2072  .I urge you to r
-00000880: 6561 6420 6162 6f75 7420 7468 650a 5b47  ead about the.[G
-00000890: 6976 6520 7570 2047 6974 4875 625d 2868  ive up GitHub](h
-000008a0: 7474 7073 3a2f 2f47 6976 6555 7047 6974  ttps://GiveUpGit
-000008b0: 4875 622e 6f72 6729 2063 616d 7061 6967  Hub.org) campaig
-000008c0: 6e20 6672 6f6d 0a5b 7468 6520 536f 6674  n from.[the Soft
-000008d0: 7761 7265 2046 7265 6564 6f6d 2043 6f6e  ware Freedom Con
-000008e0: 7365 7276 616e 6379 5d28 6874 7470 733a  servancy](https:
-000008f0: 2f2f 7366 636f 6e73 6572 7661 6e63 792e  //sfconservancy.
-00000900: 6f72 6729 2e0a 0a57 6869 6c65 2049 2064  org)...While I d
-00000910: 6f20 6e6f 7420 6164 766f 6361 7465 2066  o not advocate f
-00000920: 6f72 2061 6c6c 2074 6865 2069 7373 7565  or all the issue
-00000930: 7320 6c69 7374 6564 2074 6865 7265 2049  s listed there I
-00000940: 2064 6f20 6e6f 7420 6c69 6b65 2074 6861   do not like tha
-00000950: 740a 6120 636f 6d70 616e 7920 6c69 6b65  t.a company like
-00000960: 204d 6963 726f 736f 6674 206d 6179 2070   Microsoft may p
-00000970: 726f 6669 7420 6672 6f6d 206f 7065 6e20  rofit from open 
-00000980: 736f 7572 6365 2070 726f 6a65 6374 732e  source projects.
-00000990: 0a0a 4920 636f 6e74 696e 7565 2074 6f20  ..I continue to 
-000009a0: 7573 6520 4769 7448 7562 2062 6563 6175  use GitHub becau
-000009b0: 7365 2069 7420 6f66 6665 7273 2074 6865  se it offers the
-000009c0: 2073 6572 7669 6365 7320 4920 6e65 6564   services I need
-000009d0: 2066 6f72 2066 7265 652e 2020 4275 742c   for free.  But,
-000009e0: 2049 2063 6f6e 7469 6e75 650a 746f 206d   I continue.to m
-000009f0: 6f6e 6974 6f72 2074 6865 6972 2074 6572  onitor their ter
-00000a00: 6d73 206f 6620 7365 7276 6963 652e 0a0a  ms of service...
-00000a10: 416e 7920 7573 6520 6f66 2074 6869 7320  Any use of this 
-00000a20: 7072 6f6a 6563 7427 7320 636f 6465 2062  project's code b
-00000a30: 7920 4769 7448 7562 2043 6f70 696c 6f74  y GitHub Copilot
-00000a40: 2c20 7061 7374 206f 7220 7072 6573 656e  , past or presen
-00000a50: 742c 2069 7320 646f 6e65 0a77 6974 686f  t, is done.witho
-00000a60: 7574 206d 7920 7065 726d 6973 7369 6f6e  ut my permission
-00000a70: 2e20 2049 2064 6f20 6e6f 7420 636f 6e73  .  I do not cons
-00000a80: 656e 7420 746f 2047 6974 4875 6227 7320  ent to GitHub's 
-00000a90: 7573 6520 6f66 2074 6869 7320 7072 6f6a  use of this proj
-00000aa0: 6563 7427 730a 636f 6465 2069 6e20 436f  ect's.code in Co
-00000ab0: 7069 6c6f 742e 0a0a 4120 7265 706f 7369  pilot...A reposi
-00000ac0: 746f 7279 206f 776e 6572 206d 6179 206f  tory owner may o
-00000ad0: 7074 206f 7574 206f 6620 436f 7069 6c6f  pt out of Copilo
-00000ae0: 7420 6279 2063 6861 6e67 696e 6720 5365  t by changing Se
-00000af0: 7474 696e 6773 202d 2d3e 2047 6974 4875  ttings --> GitHu
-00000b00: 6220 436f 7069 6c6f 742e 0a0a 4920 6861  b Copilot...I ha
-00000b10: 7665 2064 6f6e 6520 736f 2e0a            ve done so..
+00000000: 3c69 6d67 2073 7263 3d22 2e2f 646f 6373  <img src="./docs
+00000010: 2f61 6770 6c2d 6c69 6365 6e73 652d 7765  /agpl-license-we
+00000020: 622d 6261 6467 652d 7665 7273 696f 6e2d  b-badge-version-
+00000030: 322d 3235 3678 3438 2e70 6e67 222f 3e0a  2-256x48.png"/>.
+00000040: 0a5b 215b 4369 7263 6c65 4349 5d28 6874  .[![CircleCI](ht
+00000050: 7470 733a 2f2f 646c 2e63 6972 636c 6563  tps://dl.circlec
+00000060: 692e 636f 6d2f 696e 7369 6768 7473 2d73  i.com/insights-s
+00000070: 6e61 7073 686f 742f 6768 2f68 6173 6969  napshot/gh/hasii
+00000080: 3230 3131 2f75 6e74 616e 676c 6570 7975  2011/untanglepyu
+00000090: 742f 6d61 7374 6572 2f6d 6169 6e2f 6261  t/master/main/ba
+000000a0: 6467 652e 7376 673f 7769 6e64 6f77 3d33  dge.svg?window=3
+000000b0: 3064 295d 2868 7474 7073 3a2f 2f61 7070  0d)](https://app
+000000c0: 2e63 6972 636c 6563 692e 636f 6d2f 696e  .circleci.com/in
+000000d0: 7369 6768 7473 2f67 6974 6875 622f 6861  sights/github/ha
+000000e0: 7369 6932 3031 312f 756e 7461 6e67 6c65  sii2011/untangle
+000000f0: 7079 7574 2f77 6f72 6b66 6c6f 7773 2f6d  pyut/workflows/m
+00000100: 6169 6e2f 6f76 6572 7669 6577 3f62 7261  ain/overview?bra
+00000110: 6e63 683d 6d61 7374 6572 2672 6570 6f72  nch=master&repor
+00000120: 7469 6e67 2d77 696e 646f 773d 6c61 7374  ting-window=last
+00000130: 2d33 302d 6461 7973 2669 6e73 6967 6874  -30-days&insight
+00000140: 732d 736e 6170 7368 6f74 3d74 7275 6529  s-snapshot=true)
+00000150: 0a0a 5b21 5b43 6972 636c 6543 495d 2868  ..[![CircleCI](h
+00000160: 7474 7073 3a2f 2f64 6c2e 6369 7263 6c65  ttps://dl.circle
+00000170: 6369 2e63 6f6d 2f73 7461 7475 732d 6261  ci.com/status-ba
+00000180: 6467 652f 696d 672f 6768 2f68 6173 6969  dge/img/gh/hasii
+00000190: 3230 3131 2f75 6e74 616e 676c 6570 7975  2011/untanglepyu
+000001a0: 742f 7472 6565 2f6d 6173 7465 722e 7376  t/tree/master.sv
+000001b0: 673f 7374 796c 653d 7368 6965 6c64 295d  g?style=shield)]
+000001c0: 2868 7474 7073 3a2f 2f64 6c2e 6369 7263  (https://dl.circ
+000001d0: 6c65 6369 2e63 6f6d 2f73 7461 7475 732d  leci.com/status-
+000001e0: 6261 6467 652f 7265 6469 7265 6374 2f67  badge/redirect/g
+000001f0: 682f 6861 7369 6932 3031 312f 756e 7461  h/hasii2011/unta
+00000200: 6e67 6c65 7079 7574 2f74 7265 652f 6d61  nglepyut/tree/ma
+00000210: 7374 6572 290a 5b21 5b4d 6169 6e74 656e  ster).[![Mainten
+00000220: 616e 6365 5d28 6874 7470 733a 2f2f 696d  ance](https://im
+00000230: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00000240: 6765 2f4d 6169 6e74 6169 6e65 6425 3346  ge/Maintained%3F
+00000250: 2d79 6573 2d67 7265 656e 2e73 7667 295d  -yes-green.svg)]
+00000260: 2868 7474 7073 3a2f 2f47 6974 4875 622e  (https://GitHub.
+00000270: 636f 6d2f 4e61 6572 6565 6e2f 5374 7261  com/Naereen/Stra
+00000280: 7044 6f77 6e2e 6a73 2f67 7261 7068 732f  pDown.js/graphs/
+00000290: 636f 6d6d 6974 2d61 6374 6976 6974 7929  commit-activity)
+000002a0: 0a5b 215b 6d61 634f 535d 2868 7474 7073  .[![macOS](https
+000002b0: 3a2f 2f73 7667 7368 6172 652e 636f 6d2f  ://svgshare.com/
+000002c0: 692f 5a6a 502e 7376 6729 5d28 6874 7470  i/ZjP.svg)](http
+000002d0: 733a 2f2f 7376 6773 6861 7265 2e63 6f6d  s://svgshare.com
+000002e0: 2f69 2f5a 6a50 2e73 7667 290a 0a5b 215b  /i/ZjP.svg)..[![
+000002f0: 666f 7274 6865 6261 6467 6520 6d61 6465  forthebadge made
+00000300: 2d77 6974 682d 7079 7468 6f6e 5d28 6874  -with-python](ht
+00000310: 7470 3a2f 2f46 6f72 5468 6542 6164 6765  tp://ForTheBadge
+00000320: 2e63 6f6d 2f69 6d61 6765 732f 6261 6467  .com/images/badg
+00000330: 6573 2f6d 6164 652d 7769 7468 2d70 7974  es/made-with-pyt
+00000340: 686f 6e2e 7376 6729 5d28 6874 7470 733a  hon.svg)](https:
+00000350: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+00000360: 2f29 0a0a 5468 6973 2070 726f 6a65 6374  /)..This project
+00000370: 2069 7320 696e 7465 6e64 6564 2074 6f20   is intended to 
+00000380: 6265 2075 7365 6420 6279 205b 5079 7574  be used by [Pyut
+00000390: 2050 6c75 6769 6e5d 2868 7474 7073 3a2f   Plugin](https:/
+000003a0: 2f67 6974 6875 622e 636f 6d2f 6861 7369  /github.com/hasi
+000003b0: 6932 3031 312f 7079 7574 706c 7567 696e  i2011/pyutplugin
+000003c0: 636f 7265 2920 6465 7665 6c6f 7065 7273  core) developers
+000003d0: 2074 6f20 636f 6e76 6572 7420 5b50 7975   to convert [Pyu
+000003e0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+000003f0: 622e 636f 6d2f 6861 7369 6932 3031 312f  b.com/hasii2011/
+00000400: 5079 5574 2920 584d 4c20 6669 6c65 7320  PyUt) XML files 
+00000410: 746f 2074 6865 205b 4f67 6c20 4d6f 6465  to the [Ogl Mode
+00000420: 6c5d 2868 7474 7073 3a2f 2f67 6974 6875  l](https://githu
+00000430: 622e 636f 6d2f 6861 7369 6932 3031 312f  b.com/hasii2011/
+00000440: 6f67 6c29 2063 6c61 7373 6573 2e20 2054  ogl) classes.  T
+00000450: 6865 7365 206d 6f64 656c 2063 6c61 7373  hese model class
+00000460: 6573 2063 616e 2074 6865 6e20 6265 2075  es can then be u
+00000470: 7365 6420 6279 2074 6865 2050 7975 7420  sed by the Pyut 
+00000480: 5549 2074 6f20 6469 7370 6c61 7920 6173  UI to display as
+00000490: 2055 4d4c 2044 6961 6772 616d 732e 0a0a   UML Diagrams...
+000004a0: 2d2d 2d2d 2d2d 0a0a 5573 6520 6173 2066  ------..Use as f
+000004b0: 6f6c 6c6f 7773 3a0a 0a60 6060 7079 7468  ollows:..```pyth
+000004c0: 6f6e 0a66 726f 6d20 756e 7461 6e67 6c65  on.from untangle
+000004d0: 7079 7574 2e55 6e54 616e 676c 6572 2069  pyut.UnTangler i
+000004e0: 6d70 6f72 7420 446f 6375 6d65 6e74 0a66  mport Document.f
+000004f0: 726f 6d20 756e 7461 6e67 6c65 7079 7574  rom untanglepyut
+00000500: 2e55 6e54 616e 676c 6572 2069 6d70 6f72  .UnTangler impor
+00000510: 7420 556e 5461 6e67 6c65 720a 0a66 726f  t UnTangler..fro
+00000520: 6d20 756e 7461 6e67 6c65 7079 7574 2e54  m untanglepyut.T
+00000530: 7970 6573 2069 6d70 6f72 7420 556e 7461  ypes import Unta
+00000540: 6e67 6c65 644f 676c 436c 6173 7365 730a  ngledOglClasses.
+00000550: 6672 6f6d 2075 6e74 616e 676c 6570 7975  from untanglepyu
+00000560: 742e 5479 7065 7320 696d 706f 7274 2055  t.Types import U
+00000570: 6e74 616e 676c 6564 4f67 6c4c 696e 6b73  ntangledOglLinks
+00000580: 0a66 726f 6d20 756e 7461 6e67 6c65 7079  .from untanglepy
+00000590: 7574 2e54 7970 6573 2069 6d70 6f72 7420  ut.Types import 
+000005a0: 556e 7461 6e67 6c65 644f 676c 4e6f 7465  UntangledOglNote
+000005b0: 730a 6672 6f6d 2075 6e74 616e 676c 6570  s.from untanglep
+000005c0: 7975 742e 5479 7065 7320 696d 706f 7274  yut.Types import
+000005d0: 2055 6e74 616e 676c 6564 4f67 6c54 6578   UntangledOglTex
+000005e0: 7473 0a0a 756e 7461 6e67 6c65 723a 2055  ts..untangler: U
+000005f0: 6e54 616e 676c 6572 203d 2055 6e54 616e  nTangler = UnTan
+00000600: 676c 6572 2866 7146 696c 654e 616d 653d  gler(fqFileName=
+00000610: 274d 756c 7469 446f 6375 6d65 6e74 5072  'MultiDocumentPr
+00000620: 6f6a 6563 742e 786d 6c27 290a 0a64 6f63  oject.xml')..doc
+00000630: 756d 656e 743a 2044 6f63 756d 656e 7420  ument: Document 
+00000640: 3d20 756e 7461 6e67 6c65 722e 646f 6375  = untangler.docu
+00000650: 6d65 6e74 735b 2744 6961 6772 616d 2d31  ments['Diagram-1
+00000660: 275d 0a0a 6f67 6c43 6c61 7373 6573 3a20  ']..oglClasses: 
+00000670: 556e 7461 6e67 6c65 644f 676c 436c 6173  UntangledOglClas
+00000680: 7365 7320 3d20 646f 6375 6d65 6e74 2e6f  ses = document.o
+00000690: 676c 436c 6173 7365 730a 6f67 6c4c 696e  glClasses.oglLin
+000006a0: 6b73 3a20 2020 556e 7461 6e67 6c65 644f  ks:   UntangledO
+000006b0: 676c 4c69 6e6b 7320 2020 3d20 646f 6375  glLinks   = docu
+000006c0: 6d65 6e74 2e6f 676c 4c69 6e6b 730a 6f67  ment.oglLinks.og
+000006d0: 6c4e 6f74 6573 3a20 2020 556e 7461 6e67  lNotes:   Untang
+000006e0: 6c65 644f 676c 4e6f 7465 7320 2020 3d20  ledOglNotes   = 
+000006f0: 646f 6375 6d65 6e74 2e6f 676c 4e6f 7465  document.oglNote
+00000700: 730a 6f67 6c54 6578 7473 3a20 2020 556e  s.oglTexts:   Un
+00000710: 7461 6e67 6c65 644f 676c 5465 7874 7320  tangledOglTexts 
+00000720: 2020 3d20 646f 6375 6d65 6e74 2e6f 676c    = document.ogl
+00000730: 5465 7874 730a 0a60 6060 0a0a 0a0a 5468  Texts..```....Th
+00000740: 6520 666f 6c6c 6f77 696e 6720 6973 2074  e following is t
+00000750: 6865 2055 4d4c 2064 6961 6772 616d 2066  he UML diagram f
+00000760: 6f72 2074 6865 2050 7975 7420 556e 7461  or the Pyut Unta
+00000770: 6e67 6c65 720a 0a21 5b55 6e74 616e 676c  ngler..![Untangl
+00000780: 6550 7975 745d 2868 7474 7073 3a2f 2f67  ePyut](https://g
+00000790: 6974 6875 622e 636f 6d2f 6861 7369 6932  ithub.com/hasii2
+000007a0: 3031 312f 756e 7461 6e67 6c65 7079 7574  011/untanglepyut
+000007b0: 2f62 6c6f 622f 6d61 7374 6572 2f64 6f63  /blob/master/doc
+000007c0: 732f 556e 7461 6e67 6c65 5079 7574 2e70  s/UntanglePyut.p
+000007d0: 6e67 290a 0a0a 5f5f 5f0a 0a23 2320 4465  ng)...___..## De
+000007e0: 7665 6c6f 7065 7220 4e6f 7465 730a 5468  veloper Notes.Th
+000007f0: 6973 2070 726f 6a65 6374 2075 7365 7320  is project uses 
+00000800: 5b62 7569 6c64 6c61 636b 6579 5d28 6874  [buildlackey](ht
+00000810: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000820: 2f68 6173 6969 3230 3131 2f62 7569 6c64  /hasii2011/build
+00000830: 6c61 636b 6579 2920 666f 7220 6461 7920  lackey) for day 
+00000840: 746f 2064 6179 2064 6576 656c 6f70 6d65  to day developme
+00000850: 6e74 2062 7569 6c64 730a 0a5f 5f5f 0a0a  nt builds..___..
+00000860: 5772 6974 7465 6e20 6279 203c 6120 6872  Written by <a hr
+00000870: 6566 3d22 6d61 696c 746f 3a65 6d61 696c  ef="mailto:email
+00000880: 4068 756d 6265 7274 6f2e 612e 7361 6e63  @humberto.a.sanc
+00000890: 6865 7a2e 6969 4067 6d61 696c 2e63 6f6d  hez.ii@gmail.com
+000008a0: 3f73 7562 6a65 6374 3d48 656c 6c6f 2048  ?subject=Hello H
+000008b0: 756d 6265 7274 6f22 3e48 756d 6265 7274  umberto">Humbert
+000008c0: 6f20 412e 2053 616e 6368 657a 2049 493c  o A. Sanchez II<
+000008d0: 2f61 3e20 2028 4329 2032 3032 330a 0a23  /a>  (C) 2023..#
+000008e0: 2320 4e6f 7465 0a46 6f72 2061 6c6c 206b  # Note.For all k
+000008f0: 696e 6420 6f66 2070 726f 626c 656d 732c  ind of problems,
+00000900: 2072 6571 7565 7374 732c 2065 6e68 616e   requests, enhan
+00000910: 6365 6d65 6e74 732c 2062 7567 2072 6570  cements, bug rep
+00000920: 6f72 7473 2c20 6574 632e 2c0a 706c 6561  orts, etc.,.plea
+00000930: 7365 2064 726f 7020 6d65 2061 6e20 652d  se drop me an e-
+00000940: 6d61 696c 2e0a 0a0a 215b 4875 6d62 6572  mail....![Humber
+00000950: 746f 2773 204d 6f64 6966 6965 6420 4c6f  to's Modified Lo
+00000960: 676f 5d28 6874 7470 733a 2f2f 7261 772e  go](https://raw.
+00000970: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000980: 742e 636f 6d2f 7769 6b69 2f68 6173 6969  t.com/wiki/hasii
+00000990: 3230 3131 2f67 6974 746f 646f 6973 7463  2011/gittodoistc
+000009a0: 6c6f 6e65 2f69 6d61 6765 732f 5369 6c6c  lone/images/Sill
+000009b0: 7947 6974 4875 622e 706e 6729 0a0a 4920  yGitHub.png)..I 
+000009c0: 616d 2063 6f6e 6365 726e 6564 2061 626f  am concerned abo
+000009d0: 7574 2047 6974 4875 6227 7320 436f 7069  ut GitHub's Copi
+000009e0: 6c6f 7420 7072 6f6a 6563 740a 0a0a 0a49  lot project....I
+000009f0: 2075 7267 6520 796f 7520 746f 2072 6561   urge you to rea
+00000a00: 6420 6162 6f75 7420 7468 650a 5b47 6976  d about the.[Giv
+00000a10: 6520 7570 2047 6974 4875 625d 2868 7474  e up GitHub](htt
+00000a20: 7073 3a2f 2f47 6976 6555 7047 6974 4875  ps://GiveUpGitHu
+00000a30: 622e 6f72 6729 2063 616d 7061 6967 6e20  b.org) campaign 
+00000a40: 6672 6f6d 0a5b 7468 6520 536f 6674 7761  from.[the Softwa
+00000a50: 7265 2046 7265 6564 6f6d 2043 6f6e 7365  re Freedom Conse
+00000a60: 7276 616e 6379 5d28 6874 7470 733a 2f2f  rvancy](https://
+00000a70: 7366 636f 6e73 6572 7661 6e63 792e 6f72  sfconservancy.or
+00000a80: 6729 2e0a 0a57 6869 6c65 2049 2064 6f20  g)...While I do 
+00000a90: 6e6f 7420 6164 766f 6361 7465 2066 6f72  not advocate for
+00000aa0: 2061 6c6c 2074 6865 2069 7373 7565 7320   all the issues 
+00000ab0: 6c69 7374 6564 2074 6865 7265 2049 2064  listed there I d
+00000ac0: 6f20 6e6f 7420 6c69 6b65 2074 6861 740a  o not like that.
+00000ad0: 6120 636f 6d70 616e 7920 6c69 6b65 204d  a company like M
+00000ae0: 6963 726f 736f 6674 206d 6179 2070 726f  icrosoft may pro
+00000af0: 6669 7420 6672 6f6d 206f 7065 6e20 736f  fit from open so
+00000b00: 7572 6365 2070 726f 6a65 6374 732e 0a0a  urce projects...
+00000b10: 4920 636f 6e74 696e 7565 2074 6f20 7573  I continue to us
+00000b20: 6520 4769 7448 7562 2062 6563 6175 7365  e GitHub because
+00000b30: 2069 7420 6f66 6665 7273 2074 6865 2073   it offers the s
+00000b40: 6572 7669 6365 7320 4920 6e65 6564 2066  ervices I need f
+00000b50: 6f72 2066 7265 652e 2020 4275 742c 2049  or free.  But, I
+00000b60: 2063 6f6e 7469 6e75 650a 746f 206d 6f6e   continue.to mon
+00000b70: 6974 6f72 2074 6865 6972 2074 6572 6d73  itor their terms
+00000b80: 206f 6620 7365 7276 6963 652e 0a0a 416e   of service...An
+00000b90: 7920 7573 6520 6f66 2074 6869 7320 7072  y use of this pr
+00000ba0: 6f6a 6563 7427 7320 636f 6465 2062 7920  oject's code by 
+00000bb0: 4769 7448 7562 2043 6f70 696c 6f74 2c20  GitHub Copilot, 
+00000bc0: 7061 7374 206f 7220 7072 6573 656e 742c  past or present,
+00000bd0: 2069 7320 646f 6e65 0a77 6974 686f 7574   is done.without
+00000be0: 206d 7920 7065 726d 6973 7369 6f6e 2e20   my permission. 
+00000bf0: 2049 2064 6f20 6e6f 7420 636f 6e73 656e   I do not consen
+00000c00: 7420 746f 2047 6974 4875 6227 7320 7573  t to GitHub's us
+00000c10: 6520 6f66 2074 6869 7320 7072 6f6a 6563  e of this projec
+00000c20: 7427 730a 636f 6465 2069 6e20 436f 7069  t's.code in Copi
+00000c30: 6c6f 742e 0a0a 4120 7265 706f 7369 746f  lot...A reposito
+00000c40: 7279 206f 776e 6572 206d 6179 206f 7074  ry owner may opt
+00000c50: 206f 7574 206f 6620 436f 7069 6c6f 7420   out of Copilot 
+00000c60: 6279 2063 6861 6e67 696e 6720 5365 7474  by changing Sett
+00000c70: 696e 6773 202d 2d3e 2047 6974 4875 6220  ings --> GitHub 
+00000c80: 436f 7069 6c6f 742e 0a0a 4920 6861 7665  Copilot...I have
+00000c90: 2064 6f6e 6520 736f 2e0a                  done so..
```

### Comparing `untanglepyut-0.6.6/setup.py` & `untanglepyut-0.6.60/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 LICENSE = (HERE / 'LICENSE').read_text()
 
 setup(
     name="untanglepyut",
-    version="0.6.6",
+    version="0.6.60",
     author_email='Humberto.A.Sanchez.II@gmail.com',
     description='XML to Ogl Object Model',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hasii2011/untanglepyut",
     packages=[
         'untanglepyut'
     ],
     package_data={
         'untanglepyut': ['py.typed'],
     },
 
-    install_requires=['ogl==0.60.30', 'untangle==1.2.1'],
+    install_requires=['hasiihelper~=0.2.0', 'hasiicommon~=0.2.2', 'pyutmodel~=1.4.3', 'ogl==0.70.26', 'untangle==1.2.1'],
 )
```

### Comparing `untanglepyut-0.6.6/untanglepyut/BaseUnTangle.py` & `untanglepyut-0.6.60/untanglepyut/BaseUnTangle.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.6/untanglepyut/Common.py` & `untanglepyut-0.6.60/untanglepyut/Common.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.6/untanglepyut/Types.py` & `untanglepyut-0.6.60/untanglepyut/Types.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.6/untanglepyut/UnTangleOglLinks.py` & `untanglepyut-0.6.60/untanglepyut/UnTangleOglLinks.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 from typing import List
 from typing import NewType
 from typing import Union
 from typing import cast
 
 from dataclasses import dataclass
 
+from miniogl.AttachmentSide import AttachmentSide
 from pyutmodel.PyutClass import PyutClass
 from untangle import Element
 
-from miniogl.AttachmentLocation import AttachmentLocation
+
 from miniogl.ControlPoint import ControlPoint
 from miniogl.SelectAnchorPoint import SelectAnchorPoint
 
 from pyutmodel.PyutLinkType import PyutLinkType
 from pyutmodel.PyutInterface import PyutInterface
 from pyutmodel.PyutLink import PyutLink
 
@@ -157,39 +158,39 @@
                                                   dstPos=(gla.dstX, gla.dstY)
                                                   )
         oglLink.SetSpline(gla.spline)
         srcShape.addLink(oglLink)
         dstShape.addLink(oglLink)
 
         # put the anchors at the right position
-        srcAnchor = oglLink.GetSource()
-        dstAnchor = oglLink.GetDestination()
+        srcAnchor = oglLink.sourceAnchor
+        dstAnchor = oglLink.destinationAnchor
         srcAnchor.SetPosition(gla.srcX, gla.srcY)
         dstAnchor.SetPosition(gla.dstX, gla.dstY)
 
         srcModel = srcAnchor.GetModel()
         srcModel.SetPosition(x=gla.srcX, y=gla.srcY)
         dstModel = dstAnchor.GetModel()
         dstModel.SetPosition(x=gla.dstX, y=gla.dstY)
 
         # add the control points to the line
         line   = srcAnchor.GetLines()[0]     # only 1 line per anchor in Pyut
-        parent = line.GetSource().GetParent()
-        selfLink: bool = parent is oglLink.GetDestination().GetParent()
+        parent = line.sourceAnchor.GetParent()
+        selfLink: bool = parent is oglLink.destinationAnchor.GetParent()
 
         controlPoints: UntangledControlPoints = self._generateControlPoints(graphicLink=graphicLink)
         for controlPoint in controlPoints:
             oglLink.AddControl(control=controlPoint, after=None)
             if selfLink:
                 x, y = controlPoint.GetPosition()
                 controlPoint.SetParent(parent)
                 controlPoint.SetPosition(x, y)
 
         if isinstance(oglLink, OglAssociation):
-            self.__furtherCustomizeAssociationLink(graphicLink, oglLink)
+            oglLink = self.__furtherCustomizeAssociationLink(graphicLink, oglLink)
 
         self._reconstituteLinkDataModel(oglLink)
 
         return oglLink
 
     def _oglLinkFactory(self, srcShape, pyutLink, destShape, linkType: PyutLinkType, srcPos=None, dstPos=None):
         """
@@ -235,27 +236,27 @@
         assert len(linkableOglObjects) != 0, 'Developer forgot to create dictionary'
 
         #
         # TODO: Do not use these x,y positions;  They are diagram relative
         #
         # x: int = int(graphicLollipop['x'])
         # y: int = int(graphicLollipop['y'])
-        attachmentLocationStr: str                = graphicLollipop['attachmentPoint']
-        attachmentLocation:    AttachmentLocation = AttachmentLocation.toEnum(attachmentLocationStr)
+        attachmentLocationStr: str            = graphicLollipop['attachmentPoint']
+        attachmentSide:        AttachmentSide = AttachmentSide.toEnum(attachmentLocationStr)
 
         elements: Element = graphicLollipop.get_elements('Interface')
         assert len(elements) == 1, 'If more than one interface tag the XML is invalid'
         interfaceElement: Element        = elements[0]
         pyutInterface:    PyutInterface = self._untanglePyut.interfaceToPyutInterface(interface=interfaceElement)
 
         oglClass:    OglClass    = self._getOglClassFromName(pyutInterface.implementors[0], linkableOglObjects)
-        oglPosition: OglPosition = self._determineAttachmentPoint(attachmentLocation, oglClass)
+        oglPosition: OglPosition = self._determineAttachmentPoint(attachmentSide, oglClass)
         self.logger.debug(f'{oglPosition.x=},{oglPosition.y=}')
 
-        anchorPoint:      SelectAnchorPoint = SelectAnchorPoint(x=oglPosition.x, y=oglPosition.y, attachmentPoint=attachmentLocation, parent=oglClass)
+        anchorPoint:      SelectAnchorPoint = SelectAnchorPoint(x=oglPosition.x, y=oglPosition.y, attachmentSide=attachmentSide, parent=oglClass)
         oglInterface2:    OglInterface2     = OglInterface2(pyutInterface=pyutInterface, destinationAnchor=anchorPoint)
 
         return oglInterface2
 
     def _getOglClassFromName(self, className: str, linkableOglObjects: LinkableOglObjects) -> OglClass:
         """
         Looks up a name in the linkable objects dictionary and return the associated class
@@ -272,15 +273,15 @@
         for oglClass in linkableOglObjects.values():
             if oglClass.pyutObject.name == className:
                 foundClass = cast(OglClass, oglClass)
                 break
         assert foundClass is not None, 'XML must be in error'
         return foundClass
 
-    def _determineAttachmentPoint(self, attachmentPoint: AttachmentLocation, oglClass: OglClass) -> OglPosition:
+    def _determineAttachmentPoint(self, attachmentPoint: AttachmentSide, oglClass: OglClass) -> OglPosition:
         """
         Even though we serialize the attachment point location that position is relative to the diagram.
         When we recreate the attachment point position we have to create it relative to its parent
         TODO: When the Pyut serializer makes the positions relative to the implementor we will not need this code
 
         Args:
             attachmentPoint:    Where on the parent
@@ -289,30 +290,30 @@
         Returns:  An OglPosition with coordinates relative to the implementor
         """
 
         oglPosition: OglPosition = OglPosition()
 
         dw, dh     = oglClass.GetSize()
 
-        if attachmentPoint == AttachmentLocation.NORTH:
+        if attachmentPoint == AttachmentSide.NORTH:
             northX: int = dw // 2
             northY: int = 0
             oglPosition.x = northX
             oglPosition.y = northY
-        elif attachmentPoint == AttachmentLocation.SOUTH:
+        elif attachmentPoint == AttachmentSide.SOUTH:
             southX = dw // 2
             southY = dh
             oglPosition.x = southX
             oglPosition.y = southY
-        elif attachmentPoint == AttachmentLocation.WEST:
+        elif attachmentPoint == AttachmentSide.WEST:
             westX: int = 0
             westY: int = dh // 2
             oglPosition.x = westX
             oglPosition.y = westY
-        elif attachmentPoint == AttachmentLocation.EAST:
+        elif attachmentPoint == AttachmentSide.EAST:
             eastX: int = dw
             eastY: int = dh // 2
             oglPosition.x = eastX
             oglPosition.y = eastY
         else:
             self.logger.warning(f'Unknown attachment point: {attachmentPoint}')
             assert False, 'Unknown attachment point'
@@ -338,57 +339,65 @@
 
         ._parents   for Inheritance links
         ._links     for all other link types
 
         Args:
             oglLink:       An OglLink
         """
-        srcShape:  OglClass = oglLink.getSourceShape()
-        destShape: OglClass = oglLink.getDestinationShape()
+        srcShape:  OglClass = oglLink.sourceShape
+        destShape: OglClass = oglLink.destinationShape
         self.logger.debug(f'source ID: {srcShape.id} - destination ID: {destShape.id}')
 
         pyutLink: PyutLink = oglLink.pyutObject
 
         if pyutLink.linkType == PyutLinkType.INHERITANCE:
             childPyutClass:  PyutClass = cast(PyutClass, srcShape.pyutObject)
             parentPyutClass: PyutClass = cast(PyutClass, destShape.pyutObject)
             childPyutClass.addParent(parentPyutClass)
         else:
             srcPyutClass:  PyutClass = cast(PyutClass, srcShape.pyutObject)
             srcPyutClass.addLink(pyutLink)
 
-    def __furtherCustomizeAssociationLink(self, graphicLink: Element, oglLink: OglAssociation):
+    def __furtherCustomizeAssociationLink(self, graphicLink: Element, oglLink: OglAssociation) -> OglAssociation:
         """
         Customize the visual aspects of an Association link
 
         TODO:  There is no support for this yet.  Need to add it to OglAssociation
 
         Args:
             graphicLink:  The top level GraphicLink Element
             oglLink:      The current OGL representation of the graphicLink
+
+        Returns:  The updated association link
         """
         center: OglAssociationLabel = oglLink.centerLabel
         src:    OglAssociationLabel = oglLink.sourceCardinality
         dest:   OglAssociationLabel = oglLink.destinationCardinality
 
-        self.__setAssociationLabelPosition(graphicLink, 'LabelCenter', center)
-        self.__setAssociationLabelPosition(graphicLink, 'LabelSrc',    src)
-        self.__setAssociationLabelPosition(graphicLink, 'LabelDst',    dest)
+        oglLink.centerLabel            = self.__setAssociationLabelPosition(graphicLink, 'LabelCenter', center)
+        oglLink.sourceCardinality      = self.__setAssociationLabelPosition(graphicLink, 'LabelSrc',    src)
+        oglLink.destinationCardinality = self.__setAssociationLabelPosition(graphicLink, 'LabelDst',    dest)
+
+        return oglLink
 
-    def __setAssociationLabelPosition(self, graphicLink: Element, tagName: str, associationLabel: OglAssociationLabel):
+    def __setAssociationLabelPosition(self, graphicLink: Element, tagName: str, associationLabel: OglAssociationLabel) -> OglAssociationLabel:
         """
 
         Args:
             graphicLink:  The top level GraphicLink Element
             tagName:      The XML Element name
             associationLabel:  The Ogl association label to update
+
+        Returns:  The updated association label
         """
         labels:  List[Element]   = graphicLink.get_elements(tagName)
         assert len(labels) == 1, 'There can be only one'
         label: Element = labels[0]
         x: int = int(label['x'])
         y: int = int(label['y'])
 
         self.logger.debug(f'tagName: {tagName} `{associationLabel.text=}`  pos: ({x},{y})')
 
         associationLabel.oglPosition.x = x
         associationLabel.oglPosition.y = y
+
+        return associationLabel
```

### Comparing `untanglepyut-0.6.6/untanglepyut/UnTanglePyut.py` & `untanglepyut-0.6.60/untanglepyut/UnTanglePyut.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import List
 from typing import NewType
 from typing import cast
 
 from logging import Logger
 from logging import getLogger
 
+from os import linesep as osLineSep
+
 from untangle import Element
 
 from pyutmodel.PyutField import PyutField
 from pyutmodel.PyutField import PyutFields
 
 from pyutmodel.PyutObject import PyutObject
 from pyutmodel.PyutUseCase import PyutUseCase
@@ -54,14 +56,17 @@
     destinationId: int           = -1
 
 
 class UnTanglePyut:
     """
     Converts PyutModel XML to Pyut Objects
     """
+    # https://www.codetable.net/hex/a
+    END_OF_LINE_MARKER: str ='&#xA;'
+
     def __init__(self):
 
         self.logger: Logger = getLogger(__name__)
 
     def classToPyutClass(self, graphicClass: Element) -> PyutClass:
         classElement: Element = graphicClass.Class
 
@@ -97,33 +102,39 @@
             graphicText:   Of the form:   <Text id="3" content="I am standalone text"/>
 
         Returns: A PyutText Object
         """
         textElement: Element  = graphicText.Text
         pyutText:    PyutText = PyutText()
 
-        pyutText.id     = textElement['id']
-        pyutText.content = textElement['content']
+        pyutText.id  = textElement['id']
+
+        rawContent:   str = textElement['content']
+        cleanContent: str = rawContent.replace(UnTanglePyut.END_OF_LINE_MARKER, osLineSep)
+        pyutText.content = cleanContent
 
         return pyutText
 
     def noteToPyutNote(self, graphicNote: Element) -> PyutNote:
         """
         Parse Note elements
         Args:
             graphicNote: of the form:  <Note id="2" content="I am a UML Note" filename=""/>
 
         Returns: A PyutNote Object
         """
         noteElement: Element = graphicNote.Note
         pyutNote: PyutNote = PyutNote()
 
+        # fix line feeds
         pyutNote = cast(PyutNote, self._addPyutObjectAttributes(pyutElement=noteElement, pyutObject=pyutNote))
 
-        pyutNote.content = noteElement['content']
+        rawContent:   str = noteElement['content']
+        cleanContent: str = rawContent.replace(UnTanglePyut.END_OF_LINE_MARKER, osLineSep)
+        pyutNote.content = cleanContent
         return pyutNote
 
     def interfaceToPyutInterface(self, interface: Element) -> PyutInterface:
 
         interfaceId: int = int(interface['id'])
         name:        str = interface['name']
         description: str = interface['description']
@@ -212,25 +223,25 @@
         Returns:  Bogus data class
         """
 
         messageElement: Element       = graphicSDMessage.SDMessage
         pyutSDMessage:  PyutSDMessage = PyutSDMessage()
 
         pyutSDMessage.id = int(messageElement['id'])
-        pyutSDMessage.setMessage(messageElement['message'])
+        pyutSDMessage.message = messageElement['message']
         pyutSDMessage.linkType = PyutLinkType.SD_MESSAGE
 
         srcID: int = int(messageElement['srcID'])
         dstID: int = int(messageElement['dstID'])
 
         srcTime: int = int(messageElement['srcTime'])
         dstTime: int = int(messageElement['dstTime'])
 
-        pyutSDMessage.setSrcTime(value=srcTime, updateOGLObject=False)
-        pyutSDMessage.setDstTime(value=dstTime, updateOGLObject=False)
+        pyutSDMessage.sourceY      = srcTime
+        pyutSDMessage.destinationY = dstTime
 
         bogus: ConvolutedPyutSDMessageInformation = ConvolutedPyutSDMessageInformation()
 
         bogus.pyutSDMessage = pyutSDMessage
         bogus.sourceId      = srcID
         bogus.destinationId = dstID
 
@@ -276,43 +287,46 @@
         fieldElements: Elements = classElement.get_elements('Field')
         for fieldElement in fieldElements:
             visibility:    PyutVisibilityEnum = PyutVisibilityEnum.toEnum(fieldElement['visibility'])
             paramElements: Elements           = fieldElement.get_elements('Param')
             assert len(paramElements) == 1, 'Curiously there should be only one'
 
             paramElement: Element = paramElements[0]
-            fieldName: str = paramElement['name']
-            pyutType:  PyutType  = PyutType(paramElement['type'])
-
-            pyutField: PyutField = PyutField(name=fieldName, visibility=visibility, fieldType=pyutType)
+            fieldName:    str       = paramElement['name']
+            pyutType:     PyutType  = PyutType(paramElement['type'])
+            defaultValue: str       = paramElement['defaultValue']
+            if defaultValue is None:
+                defaultValue = ''
+            pyutField: PyutField = PyutField(name=fieldName, visibility=visibility, fieldType=pyutType, defaultValue=defaultValue)
 
             untangledPyutFields.append(pyutField)
 
         return untangledPyutFields
 
     def _modifierToPyutMethodModifiers(self, methodElement: Element) -> PyutModifiers:
         """
         Should be in this form:
 
-        <Modifier name="modifier1,modifier2,modifier3"/>
+            <Modifier name="Modifier1"/>
+            <Modifier name="Modifier2"/>
+            <Modifier name="Modifier3"/>
+            <Modifier name="Modifier4"/>
 
         Args:
             methodElement:
 
         Returns:  PyutModifiers if not exist returns an empty
         """
 
         modifierElements = methodElement.get_elements('Modifier')
 
         pyutModifiers: PyutModifiers = PyutModifiers([])
         if len(modifierElements) > 0:
-            modifierElement: Element   = modifierElements[0]
-            names:           str       = modifierElement['name']    # comma delimited string
-            nameList:        List[str] = names.split(',')
-            for modifierName in nameList:
+            for modifierElement in modifierElements:
+                modifierName:           str       = modifierElement['name']
                 pyutModifier: PyutModifier = PyutModifier(modifierTypeName=modifierName)
                 pyutModifiers.append(pyutModifier)
 
         return pyutModifiers
 
     def _paramToPyutParameters(self, methodElement: Element) -> PyutParameters:
```

### Comparing `untanglepyut-0.6.6/untanglepyut/UnTangleUseCaseDiagram.py` & `untanglepyut-0.6.60/untanglepyut/UnTangleUseCaseDiagram.py`

 * *Files identical despite different names*

### Comparing `untanglepyut-0.6.6/untanglepyut/UnTangler.py` & `untanglepyut-0.6.60/untanglepyut/UnTangler.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,16 @@
             elif document.documentType == 'USECASE_DIAGRAM':
 
                 unTangleUseCaseDiagram: UnTangleUseCaseDiagram = UnTangleUseCaseDiagram()
 
                 unTangleUseCaseDiagram.unTangle(pyutDocument=pyutDocument)
                 document.oglActors   = unTangleUseCaseDiagram.oglActors
                 document.oglUseCases = unTangleUseCaseDiagram.oglUseCases
+                document.oglNotes    = self._graphicNotesToOglNotes(pyutDocument=pyutDocument)
+                document.oglTexts    = self._graphicalTextToOglTexts(pyutDocument=pyutDocument)
 
                 linkableOglObjects = self._buildDictionary(document=document)
                 document.oglLinks  = self._untangleOglLinks.graphicLinksToOglLinks(pyutDocument, linkableOglObjects=linkableOglObjects)
             else:
                 assert False, f'Unknown document type: {document.documentType}'
 
     def getRawXml(self, fqFileName: str) -> str:
```

### Comparing `untanglepyut-0.6.6/untanglepyut/UntangleSequenceDiagram.py` & `untanglepyut-0.6.60/untanglepyut/UntangleSequenceDiagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Dict
+
 from typing import List
-from typing import NewType
 
 from logging import Logger
 from logging import getLogger
 
 from untangle import Element
 
 from pyutmodel.PyutSDInstance import PyutSDInstance
@@ -94,15 +93,15 @@
             pyutSDMessage: PyutSDMessage = bogus.pyutSDMessage
 
             srcInstance: OglSDInstance = self._oglSDInstances[bogus.sourceId]
             dstInstance: OglSDInstance = self._oglSDInstances[bogus.destinationId]
 
             pyutSDMessage.setSource(srcInstance.pyutObject)          # Ugh, time was set by sdMessageToPyutSDMessage
             pyutSDMessage.setDestination(dstInstance.pyutObject)     # This "split" functionality must be fixed
-            oglSDMessage: OglSDMessage = OglSDMessage(srcShape=srcInstance, pyutSDMessage=pyutSDMessage, dstShape=dstInstance)
+            oglSDMessage: OglSDMessage = OglSDMessage(srcSDInstance=srcInstance, pyutSDMessage=pyutSDMessage, dstSDInstance=dstInstance)
 
             srcInstance.addLink(link=oglSDMessage)
             dstInstance.addLink(link=oglSDMessage)
 
             oglSDMessages[pyutSDMessage.id] = oglSDMessage
 
         return oglSDMessages
```

### Comparing `untanglepyut-0.6.6/untanglepyut.egg-info/PKG-INFO` & `untanglepyut-0.6.60/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,178 +1,218 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 756e 7461  : 2.1.Name: unta
 00000020: 6e67 6c65 7079 7574 0a56 6572 7369 6f6e  nglepyut.Version
-00000030: 3a20 302e 362e 360a 5375 6d6d 6172 793a  : 0.6.6.Summary:
-00000040: 2058 4d4c 2074 6f20 4f67 6c20 4f62 6a65   XML to Ogl Obje
-00000050: 6374 204d 6f64 656c 0a48 6f6d 652d 7061  ct Model.Home-pa
-00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000070: 7562 2e63 6f6d 2f68 6173 6969 3230 3131  ub.com/hasii2011
-00000080: 2f75 6e74 616e 676c 6570 7975 740a 4175  /untanglepyut.Au
-00000090: 7468 6f72 2d65 6d61 696c 3a20 4875 6d62  thor-email: Humb
-000000a0: 6572 746f 2e41 2e53 616e 6368 657a 2e49  erto.A.Sanchez.I
-000000b0: 4940 676d 6169 6c2e 636f 6d0a 4465 7363  I@gmail.com.Desc
-000000c0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-000000d0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-000000e0: 6f77 6e0a 4c69 6365 6e73 652d 4669 6c65  own.License-File
-000000f0: 3a20 4c49 4345 4e53 450a 0a3c 696d 6720  : LICENSE..<img 
-00000100: 7372 633d 222e 2f64 6f63 732f 6167 706c  src="./docs/agpl
-00000110: 2d6c 6963 656e 7365 2d77 6562 2d62 6164  -license-web-bad
-00000120: 6765 2d76 6572 7369 6f6e 2d32 2d32 3536  ge-version-2-256
-00000130: 7834 382e 706e 6722 2f3e 0a0a 5b21 5b4d  x48.png"/>..[![M
-00000140: 6169 6e74 656e 616e 6365 5d28 6874 7470  aintenance](http
-00000150: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000160: 696f 2f62 6164 6765 2f4d 6169 6e74 6169  io/badge/Maintai
-00000170: 6e65 6425 3346 2d79 6573 2d67 7265 656e  ned%3F-yes-green
-00000180: 2e73 7667 295d 2868 7474 7073 3a2f 2f47  .svg)](https://G
-00000190: 6974 4875 622e 636f 6d2f 4e61 6572 6565  itHub.com/Naeree
-000001a0: 6e2f 5374 7261 7044 6f77 6e2e 6a73 2f67  n/StrapDown.js/g
-000001b0: 7261 7068 732f 636f 6d6d 6974 2d61 6374  raphs/commit-act
-000001c0: 6976 6974 7929 0a5b 215b 4369 7263 6c65  ivity).[![Circle
-000001d0: 4349 5d28 6874 7470 733a 2f2f 646c 2e63  CI](https://dl.c
-000001e0: 6972 636c 6563 692e 636f 6d2f 7374 6174  ircleci.com/stat
-000001f0: 7573 2d62 6164 6765 2f69 6d67 2f67 682f  us-badge/img/gh/
-00000200: 6861 7369 6932 3031 312f 756e 7461 6e67  hasii2011/untang
-00000210: 6c65 7079 7574 2f74 7265 652f 6d61 7374  lepyut/tree/mast
-00000220: 6572 2e73 7667 3f73 7479 6c65 3d73 6869  er.svg?style=shi
-00000230: 656c 6429 5d28 6874 7470 733a 2f2f 646c  eld)](https://dl
-00000240: 2e63 6972 636c 6563 692e 636f 6d2f 7374  .circleci.com/st
-00000250: 6174 7573 2d62 6164 6765 2f72 6564 6972  atus-badge/redir
-00000260: 6563 742f 6768 2f68 6173 6969 3230 3131  ect/gh/hasii2011
-00000270: 2f75 6e74 616e 676c 6570 7975 742f 7472  /untanglepyut/tr
-00000280: 6565 2f6d 6173 7465 7229 0a5b 215b 6d61  ee/master).[![ma
-00000290: 634f 535d 2868 7474 7073 3a2f 2f73 7667  cOS](https://svg
-000002a0: 7368 6172 652e 636f 6d2f 692f 5a6a 502e  share.com/i/ZjP.
-000002b0: 7376 6729 5d28 6874 7470 733a 2f2f 7376  svg)](https://sv
-000002c0: 6773 6861 7265 2e63 6f6d 2f69 2f5a 6a50  gshare.com/i/ZjP
-000002d0: 2e73 7667 290a 0a5b 215b 666f 7274 6865  .svg)..[![forthe
-000002e0: 6261 6467 6520 6d61 6465 2d77 6974 682d  badge made-with-
-000002f0: 7079 7468 6f6e 5d28 6874 7470 3a2f 2f46  python](http://F
-00000300: 6f72 5468 6542 6164 6765 2e63 6f6d 2f69  orTheBadge.com/i
-00000310: 6d61 6765 732f 6261 6467 6573 2f6d 6164  mages/badges/mad
-00000320: 652d 7769 7468 2d70 7974 686f 6e2e 7376  e-with-python.sv
-00000330: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
-00000340: 7079 7468 6f6e 2e6f 7267 2f29 0a0a 5468  python.org/)..Th
-00000350: 6973 2070 726f 6a65 6374 2069 7320 696e  is project is in
-00000360: 7465 6e64 6564 2074 6f20 6265 2075 7365  tended to be use
-00000370: 6420 6279 205b 5079 7574 2050 6c75 6769  d by [Pyut Plugi
-00000380: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
-00000390: 622e 636f 6d2f 6861 7369 6932 3031 312f  b.com/hasii2011/
-000003a0: 7079 7574 706c 7567 696e 636f 7265 2920  pyutplugincore) 
-000003b0: 6465 7665 6c6f 7065 7273 2074 6f20 636f  developers to co
-000003c0: 6e76 6572 7420 5b50 7975 745d 2868 7474  nvert [Pyut](htt
-000003d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000003e0: 6861 7369 6932 3031 312f 5079 5574 2920  hasii2011/PyUt) 
-000003f0: 584d 4c20 6669 6c65 7320 746f 2074 6865  XML files to the
-00000400: 205b 4f67 6c20 4d6f 6465 6c5d 2868 7474   [Ogl Model](htt
-00000410: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000420: 6861 7369 6932 3031 312f 6f67 6c29 2063  hasii2011/ogl) c
-00000430: 6c61 7373 6573 2e20 2054 6865 7365 206d  lasses.  These m
-00000440: 6f64 656c 2063 6c61 7373 6573 2063 616e  odel classes can
-00000450: 2074 6865 6e20 6265 2075 7365 6420 6279   then be used by
-00000460: 2074 6865 2050 7975 7420 5549 2074 6f20   the Pyut UI to 
-00000470: 6469 7370 6c61 7920 6173 2055 4d4c 2044  display as UML D
-00000480: 6961 6772 616d 732e 0a0a 2d2d 2d2d 2d2d  iagrams...------
-00000490: 0a0a 5573 6520 6173 2066 6f6c 6c6f 7773  ..Use as follows
-000004a0: 3a0a 0a60 6060 7079 7468 6f6e 0a66 726f  :..```python.fro
-000004b0: 6d20 756e 7461 6e67 6c65 7079 7574 2e55  m untanglepyut.U
-000004c0: 6e54 616e 676c 6572 2069 6d70 6f72 7420  nTangler import 
-000004d0: 446f 6375 6d65 6e74 0a66 726f 6d20 756e  Document.from un
-000004e0: 7461 6e67 6c65 7079 7574 2e55 6e54 616e  tanglepyut.UnTan
-000004f0: 676c 6572 2069 6d70 6f72 7420 556e 5461  gler import UnTa
-00000500: 6e67 6c65 720a 0a66 726f 6d20 756e 7461  ngler..from unta
-00000510: 6e67 6c65 7079 7574 2e54 7970 6573 2069  nglepyut.Types i
-00000520: 6d70 6f72 7420 556e 7461 6e67 6c65 644f  mport UntangledO
-00000530: 676c 436c 6173 7365 730a 6672 6f6d 2075  glClasses.from u
-00000540: 6e74 616e 676c 6570 7975 742e 5479 7065  ntanglepyut.Type
-00000550: 7320 696d 706f 7274 2055 6e74 616e 676c  s import Untangl
-00000560: 6564 4f67 6c4c 696e 6b73 0a66 726f 6d20  edOglLinks.from 
-00000570: 756e 7461 6e67 6c65 7079 7574 2e54 7970  untanglepyut.Typ
-00000580: 6573 2069 6d70 6f72 7420 556e 7461 6e67  es import Untang
-00000590: 6c65 644f 676c 4e6f 7465 730a 6672 6f6d  ledOglNotes.from
-000005a0: 2075 6e74 616e 676c 6570 7975 742e 5479   untanglepyut.Ty
-000005b0: 7065 7320 696d 706f 7274 2055 6e74 616e  pes import Untan
-000005c0: 676c 6564 4f67 6c54 6578 7473 0a0a 756e  gledOglTexts..un
-000005d0: 7461 6e67 6c65 723a 2055 6e54 616e 676c  tangler: UnTangl
-000005e0: 6572 203d 2055 6e54 616e 676c 6572 2866  er = UnTangler(f
-000005f0: 7146 696c 654e 616d 653d 274d 756c 7469  qFileName='Multi
-00000600: 446f 6375 6d65 6e74 5072 6f6a 6563 742e  DocumentProject.
-00000610: 786d 6c27 290a 0a64 6f63 756d 656e 743a  xml')..document:
-00000620: 2044 6f63 756d 656e 7420 3d20 756e 7461   Document = unta
-00000630: 6e67 6c65 722e 646f 6375 6d65 6e74 735b  ngler.documents[
-00000640: 2744 6961 6772 616d 2d31 275d 0a0a 6f67  'Diagram-1']..og
-00000650: 6c43 6c61 7373 6573 3a20 556e 7461 6e67  lClasses: Untang
-00000660: 6c65 644f 676c 436c 6173 7365 7320 3d20  ledOglClasses = 
-00000670: 646f 6375 6d65 6e74 2e6f 676c 436c 6173  document.oglClas
-00000680: 7365 730a 6f67 6c4c 696e 6b73 3a20 2020  ses.oglLinks:   
-00000690: 556e 7461 6e67 6c65 644f 676c 4c69 6e6b  UntangledOglLink
-000006a0: 7320 2020 3d20 646f 6375 6d65 6e74 2e6f  s   = document.o
-000006b0: 676c 4c69 6e6b 730a 6f67 6c4e 6f74 6573  glLinks.oglNotes
-000006c0: 3a20 2020 556e 7461 6e67 6c65 644f 676c  :   UntangledOgl
-000006d0: 4e6f 7465 7320 2020 3d20 646f 6375 6d65  Notes   = docume
-000006e0: 6e74 2e6f 676c 4e6f 7465 730a 6f67 6c54  nt.oglNotes.oglT
-000006f0: 6578 7473 3a20 2020 556e 7461 6e67 6c65  exts:   Untangle
-00000700: 644f 676c 5465 7874 7320 2020 3d20 646f  dOglTexts   = do
-00000710: 6375 6d65 6e74 2e6f 676c 5465 7874 730a  cument.oglTexts.
-00000720: 0a60 6060 0a0a 0a0a 5468 6520 666f 6c6c  .```....The foll
-00000730: 6f77 696e 6720 6973 2074 6865 2055 4d4c  owing is the UML
-00000740: 2064 6961 6772 616d 2066 6f72 2074 6865   diagram for the
-00000750: 2050 7975 7420 556e 7461 6e67 6c65 720a   Pyut Untangler.
-00000760: 0a21 5b55 6e74 616e 676c 6550 7975 745d  .![UntanglePyut]
-00000770: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000780: 636f 6d2f 6861 7369 6932 3031 312f 756e  com/hasii2011/un
-00000790: 7461 6e67 6c65 7079 7574 2f62 6c6f 622f  tanglepyut/blob/
-000007a0: 6d61 7374 6572 2f64 6f63 732f 556e 7461  master/docs/Unta
-000007b0: 6e67 6c65 5079 7574 2e70 6e67 290a 0a0a  nglePyut.png)...
-000007c0: 0a2d 2d2d 2d2d 2d0a 0a0a 215b 4875 6d62  .------...![Humb
-000007d0: 6572 746f 2773 204d 6f64 6966 6965 6420  erto's Modified 
-000007e0: 4c6f 676f 5d28 6874 7470 733a 2f2f 7261  Logo](https://ra
-000007f0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00000800: 656e 742e 636f 6d2f 7769 6b69 2f68 6173  ent.com/wiki/has
-00000810: 6969 3230 3131 2f67 6974 746f 646f 6973  ii2011/gittodois
-00000820: 7463 6c6f 6e65 2f69 6d61 6765 732f 5369  tclone/images/Si
-00000830: 6c6c 7947 6974 4875 622e 706e 6729 0a0a  llyGitHub.png)..
-00000840: 4920 616d 2063 6f6e 6365 726e 6564 2061  I am concerned a
-00000850: 626f 7574 2047 6974 4875 6227 7320 436f  bout GitHub's Co
-00000860: 7069 6c6f 7420 7072 6f6a 6563 740a 0a0a  pilot project...
-00000870: 0a49 2075 7267 6520 796f 7520 746f 2072  .I urge you to r
-00000880: 6561 6420 6162 6f75 7420 7468 650a 5b47  ead about the.[G
-00000890: 6976 6520 7570 2047 6974 4875 625d 2868  ive up GitHub](h
-000008a0: 7474 7073 3a2f 2f47 6976 6555 7047 6974  ttps://GiveUpGit
-000008b0: 4875 622e 6f72 6729 2063 616d 7061 6967  Hub.org) campaig
-000008c0: 6e20 6672 6f6d 0a5b 7468 6520 536f 6674  n from.[the Soft
-000008d0: 7761 7265 2046 7265 6564 6f6d 2043 6f6e  ware Freedom Con
-000008e0: 7365 7276 616e 6379 5d28 6874 7470 733a  servancy](https:
-000008f0: 2f2f 7366 636f 6e73 6572 7661 6e63 792e  //sfconservancy.
-00000900: 6f72 6729 2e0a 0a57 6869 6c65 2049 2064  org)...While I d
-00000910: 6f20 6e6f 7420 6164 766f 6361 7465 2066  o not advocate f
-00000920: 6f72 2061 6c6c 2074 6865 2069 7373 7565  or all the issue
-00000930: 7320 6c69 7374 6564 2074 6865 7265 2049  s listed there I
-00000940: 2064 6f20 6e6f 7420 6c69 6b65 2074 6861   do not like tha
-00000950: 740a 6120 636f 6d70 616e 7920 6c69 6b65  t.a company like
-00000960: 204d 6963 726f 736f 6674 206d 6179 2070   Microsoft may p
-00000970: 726f 6669 7420 6672 6f6d 206f 7065 6e20  rofit from open 
-00000980: 736f 7572 6365 2070 726f 6a65 6374 732e  source projects.
-00000990: 0a0a 4920 636f 6e74 696e 7565 2074 6f20  ..I continue to 
-000009a0: 7573 6520 4769 7448 7562 2062 6563 6175  use GitHub becau
-000009b0: 7365 2069 7420 6f66 6665 7273 2074 6865  se it offers the
-000009c0: 2073 6572 7669 6365 7320 4920 6e65 6564   services I need
-000009d0: 2066 6f72 2066 7265 652e 2020 4275 742c   for free.  But,
-000009e0: 2049 2063 6f6e 7469 6e75 650a 746f 206d   I continue.to m
-000009f0: 6f6e 6974 6f72 2074 6865 6972 2074 6572  onitor their ter
-00000a00: 6d73 206f 6620 7365 7276 6963 652e 0a0a  ms of service...
-00000a10: 416e 7920 7573 6520 6f66 2074 6869 7320  Any use of this 
-00000a20: 7072 6f6a 6563 7427 7320 636f 6465 2062  project's code b
-00000a30: 7920 4769 7448 7562 2043 6f70 696c 6f74  y GitHub Copilot
-00000a40: 2c20 7061 7374 206f 7220 7072 6573 656e  , past or presen
-00000a50: 742c 2069 7320 646f 6e65 0a77 6974 686f  t, is done.witho
-00000a60: 7574 206d 7920 7065 726d 6973 7369 6f6e  ut my permission
-00000a70: 2e20 2049 2064 6f20 6e6f 7420 636f 6e73  .  I do not cons
-00000a80: 656e 7420 746f 2047 6974 4875 6227 7320  ent to GitHub's 
-00000a90: 7573 6520 6f66 2074 6869 7320 7072 6f6a  use of this proj
-00000aa0: 6563 7427 730a 636f 6465 2069 6e20 436f  ect's.code in Co
-00000ab0: 7069 6c6f 742e 0a0a 4120 7265 706f 7369  pilot...A reposi
-00000ac0: 746f 7279 206f 776e 6572 206d 6179 206f  tory owner may o
-00000ad0: 7074 206f 7574 206f 6620 436f 7069 6c6f  pt out of Copilo
-00000ae0: 7420 6279 2063 6861 6e67 696e 6720 5365  t by changing Se
-00000af0: 7474 696e 6773 202d 2d3e 2047 6974 4875  ttings --> GitHu
-00000b00: 6220 436f 7069 6c6f 742e 0a0a 4920 6861  b Copilot...I ha
-00000b10: 7665 2064 6f6e 6520 736f 2e0a            ve done so..
+00000030: 3a20 302e 362e 3630 0a53 756d 6d61 7279  : 0.6.60.Summary
+00000040: 3a20 584d 4c20 746f 204f 676c 204f 626a  : XML to Ogl Obj
+00000050: 6563 7420 4d6f 6465 6c0a 486f 6d65 2d70  ect Model.Home-p
+00000060: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
+00000070: 6875 622e 636f 6d2f 6861 7369 6932 3031  hub.com/hasii201
+00000080: 312f 756e 7461 6e67 6c65 7079 7574 0a41  1/untanglepyut.A
+00000090: 7574 686f 722d 656d 6169 6c3a 2048 756d  uthor-email: Hum
+000000a0: 6265 7274 6f2e 412e 5361 6e63 6865 7a2e  berto.A.Sanchez.
+000000b0: 4949 4067 6d61 696c 2e63 6f6d 0a44 6573  II@gmail.com.Des
+000000c0: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+000000d0: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+000000e0: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
+000000f0: 653a 204c 4943 454e 5345 0a0a 3c69 6d67  e: LICENSE..<img
+00000100: 2073 7263 3d22 2e2f 646f 6373 2f61 6770   src="./docs/agp
+00000110: 6c2d 6c69 6365 6e73 652d 7765 622d 6261  l-license-web-ba
+00000120: 6467 652d 7665 7273 696f 6e2d 322d 3235  dge-version-2-25
+00000130: 3678 3438 2e70 6e67 222f 3e0a 0a5b 215b  6x48.png"/>..[![
+00000140: 4369 7263 6c65 4349 5d28 6874 7470 733a  CircleCI](https:
+00000150: 2f2f 646c 2e63 6972 636c 6563 692e 636f  //dl.circleci.co
+00000160: 6d2f 696e 7369 6768 7473 2d73 6e61 7073  m/insights-snaps
+00000170: 686f 742f 6768 2f68 6173 6969 3230 3131  hot/gh/hasii2011
+00000180: 2f75 6e74 616e 676c 6570 7975 742f 6d61  /untanglepyut/ma
+00000190: 7374 6572 2f6d 6169 6e2f 6261 6467 652e  ster/main/badge.
+000001a0: 7376 673f 7769 6e64 6f77 3d33 3064 295d  svg?window=30d)]
+000001b0: 2868 7474 7073 3a2f 2f61 7070 2e63 6972  (https://app.cir
+000001c0: 636c 6563 692e 636f 6d2f 696e 7369 6768  cleci.com/insigh
+000001d0: 7473 2f67 6974 6875 622f 6861 7369 6932  ts/github/hasii2
+000001e0: 3031 312f 756e 7461 6e67 6c65 7079 7574  011/untanglepyut
+000001f0: 2f77 6f72 6b66 6c6f 7773 2f6d 6169 6e2f  /workflows/main/
+00000200: 6f76 6572 7669 6577 3f62 7261 6e63 683d  overview?branch=
+00000210: 6d61 7374 6572 2672 6570 6f72 7469 6e67  master&reporting
+00000220: 2d77 696e 646f 773d 6c61 7374 2d33 302d  -window=last-30-
+00000230: 6461 7973 2669 6e73 6967 6874 732d 736e  days&insights-sn
+00000240: 6170 7368 6f74 3d74 7275 6529 0a0a 5b21  apshot=true)..[!
+00000250: 5b43 6972 636c 6543 495d 2868 7474 7073  [CircleCI](https
+00000260: 3a2f 2f64 6c2e 6369 7263 6c65 6369 2e63  ://dl.circleci.c
+00000270: 6f6d 2f73 7461 7475 732d 6261 6467 652f  om/status-badge/
+00000280: 696d 672f 6768 2f68 6173 6969 3230 3131  img/gh/hasii2011
+00000290: 2f75 6e74 616e 676c 6570 7975 742f 7472  /untanglepyut/tr
+000002a0: 6565 2f6d 6173 7465 722e 7376 673f 7374  ee/master.svg?st
+000002b0: 796c 653d 7368 6965 6c64 295d 2868 7474  yle=shield)](htt
+000002c0: 7073 3a2f 2f64 6c2e 6369 7263 6c65 6369  ps://dl.circleci
+000002d0: 2e63 6f6d 2f73 7461 7475 732d 6261 6467  .com/status-badg
+000002e0: 652f 7265 6469 7265 6374 2f67 682f 6861  e/redirect/gh/ha
+000002f0: 7369 6932 3031 312f 756e 7461 6e67 6c65  sii2011/untangle
+00000300: 7079 7574 2f74 7265 652f 6d61 7374 6572  pyut/tree/master
+00000310: 290a 5b21 5b4d 6169 6e74 656e 616e 6365  ).[![Maintenance
+00000320: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000330: 6965 6c64 732e 696f 2f62 6164 6765 2f4d  ields.io/badge/M
+00000340: 6169 6e74 6169 6e65 6425 3346 2d79 6573  aintained%3F-yes
+00000350: 2d67 7265 656e 2e73 7667 295d 2868 7474  -green.svg)](htt
+00000360: 7073 3a2f 2f47 6974 4875 622e 636f 6d2f  ps://GitHub.com/
+00000370: 4e61 6572 6565 6e2f 5374 7261 7044 6f77  Naereen/StrapDow
+00000380: 6e2e 6a73 2f67 7261 7068 732f 636f 6d6d  n.js/graphs/comm
+00000390: 6974 2d61 6374 6976 6974 7929 0a5b 215b  it-activity).[![
+000003a0: 6d61 634f 535d 2868 7474 7073 3a2f 2f73  macOS](https://s
+000003b0: 7667 7368 6172 652e 636f 6d2f 692f 5a6a  vgshare.com/i/Zj
+000003c0: 502e 7376 6729 5d28 6874 7470 733a 2f2f  P.svg)](https://
+000003d0: 7376 6773 6861 7265 2e63 6f6d 2f69 2f5a  svgshare.com/i/Z
+000003e0: 6a50 2e73 7667 290a 0a5b 215b 666f 7274  jP.svg)..[![fort
+000003f0: 6865 6261 6467 6520 6d61 6465 2d77 6974  hebadge made-wit
+00000400: 682d 7079 7468 6f6e 5d28 6874 7470 3a2f  h-python](http:/
+00000410: 2f46 6f72 5468 6542 6164 6765 2e63 6f6d  /ForTheBadge.com
+00000420: 2f69 6d61 6765 732f 6261 6467 6573 2f6d  /images/badges/m
+00000430: 6164 652d 7769 7468 2d70 7974 686f 6e2e  ade-with-python.
+00000440: 7376 6729 5d28 6874 7470 733a 2f2f 7777  svg)](https://ww
+00000450: 772e 7079 7468 6f6e 2e6f 7267 2f29 0a0a  w.python.org/)..
+00000460: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
+00000470: 696e 7465 6e64 6564 2074 6f20 6265 2075  intended to be u
+00000480: 7365 6420 6279 205b 5079 7574 2050 6c75  sed by [Pyut Plu
+00000490: 6769 6e5d 2868 7474 7073 3a2f 2f67 6974  gin](https://git
+000004a0: 6875 622e 636f 6d2f 6861 7369 6932 3031  hub.com/hasii201
+000004b0: 312f 7079 7574 706c 7567 696e 636f 7265  1/pyutplugincore
+000004c0: 2920 6465 7665 6c6f 7065 7273 2074 6f20  ) developers to 
+000004d0: 636f 6e76 6572 7420 5b50 7975 745d 2868  convert [Pyut](h
+000004e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000004f0: 6d2f 6861 7369 6932 3031 312f 5079 5574  m/hasii2011/PyUt
+00000500: 2920 584d 4c20 6669 6c65 7320 746f 2074  ) XML files to t
+00000510: 6865 205b 4f67 6c20 4d6f 6465 6c5d 2868  he [Ogl Model](h
+00000520: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000530: 6d2f 6861 7369 6932 3031 312f 6f67 6c29  m/hasii2011/ogl)
+00000540: 2063 6c61 7373 6573 2e20 2054 6865 7365   classes.  These
+00000550: 206d 6f64 656c 2063 6c61 7373 6573 2063   model classes c
+00000560: 616e 2074 6865 6e20 6265 2075 7365 6420  an then be used 
+00000570: 6279 2074 6865 2050 7975 7420 5549 2074  by the Pyut UI t
+00000580: 6f20 6469 7370 6c61 7920 6173 2055 4d4c  o display as UML
+00000590: 2044 6961 6772 616d 732e 0a0a 2d2d 2d2d   Diagrams...----
+000005a0: 2d2d 0a0a 5573 6520 6173 2066 6f6c 6c6f  --..Use as follo
+000005b0: 7773 3a0a 0a60 6060 7079 7468 6f6e 0a66  ws:..```python.f
+000005c0: 726f 6d20 756e 7461 6e67 6c65 7079 7574  rom untanglepyut
+000005d0: 2e55 6e54 616e 676c 6572 2069 6d70 6f72  .UnTangler impor
+000005e0: 7420 446f 6375 6d65 6e74 0a66 726f 6d20  t Document.from 
+000005f0: 756e 7461 6e67 6c65 7079 7574 2e55 6e54  untanglepyut.UnT
+00000600: 616e 676c 6572 2069 6d70 6f72 7420 556e  angler import Un
+00000610: 5461 6e67 6c65 720a 0a66 726f 6d20 756e  Tangler..from un
+00000620: 7461 6e67 6c65 7079 7574 2e54 7970 6573  tanglepyut.Types
+00000630: 2069 6d70 6f72 7420 556e 7461 6e67 6c65   import Untangle
+00000640: 644f 676c 436c 6173 7365 730a 6672 6f6d  dOglClasses.from
+00000650: 2075 6e74 616e 676c 6570 7975 742e 5479   untanglepyut.Ty
+00000660: 7065 7320 696d 706f 7274 2055 6e74 616e  pes import Untan
+00000670: 676c 6564 4f67 6c4c 696e 6b73 0a66 726f  gledOglLinks.fro
+00000680: 6d20 756e 7461 6e67 6c65 7079 7574 2e54  m untanglepyut.T
+00000690: 7970 6573 2069 6d70 6f72 7420 556e 7461  ypes import Unta
+000006a0: 6e67 6c65 644f 676c 4e6f 7465 730a 6672  ngledOglNotes.fr
+000006b0: 6f6d 2075 6e74 616e 676c 6570 7975 742e  om untanglepyut.
+000006c0: 5479 7065 7320 696d 706f 7274 2055 6e74  Types import Unt
+000006d0: 616e 676c 6564 4f67 6c54 6578 7473 0a0a  angledOglTexts..
+000006e0: 756e 7461 6e67 6c65 723a 2055 6e54 616e  untangler: UnTan
+000006f0: 676c 6572 203d 2055 6e54 616e 676c 6572  gler = UnTangler
+00000700: 2866 7146 696c 654e 616d 653d 274d 756c  (fqFileName='Mul
+00000710: 7469 446f 6375 6d65 6e74 5072 6f6a 6563  tiDocumentProjec
+00000720: 742e 786d 6c27 290a 0a64 6f63 756d 656e  t.xml')..documen
+00000730: 743a 2044 6f63 756d 656e 7420 3d20 756e  t: Document = un
+00000740: 7461 6e67 6c65 722e 646f 6375 6d65 6e74  tangler.document
+00000750: 735b 2744 6961 6772 616d 2d31 275d 0a0a  s['Diagram-1']..
+00000760: 6f67 6c43 6c61 7373 6573 3a20 556e 7461  oglClasses: Unta
+00000770: 6e67 6c65 644f 676c 436c 6173 7365 7320  ngledOglClasses 
+00000780: 3d20 646f 6375 6d65 6e74 2e6f 676c 436c  = document.oglCl
+00000790: 6173 7365 730a 6f67 6c4c 696e 6b73 3a20  asses.oglLinks: 
+000007a0: 2020 556e 7461 6e67 6c65 644f 676c 4c69    UntangledOglLi
+000007b0: 6e6b 7320 2020 3d20 646f 6375 6d65 6e74  nks   = document
+000007c0: 2e6f 676c 4c69 6e6b 730a 6f67 6c4e 6f74  .oglLinks.oglNot
+000007d0: 6573 3a20 2020 556e 7461 6e67 6c65 644f  es:   UntangledO
+000007e0: 676c 4e6f 7465 7320 2020 3d20 646f 6375  glNotes   = docu
+000007f0: 6d65 6e74 2e6f 676c 4e6f 7465 730a 6f67  ment.oglNotes.og
+00000800: 6c54 6578 7473 3a20 2020 556e 7461 6e67  lTexts:   Untang
+00000810: 6c65 644f 676c 5465 7874 7320 2020 3d20  ledOglTexts   = 
+00000820: 646f 6375 6d65 6e74 2e6f 676c 5465 7874  document.oglText
+00000830: 730a 0a60 6060 0a0a 0a0a 5468 6520 666f  s..```....The fo
+00000840: 6c6c 6f77 696e 6720 6973 2074 6865 2055  llowing is the U
+00000850: 4d4c 2064 6961 6772 616d 2066 6f72 2074  ML diagram for t
+00000860: 6865 2050 7975 7420 556e 7461 6e67 6c65  he Pyut Untangle
+00000870: 720a 0a21 5b55 6e74 616e 676c 6550 7975  r..![UntanglePyu
+00000880: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00000890: 622e 636f 6d2f 6861 7369 6932 3031 312f  b.com/hasii2011/
+000008a0: 756e 7461 6e67 6c65 7079 7574 2f62 6c6f  untanglepyut/blo
+000008b0: 622f 6d61 7374 6572 2f64 6f63 732f 556e  b/master/docs/Un
+000008c0: 7461 6e67 6c65 5079 7574 2e70 6e67 290a  tanglePyut.png).
+000008d0: 0a0a 5f5f 5f0a 0a23 2320 4465 7665 6c6f  ..___..## Develo
+000008e0: 7065 7220 4e6f 7465 730a 5468 6973 2070  per Notes.This p
+000008f0: 726f 6a65 6374 2075 7365 7320 5b62 7569  roject uses [bui
+00000900: 6c64 6c61 636b 6579 5d28 6874 7470 733a  ldlackey](https:
+00000910: 2f2f 6769 7468 7562 2e63 6f6d 2f68 6173  //github.com/has
+00000920: 6969 3230 3131 2f62 7569 6c64 6c61 636b  ii2011/buildlack
+00000930: 6579 2920 666f 7220 6461 7920 746f 2064  ey) for day to d
+00000940: 6179 2064 6576 656c 6f70 6d65 6e74 2062  ay development b
+00000950: 7569 6c64 730a 0a5f 5f5f 0a0a 5772 6974  uilds..___..Writ
+00000960: 7465 6e20 6279 203c 6120 6872 6566 3d22  ten by <a href="
+00000970: 6d61 696c 746f 3a65 6d61 696c 4068 756d  mailto:email@hum
+00000980: 6265 7274 6f2e 612e 7361 6e63 6865 7a2e  berto.a.sanchez.
+00000990: 6969 4067 6d61 696c 2e63 6f6d 3f73 7562  ii@gmail.com?sub
+000009a0: 6a65 6374 3d48 656c 6c6f 2048 756d 6265  ject=Hello Humbe
+000009b0: 7274 6f22 3e48 756d 6265 7274 6f20 412e  rto">Humberto A.
+000009c0: 2053 616e 6368 657a 2049 493c 2f61 3e20   Sanchez II</a> 
+000009d0: 2028 4329 2032 3032 330a 0a23 2320 4e6f   (C) 2023..## No
+000009e0: 7465 0a46 6f72 2061 6c6c 206b 696e 6420  te.For all kind 
+000009f0: 6f66 2070 726f 626c 656d 732c 2072 6571  of problems, req
+00000a00: 7565 7374 732c 2065 6e68 616e 6365 6d65  uests, enhanceme
+00000a10: 6e74 732c 2062 7567 2072 6570 6f72 7473  nts, bug reports
+00000a20: 2c20 6574 632e 2c0a 706c 6561 7365 2064  , etc.,.please d
+00000a30: 726f 7020 6d65 2061 6e20 652d 6d61 696c  rop me an e-mail
+00000a40: 2e0a 0a0a 215b 4875 6d62 6572 746f 2773  ....![Humberto's
+00000a50: 204d 6f64 6966 6965 6420 4c6f 676f 5d28   Modified Logo](
+00000a60: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+00000a70: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00000a80: 6d2f 7769 6b69 2f68 6173 6969 3230 3131  m/wiki/hasii2011
+00000a90: 2f67 6974 746f 646f 6973 7463 6c6f 6e65  /gittodoistclone
+00000aa0: 2f69 6d61 6765 732f 5369 6c6c 7947 6974  /images/SillyGit
+00000ab0: 4875 622e 706e 6729 0a0a 4920 616d 2063  Hub.png)..I am c
+00000ac0: 6f6e 6365 726e 6564 2061 626f 7574 2047  oncerned about G
+00000ad0: 6974 4875 6227 7320 436f 7069 6c6f 7420  itHub's Copilot 
+00000ae0: 7072 6f6a 6563 740a 0a0a 0a49 2075 7267  project....I urg
+00000af0: 6520 796f 7520 746f 2072 6561 6420 6162  e you to read ab
+00000b00: 6f75 7420 7468 650a 5b47 6976 6520 7570  out the.[Give up
+00000b10: 2047 6974 4875 625d 2868 7474 7073 3a2f   GitHub](https:/
+00000b20: 2f47 6976 6555 7047 6974 4875 622e 6f72  /GiveUpGitHub.or
+00000b30: 6729 2063 616d 7061 6967 6e20 6672 6f6d  g) campaign from
+00000b40: 0a5b 7468 6520 536f 6674 7761 7265 2046  .[the Software F
+00000b50: 7265 6564 6f6d 2043 6f6e 7365 7276 616e  reedom Conservan
+00000b60: 6379 5d28 6874 7470 733a 2f2f 7366 636f  cy](https://sfco
+00000b70: 6e73 6572 7661 6e63 792e 6f72 6729 2e0a  nservancy.org)..
+00000b80: 0a57 6869 6c65 2049 2064 6f20 6e6f 7420  .While I do not 
+00000b90: 6164 766f 6361 7465 2066 6f72 2061 6c6c  advocate for all
+00000ba0: 2074 6865 2069 7373 7565 7320 6c69 7374   the issues list
+00000bb0: 6564 2074 6865 7265 2049 2064 6f20 6e6f  ed there I do no
+00000bc0: 7420 6c69 6b65 2074 6861 740a 6120 636f  t like that.a co
+00000bd0: 6d70 616e 7920 6c69 6b65 204d 6963 726f  mpany like Micro
+00000be0: 736f 6674 206d 6179 2070 726f 6669 7420  soft may profit 
+00000bf0: 6672 6f6d 206f 7065 6e20 736f 7572 6365  from open source
+00000c00: 2070 726f 6a65 6374 732e 0a0a 4920 636f   projects...I co
+00000c10: 6e74 696e 7565 2074 6f20 7573 6520 4769  ntinue to use Gi
+00000c20: 7448 7562 2062 6563 6175 7365 2069 7420  tHub because it 
+00000c30: 6f66 6665 7273 2074 6865 2073 6572 7669  offers the servi
+00000c40: 6365 7320 4920 6e65 6564 2066 6f72 2066  ces I need for f
+00000c50: 7265 652e 2020 4275 742c 2049 2063 6f6e  ree.  But, I con
+00000c60: 7469 6e75 650a 746f 206d 6f6e 6974 6f72  tinue.to monitor
+00000c70: 2074 6865 6972 2074 6572 6d73 206f 6620   their terms of 
+00000c80: 7365 7276 6963 652e 0a0a 416e 7920 7573  service...Any us
+00000c90: 6520 6f66 2074 6869 7320 7072 6f6a 6563  e of this projec
+00000ca0: 7427 7320 636f 6465 2062 7920 4769 7448  t's code by GitH
+00000cb0: 7562 2043 6f70 696c 6f74 2c20 7061 7374  ub Copilot, past
+00000cc0: 206f 7220 7072 6573 656e 742c 2069 7320   or present, is 
+00000cd0: 646f 6e65 0a77 6974 686f 7574 206d 7920  done.without my 
+00000ce0: 7065 726d 6973 7369 6f6e 2e20 2049 2064  permission.  I d
+00000cf0: 6f20 6e6f 7420 636f 6e73 656e 7420 746f  o not consent to
+00000d00: 2047 6974 4875 6227 7320 7573 6520 6f66   GitHub's use of
+00000d10: 2074 6869 7320 7072 6f6a 6563 7427 730a   this project's.
+00000d20: 636f 6465 2069 6e20 436f 7069 6c6f 742e  code in Copilot.
+00000d30: 0a0a 4120 7265 706f 7369 746f 7279 206f  ..A repository o
+00000d40: 776e 6572 206d 6179 206f 7074 206f 7574  wner may opt out
+00000d50: 206f 6620 436f 7069 6c6f 7420 6279 2063   of Copilot by c
+00000d60: 6861 6e67 696e 6720 5365 7474 696e 6773  hanging Settings
+00000d70: 202d 2d3e 2047 6974 4875 6220 436f 7069   --> GitHub Copi
+00000d80: 6c6f 742e 0a0a 4920 6861 7665 2064 6f6e  lot...I have don
+00000d90: 6520 736f 2e0a                           e so..
```

