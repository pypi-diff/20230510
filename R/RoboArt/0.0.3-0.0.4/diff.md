# Comparing `tmp/RoboArt-0.0.3.tar.gz` & `tmp/RoboArt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoboArt-0.0.3.tar", last modified: Wed May 10 10:44:53 2023, max compression
+gzip compressed data, was "RoboArt-0.0.4.tar", last modified: Wed May 10 11:03:28 2023, max compression
```

## Comparing `RoboArt-0.0.3.tar` & `RoboArt-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:44:53.738748 RoboArt-0.0.3/
--rw-r--r--   0 puang59    (501) staff       (20)     1064 2023-05-10 08:26:19.000000 RoboArt-0.0.3/LICENSE.txt
--rw-r--r--   0 puang59    (501) staff       (20)     1266 2023-05-10 10:44:53.738585 RoboArt-0.0.3/PKG-INFO
--rw-r--r--   0 puang59    (501) staff       (20)      659 2023-05-10 10:38:49.000000 RoboArt-0.0.3/README.md
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:44:53.737065 RoboArt-0.0.3/RoboArt/
--rw-r--r--   0 puang59    (501) staff       (20)      613 2023-05-10 10:24:35.000000 RoboArt-0.0.3/RoboArt/RoboArt.py
--rw-r--r--   0 puang59    (501) staff       (20)      308 2023-05-10 08:30:21.000000 RoboArt-0.0.3/RoboArt/__init__.py
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 10:44:53.738007 RoboArt-0.0.3/RoboArt.egg-info/
--rw-r--r--   0 puang59    (501) staff       (20)     1266 2023-05-10 10:44:53.000000 RoboArt-0.0.3/RoboArt.egg-info/PKG-INFO
--rw-r--r--   0 puang59    (501) staff       (20)      356 2023-05-10 10:44:53.000000 RoboArt-0.0.3/RoboArt.egg-info/SOURCES.txt
--rw-r--r--   0 puang59    (501) staff       (20)        1 2023-05-10 10:44:53.000000 RoboArt-0.0.3/RoboArt.egg-info/dependency_links.txt
--rw-r--r--   0 puang59    (501) staff       (20)        8 2023-05-10 10:44:53.000000 RoboArt-0.0.3/RoboArt.egg-info/top_level.txt
--rw-r--r--   0 puang59    (501) staff       (20)       38 2023-05-10 10:44:53.738804 RoboArt-0.0.3/setup.cfg
--rw-r--r--   0 puang59    (501) staff       (20)      945 2023-05-10 10:44:43.000000 RoboArt-0.0.3/setup.py
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:03:28.100244 RoboArt-0.0.4/
+-rw-r--r--   0 puang59    (501) staff       (20)     1064 2023-05-10 08:26:19.000000 RoboArt-0.0.4/LICENSE.txt
+-rw-r--r--   0 puang59    (501) staff       (20)     1545 2023-05-10 11:03:28.100135 RoboArt-0.0.4/PKG-INFO
+-rw-r--r--   0 puang59    (501) staff       (20)      938 2023-05-10 11:03:00.000000 RoboArt-0.0.4/README.md
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:03:28.099226 RoboArt-0.0.4/RoboArt/
+-rw-r--r--   0 puang59    (501) staff       (20)      612 2023-05-10 11:03:08.000000 RoboArt-0.0.4/RoboArt/RoboArt.py
+-rw-r--r--   0 puang59    (501) staff       (20)      308 2023-05-10 08:30:21.000000 RoboArt-0.0.4/RoboArt/__init__.py
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:03:28.099753 RoboArt-0.0.4/RoboArt.egg-info/
+-rw-r--r--   0 puang59    (501) staff       (20)     1545 2023-05-10 11:03:28.000000 RoboArt-0.0.4/RoboArt.egg-info/PKG-INFO
+-rw-r--r--   0 puang59    (501) staff       (20)      356 2023-05-10 11:03:28.000000 RoboArt-0.0.4/RoboArt.egg-info/SOURCES.txt
+-rw-r--r--   0 puang59    (501) staff       (20)        1 2023-05-10 11:03:28.000000 RoboArt-0.0.4/RoboArt.egg-info/dependency_links.txt
+-rw-r--r--   0 puang59    (501) staff       (20)        8 2023-05-10 11:03:28.000000 RoboArt-0.0.4/RoboArt.egg-info/top_level.txt
+-rw-r--r--   0 puang59    (501) staff       (20)       38 2023-05-10 11:03:28.100288 RoboArt-0.0.4/setup.cfg
+-rw-r--r--   0 puang59    (501) staff       (20)      945 2023-05-10 10:56:17.000000 RoboArt-0.0.4/setup.py
```

### Comparing `RoboArt-0.0.3/LICENSE.txt` & `RoboArt-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RoboArt-0.0.3/PKG-INFO` & `RoboArt-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoboArt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A basic random avatar generator
 Home-page: UNKNOWN
 Author: puang59
 Author-email: puang59@proton.me
 License: UNKNOWN
 Keywords: python,avatar,roboart,random avatar,robohash,robots art
 Platform: UNKNOWN
@@ -15,39 +15,52 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # RoboArt
 
-RoboArt is a basic random avatar generator which generates avatar in 3 different sets when hash is provided.
+RoboArt is a basic random avatar generator which generates avatar in 4 different sets when hash is provided.
 
 ## Installation
 
 You can install RoboArt via pip:
 
 ```bash
-pip install RoboArt
+pip install roboart
 ```
 
 ## Usage
 
 Import RoboArt in your Python script and create an instance of the roboart class:
 
 ```python
-from RoboArt import roboart
+from roboart import roboart
 ra = roboart()
 ```
 
 Then, generate an avatar by passing a hash value to the robo() method:
 
 ```python
 ra.robo("thisishash")
 ```
 
 This will generate an avatar based on the provided hash value.
 
+## Quick Example
+
+```python
+from roboart impot roboart
+
+ra = roboart()
+
+ra.robo("Robot") # It generates a robot avatar
+ra.monster("Monster") # It generates a monster avatar
+ra.robohead("Head") # It generates a robot head avatar
+ra.kitten('cats') # It generates a cat avatar
+```
+
 ## License:
 
 This project is licensed under the terms of the MIT license. You can find the full license text in the LICENSE file.
```

### Comparing `RoboArt-0.0.3/README.md` & `RoboArt-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 # RoboArt
 
-RoboArt is a basic random avatar generator which generates avatar in 3 different sets when hash is provided.
+RoboArt is a basic random avatar generator which generates avatar in 4 different sets when hash is provided.
 
 ## Installation
 
 You can install RoboArt via pip:
 
 ```bash
-pip install RoboArt
+pip install roboart
 ```
 
 ## Usage
 
 Import RoboArt in your Python script and create an instance of the roboart class:
 
 ```python
-from RoboArt import roboart
+from roboart import roboart
 ra = roboart()
 ```
 
 Then, generate an avatar by passing a hash value to the robo() method:
 
 ```python
 ra.robo("thisishash")
 ```
 
 This will generate an avatar based on the provided hash value.
 
+## Quick Example
+
+```python
+from roboart impot roboart
+
+ra = roboart()
+
+ra.robo("Robot") # It generates a robot avatar
+ra.monster("Monster") # It generates a monster avatar
+ra.robohead("Head") # It generates a robot head avatar
+ra.kitten('cats') # It generates a cat avatar
+```
+
 ## License:
 
 This project is licensed under the terms of the MIT license. You can find the full license text in the LICENSE file.
```

### Comparing `RoboArt-0.0.3/RoboArt/RoboArt.py` & `RoboArt-0.0.4/RoboArt/RoboArt.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,11 +10,11 @@
         avatar = f"{self.base_url}/{hash}.png/?set=set{int(set)}"
         return avatar
     
     def robohead(self, hash: str, set=3): 
         avatar = f"{self.base_url}/{hash}.png/?set=set{int(set)}"
         return avatar
 
-    def kittens(self, hash: str, set=4): 
+    def kitten(self, hash: str, set=4): 
         avatar = f"{self.base_url}/{hash}.png/?set=set{int(set)}"
         return avatar
```

### Comparing `RoboArt-0.0.3/RoboArt.egg-info/PKG-INFO` & `RoboArt-0.0.4/RoboArt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoboArt
-Version: 0.0.3
+Version: 0.0.4
 Summary: A basic random avatar generator
 Home-page: UNKNOWN
 Author: puang59
 Author-email: puang59@proton.me
 License: UNKNOWN
 Keywords: python,avatar,roboart,random avatar,robohash,robots art
 Platform: UNKNOWN
@@ -15,39 +15,52 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # RoboArt
 
-RoboArt is a basic random avatar generator which generates avatar in 3 different sets when hash is provided.
+RoboArt is a basic random avatar generator which generates avatar in 4 different sets when hash is provided.
 
 ## Installation
 
 You can install RoboArt via pip:
 
 ```bash
-pip install RoboArt
+pip install roboart
 ```
 
 ## Usage
 
 Import RoboArt in your Python script and create an instance of the roboart class:
 
 ```python
-from RoboArt import roboart
+from roboart import roboart
 ra = roboart()
 ```
 
 Then, generate an avatar by passing a hash value to the robo() method:
 
 ```python
 ra.robo("thisishash")
 ```
 
 This will generate an avatar based on the provided hash value.
 
+## Quick Example
+
+```python
+from roboart impot roboart
+
+ra = roboart()
+
+ra.robo("Robot") # It generates a robot avatar
+ra.monster("Monster") # It generates a monster avatar
+ra.robohead("Head") # It generates a robot head avatar
+ra.kitten('cats') # It generates a cat avatar
+```
+
 ## License:
 
 This project is licensed under the terms of the MIT license. You can find the full license text in the LICENSE file.
```

### Comparing `RoboArt-0.0.3/setup.py` & `RoboArt-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A basic random avatar generator'
 
 # Setting up
 setup(
     name="RoboArt",
     version=VERSION,
     author="puang59",
```

