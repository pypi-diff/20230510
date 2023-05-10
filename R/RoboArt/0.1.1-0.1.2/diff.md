# Comparing `tmp/RoboArt-0.1.1.tar.gz` & `tmp/RoboArt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoboArt-0.1.1.tar", last modified: Wed May 10 11:46:58 2023, max compression
+gzip compressed data, was "RoboArt-0.1.2.tar", last modified: Wed May 10 11:53:34 2023, max compression
```

## Comparing `RoboArt-0.1.1.tar` & `RoboArt-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:46:58.940799 RoboArt-0.1.1/
--rw-r--r--   0 puang59    (501) staff       (20)     1064 2023-05-10 08:26:19.000000 RoboArt-0.1.1/LICENSE.txt
--rw-r--r--   0 puang59    (501) staff       (20)     1538 2023-05-10 11:46:58.940672 RoboArt-0.1.1/PKG-INFO
--rw-r--r--   0 puang59    (501) staff       (20)      987 2023-05-10 11:30:24.000000 RoboArt-0.1.1/README.md
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:46:58.939833 RoboArt-0.1.1/RoboArt/
--rw-r--r--   0 puang59    (501) staff       (20)      612 2023-05-10 11:33:04.000000 RoboArt-0.1.1/RoboArt/RoboArt.py
--rw-r--r--   0 puang59    (501) staff       (20)      308 2023-05-10 08:30:21.000000 RoboArt-0.1.1/RoboArt/__init__.py
-drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:46:58.940488 RoboArt-0.1.1/RoboArt.egg-info/
--rw-r--r--   0 puang59    (501) staff       (20)     1538 2023-05-10 11:46:58.000000 RoboArt-0.1.1/RoboArt.egg-info/PKG-INFO
--rw-r--r--   0 puang59    (501) staff       (20)      193 2023-05-10 11:46:58.000000 RoboArt-0.1.1/RoboArt.egg-info/SOURCES.txt
--rw-r--r--   0 puang59    (501) staff       (20)        1 2023-05-10 11:46:58.000000 RoboArt-0.1.1/RoboArt.egg-info/dependency_links.txt
--rw-r--r--   0 puang59    (501) staff       (20)        8 2023-05-10 11:46:58.000000 RoboArt-0.1.1/RoboArt.egg-info/top_level.txt
--rw-r--r--   0 puang59    (501) staff       (20)       38 2023-05-10 11:46:58.940852 RoboArt-0.1.1/setup.cfg
--rw-r--r--   0 puang59    (501) staff       (20)      921 2023-05-10 11:46:07.000000 RoboArt-0.1.1/setup.py
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:53:34.399949 RoboArt-0.1.2/
+-rw-r--r--   0 puang59    (501) staff       (20)     1064 2023-05-10 08:26:19.000000 RoboArt-0.1.2/LICENSE.txt
+-rw-r--r--   0 puang59    (501) staff       (20)     1538 2023-05-10 11:53:34.399825 RoboArt-0.1.2/PKG-INFO
+-rw-r--r--   0 puang59    (501) staff       (20)      987 2023-05-10 11:30:24.000000 RoboArt-0.1.2/README.md
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:53:34.399096 RoboArt-0.1.2/RoboArt/
+-rw-r--r--   0 puang59    (501) staff       (20)      612 2023-05-10 11:33:04.000000 RoboArt-0.1.2/RoboArt/RoboArt.py
+-rw-r--r--   0 puang59    (501) staff       (20)      306 2023-05-10 11:53:18.000000 RoboArt-0.1.2/RoboArt/__init__.py
+drwxr-xr-x   0 puang59    (501) staff       (20)        0 2023-05-10 11:53:34.399641 RoboArt-0.1.2/RoboArt.egg-info/
+-rw-r--r--   0 puang59    (501) staff       (20)     1538 2023-05-10 11:53:34.000000 RoboArt-0.1.2/RoboArt.egg-info/PKG-INFO
+-rw-r--r--   0 puang59    (501) staff       (20)      193 2023-05-10 11:53:34.000000 RoboArt-0.1.2/RoboArt.egg-info/SOURCES.txt
+-rw-r--r--   0 puang59    (501) staff       (20)        1 2023-05-10 11:53:34.000000 RoboArt-0.1.2/RoboArt.egg-info/dependency_links.txt
+-rw-r--r--   0 puang59    (501) staff       (20)        8 2023-05-10 11:53:34.000000 RoboArt-0.1.2/RoboArt.egg-info/top_level.txt
+-rw-r--r--   0 puang59    (501) staff       (20)       38 2023-05-10 11:53:34.399996 RoboArt-0.1.2/setup.cfg
+-rw-r--r--   0 puang59    (501) staff       (20)      921 2023-05-10 11:53:26.000000 RoboArt-0.1.2/setup.py
```

### Comparing `RoboArt-0.1.1/LICENSE.txt` & `RoboArt-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RoboArt-0.1.1/PKG-INFO` & `RoboArt-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoboArt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A basic random avatar generator
 Author: puang59
 Author-email: puang59@proton.me
 Keywords: python,avatar,roboart,random avatar,robohash,robots art
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RoboArt-0.1.1/README.md` & `RoboArt-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `RoboArt-0.1.1/RoboArt/RoboArt.py` & `RoboArt-0.1.2/RoboArt/RoboArt.py`

 * *Files identical despite different names*

### Comparing `RoboArt-0.1.1/RoboArt.egg-info/PKG-INFO` & `RoboArt-0.1.2/RoboArt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoboArt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A basic random avatar generator
 Author: puang59
 Author-email: puang59@proton.me
 Keywords: python,avatar,roboart,random avatar,robohash,robots art
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RoboArt-0.1.1/setup.py` & `RoboArt-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'A basic random avatar generator'
 
 # Setting up
 setup(
     name="RoboArt",
     version=VERSION,
     author="puang59",
```

