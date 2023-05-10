# Comparing `tmp/pytestifyx-0.4.1-py2.py3-none-any.whl.zip` & `tmp/pytestifyx-0.4.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 55873 bytes, number of entries: 88
--rw-r--r--  2.0 unx      208 b- defN 23-May-10 13:56 pytestifyx/__init__.py
+Zip file size: 55870 bytes, number of entries: 88
+-rw-r--r--  2.0 unx      208 b- defN 23-May-10 13:59 pytestifyx/__init__.py
 -rw-r--r--  2.0 unx      302 b- defN 23-May-10 13:55 pytestifyx/chinese_fix.py
 -rw-r--r--  2.0 unx      846 b- defN 23-Apr-02 10:19 pytestifyx/cli.py
 -rw-r--r--  2.0 unx     1708 b- defN 23-Apr-02 08:42 pytestifyx/config.py
 -rw-r--r--  2.0 unx      722 b- defN 23-Apr-02 08:45 pytestifyx/core.py
 -rw-r--r--  2.0 unx     2085 b- defN 23-Apr-02 11:05 pytestifyx/scaffold.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 12:47 pytestifyx/driver/__init__.py
 -rw-r--r--  2.0 unx    14025 b- defN 23-May-10 13:45 pytestifyx/driver/api.py
@@ -77,14 +77,14 @@
 -rw-r--r--  2.0 unx      623 b- defN 23-Apr-02 08:59 pytestifyx/utils/public/get_project_path.py
 -rw-r--r--  2.0 unx      300 b- defN 23-Feb-23 12:06 pytestifyx/utils/public/img_to_base64.py
 -rw-r--r--  2.0 unx      372 b- defN 23-May-10 13:35 pytestifyx/utils/public/printify_table.py
 -rw-r--r--  2.0 unx      608 b- defN 23-May-10 13:36 pytestifyx/utils/public/trans_param_style.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-19 04:37 pytestifyx/utils/requests/__init__.py
 -rw-r--r--  2.0 unx      464 b- defN 22-Nov-21 14:29 pytestifyx/utils/requests/reload_all.py
 -rw-r--r--  2.0 unx     2434 b- defN 23-May-10 13:29 pytestifyx/utils/requests/requests_config.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-10 13:56 pytestifyx-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1078 b- defN 23-May-10 13:56 pytestifyx-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-10 13:56 pytestifyx-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 23-May-10 13:56 pytestifyx-0.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-10 13:56 pytestifyx-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8741 b- defN 23-May-10 13:56 pytestifyx-0.4.1.dist-info/RECORD
-88 files, 133219 bytes uncompressed, 41329 bytes compressed:  69.0%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-10 13:59 pytestifyx-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1078 b- defN 23-May-10 13:59 pytestifyx-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-10 13:59 pytestifyx-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      132 b- defN 23-May-10 13:59 pytestifyx-0.4.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-10 13:59 pytestifyx-0.4.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     8741 b- defN 23-May-10 13:59 pytestifyx-0.4.2.dist-info/RECORD
+88 files, 133212 bytes uncompressed, 41326 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -240,26 +240,26 @@
 
 Filename: pytestifyx/utils/requests/reload_all.py
 Comment: 
 
 Filename: pytestifyx/utils/requests/requests_config.py
 Comment: 
 
-Filename: pytestifyx-0.4.1.dist-info/LICENSE
+Filename: pytestifyx-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: pytestifyx-0.4.1.dist-info/METADATA
+Filename: pytestifyx-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: pytestifyx-0.4.1.dist-info/WHEEL
+Filename: pytestifyx-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: pytestifyx-0.4.1.dist-info/entry_points.txt
+Filename: pytestifyx-0.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytestifyx-0.4.1.dist-info/top_level.txt
+Filename: pytestifyx-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pytestifyx-0.4.1.dist-info/RECORD
+Filename: pytestifyx-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytestifyx/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .core import TestCase
 from .utils.logs.core import log
 
 __author__ = "luyh"
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 __description__ = "pytestifyx is a pytest-based automation testing framework for api, ui, app testing"
```

## Comparing `pytestifyx-0.4.1.dist-info/LICENSE` & `pytestifyx-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytestifyx-0.4.1.dist-info/METADATA` & `pytestifyx-0.4.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestifyx
-Version: 0.4.1
+Version: 0.4.2
 Summary: pytestifyx is a pytest-based automation testing framework for api, ui, app testing
 Home-page: https://github.com/jaylu2018/PyTestifyx
 Author: luyh
 Author-email: jaylu1995@outlook.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `pytestifyx-0.4.1.dist-info/RECORD` & `pytestifyx-0.4.2.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pytestifyx/__init__.py,sha256=L9nfitHM2y7XSbVITupEGOg-UsUlCcBDG47uPLQG0JU,208
+pytestifyx/__init__.py,sha256=tBSTC4khrv2Dtny67VUp2_RbvGqNXcvWxxFrvZM7CjI,208
 pytestifyx/chinese_fix.py,sha256=qFkCAFR4EspSMgeBwuiAZ9zl51SEESgp4wKqEFqzGe8,302
 pytestifyx/cli.py,sha256=VZn72UAbdOG2n5SAZ5Q8OigiukupTPb28jbGsER12Y8,846
 pytestifyx/config.py,sha256=gL13H5yDGh_B4_MPDIGVx7JcZOUjWxRISKJNMUkSLUA,1708
 pytestifyx/core.py,sha256=b3csTW1gnhPalyhxHOWC5SAnh1jOZ0lYznBxVT5QlRo,722
 pytestifyx/scaffold.py,sha256=c-zhigz3Zqo2zwt3r9H6Wu-6MQPR27-Q4qU6M3-cQGc,2085
 pytestifyx/driver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/driver/api.py,sha256=g5re2-EQCmUnxX-kpP2XthtfyDR0lULF7MokQdQRcVg,14025
@@ -76,13 +76,13 @@
 pytestifyx/utils/public/get_project_path.py,sha256=ijIqYm2fHT4dV_3IcTqllk5lmLlAGVn59zPU-juiGL4,623
 pytestifyx/utils/public/img_to_base64.py,sha256=IxTLg8b_QINdixlU-HTiWQ57CT4F8Yu3VXIcms2QRHo,300
 pytestifyx/utils/public/printify_table.py,sha256=9fWgPBfsDwnnkFJKi57tHFZtdFARdYoWS-3le4I_Jpk,372
 pytestifyx/utils/public/trans_param_style.py,sha256=lYJR85uWtLPoqpK3N_ja53jqMu3tMasR61PGsUQCZqk,608
 pytestifyx/utils/requests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytestifyx/utils/requests/reload_all.py,sha256=rB3ORnl1cYZ7vkAUitzVNOg2TV2Ao1OlvQqmZVopZ6w,464
 pytestifyx/utils/requests/requests_config.py,sha256=FVSD8oPa4IAINPcJHYU0WkRIDvB_XYC0iO41rGr-BxI,2434
-pytestifyx-0.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytestifyx-0.4.1.dist-info/METADATA,sha256=vJArniY540xPjcdvP3ya-jB1dqg1yWtPEpBd84ZvCXo,1078
-pytestifyx-0.4.1.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-pytestifyx-0.4.1.dist-info/entry_points.txt,sha256=Dt5CHNF5Enqy_JSKmcQNCZr1UrrW4Dbgg_qb48pkjuI,139
-pytestifyx-0.4.1.dist-info/top_level.txt,sha256=23Gy2nqjjqGWQb8BZflCf5s-b45IGeZf8rn1Xnwzey4,11
-pytestifyx-0.4.1.dist-info/RECORD,,
+pytestifyx-0.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytestifyx-0.4.2.dist-info/METADATA,sha256=wQwO0hNMxnnvNDSSx2k_QbGeQzmmQb1HqxolSVxALBE,1078
+pytestifyx-0.4.2.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+pytestifyx-0.4.2.dist-info/entry_points.txt,sha256=_NGX3x3KtjAIOUbVkx_ThOrqE5vJzHT3WemSc0ZHEn0,132
+pytestifyx-0.4.2.dist-info/top_level.txt,sha256=23Gy2nqjjqGWQb8BZflCf5s-b45IGeZf8rn1Xnwzey4,11
+pytestifyx-0.4.2.dist-info/RECORD,,
```

