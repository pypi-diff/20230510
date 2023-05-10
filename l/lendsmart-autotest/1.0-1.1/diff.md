# Comparing `tmp/lendsmart_autotest-1.0.tar.gz` & `tmp/lendsmart_autotest-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_autotest-1.0.tar", last modified: Wed May 10 11:37:36 2023, max compression
+gzip compressed data, was "lendsmart_autotest-1.1.tar", last modified: Wed May 10 12:14:01 2023, max compression
```

## Comparing `lendsmart_autotest-1.0.tar` & `lendsmart_autotest-1.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 11:37:36.332110 lendsmart_autotest-1.0/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 11:37:36.328110 lendsmart_autotest-1.0/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 11:37:36.324110 lendsmart_autotest-1.0/base/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.0/base/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    13128 2023-05-10 10:48:50.000000 lendsmart_autotest-1.0/base/commons.py
--rw-rw-r--   0 user      (1000) user      (1000)     9148 2023-05-10 10:48:50.000000 lendsmart_autotest-1.0/base/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)    13311 2023-05-10 10:48:50.000000 lendsmart_autotest-1.0/base/webActions.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 11:37:36.328110 lendsmart_autotest-1.0/lendsmart_autotest.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 11:37:36.000000 lendsmart_autotest-1.0/lendsmart_autotest.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      372 2023-05-10 11:37:36.000000 lendsmart_autotest-1.0/lendsmart_autotest.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-10 11:37:36.000000 lendsmart_autotest-1.0/lendsmart_autotest.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-10 11:37:36.000000 lendsmart_autotest-1.0/lendsmart_autotest.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       22 2023-05-10 11:37:36.000000 lendsmart_autotest-1.0/lendsmart_autotest.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 11:37:36.328110 lendsmart_autotest-1.0/runner/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.0/runner/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1444 2023-05-10 10:48:50.000000 lendsmart_autotest-1.0/runner/initializer.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-10 11:37:36.332110 lendsmart_autotest-1.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-10 11:36:44.000000 lendsmart_autotest-1.0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 11:37:36.328110 lendsmart_autotest-1.0/utilities/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.0/utilities/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      440 2023-05-10 10:48:50.000000 lendsmart_autotest-1.0/utilities/random_email.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:14:01.774419 lendsmart_autotest-1.1/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 12:14:01.774419 lendsmart_autotest-1.1/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:14:01.774419 lendsmart_autotest-1.1/lendsmart_autotest.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 12:14:01.000000 lendsmart_autotest-1.1/lendsmart_autotest.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      420 2023-05-10 12:14:01.000000 lendsmart_autotest-1.1/lendsmart_autotest.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-10 12:14:01.000000 lendsmart_autotest-1.1/lendsmart_autotest.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-10 12:14:01.000000 lendsmart_autotest-1.1/lendsmart_autotest.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2023-05-10 12:14:01.000000 lendsmart_autotest-1.1/lendsmart_autotest.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:14:01.774419 lendsmart_autotest-1.1/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:14:01.774419 lendsmart_autotest-1.1/lib/base/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/base/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13128 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/base/commons.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9148 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/base/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13311 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/base/webActions.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:14:01.774419 lendsmart_autotest-1.1/lib/runner/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/runner/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1444 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/runner/initializer.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:14:01.774419 lendsmart_autotest-1.1/lib/utilities/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/utilities/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      440 2023-05-10 10:48:50.000000 lendsmart_autotest-1.1/lib/utilities/random_email.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-10 12:14:01.774419 lendsmart_autotest-1.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-10 12:13:31.000000 lendsmart_autotest-1.1/setup.py
```

### Comparing `lendsmart_autotest-1.0/base/commons.py` & `lendsmart_autotest-1.1/lib/base/commons.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.0/base/setup.py` & `lendsmart_autotest-1.1/lib/base/setup.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.0/base/webActions.py` & `lendsmart_autotest-1.1/lib/base/webActions.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.0/runner/initializer.py` & `lendsmart_autotest-1.1/lib/runner/initializer.py`

 * *Files identical despite different names*

### Comparing `lendsmart_autotest-1.0/setup.py` & `lendsmart_autotest-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name="lendsmart_autotest",
-    version="1.0",
+    version="1.1",
     description="The internal SDK for lendsmart autotest",
     url="https://bitbucket.org/lendsmartlabs/lendsmart_py/",
     # Author details
     author="Lendsmart",
     author_email="infos@lendsmart.ai",
     license="MIT",
     classifiers=[
```

