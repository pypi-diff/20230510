# Comparing `tmp/mongogettersetter-1.4.1.tar.gz` & `tmp/mongogettersetter-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.4.1.tar", last modified: Tue May  9 05:23:47 2023, max compression
+gzip compressed data, was "mongogettersetter-1.4.2.tar", last modified: Wed May 10 01:26:54 2023, max compression
```

## Comparing `mongogettersetter-1.4.1.tar` & `mongogettersetter-1.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30181 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29584 2023-05-08 19:25:09.000000 mongogettersetter-1.4.1/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    26957 2023-05-08 19:15:12.000000 mongogettersetter-1.4.1/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30181 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-08 19:15:30.000000 mongogettersetter-1.4.1/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:26:54.918196 mongogettersetter-1.4.2/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31062 2023-05-10 01:26:54.918196 mongogettersetter-1.4.2/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30474 2023-05-10 01:17:54.000000 mongogettersetter-1.4.2/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:26:54.914196 mongogettersetter-1.4.2/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29255 2023-05-10 01:24:40.000000 mongogettersetter-1.4.2/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:26:54.918196 mongogettersetter-1.4.2/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31062 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-10 01:26:54.918196 mongogettersetter-1.4.2/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      870 2023-05-10 00:26:21.000000 mongogettersetter-1.4.2/setup.py
```

### Comparing `mongogettersetter-1.4.1/PKG-INFO` & `mongogettersetter-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.4.1
-Summary: A clean realtime way to handle MongoDB documents in Pythonic way
+Version: 1.4.2
+Summary: A clean way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
-# MongoGetterSetter - A Clean Realtime MongoDB Getter Setter API for Python
+# MongoGetterSetter - A Clean MongoDB Getter Setter API for Python
 
 
 [![PyPI version](https://badge.fury.io/py/mongogettersetter.svg)](https://badge.fury.io/py/mongogettersetter)
 [![Downloads](https://pepy.tech/badge/mongogettersetter)](https://pepy.tech/project/mongogettersetter)
 [![Downloads](https://pepy.tech/badge/mongogettersetter/month)](https://pepy.tech/project/mongogettersetter/month)
 [![Downloads](https://pepy.tech/badge/mongogettersetter/week)](https://pepy.tech/project/mongogettersetter/week)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 
-The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and other datatypes like `int`, `bool` `float` and `list` are all handled by `MongoDataWrapper`.
+The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and primitive datatypes like `int`, `bool` `float` are accessed as attributes of `MongoDictWrapper` and `MongoDataWrapper`. `MongoDataWrapper` is to handle lists and all list/array operations.
 
-Here, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
+This library is created with performance in mind so that only when you initialize the MongoGetterSetter class for the first time into an Collection object, it will fetch the document from the MongoDB only once and cache it in the memory. All the subsequent operations will be done on the cached document. If you want to refresh the document, you can call `refresh()` method on the object. If you make changes to the object, it will be reflected in the MongoDB document and the Python Object will be updated with the new changes.
+
+To Get Started, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
 
 
 ### Usage of `MongoGetterSetter` metaclass
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
@@ -237,29 +239,29 @@
 
 You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array.
 
 ```
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> type(e.data)
-<class 'mongogettersetter.MongoDataWrapper'>
+<class 'mongogettersetter.MongoDictWrapper'>
 >>> type(e.data.get())
 <class 'dict'>
 >>> e.data.arr.push(9)
 True
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8, 9], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> e.data.arr[1] = 100
 >>> e.data.arr
 [1, 100, 3, 4, 5, 6, 7, 8, 9]
 >>> e.data.arr[1]
 100
 ```
 
-All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
+All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB-supported operations.
 
 ```
 >>> e.data.hobies
 {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}
 >>> e.data.hobies.composer
 ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan']
 >>> e.data.hobies.composer.push('rahman')
@@ -300,14 +302,16 @@
 ['sushila', 'rakshitha', 'divagar']
 >>> e.data.hobies.composer[1].get()
 {'co_singer': ['sushila', 'rakshitha', 'divagar'], 'main_singer': 'SPB'}
 >>> type(e.data.hobies.composer[1].get())
 <class 'dict'>
 >>> 
 ```
+
+```
 ## MongoGetterSetter
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
 
@@ -384,14 +388,20 @@
     Example:
     ```
     obj.set({
         "password": "$2$somenewpassword",
         "country": "Malaysia"
     })
     ```
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection
+
+    Example:
+    ```
+    obj.refresh()
+    ```
 
 ## MongoDataWrapper
 
 `MongoDataWrapper` is a subscriptable class, which wraps MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection. Check the list of methods for the allowed operations.
 
 ### Methods
 
@@ -444,14 +454,16 @@
 
 ### Methods
 
 - `__init__(self, *args, **kwargs)`: Constructor method that initializes the base `dict` class.
 
 - `prepare(self, _id, key, collection, filter_query)`: This method initializes the internal data structure that stores information about the document's location in the MongoDB collection.
 
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection.
+
 - `__getitem__(self, key)`: Overrides the base `dict` method to return a wrapped MongoDictWrapper when accessing a nested dictionary.
 
 - `__setitem__(self, key, value)`: Overrides the base `dict` method to update the MongoDB document when setting a key-value pair.
 
 - `__delattr__(self, key)`: Overrides the base `dict` method to delete a key-value pair from the MongoDB document when deleting an attribute.
 
 - `__getattr__(self, key)`: Overrides the base `dict` method to return a wrapped MongoDictWrapper when accessing a nested dictionary.
@@ -729,14 +741,15 @@
    - `__setitem__`
    - `__delitem__`
    - `get`
    - `pop`
    - `update`
    - `clear`
    - `delete`
+   - `refresh`
 
 2. `MongoDataWrapper`: A wrapper class for the data stored in MongoDB documents.
 
    Methods:
    - `get`
    - `inArray`
    - `push`
@@ -771,13 +784,14 @@
    - `__setitem__`
    - `__contains__`
    - `__str__`
    - `__repr__`
    - `__delattr__`
    - `__delitem__`
    - `delete`
+   - `refresh`
 
 
 ## Credits
 
 Thanks to GPT-4 for helping me write this documentation. If you find any errors or something doesn't work as the documentation says, raise an issue here https://git.selfmade.ninja/sibidharan/pymongogettersetter
```

### Comparing `mongogettersetter-1.4.1/README.md` & `mongogettersetter-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# MongoGetterSetter - A Clean Realtime MongoDB Getter Setter API for Python
+# MongoGetterSetter - A Clean MongoDB Getter Setter API for Python
 
 
 [![PyPI version](https://badge.fury.io/py/mongogettersetter.svg)](https://badge.fury.io/py/mongogettersetter)
 [![Downloads](https://pepy.tech/badge/mongogettersetter)](https://pepy.tech/project/mongogettersetter)
 [![Downloads](https://pepy.tech/badge/mongogettersetter/month)](https://pepy.tech/project/mongogettersetter/month)
 [![Downloads](https://pepy.tech/badge/mongogettersetter/week)](https://pepy.tech/project/mongogettersetter/week)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 
-The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and other datatypes like `int`, `bool` `float` and `list` are all handled by `MongoDataWrapper`.
+The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and primitive datatypes like `int`, `bool` `float` are accessed as attributes of `MongoDictWrapper` and `MongoDataWrapper`. `MongoDataWrapper` is to handle lists and all list/array operations.
 
-Here, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
+This library is created with performance in mind so that only when you initialize the MongoGetterSetter class for the first time into an Collection object, it will fetch the document from the MongoDB only once and cache it in the memory. All the subsequent operations will be done on the cached document. If you want to refresh the document, you can call `refresh()` method on the object. If you make changes to the object, it will be reflected in the MongoDB document and the Python Object will be updated with the new changes.
+
+To Get Started, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
 
 
 ### Usage of `MongoGetterSetter` metaclass
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
@@ -221,29 +223,29 @@
 
 You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array.
 
 ```
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> type(e.data)
-<class 'mongogettersetter.MongoDataWrapper'>
+<class 'mongogettersetter.MongoDictWrapper'>
 >>> type(e.data.get())
 <class 'dict'>
 >>> e.data.arr.push(9)
 True
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8, 9], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> e.data.arr[1] = 100
 >>> e.data.arr
 [1, 100, 3, 4, 5, 6, 7, 8, 9]
 >>> e.data.arr[1]
 100
 ```
 
-All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
+All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB-supported operations.
 
 ```
 >>> e.data.hobies
 {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}
 >>> e.data.hobies.composer
 ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan']
 >>> e.data.hobies.composer.push('rahman')
@@ -284,14 +286,16 @@
 ['sushila', 'rakshitha', 'divagar']
 >>> e.data.hobies.composer[1].get()
 {'co_singer': ['sushila', 'rakshitha', 'divagar'], 'main_singer': 'SPB'}
 >>> type(e.data.hobies.composer[1].get())
 <class 'dict'>
 >>> 
 ```
+
+```
 ## MongoGetterSetter
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
 
@@ -368,14 +372,20 @@
     Example:
     ```
     obj.set({
         "password": "$2$somenewpassword",
         "country": "Malaysia"
     })
     ```
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection
+
+    Example:
+    ```
+    obj.refresh()
+    ```
 
 ## MongoDataWrapper
 
 `MongoDataWrapper` is a subscriptable class, which wraps MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection. Check the list of methods for the allowed operations.
 
 ### Methods
 
@@ -428,14 +438,16 @@
 
 ### Methods
 
 - `__init__(self, *args, **kwargs)`: Constructor method that initializes the base `dict` class.
 
 - `prepare(self, _id, key, collection, filter_query)`: This method initializes the internal data structure that stores information about the document's location in the MongoDB collection.
 
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection.
+
 - `__getitem__(self, key)`: Overrides the base `dict` method to return a wrapped MongoDictWrapper when accessing a nested dictionary.
 
 - `__setitem__(self, key, value)`: Overrides the base `dict` method to update the MongoDB document when setting a key-value pair.
 
 - `__delattr__(self, key)`: Overrides the base `dict` method to delete a key-value pair from the MongoDB document when deleting an attribute.
 
 - `__getattr__(self, key)`: Overrides the base `dict` method to return a wrapped MongoDictWrapper when accessing a nested dictionary.
@@ -713,14 +725,15 @@
    - `__setitem__`
    - `__delitem__`
    - `get`
    - `pop`
    - `update`
    - `clear`
    - `delete`
+   - `refresh`
 
 2. `MongoDataWrapper`: A wrapper class for the data stored in MongoDB documents.
 
    Methods:
    - `get`
    - `inArray`
    - `push`
@@ -755,12 +768,13 @@
    - `__setitem__`
    - `__contains__`
    - `__str__`
    - `__repr__`
    - `__delattr__`
    - `__delitem__`
    - `delete`
+   - `refresh`
 
 
 ## Credits
 
 Thanks to GPT-4 for helping me write this documentation. If you find any errors or something doesn't work as the documentation says, raise an issue here https://git.selfmade.ninja/sibidharan/pymongogettersetter
```

### Comparing `mongogettersetter-1.4.1/mongogettersetter/__init__.py` & `mongogettersetter-1.4.2/mongogettersetter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
     """
 
     def __call__(cls, *args, **kwargs):
         """
         Return a new instance of the class
         """
-
+        # print(args)
+        # print(kwargs)
         instance = super().__call__(*args, **kwargs)
         instance.__class__ = type(
             "PyMongoGetterSetter",
             (cls,), 
             {
                 "__getattr__": cls.PyMongoGetterSetter.__getattr__,
                 "__getitem__": cls.PyMongoGetterSetter.__getitem__,
@@ -24,118 +25,130 @@
                 "__str__": cls.PyMongoGetterSetter.__str__,
                 "__repr__": cls.PyMongoGetterSetter.__repr__,
                 "__delattr__": cls.PyMongoGetterSetter.__delattr__,
                 "__delitem__": cls.PyMongoGetterSetter.__delitem__,
                 "delete": cls.PyMongoGetterSetter.delete,
                 "set": cls.PyMongoGetterSetter.set,
                 "get": cls.PyMongoGetterSetter.get,
+                "refresh": cls.PyMongoGetterSetter.refresh,
+                "_data": None,
             },
         )
         return instance
 
     class PyMongoGetterSetter:
 
         """
         `PyMongoGetterSetter` is a class that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
         """
 
         def __getattr__(self, _key):
             """
             Return the value of the key in the array/string/object
             """
-            data = self._collection.find_one(self._filter_query)
-            if isinstance(data[_key], dict):
-                dictwrapper = MongoDictWrapper(data[_key])
-                dictwrapper.prepare(
-                    data, [_key], self._collection, self._filter_query
-                )
-                return dictwrapper
-            elif isinstance(data[_key], list):
-                datawrapper = MongoDataWrapper(
-                    data, [_key], self._collection, self._filter_query
-                )
-                return datawrapper
+            if _key in self.__dict__:
+                return self.__dict__[_key]
             else:
-                return data[_key]
+                data = self._data = self._collection.find_one(self._filter_query) if self._data is None else self._data
+                if isinstance(data[_key], dict):
+                    dictwrapper = MongoDictWrapper(data[_key])
+                    dictwrapper.prepare(
+                        data, [_key], self._collection, self._filter_query, self
+                    )
+                    return dictwrapper
+                elif isinstance(data[_key], list):
+                    datawrapper = MongoDataWrapper(
+                        data, [_key], self._collection, self._filter_query, self
+                    )
+                    return datawrapper
+                else:
+                    return data[_key]
                 
         def __getitem__(self, _key):
             """
             Return the value of the key in the array/string/object
             """
-            #TODO: make sure the filter query runs only once
-            data = self._collection.find_one(self._filter_query)
+            data = self._data = self._collection.find_one(self._filter_query) if self._data is None else self._data
             if isinstance(data[_key], dict):
                 dictwrapper = MongoDictWrapper(data)
                 dictwrapper.prepare(
-                    data, [_key], self._collection, self._filter_query
+                    data, [_key], self._collection, self._filter_query, self
                 )
                 return dictwrapper
             elif isinstance(data[_key], list):
                 datawrapper = MongoDataWrapper(
-                    data, [_key], self._collection, self._filter_query
+                    data, [_key], self._collection, self._filter_query, self
                 )
                 return datawrapper
             else:
                 return data[_key]
 
         def __setattr__(self, _key, value):
             """
             Set the value of the key in the array/string/object
             """
-            _filter_query = self._filter_query
-            self._collection.update_one(_filter_query, {"$set": {_key: value}})
+            if _key in ["_filter_query", "_collection", "_keys", "_data"]:
+                self.__dict__[_key] = value
+            else:
+                _filter_query = self._filter_query
+                self._collection.update_one(_filter_query, {"$set": {_key: value}})
+                self._data = self._collection.find_one(self._filter_query)
 
         def __setitem__(self, _key, value):
             """
             Set the value of the key in the array/string/object
             """
             _filter_query = self._filter_query
             self._collection.update_one(_filter_query, {"$set": {_key: value}})
+            self._data = self._collection.find_one(self._filter_query)
 
         def __contains__(self, _key):
             """
             Return the value of the key in the array/string/object
             """
-            return self._collection.find_one({_key: {"$exists": True}})
+            self._data = self._collection.find_one(self._filter_query) if self._data is None else self._data
+            return _key in self._data
 
         def __str__(self):
             """
             Return the string representation of the array/string/object
             """
-            _filter_query = self._filter_query
-            doc = self._collection.find_one(_filter_query)
-            return json.dumps(doc, indent=4, default=str)
+            self._data = self._collection.find_one(self._filter_query) if self._data is None else self._data
+            return json.dumps(self._data, indent=4, default=str)
 
         def __repr__(self):
             """
             Return the string representation of the array/string/object
             """
-            _filter_query = self._filter_query
-            return str(self._collection.find_one(_filter_query))
+            self._data = self._collection.find_one(self._filter_query) if self._data is None else self._data
+            return json.dumps(self._data, indent=4, default=str)
 
         def __delattr__(self, name):
             """
             Delete the key in the array/string/object using del keyword
             """
             # print(f"___delattr___ name = {name}")
             self._collection.update_one(self._filter_query, {"$unset": {name: ""}})
+            self._data = self._collection.find_one(self._filter_query)
 
         def __delitem__(self, name):
             """
             Delete the key in the array/string/object using del keyword
             """
             # print(f"___delattr___ name = {name}")
             self._collection.update_one(self._filter_query, {"$unset": {name: ""}})
+            self._data = self._collection.find_one(self._filter_query)
             
         def delete(self):
             """
             Delete object from the MongoDB Collection using $unset
             """
             # print(f"deleting {self._id}")
             self._collection.delete_one(self._filter_query)
+            self._data = None
             
         
         def __eq__(self, other):
             """
             Return True if the two objects are equal
             """
             return repr(self) == repr(other)
@@ -147,33 +160,49 @@
             return repr(self) != repr(other)
         
         def set(self, data):
             """
             Set the document in the MongoDB Collection
             """
             self._collection.update_one(self._filter_query, {"$set": data})
+            self._data = self._collection.find_one(self._filter_query)
             
-        def get(self):
+        def get(self, realtime=True):
             """
             Get the document from the MongoDB Collection
             """
-            return self._collection.find_one(self._filter_query)
+            if realtime:
+                self._data = self._collection.find_one(self._filter_query)
+            
+            return self._data
+
+        def refresh(self, _data=None):
+            """
+            Refresh the document from the MongoDB Collection
+            """
+            if _data is not None:
+                self._data = _data
+            else:
+                self._data = self._collection.find_one(self._filter_query)
+                
+            return self._data
             
 
 class MongoDataWrapper:
 
     """
     `MongoDataWrapper` is a subscriptable class, which wraps MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection. Check the list of methods for the allowed operations.
     """
 
-    def __init__(self, data, _key, _collection, _filter_query):
+    def __init__(self, data, _key, _collection, _filter_query, _context):
         self._data = data
         self._filter_query = _filter_query
         self._collection = _collection
         self._keys = _key
+        self._context = _context
 
     def get(self, _key=None, realtime=False):
         """
         Get the original representation of the document as it exists without MongoGetterSetter Wrappers.
         If no arguments are passed, then return the whole data.
         If _key is passed, it will return the specific value w.r.t the key.
         If realtime is set to true, the data is fetched from MongoDB in realtime
@@ -185,84 +214,94 @@
         Returns:
             any: Original Data without Wrapper
 
         """
         if realtime:
             self._data = nested_dict = self._collection.find_one(self._filter_query)
         else:
-            nested_dict = self._data
+            nested_dict = self._context._data
 
         for k in self._keys:
             nested_dict = nested_dict[k]
         if _key is None:
             return nested_dict
         else:
             return nested_dict[_key]
+        
+    def refresh(self):
+        self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
 
     def append(self, *value):
         """
         Append the value to the array. Returns True if the value is appended, else False.
         """
 
         result = self.push(*value)
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         return result
 
     def push(self, *values, maximum=0):
         """
         Push the value to the array. Returns True if the value is pushed, else False.
         """
 
         path = ".".join(str(v) for v in self._keys)
         if maximum == 0:
             result = self._collection.update_one(
                 self._filter_query, {"$push": {path: {"$each": values}}}
             )
             self._data = self._collection.find_one(self._filter_query)
+            self._context.refresh(self._data)
             return result.modified_count > 0
         else:
             update_operation = {"$push": {path: {"$each": values, "$slice": -maximum}}}
 
             result = self._collection.update_one(
                 self._filter_query, update_operation
             ).modified_count
             self._data = self._collection.find_one(self._filter_query)
+            self._context.refresh(self._data)
             return result.modified_count > 0
 
     def addToSet(self, value):
         """
         Add the value to the array if it does not exist. Returns True if the value is added, else False.
         """
 
         path = ".".join(str(v) for v in self._keys)
         result = self._collection.update_one(
             self._filter_query, {"$addToSet": {path: value}}
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         return result.modified_count > 0
 
     def pop(self, direction=1):
         """
         Pop the value from the array. Returns True if the value is popped, else False. direction=1 for popping from the end, direction=-1 for popping from the beginning.
         """
 
         path = ".".join(str(v) for v in self._keys)
         result = self._collection.update_one(
             self._filter_query, {"$pop": {path: direction}}
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         return result.modified_count > 0
 
     def remove(self, item):
         """
         Remove the value from the array. Returns True if the value is removed, else False.
         """
 
         result = self.pull(item)
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         return result
 
     def count(self):
         """
         Return the length of the array/string/object
         """
 
@@ -274,25 +313,27 @@
         """
         
         path = ".".join(str(v) for v in self._keys)
         result = self._collection.update_one(
             self._filter_query, {"$pull": {path: value}}
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         return result.modified_count > 0
 
     def insert(self, index, value):
         """
         Insert the value at the index in the array. Returns True if the value is inserted, else False.
         """
 
         path = ".".join(str(v) for v in self._keys)
         insert_query = {"$push": {path: {"$each": [value], "$position": index}}}
         result = self._collection.update_one(self._filter_query, insert_query)
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         return result.modified_count > 0
         
     def index(self, value):
         """
         Find the index of the value in array. If the value is not present, you will get -1.
         """
         path = ".".join(str(v) for v in self._keys)
@@ -318,14 +359,15 @@
         """
 
         path = ".".join(str(v) for v in self._keys)
         result = self._collection.update_one(
             self._filter_query, {"$pullAll": {path: values}}
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         return result.modified_count > 0
 
     def matchSize(self, value):
         """
         Check if the array has the given size. Returns True if the array has the given size, else False.
         """
 
@@ -362,283 +404,262 @@
         result = self._collection.update_one(
             self._filter_query,
             {"$set": update_query},
             array_filters=[{f"elem.{field}": match}],
             upsert=True,
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         return result.modified_count > 0
 
     def __len__(self):
         """
         Return the length of the array/string/object
         """
 
         return len(self.get())
 
     def __str__(self):
         """
         Return the string representation of the array/string/object
         """
 
-        nested_dict = self._data
-        for k in self._keys:
-            nested_dict = nested_dict[k]
-        return json.dumps(nested_dict, indent=4, default=str)
+        # nested_dict = self._data
+        # for k in self._keys:
+        #     nested_dict = nested_dict[k]
+        return json.dumps(self.get(), indent=4, default=str)
 
     def __repr__(self):
         """
         Return the string representation of the array/string/object
         """
 
-        nested_dict = self._data
-        for k in self._keys:
-            nested_dict = nested_dict[k]
-        return str(nested_dict)
-
-    def __int__(self):
-        """
-        Return the integer representation of the array/string/object
-        """
-
-        nested_dict = self._data
-        for k in self._keys:
-            nested_dict = nested_dict[k]
-        return int(nested_dict)
-
-    def __float__(self):
-        """
-        Return the float representation of the array/string/object
-        """
-
-        nested_dict = self._data
-        for k in self._keys:
-            nested_dict = nested_dict[k]
-        return float(nested_dict)
-
-    def __bool__(self):
-        """
-        Return the boolean representation of the array/string/object
-        """
-
-        nested_dict = self._data
-        for k in self._keys:
-            nested_dict = nested_dict[k]
-        return bool(nested_dict)
+        # nested_dict = self._data
+        # for k in self._keys:
+        #     nested_dict = nested_dict[k]
+        return json.dumps(self.get(), indent=4, default=str)
 
     def __getitem__(self, _key):
         """
         Return the value of the key in the array/string/object
         """
 
-        data = self.get(_key, realtime=True)
+        data = self.get(_key)
         # return data[_key]
         if isinstance(data, dict):
             dictwrapper = MongoDictWrapper(data)
             dictwrapper.prepare(
-                self._data, self._keys + [_key], self._collection, self._filter_query
+                self._data, self._keys + [_key], self._collection, self._filter_query, self._context
             )
             return dictwrapper
         elif isinstance(data, list):
             datawrapper = MongoDataWrapper(
-                self._data, self._keys + [_key], self._collection, self._filter_query
+                self._data, self._keys + [_key], self._collection, self._filter_query, self._context
             )
             return datawrapper
         else:
             return data
             
     def __getattr__(self, _key):
         """
         Return the value of the key in the array/string/object
         """
 
         if _key in self.__dict__:
             return self.__dict__[_key]
         else:
-            data = self.get(_key, realtime=True)
+            data = self.get(_key)
             # return data[_key]
             if isinstance(data, dict):
                 dictwrapper = MongoDictWrapper(data)
                 dictwrapper.prepare(
-                    self._data, self._keys + [_key], self._collection, self._filter_query
+                    self._data, self._keys + [_key], self._collection, self._filter_query, self._context
                 )
                 return dictwrapper
             elif isinstance(data, list):
                 datawrapper = MongoDataWrapper(
-                    self._data, self._keys + [_key], self._collection, self._filter_query
+                    self._data, self._keys + [_key], self._collection, self._filter_query, self._context
                 )
                 return datawrapper
             else:
                 return data
                 
     def __setattr__(self, _key, value):
         """
         Set the value of the key in the array/string/object
         """
         _key = str(_key)
-        if _key in ["_filter_query", "_collection", "_keys", "_data"]:
+        if _key in ["_filter_query", "_collection", "_keys", "_data", "_context"]:
             self.__dict__[_key] = value
         else:
             path = ".".join(str(v) for v in self._keys)
             self._collection.update_one(
                 self._filter_query, {"$set": {path + "." + _key: value}}
             )
             self._data = self._collection.find_one(self._filter_query)
+            self._context.refresh(self._data)
 
     def __setitem__(self, index, value):
         """
         Set the value of the key in the array/string/object
         """
         path = ".".join(str(v) for v in self._keys)
         update_query = {path + "." + str(index): value}
         self._collection.update_one(self._filter_query, {"$set": update_query})
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
 
     def __delitem__(self, _key):
         """
         Delete the key in the array/string/object using del keyword
         """
         path = ".".join(str(v) for v in self._keys)
         data = self.get()
         _key = str(_key)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
         if isinstance(data, list):
             self.pull(None)
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
 
     def __delattr__(self, _key):
         """
         Delete the key in the array/string/object using del keyword
         """
         path = ".".join(str(v) for v in self._keys + [_key])
         data = self.get()
         _key = str(_key)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
         if isinstance(data, list):
             self.pull(None)
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
     
     def __contains__(self, _key):
         return _key in self.get()
 
     def delete(self):
         """
         Delete the nested object from the MongoDB Document using $unset
         """
         
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path: ""}}
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
     
     def refresh(self):
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
 
 class MongoDictWrapper(dict):
     """
     MongoDictWrapper is a wrapper around the dictionary object to provide the functionality of updating the database when the dictionary is updated. It is used to wrap the dictionary object in the MongoGetterSetter class. It is not meant to be used directly.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
     
     def refresh(self):
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
 
-    def prepare(self, _data, _keys, _collection, _filter_query):
+    def prepare(self, _data, _keys, _collection, _filter_query, _context):
         """
         Prepare the MongoDictWrapper object to be used. This method is called by the MongoGetterSetter class when the object is created.
         """
         self._data = _data
         self._filter_query = _filter_query
         self._collection = _collection
         self._keys = _keys
+        self._context = _context
         # path = '.'.join(str(v) for v in self._keys)
         # print(f"__prepare__ you are at: {path}")
 
     def __setattr__(self, _key, value):
         _key = str(_key)
         """
         Set the value of the key in the dictionary and update the database.
         """
-        if _key in ["_filter_query", "_collection", "_keys", "_data"]:
+        if _key in ["_filter_query", "_collection", "_keys", "_data", "_context"]:
             self.__dict__[_key] = value
         else:
             # Call the parent __setitem__ method to actually set the value in the dictionary
             path = ".".join(str(v) for v in self._keys)
             # Execute your function here
             # # print(f"Dictionary updated: {path}.{_key}={value}")
             update = {"$set": {"{}.{}".format(path, _key): value}}
             result = self._collection.update_one(self._filter_query, update)
-            nested_dict = self._collection.find_one(self._filter_query)
+            self._data = nested_dict = self._collection.find_one(self._filter_query)
             for k in self._keys:
                 nested_dict = nested_dict[k]
             # print(f"__setitem__ {str(nested_dict)}")
             super().update(nested_dict)
-            self._data = self._collection.find_one(self._filter_query)
+            self._context.refresh(self._data)
         
 
     def __getattr__(self, _key):
         """
         Get the value of the key in the dictionary.
         """
         
         _key = str(_key)
         if _key in self.__dict__:
             return self.__dict__[_key]
         else:
             path = ".".join(str(v) for v in self._keys)
             # print(f"__getitem__ you are at: {path}")
-            original_dict = self._data
+            original_dict = self._context._data
             nested_dict = dict(original_dict)
             for k in self._keys:
                 nested_dict = nested_dict[k]
             super().update(nested_dict)
             # print(f"__getitem__ {str(nested_dict)}")
             if isinstance(nested_dict[_key], dict):
                 dictwrapper = MongoDictWrapper(nested_dict[_key])
                 dictwrapper.prepare(
-                    original_dict, self._keys + [_key], self._collection, self._filter_query
+                    original_dict, self._keys + [_key], self._collection, self._filter_query, self._context
                 )
                 return dictwrapper
             elif isinstance(nested_dict[_key], list):
                 datawrapper = MongoDataWrapper(
-                    original_dict, self._keys + [_key], self._collection, self._filter_query
+                    original_dict, self._keys + [_key], self._collection, self._filter_query, self._context
                 )
                 return datawrapper
             else:
                 return nested_dict[_key]
 
     def __getitem__(self, _key):
         _key = str(_key)
         """
         Get the value of the key in the dictionary.
         """
         path = ".".join(str(v) for v in self._keys)
         # print(f"__getitem__ you are at: {path}")
-        original_dict = self._data
+        original_dict = self._context._data
         nested_dict = dict(original_dict)
         for k in self._keys:
             nested_dict = nested_dict[k]
         super().update(nested_dict)
         # print(f"__getitem__ {str(nested_dict)}")
         if isinstance(nested_dict[_key], dict):
             dictwrapper = MongoDictWrapper(nested_dict[_key])
             dictwrapper.prepare(
-                original_dict, self._keys + [_key], self._collection, self._filter_query
+                original_dict, self._keys + [_key], self._collection, self._filter_query, self._context
             )
             return dictwrapper
         elif isinstance(nested_dict[_key], list):
             datawrapper = MongoDataWrapper(
-                original_dict, self._keys + [_key], self._collection, self._filter_query
+                original_dict, self._keys + [_key], self._collection, self._filter_query, self._context
             )
             return datawrapper
         else:
             return nested_dict[_key]
 
     def __setitem__(self, _key, value):
         _key = str(_key)
@@ -648,14 +669,15 @@
         # Call the parent __setitem__ method to actually set the value in the dictionary
         path = ".".join(str(v) for v in self._keys)
         # Execute your function here
         # # print(f"Dictionary updated: {path}.{_key}={value}")
         update = {"$set": {"{}.{}".format(path, _key): value}}
         result = self._collection.update_one(self._filter_query, update)
         self._data = nested_dict = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
         for k in self._keys:
             nested_dict = nested_dict[k]
         # print(f"__setitem__ {str(nested_dict)}")
         super().update(nested_dict)
 
     def __delitem__(self, _key):
         _key = str(_key)
@@ -664,51 +686,59 @@
         """
         super().__delitem__(_key)
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
 
     def __delattr_(self, _key):
         _key = str(_key)
         """
         Delete the item from the dictionary and update the database.
         """
         super().__delitem__(_key)
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
     
     def delete(self):
         """
         Delete the nested object from the MongoDB Document using $unset
         """
         
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path: ""}}
         )
         self._data = self._collection.find_one(self._filter_query)
+        self._context.refresh(self._data)
 
     def get(self, _key=None, default=None, realtime=False):
         """
         Get the value of the key from the dictionary. If the key is not present, return the default value.
         """
         if realtime:
             self._data = self._collection.find_one(self._filter_query)
             original_dict = self._data
+            self._context.refresh(self._data)
             nested_dict = dict(original_dict)
             for k in self._keys:
                 nested_dict = nested_dict[k]
             data = nested_dict
         else:
-            data = dict(self)
+            nested_dict = self._context._data
+            for k in self._keys:
+                nested_dict = nested_dict[k]
+            data = nested_dict
+            # data = dict(self)
 
 
         if _key is None:
             return dict(data)
         if _key in self:
             return self[_key]
         else:
@@ -716,14 +746,15 @@
 
     def pop(self, _key, default=None):
         """
         Pop the value of the key from the dictionary and update the database. If the key is not present, return the default value.
         """
 
         value = super().pop(_key, default)
+        self._context.refresh()
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
         return value
 
     def update(self, other):
@@ -733,19 +764,21 @@
 
         super().update(other)
         d = dict(self)
         other.update(d)
         path = ".".join(str(v) for v in self._keys)
         update = {"$set": {path: other}}
         self._collection.update_one(self._filter_query, update, upsert=True)
+        self._context.refresh()
 
     def clear(self):
         """
         Clear the dictionary and update the database.
         """
 
         # print("__clear__ ")
         path = ".".join(str(v) for v in self._keys)
         update = {"$set": {path: {}}}
         self._collection.update_one(self._filter_query, update)
         super().clear()
+        self._context.refresh()
```

### Comparing `mongogettersetter-1.4.1/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.4.2/mongogettersetter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.4.1
-Summary: A clean realtime way to handle MongoDB documents in Pythonic way
+Version: 1.4.2
+Summary: A clean way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 
-# MongoGetterSetter - A Clean Realtime MongoDB Getter Setter API for Python
+# MongoGetterSetter - A Clean MongoDB Getter Setter API for Python
 
 
 [![PyPI version](https://badge.fury.io/py/mongogettersetter.svg)](https://badge.fury.io/py/mongogettersetter)
 [![Downloads](https://pepy.tech/badge/mongogettersetter)](https://pepy.tech/project/mongogettersetter)
 [![Downloads](https://pepy.tech/badge/mongogettersetter/month)](https://pepy.tech/project/mongogettersetter/month)
 [![Downloads](https://pepy.tech/badge/mongogettersetter/week)](https://pepy.tech/project/mongogettersetter/week)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 
-The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and other datatypes like `int`, `bool` `float` and `list` are all handled by `MongoDataWrapper`.
+The idea is to convert MongoDB Document into Python Object of Type `MongoGetterSetter` in High Level, and all other document's sub documents are treated as `dict` wrapped with `MongoDictWrapper` and primitive datatypes like `int`, `bool` `float` are accessed as attributes of `MongoDictWrapper` and `MongoDataWrapper`. `MongoDataWrapper` is to handle lists and all list/array operations.
 
-Here, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
+This library is created with performance in mind so that only when you initialize the MongoGetterSetter class for the first time into an Collection object, it will fetch the document from the MongoDB only once and cache it in the memory. All the subsequent operations will be done on the cached document. If you want to refresh the document, you can call `refresh()` method on the object. If you make changes to the object, it will be reflected in the MongoDB document and the Python Object will be updated with the new changes.
+
+To Get Started, we initialize `Employee` and `EmployeeCollection` class with `_collection` and `_filter_query` as mandatory attributes for `MongoGetterSetter` to function properly. These 2 attributes are used internally to do further manipulations to MongoDB documents. You can change the `_filter_query` attribute to customize the filter query as per your needs. `_collection` should point to the MongoDB collection.
 
 
 ### Usage of `MongoGetterSetter` metaclass
 ```
 from pymongo import MongoClient
 from mongogettersetter import MongoGetterSetter
 
@@ -237,29 +239,29 @@
 
 You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array.
 
 ```
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> type(e.data)
-<class 'mongogettersetter.MongoDataWrapper'>
+<class 'mongogettersetter.MongoDictWrapper'>
 >>> type(e.data.get())
 <class 'dict'>
 >>> e.data.arr.push(9)
 True
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8, 9], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> e.data.arr[1] = 100
 >>> e.data.arr
 [1, 100, 3, 4, 5, 6, 7, 8, 9]
 >>> e.data.arr[1]
 100
 ```
 
-All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
+All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB-supported operations.
 
 ```
 >>> e.data.hobies
 {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}
 >>> e.data.hobies.composer
 ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan']
 >>> e.data.hobies.composer.push('rahman')
@@ -300,14 +302,16 @@
 ['sushila', 'rakshitha', 'divagar']
 >>> e.data.hobies.composer[1].get()
 {'co_singer': ['sushila', 'rakshitha', 'divagar'], 'main_singer': 'SPB'}
 >>> type(e.data.hobies.composer[1].get())
 <class 'dict'>
 >>> 
 ```
+
+```
 ## MongoGetterSetter
 
 `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
 ### Methods
 
 - `__getattr__(self, key)`: Returns a `MongoDataWrapper` instance for the given `key`. See below for the capabalities of `MongoDataWrapper`
 
@@ -384,14 +388,20 @@
     Example:
     ```
     obj.set({
         "password": "$2$somenewpassword",
         "country": "Malaysia"
     })
     ```
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection
+
+    Example:
+    ```
+    obj.refresh()
+    ```
 
 ## MongoDataWrapper
 
 `MongoDataWrapper` is a subscriptable class, which wraps MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection. Check the list of methods for the allowed operations.
 
 ### Methods
 
@@ -444,14 +454,16 @@
 
 ### Methods
 
 - `__init__(self, *args, **kwargs)`: Constructor method that initializes the base `dict` class.
 
 - `prepare(self, _id, key, collection, filter_query)`: This method initializes the internal data structure that stores information about the document's location in the MongoDB collection.
 
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection.
+
 - `__getitem__(self, key)`: Overrides the base `dict` method to return a wrapped MongoDictWrapper when accessing a nested dictionary.
 
 - `__setitem__(self, key, value)`: Overrides the base `dict` method to update the MongoDB document when setting a key-value pair.
 
 - `__delattr__(self, key)`: Overrides the base `dict` method to delete a key-value pair from the MongoDB document when deleting an attribute.
 
 - `__getattr__(self, key)`: Overrides the base `dict` method to return a wrapped MongoDictWrapper when accessing a nested dictionary.
@@ -729,14 +741,15 @@
    - `__setitem__`
    - `__delitem__`
    - `get`
    - `pop`
    - `update`
    - `clear`
    - `delete`
+   - `refresh`
 
 2. `MongoDataWrapper`: A wrapper class for the data stored in MongoDB documents.
 
    Methods:
    - `get`
    - `inArray`
    - `push`
@@ -771,13 +784,14 @@
    - `__setitem__`
    - `__contains__`
    - `__str__`
    - `__repr__`
    - `__delattr__`
    - `__delitem__`
    - `delete`
+   - `refresh`
 
 
 ## Credits
 
 Thanks to GPT-4 for helping me write this documentation. If you find any errors or something doesn't work as the documentation says, raise an issue here https://git.selfmade.ninja/sibidharan/pymongogettersetter
```

### Comparing `mongogettersetter-1.4.1/setup.py` & `mongogettersetter-1.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.4.1',
+    version='1.4.2',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
-    description='A clean realtime way to handle MongoDB documents in Pythonic way',
+    description='A clean way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
```

