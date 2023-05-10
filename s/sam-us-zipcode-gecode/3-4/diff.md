# Comparing `tmp/sam_us_zipcode_gecode-3.tar.gz` & `tmp/sam_us_zipcode_gecode-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_us_zipcode_gecode-3.tar", last modified: Wed May 10 01:27:31 2023, max compression
+gzip compressed data, was "sam_us_zipcode_gecode-4.tar", last modified: Wed May 10 01:28:34 2023, max compression
```

## Comparing `sam_us_zipcode_gecode-3.tar` & `sam_us_zipcode_gecode-4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 01:27:31.218478 sam_us_zipcode_gecode-3/
--rw-rw-rw-   0        0        0      318 2023-05-10 01:27:31.218478 sam_us_zipcode_gecode-3/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-10 01:23:20.000000 sam_us_zipcode_gecode-3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 01:27:31.216472 sam_us_zipcode_gecode-3/sam_us_zipcode_gecode.egg-info/
--rw-rw-rw-   0        0        0      318 2023-05-10 01:27:31.000000 sam_us_zipcode_gecode-3/sam_us_zipcode_gecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-10 01:27:31.000000 sam_us_zipcode_gecode-3/sam_us_zipcode_gecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 01:27:31.000000 sam_us_zipcode_gecode-3/sam_us_zipcode_gecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-10 01:27:31.000000 sam_us_zipcode_gecode-3/sam_us_zipcode_gecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-10 01:27:31.000000 sam_us_zipcode_gecode-3/sam_us_zipcode_gecode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 01:27:31.218478 sam_us_zipcode_gecode-3/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-05-10 01:26:42.000000 sam_us_zipcode_gecode-3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:28:34.760300 sam_us_zipcode_gecode-4/
+-rw-rw-rw-   0        0        0     1047 2023-05-10 01:28:34.759298 sam_us_zipcode_gecode-4/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-10 01:23:20.000000 sam_us_zipcode_gecode-4/README.md
+-rw-rw-rw-   0        0        0     1369 2023-05-10 01:20:44.000000 sam_us_zipcode_gecode-4/cacheHandler.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:28:34.758299 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/
+-rw-rw-rw-   0        0        0     1047 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-10 01:28:34.000000 sam_us_zipcode_gecode-4/sam_us_zipcode_gecode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 01:28:34.760300 sam_us_zipcode_gecode-4/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-05-10 01:28:29.000000 sam_us_zipcode_gecode-4/setup.py
```

### Comparing `sam_us_zipcode_gecode-3/README.md` & `sam_us_zipcode_gecode-4/README.md`

 * *Files identical despite different names*

