# Comparing `tmp/jetha_ai-0.tar.gz` & `tmp/jetha_ai-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetha_ai-0.tar", last modified: Wed May 10 17:25:43 2023, max compression
+gzip compressed data, was "jetha_ai-1.tar", last modified: Wed May 10 17:29:12 2023, max compression
```

## Comparing `jetha_ai-0.tar` & `jetha_ai-1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:43.661470 jetha_ai-0/
--rw-rw-rw-   0        0        0      467 2023-05-10 17:25:43.660471 jetha_ai-0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:43.641472 jetha_ai-0/ai/
--rw-rw-rw-   0        0        0       27 2023-05-10 16:50:42.000000 jetha_ai-0/ai/__init__.py
--rw-rw-rw-   0        0        0     6689 2023-05-10 17:13:26.000000 jetha_ai-0/ai/solve.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:43.658470 jetha_ai-0/jetha_ai.egg-info/
--rw-rw-rw-   0        0        0      467 2023-05-10 17:25:43.000000 jetha_ai-0/jetha_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-10 17:25:43.000000 jetha_ai-0/jetha_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:25:43.000000 jetha_ai-0/jetha_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-05-10 17:25:43.000000 jetha_ai-0/jetha_ai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 17:25:43.662471 jetha_ai-0/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-05-10 17:22:51.000000 jetha_ai-0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:29:12.699323 jetha_ai-1/
+-rw-rw-rw-   0        0        0      467 2023-05-10 17:29:12.698325 jetha_ai-1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 17:29:12.685320 jetha_ai-1/ai/
+-rw-rw-rw-   0        0        0       27 2023-05-10 17:28:29.000000 jetha_ai-1/ai/__init__.py
+-rw-rw-rw-   0        0        0     3250 2023-05-10 17:28:52.000000 jetha_ai-1/ai/solve.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:29:12.697322 jetha_ai-1/jetha_ai.egg-info/
+-rw-rw-rw-   0        0        0      467 2023-05-10 17:29:12.000000 jetha_ai-1/jetha_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-10 17:29:12.000000 jetha_ai-1/jetha_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 17:29:12.000000 jetha_ai-1/jetha_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-05-10 17:29:12.000000 jetha_ai-1/jetha_ai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 17:29:12.700324 jetha_ai-1/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-05-10 17:29:10.000000 jetha_ai-1/setup.py
```

### Comparing `jetha_ai-0/setup.py` & `jetha_ai-1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0'
+VERSION = '1'
 DESCRIPTION = 'all solutions'
 LONG_DESCRIPTION = 'A package that allows to print all codes of ai lab.'
 
 # Setting up
 setup(
     name="jetha_ai",
     version=VERSION,
```

