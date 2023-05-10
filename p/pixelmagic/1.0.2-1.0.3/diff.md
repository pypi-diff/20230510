# Comparing `tmp/pixelmagic-1.0.2.tar.gz` & `tmp/pixelmagic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelmagic-1.0.2.tar", last modified: Wed May 10 06:15:25 2023, max compression
+gzip compressed data, was "pixelmagic-1.0.3.tar", last modified: Wed May 10 06:44:42 2023, max compression
```

## Comparing `pixelmagic-1.0.2.tar` & `pixelmagic-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:15:25.706016 pixelmagic-1.0.2/
--rw-r--r--   0 madhawaperera   (501) staff       (20)     1071 2023-05-10 06:09:39.000000 pixelmagic-1.0.2/LICENSE
--rw-r--r--   0 madhawaperera   (501) staff       (20)     3230 2023-05-10 06:15:25.705769 pixelmagic-1.0.2/PKG-INFO
--rw-r--r--   0 madhawaperera   (501) staff       (20)     2470 2023-05-10 06:09:39.000000 pixelmagic-1.0.2/README.md
-drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:15:25.705407 pixelmagic-1.0.2/pixelmagic.egg-info/
--rw-r--r--   0 madhawaperera   (501) staff       (20)     3230 2023-05-10 06:15:25.000000 pixelmagic-1.0.2/pixelmagic.egg-info/PKG-INFO
--rw-r--r--   0 madhawaperera   (501) staff       (20)      195 2023-05-10 06:15:25.000000 pixelmagic-1.0.2/pixelmagic.egg-info/SOURCES.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 06:15:25.000000 pixelmagic-1.0.2/pixelmagic.egg-info/dependency_links.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)       15 2023-05-10 06:15:25.000000 pixelmagic-1.0.2/pixelmagic.egg-info/requires.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 06:15:25.000000 pixelmagic-1.0.2/pixelmagic.egg-info/top_level.txt
--rw-r--r--   0 madhawaperera   (501) staff       (20)       38 2023-05-10 06:15:25.706101 pixelmagic-1.0.2/setup.cfg
--rw-r--r--   0 madhawaperera   (501) staff       (20)      980 2023-05-10 06:14:40.000000 pixelmagic-1.0.2/setup.py
+drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:44:42.432677 pixelmagic-1.0.3/
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     1071 2023-05-10 06:09:39.000000 pixelmagic-1.0.3/LICENSE
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     3242 2023-05-10 06:44:42.432429 pixelmagic-1.0.3/PKG-INFO
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     2482 2023-05-10 06:42:58.000000 pixelmagic-1.0.3/README.md
+drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:44:42.430804 pixelmagic-1.0.3/pixelmagic/
+-rw-r--r--   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:09:39.000000 pixelmagic-1.0.3/pixelmagic/__init__.py
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     3631 2023-05-10 06:09:39.000000 pixelmagic-1.0.3/pixelmagic/pixelmagic.py
+drwxr-xr-x   0 madhawaperera   (501) staff       (20)        0 2023-05-10 06:44:42.432071 pixelmagic-1.0.3/pixelmagic.egg-info/
+-rw-r--r--   0 madhawaperera   (501) staff       (20)     3242 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/PKG-INFO
+-rw-r--r--   0 madhawaperera   (501) staff       (20)      243 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/SOURCES.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)        1 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/dependency_links.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       15 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/requires.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       11 2023-05-10 06:44:42.000000 pixelmagic-1.0.3/pixelmagic.egg-info/top_level.txt
+-rw-r--r--   0 madhawaperera   (501) staff       (20)       38 2023-05-10 06:44:42.432766 pixelmagic-1.0.3/setup.cfg
+-rw-r--r--   0 madhawaperera   (501) staff       (20)      979 2023-05-10 06:44:12.000000 pixelmagic-1.0.3/setup.py
```

### Comparing `pixelmagic-1.0.2/LICENSE` & `pixelmagic-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelmagic-1.0.2/PKG-INFO` & `pixelmagic-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelmagic
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for creating pixelated GIFs from images
 Home-page: https://github.com/madhawap/pixelmagic
 Author: madhawap
 Author-email: madhawa.perera@anu.edu.au
 Keywords: pixelated gif imageio pillow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -54,22 +54,22 @@
     from PIL import Image
 ```
 
 ## Usage
 Here's an example of how to create a pixelated GIF using `pixelmagic`:
 
 ```python
-from pixelmagic import create_pixelated_gif
+from pixelmagic.pixelmagic import create_pixelated_gif
 
 image_path = 'path/to/image.jpg'
 duration = 0.1
 loops = 0
 start_pixel_size = 20
 output_path = 'path/to/output.gif'
-reverse = False # Optional
+reverse = False  # Optional
 
 create_pixelated_gif(image_path, duration, loops, start_pixel_size, output_path, reverse)
 ```
 
 ## Function Reference
 ```python
 def create_pixelated_gif(image_path: str, duration: float, loops: int, start_pixel_size: int = 20,
```

### Comparing `pixelmagic-1.0.2/README.md` & `pixelmagic-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,22 @@
     from PIL import Image
 ```
 
 ## Usage
 Here's an example of how to create a pixelated GIF using `pixelmagic`:
 
 ```python
-from pixelmagic import create_pixelated_gif
+from pixelmagic.pixelmagic import create_pixelated_gif
 
 image_path = 'path/to/image.jpg'
 duration = 0.1
 loops = 0
 start_pixel_size = 20
 output_path = 'path/to/output.gif'
-reverse = False # Optional
+reverse = False  # Optional
 
 create_pixelated_gif(image_path, duration, loops, start_pixel_size, output_path, reverse)
 ```
 
 ## Function Reference
 ```python
 def create_pixelated_gif(image_path: str, duration: float, loops: int, start_pixel_size: int = 20,
```

### Comparing `pixelmagic-1.0.2/pixelmagic.egg-info/PKG-INFO` & `pixelmagic-1.0.3/pixelmagic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelmagic
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for creating pixelated GIFs from images
 Home-page: https://github.com/madhawap/pixelmagic
 Author: madhawap
 Author-email: madhawa.perera@anu.edu.au
 Keywords: pixelated gif imageio pillow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -54,22 +54,22 @@
     from PIL import Image
 ```
 
 ## Usage
 Here's an example of how to create a pixelated GIF using `pixelmagic`:
 
 ```python
-from pixelmagic import create_pixelated_gif
+from pixelmagic.pixelmagic import create_pixelated_gif
 
 image_path = 'path/to/image.jpg'
 duration = 0.1
 loops = 0
 start_pixel_size = 20
 output_path = 'path/to/output.gif'
-reverse = False # Optional
+reverse = False  # Optional
 
 create_pixelated_gif(image_path, duration, loops, start_pixel_size, output_path, reverse)
 ```
 
 ## Function Reference
 ```python
 def create_pixelated_gif(image_path: str, duration: float, loops: int, start_pixel_size: int = 20,
```

### Comparing `pixelmagic-1.0.2/setup.py` & `pixelmagic-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pixelmagic',
-    version='1.0.2',
+    version='1.0.3',
     author='madhawap',
     author_email='madhawa.perera@anu.edu.au',
     description='A package for creating pixelated GIFs from images',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/madhawap/pixelmagic',
-    packages=find_packages(),
+    packages=['pixelmagic'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

