# Comparing `tmp/codeoffer-0.2.0.tar.gz` & `tmp/codeoffer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codeoffer-0.2.0.tar", last modified: Wed May 10 10:38:46 2023, max compression
+gzip compressed data, was "dist/codeoffer-0.4.0.tar", last modified: Wed May 10 10:45:00 2023, max compression
```

## Comparing `codeoffer-0.2.0.tar` & `codeoffer-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 maximilianosinski   (501) staff       (20)        0 2023-05-10 10:38:46.000000 codeoffer-0.2.0/
--rw-r--r--   0 maximilianosinski   (501) staff       (20)      439 2023-05-10 10:38:46.000000 codeoffer-0.2.0/PKG-INFO
--rw-r--r--   0 maximilianosinski   (501) staff       (20)     2394 2023-05-10 10:38:10.000000 codeoffer-0.2.0/README.md
-drwxr-xr-x   0 maximilianosinski   (501) staff       (20)        0 2023-05-10 10:38:46.000000 codeoffer-0.2.0/codeoffer.egg-info/
--rw-r--r--   0 maximilianosinski   (501) staff       (20)      439 2023-05-10 10:38:45.000000 codeoffer-0.2.0/codeoffer.egg-info/PKG-INFO
--rw-r--r--   0 maximilianosinski   (501) staff       (20)      150 2023-05-10 10:38:45.000000 codeoffer-0.2.0/codeoffer.egg-info/SOURCES.txt
--rw-r--r--   0 maximilianosinski   (501) staff       (20)        1 2023-05-10 10:38:45.000000 codeoffer-0.2.0/codeoffer.egg-info/dependency_links.txt
--rw-r--r--   0 maximilianosinski   (501) staff       (20)        1 2023-05-10 10:38:45.000000 codeoffer-0.2.0/codeoffer.egg-info/top_level.txt
--rw-r--r--   0 maximilianosinski   (501) staff       (20)       38 2023-05-10 10:38:46.000000 codeoffer-0.2.0/setup.cfg
--rw-r--r--   0 maximilianosinski   (501) staff       (20)      519 2023-05-10 10:38:32.000000 codeoffer-0.2.0/setup.py
+drwxr-xr-x   0 maximilianosinski   (501) staff       (20)        0 2023-05-10 10:45:00.000000 codeoffer-0.4.0/
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)       17 2023-05-10 10:44:55.000000 codeoffer-0.4.0/MANIFEST.in
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)      439 2023-05-10 10:45:00.000000 codeoffer-0.4.0/PKG-INFO
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)     2394 2023-05-10 10:38:10.000000 codeoffer-0.4.0/README.md
+drwxr-xr-x   0 maximilianosinski   (501) staff       (20)        0 2023-05-10 10:45:00.000000 codeoffer-0.4.0/codeoffer.egg-info/
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)      439 2023-05-10 10:45:00.000000 codeoffer-0.4.0/codeoffer.egg-info/PKG-INFO
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)      162 2023-05-10 10:45:00.000000 codeoffer-0.4.0/codeoffer.egg-info/SOURCES.txt
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)        1 2023-05-10 10:45:00.000000 codeoffer-0.4.0/codeoffer.egg-info/dependency_links.txt
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)        1 2023-05-10 10:45:00.000000 codeoffer-0.4.0/codeoffer.egg-info/top_level.txt
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)       38 2023-05-10 10:45:00.000000 codeoffer-0.4.0/setup.cfg
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)      519 2023-05-10 10:44:37.000000 codeoffer-0.4.0/setup.py
```

### Comparing `codeoffer-0.2.0/README.md` & `codeoffer-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `codeoffer-0.2.0/setup.py` & `codeoffer-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='codeoffer',
-    version='0.2.0',
+    version='0.4.0',
     description='Python library that simplifies access to the Public CodeOffer API',
     author='CodeOffer',
     author_email='contact@codeoffer.net',
     packages=find_packages(),
     url='https://github.com/codeoffer/v1-python-library',
     project_urls={
         'Documentation': 'https://github.com/codeoffer/v1-python-library',
```

