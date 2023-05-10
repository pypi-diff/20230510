# Comparing `tmp/eFatura-1.0.0.tar.gz` & `tmp/eFatura-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-1.0.0.tar", last modified: Wed May 10 14:06:12 2023, max compression
+gzip compressed data, was "eFatura-1.0.1.tar", last modified: Wed May 10 14:07:50 2023, max compression
```

## Comparing `eFatura-1.0.0.tar` & `eFatura-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:06:12.752952 eFatura-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 14:05:54.000000 eFatura-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-10 14:06:12.752952 eFatura-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-10 14:05:54.000000 eFatura-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:06:12.752952 eFatura-1.0.0/eFatura/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 14:05:54.000000 eFatura-1.0.0/eFatura/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 14:05:54.000000 eFatura-1.0.0/eFatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-10 14:05:54.000000 eFatura-1.0.0/eFatura/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:06:12.752952 eFatura-1.0.0/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-10 14:06:12.000000 eFatura-1.0.0/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 14:06:12.000000 eFatura-1.0.0/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:06:12.000000 eFatura-1.0.0/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 14:06:12.000000 eFatura-1.0.0/eFatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 14:06:12.000000 eFatura-1.0.0/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 14:06:12.000000 eFatura-1.0.0/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:06:12.752952 eFatura-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-10 14:05:54.000000 eFatura-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:50.868749 eFatura-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 14:07:30.000000 eFatura-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-10 14:07:50.868749 eFatura-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-10 14:07:30.000000 eFatura-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:50.868749 eFatura-1.0.1/eFatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 14:07:30.000000 eFatura-1.0.1/eFatura/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 14:07:30.000000 eFatura-1.0.1/eFatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-10 14:07:30.000000 eFatura-1.0.1/eFatura/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:50.868749 eFatura-1.0.1/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 14:07:50.000000 eFatura-1.0.1/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:07:50.872749 eFatura-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-10 14:07:30.000000 eFatura-1.0.1/setup.py
```

### Comparing `eFatura-1.0.0/PKG-INFO` & `eFatura-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.0
+Version: 1.0.1
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.0 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.0.1 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
```

### Comparing `eFatura-1.0.0/README.md` & `eFatura-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.0/eFatura/Oturum.py` & `eFatura-1.0.1/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.0/eFatura/__init__.py` & `eFatura-1.0.1/eFatura/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.0/eFatura/konsol.py` & `eFatura-1.0.1/eFatura/konsol.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.0/eFatura.egg-info/PKG-INFO` & `eFatura-1.0.1/eFatura.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.0
+Version: 1.0.1
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.0 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.0.1 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
```

### Comparing `eFatura-1.0.0/setup.py` & `eFatura-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eFatura",
-    version      = "1.0.0",
+    version      = "1.0.1",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["eFatura", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -23,14 +23,15 @@
 
     # ? Paket Bilgileri
     packages         = ["eFatura"],
     python_requires  = ">=3.10",
     install_requires = [
         "setuptools",
         "wheel",
+        "Kekik",
         "requests",
         "urllib3",
         "Pillow",
         "pytesseract"
     ],
 
     # ? Konsoldan Çalıştırılabilir
```

