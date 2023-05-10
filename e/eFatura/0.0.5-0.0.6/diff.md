# Comparing `tmp/eFatura-0.0.5.tar.gz` & `tmp/eFatura-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-0.0.5.tar", last modified: Wed May 10 12:39:31 2023, max compression
+gzip compressed data, was "eFatura-0.0.6.tar", last modified: Wed May 10 12:42:57 2023, max compression
```

## Comparing `eFatura-0.0.5.tar` & `eFatura-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:39:31.685209 eFatura-0.0.5/
--rw-r--r--   0 sancak    (1000) sancak    (1000)       27 2023-05-10 08:30:46.000000 eFatura-0.0.5/MANIFEST.in
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2826 2023-05-10 12:39:31.685209 eFatura-0.0.5/PKG-INFO
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2250 2023-05-10 12:39:01.000000 eFatura-0.0.5/README.md
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:39:31.681876 eFatura-0.0.5/eFatura/
--rw-r--r--   0 sancak    (1000) sancak    (1000)      785 2023-05-10 11:53:39.000000 eFatura-0.0.5/eFatura/Oturum.py
--rw-r--r--   0 sancak    (1000) sancak    (1000)     1446 2023-05-10 12:39:23.000000 eFatura-0.0.5/eFatura/__init__.py
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:39:31.685209 eFatura-0.0.5/eFatura.egg-info/
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2826 2023-05-10 12:39:31.000000 eFatura-0.0.5/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 sancak    (1000) sancak    (1000)      222 2023-05-10 12:39:31.000000 eFatura-0.0.5/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)        1 2023-05-10 12:39:31.000000 eFatura-0.0.5/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)       53 2023-05-10 12:39:31.000000 eFatura-0.0.5/eFatura.egg-info/requires.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)        8 2023-05-10 12:39:31.000000 eFatura-0.0.5/eFatura.egg-info/top_level.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)       38 2023-05-10 12:39:31.685209 eFatura-0.0.5/setup.cfg
--rw-r--r--   0 sancak    (1000) sancak    (1000)     1185 2023-05-10 12:39:09.000000 eFatura-0.0.5/setup.py
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:42:57.053460 eFatura-0.0.6/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       27 2023-05-10 08:30:46.000000 eFatura-0.0.6/MANIFEST.in
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2831 2023-05-10 12:42:57.053460 eFatura-0.0.6/PKG-INFO
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2252 2023-05-10 12:42:19.000000 eFatura-0.0.6/README.md
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:42:57.050127 eFatura-0.0.6/eFatura/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)      785 2023-05-10 11:53:39.000000 eFatura-0.0.6/eFatura/Oturum.py
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     1448 2023-05-10 12:42:19.000000 eFatura-0.0.6/eFatura/__init__.py
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:42:57.053460 eFatura-0.0.6/eFatura.egg-info/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2831 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 sancak    (1000) sancak    (1000)      222 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)        1 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       53 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/requires.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)        8 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       38 2023-05-10 12:42:57.053460 eFatura-0.0.6/setup.cfg
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     1188 2023-05-10 12:42:38.000000 eFatura-0.0.6/setup.py
```

### Comparing `eFatura-0.0.5/PKG-INFO` & `eFatura-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.5
-Summary: Vergi ve TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
+Version: 0.0.6
+Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
-Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun
+Keywords: Mükellef Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🔍 E-Fatura Sorgu
@@ -23,15 +23,15 @@
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
-*Vergi ve TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
+*Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.5 Summary: Vergi ve TC Kimlik
-NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://github.com/
-keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
-keyiflerolsun@gmail.com License: GPLv3+ Keywords: E-
-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: GNU General
-Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
-:: 3 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-
-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
-keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme]
-(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.6 Summary: Vergi veya TC
+Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
+github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
+keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
+Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
+Production/Stable Classifier: License :: OSI Approved :: GNU General Public
+License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
+Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-
+Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
+hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/E-Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/
 badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
 pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
 img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
 img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
 [PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-eFatura?logo=pypi&logoColor=white) *Vergi ve TC Kimlik NumarasÄ±ndan E-Fatura
+eFatura?logo=pypi&logoColor=white) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura
 MÃ¼kellefiyet Sorgusu* [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
 YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
 KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
 # Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð
```

### Comparing `eFatura-0.0.5/README.md` & `eFatura-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
-*Vergi ve TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
+*Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
 pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
 img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
 img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
 [PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-eFatura?logo=pypi&logoColor=white) *Vergi ve TC Kimlik NumarasÄ±ndan E-Fatura
+eFatura?logo=pypi&logoColor=white) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura
 MÃ¼kellefiyet Sorgusu* [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
 YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
 KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
 # Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð
```

### Comparing `eFatura-0.0.5/eFatura/Oturum.py` & `eFatura-0.0.6/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.5/eFatura/__init__.py` & `eFatura-0.0.6/eFatura/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from shutil      import copyfileobj
 from uuid        import uuid4
 from os          import remove
 from PIL         import Image
 from pytesseract import image_to_string
 
 def e_fatura(vergi_numarasi:str) -> bool | None:
-    """Vergi ve TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu"""
+    """Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu"""
     captcha_resmi = f"captcha_{uuid4()}.jpg"
 
     while True:
         oturum = legacy_session()
         oturum.headers.update({
             "User-Agent" : "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"
         })
```

### Comparing `eFatura-0.0.5/eFatura.egg-info/PKG-INFO` & `eFatura-0.0.6/eFatura.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.5
-Summary: Vergi ve TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
+Version: 0.0.6
+Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
-Keywords: E-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun
+Keywords: Mükellef Sorgu,eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 🔍 E-Fatura Sorgu
@@ -23,15 +23,15 @@
 ![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
 ![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
 
 ![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)
 
-*Vergi ve TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
+*Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
 ```bash
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.5 Summary: Vergi ve TC Kimlik
-NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://github.com/
-keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
-keyiflerolsun@gmail.com License: GPLv3+ Keywords: E-
-Fatura_Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status
-:: 5 - Production/Stable Classifier: License :: OSI Approved :: GNU General
-Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
-:: 3 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-
-Fatura Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/
-keyiflerolsun/E-Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme]
-(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.6 Summary: Vergi veya TC
+Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
+github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
+keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
+Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
+Production/Stable Classifier: License :: OSI Approved :: GNU General Public
+License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
+Sorgu ![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/E-
+Fatura_Sorgu?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
+hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
 keyiflerolsun/E-Fatura_Sorgu&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/
 badge/âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/
 pypi/pyversions/eFatura?logo=python&logoColor=white) ![License](https://
 img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
 img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) !
 [PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white) ![PyPI
 - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/
-eFatura?logo=pypi&logoColor=white) *Vergi ve TC Kimlik NumarasÄ±ndan E-Fatura
+eFatura?logo=pypi&logoColor=white) *Vergi veya TC Kimlik NumarasÄ±ndan E-Fatura
 MÃ¼kellefiyet Sorgusu* [![ForTheBadge made-with-python](https://
 ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
 with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Kurulum ```bash #
 YÃ¼klemek pip install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð
 KullanÄ±m ```python from eFatura import e_fatura print(e_fatura("11111111111"))
 # Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False | None ``` ## ð
```

### Comparing `eFatura-0.0.5/setup.py` & `eFatura-0.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["eFatura"],
 
     name         = "eFatura",
-    version      = "0.0.5",
+    version      = "0.0.6",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
-    description  = "Vergi ve TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
-    keywords     = ["E-Fatura_Sorgu", "eFatura", "KekikAkademi", "keyiflerolsun"],
+    description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
+    keywords     = ["Mükellef Sorgu", "eFatura", "KekikAkademi", "keyiflerolsun"],
 
     long_description_content_type   = "text/markdown",
     long_description                = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data            = True,
 
     license     = "GPLv3+",
     classifiers = [
```

