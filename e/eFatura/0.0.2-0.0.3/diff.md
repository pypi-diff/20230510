# Comparing `tmp/eFatura-0.0.2.tar.gz` & `tmp/eFatura-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-0.0.2.tar", last modified: Tue May 24 01:54:00 2022, max compression
+gzip compressed data, was "eFatura-0.0.3.tar", last modified: Wed May 10 12:31:40 2023, max compression
```

## Comparing `eFatura-0.0.2.tar` & `eFatura-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,15 @@
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2022-05-24 01:54:00.817479 eFatura-0.0.2/
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2022-05-24 01:54:00.817479 eFatura-0.0.2/.github/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      111 2022-05-24 01:51:27.000000 eFatura-0.0.2/.github/FUNDING.yml
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1799 2022-05-24 01:51:05.000000 eFatura-0.0.2/.gitignore
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       27 2022-05-24 01:51:53.000000 eFatura-0.0.2/MANIFEST.in
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2571 2022-05-24 01:54:00.817479 eFatura-0.0.2/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2023 2022-05-24 01:51:05.000000 eFatura-0.0.2/README.md
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       48 2022-05-24 01:51:41.000000 eFatura-0.0.2/_config.yml
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2022-05-24 01:54:00.817479 eFatura-0.0.2/eFatura/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1351 2022-05-24 01:51:05.000000 eFatura-0.0.2/eFatura/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2022-05-24 01:54:00.817479 eFatura-0.0.2/eFatura.egg-info/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2571 2022-05-24 01:53:59.000000 eFatura-0.0.2/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      303 2022-05-24 01:53:59.000000 eFatura-0.0.2/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        1 2022-05-24 01:53:59.000000 eFatura-0.0.2/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       43 2022-05-24 01:53:59.000000 eFatura-0.0.2/eFatura.egg-info/requires.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        8 2022-05-24 01:53:59.000000 eFatura-0.0.2/eFatura.egg-info/top_level.txt
--rwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      152 2022-05-24 01:51:05.000000 eFatura-0.0.2/pyCacheTemizleyici.sh
--rwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      209 2022-05-24 01:51:05.000000 eFatura-0.0.2/pypiYukleyici.sh
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       42 2022-05-24 01:51:05.000000 eFatura-0.0.2/requirements.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       38 2022-05-24 01:54:00.817479 eFatura-0.0.2/setup.cfg
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1113 2022-05-24 01:52:07.000000 eFatura-0.0.2/setup.py
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:31:40.570857 eFatura-0.0.3/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       27 2023-05-10 08:30:46.000000 eFatura-0.0.3/MANIFEST.in
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2765 2023-05-10 12:31:40.567524 eFatura-0.0.3/PKG-INFO
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2216 2023-05-10 12:29:28.000000 eFatura-0.0.3/README.md
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:31:40.564191 eFatura-0.0.3/eFatura/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)      785 2023-05-10 11:53:39.000000 eFatura-0.0.3/eFatura/Oturum.py
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     1343 2023-05-10 12:25:47.000000 eFatura-0.0.3/eFatura/__init__.py
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:31:40.567524 eFatura-0.0.3/eFatura.egg-info/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2765 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 sancak    (1000) sancak    (1000)      222 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)        1 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       53 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/requires.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)        8 2023-05-10 12:31:40.000000 eFatura-0.0.3/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       38 2023-05-10 12:31:40.570857 eFatura-0.0.3/setup.cfg
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     1158 2023-05-10 12:00:28.000000 eFatura-0.0.3/setup.py
```

### Comparing `eFatura-0.0.2/PKG-INFO` & `eFatura-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.2
+Version: 0.0.3
 Summary: Vergi Numarasından E-Fatura Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🔍 E-Fatura Sorgu
 
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu)
-![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Profile%20Views)
-<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/%E2%98%95%EF%B8%8F-Kahve%20Ismarla-ffdd00" title="☕️" style="padding-left:5px;"></a>
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eFatura)
-![PyPI - Status](https://img.shields.io/pypi/status/eFatura)
-![PyPI](https://img.shields.io/pypi/v/eFatura)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura)
-![PyPI - License](https://img.shields.io/pypi/l/eFatura)
-
+![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
+![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
+<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+
+![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
+![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
+![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
+
+![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
 *Vergi Numarasından E-Fatura Sorgusu*
 
-[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
 pip install eFatura
 
@@ -43,31 +43,31 @@
 ```
 
 ## 📝 Kullanım
 
 ```python
 from eFatura import e_fatura
 
-print(e_fatura(11111111111)) # Vergi Numarası
+print(e_fatura("11111111111")) # Vergi Numarası veya TC Kimlik Numarası
 
->> True | False | None
+>> True | False
 ```
 
 ## 📝 Proje Sahibi
 
 - ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
 
 ## 🌐 Telif Hakkı ve Lisans
 
-* *Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
-* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/keyifUserBot/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
-*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/keyiflerolsun)
+*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ##
```

#### html2text {}

```diff
@@ -1,33 +1,35 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.2 Summary: Vergi NumarasÄ±ndan
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.3 Summary: Vergi NumarasÄ±ndan
 E-Fatura Sorgusu Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+
 Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/
+Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown # ð E-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/
-repo-size/keyiflerolsun/E-Fatura_Sorgu) ![GÃ¶rÃ¼ntÃ¼lenme](https://
-hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/E-Fatura_Sorgu&title=Profile%20Views) [https://img.shields.io/
-badge/%E2%98%95%EF%B8%8F-Kahve%20Ismarla-ffdd00] ![PyPI - Python Version]
-(https://img.shields.io/pypi/pyversions/eFatura) ![PyPI - Status](https://
-img.shields.io/pypi/status/eFatura) ![PyPI](https://img.shields.io/pypi/v/
-eFatura) ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura) ![PyPI -
-Wheel](https://img.shields.io/pypi/wheel/eFatura) ![PyPI - License](https://
-img.shields.io/pypi/l/eFatura) *Vergi NumarasÄ±ndan E-Fatura Sorgusu* [!
-[forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](http://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
-GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
-eFatura import e_fatura print(e_fatura(11111111111)) # Vergi NumarasÄ± >> True
-| False | None ``` ## ð Proje Sahibi - â **[kmprens/CheckEinvoice](https:/
-/github.com/kmprens/CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans *
-*Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun)
-â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://
-github.com/keyiflerolsun/keyifUserBot/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
-lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/keyiflerolsun) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla]
-(https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi](https://t.me/
-KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white) !
+[GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https://github.com/keyiflerolsun/E-
+Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/âï¸-Kahve
+Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/pyversions/
+eFatura?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
+eFatura?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
+eFatura?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
+pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white) ![PyPI - Wheel]
+(https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
+NumarasÄ±ndan E-Fatura Sorgusu* [![ForTheBadge made-with-python](https://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
+YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
+KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
+# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ``` ## ð Proje
+Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
+CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-
+Fatura_Sorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eFatura-0.0.2/README.md` & `eFatura-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # 🔍 E-Fatura Sorgu
 
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu)
-![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Profile%20Views)
-<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/%E2%98%95%EF%B8%8F-Kahve%20Ismarla-ffdd00" title="☕️" style="padding-left:5px;"></a>
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eFatura)
-![PyPI - Status](https://img.shields.io/pypi/status/eFatura)
-![PyPI](https://img.shields.io/pypi/v/eFatura)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura)
-![PyPI - License](https://img.shields.io/pypi/l/eFatura)
-
+![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
+![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
+<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+
+![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
+![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
+![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
+
+![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
 *Vergi Numarasından E-Fatura Sorgusu*
 
-[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
 pip install eFatura
 
@@ -28,31 +28,31 @@
 ```
 
 ## 📝 Kullanım
 
 ```python
 from eFatura import e_fatura
 
-print(e_fatura(11111111111)) # Vergi Numarası
+print(e_fatura("11111111111")) # Vergi Numarası veya TC Kimlik Numarası
 
->> True | False | None
+>> True | False
 ```
 
 ## 📝 Proje Sahibi
 
 - ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
 
 ## 🌐 Telif Hakkı ve Lisans
 
-* *Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
-* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/keyifUserBot/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
-*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/keyiflerolsun)
+*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ##
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
 # ð E-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
-keyiflerolsun/E-Fatura_Sorgu) ![GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/
-api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-
-Fatura_Sorgu&title=Profile%20Views) [https://img.shields.io/badge/
-%E2%98%95%EF%B8%8F-Kahve%20Ismarla-ffdd00] ![PyPI - Python Version](https://
-img.shields.io/pypi/pyversions/eFatura) ![PyPI - Status](https://
-img.shields.io/pypi/status/eFatura) ![PyPI](https://img.shields.io/pypi/v/
-eFatura) ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura) ![PyPI -
-Wheel](https://img.shields.io/pypi/wheel/eFatura) ![PyPI - License](https://
-img.shields.io/pypi/l/eFatura) *Vergi NumarasÄ±ndan E-Fatura Sorgusu* [!
-[forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](http://
+keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme]
+(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+keyiflerolsun/E-Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/
+badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
+pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
+img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
+img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
+[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
+- Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+eFatura?logo=pypi&logoColor=white) *Vergi NumarasÄ±ndan E-Fatura Sorgusu* [!
+[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
+python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
 ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
 keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
 GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
-eFatura import e_fatura print(e_fatura(11111111111)) # Vergi NumarasÄ± >> True
-| False | None ``` ## ð Proje Sahibi - â **[kmprens/CheckEinvoice](https:/
-/github.com/kmprens/CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans *
-*Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun)
-â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://
-github.com/keyiflerolsun/keyifUserBot/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
-lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/keyiflerolsun) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla]
-(https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi](https://t.me/
-KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ± veya
+TC Kimlik NumarasÄ± >> True | False ``` ## ð Proje Sahibi - â **[kmprens/
+CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð Telif HakkÄ±
+ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
+(https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi]
+(https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eFatura-0.0.2/eFatura/__init__.py` & `eFatura-0.0.3/eFatura/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-# https://ebelge.gib.gov.tr/efaturakayitlikullanicilar.html
+# Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
-from requests    import Session
+from .Oturum     import legacy_session
 from shutil      import copyfileobj
 from uuid        import uuid4
 from os          import remove
-from bs4         import BeautifulSoup
 from PIL         import Image
 from pytesseract import image_to_string
 
-def e_fatura(vergi_numarasi:str | int) -> bool | None:
+def e_fatura(vergi_numarasi:str) -> bool:
     """Vergi Numarasından E-Fatura Kontrolü Sağlama"""
     captcha_resmi = f"captcha_{uuid4()}.jpg"
 
-    oturum = Session()
+    while True:
+        oturum = legacy_session()
+        oturum.headers.update({
+            "User-Agent" : "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"
+        })
+
+        captcha_istek = oturum.get("https://sorgu.efatura.gov.tr/kullanicilar/img.php", stream=True)
+        with open(captcha_resmi, "wb") as dosya:
+            copyfileobj(captcha_istek.raw, dosya)
+
+        captcha_metni = image_to_string(Image.open(captcha_resmi)).strip()
+        remove(captcha_resmi)
+
+        e_fatura_istek = oturum.post(
+            url  = "https://sorgu.efatura.gov.tr/kullanicilar/xliste.php",
+            data = {"search_string": f"{vergi_numarasi}", "captcha_code": f"{captcha_metni}", "submit": "Ara"}
+        )
+        if "Güvenlik kodu hatalı" in e_fatura_istek.text:
+            continue
 
-    captcha_istek = oturum.get("https://sorgu.efatura.gov.tr/kullanicilar/img.php", stream=True)
-    with open(captcha_resmi, "wb") as file:
-        copyfileobj(captcha_istek.raw, file)
-
-    captcha_metni = image_to_string(Image.open(captcha_resmi))
-    remove(captcha_resmi)
-
-    e_fatura_istek = oturum.post(
-        url     = "https://sorgu.efatura.gov.tr/kullanicilar/xliste.php",
-        headers = {"User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/101.0.4951.67 Safari/537.36"},
-        data    = {"search_string": f"{vergi_numarasi}", "captcha_code": f"{captcha_metni}"}
-    )
-
-    corba = BeautifulSoup(e_fatura_istek.text, features="html.parser")
-
-    if corba.find("p", attrs={"style": "color:red;font-weight:bold"}):
-        return False
-    elif corba.find("div"):
-        return True
-    else:
-        return None
+        return "Mükellef kayıtlıdır." in e_fatura_istek.text
```

### Comparing `eFatura-0.0.2/eFatura.egg-info/PKG-INFO` & `eFatura-0.0.3/eFatura.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.2
+Version: 0.0.3
 Summary: Vergi Numarasından E-Fatura Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🔍 E-Fatura Sorgu
 
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu)
-![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Profile%20Views)
-<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/%E2%98%95%EF%B8%8F-Kahve%20Ismarla-ffdd00" title="☕️" style="padding-left:5px;"></a>
-
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eFatura)
-![PyPI - Status](https://img.shields.io/pypi/status/eFatura)
-![PyPI](https://img.shields.io/pypi/v/eFatura)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura)
-![PyPI - License](https://img.shields.io/pypi/l/eFatura)
-
+![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
+![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
+<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+
+![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
+![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
+![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
+
+![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
 *Vergi Numarasından E-Fatura Sorgusu*
 
-[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
 # Yüklemek
 pip install eFatura
 
@@ -43,31 +43,31 @@
 ```
 
 ## 📝 Kullanım
 
 ```python
 from eFatura import e_fatura
 
-print(e_fatura(11111111111)) # Vergi Numarası
+print(e_fatura("11111111111")) # Vergi Numarası veya TC Kimlik Numarası
 
->> True | False | None
+>> True | False
 ```
 
 ## 📝 Proje Sahibi
 
 - ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
 
 ## 🌐 Telif Hakkı ve Lisans
 
-* *Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
-* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/keyifUserBot/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
+* *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
+* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
-*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/keyiflerolsun)
+*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ##
```

#### html2text {}

```diff
@@ -1,33 +1,35 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.2 Summary: Vergi NumarasÄ±ndan
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.3 Summary: Vergi NumarasÄ±ndan
 E-Fatura Sorgusu Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com License: GPLv3+
 Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/
+Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown # ð E-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/
-repo-size/keyiflerolsun/E-Fatura_Sorgu) ![GÃ¶rÃ¼ntÃ¼lenme](https://
-hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/E-Fatura_Sorgu&title=Profile%20Views) [https://img.shields.io/
-badge/%E2%98%95%EF%B8%8F-Kahve%20Ismarla-ffdd00] ![PyPI - Python Version]
-(https://img.shields.io/pypi/pyversions/eFatura) ![PyPI - Status](https://
-img.shields.io/pypi/status/eFatura) ![PyPI](https://img.shields.io/pypi/v/
-eFatura) ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura) ![PyPI -
-Wheel](https://img.shields.io/pypi/wheel/eFatura) ![PyPI - License](https://
-img.shields.io/pypi/l/eFatura) *Vergi NumarasÄ±ndan E-Fatura Sorgusu* [!
-[forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](http://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
-GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
-eFatura import e_fatura print(e_fatura(11111111111)) # Vergi NumarasÄ± >> True
-| False | None ``` ## ð Proje Sahibi - â **[kmprens/CheckEinvoice](https:/
-/github.com/kmprens/CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans *
-*Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun)
-â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://
-github.com/keyiflerolsun/keyifUserBot/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
-lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
-isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
-(https://t.me/keyiflerolsun) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla]
-(https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi](https://t.me/
-KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white) !
+[GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https://github.com/keyiflerolsun/E-
+Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/âï¸-Kahve
+Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/pyversions/
+eFatura?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
+eFatura?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
+eFatura?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
+pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white) ![PyPI - Wheel]
+(https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
+NumarasÄ±ndan E-Fatura Sorgusu* [![ForTheBadge made-with-python](https://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
+[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
+YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
+KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
+# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ``` ## ð Proje
+Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
+CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-
+Fatura_Sorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

