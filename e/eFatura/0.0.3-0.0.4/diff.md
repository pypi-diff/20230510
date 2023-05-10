# Comparing `tmp/eFatura-0.0.3.tar.gz` & `tmp/eFatura-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-0.0.3.tar", last modified: Wed May 10 12:31:40 2023, max compression
+gzip compressed data, was "eFatura-0.0.4.tar", last modified: Wed May 10 12:37:13 2023, max compression
```

## Comparing `eFatura-0.0.3.tar` & `eFatura-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:31:40.570857 eFatura-0.0.3/
--rw-r--r--   0 sancak    (1000) sancak    (1000)       27 2023-05-10 08:30:46.000000 eFatura-0.0.3/MANIFEST.in
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2765 2023-05-10 12:31:40.567524 eFatura-0.0.3/PKG-INFO
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2216 2023-05-10 12:29:28.000000 eFatura-0.0.3/README.md
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:31:40.564191 eFatura-0.0.3/eFatura/
--rw-r--r--   0 sancak    (1000) sancak    (1000)      785 2023-05-10 11:53:39.000000 eFatura-0.0.3/eFatura/Oturum.py
--rw-r--r--   0 sancak    (1000) sancak    (1000)     1343 2023-05-10 12:25:47.000000 eFatura-0.0.3/eFatura/__init__.py
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:31:40.567524 eFatura-0.0.3/eFatura.egg-info/
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2765 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 sancak    (1000) sancak    (1000)      222 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)        1 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)       53 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/requires.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)        8 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/top_level.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)       38 2023-05-10 12:31:40.570857 eFatura-0.0.3/setup.cfg
--rw-r--r--   0 sancak    (1000) sancak    (1000)     1158 2023-05-10 12:00:28.000000 eFatura-0.0.3/setup.py
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:37:13.304803 eFatura-0.0.4/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       27 2023-05-10 08:30:46.000000 eFatura-0.0.4/MANIFEST.in
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2772 2023-05-10 12:37:13.304803 eFatura-0.0.4/PKG-INFO
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2223 2023-05-10 12:36:54.000000 eFatura-0.0.4/README.md
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:37:13.304803 eFatura-0.0.4/eFatura/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)      785 2023-05-10 11:53:39.000000 eFatura-0.0.4/eFatura/Oturum.py
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     1430 2023-05-10 12:36:41.000000 eFatura-0.0.4/eFatura/__init__.py
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:37:13.304803 eFatura-0.0.4/eFatura.egg-info/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2772 2023-05-10 12:37:12.000000 eFatura-0.0.4/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 sancak    (1000) sancak    (1000)      222 2023-05-10 12:37:13.000000 eFatura-0.0.4/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)        1 2023-05-10 12:37:12.000000 eFatura-0.0.4/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       53 2023-05-10 12:37:12.000000 eFatura-0.0.4/eFatura.egg-info/requires.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)        8 2023-05-10 12:37:12.000000 eFatura-0.0.4/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       38 2023-05-10 12:37:13.304803 eFatura-0.0.4/setup.cfg
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     1158 2023-05-10 12:37:04.000000 eFatura-0.0.4/setup.py
```

### Comparing `eFatura-0.0.3/PKG-INFO` & `eFatura-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vergi Numarasından E-Fatura Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,15 +45,15 @@
 ## 📝 Kullanım
 
 ```python
 from eFatura import e_fatura
 
 print(e_fatura("11111111111")) # Vergi Numarası veya TC Kimlik Numarası
 
->> True | False
+>> True | False | None
 ```
 
 ## 📝 Proje Sahibi
 
 - ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
 
 ## 🌐 Telif Hakkı ve Lisans
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.3 Summary: Vergi NumarasÄ±ndan
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.4 Summary: Vergi NumarasÄ±ndan
 E-Fatura Sorgusu Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+
 Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown # ð E-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/
@@ -19,16 +19,16 @@
 (https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
 NumarasÄ±ndan E-Fatura Sorgusu* [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
 YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
 KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
-# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ``` ## ð Proje
-Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
+# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð
+Proje Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
 CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
 [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
 PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-
 Fatura_Sorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
 â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
 mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
 ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
```

### Comparing `eFatura-0.0.3/README.md` & `eFatura-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ## 📝 Kullanım
 
 ```python
 from eFatura import e_fatura
 
 print(e_fatura("11111111111")) # Vergi Numarası veya TC Kimlik Numarası
 
->> True | False
+>> True | False | None
 ```
 
 ## 📝 Proje Sahibi
 
 - ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
 
 ## 🌐 Telif Hakkı ve Lisans
```

#### html2text {}

```diff
@@ -12,17 +12,17 @@
 eFatura?logo=pypi&logoColor=white) *Vergi NumarasÄ±ndan E-Fatura Sorgusu* [!
 [ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
 python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
 ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
 keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
 GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
 eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ± veya
-TC Kimlik NumarasÄ± >> True | False ``` ## ð Proje Sahibi - â **[kmprens/
-CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð Telif HakkÄ±
-ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
+TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â **
+[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
+Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://
+github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29
+June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
 *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
 iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
 Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
 [âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi]
 (https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eFatura-0.0.3/eFatura/Oturum.py` & `eFatura-0.0.4/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.3/eFatura/__init__.py` & `eFatura-0.0.4/eFatura/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .Oturum     import legacy_session
 from shutil      import copyfileobj
 from uuid        import uuid4
 from os          import remove
 from PIL         import Image
 from pytesseract import image_to_string
 
-def e_fatura(vergi_numarasi:str) -> bool:
+def e_fatura(vergi_numarasi:str) -> bool | None:
     """Vergi Numarasından E-Fatura Kontrolü Sağlama"""
     captcha_resmi = f"captcha_{uuid4()}.jpg"
 
     while True:
         oturum = legacy_session()
         oturum.headers.update({
             "User-Agent" : "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"
@@ -27,8 +27,11 @@
         e_fatura_istek = oturum.post(
             url  = "https://sorgu.efatura.gov.tr/kullanicilar/xliste.php",
             data = {"search_string": f"{vergi_numarasi}", "captcha_code": f"{captcha_metni}", "submit": "Ara"}
         )
         if "Güvenlik kodu hatalı" in e_fatura_istek.text:
             continue
 
-        return "Mükellef kayıtlıdır." in e_fatura_istek.text
+        if "kayıt bulunamadı" in e_fatura_istek.text:
+            return None
+
+        return "Mükellef kayıtlıdır" in e_fatura_istek.text
```

### Comparing `eFatura-0.0.3/eFatura.egg-info/PKG-INFO` & `eFatura-0.0.4/eFatura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.3
+Version: 0.0.4
 Summary: Vergi Numarasından E-Fatura Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,15 +45,15 @@
 ## 📝 Kullanım
 
 ```python
 from eFatura import e_fatura
 
 print(e_fatura("11111111111")) # Vergi Numarası veya TC Kimlik Numarası
 
->> True | False
+>> True | False | None
 ```
 
 ## 📝 Proje Sahibi
 
 - ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
 
 ## 🌐 Telif Hakkı ve Lisans
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.3 Summary: Vergi NumarasÄ±ndan
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.4 Summary: Vergi NumarasÄ±ndan
 E-Fatura Sorgusu Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+
 Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown # ð E-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/
@@ -19,16 +19,16 @@
 (https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
 NumarasÄ±ndan E-Fatura Sorgusu* [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
 YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
 KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
-# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ``` ## ð Proje
-Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
+# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð
+Proje Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
 CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
 [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
 PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-
 Fatura_Sorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
 â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
 mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
 ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
```

### Comparing `eFatura-0.0.3/setup.py` & `eFatura-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["eFatura"],
 
     name         = "eFatura",
-    version      = "0.0.3",
+    version      = "0.0.4",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi Numarasından E-Fatura Sorgusu",
     keywords     = ["E-Fatura_Sorgu", "eFatura", "KekikAkademi", "keyiflerolsun"],
 
     long_description_content_type   = "text/markdown",
     long_description                = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data            = True,
```

