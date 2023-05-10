# Comparing `tmp/eFatura-0.1.1.tar.gz` & `tmp/eFatura-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-0.1.1.tar", last modified: Wed May 10 13:36:03 2023, max compression
+gzip compressed data, was "eFatura-0.1.2.tar", last modified: Wed May 10 13:39:25 2023, max compression
```

## Comparing `eFatura-0.1.1.tar` & `eFatura-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:36:03.300023 eFatura-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 13:35:43.000000 eFatura-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 13:36:03.296023 eFatura-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-10 13:35:43.000000 eFatura-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:36:03.296023 eFatura-0.1.1/eFatura/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 13:35:43.000000 eFatura-0.1.1/eFatura/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 13:35:43.000000 eFatura-0.1.1/eFatura/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:36:03.296023 eFatura-0.1.1/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:36:03.000000 eFatura-0.1.1/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:36:03.300023 eFatura-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 13:35:43.000000 eFatura-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:25.399128 eFatura-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 13:39:06.000000 eFatura-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-10 13:39:25.399128 eFatura-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-10 13:39:06.000000 eFatura-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:25.399128 eFatura-0.1.2/eFatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-10 13:39:06.000000 eFatura-0.1.2/eFatura/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 13:39:06.000000 eFatura-0.1.2/eFatura/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:25.399128 eFatura-0.1.2/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-10 13:39:25.000000 eFatura-0.1.2/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 13:39:25.000000 eFatura-0.1.2/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:39:25.000000 eFatura-0.1.2/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 13:39:25.000000 eFatura-0.1.2/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:39:25.000000 eFatura-0.1.2/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:39:25.399128 eFatura-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 13:39:06.000000 eFatura-0.1.2/setup.py
```

### Comparing `eFatura-0.1.1/PKG-INFO` & `eFatura-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.1.1
+Version: 0.1.2
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Mükellef Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,24 +14,25 @@
 Description-Content-Type: text/markdown
 
 # 🔍 E-Fatura Sorgu
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
-[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
+[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
+
 *Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.1.1 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.1.2 Summary: Vergi veya TC
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
-badge/âï¸-Kahve_Ismarla-ffdd00] [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
+badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
+pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
+img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
+img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
+[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
+- Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+eFatura?logo=pypi&logoColor=white) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
 //github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/
 badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/
-KekikFlow.yml) ![Python Version](https://img.shields.io/pypi/pyversions/
-eFatura?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
-eFatura?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
-eFatura?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
-pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white) ![PyPI - Wheel]
-(https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
-veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![ForTheBadge
-made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
-(https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
-GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
-eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ± veya
-TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â **
-[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
+KekikFlow.yml) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet
+Sorgusu* [![ForTheBadge made-with-python](https://ForTheBadge.com/images/
+badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge built-
+with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install
+eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python
+from eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ±
+veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â
+**[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
 Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://
 github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29
 June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
 *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
 iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
 Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
 [âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi]
```

### Comparing `eFatura-0.1.1/README.md` & `eFatura-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # 🔍 E-Fatura Sorgu
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
-[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
+[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
+
 *Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
 # ð E-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
 keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme]
 (https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/E-Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
+badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
+pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
+img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
+img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
+[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
+- Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+eFatura?logo=pypi&logoColor=white) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
 //github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/
 badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/
-KekikFlow.yml) ![Python Version](https://img.shields.io/pypi/pyversions/
-eFatura?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
-eFatura?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
-eFatura?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
-pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white) ![PyPI - Wheel]
-(https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
-veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![ForTheBadge
-made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
-(https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
-GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
-eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ± veya
-TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â **
-[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
+KekikFlow.yml) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet
+Sorgusu* [![ForTheBadge made-with-python](https://ForTheBadge.com/images/
+badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge built-
+with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install
+eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python
+from eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ±
+veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â
+**[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
 Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://
 github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29
 June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
 *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
 iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
 Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
 [âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi]
```

### Comparing `eFatura-0.1.1/eFatura/Oturum.py` & `eFatura-0.1.2/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.1.1/eFatura/__init__.py` & `eFatura-0.1.2/eFatura/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.1.1/eFatura.egg-info/PKG-INFO` & `eFatura-0.1.2/eFatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.1.1
+Version: 0.1.2
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Mükellef Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,24 +14,25 @@
 Description-Content-Type: text/markdown
 
 # 🔍 E-Fatura Sorgu
 
 ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white)
 ![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/E-Fatura_Sorgu&title=Görüntülenme)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
-[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
+[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml)
+
 *Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.1.1 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.1.2 Summary: Vergi veya TC
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
-badge/âï¸-Kahve_Ismarla-ffdd00] [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
+badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
+pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
+img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
+img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
+[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
+- Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+eFatura?logo=pypi&logoColor=white) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https:
 //github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/KekikFlow.yml/
 badge.svg)](https://github.com/keyiflerolsun/E-Fatura_Sorgu/actions/workflows/
-KekikFlow.yml) ![Python Version](https://img.shields.io/pypi/pyversions/
-eFatura?logo=python&logoColor=white) ![License](https://img.shields.io/pypi/l/
-eFatura?logo=gnu&logoColor=white) ![Status](https://img.shields.io/pypi/status/
-eFatura?logo=windowsterminal&logoColor=white) ![PyPI](https://img.shields.io/
-pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white) ![PyPI - Wheel]
-(https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white) *Vergi
-veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![ForTheBadge
-made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)]
-(https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install eFatura #
-GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python from
-eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ± veya
-TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â **
-[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
+KekikFlow.yml) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet
+Sorgusu* [![ForTheBadge made-with-python](https://ForTheBadge.com/images/
+badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge built-
+with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash # YÃ¼klemek pip install
+eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ```python
+from eFatura import e_fatura print(e_fatura("11111111111")) # Vergi NumarasÄ±
+veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð Proje Sahibi - â
+**[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð
 Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://
 github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29
 June 2007](https://github.com/keyiflerolsun/E-Fatura_Sorgu/blob/master/LICENSE)
 *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
 iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
 Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
 [âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** ## > **[@KekikAkademi]
```

### Comparing `eFatura-0.1.1/setup.py` & `eFatura-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["eFatura"],
 
     name         = "eFatura",
-    version      = "0.1.1",
+    version      = "0.1.2",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["Mükellef Sorgu", "eFatura", "KekikAkademi", "keyiflerolsun"],
 
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True,
```

