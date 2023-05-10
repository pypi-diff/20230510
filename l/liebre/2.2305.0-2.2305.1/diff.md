# Comparing `tmp/liebre-2.2305.0-py3-none-any.whl.zip` & `tmp/liebre-2.2305.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20147 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      222 b- defN 23-May-03 10:32 liebre/__init__.py
+Zip file size: 20153 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      222 b- defN 23-May-09 21:05 liebre/__init__.py
 -rw-rw-r--  2.0 unx     8384 b- defN 23-Apr-27 22:14 liebre/consumer.py
 -rw-rw-r--  2.0 unx       46 b- defN 22-Dec-07 11:43 liebre/liebre.py
 -rw-rw-r--  2.0 unx       69 b- defN 22-Dec-07 11:44 liebre/logger.py
 -rw-rw-r--  2.0 unx      490 b- defN 23-Apr-19 20:41 liebre/message.py
 -rw-rw-r--  2.0 unx     2535 b- defN 23-Apr-27 14:44 liebre/producer.py
--rw-rw-r--  2.0 unx     8171 b- defN 23-Apr-27 22:14 liebre/rabbit_store.py
+-rw-rw-r--  2.0 unx     8217 b- defN 23-May-09 21:05 liebre/rabbit_store.py
 -rw-rw-r--  2.0 unx     1018 b- defN 23-Apr-27 14:55 liebre/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      730 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      985 b- defN 23-May-03 10:32 liebre-2.2305.0.dist-info/RECORD
-13 files, 57898 bytes uncompressed, 18519 bytes compressed:  68.0%
+-rw-rw-r--  2.0 unx    35149 b- defN 23-May-10 18:05 liebre-2.2305.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      730 b- defN 23-May-10 18:05 liebre-2.2305.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-10 18:05 liebre-2.2305.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-10 18:05 liebre-2.2305.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      985 b- defN 23-May-10 18:05 liebre-2.2305.1.dist-info/RECORD
+13 files, 57944 bytes uncompressed, 18525 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: liebre/rabbit_store.py
 Comment: 
 
 Filename: liebre/utils.py
 Comment: 
 
-Filename: liebre-2.2305.0.dist-info/LICENSE
+Filename: liebre-2.2305.1.dist-info/LICENSE
 Comment: 
 
-Filename: liebre-2.2305.0.dist-info/METADATA
+Filename: liebre-2.2305.1.dist-info/METADATA
 Comment: 
 
-Filename: liebre-2.2305.0.dist-info/WHEEL
+Filename: liebre-2.2305.1.dist-info/WHEEL
 Comment: 
 
-Filename: liebre-2.2305.0.dist-info/top_level.txt
+Filename: liebre-2.2305.1.dist-info/top_level.txt
 Comment: 
 
-Filename: liebre-2.2305.0.dist-info/RECORD
+Filename: liebre-2.2305.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## liebre/__init__.py

```diff
@@ -2,10 +2,10 @@
 # -*- coding: utf-8 -*-
 
 from .consumer import Consumer  # noqa F401
 from .producer import Producer  # noqa F401
 
 import logging
 
-__version__ = '2.2305.0'
+__version__ = '2.2305.1'
 
 logging.getLogger('pika').propagate = False
```

## liebre/rabbit_store.py

```diff
@@ -84,14 +84,15 @@
         self._declared_queues = set()
         self._declared_logical_queues = set()
 
         self._message_retries = {}
         self._lock = Lock()
 
         self._initialized = False
+        self._channel = None
 
     def reconnect(function):
 
         def _(*args, **kwargs):
             retries = 0
             instance = args[0]
 
@@ -133,15 +134,16 @@
                 return function(*args, **kwargs)
 
         return _
 
     def connect(self, force=False):
         if self._initialized and not force:
             return
-        elif force:
+
+        if force and self._channel:
             RabbitStore._close_channel(self._channel)
 
         self._channel = self._get_channel()
         self._declare_exchange()
 
         self._initialized = True
```

## Comparing `liebre-2.2305.0.dist-info/LICENSE` & `liebre-2.2305.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `liebre-2.2305.0.dist-info/METADATA` & `liebre-2.2305.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liebre
-Version: 2.2305.0
+Version: 2.2305.1
 Home-page: https://github.com/councilbox/liebre-python
 Author: 
 Author-email: 
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

## Comparing `liebre-2.2305.0.dist-info/RECORD` & `liebre-2.2305.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-liebre/__init__.py,sha256=lagqSobqe189CGJzaJCLOxZuL4RX1kAfeaROcVGvaCI,222
+liebre/__init__.py,sha256=qtiQwtoOUfmCx9DRC5JBCxZaZx8xSmrm-LlK-j1kQbE,222
 liebre/consumer.py,sha256=5ZWDGJPsb6k_rLpMKdN4597jL8SCgI1WyCq5tSqBWxU,8384
 liebre/liebre.py,sha256=FZk9hm7vBsK8G16pNugputbrrEciYqJc_XRAhTCcojI,46
 liebre/logger.py,sha256=gFdT_UHqta9GXzzGK44_sDagnInpWDLKXDJ3J4ZJkmc,69
 liebre/message.py,sha256=LsyOktRKgYOs5FzllpmfuoWWKM8t9mB7-OSRFVnjXxE,490
 liebre/producer.py,sha256=JFjqRpR5k7Sl2c3ZM2I-HoWOIbjMOUb-sQ4uk3JXa00,2535
-liebre/rabbit_store.py,sha256=Eg_Crj1e1LH3KkENMlVROWmvhT8yac8P3BMlLWIuMkI,8171
+liebre/rabbit_store.py,sha256=4qHpJw1rtKDtijD3zsqfCkWcJLknJ_PM4ebb75dO8uc,8217
 liebre/utils.py,sha256=2SElH6GLKFTuLpSzZwWfLa2VTzHetfxtXPfGuEuLcWM,1018
-liebre-2.2305.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-liebre-2.2305.0.dist-info/METADATA,sha256=khfOlvYmOOIbawqkcoONKA28IQQXfpVFcKcbfltnm44,730
-liebre-2.2305.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-liebre-2.2305.0.dist-info/top_level.txt,sha256=cl5ALalM53myFXDcFp7jtynIzvwoKF4RqF1x1Aw4WwY,7
-liebre-2.2305.0.dist-info/RECORD,,
+liebre-2.2305.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+liebre-2.2305.1.dist-info/METADATA,sha256=cO60GDVC2I28QhbUsih2RNpgPjUoq2k2K9RkuvEgk3k,730
+liebre-2.2305.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+liebre-2.2305.1.dist-info/top_level.txt,sha256=cl5ALalM53myFXDcFp7jtynIzvwoKF4RqF1x1Aw4WwY,7
+liebre-2.2305.1.dist-info/RECORD,,
```

