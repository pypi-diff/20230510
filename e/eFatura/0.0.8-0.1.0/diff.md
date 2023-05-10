# Comparing `tmp/eFatura-0.0.8.tar.gz` & `tmp/eFatura-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-0.0.8.tar", last modified: Wed May 10 13:16:52 2023, max compression
+gzip compressed data, was "eFatura-0.1.0.tar", last modified: Wed May 10 13:28:49 2023, max compression
```

## Comparing `eFatura-0.0.8.tar` & `eFatura-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:16:52.893552 eFatura-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 13:16:27.000000 eFatura-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-10 13:16:52.893552 eFatura-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-10 13:16:27.000000 eFatura-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:16:52.893552 eFatura-0.0.8/eFatura/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 13:16:27.000000 eFatura-0.0.8/eFatura/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 13:16:27.000000 eFatura-0.0.8/eFatura/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:16:52.893552 eFatura-0.0.8/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:16:52.000000 eFatura-0.0.8/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:16:52.893552 eFatura-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 13:16:27.000000 eFatura-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:28:49.114441 eFatura-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 13:28:31.000000 eFatura-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 13:28:49.114441 eFatura-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-10 13:28:31.000000 eFatura-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:28:49.114441 eFatura-0.1.0/eFatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 13:28:31.000000 eFatura-0.1.0/eFatura/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 13:28:31.000000 eFatura-0.1.0/eFatura/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:28:49.114441 eFatura-0.1.0/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:28:49.000000 eFatura-0.1.0/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:28:49.114441 eFatura-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 13:28:31.000000 eFatura-0.1.0/setup.py
```

### Comparing `eFatura-0.0.8/PKG-INFO` & `eFatura-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.8
+Version: 0.1.0
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Mükellef Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Description-Content-Type: text/markdown
 
 # 🔍 E-Fatura Sorgu
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
```

#### html2text {}

```diff
@@ -1,36 +1,39 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.8 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.1.0 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
 Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
 Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-
 Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
 hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/E-Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
-pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
-img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
-[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
-- Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-eFatura?logo=pypi&logoColor=white) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura
-MÃ¼kellefiyet Sorgusu* [![ForTheBadge made-with-python](https://
-ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
-YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
-KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
-# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð
-Proje Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
-CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-
-Fatura_Sorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+badge/âï¸-Kahve_Ismarla-ffdd00] [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
+//github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/
+badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/
+KekikFlow.yml) ![Python Version](https://img.shields.io/pypi/pyversions/
+eFatura?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
+eFatura?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
+eFatura?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
+pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white) ![PyPI - Wheel]
+(https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
+veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![ForTheBadge
+made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
+(https://www.python.org/) [![ForTheBadge built-with-love](https://
+ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
+keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
+GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
+eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ± veya
+TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â **
+[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
+Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://
+github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29
+June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi]
+(https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eFatura-0.0.8/README.md` & `eFatura-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # 🔍 E-Fatura Sorgu
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
```

#### html2text {}

```diff
@@ -1,28 +1,31 @@
 # ð E-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
 keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme]
 (https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/E-Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
-pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
-img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
-[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
-- Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-eFatura?logo=pypi&logoColor=white) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura
-MÃ¼kellefiyet Sorgusu* [![ForTheBadge made-with-python](https://
-ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
-YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
-KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
-# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð
-Proje Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
-CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-
-Fatura_Sorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+badge/âï¸-Kahve_Ismarla-ffdd00] [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
+//github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/
+badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/
+KekikFlow.yml) ![Python Version](https://img.shields.io/pypi/pyversions/
+eFatura?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
+eFatura?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
+eFatura?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
+pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white) ![PyPI - Wheel]
+(https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
+veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![ForTheBadge
+made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
+(https://www.python.org/) [![ForTheBadge built-with-love](https://
+ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
+keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
+GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
+eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ± veya
+TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â **
+[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
+Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://
+github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29
+June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi]
+(https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eFatura-0.0.8/eFatura/Oturum.py` & `eFatura-0.1.0/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.8/eFatura/__init__.py` & `eFatura-0.1.0/eFatura/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.8/eFatura.egg-info/PKG-INFO` & `eFatura-0.1.0/eFatura.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.8
+Version: 0.1.0
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Mükellef Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Description-Content-Type: text/markdown
 
 # 🔍 E-Fatura Sorgu
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
+[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
```

#### html2text {}

```diff
@@ -1,36 +1,39 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.8 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.1.0 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
 Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
 Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-
 Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
 hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/E-Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
-pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
-img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
-[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
-- Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-eFatura?logo=pypi&logoColor=white) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura
-MÃ¼kellefiyet Sorgusu* [![ForTheBadge made-with-python](https://
-ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
-YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
-KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
-# Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð
-Proje Sahibi - â **[kmprens/CheckEinvoice](https://github.com/kmprens/
-CheckEinvoice)** ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/E-
-Fatura_Sorgu/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ##
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+badge/âï¸-Kahve_Ismarla-ffdd00] [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
+//github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/
+badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/
+KekikFlow.yml) ![Python Version](https://img.shields.io/pypi/pyversions/
+eFatura?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
+eFatura?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
+eFatura?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
+pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white) ![PyPI - Wheel]
+(https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
+veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![ForTheBadge
+made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
+(https://www.python.org/) [![ForTheBadge built-with-love](https://
+ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
+keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
+GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
+eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ± veya
+TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â **
+[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
+Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://
+github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29
+June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi]
+(https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eFatura-0.0.8/setup.py` & `eFatura-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["eFatura"],
 
     name         = "eFatura",
-    version      = "0.0.8",
+    version      = "0.1.0",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["Mükellef Sorgu", "eFatura", "KekikAkademi", "keyiflerolsun"],
 
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True,
```

