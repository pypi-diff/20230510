# Comparing `tmp/roboart-0.0.1.tar.gz` & `tmp/RoboArt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboart-0.0.1.tar", last modified: Wed May 10 10:02:55 2023, max compression
+gzip compressed data, was "RoboArt-0.0.2.tar", last modified: Wed May 10 10:39:50 2023, max compression
```

## Comparing `roboart-0.0.1.tar` & `RoboArt-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:02:55.246408 roboart-0.0.1/
--rw-r--r--   0 puang59    (501) staff       (20)     1064 2023-05-10 08:26:19.000000 roboart-0.0.1/LICENSE.txt
--rw-r--r--   0 puang59    (501) staff       (20)      685 2023-05-10 10:02:55.246280 roboart-0.0.1/PKG-INFO
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:02:55.245381 roboart-0.0.1/roboart/
--rw-r--r--   0 puang59    (501) staff       (20)      613 2023-05-10 08:23:59.000000 roboart-0.0.1/roboart/HashFaces.py
--rw-r--r--   0 puang59    (501) staff       (20)      308 2023-05-10 08:30:21.000000 roboart-0.0.1/roboart/__init__.py
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:02:55.246072 roboart-0.0.1/roboart.egg-info/
--rw-r--r--   0 puang59    (501) staff       (20)      685 2023-05-10 10:02:55.000000 roboart-0.0.1/roboart.egg-info/PKG-INFO
--rw-r--r--   0 puang59    (501) staff       (20)      185 2023-05-10 10:02:55.000000 roboart-0.0.1/roboart.egg-info/SOURCES.txt
--rw-r--r--   0 puang59    (501) staff       (20)        1 2023-05-10 10:02:55.000000 roboart-0.0.1/roboart.egg-info/dependency_links.txt
--rw-r--r--   0 puang59    (501) staff       (20)        8 2023-05-10 10:02:55.000000 roboart-0.0.1/roboart.egg-info/top_level.txt
--rw-r--r--   0 puang59    (501) staff       (20)       38 2023-05-10 10:02:55.246466 roboart-0.0.1/setup.cfg
--rw-r--r--   0 puang59    (501) staff       (20)      918 2023-05-10 10:01:28.000000 roboart-0.0.1/setup.py
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:39:50.162409 RoboArt-0.0.2/
+-rw-r--r--   0 puang59    (501) staff       (20)     1064 2023-05-10 08:26:19.000000 RoboArt-0.0.2/LICENSE.txt
+-rw-r--r--   0 puang59    (501) staff       (20)     1266 2023-05-10 10:39:50.162285 RoboArt-0.0.2/PKG-INFO
+-rw-r--r--   0 puang59    (501) staff       (20)      659 2023-05-10 10:38:49.000000 RoboArt-0.0.2/README.md
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:39:50.161518 RoboArt-0.0.2/RoboArt.egg-info/
+-rw-r--r--   0 puang59    (501) staff       (20)     1266 2023-05-10 10:39:50.000000 RoboArt-0.0.2/RoboArt.egg-info/PKG-INFO
+-rw-r--r--   0 puang59    (501) staff       (20)      317 2023-05-10 10:39:50.000000 RoboArt-0.0.2/RoboArt.egg-info/SOURCES.txt
+-rw-r--r--   0 puang59    (501) staff       (20)        1 2023-05-10 10:39:50.000000 RoboArt-0.0.2/RoboArt.egg-info/dependency_links.txt
+-rw-r--r--   0 puang59    (501) staff       (20)        8 2023-05-10 10:39:50.000000 RoboArt-0.0.2/RoboArt.egg-info/top_level.txt
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:39:50.161850 RoboArt-0.0.2/roboart/
+-rw-r--r--   0 puang59    (501) staff       (20)      613 2023-05-10 10:24:35.000000 RoboArt-0.0.2/roboart/RoboArt.py
+-rw-r--r--   0 puang59    (501) staff       (20)      308 2023-05-10 08:30:21.000000 RoboArt-0.0.2/roboart/__init__.py
+-rw-r--r--   0 puang59    (501) staff       (20)       38 2023-05-10 10:39:50.162458 RoboArt-0.0.2/setup.cfg
+-rw-r--r--   0 puang59    (501) staff       (20)      945 2023-05-10 10:29:14.000000 RoboArt-0.0.2/setup.py
```

### Comparing `roboart-0.0.1/LICENSE.txt` & `RoboArt-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roboart-0.0.1/roboart/HashFaces.py` & `RoboArt-0.0.2/roboart/RoboArt.py`

 * *Files identical despite different names*

### Comparing `roboart-0.0.1/setup.py` & `RoboArt-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+VERSION = '0.0.2'
 DESCRIPTION = 'A basic random avatar generator'
-LONG_DESCRIPTION = 'A package which generates a random avatar in 4 different sets on specific hash'
 
 # Setting up
 setup(
-    name="roboart",
+    name="RoboArt",
     version=VERSION,
     author="puang59",
     author_email="puang59@proton.me",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
+    long_description=long_description,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'avatar', 'roboart', 'random avatar', 'robohash', 'robots art'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

