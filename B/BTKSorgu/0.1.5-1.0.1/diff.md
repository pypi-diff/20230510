# Comparing `tmp/BTKSorgu-0.1.5.tar.gz` & `tmp/BTKSorgu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTKSorgu-0.1.5.tar", last modified: Sun Jul  4 10:56:08 2021, max compression
+gzip compressed data, was "BTKSorgu-1.0.1.tar", last modified: Wed May 10 18:28:02 2023, max compression
```

## Comparing `BTKSorgu-0.1.5.tar` & `BTKSorgu-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2021-07-04 10:56:08.141203 BTKSorgu-0.1.5/
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2021-07-04 10:56:08.134536 BTKSorgu-0.1.5/BTKSorgu/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     3176 2021-07-04 10:51:09.000000 BTKSorgu-0.1.5/BTKSorgu/Erisim_Engeli.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     4284 2021-07-04 10:55:24.000000 BTKSorgu-0.1.5/BTKSorgu/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2021-07-04 10:56:08.137869 BTKSorgu-0.1.5/BTKSorgu.egg-info/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     4816 2021-07-04 10:56:07.000000 BTKSorgu-0.1.5/BTKSorgu.egg-info/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      232 2021-07-04 10:56:07.000000 BTKSorgu-0.1.5/BTKSorgu.egg-info/SOURCES.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        1 2021-07-04 10:56:07.000000 BTKSorgu-0.1.5/BTKSorgu.egg-info/dependency_links.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       35 2021-07-04 10:56:07.000000 BTKSorgu-0.1.5/BTKSorgu.egg-info/requires.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        9 2021-07-04 10:56:07.000000 BTKSorgu-0.1.5/BTKSorgu.egg-info/top_level.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    35149 2021-07-04 10:51:09.000000 BTKSorgu-0.1.5/LICENSE
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     4816 2021-07-04 10:56:08.137869 BTKSorgu-0.1.5/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     4225 2021-07-04 10:51:09.000000 BTKSorgu-0.1.5/README.md
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       38 2021-07-04 10:56:08.141203 BTKSorgu-0.1.5/setup.cfg
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1109 2021-07-04 10:54:07.000000 BTKSorgu-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/BTKSorgu/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/BTKSorgu/Erisim_Engeli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/BTKSorgu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/BTKSorgu/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/BTKSorgu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 18:28:02.000000 BTKSorgu-1.0.1/BTKSorgu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:28:02.436343 BTKSorgu-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-10 18:27:40.000000 BTKSorgu-1.0.1/setup.py
```

### Comparing `BTKSorgu-0.1.5/BTKSorgu/Erisim_Engeli.py` & `BTKSorgu-1.0.1/BTKSorgu/Erisim_Engeli.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,90 +2,92 @@
 
 from requests import Session
 from parsel   import Selector
 
 from shutil      import copyfileobj
 from pytesseract import image_to_string 
 from PIL         import Image
+from re          import search
 
 from os import remove
 
 class BTKSorgu(object):
     """
     BTKSorgu : Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu
 
     Dönüş
     ----------
         (str):
             {domain}, {karar} Karar Bulunamadı.
     """
     def __init__(self, sorgu_url:str, arka_plan:bool=False):
-        "Karar Döndürür"
-        self.arka_plan     = arka_plan
-        self.ana_sayfa     = "https://internet2.btk.gov.tr"
-        self.sorgu_sayfasi = "https://internet2.btk.gov.tr/sitesorgu/"
-        self.sorgu_url     = sorgu_url
+        """Karar Döndürür"""
+        self.arka_plan      = arka_plan
+        self.ana_sayfa      = "https://internet2.btk.gov.tr"
+        self.sorgu_sayfasi  = "https://internet2.btk.gov.tr/sitesorgu/"
+        self.sorgu_url      = search(r"(?:https?://)?(?:www\.)?([^/]+)", sorgu_url).group(1)
+        self._gecici_gorsel = "captcha.png"
 
         self.oturum = Session()
 
     @property
     def captcha_ver(self):
-        "Captcha görselini indirip OCR ile okur"
+        """Captcha görselini indirip OCR ile okur"""
         ilk_bakis    = self.oturum.get(self.sorgu_sayfasi, allow_redirects=True)
         captcha_yolu = Selector(ilk_bakis.text).xpath("//div[@class='arama_captcha']/img/@src").get()
 
         captcha_data = self.oturum.get(f"{self.ana_sayfa}{captcha_yolu}", stream=True)
-        with open('captcha.png', 'wb') as captcha_gorsel:
+        with open(self._gecici_gorsel, "wb") as captcha_gorsel:
             copyfileobj(captcha_data.raw, captcha_gorsel)
 
-        return image_to_string(Image.open('captcha.png')).strip().replace(' ', '')
+        return image_to_string(Image.open(self._gecici_gorsel)).strip().replace(" ", "")
 
     @property
     def karar(self):
-        "Captcha ile birlikte sorgu sitesini POST eder"
+        """Captcha ile birlikte sorgu sitesini POST eder"""
         captcha = self.captcha_ver
 
-        payload = {
-            "deger"             : self.sorgu_url,
-            "ipw"               : '',
-            "kat"               : '',
-            "tr"                : '',
-            "eg"                : '',
-            "ayrintili"         : 0,
-            "submit"            : "Sorgula",
-            "security_code"     : captcha
-        }
-
-        kimlik = {
-            "Content-Type"             : "application/x-www-form-urlencoded",
-            "Host"                     : "internet2.btk.gov.tr",
-            "Origin"                   : self.ana_sayfa,
-            "Referer"                  : self.sorgu_sayfasi,
-        }
-
-        karar_sayfasi = self.oturum.post(self.sorgu_sayfasi, headers=kimlik, data=payload)
+        karar_sayfasi = self.oturum.post(
+            url     = self.sorgu_sayfasi,
+            headers = {
+                "Content-Type" : "application/x-www-form-urlencoded",
+                "Host"         : "internet2.btk.gov.tr",
+                "Origin"       : self.ana_sayfa,
+                "Referer"      : self.sorgu_sayfasi,
+            },
+            data    = {
+                "deger"         : self.sorgu_url,
+                "ipw"           : "",
+                "kat"           : "",
+                "tr"            : "",
+                "eg"            : "",
+                "ayrintili"     : 0,
+                "submit"        : "Sorgula",
+                "security_code" : captcha
+            }
+        )
 
         # print(karar_sayfasi.text)
         secici     = Selector(karar_sayfasi.text)
         hatali_kod = secici.xpath("//div[@class='icerik']/ul/li/text()").get()
         erisim_var = secici.xpath("//div[@class='yazi2']/text()").get()
         erisim_yok = secici.xpath("//span[@class='yazi2_2']/text()").get()
-        karar  = hatali_kod or erisim_var or erisim_yok or ''
+        karar      = hatali_kod or erisim_var or erisim_yok or ""
 
         if self.arka_plan:
             print(f"""
 
             # Sorgu   : {self.sorgu_url}
             # Captcha : {captcha}
             # Karar   : {karar}
 
 """)
         return karar
 
     def __repr__(self) -> str:
-        "Kararı Döndürür"
-        hatalar = ['Lütfen güvenlik kodunu giriniz.', 'Güvenlik kodunu yanlış girdiniz. Lütfen Güvenlik Kodunu resimde gördüğünüz şekilde giriniz.']
+        """Kararı Döndürür"""
+        hatalar = ["Lütfen güvenlik kodunu giriniz.", "Güvenlik kodunu yanlış girdiniz. Lütfen Güvenlik Kodunu resimde gördüğünüz şekilde giriniz."]
         while True:
             karar = self.karar
             if karar not in hatalar:
-                remove('captcha.png')
-                return karar
+                remove(self._gecici_gorsel)
+                return karar
```

### Comparing `BTKSorgu-0.1.5/BTKSorgu/__init__.py` & `BTKSorgu-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,268 +1,280 @@
-00000000: 7227 2727 0a23 20f0 9f94 8d20 4254 4b53  r'''.# .... BTKS
-00000010: 6f72 6775 0a0a 5b21 5b43 6f64 6163 7920  orgu..[![Codacy 
-00000020: 4261 6467 655d 2868 7474 7073 3a2f 2f61  Badge](https://a
-00000030: 7070 2e63 6f64 6163 792e 636f 6d2f 7072  pp.codacy.com/pr
-00000040: 6f6a 6563 742f 6261 6467 652f 4772 6164  oject/badge/Grad
-00000050: 652f 6263 3061 3532 6139 6235 3766 3463  e/bc0a52a9b57f4c
-00000060: 3239 3933 3063 6264 3663 3739 3666 3961  29930cbd6c796f9a
-00000070: 3862 295d 2868 7474 7073 3a2f 2f77 7777  8b)](https://www
-00000080: 2e63 6f64 6163 792e 636f 6d2f 6768 2f6b  .codacy.com/gh/k
-00000090: 6579 6966 6c65 726f 6c73 756e 2f42 544b  eyiflerolsun/BTK
-000000a0: 536f 7267 752f 6461 7368 626f 6172 643f  Sorgu/dashboard?
-000000b0: 7574 6d5f 736f 7572 6365 3d67 6974 6875  utm_source=githu
-000000c0: 622e 636f 6d26 616d 703b 7574 6d5f 6d65  b.com&amp;utm_me
-000000d0: 6469 756d 3d72 6566 6572 7261 6c26 616d  dium=referral&am
-000000e0: 703b 7574 6d5f 636f 6e74 656e 743d 6b65  p;utm_content=ke
-000000f0: 7969 666c 6572 6f6c 7375 6e2f 4254 4b53  yiflerolsun/BTKS
-00000100: 6f72 6775 2661 6d70 3b75 746d 5f63 616d  orgu&amp;utm_cam
-00000110: 7061 6967 6e3d 4261 6467 655f 4772 6164  paign=Badge_Grad
-00000120: 6529 2021 5b52 6570 6f20 426f 7975 7475  e) ![Repo Boyutu
-00000130: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000140: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00000150: 7265 706f 2d73 697a 652f 6b65 7969 666c  repo-size/keyifl
-00000160: 6572 6f6c 7375 6e2f 4254 4b53 6f72 6775  erolsun/BTKSorgu
-00000170: 2920 215b 5669 6577 735d 2868 7474 7073  ) ![Views](https
-00000180: 3a2f 2f68 6974 732e 7365 6579 6f75 6661  ://hits.seeyoufa
-00000190: 726d 2e63 6f6d 2f61 7069 2f63 6f75 6e74  rm.com/api/count
-000001a0: 2f69 6e63 722f 6261 6467 652e 7376 673f  /incr/badge.svg?
-000001b0: 7572 6c3d 6874 7470 733a 2f2f 6769 7468  url=https://gith
-000001c0: 7562 2e63 6f6d 2f6b 6579 6966 6c65 726f  ub.com/keyiflero
-000001d0: 6c73 756e 2f42 544b 536f 7267 7526 7469  lsun/BTKSorgu&ti
-000001e0: 746c 653d 5072 6f66 696c 6525 3230 5669  tle=Profile%20Vi
-000001f0: 6577 7329 205b 215b 4769 7470 6f64 2072  ews) [![Gitpod r
-00000200: 6561 6479 2d74 6f2d 636f 6465 5d28 6874  eady-to-code](ht
-00000210: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000220: 732e 696f 2f62 6164 6765 2f47 6974 706f  s.io/badge/Gitpo
-00000230: 642d 7265 6164 792d 2d74 6f2d 2d63 6f64  d-ready--to--cod
-00000240: 652d 626c 7565 3f6c 6f67 6f3d 6769 7470  e-blue?logo=gitp
-00000250: 6f64 295d 2868 7474 7073 3a2f 2f67 6974  od)](https://git
-00000260: 706f 642e 696f 2f23 6874 7470 733a 2f2f  pod.io/#https://
-00000270: 6769 7468 7562 2e63 6f6d 2f6b 6579 6966  github.com/keyif
-00000280: 6c65 726f 6c73 756e 2f42 544b 536f 7267  lerolsun/BTKSorg
-00000290: 7529 0a0a 215b 5079 5049 202d 2050 7974  u)..![PyPI - Pyt
-000002a0: 686f 6e20 5665 7273 696f 6e5d 2868 7474  hon Version](htt
-000002b0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000002c0: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-000002d0: 6f6e 732f 4254 4b53 6f72 6775 290a 215b  ons/BTKSorgu).![
-000002e0: 5079 5049 202d 2053 7461 7475 735d 2868  PyPI - Status](h
-000002f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000300: 6473 2e69 6f2f 7079 7069 2f73 7461 7475  ds.io/pypi/statu
-00000310: 732f 4254 4b53 6f72 6775 290a 215b 5079  s/BTKSorgu).![Py
-00000320: 5049 5d28 6874 7470 733a 2f2f 696d 672e  PI](https://img.
-00000330: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000340: 762f 4254 4b53 6f72 6775 290a 215b 5079  v/BTKSorgu).![Py
-00000350: 5049 202d 2044 6f77 6e6c 6f61 6473 5d28  PI - Downloads](
-00000360: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000370: 6c64 732e 696f 2f70 7970 692f 646d 2f42  lds.io/pypi/dm/B
-00000380: 544b 536f 7267 7529 0a21 5b50 7950 4920  TKSorgu).![PyPI 
-00000390: 2d20 5768 6565 6c5d 2868 7474 7073 3a2f  - Wheel](https:/
-000003a0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000003b0: 7079 7069 2f77 6865 656c 2f42 544b 536f  pypi/wheel/BTKSo
-000003c0: 7267 7529 0a21 5b50 7950 4920 2d20 4c69  rgu).![PyPI - Li
-000003d0: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
-000003e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000003f0: 7069 2f6c 2f42 544b 536f 7267 7529 0a0a  pi/l/BTKSorgu)..
-00000400: 2a48 6564 6566 2077 6562 7369 7465 7369  *Hedef websitesi
-00000410: 6e69 6e20 4254 4b20 5461 7261 66c4 b16e  nin BTK Taraf..n
-00000420: 6461 6e20 4572 69c5 9f69 6d20 456e 6765  dan Eri..im Enge
-00000430: 6c69 2053 6f72 6775 7375 2e2e 2a0a 0a5b  li Sorgusu..*..[
-00000440: 215b 666f 7274 6865 6261 6467 6520 6d61  ![forthebadge ma
-00000450: 6465 2d77 6974 682d 7079 7468 6f6e 5d28  de-with-python](
-00000460: 6874 7470 3a2f 2f46 6f72 5468 6542 6164  http://ForTheBad
-00000470: 6765 2e63 6f6d 2f69 6d61 6765 732f 6261  ge.com/images/ba
-00000480: 6467 6573 2f6d 6164 652d 7769 7468 2d70  dges/made-with-p
-00000490: 7974 686f 6e2e 7376 6729 5d28 6874 7470  ython.svg)](http
-000004a0: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
-000004b0: 7267 2f29 0a5b 215b 466f 7254 6865 4261  rg/).[![ForTheBa
-000004c0: 6467 6520 6275 696c 742d 7769 7468 2d6c  dge built-with-l
-000004d0: 6f76 655d 2868 7474 703a 2f2f 466f 7254  ove](http://ForT
-000004e0: 6865 4261 6467 652e 636f 6d2f 696d 6167  heBadge.com/imag
-000004f0: 6573 2f62 6164 6765 732f 6275 696c 742d  es/badges/built-
-00000500: 7769 7468 2d6c 6f76 652e 7376 6729 5d28  with-love.svg)](
-00000510: 6874 7470 733a 2f2f 4769 7448 7562 2e63  https://GitHub.c
-00000520: 6f6d 2f6b 6579 6966 6c65 726f 6c73 756e  om/keyiflerolsun
-00000530: 2f29 0a0a 2323 20f0 9f9a 8020 4b75 7275  /)..## .... Kuru
-00000540: 6c75 6d0a 0a60 6060 6261 7368 0a23 2059  lum..```bash.# Y
-00000550: c3bc 6b6c 656d 656b 0a70 6970 2069 6e73  ..klemek.pip ins
-00000560: 7461 6c6c 2042 544b 536f 7267 750a 0a23  tall BTKSorgu..#
-00000570: 2047 c3bc 6e63 656c 6c65 6d65 6b0a 7069   G..ncellemek.pi
-00000580: 7020 696e 7374 616c 6c20 2d55 2042 544b  p install -U BTK
-00000590: 536f 7267 750a 6060 600a 0a23 2320 f09f  Sorgu.```..## ..
-000005a0: 939d 204b 756c 6c61 6ec4 b16d 0a0a 6060  .. Kullan..m..``
-000005b0: 6070 7974 686f 6e0a 6672 6f6d 2042 544b  `python.from BTK
-000005c0: 536f 7267 7520 696d 706f 7274 2042 544b  Sorgu import BTK
-000005d0: 536f 7267 750a 6672 6f6d 2074 696d 6520  Sorgu.from time 
-000005e0: 2020 2020 696d 706f 7274 2074 696d 650a      import time.
-000005f0: 0a62 6173 6c61 203d 2074 696d 6528 290a  .basla = time().
-00000600: 7072 696e 7428 4254 4b53 6f72 6775 2827  print(BTKSorgu('
-00000610: 7265 6474 7562 652e 636f 6d27 2929 0a20  redtube.com')). 
-00000620: 2020 2023 20c2 bb20 7265 6474 7562 652e     # .. redtube.
-00000630: 636f 6d2c 2033 302f 3031 2f32 3030 3820  com, 30/01/2008 
-00000640: 7461 7269 686c 6920 7665 2034 3130 2e30  tarihli ve 410.0
-00000650: 312e 3032 2e32 3030 382d 3032 3831 3035  1.02.2008-028105
-00000660: 2073 6179 c4b1 6cc4 b120 5465 6c65 6b6f   say..l.. Teleko
-00000670: 6dc3 bc6e 696b 6173 796f 6e20 c4b0 6c65  m..nikasyon ..le
-00000680: 7469 c59f 696d 2042 61c5 9f6b 616e 6cc4  ti..im Ba..kanl.
-00000690: b1c4 9fc4 b120 6b61 7261 72c4 b179 6c61  ..... karar..yla
-000006a0: 2065 7269 c59f 696d 6520 656e 6765 6c6c   eri..ime engell
-000006b0: 656e 6d69 c59f 7469 722e 0a70 7269 6e74  enmi..tir..print
-000006c0: 2842 544b 536f 7267 7528 276b 656b 696b  (BTKSorgu('kekik
-000006d0: 616b 6164 656d 692e 6f72 6727 2929 0a20  akademi.org')). 
-000006e0: 2020 2023 20c2 bb20 4269 6c67 6920 5465     # .. Bilgi Te
-000006f0: 6b6e 6f6c 6f6a 696c 6572 6920 7665 20c4  knolojileri ve .
-00000700: b06c 6574 69c5 9f69 6d20 4b75 7275 6d75  .leti..im Kurumu
-00000710: 2074 6172 6166 c4b1 6e64 616e 2075 7967   taraf..ndan uyg
-00000720: 756c 616e 616e 2062 6972 206b 6172 6172  ulanan bir karar
-00000730: 2062 756c 756e 616d 6164 c4b1 2e0a 7072   bulunamad....pr
-00000740: 696e 7428 4254 4b53 6f72 6775 2827 786e  int(BTKSorgu('xn
-00000750: 7878 2e63 6f6d 2729 290a 2020 2020 2320  xx.com')).    # 
-00000760: c2bb 2078 6e78 782e 636f 6d2c 2032 332f  .. xnxx.com, 23/
-00000770: 3032 2f32 3030 3820 7461 7269 686c 6920  02/2008 tarihli 
-00000780: 7665 2034 3130 2e30 312e 3032 2e32 3030  ve 410.01.02.200
-00000790: 382d 3035 3430 3033 2073 6179 c4b1 6cc4  8-054003 say..l.
-000007a0: b120 5465 6c65 6b6f 6dc3 bc6e 696b 6173  . Telekom..nikas
-000007b0: 796f 6e20 c4b0 6c65 7469 c59f 696d 2042  yon ..leti..im B
-000007c0: 61c5 9f6b 616e 6cc4 b1c4 9fc4 b120 6b61  a..kanl...... ka
-000007d0: 7261 72c4 b179 6c61 2065 7269 c59f 696d  rar..yla eri..im
-000007e0: 6520 656e 6765 6c6c 656e 6d69 c59f 7469  e engellenmi..ti
-000007f0: 722e 0a62 6974 6972 203d 2074 696d 6528  r..bitir = time(
-00000800: 290a 0a70 7269 6e74 2862 6974 6972 2d62  )..print(bitir-b
-00000810: 6173 6c61 290a 2020 2020 2320 c2bb 2038  asla).    # .. 8
-00000820: 2e33 3532 3736 3635 3133 3832 3434 3633  .352766513824463
-00000830: 0a60 6060 0a0a 2323 20f0 9f94 9620 5072  .```..## .... Pr
-00000840: 6f67 7261 6d20 416b c4b1 c59f 20c5 9e65  ogram Ak.... ..e
-00000850: 6d61 73c4 b10a 0a31 2e20 2a4f 7475 7275  mas....1. *Oturu
-00000860: 6d20 4261 c59f 6c61 742c 2a0a 322e 202a  m Ba..lat,*.2. *
-00000870: 5b68 7474 7073 3a2f 2f69 6e74 6572 6e65  [https://interne
-00000880: 7432 2e62 746b 2e67 6f76 2e74 725d 2868  t2.btk.gov.tr](h
-00000890: 7474 7073 3a2f 2f69 6e74 6572 6e65 7432  ttps://internet2
-000008a0: 2e62 746b 2e67 6f76 2e74 722f 2920 6164  .btk.gov.tr/) ad
-000008b0: 7265 7369 6e65 2079 c3b6 6e6c 656e 6469  resine y..nlendi
-000008c0: 726d 656c 6572 6920 6b61 6275 6c20 6564  rmeleri kabul ed
-000008d0: 6572 656b 2067 6974 3a20 6b75 7261 6269  erek git: kurabi
-000008e0: 7965 6c65 7269 2079 652c 2a0a 332e 202a  yeleri ye,*.3. *
-000008f0: 44c3 b66e 656e 206b 6179 6e61 6b20 6b6f  D..nen kaynak ko
-00000900: 6475 6e64 616e 2064 6fc4 9f72 756c 616d  dundan do..rulam
-00000910: 6120 7265 736d 696e 6920 696e 6469 722c  a resmini indir,
-00000920: 2a0a 342e 202a 446f c49f 7275 6c61 6d61  *.4. *Do..rulama
-00000930: 2072 6573 6d69 6e69 204f 4352 2069 6c65   resmini OCR ile
-00000940: 2068 6172 666c 6572 6520 64c3 b66e c3bc   harflere d..n..
-00000950: c59f 74c3 bc72 2c20 626f c59f 6c75 6b6c  ..t..r, bo..lukl
-00000960: 6172 c4b1 2073 696c 2c2a 0a35 2e20 2a53  ar.. sil,*.5. *S
-00000970: 6f72 6775 2061 6472 6573 696e 6920 6f6b  orgu adresini ok
-00000980: 7564 75c4 9f75 6e20 646f c49f 7275 6c61  udu..un do..rula
-00000990: 6d61 206b 6f64 7579 6c61 2062 6972 6c69  ma koduyla birli
-000009a0: 6b74 6520 706f 7374 2061 742c 2a0a 362e  kte post at,*.6.
-000009b0: 202a 44c3 b66e 656e 2079 616e c4b1 74c4   *D..nen yan..t.
-000009c0: b120 6179 72c4 b1c5 9f74 c4b1 72c4 b170  . ayr....t..r..p
-000009d0: 2065 6469 7020 6765 7269 2064 c3b6 6e64   edip geri d..nd
-000009e0: c3bc 722e 2e2a 0a0a 3e20 4275 2070 726f  ..r..*..> Bu pro
-000009f0: 6772 616d c4b1 6e20 7961 7ac4 b16c 6d61  gram..n yaz..lma
-00000a00: 2076 6520 61c3 a7c4 b16b 206b 6179 6e61   ve a....k kayna
-00000a10: 6b20 6b6f 646c 7520 6f6c 6172 616b 2070  k kodlu olarak p
-00000a20: 6179 6c61 c59f c4b1 6c6d 6120 616d 6163  ayla....lma amac
-00000a30: c4b1 3a20 2a54 6172 6179 c4b1 63c4 b120  ..: *Taray..c.. 
-00000a40: 4f74 6f6d 6173 796f 6e6c 6172 c4b1 6ec4  Otomasyonlar..n.
-00000a50: b16e 2073 6562 6570 206f 6c64 75c4 9f75  .n sebep oldu..u
-00000a60: 2020 2a2a 6765 7265 6b73 697a 206b 6179    **gereksiz kay
-00000a70: 6e61 6b20 74c3 bc6b 6574 696d 692a 2a20  nak t..ketimi** 
-00000a80: 7665 2020 2a2a 7a61 6d61 6e20 6b61 7962  ve  **zaman kayb
-00000a90: c4b1 6ec4 b16e 2a2a 2020 c3b6 6ec3 bc6e  ..n..n**  ..n..n
-00000aa0: 6520 6765 c3a7 6d65 7965 2074 65c5 9f76  e ge..meye te..v
-00000ab0: 696b 2065 746d 656b 7469 72e2 80a6 2a0a  ik etmektir...*.
-00000ac0: 0a3e 2054 6172 6179 c4b1 63c4 b120 4f74  .> Taray..c.. Ot
-00000ad0: 6f6d 6173 796f 6e75 203a 202a 5b53 656c  omasyonu : *[Sel
-00000ae0: 656e 6975 6d20 4944 455d 2868 7474 7073  enium IDE](https
-00000af0: 3a2f 2f77 7777 2e73 656c 656e 6975 6d2e  ://www.selenium.
-00000b00: 6465 762f 7365 6c65 6e69 756d 2d69 6465  dev/selenium-ide
-00000b10: 2f29 2a20 2a2a 2d2a 2a20 2a5b 4b61 7461  /)* **-** *[Kata
-00000b20: 6c6f 6e20 4175 746f 6d61 7469 6f6e 2052  lon Automation R
-00000b30: 6563 6f72 6465 725d 2868 7474 7073 3a2f  ecorder](https:/
-00000b40: 2f77 7777 2e6b 6174 616c 6f6e 2e63 6f6d  /www.katalon.com
-00000b50: 2f72 6573 6f75 7263 6573 2d63 656e 7465  /resources-cente
-00000b60: 722f 626c 6f67 2f6b 6174 616c 6f6e 2d61  r/blog/katalon-a
-00000b70: 7574 6f6d 6174 696f 6e2d 7265 636f 7264  utomation-record
-00000b80: 6572 2f29 2a20 2a2a 2d2a 2a20 2a5b 4272  er/)* **-** *[Br
-00000b90: 6f77 7365 7241 7574 6f6d 6174 696f 6e53  owserAutomationS
-00000ba0: 7475 6469 6f5d 2868 7474 7073 3a2f 2f62  tudio](https://b
-00000bb0: 6162 6c6f 736f 6674 2e63 6f6d 2f73 686f  ablosoft.com/sho
-00000bc0: 702f 4272 6f77 7365 7241 7574 6f6d 6174  p/BrowserAutomat
-00000bd0: 696f 6e53 7475 6469 6f29 2a0a 0a3e 204b  ionStudio)*..> K
-00000be0: 6172 c59f c4b1 6c61 c59f 74c4 b172 6d61  ar....la..t..rma
-00000bf0: 73c4 b120 3a20 2a2a 5b53 656c 656e 6975  s.. : **[Seleniu
-00000c00: 6d20 5653 2052 6571 7565 7374 735d 2868  m VS Requests](h
-00000c10: 7474 7073 3a2f 2f77 7777 2e72 3130 2e6e  ttps://www.r10.n
-00000c20: 6574 2f6f 6666 2d74 6f70 6963 2f32 3735  et/off-topic/275
-00000c30: 3134 3132 2d73 656c 656e 6975 6d2d 7673  1412-selenium-vs
-00000c40: 2d72 6571 7565 7374 732e 6874 6d6c 292a  -requests.html)*
-00000c50: 2a0a 0a23 2320 f09f 939d 2050 726f 6a65  *..## .... Proje
-00000c60: 20c4 b06c 6572 6c65 6d65 7369 0a0a 2d20   ..lerlemesi..- 
-00000c70: e29c 8520 2a2a 5b40 7261 6966 7079 5d28  ... **[@raifpy](
-00000c80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c90: 6f6d 2f72 6169 6670 7929 2a2a 202a 7461  om/raifpy)** *ta
-00000ca0: 7261 66c4 b16e 6461 6e20 6b6f 646c 616e  raf..ndan kodlan
-00000cb0: 6dc4 b1c5 9f20 7072 6f6a 656e 696e 2068  m.... projenin h
-00000cc0: 616e 7461 6c20 6269 7220 6269 6c65 c59f  antal bir bile..
-00000cd0: 656e 6920 6974 696e 6179 6c61 2060 64c4  eni itinayla `d.
-00000ce0: b17a 7a20 f09f 908d 6027 6c61 6e6d c4b1  .zz ....`'lanm..
-00000cf0: c59f 74c4 b172 2e2e 2a0a 2d20 e29c 8520  ..t..r..*.- ... 
-00000d00: 2a2a 5365 6c65 6e69 756d 2a2a 202a 6261  **Selenium** *ba
-00000d10: c49f c4b1 6d6c c4b1 6cc4 b1c4 9fc4 b16e  ....ml..l......n
-00000d20: 6461 6e20 646f 6c61 79c4 b120 6861 6e74  dan dolay.. hant
-00000d30: 616c 20c3 a761 6cc4 b1c5 9f61 6e20 6b6f  al ..al....an ko
-00000d40: 6420 7961 70c4 b173 c4b1 2074 616d 616d  d yap..s.. tamam
-00000d50: 656e 2061 79c4 b16b 6c61 6ec4 b170 2062  en ay..klan..p b
-00000d60: c3bc 74c3 bc6e 2069 c59f 2a20 6072 6571  ..t..n i..* `req
-00000d70: 7565 7374 7360 2a27 6520 7961 7074 c4b1  uests`*'e yapt..
-00000d80: 72c4 b16c c4b1 7020 6369 6464 6920 6d69  r..l..p ciddi mi
-00000d90: 6b74 6172 6461 206b 6179 6e61 6b20 7665  ktarda kaynak ve
-00000da0: 207a 616d 616e 2074 6173 6172 7275 6675   zaman tasarrufu
-00000db0: 2065 7474 6972 696c 6d69 c59f 7469 722e   ettirilmi..tir.
-00000dc0: 2e2a 0a2d 20e2 9c85 202a 4b6f 6c61 7920  .*.- ... *Kolay 
-00000dd0: 6572 69c5 9f69 6c65 6269 6c69 7220 6f6c  eri..ilebilir ol
-00000de0: 6d61 73c4 b120 7665 2069 6c68 616d 2079  mas.. ve ilham y
-00000df0: 6172 6174 6d61 73c4 b120 69c3 a769 6e2a  aratmas.. i..in*
-00000e00: 202a 2a70 7970 692a 2a20 2a64 6570 6f6c   **pypi** *depol
-00000e10: 6172 c4b1 6e61 2079 c3bc 6b6c 656e 6d69  ar..na y..klenmi
-00000e20: c59f 7469 722e 2e2a 0a0a 2323 20f0 9f8c  ..tir..*..## ...
-00000e30: 9020 5465 6c69 6620 4861 6b6b c4b1 2076  . Telif Hakk.. v
-00000e40: 6520 4c69 7361 6e73 0a0a 2a20 2a43 6f70  e Lisans..* *Cop
-00000e50: 7972 6967 6874 2028 4329 2032 3032 3120  yright (C) 2021 
-00000e60: 6279 2a20 5b6b 6579 6966 6c65 726f 6c73  by* [keyiflerols
-00000e70: 756e 5d28 6874 7470 733a 2f2f 6769 7468  un](https://gith
-00000e80: 7562 2e63 6f6d 2f6b 6579 6966 6c65 726f  ub.com/keyiflero
-00000e90: 6c73 756e 2920 e29d a4ef b88f efb8 8f0a  lsun) ..........
-00000ea0: 2a20 5b47 4e55 2047 454e 4552 414c 2050  * [GNU GENERAL P
-00000eb0: 5542 4c49 4320 4c49 4345 4e53 4520 5665  UBLIC LICENSE Ve
-00000ec0: 7273 696f 6e20 332c 2032 3920 4a75 6e65  rsion 3, 29 June
-00000ed0: 2032 3030 375d 2868 7474 7073 3a2f 2f67   2007](https://g
-00000ee0: 6974 6875 622e 636f 6d2f 6b65 7969 666c  ithub.com/keyifl
-00000ef0: 6572 6f6c 7375 6e2f 6b65 7969 6655 7365  erolsun/keyifUse
-00000f00: 7242 6f74 2f62 6c6f 622f 6d61 7374 6572  rBot/blob/master
-00000f10: 2f4c 4943 454e 5345 2920 2a4b 6fc5 9f75  /LICENSE) *Ko..u
-00000f20: 6c6c 6172 c4b1 6e61 2067 c3b6 7265 206c  llar..na g..re l
-00000f30: 6973 616e 736c 616e 6dc4 b1c5 9f74 c4b1  isanslanm....t..
-00000f40: 722e 2e2a 0a0a 2323 20e2 99bb efb8 8f20  r..*..## ...... 
-00000f50: c4b0 6c65 7469 c59f 696d 0a0a 2a42 656e  ..leti..im..*Ben
-00000f60: 696d 6c65 2069 6c65 7469 c59f 696d 6520  imle ileti..ime 
-00000f70: 6765 c3a7 6d65 6b20 6973 7465 7273 656e  ge..mek istersen
-00000f80: 697a 2c20 2a2a 5465 6c65 6772 616d 2a2a  iz, **Telegram**
-00000f90: 2764 616e 206d 6573 616a 2067 c3b6 6e64  'dan mesaj g..nd
-00000fa0: 6572 6d65 6b74 656e 20c3 a765 6b69 6e6d  ermekten ..ekinm
-00000fb0: 6579 696e 3b2a 205b 406b 6579 6966 6c65  eyin;* [@keyifle
-00000fc0: 726f 6c73 756e 5d28 6874 7470 733a 2f2f  rolsun](https://
-00000fd0: 742e 6d65 2f6b 6579 6966 6c65 726f 6c73  t.me/keyiflerols
-00000fe0: 756e 290a 0a23 2320 f09f 92b8 2042 61c4  un)..## .... Ba.
-00000ff0: 9fc4 b1c5 9f20 5961 700a 0a2a 2a5b e298  ..... Yap..**[..
-00001000: 95ef b88f 204b 6168 7665 2049 736d 6172  .... Kahve Ismar
-00001010: 6c61 5d28 6874 7470 733a 2f2f 4b65 6b69  la](https://Keki
-00001020: 6b41 6b61 6465 6d69 2e6f 7267 2f4b 6168  kAkademi.org/Kah
-00001030: 7665 292a 2a0a 0a3e 202a 2a5b 404b 656b  ve)**..> **[@Kek
-00001040: 696b 416b 6164 656d 695d 2868 7474 7073  ikAkademi](https
-00001050: 3a2f 2f74 2e6d 652f 4b65 6b69 6b41 6b61  ://t.me/KekikAka
-00001060: 6465 6d69 292a 2a20 2a69 c3a7 696e 2079  demi)** *i..in y
-00001070: 617a c4b1 6c6d c4b1 c59f 74c4 b172 2e2e  az..lm....t..r..
-00001080: 2a0a 2727 270a 0a23 2323 230a 6672 6f6d  *.'''..####.from
-00001090: 2042 544b 536f 7267 752e 4572 6973 696d   BTKSorgu.Erisim
-000010a0: 5f45 6e67 656c 6920 696d 706f 7274 2042  _Engeli import B
-000010b0: 544b 536f 7267 750a 2323 2323            TKSorgu.####
+00000000: 2320 f09f 948d 2042 544b 536f 7267 750a  # .... BTKSorgu.
+00000010: 0a21 5b52 6570 6f20 426f 7975 7475 5d28  .![Repo Boyutu](
+00000020: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000030: 6c64 732e 696f 2f67 6974 6875 622f 7265  lds.io/github/re
+00000040: 706f 2d73 697a 652f 6b65 7969 666c 6572  po-size/keyifler
+00000050: 6f6c 7375 6e2f 4254 4b53 6f72 6775 3f6c  olsun/BTKSorgu?l
+00000060: 6f67 6f3d 6769 7426 6c6f 676f 436f 6c6f  ogo=git&logoColo
+00000070: 723d 7768 6974 6529 0a21 5b47 c3b6 72c3  r=white).![G..r.
+00000080: bc6e 74c3 bc6c 656e 6d65 5d28 6874 7470  .nt..lenme](http
+00000090: 733a 2f2f 6869 7473 2e73 6565 796f 7566  s://hits.seeyouf
+000000a0: 6172 6d2e 636f 6d2f 6170 692f 636f 756e  arm.com/api/coun
+000000b0: 742f 696e 6372 2f62 6164 6765 2e73 7667  t/incr/badge.svg
+000000c0: 3f75 726c 3d68 7474 7073 3a2f 2f67 6974  ?url=https://git
+000000d0: 6875 622e 636f 6d2f 6b65 7969 666c 6572  hub.com/keyifler
+000000e0: 6f6c 7375 6e2f 4254 4b53 6f72 6775 2674  olsun/BTKSorgu&t
+000000f0: 6974 6c65 3d47 c3b6 72c3 bc6e 74c3 bc6c  itle=G..r..nt..l
+00000100: 656e 6d65 290a 3c61 2068 7265 663d 2268  enme).<a href="h
+00000110: 7474 7073 3a2f 2f4b 656b 696b 416b 6164  ttps://KekikAkad
+00000120: 656d 692e 6f72 672f 4b61 6876 6522 2074  emi.org/Kahve" t
+00000130: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+00000140: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000150: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000160: 6261 6467 652f e298 95ef b88f 2d4b 6168  badge/......-Kah
+00000170: 7665 2049 736d 6172 6c61 2d66 6664 6430  ve Ismarla-ffdd0
+00000180: 3022 2074 6974 6c65 3d22 e298 95ef b88f  0" title="......
+00000190: 204b 6168 7665 2049 736d 6172 6c61 2220   Kahve Ismarla" 
+000001a0: 7374 796c 653d 2270 6164 6469 6e67 2d6c  style="padding-l
+000001b0: 6566 743a 3570 783b 223e 3c2f 613e 0a0a  eft:5px;"></a>..
+000001c0: 215b 5079 7468 6f6e 2056 6572 7369 6f6e  ![Python Version
+000001d0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000001e0: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
+000001f0: 7665 7273 696f 6e73 2f42 544b 536f 7267  versions/BTKSorg
+00000200: 753f 6c6f 676f 3d70 7974 686f 6e26 6c6f  u?logo=python&lo
+00000210: 676f 436f 6c6f 723d 7768 6974 6529 0a21  goColor=white).!
+00000220: 5b4c 6963 656e 7365 5d28 6874 7470 733a  [License](https:
+00000230: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000240: 2f70 7970 692f 6c2f 4254 4b53 6f72 6775  /pypi/l/BTKSorgu
+00000250: 3f6c 6f67 6f3d 676e 7526 6c6f 676f 436f  ?logo=gnu&logoCo
+00000260: 6c6f 723d 7768 6974 6529 0a21 5b53 7461  lor=white).![Sta
+00000270: 7475 735d 2868 7474 7073 3a2f 2f69 6d67  tus](https://img
+00000280: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000290: 2f73 7461 7475 732f 4254 4b53 6f72 6775  /status/BTKSorgu
+000002a0: 3f6c 6f67 6f3d 7769 6e64 6f77 7374 6572  ?logo=windowster
+000002b0: 6d69 6e61 6c26 6c6f 676f 436f 6c6f 723d  minal&logoColor=
+000002c0: 7768 6974 6529 0a0a 215b 5079 5049 5d28  white)..![PyPI](
+000002d0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000002e0: 6c64 732e 696f 2f70 7970 692f 762f 4254  lds.io/pypi/v/BT
+000002f0: 4b53 6f72 6775 3f6c 6f67 6f3d 7079 7069  KSorgu?logo=pypi
+00000300: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
+00000310: 290a 215b 5079 5049 202d 2044 6f77 6e6c  ).![PyPI - Downl
+00000320: 6f61 6473 5d28 6874 7470 733a 2f2f 696d  oads](https://im
+00000330: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000340: 692f 646d 2f42 544b 536f 7267 753f 6c6f  i/dm/BTKSorgu?lo
+00000350: 676f 3d70 7970 6926 6c6f 676f 436f 6c6f  go=pypi&logoColo
+00000360: 723d 7768 6974 6529 0a21 5b50 7950 4920  r=white).![PyPI 
+00000370: 2d20 5768 6565 6c5d 2868 7474 7073 3a2f  - Wheel](https:/
+00000380: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000390: 7079 7069 2f77 6865 656c 2f42 544b 536f  pypi/wheel/BTKSo
+000003a0: 7267 753f 6c6f 676f 3d70 7970 6926 6c6f  rgu?logo=pypi&lo
+000003b0: 676f 436f 6c6f 723d 7768 6974 6529 0a0a  goColor=white)..
+000003c0: 5b21 5b50 7950 4920 59c3 bc6b 6c65 5d28  [![PyPI Y..kle](
+000003d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000003e0: 6f6d 2f6b 6579 6966 6c65 726f 6c73 756e  om/keyiflerolsun
+000003f0: 2f42 544b 536f 7267 752f 6163 7469 6f6e  /BTKSorgu/action
+00000400: 732f 776f 726b 666c 6f77 732f 4b65 6b69  s/workflows/Keki
+00000410: 6b46 6c6f 772e 796d 6c2f 6261 6467 652e  kFlow.yml/badge.
+00000420: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00000430: 7468 7562 2e63 6f6d 2f6b 6579 6966 6c65  thub.com/keyifle
+00000440: 726f 6c73 756e 2f42 544b 536f 7267 752f  rolsun/BTKSorgu/
+00000450: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000460: 732f 4b65 6b69 6b46 6c6f 772e 796d 6c29  s/KekikFlow.yml)
+00000470: 0a0a 2a48 6564 6566 2077 6562 7369 7465  ..*Hedef website
+00000480: 7369 6e69 6e20 4254 4b20 5461 7261 66c4  sinin BTK Taraf.
+00000490: b16e 6461 6e20 4572 69c5 9f69 6d20 456e  .ndan Eri..im En
+000004a0: 6765 6c69 2053 6f72 6775 7375 2e2e 2a0a  geli Sorgusu..*.
+000004b0: 0a5b 215b 466f 7254 6865 4261 6467 6520  .[![ForTheBadge 
+000004c0: 6d61 6465 2d77 6974 682d 7079 7468 6f6e  made-with-python
+000004d0: 5d28 6874 7470 733a 2f2f 466f 7254 6865  ](https://ForThe
+000004e0: 4261 6467 652e 636f 6d2f 696d 6167 6573  Badge.com/images
+000004f0: 2f62 6164 6765 732f 6d61 6465 2d77 6974  /badges/made-wit
+00000500: 682d 7079 7468 6f6e 2e73 7667 295d 2868  h-python.svg)](h
+00000510: 7474 7073 3a2f 2f77 7777 2e70 7974 686f  ttps://www.pytho
+00000520: 6e2e 6f72 672f 290a 5b21 5b46 6f72 5468  n.org/).[![ForTh
+00000530: 6542 6164 6765 2062 7569 6c74 2d77 6974  eBadge built-wit
+00000540: 682d 6c6f 7665 5d28 6874 7470 733a 2f2f  h-love](https://
+00000550: 466f 7254 6865 4261 6467 652e 636f 6d2f  ForTheBadge.com/
+00000560: 696d 6167 6573 2f62 6164 6765 732f 6275  images/badges/bu
+00000570: 696c 742d 7769 7468 2d6c 6f76 652e 7376  ilt-with-love.sv
+00000580: 6729 5d28 6874 7470 733a 2f2f 4769 7448  g)](https://GitH
+00000590: 7562 2e63 6f6d 2f6b 6579 6966 6c65 726f  ub.com/keyiflero
+000005a0: 6c73 756e 2f29 0a0a 2323 20f0 9f9a 8020  lsun/)..## .... 
+000005b0: 4b75 7275 6c75 6d0a 0a60 6060 6261 7368  Kurulum..```bash
+000005c0: 0a23 2059 c3bc 6b6c 656d 656b 0a70 6970  .# Y..klemek.pip
+000005d0: 2069 6e73 7461 6c6c 2042 544b 536f 7267   install BTKSorg
+000005e0: 750a 0a23 2047 c3bc 6e63 656c 6c65 6d65  u..# G..ncelleme
+000005f0: 6b0a 7069 7020 696e 7374 616c 6c20 2d55  k.pip install -U
+00000600: 2042 544b 536f 7267 750a 6060 600a 0a23   BTKSorgu.```..#
+00000610: 2320 f09f 939d 204b 756c 6c61 6ec4 b16d  # .... Kullan..m
+00000620: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000630: 2042 544b 536f 7267 7520 696d 706f 7274   BTKSorgu import
+00000640: 2042 544b 536f 7267 750a 6672 6f6d 2074   BTKSorgu.from t
+00000650: 696d 6520 2020 2020 696d 706f 7274 2074  ime     import t
+00000660: 696d 650a 0a62 6173 6c61 203d 2074 696d  ime..basla = tim
+00000670: 6528 290a 7072 696e 7428 4254 4b53 6f72  e().print(BTKSor
+00000680: 6775 2822 7265 6474 7562 652e 636f 6d22  gu("redtube.com"
+00000690: 2929 0a20 2020 2023 20c2 bb20 7265 6474  )).    # .. redt
+000006a0: 7562 652e 636f 6d2c 2033 302f 3031 2f32  ube.com, 30/01/2
+000006b0: 3030 3820 7461 7269 686c 6920 7665 2034  008 tarihli ve 4
+000006c0: 3130 2e30 312e 3032 2e32 3030 382d 3032  10.01.02.2008-02
+000006d0: 3831 3035 2073 6179 c4b1 6cc4 b120 5465  8105 say..l.. Te
+000006e0: 6c65 6b6f 6dc3 bc6e 696b 6173 796f 6e20  lekom..nikasyon 
+000006f0: c4b0 6c65 7469 c59f 696d 2042 61c5 9f6b  ..leti..im Ba..k
+00000700: 616e 6cc4 b1c4 9fc4 b120 6b61 7261 72c4  anl...... karar.
+00000710: b179 6c61 2065 7269 c59f 696d 6520 656e  .yla eri..ime en
+00000720: 6765 6c6c 656e 6d69 c59f 7469 722e 0a70  gellenmi..tir..p
+00000730: 7269 6e74 2842 544b 536f 7267 7528 226b  rint(BTKSorgu("k
+00000740: 656b 696b 616b 6164 656d 692e 6f72 6722  ekikakademi.org"
+00000750: 2929 0a20 2020 2023 20c2 bb20 4269 6c67  )).    # .. Bilg
+00000760: 6920 5465 6b6e 6f6c 6f6a 696c 6572 6920  i Teknolojileri 
+00000770: 7665 20c4 b06c 6574 69c5 9f69 6d20 4b75  ve ..leti..im Ku
+00000780: 7275 6d75 2074 6172 6166 c4b1 6e64 616e  rumu taraf..ndan
+00000790: 2075 7967 756c 616e 616e 2062 6972 206b   uygulanan bir k
+000007a0: 6172 6172 2062 756c 756e 616d 6164 c4b1  arar bulunamad..
+000007b0: 2e0a 7072 696e 7428 4254 4b53 6f72 6775  ..print(BTKSorgu
+000007c0: 2822 786e 7878 2e63 6f6d 2229 290a 2020  ("xnxx.com")).  
+000007d0: 2020 2320 c2bb 2078 6e78 782e 636f 6d2c    # .. xnxx.com,
+000007e0: 2032 332f 3032 2f32 3030 3820 7461 7269   23/02/2008 tari
+000007f0: 686c 6920 7665 2034 3130 2e30 312e 3032  hli ve 410.01.02
+00000800: 2e32 3030 382d 3035 3430 3033 2073 6179  .2008-054003 say
+00000810: c4b1 6cc4 b120 5465 6c65 6b6f 6dc3 bc6e  ..l.. Telekom..n
+00000820: 696b 6173 796f 6e20 c4b0 6c65 7469 c59f  ikasyon ..leti..
+00000830: 696d 2042 61c5 9f6b 616e 6cc4 b1c4 9fc4  im Ba..kanl.....
+00000840: b120 6b61 7261 72c4 b179 6c61 2065 7269  . karar..yla eri
+00000850: c59f 696d 6520 656e 6765 6c6c 656e 6d69  ..ime engellenmi
+00000860: c59f 7469 722e 0a62 6974 6972 203d 2074  ..tir..bitir = t
+00000870: 696d 6528 290a 0a70 7269 6e74 2862 6974  ime()..print(bit
+00000880: 6972 2d62 6173 6c61 290a 2020 2020 2320  ir-basla).    # 
+00000890: c2bb 2038 2e33 3532 3736 3635 3133 3832  .. 8.35276651382
+000008a0: 3434 3633 0a60 6060 0a0a 6060 6062 6173  4463.```..```bas
+000008b0: 680a 4254 4b53 6f72 6775 206b 6579 6966  h.BTKSorgu keyif
+000008c0: 6c65 726f 6c73 756e 2e64 6576 0a0a 2320  lerolsun.dev..# 
+000008d0: 3e20 4269 6c67 6920 5465 6b6e 6f6c 6f6a  > Bilgi Teknoloj
+000008e0: 696c 6572 6920 7665 20c4 b06c 6574 69c5  ileri ve ..leti.
+000008f0: 9f69 6d20 4b75 7275 6d75 2074 6172 6166  .im Kurumu taraf
+00000900: c4b1 6e64 616e 2075 7967 756c 616e 616e  ..ndan uygulanan
+00000910: 2062 6972 206b 6172 6172 2062 756c 756e   bir karar bulun
+00000920: 616d 6164 c4b1 2e0a 6060 600a 0a23 2320  amad....```..## 
+00000930: f09f 9496 2050 726f 6772 616d 2041 6bc4  .... Program Ak.
+00000940: b1c5 9f20 c59e 656d 6173 c4b1 0a0a 312e  ... ..emas....1.
+00000950: 202a 4f74 7572 756d 2042 61c5 9f6c 6174   *Oturum Ba..lat
+00000960: 2c2a 0a32 2e20 2a5b 6874 7470 733a 2f2f  ,*.2. *[https://
+00000970: 696e 7465 726e 6574 322e 6274 6b2e 676f  internet2.btk.go
+00000980: 762e 7472 5d28 6874 7470 733a 2f2f 696e  v.tr](https://in
+00000990: 7465 726e 6574 322e 6274 6b2e 676f 762e  ternet2.btk.gov.
+000009a0: 7472 2f29 2061 6472 6573 696e 6520 79c3  tr/) adresine y.
+000009b0: b66e 6c65 6e64 6972 6d65 6c65 7269 206b  .nlendirmeleri k
+000009c0: 6162 756c 2065 6465 7265 6b20 6769 743a  abul ederek git:
+000009d0: 206b 7572 6162 6979 656c 6572 6920 7965   kurabiyeleri ye
+000009e0: 2c2a 0a33 2e20 2a44 c3b6 6e65 6e20 6b61  ,*.3. *D..nen ka
+000009f0: 796e 616b 206b 6f64 756e 6461 6e20 646f  ynak kodundan do
+00000a00: c49f 7275 6c61 6d61 2072 6573 6d69 6e69  ..rulama resmini
+00000a10: 2069 6e64 6972 2c2a 0a34 2e20 2a44 6fc4   indir,*.4. *Do.
+00000a20: 9f72 756c 616d 6120 7265 736d 696e 6920  .rulama resmini 
+00000a30: 4f43 5220 696c 6520 6861 7266 6c65 7265  OCR ile harflere
+00000a40: 2064 c3b6 6ec3 bcc5 9f74 c3bc 722c 2062   d..n....t..r, b
+00000a50: 6fc5 9f6c 756b 6c61 72c4 b120 7369 6c2c  o..luklar.. sil,
+00000a60: 2a0a 352e 202a 536f 7267 7520 6164 7265  *.5. *Sorgu adre
+00000a70: 7369 6e69 206f 6b75 6475 c49f 756e 2064  sini okudu..un d
+00000a80: 6fc4 9f72 756c 616d 6120 6b6f 6475 796c  o..rulama koduyl
+00000a90: 6120 6269 726c 696b 7465 2070 6f73 7420  a birlikte post 
+00000aa0: 6174 2c2a 0a36 2e20 2a44 c3b6 6e65 6e20  at,*.6. *D..nen 
+00000ab0: 7961 6ec4 b174 c4b1 2061 7972 c4b1 c59f  yan..t.. ayr....
+00000ac0: 74c4 b172 c4b1 7020 6564 6970 2067 6572  t..r..p edip ger
+00000ad0: 6920 64c3 b66e 64c3 bc72 2e2e 2a0a 0a3e  i d..nd..r..*..>
+00000ae0: 2042 7520 7072 6f67 7261 6dc4 b16e 2079   Bu program..n y
+00000af0: 617a c4b1 6c6d 6120 7665 2061 c3a7 c4b1  az..lma ve a....
+00000b00: 6b20 6b61 796e 616b 206b 6f64 6c75 206f  k kaynak kodlu o
+00000b10: 6c61 7261 6b20 7061 796c 61c5 9fc4 b16c  larak payla....l
+00000b20: 6d61 2061 6d61 63c4 b13a 202a 5461 7261  ma amac..: *Tara
+00000b30: 79c4 b163 c4b1 204f 746f 6d61 7379 6f6e  y..c.. Otomasyon
+00000b40: 6c61 72c4 b16e c4b1 6e20 7365 6265 7020  lar..n..n sebep 
+00000b50: 6f6c 6475 c49f 7520 202a 2a67 6572 656b  oldu..u  **gerek
+00000b60: 7369 7a20 6b61 796e 616b 2074 c3bc 6b65  siz kaynak t..ke
+00000b70: 7469 6d69 2a2a 2076 6520 202a 2a7a 616d  timi** ve  **zam
+00000b80: 616e 206b 6179 62c4 b16e c4b1 6e2a 2a20  an kayb..n..n** 
+00000b90: 20c3 b66e c3bc 6e65 2067 65c3 a76d 6579   ..n..ne ge..mey
+00000ba0: 6520 7465 c59f 7669 6b20 6574 6d65 6b74  e te..vik etmekt
+00000bb0: 6972 e280 a62a 0a0a 3e20 5461 7261 79c4  ir...*..> Taray.
+00000bc0: b163 c4b1 204f 746f 6d61 7379 6f6e 7520  .c.. Otomasyonu 
+00000bd0: 3a20 2a5b 5365 6c65 6e69 756d 2049 4445  : *[Selenium IDE
+00000be0: 5d28 6874 7470 733a 2f2f 7777 772e 7365  ](https://www.se
+00000bf0: 6c65 6e69 756d 2e64 6576 2f73 656c 656e  lenium.dev/selen
+00000c00: 6975 6d2d 6964 652f 292a 202a 2a2d 2a2a  ium-ide/)* **-**
+00000c10: 202a 5b4b 6174 616c 6f6e 2041 7574 6f6d   *[Katalon Autom
+00000c20: 6174 696f 6e20 5265 636f 7264 6572 5d28  ation Recorder](
+00000c30: 6874 7470 733a 2f2f 7777 772e 6b61 7461  https://www.kata
+00000c40: 6c6f 6e2e 636f 6d2f 7265 736f 7572 6365  lon.com/resource
+00000c50: 732d 6365 6e74 6572 2f62 6c6f 672f 6b61  s-center/blog/ka
+00000c60: 7461 6c6f 6e2d 6175 746f 6d61 7469 6f6e  talon-automation
+00000c70: 2d72 6563 6f72 6465 722f 292a 202a 2a2d  -recorder/)* **-
+00000c80: 2a2a 202a 5b42 726f 7773 6572 4175 746f  ** *[BrowserAuto
+00000c90: 6d61 7469 6f6e 5374 7564 696f 5d28 6874  mationStudio](ht
+00000ca0: 7470 733a 2f2f 6261 626c 6f73 6f66 742e  tps://bablosoft.
+00000cb0: 636f 6d2f 7368 6f70 2f42 726f 7773 6572  com/shop/Browser
+00000cc0: 4175 746f 6d61 7469 6f6e 5374 7564 696f  AutomationStudio
+00000cd0: 292a 0a0a 3e20 4b61 72c5 9fc4 b16c 61c5  )*..> Kar....la.
+00000ce0: 9f74 c4b1 726d 6173 c4b1 203a 202a 2a5b  .t..rmas.. : **[
+00000cf0: 5365 6c65 6e69 756d 2056 5320 5265 7175  Selenium VS Requ
+00000d00: 6573 7473 5d28 6874 7470 733a 2f2f 7777  ests](https://ww
+00000d10: 772e 7231 302e 6e65 742f 6f66 662d 746f  w.r10.net/off-to
+00000d20: 7069 632f 3237 3531 3431 322d 7365 6c65  pic/2751412-sele
+00000d30: 6e69 756d 2d76 732d 7265 7175 6573 7473  nium-vs-requests
+00000d40: 2e68 746d 6c29 2a2a 0a0a 2323 20f0 9f93  .html)**..## ...
+00000d50: 9d20 5072 6f6a 6520 c4b0 6c65 726c 656d  . Proje ..lerlem
+00000d60: 6573 690a 0a2d 20e2 9c85 202a 2a5b 4072  esi..- ... **[@r
+00000d70: 6169 6670 795d 2868 7474 7073 3a2f 2f67  aifpy](https://g
+00000d80: 6974 6875 622e 636f 6d2f 7261 6966 7079  ithub.com/raifpy
+00000d90: 292a 2a20 2a74 6172 6166 c4b1 6e64 616e  )** *taraf..ndan
+00000da0: 206b 6f64 6c61 6e6d c4b1 c59f 2070 726f   kodlanm.... pro
+00000db0: 6a65 6e69 6e20 6861 6e74 616c 2062 6972  jenin hantal bir
+00000dc0: 2062 696c 65c5 9f65 6e69 2069 7469 6e61   bile..eni itina
+00000dd0: 796c 6120 6064 c4b1 7a7a 20f0 9f90 8d60  yla `d..zz ....`
+00000de0: 276c 616e 6dc4 b1c5 9f74 c4b1 722e 2e2a  'lanm....t..r..*
+00000df0: 0a2d 20e2 9c85 202a 2a53 656c 656e 6975  .- ... **Seleniu
+00000e00: 6d2a 2a20 2a62 61c4 9fc4 b16d 6cc4 b16c  m** *ba....ml..l
+00000e10: c4b1 c49f c4b1 6e64 616e 2064 6f6c 6179  ......ndan dolay
+00000e20: c4b1 2068 616e 7461 6c20 c3a7 616c c4b1  .. hantal ..al..
+00000e30: c59f 616e 206b 6f64 2079 6170 c4b1 73c4  ..an kod yap..s.
+00000e40: b120 7461 6d61 6d65 6e20 6179 c4b1 6b6c  . tamamen ay..kl
+00000e50: 616e c4b1 7020 62c3 bc74 c3bc 6e20 69c5  an..p b..t..n i.
+00000e60: 9f2a 2060 7265 7175 6573 7473 602a 2765  .* `requests`*'e
+00000e70: 2079 6170 74c4 b172 c4b1 6cc4 b170 2063   yapt..r..l..p c
+00000e80: 6964 6469 206d 696b 7461 7264 6120 6b61  iddi miktarda ka
+00000e90: 796e 616b 2076 6520 7a61 6d61 6e20 7461  ynak ve zaman ta
+00000ea0: 7361 7272 7566 7520 6574 7469 7269 6c6d  sarrufu ettirilm
+00000eb0: 69c5 9f74 6972 2e2e 2a0a 2d20 e29c 8520  i..tir..*.- ... 
+00000ec0: 2a4b 6f6c 6179 2065 7269 c59f 696c 6562  *Kolay eri..ileb
+00000ed0: 696c 6972 206f 6c6d 6173 c4b1 2076 6520  ilir olmas.. ve 
+00000ee0: 696c 6861 6d20 7961 7261 746d 6173 c4b1  ilham yaratmas..
+00000ef0: 2069 c3a7 696e 2a20 2a2a 7079 7069 2a2a   i..in* **pypi**
+00000f00: 202a 6465 706f 6c61 72c4 b16e 6120 79c3   *depolar..na y.
+00000f10: bc6b 6c65 6e6d 69c5 9f74 6972 2e2e 2a0a  .klenmi..tir..*.
+00000f20: 0a23 2320 f09f 8c90 2054 656c 6966 2048  .## .... Telif H
+00000f30: 616b 6bc4 b120 7665 204c 6973 616e 730a  akk.. ve Lisans.
+00000f40: 0a2a 202a 436f 7079 7269 6768 7420 2843  .* *Copyright (C
+00000f50: 2920 3230 3233 2062 792a 205b 6b65 7969  ) 2023 by* [keyi
+00000f60: 666c 6572 6f6c 7375 6e5d 2868 7474 7073  flerolsun](https
+00000f70: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+00000f80: 7969 666c 6572 6f6c 7375 6e29 20e2 9da4  yiflerolsun) ...
+00000f90: efb8 8fef b88f 0a2a 205b 474e 5520 4745  .......* [GNU GE
+00000fa0: 4e45 5241 4c20 5055 424c 4943 204c 4943  NERAL PUBLIC LIC
+00000fb0: 454e 5345 2056 6572 7369 6f6e 2033 2c20  ENSE Version 3, 
+00000fc0: 3239 204a 756e 6520 3230 3037 5d28 6874  29 June 2007](ht
+00000fd0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000fe0: 2f6b 6579 6966 6c65 726f 6c73 756e 2f42  /keyiflerolsun/B
+00000ff0: 544b 536f 7267 752f 626c 6f62 2f6d 6173  TKSorgu/blob/mas
+00001000: 7465 722f 4c49 4345 4e53 4529 202a 4b6f  ter/LICENSE) *Ko
+00001010: c59f 756c 6c61 72c4 b16e 6120 67c3 b672  ..ullar..na g..r
+00001020: 6520 6c69 7361 6e73 6c61 6e6d c4b1 c59f  e lisanslanm....
+00001030: 74c4 b172 2e2e 2a0a 0a23 2320 e299 bbef  t..r..*..## ....
+00001040: b88f 20c4 b06c 6574 69c5 9f69 6d0a 0a2a  .. ..leti..im..*
+00001050: 4265 6e69 6d6c 6520 696c 6574 69c5 9f69  Benimle ileti..i
+00001060: 6d65 2067 65c3 a76d 656b 2069 7374 6572  me ge..mek ister
+00001070: 7365 6e69 7a2c 202a 2a54 656c 6567 7261  seniz, **Telegra
+00001080: 6d2a 2a27 6461 6e20 6d65 7361 6a20 67c3  m**'dan mesaj g.
+00001090: b66e 6465 726d 656b 7465 6e20 c3a7 656b  .ndermekten ..ek
+000010a0: 696e 6d65 7969 6e3b 2a20 5b40 6b65 7969  inmeyin;* [@keyi
+000010b0: 666c 6572 6f6c 7375 6e5d 2868 7474 7073  flerolsun](https
+000010c0: 3a2f 2f74 2e6d 652f 4b65 6b69 6b4b 6168  ://t.me/KekikKah
+000010d0: 7665 290a 0a23 2320 f09f 92b8 2042 61c4  ve)..## .... Ba.
+000010e0: 9fc4 b1c5 9f20 5961 700a 0a2a 2a5b e298  ..... Yap..**[..
+000010f0: 95ef b88f 204b 6168 7665 2049 736d 6172  .... Kahve Ismar
+00001100: 6c61 5d28 6874 7470 733a 2f2f 4b65 6b69  la](https://Keki
+00001110: 6b41 6b61 6465 6d69 2e6f 7267 2f4b 6168  kAkademi.org/Kah
+00001120: 7665 292a 2a0a 0a23 230a 0a3e 202a 2a5b  ve)**..##..> **[
+00001130: 404b 656b 696b 416b 6164 656d 695d 2868  @KekikAkademi](h
+00001140: 7474 7073 3a2f 2f74 2e6d 652f 4b65 6b69  ttps://t.me/Keki
+00001150: 6b41 6b61 6465 6d69 292a 2a20 2a69 c3a7  kAkademi)** *i..
+00001160: 696e 2079 617a c4b1 6c6d c4b1 c59f 74c4  in yaz..lm....t.
+00001170: b172 2e2e 2a0a                           .r..*.
```

### Comparing `BTKSorgu-0.1.5/BTKSorgu.egg-info/PKG-INFO` & `BTKSorgu-1.0.1/BTKSorgu.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,301 +1,316 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4254 4b53  : 2.1.Name: BTKS
-00000020: 6f72 6775 0a56 6572 7369 6f6e 3a20 302e  orgu.Version: 0.
-00000030: 312e 350a 5375 6d6d 6172 793a 2048 6564  1.5.Summary: Hed
+00000020: 6f72 6775 0a56 6572 7369 6f6e 3a20 312e  orgu.Version: 1.
+00000030: 302e 310a 5375 6d6d 6172 793a 2048 6564  0.1.Summary: Hed
 00000040: 6566 2077 6562 7369 7465 7369 6e69 6e20  ef websitesinin 
 00000050: 4254 4b20 5461 7261 66c4 b16e 6461 6e20  BTK Taraf..ndan 
 00000060: 4572 69c5 9f69 6d20 456e 6765 6c69 2053  Eri..im Engeli S
 00000070: 6f72 6775 7375 0a48 6f6d 652d 7061 6765  orgusu.Home-page
 00000080: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000090: 2e63 6f6d 2f6b 6579 6966 6c65 726f 6c73  .com/keyiflerols
-000000a0: 756e 2f42 544b 536f 7267 750a 4175 7468  un/BTKSorgu.Auth
-000000b0: 6f72 3a20 6b65 7969 666c 6572 6f6c 7375  or: keyiflerolsu
-000000c0: 6e0a 4175 7468 6f72 2d65 6d61 696c 3a20  n.Author-email: 
-000000d0: 6b65 7969 666c 6572 6f6c 7375 6e40 676d  keyiflerolsun@gm
-000000e0: 6169 6c2e 636f 6d0a 4c69 6365 6e73 653a  ail.com.License:
-000000f0: 2047 504c 7633 2b0a 4b65 7977 6f72 6473   GPLv3+.Keywords
-00000100: 3a20 4254 4b53 6f72 6775 2c4b 656b 696b  : BTKSorgu,Kekik
-00000110: 416b 6164 656d 692c 6b65 7969 666c 6572  Akademi,keyifler
-00000120: 6f6c 7375 6e0a 506c 6174 666f 726d 3a20  olsun.Platform: 
-00000130: 554e 4b4e 4f57 4e0a 436c 6173 7369 6669  UNKNOWN.Classifi
-00000140: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
-00000150: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
-00000160: 6f64 7563 7469 6f6e 2f53 7461 626c 650a  oduction/Stable.
-00000170: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
-00000180: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000190: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
-000001a0: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-000001b0: 6520 7633 206f 7220 6c61 7465 7220 2847  e v3 or later (G
-000001c0: 504c 7633 2b29 0a43 6c61 7373 6966 6965  PLv3+).Classifie
-000001d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001f0: 6e20 3a3a 2033 0a52 6571 7569 7265 732d  n :: 3.Requires-
-00000200: 5079 7468 6f6e 3a20 3e3d 332e 360a 4465  Python: >=3.6.De
-00000210: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000220: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000230: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
-00000240: 6c65 3a20 4c49 4345 4e53 450a 0a23 20f0  le: LICENSE..# .
-00000250: 9f94 8d20 4254 4b53 6f72 6775 0a0a 5b21  ... BTKSorgu..[!
-00000260: 5b43 6f64 6163 7920 4261 6467 655d 2868  [Codacy Badge](h
-00000270: 7474 7073 3a2f 2f61 7070 2e63 6f64 6163  ttps://app.codac
-00000280: 792e 636f 6d2f 7072 6f6a 6563 742f 6261  y.com/project/ba
-00000290: 6467 652f 4772 6164 652f 6263 3061 3532  dge/Grade/bc0a52
-000002a0: 6139 6235 3766 3463 3239 3933 3063 6264  a9b57f4c29930cbd
-000002b0: 3663 3739 3666 3961 3862 295d 2868 7474  6c796f9a8b)](htt
-000002c0: 7073 3a2f 2f77 7777 2e63 6f64 6163 792e  ps://www.codacy.
-000002d0: 636f 6d2f 6768 2f6b 6579 6966 6c65 726f  com/gh/keyiflero
-000002e0: 6c73 756e 2f42 544b 536f 7267 752f 6461  lsun/BTKSorgu/da
-000002f0: 7368 626f 6172 643f 7574 6d5f 736f 7572  shboard?utm_sour
-00000300: 6365 3d67 6974 6875 622e 636f 6d26 616d  ce=github.com&am
-00000310: 703b 7574 6d5f 6d65 6469 756d 3d72 6566  p;utm_medium=ref
-00000320: 6572 7261 6c26 616d 703b 7574 6d5f 636f  erral&amp;utm_co
-00000330: 6e74 656e 743d 6b65 7969 666c 6572 6f6c  ntent=keyiflerol
-00000340: 7375 6e2f 4254 4b53 6f72 6775 2661 6d70  sun/BTKSorgu&amp
-00000350: 3b75 746d 5f63 616d 7061 6967 6e3d 4261  ;utm_campaign=Ba
-00000360: 6467 655f 4772 6164 6529 2021 5b52 6570  dge_Grade) ![Rep
-00000370: 6f20 426f 7975 7475 5d28 6874 7470 733a  o Boyutu](https:
-00000380: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000390: 2f67 6974 6875 622f 7265 706f 2d73 697a  /github/repo-siz
-000003a0: 652f 6b65 7969 666c 6572 6f6c 7375 6e2f  e/keyiflerolsun/
-000003b0: 4254 4b53 6f72 6775 2920 215b 5669 6577  BTKSorgu) ![View
-000003c0: 735d 2868 7474 7073 3a2f 2f68 6974 732e  s](https://hits.
-000003d0: 7365 6579 6f75 6661 726d 2e63 6f6d 2f61  seeyoufarm.com/a
-000003e0: 7069 2f63 6f75 6e74 2f69 6e63 722f 6261  pi/count/incr/ba
-000003f0: 6467 652e 7376 673f 7572 6c3d 6874 7470  dge.svg?url=http
-00000400: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-00000410: 6579 6966 6c65 726f 6c73 756e 2f42 544b  eyiflerolsun/BTK
-00000420: 536f 7267 7526 7469 746c 653d 5072 6f66  Sorgu&title=Prof
-00000430: 696c 6525 3230 5669 6577 7329 205b 215b  ile%20Views) [![
-00000440: 4769 7470 6f64 2072 6561 6479 2d74 6f2d  Gitpod ready-to-
-00000450: 636f 6465 5d28 6874 7470 733a 2f2f 696d  code](https://im
-00000460: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000470: 6765 2f47 6974 706f 642d 7265 6164 792d  ge/Gitpod-ready-
-00000480: 2d74 6f2d 2d63 6f64 652d 626c 7565 3f6c  -to--code-blue?l
-00000490: 6f67 6f3d 6769 7470 6f64 295d 2868 7474  ogo=gitpod)](htt
-000004a0: 7073 3a2f 2f67 6974 706f 642e 696f 2f23  ps://gitpod.io/#
-000004b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000004c0: 6f6d 2f6b 6579 6966 6c65 726f 6c73 756e  om/keyiflerolsun
-000004d0: 2f42 544b 536f 7267 7529 0a0a 215b 5079  /BTKSorgu)..![Py
-000004e0: 5049 202d 2050 7974 686f 6e20 5665 7273  PI - Python Vers
-000004f0: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00000500: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000510: 2f70 7976 6572 7369 6f6e 732f 4254 4b53  /pyversions/BTKS
-00000520: 6f72 6775 290a 215b 5079 5049 202d 2053  orgu).![PyPI - S
-00000530: 7461 7475 735d 2868 7474 7073 3a2f 2f69  tatus](https://i
-00000540: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000550: 7069 2f73 7461 7475 732f 4254 4b53 6f72  pi/status/BTKSor
-00000560: 6775 290a 215b 5079 5049 5d28 6874 7470  gu).![PyPI](http
-00000570: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000580: 696f 2f70 7970 692f 762f 4254 4b53 6f72  io/pypi/v/BTKSor
-00000590: 6775 290a 215b 5079 5049 202d 2044 6f77  gu).![PyPI - Dow
-000005a0: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
-000005b0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-000005c0: 7970 692f 646d 2f42 544b 536f 7267 7529  ypi/dm/BTKSorgu)
-000005d0: 0a21 5b50 7950 4920 2d20 5768 6565 6c5d  .![PyPI - Wheel]
-000005e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000005f0: 656c 6473 2e69 6f2f 7079 7069 2f77 6865  elds.io/pypi/whe
-00000600: 656c 2f42 544b 536f 7267 7529 0a21 5b50  el/BTKSorgu).![P
-00000610: 7950 4920 2d20 4c69 6365 6e73 655d 2868  yPI - License](h
-00000620: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000630: 6473 2e69 6f2f 7079 7069 2f6c 2f42 544b  ds.io/pypi/l/BTK
-00000640: 536f 7267 7529 0a0a 2a48 6564 6566 2077  Sorgu)..*Hedef w
-00000650: 6562 7369 7465 7369 6e69 6e20 4254 4b20  ebsitesinin BTK 
-00000660: 5461 7261 66c4 b16e 6461 6e20 4572 69c5  Taraf..ndan Eri.
-00000670: 9f69 6d20 456e 6765 6c69 2053 6f72 6775  .im Engeli Sorgu
-00000680: 7375 2e2e 2a0a 0a5b 215b 666f 7274 6865  su..*..[![forthe
-00000690: 6261 6467 6520 6d61 6465 2d77 6974 682d  badge made-with-
-000006a0: 7079 7468 6f6e 5d28 6874 7470 3a2f 2f46  python](http://F
-000006b0: 6f72 5468 6542 6164 6765 2e63 6f6d 2f69  orTheBadge.com/i
-000006c0: 6d61 6765 732f 6261 6467 6573 2f6d 6164  mages/badges/mad
-000006d0: 652d 7769 7468 2d70 7974 686f 6e2e 7376  e-with-python.sv
-000006e0: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
-000006f0: 7079 7468 6f6e 2e6f 7267 2f29 0a5b 215b  python.org/).[![
-00000700: 466f 7254 6865 4261 6467 6520 6275 696c  ForTheBadge buil
-00000710: 742d 7769 7468 2d6c 6f76 655d 2868 7474  t-with-love](htt
-00000720: 703a 2f2f 466f 7254 6865 4261 6467 652e  p://ForTheBadge.
-00000730: 636f 6d2f 696d 6167 6573 2f62 6164 6765  com/images/badge
-00000740: 732f 6275 696c 742d 7769 7468 2d6c 6f76  s/built-with-lov
-00000750: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000760: 4769 7448 7562 2e63 6f6d 2f6b 6579 6966  GitHub.com/keyif
-00000770: 6c65 726f 6c73 756e 2f29 0a0a 2323 20f0  lerolsun/)..## .
-00000780: 9f9a 8020 4b75 7275 6c75 6d0a 0a60 6060  ... Kurulum..```
-00000790: 6261 7368 0a23 2059 c3bc 6b6c 656d 656b  bash.# Y..klemek
-000007a0: 0a70 6970 2069 6e73 7461 6c6c 2042 544b  .pip install BTK
-000007b0: 536f 7267 750a 0a23 2047 c3bc 6e63 656c  Sorgu..# G..ncel
-000007c0: 6c65 6d65 6b0a 7069 7020 696e 7374 616c  lemek.pip instal
-000007d0: 6c20 2d55 2042 544b 536f 7267 750a 6060  l -U BTKSorgu.``
-000007e0: 600a 0a23 2320 f09f 939d 204b 756c 6c61  `..## .... Kulla
-000007f0: 6ec4 b16d 0a0a 6060 6070 7974 686f 6e0a  n..m..```python.
-00000800: 6672 6f6d 2042 544b 536f 7267 7520 696d  from BTKSorgu im
-00000810: 706f 7274 2042 544b 536f 7267 750a 6672  port BTKSorgu.fr
-00000820: 6f6d 2074 696d 6520 2020 2020 696d 706f  om time     impo
-00000830: 7274 2074 696d 650a 0a62 6173 6c61 203d  rt time..basla =
-00000840: 2074 696d 6528 290a 7072 696e 7428 4254   time().print(BT
-00000850: 4b53 6f72 6775 2827 7265 6474 7562 652e  KSorgu('redtube.
-00000860: 636f 6d27 2929 0a20 2020 2023 20c2 bb20  com')).    # .. 
-00000870: 7265 6474 7562 652e 636f 6d2c 2033 302f  redtube.com, 30/
-00000880: 3031 2f32 3030 3820 7461 7269 686c 6920  01/2008 tarihli 
-00000890: 7665 2034 3130 2e30 312e 3032 2e32 3030  ve 410.01.02.200
-000008a0: 382d 3032 3831 3035 2073 6179 c4b1 6cc4  8-028105 say..l.
-000008b0: b120 5465 6c65 6b6f 6dc3 bc6e 696b 6173  . Telekom..nikas
-000008c0: 796f 6e20 c4b0 6c65 7469 c59f 696d 2042  yon ..leti..im B
-000008d0: 61c5 9f6b 616e 6cc4 b1c4 9fc4 b120 6b61  a..kanl...... ka
-000008e0: 7261 72c4 b179 6c61 2065 7269 c59f 696d  rar..yla eri..im
-000008f0: 6520 656e 6765 6c6c 656e 6d69 c59f 7469  e engellenmi..ti
-00000900: 722e 0a70 7269 6e74 2842 544b 536f 7267  r..print(BTKSorg
-00000910: 7528 276b 656b 696b 616b 6164 656d 692e  u('kekikakademi.
-00000920: 6f72 6727 2929 0a20 2020 2023 20c2 bb20  org')).    # .. 
-00000930: 4269 6c67 6920 5465 6b6e 6f6c 6f6a 696c  Bilgi Teknolojil
-00000940: 6572 6920 7665 20c4 b06c 6574 69c5 9f69  eri ve ..leti..i
-00000950: 6d20 4b75 7275 6d75 2074 6172 6166 c4b1  m Kurumu taraf..
-00000960: 6e64 616e 2075 7967 756c 616e 616e 2062  ndan uygulanan b
-00000970: 6972 206b 6172 6172 2062 756c 756e 616d  ir karar bulunam
-00000980: 6164 c4b1 2e0a 7072 696e 7428 4254 4b53  ad....print(BTKS
-00000990: 6f72 6775 2827 786e 7878 2e63 6f6d 2729  orgu('xnxx.com')
-000009a0: 290a 2020 2020 2320 c2bb 2078 6e78 782e  ).    # .. xnxx.
-000009b0: 636f 6d2c 2032 332f 3032 2f32 3030 3820  com, 23/02/2008 
-000009c0: 7461 7269 686c 6920 7665 2034 3130 2e30  tarihli ve 410.0
-000009d0: 312e 3032 2e32 3030 382d 3035 3430 3033  1.02.2008-054003
-000009e0: 2073 6179 c4b1 6cc4 b120 5465 6c65 6b6f   say..l.. Teleko
-000009f0: 6dc3 bc6e 696b 6173 796f 6e20 c4b0 6c65  m..nikasyon ..le
-00000a00: 7469 c59f 696d 2042 61c5 9f6b 616e 6cc4  ti..im Ba..kanl.
-00000a10: b1c4 9fc4 b120 6b61 7261 72c4 b179 6c61  ..... karar..yla
-00000a20: 2065 7269 c59f 696d 6520 656e 6765 6c6c   eri..ime engell
-00000a30: 656e 6d69 c59f 7469 722e 0a62 6974 6972  enmi..tir..bitir
-00000a40: 203d 2074 696d 6528 290a 0a70 7269 6e74   = time()..print
-00000a50: 2862 6974 6972 2d62 6173 6c61 290a 2020  (bitir-basla).  
-00000a60: 2020 2320 c2bb 2038 2e33 3532 3736 3635    # .. 8.3527665
-00000a70: 3133 3832 3434 3633 0a60 6060 0a0a 2323  13824463.```..##
-00000a80: 20f0 9f94 9620 5072 6f67 7261 6d20 416b   .... Program Ak
-00000a90: c4b1 c59f 20c5 9e65 6d61 73c4 b10a 0a31  .... ..emas....1
-00000aa0: 2e20 2a4f 7475 7275 6d20 4261 c59f 6c61  . *Oturum Ba..la
-00000ab0: 742c 2a0a 322e 202a 5b68 7474 7073 3a2f  t,*.2. *[https:/
-00000ac0: 2f69 6e74 6572 6e65 7432 2e62 746b 2e67  /internet2.btk.g
-00000ad0: 6f76 2e74 725d 2868 7474 7073 3a2f 2f69  ov.tr](https://i
-00000ae0: 6e74 6572 6e65 7432 2e62 746b 2e67 6f76  nternet2.btk.gov
-00000af0: 2e74 722f 2920 6164 7265 7369 6e65 2079  .tr/) adresine y
-00000b00: c3b6 6e6c 656e 6469 726d 656c 6572 6920  ..nlendirmeleri 
-00000b10: 6b61 6275 6c20 6564 6572 656b 2067 6974  kabul ederek git
-00000b20: 3a20 6b75 7261 6269 7965 6c65 7269 2079  : kurabiyeleri y
-00000b30: 652c 2a0a 332e 202a 44c3 b66e 656e 206b  e,*.3. *D..nen k
-00000b40: 6179 6e61 6b20 6b6f 6475 6e64 616e 2064  aynak kodundan d
-00000b50: 6fc4 9f72 756c 616d 6120 7265 736d 696e  o..rulama resmin
-00000b60: 6920 696e 6469 722c 2a0a 342e 202a 446f  i indir,*.4. *Do
-00000b70: c49f 7275 6c61 6d61 2072 6573 6d69 6e69  ..rulama resmini
-00000b80: 204f 4352 2069 6c65 2068 6172 666c 6572   OCR ile harfler
-00000b90: 6520 64c3 b66e c3bc c59f 74c3 bc72 2c20  e d..n....t..r, 
-00000ba0: 626f c59f 6c75 6b6c 6172 c4b1 2073 696c  bo..luklar.. sil
-00000bb0: 2c2a 0a35 2e20 2a53 6f72 6775 2061 6472  ,*.5. *Sorgu adr
-00000bc0: 6573 696e 6920 6f6b 7564 75c4 9f75 6e20  esini okudu..un 
-00000bd0: 646f c49f 7275 6c61 6d61 206b 6f64 7579  do..rulama koduy
-00000be0: 6c61 2062 6972 6c69 6b74 6520 706f 7374  la birlikte post
-00000bf0: 2061 742c 2a0a 362e 202a 44c3 b66e 656e   at,*.6. *D..nen
-00000c00: 2079 616e c4b1 74c4 b120 6179 72c4 b1c5   yan..t.. ayr...
-00000c10: 9f74 c4b1 72c4 b170 2065 6469 7020 6765  .t..r..p edip ge
-00000c20: 7269 2064 c3b6 6e64 c3bc 722e 2e2a 0a0a  ri d..nd..r..*..
-00000c30: 3e20 4275 2070 726f 6772 616d c4b1 6e20  > Bu program..n 
-00000c40: 7961 7ac4 b16c 6d61 2076 6520 61c3 a7c4  yaz..lma ve a...
-00000c50: b16b 206b 6179 6e61 6b20 6b6f 646c 7520  .k kaynak kodlu 
-00000c60: 6f6c 6172 616b 2070 6179 6c61 c59f c4b1  olarak payla....
-00000c70: 6c6d 6120 616d 6163 c4b1 3a20 2a54 6172  lma amac..: *Tar
-00000c80: 6179 c4b1 63c4 b120 4f74 6f6d 6173 796f  ay..c.. Otomasyo
-00000c90: 6e6c 6172 c4b1 6ec4 b16e 2073 6562 6570  nlar..n..n sebep
-00000ca0: 206f 6c64 75c4 9f75 2020 2a2a 6765 7265   oldu..u  **gere
-00000cb0: 6b73 697a 206b 6179 6e61 6b20 74c3 bc6b  ksiz kaynak t..k
-00000cc0: 6574 696d 692a 2a20 7665 2020 2a2a 7a61  etimi** ve  **za
-00000cd0: 6d61 6e20 6b61 7962 c4b1 6ec4 b16e 2a2a  man kayb..n..n**
-00000ce0: 2020 c3b6 6ec3 bc6e 6520 6765 c3a7 6d65    ..n..ne ge..me
-00000cf0: 7965 2074 65c5 9f76 696b 2065 746d 656b  ye te..vik etmek
-00000d00: 7469 72e2 80a6 2a0a 0a3e 2054 6172 6179  tir...*..> Taray
-00000d10: c4b1 63c4 b120 4f74 6f6d 6173 796f 6e75  ..c.. Otomasyonu
-00000d20: 203a 202a 5b53 656c 656e 6975 6d20 4944   : *[Selenium ID
-00000d30: 455d 2868 7474 7073 3a2f 2f77 7777 2e73  E](https://www.s
-00000d40: 656c 656e 6975 6d2e 6465 762f 7365 6c65  elenium.dev/sele
-00000d50: 6e69 756d 2d69 6465 2f29 2a20 2a2a 2d2a  nium-ide/)* **-*
-00000d60: 2a20 2a5b 4b61 7461 6c6f 6e20 4175 746f  * *[Katalon Auto
-00000d70: 6d61 7469 6f6e 2052 6563 6f72 6465 725d  mation Recorder]
-00000d80: 2868 7474 7073 3a2f 2f77 7777 2e6b 6174  (https://www.kat
-00000d90: 616c 6f6e 2e63 6f6d 2f72 6573 6f75 7263  alon.com/resourc
-00000da0: 6573 2d63 656e 7465 722f 626c 6f67 2f6b  es-center/blog/k
-00000db0: 6174 616c 6f6e 2d61 7574 6f6d 6174 696f  atalon-automatio
-00000dc0: 6e2d 7265 636f 7264 6572 2f29 2a20 2a2a  n-recorder/)* **
-00000dd0: 2d2a 2a20 2a5b 4272 6f77 7365 7241 7574  -** *[BrowserAut
-00000de0: 6f6d 6174 696f 6e53 7475 6469 6f5d 2868  omationStudio](h
-00000df0: 7474 7073 3a2f 2f62 6162 6c6f 736f 6674  ttps://bablosoft
-00000e00: 2e63 6f6d 2f73 686f 702f 4272 6f77 7365  .com/shop/Browse
-00000e10: 7241 7574 6f6d 6174 696f 6e53 7475 6469  rAutomationStudi
-00000e20: 6f29 2a0a 0a3e 204b 6172 c59f c4b1 6c61  o)*..> Kar....la
-00000e30: c59f 74c4 b172 6d61 73c4 b120 3a20 2a2a  ..t..rmas.. : **
-00000e40: 5b53 656c 656e 6975 6d20 5653 2052 6571  [Selenium VS Req
-00000e50: 7565 7374 735d 2868 7474 7073 3a2f 2f77  uests](https://w
-00000e60: 7777 2e72 3130 2e6e 6574 2f6f 6666 2d74  ww.r10.net/off-t
-00000e70: 6f70 6963 2f32 3735 3134 3132 2d73 656c  opic/2751412-sel
-00000e80: 656e 6975 6d2d 7673 2d72 6571 7565 7374  enium-vs-request
-00000e90: 732e 6874 6d6c 292a 2a0a 0a23 2320 f09f  s.html)**..## ..
-00000ea0: 939d 2050 726f 6a65 20c4 b06c 6572 6c65  .. Proje ..lerle
-00000eb0: 6d65 7369 0a0a 2d20 e29c 8520 2a2a 5b40  mesi..- ... **[@
-00000ec0: 7261 6966 7079 5d28 6874 7470 733a 2f2f  raifpy](https://
-00000ed0: 6769 7468 7562 2e63 6f6d 2f72 6169 6670  github.com/raifp
-00000ee0: 7929 2a2a 202a 7461 7261 66c4 b16e 6461  y)** *taraf..nda
-00000ef0: 6e20 6b6f 646c 616e 6dc4 b1c5 9f20 7072  n kodlanm.... pr
-00000f00: 6f6a 656e 696e 2068 616e 7461 6c20 6269  ojenin hantal bi
-00000f10: 7220 6269 6c65 c59f 656e 6920 6974 696e  r bile..eni itin
-00000f20: 6179 6c61 2060 64c4 b17a 7a20 f09f 908d  ayla `d..zz ....
-00000f30: 6027 6c61 6e6d c4b1 c59f 74c4 b172 2e2e  `'lanm....t..r..
-00000f40: 2a0a 2d20 e29c 8520 2a2a 5365 6c65 6e69  *.- ... **Seleni
-00000f50: 756d 2a2a 202a 6261 c49f c4b1 6d6c c4b1  um** *ba....ml..
-00000f60: 6cc4 b1c4 9fc4 b16e 6461 6e20 646f 6c61  l......ndan dola
-00000f70: 79c4 b120 6861 6e74 616c 20c3 a761 6cc4  y.. hantal ..al.
-00000f80: b1c5 9f61 6e20 6b6f 6420 7961 70c4 b173  ...an kod yap..s
-00000f90: c4b1 2074 616d 616d 656e 2061 79c4 b16b  .. tamamen ay..k
-00000fa0: 6c61 6ec4 b170 2062 c3bc 74c3 bc6e 2069  lan..p b..t..n i
-00000fb0: c59f 2a20 6072 6571 7565 7374 7360 2a27  ..* `requests`*'
-00000fc0: 6520 7961 7074 c4b1 72c4 b16c c4b1 7020  e yapt..r..l..p 
-00000fd0: 6369 6464 6920 6d69 6b74 6172 6461 206b  ciddi miktarda k
-00000fe0: 6179 6e61 6b20 7665 207a 616d 616e 2074  aynak ve zaman t
-00000ff0: 6173 6172 7275 6675 2065 7474 6972 696c  asarrufu ettiril
-00001000: 6d69 c59f 7469 722e 2e2a 0a2d 20e2 9c85  mi..tir..*.- ...
-00001010: 202a 4b6f 6c61 7920 6572 69c5 9f69 6c65   *Kolay eri..ile
-00001020: 6269 6c69 7220 6f6c 6d61 73c4 b120 7665  bilir olmas.. ve
-00001030: 2069 6c68 616d 2079 6172 6174 6d61 73c4   ilham yaratmas.
-00001040: b120 69c3 a769 6e2a 202a 2a70 7970 692a  . i..in* **pypi*
-00001050: 2a20 2a64 6570 6f6c 6172 c4b1 6e61 2079  * *depolar..na y
-00001060: c3bc 6b6c 656e 6d69 c59f 7469 722e 2e2a  ..klenmi..tir..*
-00001070: 0a0a 2323 20f0 9f8c 9020 5465 6c69 6620  ..## .... Telif 
-00001080: 4861 6b6b c4b1 2076 6520 4c69 7361 6e73  Hakk.. ve Lisans
-00001090: 0a0a 2a20 2a43 6f70 7972 6967 6874 2028  ..* *Copyright (
-000010a0: 4329 2032 3032 3120 6279 2a20 5b6b 6579  C) 2021 by* [key
-000010b0: 6966 6c65 726f 6c73 756e 5d28 6874 7470  iflerolsun](http
-000010c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-000010d0: 6579 6966 6c65 726f 6c73 756e 2920 e29d  eyiflerolsun) ..
-000010e0: a4ef b88f efb8 8f0a 2a20 5b47 4e55 2047  ........* [GNU G
-000010f0: 454e 4552 414c 2050 5542 4c49 4320 4c49  ENERAL PUBLIC LI
-00001100: 4345 4e53 4520 5665 7273 696f 6e20 332c  CENSE Version 3,
-00001110: 2032 3920 4a75 6e65 2032 3030 375d 2868   29 June 2007](h
-00001120: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001130: 6d2f 6b65 7969 666c 6572 6f6c 7375 6e2f  m/keyiflerolsun/
-00001140: 6b65 7969 6655 7365 7242 6f74 2f62 6c6f  keyifUserBot/blo
-00001150: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
-00001160: 2920 2a4b 6fc5 9f75 6c6c 6172 c4b1 6e61  ) *Ko..ullar..na
-00001170: 2067 c3b6 7265 206c 6973 616e 736c 616e   g..re lisanslan
-00001180: 6dc4 b1c5 9f74 c4b1 722e 2e2a 0a0a 2323  m....t..r..*..##
-00001190: 20e2 99bb efb8 8f20 c4b0 6c65 7469 c59f   ...... ..leti..
-000011a0: 696d 0a0a 2a42 656e 696d 6c65 2069 6c65  im..*Benimle ile
-000011b0: 7469 c59f 696d 6520 6765 c3a7 6d65 6b20  ti..ime ge..mek 
-000011c0: 6973 7465 7273 656e 697a 2c20 2a2a 5465  isterseniz, **Te
-000011d0: 6c65 6772 616d 2a2a 2764 616e 206d 6573  legram**'dan mes
-000011e0: 616a 2067 c3b6 6e64 6572 6d65 6b74 656e  aj g..ndermekten
-000011f0: 20c3 a765 6b69 6e6d 6579 696e 3b2a 205b   ..ekinmeyin;* [
-00001200: 406b 6579 6966 6c65 726f 6c73 756e 5d28  @keyiflerolsun](
-00001210: 6874 7470 733a 2f2f 742e 6d65 2f6b 6579  https://t.me/key
-00001220: 6966 6c65 726f 6c73 756e 290a 0a23 2320  iflerolsun)..## 
-00001230: f09f 92b8 2042 61c4 9fc4 b1c5 9f20 5961  .... Ba...... Ya
-00001240: 700a 0a2a 2a5b e298 95ef b88f 204b 6168  p..**[...... Kah
-00001250: 7665 2049 736d 6172 6c61 5d28 6874 7470  ve Ismarla](http
-00001260: 733a 2f2f 4b65 6b69 6b41 6b61 6465 6d69  s://KekikAkademi
-00001270: 2e6f 7267 2f4b 6168 7665 292a 2a0a 0a23  .org/Kahve)**..#
-00001280: 230a 0a3e 202a 2a5b 404b 656b 696b 416b  #..> **[@KekikAk
-00001290: 6164 656d 695d 2868 7474 7073 3a2f 2f74  ademi](https://t
-000012a0: 2e6d 652f 4b65 6b69 6b41 6b61 6465 6d69  .me/KekikAkademi
-000012b0: 292a 2a20 2a69 c3a7 696e 2079 617a c4b1  )** *i..in yaz..
-000012c0: 6c6d c4b1 c59f 74c4 b172 2e2e 2a0a 0a0a  lm....t..r..*...
+000000a0: 756e 2f45 2d46 6174 7572 615f 536f 7267  un/E-Fatura_Sorg
+000000b0: 750a 4175 7468 6f72 3a20 6b65 7969 666c  u.Author: keyifl
+000000c0: 6572 6f6c 7375 6e0a 4175 7468 6f72 2d65  erolsun.Author-e
+000000d0: 6d61 696c 3a20 6b65 7969 666c 6572 6f6c  mail: keyiflerol
+000000e0: 7375 6e40 676d 6169 6c2e 636f 6d0a 4c69  sun@gmail.com.Li
+000000f0: 6365 6e73 653a 2047 504c 7633 2b0a 4b65  cense: GPLv3+.Ke
+00000100: 7977 6f72 6473 3a20 4254 4b53 6f72 6775  ywords: BTKSorgu
+00000110: 2c4b 656b 696b 416b 6164 656d 692c 6b65  ,KekikAkademi,ke
+00000120: 7969 666c 6572 6f6c 7375 6e0a 436c 6173  yiflerolsun.Clas
+00000130: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
+00000140: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
+00000150: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
+00000160: 626c 650a 436c 6173 7369 6669 6572 3a20  ble.Classifier: 
+00000170: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000180: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
+00000190: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
+000001a0: 6365 6e73 6520 7633 206f 7220 6c61 7465  cense v3 or late
+000001b0: 7220 2847 504c 7633 2b29 0a43 6c61 7373  r (GPLv3+).Class
+000001c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001e0: 7974 686f 6e20 3a3a 2033 0a52 6571 7569  ython :: 3.Requi
+000001f0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+00000200: 3130 0a44 6573 6372 6970 7469 6f6e 2d43  10.Description-C
+00000210: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000220: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
+00000230: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000240: 0a0a 2320 f09f 948d 2042 544b 536f 7267  ..# .... BTKSorg
+00000250: 750a 0a21 5b52 6570 6f20 426f 7975 7475  u..![Repo Boyutu
+00000260: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000270: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000280: 7265 706f 2d73 697a 652f 6b65 7969 666c  repo-size/keyifl
+00000290: 6572 6f6c 7375 6e2f 4254 4b53 6f72 6775  erolsun/BTKSorgu
+000002a0: 3f6c 6f67 6f3d 6769 7426 6c6f 676f 436f  ?logo=git&logoCo
+000002b0: 6c6f 723d 7768 6974 6529 0a21 5b47 c3b6  lor=white).![G..
+000002c0: 72c3 bc6e 74c3 bc6c 656e 6d65 5d28 6874  r..nt..lenme](ht
+000002d0: 7470 733a 2f2f 6869 7473 2e73 6565 796f  tps://hits.seeyo
+000002e0: 7566 6172 6d2e 636f 6d2f 6170 692f 636f  ufarm.com/api/co
+000002f0: 756e 742f 696e 6372 2f62 6164 6765 2e73  unt/incr/badge.s
+00000300: 7667 3f75 726c 3d68 7474 7073 3a2f 2f67  vg?url=https://g
+00000310: 6974 6875 622e 636f 6d2f 6b65 7969 666c  ithub.com/keyifl
+00000320: 6572 6f6c 7375 6e2f 4254 4b53 6f72 6775  erolsun/BTKSorgu
+00000330: 2674 6974 6c65 3d47 c3b6 72c3 bc6e 74c3  &title=G..r..nt.
+00000340: bc6c 656e 6d65 290a 3c61 2068 7265 663d  .lenme).<a href=
+00000350: 2268 7474 7073 3a2f 2f4b 656b 696b 416b  "https://KekikAk
+00000360: 6164 656d 692e 6f72 672f 4b61 6876 6522  ademi.org/Kahve"
+00000370: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000380: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000390: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000003a0: 6f2f 6261 6467 652f e298 95ef b88f 2d4b  o/badge/......-K
+000003b0: 6168 7665 2049 736d 6172 6c61 2d66 6664  ahve Ismarla-ffd
+000003c0: 6430 3022 2074 6974 6c65 3d22 e298 95ef  d00" title="....
+000003d0: b88f 204b 6168 7665 2049 736d 6172 6c61  .. Kahve Ismarla
+000003e0: 2220 7374 796c 653d 2270 6164 6469 6e67  " style="padding
+000003f0: 2d6c 6566 743a 3570 783b 223e 3c2f 613e  -left:5px;"></a>
+00000400: 0a0a 215b 5079 7468 6f6e 2056 6572 7369  ..![Python Versi
+00000410: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
+00000420: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000430: 7079 7665 7273 696f 6e73 2f42 544b 536f  pyversions/BTKSo
+00000440: 7267 753f 6c6f 676f 3d70 7974 686f 6e26  rgu?logo=python&
+00000450: 6c6f 676f 436f 6c6f 723d 7768 6974 6529  logoColor=white)
+00000460: 0a21 5b4c 6963 656e 7365 5d28 6874 7470  .![License](http
+00000470: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000480: 696f 2f70 7970 692f 6c2f 4254 4b53 6f72  io/pypi/l/BTKSor
+00000490: 6775 3f6c 6f67 6f3d 676e 7526 6c6f 676f  gu?logo=gnu&logo
+000004a0: 436f 6c6f 723d 7768 6974 6529 0a21 5b53  Color=white).![S
+000004b0: 7461 7475 735d 2868 7474 7073 3a2f 2f69  tatus](https://i
+000004c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000004d0: 7069 2f73 7461 7475 732f 4254 4b53 6f72  pi/status/BTKSor
+000004e0: 6775 3f6c 6f67 6f3d 7769 6e64 6f77 7374  gu?logo=windowst
+000004f0: 6572 6d69 6e61 6c26 6c6f 676f 436f 6c6f  erminal&logoColo
+00000500: 723d 7768 6974 6529 0a0a 215b 5079 5049  r=white)..![PyPI
+00000510: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000520: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000530: 4254 4b53 6f72 6775 3f6c 6f67 6f3d 7079  BTKSorgu?logo=py
+00000540: 7069 266c 6f67 6f43 6f6c 6f72 3d77 6869  pi&logoColor=whi
+00000550: 7465 290a 215b 5079 5049 202d 2044 6f77  te).![PyPI - Dow
+00000560: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
+00000570: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000580: 7970 692f 646d 2f42 544b 536f 7267 753f  ypi/dm/BTKSorgu?
+00000590: 6c6f 676f 3d70 7970 6926 6c6f 676f 436f  logo=pypi&logoCo
+000005a0: 6c6f 723d 7768 6974 6529 0a21 5b50 7950  lor=white).![PyP
+000005b0: 4920 2d20 5768 6565 6c5d 2868 7474 7073  I - Wheel](https
+000005c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000005d0: 6f2f 7079 7069 2f77 6865 656c 2f42 544b  o/pypi/wheel/BTK
+000005e0: 536f 7267 753f 6c6f 676f 3d70 7970 6926  Sorgu?logo=pypi&
+000005f0: 6c6f 676f 436f 6c6f 723d 7768 6974 6529  logoColor=white)
+00000600: 0a0a 5b21 5b50 7950 4920 59c3 bc6b 6c65  ..[![PyPI Y..kle
+00000610: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000620: 2e63 6f6d 2f6b 6579 6966 6c65 726f 6c73  .com/keyiflerols
+00000630: 756e 2f42 544b 536f 7267 752f 6163 7469  un/BTKSorgu/acti
+00000640: 6f6e 732f 776f 726b 666c 6f77 732f 4b65  ons/workflows/Ke
+00000650: 6b69 6b46 6c6f 772e 796d 6c2f 6261 6467  kikFlow.yml/badg
+00000660: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000670: 6769 7468 7562 2e63 6f6d 2f6b 6579 6966  github.com/keyif
+00000680: 6c65 726f 6c73 756e 2f42 544b 536f 7267  lerolsun/BTKSorg
+00000690: 752f 6163 7469 6f6e 732f 776f 726b 666c  u/actions/workfl
+000006a0: 6f77 732f 4b65 6b69 6b46 6c6f 772e 796d  ows/KekikFlow.ym
+000006b0: 6c29 0a0a 2a48 6564 6566 2077 6562 7369  l)..*Hedef websi
+000006c0: 7465 7369 6e69 6e20 4254 4b20 5461 7261  tesinin BTK Tara
+000006d0: 66c4 b16e 6461 6e20 4572 69c5 9f69 6d20  f..ndan Eri..im 
+000006e0: 456e 6765 6c69 2053 6f72 6775 7375 2e2e  Engeli Sorgusu..
+000006f0: 2a0a 0a5b 215b 466f 7254 6865 4261 6467  *..[![ForTheBadg
+00000700: 6520 6d61 6465 2d77 6974 682d 7079 7468  e made-with-pyth
+00000710: 6f6e 5d28 6874 7470 733a 2f2f 466f 7254  on](https://ForT
+00000720: 6865 4261 6467 652e 636f 6d2f 696d 6167  heBadge.com/imag
+00000730: 6573 2f62 6164 6765 732f 6d61 6465 2d77  es/badges/made-w
+00000740: 6974 682d 7079 7468 6f6e 2e73 7667 295d  ith-python.svg)]
+00000750: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
+00000760: 686f 6e2e 6f72 672f 290a 5b21 5b46 6f72  hon.org/).[![For
+00000770: 5468 6542 6164 6765 2062 7569 6c74 2d77  TheBadge built-w
+00000780: 6974 682d 6c6f 7665 5d28 6874 7470 733a  ith-love](https:
+00000790: 2f2f 466f 7254 6865 4261 6467 652e 636f  //ForTheBadge.co
+000007a0: 6d2f 696d 6167 6573 2f62 6164 6765 732f  m/images/badges/
+000007b0: 6275 696c 742d 7769 7468 2d6c 6f76 652e  built-with-love.
+000007c0: 7376 6729 5d28 6874 7470 733a 2f2f 4769  svg)](https://Gi
+000007d0: 7448 7562 2e63 6f6d 2f6b 6579 6966 6c65  tHub.com/keyifle
+000007e0: 726f 6c73 756e 2f29 0a0a 2323 20f0 9f9a  rolsun/)..## ...
+000007f0: 8020 4b75 7275 6c75 6d0a 0a60 6060 6261  . Kurulum..```ba
+00000800: 7368 0a23 2059 c3bc 6b6c 656d 656b 0a70  sh.# Y..klemek.p
+00000810: 6970 2069 6e73 7461 6c6c 2042 544b 536f  ip install BTKSo
+00000820: 7267 750a 0a23 2047 c3bc 6e63 656c 6c65  rgu..# G..ncelle
+00000830: 6d65 6b0a 7069 7020 696e 7374 616c 6c20  mek.pip install 
+00000840: 2d55 2042 544b 536f 7267 750a 6060 600a  -U BTKSorgu.```.
+00000850: 0a23 2320 f09f 939d 204b 756c 6c61 6ec4  .## .... Kullan.
+00000860: b16d 0a0a 6060 6070 7974 686f 6e0a 6672  .m..```python.fr
+00000870: 6f6d 2042 544b 536f 7267 7520 696d 706f  om BTKSorgu impo
+00000880: 7274 2042 544b 536f 7267 750a 6672 6f6d  rt BTKSorgu.from
+00000890: 2074 696d 6520 2020 2020 696d 706f 7274   time     import
+000008a0: 2074 696d 650a 0a62 6173 6c61 203d 2074   time..basla = t
+000008b0: 696d 6528 290a 7072 696e 7428 4254 4b53  ime().print(BTKS
+000008c0: 6f72 6775 2822 7265 6474 7562 652e 636f  orgu("redtube.co
+000008d0: 6d22 2929 0a20 2020 2023 20c2 bb20 7265  m")).    # .. re
+000008e0: 6474 7562 652e 636f 6d2c 2033 302f 3031  dtube.com, 30/01
+000008f0: 2f32 3030 3820 7461 7269 686c 6920 7665  /2008 tarihli ve
+00000900: 2034 3130 2e30 312e 3032 2e32 3030 382d   410.01.02.2008-
+00000910: 3032 3831 3035 2073 6179 c4b1 6cc4 b120  028105 say..l.. 
+00000920: 5465 6c65 6b6f 6dc3 bc6e 696b 6173 796f  Telekom..nikasyo
+00000930: 6e20 c4b0 6c65 7469 c59f 696d 2042 61c5  n ..leti..im Ba.
+00000940: 9f6b 616e 6cc4 b1c4 9fc4 b120 6b61 7261  .kanl...... kara
+00000950: 72c4 b179 6c61 2065 7269 c59f 696d 6520  r..yla eri..ime 
+00000960: 656e 6765 6c6c 656e 6d69 c59f 7469 722e  engellenmi..tir.
+00000970: 0a70 7269 6e74 2842 544b 536f 7267 7528  .print(BTKSorgu(
+00000980: 226b 656b 696b 616b 6164 656d 692e 6f72  "kekikakademi.or
+00000990: 6722 2929 0a20 2020 2023 20c2 bb20 4269  g")).    # .. Bi
+000009a0: 6c67 6920 5465 6b6e 6f6c 6f6a 696c 6572  lgi Teknolojiler
+000009b0: 6920 7665 20c4 b06c 6574 69c5 9f69 6d20  i ve ..leti..im 
+000009c0: 4b75 7275 6d75 2074 6172 6166 c4b1 6e64  Kurumu taraf..nd
+000009d0: 616e 2075 7967 756c 616e 616e 2062 6972  an uygulanan bir
+000009e0: 206b 6172 6172 2062 756c 756e 616d 6164   karar bulunamad
+000009f0: c4b1 2e0a 7072 696e 7428 4254 4b53 6f72  ....print(BTKSor
+00000a00: 6775 2822 786e 7878 2e63 6f6d 2229 290a  gu("xnxx.com")).
+00000a10: 2020 2020 2320 c2bb 2078 6e78 782e 636f      # .. xnxx.co
+00000a20: 6d2c 2032 332f 3032 2f32 3030 3820 7461  m, 23/02/2008 ta
+00000a30: 7269 686c 6920 7665 2034 3130 2e30 312e  rihli ve 410.01.
+00000a40: 3032 2e32 3030 382d 3035 3430 3033 2073  02.2008-054003 s
+00000a50: 6179 c4b1 6cc4 b120 5465 6c65 6b6f 6dc3  ay..l.. Telekom.
+00000a60: bc6e 696b 6173 796f 6e20 c4b0 6c65 7469  .nikasyon ..leti
+00000a70: c59f 696d 2042 61c5 9f6b 616e 6cc4 b1c4  ..im Ba..kanl...
+00000a80: 9fc4 b120 6b61 7261 72c4 b179 6c61 2065  ... karar..yla e
+00000a90: 7269 c59f 696d 6520 656e 6765 6c6c 656e  ri..ime engellen
+00000aa0: 6d69 c59f 7469 722e 0a62 6974 6972 203d  mi..tir..bitir =
+00000ab0: 2074 696d 6528 290a 0a70 7269 6e74 2862   time()..print(b
+00000ac0: 6974 6972 2d62 6173 6c61 290a 2020 2020  itir-basla).    
+00000ad0: 2320 c2bb 2038 2e33 3532 3736 3635 3133  # .. 8.352766513
+00000ae0: 3832 3434 3633 0a60 6060 0a0a 6060 6062  824463.```..```b
+00000af0: 6173 680a 4254 4b53 6f72 6775 206b 6579  ash.BTKSorgu key
+00000b00: 6966 6c65 726f 6c73 756e 2e64 6576 0a0a  iflerolsun.dev..
+00000b10: 2320 3e20 4269 6c67 6920 5465 6b6e 6f6c  # > Bilgi Teknol
+00000b20: 6f6a 696c 6572 6920 7665 20c4 b06c 6574  ojileri ve ..let
+00000b30: 69c5 9f69 6d20 4b75 7275 6d75 2074 6172  i..im Kurumu tar
+00000b40: 6166 c4b1 6e64 616e 2075 7967 756c 616e  af..ndan uygulan
+00000b50: 616e 2062 6972 206b 6172 6172 2062 756c  an bir karar bul
+00000b60: 756e 616d 6164 c4b1 2e0a 6060 600a 0a23  unamad....```..#
+00000b70: 2320 f09f 9496 2050 726f 6772 616d 2041  # .... Program A
+00000b80: 6bc4 b1c5 9f20 c59e 656d 6173 c4b1 0a0a  k.... ..emas....
+00000b90: 312e 202a 4f74 7572 756d 2042 61c5 9f6c  1. *Oturum Ba..l
+00000ba0: 6174 2c2a 0a32 2e20 2a5b 6874 7470 733a  at,*.2. *[https:
+00000bb0: 2f2f 696e 7465 726e 6574 322e 6274 6b2e  //internet2.btk.
+00000bc0: 676f 762e 7472 5d28 6874 7470 733a 2f2f  gov.tr](https://
+00000bd0: 696e 7465 726e 6574 322e 6274 6b2e 676f  internet2.btk.go
+00000be0: 762e 7472 2f29 2061 6472 6573 696e 6520  v.tr/) adresine 
+00000bf0: 79c3 b66e 6c65 6e64 6972 6d65 6c65 7269  y..nlendirmeleri
+00000c00: 206b 6162 756c 2065 6465 7265 6b20 6769   kabul ederek gi
+00000c10: 743a 206b 7572 6162 6979 656c 6572 6920  t: kurabiyeleri 
+00000c20: 7965 2c2a 0a33 2e20 2a44 c3b6 6e65 6e20  ye,*.3. *D..nen 
+00000c30: 6b61 796e 616b 206b 6f64 756e 6461 6e20  kaynak kodundan 
+00000c40: 646f c49f 7275 6c61 6d61 2072 6573 6d69  do..rulama resmi
+00000c50: 6e69 2069 6e64 6972 2c2a 0a34 2e20 2a44  ni indir,*.4. *D
+00000c60: 6fc4 9f72 756c 616d 6120 7265 736d 696e  o..rulama resmin
+00000c70: 6920 4f43 5220 696c 6520 6861 7266 6c65  i OCR ile harfle
+00000c80: 7265 2064 c3b6 6ec3 bcc5 9f74 c3bc 722c  re d..n....t..r,
+00000c90: 2062 6fc5 9f6c 756b 6c61 72c4 b120 7369   bo..luklar.. si
+00000ca0: 6c2c 2a0a 352e 202a 536f 7267 7520 6164  l,*.5. *Sorgu ad
+00000cb0: 7265 7369 6e69 206f 6b75 6475 c49f 756e  resini okudu..un
+00000cc0: 2064 6fc4 9f72 756c 616d 6120 6b6f 6475   do..rulama kodu
+00000cd0: 796c 6120 6269 726c 696b 7465 2070 6f73  yla birlikte pos
+00000ce0: 7420 6174 2c2a 0a36 2e20 2a44 c3b6 6e65  t at,*.6. *D..ne
+00000cf0: 6e20 7961 6ec4 b174 c4b1 2061 7972 c4b1  n yan..t.. ayr..
+00000d00: c59f 74c4 b172 c4b1 7020 6564 6970 2067  ..t..r..p edip g
+00000d10: 6572 6920 64c3 b66e 64c3 bc72 2e2e 2a0a  eri d..nd..r..*.
+00000d20: 0a3e 2042 7520 7072 6f67 7261 6dc4 b16e  .> Bu program..n
+00000d30: 2079 617a c4b1 6c6d 6120 7665 2061 c3a7   yaz..lma ve a..
+00000d40: c4b1 6b20 6b61 796e 616b 206b 6f64 6c75  ..k kaynak kodlu
+00000d50: 206f 6c61 7261 6b20 7061 796c 61c5 9fc4   olarak payla...
+00000d60: b16c 6d61 2061 6d61 63c4 b13a 202a 5461  .lma amac..: *Ta
+00000d70: 7261 79c4 b163 c4b1 204f 746f 6d61 7379  ray..c.. Otomasy
+00000d80: 6f6e 6c61 72c4 b16e c4b1 6e20 7365 6265  onlar..n..n sebe
+00000d90: 7020 6f6c 6475 c49f 7520 202a 2a67 6572  p oldu..u  **ger
+00000da0: 656b 7369 7a20 6b61 796e 616b 2074 c3bc  eksiz kaynak t..
+00000db0: 6b65 7469 6d69 2a2a 2076 6520 202a 2a7a  ketimi** ve  **z
+00000dc0: 616d 616e 206b 6179 62c4 b16e c4b1 6e2a  aman kayb..n..n*
+00000dd0: 2a20 20c3 b66e c3bc 6e65 2067 65c3 a76d  *  ..n..ne ge..m
+00000de0: 6579 6520 7465 c59f 7669 6b20 6574 6d65  eye te..vik etme
+00000df0: 6b74 6972 e280 a62a 0a0a 3e20 5461 7261  ktir...*..> Tara
+00000e00: 79c4 b163 c4b1 204f 746f 6d61 7379 6f6e  y..c.. Otomasyon
+00000e10: 7520 3a20 2a5b 5365 6c65 6e69 756d 2049  u : *[Selenium I
+00000e20: 4445 5d28 6874 7470 733a 2f2f 7777 772e  DE](https://www.
+00000e30: 7365 6c65 6e69 756d 2e64 6576 2f73 656c  selenium.dev/sel
+00000e40: 656e 6975 6d2d 6964 652f 292a 202a 2a2d  enium-ide/)* **-
+00000e50: 2a2a 202a 5b4b 6174 616c 6f6e 2041 7574  ** *[Katalon Aut
+00000e60: 6f6d 6174 696f 6e20 5265 636f 7264 6572  omation Recorder
+00000e70: 5d28 6874 7470 733a 2f2f 7777 772e 6b61  ](https://www.ka
+00000e80: 7461 6c6f 6e2e 636f 6d2f 7265 736f 7572  talon.com/resour
+00000e90: 6365 732d 6365 6e74 6572 2f62 6c6f 672f  ces-center/blog/
+00000ea0: 6b61 7461 6c6f 6e2d 6175 746f 6d61 7469  katalon-automati
+00000eb0: 6f6e 2d72 6563 6f72 6465 722f 292a 202a  on-recorder/)* *
+00000ec0: 2a2d 2a2a 202a 5b42 726f 7773 6572 4175  *-** *[BrowserAu
+00000ed0: 746f 6d61 7469 6f6e 5374 7564 696f 5d28  tomationStudio](
+00000ee0: 6874 7470 733a 2f2f 6261 626c 6f73 6f66  https://bablosof
+00000ef0: 742e 636f 6d2f 7368 6f70 2f42 726f 7773  t.com/shop/Brows
+00000f00: 6572 4175 746f 6d61 7469 6f6e 5374 7564  erAutomationStud
+00000f10: 696f 292a 0a0a 3e20 4b61 72c5 9fc4 b16c  io)*..> Kar....l
+00000f20: 61c5 9f74 c4b1 726d 6173 c4b1 203a 202a  a..t..rmas.. : *
+00000f30: 2a5b 5365 6c65 6e69 756d 2056 5320 5265  *[Selenium VS Re
+00000f40: 7175 6573 7473 5d28 6874 7470 733a 2f2f  quests](https://
+00000f50: 7777 772e 7231 302e 6e65 742f 6f66 662d  www.r10.net/off-
+00000f60: 746f 7069 632f 3237 3531 3431 322d 7365  topic/2751412-se
+00000f70: 6c65 6e69 756d 2d76 732d 7265 7175 6573  lenium-vs-reques
+00000f80: 7473 2e68 746d 6c29 2a2a 0a0a 2323 20f0  ts.html)**..## .
+00000f90: 9f93 9d20 5072 6f6a 6520 c4b0 6c65 726c  ... Proje ..lerl
+00000fa0: 656d 6573 690a 0a2d 20e2 9c85 202a 2a5b  emesi..- ... **[
+00000fb0: 4072 6169 6670 795d 2868 7474 7073 3a2f  @raifpy](https:/
+00000fc0: 2f67 6974 6875 622e 636f 6d2f 7261 6966  /github.com/raif
+00000fd0: 7079 292a 2a20 2a74 6172 6166 c4b1 6e64  py)** *taraf..nd
+00000fe0: 616e 206b 6f64 6c61 6e6d c4b1 c59f 2070  an kodlanm.... p
+00000ff0: 726f 6a65 6e69 6e20 6861 6e74 616c 2062  rojenin hantal b
+00001000: 6972 2062 696c 65c5 9f65 6e69 2069 7469  ir bile..eni iti
+00001010: 6e61 796c 6120 6064 c4b1 7a7a 20f0 9f90  nayla `d..zz ...
+00001020: 8d60 276c 616e 6dc4 b1c5 9f74 c4b1 722e  .`'lanm....t..r.
+00001030: 2e2a 0a2d 20e2 9c85 202a 2a53 656c 656e  .*.- ... **Selen
+00001040: 6975 6d2a 2a20 2a62 61c4 9fc4 b16d 6cc4  ium** *ba....ml.
+00001050: b16c c4b1 c49f c4b1 6e64 616e 2064 6f6c  .l......ndan dol
+00001060: 6179 c4b1 2068 616e 7461 6c20 c3a7 616c  ay.. hantal ..al
+00001070: c4b1 c59f 616e 206b 6f64 2079 6170 c4b1  ....an kod yap..
+00001080: 73c4 b120 7461 6d61 6d65 6e20 6179 c4b1  s.. tamamen ay..
+00001090: 6b6c 616e c4b1 7020 62c3 bc74 c3bc 6e20  klan..p b..t..n 
+000010a0: 69c5 9f2a 2060 7265 7175 6573 7473 602a  i..* `requests`*
+000010b0: 2765 2079 6170 74c4 b172 c4b1 6cc4 b170  'e yapt..r..l..p
+000010c0: 2063 6964 6469 206d 696b 7461 7264 6120   ciddi miktarda 
+000010d0: 6b61 796e 616b 2076 6520 7a61 6d61 6e20  kaynak ve zaman 
+000010e0: 7461 7361 7272 7566 7520 6574 7469 7269  tasarrufu ettiri
+000010f0: 6c6d 69c5 9f74 6972 2e2e 2a0a 2d20 e29c  lmi..tir..*.- ..
+00001100: 8520 2a4b 6f6c 6179 2065 7269 c59f 696c  . *Kolay eri..il
+00001110: 6562 696c 6972 206f 6c6d 6173 c4b1 2076  ebilir olmas.. v
+00001120: 6520 696c 6861 6d20 7961 7261 746d 6173  e ilham yaratmas
+00001130: c4b1 2069 c3a7 696e 2a20 2a2a 7079 7069  .. i..in* **pypi
+00001140: 2a2a 202a 6465 706f 6c61 72c4 b16e 6120  ** *depolar..na 
+00001150: 79c3 bc6b 6c65 6e6d 69c5 9f74 6972 2e2e  y..klenmi..tir..
+00001160: 2a0a 0a23 2320 f09f 8c90 2054 656c 6966  *..## .... Telif
+00001170: 2048 616b 6bc4 b120 7665 204c 6973 616e   Hakk.. ve Lisan
+00001180: 730a 0a2a 202a 436f 7079 7269 6768 7420  s..* *Copyright 
+00001190: 2843 2920 3230 3233 2062 792a 205b 6b65  (C) 2023 by* [ke
+000011a0: 7969 666c 6572 6f6c 7375 6e5d 2868 7474  yiflerolsun](htt
+000011b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000011c0: 6b65 7969 666c 6572 6f6c 7375 6e29 20e2  keyiflerolsun) .
+000011d0: 9da4 efb8 8fef b88f 0a2a 205b 474e 5520  .........* [GNU 
+000011e0: 4745 4e45 5241 4c20 5055 424c 4943 204c  GENERAL PUBLIC L
+000011f0: 4943 454e 5345 2056 6572 7369 6f6e 2033  ICENSE Version 3
+00001200: 2c20 3239 204a 756e 6520 3230 3037 5d28  , 29 June 2007](
+00001210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001220: 6f6d 2f6b 6579 6966 6c65 726f 6c73 756e  om/keyiflerolsun
+00001230: 2f42 544b 536f 7267 752f 626c 6f62 2f6d  /BTKSorgu/blob/m
+00001240: 6173 7465 722f 4c49 4345 4e53 4529 202a  aster/LICENSE) *
+00001250: 4b6f c59f 756c 6c61 72c4 b16e 6120 67c3  Ko..ullar..na g.
+00001260: b672 6520 6c69 7361 6e73 6c61 6e6d c4b1  .re lisanslanm..
+00001270: c59f 74c4 b172 2e2e 2a0a 0a23 2320 e299  ..t..r..*..## ..
+00001280: bbef b88f 20c4 b06c 6574 69c5 9f69 6d0a  .... ..leti..im.
+00001290: 0a2a 4265 6e69 6d6c 6520 696c 6574 69c5  .*Benimle ileti.
+000012a0: 9f69 6d65 2067 65c3 a76d 656b 2069 7374  .ime ge..mek ist
+000012b0: 6572 7365 6e69 7a2c 202a 2a54 656c 6567  erseniz, **Teleg
+000012c0: 7261 6d2a 2a27 6461 6e20 6d65 7361 6a20  ram**'dan mesaj 
+000012d0: 67c3 b66e 6465 726d 656b 7465 6e20 c3a7  g..ndermekten ..
+000012e0: 656b 696e 6d65 7969 6e3b 2a20 5b40 6b65  ekinmeyin;* [@ke
+000012f0: 7969 666c 6572 6f6c 7375 6e5d 2868 7474  yiflerolsun](htt
+00001300: 7073 3a2f 2f74 2e6d 652f 4b65 6b69 6b4b  ps://t.me/KekikK
+00001310: 6168 7665 290a 0a23 2320 f09f 92b8 2042  ahve)..## .... B
+00001320: 61c4 9fc4 b1c5 9f20 5961 700a 0a2a 2a5b  a...... Yap..**[
+00001330: e298 95ef b88f 204b 6168 7665 2049 736d  ...... Kahve Ism
+00001340: 6172 6c61 5d28 6874 7470 733a 2f2f 4b65  arla](https://Ke
+00001350: 6b69 6b41 6b61 6465 6d69 2e6f 7267 2f4b  kikAkademi.org/K
+00001360: 6168 7665 292a 2a0a 0a23 230a 0a3e 202a  ahve)**..##..> *
+00001370: 2a5b 404b 656b 696b 416b 6164 656d 695d  *[@KekikAkademi]
+00001380: 2868 7474 7073 3a2f 2f74 2e6d 652f 4b65  (https://t.me/Ke
+00001390: 6b69 6b41 6b61 6465 6d69 292a 2a20 2a69  kikAkademi)** *i
+000013a0: c3a7 696e 2079 617a c4b1 6c6d c4b1 c59f  ..in yaz..lm....
+000013b0: 74c4 b172 2e2e 2a0a                      t..r..*.
```

### Comparing `BTKSorgu-0.1.5/LICENSE` & `BTKSorgu-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BTKSorgu-0.1.5/PKG-INFO` & `BTKSorgu-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,301 +1,316 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4254 4b53  : 2.1.Name: BTKS
-00000020: 6f72 6775 0a56 6572 7369 6f6e 3a20 302e  orgu.Version: 0.
-00000030: 312e 350a 5375 6d6d 6172 793a 2048 6564  1.5.Summary: Hed
+00000020: 6f72 6775 0a56 6572 7369 6f6e 3a20 312e  orgu.Version: 1.
+00000030: 302e 310a 5375 6d6d 6172 793a 2048 6564  0.1.Summary: Hed
 00000040: 6566 2077 6562 7369 7465 7369 6e69 6e20  ef websitesinin 
 00000050: 4254 4b20 5461 7261 66c4 b16e 6461 6e20  BTK Taraf..ndan 
 00000060: 4572 69c5 9f69 6d20 456e 6765 6c69 2053  Eri..im Engeli S
 00000070: 6f72 6775 7375 0a48 6f6d 652d 7061 6765  orgusu.Home-page
 00000080: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
 00000090: 2e63 6f6d 2f6b 6579 6966 6c65 726f 6c73  .com/keyiflerols
-000000a0: 756e 2f42 544b 536f 7267 750a 4175 7468  un/BTKSorgu.Auth
-000000b0: 6f72 3a20 6b65 7969 666c 6572 6f6c 7375  or: keyiflerolsu
-000000c0: 6e0a 4175 7468 6f72 2d65 6d61 696c 3a20  n.Author-email: 
-000000d0: 6b65 7969 666c 6572 6f6c 7375 6e40 676d  keyiflerolsun@gm
-000000e0: 6169 6c2e 636f 6d0a 4c69 6365 6e73 653a  ail.com.License:
-000000f0: 2047 504c 7633 2b0a 4b65 7977 6f72 6473   GPLv3+.Keywords
-00000100: 3a20 4254 4b53 6f72 6775 2c4b 656b 696b  : BTKSorgu,Kekik
-00000110: 416b 6164 656d 692c 6b65 7969 666c 6572  Akademi,keyifler
-00000120: 6f6c 7375 6e0a 506c 6174 666f 726d 3a20  olsun.Platform: 
-00000130: 554e 4b4e 4f57 4e0a 436c 6173 7369 6669  UNKNOWN.Classifi
-00000140: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
-00000150: 5374 6174 7573 203a 3a20 3520 2d20 5072  Status :: 5 - Pr
-00000160: 6f64 7563 7469 6f6e 2f53 7461 626c 650a  oduction/Stable.
-00000170: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
-00000180: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000190: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
-000001a0: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-000001b0: 6520 7633 206f 7220 6c61 7465 7220 2847  e v3 or later (G
-000001c0: 504c 7633 2b29 0a43 6c61 7373 6966 6965  PLv3+).Classifie
-000001d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001f0: 6e20 3a3a 2033 0a52 6571 7569 7265 732d  n :: 3.Requires-
-00000200: 5079 7468 6f6e 3a20 3e3d 332e 360a 4465  Python: >=3.6.De
-00000210: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000220: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000230: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
-00000240: 6c65 3a20 4c49 4345 4e53 450a 0a23 20f0  le: LICENSE..# .
-00000250: 9f94 8d20 4254 4b53 6f72 6775 0a0a 5b21  ... BTKSorgu..[!
-00000260: 5b43 6f64 6163 7920 4261 6467 655d 2868  [Codacy Badge](h
-00000270: 7474 7073 3a2f 2f61 7070 2e63 6f64 6163  ttps://app.codac
-00000280: 792e 636f 6d2f 7072 6f6a 6563 742f 6261  y.com/project/ba
-00000290: 6467 652f 4772 6164 652f 6263 3061 3532  dge/Grade/bc0a52
-000002a0: 6139 6235 3766 3463 3239 3933 3063 6264  a9b57f4c29930cbd
-000002b0: 3663 3739 3666 3961 3862 295d 2868 7474  6c796f9a8b)](htt
-000002c0: 7073 3a2f 2f77 7777 2e63 6f64 6163 792e  ps://www.codacy.
-000002d0: 636f 6d2f 6768 2f6b 6579 6966 6c65 726f  com/gh/keyiflero
-000002e0: 6c73 756e 2f42 544b 536f 7267 752f 6461  lsun/BTKSorgu/da
-000002f0: 7368 626f 6172 643f 7574 6d5f 736f 7572  shboard?utm_sour
-00000300: 6365 3d67 6974 6875 622e 636f 6d26 616d  ce=github.com&am
-00000310: 703b 7574 6d5f 6d65 6469 756d 3d72 6566  p;utm_medium=ref
-00000320: 6572 7261 6c26 616d 703b 7574 6d5f 636f  erral&amp;utm_co
-00000330: 6e74 656e 743d 6b65 7969 666c 6572 6f6c  ntent=keyiflerol
-00000340: 7375 6e2f 4254 4b53 6f72 6775 2661 6d70  sun/BTKSorgu&amp
-00000350: 3b75 746d 5f63 616d 7061 6967 6e3d 4261  ;utm_campaign=Ba
-00000360: 6467 655f 4772 6164 6529 2021 5b52 6570  dge_Grade) ![Rep
-00000370: 6f20 426f 7975 7475 5d28 6874 7470 733a  o Boyutu](https:
-00000380: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000390: 2f67 6974 6875 622f 7265 706f 2d73 697a  /github/repo-siz
-000003a0: 652f 6b65 7969 666c 6572 6f6c 7375 6e2f  e/keyiflerolsun/
-000003b0: 4254 4b53 6f72 6775 2920 215b 5669 6577  BTKSorgu) ![View
-000003c0: 735d 2868 7474 7073 3a2f 2f68 6974 732e  s](https://hits.
-000003d0: 7365 6579 6f75 6661 726d 2e63 6f6d 2f61  seeyoufarm.com/a
-000003e0: 7069 2f63 6f75 6e74 2f69 6e63 722f 6261  pi/count/incr/ba
-000003f0: 6467 652e 7376 673f 7572 6c3d 6874 7470  dge.svg?url=http
-00000400: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-00000410: 6579 6966 6c65 726f 6c73 756e 2f42 544b  eyiflerolsun/BTK
-00000420: 536f 7267 7526 7469 746c 653d 5072 6f66  Sorgu&title=Prof
-00000430: 696c 6525 3230 5669 6577 7329 205b 215b  ile%20Views) [![
-00000440: 4769 7470 6f64 2072 6561 6479 2d74 6f2d  Gitpod ready-to-
-00000450: 636f 6465 5d28 6874 7470 733a 2f2f 696d  code](https://im
-00000460: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000470: 6765 2f47 6974 706f 642d 7265 6164 792d  ge/Gitpod-ready-
-00000480: 2d74 6f2d 2d63 6f64 652d 626c 7565 3f6c  -to--code-blue?l
-00000490: 6f67 6f3d 6769 7470 6f64 295d 2868 7474  ogo=gitpod)](htt
-000004a0: 7073 3a2f 2f67 6974 706f 642e 696f 2f23  ps://gitpod.io/#
-000004b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000004c0: 6f6d 2f6b 6579 6966 6c65 726f 6c73 756e  om/keyiflerolsun
-000004d0: 2f42 544b 536f 7267 7529 0a0a 215b 5079  /BTKSorgu)..![Py
-000004e0: 5049 202d 2050 7974 686f 6e20 5665 7273  PI - Python Vers
-000004f0: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00000500: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000510: 2f70 7976 6572 7369 6f6e 732f 4254 4b53  /pyversions/BTKS
-00000520: 6f72 6775 290a 215b 5079 5049 202d 2053  orgu).![PyPI - S
-00000530: 7461 7475 735d 2868 7474 7073 3a2f 2f69  tatus](https://i
-00000540: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000550: 7069 2f73 7461 7475 732f 4254 4b53 6f72  pi/status/BTKSor
-00000560: 6775 290a 215b 5079 5049 5d28 6874 7470  gu).![PyPI](http
-00000570: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000580: 696f 2f70 7970 692f 762f 4254 4b53 6f72  io/pypi/v/BTKSor
-00000590: 6775 290a 215b 5079 5049 202d 2044 6f77  gu).![PyPI - Dow
-000005a0: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
-000005b0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-000005c0: 7970 692f 646d 2f42 544b 536f 7267 7529  ypi/dm/BTKSorgu)
-000005d0: 0a21 5b50 7950 4920 2d20 5768 6565 6c5d  .![PyPI - Wheel]
-000005e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000005f0: 656c 6473 2e69 6f2f 7079 7069 2f77 6865  elds.io/pypi/whe
-00000600: 656c 2f42 544b 536f 7267 7529 0a21 5b50  el/BTKSorgu).![P
-00000610: 7950 4920 2d20 4c69 6365 6e73 655d 2868  yPI - License](h
-00000620: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000630: 6473 2e69 6f2f 7079 7069 2f6c 2f42 544b  ds.io/pypi/l/BTK
-00000640: 536f 7267 7529 0a0a 2a48 6564 6566 2077  Sorgu)..*Hedef w
-00000650: 6562 7369 7465 7369 6e69 6e20 4254 4b20  ebsitesinin BTK 
-00000660: 5461 7261 66c4 b16e 6461 6e20 4572 69c5  Taraf..ndan Eri.
-00000670: 9f69 6d20 456e 6765 6c69 2053 6f72 6775  .im Engeli Sorgu
-00000680: 7375 2e2e 2a0a 0a5b 215b 666f 7274 6865  su..*..[![forthe
-00000690: 6261 6467 6520 6d61 6465 2d77 6974 682d  badge made-with-
-000006a0: 7079 7468 6f6e 5d28 6874 7470 3a2f 2f46  python](http://F
-000006b0: 6f72 5468 6542 6164 6765 2e63 6f6d 2f69  orTheBadge.com/i
-000006c0: 6d61 6765 732f 6261 6467 6573 2f6d 6164  mages/badges/mad
-000006d0: 652d 7769 7468 2d70 7974 686f 6e2e 7376  e-with-python.sv
-000006e0: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
-000006f0: 7079 7468 6f6e 2e6f 7267 2f29 0a5b 215b  python.org/).[![
-00000700: 466f 7254 6865 4261 6467 6520 6275 696c  ForTheBadge buil
-00000710: 742d 7769 7468 2d6c 6f76 655d 2868 7474  t-with-love](htt
-00000720: 703a 2f2f 466f 7254 6865 4261 6467 652e  p://ForTheBadge.
-00000730: 636f 6d2f 696d 6167 6573 2f62 6164 6765  com/images/badge
-00000740: 732f 6275 696c 742d 7769 7468 2d6c 6f76  s/built-with-lov
-00000750: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000760: 4769 7448 7562 2e63 6f6d 2f6b 6579 6966  GitHub.com/keyif
-00000770: 6c65 726f 6c73 756e 2f29 0a0a 2323 20f0  lerolsun/)..## .
-00000780: 9f9a 8020 4b75 7275 6c75 6d0a 0a60 6060  ... Kurulum..```
-00000790: 6261 7368 0a23 2059 c3bc 6b6c 656d 656b  bash.# Y..klemek
-000007a0: 0a70 6970 2069 6e73 7461 6c6c 2042 544b  .pip install BTK
-000007b0: 536f 7267 750a 0a23 2047 c3bc 6e63 656c  Sorgu..# G..ncel
-000007c0: 6c65 6d65 6b0a 7069 7020 696e 7374 616c  lemek.pip instal
-000007d0: 6c20 2d55 2042 544b 536f 7267 750a 6060  l -U BTKSorgu.``
-000007e0: 600a 0a23 2320 f09f 939d 204b 756c 6c61  `..## .... Kulla
-000007f0: 6ec4 b16d 0a0a 6060 6070 7974 686f 6e0a  n..m..```python.
-00000800: 6672 6f6d 2042 544b 536f 7267 7520 696d  from BTKSorgu im
-00000810: 706f 7274 2042 544b 536f 7267 750a 6672  port BTKSorgu.fr
-00000820: 6f6d 2074 696d 6520 2020 2020 696d 706f  om time     impo
-00000830: 7274 2074 696d 650a 0a62 6173 6c61 203d  rt time..basla =
-00000840: 2074 696d 6528 290a 7072 696e 7428 4254   time().print(BT
-00000850: 4b53 6f72 6775 2827 7265 6474 7562 652e  KSorgu('redtube.
-00000860: 636f 6d27 2929 0a20 2020 2023 20c2 bb20  com')).    # .. 
-00000870: 7265 6474 7562 652e 636f 6d2c 2033 302f  redtube.com, 30/
-00000880: 3031 2f32 3030 3820 7461 7269 686c 6920  01/2008 tarihli 
-00000890: 7665 2034 3130 2e30 312e 3032 2e32 3030  ve 410.01.02.200
-000008a0: 382d 3032 3831 3035 2073 6179 c4b1 6cc4  8-028105 say..l.
-000008b0: b120 5465 6c65 6b6f 6dc3 bc6e 696b 6173  . Telekom..nikas
-000008c0: 796f 6e20 c4b0 6c65 7469 c59f 696d 2042  yon ..leti..im B
-000008d0: 61c5 9f6b 616e 6cc4 b1c4 9fc4 b120 6b61  a..kanl...... ka
-000008e0: 7261 72c4 b179 6c61 2065 7269 c59f 696d  rar..yla eri..im
-000008f0: 6520 656e 6765 6c6c 656e 6d69 c59f 7469  e engellenmi..ti
-00000900: 722e 0a70 7269 6e74 2842 544b 536f 7267  r..print(BTKSorg
-00000910: 7528 276b 656b 696b 616b 6164 656d 692e  u('kekikakademi.
-00000920: 6f72 6727 2929 0a20 2020 2023 20c2 bb20  org')).    # .. 
-00000930: 4269 6c67 6920 5465 6b6e 6f6c 6f6a 696c  Bilgi Teknolojil
-00000940: 6572 6920 7665 20c4 b06c 6574 69c5 9f69  eri ve ..leti..i
-00000950: 6d20 4b75 7275 6d75 2074 6172 6166 c4b1  m Kurumu taraf..
-00000960: 6e64 616e 2075 7967 756c 616e 616e 2062  ndan uygulanan b
-00000970: 6972 206b 6172 6172 2062 756c 756e 616d  ir karar bulunam
-00000980: 6164 c4b1 2e0a 7072 696e 7428 4254 4b53  ad....print(BTKS
-00000990: 6f72 6775 2827 786e 7878 2e63 6f6d 2729  orgu('xnxx.com')
-000009a0: 290a 2020 2020 2320 c2bb 2078 6e78 782e  ).    # .. xnxx.
-000009b0: 636f 6d2c 2032 332f 3032 2f32 3030 3820  com, 23/02/2008 
-000009c0: 7461 7269 686c 6920 7665 2034 3130 2e30  tarihli ve 410.0
-000009d0: 312e 3032 2e32 3030 382d 3035 3430 3033  1.02.2008-054003
-000009e0: 2073 6179 c4b1 6cc4 b120 5465 6c65 6b6f   say..l.. Teleko
-000009f0: 6dc3 bc6e 696b 6173 796f 6e20 c4b0 6c65  m..nikasyon ..le
-00000a00: 7469 c59f 696d 2042 61c5 9f6b 616e 6cc4  ti..im Ba..kanl.
-00000a10: b1c4 9fc4 b120 6b61 7261 72c4 b179 6c61  ..... karar..yla
-00000a20: 2065 7269 c59f 696d 6520 656e 6765 6c6c   eri..ime engell
-00000a30: 656e 6d69 c59f 7469 722e 0a62 6974 6972  enmi..tir..bitir
-00000a40: 203d 2074 696d 6528 290a 0a70 7269 6e74   = time()..print
-00000a50: 2862 6974 6972 2d62 6173 6c61 290a 2020  (bitir-basla).  
-00000a60: 2020 2320 c2bb 2038 2e33 3532 3736 3635    # .. 8.3527665
-00000a70: 3133 3832 3434 3633 0a60 6060 0a0a 2323  13824463.```..##
-00000a80: 20f0 9f94 9620 5072 6f67 7261 6d20 416b   .... Program Ak
-00000a90: c4b1 c59f 20c5 9e65 6d61 73c4 b10a 0a31  .... ..emas....1
-00000aa0: 2e20 2a4f 7475 7275 6d20 4261 c59f 6c61  . *Oturum Ba..la
-00000ab0: 742c 2a0a 322e 202a 5b68 7474 7073 3a2f  t,*.2. *[https:/
-00000ac0: 2f69 6e74 6572 6e65 7432 2e62 746b 2e67  /internet2.btk.g
-00000ad0: 6f76 2e74 725d 2868 7474 7073 3a2f 2f69  ov.tr](https://i
-00000ae0: 6e74 6572 6e65 7432 2e62 746b 2e67 6f76  nternet2.btk.gov
-00000af0: 2e74 722f 2920 6164 7265 7369 6e65 2079  .tr/) adresine y
-00000b00: c3b6 6e6c 656e 6469 726d 656c 6572 6920  ..nlendirmeleri 
-00000b10: 6b61 6275 6c20 6564 6572 656b 2067 6974  kabul ederek git
-00000b20: 3a20 6b75 7261 6269 7965 6c65 7269 2079  : kurabiyeleri y
-00000b30: 652c 2a0a 332e 202a 44c3 b66e 656e 206b  e,*.3. *D..nen k
-00000b40: 6179 6e61 6b20 6b6f 6475 6e64 616e 2064  aynak kodundan d
-00000b50: 6fc4 9f72 756c 616d 6120 7265 736d 696e  o..rulama resmin
-00000b60: 6920 696e 6469 722c 2a0a 342e 202a 446f  i indir,*.4. *Do
-00000b70: c49f 7275 6c61 6d61 2072 6573 6d69 6e69  ..rulama resmini
-00000b80: 204f 4352 2069 6c65 2068 6172 666c 6572   OCR ile harfler
-00000b90: 6520 64c3 b66e c3bc c59f 74c3 bc72 2c20  e d..n....t..r, 
-00000ba0: 626f c59f 6c75 6b6c 6172 c4b1 2073 696c  bo..luklar.. sil
-00000bb0: 2c2a 0a35 2e20 2a53 6f72 6775 2061 6472  ,*.5. *Sorgu adr
-00000bc0: 6573 696e 6920 6f6b 7564 75c4 9f75 6e20  esini okudu..un 
-00000bd0: 646f c49f 7275 6c61 6d61 206b 6f64 7579  do..rulama koduy
-00000be0: 6c61 2062 6972 6c69 6b74 6520 706f 7374  la birlikte post
-00000bf0: 2061 742c 2a0a 362e 202a 44c3 b66e 656e   at,*.6. *D..nen
-00000c00: 2079 616e c4b1 74c4 b120 6179 72c4 b1c5   yan..t.. ayr...
-00000c10: 9f74 c4b1 72c4 b170 2065 6469 7020 6765  .t..r..p edip ge
-00000c20: 7269 2064 c3b6 6e64 c3bc 722e 2e2a 0a0a  ri d..nd..r..*..
-00000c30: 3e20 4275 2070 726f 6772 616d c4b1 6e20  > Bu program..n 
-00000c40: 7961 7ac4 b16c 6d61 2076 6520 61c3 a7c4  yaz..lma ve a...
-00000c50: b16b 206b 6179 6e61 6b20 6b6f 646c 7520  .k kaynak kodlu 
-00000c60: 6f6c 6172 616b 2070 6179 6c61 c59f c4b1  olarak payla....
-00000c70: 6c6d 6120 616d 6163 c4b1 3a20 2a54 6172  lma amac..: *Tar
-00000c80: 6179 c4b1 63c4 b120 4f74 6f6d 6173 796f  ay..c.. Otomasyo
-00000c90: 6e6c 6172 c4b1 6ec4 b16e 2073 6562 6570  nlar..n..n sebep
-00000ca0: 206f 6c64 75c4 9f75 2020 2a2a 6765 7265   oldu..u  **gere
-00000cb0: 6b73 697a 206b 6179 6e61 6b20 74c3 bc6b  ksiz kaynak t..k
-00000cc0: 6574 696d 692a 2a20 7665 2020 2a2a 7a61  etimi** ve  **za
-00000cd0: 6d61 6e20 6b61 7962 c4b1 6ec4 b16e 2a2a  man kayb..n..n**
-00000ce0: 2020 c3b6 6ec3 bc6e 6520 6765 c3a7 6d65    ..n..ne ge..me
-00000cf0: 7965 2074 65c5 9f76 696b 2065 746d 656b  ye te..vik etmek
-00000d00: 7469 72e2 80a6 2a0a 0a3e 2054 6172 6179  tir...*..> Taray
-00000d10: c4b1 63c4 b120 4f74 6f6d 6173 796f 6e75  ..c.. Otomasyonu
-00000d20: 203a 202a 5b53 656c 656e 6975 6d20 4944   : *[Selenium ID
-00000d30: 455d 2868 7474 7073 3a2f 2f77 7777 2e73  E](https://www.s
-00000d40: 656c 656e 6975 6d2e 6465 762f 7365 6c65  elenium.dev/sele
-00000d50: 6e69 756d 2d69 6465 2f29 2a20 2a2a 2d2a  nium-ide/)* **-*
-00000d60: 2a20 2a5b 4b61 7461 6c6f 6e20 4175 746f  * *[Katalon Auto
-00000d70: 6d61 7469 6f6e 2052 6563 6f72 6465 725d  mation Recorder]
-00000d80: 2868 7474 7073 3a2f 2f77 7777 2e6b 6174  (https://www.kat
-00000d90: 616c 6f6e 2e63 6f6d 2f72 6573 6f75 7263  alon.com/resourc
-00000da0: 6573 2d63 656e 7465 722f 626c 6f67 2f6b  es-center/blog/k
-00000db0: 6174 616c 6f6e 2d61 7574 6f6d 6174 696f  atalon-automatio
-00000dc0: 6e2d 7265 636f 7264 6572 2f29 2a20 2a2a  n-recorder/)* **
-00000dd0: 2d2a 2a20 2a5b 4272 6f77 7365 7241 7574  -** *[BrowserAut
-00000de0: 6f6d 6174 696f 6e53 7475 6469 6f5d 2868  omationStudio](h
-00000df0: 7474 7073 3a2f 2f62 6162 6c6f 736f 6674  ttps://bablosoft
-00000e00: 2e63 6f6d 2f73 686f 702f 4272 6f77 7365  .com/shop/Browse
-00000e10: 7241 7574 6f6d 6174 696f 6e53 7475 6469  rAutomationStudi
-00000e20: 6f29 2a0a 0a3e 204b 6172 c59f c4b1 6c61  o)*..> Kar....la
-00000e30: c59f 74c4 b172 6d61 73c4 b120 3a20 2a2a  ..t..rmas.. : **
-00000e40: 5b53 656c 656e 6975 6d20 5653 2052 6571  [Selenium VS Req
-00000e50: 7565 7374 735d 2868 7474 7073 3a2f 2f77  uests](https://w
-00000e60: 7777 2e72 3130 2e6e 6574 2f6f 6666 2d74  ww.r10.net/off-t
-00000e70: 6f70 6963 2f32 3735 3134 3132 2d73 656c  opic/2751412-sel
-00000e80: 656e 6975 6d2d 7673 2d72 6571 7565 7374  enium-vs-request
-00000e90: 732e 6874 6d6c 292a 2a0a 0a23 2320 f09f  s.html)**..## ..
-00000ea0: 939d 2050 726f 6a65 20c4 b06c 6572 6c65  .. Proje ..lerle
-00000eb0: 6d65 7369 0a0a 2d20 e29c 8520 2a2a 5b40  mesi..- ... **[@
-00000ec0: 7261 6966 7079 5d28 6874 7470 733a 2f2f  raifpy](https://
-00000ed0: 6769 7468 7562 2e63 6f6d 2f72 6169 6670  github.com/raifp
-00000ee0: 7929 2a2a 202a 7461 7261 66c4 b16e 6461  y)** *taraf..nda
-00000ef0: 6e20 6b6f 646c 616e 6dc4 b1c5 9f20 7072  n kodlanm.... pr
-00000f00: 6f6a 656e 696e 2068 616e 7461 6c20 6269  ojenin hantal bi
-00000f10: 7220 6269 6c65 c59f 656e 6920 6974 696e  r bile..eni itin
-00000f20: 6179 6c61 2060 64c4 b17a 7a20 f09f 908d  ayla `d..zz ....
-00000f30: 6027 6c61 6e6d c4b1 c59f 74c4 b172 2e2e  `'lanm....t..r..
-00000f40: 2a0a 2d20 e29c 8520 2a2a 5365 6c65 6e69  *.- ... **Seleni
-00000f50: 756d 2a2a 202a 6261 c49f c4b1 6d6c c4b1  um** *ba....ml..
-00000f60: 6cc4 b1c4 9fc4 b16e 6461 6e20 646f 6c61  l......ndan dola
-00000f70: 79c4 b120 6861 6e74 616c 20c3 a761 6cc4  y.. hantal ..al.
-00000f80: b1c5 9f61 6e20 6b6f 6420 7961 70c4 b173  ...an kod yap..s
-00000f90: c4b1 2074 616d 616d 656e 2061 79c4 b16b  .. tamamen ay..k
-00000fa0: 6c61 6ec4 b170 2062 c3bc 74c3 bc6e 2069  lan..p b..t..n i
-00000fb0: c59f 2a20 6072 6571 7565 7374 7360 2a27  ..* `requests`*'
-00000fc0: 6520 7961 7074 c4b1 72c4 b16c c4b1 7020  e yapt..r..l..p 
-00000fd0: 6369 6464 6920 6d69 6b74 6172 6461 206b  ciddi miktarda k
-00000fe0: 6179 6e61 6b20 7665 207a 616d 616e 2074  aynak ve zaman t
-00000ff0: 6173 6172 7275 6675 2065 7474 6972 696c  asarrufu ettiril
-00001000: 6d69 c59f 7469 722e 2e2a 0a2d 20e2 9c85  mi..tir..*.- ...
-00001010: 202a 4b6f 6c61 7920 6572 69c5 9f69 6c65   *Kolay eri..ile
-00001020: 6269 6c69 7220 6f6c 6d61 73c4 b120 7665  bilir olmas.. ve
-00001030: 2069 6c68 616d 2079 6172 6174 6d61 73c4   ilham yaratmas.
-00001040: b120 69c3 a769 6e2a 202a 2a70 7970 692a  . i..in* **pypi*
-00001050: 2a20 2a64 6570 6f6c 6172 c4b1 6e61 2079  * *depolar..na y
-00001060: c3bc 6b6c 656e 6d69 c59f 7469 722e 2e2a  ..klenmi..tir..*
-00001070: 0a0a 2323 20f0 9f8c 9020 5465 6c69 6620  ..## .... Telif 
-00001080: 4861 6b6b c4b1 2076 6520 4c69 7361 6e73  Hakk.. ve Lisans
-00001090: 0a0a 2a20 2a43 6f70 7972 6967 6874 2028  ..* *Copyright (
-000010a0: 4329 2032 3032 3120 6279 2a20 5b6b 6579  C) 2021 by* [key
-000010b0: 6966 6c65 726f 6c73 756e 5d28 6874 7470  iflerolsun](http
-000010c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-000010d0: 6579 6966 6c65 726f 6c73 756e 2920 e29d  eyiflerolsun) ..
-000010e0: a4ef b88f efb8 8f0a 2a20 5b47 4e55 2047  ........* [GNU G
-000010f0: 454e 4552 414c 2050 5542 4c49 4320 4c49  ENERAL PUBLIC LI
-00001100: 4345 4e53 4520 5665 7273 696f 6e20 332c  CENSE Version 3,
-00001110: 2032 3920 4a75 6e65 2032 3030 375d 2868   29 June 2007](h
-00001120: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001130: 6d2f 6b65 7969 666c 6572 6f6c 7375 6e2f  m/keyiflerolsun/
-00001140: 6b65 7969 6655 7365 7242 6f74 2f62 6c6f  keyifUserBot/blo
-00001150: 622f 6d61 7374 6572 2f4c 4943 454e 5345  b/master/LICENSE
-00001160: 2920 2a4b 6fc5 9f75 6c6c 6172 c4b1 6e61  ) *Ko..ullar..na
-00001170: 2067 c3b6 7265 206c 6973 616e 736c 616e   g..re lisanslan
-00001180: 6dc4 b1c5 9f74 c4b1 722e 2e2a 0a0a 2323  m....t..r..*..##
-00001190: 20e2 99bb efb8 8f20 c4b0 6c65 7469 c59f   ...... ..leti..
-000011a0: 696d 0a0a 2a42 656e 696d 6c65 2069 6c65  im..*Benimle ile
-000011b0: 7469 c59f 696d 6520 6765 c3a7 6d65 6b20  ti..ime ge..mek 
-000011c0: 6973 7465 7273 656e 697a 2c20 2a2a 5465  isterseniz, **Te
-000011d0: 6c65 6772 616d 2a2a 2764 616e 206d 6573  legram**'dan mes
-000011e0: 616a 2067 c3b6 6e64 6572 6d65 6b74 656e  aj g..ndermekten
-000011f0: 20c3 a765 6b69 6e6d 6579 696e 3b2a 205b   ..ekinmeyin;* [
-00001200: 406b 6579 6966 6c65 726f 6c73 756e 5d28  @keyiflerolsun](
-00001210: 6874 7470 733a 2f2f 742e 6d65 2f6b 6579  https://t.me/key
-00001220: 6966 6c65 726f 6c73 756e 290a 0a23 2320  iflerolsun)..## 
-00001230: f09f 92b8 2042 61c4 9fc4 b1c5 9f20 5961  .... Ba...... Ya
-00001240: 700a 0a2a 2a5b e298 95ef b88f 204b 6168  p..**[...... Kah
-00001250: 7665 2049 736d 6172 6c61 5d28 6874 7470  ve Ismarla](http
-00001260: 733a 2f2f 4b65 6b69 6b41 6b61 6465 6d69  s://KekikAkademi
-00001270: 2e6f 7267 2f4b 6168 7665 292a 2a0a 0a23  .org/Kahve)**..#
-00001280: 230a 0a3e 202a 2a5b 404b 656b 696b 416b  #..> **[@KekikAk
-00001290: 6164 656d 695d 2868 7474 7073 3a2f 2f74  ademi](https://t
-000012a0: 2e6d 652f 4b65 6b69 6b41 6b61 6465 6d69  .me/KekikAkademi
-000012b0: 292a 2a20 2a69 c3a7 696e 2079 617a c4b1  )** *i..in yaz..
-000012c0: 6c6d c4b1 c59f 74c4 b172 2e2e 2a0a 0a0a  lm....t..r..*...
+000000a0: 756e 2f45 2d46 6174 7572 615f 536f 7267  un/E-Fatura_Sorg
+000000b0: 750a 4175 7468 6f72 3a20 6b65 7969 666c  u.Author: keyifl
+000000c0: 6572 6f6c 7375 6e0a 4175 7468 6f72 2d65  erolsun.Author-e
+000000d0: 6d61 696c 3a20 6b65 7969 666c 6572 6f6c  mail: keyiflerol
+000000e0: 7375 6e40 676d 6169 6c2e 636f 6d0a 4c69  sun@gmail.com.Li
+000000f0: 6365 6e73 653a 2047 504c 7633 2b0a 4b65  cense: GPLv3+.Ke
+00000100: 7977 6f72 6473 3a20 4254 4b53 6f72 6775  ywords: BTKSorgu
+00000110: 2c4b 656b 696b 416b 6164 656d 692c 6b65  ,KekikAkademi,ke
+00000120: 7969 666c 6572 6f6c 7375 6e0a 436c 6173  yiflerolsun.Clas
+00000130: 7369 6669 6572 3a20 4465 7665 6c6f 706d  sifier: Developm
+00000140: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
+00000150: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
+00000160: 626c 650a 436c 6173 7369 6669 6572 3a20  ble.Classifier: 
+00000170: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000180: 7070 726f 7665 6420 3a3a 2047 4e55 2047  pproved :: GNU G
+00000190: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
+000001a0: 6365 6e73 6520 7633 206f 7220 6c61 7465  cense v3 or late
+000001b0: 7220 2847 504c 7633 2b29 0a43 6c61 7373  r (GPLv3+).Class
+000001c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001e0: 7974 686f 6e20 3a3a 2033 0a52 6571 7569  ython :: 3.Requi
+000001f0: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+00000200: 3130 0a44 6573 6372 6970 7469 6f6e 2d43  10.Description-C
+00000210: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000220: 742f 6d61 726b 646f 776e 0a4c 6963 656e  t/markdown.Licen
+00000230: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000240: 0a0a 2320 f09f 948d 2042 544b 536f 7267  ..# .... BTKSorg
+00000250: 750a 0a21 5b52 6570 6f20 426f 7975 7475  u..![Repo Boyutu
+00000260: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000270: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000280: 7265 706f 2d73 697a 652f 6b65 7969 666c  repo-size/keyifl
+00000290: 6572 6f6c 7375 6e2f 4254 4b53 6f72 6775  erolsun/BTKSorgu
+000002a0: 3f6c 6f67 6f3d 6769 7426 6c6f 676f 436f  ?logo=git&logoCo
+000002b0: 6c6f 723d 7768 6974 6529 0a21 5b47 c3b6  lor=white).![G..
+000002c0: 72c3 bc6e 74c3 bc6c 656e 6d65 5d28 6874  r..nt..lenme](ht
+000002d0: 7470 733a 2f2f 6869 7473 2e73 6565 796f  tps://hits.seeyo
+000002e0: 7566 6172 6d2e 636f 6d2f 6170 692f 636f  ufarm.com/api/co
+000002f0: 756e 742f 696e 6372 2f62 6164 6765 2e73  unt/incr/badge.s
+00000300: 7667 3f75 726c 3d68 7474 7073 3a2f 2f67  vg?url=https://g
+00000310: 6974 6875 622e 636f 6d2f 6b65 7969 666c  ithub.com/keyifl
+00000320: 6572 6f6c 7375 6e2f 4254 4b53 6f72 6775  erolsun/BTKSorgu
+00000330: 2674 6974 6c65 3d47 c3b6 72c3 bc6e 74c3  &title=G..r..nt.
+00000340: bc6c 656e 6d65 290a 3c61 2068 7265 663d  .lenme).<a href=
+00000350: 2268 7474 7073 3a2f 2f4b 656b 696b 416b  "https://KekikAk
+00000360: 6164 656d 692e 6f72 672f 4b61 6876 6522  ademi.org/Kahve"
+00000370: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000380: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000390: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000003a0: 6f2f 6261 6467 652f e298 95ef b88f 2d4b  o/badge/......-K
+000003b0: 6168 7665 2049 736d 6172 6c61 2d66 6664  ahve Ismarla-ffd
+000003c0: 6430 3022 2074 6974 6c65 3d22 e298 95ef  d00" title="....
+000003d0: b88f 204b 6168 7665 2049 736d 6172 6c61  .. Kahve Ismarla
+000003e0: 2220 7374 796c 653d 2270 6164 6469 6e67  " style="padding
+000003f0: 2d6c 6566 743a 3570 783b 223e 3c2f 613e  -left:5px;"></a>
+00000400: 0a0a 215b 5079 7468 6f6e 2056 6572 7369  ..![Python Versi
+00000410: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
+00000420: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000430: 7079 7665 7273 696f 6e73 2f42 544b 536f  pyversions/BTKSo
+00000440: 7267 753f 6c6f 676f 3d70 7974 686f 6e26  rgu?logo=python&
+00000450: 6c6f 676f 436f 6c6f 723d 7768 6974 6529  logoColor=white)
+00000460: 0a21 5b4c 6963 656e 7365 5d28 6874 7470  .![License](http
+00000470: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000480: 696f 2f70 7970 692f 6c2f 4254 4b53 6f72  io/pypi/l/BTKSor
+00000490: 6775 3f6c 6f67 6f3d 676e 7526 6c6f 676f  gu?logo=gnu&logo
+000004a0: 436f 6c6f 723d 7768 6974 6529 0a21 5b53  Color=white).![S
+000004b0: 7461 7475 735d 2868 7474 7073 3a2f 2f69  tatus](https://i
+000004c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000004d0: 7069 2f73 7461 7475 732f 4254 4b53 6f72  pi/status/BTKSor
+000004e0: 6775 3f6c 6f67 6f3d 7769 6e64 6f77 7374  gu?logo=windowst
+000004f0: 6572 6d69 6e61 6c26 6c6f 676f 436f 6c6f  erminal&logoColo
+00000500: 723d 7768 6974 6529 0a0a 215b 5079 5049  r=white)..![PyPI
+00000510: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000520: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000530: 4254 4b53 6f72 6775 3f6c 6f67 6f3d 7079  BTKSorgu?logo=py
+00000540: 7069 266c 6f67 6f43 6f6c 6f72 3d77 6869  pi&logoColor=whi
+00000550: 7465 290a 215b 5079 5049 202d 2044 6f77  te).![PyPI - Dow
+00000560: 6e6c 6f61 6473 5d28 6874 7470 733a 2f2f  nloads](https://
+00000570: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000580: 7970 692f 646d 2f42 544b 536f 7267 753f  ypi/dm/BTKSorgu?
+00000590: 6c6f 676f 3d70 7970 6926 6c6f 676f 436f  logo=pypi&logoCo
+000005a0: 6c6f 723d 7768 6974 6529 0a21 5b50 7950  lor=white).![PyP
+000005b0: 4920 2d20 5768 6565 6c5d 2868 7474 7073  I - Wheel](https
+000005c0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000005d0: 6f2f 7079 7069 2f77 6865 656c 2f42 544b  o/pypi/wheel/BTK
+000005e0: 536f 7267 753f 6c6f 676f 3d70 7970 6926  Sorgu?logo=pypi&
+000005f0: 6c6f 676f 436f 6c6f 723d 7768 6974 6529  logoColor=white)
+00000600: 0a0a 5b21 5b50 7950 4920 59c3 bc6b 6c65  ..[![PyPI Y..kle
+00000610: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000620: 2e63 6f6d 2f6b 6579 6966 6c65 726f 6c73  .com/keyiflerols
+00000630: 756e 2f42 544b 536f 7267 752f 6163 7469  un/BTKSorgu/acti
+00000640: 6f6e 732f 776f 726b 666c 6f77 732f 4b65  ons/workflows/Ke
+00000650: 6b69 6b46 6c6f 772e 796d 6c2f 6261 6467  kikFlow.yml/badg
+00000660: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000670: 6769 7468 7562 2e63 6f6d 2f6b 6579 6966  github.com/keyif
+00000680: 6c65 726f 6c73 756e 2f42 544b 536f 7267  lerolsun/BTKSorg
+00000690: 752f 6163 7469 6f6e 732f 776f 726b 666c  u/actions/workfl
+000006a0: 6f77 732f 4b65 6b69 6b46 6c6f 772e 796d  ows/KekikFlow.ym
+000006b0: 6c29 0a0a 2a48 6564 6566 2077 6562 7369  l)..*Hedef websi
+000006c0: 7465 7369 6e69 6e20 4254 4b20 5461 7261  tesinin BTK Tara
+000006d0: 66c4 b16e 6461 6e20 4572 69c5 9f69 6d20  f..ndan Eri..im 
+000006e0: 456e 6765 6c69 2053 6f72 6775 7375 2e2e  Engeli Sorgusu..
+000006f0: 2a0a 0a5b 215b 466f 7254 6865 4261 6467  *..[![ForTheBadg
+00000700: 6520 6d61 6465 2d77 6974 682d 7079 7468  e made-with-pyth
+00000710: 6f6e 5d28 6874 7470 733a 2f2f 466f 7254  on](https://ForT
+00000720: 6865 4261 6467 652e 636f 6d2f 696d 6167  heBadge.com/imag
+00000730: 6573 2f62 6164 6765 732f 6d61 6465 2d77  es/badges/made-w
+00000740: 6974 682d 7079 7468 6f6e 2e73 7667 295d  ith-python.svg)]
+00000750: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
+00000760: 686f 6e2e 6f72 672f 290a 5b21 5b46 6f72  hon.org/).[![For
+00000770: 5468 6542 6164 6765 2062 7569 6c74 2d77  TheBadge built-w
+00000780: 6974 682d 6c6f 7665 5d28 6874 7470 733a  ith-love](https:
+00000790: 2f2f 466f 7254 6865 4261 6467 652e 636f  //ForTheBadge.co
+000007a0: 6d2f 696d 6167 6573 2f62 6164 6765 732f  m/images/badges/
+000007b0: 6275 696c 742d 7769 7468 2d6c 6f76 652e  built-with-love.
+000007c0: 7376 6729 5d28 6874 7470 733a 2f2f 4769  svg)](https://Gi
+000007d0: 7448 7562 2e63 6f6d 2f6b 6579 6966 6c65  tHub.com/keyifle
+000007e0: 726f 6c73 756e 2f29 0a0a 2323 20f0 9f9a  rolsun/)..## ...
+000007f0: 8020 4b75 7275 6c75 6d0a 0a60 6060 6261  . Kurulum..```ba
+00000800: 7368 0a23 2059 c3bc 6b6c 656d 656b 0a70  sh.# Y..klemek.p
+00000810: 6970 2069 6e73 7461 6c6c 2042 544b 536f  ip install BTKSo
+00000820: 7267 750a 0a23 2047 c3bc 6e63 656c 6c65  rgu..# G..ncelle
+00000830: 6d65 6b0a 7069 7020 696e 7374 616c 6c20  mek.pip install 
+00000840: 2d55 2042 544b 536f 7267 750a 6060 600a  -U BTKSorgu.```.
+00000850: 0a23 2320 f09f 939d 204b 756c 6c61 6ec4  .## .... Kullan.
+00000860: b16d 0a0a 6060 6070 7974 686f 6e0a 6672  .m..```python.fr
+00000870: 6f6d 2042 544b 536f 7267 7520 696d 706f  om BTKSorgu impo
+00000880: 7274 2042 544b 536f 7267 750a 6672 6f6d  rt BTKSorgu.from
+00000890: 2074 696d 6520 2020 2020 696d 706f 7274   time     import
+000008a0: 2074 696d 650a 0a62 6173 6c61 203d 2074   time..basla = t
+000008b0: 696d 6528 290a 7072 696e 7428 4254 4b53  ime().print(BTKS
+000008c0: 6f72 6775 2822 7265 6474 7562 652e 636f  orgu("redtube.co
+000008d0: 6d22 2929 0a20 2020 2023 20c2 bb20 7265  m")).    # .. re
+000008e0: 6474 7562 652e 636f 6d2c 2033 302f 3031  dtube.com, 30/01
+000008f0: 2f32 3030 3820 7461 7269 686c 6920 7665  /2008 tarihli ve
+00000900: 2034 3130 2e30 312e 3032 2e32 3030 382d   410.01.02.2008-
+00000910: 3032 3831 3035 2073 6179 c4b1 6cc4 b120  028105 say..l.. 
+00000920: 5465 6c65 6b6f 6dc3 bc6e 696b 6173 796f  Telekom..nikasyo
+00000930: 6e20 c4b0 6c65 7469 c59f 696d 2042 61c5  n ..leti..im Ba.
+00000940: 9f6b 616e 6cc4 b1c4 9fc4 b120 6b61 7261  .kanl...... kara
+00000950: 72c4 b179 6c61 2065 7269 c59f 696d 6520  r..yla eri..ime 
+00000960: 656e 6765 6c6c 656e 6d69 c59f 7469 722e  engellenmi..tir.
+00000970: 0a70 7269 6e74 2842 544b 536f 7267 7528  .print(BTKSorgu(
+00000980: 226b 656b 696b 616b 6164 656d 692e 6f72  "kekikakademi.or
+00000990: 6722 2929 0a20 2020 2023 20c2 bb20 4269  g")).    # .. Bi
+000009a0: 6c67 6920 5465 6b6e 6f6c 6f6a 696c 6572  lgi Teknolojiler
+000009b0: 6920 7665 20c4 b06c 6574 69c5 9f69 6d20  i ve ..leti..im 
+000009c0: 4b75 7275 6d75 2074 6172 6166 c4b1 6e64  Kurumu taraf..nd
+000009d0: 616e 2075 7967 756c 616e 616e 2062 6972  an uygulanan bir
+000009e0: 206b 6172 6172 2062 756c 756e 616d 6164   karar bulunamad
+000009f0: c4b1 2e0a 7072 696e 7428 4254 4b53 6f72  ....print(BTKSor
+00000a00: 6775 2822 786e 7878 2e63 6f6d 2229 290a  gu("xnxx.com")).
+00000a10: 2020 2020 2320 c2bb 2078 6e78 782e 636f      # .. xnxx.co
+00000a20: 6d2c 2032 332f 3032 2f32 3030 3820 7461  m, 23/02/2008 ta
+00000a30: 7269 686c 6920 7665 2034 3130 2e30 312e  rihli ve 410.01.
+00000a40: 3032 2e32 3030 382d 3035 3430 3033 2073  02.2008-054003 s
+00000a50: 6179 c4b1 6cc4 b120 5465 6c65 6b6f 6dc3  ay..l.. Telekom.
+00000a60: bc6e 696b 6173 796f 6e20 c4b0 6c65 7469  .nikasyon ..leti
+00000a70: c59f 696d 2042 61c5 9f6b 616e 6cc4 b1c4  ..im Ba..kanl...
+00000a80: 9fc4 b120 6b61 7261 72c4 b179 6c61 2065  ... karar..yla e
+00000a90: 7269 c59f 696d 6520 656e 6765 6c6c 656e  ri..ime engellen
+00000aa0: 6d69 c59f 7469 722e 0a62 6974 6972 203d  mi..tir..bitir =
+00000ab0: 2074 696d 6528 290a 0a70 7269 6e74 2862   time()..print(b
+00000ac0: 6974 6972 2d62 6173 6c61 290a 2020 2020  itir-basla).    
+00000ad0: 2320 c2bb 2038 2e33 3532 3736 3635 3133  # .. 8.352766513
+00000ae0: 3832 3434 3633 0a60 6060 0a0a 6060 6062  824463.```..```b
+00000af0: 6173 680a 4254 4b53 6f72 6775 206b 6579  ash.BTKSorgu key
+00000b00: 6966 6c65 726f 6c73 756e 2e64 6576 0a0a  iflerolsun.dev..
+00000b10: 2320 3e20 4269 6c67 6920 5465 6b6e 6f6c  # > Bilgi Teknol
+00000b20: 6f6a 696c 6572 6920 7665 20c4 b06c 6574  ojileri ve ..let
+00000b30: 69c5 9f69 6d20 4b75 7275 6d75 2074 6172  i..im Kurumu tar
+00000b40: 6166 c4b1 6e64 616e 2075 7967 756c 616e  af..ndan uygulan
+00000b50: 616e 2062 6972 206b 6172 6172 2062 756c  an bir karar bul
+00000b60: 756e 616d 6164 c4b1 2e0a 6060 600a 0a23  unamad....```..#
+00000b70: 2320 f09f 9496 2050 726f 6772 616d 2041  # .... Program A
+00000b80: 6bc4 b1c5 9f20 c59e 656d 6173 c4b1 0a0a  k.... ..emas....
+00000b90: 312e 202a 4f74 7572 756d 2042 61c5 9f6c  1. *Oturum Ba..l
+00000ba0: 6174 2c2a 0a32 2e20 2a5b 6874 7470 733a  at,*.2. *[https:
+00000bb0: 2f2f 696e 7465 726e 6574 322e 6274 6b2e  //internet2.btk.
+00000bc0: 676f 762e 7472 5d28 6874 7470 733a 2f2f  gov.tr](https://
+00000bd0: 696e 7465 726e 6574 322e 6274 6b2e 676f  internet2.btk.go
+00000be0: 762e 7472 2f29 2061 6472 6573 696e 6520  v.tr/) adresine 
+00000bf0: 79c3 b66e 6c65 6e64 6972 6d65 6c65 7269  y..nlendirmeleri
+00000c00: 206b 6162 756c 2065 6465 7265 6b20 6769   kabul ederek gi
+00000c10: 743a 206b 7572 6162 6979 656c 6572 6920  t: kurabiyeleri 
+00000c20: 7965 2c2a 0a33 2e20 2a44 c3b6 6e65 6e20  ye,*.3. *D..nen 
+00000c30: 6b61 796e 616b 206b 6f64 756e 6461 6e20  kaynak kodundan 
+00000c40: 646f c49f 7275 6c61 6d61 2072 6573 6d69  do..rulama resmi
+00000c50: 6e69 2069 6e64 6972 2c2a 0a34 2e20 2a44  ni indir,*.4. *D
+00000c60: 6fc4 9f72 756c 616d 6120 7265 736d 696e  o..rulama resmin
+00000c70: 6920 4f43 5220 696c 6520 6861 7266 6c65  i OCR ile harfle
+00000c80: 7265 2064 c3b6 6ec3 bcc5 9f74 c3bc 722c  re d..n....t..r,
+00000c90: 2062 6fc5 9f6c 756b 6c61 72c4 b120 7369   bo..luklar.. si
+00000ca0: 6c2c 2a0a 352e 202a 536f 7267 7520 6164  l,*.5. *Sorgu ad
+00000cb0: 7265 7369 6e69 206f 6b75 6475 c49f 756e  resini okudu..un
+00000cc0: 2064 6fc4 9f72 756c 616d 6120 6b6f 6475   do..rulama kodu
+00000cd0: 796c 6120 6269 726c 696b 7465 2070 6f73  yla birlikte pos
+00000ce0: 7420 6174 2c2a 0a36 2e20 2a44 c3b6 6e65  t at,*.6. *D..ne
+00000cf0: 6e20 7961 6ec4 b174 c4b1 2061 7972 c4b1  n yan..t.. ayr..
+00000d00: c59f 74c4 b172 c4b1 7020 6564 6970 2067  ..t..r..p edip g
+00000d10: 6572 6920 64c3 b66e 64c3 bc72 2e2e 2a0a  eri d..nd..r..*.
+00000d20: 0a3e 2042 7520 7072 6f67 7261 6dc4 b16e  .> Bu program..n
+00000d30: 2079 617a c4b1 6c6d 6120 7665 2061 c3a7   yaz..lma ve a..
+00000d40: c4b1 6b20 6b61 796e 616b 206b 6f64 6c75  ..k kaynak kodlu
+00000d50: 206f 6c61 7261 6b20 7061 796c 61c5 9fc4   olarak payla...
+00000d60: b16c 6d61 2061 6d61 63c4 b13a 202a 5461  .lma amac..: *Ta
+00000d70: 7261 79c4 b163 c4b1 204f 746f 6d61 7379  ray..c.. Otomasy
+00000d80: 6f6e 6c61 72c4 b16e c4b1 6e20 7365 6265  onlar..n..n sebe
+00000d90: 7020 6f6c 6475 c49f 7520 202a 2a67 6572  p oldu..u  **ger
+00000da0: 656b 7369 7a20 6b61 796e 616b 2074 c3bc  eksiz kaynak t..
+00000db0: 6b65 7469 6d69 2a2a 2076 6520 202a 2a7a  ketimi** ve  **z
+00000dc0: 616d 616e 206b 6179 62c4 b16e c4b1 6e2a  aman kayb..n..n*
+00000dd0: 2a20 20c3 b66e c3bc 6e65 2067 65c3 a76d  *  ..n..ne ge..m
+00000de0: 6579 6520 7465 c59f 7669 6b20 6574 6d65  eye te..vik etme
+00000df0: 6b74 6972 e280 a62a 0a0a 3e20 5461 7261  ktir...*..> Tara
+00000e00: 79c4 b163 c4b1 204f 746f 6d61 7379 6f6e  y..c.. Otomasyon
+00000e10: 7520 3a20 2a5b 5365 6c65 6e69 756d 2049  u : *[Selenium I
+00000e20: 4445 5d28 6874 7470 733a 2f2f 7777 772e  DE](https://www.
+00000e30: 7365 6c65 6e69 756d 2e64 6576 2f73 656c  selenium.dev/sel
+00000e40: 656e 6975 6d2d 6964 652f 292a 202a 2a2d  enium-ide/)* **-
+00000e50: 2a2a 202a 5b4b 6174 616c 6f6e 2041 7574  ** *[Katalon Aut
+00000e60: 6f6d 6174 696f 6e20 5265 636f 7264 6572  omation Recorder
+00000e70: 5d28 6874 7470 733a 2f2f 7777 772e 6b61  ](https://www.ka
+00000e80: 7461 6c6f 6e2e 636f 6d2f 7265 736f 7572  talon.com/resour
+00000e90: 6365 732d 6365 6e74 6572 2f62 6c6f 672f  ces-center/blog/
+00000ea0: 6b61 7461 6c6f 6e2d 6175 746f 6d61 7469  katalon-automati
+00000eb0: 6f6e 2d72 6563 6f72 6465 722f 292a 202a  on-recorder/)* *
+00000ec0: 2a2d 2a2a 202a 5b42 726f 7773 6572 4175  *-** *[BrowserAu
+00000ed0: 746f 6d61 7469 6f6e 5374 7564 696f 5d28  tomationStudio](
+00000ee0: 6874 7470 733a 2f2f 6261 626c 6f73 6f66  https://bablosof
+00000ef0: 742e 636f 6d2f 7368 6f70 2f42 726f 7773  t.com/shop/Brows
+00000f00: 6572 4175 746f 6d61 7469 6f6e 5374 7564  erAutomationStud
+00000f10: 696f 292a 0a0a 3e20 4b61 72c5 9fc4 b16c  io)*..> Kar....l
+00000f20: 61c5 9f74 c4b1 726d 6173 c4b1 203a 202a  a..t..rmas.. : *
+00000f30: 2a5b 5365 6c65 6e69 756d 2056 5320 5265  *[Selenium VS Re
+00000f40: 7175 6573 7473 5d28 6874 7470 733a 2f2f  quests](https://
+00000f50: 7777 772e 7231 302e 6e65 742f 6f66 662d  www.r10.net/off-
+00000f60: 746f 7069 632f 3237 3531 3431 322d 7365  topic/2751412-se
+00000f70: 6c65 6e69 756d 2d76 732d 7265 7175 6573  lenium-vs-reques
+00000f80: 7473 2e68 746d 6c29 2a2a 0a0a 2323 20f0  ts.html)**..## .
+00000f90: 9f93 9d20 5072 6f6a 6520 c4b0 6c65 726c  ... Proje ..lerl
+00000fa0: 656d 6573 690a 0a2d 20e2 9c85 202a 2a5b  emesi..- ... **[
+00000fb0: 4072 6169 6670 795d 2868 7474 7073 3a2f  @raifpy](https:/
+00000fc0: 2f67 6974 6875 622e 636f 6d2f 7261 6966  /github.com/raif
+00000fd0: 7079 292a 2a20 2a74 6172 6166 c4b1 6e64  py)** *taraf..nd
+00000fe0: 616e 206b 6f64 6c61 6e6d c4b1 c59f 2070  an kodlanm.... p
+00000ff0: 726f 6a65 6e69 6e20 6861 6e74 616c 2062  rojenin hantal b
+00001000: 6972 2062 696c 65c5 9f65 6e69 2069 7469  ir bile..eni iti
+00001010: 6e61 796c 6120 6064 c4b1 7a7a 20f0 9f90  nayla `d..zz ...
+00001020: 8d60 276c 616e 6dc4 b1c5 9f74 c4b1 722e  .`'lanm....t..r.
+00001030: 2e2a 0a2d 20e2 9c85 202a 2a53 656c 656e  .*.- ... **Selen
+00001040: 6975 6d2a 2a20 2a62 61c4 9fc4 b16d 6cc4  ium** *ba....ml.
+00001050: b16c c4b1 c49f c4b1 6e64 616e 2064 6f6c  .l......ndan dol
+00001060: 6179 c4b1 2068 616e 7461 6c20 c3a7 616c  ay.. hantal ..al
+00001070: c4b1 c59f 616e 206b 6f64 2079 6170 c4b1  ....an kod yap..
+00001080: 73c4 b120 7461 6d61 6d65 6e20 6179 c4b1  s.. tamamen ay..
+00001090: 6b6c 616e c4b1 7020 62c3 bc74 c3bc 6e20  klan..p b..t..n 
+000010a0: 69c5 9f2a 2060 7265 7175 6573 7473 602a  i..* `requests`*
+000010b0: 2765 2079 6170 74c4 b172 c4b1 6cc4 b170  'e yapt..r..l..p
+000010c0: 2063 6964 6469 206d 696b 7461 7264 6120   ciddi miktarda 
+000010d0: 6b61 796e 616b 2076 6520 7a61 6d61 6e20  kaynak ve zaman 
+000010e0: 7461 7361 7272 7566 7520 6574 7469 7269  tasarrufu ettiri
+000010f0: 6c6d 69c5 9f74 6972 2e2e 2a0a 2d20 e29c  lmi..tir..*.- ..
+00001100: 8520 2a4b 6f6c 6179 2065 7269 c59f 696c  . *Kolay eri..il
+00001110: 6562 696c 6972 206f 6c6d 6173 c4b1 2076  ebilir olmas.. v
+00001120: 6520 696c 6861 6d20 7961 7261 746d 6173  e ilham yaratmas
+00001130: c4b1 2069 c3a7 696e 2a20 2a2a 7079 7069  .. i..in* **pypi
+00001140: 2a2a 202a 6465 706f 6c61 72c4 b16e 6120  ** *depolar..na 
+00001150: 79c3 bc6b 6c65 6e6d 69c5 9f74 6972 2e2e  y..klenmi..tir..
+00001160: 2a0a 0a23 2320 f09f 8c90 2054 656c 6966  *..## .... Telif
+00001170: 2048 616b 6bc4 b120 7665 204c 6973 616e   Hakk.. ve Lisan
+00001180: 730a 0a2a 202a 436f 7079 7269 6768 7420  s..* *Copyright 
+00001190: 2843 2920 3230 3233 2062 792a 205b 6b65  (C) 2023 by* [ke
+000011a0: 7969 666c 6572 6f6c 7375 6e5d 2868 7474  yiflerolsun](htt
+000011b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000011c0: 6b65 7969 666c 6572 6f6c 7375 6e29 20e2  keyiflerolsun) .
+000011d0: 9da4 efb8 8fef b88f 0a2a 205b 474e 5520  .........* [GNU 
+000011e0: 4745 4e45 5241 4c20 5055 424c 4943 204c  GENERAL PUBLIC L
+000011f0: 4943 454e 5345 2056 6572 7369 6f6e 2033  ICENSE Version 3
+00001200: 2c20 3239 204a 756e 6520 3230 3037 5d28  , 29 June 2007](
+00001210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001220: 6f6d 2f6b 6579 6966 6c65 726f 6c73 756e  om/keyiflerolsun
+00001230: 2f42 544b 536f 7267 752f 626c 6f62 2f6d  /BTKSorgu/blob/m
+00001240: 6173 7465 722f 4c49 4345 4e53 4529 202a  aster/LICENSE) *
+00001250: 4b6f c59f 756c 6c61 72c4 b16e 6120 67c3  Ko..ullar..na g.
+00001260: b672 6520 6c69 7361 6e73 6c61 6e6d c4b1  .re lisanslanm..
+00001270: c59f 74c4 b172 2e2e 2a0a 0a23 2320 e299  ..t..r..*..## ..
+00001280: bbef b88f 20c4 b06c 6574 69c5 9f69 6d0a  .... ..leti..im.
+00001290: 0a2a 4265 6e69 6d6c 6520 696c 6574 69c5  .*Benimle ileti.
+000012a0: 9f69 6d65 2067 65c3 a76d 656b 2069 7374  .ime ge..mek ist
+000012b0: 6572 7365 6e69 7a2c 202a 2a54 656c 6567  erseniz, **Teleg
+000012c0: 7261 6d2a 2a27 6461 6e20 6d65 7361 6a20  ram**'dan mesaj 
+000012d0: 67c3 b66e 6465 726d 656b 7465 6e20 c3a7  g..ndermekten ..
+000012e0: 656b 696e 6d65 7969 6e3b 2a20 5b40 6b65  ekinmeyin;* [@ke
+000012f0: 7969 666c 6572 6f6c 7375 6e5d 2868 7474  yiflerolsun](htt
+00001300: 7073 3a2f 2f74 2e6d 652f 4b65 6b69 6b4b  ps://t.me/KekikK
+00001310: 6168 7665 290a 0a23 2320 f09f 92b8 2042  ahve)..## .... B
+00001320: 61c4 9fc4 b1c5 9f20 5961 700a 0a2a 2a5b  a...... Yap..**[
+00001330: e298 95ef b88f 204b 6168 7665 2049 736d  ...... Kahve Ism
+00001340: 6172 6c61 5d28 6874 7470 733a 2f2f 4b65  arla](https://Ke
+00001350: 6b69 6b41 6b61 6465 6d69 2e6f 7267 2f4b  kikAkademi.org/K
+00001360: 6168 7665 292a 2a0a 0a23 230a 0a3e 202a  ahve)**..##..> *
+00001370: 2a5b 404b 656b 696b 416b 6164 656d 695d  *[@KekikAkademi]
+00001380: 2868 7474 7073 3a2f 2f74 2e6d 652f 4b65  (https://t.me/Ke
+00001390: 6b69 6b41 6b61 6465 6d69 292a 2a20 2a69  kikAkademi)** *i
+000013a0: c3a7 696e 2079 617a c4b1 6c6d c4b1 c59f  ..in yaz..lm....
+000013b0: 74c4 b172 2e2e 2a0a                      t..r..*.
```

### Comparing `BTKSorgu-0.1.5/setup.py` & `BTKSorgu-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
 from setuptools import setup
-from io import open
+from io         import open
 
 setup(
-    author       = 'keyiflerolsun',
-    author_email = 'keyiflerolsun@gmail.com',
-
-    packages     = ['BTKSorgu'],
-
-    name         = 'BTKSorgu',
-    version      = '0.1.5',
-    url          = 'https://github.com/keyiflerolsun/BTKSorgu',
-    description  = 'Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu',
-    keywords     = ['BTKSorgu', 'KekikAkademi', 'keyiflerolsun'],
-
-    long_description_content_type   = "text/markdown",
-    long_description                = "".join(open("README.md", encoding="utf-8").readlines()),
-    include_package_data            = True,
-
-    license     = 'GPLv3+',
-    classifiers = [
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-        'Programming Language :: Python :: 3'
+    # ? Genel Bilgiler
+    name         = "BTKSorgu",
+    version      = "1.0.1",
+    url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
+    description  = "Hedef websitesinin BTK Tarafından Erişim Engeli Sorgusu",
+    keywords     = ["BTKSorgu", "KekikAkademi", "keyiflerolsun"],
+
+    author       = "keyiflerolsun",
+    author_email = "keyiflerolsun@gmail.com",
+
+    license      = "GPLv3+",
+    classifiers  = [
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Programming Language :: Python :: 3"
     ],
 
-    python_requires     = '>=3.6',
-    install_requires    = [
+    # ? Paket Bilgileri
+    packages         = ["BTKSorgu"],
+    python_requires  = ">=3.10",
+    install_requires = [
+        "setuptools",
+        "wheel",
+        "Kekik",
         "requests",
         "parsel",
+        "regex",
         "Pillow",
         "pytesseract"
-    ]
+    ],
+
+    # ? Konsoldan Çalıştırılabilir
+    entry_points = {
+        "console_scripts": [
+            "BTKSorgu = BTKSorgu.konsol:basla",
+        ]
+    },
+
+    # ? PyPI Bilgileri
+    long_description_content_type = "text/markdown",
+    long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
+    include_package_data          = True
 )
```

