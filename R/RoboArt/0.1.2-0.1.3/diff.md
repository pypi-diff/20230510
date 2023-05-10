# Comparing `tmp/RoboArt-0.1.2.tar.gz` & `tmp/RoboArt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoboArt-0.1.2.tar", last modified: Wed May 10 11:53:34 2023, max compression
+gzip compressed data, was "RoboArt-0.1.3.tar", last modified: Wed May 10 11:59:46 2023, max compression
```

## Comparing `RoboArt-0.1.2.tar` & `RoboArt-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:53:34.399949 RoboArt-0.1.2/
--rw-r--r--   0 puang59    (501) staff       (20)     1064 2023-05-10 08:26:19.000000 RoboArt-0.1.2/LICENSE.txt
--rw-r--r--   0 puang59    (501) staff       (20)     1538 2023-05-10 11:53:34.399825 RoboArt-0.1.2/PKG-INFO
--rw-r--r--   0 puang59    (501) staff       (20)      987 2023-05-10 11:30:24.000000 RoboArt-0.1.2/README.md
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:53:34.399096 RoboArt-0.1.2/RoboArt/
--rw-r--r--   0 puang59    (501) staff       (20)      612 2023-05-10 11:33:04.000000 RoboArt-0.1.2/RoboArt/RoboArt.py
--rw-r--r--   0 puang59    (501) staff       (20)      306 2023-05-10 11:53:18.000000 RoboArt-0.1.2/RoboArt/__init__.py
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:53:34.399641 RoboArt-0.1.2/RoboArt.egg-info/
--rw-r--r--   0 puang59    (501) staff       (20)     1538 2023-05-10 11:53:34.000000 RoboArt-0.1.2/RoboArt.egg-info/PKG-INFO
--rw-r--r--   0 puang59    (501) staff       (20)      193 2023-05-10 11:53:34.000000 RoboArt-0.1.2/RoboArt.egg-info/SOURCES.txt
--rw-r--r--   0 puang59    (501) staff       (20)        1 2023-05-10 11:53:34.000000 RoboArt-0.1.2/RoboArt.egg-info/dependency_links.txt
--rw-r--r--   0 puang59    (501) staff       (20)        8 2023-05-10 11:53:34.000000 RoboArt-0.1.2/RoboArt.egg-info/top_level.txt
--rw-r--r--   0 puang59    (501) staff       (20)       38 2023-05-10 11:53:34.399996 RoboArt-0.1.2/setup.cfg
--rw-r--r--   0 puang59    (501) staff       (20)      921 2023-05-10 11:53:26.000000 RoboArt-0.1.2/setup.py
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:59:46.228991 RoboArt-0.1.3/
+-rw-r--r--   0 puang59    (501) staff       (20)     1064 2023-05-10 08:26:19.000000 RoboArt-0.1.3/LICENSE.txt
+-rw-r--r--   0 puang59    (501) staff       (20)     1713 2023-05-10 11:59:46.228861 RoboArt-0.1.3/PKG-INFO
+-rw-r--r--   0 puang59    (501) staff       (20)     1162 2023-05-10 11:59:21.000000 RoboArt-0.1.3/README.md
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:59:46.228134 RoboArt-0.1.3/RoboArt/
+-rw-r--r--   0 puang59    (501) staff       (20)      612 2023-05-10 11:33:04.000000 RoboArt-0.1.3/RoboArt/RoboArt.py
+-rw-r--r--   0 puang59    (501) staff       (20)      306 2023-05-10 11:53:18.000000 RoboArt-0.1.3/RoboArt/__init__.py
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:59:46.228670 RoboArt-0.1.3/RoboArt.egg-info/
+-rw-r--r--   0 puang59    (501) staff       (20)     1713 2023-05-10 11:59:46.000000 RoboArt-0.1.3/RoboArt.egg-info/PKG-INFO
+-rw-r--r--   0 puang59    (501) staff       (20)      193 2023-05-10 11:59:46.000000 RoboArt-0.1.3/RoboArt.egg-info/SOURCES.txt
+-rw-r--r--   0 puang59    (501) staff       (20)        1 2023-05-10 11:59:46.000000 RoboArt-0.1.3/RoboArt.egg-info/dependency_links.txt
+-rw-r--r--   0 puang59    (501) staff       (20)        8 2023-05-10 11:59:46.000000 RoboArt-0.1.3/RoboArt.egg-info/top_level.txt
+-rw-r--r--   0 puang59    (501) staff       (20)       38 2023-05-10 11:59:46.229034 RoboArt-0.1.3/setup.cfg
+-rw-r--r--   0 puang59    (501) staff       (20)      921 2023-05-10 11:59:38.000000 RoboArt-0.1.3/setup.py
```

### Comparing `RoboArt-0.1.2/LICENSE.txt` & `RoboArt-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RoboArt-0.1.2/PKG-INFO` & `RoboArt-0.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,52 @@
-Metadata-Version: 2.1
-Name: RoboArt
-Version: 0.1.2
-Summary: A basic random avatar generator
-Author: puang59
-Author-email: puang59@proton.me
-Keywords: python,avatar,roboart,random avatar,robohash,robots art
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # RoboArt
 
 ### Avatars lovingly delivered by Robohash.org
 
 RoboArt is a basic random avatar generator which generates avatar in 4 different sets when hash is provided.
 
 ## Installation
 
 You can install RoboArt via pip:
 
 ```bash
-pip install roboart
+pip3 install -U RoboArt
 ```
 
+This will install the latest version of RoboArt
+
 ## Usage
 
 Import RoboArt in your Python script and create an instance of the roboart class:
 
 ```python
-from roboart import roboart
+from RoboArt import roboart
 ra = roboart()
 ```
 
 Then, generate an avatar by passing a hash value to the robo() method:
 
 ```python
 ra.robo("thisishash")
 ```
 
 This will generate an avatar based on the provided hash value.
 
 ## Quick Example
 
 ```python
-from roboart import roboart
+from RoboArt import roboart
 
 ra = roboart()
 
-ra.robo("Robot") # It generates a robot avatar
-ra.monster("Monster") # It generates a monster avatar
-ra.robohead("Head") # It generates a robot head avatar
-ra.kitten('cats') # It generates a cat avatar
+# You can use any random string hash, it doesnt matter
+Robot = ra.robo("Robot") # It generates a robot avatar
+Monster = ra.monster("Monster") # It generates a monster avatar
+RoboHead = ra.robohead("Head") # It generates a robot head avatar
+Kittens = ra.kitten('cats') # It generates a cat avatar
+
+print(Robot) # prints robo
 ```
 
 ## License:
 
 This project is licensed under the terms of the MIT license. You can find the full license text in the LICENSE file.
```

### Comparing `RoboArt-0.1.2/RoboArt/RoboArt.py` & `RoboArt-0.1.3/RoboArt/RoboArt.py`

 * *Files identical despite different names*

### Comparing `RoboArt-0.1.2/RoboArt.egg-info/PKG-INFO` & `RoboArt-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoboArt
-Version: 0.1.2
+Version: 0.1.3
 Summary: A basic random avatar generator
 Author: puang59
 Author-email: puang59@proton.me
 Keywords: python,avatar,roboart,random avatar,robohash,robots art
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -21,43 +21,48 @@
 RoboArt is a basic random avatar generator which generates avatar in 4 different sets when hash is provided.
 
 ## Installation
 
 You can install RoboArt via pip:
 
 ```bash
-pip install roboart
+pip3 install -U RoboArt
 ```
 
+This will install the latest version of RoboArt
+
 ## Usage
 
 Import RoboArt in your Python script and create an instance of the roboart class:
 
 ```python
-from roboart import roboart
+from RoboArt import roboart
 ra = roboart()
 ```
 
 Then, generate an avatar by passing a hash value to the robo() method:
 
 ```python
 ra.robo("thisishash")
 ```
 
 This will generate an avatar based on the provided hash value.
 
 ## Quick Example
 
 ```python
-from roboart import roboart
+from RoboArt import roboart
 
 ra = roboart()
 
-ra.robo("Robot") # It generates a robot avatar
-ra.monster("Monster") # It generates a monster avatar
-ra.robohead("Head") # It generates a robot head avatar
-ra.kitten('cats') # It generates a cat avatar
+# You can use any random string hash, it doesnt matter
+Robot = ra.robo("Robot") # It generates a robot avatar
+Monster = ra.monster("Monster") # It generates a monster avatar
+RoboHead = ra.robohead("Head") # It generates a robot head avatar
+Kittens = ra.kitten('cats') # It generates a cat avatar
+
+print(Robot) # prints robo
 ```
 
 ## License:
 
 This project is licensed under the terms of the MIT license. You can find the full license text in the LICENSE file.
```

### Comparing `RoboArt-0.1.2/setup.py` & `RoboArt-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'A basic random avatar generator'
 
 # Setting up
 setup(
     name="RoboArt",
     version=VERSION,
     author="puang59",
```

