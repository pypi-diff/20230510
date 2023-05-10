# Comparing `tmp/geocodeus-8.0.tar.gz` & `tmp/geocodeus-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocodeus-8.0.tar", last modified: Wed May 10 01:52:12 2023, max compression
+gzip compressed data, was "geocodeus-9.0.tar", last modified: Wed May 10 01:56:31 2023, max compression
```

## Comparing `geocodeus-8.0.tar` & `geocodeus-9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 01:52:12.275148 geocodeus-8.0/
--rw-rw-rw-   0        0        0     1037 2023-05-10 01:52:12.274150 geocodeus-8.0/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-10 01:23:20.000000 geocodeus-8.0/README.md
--rw-rw-rw-   0        0        0     1365 2023-05-10 01:50:53.000000 geocodeus-8.0/cacheHandler.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:52:12.273151 geocodeus-8.0/geocodeus.egg-info/
--rw-rw-rw-   0        0        0     1037 2023-05-10 01:52:12.000000 geocodeus-8.0/geocodeus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-05-10 01:52:12.000000 geocodeus-8.0/geocodeus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 01:52:12.000000 geocodeus-8.0/geocodeus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-10 01:52:12.000000 geocodeus-8.0/geocodeus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 01:52:12.275148 geocodeus-8.0/setup.cfg
--rw-rw-rw-   0        0        0      470 2023-05-10 01:52:07.000000 geocodeus-8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:56:31.232646 geocodeus-9.0/
+-rw-rw-rw-   0        0        0     1037 2023-05-10 01:56:31.231644 geocodeus-9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-10 01:23:20.000000 geocodeus-9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 01:56:31.230642 geocodeus-9.0/geocodeus.egg-info/
+-rw-rw-rw-   0        0        0     1037 2023-05-10 01:56:31.000000 geocodeus-9.0/geocodeus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-10 01:56:31.000000 geocodeus-9.0/geocodeus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:56:31.000000 geocodeus-9.0/geocodeus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 01:56:31.000000 geocodeus-9.0/geocodeus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1365 2023-05-10 01:50:53.000000 geocodeus-9.0/geocodeus.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 01:56:31.232646 geocodeus-9.0/setup.cfg
+-rw-rw-rw-   0        0        0      470 2023-05-10 01:56:27.000000 geocodeus-9.0/setup.py
```

### Comparing `geocodeus-8.0/PKG-INFO` & `geocodeus-9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocodeus
-Version: 8.0
+Version: 9.0
 Summary: A Python package for converting US zip codes to latitude and longitude
 Author: Sam Mathew
 Author-email: sammathew000@gmail.com
 Description-Content-Type: text/markdown
 
 # sam-us-zipcode-gecode
```

### Comparing `geocodeus-8.0/README.md` & `geocodeus-9.0/README.md`

 * *Files identical despite different names*

### Comparing `geocodeus-8.0/cacheHandler.py` & `geocodeus-9.0/geocodeus.py`

 * *Files identical despite different names*

### Comparing `geocodeus-8.0/geocodeus.egg-info/PKG-INFO` & `geocodeus-9.0/geocodeus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocodeus
-Version: 8.0
+Version: 9.0
 Summary: A Python package for converting US zip codes to latitude and longitude
 Author: Sam Mathew
 Author-email: sammathew000@gmail.com
 Description-Content-Type: text/markdown
 
 # sam-us-zipcode-gecode
```

