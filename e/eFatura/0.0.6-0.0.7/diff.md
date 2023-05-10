# Comparing `tmp/eFatura-0.0.6.tar.gz` & `tmp/eFatura-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-0.0.6.tar", last modified: Wed May 10 12:42:57 2023, max compression
+gzip compressed data, was "eFatura-0.0.7.tar", last modified: Wed May 10 12:55:03 2023, max compression
```

## Comparing `eFatura-0.0.6.tar` & `eFatura-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:42:57.053460 eFatura-0.0.6/
--rw-r--r--   0 sancak    (1000) sancak    (1000)       27 2023-05-10 08:30:46.000000 eFatura-0.0.6/MANIFEST.in
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2831 2023-05-10 12:42:57.053460 eFatura-0.0.6/PKG-INFO
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2252 2023-05-10 12:42:19.000000 eFatura-0.0.6/README.md
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:42:57.050127 eFatura-0.0.6/eFatura/
--rw-r--r--   0 sancak    (1000) sancak    (1000)      785 2023-05-10 11:53:39.000000 eFatura-0.0.6/eFatura/Oturum.py
--rw-r--r--   0 sancak    (1000) sancak    (1000)     1448 2023-05-10 12:42:19.000000 eFatura-0.0.6/eFatura/__init__.py
-drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:42:57.053460 eFatura-0.0.6/eFatura.egg-info/
--rw-r--r--   0 sancak    (1000) sancak    (1000)     2831 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 sancak    (1000) sancak    (1000)      222 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)        1 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)       53 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/requires.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)        8 2023-05-10 12:42:56.000000 eFatura-0.0.6/eFatura.egg-info/top_level.txt
--rw-r--r--   0 sancak    (1000) sancak    (1000)       38 2023-05-10 12:42:57.053460 eFatura-0.0.6/setup.cfg
--rw-r--r--   0 sancak    (1000) sancak    (1000)     1188 2023-05-10 12:42:38.000000 eFatura-0.0.6/setup.py
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:55:03.767028 eFatura-0.0.7/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       27 2023-05-10 08:30:46.000000 eFatura-0.0.7/MANIFEST.in
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2831 2023-05-10 12:55:03.767028 eFatura-0.0.7/PKG-INFO
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2252 2023-05-10 12:42:19.000000 eFatura-0.0.7/README.md
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:55:03.763695 eFatura-0.0.7/eFatura/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)      785 2023-05-10 11:53:39.000000 eFatura-0.0.7/eFatura/Oturum.py
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     1448 2023-05-10 12:42:19.000000 eFatura-0.0.7/eFatura/__init__.py
+drwxr-xr-x   0 sancak    (1000) sancak    (1000)        0 2023-05-10 12:55:03.767028 eFatura-0.0.7/eFatura.egg-info/
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     2831 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 sancak    (1000) sancak    (1000)      222 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)        1 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       53 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/requires.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)        8 2023-05-10 12:55:03.000000 eFatura-0.0.7/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 sancak    (1000) sancak    (1000)       38 2023-05-10 12:55:03.767028 eFatura-0.0.7/setup.cfg
+-rw-r--r--   0 sancak    (1000) sancak    (1000)     1176 2023-05-10 12:54:46.000000 eFatura-0.0.7/setup.py
```

### Comparing `eFatura-0.0.6/PKG-INFO` & `eFatura-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.6
+Version: 0.0.7
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
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.6 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.7 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
 Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
```

### Comparing `eFatura-0.0.6/README.md` & `eFatura-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.6/eFatura/Oturum.py` & `eFatura-0.0.7/eFatura/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.6/eFatura/__init__.py` & `eFatura-0.0.7/eFatura/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-0.0.6/eFatura.egg-info/PKG-INFO` & `eFatura-0.0.7/eFatura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 0.0.6
+Version: 0.0.7
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
-Metadata-Version: 2.1 Name: eFatura Version: 0.0.6 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 0.0.7 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords: MÃ¼kellef
 Sorgu,eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð E-Fatura
```

### Comparing `eFatura-0.0.6/setup.py` & `eFatura-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 setup(
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
     packages     = ["eFatura"],
 
     name         = "eFatura",
-    version      = "0.0.6",
+    version      = "0.0.7",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["Mükellef Sorgu", "eFatura", "KekikAkademi", "keyiflerolsun"],
 
-    long_description_content_type   = "text/markdown",
-    long_description                = "".join(open("README.md", encoding="utf-8").readlines()),
-    include_package_data            = True,
+    long_description_content_type = "text/markdown",
+    long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
+    include_package_data          = True,
 
     license     = "GPLv3+",
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Programming Language :: Python :: 3"
     ],
 
-    python_requires     = ">=3.10",
-    install_requires    = [
+    python_requires  = ">=3.10",
+    install_requires = [
         "setuptools",
         "wheel",
         "requests",
         "urllib3",
         "Pillow",
         "pytesseract"
     ]
```

