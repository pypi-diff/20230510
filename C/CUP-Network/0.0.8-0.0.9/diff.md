# Comparing `tmp/CUP_Network-0.0.8.tar.gz` & `tmp/CUP_Network-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUP_Network-0.0.8.tar", last modified: Fri Oct 21 05:18:28 2022, max compression
+gzip compressed data, was "CUP_Network-0.0.9.tar", last modified: Fri Oct 21 05:22:51 2022, max compression
```

## Comparing `CUP_Network-0.0.8.tar` & `CUP_Network-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-10-21 05:18:28.703372 CUP_Network-0.0.8/
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-10-21 05:18:28.702259 CUP_Network-0.0.8/CUP_Network/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1658 2022-10-21 05:12:03.000000 CUP_Network-0.0.8/CUP_Network/__config__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     3178 2022-10-21 05:16:28.000000 CUP_Network-0.0.8/CUP_Network/__init__.py
--rw-r--r--   0 lianhaocheng   (501) staff       (20)     1288 2022-10-21 05:14:15.000000 CUP_Network-0.0.8/CUP_Network/main.py
-drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-10-21 05:18:28.702984 CUP_Network-0.0.8/CUP_Network.egg-info/
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      930 2022-10-21 05:18:28.000000 CUP_Network-0.0.8/CUP_Network.egg-info/PKG-INFO
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      330 2022-10-21 05:18:28.000000 CUP_Network-0.0.8/CUP_Network.egg-info/SOURCES.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-10-21 05:18:28.000000 CUP_Network-0.0.8/CUP_Network.egg-info/dependency_links.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       54 2022-10-21 05:18:28.000000 CUP_Network-0.0.8/CUP_Network.egg-info/entry_points.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       14 2022-10-21 05:18:28.000000 CUP_Network-0.0.8/CUP_Network.egg-info/requires.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       12 2022-10-21 05:18:28.000000 CUP_Network-0.0.8/CUP_Network.egg-info/top_level.txt
--rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-09-06 10:30:25.000000 CUP_Network-0.0.8/CUP_Network.egg-info/zip-safe
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      930 2022-10-21 05:18:28.703261 CUP_Network-0.0.8/PKG-INFO
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      536 2022-09-06 11:28:57.000000 CUP_Network-0.0.8/README.md
--rw-r--r--   0 lianhaocheng   (501) staff       (20)       38 2022-10-21 05:18:28.703412 CUP_Network-0.0.8/setup.cfg
--rw-r--r--   0 lianhaocheng   (501) staff       (20)      862 2022-10-21 05:18:28.000000 CUP_Network-0.0.8/setup.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-10-21 05:22:51.595792 CUP_Network-0.0.9/
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-10-21 05:22:51.594689 CUP_Network-0.0.9/CUP_Network/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1653 2022-10-21 05:22:40.000000 CUP_Network-0.0.9/CUP_Network/__config__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     3178 2022-10-21 05:16:28.000000 CUP_Network-0.0.9/CUP_Network/__init__.py
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)     1288 2022-10-21 05:14:15.000000 CUP_Network-0.0.9/CUP_Network/main.py
+drwxr-xr-x   0 lianhaocheng   (501) staff       (20)        0 2022-10-21 05:22:51.595368 CUP_Network-0.0.9/CUP_Network.egg-info/
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      930 2022-10-21 05:22:51.000000 CUP_Network-0.0.9/CUP_Network.egg-info/PKG-INFO
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      330 2022-10-21 05:22:51.000000 CUP_Network-0.0.9/CUP_Network.egg-info/SOURCES.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-10-21 05:22:51.000000 CUP_Network-0.0.9/CUP_Network.egg-info/dependency_links.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       54 2022-10-21 05:22:51.000000 CUP_Network-0.0.9/CUP_Network.egg-info/entry_points.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       14 2022-10-21 05:22:51.000000 CUP_Network-0.0.9/CUP_Network.egg-info/requires.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       12 2022-10-21 05:22:51.000000 CUP_Network-0.0.9/CUP_Network.egg-info/top_level.txt
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)        1 2022-09-06 10:30:25.000000 CUP_Network-0.0.9/CUP_Network.egg-info/zip-safe
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      930 2022-10-21 05:22:51.595677 CUP_Network-0.0.9/PKG-INFO
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      536 2022-09-06 11:28:57.000000 CUP_Network-0.0.9/README.md
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)       38 2022-10-21 05:22:51.595828 CUP_Network-0.0.9/setup.cfg
+-rw-r--r--   0 lianhaocheng   (501) staff       (20)      862 2022-10-21 05:22:51.000000 CUP_Network-0.0.9/setup.py
```

### Comparing `CUP_Network-0.0.8/CUP_Network/__config__.py` & `CUP_Network-0.0.9/CUP_Network/__config__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,9 +51,9 @@
     def select(self, item):
         if item not in self.config and item in questions:
             self.update(item, encode_password(_ask(questions[item])))
         return decode_password(self.config[item])
 
     def update(self, key, value):
         self.config[key] = value
-        with open(self.config_path, "w") as f:
+        with open(config_path, "w") as f:
             json.dump(self.config, f, indent=4, ensure_ascii=False)
```

### Comparing `CUP_Network-0.0.8/CUP_Network/__init__.py` & `CUP_Network-0.0.9/CUP_Network/__init__.py`

 * *Files identical despite different names*

### Comparing `CUP_Network-0.0.8/CUP_Network/main.py` & `CUP_Network-0.0.9/CUP_Network/main.py`

 * *Files identical despite different names*

### Comparing `CUP_Network-0.0.8/CUP_Network.egg-info/PKG-INFO` & `CUP_Network-0.0.9/CUP_Network.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUP-Network
-Version: 0.0.8
+Version: 0.0.9
 Summary: Draw Mtx As Thumbnail
 Home-page: https://github.com/Rhythmicc/CUP_Network
 Author: RhythmLian
 Author-email: RhythmLian@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CUP_Network-0.0.8/PKG-INFO` & `CUP_Network-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUP_Network
-Version: 0.0.8
+Version: 0.0.9
 Summary: Draw Mtx As Thumbnail
 Home-page: https://github.com/Rhythmicc/CUP_Network
 Author: RhythmLian
 Author-email: RhythmLian@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CUP_Network-0.0.8/README.md` & `CUP_Network-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `CUP_Network-0.0.8/setup.py` & `CUP_Network-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 setup(
     name='CUP_Network',
     version=VERSION,
     description='Draw Mtx As Thumbnail',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

