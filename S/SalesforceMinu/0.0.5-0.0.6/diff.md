# Comparing `tmp/SalesforceMinu-0.0.5.tar.gz` & `tmp/SalesforceMinu-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalesforceMinu-0.0.5.tar", last modified: Fri May  5 20:12:28 2023, max compression
+gzip compressed data, was "SalesforceMinu-0.0.6.tar", last modified: Wed May 10 18:50:57 2023, max compression
```

## Comparing `SalesforceMinu-0.0.5.tar` & `SalesforceMinu-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 20:12:28.135284 SalesforceMinu-0.0.5/
--rw-rw-rw-   0        0        0      610 2023-05-05 20:12:28.119663 SalesforceMinu-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-05 20:11:56.000000 SalesforceMinu-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 20:12:28.119663 SalesforceMinu-0.0.5/SalesforceMinu/
--rw-rw-rw-   0        0        0     4126 2023-05-05 20:11:37.000000 SalesforceMinu-0.0.5/SalesforceMinu/Funciones.py
--rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.5/SalesforceMinu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 20:12:28.119663 SalesforceMinu-0.0.5/SalesforceMinu.egg-info/
--rw-rw-rw-   0        0        0      610 2023-05-05 20:12:27.000000 SalesforceMinu-0.0.5/SalesforceMinu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-05 20:12:28.000000 SalesforceMinu-0.0.5/SalesforceMinu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 20:12:27.000000 SalesforceMinu-0.0.5/SalesforceMinu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-05 20:12:27.000000 SalesforceMinu-0.0.5/SalesforceMinu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-05 20:12:27.000000 SalesforceMinu-0.0.5/SalesforceMinu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 20:12:28.135284 SalesforceMinu-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-05-05 20:12:03.000000 SalesforceMinu-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:50:57.155804 SalesforceMinu-0.0.6/
+-rw-rw-rw-   0        0        0      610 2023-05-10 18:50:57.153809 SalesforceMinu-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-05 20:12:58.000000 SalesforceMinu-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 18:50:57.125107 SalesforceMinu-0.0.6/SalesforceMinu/
+-rw-rw-rw-   0        0        0     4357 2023-05-10 18:49:28.000000 SalesforceMinu-0.0.6/SalesforceMinu/Funciones.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.6/SalesforceMinu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:50:57.152812 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:50:57.155804 SalesforceMinu-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-05-10 18:49:41.000000 SalesforceMinu-0.0.6/setup.py
```

### Comparing `SalesforceMinu-0.0.5/PKG-INFO` & `SalesforceMinu-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SalesforceMinu
-Version: 0.0.5
+Version: 0.0.6
 Summary: Librería para extraer datos de minu en salesforce
 Home-page: https://github.com/BalamCor?tab=repositories
 Author: Corchado Ramos Itzae Balam
 Author-email: g7_corc18@ens.cnyn.unam.mx
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `SalesforceMinu-0.0.5/SalesforceMinu/Funciones.py` & `SalesforceMinu-0.0.6/SalesforceMinu/Funciones.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,21 +84,27 @@
     return products_ids
     
 
 # OBTENEMOS MODELO DE SUSCRIPCIÓN, EL CODIGO Y SU NOMBRE
 def get_model(products_ids,sf):
     
     dict_plan = {'005':'starter',
-             '009':'starter',
-             '011':'starter',
-             '013':'starter',
-             '006':'total',
-             '008':'total',
-             '010':'total',
-             '012':'total'}
+             	 '009':'starter',
+             	 '011':'starter',
+	         '013':'starter',
+             	 '006':'total',
+             	 '008':'total',
+             	 '010':'total',
+             	 '012':'total',
+             	 '004':'Addons',
+                 '007':'Modular',
+                 '001':'Pay On Demand',
+                 '002':'minunómina',
+                 '003':'Plug & Play',
+                 '002':'minu 2.0'}
     
     model = [ list(sf.query_all(f"""SELECT Name, ProductCode
                       FROM Product2
                       WHERE Id = '{row}'""")['records'][0].values()) for row in products_ids]
     # Puede haber más de una razón por empresa
     models = []
     plan = []
```

### Comparing `SalesforceMinu-0.0.5/SalesforceMinu.egg-info/PKG-INFO` & `SalesforceMinu-0.0.6/SalesforceMinu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SalesforceMinu
-Version: 0.0.5
+Version: 0.0.6
 Summary: Librería para extraer datos de minu en salesforce
 Home-page: https://github.com/BalamCor?tab=repositories
 Author: Corchado Ramos Itzae Balam
 Author-email: g7_corc18@ens.cnyn.unam.mx
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `SalesforceMinu-0.0.5/setup.py` & `SalesforceMinu-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 PACKAGE_NAME = 'SalesforceMinu' 
 AUTHOR = 'Corchado Ramos Itzae Balam' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'g7_corc18@ens.cnyn.unam.mx' 
 URL = 'https://github.com/BalamCor?tab=repositories' 
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para extraer datos de minu en salesforce'
```

