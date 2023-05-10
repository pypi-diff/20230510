# Comparing `tmp/8puzz-0.0.0.tar.gz` & `tmp/8puzz-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8puzz-0.0.0.tar", last modified: Wed May 10 17:07:28 2023, max compression
+gzip compressed data, was "8puzz-0.0.1.tar", last modified: Wed May 10 16:59:17 2023, max compression
```

## Comparing `8puzz-0.0.0.tar` & `8puzz-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:07:28.661780 8puzz-0.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-10 17:07:28.654779 8puzz-0.0.0/8puzz.egg-info/
--rw-rw-rw-   0        0        0      479 2023-05-10 17:07:28.000000 8puzz-0.0.0/8puzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      151 2023-05-10 17:07:28.000000 8puzz-0.0.0/8puzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:07:28.000000 8puzz-0.0.0/8puzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-05-10 17:07:28.000000 8puzz-0.0.0/8puzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      479 2023-05-10 17:07:28.659783 8puzz-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 17:07:28.658780 8puzz-0.0.0/ai/
--rw-rw-rw-   0        0        0       27 2023-05-10 16:50:42.000000 8puzz-0.0.0/ai/__init__.py
--rw-rw-rw-   0        0        0     3248 2023-05-10 16:50:07.000000 8puzz-0.0.0/ai/solve.py
--rw-rw-rw-   0        0        0       42 2023-05-10 17:07:28.661780 8puzz-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-05-10 17:07:25.000000 8puzz-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:59:17.400298 8puzz-0.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-10 16:59:17.374295 8puzz-0.0.1/8puzz.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-05-10 16:59:17.000000 8puzz-0.0.1/8puzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2023-05-10 16:59:17.000000 8puzz-0.0.1/8puzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:59:17.000000 8puzz-0.0.1/8puzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-05-10 16:59:17.000000 8puzz-0.0.1/8puzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      479 2023-05-10 16:59:17.398306 8puzz-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 16:59:17.396295 8puzz-0.0.1/ai/
+-rw-rw-rw-   0        0        0       27 2023-05-10 16:50:42.000000 8puzz-0.0.1/ai/__init__.py
+-rw-rw-rw-   0        0        0     3248 2023-05-10 16:50:07.000000 8puzz-0.0.1/ai/solve.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 16:59:17.401298 8puzz-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-05-10 16:35:13.000000 8puzz-0.0.1/setup.py
```

### Comparing `8puzz-0.0.0/ai/solve.py` & `8puzz-0.0.1/ai/solve.py`

 * *Files identical despite different names*

### Comparing `8puzz-0.0.0/setup.py` & `8puzz-0.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-# VERSION = '0'
+VERSION = '0.0.1'
 DESCRIPTION = '8_puzzle_problem'
 LONG_DESCRIPTION = 'A package that allows to print 8 puzzle code.'
 
 # Setting up
 setup(
     name="8puzz",
+    version=VERSION,
     author="yuvraj",
     author_email="yuvrajdevnani03@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
```

