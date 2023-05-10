# Comparing `tmp/animegifs-0.5.0.tar.gz` & `tmp/animegifs-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.5.0.tar", last modified: Wed May 10 01:22:41 2023, max compression
+gzip compressed data, was "animegifs-0.5.1.tar", last modified: Wed May 10 01:38:38 2023, max compression
```

## Comparing `animegifs-0.5.0.tar` & `animegifs-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 01:22:41.278420 animegifs-0.5.0/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     1184 2023-05-10 01:22:41.277414 animegifs-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      602 2023-05-10 01:21:45.000000 animegifs-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 01:22:41.258413 animegifs-0.5.0/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.0/animegifs/__init__.py
--rw-rw-rw-   0        0        0     2333 2023-05-10 01:17:27.000000 animegifs-0.5.0/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:22:41.275414 animegifs-0.5.0/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.0/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0      356 2023-05-10 00:52:28.000000 animegifs-0.5.0/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     1313 2023-04-28 20:51:38.000000 animegifs-0.5.0/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:22:41.269414 animegifs-0.5.0/animegifs.egg-info/
--rw-rw-rw-   0        0        0     1184 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 01:22:41.000000 animegifs-0.5.0/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 01:22:41.278420 animegifs-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1059 2023-05-10 01:21:45.000000 animegifs-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:38:38.572296 animegifs-0.5.1/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     1193 2023-05-10 01:38:38.571296 animegifs-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-05-10 01:34:05.000000 animegifs-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 01:38:38.555295 animegifs-0.5.1/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.1/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     2262 2023-05-10 01:38:16.000000 animegifs-0.5.1/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:38:38.569296 animegifs-0.5.1/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.1/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-05-10 01:38:16.000000 animegifs-0.5.1/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     1313 2023-04-28 20:51:38.000000 animegifs-0.5.1/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:38:38.564304 animegifs-0.5.1/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     1193 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 01:38:38.572296 animegifs-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-10 01:35:19.000000 animegifs-0.5.1/setup.py
```

### Comparing `animegifs-0.5.0/LICENSE` & `animegifs-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.0/PKG-INFO` & `animegifs-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.0
+Version: 0.5.1
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
-Keywords: anime,gif,python,anime-gif
+Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# anime-gifs.py
+# animegifs.py
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
 WIP - updated in time to time. Versions below v0.4.0 aren't expected to work.
 
 `pip install animegifs`
 
 # HOW TO USE
```

### Comparing `animegifs-0.5.0/README.md` & `animegifs-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# anime-gifs.py
+# animegifs.py
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
 WIP - updated in time to time. Versions below v0.4.0 aren't expected to work.
 
 `pip install animegifs`
 
 # HOW TO USE
```

### Comparing `animegifs-0.5.0/animegifs/animegifs.py` & `animegifs-0.5.1/animegifs/animegifs.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,13 @@
                 lick.
 
         Returns:
             gif: gif (url) -> str
         """
         if type(category) is int:
             raise errors.CategoryIntegral
-        elif category is None:
-            raise errors.CategoryNone
         elif category.lower() in gifs_dict:
             gif = gifs_dict[category.lower()]
         else:
             raise errors.CategoryError
         return gif
```

### Comparing `animegifs-0.5.0/animegifs/distutils/gifs.py` & `animegifs-0.5.1/animegifs/distutils/gifs.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.0/animegifs.egg-info/PKG-INFO` & `animegifs-0.5.1/animegifs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.0
+Version: 0.5.1
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
-Keywords: anime,gif,python,anime-gif
+Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# anime-gifs.py
+# animegifs.py
 Get random anime gifs by category. Use Python (intended (for now) for Discord).
 
 WIP - updated in time to time. Versions below v0.4.0 aren't expected to work.
 
 `pip install animegifs`
 
 # HOW TO USE
```

### Comparing `animegifs-0.5.0/setup.py` & `animegifs-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.5.0'
+VERSION = '0.5.1'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
@@ -23,12 +23,12 @@
     license='MIT',
     url="https://github.com/MarcoSa-2000/animegifs",
     install_requires=[
        'requests==2.28.2,<=2.29.0'
     ],
     python_requires='>=3.8',
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Microsoft :: Windows"],
-    keywords=['anime', 'gif', 'python', 'anime-gif'],
+    keywords=['anime', 'gif', 'python', 'anime-gif', 'discord'],
 )
```

