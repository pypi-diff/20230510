# Comparing `tmp/Mensajes-Nikk-6.0.tar.gz` & `tmp/Mensajes-Nikk-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-Nikk-6.0.tar", last modified: Wed May 10 13:31:51 2023, max compression
+gzip compressed data, was "Mensajes-Nikk-7.0.tar", last modified: Wed May 10 13:39:00 2023, max compression
```

## Comparing `Mensajes-Nikk-6.0.tar` & `Mensajes-Nikk-7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:31:51.583375 Mensajes-Nikk-6.0/
--rw-rw-rw-   0        0        0     1096 2023-05-10 13:09:44.000000 Mensajes-Nikk-6.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-05-10 13:09:55.000000 Mensajes-Nikk-6.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-10 13:31:51.570364 Mensajes-Nikk-6.0/Mensajes_Nikk.egg-info/
--rw-rw-rw-   0        0        0      616 2023-05-10 13:31:51.000000 Mensajes-Nikk-6.0/Mensajes_Nikk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-05-10 13:31:51.000000 Mensajes-Nikk-6.0/Mensajes_Nikk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:31:51.000000 Mensajes-Nikk-6.0/Mensajes_Nikk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-10 13:31:51.000000 Mensajes-Nikk-6.0/Mensajes_Nikk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 13:31:51.000000 Mensajes-Nikk-6.0/Mensajes_Nikk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      616 2023-05-10 13:31:51.583375 Mensajes-Nikk-6.0/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-05-10 13:05:54.000000 Mensajes-Nikk-6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 13:31:51.571364 Mensajes-Nikk-6.0/mensajes/
--rw-rw-rw-   0        0        0       38 2022-07-07 17:39:14.000000 Mensajes-Nikk-6.0/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:31:51.575367 Mensajes-Nikk-6.0/mensajes/adios/
--rw-rw-rw-   0        0        0       47 2022-07-07 17:43:51.000000 Mensajes-Nikk-6.0/mensajes/adios/__init__.py
--rw-rw-rw-   0        0        0      182 2022-07-07 17:45:52.000000 Mensajes-Nikk-6.0/mensajes/adios/despedidas.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:31:51.578370 Mensajes-Nikk-6.0/mensajes/hola/
--rw-rw-rw-   0        0        0       46 2022-07-07 17:41:56.000000 Mensajes-Nikk-6.0/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      453 2023-05-09 11:33:31.000000 Mensajes-Nikk-6.0/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       13 2022-07-08 17:50:40.000000 Mensajes-Nikk-6.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 13:31:51.584376 Mensajes-Nikk-6.0/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-10 13:31:33.000000 Mensajes-Nikk-6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:31:51.581373 Mensajes-Nikk-6.0/tests/
--rw-rw-rw-   0        0        0        0 2022-07-08 18:23:47.000000 Mensajes-Nikk-6.0/tests/__init__.py
--rw-rw-rw-   0        0        0      268 2022-07-08 18:20:55.000000 Mensajes-Nikk-6.0/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:39:00.212260 Mensajes-Nikk-7.0/
+-rw-rw-rw-   0        0        0     1096 2023-05-10 13:09:44.000000 Mensajes-Nikk-7.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-05-10 13:09:55.000000 Mensajes-Nikk-7.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-10 13:39:00.190528 Mensajes-Nikk-7.0/Mensajes_Nikk.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-05-10 13:39:00.000000 Mensajes-Nikk-7.0/Mensajes_Nikk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-05-10 13:39:00.000000 Mensajes-Nikk-7.0/Mensajes_Nikk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:39:00.000000 Mensajes-Nikk-7.0/Mensajes_Nikk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 13:39:00.000000 Mensajes-Nikk-7.0/Mensajes_Nikk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 13:39:00.000000 Mensajes-Nikk-7.0/Mensajes_Nikk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      616 2023-05-10 13:39:00.211259 Mensajes-Nikk-7.0/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2023-05-10 13:05:54.000000 Mensajes-Nikk-7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 13:39:00.193037 Mensajes-Nikk-7.0/mensajes/
+-rw-rw-rw-   0        0        0       38 2022-07-07 17:39:14.000000 Mensajes-Nikk-7.0/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:39:00.196179 Mensajes-Nikk-7.0/mensajes/adios/
+-rw-rw-rw-   0        0        0       47 2022-07-07 17:43:51.000000 Mensajes-Nikk-7.0/mensajes/adios/__init__.py
+-rw-rw-rw-   0        0        0      182 2022-07-07 17:45:52.000000 Mensajes-Nikk-7.0/mensajes/adios/despedidas.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:39:00.205391 Mensajes-Nikk-7.0/mensajes/hola/
+-rw-rw-rw-   0        0        0       46 2022-07-07 17:41:56.000000 Mensajes-Nikk-7.0/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-05-10 13:38:02.000000 Mensajes-Nikk-7.0/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       13 2022-07-08 17:50:40.000000 Mensajes-Nikk-7.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:39:00.212260 Mensajes-Nikk-7.0/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-10 13:37:03.000000 Mensajes-Nikk-7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:39:00.209314 Mensajes-Nikk-7.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-08 18:23:47.000000 Mensajes-Nikk-7.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      268 2022-07-08 18:20:55.000000 Mensajes-Nikk-7.0/tests/test_hola.py
```

### Comparing `Mensajes-Nikk-6.0/LICENSE` & `Mensajes-Nikk-7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-Nikk-6.0/Mensajes_Nikk.egg-info/PKG-INFO` & `Mensajes-Nikk-7.0/Mensajes_Nikk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-Nikk
-Version: 6.0
+Version: 7.0
 Summary: Un paquete para saludar y despedir
 Author: Nicolas Roman Blanco
 Author-email: nicolasromanblanco@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Mensajes-Nikk-6.0/PKG-INFO` & `Mensajes-Nikk-7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-Nikk
-Version: 6.0
+Version: 7.0
 Summary: Un paquete para saludar y despedir
 Author: Nicolas Roman Blanco
 Author-email: nicolasromanblanco@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Mensajes-Nikk-6.0/setup.py` & `Mensajes-Nikk-7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Mensajes-Nikk',
-    version='6.0',
+    version='7.0',
     description='Un paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Nicolas Roman Blanco',
     author_email='nicolasromanblanco@gmail.com',
     license_files=['LICENSE'],
     # busca automaticamente  los paquetes
```

