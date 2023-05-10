# Comparing `tmp/animegifs-0.4.0.tar.gz` & `tmp/animegifs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.4.0.tar", last modified: Fri Apr 28 21:03:48 2023, max compression
+gzip compressed data, was "animegifs-0.5.0.tar", last modified: Wed May 10 01:22:41 2023, max compression
```

## Comparing `animegifs-0.4.0.tar` & `animegifs-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 21:03:48.135555 animegifs-0.4.0/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1156 2023-04-28 21:03:48.134547 animegifs-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-04-28 20:51:38.000000 animegifs-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 21:03:48.122549 animegifs-0.4.0/animegifs/
--rw-rw-rw-   0        0        0        0 2023-04-28 19:02:26.000000 animegifs-0.4.0/animegifs/__init__.py
--rw-rw-rw-   0        0        0     2774 2023-04-28 20:51:38.000000 animegifs-0.4.0/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-04-28 21:03:48.132547 animegifs-0.4.0/animegifs/dis_utils/
--rw-rw-rw-   0        0        0        2 2023-04-28 19:01:35.000000 animegifs-0.4.0/animegifs/dis_utils/__init__.py
--rw-rw-rw-   0        0        0     1313 2023-04-28 20:51:38.000000 animegifs-0.4.0/animegifs/dis_utils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-04-28 21:03:48.129548 animegifs-0.4.0/animegifs.egg-info/
--rw-rw-rw-   0        0        0     1156 2023-04-28 21:03:48.000000 animegifs-0.4.0/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-28 21:03:48.000000 animegifs-0.4.0/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 21:03:48.000000 animegifs-0.4.0/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 21:03:48.000000 animegifs-0.4.0/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 21:03:48.135555 animegifs-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      939 2023-04-28 20:49:04.000000 animegifs-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:22:41.278420 animegifs-0.5.0/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1184 2023-05-10 01:22:41.277414 animegifs-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-05-10 01:21:45.000000 animegifs-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 01:22:41.258413 animegifs-0.5.0/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.0/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     2333 2023-05-10 01:17:27.000000 animegifs-0.5.0/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:22:41.275414 animegifs-0.5.0/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.0/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0      356 2023-05-10 00:52:28.000000 animegifs-0.5.0/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     1313 2023-04-28 20:51:38.000000 animegifs-0.5.0/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:22:41.269414 animegifs-0.5.0/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     1184 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 01:22:41.278420 animegifs-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2023-05-10 01:21:45.000000 animegifs-0.5.0/setup.py
```

### Comparing `animegifs-0.4.0/LICENSE` & `animegifs-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.4.0/PKG-INFO` & `animegifs-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.4.0
+Version: 0.5.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif
 Platform: UNKNOWN
@@ -13,27 +13,29 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # anime-gifs.py
-Get random anime gifs by category. Use Python (intended initially for Discord).
+Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. v0.4.0 is the only working release.
+WIP - updated in time to time. Versions below v0.4.0 aren't expected to work.
 
 `pip install animegifs`
 
 # HOW TO USE
 
 ```py
 
-from animegifs.animegifs import Animegifs
+from animegifs import animegifs
 
-gif = Animegifs().get_gif(category)
+gifs = animegifs.Animegifs()
+
+gif = gifs.get_gif(category)
 ```
 
 **Category list:** 
 
 * Attack
 * Bite
 * Bloodsuck
```

### Comparing `animegifs-0.4.0/animegifs/dis_utils/gifs.py` & `animegifs-0.5.0/animegifs/distutils/gifs.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.4.0/animegifs.egg-info/PKG-INFO` & `animegifs-0.5.0/animegifs.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.4.0
+Version: 0.5.0
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif
 Platform: UNKNOWN
@@ -13,27 +13,29 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # anime-gifs.py
-Get random anime gifs by category. Use Python (intended initially for Discord).
+Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
-WIP - updated in time to time. v0.4.0 is the only working release.
+WIP - updated in time to time. Versions below v0.4.0 aren't expected to work.
 
 `pip install animegifs`
 
 # HOW TO USE
 
 ```py
 
-from animegifs.animegifs import Animegifs
+from animegifs import animegifs
 
-gif = Animegifs().get_gif(category)
+gifs = animegifs.Animegifs()
+
+gif = gifs.get_gif(category)
 ```
 
 **Category list:** 
 
 * Attack
 * Bite
 * Bloodsuck
```

### Comparing `animegifs-0.4.0/setup.py` & `animegifs-0.5.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from setuptools import find_packages, setup
+from setuptools import setup
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.4.0'
+VERSION = '0.5.0'
 
 setup(
     name='animegifs',
-    packages=find_packages(),
+    package_dir={"anime_gifs": "animegifs"},
+    packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Marco-Sa2000',
     author_email='grest0grest@gmail.com',
     license='MIT',
     url="https://github.com/MarcoSa-2000/animegifs",
+    install_requires=[
+       'requests==2.28.2,<=2.29.0'
+    ],
     python_requires='>=3.8',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows"],
     keywords=['anime', 'gif', 'python', 'anime-gif'],
 )
```

