# Comparing `tmp/culendar-0.20230330.tar.gz` & `tmp/culendar-0.20230510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "culendar-0.20230510.tar", max compression
```

## Comparing `culendar-0.20230330.tar` & `culendar-0.20230510.tar`

### file list

```diff
@@ -1,31 +1,18 @@
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 culendar-0.20230330/.pyproject.toml.swp
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 culendar-0.20230330/BUG
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 culendar-0.20230330/HowToAddFunction
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 culendar-0.20230330/HowToGettext
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 culendar-0.20230330/TODO
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 culendar-0.20230330/calDAV_notes
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 culendar-0.20230330/caldav.conf.example
--rw-r--r--   0        0        0   180738 2020-02-02 00:00:00.000000 culendar-0.20230330/classes_No_Name.png
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 culendar-0.20230330/culendar
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 culendar-0.20230330/requirements.txt
--rw-r--r--   0        0        0   345873 2020-02-02 00:00:00.000000 culendar-0.20230330/screenshot0.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/__init__.py
--rwxr-xr-x   0        0        0     5186 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/culendar.py
--rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/calendar.py
--rw-r--r--   0        0        0    17267 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/config.py
--rw-r--r--   0        0        0    30423 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/confscr.py
--rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/culdav.py
--rw-r--r--   0        0        0    48367 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/culendar.py
--rw-r--r--   0        0        0    49621 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/culendar.py.new
--rwxr-xr-x   0        0        0     5146 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/getkey.py
--rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/helpscr.py
--rw-r--r--   0        0        0    10300 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/inputs.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/mouse.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/cul/mouse.py.new
--rw-r--r--   0        0        0    12324 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/locale/fr/LC_MESSAGES/culendar.mo
--rw-r--r--   0        0        0    15680 2020-02-02 00:00:00.000000 culendar-0.20230330/src/culendar/locale/fr/LC_MESSAGES/culendar.pot
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 culendar-0.20230330/.gitignore
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 culendar-0.20230330/LICENSE
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 culendar-0.20230330/README.md
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 culendar-0.20230330/pyproject.toml
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 culendar-0.20230330/PKG-INFO
+-rw-r--r--   0        0        0      483 2022-06-09 19:11:53.344818 culendar-0.20230510/LICENSE
+-rw-r--r--   0        0        0     1064 2023-05-10 20:16:57.398827 culendar-0.20230510/README.md
+-rw-r--r--   0        0        0     5162 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/__init__.py
+-rw-r--r--   0        0        0       25 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/__main__.py
+-rw-r--r--   0        0        0    16732 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/cul/calendar.py
+-rw-r--r--   0        0        0    17232 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/cul/config.py
+-rw-r--r--   0        0        0    30359 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/cul/confscr.py
+-rw-r--r--   0        0        0     9465 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/cul/culdav.py
+-rw-r--r--   0        0        0    48306 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/cul/culendar.py
+-rw-r--r--   0        0        0     5096 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/cul/getkey.py
+-rw-r--r--   0        0        0     8227 2023-05-10 20:19:23.982186 culendar-0.20230510/culendar/cul/helpscr.py
+-rw-r--r--   0        0        0    10258 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/cul/inputs.py
+-rw-r--r--   0        0        0     1374 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/cul/mouse.py
+-rw-r--r--   0        0        0    12328 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/locale/fr/LC_MESSAGES/culendar.mo
+-rw-r--r--   0        0        0    15684 2023-05-09 19:32:57.853686 culendar-0.20230510/culendar/locale/fr/LC_MESSAGES/culendar.pot
+-rw-r--r--   0        0        0     2624 2023-05-10 20:18:46.198469 culendar-0.20230510/pyproject.toml
+-rw-r--r--   0        0        0   345873 2022-06-09 19:11:53.348818 culendar-0.20230510/screenshot0.png
+-rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 culendar-0.20230510/PKG-INFO
```

### Comparing `culendar-0.20230330/screenshot0.png` & `culendar-0.20230510/screenshot0.png`

 * *Files identical despite different names*

### Comparing `culendar-0.20230330/src/culendar/culendar.py` & `culendar-0.20230510/culendar/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-#! /usr/bin/env python3
-# coding: utf-8
+#!/usr/bin/env python3
 import curses
 import datetime
-import icalendar
-import sys
-from .cul import config, culendar, calendar, helpscr, confscr, culdav, getkey
-from .cul import mouse
+
+from .cul import (
+    calendar,
+    config,
+    confscr,
+    culdav,
+    culendar,
+    getkey,
+    helpscr,
+    mouse,
+)
 
 
 def main(stdscr):
     # configialize ncurses and get conf
     conf = config.Config()
 
     # the current day
@@ -24,15 +30,15 @@
     cdav = culdav.Cdav(conf.caldav, stdscr, conf)
 
     # include first drawing
     cul = culendar.Culendar(stdscr, conf, day, cal, cdav, todo)
 
     # main loop
     key = ""
-    while not(key in conf.keys['quit']):
+    while key not in conf.keys['quit']:
         key = getkey.getkey(cul.screen, conf.debug)
 
         if key == 'KEY_RESIZE':
             cul.update()
 
         # repeat action at least 1, or the entered count value
         repetitions = max(1, cul.count)
```

### Comparing `culendar-0.20230330/src/culendar/cul/calendar.py` & `culendar-0.20230510/culendar/cul/calendar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-#! /usr/bin/env python3
-# coding: utf-8
-import icalendar
 import datetime
-from os import path, rename
+from os import (
+    path,
+    rename,
+)
 
+import icalendar
 
-########################################################################
-# Event class
-########################################################################
 
 class Event:
+    """
+    Event class
+    """
+
     def __init__(self, date, duration, summary, place="", tag=0,
                  url=None, caldav=None, colour=None):
         self._date = date          # datetime.datetime()
         self._duration = duration  # seconds
         self._summary = summary.strip()   # text
         self._place = place.strip()       # text
         self._tag = tag
@@ -189,19 +191,18 @@
         self.hlines = range(first_col, first_col + e_width)
 
         # too many events or too small terminal
         if len(self.hlines) < 1:
             self.hlines = (cul.lines[0][col]+1, width)
 
 
-########################################################################
-# Agenda class
-########################################################################
-
 class Agenda:
+    """
+    Agenda class
+    """
     def __init__(self):
         self._events = []
 
     def add_event(self, e):
         self._events.append(e)
 
     def del_event(self, e):
@@ -228,15 +229,15 @@
 
     for e in cal.events + caldav.calweek.events:
         # if the right day, add the event
         if e.date.toordinal() == day.toordinal():
             calday.add_event(e)
 
     calday.sort()
-    return(calday)
+    return calday
 
 
 def extract_week(cal, caldav, day, cul, autosync=1):
     # create a list of subcals for each day of the week
     calweek = []
     for i in range(7):
         calweek.append(Agenda())
```

### Comparing `culendar-0.20230330/src/culendar/cul/config.py` & `culendar-0.20230510/culendar/cul/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,1080 +1,1077 @@
-00000000: 2321 202f 7573 722f 6269 6e2f 656e 7620  #! /usr/bin/env 
-00000010: 7079 7468 6f6e 330a 2320 636f 6469 6e67  python3.# coding
-00000020: 3a20 7574 662d 380a 0a69 6d70 6f72 7420  : utf-8..import 
-00000030: 6375 7273 6573 0a69 6d70 6f72 7420 6c6f  curses.import lo
-00000040: 6361 6c65 0a69 6d70 6f72 7420 6765 7474  cale.import gett
-00000050: 6578 740a 6672 6f6d 206f 7320 696d 706f  ext.from os impo
-00000060: 7274 2065 6e76 6972 6f6e 2c20 6765 7465  rt environ, gete
-00000070: 6e76 2c20 7061 7468 2c20 6d6b 6469 722c  nv, path, mkdir,
-00000080: 2072 656e 616d 650a 0a0a 636c 6173 7320   rename...class 
-00000090: 436f 6e66 6967 3a0a 2020 2020 6465 6620  Config:.    def 
-000000a0: 5f5f 696e 6974 5f5f 2873 656c 6629 3a0a  __init__(self):.
-000000b0: 2020 2020 2020 2020 2320 4d6f 7573 6520          # Mouse 
-000000c0: 6163 7469 7661 7469 6f6e 0a20 2020 2020  activation.     
-000000d0: 2020 2073 656c 662e 5f6d 6d61 736b 203d     self._mmask =
-000000e0: 2028 6375 7273 6573 2e42 5554 544f 4e31   (curses.BUTTON1
-000000f0: 5f43 4c49 434b 4544 202b 2063 7572 7365  _CLICKED + curse
-00000100: 732e 4255 5454 4f4e 315f 444f 5542 4c45  s.BUTTON1_DOUBLE
-00000110: 5f43 4c49 434b 4544 0a20 2020 2020 2020  _CLICKED.       
-00000120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000130: 2b20 6375 7273 6573 2e42 5554 544f 4e31  + curses.BUTTON1
-00000140: 5f54 5249 504c 455f 434c 4943 4b45 4429  _TRIPLE_CLICKED)
-00000150: 0a20 2020 2020 2020 2023 2069 6e76 6973  .        # invis
-00000160: 6962 6c65 2063 7572 736f 720a 2020 2020  ible cursor.    
-00000170: 2020 2020 6375 7273 6573 2e63 7572 735f      curses.curs_
-00000180: 7365 7428 3029 0a20 2020 2020 2020 2023  set(0).        #
-00000190: 2061 6c6c 6f77 2074 7261 6e73 7061 7265   allow transpare
-000001a0: 6e63 790a 2020 2020 2020 2020 6375 7273  ncy.        curs
-000001b0: 6573 2e75 7365 5f64 6566 6175 6c74 5f63  es.use_default_c
-000001c0: 6f6c 6f72 7328 290a 2020 2020 2020 2020  olors().        
-000001d0: 2320 7573 6520 7468 6520 6c6f 6361 6c65  # use the locale
-000001e0: 210a 2020 2020 2020 2020 6c6f 6361 6c65  !.        locale
-000001f0: 2e73 6574 6c6f 6361 6c65 286c 6f63 616c  .setlocale(local
-00000200: 652e 4c43 5f41 4c4c 2c20 2727 290a 2020  e.LC_ALL, '').  
-00000210: 2020 2020 2020 6765 7474 6578 742e 696e        gettext.in
-00000220: 7374 616c 6c28 2263 756c 656e 6461 7222  stall("culendar"
-00000230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000240: 2020 2020 2020 2020 2020 7061 7468 2e64            path.d
-00000250: 6972 6e61 6d65 2870 6174 682e 7265 616c  irname(path.real
-00000260: 7061 7468 285f 5f66 696c 655f 5f29 292b  path(__file__))+
-00000270: 222f 2e2e 2f6c 6f63 616c 6522 290a 0a20  "/../locale").. 
-00000280: 2020 2020 2020 2023 2063 7265 6174 6520         # create 
-00000290: 6465 6661 756c 7420 7661 6c75 6573 0a20  default values. 
-000002a0: 2020 2020 2020 2073 656c 662e 5f68 6d69         self._hmi
-000002b0: 6e20 3d20 3720 2020 2320 3720 616d 0a20  n = 7   # 7 am. 
-000002c0: 2020 2020 2020 2073 656c 662e 5f68 6d61         self._hma
-000002d0: 7820 3d20 3230 2020 2320 3820 706d 0a20  x = 20  # 8 pm. 
-000002e0: 2020 2020 2020 2073 656c 662e 5f57 4520         self._WE 
-000002f0: 3d20 626f 6f6c 2831 2920 2023 2073 686f  = bool(1)  # sho
-00000300: 7720 7765 656b 2d65 6e64 730a 2020 2020  w week-ends.    
-00000310: 2020 2020 7365 6c66 2e5f 746f 646f 203d      self._todo =
-00000320: 2062 6f6f 6c28 3029 2020 2020 2020 2320   bool(0)      # 
-00000330: 646f 6573 6e27 7420 7368 6f77 2074 6f64  doesn't show tod
-00000340: 6f20 6c69 7374 0a20 2020 2020 2020 2073  o list.        s
-00000350: 656c 662e 5f74 6f64 6f77 6964 7468 203d  elf._todowidth =
-00000360: 2030 2e32 2020 2020 2023 2064 6566 6175   0.2     # defau
-00000370: 6c74 7320 3230 2520 7769 6474 680a 2020  lts 20% width.  
-00000380: 2020 2020 2020 7365 6c66 2e5f 6175 746f        self._auto
-00000390: 7361 7665 203d 2062 6f6f 6c28 3129 2020  save = bool(1)  
-000003a0: 2320 6465 6661 756c 7473 2074 6f20 6265  # defaults to be
-000003b0: 206c 6573 7320 756e 7573 7561 6c0a 2020   less unusual.  
-000003c0: 2020 2020 2020 7365 6c66 2e5f 636f 6c6f        self._colo
-000003d0: 7572 7365 7420 3d20 3020 2020 2020 2020  urset = 0       
-000003e0: 2320 6465 6661 756c 7473 2074 6f20 666c  # defaults to fl
-000003f0: 6173 6879 0a20 2020 2020 2020 2073 656c  ashy.        sel
-00000400: 662e 5f63 616c 6461 7620 3d20 5b5d 2020  f._caldav = []  
-00000410: 2020 2020 2020 2023 2065 6d70 7479 206c         # empty l
-00000420: 6973 7420 6f66 2063 616c 6461 7673 0a20  ist of caldavs. 
-00000430: 2020 2020 2020 2073 656c 662e 5f61 7574         self._aut
-00000440: 6f73 796e 6320 3d20 4661 6c73 6520 2020  osync = False   
-00000450: 2023 2061 7574 6f75 7064 6174 6520 616c   # autoupdate al
-00000460: 6c20 6361 6c64 6176 7320 7768 656e 2063  l caldavs when c
-00000470: 6861 6e67 696e 6720 6461 790a 2020 2020  hanging day.    
-00000480: 2020 2020 7365 6c66 2e5f 6d6f 7573 6520      self._mouse 
-00000490: 3d20 4661 6c73 6520 2020 2020 2020 2320  = False       # 
-000004a0: 6469 7361 626c 6520 6d6f 7573 650a 2020  disable mouse.  
-000004b0: 2020 2020 2020 6375 7273 6573 2e6d 6f75        curses.mou
-000004c0: 7365 6d61 736b 2830 290a 2020 2020 2020  semask(0).      
-000004d0: 2020 7365 6c66 2e5f 6465 6275 6720 3d20    self._debug = 
-000004e0: 626f 6f6c 2830 2920 2020 2020 2320 796f  bool(0)     # yo
-000004f0: 7520 7761 6e74 2074 6f20 7365 6520 6465  u want to see de
-00000500: 6164 2064 7563 6b73 0a0a 2020 2020 2020  ad ducks..      
-00000510: 2020 7365 6c66 2e63 6865 636b 6469 7228    self.checkdir(
-00000520: 2920 2023 2064 6566 696e 6520 7061 7468  )  # define path
-00000530: 730a 2020 2020 2020 2020 7365 6c66 2e5f  s.        self._
-00000540: 636f 6e66 6967 6669 6c65 203d 2073 656c  configfile = sel
-00000550: 662e 5f63 6f6e 6669 6770 6174 6820 2b20  f._configpath + 
-00000560: 272f 6375 6c65 6e64 6172 2e63 6f6e 6627  '/culendar.conf'
-00000570: 0a20 2020 2020 2020 2073 656c 662e 5f6b  .        self._k
-00000580: 6579 7366 696c 6520 3d20 7365 6c66 2e5f  eysfile = self._
-00000590: 636f 6e66 6967 7061 7468 202b 2027 2f6b  configpath + '/k
-000005a0: 6579 732e 636f 6e66 270a 2020 2020 2020  eys.conf'.      
-000005b0: 2020 7365 6c66 2e5f 636f 6c6f 7572 7366    self._coloursf
-000005c0: 696c 6520 3d20 7365 6c66 2e5f 636f 6e66  ile = self._conf
-000005d0: 6967 7061 7468 202b 2027 2f63 6f6c 6f75  igpath + '/colou
-000005e0: 7273 2e63 6f6e 6627 0a20 2020 2020 2020  rs.conf'.       
-000005f0: 2073 656c 662e 5f63 6174 6567 6f72 6965   self._categorie
-00000600: 7366 696c 6520 3d20 7365 6c66 2e5f 636f  sfile = self._co
-00000610: 6e66 6967 7061 7468 202b 2027 2f63 6174  nfigpath + '/cat
-00000620: 6567 6f72 6965 732e 636f 6e66 270a 2020  egories.conf'.  
-00000630: 2020 2020 2020 7365 6c66 2e5f 6361 6c64        self._cald
-00000640: 6176 6669 6c65 203d 2073 656c 662e 5f63  avfile = self._c
-00000650: 6f6e 6669 6770 6174 6820 2b20 272f 6361  onfigpath + '/ca
-00000660: 6c64 6176 2e63 6f6e 6627 0a20 2020 2020  ldav.conf'.     
-00000670: 2020 2073 656c 662e 5f64 6174 6166 696c     self._datafil
-00000680: 6520 3d20 7365 6c66 2e5f 6461 7461 7061  e = self._datapa
-00000690: 7468 202b 2027 2f61 7074 7327 0a20 2020  th + '/apts'.   
-000006a0: 2020 2020 2073 656c 662e 5f74 6f64 6f66       self._todof
-000006b0: 696c 6520 3d20 7365 6c66 2e5f 6461 7461  ile = self._data
-000006c0: 7061 7468 202b 2027 2f74 6f64 6f27 0a20  path + '/todo'. 
-000006d0: 2020 2020 2020 2023 2063 7265 6174 6520         # create 
-000006e0: 626c 616e 6b73 206f 6e65 2069 6620 6e6f  blanks one if no
-000006f0: 7420 6578 6973 7469 6e67 0a20 2020 2020  t existing.     
-00000700: 2020 2069 6620 6e6f 7428 7061 7468 2e65     if not(path.e
-00000710: 7869 7374 7328 7365 6c66 2e5f 6461 7461  xists(self._data
-00000720: 6669 6c65 2929 3a0a 2020 2020 2020 2020  file)):.        
-00000730: 2020 2020 7769 7468 206f 7065 6e28 7365      with open(se
-00000740: 6c66 2e5f 6461 7461 6669 6c65 2c20 2277  lf._datafile, "w
-00000750: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
-00000760: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00000770: 2822 2229 0a20 2020 2020 2020 2069 6620  ("").        if 
-00000780: 6e6f 7428 7061 7468 2e65 7869 7374 7328  not(path.exists(
-00000790: 7365 6c66 2e5f 746f 646f 6669 6c65 2929  self._todofile))
-000007a0: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-000007b0: 7468 206f 7065 6e28 7365 6c66 2e5f 746f  th open(self._to
-000007c0: 646f 6669 6c65 2c20 2277 2229 2061 7320  dofile, "w") as 
-000007d0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-000007e0: 2020 2066 2e77 7269 7465 2822 2229 0a0a     f.write("")..
-000007f0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-00000800: 6463 6f6e 6628 2920 2020 2020 2020 2020  dconf()         
-00000810: 2320 6f76 6572 7772 6974 6573 2064 6566  # overwrites def
-00000820: 6175 6c74 2076 616c 7565 730a 2020 2020  ault values.    
-00000830: 2020 2020 7365 6c66 2e72 6561 646b 6579      self.readkey
-00000840: 7328 2920 2020 2020 2020 2020 2320 6465  s()         # de
-00000850: 6669 6e65 7320 7365 6c66 2e5f 6b65 7973  fines self._keys
-00000860: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00000870: 6164 636f 6c6f 7572 7328 2920 2020 2020  adcolours()     
-00000880: 2023 2064 6566 696e 6573 2073 656c 662e   # defines self.
-00000890: 5f63 6f6c 6f75 7273 5f69 6478 0a20 2020  _colours_idx.   
-000008a0: 2020 2020 2073 656c 662e 7365 7463 6f6c       self.setcol
-000008b0: 6f75 7273 2829 2020 2020 2020 2023 2064  ours()       # d
-000008c0: 6566 696e 6573 2073 656c 662e 5f63 6f6c  efines self._col
-000008d0: 6f75 7273 0a20 2020 2020 2020 2073 656c  ours.        sel
-000008e0: 662e 7265 6164 6361 7465 676f 7269 6573  f.readcategories
-000008f0: 2829 2020 2023 2064 6566 696e 6573 2073  ()   # defines s
-00000900: 656c 662e 5f63 6174 6567 6f72 6965 730a  elf._categories.
-00000910: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-00000920: 6463 616c 6461 7628 2920 2020 2020 2020  dcaldav()       
-00000930: 2320 6765 7420 7468 6520 6361 6c64 6176  # get the caldav
-00000940: 7320 636f 6e66 6967 7572 6174 696f 6e73  s configurations
-00000950: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00000960: 2020 2020 6465 6620 686d 696e 2873 656c      def hmin(sel
-00000970: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00000980: 726e 2073 656c 662e 5f68 6d69 6e0a 0a20  rn self._hmin.. 
-00000990: 2020 2040 686d 696e 2e73 6574 7465 720a     @hmin.setter.
-000009a0: 2020 2020 6465 6620 686d 696e 2873 656c      def hmin(sel
-000009b0: 662c 2068 6d69 6e29 3a0a 2020 2020 2020  f, hmin):.      
-000009c0: 2020 6966 2068 6d69 6e20 3e3d 2073 656c    if hmin >= sel
-000009d0: 662e 5f68 6d61 783a 0a20 2020 2020 2020  f._hmax:.       
-000009e0: 2020 2020 2073 656c 662e 5f68 6d69 6e20       self._hmin 
-000009f0: 3d20 7365 6c66 2e5f 686d 6178 2d31 0a20  = self._hmax-1. 
-00000a00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00000a10: 2020 2020 2020 2020 2073 656c 662e 5f68           self._h
-00000a20: 6d69 6e20 3d20 6d61 7828 302c 2068 6d69  min = max(0, hmi
-00000a30: 6e29 0a0a 2020 2020 4070 726f 7065 7274  n)..    @propert
-00000a40: 790a 2020 2020 6465 6620 686d 6178 2873  y.    def hmax(s
-00000a50: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-00000a60: 7475 726e 2073 656c 662e 5f68 6d61 780a  turn self._hmax.
-00000a70: 0a20 2020 2040 686d 6178 2e73 6574 7465  .    @hmax.sette
-00000a80: 720a 2020 2020 6465 6620 686d 6178 2873  r.    def hmax(s
-00000a90: 656c 662c 2068 6d61 7829 3a0a 2020 2020  elf, hmax):.    
-00000aa0: 2020 2020 6966 2068 6d61 7820 3c3d 2073      if hmax <= s
-00000ab0: 656c 662e 5f68 6d69 6e3a 0a20 2020 2020  elf._hmin:.     
-00000ac0: 2020 2020 2020 2073 656c 662e 5f68 6d61         self._hma
-00000ad0: 7820 3d20 7365 6c66 2e5f 686d 696e 2b31  x = self._hmin+1
-00000ae0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00000af0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000b00: 5f68 6d61 7820 3d20 6d69 6e28 3234 2c20  _hmax = min(24, 
-00000b10: 686d 6178 290a 0a20 2020 2040 7072 6f70  hmax)..    @prop
-00000b20: 6572 7479 0a20 2020 2064 6566 2057 4528  erty.    def WE(
-00000b30: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00000b40: 6574 7572 6e20 7365 6c66 2e5f 5745 0a0a  eturn self._WE..
-00000b50: 2020 2020 4057 452e 7365 7474 6572 0a20      @WE.setter. 
-00000b60: 2020 2064 6566 2057 4528 7365 6c66 2c20     def WE(self, 
-00000b70: 5745 293a 0a20 2020 2020 2020 2073 656c  WE):.        sel
-00000b80: 662e 5f57 4520 3d20 5745 0a0a 2020 2020  f._WE = WE..    
-00000b90: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00000ba0: 6620 746f 646f 2873 656c 6629 3a0a 2020  f todo(self):.  
-00000bb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00000bc0: 662e 5f74 6f64 6f0a 0a20 2020 2040 746f  f._todo..    @to
-00000bd0: 646f 2e73 6574 7465 720a 2020 2020 6465  do.setter.    de
-00000be0: 6620 746f 646f 2873 656c 662c 2054 293a  f todo(self, T):
-00000bf0: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
-00000c00: 6f64 6f20 3d20 540a 0a20 2020 2040 7072  odo = T..    @pr
-00000c10: 6f70 6572 7479 0a20 2020 2064 6566 2074  operty.    def t
-00000c20: 6f64 6f77 6964 7468 2873 656c 6629 3a0a  odowidth(self):.
-00000c30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000c40: 656c 662e 5f74 6f64 6f77 6964 7468 0a0a  elf._todowidth..
-00000c50: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00000c60: 2020 6465 6620 6175 746f 7361 7665 2873    def autosave(s
-00000c70: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-00000c80: 7475 726e 2073 656c 662e 5f61 7574 6f73  turn self._autos
-00000c90: 6176 650a 0a20 2020 2040 6175 746f 7361  ave..    @autosa
-00000ca0: 7665 2e73 6574 7465 720a 2020 2020 6465  ve.setter.    de
-00000cb0: 6620 6175 746f 7361 7665 2873 656c 662c  f autosave(self,
-00000cc0: 2061 7574 6f73 6176 6529 3a0a 2020 2020   autosave):.    
-00000cd0: 2020 2020 7365 6c66 2e5f 6175 746f 7361      self._autosa
-00000ce0: 7665 203d 2061 7574 6f73 6176 650a 0a20  ve = autosave.. 
-00000cf0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00000d00: 2064 6566 206b 6579 7328 7365 6c66 293a   def keys(self):
-00000d10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000d20: 7365 6c66 2e5f 6b65 7973 0a0a 2020 2020  self._keys..    
-00000d30: 406b 6579 732e 7365 7474 6572 0a20 2020  @keys.setter.   
-00000d40: 2064 6566 206b 6579 7328 7365 6c66 2c20   def keys(self, 
-00000d50: 6b65 7973 293a 0a20 2020 2020 2020 2073  keys):.        s
-00000d60: 656c 662e 5f6b 6579 7320 3d20 6b65 7973  elf._keys = keys
-00000d70: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-00000d80: 2020 2020 6465 6620 6461 7461 6669 6c65      def datafile
-00000d90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00000da0: 7265 7475 726e 2073 656c 662e 5f64 6174  return self._dat
-00000db0: 6166 696c 650a 0a20 2020 2040 7072 6f70  afile..    @prop
-00000dc0: 6572 7479 0a20 2020 2064 6566 2074 6f64  erty.    def tod
-00000dd0: 6f66 696c 6528 7365 6c66 293a 0a20 2020  ofile(self):.   
-00000de0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000df0: 2e5f 746f 646f 6669 6c65 0a0a 2020 2020  ._todofile..    
-00000e00: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00000e10: 6620 636f 6c6f 7572 7365 7428 7365 6c66  f colourset(self
-00000e20: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00000e30: 6e20 7365 6c66 2e5f 636f 6c6f 7572 7365  n self._colourse
-00000e40: 740a 0a20 2020 2040 636f 6c6f 7572 7365  t..    @colourse
-00000e50: 742e 7365 7474 6572 0a20 2020 2064 6566  t.setter.    def
-00000e60: 2063 6f6c 6f75 7273 6574 2873 656c 662c   colourset(self,
-00000e70: 2063 7329 3a0a 2020 2020 2020 2020 7365   cs):.        se
-00000e80: 6c66 2e5f 636f 6c6f 7572 7365 7420 3d20  lf._colourset = 
-00000e90: 6373 0a0a 2020 2020 4070 726f 7065 7274  cs..    @propert
-00000ea0: 790a 2020 2020 6465 6620 636f 6c6f 7572  y.    def colour
-00000eb0: 735f 6964 7828 7365 6c66 293a 0a20 2020  s_idx(self):.   
-00000ec0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000ed0: 2e5f 636f 6c6f 7572 735f 6964 780a 0a20  ._colours_idx.. 
-00000ee0: 2020 2040 636f 6c6f 7572 735f 6964 782e     @colours_idx.
-00000ef0: 7365 7474 6572 0a20 2020 2064 6566 2063  setter.    def c
-00000f00: 6f6c 6f75 7273 5f69 6478 2873 656c 662c  olours_idx(self,
-00000f10: 2069 6478 293a 0a20 2020 2020 2020 2073   idx):.        s
-00000f20: 656c 662e 5f63 6f6c 6f75 7273 5f69 6478  elf._colours_idx
-00000f30: 203d 2069 6478 0a0a 2020 2020 4070 726f   = idx..    @pro
-00000f40: 7065 7274 790a 2020 2020 6465 6620 636f  perty.    def co
-00000f50: 6c6f 7572 7328 7365 6c66 293a 0a20 2020  lours(self):.   
-00000f60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000f70: 2e5f 636f 6c6f 7572 730a 0a20 2020 2040  ._colours..    @
-00000f80: 636f 6c6f 7572 732e 7365 7474 6572 0a20  colours.setter. 
-00000f90: 2020 2064 6566 2063 6f6c 6f75 7273 2873     def colours(s
-00000fa0: 656c 662c 2063 6f6c 6f75 7273 293a 0a20  elf, colours):. 
-00000fb0: 2020 2020 2020 2073 656c 662e 5f63 6f6c         self._col
-00000fc0: 6f75 7273 203d 2063 6f6c 6f75 7273 0a0a  ours = colours..
-00000fd0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00000fe0: 2020 6465 6620 6361 7465 676f 7269 6573    def categories
-00000ff0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00001000: 7265 7475 726e 2073 656c 662e 5f63 6174  return self._cat
-00001010: 6567 6f72 6965 730a 0a20 2020 2040 6361  egories..    @ca
-00001020: 7465 676f 7269 6573 2e73 6574 7465 720a  tegories.setter.
-00001030: 2020 2020 6465 6620 6361 7465 676f 7269      def categori
-00001040: 6573 2873 656c 662c 2063 6174 6567 6f72  es(self, categor
-00001050: 6965 7329 3a0a 2020 2020 2020 2020 7365  ies):.        se
-00001060: 6c66 2e5f 6361 7465 676f 7269 6573 203d  lf._categories =
-00001070: 2063 6174 6567 6f72 6965 730a 0a20 2020   categories..   
-00001080: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00001090: 6566 2063 616c 6461 7628 7365 6c66 293a  ef caldav(self):
-000010a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000010b0: 7365 6c66 2e5f 6361 6c64 6176 0a0a 2020  self._caldav..  
-000010c0: 2020 4063 616c 6461 762e 7365 7474 6572    @caldav.setter
-000010d0: 0a20 2020 2064 6566 2063 616c 6461 7628  .    def caldav(
-000010e0: 7365 6c66 2c20 6361 6c64 6176 293a 0a20  self, caldav):. 
-000010f0: 2020 2020 2020 2073 656c 662e 5f63 616c         self._cal
-00001100: 6461 7620 3d20 6361 6c64 6176 0a0a 2020  dav = caldav..  
-00001110: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00001120: 6465 6620 6175 746f 7379 6e63 2873 656c  def autosync(sel
-00001130: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00001140: 726e 2073 656c 662e 5f61 7574 6f73 796e  rn self._autosyn
-00001150: 630a 0a20 2020 2040 6175 746f 7379 6e63  c..    @autosync
-00001160: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00001170: 6175 746f 7379 6e63 2873 656c 662c 2061  autosync(self, a
-00001180: 7574 6f73 796e 6329 3a0a 2020 2020 2020  utosync):.      
-00001190: 2020 7365 6c66 2e5f 6175 746f 7379 6e63    self._autosync
-000011a0: 203d 2061 7574 6f73 796e 630a 0a20 2020   = autosync..   
-000011b0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000011c0: 6566 206d 6f75 7365 2873 656c 6629 3a0a  ef mouse(self):.
-000011d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000011e0: 656c 662e 5f6d 6f75 7365 0a0a 2020 2020  elf._mouse..    
-000011f0: 406d 6f75 7365 2e73 6574 7465 720a 2020  @mouse.setter.  
-00001200: 2020 6465 6620 6d6f 7573 6528 7365 6c66    def mouse(self
-00001210: 2c20 6d6f 7573 6529 3a0a 2020 2020 2020  , mouse):.      
-00001220: 2020 7365 6c66 2e5f 6d6f 7573 6520 3d20    self._mouse = 
-00001230: 6d6f 7573 650a 2020 2020 2020 2020 6966  mouse.        if
-00001240: 206d 6f75 7365 3a0a 2020 2020 2020 2020   mouse:.        
-00001250: 2020 2020 6375 7273 6573 2e6d 6f75 7365      curses.mouse
-00001260: 6d61 736b 2873 656c 662e 5f6d 6d61 736b  mask(self._mmask
-00001270: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00001280: 2020 2020 2020 2020 2020 2020 6375 7273              curs
-00001290: 6573 2e6d 6f75 7365 6d61 736b 2830 290a  es.mousemask(0).
-000012a0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-000012b0: 2020 2064 6566 2064 6562 7567 2873 656c     def debug(sel
-000012c0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-000012d0: 726e 2073 656c 662e 5f64 6562 7567 0a0a  rn self._debug..
-000012e0: 2020 2020 6465 6620 6368 6563 6b64 6972      def checkdir
-000012f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00001300: 2320 636f 6e66 6967 7572 6174 696f 6e20  # configuration 
-00001310: 7374 7566 660a 2020 2020 2020 2020 6966  stuff.        if
-00001320: 2027 5844 475f 434f 4e46 4947 5f48 4f4d   'XDG_CONFIG_HOM
-00001330: 4527 2069 6e20 656e 7669 726f 6e3a 0a20  E' in environ:. 
-00001340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001350: 5f63 6f6e 6669 6770 6174 6820 3d20 6765  _configpath = ge
-00001360: 7465 6e76 2827 5844 475f 4441 5441 5f48  tenv('XDG_DATA_H
-00001370: 4f4d 4527 290a 2020 2020 2020 2020 656c  OME').        el
-00001380: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00001390: 7365 6c66 2e5f 636f 6e66 6967 7061 7468  self._configpath
-000013a0: 203d 2067 6574 656e 7628 2748 4f4d 4527   = getenv('HOME'
-000013b0: 292b 272f 2e63 6f6e 6669 672f 6375 6c65  )+'/.config/cule
-000013c0: 6e64 6172 270a 0a20 2020 2020 2020 2069  ndar'..        i
-000013d0: 6620 6e6f 7428 7061 7468 2e65 7869 7374  f not(path.exist
-000013e0: 7328 7365 6c66 2e5f 636f 6e66 6967 7061  s(self._configpa
-000013f0: 7468 2929 3a0a 2020 2020 2020 2020 2020  th)):.          
-00001400: 2020 2320 696d 706c 6963 6974 6c79 2073    # implicitly s
-00001410: 7570 706f 7365 2074 6861 7420 2448 4f4d  uppose that $HOM
-00001420: 452f 2e63 6f6e 6669 6720 616c 7265 6164  E/.config alread
-00001430: 7920 6578 6973 7473 0a20 2020 2020 2020  y exists.       
-00001440: 2020 2020 206d 6b64 6972 2873 656c 662e       mkdir(self.
-00001450: 5f63 6f6e 6669 6770 6174 6829 0a0a 2020  _configpath)..  
-00001460: 2020 2020 2020 2320 6461 7461 2073 7475        # data stu
-00001470: 6666 0a20 2020 2020 2020 2069 6620 2758  ff.        if 'X
-00001480: 4447 5f44 4154 415f 484f 4d45 2720 696e  DG_DATA_HOME' in
-00001490: 2065 6e76 6972 6f6e 3a0a 2020 2020 2020   environ:.      
-000014a0: 2020 2020 2020 7365 6c66 2e5f 6461 7461        self._data
-000014b0: 7061 7468 203d 2067 6574 656e 7628 2758  path = getenv('X
-000014c0: 4447 5f44 4154 415f 484f 4d45 2729 0a20  DG_DATA_HOME'). 
-000014d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000014e0: 2020 2020 2020 2020 2073 656c 662e 5f64           self._d
-000014f0: 6174 6170 6174 6820 3d20 6765 7465 6e76  atapath = getenv
-00001500: 2827 484f 4d45 2729 2b27 2f2e 6c6f 6361  ('HOME')+'/.loca
-00001510: 6c2f 7368 6172 652f 6375 6c65 6e64 6172  l/share/culendar
-00001520: 270a 0a20 2020 2020 2020 2069 6620 6e6f  '..        if no
-00001530: 7428 7061 7468 2e65 7869 7374 7328 7365  t(path.exists(se
-00001540: 6c66 2e5f 6461 7461 7061 7468 2929 3a0a  lf._datapath)):.
-00001550: 2020 2020 2020 2020 2020 2020 2320 696d              # im
-00001560: 706c 6963 6974 6c79 2073 7570 706f 7365  plicitly suppose
-00001570: 2074 6861 7420 2448 4f4d 452f 2e6c 6f63   that $HOME/.loc
-00001580: 616c 2f73 6861 7265 2061 6c72 6561 6479  al/share already
-00001590: 2065 7869 7374 730a 2020 2020 2020 2020   exists.        
-000015a0: 2020 2020 6d6b 6469 7228 7365 6c66 2e5f      mkdir(self._
-000015b0: 6461 7461 7061 7468 290a 0a20 2020 2064  datapath)..    d
-000015c0: 6566 2072 6561 6463 6f6e 6628 7365 6c66  ef readconf(self
-000015d0: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
-000015e0: 7428 7061 7468 2e65 7869 7374 7328 7365  t(path.exists(se
-000015f0: 6c66 2e5f 636f 6e66 6967 6669 6c65 2929  lf._configfile))
-00001600: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00001610: 7772 6974 6520 7468 6520 6465 6661 756c  write the defaul
-00001620: 7420 636f 6e66 0a20 2020 2020 2020 2020  t conf.         
-00001630: 2020 2073 656c 662e 7772 6974 6563 6f6e     self.writecon
-00001640: 6628 290a 2020 2020 2020 2020 656c 7365  f().        else
-00001650: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-00001660: 7468 206f 7065 6e28 7365 6c66 2e5f 636f  th open(self._co
-00001670: 6e66 6967 6669 6c65 2920 6173 2066 3a0a  nfigfile) as f:.
+00000000: 696d 706f 7274 2063 7572 7365 730a 696d  import curses.im
+00000010: 706f 7274 2067 6574 7465 7874 0a69 6d70  port gettext.imp
+00000020: 6f72 7420 6c6f 6361 6c65 0a66 726f 6d20  ort locale.from 
+00000030: 6f73 2069 6d70 6f72 7420 280a 2020 2020  os import (.    
+00000040: 656e 7669 726f 6e2c 0a20 2020 2067 6574  environ,.    get
+00000050: 656e 762c 0a20 2020 206d 6b64 6972 2c0a  env,.    mkdir,.
+00000060: 2020 2020 7061 7468 2c0a 290a 0a0a 636c      path,.)...cl
+00000070: 6173 7320 436f 6e66 6967 3a0a 2020 2020  ass Config:.    
+00000080: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00000090: 6629 3a0a 2020 2020 2020 2020 2320 4d6f  f):.        # Mo
+000000a0: 7573 6520 6163 7469 7661 7469 6f6e 0a20  use activation. 
+000000b0: 2020 2020 2020 2073 656c 662e 5f6d 6d61         self._mma
+000000c0: 736b 203d 2028 6375 7273 6573 2e42 5554  sk = (curses.BUT
+000000d0: 544f 4e31 5f43 4c49 434b 4544 202b 2063  TON1_CLICKED + c
+000000e0: 7572 7365 732e 4255 5454 4f4e 315f 444f  urses.BUTTON1_DO
+000000f0: 5542 4c45 5f43 4c49 434b 4544 0a20 2020  UBLE_CLICKED.   
+00000100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000110: 2020 2020 2b20 6375 7273 6573 2e42 5554      + curses.BUT
+00000120: 544f 4e31 5f54 5249 504c 455f 434c 4943  TON1_TRIPLE_CLIC
+00000130: 4b45 4429 0a20 2020 2020 2020 2023 2069  KED).        # i
+00000140: 6e76 6973 6962 6c65 2063 7572 736f 720a  nvisible cursor.
+00000150: 2020 2020 2020 2020 6375 7273 6573 2e63          curses.c
+00000160: 7572 735f 7365 7428 3029 0a20 2020 2020  urs_set(0).     
+00000170: 2020 2023 2061 6c6c 6f77 2074 7261 6e73     # allow trans
+00000180: 7061 7265 6e63 790a 2020 2020 2020 2020  parency.        
+00000190: 6375 7273 6573 2e75 7365 5f64 6566 6175  curses.use_defau
+000001a0: 6c74 5f63 6f6c 6f72 7328 290a 2020 2020  lt_colors().    
+000001b0: 2020 2020 2320 7573 6520 7468 6520 6c6f      # use the lo
+000001c0: 6361 6c65 210a 2020 2020 2020 2020 6c6f  cale!.        lo
+000001d0: 6361 6c65 2e73 6574 6c6f 6361 6c65 286c  cale.setlocale(l
+000001e0: 6f63 616c 652e 4c43 5f41 4c4c 2c20 2727  ocale.LC_ALL, ''
+000001f0: 290a 2020 2020 2020 2020 6765 7474 6578  ).        gettex
+00000200: 742e 696e 7374 616c 6c28 2263 756c 656e  t.install("culen
+00000210: 6461 7222 2c0a 2020 2020 2020 2020 2020  dar",.          
+00000220: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00000230: 7468 2e64 6972 6e61 6d65 2870 6174 682e  th.dirname(path.
+00000240: 7265 616c 7061 7468 285f 5f66 696c 655f  realpath(__file_
+00000250: 5f29 292b 222f 2e2e 2f6c 6f63 616c 6522  _))+"/../locale"
+00000260: 290a 0a20 2020 2020 2020 2023 2063 7265  )..        # cre
+00000270: 6174 6520 6465 6661 756c 7420 7661 6c75  ate default valu
+00000280: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
+00000290: 5f68 6d69 6e20 3d20 3720 2020 2320 3720  _hmin = 7   # 7 
+000002a0: 616d 0a20 2020 2020 2020 2073 656c 662e  am.        self.
+000002b0: 5f68 6d61 7820 3d20 3230 2020 2320 3820  _hmax = 20  # 8 
+000002c0: 706d 0a20 2020 2020 2020 2073 656c 662e  pm.        self.
+000002d0: 5f57 4520 3d20 626f 6f6c 2831 2920 2023  _WE = bool(1)  #
+000002e0: 2073 686f 7720 7765 656b 2d65 6e64 730a   show week-ends.
+000002f0: 2020 2020 2020 2020 7365 6c66 2e5f 746f          self._to
+00000300: 646f 203d 2062 6f6f 6c28 3029 2020 2020  do = bool(0)    
+00000310: 2020 2320 646f 6573 6e27 7420 7368 6f77    # doesn't show
+00000320: 2074 6f64 6f20 6c69 7374 0a20 2020 2020   todo list.     
+00000330: 2020 2073 656c 662e 5f74 6f64 6f77 6964     self._todowid
+00000340: 7468 203d 2030 2e32 2020 2020 2023 2064  th = 0.2     # d
+00000350: 6566 6175 6c74 7320 3230 2520 7769 6474  efaults 20% widt
+00000360: 680a 2020 2020 2020 2020 7365 6c66 2e5f  h.        self._
+00000370: 6175 746f 7361 7665 203d 2062 6f6f 6c28  autosave = bool(
+00000380: 3129 2020 2320 6465 6661 756c 7473 2074  1)  # defaults t
+00000390: 6f20 6265 206c 6573 7320 756e 7573 7561  o be less unusua
+000003a0: 6c0a 2020 2020 2020 2020 7365 6c66 2e5f  l.        self._
+000003b0: 636f 6c6f 7572 7365 7420 3d20 3020 2020  colourset = 0   
+000003c0: 2020 2020 2320 6465 6661 756c 7473 2074      # defaults t
+000003d0: 6f20 666c 6173 6879 0a20 2020 2020 2020  o flashy.       
+000003e0: 2073 656c 662e 5f63 616c 6461 7620 3d20   self._caldav = 
+000003f0: 5b5d 2020 2020 2020 2020 2023 2065 6d70  []         # emp
+00000400: 7479 206c 6973 7420 6f66 2063 616c 6461  ty list of calda
+00000410: 7673 0a20 2020 2020 2020 2073 656c 662e  vs.        self.
+00000420: 5f61 7574 6f73 796e 6320 3d20 4661 6c73  _autosync = Fals
+00000430: 6520 2020 2023 2061 7574 6f75 7064 6174  e    # autoupdat
+00000440: 6520 616c 6c20 6361 6c64 6176 7320 7768  e all caldavs wh
+00000450: 656e 2063 6861 6e67 696e 6720 6461 790a  en changing day.
+00000460: 2020 2020 2020 2020 7365 6c66 2e5f 6d6f          self._mo
+00000470: 7573 6520 3d20 4661 6c73 6520 2020 2020  use = False     
+00000480: 2020 2320 6469 7361 626c 6520 6d6f 7573    # disable mous
+00000490: 650a 2020 2020 2020 2020 6375 7273 6573  e.        curses
+000004a0: 2e6d 6f75 7365 6d61 736b 2830 290a 2020  .mousemask(0).  
+000004b0: 2020 2020 2020 7365 6c66 2e5f 6465 6275        self._debu
+000004c0: 6720 3d20 626f 6f6c 2830 2920 2020 2020  g = bool(0)     
+000004d0: 2320 796f 7520 7761 6e74 2074 6f20 7365  # you want to se
+000004e0: 6520 6465 6164 2064 7563 6b73 0a0a 2020  e dead ducks..  
+000004f0: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+00000500: 6469 7228 2920 2023 2064 6566 696e 6520  dir()  # define 
+00000510: 7061 7468 730a 2020 2020 2020 2020 7365  paths.        se
+00000520: 6c66 2e5f 636f 6e66 6967 6669 6c65 203d  lf._configfile =
+00000530: 2073 656c 662e 5f63 6f6e 6669 6770 6174   self._configpat
+00000540: 6820 2b20 272f 6375 6c65 6e64 6172 2e63  h + '/culendar.c
+00000550: 6f6e 6627 0a20 2020 2020 2020 2073 656c  onf'.        sel
+00000560: 662e 5f6b 6579 7366 696c 6520 3d20 7365  f._keysfile = se
+00000570: 6c66 2e5f 636f 6e66 6967 7061 7468 202b  lf._configpath +
+00000580: 2027 2f6b 6579 732e 636f 6e66 270a 2020   '/keys.conf'.  
+00000590: 2020 2020 2020 7365 6c66 2e5f 636f 6c6f        self._colo
+000005a0: 7572 7366 696c 6520 3d20 7365 6c66 2e5f  ursfile = self._
+000005b0: 636f 6e66 6967 7061 7468 202b 2027 2f63  configpath + '/c
+000005c0: 6f6c 6f75 7273 2e63 6f6e 6627 0a20 2020  olours.conf'.   
+000005d0: 2020 2020 2073 656c 662e 5f63 6174 6567       self._categ
+000005e0: 6f72 6965 7366 696c 6520 3d20 7365 6c66  oriesfile = self
+000005f0: 2e5f 636f 6e66 6967 7061 7468 202b 2027  ._configpath + '
+00000600: 2f63 6174 6567 6f72 6965 732e 636f 6e66  /categories.conf
+00000610: 270a 2020 2020 2020 2020 7365 6c66 2e5f  '.        self._
+00000620: 6361 6c64 6176 6669 6c65 203d 2073 656c  caldavfile = sel
+00000630: 662e 5f63 6f6e 6669 6770 6174 6820 2b20  f._configpath + 
+00000640: 272f 6361 6c64 6176 2e63 6f6e 6627 0a20  '/caldav.conf'. 
+00000650: 2020 2020 2020 2073 656c 662e 5f64 6174         self._dat
+00000660: 6166 696c 6520 3d20 7365 6c66 2e5f 6461  afile = self._da
+00000670: 7461 7061 7468 202b 2027 2f61 7074 7327  tapath + '/apts'
+00000680: 0a20 2020 2020 2020 2073 656c 662e 5f74  .        self._t
+00000690: 6f64 6f66 696c 6520 3d20 7365 6c66 2e5f  odofile = self._
+000006a0: 6461 7461 7061 7468 202b 2027 2f74 6f64  datapath + '/tod
+000006b0: 6f27 0a20 2020 2020 2020 2023 2063 7265  o'.        # cre
+000006c0: 6174 6520 626c 616e 6b73 206f 6e65 2069  ate blanks one i
+000006d0: 6620 6e6f 7420 6578 6973 7469 6e67 0a20  f not existing. 
+000006e0: 2020 2020 2020 2069 6620 6e6f 7420 7061         if not pa
+000006f0: 7468 2e65 7869 7374 7328 7365 6c66 2e5f  th.exists(self._
+00000700: 6461 7461 6669 6c65 293a 0a20 2020 2020  datafile):.     
+00000710: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00000720: 2873 656c 662e 5f64 6174 6166 696c 652c  (self._datafile,
+00000730: 2022 7722 2920 6173 2066 3a0a 2020 2020   "w") as f:.    
+00000740: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
+00000750: 6974 6528 2222 290a 2020 2020 2020 2020  ite("").        
+00000760: 6966 206e 6f74 2070 6174 682e 6578 6973  if not path.exis
+00000770: 7473 2873 656c 662e 5f74 6f64 6f66 696c  ts(self._todofil
+00000780: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00000790: 7769 7468 206f 7065 6e28 7365 6c66 2e5f  with open(self._
+000007a0: 746f 646f 6669 6c65 2c20 2277 2229 2061  todofile, "w") a
+000007b0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+000007c0: 2020 2020 2066 2e77 7269 7465 2822 2229       f.write("")
+000007d0: 0a0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+000007e0: 6561 6463 6f6e 6628 2920 2020 2020 2020  eadconf()       
+000007f0: 2020 2320 6f76 6572 7772 6974 6573 2064    # overwrites d
+00000800: 6566 6175 6c74 2076 616c 7565 730a 2020  efault values.  
+00000810: 2020 2020 2020 7365 6c66 2e72 6561 646b        self.readk
+00000820: 6579 7328 2920 2020 2020 2020 2020 2320  eys()         # 
+00000830: 6465 6669 6e65 7320 7365 6c66 2e5f 6b65  defines self._ke
+00000840: 7973 0a20 2020 2020 2020 2073 656c 662e  ys.        self.
+00000850: 7265 6164 636f 6c6f 7572 7328 2920 2020  readcolours()   
+00000860: 2020 2023 2064 6566 696e 6573 2073 656c     # defines sel
+00000870: 662e 5f63 6f6c 6f75 7273 5f69 6478 0a20  f._colours_idx. 
+00000880: 2020 2020 2020 2073 656c 662e 7365 7463         self.setc
+00000890: 6f6c 6f75 7273 2829 2020 2020 2020 2023  olours()       #
+000008a0: 2064 6566 696e 6573 2073 656c 662e 5f63   defines self._c
+000008b0: 6f6c 6f75 7273 0a20 2020 2020 2020 2073  olours.        s
+000008c0: 656c 662e 7265 6164 6361 7465 676f 7269  elf.readcategori
+000008d0: 6573 2829 2020 2023 2064 6566 696e 6573  es()   # defines
+000008e0: 2073 656c 662e 5f63 6174 6567 6f72 6965   self._categorie
+000008f0: 730a 2020 2020 2020 2020 7365 6c66 2e72  s.        self.r
+00000900: 6561 6463 616c 6461 7628 2920 2020 2020  eadcaldav()     
+00000910: 2020 2320 6765 7420 7468 6520 6361 6c64    # get the cald
+00000920: 6176 7320 636f 6e66 6967 7572 6174 696f  avs configuratio
+00000930: 6e73 0a0a 2020 2020 4070 726f 7065 7274  ns..    @propert
+00000940: 790a 2020 2020 6465 6620 686d 696e 2873  y.    def hmin(s
+00000950: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00000960: 7475 726e 2073 656c 662e 5f68 6d69 6e0a  turn self._hmin.
+00000970: 0a20 2020 2040 686d 696e 2e73 6574 7465  .    @hmin.sette
+00000980: 720a 2020 2020 6465 6620 686d 696e 2873  r.    def hmin(s
+00000990: 656c 662c 2068 6d69 6e29 3a0a 2020 2020  elf, hmin):.    
+000009a0: 2020 2020 6966 2068 6d69 6e20 3e3d 2073      if hmin >= s
+000009b0: 656c 662e 5f68 6d61 783a 0a20 2020 2020  elf._hmax:.     
+000009c0: 2020 2020 2020 2073 656c 662e 5f68 6d69         self._hmi
+000009d0: 6e20 3d20 7365 6c66 2e5f 686d 6178 2d31  n = self._hmax-1
+000009e0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000009f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000a00: 5f68 6d69 6e20 3d20 6d61 7828 302c 2068  _hmin = max(0, h
+00000a10: 6d69 6e29 0a0a 2020 2020 4070 726f 7065  min)..    @prope
+00000a20: 7274 790a 2020 2020 6465 6620 686d 6178  rty.    def hmax
+00000a30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00000a40: 7265 7475 726e 2073 656c 662e 5f68 6d61  return self._hma
+00000a50: 780a 0a20 2020 2040 686d 6178 2e73 6574  x..    @hmax.set
+00000a60: 7465 720a 2020 2020 6465 6620 686d 6178  ter.    def hmax
+00000a70: 2873 656c 662c 2068 6d61 7829 3a0a 2020  (self, hmax):.  
+00000a80: 2020 2020 2020 6966 2068 6d61 7820 3c3d        if hmax <=
+00000a90: 2073 656c 662e 5f68 6d69 6e3a 0a20 2020   self._hmin:.   
+00000aa0: 2020 2020 2020 2020 2073 656c 662e 5f68           self._h
+00000ab0: 6d61 7820 3d20 7365 6c66 2e5f 686d 696e  max = self._hmin
+00000ac0: 2b31 0a20 2020 2020 2020 2065 6c73 653a  +1.        else:
+00000ad0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00000ae0: 662e 5f68 6d61 7820 3d20 6d69 6e28 3234  f._hmax = min(24
+00000af0: 2c20 686d 6178 290a 0a20 2020 2040 7072  , hmax)..    @pr
+00000b00: 6f70 6572 7479 0a20 2020 2064 6566 2057  operty.    def W
+00000b10: 4528 7365 6c66 293a 0a20 2020 2020 2020  E(self):.       
+00000b20: 2072 6574 7572 6e20 7365 6c66 2e5f 5745   return self._WE
+00000b30: 0a0a 2020 2020 4057 452e 7365 7474 6572  ..    @WE.setter
+00000b40: 0a20 2020 2064 6566 2057 4528 7365 6c66  .    def WE(self
+00000b50: 2c20 5745 293a 0a20 2020 2020 2020 2073  , WE):.        s
+00000b60: 656c 662e 5f57 4520 3d20 5745 0a0a 2020  elf._WE = WE..  
+00000b70: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00000b80: 6465 6620 746f 646f 2873 656c 6629 3a0a  def todo(self):.
+00000b90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00000ba0: 656c 662e 5f74 6f64 6f0a 0a20 2020 2040  elf._todo..    @
+00000bb0: 746f 646f 2e73 6574 7465 720a 2020 2020  todo.setter.    
+00000bc0: 6465 6620 746f 646f 2873 656c 662c 2054  def todo(self, T
+00000bd0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00000be0: 5f74 6f64 6f20 3d20 540a 0a20 2020 2040  _todo = T..    @
+00000bf0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00000c00: 2074 6f64 6f77 6964 7468 2873 656c 6629   todowidth(self)
+00000c10: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00000c20: 2073 656c 662e 5f74 6f64 6f77 6964 7468   self._todowidth
+00000c30: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00000c40: 2020 2020 6465 6620 6175 746f 7361 7665      def autosave
+00000c50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00000c60: 7265 7475 726e 2073 656c 662e 5f61 7574  return self._aut
+00000c70: 6f73 6176 650a 0a20 2020 2040 6175 746f  osave..    @auto
+00000c80: 7361 7665 2e73 6574 7465 720a 2020 2020  save.setter.    
+00000c90: 6465 6620 6175 746f 7361 7665 2873 656c  def autosave(sel
+00000ca0: 662c 2061 7574 6f73 6176 6529 3a0a 2020  f, autosave):.  
+00000cb0: 2020 2020 2020 7365 6c66 2e5f 6175 746f        self._auto
+00000cc0: 7361 7665 203d 2061 7574 6f73 6176 650a  save = autosave.
+00000cd0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00000ce0: 2020 2064 6566 206b 6579 7328 7365 6c66     def keys(self
+00000cf0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00000d00: 6e20 7365 6c66 2e5f 6b65 7973 0a0a 2020  n self._keys..  
+00000d10: 2020 406b 6579 732e 7365 7474 6572 0a20    @keys.setter. 
+00000d20: 2020 2064 6566 206b 6579 7328 7365 6c66     def keys(self
+00000d30: 2c20 6b65 7973 293a 0a20 2020 2020 2020  , keys):.       
+00000d40: 2073 656c 662e 5f6b 6579 7320 3d20 6b65   self._keys = ke
+00000d50: 7973 0a0a 2020 2020 4070 726f 7065 7274  ys..    @propert
+00000d60: 790a 2020 2020 6465 6620 6461 7461 6669  y.    def datafi
+00000d70: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
+00000d80: 2020 7265 7475 726e 2073 656c 662e 5f64    return self._d
+00000d90: 6174 6166 696c 650a 0a20 2020 2040 7072  atafile..    @pr
+00000da0: 6f70 6572 7479 0a20 2020 2064 6566 2074  operty.    def t
+00000db0: 6f64 6f66 696c 6528 7365 6c66 293a 0a20  odofile(self):. 
+00000dc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00000dd0: 6c66 2e5f 746f 646f 6669 6c65 0a0a 2020  lf._todofile..  
+00000de0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00000df0: 6465 6620 636f 6c6f 7572 7365 7428 7365  def colourset(se
+00000e00: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00000e10: 7572 6e20 7365 6c66 2e5f 636f 6c6f 7572  urn self._colour
+00000e20: 7365 740a 0a20 2020 2040 636f 6c6f 7572  set..    @colour
+00000e30: 7365 742e 7365 7474 6572 0a20 2020 2064  set.setter.    d
+00000e40: 6566 2063 6f6c 6f75 7273 6574 2873 656c  ef colourset(sel
+00000e50: 662c 2063 7329 3a0a 2020 2020 2020 2020  f, cs):.        
+00000e60: 7365 6c66 2e5f 636f 6c6f 7572 7365 7420  self._colourset 
+00000e70: 3d20 6373 0a0a 2020 2020 4070 726f 7065  = cs..    @prope
+00000e80: 7274 790a 2020 2020 6465 6620 636f 6c6f  rty.    def colo
+00000e90: 7572 735f 6964 7828 7365 6c66 293a 0a20  urs_idx(self):. 
+00000ea0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00000eb0: 6c66 2e5f 636f 6c6f 7572 735f 6964 780a  lf._colours_idx.
+00000ec0: 0a20 2020 2040 636f 6c6f 7572 735f 6964  .    @colours_id
+00000ed0: 782e 7365 7474 6572 0a20 2020 2064 6566  x.setter.    def
+00000ee0: 2063 6f6c 6f75 7273 5f69 6478 2873 656c   colours_idx(sel
+00000ef0: 662c 2069 6478 293a 0a20 2020 2020 2020  f, idx):.       
+00000f00: 2073 656c 662e 5f63 6f6c 6f75 7273 5f69   self._colours_i
+00000f10: 6478 203d 2069 6478 0a0a 2020 2020 4070  dx = idx..    @p
+00000f20: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00000f30: 636f 6c6f 7572 7328 7365 6c66 293a 0a20  colours(self):. 
+00000f40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00000f50: 6c66 2e5f 636f 6c6f 7572 730a 0a20 2020  lf._colours..   
+00000f60: 2040 636f 6c6f 7572 732e 7365 7474 6572   @colours.setter
+00000f70: 0a20 2020 2064 6566 2063 6f6c 6f75 7273  .    def colours
+00000f80: 2873 656c 662c 2063 6f6c 6f75 7273 293a  (self, colours):
+00000f90: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+00000fa0: 6f6c 6f75 7273 203d 2063 6f6c 6f75 7273  olours = colours
+00000fb0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00000fc0: 2020 2020 6465 6620 6361 7465 676f 7269      def categori
+00000fd0: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
+00000fe0: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
+00000ff0: 6174 6567 6f72 6965 730a 0a20 2020 2040  ategories..    @
+00001000: 6361 7465 676f 7269 6573 2e73 6574 7465  categories.sette
+00001010: 720a 2020 2020 6465 6620 6361 7465 676f  r.    def catego
+00001020: 7269 6573 2873 656c 662c 2063 6174 6567  ries(self, categ
+00001030: 6f72 6965 7329 3a0a 2020 2020 2020 2020  ories):.        
+00001040: 7365 6c66 2e5f 6361 7465 676f 7269 6573  self._categories
+00001050: 203d 2063 6174 6567 6f72 6965 730a 0a20   = categories.. 
+00001060: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00001070: 2064 6566 2063 616c 6461 7628 7365 6c66   def caldav(self
+00001080: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00001090: 6e20 7365 6c66 2e5f 6361 6c64 6176 0a0a  n self._caldav..
+000010a0: 2020 2020 4063 616c 6461 762e 7365 7474      @caldav.sett
+000010b0: 6572 0a20 2020 2064 6566 2063 616c 6461  er.    def calda
+000010c0: 7628 7365 6c66 2c20 6361 6c64 6176 293a  v(self, caldav):
+000010d0: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+000010e0: 616c 6461 7620 3d20 6361 6c64 6176 0a0a  aldav = caldav..
+000010f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00001100: 2020 6465 6620 6175 746f 7379 6e63 2873    def autosync(s
+00001110: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00001120: 7475 726e 2073 656c 662e 5f61 7574 6f73  turn self._autos
+00001130: 796e 630a 0a20 2020 2040 6175 746f 7379  ync..    @autosy
+00001140: 6e63 2e73 6574 7465 720a 2020 2020 6465  nc.setter.    de
+00001150: 6620 6175 746f 7379 6e63 2873 656c 662c  f autosync(self,
+00001160: 2061 7574 6f73 796e 6329 3a0a 2020 2020   autosync):.    
+00001170: 2020 2020 7365 6c66 2e5f 6175 746f 7379      self._autosy
+00001180: 6e63 203d 2061 7574 6f73 796e 630a 0a20  nc = autosync.. 
+00001190: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000011a0: 2064 6566 206d 6f75 7365 2873 656c 6629   def mouse(self)
+000011b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000011c0: 2073 656c 662e 5f6d 6f75 7365 0a0a 2020   self._mouse..  
+000011d0: 2020 406d 6f75 7365 2e73 6574 7465 720a    @mouse.setter.
+000011e0: 2020 2020 6465 6620 6d6f 7573 6528 7365      def mouse(se
+000011f0: 6c66 2c20 6d6f 7573 6529 3a0a 2020 2020  lf, mouse):.    
+00001200: 2020 2020 7365 6c66 2e5f 6d6f 7573 6520      self._mouse 
+00001210: 3d20 6d6f 7573 650a 2020 2020 2020 2020  = mouse.        
+00001220: 6966 206d 6f75 7365 3a0a 2020 2020 2020  if mouse:.      
+00001230: 2020 2020 2020 6375 7273 6573 2e6d 6f75        curses.mou
+00001240: 7365 6d61 736b 2873 656c 662e 5f6d 6d61  semask(self._mma
+00001250: 736b 290a 2020 2020 2020 2020 656c 7365  sk).        else
+00001260: 3a0a 2020 2020 2020 2020 2020 2020 6375  :.            cu
+00001270: 7273 6573 2e6d 6f75 7365 6d61 736b 2830  rses.mousemask(0
+00001280: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+00001290: 0a20 2020 2064 6566 2064 6562 7567 2873  .    def debug(s
+000012a0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+000012b0: 7475 726e 2073 656c 662e 5f64 6562 7567  turn self._debug
+000012c0: 0a0a 2020 2020 6465 6620 6368 6563 6b64  ..    def checkd
+000012d0: 6972 2873 656c 6629 3a0a 2020 2020 2020  ir(self):.      
+000012e0: 2020 2320 636f 6e66 6967 7572 6174 696f    # configuratio
+000012f0: 6e20 7374 7566 660a 2020 2020 2020 2020  n stuff.        
+00001300: 6966 2027 5844 475f 434f 4e46 4947 5f48  if 'XDG_CONFIG_H
+00001310: 4f4d 4527 2069 6e20 656e 7669 726f 6e3a  OME' in environ:
+00001320: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001330: 662e 5f63 6f6e 6669 6770 6174 6820 3d20  f._configpath = 
+00001340: 6765 7465 6e76 2827 5844 475f 4441 5441  getenv('XDG_DATA
+00001350: 5f48 4f4d 4527 290a 2020 2020 2020 2020  _HOME').        
+00001360: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00001370: 2020 7365 6c66 2e5f 636f 6e66 6967 7061    self._configpa
+00001380: 7468 203d 2067 6574 656e 7628 2748 4f4d  th = getenv('HOM
+00001390: 4527 292b 272f 2e63 6f6e 6669 672f 6375  E')+'/.config/cu
+000013a0: 6c65 6e64 6172 270a 0a20 2020 2020 2020  lendar'..       
+000013b0: 2069 6620 6e6f 7420 7061 7468 2e65 7869   if not path.exi
+000013c0: 7374 7328 7365 6c66 2e5f 636f 6e66 6967  sts(self._config
+000013d0: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
+000013e0: 2020 2023 2069 6d70 6c69 6369 746c 7920     # implicitly 
+000013f0: 7375 7070 6f73 6520 7468 6174 2024 484f  suppose that $HO
+00001400: 4d45 2f2e 636f 6e66 6967 2061 6c72 6561  ME/.config alrea
+00001410: 6479 2065 7869 7374 730a 2020 2020 2020  dy exists.      
+00001420: 2020 2020 2020 6d6b 6469 7228 7365 6c66        mkdir(self
+00001430: 2e5f 636f 6e66 6967 7061 7468 290a 0a20  ._configpath).. 
+00001440: 2020 2020 2020 2023 2064 6174 6120 7374         # data st
+00001450: 7566 660a 2020 2020 2020 2020 6966 2027  uff.        if '
+00001460: 5844 475f 4441 5441 5f48 4f4d 4527 2069  XDG_DATA_HOME' i
+00001470: 6e20 656e 7669 726f 6e3a 0a20 2020 2020  n environ:.     
+00001480: 2020 2020 2020 2073 656c 662e 5f64 6174         self._dat
+00001490: 6170 6174 6820 3d20 6765 7465 6e76 2827  apath = getenv('
+000014a0: 5844 475f 4441 5441 5f48 4f4d 4527 290a  XDG_DATA_HOME').
+000014b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000014c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000014d0: 6461 7461 7061 7468 203d 2067 6574 656e  datapath = geten
+000014e0: 7628 2748 4f4d 4527 292b 272f 2e6c 6f63  v('HOME')+'/.loc
+000014f0: 616c 2f73 6861 7265 2f63 756c 656e 6461  al/share/culenda
+00001500: 7227 0a0a 2020 2020 2020 2020 6966 206e  r'..        if n
+00001510: 6f74 2070 6174 682e 6578 6973 7473 2873  ot path.exists(s
+00001520: 656c 662e 5f64 6174 6170 6174 6829 3a0a  elf._datapath):.
+00001530: 2020 2020 2020 2020 2020 2020 2320 696d              # im
+00001540: 706c 6963 6974 6c79 2073 7570 706f 7365  plicitly suppose
+00001550: 2074 6861 7420 2448 4f4d 452f 2e6c 6f63   that $HOME/.loc
+00001560: 616c 2f73 6861 7265 2061 6c72 6561 6479  al/share already
+00001570: 2065 7869 7374 730a 2020 2020 2020 2020   exists.        
+00001580: 2020 2020 6d6b 6469 7228 7365 6c66 2e5f      mkdir(self._
+00001590: 6461 7461 7061 7468 290a 0a20 2020 2064  datapath)..    d
+000015a0: 6566 2072 6561 6463 6f6e 6628 7365 6c66  ef readconf(self
+000015b0: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
+000015c0: 7420 7061 7468 2e65 7869 7374 7328 7365  t path.exists(se
+000015d0: 6c66 2e5f 636f 6e66 6967 6669 6c65 293a  lf._configfile):
+000015e0: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
+000015f0: 7269 7465 2074 6865 2064 6566 6175 6c74  rite the default
+00001600: 2063 6f6e 660a 2020 2020 2020 2020 2020   conf.          
+00001610: 2020 7365 6c66 2e77 7269 7465 636f 6e66    self.writeconf
+00001620: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+00001630: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+00001640: 6820 6f70 656e 2873 656c 662e 5f63 6f6e  h open(self._con
+00001650: 6669 6766 696c 6529 2061 7320 663a 0a20  figfile) as f:. 
+00001660: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00001670: 6f72 206c 696e 6520 696e 2066 3a0a 2020  or line in f:.  
 00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 666f 7220 6c69 6e65 2069 6e20 663a 0a20  for line in f:. 
-000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016b0: 2020 2069 6620 6c69 6e65 5b30 3a37 5d20     if line[0:7] 
-000016c0: 3d3d 2027 686d 696e 203d 2027 3a0a 2020  == 'hmin = ':.  
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 2320 646f 6e27 7420 7573        # don't us
-000016f0: 6520 7468 6520 7365 7474 6572 2074 6f20  e the setter to 
-00001700: 6861 7665 206e 6f20 6c69 6d69 7420 6f6e  have no limit on
-00001710: 2068 6d69 6e0a 2020 2020 2020 2020 2020   hmin.          
-00001720: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001730: 6c66 2e5f 686d 696e 203d 2069 6e74 286c  lf._hmin = int(l
-00001740: 696e 655b 373a 395d 290a 2020 2020 2020  ine[7:9]).      
-00001750: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001760: 206c 696e 655b 303a 375d 203d 3d20 2768   line[0:7] == 'h
-00001770: 6d61 7820 3d20 273a 0a20 2020 2020 2020  max = ':.       
-00001780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001790: 2023 2075 7365 2074 6865 2073 6574 7465   # use the sette
-000017a0: 7220 746f 2062 6520 7375 7265 2074 6f20  r to be sure to 
-000017b0: 6265 2068 6967 6865 7220 7468 616e 2068  be higher than h
-000017c0: 6d69 6e0a 2020 2020 2020 2020 2020 2020  min.            
-000017d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000017e0: 2e68 6d61 7820 3d20 696e 7428 6c69 6e65  .hmax = int(line
-000017f0: 5b37 3a39 5d29 0a20 2020 2020 2020 2020  [7:9]).         
-00001800: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
-00001810: 6e65 5b30 3a35 5d20 3d3d 2027 5745 203d  ne[0:5] == 'WE =
-00001820: 2027 3a0a 2020 2020 2020 2020 2020 2020   ':.            
-00001830: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001840: 2e5f 5745 203d 2062 6f6f 6c28 696e 7428  ._WE = bool(int(
-00001850: 6c69 6e65 5b35 5d29 2920 2023 2022 3022  line[5]))  # "0"
-00001860: 2074 6f20 3020 746f 2046 616c 7365 0a20   to 0 to False. 
-00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001880: 2020 2069 6620 6c69 6e65 5b30 3a31 315d     if line[0:11]
-00001890: 203d 3d20 2761 7574 6f73 6176 6520 3d20   == 'autosave = 
-000018a0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-000018b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000018c0: 5f61 7574 6f73 6176 6520 3d20 626f 6f6c  _autosave = bool
-000018d0: 2869 6e74 286c 696e 655b 3131 5d29 290a  (int(line[11])).
-000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018f0: 2020 2020 6966 206c 696e 655b 303a 3132      if line[0:12
-00001900: 5d20 3d3d 2027 636f 6c6f 7572 7365 7420  ] == 'colourset 
-00001910: 3d20 273a 0a20 2020 2020 2020 2020 2020  = ':.           
-00001920: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00001930: 662e 5f63 6f6c 6f75 7273 6574 203d 2069  f._colourset = i
-00001940: 6e74 286c 696e 655b 3132 5d29 0a20 2020  nt(line[12]).   
-00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 2069 6620 6c69 6e65 5b30 3a31 315d 203d   if line[0:11] =
-00001970: 3d20 2761 7574 6f73 796e 6320 3d20 273a  = 'autosync = ':
-00001980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001990: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
-000019a0: 7574 6f73 796e 6320 3d20 626f 6f6c 2869  utosync = bool(i
-000019b0: 6e74 286c 696e 655b 3131 5d29 290a 2020  nt(line[11])).  
-000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 2020 6966 206c 696e 655b 303a 385d 203d    if line[0:8] =
-000019e0: 3d20 2764 6562 7567 203d 2027 3a0a 2020  = 'debug = ':.  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 2020 2020 7365 6c66 2e5f 6465 6275        self._debu
-00001a10: 6720 3d20 626f 6f6c 2869 6e74 286c 696e  g = bool(int(lin
-00001a20: 655b 385d 2929 0a20 2020 2020 2020 2020  e[8])).         
-00001a30: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
-00001a40: 6e65 5b30 3a37 5d20 3d3d 2027 746f 646f  ne[0:7] == 'todo
-00001a50: 203d 2027 3a0a 2020 2020 2020 2020 2020   = ':.          
-00001a60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001a70: 6c66 2e5f 746f 646f 203d 2062 6f6f 6c28  lf._todo = bool(
-00001a80: 696e 7428 6c69 6e65 5b37 5d29 290a 2020  int(line[7])).  
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 2020 6966 206c 696e 655b 303a 3132 5d20    if line[0:12] 
-00001ab0: 3d3d 2027 746f 646f 7769 6474 6820 3d20  == 'todowidth = 
-00001ac0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00001ad0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001ae0: 5f74 6f64 6f77 6964 7468 203d 2066 6c6f  _todowidth = flo
-00001af0: 6174 286c 696e 655b 3132 3a5d 290a 2020  at(line[12:]).  
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 2020 6966 206c 696e 655b 303a 385d 203d    if line[0:8] =
-00001b20: 3d20 276d 6f75 7365 203d 2027 3a0a 2020  = 'mouse = ':.  
-00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b40: 2020 2020 2020 7365 6c66 2e6d 6f75 7365        self.mouse
-00001b50: 203d 2062 6f6f 6c28 696e 7428 6c69 6e65   = bool(int(line
-00001b60: 5b38 3a5d 2929 0a20 2020 2020 2020 2020  [8:])).         
-00001b70: 2020 2020 2020 2023 2054 4f44 4f3a 2063         # TODO: c
-00001b80: 6865 636b 2069 6620 616c 6c20 6973 2066  heck if all is f
-00001b90: 696e 650a 0a20 2020 2064 6566 2077 7269  ine..    def wri
-00001ba0: 7465 636f 6e66 2873 656c 6629 3a0a 2020  teconf(self):.  
-00001bb0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00001bc0: 7365 6c66 2e5f 636f 6e66 6967 6669 6c65  self._configfile
-00001bd0: 2c20 2277 2229 2061 7320 663a 0a20 2020  , "w") as f:.   
-00001be0: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00001bf0: 2827 686d 696e 203d 2027 202b 2073 7472  ('hmin = ' + str
-00001c00: 2873 656c 662e 5f68 6d69 6e29 202b 2027  (self._hmin) + '
-00001c10: 5c6e 2729 0a20 2020 2020 2020 2020 2020  \n').           
-00001c20: 2066 2e77 7269 7465 2827 686d 6178 203d   f.write('hmax =
-00001c30: 2027 202b 2073 7472 2873 656c 662e 5f68   ' + str(self._h
-00001c40: 6d61 7829 202b 2027 5c6e 2729 0a20 2020  max) + '\n').   
-00001c50: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00001c60: 2827 5745 203d 2027 202b 2073 7472 2869  ('WE = ' + str(i
-00001c70: 6e74 2873 656c 662e 5f57 4529 2920 2b20  nt(self._WE)) + 
-00001c80: 275c 6e27 290a 2020 2020 2020 2020 2020  '\n').          
-00001c90: 2020 662e 7772 6974 6528 2761 7574 6f73    f.write('autos
-00001ca0: 6176 6520 3d20 2720 2b20 7374 7228 696e  ave = ' + str(in
-00001cb0: 7428 7365 6c66 2e5f 6175 746f 7361 7665  t(self._autosave
-00001cc0: 2929 202b 2027 5c6e 2729 0a20 2020 2020  )) + '\n').     
-00001cd0: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00001ce0: 636f 6c6f 7572 7365 7420 3d20 2720 2b20  colourset = ' + 
-00001cf0: 7374 7228 7365 6c66 2e5f 636f 6c6f 7572  str(self._colour
-00001d00: 7365 7429 202b 2027 5c6e 2729 0a20 2020  set) + '\n').   
-00001d10: 2020 2020 2020 2020 2066 2e77 7269 7465           f.write
-00001d20: 2827 6175 746f 7379 6e63 203d 2027 202b  ('autosync = ' +
-00001d30: 2073 7472 2869 6e74 2873 656c 662e 5f61   str(int(self._a
-00001d40: 7574 6f73 796e 6329 292b 275c 6e27 290a  utosync))+'\n').
-00001d50: 2020 2020 2020 2020 2020 2020 662e 7772              f.wr
-00001d60: 6974 6528 2774 6f64 6f20 3d20 2720 2b20  ite('todo = ' + 
-00001d70: 7374 7228 696e 7428 7365 6c66 2e5f 746f  str(int(self._to
-00001d80: 646f 2929 2b27 5c6e 2729 0a20 2020 2020  do))+'\n').     
-00001d90: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00001da0: 746f 646f 7769 6474 6820 3d20 2720 2b20  todowidth = ' + 
-00001db0: 7374 7228 7365 6c66 2e5f 746f 646f 7769  str(self._todowi
-00001dc0: 6474 6829 2b27 5c6e 2729 0a20 2020 2020  dth)+'\n').     
-00001dd0: 2020 2020 2020 2066 2e77 7269 7465 2827         f.write('
-00001de0: 6d6f 7573 6520 3d20 2720 2b20 7374 7228  mouse = ' + str(
-00001df0: 696e 7428 7365 6c66 2e5f 6d6f 7573 6529  int(self._mouse)
-00001e00: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
-00001e10: 6620 7365 6c66 2e5f 6465 6275 673a 2020  f self._debug:  
-00001e20: 2320 6966 2074 6865 2064 6562 7567 2069  # if the debug i
-00001e30: 7320 666f 7263 6564 2c20 7772 6974 6520  s forced, write 
-00001e40: 6974 0a20 2020 2020 2020 2020 2020 2020  it.             
-00001e50: 2020 2066 2e77 7269 7465 2827 5c6e 6465     f.write('\nde
-00001e60: 6275 6720 3d20 2720 2b20 7374 7228 696e  bug = ' + str(in
-00001e70: 7428 7365 6c66 2e5f 6465 6275 6729 2929  t(self._debug)))
-00001e80: 0a0a 2020 2020 6465 6620 7265 6164 6b65  ..    def readke
-00001e90: 7973 2873 656c 6629 3a0a 2020 2020 2020  ys(self):.      
-00001ea0: 2020 7365 6c66 2e5f 6b65 7973 203d 207b    self._keys = {
-00001eb0: 7d0a 2020 2020 2020 2020 6966 2070 6174  }.        if pat
-00001ec0: 682e 6578 6973 7473 2873 656c 662e 5f6b  h.exists(self._k
-00001ed0: 6579 7366 696c 6529 3a0a 2020 2020 2020  eysfile):.      
-00001ee0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00001ef0: 7365 6c66 2e5f 6b65 7973 6669 6c65 2920  self._keysfile) 
-00001f00: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
-00001f10: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
-00001f20: 6e20 663a 0a20 2020 2020 2020 2020 2020  n f:.           
-00001f30: 2020 2020 2020 2020 2023 2066 696e 6420           # find 
-00001f40: 7365 7061 7261 746f 7220 6265 7477 6565  separator betwee
-00001f50: 6e20 6b65 7977 6f72 6420 616e 6420 6b65  n keyword and ke
-00001f60: 7973 0a20 2020 2020 2020 2020 2020 2020  ys.             
-00001f70: 2020 2020 2020 2069 6e64 203d 206c 696e         ind = lin
-00001f80: 652e 6669 6e64 2822 3a22 290a 2020 2020  e.find(":").    
-00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fa0: 6b65 7977 6f72 6420 3d20 6c69 6e65 5b3a  keyword = line[:
-00001fb0: 696e 645d 0a20 2020 2020 2020 2020 2020  ind].           
-00001fc0: 2020 2020 2020 2020 2023 202b 3120 6967           # +1 ig
-00001fd0: 6e6f 7265 203a 2c20 2d31 2069 676e 6f72  nore :, -1 ignor
-00001fe0: 6520 6669 6e61 6c20 5c6e 0a20 2020 2020  e final \n.     
-00001ff0: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00002000: 6579 7320 3d20 6c69 6e65 5b69 6e64 2b31  eys = line[ind+1
-00002010: 3a2d 315d 2e72 6570 6c61 6365 2822 2022  :-1].replace(" "
-00002020: 2c20 2222 292e 7370 6c69 7428 222c 2229  , "").split(",")
-00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002040: 2020 2020 2069 6620 2253 5041 4345 2220       if "SPACE" 
-00002050: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 206b 6579 732e 6170 7065 6e64 2822 2022   keys.append(" "
-00002080: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002090: 2020 2020 2020 2020 2020 6b65 7973 2e72            keys.r
-000020a0: 656d 6f76 6528 2253 5041 4345 2229 0a20  emove("SPACE"). 
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2020 2073 656c 662e 5f6b 6579 735b 6b65     self._keys[ke
-000020d0: 7977 6f72 645d 203d 206b 6579 730a 0a20  yword] = keys.. 
-000020e0: 2020 2020 2020 2023 2063 6865 636b 2069         # check i
-000020f0: 6620 616c 6c20 6f70 6572 6174 696f 6e73  f all operations
-00002100: 2061 7265 2064 6566 696e 6564 2c20 6465   are defined, de
-00002110: 6661 756c 7473 2069 6620 6e65 6564 6564  faults if needed
-00002120: 0a20 2020 2020 2020 206f 6c64 6b65 7973  .        oldkeys
-00002130: 203d 2073 656c 662e 5f6b 6579 732e 636f   = self._keys.co
-00002140: 7079 2829 0a20 2020 2020 2020 2074 7279  py().        try
-00002150: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00002160: 6c66 2e5f 6b65 7973 5b27 7175 6974 275d  lf._keys['quit']
-00002170: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
-00002180: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002190: 662e 5f6b 6579 735b 2771 7569 7427 5d20  f._keys['quit'] 
-000021a0: 3d20 5b27 7127 2c20 2751 275d 0a20 2020  = ['q', 'Q'].   
-000021b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000021c0: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
-000021d0: 5b27 6e65 7874 6461 7927 5d0a 2020 2020  ['nextday'].    
-000021e0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-000021f0: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
-00002200: 7973 5b27 6e65 7874 6461 7927 5d20 3d20  ys['nextday'] = 
-00002210: 5b27 4b45 595f 5249 4748 5427 5d0a 2020  ['KEY_RIGHT'].  
-00002220: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00002230: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
-00002240: 735b 2770 7265 7664 6179 275d 0a20 2020  s['prevday'].   
-00002250: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00002260: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
-00002270: 6579 735b 2770 7265 7664 6179 275d 203d  eys['prevday'] =
-00002280: 205b 274b 4559 5f4c 4546 5427 5d0a 2020   ['KEY_LEFT'].  
-00002290: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000022a0: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
-000022b0: 735b 276e 6578 7477 6565 6b27 5d0a 2020  s['nextweek'].  
-000022c0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-000022d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000022e0: 6b65 7973 5b27 6e65 7874 7765 656b 275d  keys['nextweek']
-000022f0: 203d 205b 274b 4559 5f44 4f57 4e27 5d0a   = ['KEY_DOWN'].
-00002300: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00002310: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
-00002320: 6579 735b 2770 7265 7677 6565 6b27 5d0a  eys['prevweek'].
-00002330: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-00002340: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002350: 2e5f 6b65 7973 5b27 7072 6576 7765 656b  ._keys['prevweek
-00002360: 275d 203d 205b 274b 4559 5f55 5027 5d0a  '] = ['KEY_UP'].
-00002370: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00002380: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
-00002390: 6579 735b 276e 6578 746d 6f6e 7468 275d  eys['nextmonth']
-000023a0: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
-000023b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000023c0: 662e 5f6b 6579 735b 276e 6578 746d 6f6e  f._keys['nextmon
-000023d0: 7468 275d 203d 205b 276d 275d 0a20 2020  th'] = ['m'].   
-000023e0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000023f0: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
-00002400: 5b27 7072 6576 6d6f 6e74 6827 5d0a 2020  ['prevmonth'].  
-00002410: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00002420: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00002430: 6b65 7973 5b27 7072 6576 6d6f 6e74 6827  keys['prevmonth'
-00002440: 5d20 3d20 5b27 4d27 5d0a 2020 2020 2020  ] = ['M'].      
-00002450: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00002460: 2020 2073 656c 662e 5f6b 6579 735b 276e     self._keys['n
-00002470: 6578 7479 6561 7227 5d0a 2020 2020 2020  extyear'].      
-00002480: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00002490: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
-000024a0: 5b27 6e65 7874 7965 6172 275d 203d 205b  ['nextyear'] = [
-000024b0: 274b 4559 5f50 5041 4745 272c 2027 7927  'KEY_PPAGE', 'y'
-000024c0: 5d0a 2020 2020 2020 2020 7472 793a 0a20  ].        try:. 
-000024d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000024e0: 5f6b 6579 735b 2770 7265 7679 6561 7227  _keys['prevyear'
-000024f0: 5d0a 2020 2020 2020 2020 6578 6365 7074  ].        except
-00002500: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00002510: 6c66 2e5f 6b65 7973 5b27 7072 6576 7965  lf._keys['prevye
-00002520: 6172 275d 203d 205b 274b 4559 5f4e 5041  ar'] = ['KEY_NPA
-00002530: 4745 272c 2027 5927 5d0a 2020 2020 2020  GE', 'Y'].      
-00002540: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00002550: 2020 2073 656c 662e 5f6b 6579 735b 276e     self._keys['n
-00002560: 6578 7465 7665 6e74 275d 0a20 2020 2020  extevent'].     
-00002570: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
-00002580: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
-00002590: 735b 276e 6578 7465 7665 6e74 275d 203d  s['nextevent'] =
-000025a0: 205b 274b 4559 5f45 4e44 272c 2027 0927   ['KEY_END', '.'
-000025b0: 5d20 2023 2074 6162 0a20 2020 2020 2020  ]  # tab.       
-000025c0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-000025d0: 2020 7365 6c66 2e5f 6b65 7973 5b27 7072    self._keys['pr
-000025e0: 6576 6576 656e 7427 5d0a 2020 2020 2020  evevent'].      
-000025f0: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00002600: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
-00002610: 5b27 7072 6576 6576 656e 7427 5d20 3d20  ['prevevent'] = 
-00002620: 5b27 4b45 595f 484f 4d45 272c 2027 4b45  ['KEY_HOME', 'KE
-00002630: 595f 4254 4142 275d 0a20 2020 2020 2020  Y_BTAB'].       
-00002640: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00002650: 2020 7365 6c66 2e5f 6b65 7973 5b27 6465    self._keys['de
-00002660: 6c65 7665 6e74 275d 0a20 2020 2020 2020  levent'].       
-00002670: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00002680: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
-00002690: 2764 656c 6576 656e 7427 5d20 3d20 5b27  'delevent'] = ['
-000026a0: 6427 2c20 2744 275d 0a20 2020 2020 2020  d', 'D'].       
-000026b0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-000026c0: 2020 7365 6c66 2e5f 6b65 7973 5b27 6164    self._keys['ad
-000026d0: 6465 7665 6e74 275d 0a20 2020 2020 2020  devent'].       
-000026e0: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-000026f0: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
-00002700: 2761 6464 6576 656e 7427 5d20 3d20 5b27  'addevent'] = ['
-00002710: 6127 2c20 2741 275d 0a20 2020 2020 2020  a', 'A'].       
-00002720: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00002730: 2020 7365 6c66 2e5f 6b65 7973 5b27 6564    self._keys['ed
-00002740: 6974 6576 656e 7427 5d0a 2020 2020 2020  itevent'].      
-00002750: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00002760: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
-00002770: 5b27 6564 6974 6576 656e 7427 5d20 3d20  ['editevent'] = 
-00002780: 5b27 6527 2c20 2745 275d 0a20 2020 2020  ['e', 'E'].     
-00002790: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000027a0: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
-000027b0: 746f 6767 6c65 5745 275d 0a20 2020 2020  toggleWE'].     
-000027c0: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
-000027d0: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
-000027e0: 735b 2774 6f67 676c 6557 4527 5d20 3d20  s['toggleWE'] = 
-000027f0: 5b27 7727 2c20 2757 275d 0a20 2020 2020  ['w', 'W'].     
-00002800: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00002810: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
-00002820: 7265 6472 6177 275d 0a20 2020 2020 2020  redraw'].       
-00002830: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00002840: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
-00002850: 2772 6564 7261 7727 5d20 3d20 5b27 1227  'redraw'] = ['.'
-00002860: 2c20 270c 275d 0a20 2020 2020 2020 2074  , '.'].        t
-00002870: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00002880: 7365 6c66 2e5f 6b65 7973 5b27 7379 6e63  self._keys['sync
-00002890: 275d 0a20 2020 2020 2020 2065 7863 6570  '].        excep
-000028a0: 743a 0a20 2020 2020 2020 2020 2020 2073  t:.            s
-000028b0: 656c 662e 5f6b 6579 735b 2773 796e 6327  elf._keys['sync'
-000028c0: 5d20 3d20 5b27 1627 5d0a 2020 2020 2020  ] = ['.'].      
-000028d0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-000028e0: 2020 2073 656c 662e 5f6b 6579 735b 2773     self._keys['s
-000028f0: 6176 6527 5d0a 2020 2020 2020 2020 6578  ave'].        ex
-00002900: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
-00002910: 2020 7365 6c66 2e5f 6b65 7973 5b27 7361    self._keys['sa
-00002920: 7665 275d 203d 205b 2773 272c 2027 5327  ve'] = ['s', 'S'
-00002930: 5d0a 2020 2020 2020 2020 7472 793a 0a20  ].        try:. 
-00002940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002950: 5f6b 6579 735b 2769 6d70 6f72 7427 5d0a  _keys['import'].
-00002960: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-00002970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002980: 2e5f 6b65 7973 5b27 696d 706f 7274 275d  ._keys['import']
-00002990: 203d 205b 2769 272c 2027 4927 5d0a 2020   = ['i', 'I'].  
-000029a0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000029b0: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
-000029c0: 735b 2765 7870 6f72 7427 5d0a 2020 2020  s['export'].    
-000029d0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-000029e0: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
-000029f0: 7973 5b27 6578 706f 7274 275d 203d 205b  ys['export'] = [
-00002a00: 2778 272c 2027 5827 5d0a 2020 2020 2020  'x', 'X'].      
-00002a10: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00002a20: 2020 2073 656c 662e 5f6b 6579 735b 2774     self._keys['t
-00002a30: 6f64 6179 275d 0a20 2020 2020 2020 2065  oday'].        e
-00002a40: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-00002a50: 2020 2073 656c 662e 5f6b 6579 735b 2774     self._keys['t
-00002a60: 6f64 6179 275d 203d 205b 2707 275d 0a20  oday'] = ['.']. 
-00002a70: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00002a80: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
-00002a90: 7973 5b27 7365 7464 6179 275d 0a20 2020  ys['setday'].   
-00002aa0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00002ab0: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
-00002ac0: 6579 735b 2773 6574 6461 7927 5d20 3d20  eys['setday'] = 
-00002ad0: 5b27 6727 2c20 2747 275d 0a20 2020 2020  ['g', 'G'].     
-00002ae0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00002af0: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
-00002b00: 7374 6172 7477 6565 6b27 5d0a 2020 2020  startweek'].    
-00002b10: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-00002b20: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
-00002b30: 7973 5b27 7374 6172 7477 6565 6b27 5d20  ys['startweek'] 
-00002b40: 3d20 5b27 3027 5d0a 2020 2020 2020 2020  = ['0'].        
-00002b50: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00002b60: 2073 656c 662e 5f6b 6579 735b 2765 6e64   self._keys['end
-00002b70: 7765 656b 275d 0a20 2020 2020 2020 2065  week'].        e
-00002b80: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-00002b90: 2020 2073 656c 662e 5f6b 6579 735b 2765     self._keys['e
-00002ba0: 6e64 7765 656b 275d 203d 205b 2724 275d  ndweek'] = ['$']
-00002bb0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00002bc0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00002bd0: 6b65 7973 5b27 6865 6c70 275d 0a20 2020  keys['help'].   
-00002be0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00002bf0: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
-00002c00: 6579 735b 2768 656c 7027 5d20 3d20 5b27  eys['help'] = ['
-00002c10: 6827 2c20 2748 275d 0a20 2020 2020 2020  h', 'H'].       
-00002c20: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00002c30: 2020 7365 6c66 2e5f 6b65 7973 5b27 7461    self._keys['ta
-00002c40: 6765 7665 6e74 275d 0a20 2020 2020 2020  gevent'].       
-00002c50: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00002c60: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
-00002c70: 2774 6167 6576 656e 7427 5d20 3d20 5b27  'tagevent'] = ['
-00002c80: 7427 2c20 2754 272c 2027 7c27 5d0a 2020  t', 'T', '|'].  
-00002c90: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00002ca0: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
-00002cb0: 735b 2763 6f70 7965 7665 6e74 275d 0a20  s['copyevent']. 
-00002cc0: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
-00002cd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002ce0: 5f6b 6579 735b 2763 6f70 7965 7665 6e74  _keys['copyevent
-00002cf0: 275d 203d 205b 2770 272c 2027 5027 5d0a  '] = ['p', 'P'].
-00002d00: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00002d10: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
-00002d20: 6579 735b 276d 696e 7573 7368 6966 7468  eys['minusshifth
-00002d30: 6f75 7227 5d0a 2020 2020 2020 2020 6578  our'].        ex
-00002d40: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
-00002d50: 2020 7365 6c66 2e5f 6b65 7973 5b27 6d69    self._keys['mi
-00002d60: 6e75 7373 6869 6674 686f 7572 275d 203d  nusshifthour'] =
-00002d70: 205b 272d 275d 0a20 2020 2020 2020 2074   ['-'].        t
-00002d80: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00002d90: 7365 6c66 2e5f 6b65 7973 5b27 7368 6966  self._keys['shif
-00002da0: 7468 6f75 7227 5d0a 2020 2020 2020 2020  thour'].        
-00002db0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00002dc0: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
-00002dd0: 7368 6966 7468 6f75 7227 5d20 3d20 5b27  shifthour'] = ['
-00002de0: 2b27 5d0a 2020 2020 2020 2020 7472 793a  +'].        try:
-00002df0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002e00: 662e 5f6b 6579 735b 276d 696e 7573 7368  f._keys['minussh
-00002e10: 6966 7464 6179 275d 0a20 2020 2020 2020  iftday'].       
-00002e20: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00002e30: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
-00002e40: 276d 696e 7573 7368 6966 7464 6179 275d  'minusshiftday']
-00002e50: 203d 205b 272f 275d 0a20 2020 2020 2020   = ['/'].       
-00002e60: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00002e70: 2020 7365 6c66 2e5f 6b65 7973 5b27 7368    self._keys['sh
-00002e80: 6966 7464 6179 275d 0a20 2020 2020 2020  iftday'].       
-00002e90: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00002ea0: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
-00002eb0: 2773 6869 6674 6461 7927 5d20 3d20 5b27  'shiftday'] = ['
-00002ec0: 2a27 5d0a 2020 2020 2020 2020 7472 793a  *'].        try:
-00002ed0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002ee0: 662e 5f6b 6579 735b 2773 6574 636f 6e66  f._keys['setconf
-00002ef0: 6967 275d 0a20 2020 2020 2020 2065 7863  ig'].        exc
-00002f00: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-00002f10: 2073 656c 662e 5f6b 6579 735b 2773 6574   self._keys['set
-00002f20: 636f 6e66 6967 275d 203d 205b 2763 272c  config'] = ['c',
-00002f30: 2027 4327 5d0a 2020 2020 2020 2020 7472   'C'].        tr
-00002f40: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00002f50: 656c 662e 5f6b 6579 735b 2774 6f67 676c  elf._keys['toggl
-00002f60: 6574 6f64 6f27 5d0a 2020 2020 2020 2020  etodo'].        
-00002f70: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00002f80: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
-00002f90: 746f 6767 6c65 746f 646f 275d 203d 205b  toggletodo'] = [
-00002fa0: 2714 275d 0a0a 2020 2020 2020 2020 6966  '.']..        if
-00002fb0: 206c 656e 2873 656c 662e 5f6b 6579 7329   len(self._keys)
-00002fc0: 203e 206c 656e 286f 6c64 6b65 7973 293a   > len(oldkeys):
-00002fd0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-00002fe0: 6620 6120 6465 6661 756c 7420 636f 6e66  f a default conf
-00002ff0: 6967 7572 6174 696f 6e20 6861 7320 6265  iguration has be
-00003000: 656e 2075 7365 640a 2020 2020 2020 2020  en used.        
-00003010: 2020 2020 7365 6c66 2e77 7269 7465 6b65      self.writeke
-00003020: 7973 2829 0a0a 2020 2020 6465 6620 7772  ys()..    def wr
-00003030: 6974 656b 6579 7328 7365 6c66 293a 0a20  itekeys(self):. 
-00003040: 2020 2020 2020 206c 696e 6573 203d 2022         lines = "
-00003050: 220a 2020 2020 2020 2020 2320 6f72 6465  ".        # orde
-00003060: 7265 6420 6c69 7374 206f 6620 6974 656d  red list of item
-00003070: 730a 2020 2020 2020 2020 6b65 7977 6f72  s.        keywor
-00003080: 6473 203d 205b 276e 6578 7464 6179 272c  ds = ['nextday',
-00003090: 2027 7072 6576 6461 7927 2c20 276e 6578   'prevday', 'nex
-000030a0: 7477 6565 6b27 2c20 2770 7265 7677 6565  tweek', 'prevwee
-000030b0: 6b27 2c0a 2020 2020 2020 2020 2020 2020  k',.            
-000030c0: 2020 2020 2020 2020 276e 6578 746d 6f6e          'nextmon
-000030d0: 7468 272c 2027 7072 6576 6d6f 6e74 6827  th', 'prevmonth'
-000030e0: 2c20 276e 6578 7479 6561 7227 2c20 2770  , 'nextyear', 'p
-000030f0: 7265 7679 6561 7227 2c0a 2020 2020 2020  revyear',.      
-00003100: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-00003110: 6578 7465 7665 6e74 272c 2027 7072 6576  extevent', 'prev
-00003120: 6576 656e 7427 2c20 2764 656c 6576 656e  event', 'deleven
-00003130: 7427 2c20 2761 6464 6576 656e 7427 2c0a  t', 'addevent',.
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 2020 2020 2765 6469 7465 7665 6e74 272c      'editevent',
-00003160: 2027 746f 6767 6c65 5745 272c 2027 7175   'toggleWE', 'qu
-00003170: 6974 272c 2027 7265 6472 6177 272c 2027  it', 'redraw', '
-00003180: 7379 6e63 272c 2027 7361 7665 272c 0a20  sync', 'save',. 
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2027 696d 706f 7274 272c 2027 6578     'import', 'ex
-000031b0: 706f 7274 272c 2027 746f 6461 7927 2c20  port', 'today', 
-000031c0: 2773 6574 6461 7927 2c20 2773 7461 7274  'setday', 'start
-000031d0: 7765 656b 272c 0a20 2020 2020 2020 2020  week',.         
-000031e0: 2020 2020 2020 2020 2020 2027 656e 6477             'endw
-000031f0: 6565 6b27 2c20 2768 656c 7027 2c20 2774  eek', 'help', 't
-00003200: 6167 6576 656e 7427 2c20 2763 6f70 7965  agevent', 'copye
-00003210: 7665 6e74 272c 0a20 2020 2020 2020 2020  vent',.         
-00003220: 2020 2020 2020 2020 2020 2027 6d69 6e75             'minu
-00003230: 7373 6869 6674 686f 7572 272c 2027 7368  sshifthour', 'sh
-00003240: 6966 7468 6f75 7227 2c20 276d 696e 7573  ifthour', 'minus
-00003250: 7368 6966 7464 6179 272c 2027 7368 6966  shiftday', 'shif
-00003260: 7464 6179 272c 0a20 2020 2020 2020 2020  tday',.         
-00003270: 2020 2020 2020 2020 2020 2027 7365 7463             'setc
-00003280: 6f6e 6669 6727 2c20 2774 6f67 676c 6574  onfig', 'togglet
-00003290: 6f64 6f27 5d0a 2020 2020 2020 2020 666f  odo'].        fo
-000032a0: 7220 6f70 2069 6e20 6b65 7977 6f72 6473  r op in keywords
-000032b0: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
-000032c0: 6e65 203d 206f 7020 2b20 223a 2022 0a20  ne = op + ": ". 
-000032d0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-000032e0: 2069 6e20 7365 6c66 2e5f 6b65 7973 5b6f   in self._keys[o
-000032f0: 705d 3a0a 2020 2020 2020 2020 2020 2020  p]:.            
-00003300: 2020 2020 6966 206b 203d 3d20 2220 223a      if k == " ":
-00003310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003320: 2020 2020 206b 203d 2022 5350 4143 4522       k = "SPACE"
-00003330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003340: 206c 696e 6520 3d20 6c69 6e65 202b 206b   line = line + k
-00003350: 202b 2022 2c20 220a 2020 2020 2020 2020   + ", ".        
-00003360: 2020 2020 2320 7265 706c 6163 6520 6c61      # replace la
-00003370: 7374 2063 6f6d 6d61 2061 6e64 2073 7061  st comma and spa
-00003380: 6365 2062 7920 6120 6e65 776c 696e 650a  ce by a newline.
-00003390: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-000033a0: 203d 206c 696e 655b 3a2d 325d 202b 2022   = line[:-2] + "
-000033b0: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-000033c0: 6c69 6e65 7320 2b3d 206c 696e 650a 2020  lines += line.  
-000033d0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-000033e0: 7365 6c66 2e5f 6b65 7973 6669 6c65 2c20  self._keysfile, 
-000033f0: 2277 2229 2061 7320 663a 0a20 2020 2020  "w") as f:.     
-00003400: 2020 2020 2020 2066 2e77 7269 7465 286c         f.write(l
-00003410: 696e 6573 290a 0a20 2020 2064 6566 2072  ines)..    def r
-00003420: 6561 6463 6f6c 6f75 7273 2873 656c 6629  eadcolours(self)
-00003430: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00003440: 2870 6174 682e 6578 6973 7473 2873 656c  (path.exists(sel
-00003450: 662e 5f63 6f6c 6f75 7273 6669 6c65 2929  f._coloursfile))
-00003460: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00003470: 6465 6661 756c 7473 2061 6e64 2077 7269  defaults and wri
-00003480: 7465 2066 696c 650a 2020 2020 2020 2020  te file.        
-00003490: 2020 2020 7365 6c66 2e5f 636f 6c6f 7572      self._colour
-000034a0: 735f 6964 7820 3d20 7261 6e67 6528 3829  s_idx = range(8)
-000034b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000034c0: 662e 7772 6974 6563 6f6c 6f75 7273 2829  f.writecolours()
-000034d0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000034e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000034f0: 5f63 6f6c 6f75 7273 5f69 6478 203d 205b  _colours_idx = [
-00003500: 5d0a 2020 2020 2020 2020 2020 2020 7769  ].            wi
-00003510: 7468 206f 7065 6e28 7365 6c66 2e5f 636f  th open(self._co
-00003520: 6c6f 7572 7366 696c 6529 2061 7320 663a  loursfile) as f:
-00003530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003540: 2066 6f72 206c 696e 6520 696e 2066 3a0a   for line in f:.
-00003550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003560: 2020 2020 7365 6c66 2e5f 636f 6c6f 7572      self._colour
-00003570: 735f 6964 782e 6170 7065 6e64 2869 6e74  s_idx.append(int
-00003580: 286c 696e 6529 290a 0a20 2020 2064 6566  (line))..    def
-00003590: 2077 7269 7465 636f 6c6f 7572 7328 7365   writecolours(se
-000035a0: 6c66 293a 0a20 2020 2020 2020 206c 696e  lf):.        lin
-000035b0: 6573 203d 2022 220a 2020 2020 2020 2020  es = "".        
-000035c0: 666f 7220 636f 6c6f 7572 5f69 6478 2069  for colour_idx i
-000035d0: 6e20 7365 6c66 2e5f 636f 6c6f 7572 735f  n self._colours_
-000035e0: 6964 783a 0a20 2020 2020 2020 2020 2020  idx:.           
-000035f0: 206c 696e 6573 202b 3d20 7374 7228 636f   lines += str(co
-00003600: 6c6f 7572 5f69 6478 2920 2b20 225c 6e22  lour_idx) + "\n"
-00003610: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-00003620: 656e 2873 656c 662e 5f63 6f6c 6f75 7273  en(self._colours
-00003630: 6669 6c65 2c20 2277 2229 2061 7320 663a  file, "w") as f:
-00003640: 0a20 2020 2020 2020 2020 2020 2066 2e77  .            f.w
-00003650: 7269 7465 286c 696e 6573 290a 0a20 2020  rite(lines)..   
-00003660: 2064 6566 2073 6574 636f 6c6f 7572 7328   def setcolours(
-00003670: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00003680: 656c 662e 5f63 6f6c 6f75 7273 203d 205b  elf._colours = [
-00003690: 5d0a 2020 2020 2020 2020 2320 6465 6669  ].        # defi
-000036a0: 6e65 2074 6865 2065 6967 6874 2063 6f6c  ne the eight col
-000036b0: 6f75 7273 0a20 2020 2020 2020 2066 6f72  ours.        for
-000036c0: 2069 2069 6e20 7261 6e67 6528 3829 3a0a   i in range(8):.
-000036d0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000036e0: 2020 2320 7468 6520 7465 726d 696e 616c    # the terminal
-000036f0: 2068 6173 2061 2064 6566 6175 6c74 2062   has a default b
-00003700: 6163 6b67 726f 756e 640a 2020 2020 2020  ackground.      
-00003710: 2020 2020 2020 2020 2020 6375 7273 6573            curses
-00003720: 2e69 6e69 745f 7061 6972 2869 2c20 692c  .init_pair(i, i,
-00003730: 202d 3129 0a20 2020 2020 2020 2020 2020   -1).           
-00003740: 2065 7863 6570 743a 2020 2320 6465 6661   except:  # defa
-00003750: 756c 7473 2074 6f20 626c 6163 6b0a 2020  ults to black.  
-00003760: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00003770: 7273 6573 2e69 6e69 745f 7061 6972 2869  rses.init_pair(i
-00003780: 2c20 692c 2030 290a 2020 2020 2020 2020  , i, 0).        
-00003790: 666f 7220 6964 7820 696e 2073 656c 662e  for idx in self.
-000037a0: 5f63 6f6c 6f75 7273 5f69 6478 3a0a 2020  _colours_idx:.  
-000037b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000037c0: 636f 6c6f 7572 732e 6170 7065 6e64 2863  colours.append(c
-000037d0: 7572 7365 732e 636f 6c6f 725f 7061 6972  urses.color_pair
-000037e0: 2869 6478 2929 0a0a 2020 2020 6465 6620  (idx))..    def 
-000037f0: 7265 6164 6361 7465 676f 7269 6573 2873  readcategories(s
-00003800: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00003810: 6c66 2e5f 6361 7465 676f 7269 6573 203d  lf._categories =
-00003820: 207b 7d0a 2020 2020 2020 2020 6966 206e   {}.        if n
-00003830: 6f74 2870 6174 682e 6578 6973 7473 2873  ot(path.exists(s
-00003840: 656c 662e 5f63 6174 6567 6f72 6965 7366  elf._categoriesf
-00003850: 696c 6529 293a 0a20 2020 2020 2020 2020  ile)):.         
-00003860: 2020 2023 2064 6566 6175 6c74 7320 616e     # defaults an
-00003870: 6420 7772 6974 6520 6669 6c65 0a20 2020  d write file.   
-00003880: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00003890: 6e20 7261 6e67 6528 312c 2038 293a 0a20  n range(1, 8):. 
-000038a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000038b0: 656c 662e 5f63 6174 6567 6f72 6965 735b  elf._categories[
-000038c0: 695d 203d 205b 7374 7228 6929 5d0a 2020  i] = [str(i)].  
-000038d0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-000038e0: 7269 7465 6361 7465 676f 7269 6573 2829  ritecategories()
-000038f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00003900: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00003910: 6f70 656e 2873 656c 662e 5f63 6174 6567  open(self._categ
-00003920: 6f72 6965 7366 696c 6529 2061 7320 663a  oriesfile) as f:
-00003930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003940: 2066 6f72 2069 6478 2c20 6c69 6e65 2069   for idx, line i
-00003950: 6e20 656e 756d 6572 6174 6528 6629 3a0a  n enumerate(f):.
-00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003970: 2020 2020 6361 7420 3d20 6c69 6e65 5b3a      cat = line[:
-00003980: 2d31 5d2e 7265 706c 6163 6528 222c 2022  -1].replace(", "
-00003990: 2c20 222c 2229 2e73 706c 6974 2822 2c22  , ",").split(","
-000039a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000039b0: 2020 2020 2020 2320 2d31 2074 6f20 6967        # -1 to ig
-000039c0: 6e6f 7265 2066 696e 616c 205c 6e0a 2020  nore final \n.  
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039e0: 2020 7365 6c66 2e5f 6361 7465 676f 7269    self._categori
-000039f0: 6573 5b69 6478 2b31 5d20 3d20 6361 740a  es[idx+1] = cat.
-00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a10: 2020 2020 2320 2b31 3a20 6361 7465 676f      # +1: catego
-00003a20: 7279 2030 2069 7320 6465 6661 756c 7473  ry 0 is defaults
-00003a30: 0a0a 2020 2020 6465 6620 7772 6974 6563  ..    def writec
-00003a40: 6174 6567 6f72 6965 7328 7365 6c66 293a  ategories(self):
-00003a50: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
-00003a60: 2022 220a 2020 2020 2020 2020 666f 7220   "".        for 
-00003a70: 7461 676e 6220 696e 2072 616e 6765 2831  tagnb in range(1
-00003a80: 2c20 3829 3a0a 2020 2020 2020 2020 2020  , 8):.          
-00003a90: 2020 6c69 6e65 203d 2022 220a 2020 2020    line = "".    
-00003aa0: 2020 2020 2020 2020 666f 7220 6361 7420          for cat 
-00003ab0: 696e 2073 656c 662e 5f63 6174 6567 6f72  in self._categor
-00003ac0: 6965 735b 7461 676e 625d 3a0a 2020 2020  ies[tagnb]:.    
-00003ad0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00003ae0: 203d 206c 696e 6520 2b20 6361 7420 2b20   = line + cat + 
-00003af0: 222c 2022 0a20 2020 2020 2020 2020 2020  ", ".           
-00003b00: 2023 2072 6570 6c61 6365 206c 6173 7420   # replace last 
-00003b10: 636f 6d6d 6120 616e 6420 7370 6163 6520  comma and space 
-00003b20: 6279 2061 206e 6577 6c69 6e65 0a20 2020  by a newline.   
-00003b30: 2020 2020 2020 2020 206c 696e 6520 3d20           line = 
-00003b40: 6c69 6e65 5b3a 2d32 5d20 2b20 225c 6e22  line[:-2] + "\n"
-00003b50: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
-00003b60: 6573 202b 3d20 6c69 6e65 0a20 2020 2020  es += line.     
-00003b70: 2020 2077 6974 6820 6f70 656e 2873 656c     with open(sel
-00003b80: 662e 5f63 6174 6567 6f72 6965 7366 696c  f._categoriesfil
-00003b90: 652c 2022 7722 2920 6173 2066 3a0a 2020  e, "w") as f:.  
-00003ba0: 2020 2020 2020 2020 2020 662e 7772 6974            f.writ
-00003bb0: 6528 6c69 6e65 7329 0a0a 2020 2020 6465  e(lines)..    de
-00003bc0: 6620 7265 6164 6361 6c64 6176 2873 656c  f readcaldav(sel
-00003bd0: 6629 3a0a 2020 2020 2020 2020 6966 2070  f):.        if p
-00003be0: 6174 682e 6578 6973 7473 2873 656c 662e  ath.exists(self.
-00003bf0: 5f63 616c 6461 7666 696c 6529 3a0a 2020  _caldavfile):.  
-00003c00: 2020 2020 2020 2020 2020 7769 7468 206f            with o
-00003c10: 7065 6e28 7365 6c66 2e5f 6361 6c64 6176  pen(self._caldav
-00003c20: 6669 6c65 2920 6173 2066 3a0a 2020 2020  file) as f:.    
-00003c30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00003c40: 6c69 6e65 2069 6e20 663a 0a20 2020 2020  line in f:.     
-00003c50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003c60: 6461 7620 3d20 7b7d 2020 2320 696e 6974  dav = {}  # init
-00003c70: 6961 7465 2074 6865 2064 6963 740a 2020  iate the dict.  
-00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c90: 2020 656e 6475 726c 203d 206c 696e 652e    endurl = line.
-00003ca0: 6669 6e64 2822 2c20 7573 6572 6e61 6d65  find(", username
-00003cb0: 3d22 290a 2020 2020 2020 2020 2020 2020  =").            
-00003cc0: 2020 2020 2020 2020 656e 6475 7365 726e          endusern
-00003cd0: 616d 6520 3d20 6c69 6e65 2e66 696e 6428  ame = line.find(
-00003ce0: 222c 2070 6173 7377 6f72 643d 2229 0a20  ", password="). 
-00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d00: 2020 2065 6e64 7061 7373 776f 7264 203d     endpassword =
-00003d10: 206c 696e 652e 6669 6e64 2822 2c20 7461   line.find(", ta
-00003d20: 673d 2229 0a20 2020 2020 2020 2020 2020  g=").           
-00003d30: 2020 2020 2020 2020 2065 6e64 7461 6720           endtag 
-00003d40: 3d20 6c69 6e65 2e66 696e 6428 222c 2063  = line.find(", c
-00003d50: 6f6c 6f75 723d 2229 0a20 2020 2020 2020  olour=").       
-00003d60: 2020 2020 2020 2020 2020 2020 2023 2035               # 5
-00003d70: 2074 6f20 736b 6970 2074 6865 2073 7461   to skip the sta
-00003d80: 7274 696e 6720 2027 7572 6c3d 2227 0a20  rting  'url="'. 
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2020 2075 726c 203d 206c 696e 655b 353a     url = line[5:
-00003db0: 656e 6475 726c 2d31 5d0a 2020 2020 2020  endurl-1].      
-00003dc0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00003dd0: 6973 2074 6865 7265 2061 2070 6173 7377  is there a passw
-00003de0: 6f72 643f 0a20 2020 2020 2020 2020 2020  ord?.           
-00003df0: 2020 2020 2020 2020 2069 6620 656e 6475           if endu
-00003e00: 7365 726e 616d 6520 2d20 656e 6475 726c  sername - endurl
-00003e10: 203e 2031 333a 0a20 2020 2020 2020 2020   > 13:.         
-00003e20: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00003e30: 7365 726e 616d 6520 3d20 6c69 6e65 5b65  sername = line[e
-00003e40: 6e64 7572 6c2b 3132 3a65 6e64 7573 6572  ndurl+12:enduser
-00003e50: 6e61 6d65 2d31 5d0a 2020 2020 2020 2020  name-1].        
-00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e70: 7061 7373 776f 7264 203d 206c 696e 655b  password = line[
-00003e80: 656e 6475 7365 726e 616d 652b 3132 3a65  endusername+12:e
-00003e90: 6e64 7061 7373 776f 7264 2d31 5d0a 2020  ndpassword-1].  
-00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003eb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001690: 2020 6966 206c 696e 655b 303a 375d 203d    if line[0:7] =
+000016a0: 3d20 2768 6d69 6e20 3d20 273a 0a20 2020  = 'hmin = ':.   
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2020 2020 2023 2064 6f6e 2774 2075 7365       # don't use
+000016d0: 2074 6865 2073 6574 7465 7220 746f 2068   the setter to h
+000016e0: 6176 6520 6e6f 206c 696d 6974 206f 6e20  ave no limit on 
+000016f0: 686d 696e 0a20 2020 2020 2020 2020 2020  hmin.           
+00001700: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001710: 662e 5f68 6d69 6e20 3d20 696e 7428 6c69  f._hmin = int(li
+00001720: 6e65 5b37 3a39 5d29 0a20 2020 2020 2020  ne[7:9]).       
+00001730: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00001740: 6c69 6e65 5b30 3a37 5d20 3d3d 2027 686d  line[0:7] == 'hm
+00001750: 6178 203d 2027 3a0a 2020 2020 2020 2020  ax = ':.        
+00001760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001770: 2320 7573 6520 7468 6520 7365 7474 6572  # use the setter
+00001780: 2074 6f20 6265 2073 7572 6520 746f 2062   to be sure to b
+00001790: 6520 6869 6768 6572 2074 6861 6e20 686d  e higher than hm
+000017a0: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
+000017b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000017c0: 686d 6178 203d 2069 6e74 286c 696e 655b  hmax = int(line[
+000017d0: 373a 395d 290a 2020 2020 2020 2020 2020  7:9]).          
+000017e0: 2020 2020 2020 2020 2020 6966 206c 696e            if lin
+000017f0: 655b 303a 355d 203d 3d20 2757 4520 3d20  e[0:5] == 'WE = 
+00001800: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+00001810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001820: 5f57 4520 3d20 626f 6f6c 2869 6e74 286c  _WE = bool(int(l
+00001830: 696e 655b 355d 2929 2020 2320 2230 2220  ine[5]))  # "0" 
+00001840: 746f 2030 2074 6f20 4661 6c73 650a 2020  to 0 to False.  
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 2020 6966 206c 696e 655b 303a 3131 5d20    if line[0:11] 
+00001870: 3d3d 2027 6175 746f 7361 7665 203d 2027  == 'autosave = '
+00001880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001890: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000018a0: 6175 746f 7361 7665 203d 2062 6f6f 6c28  autosave = bool(
+000018b0: 696e 7428 6c69 6e65 5b31 315d 2929 0a20  int(line[11])). 
+000018c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018d0: 2020 2069 6620 6c69 6e65 5b30 3a31 325d     if line[0:12]
+000018e0: 203d 3d20 2763 6f6c 6f75 7273 6574 203d   == 'colourset =
+000018f0: 2027 3a0a 2020 2020 2020 2020 2020 2020   ':.            
+00001900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001910: 2e5f 636f 6c6f 7572 7365 7420 3d20 696e  ._colourset = in
+00001920: 7428 6c69 6e65 5b31 325d 290a 2020 2020  t(line[12]).    
+00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001940: 6966 206c 696e 655b 303a 3131 5d20 3d3d  if line[0:11] ==
+00001950: 2027 6175 746f 7379 6e63 203d 2027 3a0a   'autosync = ':.
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2020 2020 2020 7365 6c66 2e5f 6175          self._au
+00001980: 746f 7379 6e63 203d 2062 6f6f 6c28 696e  tosync = bool(in
+00001990: 7428 6c69 6e65 5b31 315d 2929 0a20 2020  t(line[11])).   
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2069 6620 6c69 6e65 5b30 3a38 5d20 3d3d   if line[0:8] ==
+000019c0: 2027 6465 6275 6720 3d20 273a 0a20 2020   'debug = ':.   
+000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019e0: 2020 2020 2073 656c 662e 5f64 6562 7567       self._debug
+000019f0: 203d 2062 6f6f 6c28 696e 7428 6c69 6e65   = bool(int(line
+00001a00: 5b38 5d29 290a 2020 2020 2020 2020 2020  [8])).          
+00001a10: 2020 2020 2020 2020 2020 6966 206c 696e            if lin
+00001a20: 655b 303a 375d 203d 3d20 2774 6f64 6f20  e[0:7] == 'todo 
+00001a30: 3d20 273a 0a20 2020 2020 2020 2020 2020  = ':.           
+00001a40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001a50: 662e 5f74 6f64 6f20 3d20 626f 6f6c 2869  f._todo = bool(i
+00001a60: 6e74 286c 696e 655b 375d 2929 0a20 2020  nt(line[7])).   
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2069 6620 6c69 6e65 5b30 3a31 325d 203d   if line[0:12] =
+00001a90: 3d20 2774 6f64 6f77 6964 7468 203d 2027  = 'todowidth = '
+00001aa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00001ab0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00001ac0: 746f 646f 7769 6474 6820 3d20 666c 6f61  todowidth = floa
+00001ad0: 7428 6c69 6e65 5b31 323a 5d29 0a20 2020  t(line[12:]).   
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001af0: 2069 6620 6c69 6e65 5b30 3a38 5d20 3d3d   if line[0:8] ==
+00001b00: 2027 6d6f 7573 6520 3d20 273a 0a20 2020   'mouse = ':.   
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 2020 2020 2073 656c 662e 6d6f 7573 6520       self.mouse 
+00001b30: 3d20 626f 6f6c 2869 6e74 286c 696e 655b  = bool(int(line[
+00001b40: 383a 5d29 290a 2020 2020 2020 2020 2020  8:])).          
+00001b50: 2020 2020 2020 2320 544f 444f 3a20 6368        # TODO: ch
+00001b60: 6563 6b20 6966 2061 6c6c 2069 7320 6669  eck if all is fi
+00001b70: 6e65 0a0a 2020 2020 6465 6620 7772 6974  ne..    def writ
+00001b80: 6563 6f6e 6628 7365 6c66 293a 0a20 2020  econf(self):.   
+00001b90: 2020 2020 2077 6974 6820 6f70 656e 2873       with open(s
+00001ba0: 656c 662e 5f63 6f6e 6669 6766 696c 652c  elf._configfile,
+00001bb0: 2022 7722 2920 6173 2066 3a0a 2020 2020   "w") as f:.    
+00001bc0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00001bd0: 2768 6d69 6e20 3d20 2720 2b20 7374 7228  'hmin = ' + str(
+00001be0: 7365 6c66 2e5f 686d 696e 2920 2b20 275c  self._hmin) + '\
+00001bf0: 6e27 290a 2020 2020 2020 2020 2020 2020  n').            
+00001c00: 662e 7772 6974 6528 2768 6d61 7820 3d20  f.write('hmax = 
+00001c10: 2720 2b20 7374 7228 7365 6c66 2e5f 686d  ' + str(self._hm
+00001c20: 6178 2920 2b20 275c 6e27 290a 2020 2020  ax) + '\n').    
+00001c30: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00001c40: 2757 4520 3d20 2720 2b20 7374 7228 696e  'WE = ' + str(in
+00001c50: 7428 7365 6c66 2e5f 5745 2929 202b 2027  t(self._WE)) + '
+00001c60: 5c6e 2729 0a20 2020 2020 2020 2020 2020  \n').           
+00001c70: 2066 2e77 7269 7465 2827 6175 746f 7361   f.write('autosa
+00001c80: 7665 203d 2027 202b 2073 7472 2869 6e74  ve = ' + str(int
+00001c90: 2873 656c 662e 5f61 7574 6f73 6176 6529  (self._autosave)
+00001ca0: 2920 2b20 275c 6e27 290a 2020 2020 2020  ) + '\n').      
+00001cb0: 2020 2020 2020 662e 7772 6974 6528 2763        f.write('c
+00001cc0: 6f6c 6f75 7273 6574 203d 2027 202b 2073  olourset = ' + s
+00001cd0: 7472 2873 656c 662e 5f63 6f6c 6f75 7273  tr(self._colours
+00001ce0: 6574 2920 2b20 275c 6e27 290a 2020 2020  et) + '\n').    
+00001cf0: 2020 2020 2020 2020 662e 7772 6974 6528          f.write(
+00001d00: 2761 7574 6f73 796e 6320 3d20 2720 2b20  'autosync = ' + 
+00001d10: 7374 7228 696e 7428 7365 6c66 2e5f 6175  str(int(self._au
+00001d20: 746f 7379 6e63 2929 2b27 5c6e 2729 0a20  tosync))+'\n'). 
+00001d30: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00001d40: 7465 2827 746f 646f 203d 2027 202b 2073  te('todo = ' + s
+00001d50: 7472 2869 6e74 2873 656c 662e 5f74 6f64  tr(int(self._tod
+00001d60: 6f29 292b 275c 6e27 290a 2020 2020 2020  o))+'\n').      
+00001d70: 2020 2020 2020 662e 7772 6974 6528 2774        f.write('t
+00001d80: 6f64 6f77 6964 7468 203d 2027 202b 2073  odowidth = ' + s
+00001d90: 7472 2873 656c 662e 5f74 6f64 6f77 6964  tr(self._todowid
+00001da0: 7468 292b 275c 6e27 290a 2020 2020 2020  th)+'\n').      
+00001db0: 2020 2020 2020 662e 7772 6974 6528 276d        f.write('m
+00001dc0: 6f75 7365 203d 2027 202b 2073 7472 2869  ouse = ' + str(i
+00001dd0: 6e74 2873 656c 662e 5f6d 6f75 7365 2929  nt(self._mouse))
+00001de0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00001df0: 2073 656c 662e 5f64 6562 7567 3a20 2023   self._debug:  #
+00001e00: 2069 6620 7468 6520 6465 6275 6720 6973   if the debug is
+00001e10: 2066 6f72 6365 642c 2077 7269 7465 2069   forced, write i
+00001e20: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00001e30: 2020 662e 7772 6974 6528 275c 6e64 6562    f.write('\ndeb
+00001e40: 7567 203d 2027 202b 2073 7472 2869 6e74  ug = ' + str(int
+00001e50: 2873 656c 662e 5f64 6562 7567 2929 290a  (self._debug))).
+00001e60: 0a20 2020 2064 6566 2072 6561 646b 6579  .    def readkey
+00001e70: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00001e80: 2073 656c 662e 5f6b 6579 7320 3d20 7b7d   self._keys = {}
+00001e90: 0a20 2020 2020 2020 2069 6620 7061 7468  .        if path
+00001ea0: 2e65 7869 7374 7328 7365 6c66 2e5f 6b65  .exists(self._ke
+00001eb0: 7973 6669 6c65 293a 0a20 2020 2020 2020  ysfile):.       
+00001ec0: 2020 2020 2077 6974 6820 6f70 656e 2873       with open(s
+00001ed0: 656c 662e 5f6b 6579 7366 696c 6529 2061  elf._keysfile) a
+00001ee0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+00001ef0: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+00001f00: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
+00001f10: 2020 2020 2020 2020 2320 6669 6e64 2073          # find s
+00001f20: 6570 6172 6174 6f72 2062 6574 7765 656e  eparator between
+00001f30: 206b 6579 776f 7264 2061 6e64 206b 6579   keyword and key
+00001f40: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00001f50: 2020 2020 2020 696e 6420 3d20 6c69 6e65        ind = line
+00001f60: 2e66 696e 6428 223a 2229 0a20 2020 2020  .find(":").     
+00001f70: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00001f80: 6579 776f 7264 203d 206c 696e 655b 3a69  eyword = line[:i
+00001f90: 6e64 5d0a 2020 2020 2020 2020 2020 2020  nd].            
+00001fa0: 2020 2020 2020 2020 2320 2b31 2069 676e          # +1 ign
+00001fb0: 6f72 6520 3a2c 202d 3120 6967 6e6f 7265  ore :, -1 ignore
+00001fc0: 2066 696e 616c 205c 6e0a 2020 2020 2020   final \n.      
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 6b65                ke
+00001fe0: 7973 203d 206c 696e 655b 696e 642b 313a  ys = line[ind+1:
+00001ff0: 2d31 5d2e 7265 706c 6163 6528 2220 222c  -1].replace(" ",
+00002000: 2022 2229 2e73 706c 6974 2822 2c22 290a   "").split(",").
+00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002020: 2020 2020 6966 2022 5350 4143 4522 2069      if "SPACE" i
+00002030: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002050: 6b65 7973 2e61 7070 656e 6428 2220 2229  keys.append(" ")
+00002060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002070: 2020 2020 2020 2020 206b 6579 732e 7265           keys.re
+00002080: 6d6f 7665 2822 5350 4143 4522 290a 2020  move("SPACE").  
+00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020a0: 2020 7365 6c66 2e5f 6b65 7973 5b6b 6579    self._keys[key
+000020b0: 776f 7264 5d20 3d20 6b65 7973 0a0a 2020  word] = keys..  
+000020c0: 2020 2020 2020 2320 6368 6563 6b20 6966        # check if
+000020d0: 2061 6c6c 206f 7065 7261 7469 6f6e 7320   all operations 
+000020e0: 6172 6520 6465 6669 6e65 642c 2064 6566  are defined, def
+000020f0: 6175 6c74 7320 6966 206e 6565 6465 640a  aults if needed.
+00002100: 2020 2020 2020 2020 6f6c 646b 6579 7320          oldkeys 
+00002110: 3d20 7365 6c66 2e5f 6b65 7973 2e63 6f70  = self._keys.cop
+00002120: 7928 290a 2020 2020 2020 2020 7472 793a  y().        try:
+00002130: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002140: 662e 5f6b 6579 735b 2771 7569 7427 5d0a  f._keys['quit'].
+00002150: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+00002160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002170: 2e5f 6b65 7973 5b27 7175 6974 275d 203d  ._keys['quit'] =
+00002180: 205b 2771 272c 2027 5127 5d0a 2020 2020   ['q', 'Q'].    
+00002190: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000021a0: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
+000021b0: 276e 6578 7464 6179 275d 0a20 2020 2020  'nextday'].     
+000021c0: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+000021d0: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
+000021e0: 735b 276e 6578 7464 6179 275d 203d 205b  s['nextday'] = [
+000021f0: 274b 4559 5f52 4947 4854 275d 0a20 2020  'KEY_RIGHT'].   
+00002200: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00002210: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
+00002220: 5b27 7072 6576 6461 7927 5d0a 2020 2020  ['prevday'].    
+00002230: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+00002240: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
+00002250: 7973 5b27 7072 6576 6461 7927 5d20 3d20  ys['prevday'] = 
+00002260: 5b27 4b45 595f 4c45 4654 275d 0a20 2020  ['KEY_LEFT'].   
+00002270: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00002280: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
+00002290: 5b27 6e65 7874 7765 656b 275d 0a20 2020  ['nextweek'].   
+000022a0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+000022b0: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
+000022c0: 6579 735b 276e 6578 7477 6565 6b27 5d20  eys['nextweek'] 
+000022d0: 3d20 5b27 4b45 595f 444f 574e 275d 0a20  = ['KEY_DOWN']. 
+000022e0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+000022f0: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
+00002300: 7973 5b27 7072 6576 7765 656b 275d 0a20  ys['prevweek']. 
+00002310: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+00002320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002330: 5f6b 6579 735b 2770 7265 7677 6565 6b27  _keys['prevweek'
+00002340: 5d20 3d20 5b27 4b45 595f 5550 275d 0a20  ] = ['KEY_UP']. 
+00002350: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00002360: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
+00002370: 7973 5b27 6e65 7874 6d6f 6e74 6827 5d0a  ys['nextmonth'].
+00002380: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+00002390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000023a0: 2e5f 6b65 7973 5b27 6e65 7874 6d6f 6e74  ._keys['nextmont
+000023b0: 6827 5d20 3d20 5b27 6d27 5d0a 2020 2020  h'] = ['m'].    
+000023c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000023d0: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
+000023e0: 2770 7265 766d 6f6e 7468 275d 0a20 2020  'prevmonth'].   
+000023f0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00002400: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
+00002410: 6579 735b 2770 7265 766d 6f6e 7468 275d  eys['prevmonth']
+00002420: 203d 205b 274d 275d 0a20 2020 2020 2020   = ['M'].       
+00002430: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00002440: 2020 7365 6c66 2e5f 6b65 7973 5b27 6e65    self._keys['ne
+00002450: 7874 7965 6172 275d 0a20 2020 2020 2020  xtyear'].       
+00002460: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+00002470: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
+00002480: 276e 6578 7479 6561 7227 5d20 3d20 5b27  'nextyear'] = ['
+00002490: 4b45 595f 5050 4147 4527 2c20 2779 275d  KEY_PPAGE', 'y']
+000024a0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+000024b0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000024c0: 6b65 7973 5b27 7072 6576 7965 6172 275d  keys['prevyear']
+000024d0: 0a20 2020 2020 2020 2065 7863 6570 743a  .        except:
+000024e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000024f0: 662e 5f6b 6579 735b 2770 7265 7679 6561  f._keys['prevyea
+00002500: 7227 5d20 3d20 5b27 4b45 595f 4e50 4147  r'] = ['KEY_NPAG
+00002510: 4527 2c20 2759 275d 0a20 2020 2020 2020  E', 'Y'].       
+00002520: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00002530: 2020 7365 6c66 2e5f 6b65 7973 5b27 6e65    self._keys['ne
+00002540: 7874 6576 656e 7427 5d0a 2020 2020 2020  xtevent'].      
+00002550: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+00002560: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
+00002570: 5b27 6e65 7874 6576 656e 7427 5d20 3d20  ['nextevent'] = 
+00002580: 5b27 4b45 595f 454e 4427 2c20 2709 275d  ['KEY_END', '.']
+00002590: 2020 2320 7461 620a 2020 2020 2020 2020    # tab.        
+000025a0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000025b0: 2073 656c 662e 5f6b 6579 735b 2770 7265   self._keys['pre
+000025c0: 7665 7665 6e74 275d 0a20 2020 2020 2020  vevent'].       
+000025d0: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+000025e0: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
+000025f0: 2770 7265 7665 7665 6e74 275d 203d 205b  'prevevent'] = [
+00002600: 274b 4559 5f48 4f4d 4527 2c20 274b 4559  'KEY_HOME', 'KEY
+00002610: 5f42 5441 4227 5d0a 2020 2020 2020 2020  _BTAB'].        
+00002620: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00002630: 2073 656c 662e 5f6b 6579 735b 2764 656c   self._keys['del
+00002640: 6576 656e 7427 5d0a 2020 2020 2020 2020  event'].        
+00002650: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00002660: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
+00002670: 6465 6c65 7665 6e74 275d 203d 205b 2764  delevent'] = ['d
+00002680: 272c 2027 4427 5d0a 2020 2020 2020 2020  ', 'D'].        
+00002690: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000026a0: 2073 656c 662e 5f6b 6579 735b 2761 6464   self._keys['add
+000026b0: 6576 656e 7427 5d0a 2020 2020 2020 2020  event'].        
+000026c0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+000026d0: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
+000026e0: 6164 6465 7665 6e74 275d 203d 205b 2761  addevent'] = ['a
+000026f0: 272c 2027 4127 5d0a 2020 2020 2020 2020  ', 'A'].        
+00002700: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00002710: 2073 656c 662e 5f6b 6579 735b 2765 6469   self._keys['edi
+00002720: 7465 7665 6e74 275d 0a20 2020 2020 2020  tevent'].       
+00002730: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+00002740: 2020 2020 2073 656c 662e 5f6b 6579 735b       self._keys[
+00002750: 2765 6469 7465 7665 6e74 275d 203d 205b  'editevent'] = [
+00002760: 2765 272c 2027 4527 5d0a 2020 2020 2020  'e', 'E'].      
+00002770: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00002780: 2020 2073 656c 662e 5f6b 6579 735b 2774     self._keys['t
+00002790: 6f67 676c 6557 4527 5d0a 2020 2020 2020  oggleWE'].      
+000027a0: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+000027b0: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
+000027c0: 5b27 746f 6767 6c65 5745 275d 203d 205b  ['toggleWE'] = [
+000027d0: 2777 272c 2027 5727 5d0a 2020 2020 2020  'w', 'W'].      
+000027e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000027f0: 2020 2073 656c 662e 5f6b 6579 735b 2772     self._keys['r
+00002800: 6564 7261 7727 5d0a 2020 2020 2020 2020  edraw'].        
+00002810: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00002820: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
+00002830: 7265 6472 6177 275d 203d 205b 2712 272c  redraw'] = ['.',
+00002840: 2027 0c27 5d0a 2020 2020 2020 2020 7472   '.'].        tr
+00002850: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00002860: 656c 662e 5f6b 6579 735b 2773 796e 6327  elf._keys['sync'
+00002870: 5d0a 2020 2020 2020 2020 6578 6365 7074  ].        except
+00002880: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00002890: 6c66 2e5f 6b65 7973 5b27 7379 6e63 275d  lf._keys['sync']
+000028a0: 203d 205b 2716 275d 0a20 2020 2020 2020   = ['.'].       
+000028b0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+000028c0: 2020 7365 6c66 2e5f 6b65 7973 5b27 7361    self._keys['sa
+000028d0: 7665 275d 0a20 2020 2020 2020 2065 7863  ve'].        exc
+000028e0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+000028f0: 2073 656c 662e 5f6b 6579 735b 2773 6176   self._keys['sav
+00002900: 6527 5d20 3d20 5b27 7327 2c20 2753 275d  e'] = ['s', 'S']
+00002910: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00002920: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00002930: 6b65 7973 5b27 696d 706f 7274 275d 0a20  keys['import']. 
+00002940: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+00002950: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002960: 5f6b 6579 735b 2769 6d70 6f72 7427 5d20  _keys['import'] 
+00002970: 3d20 5b27 6927 2c20 2749 275d 0a20 2020  = ['i', 'I'].   
+00002980: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00002990: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
+000029a0: 5b27 6578 706f 7274 275d 0a20 2020 2020  ['export'].     
+000029b0: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+000029c0: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
+000029d0: 735b 2765 7870 6f72 7427 5d20 3d20 5b27  s['export'] = ['
+000029e0: 7827 2c20 2758 275d 0a20 2020 2020 2020  x', 'X'].       
+000029f0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00002a00: 2020 7365 6c66 2e5f 6b65 7973 5b27 746f    self._keys['to
+00002a10: 6461 7927 5d0a 2020 2020 2020 2020 6578  day'].        ex
+00002a20: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+00002a30: 2020 7365 6c66 2e5f 6b65 7973 5b27 746f    self._keys['to
+00002a40: 6461 7927 5d20 3d20 5b27 0727 5d0a 2020  day'] = ['.'].  
+00002a50: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00002a60: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
+00002a70: 735b 2773 6574 6461 7927 5d0a 2020 2020  s['setday'].    
+00002a80: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+00002a90: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
+00002aa0: 7973 5b27 7365 7464 6179 275d 203d 205b  ys['setday'] = [
+00002ab0: 2767 272c 2027 4727 5d0a 2020 2020 2020  'g', 'G'].      
+00002ac0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00002ad0: 2020 2073 656c 662e 5f6b 6579 735b 2773     self._keys['s
+00002ae0: 7461 7274 7765 656b 275d 0a20 2020 2020  tartweek'].     
+00002af0: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+00002b00: 2020 2020 2020 2073 656c 662e 5f6b 6579         self._key
+00002b10: 735b 2773 7461 7274 7765 656b 275d 203d  s['startweek'] =
+00002b20: 205b 2730 275d 0a20 2020 2020 2020 2074   ['0'].        t
+00002b30: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00002b40: 7365 6c66 2e5f 6b65 7973 5b27 656e 6477  self._keys['endw
+00002b50: 6565 6b27 5d0a 2020 2020 2020 2020 6578  eek'].        ex
+00002b60: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+00002b70: 2020 7365 6c66 2e5f 6b65 7973 5b27 656e    self._keys['en
+00002b80: 6477 6565 6b27 5d20 3d20 5b27 2427 5d0a  dweek'] = ['$'].
+00002b90: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00002ba0: 2020 2020 2020 2020 2073 656c 662e 5f6b           self._k
+00002bb0: 6579 735b 2768 656c 7027 5d0a 2020 2020  eys['help'].    
+00002bc0: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+00002bd0: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
+00002be0: 7973 5b27 6865 6c70 275d 203d 205b 2768  ys['help'] = ['h
+00002bf0: 272c 2027 4827 5d0a 2020 2020 2020 2020  ', 'H'].        
+00002c00: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00002c10: 2073 656c 662e 5f6b 6579 735b 2774 6167   self._keys['tag
+00002c20: 6576 656e 7427 5d0a 2020 2020 2020 2020  event'].        
+00002c30: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00002c40: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
+00002c50: 7461 6765 7665 6e74 275d 203d 205b 2774  tagevent'] = ['t
+00002c60: 272c 2027 5427 2c20 277c 275d 0a20 2020  ', 'T', '|'].   
+00002c70: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00002c80: 2020 2020 2020 7365 6c66 2e5f 6b65 7973        self._keys
+00002c90: 5b27 636f 7079 6576 656e 7427 5d0a 2020  ['copyevent'].  
+00002ca0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00002cb0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00002cc0: 6b65 7973 5b27 636f 7079 6576 656e 7427  keys['copyevent'
+00002cd0: 5d20 3d20 5b27 7027 2c20 2750 275d 0a20  ] = ['p', 'P']. 
+00002ce0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00002cf0: 2020 2020 2020 2020 7365 6c66 2e5f 6b65          self._ke
+00002d00: 7973 5b27 6d69 6e75 7373 6869 6674 686f  ys['minusshiftho
+00002d10: 7572 275d 0a20 2020 2020 2020 2065 7863  ur'].        exc
+00002d20: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+00002d30: 2073 656c 662e 5f6b 6579 735b 276d 696e   self._keys['min
+00002d40: 7573 7368 6966 7468 6f75 7227 5d20 3d20  usshifthour'] = 
+00002d50: 5b27 2d27 5d0a 2020 2020 2020 2020 7472  ['-'].        tr
+00002d60: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00002d70: 656c 662e 5f6b 6579 735b 2773 6869 6674  elf._keys['shift
+00002d80: 686f 7572 275d 0a20 2020 2020 2020 2065  hour'].        e
+00002d90: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+00002da0: 2020 2073 656c 662e 5f6b 6579 735b 2773     self._keys['s
+00002db0: 6869 6674 686f 7572 275d 203d 205b 272b  hifthour'] = ['+
+00002dc0: 275d 0a20 2020 2020 2020 2074 7279 3a0a  '].        try:.
+00002dd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002de0: 2e5f 6b65 7973 5b27 6d69 6e75 7373 6869  ._keys['minusshi
+00002df0: 6674 6461 7927 5d0a 2020 2020 2020 2020  ftday'].        
+00002e00: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00002e10: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
+00002e20: 6d69 6e75 7373 6869 6674 6461 7927 5d20  minusshiftday'] 
+00002e30: 3d20 5b27 2f27 5d0a 2020 2020 2020 2020  = ['/'].        
+00002e40: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00002e50: 2073 656c 662e 5f6b 6579 735b 2773 6869   self._keys['shi
+00002e60: 6674 6461 7927 5d0a 2020 2020 2020 2020  ftday'].        
+00002e70: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00002e80: 2020 2020 7365 6c66 2e5f 6b65 7973 5b27      self._keys['
+00002e90: 7368 6966 7464 6179 275d 203d 205b 272a  shiftday'] = ['*
+00002ea0: 275d 0a20 2020 2020 2020 2074 7279 3a0a  '].        try:.
+00002eb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002ec0: 2e5f 6b65 7973 5b27 7365 7463 6f6e 6669  ._keys['setconfi
+00002ed0: 6727 5d0a 2020 2020 2020 2020 6578 6365  g'].        exce
+00002ee0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+00002ef0: 7365 6c66 2e5f 6b65 7973 5b27 7365 7463  self._keys['setc
+00002f00: 6f6e 6669 6727 5d20 3d20 5b27 6327 2c20  onfig'] = ['c', 
+00002f10: 2743 275d 0a20 2020 2020 2020 2074 7279  'C'].        try
+00002f20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00002f30: 6c66 2e5f 6b65 7973 5b27 746f 6767 6c65  lf._keys['toggle
+00002f40: 746f 646f 275d 0a20 2020 2020 2020 2065  todo'].        e
+00002f50: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+00002f60: 2020 2073 656c 662e 5f6b 6579 735b 2774     self._keys['t
+00002f70: 6f67 676c 6574 6f64 6f27 5d20 3d20 5b27  oggletodo'] = ['
+00002f80: 1427 5d0a 0a20 2020 2020 2020 2069 6620  .']..        if 
+00002f90: 6c65 6e28 7365 6c66 2e5f 6b65 7973 2920  len(self._keys) 
+00002fa0: 3e20 6c65 6e28 6f6c 646b 6579 7329 3a0a  > len(oldkeys):.
+00002fb0: 2020 2020 2020 2020 2020 2020 2320 6966              # if
+00002fc0: 2061 2064 6566 6175 6c74 2063 6f6e 6669   a default confi
+00002fd0: 6775 7261 7469 6f6e 2068 6173 2062 6565  guration has bee
+00002fe0: 6e20 7573 6564 0a20 2020 2020 2020 2020  n used.         
+00002ff0: 2020 2073 656c 662e 7772 6974 656b 6579     self.writekey
+00003000: 7328 290a 0a20 2020 2064 6566 2077 7269  s()..    def wri
+00003010: 7465 6b65 7973 2873 656c 6629 3a0a 2020  tekeys(self):.  
+00003020: 2020 2020 2020 6c69 6e65 7320 3d20 2222        lines = ""
+00003030: 0a20 2020 2020 2020 2023 206f 7264 6572  .        # order
+00003040: 6564 206c 6973 7420 6f66 2069 7465 6d73  ed list of items
+00003050: 0a20 2020 2020 2020 206b 6579 776f 7264  .        keyword
+00003060: 7320 3d20 5b27 6e65 7874 6461 7927 2c20  s = ['nextday', 
+00003070: 2770 7265 7664 6179 272c 2027 6e65 7874  'prevday', 'next
+00003080: 7765 656b 272c 2027 7072 6576 7765 656b  week', 'prevweek
+00003090: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+000030a0: 2020 2020 2020 2027 6e65 7874 6d6f 6e74         'nextmont
+000030b0: 6827 2c20 2770 7265 766d 6f6e 7468 272c  h', 'prevmonth',
+000030c0: 2027 6e65 7874 7965 6172 272c 2027 7072   'nextyear', 'pr
+000030d0: 6576 7965 6172 272c 0a20 2020 2020 2020  evyear',.       
+000030e0: 2020 2020 2020 2020 2020 2020 2027 6e65               'ne
+000030f0: 7874 6576 656e 7427 2c20 2770 7265 7665  xtevent', 'preve
+00003100: 7665 6e74 272c 2027 6465 6c65 7665 6e74  vent', 'delevent
+00003110: 272c 2027 6164 6465 7665 6e74 272c 0a20  ', 'addevent',. 
+00003120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003130: 2020 2027 6564 6974 6576 656e 7427 2c20     'editevent', 
+00003140: 2774 6f67 676c 6557 4527 2c20 2771 7569  'toggleWE', 'qui
+00003150: 7427 2c20 2772 6564 7261 7727 2c20 2773  t', 'redraw', 's
+00003160: 796e 6327 2c20 2773 6176 6527 2c0a 2020  ync', 'save',.  
+00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003180: 2020 2769 6d70 6f72 7427 2c20 2765 7870    'import', 'exp
+00003190: 6f72 7427 2c20 2774 6f64 6179 272c 2027  ort', 'today', '
+000031a0: 7365 7464 6179 272c 2027 7374 6172 7477  setday', 'startw
+000031b0: 6565 6b27 2c0a 2020 2020 2020 2020 2020  eek',.          
+000031c0: 2020 2020 2020 2020 2020 2765 6e64 7765            'endwe
+000031d0: 656b 272c 2027 6865 6c70 272c 2027 7461  ek', 'help', 'ta
+000031e0: 6765 7665 6e74 272c 2027 636f 7079 6576  gevent', 'copyev
+000031f0: 656e 7427 2c0a 2020 2020 2020 2020 2020  ent',.          
+00003200: 2020 2020 2020 2020 2020 276d 696e 7573            'minus
+00003210: 7368 6966 7468 6f75 7227 2c20 2773 6869  shifthour', 'shi
+00003220: 6674 686f 7572 272c 2027 6d69 6e75 7373  fthour', 'minuss
+00003230: 6869 6674 6461 7927 2c20 2773 6869 6674  hiftday', 'shift
+00003240: 6461 7927 2c0a 2020 2020 2020 2020 2020  day',.          
+00003250: 2020 2020 2020 2020 2020 2773 6574 636f            'setco
+00003260: 6e66 6967 272c 2027 746f 6767 6c65 746f  nfig', 'toggleto
+00003270: 646f 275d 0a20 2020 2020 2020 2066 6f72  do'].        for
+00003280: 206f 7020 696e 206b 6579 776f 7264 733a   op in keywords:
+00003290: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
+000032a0: 6520 3d20 6f70 202b 2022 3a20 220a 2020  e = op + ": ".  
+000032b0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+000032c0: 696e 2073 656c 662e 5f6b 6579 735b 6f70  in self._keys[op
+000032d0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+000032e0: 2020 2069 6620 6b20 3d3d 2022 2022 3a0a     if k == " ":.
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 2020 2020 6b20 3d20 2253 5041 4345 220a      k = "SPACE".
+00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003320: 6c69 6e65 203d 206c 696e 6520 2b20 6b20  line = line + k 
+00003330: 2b20 222c 2022 0a20 2020 2020 2020 2020  + ", ".         
+00003340: 2020 2023 2072 6570 6c61 6365 206c 6173     # replace las
+00003350: 7420 636f 6d6d 6120 616e 6420 7370 6163  t comma and spac
+00003360: 6520 6279 2061 206e 6577 6c69 6e65 0a20  e by a newline. 
+00003370: 2020 2020 2020 2020 2020 206c 696e 6520             line 
+00003380: 3d20 6c69 6e65 5b3a 2d32 5d20 2b20 225c  = line[:-2] + "\
+00003390: 6e22 0a20 2020 2020 2020 2020 2020 206c  n".            l
+000033a0: 696e 6573 202b 3d20 6c69 6e65 0a20 2020  ines += line.   
+000033b0: 2020 2020 2077 6974 6820 6f70 656e 2873       with open(s
+000033c0: 656c 662e 5f6b 6579 7366 696c 652c 2022  elf._keysfile, "
+000033d0: 7722 2920 6173 2066 3a0a 2020 2020 2020  w") as f:.      
+000033e0: 2020 2020 2020 662e 7772 6974 6528 6c69        f.write(li
+000033f0: 6e65 7329 0a0a 2020 2020 6465 6620 7265  nes)..    def re
+00003400: 6164 636f 6c6f 7572 7328 7365 6c66 293a  adcolours(self):
+00003410: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00003420: 7061 7468 2e65 7869 7374 7328 7365 6c66  path.exists(self
+00003430: 2e5f 636f 6c6f 7572 7366 696c 6529 3a0a  ._coloursfile):.
+00003440: 2020 2020 2020 2020 2020 2020 2320 6465              # de
+00003450: 6661 756c 7473 2061 6e64 2077 7269 7465  faults and write
+00003460: 2066 696c 650a 2020 2020 2020 2020 2020   file.          
+00003470: 2020 7365 6c66 2e5f 636f 6c6f 7572 735f    self._colours_
+00003480: 6964 7820 3d20 7261 6e67 6528 3829 0a20  idx = range(8). 
+00003490: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000034a0: 7772 6974 6563 6f6c 6f75 7273 2829 0a20  writecolours(). 
+000034b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000034c0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+000034d0: 6f6c 6f75 7273 5f69 6478 203d 205b 5d0a  olours_idx = [].
+000034e0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000034f0: 206f 7065 6e28 7365 6c66 2e5f 636f 6c6f   open(self._colo
+00003500: 7572 7366 696c 6529 2061 7320 663a 0a20  ursfile) as f:. 
+00003510: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00003520: 6f72 206c 696e 6520 696e 2066 3a0a 2020  or line in f:.  
+00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003540: 2020 7365 6c66 2e5f 636f 6c6f 7572 735f    self._colours_
+00003550: 6964 782e 6170 7065 6e64 2869 6e74 286c  idx.append(int(l
+00003560: 696e 6529 290a 0a20 2020 2064 6566 2077  ine))..    def w
+00003570: 7269 7465 636f 6c6f 7572 7328 7365 6c66  ritecolours(self
+00003580: 293a 0a20 2020 2020 2020 206c 696e 6573  ):.        lines
+00003590: 203d 2022 220a 2020 2020 2020 2020 666f   = "".        fo
+000035a0: 7220 636f 6c6f 7572 5f69 6478 2069 6e20  r colour_idx in 
+000035b0: 7365 6c66 2e5f 636f 6c6f 7572 735f 6964  self._colours_id
+000035c0: 783a 0a20 2020 2020 2020 2020 2020 206c  x:.            l
+000035d0: 696e 6573 202b 3d20 7374 7228 636f 6c6f  ines += str(colo
+000035e0: 7572 5f69 6478 2920 2b20 225c 6e22 0a20  ur_idx) + "\n". 
+000035f0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00003600: 2873 656c 662e 5f63 6f6c 6f75 7273 6669  (self._coloursfi
+00003610: 6c65 2c20 2277 2229 2061 7320 663a 0a20  le, "w") as f:. 
+00003620: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+00003630: 7465 286c 696e 6573 290a 0a20 2020 2064  te(lines)..    d
+00003640: 6566 2073 6574 636f 6c6f 7572 7328 7365  ef setcolours(se
+00003650: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00003660: 662e 5f63 6f6c 6f75 7273 203d 205b 5d0a  f._colours = [].
+00003670: 2020 2020 2020 2020 2320 6465 6669 6e65          # define
+00003680: 2074 6865 2065 6967 6874 2063 6f6c 6f75   the eight colou
+00003690: 7273 0a20 2020 2020 2020 2066 6f72 2069  rs.        for i
+000036a0: 2069 6e20 7261 6e67 6528 3829 3a0a 2020   in range(8):.  
+000036b0: 2020 2020 2020 2020 2020 7472 793a 2020            try:  
+000036c0: 2320 7468 6520 7465 726d 696e 616c 2068  # the terminal h
+000036d0: 6173 2061 2064 6566 6175 6c74 2062 6163  as a default bac
+000036e0: 6b67 726f 756e 640a 2020 2020 2020 2020  kground.        
+000036f0: 2020 2020 2020 2020 6375 7273 6573 2e69          curses.i
+00003700: 6e69 745f 7061 6972 2869 2c20 692c 202d  nit_pair(i, i, -
+00003710: 3129 0a20 2020 2020 2020 2020 2020 2065  1).            e
+00003720: 7863 6570 743a 2020 2320 6465 6661 756c  xcept:  # defaul
+00003730: 7473 2074 6f20 626c 6163 6b0a 2020 2020  ts to black.    
+00003740: 2020 2020 2020 2020 2020 2020 6375 7273              curs
+00003750: 6573 2e69 6e69 745f 7061 6972 2869 2c20  es.init_pair(i, 
+00003760: 692c 2030 290a 2020 2020 2020 2020 666f  i, 0).        fo
+00003770: 7220 6964 7820 696e 2073 656c 662e 5f63  r idx in self._c
+00003780: 6f6c 6f75 7273 5f69 6478 3a0a 2020 2020  olours_idx:.    
+00003790: 2020 2020 2020 2020 7365 6c66 2e5f 636f          self._co
+000037a0: 6c6f 7572 732e 6170 7065 6e64 2863 7572  lours.append(cur
+000037b0: 7365 732e 636f 6c6f 725f 7061 6972 2869  ses.color_pair(i
+000037c0: 6478 2929 0a0a 2020 2020 6465 6620 7265  dx))..    def re
+000037d0: 6164 6361 7465 676f 7269 6573 2873 656c  adcategories(sel
+000037e0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+000037f0: 2e5f 6361 7465 676f 7269 6573 203d 207b  ._categories = {
+00003800: 7d0a 2020 2020 2020 2020 6966 206e 6f74  }.        if not
+00003810: 2070 6174 682e 6578 6973 7473 2873 656c   path.exists(sel
+00003820: 662e 5f63 6174 6567 6f72 6965 7366 696c  f._categoriesfil
+00003830: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00003840: 2320 6465 6661 756c 7473 2061 6e64 2077  # defaults and w
+00003850: 7269 7465 2066 696c 650a 2020 2020 2020  rite file.      
+00003860: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00003870: 616e 6765 2831 2c20 3829 3a0a 2020 2020  ange(1, 8):.    
+00003880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003890: 2e5f 6361 7465 676f 7269 6573 5b69 5d20  ._categories[i] 
+000038a0: 3d20 5b73 7472 2869 295d 0a20 2020 2020  = [str(i)].     
+000038b0: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
+000038c0: 6563 6174 6567 6f72 6965 7328 290a 2020  ecategories().  
+000038d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000038e0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+000038f0: 6e28 7365 6c66 2e5f 6361 7465 676f 7269  n(self._categori
+00003900: 6573 6669 6c65 2920 6173 2066 3a0a 2020  esfile) as f:.  
+00003910: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00003920: 7220 6964 782c 206c 696e 6520 696e 2065  r idx, line in e
+00003930: 6e75 6d65 7261 7465 2866 293a 0a20 2020  numerate(f):.   
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2063 6174 203d 206c 696e 655b 3a2d 315d   cat = line[:-1]
+00003960: 2e72 6570 6c61 6365 2822 2c20 222c 2022  .replace(", ", "
+00003970: 2c22 292e 7370 6c69 7428 222c 2229 0a20  ,").split(","). 
+00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003990: 2020 2023 202d 3120 746f 2069 676e 6f72     # -1 to ignor
+000039a0: 6520 6669 6e61 6c20 5c6e 0a20 2020 2020  e final \n.     
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000039c0: 656c 662e 5f63 6174 6567 6f72 6965 735b  elf._categories[
+000039d0: 6964 782b 315d 203d 2063 6174 0a20 2020  idx+1] = cat.   
+000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039f0: 2023 202b 313a 2063 6174 6567 6f72 7920   # +1: category 
+00003a00: 3020 6973 2064 6566 6175 6c74 730a 0a20  0 is defaults.. 
+00003a10: 2020 2064 6566 2077 7269 7465 6361 7465     def writecate
+00003a20: 676f 7269 6573 2873 656c 6629 3a0a 2020  gories(self):.  
+00003a30: 2020 2020 2020 6c69 6e65 7320 3d20 2222        lines = ""
+00003a40: 0a20 2020 2020 2020 2066 6f72 2074 6167  .        for tag
+00003a50: 6e62 2069 6e20 7261 6e67 6528 312c 2038  nb in range(1, 8
+00003a60: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+00003a70: 696e 6520 3d20 2222 0a20 2020 2020 2020  ine = "".       
+00003a80: 2020 2020 2066 6f72 2063 6174 2069 6e20       for cat in 
+00003a90: 7365 6c66 2e5f 6361 7465 676f 7269 6573  self._categories
+00003aa0: 5b74 6167 6e62 5d3a 0a20 2020 2020 2020  [tagnb]:.       
+00003ab0: 2020 2020 2020 2020 206c 696e 6520 3d20           line = 
+00003ac0: 6c69 6e65 202b 2063 6174 202b 2022 2c20  line + cat + ", 
+00003ad0: 220a 2020 2020 2020 2020 2020 2020 2320  ".            # 
+00003ae0: 7265 706c 6163 6520 6c61 7374 2063 6f6d  replace last com
+00003af0: 6d61 2061 6e64 2073 7061 6365 2062 7920  ma and space by 
+00003b00: 6120 6e65 776c 696e 650a 2020 2020 2020  a newline.      
+00003b10: 2020 2020 2020 6c69 6e65 203d 206c 696e        line = lin
+00003b20: 655b 3a2d 325d 202b 2022 5c6e 220a 2020  e[:-2] + "\n".  
+00003b30: 2020 2020 2020 2020 2020 6c69 6e65 7320            lines 
+00003b40: 2b3d 206c 696e 650a 2020 2020 2020 2020  += line.        
+00003b50: 7769 7468 206f 7065 6e28 7365 6c66 2e5f  with open(self._
+00003b60: 6361 7465 676f 7269 6573 6669 6c65 2c20  categoriesfile, 
+00003b70: 2277 2229 2061 7320 663a 0a20 2020 2020  "w") as f:.     
+00003b80: 2020 2020 2020 2066 2e77 7269 7465 286c         f.write(l
+00003b90: 696e 6573 290a 0a20 2020 2064 6566 2072  ines)..    def r
+00003ba0: 6561 6463 616c 6461 7628 7365 6c66 293a  eadcaldav(self):
+00003bb0: 0a20 2020 2020 2020 2069 6620 7061 7468  .        if path
+00003bc0: 2e65 7869 7374 7328 7365 6c66 2e5f 6361  .exists(self._ca
+00003bd0: 6c64 6176 6669 6c65 293a 0a20 2020 2020  ldavfile):.     
+00003be0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00003bf0: 2873 656c 662e 5f63 616c 6461 7666 696c  (self._caldavfil
+00003c00: 6529 2061 7320 663a 0a20 2020 2020 2020  e) as f:.       
+00003c10: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
+00003c20: 6520 696e 2066 3a0a 2020 2020 2020 2020  e in f:.        
+00003c30: 2020 2020 2020 2020 2020 2020 6364 6176              cdav
+00003c40: 203d 207b 7d20 2023 2069 6e69 7469 6174   = {}  # initiat
+00003c50: 6520 7468 6520 6469 6374 0a20 2020 2020  e the dict.     
+00003c60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003c70: 6e64 7572 6c20 3d20 6c69 6e65 2e66 696e  ndurl = line.fin
+00003c80: 6428 222c 2075 7365 726e 616d 653d 2229  d(", username=")
+00003c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ca0: 2020 2020 2065 6e64 7573 6572 6e61 6d65       endusername
+00003cb0: 203d 206c 696e 652e 6669 6e64 2822 2c20   = line.find(", 
+00003cc0: 7061 7373 776f 7264 3d22 290a 2020 2020  password=").    
+00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ce0: 656e 6470 6173 7377 6f72 6420 3d20 6c69  endpassword = li
+00003cf0: 6e65 2e66 696e 6428 222c 2074 6167 3d22  ne.find(", tag="
+00003d00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003d10: 2020 2020 2020 656e 6474 6167 203d 206c        endtag = l
+00003d20: 696e 652e 6669 6e64 2822 2c20 636f 6c6f  ine.find(", colo
+00003d30: 7572 3d22 290a 2020 2020 2020 2020 2020  ur=").          
+00003d40: 2020 2020 2020 2020 2020 2320 3520 746f            # 5 to
+00003d50: 2073 6b69 7020 7468 6520 7374 6172 7469   skip the starti
+00003d60: 6e67 2020 2775 726c 3d22 270a 2020 2020  ng  'url="'.    
+00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d80: 7572 6c20 3d20 6c69 6e65 5b35 3a65 6e64  url = line[5:end
+00003d90: 7572 6c2d 315d 0a20 2020 2020 2020 2020  url-1].         
+00003da0: 2020 2020 2020 2020 2020 2023 2069 7320             # is 
+00003db0: 7468 6572 6520 6120 7061 7373 776f 7264  there a password
+00003dc0: 3f0a 2020 2020 2020 2020 2020 2020 2020  ?.              
+00003dd0: 2020 2020 2020 6966 2065 6e64 7573 6572        if enduser
+00003de0: 6e61 6d65 202d 2065 6e64 7572 6c20 3e20  name - endurl > 
+00003df0: 3133 3a0a 2020 2020 2020 2020 2020 2020  13:.            
+00003e00: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00003e10: 6e61 6d65 203d 206c 696e 655b 656e 6475  name = line[endu
+00003e20: 726c 2b31 323a 656e 6475 7365 726e 616d  rl+12:endusernam
+00003e30: 652d 315d 0a20 2020 2020 2020 2020 2020  e-1].           
+00003e40: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00003e50: 7377 6f72 6420 3d20 6c69 6e65 5b65 6e64  sword = line[end
+00003e60: 7573 6572 6e61 6d65 2b31 323a 656e 6470  username+12:endp
+00003e70: 6173 7377 6f72 642d 315d 0a20 2020 2020  assword-1].     
+00003e80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003e90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003ea0: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00003eb0: 726e 616d 6520 3d20 2222 0a20 2020 2020  rname = "".     
 00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ed0: 7573 6572 6e61 6d65 203d 2022 220a 2020  username = "".  
-00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ef0: 2020 2020 2020 7061 7373 776f 7264 203d        password =
-00003f00: 2022 220a 2020 2020 2020 2020 2020 2020   "".            
-00003f10: 2020 2020 2020 2020 7461 6720 3d20 6c69          tag = li
-00003f20: 6e65 5b65 6e64 7061 7373 776f 7264 2b37  ne[endpassword+7
-00003f30: 3a65 6e64 7461 672d 315d 0a20 2020 2020  :endtag-1].     
-00003f40: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003f50: 206c 696e 6520 6669 6e69 7368 2062 7920   line finish by 
-00003f60: 2763 6f6c 6f75 723d 2258 225c 6e27 2c20  'colour="X"\n', 
-00003f70: 6765 7420 7468 6520 580a 2020 2020 2020  get the X.      
-00003f80: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00003f90: 6c6f 7572 203d 2069 6e74 286c 696e 655b  lour = int(line[
-00003fa0: 2d33 5d29 0a20 2020 2020 2020 2020 2020  -3]).           
-00003fb0: 2020 2020 2020 2020 2023 2066 696c 6c20           # fill 
-00003fc0: 7570 2074 6865 2063 616c 6461 7627 7320  up the caldav's 
-00003fd0: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
-00003fe0: 2020 2020 2020 2020 2063 6461 765b 2275           cdav["u
-00003ff0: 726c 225d 203d 2075 726c 0a20 2020 2020  rl"] = url.     
-00004000: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004010: 6461 765b 2275 7365 726e 616d 6522 5d20  dav["username"] 
-00004020: 3d20 7573 6572 6e61 6d65 0a20 2020 2020  = username.     
-00004030: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004040: 6461 765b 2270 6173 7377 6f72 6422 5d20  dav["password"] 
-00004050: 3d20 7061 7373 776f 7264 0a20 2020 2020  = password.     
-00004060: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00004070: 6461 765b 2274 6167 225d 203d 2074 6167  dav["tag"] = tag
-00004080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004090: 2020 2020 2063 6461 765b 2263 6f6c 6f75       cdav["colou
-000040a0: 7222 5d20 3d20 636f 6c6f 7572 0a20 2020  r"] = colour.   
-000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040c0: 2023 2073 7461 636b 2069 7420 696e 2074   # stack it in t
-000040d0: 6865 206c 6973 740a 2020 2020 2020 2020  he list.        
-000040e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000040f0: 2e5f 6361 6c64 6176 2e61 7070 656e 6428  ._caldav.append(
-00004100: 6364 6176 290a 0a20 2020 2064 6566 2077  cdav)..    def w
-00004110: 7269 7465 6361 6c64 6176 2873 656c 6629  ritecaldav(self)
-00004120: 3a0a 2020 2020 2020 2020 6c69 6e65 7320  :.        lines 
-00004130: 3d20 2222 0a20 2020 2020 2020 2066 6f72  = "".        for
-00004140: 2063 6461 7620 696e 2073 656c 662e 5f63   cdav in self._c
-00004150: 616c 6461 763a 0a20 2020 2020 2020 2020  aldav:.         
-00004160: 2020 206c 696e 6520 3d20 2222 0a20 2020     line = "".   
-00004170: 2020 2020 2020 2020 206c 696e 6520 2b3d           line +=
-00004180: 2027 7572 6c3d 2227 202b 2063 6461 765b   'url="' + cdav[
-00004190: 2275 726c 225d 0a20 2020 2020 2020 2020  "url"].         
-000041a0: 2020 206c 696e 6520 2b3d 2027 222c 2075     line += '", u
-000041b0: 7365 726e 616d 653d 2227 202b 2063 6461  sername="' + cda
-000041c0: 765b 2275 7365 726e 616d 6522 5d0a 2020  v["username"].  
-000041d0: 2020 2020 2020 2020 2020 6c69 6e65 202b            line +
-000041e0: 3d20 2722 2c20 7061 7373 776f 7264 3d22  = '", password="
-000041f0: 2720 2b20 6364 6176 5b22 7061 7373 776f  ' + cdav["passwo
-00004200: 7264 225d 0a20 2020 2020 2020 2020 2020  rd"].           
-00004210: 206c 696e 6520 2b3d 2027 222c 2074 6167   line += '", tag
-00004220: 3d22 2720 2b20 6364 6176 5b22 7461 6722  ="' + cdav["tag"
-00004230: 5d0a 2020 2020 2020 2020 2020 2020 6c69  ].            li
-00004240: 6e65 202b 3d20 2722 2c20 636f 6c6f 7572  ne += '", colour
-00004250: 3d22 2720 2b20 7374 7228 6364 6176 5b22  ="' + str(cdav["
-00004260: 636f 6c6f 7572 225d 2920 2b20 2722 5c6e  colour"]) + '"\n
-00004270: 270a 2020 2020 2020 2020 2020 2020 6c69  '.            li
-00004280: 6e65 7320 2b3d 206c 696e 650a 2020 2020  nes += line.    
-00004290: 2020 2020 7769 7468 206f 7065 6e28 7365      with open(se
-000042a0: 6c66 2e5f 6361 6c64 6176 6669 6c65 2c20  lf._caldavfile, 
-000042b0: 2277 2229 2061 7320 663a 0a20 2020 2020  "w") as f:.     
-000042c0: 2020 2020 2020 2066 2e77 7269 7465 286c         f.write(l
-000042d0: 696e 6573 290a 0a20 2020 2064 6566 2073  ines)..    def s
-000042e0: 6176 6528 7365 6c66 293a 0a20 2020 2020  ave(self):.     
-000042f0: 2020 2073 656c 662e 7772 6974 6563 6f6e     self.writecon
-00004300: 6628 290a 2020 2020 2020 2020 7365 6c66  f().        self
-00004310: 2e77 7269 7465 6b65 7973 2829 0a20 2020  .writekeys().   
-00004320: 2020 2020 2073 656c 662e 7772 6974 6563       self.writec
-00004330: 6f6c 6f75 7273 2829 0a20 2020 2020 2020  olours().       
-00004340: 2073 656c 662e 7772 6974 6563 6174 6567   self.writecateg
-00004350: 6f72 6965 7328 290a 2020 2020 2020 2020  ories().        
-00004360: 7365 6c66 2e77 7269 7465 6361 6c64 6176  self.writecaldav
-00004370: 2829 0a                                  ().
+00003ed0: 2020 2070 6173 7377 6f72 6420 3d20 2222     password = ""
+00003ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ef0: 2020 2020 2074 6167 203d 206c 696e 655b       tag = line[
+00003f00: 656e 6470 6173 7377 6f72 642b 373a 656e  endpassword+7:en
+00003f10: 6474 6167 2d31 5d0a 2020 2020 2020 2020  dtag-1].        
+00003f20: 2020 2020 2020 2020 2020 2020 2320 6c69              # li
+00003f30: 6e65 2066 696e 6973 6820 6279 2027 636f  ne finish by 'co
+00003f40: 6c6f 7572 3d22 5822 5c6e 272c 2067 6574  lour="X"\n', get
+00003f50: 2074 6865 2058 0a20 2020 2020 2020 2020   the X.         
+00003f60: 2020 2020 2020 2020 2020 2063 6f6c 6f75             colou
+00003f70: 7220 3d20 696e 7428 6c69 6e65 5b2d 335d  r = int(line[-3]
+00003f80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003f90: 2020 2020 2020 2320 6669 6c6c 2075 7020        # fill up 
+00003fa0: 7468 6520 6361 6c64 6176 2773 2064 6963  the caldav's dic
+00003fb0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00003fc0: 2020 2020 2020 6364 6176 5b22 7572 6c22        cdav["url"
+00003fd0: 5d20 3d20 7572 6c0a 2020 2020 2020 2020  ] = url.        
+00003fe0: 2020 2020 2020 2020 2020 2020 6364 6176              cdav
+00003ff0: 5b22 7573 6572 6e61 6d65 225d 203d 2075  ["username"] = u
+00004000: 7365 726e 616d 650a 2020 2020 2020 2020  sername.        
+00004010: 2020 2020 2020 2020 2020 2020 6364 6176              cdav
+00004020: 5b22 7061 7373 776f 7264 225d 203d 2070  ["password"] = p
+00004030: 6173 7377 6f72 640a 2020 2020 2020 2020  assword.        
+00004040: 2020 2020 2020 2020 2020 2020 6364 6176              cdav
+00004050: 5b22 7461 6722 5d20 3d20 7461 670a 2020  ["tag"] = tag.  
+00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004070: 2020 6364 6176 5b22 636f 6c6f 7572 225d    cdav["colour"]
+00004080: 203d 2063 6f6c 6f75 720a 2020 2020 2020   = colour.      
+00004090: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000040a0: 7374 6163 6b20 6974 2069 6e20 7468 6520  stack it in the 
+000040b0: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
+000040c0: 2020 2020 2020 2020 2073 656c 662e 5f63           self._c
+000040d0: 616c 6461 762e 6170 7065 6e64 2863 6461  aldav.append(cda
+000040e0: 7629 0a0a 2020 2020 6465 6620 7772 6974  v)..    def writ
+000040f0: 6563 616c 6461 7628 7365 6c66 293a 0a20  ecaldav(self):. 
+00004100: 2020 2020 2020 206c 696e 6573 203d 2022         lines = "
+00004110: 220a 2020 2020 2020 2020 666f 7220 6364  ".        for cd
+00004120: 6176 2069 6e20 7365 6c66 2e5f 6361 6c64  av in self._cald
+00004130: 6176 3a0a 2020 2020 2020 2020 2020 2020  av:.            
+00004140: 6c69 6e65 203d 2022 220a 2020 2020 2020  line = "".      
+00004150: 2020 2020 2020 6c69 6e65 202b 3d20 2775        line += 'u
+00004160: 726c 3d22 2720 2b20 6364 6176 5b22 7572  rl="' + cdav["ur
+00004170: 6c22 5d0a 2020 2020 2020 2020 2020 2020  l"].            
+00004180: 6c69 6e65 202b 3d20 2722 2c20 7573 6572  line += '", user
+00004190: 6e61 6d65 3d22 2720 2b20 6364 6176 5b22  name="' + cdav["
+000041a0: 7573 6572 6e61 6d65 225d 0a20 2020 2020  username"].     
+000041b0: 2020 2020 2020 206c 696e 6520 2b3d 2027         line += '
+000041c0: 222c 2070 6173 7377 6f72 643d 2227 202b  ", password="' +
+000041d0: 2063 6461 765b 2270 6173 7377 6f72 6422   cdav["password"
+000041e0: 5d0a 2020 2020 2020 2020 2020 2020 6c69  ].            li
+000041f0: 6e65 202b 3d20 2722 2c20 7461 673d 2227  ne += '", tag="'
+00004200: 202b 2063 6461 765b 2274 6167 225d 0a20   + cdav["tag"]. 
+00004210: 2020 2020 2020 2020 2020 206c 696e 6520             line 
+00004220: 2b3d 2027 222c 2063 6f6c 6f75 723d 2227  += '", colour="'
+00004230: 202b 2073 7472 2863 6461 765b 2263 6f6c   + str(cdav["col
+00004240: 6f75 7222 5d29 202b 2027 225c 6e27 0a20  our"]) + '"\n'. 
+00004250: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+00004260: 202b 3d20 6c69 6e65 0a20 2020 2020 2020   += line.       
+00004270: 2077 6974 6820 6f70 656e 2873 656c 662e   with open(self.
+00004280: 5f63 616c 6461 7666 696c 652c 2022 7722  _caldavfile, "w"
+00004290: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+000042a0: 2020 2020 662e 7772 6974 6528 6c69 6e65      f.write(line
+000042b0: 7329 0a0a 2020 2020 6465 6620 7361 7665  s)..    def save
+000042c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000042d0: 7365 6c66 2e77 7269 7465 636f 6e66 2829  self.writeconf()
+000042e0: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
+000042f0: 6974 656b 6579 7328 290a 2020 2020 2020  itekeys().      
+00004300: 2020 7365 6c66 2e77 7269 7465 636f 6c6f    self.writecolo
+00004310: 7572 7328 290a 2020 2020 2020 2020 7365  urs().        se
+00004320: 6c66 2e77 7269 7465 6361 7465 676f 7269  lf.writecategori
+00004330: 6573 2829 0a20 2020 2020 2020 2073 656c  es().        sel
+00004340: 662e 7772 6974 6563 616c 6461 7628 290a  f.writecaldav().
```

### Comparing `culendar-0.20230330/src/culendar/cul/confscr.py` & `culendar-0.20230510/culendar/cul/confscr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-#! /usr/bin/env python3
-# coding: utf-8
 import curses
-from . import inputs, getkey
 from collections import OrderedDict
 
+from . import (
+    getkey,
+    inputs,
+)
+
 
 class Conf:
     def __init__(self, scr, conf, caldav):
         self._screen = scr
         self._caldav = caldav
         self._y, self._x = self._screen.getmaxyx()
         self._top = 0  # offset between screen and pad
         self._conf = conf
         self._general = OrderedDict()
         self._general["hmin"] = conf.hmin
         self._general["hmax"] = conf.hmax
         self._general["WE"] = conf.WE
-        self._general["TODO"] = conf.todo
+        self._general["TODO"] = conf.todo  # noqa: T101
         self._general["autosave"] = conf.autosave
         self._general["colourset"] = conf.colourset
         self._general["autosync"] = conf.autosync
         self._general["mouse"] = conf.mouse
         self._tab = 0
         self._tabs = [self._general,
                       self._conf.keys,
@@ -47,16 +49,15 @@
         # if ridiculously small terminal
         if (self._x < 25) or (self._y < 6):
             self._screen.clear()
             text = _("\_x< A dead duck. That's all such a small terminal deserves.")
             self._screen.addstr(0, 0, text[0:(self._x-1)*(self._y-1)])
 
             key = ""
-            while not((key in self._conf.keys["quit"])
-                      or (key == "KEY_RESIZE")):
+            while key not in self._conf.keys["quit"] and key != "KEY_RESIZE":
                 key = getkey.getkey(self._screen, self._conf.debug)
             if key in self._conf.keys["quit"]:
                 exit()
             else:
                 self.draw_conf_screen()
 
         # draw screen
@@ -312,16 +313,15 @@
                 self.edit_colourset()
             elif type(self._tabs[self._tab][self._editing_key]) == int:
                 self.edit_int_hour()
         elif self._tab == 2:  # change category colour
             self.edit_change_colour()
 
     def edit_bool(self):
-        self._tabs[self._tab][self._editing_key] = not(
-                        self._tabs[self._tab][self._editing_key])
+        self._tabs[self._tab][self._editing_key] = not self._tabs[self._tab][self._editing_key]
 
     def edit_colourset(self):
         self._tabs[self._tab][self._editing_key] = (
                         self._tabs[self._tab][self._editing_key] + 1) % 3
         # 3 coloursets avalaible
 
     def edit_generic(self, question, default="", pwd=False):
@@ -371,15 +371,15 @@
         else:
             self._item_idx = 0
             self.oneline_footer()
             helpmsg = _("Select item to delete, press Enter")
             self._screen.addstr(self._y-1, 0, helpmsg[:self._x-1])
             self.edit_delete_item_draw()
             key = getkey.getkey(self._screen, self._conf.debug)
-            while not(key in ["q", ""] + self._conf.keys["quit"]):
+            while key not in (["q", ""] + self._conf.keys["quit"]):
                 if key == "KEY_RESIZE":
                     self.draw_conf_screen()
                     return
                 elif key in (["\t", "KEY_RIGHT"]
                              + self._conf.keys["nextday"]):
                     self._item_idx += 1
                     if self._item_idx > len(
@@ -430,15 +430,15 @@
         self.oneline_footer()
         question = _("Press the key to add (Escape to cancel)")
         self._screen.addstr(self._y-1, 0, question[:self._x-1])
         key = getkey.getkey(self._screen, self._conf.debug)
         if key == "KEY_RESIZE":
             self.draw_conf_screen()
         elif key != "":
-            if not(key in self._tabs[self._tab][self._editing_key]):
+            if key not in self._tabs[self._tab][self._editing_key]:
                 # nothing to add, already here
                 self._tabs[self._tab][self._editing_key].append(key)
             # check if added key is present elsewhere
             for k in self._tabs[self._tab].keys():
                 # we don't care about the current edited key
                 if k != self._editing_key:
                     if key in self._tabs[self._tab][k]:
```

### Comparing `culendar-0.20230330/src/culendar/cul/culdav.py` & `culendar-0.20230510/culendar/cul/culdav.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-#! /usr/bin/env python3
-# coding: utf-8
-import caldav
 import datetime
-import icalendar
-from . import calendar, getkey
 from urllib import request
 
+import caldav
+import icalendar
+
+from . import (
+    calendar,
+    getkey,
+)
+
 
 class Cdav:
     def __init__(self, caldav_dict, screen, conf):
         self._list = caldav_dict
         self._conf = conf
         self._icals = []        # list of Icalendar, for each caldav
                                 # proper url if webcal; None if offline
```

### Comparing `culendar-0.20230330/src/culendar/cul/culendar.py` & `culendar-0.20230510/culendar/cul/culendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-#! /usr/bin/env python3
-# coding: utf-8
 import curses
 import datetime
-from . import calendar, inputs, culdav, getkey
+import re
+
+from . import (
+    calendar,
+    culdav,
+    getkey,
+    inputs,
+)
 
 
 class Culendar:
     def __init__(self, screen, conf, day, cal, caldav, todo):
         self._screen = screen
         self.conf = conf  # use the specific setter
 
@@ -113,15 +118,15 @@
 ###############################################################################
     def dead_duck(self):
         self.clear_cal()
         text = _("\_x< A dead duck. That's all such a small terminal deserves.")
         self._screen.addstr(0, 0, text[0:(self._width-1)*(self._ymax-1)])
 
         key = ""
-        while not((key in self.conf.keys['quit']) or (key == 'KEY_RESIZE')):
+        while key not in self.conf.keys['quit'] and key != 'KEY_RESIZE':
             key = self.getkey()
         if key in self.conf.keys['quit']:
             exit()
         else:
             self.update()
 
     def update(self):
@@ -221,15 +226,15 @@
         try:
             if abs(self.day.month-newmonth) != abs(shift):  # year changed
                 self.addyear(int(shift/abs(shift)))  # sign(shift)
             daytmp = self.day.replace(month=newmonth)
             delta = daytmp - self.day
             self.addday(delta.days)  # use the proper function
         except:  # we can't, that's a day is out of range for month
-                # ie, from 31 January to 31 February
+                 # ie, from 31 January to 31 February
             self.addday(shift*30)  # fallback function
 
     def addday(self, shift):
         # change day: autoswitch from todo bar if any
         if self._todohl:
             self._todohl = 0
             self.draw_header()  # hl the weekbar
@@ -358,57 +363,55 @@
                     self.update()
                 self.clear_footer()
                 return  # exit here
 
             # the footer will be useful, clear it
             self.clear_footer()
             # ask question
-            self._screen.addstr(self._ymax-2, 0,
-  _("Edit: (1) [s]tart time, (2) [e]nd time, (3) [d]escription, (4) [p]lace"))
+            label = _("Edit: (1) [s]tart time, (2) [e]nd time, (3) [d]escription, (4) [p]lace")
+            keys = re.findall('\[(.)\]', label)
+            self._screen.addstr(self._ymax-2, 0, label)
             s = self.getkey()
             if s == "KEY_RESIZE":
                 self.update()
                 return
             self.clear_footer()
-            if not (s in ['1', '2', '3', '4', 's', 'e', 'd', 'p']):
-                return
-            if s in ['1', 's']:
+            if s in ('1', keys[0]):
                 ed = event.date+datetime.timedelta(seconds=event.duration)
                 sd = self.ask_starttime()
                 if sd == "CUL_CANCEL":
                     return   # cancel edit event
                 if sd > ed:  # shift the event to the new starting hour
                     d = event.duration
                 else:  # keep the same end hour
                     # recompute duration
                     d = (ed-sd).seconds
-            if s in ['2', 'e']:
+                event.date = sd
+                event.duration = d
+            elif s in ('2', keys[1]):
                 ed = self.ask_endtime(event.date)
                 if ed == "CUL_CANCEL":
                     return  # cancel edit event
                 d = (ed - event.date).seconds
-            if s in ['3', 'd']:
+                event.duration = d
+            elif s in ('3', keys[2]):
                 desc, place = self.ask_description(event)
                 if desc == "CUL_CANCEL":
                     return  # canceled edition
-            if s in ['4', 'p']:
-                place = self.ask_place(event)
-                if place == "CUL_CANCEL":
-                    return  # canceled edition
-            # update the event
-            if s in ['1', 's']:
-                event.date = sd
-            if s in ['1', 's', '2', 'e']:
-                event.duration = d
-            if s in ['3', 'd']:
                 event.summary = desc
                 if place:  # non empty
                     event.place = place
-            if s in ['4', 'p']:
+            elif s in ('4', keys[3]):
+                place = self.ask_place(event)
+                if place == "CUL_CANCEL":
+                    return  # canceled edition
                 event.place = place
+            else:
+                return
+
             # sort the events
             self._cal.sort()
             # recompute calweek
             self._calweek = calendar.extract_week(self._cal, self._caldav,
                                                   self._day, self,
                                                   autosync=0)
             if event.caldav:  # update the corresponding caldav
@@ -525,15 +528,16 @@
                 data = "CUL_CANCEL"
                 start_time = 0
         return self.post_check_input(data, start_time)
 
     def ask_endtime(self, start_date):
         # ask endtime, return duration of event
         question = (
-       _("Enter end time ([hh:mm], [hhmm], [hh] or [h]) or duration ([+mm]):"))
+            _("Enter end time ([hh:mm], [hhmm], [hh] or [h]) or duration ([+mm]):")
+        )
         end_date = None
         while end_date is None:
             data = self.ask_generic(question)
             if data != "CUL_CANCEL":
                 end_date = data.check_duration(self._day, start_date)
             else:
                 data = "CUL_CANCEL"
@@ -564,15 +568,16 @@
         try:
             return data.text
         except:
             return "CUL_CANCEL"
 
     def ask_day(self):
         question = (
-        _("Enter day ([yyyy/]mm/dd] or [yyyy]mmdd, [Enter for today]):"))
+            _("Enter day ([yyyy/]mm/dd] or [yyyy]mmdd, [Enter for today]):")
+        )
         new_day = None
         while new_day is None:
             data = self.ask_generic(question)
             if data != "CUL_CANCEL":
                 new_day = data.check_day(self._day)
             else:
                 data = "CUL_CANCEL"
@@ -1157,15 +1162,16 @@
 ###############################################################################
 
     def save(self):
         calendar.save(self._cal, self._todo, self._conf, self._caldav)
 
     def importcal(self):
         question = (
-       _("Enter the file name to import (ical or calcurse): (filename [tag])"))
+            _("Enter the file name to import (ical or calcurse): (filename [tag])")
+        )
         filename = self.ask_filename("rb", question)
         tag = 0  # default value
         if filename == "CUL_CANCEL":
             return
         if ((filename[-2] == " ")
                 and (filename[-1] in [str(i) for i in range(8)])):
             tag = int(filename[-1])
@@ -1192,25 +1198,25 @@
             existingevents.append(se.date.strftime('%Y%m%d%H%M')
                                   + str(se.duration)
                                   + se.summary.replace(' ', ''))
         for e in cal.events:
             currentevent = (e.date.strftime('%Y%m%d%H%M')
                             + str(e.duration)
                             + e.summary.replace(' ', ''))
-            if not(currentevent in existingevents):
+            if currentevent not in existingevents:
                 self._cal.add_event(e)
         self._cal.sort()
         self.draw_cal()
         self.inform(_("New events imported!"))
 
     def exportcal(self):
         # returns 1 if successful
         self.clear_footer()
         key = ""
-        while not(key in ["i", "I", "c", "C", "q", "Q", ""]):
+        while key not in ["i", "I", "c", "C", "q", "Q", ""]:
             self._screen.addstr(self._ymax-2, 0,
                                 _("Export to [i]cal or to [c]alcurse?"))
             self._screen.addstr(self._ymax-1, 0, "[i/c]")
             key = self.getkey()
             if key == "KEY_RESIZE":
                 self.update()
                 return
```

### Comparing `culendar-0.20230330/src/culendar/cul/getkey.py` & `culendar-0.20230510/culendar/cul/getkey.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-#! /usr/bin/env python3
-# coding: utf-8
+"""
+function to deal properly with all kind of typed key
+get_wch() returns a str for standard keys;
+for functions keys, sometimes string names, sometimes escaped sequences,
+sometimes ordinal integers.
+stupid function that translates different possibilities into strings
+for the fun, it's terminal-dependant
+
+roughly tested with urvxt, screen, xterm terminals
+probably doesn't work with yours
+"""
 import curses
 
-# function to deal properly with all kind of typed key
-# get_wch() returns a str for standard keys;
-# for functions keys, sometimes string names, sometimes escaped sequences,
-# sometimes ordinal integers.
-# stupid function that translates different possibilities into strings
-# for the fun, it's terminal-dependant
-
-# roughly tested with urvxt, screen, xterm terminals
-# probably doesn't work with yours
-
 
 def getkey(stdscr, debug=False):
     key = stdscr.get_wch()
     origkey = key
     if key == "":
         # half delay mode of 1/10s: no input key raises an error
         # assumption: no humain being type ESC + real keys so fast
@@ -135,24 +134,24 @@
         else:
             if not debug:
                 key = ""
             else:
                 key = str(key)
     return key
 
-## comment previous line and uncomment the followings to use the standalone
+# comment previous line and uncomment the followings to use the standalone
 #    if debug:
 #        return key, origkey
 #    else:
 #        return key
 #
-## standalone function
-## useful to complete the lists
-##import curses
-#def main(stdscr):
+# standalone function
+# useful to complete the lists
+# import curses
+# def main(stdscr):
 #    curses.noecho()
 #    mmask = (curses.BUTTON1_PRESSED + curses.BUTTON1_RELEASED
 #             + curses.BUTTON1_CLICKED + curses.BUTTON1_DOUBLE_CLICKED
 #             + curses.BUTTON1_TRIPLE_CLICKED + curses.BUTTON_CTRL)
 #    curses.mousemask(mmask)
 #
 #    ymax, xmax = stdscr.getmaxyx()
@@ -160,8 +159,8 @@
 #    i = 0
 #    while k != "q":
 #        k, ok = getkey(stdscr, debug=True)
 #        stdscr.addstr(i%ymax, 0, "                       ")
 #        stdscr.addstr(i%ymax, 0, str(k))
 #        stdscr.addstr(i%ymax, 15, str(ok))
 #        i += 1
-#curses.wrapper(main)
+# curses.wrapper(main)
```

### Comparing `culendar-0.20230330/src/culendar/cul/helpscr.py` & `culendar-0.20230510/culendar/cul/helpscr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-#! /usr/bin/env python3
-# coding: utf-8
 import curses
+
 from . import getkey
 
 
 class Help:
     def __init__(self, scr, conf):
         self._screen = scr
         self._conf = conf
@@ -75,26 +74,25 @@
         # if ridiculously small terminal
         if (self._x < 25) or (self._y < 5):
             self._screen.clear()
             text = _("\_x< A dead duck. That's all such a small terminal deserves.")
             self._screen.addstr(0, 0, text[0:(self._x-1)*(self._y-1)])
 
             key = ""
-            while not((key in self._conf.keys['quit'])
-                      or (key == 'KEY_RESIZE')):
+            while key not in self._conf.keys['quit'] and key != 'KEY_RESIZE':
                 key = getkey.getkey(self._screen, self._conf.debug)
             if key in self._conf.keys['quit']:
                 exit()
             else:
                 self.draw_help_screen()
 
         # draw screen
         headleft = _("q: quit help")
         headcenter = _("Culendar help screen")
-        headcenter += " 0.20230401"
+        headcenter += " 0.20230510"
         self._screen.border()
         self._screen.hline(2, 1, curses.ACS_HLINE, self._x-2)
         self._screen.addch(2, 0, curses.ACS_LTEE)
         self._screen.addch(2, self._x-1, curses.ACS_RTEE)
         self._screen.addstr(1, 1, headleft, curses.A_BOLD)
         self._screen.addstr(1, (self._x-len(headcenter))//2+1,
                             headcenter, curses.A_BOLD)
@@ -124,15 +122,15 @@
                 # treat it separately
                 self._pad.addstr(shift, 0, _("number n>0"))
                 # second column: small name
                 self._pad.addstr(shift, colsize, "repetition")
                 # third column: description
                 desc = _("Repeat following command n times (when reasonable)")
                 self._pad.addstr(shift, 2*colsize, desc)
-                shift +=1
+                shift += 1
 
             for i, k in enumerate(category[0]):
                 # first column: keys
                 listkeys = ""
                 for ck in self._conf.keys[k]:
                     if ck == "\t":
                         listkeys += "TAB, "
```

### Comparing `culendar-0.20230330/src/culendar/cul/inputs.py` & `culendar-0.20230510/culendar/cul/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,644 +1,642 @@
-00000000: 2321 202f 7573 722f 6269 6e2f 656e 7620  #! /usr/bin/env 
-00000010: 7079 7468 6f6e 330a 2320 636f 6469 6e67  python3.# coding
-00000020: 3a20 7574 662d 380a 696d 706f 7274 2063  : utf-8.import c
-00000030: 7572 7365 730a 696d 706f 7274 2064 6174  urses.import dat
-00000040: 6574 696d 650a 6672 6f6d 202e 2069 6d70  etime.from . imp
-00000050: 6f72 7420 6765 746b 6579 0a0a 0a23 2054  ort getkey...# T
-00000060: 4f44 4f3a 2064 6561 6c20 7769 7468 2074  ODO: deal with t
-00000070: 6f6f 206c 6f6e 6720 6c69 6e65 730a 636c  oo long lines.cl
-00000080: 6173 7320 496e 7075 743a 0a20 2020 2064  ass Input:.    d
-00000090: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000000a0: 2c20 7363 7265 656e 2c20 7465 7874 3d22  , screen, text="
-000000b0: 222c 2070 7764 3d46 616c 7365 293a 0a20  ", pwd=False):. 
-000000c0: 2020 2020 2020 2073 656c 662e 5f73 6372         self._scr
-000000d0: 6565 6e20 3d20 7363 7265 656e 0a20 2020  een = screen.   
-000000e0: 2020 2020 2073 656c 662e 7363 7265 656e       self.screen
-000000f0: 5f75 7064 6174 6528 290a 2020 2020 2020  _update().      
-00000100: 2020 7365 6c66 2e74 6578 7420 3d20 7465    self.text = te
-00000110: 7874 0a20 2020 2020 2020 2023 2073 656c  xt.        # sel
-00000120: 662e 5f6d 6178 706f 7320 6973 2063 7572  f._maxpos is cur
-00000130: 736f 7220 6d61 7820 706f 7369 7469 6f6e  sor max position
-00000140: 2069 6e20 782c 2064 6566 696e 6564 2062   in x, defined b
-00000150: 7920 7465 7874 2073 6574 7465 720a 2020  y text setter.  
-00000160: 2020 2020 2020 7365 6c66 2e5f 706f 7320        self._pos 
-00000170: 3d20 7365 6c66 2e5f 6d61 7870 6f73 2020  = self._maxpos  
-00000180: 2023 2063 7572 736f 7220 706f 7369 7469   # cursor positi
-00000190: 6f6e 2069 6e20 7465 7874 0a20 2020 2020  on in text.     
-000001a0: 2020 2073 656c 662e 5f70 7764 203d 2070     self._pwd = p
-000001b0: 7764 0a0a 2020 2020 4070 726f 7065 7274  wd..    @propert
-000001c0: 790a 2020 2020 6465 6620 7465 7874 2873  y.    def text(s
-000001d0: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
-000001e0: 7475 726e 2073 656c 662e 5f74 6578 740a  turn self._text.
-000001f0: 0a20 2020 2040 7465 7874 2e73 6574 7465  .    @text.sette
-00000200: 720a 2020 2020 6465 6620 7465 7874 2873  r.    def text(s
-00000210: 656c 662c 206e 6577 7465 7874 293a 0a20  elf, newtext):. 
-00000220: 2020 2020 2020 2073 656c 662e 5f74 6578         self._tex
-00000230: 7420 3d20 6e65 7774 6578 740a 2020 2020  t = newtext.    
-00000240: 2020 2020 7365 6c66 2e5f 6d61 7870 6f73      self._maxpos
-00000250: 203d 206c 656e 2873 656c 662e 5f74 6578   = len(self._tex
-00000260: 7429 0a0a 2020 2020 6465 6620 7363 7265  t)..    def scre
-00000270: 656e 5f75 7064 6174 6528 7365 6c66 293a  en_update(self):
-00000280: 0a20 2020 2020 2020 2073 656c 662e 5f79  .        self._y
-00000290: 6d61 782c 2073 656c 662e 5f78 6d61 7820  max, self._xmax 
-000002a0: 3d20 7365 6c66 2e5f 7363 7265 656e 2e67  = self._screen.g
-000002b0: 6574 6d61 7879 7828 290a 2020 2020 2020  etmaxyx().      
-000002c0: 2020 7365 6c66 2e5f 7920 3d20 7365 6c66    self._y = self
-000002d0: 2e5f 796d 6178 202d 2031 0a0a 2020 2020  ._ymax - 1..    
-000002e0: 6465 6620 7265 7365 745f 7465 7874 2873  def reset_text(s
-000002f0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00000300: 6c66 2e74 6578 7420 3d20 2222 0a20 2020  lf.text = "".   
-00000310: 2020 2020 2073 656c 662e 5f70 6f73 203d       self._pos =
-00000320: 2030 0a0a 2020 2020 6465 6620 6465 6c65   0..    def dele
-00000330: 7465 5f63 6861 7228 7365 6c66 2c20 6f66  te_char(self, of
-00000340: 6673 6574 293a 0a20 2020 2020 2020 2069  fset):.        i
-00000350: 6620 7365 6c66 2e5f 706f 7320 3d3d 2030  f self._pos == 0
-00000360: 3a0a 2020 2020 2020 2020 2020 2020 6f66  :.            of
-00000370: 6673 6574 203d 2030 2020 2320 6176 6f69  fset = 0  # avoi
-00000380: 6420 6261 636b 7370 6163 696e 6720 2d31  d backspacing -1
-00000390: 2063 6861 7261 6374 6572 0a20 2020 2020   character.     
-000003a0: 2020 2064 656c 6574 6564 203d 2073 656c     deleted = sel
-000003b0: 662e 5f70 6f73 202b 206f 6666 7365 740a  f._pos + offset.
-000003c0: 2020 2020 2020 2020 7365 6c66 2e74 6578          self.tex
-000003d0: 7420 3d20 7365 6c66 2e74 6578 745b 3a64  t = self.text[:d
-000003e0: 656c 6574 6564 5d20 2b20 7365 6c66 2e74  eleted] + self.t
-000003f0: 6578 745b 6465 6c65 7465 642b 313a 5d0a  ext[deleted+1:].
-00000400: 2020 2020 2020 2020 7365 6c66 2e5f 706f          self._po
-00000410: 7320 2b3d 206f 6666 7365 740a 2020 2020  s += offset.    
-00000420: 2020 2020 2320 6572 6173 6520 616e 6420      # erase and 
-00000430: 7265 6472 6177 2074 6865 206e 6577 2074  redraw the new t
-00000440: 6578 740a 2020 2020 2020 2020 7365 6c66  ext.        self
-00000450: 2e64 656c 6574 655f 7465 7874 2829 0a20  .delete_text(). 
-00000460: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
-00000470: 5f74 6578 7428 290a 0a20 2020 2064 6566  _text()..    def
-00000480: 2064 656c 6574 655f 7061 7274 2873 656c   delete_part(sel
-00000490: 662c 2062 6567 696e 2c20 656e 6429 3a0a  f, begin, end):.
-000004a0: 2020 2020 2020 2020 7365 6c66 2e74 6578          self.tex
-000004b0: 7420 3d20 7365 6c66 2e74 6578 745b 3a62  t = self.text[:b
-000004c0: 6567 696e 5d20 2b20 7365 6c66 2e74 6578  egin] + self.tex
-000004d0: 745b 656e 643a 5d0a 2020 2020 2020 2020  t[end:].        
-000004e0: 7365 6c66 2e5f 706f 7320 3d20 6d61 7828  self._pos = max(
-000004f0: 302c 2073 656c 662e 5f70 6f73 202d 2028  0, self._pos - (
-00000500: 656e 642d 6265 6769 6e29 290a 2020 2020  end-begin)).    
-00000510: 2020 2020 2320 6572 6173 6520 616e 6420      # erase and 
-00000520: 7265 6472 6177 2074 6865 206e 6577 2074  redraw the new t
-00000530: 6578 740a 2020 2020 2020 2020 7365 6c66  ext.        self
-00000540: 2e64 656c 6574 655f 7465 7874 2829 0a20  .delete_text(). 
-00000550: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
-00000560: 5f74 6578 7428 290a 0a20 2020 2064 6566  _text()..    def
-00000570: 2061 6464 5f63 6861 7228 7365 6c66 2c20   add_char(self, 
-00000580: 6b65 7929 3a0a 2020 2020 2020 2020 7365  key):.        se
-00000590: 6c66 2e74 6578 7420 3d20 7365 6c66 2e74  lf.text = self.t
-000005a0: 6578 745b 3a73 656c 662e 5f70 6f73 5d20  ext[:self._pos] 
-000005b0: 2b20 6b65 7920 2b20 7365 6c66 2e74 6578  + key + self.tex
-000005c0: 745b 7365 6c66 2e5f 706f 733a 5d0a 2020  t[self._pos:].  
-000005d0: 2020 2020 2020 7365 6c66 2e5f 706f 7320        self._pos 
-000005e0: 2b3d 2031 0a20 2020 2020 2020 2073 656c  += 1.        sel
-000005f0: 662e 6472 6177 5f74 6578 7428 290a 0a20  f.draw_text().. 
-00000600: 2020 2064 6566 2064 7261 775f 7465 7874     def draw_text
-00000610: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00000620: 6c65 6e74 6578 7420 3d20 6c65 6e28 7365  lentext = len(se
-00000630: 6c66 2e5f 7465 7874 290a 2020 2020 2020  lf._text).      
-00000640: 2020 6f6c 645f 706f 7320 3d20 4e6f 6e65    old_pos = None
-00000650: 0a20 2020 2020 2020 2069 6620 6c65 6e74  .        if lent
-00000660: 6578 7420 3e20 7365 6c66 2e5f 786d 6178  ext > self._xmax
-00000670: 202d 2031 3a0a 2020 2020 2020 2020 2020   - 1:.          
-00000680: 2020 7465 7874 203d 2073 656c 662e 5f74    text = self._t
-00000690: 6578 745b 6c65 6e74 6578 7420 2d20 7365  ext[lentext - se
-000006a0: 6c66 2e5f 786d 6178 202b 2031 3a5d 0a20  lf._xmax + 1:]. 
-000006b0: 2020 2020 2020 2020 2020 206f 6c64 5f70             old_p
-000006c0: 6f73 203d 2073 656c 662e 5f70 6f73 0a20  os = self._pos. 
-000006d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000006e0: 5f70 6f73 203d 2073 656c 662e 5f78 6d61  _pos = self._xma
-000006f0: 7820 2d20 310a 2020 2020 2020 2020 656c  x - 1.        el
-00000700: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00000710: 7465 7874 203d 2073 656c 662e 5f74 6578  text = self._tex
-00000720: 740a 2020 2020 2020 2020 6966 206e 6f74  t.        if not
-00000730: 2073 656c 662e 5f70 7764 3a0a 2020 2020   self._pwd:.    
-00000740: 2020 2020 2020 2020 7365 6c66 2e5f 7363          self._sc
-00000750: 7265 656e 2e61 6464 7374 7228 7365 6c66  reen.addstr(self
-00000760: 2e5f 792c 2030 2c20 7465 7874 290a 2020  ._y, 0, text).  
-00000770: 2020 2020 2020 656c 7365 3a20 2023 206f        else:  # o
-00000780: 6266 7573 6361 7465 2070 6173 7377 6f72  bfuscate passwor
-00000790: 640a 2020 2020 2020 2020 2020 2020 7365  d.            se
-000007a0: 6c66 2e5f 7363 7265 656e 2e61 6464 7374  lf._screen.addst
-000007b0: 7228 7365 6c66 2e5f 792c 2030 2c20 222a  r(self._y, 0, "*
-000007c0: 222a 6c65 6e28 7465 7874 2929 0a20 2020  "*len(text)).   
-000007d0: 2020 2020 2073 656c 662e 6472 6177 5f63       self.draw_c
-000007e0: 7572 736f 7228 290a 2020 2020 2020 2020  ursor().        
-000007f0: 6966 206f 6c64 5f70 6f73 3a0a 2020 2020  if old_pos:.    
-00000800: 2020 2020 2020 2020 7365 6c66 2e5f 706f          self._po
-00000810: 7320 3d20 6f6c 645f 706f 730a 0a20 2020  s = old_pos..   
-00000820: 2064 6566 2064 656c 6574 655f 7465 7874   def delete_text
-00000830: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00000840: 7365 6c66 2e5f 7363 7265 656e 2e68 6c69  self._screen.hli
-00000850: 6e65 2873 656c 662e 5f79 2c20 302c 2022  ne(self._y, 0, "
-00000860: 2022 2c20 7365 6c66 2e5f 786d 6178 2d31   ", self._xmax-1
-00000870: 290a 0a20 2020 2064 6566 2064 7261 775f  )..    def draw_
-00000880: 6375 7273 6f72 2873 656c 6629 3a0a 2020  cursor(self):.  
-00000890: 2020 2020 2020 2320 7075 7420 7468 6520        # put the 
-000008a0: 6375 7273 6f73 2061 7420 7468 6520 676f  cursos at the go
-000008b0: 6f64 2070 6f73 6974 696f 6e0a 2020 2020  od position.    
-000008c0: 2020 2020 6966 2073 656c 662e 5f70 6f73      if self._pos
-000008d0: 203e 2073 656c 662e 5f78 6d61 782d 313a   > self._xmax-1:
-000008e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000008f0: 662e 5f73 6372 6565 6e2e 6d6f 7665 2873  f._screen.move(s
-00000900: 656c 662e 5f79 2c20 7365 6c66 2e5f 786d  elf._y, self._xm
-00000910: 6178 2d31 290a 2020 2020 2020 2020 656c  ax-1).        el
-00000920: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00000930: 7365 6c66 2e5f 7363 7265 656e 2e6d 6f76  self._screen.mov
-00000940: 6528 7365 6c66 2e5f 792c 2073 656c 662e  e(self._y, self.
-00000950: 5f70 6f73 290a 0a20 2020 2064 6566 206d  _pos)..    def m
-00000960: 6f76 655f 6375 7273 6f72 2873 656c 662c  ove_cursor(self,
-00000970: 206e 6577 706f 7329 3a0a 2020 2020 2020   newpos):.      
-00000980: 2020 7365 6c66 2e5f 706f 7320 3d20 6e65    self._pos = ne
-00000990: 7770 6f73 0a20 2020 2020 2020 2073 656c  wpos.        sel
-000009a0: 662e 6472 6177 5f63 7572 736f 7228 290a  f.draw_cursor().
-000009b0: 0a20 2020 2064 6566 2064 656c 6574 655f  .    def delete_
-000009c0: 6672 6f6d 5f63 7572 736f 7228 7365 6c66  from_cursor(self
-000009d0: 2c20 6469 7265 6374 696f 6e29 3a0a 2020  , direction):.  
-000009e0: 2020 2020 2020 6f6c 645f 6d61 7870 6f73        old_maxpos
-000009f0: 203d 2073 656c 662e 5f6d 6178 706f 730a   = self._maxpos.
-00000a00: 2020 2020 2020 2020 6966 2064 6972 6563          if direc
-00000a10: 7469 6f6e 203d 3d20 226c 6566 7422 3a0a  tion == "left":.
-00000a20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000a30: 2e74 6578 7420 3d20 7365 6c66 2e74 6578  .text = self.tex
-00000a40: 745b 7365 6c66 2e5f 706f 733a 5d0a 2020  t[self._pos:].  
-00000a50: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00000a60: 706f 7320 3d20 300a 2020 2020 2020 2020  pos = 0.        
-00000a70: 656c 6966 2064 6972 6563 7469 6f6e 203d  elif direction =
-00000a80: 3d20 2272 6967 6874 223a 0a20 2020 2020  = "right":.     
-00000a90: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
-00000aa0: 203d 2073 656c 662e 7465 7874 5b3a 7365   = self.text[:se
-00000ab0: 6c66 2e5f 706f 735d 0a20 2020 2020 2020  lf._pos].       
-00000ac0: 2020 2020 2073 656c 662e 5f70 6f73 203d       self._pos =
-00000ad0: 2073 656c 662e 5f6d 6178 706f 730a 2020   self._maxpos.  
-00000ae0: 2020 2020 2020 2320 6572 6173 6520 616e        # erase an
-00000af0: 6420 7265 6472 6177 2074 6865 206e 6577  d redraw the new
-00000b00: 2074 6578 740a 2020 2020 2020 2020 7365   text.        se
-00000b10: 6c66 2e64 656c 6574 655f 7465 7874 2829  lf.delete_text()
-00000b20: 0a20 2020 2020 2020 2073 656c 662e 6472  .        self.dr
-00000b30: 6177 5f74 6578 7428 290a 0a20 2020 2064  aw_text()..    d
-00000b40: 6566 2066 696e 645f 6c65 6674 5f77 6f72  ef find_left_wor
-00000b50: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
-00000b60: 2069 6478 203d 202d 310a 2020 2020 2020   idx = -1.      
-00000b70: 2020 666f 7220 692c 2073 2069 6e20 656e    for i, s in en
-00000b80: 756d 6572 6174 6528 7365 6c66 2e74 6578  umerate(self.tex
-00000b90: 745b 3a73 656c 662e 5f70 6f73 2d31 5d29  t[:self._pos-1])
-00000ba0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00000bb0: 2073 203d 3d20 2220 223a 0a20 2020 2020   s == " ":.     
-00000bc0: 2020 2020 2020 2020 2020 2069 6478 203d             idx =
-00000bd0: 2069 202b 2031 0a20 2020 2020 2020 2069   i + 1.        i
-00000be0: 6620 2869 6478 203e 2030 2920 2620 2869  f (idx > 0) & (i
-00000bf0: 6478 203c 2073 656c 662e 5f70 6f73 293a  dx < self._pos):
-00000c00: 2020 2320 736f 6d65 7468 696e 6720 6861    # something ha
-00000c10: 7320 6265 656e 2066 6f75 6e64 0a20 2020  s been found.   
-00000c20: 2020 2020 2020 2020 2023 2073 6563 6f6e           # secon
-00000c30: 6420 636f 6e64 6974 696f 6e20 746f 2070  d condition to p
-00000c40: 7265 7665 6e74 2074 6865 2073 6561 7263  revent the searc
-00000c50: 6820 6672 6f6d 2073 6c69 6365 205b 3a2d  h from slice [:-
-00000c60: 315d 0a20 2020 2020 2020 2020 2020 2072  1].            r
-00000c70: 6574 7572 6e20 6964 780a 2020 2020 2020  eturn idx.      
-00000c80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00000c90: 2020 2020 7265 7475 726e 2030 0a0a 2020      return 0..  
-00000ca0: 2020 6465 6620 6d6f 7665 5f6c 6566 745f    def move_left_
-00000cb0: 776f 7264 2873 656c 6629 3a0a 2020 2020  word(self):.    
-00000cc0: 2020 2020 7365 6c66 2e5f 706f 7320 3d20      self._pos = 
-00000cd0: 7365 6c66 2e66 696e 645f 6c65 6674 5f77  self.find_left_w
-00000ce0: 6f72 6428 290a 2020 2020 2020 2020 7365  ord().        se
-00000cf0: 6c66 2e64 7261 775f 6375 7273 6f72 2829  lf.draw_cursor()
-00000d00: 0a0a 2020 2020 6465 6620 6465 6c65 7465  ..    def delete
-00000d10: 5f6c 6566 745f 776f 7264 2873 656c 6629  _left_word(self)
-00000d20: 3a0a 2020 2020 2020 2020 676f 616c 203d  :.        goal =
-00000d30: 2073 656c 662e 6669 6e64 5f6c 6566 745f   self.find_left_
-00000d40: 776f 7264 2829 0a20 2020 2020 2020 2073  word().        s
-00000d50: 656c 662e 6465 6c65 7465 5f70 6172 7428  elf.delete_part(
-00000d60: 676f 616c 2c20 7365 6c66 2e5f 706f 7329  goal, self._pos)
-00000d70: 0a0a 2020 2020 6465 6620 6669 6e64 5f72  ..    def find_r
-00000d80: 6967 6874 5f77 6f72 6428 7365 6c66 293a  ight_word(self):
-00000d90: 0a20 2020 2020 2020 2069 6478 203d 2073  .        idx = s
-00000da0: 656c 662e 7465 7874 5b73 656c 662e 5f70  elf.text[self._p
-00000db0: 6f73 2b31 3a5d 2e66 696e 6428 2220 2229  os+1:].find(" ")
-00000dc0: 0a20 2020 2020 2020 2069 6620 6964 7820  .        if idx 
-00000dd0: 3e20 303a 2020 2320 736f 6d65 7468 696e  > 0:  # somethin
-00000de0: 6720 6861 7320 6265 656e 2066 6f75 6e64  g has been found
-00000df0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00000e00: 7572 6e20 7365 6c66 2e5f 706f 7320 2b20  urn self._pos + 
-00000e10: 7365 6c66 2e74 6578 745b 7365 6c66 2e5f  self.text[self._
-00000e20: 706f 732b 313a 5d2e 6669 6e64 2822 2022  pos+1:].find(" "
-00000e30: 2920 2b20 310a 2020 2020 2020 2020 656c  ) + 1.        el
-00000e40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00000e50: 7265 7475 726e 2073 656c 662e 5f6d 6178  return self._max
-00000e60: 706f 730a 0a20 2020 2064 6566 206d 6f76  pos..    def mov
-00000e70: 655f 7269 6768 745f 776f 7264 2873 656c  e_right_word(sel
-00000e80: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00000e90: 2e5f 706f 7320 3d20 7365 6c66 2e66 696e  ._pos = self.fin
-00000ea0: 645f 7269 6768 745f 776f 7264 2829 0a20  d_right_word(). 
-00000eb0: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
-00000ec0: 5f63 7572 736f 7228 290a 0a23 2323 2323  _cursor()..#####
+00000000: 696d 706f 7274 2063 7572 7365 730a 696d  import curses.im
+00000010: 706f 7274 2064 6174 6574 696d 650a 0a66  port datetime..f
+00000020: 726f 6d20 2e20 696d 706f 7274 2067 6574  rom . import get
+00000030: 6b65 790a 0a0a 2320 544f 444f 3a20 6465  key...# TODO: de
+00000040: 616c 2077 6974 6820 746f 6f20 6c6f 6e67  al with too long
+00000050: 206c 696e 6573 0a63 6c61 7373 2049 6e70   lines.class Inp
+00000060: 7574 3a0a 2020 2020 6465 6620 5f5f 696e  ut:.    def __in
+00000070: 6974 5f5f 2873 656c 662c 2073 6372 6565  it__(self, scree
+00000080: 6e2c 2074 6578 743d 2222 2c20 7077 643d  n, text="", pwd=
+00000090: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+000000a0: 7365 6c66 2e5f 7363 7265 656e 203d 2073  self._screen = s
+000000b0: 6372 6565 6e0a 2020 2020 2020 2020 7365  creen.        se
+000000c0: 6c66 2e73 6372 6565 6e5f 7570 6461 7465  lf.screen_update
+000000d0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000000e0: 7465 7874 203d 2074 6578 740a 2020 2020  text = text.    
+000000f0: 2020 2020 2320 7365 6c66 2e5f 6d61 7870      # self._maxp
+00000100: 6f73 2069 7320 6375 7273 6f72 206d 6178  os is cursor max
+00000110: 2070 6f73 6974 696f 6e20 696e 2078 2c20   position in x, 
+00000120: 6465 6669 6e65 6420 6279 2074 6578 7420  defined by text 
+00000130: 7365 7474 6572 0a20 2020 2020 2020 2073  setter.        s
+00000140: 656c 662e 5f70 6f73 203d 2073 656c 662e  elf._pos = self.
+00000150: 5f6d 6178 706f 7320 2020 2320 6375 7273  _maxpos   # curs
+00000160: 6f72 2070 6f73 6974 696f 6e20 696e 2074  or position in t
+00000170: 6578 740a 2020 2020 2020 2020 7365 6c66  ext.        self
+00000180: 2e5f 7077 6420 3d20 7077 640a 0a20 2020  ._pwd = pwd..   
+00000190: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+000001a0: 6566 2074 6578 7428 7365 6c66 293a 0a20  ef text(self):. 
+000001b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000001c0: 6c66 2e5f 7465 7874 0a0a 2020 2020 4074  lf._text..    @t
+000001d0: 6578 742e 7365 7474 6572 0a20 2020 2064  ext.setter.    d
+000001e0: 6566 2074 6578 7428 7365 6c66 2c20 6e65  ef text(self, ne
+000001f0: 7774 6578 7429 3a0a 2020 2020 2020 2020  wtext):.        
+00000200: 7365 6c66 2e5f 7465 7874 203d 206e 6577  self._text = new
+00000210: 7465 7874 0a20 2020 2020 2020 2073 656c  text.        sel
+00000220: 662e 5f6d 6178 706f 7320 3d20 6c65 6e28  f._maxpos = len(
+00000230: 7365 6c66 2e5f 7465 7874 290a 0a20 2020  self._text)..   
+00000240: 2064 6566 2073 6372 6565 6e5f 7570 6461   def screen_upda
+00000250: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00000260: 2020 7365 6c66 2e5f 796d 6178 2c20 7365    self._ymax, se
+00000270: 6c66 2e5f 786d 6178 203d 2073 656c 662e  lf._xmax = self.
+00000280: 5f73 6372 6565 6e2e 6765 746d 6178 7978  _screen.getmaxyx
+00000290: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000002a0: 5f79 203d 2073 656c 662e 5f79 6d61 7820  _y = self._ymax 
+000002b0: 2d20 310a 0a20 2020 2064 6566 2072 6573  - 1..    def res
+000002c0: 6574 5f74 6578 7428 7365 6c66 293a 0a20  et_text(self):. 
+000002d0: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
+000002e0: 203d 2022 220a 2020 2020 2020 2020 7365   = "".        se
+000002f0: 6c66 2e5f 706f 7320 3d20 300a 0a20 2020  lf._pos = 0..   
+00000300: 2064 6566 2064 656c 6574 655f 6368 6172   def delete_char
+00000310: 2873 656c 662c 206f 6666 7365 7429 3a0a  (self, offset):.
+00000320: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00000330: 5f70 6f73 203d 3d20 303a 0a20 2020 2020  _pos == 0:.     
+00000340: 2020 2020 2020 206f 6666 7365 7420 3d20         offset = 
+00000350: 3020 2023 2061 766f 6964 2062 6163 6b73  0  # avoid backs
+00000360: 7061 6369 6e67 202d 3120 6368 6172 6163  pacing -1 charac
+00000370: 7465 720a 2020 2020 2020 2020 6465 6c65  ter.        dele
+00000380: 7465 6420 3d20 7365 6c66 2e5f 706f 7320  ted = self._pos 
+00000390: 2b20 6f66 6673 6574 0a20 2020 2020 2020  + offset.       
+000003a0: 2073 656c 662e 7465 7874 203d 2073 656c   self.text = sel
+000003b0: 662e 7465 7874 5b3a 6465 6c65 7465 645d  f.text[:deleted]
+000003c0: 202b 2073 656c 662e 7465 7874 5b64 656c   + self.text[del
+000003d0: 6574 6564 2b31 3a5d 0a20 2020 2020 2020  eted+1:].       
+000003e0: 2073 656c 662e 5f70 6f73 202b 3d20 6f66   self._pos += of
+000003f0: 6673 6574 0a20 2020 2020 2020 2023 2065  fset.        # e
+00000400: 7261 7365 2061 6e64 2072 6564 7261 7720  rase and redraw 
+00000410: 7468 6520 6e65 7720 7465 7874 0a20 2020  the new text.   
+00000420: 2020 2020 2073 656c 662e 6465 6c65 7465       self.delete
+00000430: 5f74 6578 7428 290a 2020 2020 2020 2020  _text().        
+00000440: 7365 6c66 2e64 7261 775f 7465 7874 2829  self.draw_text()
+00000450: 0a0a 2020 2020 6465 6620 6465 6c65 7465  ..    def delete
+00000460: 5f70 6172 7428 7365 6c66 2c20 6265 6769  _part(self, begi
+00000470: 6e2c 2065 6e64 293a 0a20 2020 2020 2020  n, end):.       
+00000480: 2073 656c 662e 7465 7874 203d 2073 656c   self.text = sel
+00000490: 662e 7465 7874 5b3a 6265 6769 6e5d 202b  f.text[:begin] +
+000004a0: 2073 656c 662e 7465 7874 5b65 6e64 3a5d   self.text[end:]
+000004b0: 0a20 2020 2020 2020 2073 656c 662e 5f70  .        self._p
+000004c0: 6f73 203d 206d 6178 2830 2c20 7365 6c66  os = max(0, self
+000004d0: 2e5f 706f 7320 2d20 2865 6e64 2d62 6567  ._pos - (end-beg
+000004e0: 696e 2929 0a20 2020 2020 2020 2023 2065  in)).        # e
+000004f0: 7261 7365 2061 6e64 2072 6564 7261 7720  rase and redraw 
+00000500: 7468 6520 6e65 7720 7465 7874 0a20 2020  the new text.   
+00000510: 2020 2020 2073 656c 662e 6465 6c65 7465       self.delete
+00000520: 5f74 6578 7428 290a 2020 2020 2020 2020  _text().        
+00000530: 7365 6c66 2e64 7261 775f 7465 7874 2829  self.draw_text()
+00000540: 0a0a 2020 2020 6465 6620 6164 645f 6368  ..    def add_ch
+00000550: 6172 2873 656c 662c 206b 6579 293a 0a20  ar(self, key):. 
+00000560: 2020 2020 2020 2073 656c 662e 7465 7874         self.text
+00000570: 203d 2073 656c 662e 7465 7874 5b3a 7365   = self.text[:se
+00000580: 6c66 2e5f 706f 735d 202b 206b 6579 202b  lf._pos] + key +
+00000590: 2073 656c 662e 7465 7874 5b73 656c 662e   self.text[self.
+000005a0: 5f70 6f73 3a5d 0a20 2020 2020 2020 2073  _pos:].        s
+000005b0: 656c 662e 5f70 6f73 202b 3d20 310a 2020  elf._pos += 1.  
+000005c0: 2020 2020 2020 7365 6c66 2e64 7261 775f        self.draw_
+000005d0: 7465 7874 2829 0a0a 2020 2020 6465 6620  text()..    def 
+000005e0: 6472 6177 5f74 6578 7428 7365 6c66 293a  draw_text(self):
+000005f0: 0a20 2020 2020 2020 206c 656e 7465 7874  .        lentext
+00000600: 203d 206c 656e 2873 656c 662e 5f74 6578   = len(self._tex
+00000610: 7429 0a20 2020 2020 2020 206f 6c64 5f70  t).        old_p
+00000620: 6f73 203d 204e 6f6e 650a 2020 2020 2020  os = None.      
+00000630: 2020 6966 206c 656e 7465 7874 203e 2073    if lentext > s
+00000640: 656c 662e 5f78 6d61 7820 2d20 313a 0a20  elf._xmax - 1:. 
+00000650: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+00000660: 3d20 7365 6c66 2e5f 7465 7874 5b6c 656e  = self._text[len
+00000670: 7465 7874 202d 2073 656c 662e 5f78 6d61  text - self._xma
+00000680: 7820 2b20 313a 5d0a 2020 2020 2020 2020  x + 1:].        
+00000690: 2020 2020 6f6c 645f 706f 7320 3d20 7365      old_pos = se
+000006a0: 6c66 2e5f 706f 730a 2020 2020 2020 2020  lf._pos.        
+000006b0: 2020 2020 7365 6c66 2e5f 706f 7320 3d20      self._pos = 
+000006c0: 7365 6c66 2e5f 786d 6178 202d 2031 0a20  self._xmax - 1. 
+000006d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000006e0: 2020 2020 2020 2020 2074 6578 7420 3d20           text = 
+000006f0: 7365 6c66 2e5f 7465 7874 0a20 2020 2020  self._text.     
+00000700: 2020 2069 6620 6e6f 7420 7365 6c66 2e5f     if not self._
+00000710: 7077 643a 0a20 2020 2020 2020 2020 2020  pwd:.           
+00000720: 2073 656c 662e 5f73 6372 6565 6e2e 6164   self._screen.ad
+00000730: 6473 7472 2873 656c 662e 5f79 2c20 302c  dstr(self._y, 0,
+00000740: 2074 6578 7429 0a20 2020 2020 2020 2065   text).        e
+00000750: 6c73 653a 2020 2320 6f62 6675 7363 6174  lse:  # obfuscat
+00000760: 6520 7061 7373 776f 7264 0a20 2020 2020  e password.     
+00000770: 2020 2020 2020 2073 656c 662e 5f73 6372         self._scr
+00000780: 6565 6e2e 6164 6473 7472 2873 656c 662e  een.addstr(self.
+00000790: 5f79 2c20 302c 2022 2a22 2a6c 656e 2874  _y, 0, "*"*len(t
+000007a0: 6578 7429 290a 2020 2020 2020 2020 7365  ext)).        se
+000007b0: 6c66 2e64 7261 775f 6375 7273 6f72 2829  lf.draw_cursor()
+000007c0: 0a20 2020 2020 2020 2069 6620 6f6c 645f  .        if old_
+000007d0: 706f 733a 0a20 2020 2020 2020 2020 2020  pos:.           
+000007e0: 2073 656c 662e 5f70 6f73 203d 206f 6c64   self._pos = old
+000007f0: 5f70 6f73 0a0a 2020 2020 6465 6620 6465  _pos..    def de
+00000800: 6c65 7465 5f74 6578 7428 7365 6c66 293a  lete_text(self):
+00000810: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+00000820: 6372 6565 6e2e 686c 696e 6528 7365 6c66  creen.hline(self
+00000830: 2e5f 792c 2030 2c20 2220 222c 2073 656c  ._y, 0, " ", sel
+00000840: 662e 5f78 6d61 782d 3129 0a0a 2020 2020  f._xmax-1)..    
+00000850: 6465 6620 6472 6177 5f63 7572 736f 7228  def draw_cursor(
+00000860: 7365 6c66 293a 0a20 2020 2020 2020 2023  self):.        #
+00000870: 2070 7574 2074 6865 2063 7572 736f 7320   put the cursos 
+00000880: 6174 2074 6865 2067 6f6f 6420 706f 7369  at the good posi
+00000890: 7469 6f6e 0a20 2020 2020 2020 2069 6620  tion.        if 
+000008a0: 7365 6c66 2e5f 706f 7320 3e20 7365 6c66  self._pos > self
+000008b0: 2e5f 786d 6178 2d31 3a0a 2020 2020 2020  ._xmax-1:.      
+000008c0: 2020 2020 2020 7365 6c66 2e5f 7363 7265        self._scre
+000008d0: 656e 2e6d 6f76 6528 7365 6c66 2e5f 792c  en.move(self._y,
+000008e0: 2073 656c 662e 5f78 6d61 782d 3129 0a20   self._xmax-1). 
+000008f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00000900: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
+00000910: 6372 6565 6e2e 6d6f 7665 2873 656c 662e  creen.move(self.
+00000920: 5f79 2c20 7365 6c66 2e5f 706f 7329 0a0a  _y, self._pos)..
+00000930: 2020 2020 6465 6620 6d6f 7665 5f63 7572      def move_cur
+00000940: 736f 7228 7365 6c66 2c20 6e65 7770 6f73  sor(self, newpos
+00000950: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00000960: 5f70 6f73 203d 206e 6577 706f 730a 2020  _pos = newpos.  
+00000970: 2020 2020 2020 7365 6c66 2e64 7261 775f        self.draw_
+00000980: 6375 7273 6f72 2829 0a0a 2020 2020 6465  cursor()..    de
+00000990: 6620 6465 6c65 7465 5f66 726f 6d5f 6375  f delete_from_cu
+000009a0: 7273 6f72 2873 656c 662c 2064 6972 6563  rsor(self, direc
+000009b0: 7469 6f6e 293a 0a20 2020 2020 2020 206f  tion):.        o
+000009c0: 6c64 5f6d 6178 706f 7320 3d20 7365 6c66  ld_maxpos = self
+000009d0: 2e5f 6d61 7870 6f73 0a20 2020 2020 2020  ._maxpos.       
+000009e0: 2069 6620 6469 7265 6374 696f 6e20 3d3d   if direction ==
+000009f0: 2022 6c65 6674 223a 0a20 2020 2020 2020   "left":.       
+00000a00: 2020 2020 2073 656c 662e 7465 7874 203d       self.text =
+00000a10: 2073 656c 662e 7465 7874 5b73 656c 662e   self.text[self.
+00000a20: 5f70 6f73 3a5d 0a20 2020 2020 2020 2020  _pos:].         
+00000a30: 2020 2073 656c 662e 5f70 6f73 203d 2030     self._pos = 0
+00000a40: 0a20 2020 2020 2020 2065 6c69 6620 6469  .        elif di
+00000a50: 7265 6374 696f 6e20 3d3d 2022 7269 6768  rection == "righ
+00000a60: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
+00000a70: 7365 6c66 2e74 6578 7420 3d20 7365 6c66  self.text = self
+00000a80: 2e74 6578 745b 3a73 656c 662e 5f70 6f73  .text[:self._pos
+00000a90: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
+00000aa0: 6c66 2e5f 706f 7320 3d20 7365 6c66 2e5f  lf._pos = self._
+00000ab0: 6d61 7870 6f73 0a20 2020 2020 2020 2023  maxpos.        #
+00000ac0: 2065 7261 7365 2061 6e64 2072 6564 7261   erase and redra
+00000ad0: 7720 7468 6520 6e65 7720 7465 7874 0a20  w the new text. 
+00000ae0: 2020 2020 2020 2073 656c 662e 6465 6c65         self.dele
+00000af0: 7465 5f74 6578 7428 290a 2020 2020 2020  te_text().      
+00000b00: 2020 7365 6c66 2e64 7261 775f 7465 7874    self.draw_text
+00000b10: 2829 0a0a 2020 2020 6465 6620 6669 6e64  ()..    def find
+00000b20: 5f6c 6566 745f 776f 7264 2873 656c 6629  _left_word(self)
+00000b30: 3a0a 2020 2020 2020 2020 6964 7820 3d20  :.        idx = 
+00000b40: 2d31 0a20 2020 2020 2020 2066 6f72 2069  -1.        for i
+00000b50: 2c20 7320 696e 2065 6e75 6d65 7261 7465  , s in enumerate
+00000b60: 2873 656c 662e 7465 7874 5b3a 7365 6c66  (self.text[:self
+00000b70: 2e5f 706f 732d 315d 293a 0a20 2020 2020  ._pos-1]):.     
+00000b80: 2020 2020 2020 2069 6620 7320 3d3d 2022         if s == "
+00000b90: 2022 3a0a 2020 2020 2020 2020 2020 2020   ":.            
+00000ba0: 2020 2020 6964 7820 3d20 6920 2b20 310a      idx = i + 1.
+00000bb0: 2020 2020 2020 2020 6966 2028 6964 7820          if (idx 
+00000bc0: 3e20 3029 2026 2028 6964 7820 3c20 7365  > 0) & (idx < se
+00000bd0: 6c66 2e5f 706f 7329 3a20 2023 2073 6f6d  lf._pos):  # som
+00000be0: 6574 6869 6e67 2068 6173 2062 6565 6e20  ething has been 
+00000bf0: 666f 756e 640a 2020 2020 2020 2020 2020  found.          
+00000c00: 2020 2320 7365 636f 6e64 2063 6f6e 6469    # second condi
+00000c10: 7469 6f6e 2074 6f20 7072 6576 656e 7420  tion to prevent 
+00000c20: 7468 6520 7365 6172 6368 2066 726f 6d20  the search from 
+00000c30: 736c 6963 6520 5b3a 2d31 5d0a 2020 2020  slice [:-1].    
+00000c40: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+00000c50: 6478 0a20 2020 2020 2020 2065 6c73 653a  dx.        else:
+00000c60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00000c70: 7572 6e20 300a 0a20 2020 2064 6566 206d  urn 0..    def m
+00000c80: 6f76 655f 6c65 6674 5f77 6f72 6428 7365  ove_left_word(se
+00000c90: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00000ca0: 662e 5f70 6f73 203d 2073 656c 662e 6669  f._pos = self.fi
+00000cb0: 6e64 5f6c 6566 745f 776f 7264 2829 0a20  nd_left_word(). 
+00000cc0: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
+00000cd0: 5f63 7572 736f 7228 290a 0a20 2020 2064  _cursor()..    d
+00000ce0: 6566 2064 656c 6574 655f 6c65 6674 5f77  ef delete_left_w
+00000cf0: 6f72 6428 7365 6c66 293a 0a20 2020 2020  ord(self):.     
+00000d00: 2020 2067 6f61 6c20 3d20 7365 6c66 2e66     goal = self.f
+00000d10: 696e 645f 6c65 6674 5f77 6f72 6428 290a  ind_left_word().
+00000d20: 2020 2020 2020 2020 7365 6c66 2e64 656c          self.del
+00000d30: 6574 655f 7061 7274 2867 6f61 6c2c 2073  ete_part(goal, s
+00000d40: 656c 662e 5f70 6f73 290a 0a20 2020 2064  elf._pos)..    d
+00000d50: 6566 2066 696e 645f 7269 6768 745f 776f  ef find_right_wo
+00000d60: 7264 2873 656c 6629 3a0a 2020 2020 2020  rd(self):.      
+00000d70: 2020 6964 7820 3d20 7365 6c66 2e74 6578    idx = self.tex
+00000d80: 745b 7365 6c66 2e5f 706f 732b 313a 5d2e  t[self._pos+1:].
+00000d90: 6669 6e64 2822 2022 290a 2020 2020 2020  find(" ").      
+00000da0: 2020 6966 2069 6478 203e 2030 3a20 2023    if idx > 0:  #
+00000db0: 2073 6f6d 6574 6869 6e67 2068 6173 2062   something has b
+00000dc0: 6565 6e20 666f 756e 640a 2020 2020 2020  een found.      
+00000dd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00000de0: 662e 5f70 6f73 202b 2073 656c 662e 7465  f._pos + self.te
+00000df0: 7874 5b73 656c 662e 5f70 6f73 2b31 3a5d  xt[self._pos+1:]
+00000e00: 2e66 696e 6428 2220 2229 202b 2031 0a20  .find(" ") + 1. 
+00000e10: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00000e20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00000e30: 7365 6c66 2e5f 6d61 7870 6f73 0a0a 2020  self._maxpos..  
+00000e40: 2020 6465 6620 6d6f 7665 5f72 6967 6874    def move_right
+00000e50: 5f77 6f72 6428 7365 6c66 293a 0a20 2020  _word(self):.   
+00000e60: 2020 2020 2073 656c 662e 5f70 6f73 203d       self._pos =
+00000e70: 2073 656c 662e 6669 6e64 5f72 6967 6874   self.find_right
+00000e80: 5f77 6f72 6428 290a 2020 2020 2020 2020  _word().        
+00000e90: 7365 6c66 2e64 7261 775f 6375 7273 6f72  self.draw_cursor
+00000ea0: 2829 0a0a 2323 2323 2323 2323 2323 2323  ()..############
+00000eb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00000ed0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000ee0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000ef0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000f00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000f10: 2323 230a 2320 6765 7420 696e 7075 7420  ###.# get input 
-00000f20: 616e 6420 6465 6669 6e69 7469 6f6e 206f  and definition o
-00000f30: 6620 6b65 7962 696e 6469 6e67 730a 2323  f keybindings.##
+00000ee0: 2323 2323 2323 2323 2323 2323 0a23 2067  ############.# g
+00000ef0: 6574 2069 6e70 7574 2061 6e64 2064 6566  et input and def
+00000f00: 696e 6974 696f 6e20 6f66 206b 6579 6269  inition of keybi
+00000f10: 6e64 696e 6773 0a23 2323 2323 2323 2323  ndings.#########
+00000f20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000f30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00000f40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000f70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000f80: 2323 2323 2323 0a0a 2020 2020 6465 6620  ######..    def 
-00000f90: 6765 745f 696e 7075 7428 7365 6c66 293a  get_input(self):
-00000fa0: 0a20 2020 2020 2020 2063 7572 7365 732e  .        curses.
-00000fb0: 6375 7273 5f73 6574 2831 2920 2023 2073  curs_set(1)  # s
-00000fc0: 7461 7274 206f 6620 696e 7075 743a 2072  tart of input: r
-00000fd0: 6564 7261 7720 6375 7273 6f72 0a20 2020  edraw cursor.   
-00000fe0: 2020 2020 206b 6579 203d 2030 2020 2320       key = 0  # 
-00000ff0: 696e 7465 6765 7220 7468 6174 2064 6f65  integer that doe
-00001000: 7320 6e6f 7468 696e 6720 696e 2074 6865  s nothing in the
-00001010: 206c 6f6f 700a 2020 2020 2020 2020 7365   loop.        se
-00001020: 6c66 2e64 7261 775f 7465 7874 2829 0a20  lf.draw_text(). 
-00001030: 2020 2020 2020 2077 6869 6c65 206e 6f74         while not
-00001040: 286b 6579 2069 6e20 5b22 5c6e 222c 2022  (key in ["\n", "
-00001050: 1b22 5d29 3a0a 2020 2020 2020 2020 2020  ."]):.          
-00001060: 2020 6966 206b 6579 2069 6e20 5b22 4b45    if key in ["KE
-00001070: 595f 5245 5349 5a45 225d 3a0a 2020 2020  Y_RESIZE"]:.    
-00001080: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001090: 726e 202d 310a 0a20 2020 2020 2020 2020  rn -1..         
-000010a0: 2020 2065 6c69 6620 6b65 7920 696e 205b     elif key in [
-000010b0: 224b 4559 5f44 4322 2c20 2204 225d 3a0a  "KEY_DC", "."]:.
-000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 7365 6c66 2e64 656c 6574 655f 6368 6172  self.delete_char
-000010e0: 2830 290a 0a20 2020 2020 2020 2020 2020  (0)..           
-000010f0: 2065 6c69 6620 6b65 7920 696e 205b 224b   elif key in ["K
-00001100: 4559 5f49 4322 5d3a 0a20 2020 2020 2020  EY_IC"]:.       
-00001110: 2020 2020 2020 2020 2070 6173 7320 2023           pass  #
-00001120: 2054 4f44 4f0a 0a20 2020 2020 2020 2020   TODO..         
-00001130: 2020 2065 6c69 6620 6b65 7920 696e 205b     elif key in [
-00001140: 224b 4559 5f42 4143 4b53 5041 4345 222c  "KEY_BACKSPACE",
-00001150: 2022 0822 5d3a 0a20 2020 2020 2020 2020   "."]:.         
-00001160: 2020 2020 2020 2073 656c 662e 6465 6c65         self.dele
-00001170: 7465 5f63 6861 7228 2d31 290a 0a20 2020  te_char(-1)..   
-00001180: 2020 2020 2020 2020 2065 6c69 6620 6b65           elif ke
-00001190: 7920 696e 205b 224b 4559 5f48 4f4d 4522  y in ["KEY_HOME"
-000011a0: 2c20 224b 4559 5f44 4f57 4e22 2c20 2201  , "KEY_DOWN", ".
-000011b0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-000011c0: 2020 2020 7365 6c66 2e6d 6f76 655f 6375      self.move_cu
-000011d0: 7273 6f72 2830 290a 0a20 2020 2020 2020  rsor(0)..       
-000011e0: 2020 2020 2065 6c69 6620 6b65 7920 696e       elif key in
-000011f0: 205b 224b 4559 5f45 4e44 222c 2022 4b45   ["KEY_END", "KE
-00001200: 595f 5550 222c 2022 0522 5d3a 0a20 2020  Y_UP", "."]:.   
-00001210: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00001220: 662e 6d6f 7665 5f63 7572 736f 7228 7365  f.move_cursor(se
-00001230: 6c66 2e5f 6d61 7870 6f73 290a 0a20 2020  lf._maxpos)..   
-00001240: 2020 2020 2020 2020 2065 6c69 6620 6b65           elif ke
-00001250: 7920 696e 205b 224b 4559 5f4c 4546 5422  y in ["KEY_LEFT"
-00001260: 2c20 2022 0222 5d3a 0a20 2020 2020 2020  ,  "."]:.       
-00001270: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
-00001280: 7665 5f63 7572 736f 7228 6d61 7828 302c  ve_cursor(max(0,
-00001290: 2073 656c 662e 5f70 6f73 202d 2031 2929   self._pos - 1))
-000012a0: 0a0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-000012b0: 6966 206b 6579 2069 6e20 5b22 4b45 595f  if key in ["KEY_
-000012c0: 5249 4748 5422 2c20 2206 225d 3a0a 2020  RIGHT", "."]:.  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000012e0: 6c66 2e6d 6f76 655f 6375 7273 6f72 286d  lf.move_cursor(m
-000012f0: 696e 2873 656c 662e 5f6d 6178 706f 732c  in(self._maxpos,
-00001300: 2073 656c 662e 5f70 6f73 202b 2031 2929   self._pos + 1))
-00001310: 0a0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00001320: 6966 206b 6579 2069 6e20 5b22 1522 5d3a  if key in ["."]:
-00001330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001340: 2073 656c 662e 6465 6c65 7465 5f66 726f   self.delete_fro
-00001350: 6d5f 6375 7273 6f72 2822 6c65 6674 2229  m_cursor("left")
-00001360: 0a0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00001370: 6966 206b 6579 2069 6e20 5b22 0b22 5d3a  if key in ["."]:
-00001380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001390: 2073 656c 662e 6465 6c65 7465 5f66 726f   self.delete_fro
-000013a0: 6d5f 6375 7273 6f72 2822 7269 6768 7422  m_cursor("right"
-000013b0: 290a 0a20 2020 2020 2020 2020 2020 2065  )..            e
-000013c0: 6c69 6620 6b65 7920 696e 205b 224b 4559  lif key in ["KEY
-000013d0: 5f53 4c45 4654 222c 2022 4b45 595f 434c  _SLEFT", "KEY_CL
-000013e0: 4546 5422 5d3a 0a20 2020 2020 2020 2020  EFT"]:.         
-000013f0: 2020 2020 2020 2073 656c 662e 6d6f 7665         self.move
-00001400: 5f6c 6566 745f 776f 7264 2829 0a0a 2020  _left_word()..  
-00001410: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
-00001420: 6579 2069 6e20 5b22 4b45 595f 5352 4947  ey in ["KEY_SRIG
-00001430: 4854 222c 2022 4b45 595f 4352 4947 4854  HT", "KEY_CRIGHT
-00001440: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00001450: 2020 2020 7365 6c66 2e6d 6f76 655f 7269      self.move_ri
-00001460: 6768 745f 776f 7264 2829 0a0a 2020 2020  ght_word()..    
-00001470: 2020 2020 2020 2020 656c 6966 206b 6579          elif key
-00001480: 2069 6e20 5b22 1722 5d3a 0a20 2020 2020   in ["."]:.     
-00001490: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000014a0: 6465 6c65 7465 5f6c 6566 745f 776f 7264  delete_left_word
-000014b0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-000014c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000014d0: 2020 2020 2020 6966 2074 7970 6528 6b65        if type(ke
-000014e0: 7929 203d 3d20 7374 723a 0a20 2020 2020  y) == str:.     
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001500: 656c 662e 6164 645f 6368 6172 286b 6579  elf.add_char(key
-00001510: 290a 0a20 2020 2020 2020 2020 2020 206b  )..            k
-00001520: 6579 203d 2067 6574 6b65 792e 6765 746b  ey = getkey.getk
-00001530: 6579 2873 656c 662e 5f73 6372 6565 6e29  ey(self._screen)
-00001540: 0a0a 2020 2020 2020 2020 6375 7273 6573  ..        curses
-00001550: 2e63 7572 735f 7365 7428 3029 2020 2320  .curs_set(0)  # 
-00001560: 656e 6420 6f66 2069 6e70 7574 3a20 7265  end of input: re
-00001570: 6d6f 7665 2063 7572 736f 720a 0a20 2020  move cursor..   
-00001580: 2020 2020 2069 6620 6b65 7920 3d3d 2022       if key == "
-00001590: 1b22 3a20 2023 2065 7363 6170 6520 6b65  .":  # escape ke
-000015a0: 793a 2063 616e 6365 6c20 7465 7874 0a20  y: cancel text. 
-000015b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000015c0: 6e20 310a 2020 2020 2020 2020 656c 7365  n 1.        else
-000015d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000015e0: 7475 726e 2030 0a0a 2323 2323 2323 2323  turn 0..########
+00000f50: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00000f60: 0a20 2020 2064 6566 2067 6574 5f69 6e70  .    def get_inp
+00000f70: 7574 2873 656c 6629 3a0a 2020 2020 2020  ut(self):.      
+00000f80: 2020 6375 7273 6573 2e63 7572 735f 7365    curses.curs_se
+00000f90: 7428 3129 2020 2320 7374 6172 7420 6f66  t(1)  # start of
+00000fa0: 2069 6e70 7574 3a20 7265 6472 6177 2063   input: redraw c
+00000fb0: 7572 736f 720a 2020 2020 2020 2020 6b65  ursor.        ke
+00000fc0: 7920 3d20 3020 2023 2069 6e74 6567 6572  y = 0  # integer
+00000fd0: 2074 6861 7420 646f 6573 206e 6f74 6869   that does nothi
+00000fe0: 6e67 2069 6e20 7468 6520 6c6f 6f70 0a20  ng in the loop. 
+00000ff0: 2020 2020 2020 2073 656c 662e 6472 6177         self.draw
+00001000: 5f74 6578 7428 290a 2020 2020 2020 2020  _text().        
+00001010: 7768 696c 6520 6b65 7920 6e6f 7420 696e  while key not in
+00001020: 2028 225c 6e22 2c20 221b 2229 3a0a 2020   ("\n", "."):.  
+00001030: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+00001040: 2069 6e20 5b22 4b45 595f 5245 5349 5a45   in ["KEY_RESIZE
+00001050: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00001060: 2020 2020 7265 7475 726e 202d 310a 0a20      return -1.. 
+00001070: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00001080: 6b65 7920 696e 205b 224b 4559 5f44 4322  key in ["KEY_DC"
+00001090: 2c20 2204 225d 3a0a 2020 2020 2020 2020  , "."]:.        
+000010a0: 2020 2020 2020 2020 7365 6c66 2e64 656c          self.del
+000010b0: 6574 655f 6368 6172 2830 290a 0a20 2020  ete_char(0)..   
+000010c0: 2020 2020 2020 2020 2065 6c69 6620 6b65           elif ke
+000010d0: 7920 696e 205b 224b 4559 5f49 4322 5d3a  y in ["KEY_IC"]:
+000010e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010f0: 2070 6173 7320 2023 2054 4f44 4f0a 0a20   pass  # TODO.. 
+00001100: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00001110: 6b65 7920 696e 205b 224b 4559 5f42 4143  key in ["KEY_BAC
+00001120: 4b53 5041 4345 222c 2022 0822 5d3a 0a20  KSPACE", "."]:. 
+00001130: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001140: 656c 662e 6465 6c65 7465 5f63 6861 7228  elf.delete_char(
+00001150: 2d31 290a 0a20 2020 2020 2020 2020 2020  -1)..           
+00001160: 2065 6c69 6620 6b65 7920 696e 205b 224b   elif key in ["K
+00001170: 4559 5f48 4f4d 4522 2c20 224b 4559 5f44  EY_HOME", "KEY_D
+00001180: 4f57 4e22 2c20 2201 225d 3a0a 2020 2020  OWN", "."]:.    
+00001190: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000011a0: 2e6d 6f76 655f 6375 7273 6f72 2830 290a  .move_cursor(0).
+000011b0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000011c0: 6620 6b65 7920 696e 205b 224b 4559 5f45  f key in ["KEY_E
+000011d0: 4e44 222c 2022 4b45 595f 5550 222c 2022  ND", "KEY_UP", "
+000011e0: 0522 5d3a 0a20 2020 2020 2020 2020 2020  ."]:.           
+000011f0: 2020 2020 2073 656c 662e 6d6f 7665 5f63       self.move_c
+00001200: 7572 736f 7228 7365 6c66 2e5f 6d61 7870  ursor(self._maxp
+00001210: 6f73 290a 0a20 2020 2020 2020 2020 2020  os)..           
+00001220: 2065 6c69 6620 6b65 7920 696e 205b 224b   elif key in ["K
+00001230: 4559 5f4c 4546 5422 2c20 2022 0222 5d3a  EY_LEFT",  "."]:
+00001240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001250: 2073 656c 662e 6d6f 7665 5f63 7572 736f   self.move_curso
+00001260: 7228 6d61 7828 302c 2073 656c 662e 5f70  r(max(0, self._p
+00001270: 6f73 202d 2031 2929 0a0a 2020 2020 2020  os - 1))..      
+00001280: 2020 2020 2020 656c 6966 206b 6579 2069        elif key i
+00001290: 6e20 5b22 4b45 595f 5249 4748 5422 2c20  n ["KEY_RIGHT", 
+000012a0: 2206 225d 3a0a 2020 2020 2020 2020 2020  "."]:.          
+000012b0: 2020 2020 2020 7365 6c66 2e6d 6f76 655f        self.move_
+000012c0: 6375 7273 6f72 286d 696e 2873 656c 662e  cursor(min(self.
+000012d0: 5f6d 6178 706f 732c 2073 656c 662e 5f70  _maxpos, self._p
+000012e0: 6f73 202b 2031 2929 0a0a 2020 2020 2020  os + 1))..      
+000012f0: 2020 2020 2020 656c 6966 206b 6579 2069        elif key i
+00001300: 6e20 5b22 1522 5d3a 0a20 2020 2020 2020  n ["."]:.       
+00001310: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00001320: 6c65 7465 5f66 726f 6d5f 6375 7273 6f72  lete_from_cursor
+00001330: 2822 6c65 6674 2229 0a0a 2020 2020 2020  ("left")..      
+00001340: 2020 2020 2020 656c 6966 206b 6579 2069        elif key i
+00001350: 6e20 5b22 0b22 5d3a 0a20 2020 2020 2020  n ["."]:.       
+00001360: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00001370: 6c65 7465 5f66 726f 6d5f 6375 7273 6f72  lete_from_cursor
+00001380: 2822 7269 6768 7422 290a 0a20 2020 2020  ("right")..     
+00001390: 2020 2020 2020 2065 6c69 6620 6b65 7920         elif key 
+000013a0: 696e 205b 224b 4559 5f53 4c45 4654 222c  in ["KEY_SLEFT",
+000013b0: 2022 4b45 595f 434c 4546 5422 5d3a 0a20   "KEY_CLEFT"]:. 
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000013d0: 656c 662e 6d6f 7665 5f6c 6566 745f 776f  elf.move_left_wo
+000013e0: 7264 2829 0a0a 2020 2020 2020 2020 2020  rd()..          
+000013f0: 2020 656c 6966 206b 6579 2069 6e20 5b22    elif key in ["
+00001400: 4b45 595f 5352 4947 4854 222c 2022 4b45  KEY_SRIGHT", "KE
+00001410: 595f 4352 4947 4854 225d 3a0a 2020 2020  Y_CRIGHT"]:.    
+00001420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001430: 2e6d 6f76 655f 7269 6768 745f 776f 7264  .move_right_word
+00001440: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00001450: 656c 6966 206b 6579 2069 6e20 5b22 1722  elif key in ["."
+00001460: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00001470: 2020 2073 656c 662e 6465 6c65 7465 5f6c     self.delete_l
+00001480: 6566 745f 776f 7264 2829 0a0a 2020 2020  eft_word()..    
+00001490: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000014a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000014b0: 2074 7970 6528 6b65 7929 203d 3d20 7374   type(key) == st
+000014c0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+000014d0: 2020 2020 2020 2073 656c 662e 6164 645f         self.add_
+000014e0: 6368 6172 286b 6579 290a 0a20 2020 2020  char(key)..     
+000014f0: 2020 2020 2020 206b 6579 203d 2067 6574         key = get
+00001500: 6b65 792e 6765 746b 6579 2873 656c 662e  key.getkey(self.
+00001510: 5f73 6372 6565 6e29 0a0a 2020 2020 2020  _screen)..      
+00001520: 2020 6375 7273 6573 2e63 7572 735f 7365    curses.curs_se
+00001530: 7428 3029 2020 2320 656e 6420 6f66 2069  t(0)  # end of i
+00001540: 6e70 7574 3a20 7265 6d6f 7665 2063 7572  nput: remove cur
+00001550: 736f 720a 0a20 2020 2020 2020 2069 6620  sor..        if 
+00001560: 6b65 7920 3d3d 2022 1b22 3a20 2023 2065  key == ".":  # e
+00001570: 7363 6170 6520 6b65 793a 2063 616e 6365  scape key: cance
+00001580: 6c20 7465 7874 0a20 2020 2020 2020 2020  l text.         
+00001590: 2020 2072 6574 7572 6e20 310a 2020 2020     return 1.    
+000015a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000015b0: 2020 2020 2020 7265 7475 726e 2030 0a0a        return 0..
+000015c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000015d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000015e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000015f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001600: 2323 2323 2323 2323 0a23 2043 6865 636b  ########.# Check
+00001610: 2069 6e70 7574 2076 616c 6964 6974 790a   input validity.
 00001620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001630: 0a23 2043 6865 636b 2069 6e70 7574 2076  .# Check input v
-00001640: 616c 6964 6974 790a 2323 2323 2323 2323  alidity.########
+00001630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00001640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00001650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001670: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001690: 0a20 2020 2064 6566 2065 7272 6f72 2873  .    def error(s
-000016a0: 656c 662c 2065 7272 6d73 6729 3a0a 2020  elf, errmsg):.  
-000016b0: 2020 2020 2020 7365 6c66 2e5f 7363 7265        self._scre
-000016c0: 656e 2e68 6c69 6e65 2873 656c 662e 5f79  en.hline(self._y
-000016d0: 6d61 782d 322c 2030 2c20 2220 222c 2073  max-2, 0, " ", s
-000016e0: 656c 662e 5f78 6d61 7829 0a20 2020 2020  elf._xmax).     
-000016f0: 2020 2073 656c 662e 5f73 6372 6565 6e2e     self._screen.
-00001700: 686c 696e 6528 7365 6c66 2e5f 796d 6178  hline(self._ymax
-00001710: 2d31 2c20 302c 2022 2022 2c20 7365 6c66  -1, 0, " ", self
-00001720: 2e5f 786d 6178 290a 2020 2020 2020 2020  ._xmax).        
-00001730: 7365 6c66 2e5f 7363 7265 656e 2e61 6464  self._screen.add
-00001740: 7374 7228 7365 6c66 2e5f 796d 6178 2d32  str(self._ymax-2
-00001750: 2c20 302c 2065 7272 6d73 6729 0a20 2020  , 0, errmsg).   
-00001760: 2020 2020 2073 656c 662e 5f73 6372 6565       self._scree
-00001770: 6e2e 6164 6473 7472 2873 656c 662e 5f79  n.addstr(self._y
-00001780: 6d61 782d 312c 2030 2c0a 2020 2020 2020  max-1, 0,.      
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 2020 2020 5f28 2250 7265 7373 205b        _("Press [
-000017b0: 456e 7465 725d 2074 6f20 636f 6e74 696e  Enter] to contin
-000017c0: 7565 2229 290a 2020 2020 2020 2020 6b20  ue")).        k 
-000017d0: 3d20 6765 746b 6579 2e67 6574 6b65 7928  = getkey.getkey(
-000017e0: 7365 6c66 2e5f 7363 7265 656e 290a 2020  self._screen).  
-000017f0: 2020 2020 2020 6966 206b 2069 6e20 5b27        if k in ['
-00001800: 7127 2c20 2751 272c 2027 1b27 5d3a 0a20  q', 'Q', '.']:. 
-00001810: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001820: 6e20 2243 554c 5f43 414e 4345 4c22 0a20  n "CUL_CANCEL". 
-00001830: 2020 2020 2020 2065 6c69 6620 6b20 3d3d         elif k ==
-00001840: 2027 4b45 595f 5245 5349 5a45 273a 0a20   'KEY_RESIZE':. 
-00001850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001860: 6e20 6b0a 2020 2020 2020 2020 656c 7365  n k.        else
-00001870: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00001880: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
-00001890: 6566 2063 6865 636b 5f68 6f75 7228 7365  ef check_hour(se
-000018a0: 6c66 2c20 6461 792c 2073 7461 7274 3d46  lf, day, start=F
-000018b0: 616c 7365 293a 0a20 2020 2020 2020 2074  alse):.        t
-000018c0: 7279 3a20 2023 2074 6f20 6372 6561 7465  ry:  # to create
-000018d0: 2061 2074 696d 650a 2020 2020 2020 2020   a time.        
-000018e0: 2020 2020 6966 2022 3a22 2069 6e20 7365      if ":" in se
-000018f0: 6c66 2e74 6578 743a 0a20 2020 2020 2020  lf.text:.       
-00001900: 2020 2020 2020 2020 2068 203d 2069 6e74           h = int
-00001910: 2873 656c 662e 7465 7874 5b3a 7365 6c66  (self.text[:self
-00001920: 2e74 6578 742e 6669 6e64 2822 3a22 295d  .text.find(":")]
-00001930: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001940: 2020 6d20 3d20 696e 7428 7365 6c66 2e74    m = int(self.t
-00001950: 6578 745b 7365 6c66 2e74 6578 742e 6669  ext[self.text.fi
-00001960: 6e64 2822 3a22 292b 313a 5d29 0a20 2020  nd(":")+1:]).   
-00001970: 2020 2020 2020 2020 2065 6c69 6620 6c65           elif le
-00001980: 6e28 7365 6c66 2e74 6578 7429 203c 2033  n(self.text) < 3
-00001990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000019a0: 2020 6820 3d20 696e 7428 7365 6c66 2e74    h = int(self.t
-000019b0: 6578 7429 0a20 2020 2020 2020 2020 2020  ext).           
-000019c0: 2020 2020 206d 203d 2030 0a20 2020 2020       m = 0.     
-000019d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000019e0: 2020 2020 2020 2020 2020 2020 206d 203d               m =
-000019f0: 2069 6e74 2873 656c 662e 7465 7874 5b2d   int(self.text[-
-00001a00: 323a 5d29 0a20 2020 2020 2020 2020 2020  2:]).           
-00001a10: 2020 2020 2068 203d 2069 6e74 2873 656c       h = int(sel
-00001a20: 662e 7465 7874 5b3a 2d32 5d29 0a20 2020  f.text[:-2]).   
-00001a30: 2020 2020 2020 2020 2069 6620 6820 3d3d           if h ==
-00001a40: 2032 343a 0a20 2020 2020 2020 2020 2020   24:.           
-00001a50: 2020 2020 2069 6620 7374 6172 743a 0a20       if start:. 
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a70: 2020 2068 203d 2032 330a 2020 2020 2020     h = 23.      
-00001a80: 2020 2020 2020 2020 2020 2020 2020 6d20                m 
-00001a90: 3d20 3539 0a20 2020 2020 2020 2020 2020  = 59.           
-00001aa0: 2020 2020 2020 2020 2074 6d70 6461 7920           tmpday 
-00001ab0: 3d20 6461 790a 2020 2020 2020 2020 2020  = day.          
-00001ac0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 6820 3d20 300a 2020 2020 2020 2020 2020  h = 0.          
-00001af0: 2020 2020 2020 2020 2020 2320 6164 6420            # add 
-00001b00: 686f 7572 2061 6e64 206d 696e 7574 6520  hour and minute 
-00001b10: 746f 2064 6179 2062 7920 7573 696e 6720  to day by using 
-00001b20: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-00001b30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00001b40: 2020 2020 2020 746d 7064 6179 203d 2064        tmpday = d
-00001b50: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
-00001b60: 2e66 726f 6d6f 7264 696e 616c 2864 6179  .fromordinal(day
-00001b70: 2e74 6f6f 7264 696e 616c 2829 2b31 290a  .toordinal()+1).
-00001b80: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00001b90: 3a20 2023 2069 6465 6d0a 2020 2020 2020  :  # idem.      
-00001ba0: 2020 2020 2020 2020 2020 746d 7064 6179            tmpday
-00001bb0: 203d 2064 6174 6574 696d 652e 6461 7465   = datetime.date
-00001bc0: 7469 6d65 2e66 726f 6d6f 7264 696e 616c  time.fromordinal
-00001bd0: 2864 6179 2e74 6f6f 7264 696e 616c 2829  (day.toordinal()
-00001be0: 290a 2020 2020 2020 2020 2020 2020 6420  ).            d 
-00001bf0: 3d20 746d 7064 6179 2e72 6570 6c61 6365  = tmpday.replace
-00001c00: 2868 6f75 723d 682c 206d 696e 7574 653d  (hour=h, minute=
-00001c10: 6d29 0a20 2020 2020 2020 2020 2020 2072  m).            r
-00001c20: 6574 7572 6e20 640a 2020 2020 2020 2020  eturn d.        
-00001c30: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00001c40: 2020 2020 6572 726d 7367 203d 205f 2822      errmsg = _("
-00001c50: 596f 7520 656e 7465 7265 6420 616e 2069  You entered an i
-00001c60: 6e76 616c 6964 2074 696d 6522 290a 2020  nvalid time").  
-00001c70: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001c80: 2073 656c 662e 6572 726f 7228 6572 726d   self.error(errm
-00001c90: 7367 290a 0a20 2020 2064 6566 2063 6865  sg)..    def che
-00001ca0: 636b 5f64 7572 6174 696f 6e28 7365 6c66  ck_duration(self
-00001cb0: 2c20 6461 792c 2073 7461 7274 5f64 6174  , day, start_dat
-00001cc0: 6529 3a0a 2020 2020 2020 2020 6966 2022  e):.        if "
-00001cd0: 2b22 2069 6e20 7365 6c66 2e74 6578 743a  +" in self.text:
-00001ce0: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
-00001cf0: 5f64 6174 6520 3d20 7365 6c66 2e63 6865  _date = self.che
-00001d00: 636b 5f61 6464 5f74 696d 6528 7374 6172  ck_add_time(star
-00001d10: 745f 6461 7465 290a 2020 2020 2020 2020  t_date).        
-00001d20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00001d30: 2020 656e 645f 6461 7465 203d 2073 656c    end_date = sel
-00001d40: 662e 6368 6563 6b5f 686f 7572 2864 6179  f.check_hour(day
-00001d50: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-00001d60: 2865 6e64 5f64 6174 6520 696e 205b 4e6f  (end_date in [No
-00001d70: 6e65 2c20 2243 554c 5f43 414e 4345 4c22  ne, "CUL_CANCEL"
-00001d80: 2c20 224b 4559 5f52 4553 495a 4522 5d29  , "KEY_RESIZE"])
-00001d90: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00001da0: 2065 6e64 5f64 6174 6520 3c20 7374 6172   end_date < star
-00001db0: 745f 6461 7465 3a0a 2020 2020 2020 2020  t_date:.        
-00001dc0: 2020 2020 2020 2020 7374 203d 2028 7374          st = (st
-00001dd0: 7228 7374 6172 745f 6461 7465 2e68 6f75  r(start_date.hou
-00001de0: 7229 202b 2022 3a22 0a20 2020 2020 2020  r) + ":".       
-00001df0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00001e00: 2028 2230 222b 7374 7228 7374 6172 745f   ("0"+str(start_
-00001e10: 6461 7465 2e6d 696e 7574 6529 295b 2d32  date.minute))[-2
-00001e20: 3a5d 290a 2020 2020 2020 2020 2020 2020  :]).            
-00001e30: 2020 2020 6572 726d 7367 203d 205f 2822      errmsg = _("
-00001e40: 456e 6469 6e67 2074 696d 6520 7368 6f75  Ending time shou
-00001e50: 6c64 2062 6520 6772 6561 7465 7220 7468  ld be greater th
-00001e60: 616e 2022 292b 7374 0a20 2020 2020 2020  an ")+st.       
-00001e70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001e80: 7365 6c66 2e65 7272 6f72 2865 7272 6d73  self.error(errms
-00001e90: 6729 0a20 2020 2020 2020 2072 6574 7572  g).        retur
-00001ea0: 6e20 656e 645f 6461 7465 0a0a 2020 2020  n end_date..    
-00001eb0: 6465 6620 6368 6563 6b5f 6164 645f 7469  def check_add_ti
-00001ec0: 6d65 2873 656c 662c 2073 7461 7274 5f64  me(self, start_d
-00001ed0: 6174 6529 3a0a 2020 2020 2020 2020 7472  ate):.        tr
-00001ee0: 793a 0a20 2020 2020 2020 2020 2020 2064  y:.            d
-00001ef0: 7572 6174 696f 6e20 3d20 696e 7428 7365  uration = int(se
-00001f00: 6c66 2e74 6578 745b 313a 5d29 2a36 3020  lf.text[1:])*60 
-00001f10: 2023 2069 6e20 7365 636f 6e64 730a 2020   # in seconds.  
-00001f20: 2020 2020 2020 2020 2020 656e 645f 6461            end_da
-00001f30: 7465 203d 2073 7461 7274 5f64 6174 6520  te = start_date 
-00001f40: 2b20 6461 7465 7469 6d65 2e74 696d 6564  + datetime.timed
-00001f50: 656c 7461 2873 6563 6f6e 6473 3d64 7572  elta(seconds=dur
-00001f60: 6174 696f 6e29 0a20 2020 2020 2020 2020  ation).         
-00001f70: 2020 2072 6574 7572 6e20 656e 645f 6461     return end_da
-00001f80: 7465 0a20 2020 2020 2020 2065 7863 6570  te.        excep
-00001f90: 743a 0a20 2020 2020 2020 2020 2020 2065  t:.            e
-00001fa0: 7272 6d73 6720 3d20 5f28 2259 6f75 2065  rrmsg = _("You e
-00001fb0: 6e74 6572 6564 2061 6e20 696e 7661 6c69  ntered an invali
-00001fc0: 6420 6475 7261 7469 6f6e 2229 0a20 2020  d duration").   
-00001fd0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001fe0: 7365 6c66 2e65 7272 6f72 2865 7272 6d73  self.error(errms
-00001ff0: 6729 0a0a 2020 2020 6465 6620 6368 6563  g)..    def chec
-00002000: 6b5f 6461 7928 7365 6c66 2c20 6461 7929  k_day(self, day)
-00002010: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00002020: 2873 656c 662e 7465 7874 293a 2020 2320  (self.text):  # 
-00002030: 656d 7074 7920 6461 793a 2073 6574 2074  empty day: set t
-00002040: 6f20 746f 6461 790a 2020 2020 2020 2020  o today.        
-00002050: 2020 2020 7265 7475 726e 2064 6174 6574      return datet
-00002060: 696d 652e 6461 7465 2e74 6f64 6179 2829  ime.date.today()
-00002070: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00002080: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020a0: 6966 2027 2f27 2069 6e20 7365 6c66 2e74  if '/' in self.t
-000020b0: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-000020c0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-000020d0: 7365 6c66 2e74 6578 7429 203e 2035 3a0a  self.text) > 5:.
-000020e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020f0: 2020 2020 2020 2020 7920 3d20 696e 7428          y = int(
-00002100: 7365 6c66 2e74 6578 745b 303a 345d 290a  self.text[0:4]).
-00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 2020 2020 2020 6465 6320 3d20 350a          dec = 5.
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00002150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002160: 2020 7920 3d20 6461 792e 7965 6172 0a20    y = day.year. 
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 2020 2020 2064 6563 203d 2030 0a20         dec = 0. 
-00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021a0: 2020 206d 203d 2069 6e74 2873 656c 662e     m = int(self.
-000021b0: 7465 7874 5b64 6563 3a64 6563 2b32 5d29  text[dec:dec+2])
-000021c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021d0: 2020 2020 2064 203d 2069 6e74 2873 656c       d = int(sel
-000021e0: 662e 7465 7874 5b64 6563 2b33 3a5d 290a  f.text[dec+3:]).
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00002210: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00002220: 2873 656c 662e 7465 7874 2920 3e20 343a  (self.text) > 4:
-00002230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002240: 2020 2020 2020 2020 2079 203d 2069 6e74           y = int
-00002250: 2873 656c 662e 7465 7874 5b30 3a34 5d29  (self.text[0:4])
-00002260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002270: 2020 2020 2020 2020 2064 6563 203d 2034           dec = 4
-00002280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002290: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 2020 2079 203d 2064 6179 2e79 6561 720a     y = day.year.
-000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2020 2020 2020 2020 6465 6320 3d20 300a          dec = 0.
-000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022f0: 2020 2020 6d20 3d20 696e 7428 7365 6c66      m = int(self
-00002300: 2e74 6578 745b 6465 633a 6465 632b 325d  .text[dec:dec+2]
-00002310: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002320: 2020 2020 2020 6420 3d20 696e 7428 7365        d = int(se
-00002330: 6c66 2e74 6578 745b 6465 632b 323a 5d29  lf.text[dec+2:])
-00002340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002350: 2072 6574 7572 6e20 6461 7465 7469 6d65   return datetime
-00002360: 2e64 6174 6528 792c 206d 2c20 6429 0a20  .date(y, m, d). 
-00002370: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00002380: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-00002390: 2020 2065 7272 6d73 6720 3d20 5f28 2245     errmsg = _("E
-000023a0: 7272 6f72 3a20 636f 756c 6420 6e6f 7420  rror: could not 
-000023b0: 756e 6465 7273 7461 6e64 2064 6174 6522  understand date"
-000023c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000023d0: 2020 7265 7475 726e 2073 656c 662e 6572    return self.er
-000023e0: 726f 7228 6572 726d 7367 290a 0a20 2020  ror(errmsg)..   
-000023f0: 2064 6566 2063 6865 636b 5f66 696c 656e   def check_filen
-00002400: 616d 6528 7365 6c66 2c20 6d6f 6465 293a  ame(self, mode):
-00002410: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00002420: 2020 2020 2020 2020 2020 6966 2028 2873            if ((s
-00002430: 656c 662e 7465 7874 5b2d 325d 203d 3d20  elf.text[-2] == 
-00002440: 2220 2229 0a20 2020 2020 2020 2020 2020  " ").           
-00002450: 2020 2020 616e 6420 2873 656c 662e 7465      and (self.te
-00002460: 7874 5b2d 315d 2069 6e20 5b73 7472 2869  xt[-1] in [str(i
-00002470: 2920 666f 7220 6920 696e 2072 616e 6765  ) for i in range
-00002480: 2838 295d 2929 3a0a 2020 2020 2020 2020  (8)])):.        
-00002490: 2020 2020 2020 2020 2320 7370 6563 6961          # specia
-000024a0: 6c20 6361 7365 3a20 6869 6464 656e 2066  l case: hidden f
-000024b0: 696e 616c 2074 6167 0a20 2020 2020 2020  inal tag.       
-000024c0: 2020 2020 2020 2020 2066 203d 206f 7065           f = ope
-000024d0: 6e28 7365 6c66 2e74 6578 745b 3a2d 325d  n(self.text[:-2]
-000024e0: 2c20 6d6f 6465 290a 2020 2020 2020 2020  , mode).        
-000024f0: 2020 2020 2020 2020 662e 636c 6f73 6528          f.close(
-00002500: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00002510: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00002520: 2020 2020 6620 3d20 6f70 656e 2873 656c      f = open(sel
-00002530: 662e 7465 7874 2c20 6d6f 6465 290a 2020  f.text, mode).  
-00002540: 2020 2020 2020 2020 2020 2020 2020 662e                f.
-00002550: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-00002560: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002570: 7465 7874 0a20 2020 2020 2020 2065 7863  text.        exc
-00002580: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-00002590: 2069 6620 6d6f 6465 203d 3d20 2272 6222   if mode == "rb"
-000025a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000025b0: 2020 6572 726d 7367 203d 205f 2822 4572    errmsg = _("Er
-000025c0: 726f 723a 2075 6e61 626c 6520 746f 2072  ror: unable to r
-000025d0: 6561 6420 7468 6520 6669 6c65 2022 290a  ead the file ").
-000025e0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000025f0: 206d 6f64 6520 3d3d 2022 7762 223a 0a20   mode == "wb":. 
-00002600: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002610: 7272 6d73 6720 3d20 5f28 2245 7272 6f72  rrmsg = _("Error
-00002620: 3a20 756e 6162 6c65 2074 6f20 7772 6974  : unable to writ
-00002630: 6520 7468 6520 6669 6c65 2022 290a 2020  e the file ").  
-00002640: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002650: 2073 656c 662e 6572 726f 7228 6572 726d   self.error(errm
-00002660: 7367 202b 2073 656c 662e 7465 7874 290a  sg + self.text).
-00002670: 0a20 2020 2064 6566 2063 6865 636b 5f69  .    def check_i
-00002680: 6e74 686f 7572 2873 656c 6629 3a0a 2020  nthour(self):.  
-00002690: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000026a0: 2020 2020 2020 2069 6620 696e 7428 7365         if int(se
-000026b0: 6c66 2e74 6578 7429 203c 2030 3a0a 2020  lf.text) < 0:.  
-000026c0: 2020 2020 2020 2020 2020 2020 2020 6572                er
-000026d0: 726d 7367 203d 205f 2822 4572 726f 723a  rmsg = _("Error:
-000026e0: 2073 686f 756c 6420 6265 2068 6967 6865   should be highe
-000026f0: 7220 7468 616e 2030 2229 0a20 2020 2020  r than 0").     
-00002700: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00002710: 6e20 7365 6c66 2e65 7272 6f72 2865 7272  n self.error(err
-00002720: 6d73 6729 0a20 2020 2020 2020 2020 2020  msg).           
-00002730: 2069 6620 696e 7428 7365 6c66 2e74 6578   if int(self.tex
-00002740: 7429 203e 2032 343a 0a20 2020 2020 2020  t) > 24:.       
-00002750: 2020 2020 2020 2020 2065 7272 6d73 6720           errmsg 
-00002760: 3d20 5f28 2245 7272 6f72 3a20 7368 6f75  = _("Error: shou
-00002770: 6c64 2062 6520 6c6f 7765 7220 7468 616e  ld be lower than
-00002780: 2032 3422 290a 2020 2020 2020 2020 2020   24").          
-00002790: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000027a0: 662e 6572 726f 7228 6572 726d 7367 290a  f.error(errmsg).
-000027b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000027c0: 726e 2069 6e74 2873 656c 662e 7465 7874  rn int(self.text
-000027d0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-000027e0: 3a0a 2020 2020 2020 2020 2020 2020 6572  :.            er
-000027f0: 726d 7367 203d 205f 2822 4572 726f 723a  rmsg = _("Error:
-00002800: 206d 7573 7420 6265 2061 6e20 696e 7465   must be an inte
-00002810: 6765 7222 290a 2020 2020 2020 2020 2020  ger").          
-00002820: 2020 7265 7475 726e 2073 656c 662e 6572    return self.er
-00002830: 726f 7228 6572 726d 7367 290a            ror(errmsg).
+00001660: 2323 2323 2323 2323 0a20 2020 2064 6566  ########.    def
+00001670: 2065 7272 6f72 2873 656c 662c 2065 7272   error(self, err
+00001680: 6d73 6729 3a0a 2020 2020 2020 2020 7365  msg):.        se
+00001690: 6c66 2e5f 7363 7265 656e 2e68 6c69 6e65  lf._screen.hline
+000016a0: 2873 656c 662e 5f79 6d61 782d 322c 2030  (self._ymax-2, 0
+000016b0: 2c20 2220 222c 2073 656c 662e 5f78 6d61  , " ", self._xma
+000016c0: 7829 0a20 2020 2020 2020 2073 656c 662e  x).        self.
+000016d0: 5f73 6372 6565 6e2e 686c 696e 6528 7365  _screen.hline(se
+000016e0: 6c66 2e5f 796d 6178 2d31 2c20 302c 2022  lf._ymax-1, 0, "
+000016f0: 2022 2c20 7365 6c66 2e5f 786d 6178 290a   ", self._xmax).
+00001700: 2020 2020 2020 2020 7365 6c66 2e5f 7363          self._sc
+00001710: 7265 656e 2e61 6464 7374 7228 7365 6c66  reen.addstr(self
+00001720: 2e5f 796d 6178 2d32 2c20 302c 2065 7272  ._ymax-2, 0, err
+00001730: 6d73 6729 0a20 2020 2020 2020 2073 656c  msg).        sel
+00001740: 662e 5f73 6372 6565 6e2e 6164 6473 7472  f._screen.addstr
+00001750: 2873 656c 662e 5f79 6d61 782d 312c 2030  (self._ymax-1, 0
+00001760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001770: 2020 2020 2020 2020 2020 2020 2020 5f28                _(
+00001780: 2250 7265 7373 205b 456e 7465 725d 2074  "Press [Enter] t
+00001790: 6f20 636f 6e74 696e 7565 2229 290a 2020  o continue")).  
+000017a0: 2020 2020 2020 6b20 3d20 6765 746b 6579        k = getkey
+000017b0: 2e67 6574 6b65 7928 7365 6c66 2e5f 7363  .getkey(self._sc
+000017c0: 7265 656e 290a 2020 2020 2020 2020 6966  reen).        if
+000017d0: 206b 2069 6e20 5b27 7127 2c20 2751 272c   k in ['q', 'Q',
+000017e0: 2027 1b27 5d3a 0a20 2020 2020 2020 2020   '.']:.         
+000017f0: 2020 2072 6574 7572 6e20 2243 554c 5f43     return "CUL_C
+00001800: 414e 4345 4c22 0a20 2020 2020 2020 2065  ANCEL".        e
+00001810: 6c69 6620 6b20 3d3d 2027 4b45 595f 5245  lif k == 'KEY_RE
+00001820: 5349 5a45 273a 0a20 2020 2020 2020 2020  SIZE':.         
+00001830: 2020 2072 6574 7572 6e20 6b0a 2020 2020     return k.    
+00001840: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001850: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00001860: 650a 0a20 2020 2064 6566 2063 6865 636b  e..    def check
+00001870: 5f68 6f75 7228 7365 6c66 2c20 6461 792c  _hour(self, day,
+00001880: 2073 7461 7274 3d46 616c 7365 293a 0a20   start=False):. 
+00001890: 2020 2020 2020 2074 7279 3a20 2023 2074         try:  # t
+000018a0: 6f20 6372 6561 7465 2061 2074 696d 650a  o create a time.
+000018b0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+000018c0: 3a22 2069 6e20 7365 6c66 2e74 6578 743a  :" in self.text:
+000018d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018e0: 2068 203d 2069 6e74 2873 656c 662e 7465   h = int(self.te
+000018f0: 7874 5b3a 7365 6c66 2e74 6578 742e 6669  xt[:self.text.fi
+00001900: 6e64 2822 3a22 295d 290a 2020 2020 2020  nd(":")]).      
+00001910: 2020 2020 2020 2020 2020 6d20 3d20 696e            m = in
+00001920: 7428 7365 6c66 2e74 6578 745b 7365 6c66  t(self.text[self
+00001930: 2e74 6578 742e 6669 6e64 2822 3a22 292b  .text.find(":")+
+00001940: 313a 5d29 0a20 2020 2020 2020 2020 2020  1:]).           
+00001950: 2065 6c69 6620 6c65 6e28 7365 6c66 2e74   elif len(self.t
+00001960: 6578 7429 203c 2033 3a0a 2020 2020 2020  ext) < 3:.      
+00001970: 2020 2020 2020 2020 2020 6820 3d20 696e            h = in
+00001980: 7428 7365 6c66 2e74 6578 7429 0a20 2020  t(self.text).   
+00001990: 2020 2020 2020 2020 2020 2020 206d 203d               m =
+000019a0: 2030 0a20 2020 2020 2020 2020 2020 2065   0.            e
+000019b0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000019c0: 2020 2020 206d 203d 2069 6e74 2873 656c       m = int(sel
+000019d0: 662e 7465 7874 5b2d 323a 5d29 0a20 2020  f.text[-2:]).   
+000019e0: 2020 2020 2020 2020 2020 2020 2068 203d               h =
+000019f0: 2069 6e74 2873 656c 662e 7465 7874 5b3a   int(self.text[:
+00001a00: 2d32 5d29 0a20 2020 2020 2020 2020 2020  -2]).           
+00001a10: 2069 6620 6820 3d3d 2032 343a 0a20 2020   if h == 24:.   
+00001a20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00001a30: 7374 6172 743a 0a20 2020 2020 2020 2020  start:.         
+00001a40: 2020 2020 2020 2020 2020 2068 203d 2032             h = 2
+00001a50: 330a 2020 2020 2020 2020 2020 2020 2020  3.              
+00001a60: 2020 2020 2020 6d20 3d20 3539 0a20 2020        m = 59.   
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2074 6d70 6461 7920 3d20 6461 790a 2020   tmpday = day.  
+00001a90: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00001aa0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00001ab0: 2020 2020 2020 2020 6820 3d20 300a 2020          h = 0.  
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2320 6164 6420 686f 7572 2061 6e64    # add hour and
+00001ae0: 206d 696e 7574 6520 746f 2064 6179 2062   minute to day b
+00001af0: 7920 7573 696e 6720 6461 7465 7469 6d65  y using datetime
+00001b00: 2e64 6174 6574 696d 650a 2020 2020 2020  .datetime.      
+00001b10: 2020 2020 2020 2020 2020 2020 2020 746d                tm
+00001b20: 7064 6179 203d 2064 6174 6574 696d 652e  pday = datetime.
+00001b30: 6461 7465 7469 6d65 2e66 726f 6d6f 7264  datetime.fromord
+00001b40: 696e 616c 2864 6179 2e74 6f6f 7264 696e  inal(day.toordin
+00001b50: 616c 2829 2b31 290a 2020 2020 2020 2020  al()+1).        
+00001b60: 2020 2020 656c 7365 3a20 2023 2069 6465      else:  # ide
+00001b70: 6d0a 2020 2020 2020 2020 2020 2020 2020  m.              
+00001b80: 2020 746d 7064 6179 203d 2064 6174 6574    tmpday = datet
+00001b90: 696d 652e 6461 7465 7469 6d65 2e66 726f  ime.datetime.fro
+00001ba0: 6d6f 7264 696e 616c 2864 6179 2e74 6f6f  mordinal(day.too
+00001bb0: 7264 696e 616c 2829 290a 2020 2020 2020  rdinal()).      
+00001bc0: 2020 2020 2020 6420 3d20 746d 7064 6179        d = tmpday
+00001bd0: 2e72 6570 6c61 6365 2868 6f75 723d 682c  .replace(hour=h,
+00001be0: 206d 696e 7574 653d 6d29 0a20 2020 2020   minute=m).     
+00001bf0: 2020 2020 2020 2072 6574 7572 6e20 640a         return d.
+00001c00: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+00001c10: 2020 2020 2020 2020 2020 2020 6572 726d              errm
+00001c20: 7367 203d 205f 2822 596f 7520 656e 7465  sg = _("You ente
+00001c30: 7265 6420 616e 2069 6e76 616c 6964 2074  red an invalid t
+00001c40: 696d 6522 290a 2020 2020 2020 2020 2020  ime").          
+00001c50: 2020 7265 7475 726e 2073 656c 662e 6572    return self.er
+00001c60: 726f 7228 6572 726d 7367 290a 0a20 2020  ror(errmsg)..   
+00001c70: 2064 6566 2063 6865 636b 5f64 7572 6174   def check_durat
+00001c80: 696f 6e28 7365 6c66 2c20 6461 792c 2073  ion(self, day, s
+00001c90: 7461 7274 5f64 6174 6529 3a0a 2020 2020  tart_date):.    
+00001ca0: 2020 2020 6966 2022 2b22 2069 6e20 7365      if "+" in se
+00001cb0: 6c66 2e74 6578 743a 0a20 2020 2020 2020  lf.text:.       
+00001cc0: 2020 2020 2065 6e64 5f64 6174 6520 3d20       end_date = 
+00001cd0: 7365 6c66 2e63 6865 636b 5f61 6464 5f74  self.check_add_t
+00001ce0: 696d 6528 7374 6172 745f 6461 7465 290a  ime(start_date).
+00001cf0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00001d00: 2020 2020 2020 2020 2020 656e 645f 6461            end_da
+00001d10: 7465 203d 2073 656c 662e 6368 6563 6b5f  te = self.check_
+00001d20: 686f 7572 2864 6179 290a 2020 2020 2020  hour(day).      
+00001d30: 2020 6966 2065 6e64 5f64 6174 6520 6e6f    if end_date no
+00001d40: 7420 696e 2028 4e6f 6e65 2c20 2243 554c  t in (None, "CUL
+00001d50: 5f43 414e 4345 4c22 2c20 224b 4559 5f52  _CANCEL", "KEY_R
+00001d60: 4553 495a 4522 293a 0a20 2020 2020 2020  ESIZE"):.       
+00001d70: 2020 2020 2069 6620 656e 645f 6461 7465       if end_date
+00001d80: 203c 2073 7461 7274 5f64 6174 653a 0a20   < start_date:. 
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001da0: 7420 3d20 2873 7472 2873 7461 7274 5f64  t = (str(start_d
+00001db0: 6174 652e 686f 7572 2920 2b20 223a 220a  ate.hour) + ":".
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 2020 2020 2020 2b20 2822 3022 2b73 7472        + ("0"+str
+00001de0: 2873 7461 7274 5f64 6174 652e 6d69 6e75  (start_date.minu
+00001df0: 7465 2929 5b2d 323a 5d29 0a20 2020 2020  te))[-2:]).     
+00001e00: 2020 2020 2020 2020 2020 2065 7272 6d73             errms
+00001e10: 6720 3d20 5f28 2245 6e64 696e 6720 7469  g = _("Ending ti
+00001e20: 6d65 2073 686f 756c 6420 6265 2067 7265  me should be gre
+00001e30: 6174 6572 2074 6861 6e20 2229 2b73 740a  ater than ")+st.
+00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e50: 7265 7475 726e 2073 656c 662e 6572 726f  return self.erro
+00001e60: 7228 6572 726d 7367 290a 2020 2020 2020  r(errmsg).      
+00001e70: 2020 7265 7475 726e 2065 6e64 5f64 6174    return end_dat
+00001e80: 650a 0a20 2020 2064 6566 2063 6865 636b  e..    def check
+00001e90: 5f61 6464 5f74 696d 6528 7365 6c66 2c20  _add_time(self, 
+00001ea0: 7374 6172 745f 6461 7465 293a 0a20 2020  start_date):.   
+00001eb0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00001ec0: 2020 2020 2020 6475 7261 7469 6f6e 203d        duration =
+00001ed0: 2069 6e74 2873 656c 662e 7465 7874 5b31   int(self.text[1
+00001ee0: 3a5d 292a 3630 2020 2320 696e 2073 6563  :])*60  # in sec
+00001ef0: 6f6e 6473 0a20 2020 2020 2020 2020 2020  onds.           
+00001f00: 2065 6e64 5f64 6174 6520 3d20 7374 6172   end_date = star
+00001f10: 745f 6461 7465 202b 2064 6174 6574 696d  t_date + datetim
+00001f20: 652e 7469 6d65 6465 6c74 6128 7365 636f  e.timedelta(seco
+00001f30: 6e64 733d 6475 7261 7469 6f6e 290a 2020  nds=duration).  
+00001f40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00001f50: 2065 6e64 5f64 6174 650a 2020 2020 2020   end_date.      
+00001f60: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+00001f70: 2020 2020 2020 6572 726d 7367 203d 205f        errmsg = _
+00001f80: 2822 596f 7520 656e 7465 7265 6420 616e  ("You entered an
+00001f90: 2069 6e76 616c 6964 2064 7572 6174 696f   invalid duratio
+00001fa0: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00001fb0: 7265 7475 726e 2073 656c 662e 6572 726f  return self.erro
+00001fc0: 7228 6572 726d 7367 290a 0a20 2020 2064  r(errmsg)..    d
+00001fd0: 6566 2063 6865 636b 5f64 6179 2873 656c  ef check_day(sel
+00001fe0: 662c 2064 6179 293a 0a20 2020 2020 2020  f, day):.       
+00001ff0: 2069 6620 6e6f 7420 7365 6c66 2e74 6578   if not self.tex
+00002000: 743a 2020 2320 656d 7074 7920 6461 793a  t:  # empty day:
+00002010: 2073 6574 2074 6f20 746f 6461 790a 2020   set to today.  
+00002020: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002030: 2064 6174 6574 696d 652e 6461 7465 2e74   datetime.date.t
+00002040: 6f64 6179 2829 0a20 2020 2020 2020 2065  oday().        e
+00002050: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00002060: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00002070: 2020 2020 2020 6966 2027 2f27 2069 6e20        if '/' in 
+00002080: 7365 6c66 2e74 6578 743a 0a20 2020 2020  self.text:.     
+00002090: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000020a0: 6620 6c65 6e28 7365 6c66 2e74 6578 7429  f len(self.text)
+000020b0: 203e 2035 3a0a 2020 2020 2020 2020 2020   > 5:.          
+000020c0: 2020 2020 2020 2020 2020 2020 2020 7920                y 
+000020d0: 3d20 696e 7428 7365 6c66 2e74 6578 745b  = int(self.text[
+000020e0: 303a 345d 290a 2020 2020 2020 2020 2020  0:4]).          
+000020f0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00002100: 6320 3d20 350a 2020 2020 2020 2020 2020  c = 5.          
+00002110: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002130: 2020 2020 2020 2020 7920 3d20 6461 792e          y = day.
+00002140: 7965 6172 0a20 2020 2020 2020 2020 2020  year.           
+00002150: 2020 2020 2020 2020 2020 2020 2064 6563               dec
+00002160: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
+00002170: 2020 2020 2020 2020 206d 203d 2069 6e74           m = int
+00002180: 2873 656c 662e 7465 7874 5b64 6563 3a64  (self.text[dec:d
+00002190: 6563 2b32 5d29 0a20 2020 2020 2020 2020  ec+2]).         
+000021a0: 2020 2020 2020 2020 2020 2064 203d 2069             d = i
+000021b0: 6e74 2873 656c 662e 7465 7874 5b64 6563  nt(self.text[dec
+000021c0: 2b33 3a5d 290a 2020 2020 2020 2020 2020  +3:]).          
+000021d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021f0: 6966 206c 656e 2873 656c 662e 7465 7874  if len(self.text
+00002200: 2920 3e20 343a 0a20 2020 2020 2020 2020  ) > 4:.         
+00002210: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00002220: 203d 2069 6e74 2873 656c 662e 7465 7874   = int(self.text
+00002230: 5b30 3a34 5d29 0a20 2020 2020 2020 2020  [0:4]).         
+00002240: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00002250: 6563 203d 2034 0a20 2020 2020 2020 2020  ec = 4.         
+00002260: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00002270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002280: 2020 2020 2020 2020 2079 203d 2064 6179           y = day
+00002290: 2e79 6561 720a 2020 2020 2020 2020 2020  .year.          
+000022a0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+000022b0: 6320 3d20 300a 2020 2020 2020 2020 2020  c = 0.          
+000022c0: 2020 2020 2020 2020 2020 6d20 3d20 696e            m = in
+000022d0: 7428 7365 6c66 2e74 6578 745b 6465 633a  t(self.text[dec:
+000022e0: 6465 632b 325d 290a 2020 2020 2020 2020  dec+2]).        
+000022f0: 2020 2020 2020 2020 2020 2020 6420 3d20              d = 
+00002300: 696e 7428 7365 6c66 2e74 6578 745b 6465  int(self.text[de
+00002310: 632b 323a 5d29 0a20 2020 2020 2020 2020  c+2:]).         
+00002320: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
+00002330: 7465 7469 6d65 2e64 6174 6528 792c 206d  tetime.date(y, m
+00002340: 2c20 6429 0a20 2020 2020 2020 2020 2020  , d).           
+00002350: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+00002360: 2020 2020 2020 2020 2065 7272 6d73 6720           errmsg 
+00002370: 3d20 5f28 2245 7272 6f72 3a20 636f 756c  = _("Error: coul
+00002380: 6420 6e6f 7420 756e 6465 7273 7461 6e64  d not understand
+00002390: 2064 6174 6522 290a 2020 2020 2020 2020   date").        
+000023a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000023b0: 656c 662e 6572 726f 7228 6572 726d 7367  elf.error(errmsg
+000023c0: 290a 0a20 2020 2064 6566 2063 6865 636b  )..    def check
+000023d0: 5f66 696c 656e 616d 6528 7365 6c66 2c20  _filename(self, 
+000023e0: 6d6f 6465 293a 0a20 2020 2020 2020 2074  mode):.        t
+000023f0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00002400: 6966 2028 2873 656c 662e 7465 7874 5b2d  if ((self.text[-
+00002410: 325d 203d 3d20 2220 2229 0a20 2020 2020  2] == " ").     
+00002420: 2020 2020 2020 2020 2020 616e 6420 2873            and (s
+00002430: 656c 662e 7465 7874 5b2d 315d 2069 6e20  elf.text[-1] in 
+00002440: 5b73 7472 2869 2920 666f 7220 6920 696e  [str(i) for i in
+00002450: 2072 616e 6765 2838 295d 2929 3a0a 2020   range(8)])):.  
+00002460: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00002470: 7370 6563 6961 6c20 6361 7365 3a20 6869  special case: hi
+00002480: 6464 656e 2066 696e 616c 2074 6167 0a20  dden final tag. 
+00002490: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000024a0: 203d 206f 7065 6e28 7365 6c66 2e74 6578   = open(self.tex
+000024b0: 745b 3a2d 325d 2c20 6d6f 6465 290a 2020  t[:-2], mode).  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 662e                f.
+000024d0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
+000024e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000024f0: 2020 2020 2020 2020 2020 6620 3d20 6f70            f = op
+00002500: 656e 2873 656c 662e 7465 7874 2c20 6d6f  en(self.text, mo
+00002510: 6465 290a 2020 2020 2020 2020 2020 2020  de).            
+00002520: 2020 2020 662e 636c 6f73 6528 290a 2020      f.close().  
+00002530: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002540: 2073 656c 662e 7465 7874 0a20 2020 2020   self.text.     
+00002550: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+00002560: 2020 2020 2020 2069 6620 6d6f 6465 203d         if mode =
+00002570: 3d20 2272 6222 3a0a 2020 2020 2020 2020  = "rb":.        
+00002580: 2020 2020 2020 2020 6572 726d 7367 203d          errmsg =
+00002590: 205f 2822 4572 726f 723a 2075 6e61 626c   _("Error: unabl
+000025a0: 6520 746f 2072 6561 6420 7468 6520 6669  e to read the fi
+000025b0: 6c65 2022 290a 2020 2020 2020 2020 2020  le ").          
+000025c0: 2020 656c 6966 206d 6f64 6520 3d3d 2022    elif mode == "
+000025d0: 7762 223a 0a20 2020 2020 2020 2020 2020  wb":.           
+000025e0: 2020 2020 2065 7272 6d73 6720 3d20 5f28       errmsg = _(
+000025f0: 2245 7272 6f72 3a20 756e 6162 6c65 2074  "Error: unable t
+00002600: 6f20 7772 6974 6520 7468 6520 6669 6c65  o write the file
+00002610: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
+00002620: 7265 7475 726e 2073 656c 662e 6572 726f  return self.erro
+00002630: 7228 6572 726d 7367 202b 2073 656c 662e  r(errmsg + self.
+00002640: 7465 7874 290a 0a20 2020 2064 6566 2063  text)..    def c
+00002650: 6865 636b 5f69 6e74 686f 7572 2873 656c  heck_inthour(sel
+00002660: 6629 3a0a 2020 2020 2020 2020 7472 793a  f):.        try:
+00002670: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00002680: 696e 7428 7365 6c66 2e74 6578 7429 203c  int(self.text) <
+00002690: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+000026a0: 2020 2020 6572 726d 7367 203d 205f 2822      errmsg = _("
+000026b0: 4572 726f 723a 2073 686f 756c 6420 6265  Error: should be
+000026c0: 2068 6967 6865 7220 7468 616e 2030 2229   higher than 0")
+000026d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026e0: 2072 6574 7572 6e20 7365 6c66 2e65 7272   return self.err
+000026f0: 6f72 2865 7272 6d73 6729 0a20 2020 2020  or(errmsg).     
+00002700: 2020 2020 2020 2069 6620 696e 7428 7365         if int(se
+00002710: 6c66 2e74 6578 7429 203e 2032 343a 0a20  lf.text) > 24:. 
+00002720: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00002730: 7272 6d73 6720 3d20 5f28 2245 7272 6f72  rrmsg = _("Error
+00002740: 3a20 7368 6f75 6c64 2062 6520 6c6f 7765  : should be lowe
+00002750: 7220 7468 616e 2032 3422 290a 2020 2020  r than 24").    
+00002760: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002770: 726e 2073 656c 662e 6572 726f 7228 6572  rn self.error(er
+00002780: 726d 7367 290a 2020 2020 2020 2020 2020  rmsg).          
+00002790: 2020 7265 7475 726e 2069 6e74 2873 656c    return int(sel
+000027a0: 662e 7465 7874 290a 2020 2020 2020 2020  f.text).        
+000027b0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+000027c0: 2020 2020 6572 726d 7367 203d 205f 2822      errmsg = _("
+000027d0: 4572 726f 723a 206d 7573 7420 6265 2061  Error: must be a
+000027e0: 6e20 696e 7465 6765 7222 290a 2020 2020  n integer").    
+000027f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002800: 656c 662e 6572 726f 7228 6572 726d 7367  elf.error(errmsg
+00002810: 290a                                     ).
```

### Comparing `culendar-0.20230330/src/culendar/cul/mouse.py` & `culendar-0.20230510/culendar/cul/mouse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#! /usr/bin/env python3
-# coding: utf-8
 import curses
 
 
 def clicked(cul):
     try:
         _, x, y, _, click_type = curses.getmouse()
     except:
@@ -11,15 +9,15 @@
         y = -1
         click_type = -1
         click = "bug"
         cul.screen.addstr(1, 1, "bug detected")
 
     # the todo list has been clicked
     if cul.conf.todo and x >= cul._xmax:  # MOCHE²
-        if not(cul._todohl):  # MOCHE
+        if not cul._todohl:  # MOCHE
             cul.toggle_TODO()
         if (y-2) in range(len(cul._todo.events)):
             # select a todo, starting on line 2, todohl starts at 1
             cul._todohl = y-2 + 1
             cul.draw_todo()
 
     elif x <= cul._xoffset:
```

### Comparing `culendar-0.20230330/src/culendar/locale/fr/LC_MESSAGES/culendar.mo` & `culendar-0.20230510/culendar/locale/fr/LC_MESSAGES/culendar.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -116,15 +116,16 @@
 msgstr "Éditer l'événement ou la tâche sélectionné (le cas échéant)"
 
 msgid "Edit: (1) [i]tem, (2) [d]ate, (3) [r]emove date"
 msgstr "Éditer : (1) tâche, (2) [d]ate, (3) supp[r]imer la date"
 
 msgid "Edit: (1) [s]tart time, (2) [e]nd time, (3) [d]escription, (4) [p]lace"
 msgstr ""
-"Éditer : (1) heure de début, (2) h[e]ure de fin, (3) [d]escription, (4) lieu"
+"Éditer : (1) heure de [d]ébut, (2) heure de [f]in, (3) de[s]cription, (4) "
+"[l]ieu"
 
 msgid "End date:   {}"
 msgstr "Date de fin :   {}"
 
 msgid "Ending time should be greater than "
 msgstr "L'heure de fin doit être supérieure à "
```

### Comparing `culendar-0.20230330/src/culendar/locale/fr/LC_MESSAGES/culendar.pot` & `culendar-0.20230510/culendar/locale/fr/LC_MESSAGES/culendar.pot`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
 #: cul/culendar.py:352
 msgid "Error: can't delete webcal event"
 msgstr "Erreur : impossible de supprimer des événements d'un webcal"
 
 #: cul/culendar.py:366
 msgid "Edit: (1) [s]tart time, (2) [e]nd time, (3) [d]escription, (4) [p]lace"
 msgstr ""
-"Éditer : (1) heure de début, (2) h[e]ure de fin, (3) [d]escription, (4) lieu"
+"Éditer : (1) heure de [d]ébut, (2) heure de [f]in, (3) de[s]cription, (4) [l]ieu"
 
 #: cul/culendar.py:426
 msgid "Edit: (1) [i]tem, (2) [d]ate, (3) [r]emove date"
 msgstr "Éditer : (1) tâche, (2) [d]ate, (3) supp[r]imer la date"
 
 #: cul/culendar.py:518
 msgid "Enter start time ([hh:mm], [hhmm], [hh] or [h]):"
```

### Comparing `culendar-0.20230330/README.md` & `culendar-0.20230510/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,26 +11,30 @@
   files
 - Customizable
 - Displays webcals
 - Deals with caldavs
 
 ## How to install
 - pip install culendar
+
 or
+
 - git clone https://framagit.org/mit/culendar
-- pip install icalendar caldav
+- cd culendar
+- poetry install
+- poetry run culendar to run it
 
 ## How to use
 - Run it. Default key "h" to get help, "c" to configure.
 
 ## No warranties
 Culendar has been tested on Debian stable and old-stable,
 rxvt-unicode as a terminal and UTF-8 encoding only.
 It needs much more testing to be officially reliable.
 
-Don't hesitate to report bugs or request features.
+Don't hesitate to [report bugs](https://framagit.org/mit/culendar/-/issues) or [request features](https://framagit.org/mit/culendar/-/merge_requests).
 
 ## Screenshots
 ![culendar screenshot](screenshot0.png)
 
 ## Chat:
 IRC: #culendar on irc.geeknode.org/6697
```

