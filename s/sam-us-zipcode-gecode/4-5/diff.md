# Comparing `tmp/sam_us_zipcode_gecode-4.tar.gz` & `tmp/sam_us_zipcode_gecode-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_us_zipcode_gecode-4.tar", last modified: Wed May 10 01:28:34 2023, max compression
+gzip compressed data, was "sam_us_zipcode_gecode-5.tar", last modified: Wed May 10 01:35:31 2023, max compression
```

## Comparing `sam_us_zipcode_gecode-4.tar` & `sam_us_zipcode_gecode-5.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 01:28:34.760300 sam_us_zipcode_gecode-4/
--rw-rw-rw-   0        0        0     1047 2023-05-10 01:28:34.759298 sam_us_zipcode_gecode-4/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-10 01:23:20.000000 sam_us_zipcode_gecode-4/README.md
--rw-rw-rw-   0        0        0     1369 2023-05-10 01:20:44.000000 sam_us_zipcode_gecode-4/cacheHandler.py
-drwxrwxrwx   0        0        0        0 2023-05-10 01:28:34.758299 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/
--rw-rw-rw-   0        0        0     1047 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 01:28:34.760300 sam_us_zipcode_gecode-4/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-05-10 01:28:29.000000 sam_us_zipcode_gecode-4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:35:31.832871 sam_us_zipcode_gecode-5/
+-rw-rw-rw-   0        0        0     1047 2023-05-10 01:35:31.831874 sam_us_zipcode_gecode-5/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-10 01:23:20.000000 sam_us_zipcode_gecode-5/README.md
+-rw-rw-rw-   0        0        0     1369 2023-05-10 01:20:44.000000 sam_us_zipcode_gecode-5/cacheHandler.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:35:31.830868 sam_us_zipcode_gecode-5/sam_us_zipcode_gecode.egg-info/
+-rw-rw-rw-   0        0        0     1047 2023-05-10 01:35:31.000000 sam_us_zipcode_gecode-5/sam_us_zipcode_gecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-10 01:35:31.000000 sam_us_zipcode_gecode-5/sam_us_zipcode_gecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:35:31.000000 sam_us_zipcode_gecode-5/sam_us_zipcode_gecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-10 01:35:31.000000 sam_us_zipcode_gecode-5/sam_us_zipcode_gecode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 01:35:31.832871 sam_us_zipcode_gecode-5/setup.cfg
+-rw-rw-rw-   0        0        0      480 2023-05-10 01:35:10.000000 sam_us_zipcode_gecode-5/setup.py
```

### Comparing `sam_us_zipcode_gecode-4/PKG-INFO` & `sam_us_zipcode_gecode-5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam_us_zipcode_gecode
-Version: 4
+Version: 5
 Summary: A Python package for converting US zip codes to latitude and longitude
 Author: Sam Mathew
 Author-email: sammathew000@gmail.com
 Description-Content-Type: text/markdown
 
 # sam-us-zipcode-gecode
```

### Comparing `sam_us_zipcode_gecode-4/README.md` & `sam_us_zipcode_gecode-5/README.md`

 * *Files identical despite different names*

### Comparing `sam_us_zipcode_gecode-4/cacheHandler.py` & `sam_us_zipcode_gecode-5/cacheHandler.py`

 * *Files identical despite different names*

### Comparing `sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/PKG-INFO` & `sam_us_zipcode_gecode-5/sam_us_zipcode_gecode.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam-us-zipcode-gecode
-Version: 4
+Version: 5
 Summary: A Python package for converting US zip codes to latitude and longitude
 Author: Sam Mathew
 Author-email: sammathew000@gmail.com
 Description-Content-Type: text/markdown
 
 # sam-us-zipcode-gecode
```

