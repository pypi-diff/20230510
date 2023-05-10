# Comparing `tmp/mongogettersetter-1.4.3.tar.gz` & `tmp/mongogettersetter-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.4.3.tar", last modified: Wed May 10 01:32:11 2023, max compression
+gzip compressed data, was "mongogettersetter-1.4.4.tar", last modified: Wed May 10 01:39:00 2023, max compression
```

## Comparing `mongogettersetter-1.4.3.tar` & `mongogettersetter-1.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31168 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30580 2023-05-10 01:31:50.000000 mongogettersetter-1.4.3/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29255 2023-05-10 01:29:49.000000 mongogettersetter-1.4.3/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31168 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      870 2023-05-10 01:30:50.000000 mongogettersetter-1.4.3/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:39:00.977051 mongogettersetter-1.4.4/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31159 2023-05-10 01:39:00.977051 mongogettersetter-1.4.4/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30571 2023-05-10 01:38:20.000000 mongogettersetter-1.4.4/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:39:00.977051 mongogettersetter-1.4.4/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29255 2023-05-10 01:29:49.000000 mongogettersetter-1.4.4/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:39:00.977051 mongogettersetter-1.4.4/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31159 2023-05-10 01:39:00.000000 mongogettersetter-1.4.4/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-10 01:39:00.000000 mongogettersetter-1.4.4/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-10 01:39:00.000000 mongogettersetter-1.4.4/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-10 01:39:00.000000 mongogettersetter-1.4.4/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-10 01:39:00.000000 mongogettersetter-1.4.4/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-10 01:39:00.977051 mongogettersetter-1.4.4/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      870 2023-05-10 01:38:06.000000 mongogettersetter-1.4.4/setup.py
```

### Comparing `mongogettersetter-1.4.3/PKG-INFO` & `mongogettersetter-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.4.3
+Version: 1.4.4
 Summary: A clean way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -300,18 +300,16 @@
 <class 'mongogettersetter.MongoDictWrapper'>
 >>> e.data.hobies.composer[1].get('co_singer')
 ['sushila', 'rakshitha', 'divagar']
 >>> e.data.hobies.composer[1].get()
 {'co_singer': ['sushila', 'rakshitha', 'divagar'], 'main_singer': 'SPB'}
 >>> type(e.data.hobies.composer[1].get())
 <class 'dict'>
->>> 
 ```
 
-```
 ## MongoGetterSetter
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
```

### Comparing `mongogettersetter-1.4.3/README.md` & `mongogettersetter-1.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -284,18 +284,16 @@
 <class 'mongogettersetter.MongoDictWrapper'>
 >>> e.data.hobies.composer[1].get('co_singer')
 ['sushila', 'rakshitha', 'divagar']
 >>> e.data.hobies.composer[1].get()
 {'co_singer': ['sushila', 'rakshitha', 'divagar'], 'main_singer': 'SPB'}
 >>> type(e.data.hobies.composer[1].get())
 <class 'dict'>
->>> 
 ```
 
-```
 ## MongoGetterSetter
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
```

### Comparing `mongogettersetter-1.4.3/mongogettersetter/__init__.py` & `mongogettersetter-1.4.4/mongogettersetter/__init__.py`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.4.3/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.4.4/mongogettersetter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.4.3
+Version: 1.4.4
 Summary: A clean way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -300,18 +300,16 @@
 <class 'mongogettersetter.MongoDictWrapper'>
 >>> e.data.hobies.composer[1].get('co_singer')
 ['sushila', 'rakshitha', 'divagar']
 >>> e.data.hobies.composer[1].get()
 {'co_singer': ['sushila', 'rakshitha', 'divagar'], 'main_singer': 'SPB'}
 >>> type(e.data.hobies.composer[1].get())
 <class 'dict'>
->>> 
 ```
 
-```
 ## MongoGetterSetter
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
```

### Comparing `mongogettersetter-1.4.3/setup.py` & `mongogettersetter-1.4.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.4.3',
+    version='1.4.4',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

