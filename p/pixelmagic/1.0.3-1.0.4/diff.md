# Comparing `tmp/pixelmagic-1.0.3.tar.gz` & `tmp/pixelmagic-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelmagic-1.0.3.tar", last modified: Wed May 10 06:44:42 2023, max compression
+gzip compressed data, was "pixelmagic-1.0.4.tar", last modified: Wed May 10 06:50:45 2023, max compression
```

## Comparing `pixelmagic-1.0.3.tar` & `pixelmagic-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:44:42.432677 pixelmagic-1.0.3/
--rw-r--r--   0 madhawaperera   (501) staff       (20)     1071 2023-05-10 06:09:39.000000 pixelmagic-1.0.3/LICENSE
--rw-r--r--   0 madhawaperera   (501) staff       (20)     3242 2023-05-10 06:44:42.432429 pixelmagic-1.0.3/PKG-INFO
--rw-r--r--   0 madhawaperera   (501) staff       (20)     2482 2023-05-10 06:42:58.000000 pixelmagic-1.0.3/README.md
-drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:44:42.430804 pixelmagic-1.0.3/pixelmagic/
--rw-r--r--   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:09:39.000000 pixelmagic-1.0.3/pixelmagic/__init__.py
--rw-r--r--   0 madhawaperera   (501) staff       (20)     3631 2023-05-10 06:09:39.000000 pixelmagic-1.0.3/pixelmagic/pixelmagic.py
-drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:44:42.432071 pixelmagic-1.0.3/pixelmagic.egg-info/
--rw-r--r--   0 madhawaperera   (501) staff       (20)     3242 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/PKG-INFO
--rw-r--r--   0 madhawaperera   (501) staff       (20)      243 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/SOURCES.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/dependency_links.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)       15 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/requires.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)       11 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/top_level.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)       38 2023-05-10 06:44:42.432766 pixelmagic-1.0.3/setup.cfg
--rw-r--r--   0 madhawaperera   (501) staff       (20)      979 2023-05-10 06:44:12.000000 pixelmagic-1.0.3/setup.py
+drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:50:45.253197 pixelmagic-1.0.4/
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     1071 2023-05-10 06:09:39.000000 pixelmagic-1.0.4/LICENSE
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     3242 2023-05-10 06:50:45.252862 pixelmagic-1.0.4/PKG-INFO
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     2482 2023-05-10 06:42:58.000000 pixelmagic-1.0.4/README.md
+drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:50:45.249922 pixelmagic-1.0.4/pixelmagic/
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       45 2023-05-10 06:49:50.000000 pixelmagic-1.0.4/pixelmagic/__init__.py
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     3631 2023-05-10 06:09:39.000000 pixelmagic-1.0.4/pixelmagic/pixelmagic.py
+drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:50:45.252386 pixelmagic-1.0.4/pixelmagic.egg-info/
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     3242 2023-05-10 06:50:45.000000 pixelmagic-1.0.4/pixelmagic.egg-info/PKG-INFO
+-rw-r--r--   0 madhawaperera   (501) staff       (20)      243 2023-05-10 06:50:45.000000 pixelmagic-1.0.4/pixelmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 06:50:45.000000 pixelmagic-1.0.4/pixelmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       15 2023-05-10 06:50:45.000000 pixelmagic-1.0.4/pixelmagic.egg-info/requires.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       11 2023-05-10 06:50:45.000000 pixelmagic-1.0.4/pixelmagic.egg-info/top_level.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       38 2023-05-10 06:50:45.253317 pixelmagic-1.0.4/setup.cfg
+-rw-r--r--   0 madhawaperera   (501) staff       (20)      979 2023-05-10 06:50:17.000000 pixelmagic-1.0.4/setup.py
```

### Comparing `pixelmagic-1.0.3/LICENSE` & `pixelmagic-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelmagic-1.0.3/PKG-INFO` & `pixelmagic-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelmagic
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for creating pixelated GIFs from images
 Home-page: https://github.com/madhawap/pixelmagic
 Author: madhawap
 Author-email: madhawa.perera@anu.edu.au
 Keywords: pixelated gif imageio pillow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pixelmagic-1.0.3/README.md` & `pixelmagic-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pixelmagic-1.0.3/pixelmagic/pixelmagic.py` & `pixelmagic-1.0.4/pixelmagic/pixelmagic.py`

 * *Files identical despite different names*

### Comparing `pixelmagic-1.0.3/pixelmagic.egg-info/PKG-INFO` & `pixelmagic-1.0.4/pixelmagic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelmagic
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for creating pixelated GIFs from images
 Home-page: https://github.com/madhawap/pixelmagic
 Author: madhawap
 Author-email: madhawa.perera@anu.edu.au
 Keywords: pixelated gif imageio pillow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pixelmagic-1.0.3/setup.py` & `pixelmagic-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pixelmagic',
-    version='1.0.3',
+    version='1.0.4',
     author='madhawap',
     author_email='madhawa.perera@anu.edu.au',
     description='A package for creating pixelated GIFs from images',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/madhawap/pixelmagic',
     packages=['pixelmagic'],
```

