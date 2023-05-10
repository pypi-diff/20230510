# Comparing `tmp/eFatura-0.1.0.tar.gz` & `tmp/eFatura-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-0.1.0.tar", last modified: Wed May 10 13:28:49 2023, max compression
+gzip compressed data, was "eFatura-0.1.1.tar", last modified: Wed May 10 13:36:03 2023, max compression
```

## Comparing `eFatura-0.1.0.tar` & `eFatura-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:28:49.114441 eFatura-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 13:28:31.000000 eFatura-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 13:28:49.114441 eFatura-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-10 13:28:31.000000 eFatura-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:28:49.114441 eFatura-0.1.0/eFatura/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 13:28:31.000000 eFatura-0.1.0/eFatura/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 13:28:31.000000 eFatura-0.1.0/eFatura/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:28:49.114441 eFatura-0.1.0/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:28:49.114441 eFatura-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 13:28:31.000000 eFatura-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:36:03.300023 eFatura-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 13:35:43.000000 eFatura-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 13:36:03.296023 eFatura-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-10 13:35:43.000000 eFatura-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:36:03.296023 eFatura-0.1.1/eFatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 13:35:43.000000 eFatura-0.1.1/eFatura/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 13:35:43.000000 eFatura-0.1.1/eFatura/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:36:03.296023 eFatura-0.1.1/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:36:03.300023 eFatura-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 13:35:43.000000 eFatura-0.1.1/setup.py
```

### Comparing `eFatura-0.1.0/PKG-INFO` & `eFatura-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.1.0
+Version: 0.1.1
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Mükellef Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.1.0 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.1.1 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
 Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
```

### Comparing `eFatura-0.1.0/README.md` & `eFatura-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `eFatura-0.1.0/eFatura/Oturum.py` & `eFatura-0.1.1/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.1.0/eFatura/__init__.py` & `eFatura-0.1.1/eFatura/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.1.0/eFatura.egg-info/PKG-INFO` & `eFatura-0.1.1/eFatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.1.0
+Version: 0.1.1
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Mükellef Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.1.0 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.1.1 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
 Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
```

### Comparing `eFatura-0.1.0/setup.py` & `eFatura-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["eFatura"],
 
     name         = "eFatura",
-    version      = "0.1.0",
+    version      = "0.1.1",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["Mükellef Sorgu", "eFatura", "KekikAkademi", "keyiflerolsun"],
 
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True,
```

