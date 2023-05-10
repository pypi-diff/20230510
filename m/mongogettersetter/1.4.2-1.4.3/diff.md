# Comparing `tmp/mongogettersetter-1.4.2.tar.gz` & `tmp/mongogettersetter-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.4.2.tar", last modified: Wed May 10 01:26:54 2023, max compression
+gzip compressed data, was "mongogettersetter-1.4.3.tar", last modified: Wed May 10 01:32:11 2023, max compression
```

## Comparing `mongogettersetter-1.4.2.tar` & `mongogettersetter-1.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:26:54.918196 mongogettersetter-1.4.2/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31062 2023-05-10 01:26:54.918196 mongogettersetter-1.4.2/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30474 2023-05-10 01:17:54.000000 mongogettersetter-1.4.2/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:26:54.914196 mongogettersetter-1.4.2/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29255 2023-05-10 01:24:40.000000 mongogettersetter-1.4.2/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:26:54.918196 mongogettersetter-1.4.2/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31062 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-10 01:26:54.000000 mongogettersetter-1.4.2/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-10 01:26:54.918196 mongogettersetter-1.4.2/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      870 2023-05-10 00:26:21.000000 mongogettersetter-1.4.2/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31168 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30580 2023-05-10 01:31:50.000000 mongogettersetter-1.4.3/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29255 2023-05-10 01:29:49.000000 mongogettersetter-1.4.3/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    31168 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-10 01:32:11.000000 mongogettersetter-1.4.3/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-10 01:32:11.281675 mongogettersetter-1.4.3/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      870 2023-05-10 01:30:50.000000 mongogettersetter-1.4.3/setup.py
```

### Comparing `mongogettersetter-1.4.2/PKG-INFO` & `mongogettersetter-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.4.2
+Version: 1.4.3
 Summary: A clean way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -429,14 +429,16 @@
 
 - `update(self, field, match, **kvalues)`: Updates the nested field `field` of the document's key where the `field` value matches `match`, with the key-value pairs provided in `kvalues`.
 
 - `insert(self, index, value)`: Inserts the given `value` at the specified `index` in the array of the document's key.
 
 - `index(self, value)`: Find the index of the given value in array. It will return -1 if the value is not present in the list.
 
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection.
+
 - `delete(self)`: Delets the key from MongoDB Document
 
 - `__getitem__(self, index)`: Returns the value of the array of the document's key at the specified `index`.
 
 - `__setitem__(self, index, value)`: Sets the value of the array of the document's key at the specified `index` to the given `value`.
 
 - `__delitem__(self, index)`: Removes the value of the array of the document's key at the specified `index`.
@@ -758,14 +760,15 @@
    - `pull`
    - `pullAll`
    - `size`
    - `elemMatch`
    - `all`
    - `update`
    - `delete`
+   - `refresh`
    - `__len__`
    - `__str__`
    - `__repr__`
    - `__getattr__`
    - `__getitem__`
    - `__setattr__`
    - `__setitem__`
```

### Comparing `mongogettersetter-1.4.2/README.md` & `mongogettersetter-1.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -413,14 +413,16 @@
 
 - `update(self, field, match, **kvalues)`: Updates the nested field `field` of the document's key where the `field` value matches `match`, with the key-value pairs provided in `kvalues`.
 
 - `insert(self, index, value)`: Inserts the given `value` at the specified `index` in the array of the document's key.
 
 - `index(self, value)`: Find the index of the given value in array. It will return -1 if the value is not present in the list.
 
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection.
+
 - `delete(self)`: Delets the key from MongoDB Document
 
 - `__getitem__(self, index)`: Returns the value of the array of the document's key at the specified `index`.
 
 - `__setitem__(self, index, value)`: Sets the value of the array of the document's key at the specified `index` to the given `value`.
 
 - `__delitem__(self, index)`: Removes the value of the array of the document's key at the specified `index`.
@@ -742,14 +744,15 @@
    - `pull`
    - `pullAll`
    - `size`
    - `elemMatch`
    - `all`
    - `update`
    - `delete`
+   - `refresh`
    - `__len__`
    - `__str__`
    - `__repr__`
    - `__getattr__`
    - `__getitem__`
    - `__setattr__`
    - `__setitem__`
```

### Comparing `mongogettersetter-1.4.2/mongogettersetter/__init__.py` & `mongogettersetter-1.4.3/mongogettersetter/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -746,19 +746,19 @@
 
     def pop(self, _key, default=None):
         """
         Pop the value of the key from the dictionary and update the database. If the key is not present, return the default value.
         """
 
         value = super().pop(_key, default)
-        self._context.refresh()
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path + "." + _key: ""}}
         )
+        self._context.refresh()
         return value
 
     def update(self, other):
         """
         Update the dictionary with the other dictionary and update the database.
         """
```

### Comparing `mongogettersetter-1.4.2/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.4.3/mongogettersetter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.4.2
+Version: 1.4.3
 Summary: A clean way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -429,14 +429,16 @@
 
 - `update(self, field, match, **kvalues)`: Updates the nested field `field` of the document's key where the `field` value matches `match`, with the key-value pairs provided in `kvalues`.
 
 - `insert(self, index, value)`: Inserts the given `value` at the specified `index` in the array of the document's key.
 
 - `index(self, value)`: Find the index of the given value in array. It will return -1 if the value is not present in the list.
 
+- `refresh(self)`: Refreshes the object with the latest data from the MongoDB collection.
+
 - `delete(self)`: Delets the key from MongoDB Document
 
 - `__getitem__(self, index)`: Returns the value of the array of the document's key at the specified `index`.
 
 - `__setitem__(self, index, value)`: Sets the value of the array of the document's key at the specified `index` to the given `value`.
 
 - `__delitem__(self, index)`: Removes the value of the array of the document's key at the specified `index`.
@@ -758,14 +760,15 @@
    - `pull`
    - `pullAll`
    - `size`
    - `elemMatch`
    - `all`
    - `update`
    - `delete`
+   - `refresh`
    - `__len__`
    - `__str__`
    - `__repr__`
    - `__getattr__`
    - `__getitem__`
    - `__setattr__`
    - `__setitem__`
```

### Comparing `mongogettersetter-1.4.2/setup.py` & `mongogettersetter-1.4.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.4.2',
+    version='1.4.3',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

