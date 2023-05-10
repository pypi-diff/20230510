# Comparing `tmp/plover_spanish_mqd-2.1.6.tar.gz` & `tmp/plover_spanish_mqd-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover_spanish_mqd-2.1.6.tar", last modified: Wed Feb 22 08:06:16 2023, max compression
+gzip compressed data, was "plover_spanish_mqd-2.1.7.tar", last modified: Wed May 10 08:01:26 2023, max compression
```

## Comparing `plover_spanish_mqd-2.1.6.tar` & `plover_spanish_mqd-2.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 08:06:16.915142 plover_spanish_mqd-2.1.6/
--rw-rw-rw-   0        0        0    35823 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/LICENSE
--rw-rw-rw-   0        0        0       41 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1870 2023-02-22 08:06:16.915142 plover_spanish_mqd-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-02-22 08:06:16.899519 plover_spanish_mqd-2.1.6/plover_spanish_mqd/
--rw-rw-rw-   0        0        0        0 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:06:16.915142 plover_spanish_mqd-2.1.6/plover_spanish_mqd/dictionaries/
--rw-rw-rw-   0        0        0    14475 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd/dictionaries/initial.json
--rw-rw-rw-   0        0        0      905 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd/dictionaries/punctuation.json
--rw-rw-rw-   0        0        0      397 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd/dictionaries/spanish_mqd.py
--rw-rw-rw-   0        0        0   107045 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd/dictionaries/user_es.json
--rw-rw-rw-   0        0        0    19962 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd/spanish_mqd_double.py
--rw-rw-rw-   0        0        0   425205 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd/spanish_mqd_single.py
--rw-rw-rw-   0        0        0     3402 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd/system.py
-drwxrwxrwx   0        0        0        0 2023-02-22 08:06:16.899519 plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/
--rw-rw-rw-   0        0        0     1870 2023-02-22 08:06:16.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-02-22 08:06:16.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 08:06:16.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-02-22 08:06:16.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      154 2023-02-22 08:06:16.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-22 08:06:16.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-22 08:06:16.000000 plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/zip-safe
--rw-rw-rw-   0        0        0     2131 2023-02-22 08:06:16.915142 plover_spanish_mqd-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0       69 2023-02-22 08:05:33.000000 plover_spanish_mqd-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:01:26.472511 plover_spanish_mqd-2.1.7/
+-rw-rw-rw-   0        0        0    35823 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0       41 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1870 2023-05-10 08:01:26.472511 plover_spanish_mqd-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 08:01:26.472511 plover_spanish_mqd-2.1.7/plover_spanish_mqd/
+-rw-rw-rw-   0        0        0        0 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:01:26.472511 plover_spanish_mqd-2.1.7/plover_spanish_mqd/dictionaries/
+-rw-rw-rw-   0        0        0    14444 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd/dictionaries/initial.json
+-rw-rw-rw-   0        0        0      905 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd/dictionaries/punctuation.json
+-rw-rw-rw-   0        0        0      397 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd/dictionaries/spanish_mqd.py
+-rw-rw-rw-   0        0        0   107045 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd/dictionaries/user_es.json
+-rw-rw-rw-   0        0        0    19962 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd/spanish_mqd_double.py
+-rw-rw-rw-   0        0        0   425354 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd/spanish_mqd_single.py
+-rw-rw-rw-   0        0        0     3402 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd/system.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:01:26.472511 plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/
+-rw-rw-rw-   0        0        0     1870 2023-05-10 08:01:25.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-05-10 08:01:26.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:01:25.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-10 08:01:25.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      154 2023-05-10 08:01:25.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-10 08:01:25.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 08:01:25.000000 plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     2131 2023-05-10 08:01:26.472511 plover_spanish_mqd-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       69 2023-05-10 08:00:53.000000 plover_spanish_mqd-2.1.7/setup.py
```

### Comparing `plover_spanish_mqd-2.1.6/LICENSE` & `plover_spanish_mqd-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plover_spanish_mqd-2.1.6/PKG-INFO` & `plover_spanish_mqd-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover_spanish_mqd
-Version: 2.1.6
+Version: 2.1.7
 Summary: Support for plover in Spanish (Melany system)
 Home-page: https://github.com/nvdaes/plover_spanish_mqd
 Author: Noelia Ruiz
 Author-email: nrm1977@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Source Code, https://github.com/nvdaes/plover_spanish_mqd
 Project-URL: Issue Tracker, https://github.com/nvdaes/plover_spanish_mqd/issues
```

### Comparing `plover_spanish_mqd-2.1.6/README.md` & `plover_spanish_mqd-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `plover_spanish_mqd-2.1.6/plover_spanish_mqd/dictionaries/initial.json` & `plover_spanish_mqd-2.1.7/plover_spanish_mqd/dictionaries/initial.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982300884955753%*

 * *Differences: {'delete': "['/Ie*']"}*

```diff
@@ -110,15 +110,14 @@
     "/Csia": "con esas",
     "/Cso": "con eso",
     "/Ctna": "adicional",
     "/Ctnia": "adicionales",
     "/Ctnie": "adicionalmente",
     "/EOt": "ultra{^}",
     "/Ere*": "Esquerra Republicana",
-    "/Ie*": "Izquierda-Ezkerra",
     "/Itnie": "idos",
     "/NEOro": "neuro{^}",
     "/NEOro*": "neur\u00f3{^}",
     "/NEe": "necesidades educativas especiales",
     "/NIco": "Instituto de Integraci\u00f3n a la Comunidad",
     "/NIco*": "INICO",
     "/NIsa": "ni siquiera",
```

### Comparing `plover_spanish_mqd-2.1.6/plover_spanish_mqd/dictionaries/punctuation.json` & `plover_spanish_mqd-2.1.7/plover_spanish_mqd/dictionaries/punctuation.json`

 * *Files identical despite different names*

### Comparing `plover_spanish_mqd-2.1.6/plover_spanish_mqd/dictionaries/user_es.json` & `plover_spanish_mqd-2.1.7/plover_spanish_mqd/dictionaries/user_es.json`

 * *Files identical despite different names*

### Comparing `plover_spanish_mqd-2.1.6/plover_spanish_mqd/spanish_mqd_double.py` & `plover_spanish_mqd-2.1.7/plover_spanish_mqd/spanish_mqd_double.py`

 * *Files identical despite different names*

### Comparing `plover_spanish_mqd-2.1.6/plover_spanish_mqd/spanish_mqd_single.py` & `plover_spanish_mqd-2.1.7/plover_spanish_mqd/spanish_mqd_single.py`

 * *Files 0% similar despite different names*

```diff
@@ -3281,18 +3281,21 @@
 	"PCNRcsnr": ("agilizar ", "agilizador"),
 	"PCNRcsnre": ("agilizadores ", "ágiles "),
 	"PCNRcsnreo": ("agilizador ", "ágil "),
 	"PCNRcsnrie": ("agilizarse ", "ágilmente "),
 	"PCNRcspie": ("regulaciones ", ""),
 	"PCNRcspr": ("", "glill"),
 	"PCNRcspreo": ("", "glillos "),
-	"PCNRcsr": ("regular ", "regulador"),
-	"PCNRcsr*": ("regulares ", ""),
+	"PCNRcsr": ("regular ", "regulares "),
+	"PCNRcsra": ("reguladora ", "regulatoria "),
 	"PCNRcsre": ("reguladores ", ""),
+	"PCNRcsreo": ("regulador ", "regulatorios "),
+	"PCNRcsria": ("reguladoras ", "regulatorias "),
 	"PCNRcsrie": ("regularse ", "regularmente "),
+	"PCNRcsro*": ("regulatorio ", ""),
 	"PCNRcstn": ("empequeñe", "empequeñezc"),
 	"PCNRcstn*": ("empequeñéz", ""),
 	"PCNRcstne": ("empequeñece ", ""),
 	"PCNRcstneo": ("empequeñeces ", ""),
 	"PCNRcstni*": ("empequeñecí ", ""),
 	"PCNRcstnie": ("empequeñecimiento ", ""),
 	"PCNRcstno*": ("empequeñeció ", ""),
```

### Comparing `plover_spanish_mqd-2.1.6/plover_spanish_mqd/system.py` & `plover_spanish_mqd-2.1.7/plover_spanish_mqd/system.py`

 * *Files identical despite different names*

### Comparing `plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/PKG-INFO` & `plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-spanish-mqd
-Version: 2.1.6
+Version: 2.1.7
 Summary: Support for plover in Spanish (Melany system)
 Home-page: https://github.com/nvdaes/plover_spanish_mqd
 Author: Noelia Ruiz
 Author-email: nrm1977@gmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Source Code, https://github.com/nvdaes/plover_spanish_mqd
 Project-URL: Issue Tracker, https://github.com/nvdaes/plover_spanish_mqd/issues
```

### Comparing `plover_spanish_mqd-2.1.6/plover_spanish_mqd.egg-info/SOURCES.txt` & `plover_spanish_mqd-2.1.7/plover_spanish_mqd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plover_spanish_mqd-2.1.6/setup.cfg` & `plover_spanish_mqd-2.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6c6f 7665 725f 7370 616e 6973   = plover_spanis
 00000020: 685f 6d71 640d 0a76 6572 7369 6f6e 203d  h_mqd..version =
-00000030: 2032 2e31 2e36 0d0a 6465 7363 7269 7074   2.1.6..descript
+00000030: 2032 2e31 2e37 0d0a 6465 7363 7269 7074   2.1.7..descript
 00000040: 696f 6e20 3d20 5375 7070 6f72 7420 666f  ion = Support fo
 00000050: 7220 706c 6f76 6572 2069 6e20 5370 616e  r plover in Span
 00000060: 6973 6820 284d 656c 616e 7920 7379 7374  ish (Melany syst
 00000070: 656d 290d 0a6c 6f6e 675f 6465 7363 7269  em)..long_descri
 00000080: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
 00000090: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
 000000a0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
```

