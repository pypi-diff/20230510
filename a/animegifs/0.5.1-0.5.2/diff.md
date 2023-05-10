# Comparing `tmp/animegifs-0.5.1.tar.gz` & `tmp/animegifs-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animegifs-0.5.1.tar", last modified: Wed May 10 01:38:38 2023, max compression
+gzip compressed data, was "animegifs-0.5.2.tar", last modified: Wed May 10 14:34:39 2023, max compression
```

## Comparing `animegifs-0.5.1.tar` & `animegifs-0.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 01:38:38.572296 animegifs-0.5.1/
--rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     1193 2023-05-10 01:38:38.571296 animegifs-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      601 2023-05-10 01:34:05.000000 animegifs-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 01:38:38.555295 animegifs-0.5.1/animegifs/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.1/animegifs/__init__.py
--rw-rw-rw-   0        0        0     2262 2023-05-10 01:38:16.000000 animegifs-0.5.1/animegifs/animegifs.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:38:38.569296 animegifs-0.5.1/animegifs/distutils/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.1/animegifs/distutils/__init__.py
--rw-rw-rw-   0        0        0      201 2023-05-10 01:38:16.000000 animegifs-0.5.1/animegifs/distutils/errors.py
--rw-rw-rw-   0        0        0     1313 2023-04-28 20:51:38.000000 animegifs-0.5.1/animegifs/distutils/gifs.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:38:38.564304 animegifs-0.5.1/animegifs.egg-info/
--rw-rw-rw-   0        0        0     1193 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 01:38:38.000000 animegifs-0.5.1/animegifs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 01:38:38.572296 animegifs-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-05-10 01:35:19.000000 animegifs-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:34:39.921667 animegifs-0.5.2/
+-rw-rw-rw-   0        0        0     1086 2022-05-19 16:45:41.000000 animegifs-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0     1193 2023-05-10 14:34:39.920668 animegifs-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2023-05-10 01:34:05.000000 animegifs-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 14:34:39.903665 animegifs-0.5.2/animegifs/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:36.000000 animegifs-0.5.2/animegifs/__init__.py
+-rw-rw-rw-   0        0        0     2383 2023-05-10 14:08:03.000000 animegifs-0.5.2/animegifs/animegifs.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:34:39.918669 animegifs-0.5.2/animegifs/distutils/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:54:59.000000 animegifs-0.5.2/animegifs/distutils/__init__.py
+-rw-rw-rw-   0        0        0     1186 2023-05-10 14:18:41.000000 animegifs-0.5.2/animegifs/distutils/errors.py
+-rw-rw-rw-   0        0        0     1313 2023-04-28 20:51:38.000000 animegifs-0.5.2/animegifs/distutils/gifs.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:34:39.913668 animegifs-0.5.2/animegifs.egg-info/
+-rw-rw-rw-   0        0        0     1193 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 14:34:39.000000 animegifs-0.5.2/animegifs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 14:34:39.921667 animegifs-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-05-10 14:33:56.000000 animegifs-0.5.2/setup.py
```

### Comparing `animegifs-0.5.1/LICENSE` & `animegifs-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.1/PKG-INFO` & `animegifs-0.5.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.1
+Version: 0.5.2
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
```

### Comparing `animegifs-0.5.1/README.md` & `animegifs-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.1/animegifs/animegifs.py` & `animegifs-0.5.2/animegifs/animegifs.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,16 @@
                 handhold, happy, harass, highfive, hug, icecream, insult, kill, kiss,
                 lick.
 
         Returns:
             gif: gif (url) -> str
         """
         if type(category) is int:
-            raise errors.CategoryIntegral
+            raise errors.CategoryIntegral(category)
         elif category.lower() in gifs_dict:
             gif = gifs_dict[category.lower()]
+        elif category.lower() not in gifs_dict:
+            raise errors.CategoryError(category)
         else:
-            raise errors.CategoryError
+            raise errors.CategoryUnknown(category)
         return gif
```

### Comparing `animegifs-0.5.1/animegifs/distutils/gifs.py` & `animegifs-0.5.2/animegifs/distutils/gifs.py`

 * *Files identical despite different names*

### Comparing `animegifs-0.5.1/animegifs.egg-info/PKG-INFO` & `animegifs-0.5.2/animegifs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animegifs
-Version: 0.5.1
+Version: 0.5.2
 Summary: Get random anime gifs by category.
 Home-page: https://github.com/MarcoSa-2000/animegifs
 Author: Marco-Sa2000
 Author-email: grest0grest@gmail.com
 License: MIT
 Keywords: anime,gif,python,anime-gif,discord
 Platform: UNKNOWN
```

### Comparing `animegifs-0.5.1/setup.py` & `animegifs-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 LONG_DESCRIPTION = long_description
-VERSION = '0.5.1'
+VERSION = '0.5.2'
 
 setup(
     name='animegifs',
     package_dir={"anime_gifs": "animegifs"},
     packages=["animegifs", "animegifs.distutils"],
     version=VERSION,
     description='Get random anime gifs by category.',
```

