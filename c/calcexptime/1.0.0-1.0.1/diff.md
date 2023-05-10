# Comparing `tmp/calcexptime-1.0.0-py3-none-any.whl.zip` & `tmp/calcexptime-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3482 bytes, number of entries: 8
--rw-rw-r--  2.0 unx       47 b- defN 23-May-10 14:45 calcexptime/__init__.py
+Zip file size: 3526 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx       47 b- defN 23-May-10 14:54 calcexptime/__init__.py
 -rw-rw-r--  2.0 unx      789 b- defN 23-May-10 14:50 calcexptime/__main__.py
 -rw-rw-r--  2.0 unx      749 b- defN 23-May-10 14:33 calcexptime/functions.py
--rw-rw-r--  2.0 unx     1072 b- defN 23-May-10 14:50 calcexptime-1.0.0.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      589 b- defN 23-May-10 14:50 calcexptime-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-10 14:50 calcexptime-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       12 b- defN 23-May-10 14:50 calcexptime-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-May-10 14:50 calcexptime-1.0.0.dist-info/RECORD
-8 files, 3996 bytes uncompressed, 2346 bytes compressed:  41.3%
+-rw-rw-r--  2.0 unx     1072 b- defN 23-May-10 14:55 calcexptime-1.0.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      658 b- defN 23-May-10 14:55 calcexptime-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-10 14:55 calcexptime-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-May-10 14:55 calcexptime-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-May-10 14:55 calcexptime-1.0.1.dist-info/RECORD
+8 files, 4065 bytes uncompressed, 2390 bytes compressed:  41.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: calcexptime/__main__.py
 Comment: 
 
 Filename: calcexptime/functions.py
 Comment: 
 
-Filename: calcexptime-1.0.0.dist-info/LICENSE.txt
+Filename: calcexptime-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: calcexptime-1.0.0.dist-info/METADATA
+Filename: calcexptime-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: calcexptime-1.0.0.dist-info/WHEEL
+Filename: calcexptime-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: calcexptime-1.0.0.dist-info/top_level.txt
+Filename: calcexptime-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: calcexptime-1.0.0.dist-info/RECORD
+Filename: calcexptime-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## calcexptime/__init__.py

```diff
@@ -1,3 +1,3 @@
 #! /usr/bin/env python3
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
```

## Comparing `calcexptime-1.0.0.dist-info/LICENSE.txt` & `calcexptime-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `calcexptime-1.0.0.dist-info/METADATA` & `calcexptime-1.0.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: calcexptime
-Version: 1.0.0
+Version: 1.0.1
 Summary: Calculates the duration of an experiment and tells when it does end.
 Home-page: https://github.com/MetallerTM/calcexptime
 Author: Francesco Bruno
 Author-email: bruno@cerm.unifi.it
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 Calculates the duration of an experiment and tells when it does end.
+## USAGE
+$ python -m calcexptime <days> <hours> <minutes> <seconds>
+
```

## Comparing `calcexptime-1.0.0.dist-info/RECORD` & `calcexptime-1.0.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-calcexptime/__init__.py,sha256=zHzp4AlYOF3j_HIphmwhDr2ejLRodxGEZrKN4pvnQdc,47
+calcexptime/__init__.py,sha256=UKZkLK3K5McRG-HCUMrAJMu0Mjp_4ziqOMlPQRXx84g,47
 calcexptime/__main__.py,sha256=5iM0s17FhIz4HsneqNn4qgUp_wbVKOK9-9KhOHuL_VQ,789
 calcexptime/functions.py,sha256=UVhJsN_XOfy8kq8mJvyPizxxMLacI7youQqfG36WNCw,749
-calcexptime-1.0.0.dist-info/LICENSE.txt,sha256=32XIIeXICyXXJGzWS0m_8zV3ebN6RACNkDoHRlWLVwM,1072
-calcexptime-1.0.0.dist-info/METADATA,sha256=9ujB2RT_qftSIqocjFRgiiV-g0sT8KEKvlTMJS95Yn0,589
-calcexptime-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-calcexptime-1.0.0.dist-info/top_level.txt,sha256=q7V3dOKjI3JhDlJmsgjNYfeSRKhfkXvw36oFytsUOxE,12
-calcexptime-1.0.0.dist-info/RECORD,,
+calcexptime-1.0.1.dist-info/LICENSE.txt,sha256=32XIIeXICyXXJGzWS0m_8zV3ebN6RACNkDoHRlWLVwM,1072
+calcexptime-1.0.1.dist-info/METADATA,sha256=UKrD1RxBKPVfNMwTCHl8hRwrrC8mAPuUeGt4Oj4Dy1U,658
+calcexptime-1.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+calcexptime-1.0.1.dist-info/top_level.txt,sha256=q7V3dOKjI3JhDlJmsgjNYfeSRKhfkXvw36oFytsUOxE,12
+calcexptime-1.0.1.dist-info/RECORD,,
```

