# Comparing `tmp/clabe-1.2.8.tar.gz` & `tmp/clabe-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clabe-1.2.8.tar", last modified: Tue Oct 25 16:38:47 2022, max compression
+gzip compressed data, was "clabe-1.2.9.tar", last modified: Wed May 10 19:52:06 2023, max compression
```

## Comparing `clabe-1.2.8.tar` & `clabe-1.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:38:47.218442 clabe-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-10-25 16:38:39.000000 clabe-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-10-25 16:38:47.218442 clabe-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-10-25 16:38:39.000000 clabe-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:38:47.218442 clabe-1.2.8/clabe/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-25 16:38:39.000000 clabe-1.2.8/clabe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3874 2022-10-25 16:38:39.000000 clabe-1.2.8/clabe/banks.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-10-25 16:38:39.000000 clabe-1.2.8/clabe/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 16:38:39.000000 clabe-1.2.8/clabe/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-10-25 16:38:39.000000 clabe-1.2.8/clabe/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-25 16:38:39.000000 clabe-1.2.8/clabe/validations.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-25 16:38:39.000000 clabe-1.2.8/clabe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:38:47.218442 clabe-1.2.8/clabe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-10-25 16:38:47.000000 clabe-1.2.8/clabe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-10-25 16:38:47.000000 clabe-1.2.8/clabe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 16:38:47.000000 clabe-1.2.8/clabe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-25 16:38:47.000000 clabe-1.2.8/clabe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-25 16:38:47.000000 clabe-1.2.8/clabe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-10-25 16:38:47.218442 clabe-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-10-25 16:38:39.000000 clabe-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:38:47.218442 clabe-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 16:38:39.000000 clabe-1.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-10-25 16:38:39.000000 clabe-1.2.8/tests/test_clabe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-10-25 16:38:39.000000 clabe-1.2.8/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:52:06.954410 clabe-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 19:51:55.000000 clabe-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-10 19:52:06.954410 clabe-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 19:51:55.000000 clabe-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:52:06.950410 clabe-1.2.9/clabe/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 19:51:55.000000 clabe-1.2.9/clabe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-10 19:51:55.000000 clabe-1.2.9/clabe/banks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 19:51:55.000000 clabe-1.2.9/clabe/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 19:51:55.000000 clabe-1.2.9/clabe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-10 19:51:55.000000 clabe-1.2.9/clabe/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-10 19:51:55.000000 clabe-1.2.9/clabe/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 19:51:55.000000 clabe-1.2.9/clabe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:52:06.950410 clabe-1.2.9/clabe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-10 19:52:06.000000 clabe-1.2.9/clabe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-10 19:52:06.000000 clabe-1.2.9/clabe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:52:06.000000 clabe-1.2.9/clabe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 19:52:06.000000 clabe-1.2.9/clabe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 19:52:06.000000 clabe-1.2.9/clabe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-10 19:52:06.954410 clabe-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-10 19:51:55.000000 clabe-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:52:06.954410 clabe-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 19:51:55.000000 clabe-1.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-10 19:51:55.000000 clabe-1.2.9/tests/test_clabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-10 19:51:55.000000 clabe-1.2.9/tests/test_types.py
```

### Comparing `clabe-1.2.8/LICENSE` & `clabe-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clabe-1.2.8/PKG-INFO` & `clabe-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clabe
-Version: 1.2.8
+Version: 1.2.9
 Summary: Validate and generate the control digit of a CLABE in Mexico
 Home-page: https://github.com/cuenca-mx/clabe
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clabe-1.2.8/README.md` & `clabe-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `clabe-1.2.8/clabe/banks.py` & `clabe-1.2.9/clabe/banks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 BANKS = {
     '138': '40138',
     '133': '40133',
     '062': '40062',
+    '661': '90661',
     '638': '90638',
     '706': '90706',
     '659': '90659',
     '128': '40128',
     '127': '40127',
     '166': '37166',
     '030': '40030',
@@ -34,14 +35,15 @@
     '143': '40143',
     '631': '90631',
     '901': '90901',
     '903': '90903',
     '130': '40130',
     '140': '40140',
     '652': '90652',
+    '688': '90688',
     '126': '40126',
     '680': '90680',
     '151': '40151',
     '616': '90616',
     '634': '90634',
     '689': '90689',
     '685': '90685',
@@ -87,15 +89,15 @@
 
 # Descargado de https://www.banxico.org.mx/cep-scl/listaInstituciones.do
 # 2022-10-18
 BANK_NAMES = {
     '40138': 'ABC Capital',
     '40133': 'Actinver',
     '40062': 'Afirme',
-    '90638': 'Akala',
+    '90661': 'ALTERNATIVOS',
     '90706': 'Arcus',
     '90659': 'Asp Integra Opc',
     '40128': 'Autofin',
     '40127': 'Azteca',
     '37166': 'Babien',
     '40030': 'Bajio',
     '40002': 'Banamex',
@@ -123,14 +125,15 @@
     '40143': 'CI Banco',
     '90631': 'CI Bolsa',
     '90901': 'Cls',
     '90903': 'CoDi Valida',
     '40130': 'Compartamos',
     '40140': 'Consubanco',
     '90652': 'Credicapital',
+    '90688': 'Crediclub',
     '40126': 'Credit Suisse',
     '90680': 'Cristobal Colon',
     '40151': 'Donde',
     '90616': 'Finamex',
     '90634': 'Fincomun',
     '90689': 'Fomped',
     '90685': 'Fondo (Fira)',
@@ -151,14 +154,15 @@
     '40042': 'Mifel',
     '40158': 'Mizuho Bank',
     '90600': 'Monexcb',
     '40108': 'Mufg',
     '40132': 'Multiva Banco',
     '90613': 'Multiva Cbolsa',
     '37135': 'Nafin',
+    '90638': 'NU MEXICO',
     '90710': 'NVIO',
     '90684': 'Opm',
     '40148': 'Pagatodo',
     '90620': 'Profuturo',
     '40156': 'Sabadell',
     '40014': 'Santander',
     '40044': 'Scotiabank',
```

### Comparing `clabe-1.2.8/clabe/types.py` & `clabe-1.2.9/clabe/types.py`

 * *Files identical despite different names*

### Comparing `clabe-1.2.8/clabe/validations.py` & `clabe-1.2.9/clabe/validations.py`

 * *Files identical despite different names*

### Comparing `clabe-1.2.8/clabe.egg-info/PKG-INFO` & `clabe-1.2.9/clabe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clabe
-Version: 1.2.8
+Version: 1.2.9
 Summary: Validate and generate the control digit of a CLABE in Mexico
 Home-page: https://github.com/cuenca-mx/clabe
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clabe-1.2.8/setup.py` & `clabe-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `clabe-1.2.8/tests/test_clabe.py` & `clabe-1.2.9/tests/test_clabe.py`

 * *Files identical despite different names*

### Comparing `clabe-1.2.8/tests/test_types.py` & `clabe-1.2.9/tests/test_types.py`

 * *Files identical despite different names*

