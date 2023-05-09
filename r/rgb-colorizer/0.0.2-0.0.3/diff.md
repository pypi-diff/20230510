# Comparing `tmp/rgb-colorizer-0.0.2.tar.gz` & `tmp/rgb-colorizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgb-colorizer-0.0.2.tar", last modified: Tue May  9 21:51:49 2023, max compression
+gzip compressed data, was "rgb-colorizer-0.0.3.tar", last modified: Tue May  9 21:56:06 2023, max compression
```

## Comparing `rgb-colorizer-0.0.2.tar` & `rgb-colorizer-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 21:51:49.719314 rgb-colorizer-0.0.2/
--rw-rw-rw-   0        0        0     1101 2023-05-09 21:15:09.000000 rgb-colorizer-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      598 2023-05-09 21:51:49.718314 rgb-colorizer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-05-09 21:30:14.000000 rgb-colorizer-0.0.2/README.md
--rw-rw-rw-   0        0        0      573 2023-05-09 21:51:20.000000 rgb-colorizer-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 21:51:49.719314 rgb-colorizer-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 21:51:49.692331 rgb-colorizer-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2023-05-09 21:45:31.000000 rgb-colorizer-0.0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 21:51:49.715324 rgb-colorizer-0.0.2/src/rgb_colorizer.egg-info/
--rw-rw-rw-   0        0        0      598 2023-05-09 21:51:49.000000 rgb-colorizer-0.0.2/src/rgb_colorizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-09 21:51:49.000000 rgb-colorizer-0.0.2/src/rgb_colorizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 21:51:49.000000 rgb-colorizer-0.0.2/src/rgb_colorizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 21:51:49.000000 rgb-colorizer-0.0.2/src/rgb_colorizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 21:56:06.354590 rgb-colorizer-0.0.3/
+-rw-rw-rw-   0        0        0     1101 2023-05-09 21:15:09.000000 rgb-colorizer-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      598 2023-05-09 21:56:06.353591 rgb-colorizer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-05-09 21:30:14.000000 rgb-colorizer-0.0.3/README.md
+-rw-rw-rw-   0        0        0      573 2023-05-09 21:55:35.000000 rgb-colorizer-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 21:56:06.354590 rgb-colorizer-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 21:56:06.307332 rgb-colorizer-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 21:56:06.323324 rgb-colorizer-0.0.3/src/rgb-colorizer/
+-rw-rw-rw-   0        0        0        0 2023-05-09 21:45:31.000000 rgb-colorizer-0.0.3/src/rgb-colorizer/__init__.py
+-rw-rw-rw-   0        0        0     5726 2023-05-09 21:13:48.000000 rgb-colorizer-0.0.3/src/rgb-colorizer/rgb-colorizer.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:56:06.351589 rgb-colorizer-0.0.3/src/rgb_colorizer.egg-info/
+-rw-rw-rw-   0        0        0      598 2023-05-09 21:56:06.000000 rgb-colorizer-0.0.3/src/rgb_colorizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-09 21:56:06.000000 rgb-colorizer-0.0.3/src/rgb_colorizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 21:56:06.000000 rgb-colorizer-0.0.3/src/rgb_colorizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-09 21:56:06.000000 rgb-colorizer-0.0.3/src/rgb_colorizer.egg-info/top_level.txt
```

### Comparing `rgb-colorizer-0.0.2/LICENSE` & `rgb-colorizer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rgb-colorizer-0.0.2/PKG-INFO` & `rgb-colorizer-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgb-colorizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author: Vlad Bilskiy
 Project-URL: Homepage, https://github.com/hittiks/rgb-colorizer
 Project-URL: Bug Tracker, https://github.com/hittiks/rgb-colorizer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rgb-colorizer-0.0.2/pyproject.toml` & `rgb-colorizer-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rgb-colorizer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Vlad Bilskiy"},
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rgb-colorizer-0.0.2/src/rgb_colorizer.egg-info/PKG-INFO` & `rgb-colorizer-0.0.3/src/rgb_colorizer.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgb-colorizer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author: Vlad Bilskiy
 Project-URL: Homepage, https://github.com/hittiks/rgb-colorizer
 Project-URL: Bug Tracker, https://github.com/hittiks/rgb-colorizer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

