# Comparing `tmp/spotipy_anon-1.1.tar.gz` & `tmp/spotipy_anon-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotipy_anon-1.1.tar", last modified: Tue May  9 16:14:18 2023, max compression
+gzip compressed data, was "spotipy_anon-1.2.tar", last modified: Wed May 10 09:53:12 2023, max compression
```

## Comparing `spotipy_anon-1.1.tar` & `spotipy_anon-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 16:14:18.535687 spotipy_anon-1.1/
--rw-rw-rw-   0        0        0     1102 2023-05-09 16:13:32.000000 spotipy_anon-1.1/LICENSE
--rw-rw-rw-   0        0        0     1843 2023-05-09 16:14:18.535687 spotipy_anon-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-05-09 16:13:32.000000 spotipy_anon-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 16:14:18.535687 spotipy_anon-1.1/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-05-09 16:13:32.000000 spotipy_anon-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:14:18.519165 spotipy_anon-1.1/spotipy_anon/
--rw-rw-rw-   0        0        0       56 2023-05-09 16:13:32.000000 spotipy_anon-1.1/spotipy_anon/__init__.py
--rw-rw-rw-   0        0        0     3991 2023-05-09 16:13:32.000000 spotipy_anon-1.1/spotipy_anon/oauth2.py
-drwxrwxrwx   0        0        0        0 2023-05-09 16:14:18.535687 spotipy_anon-1.1/spotipy_anon.egg-info/
--rw-rw-rw-   0        0        0     1843 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-09 16:14:18.000000 spotipy_anon-1.1/spotipy_anon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 09:53:12.447143 spotipy_anon-1.2/
+-rw-rw-rw-   0        0        0     1102 2023-05-10 09:23:29.000000 spotipy_anon-1.2/LICENSE
+-rw-rw-rw-   0        0        0     1843 2023-05-10 09:53:12.447143 spotipy_anon-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2023-05-10 09:23:29.000000 spotipy_anon-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:53:12.447143 spotipy_anon-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      650 2023-05-10 09:50:38.000000 spotipy_anon-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:53:12.447143 spotipy_anon-1.2/spotipy_anon/
+-rw-rw-rw-   0        0        0       56 2023-05-10 09:50:49.000000 spotipy_anon-1.2/spotipy_anon/__init__.py
+-rw-rw-rw-   0        0        0     3991 2023-05-10 09:23:29.000000 spotipy_anon-1.2/spotipy_anon/oauth2.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:53:12.447143 spotipy_anon-1.2/spotipy_anon.egg-info/
+-rw-rw-rw-   0        0        0     1843 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-10 09:53:12.000000 spotipy_anon-1.2/spotipy_anon.egg-info/top_level.txt
```

### Comparing `spotipy_anon-1.1/LICENSE` & `spotipy_anon-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotipy_anon-1.1/PKG-INFO` & `spotipy_anon-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotipy_anon
-Version: 1.1
+Version: 1.2
 Summary: An extension to Spotipy for anonymous access to the Spotify Web API
 Home-page: https://github.com/dieser-niko/spotipy-anon
 Author: @dieserniko
 Author-email: dieserniko@gmx.de
 License: MIT
 Project-URL: Source, https://github.com/dieserniko/spotipy-anon
 Description: # SpotipyAnon
```

### Comparing `spotipy_anon-1.1/README.md` & `spotipy_anon-1.2/README.md`

 * *Files identical despite different names*

### Comparing `spotipy_anon-1.1/setup.py` & `spotipy_anon-1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 
 setup(
     name='spotipy_anon',
-    version='1.1',
+    version='1.2',
     description='An extension to Spotipy for anonymous access to the Spotify Web API',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="@dieserniko",
     author_email="dieserniko@gmx.de",
     url='https://github.com/dieser-niko/spotipy-anon',
     project_urls={
```

### Comparing `spotipy_anon-1.1/spotipy_anon/oauth2.py` & `spotipy_anon-1.2/spotipy_anon/oauth2.py`

 * *Files identical despite different names*

### Comparing `spotipy_anon-1.1/spotipy_anon.egg-info/PKG-INFO` & `spotipy_anon-1.2/spotipy_anon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotipy-anon
-Version: 1.1
+Version: 1.2
 Summary: An extension to Spotipy for anonymous access to the Spotify Web API
 Home-page: https://github.com/dieser-niko/spotipy-anon
 Author: @dieserniko
 Author-email: dieserniko@gmx.de
 License: MIT
 Project-URL: Source, https://github.com/dieserniko/spotipy-anon
 Description: # SpotipyAnon
```

