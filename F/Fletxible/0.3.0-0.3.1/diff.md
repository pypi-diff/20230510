# Comparing `tmp/Fletxible-0.3.0.tar.gz` & `tmp/Fletxible-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fletxible-0.3.0.tar", last modified: Mon May  1 14:50:38 2023, max compression
+gzip compressed data, was "Fletxible-0.3.1.tar", last modified: Wed May 10 13:03:13 2023, max compression
```

## Comparing `Fletxible-0.3.0.tar` & `Fletxible-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-01 14:50:38.991235 Fletxible-0.3.0/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-01 14:50:38.988875 Fletxible-0.3.0/Fletxible.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-01 14:50:38.000000 Fletxible-0.3.0/Fletxible.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)      326 2023-05-01 14:50:38.000000 Fletxible-0.3.0/Fletxible.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-01 14:50:38.000000 Fletxible-0.3.0/Fletxible.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-01 14:50:38.000000 Fletxible-0.3.0/Fletxible.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       53 2023-05-01 14:50:38.000000 Fletxible-0.3.0/Fletxible.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-01 14:50:38.000000 Fletxible-0.3.0/Fletxible.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.3.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-01 14:50:38.991031 Fletxible-0.3.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     3282 2023-05-01 14:48:32.000000 Fletxible-0.3.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-01 14:50:38.990315 Fletxible-0.3.0/logic/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.3.0/logic/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1288 2023-05-01 13:50:27.000000 Fletxible-0.3.0/logic/cli.py
--rw-r--r--   0 ahmad      (501) staff       (20)      164 2023-05-01 12:45:39.000000 Fletxible-0.3.0/logic/main.py
--rw-r--r--   0 ahmad      (501) staff       (20)     6566 2023-05-01 12:53:10.000000 Fletxible-0.3.0/logic/script.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1860 2023-05-01 13:04:12.000000 Fletxible-0.3.0/logic/utilities.py
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-01 14:50:38.991300 Fletxible-0.3.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)     1130 2023-05-01 14:49:54.000000 Fletxible-0.3.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-01 14:50:38.990640 Fletxible-0.3.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.3.0/tests/test_route.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-10 13:03:13.807184 Fletxible-0.3.1/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-10 13:03:13.803251 Fletxible-0.3.1/Fletxible.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-10 13:03:13.000000 Fletxible-0.3.1/Fletxible.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)      357 2023-05-10 13:03:13.000000 Fletxible-0.3.1/Fletxible.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-10 13:03:13.000000 Fletxible-0.3.1/Fletxible.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       50 2023-05-10 13:03:13.000000 Fletxible-0.3.1/Fletxible.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       53 2023-05-10 13:03:13.000000 Fletxible-0.3.1/Fletxible.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        6 2023-05-10 13:03:13.000000 Fletxible-0.3.1/Fletxible.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-29 15:25:05.000000 Fletxible-0.3.1/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      830 2023-05-10 13:03:13.806912 Fletxible-0.3.1/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4106 2023-05-01 16:06:19.000000 Fletxible-0.3.1/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-10 13:03:13.805901 Fletxible-0.3.1/logic/
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-05-01 13:39:08.000000 Fletxible-0.3.1/logic/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1288 2023-05-01 13:50:27.000000 Fletxible-0.3.1/logic/cli.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      164 2023-05-02 14:50:14.000000 Fletxible-0.3.1/logic/main.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      243 2023-05-02 14:50:26.000000 Fletxible-0.3.1/logic/mapped.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      343 2023-05-02 14:50:26.000000 Fletxible-0.3.1/logic/route.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     6566 2023-05-02 11:51:56.000000 Fletxible-0.3.1/logic/script.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1860 2023-05-01 13:04:12.000000 Fletxible-0.3.1/logic/utilities.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-10 13:03:13.807267 Fletxible-0.3.1/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)     1130 2023-05-10 13:02:35.000000 Fletxible-0.3.1/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-10 13:03:13.806359 Fletxible-0.3.1/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)        5 2023-05-01 14:25:50.000000 Fletxible-0.3.1/tests/test_route.py
```

### Comparing `Fletxible-0.3.0/Fletxible.egg-info/PKG-INFO` & `Fletxible-0.3.1/Fletxible.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.3.0
+Version: 0.3.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.3.0/LICENSE` & `Fletxible-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Fletxible-0.3.0/PKG-INFO` & `Fletxible-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fletxible
-Version: 0.3.0
+Version: 0.3.1
 Summary: Web Boilerplate for Flet Library
 Home-page: https://github.com/LineIndent/fletxible
 Author: S. Ahmad P. Hakimi
 Author-email: pourhakimi@pm.me
 Keywords: python web template,web application,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Fletxible-0.3.0/logic/cli.py` & `Fletxible-0.3.1/logic/cli.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.3.0/logic/script.py` & `Fletxible-0.3.1/logic/script.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.3.0/logic/utilities.py` & `Fletxible-0.3.1/logic/utilities.py`

 * *Files identical despite different names*

### Comparing `Fletxible-0.3.0/setup.py` & `Fletxible-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
     name="Fletxible",
-    version="0.3.0",
+    version="0.3.1",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Web Boilerplate for Flet Library",
     long_description="Fletxible is a Python web boilerplate project designed to provide a solid foundation for building web applications with Python and Flet. The project comes pre-configured with a range of tools and features to make it easy for developers to get started building their applications, without the need to spend time setting up infrastructure or configuring tools.",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/fletxible",
     packages=["logic"],
-    install_requires=["click==8.1.3", "flet==0.6.2", " pickle5==0.0.11", "PyYAML==6.0"],
+    install_requires=["click==8.1.3", "flet==0.6.2", " pickle5==0.0.12", "PyYAML==6.0"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": ["fletxible-init=logic.cli:init"],
```

