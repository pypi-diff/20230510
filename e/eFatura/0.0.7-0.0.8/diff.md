# Comparing `tmp/eFatura-0.0.7.tar.gz` & `tmp/eFatura-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-0.0.7.tar", last modified: Wed May 10 12:55:03 2023, max compression
+gzip compressed data, was "eFatura-0.0.8.tar", last modified: Wed May 10 13:16:52 2023, max compression
```

## Comparing `eFatura-0.0.7.tar` & `eFatura-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:55:03.767028 eFatura-0.0.7/
--rw-r--r--   0 sancak    (1000) sancak    (1000)       27 2023-05-10 08:30:46.000000 eFatura-0.0.7/MANIFEST.in
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2831 2023-05-10 12:55:03.767028 eFatura-0.0.7/PKG-INFO
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2252 2023-05-10 12:42:19.000000 eFatura-0.0.7/README.md
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:55:03.763695 eFatura-0.0.7/eFatura/
--rw-r--r--   0 sancak    (1000) sancak    (1000)      785 2023-05-10 11:53:39.000000 eFatura-0.0.7/eFatura/Oturum.py
--rw-r--r--   0 sancak    (1000) sancak    (1000)     1448 2023-05-10 12:42:19.000000 eFatura-0.0.7/eFatura/__init__.py
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:55:03.767028 eFatura-0.0.7/eFatura.egg-info/
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2831 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 sancak    (1000) sancak    (1000)      222 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)        1 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)       53 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/requires.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)        8 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/top_level.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)       38 2023-05-10 12:55:03.767028 eFatura-0.0.7/setup.cfg
--rw-r--r--   0 sancak    (1000) sancak    (1000)     1176 2023-05-10 12:54:46.000000 eFatura-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:16:52.893552 eFatura-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 13:16:27.000000 eFatura-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-10 13:16:52.893552 eFatura-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-10 13:16:27.000000 eFatura-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:16:52.893552 eFatura-0.0.8/eFatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 13:16:27.000000 eFatura-0.0.8/eFatura/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 13:16:27.000000 eFatura-0.0.8/eFatura/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:16:52.893552 eFatura-0.0.8/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:16:52.893552 eFatura-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 13:16:27.000000 eFatura-0.0.8/setup.py
```

### Comparing `eFatura-0.0.7/PKG-INFO` & `eFatura-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.7 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.8 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
 Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
```

### Comparing `eFatura-0.0.7/README.md` & `eFatura-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.7/eFatura/Oturum.py` & `eFatura-0.0.8/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.7/eFatura/__init__.py` & `eFatura-0.0.8/eFatura/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .Oturum     import legacy_session
 from shutil      import copyfileobj
 from uuid        import uuid4
 from os          import remove
 from PIL         import Image
 from pytesseract import image_to_string
 
-def e_fatura(vergi_numarasi:str) -> bool | None:
+def e_fatura(vergi_numarasi:str) -> bool:
     """Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu"""
     captcha_resmi = f"captcha_{uuid4()}.jpg"
 
     while True:
         oturum = legacy_session()
         oturum.headers.update({
             "User-Agent" : "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"
@@ -27,11 +27,8 @@
         e_fatura_istek = oturum.post(
             url  = "https://sorgu.efatura.gov.tr/kullanicilar/xliste.php",
             data = {"search_string": f"{vergi_numarasi}", "captcha_code": f"{captcha_metni}", "submit": "Ara"}
         )
         if "Güvenlik kodu hatalı" in e_fatura_istek.text:
             continue
 
-        if "kayıt bulunamadı" in e_fatura_istek.text:
-            return None
-
         return "Mükellef kayıtlıdır" in e_fatura_istek.text
```

### Comparing `eFatura-0.0.7/eFatura.egg-info/PKG-INFO` & `eFatura-0.0.8/eFatura.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.7 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.8 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
 Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
```

### Comparing `eFatura-0.0.7/setup.py` & `eFatura-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["eFatura"],
 
     name         = "eFatura",
-    version      = "0.0.7",
+    version      = "0.0.8",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["Mükellef Sorgu", "eFatura", "KekikAkademi", "keyiflerolsun"],
 
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True,
```

