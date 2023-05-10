# Comparing `tmp/pixelmagic-1.0.0.tar.gz` & `tmp/pixelmagic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelmagic-1.0.0.tar", last modified: Wed May 10 04:25:38 2023, max compression
+gzip compressed data, was "pixelmagic-1.0.1.tar", last modified: Wed May 10 05:50:45 2023, max compression
```

## Comparing `pixelmagic-1.0.0.tar` & `pixelmagic-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 04:25:38.366291 pixelmagic-1.0.0/
--rw-r--r--   0 madhawaperera   (501) staff       (20)     1071 2023-05-10 02:46:37.000000 pixelmagic-1.0.0/LICENSE
--rw-r--r--   0 madhawaperera   (501) staff       (20)     3179 2023-05-10 04:25:38.365860 pixelmagic-1.0.0/PKG-INFO
--rw-r--r--   0 madhawaperera   (501) staff       (20)     2470 2023-05-10 04:14:59.000000 pixelmagic-1.0.0/README.md
-drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 04:25:38.365299 pixelmagic-1.0.0/pixelmagic.egg-info/
--rw-r--r--   0 madhawaperera   (501) staff       (20)     3179 2023-05-10 04:25:38.000000 pixelmagic-1.0.0/pixelmagic.egg-info/PKG-INFO
--rw-r--r--   0 madhawaperera   (501) staff       (20)      195 2023-05-10 04:25:38.000000 pixelmagic-1.0.0/pixelmagic.egg-info/SOURCES.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 04:25:38.000000 pixelmagic-1.0.0/pixelmagic.egg-info/dependency_links.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)       15 2023-05-10 04:25:38.000000 pixelmagic-1.0.0/pixelmagic.egg-info/requires.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 04:25:38.000000 pixelmagic-1.0.0/pixelmagic.egg-info/top_level.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)       38 2023-05-10 04:25:38.366456 pixelmagic-1.0.0/setup.cfg
--rw-r--r--   0 madhawaperera   (501) staff       (20)      930 2023-05-10 04:11:52.000000 pixelmagic-1.0.0/setup.py
+drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 05:50:45.201569 pixelmagic-1.0.1/
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     1071 2023-05-10 02:46:37.000000 pixelmagic-1.0.1/LICENSE
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     3230 2023-05-10 05:50:45.201266 pixelmagic-1.0.1/PKG-INFO
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     2470 2023-05-10 04:14:59.000000 pixelmagic-1.0.1/README.md
+drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 05:50:45.200849 pixelmagic-1.0.1/pixelmagic.egg-info/
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     3230 2023-05-10 05:50:45.000000 pixelmagic-1.0.1/pixelmagic.egg-info/PKG-INFO
+-rw-r--r--   0 madhawaperera   (501) staff       (20)      195 2023-05-10 05:50:45.000000 pixelmagic-1.0.1/pixelmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 05:50:45.000000 pixelmagic-1.0.1/pixelmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       15 2023-05-10 05:50:45.000000 pixelmagic-1.0.1/pixelmagic.egg-info/requires.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 05:50:45.000000 pixelmagic-1.0.1/pixelmagic.egg-info/top_level.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       38 2023-05-10 05:50:45.201676 pixelmagic-1.0.1/setup.cfg
+-rw-r--r--   0 madhawaperera   (501) staff       (20)      980 2023-05-10 05:47:23.000000 pixelmagic-1.0.1/setup.py
```

### Comparing `pixelmagic-1.0.0/LICENSE` & `pixelmagic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelmagic-1.0.0/PKG-INFO` & `pixelmagic-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pixelmagic
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for creating pixelated GIFs from images
 Home-page: https://github.com/madhawap/pixelmagic
 Author: madhawap
 Author-email: madhawa.perera@anu.edu.au
 Keywords: pixelated gif imageio pillow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pixelmagic
 
 `pixelmagic` is a Python package for creating pixelated GIFs from image files.
```

### Comparing `pixelmagic-1.0.0/README.md` & `pixelmagic-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pixelmagic-1.0.0/pixelmagic.egg-info/PKG-INFO` & `pixelmagic-1.0.1/pixelmagic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pixelmagic
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for creating pixelated GIFs from images
 Home-page: https://github.com/madhawap/pixelmagic
 Author: madhawap
 Author-email: madhawa.perera@anu.edu.au
 Keywords: pixelated gif imageio pillow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pixelmagic
 
 `pixelmagic` is a Python package for creating pixelated GIFs from image files.
```

### Comparing `pixelmagic-1.0.0/setup.py` & `pixelmagic-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pixelmagic',
-    version='1.0.0',
+    version='1.0.1',
     author='madhawap',
     author_email='madhawa.perera@anu.edu.au',
     description='A package for creating pixelated GIFs from images',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/madhawap/pixelmagic',
     packages=find_packages(),
@@ -15,14 +15,15 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     keywords='pixelated gif imageio pillow',
     install_requires=[
         'imageio',
         'Pillow',
     ],
 )
```

