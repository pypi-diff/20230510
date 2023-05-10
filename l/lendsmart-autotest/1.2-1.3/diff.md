# Comparing `tmp/lendsmart_autotest-1.2.tar.gz` & `tmp/lendsmart_autotest-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lendsmart_autotest-1.2.tar", last modified: Wed May 10 12:19:50 2023, max compression
+gzip compressed data, was "lendsmart_autotest-1.3.tar", last modified: Wed May 10 13:16:32 2023, max compression
```

## Comparing `lendsmart_autotest-1.2.tar` & `lendsmart_autotest-1.3.tar`

### file list

```diff
@@ -1,39 +1,10 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.650255 lendsmart_autotest-1.2/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 12:19:50.646255 lendsmart_autotest-1.2/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.634255 lendsmart_autotest-1.2/lendsmart_autotest.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 12:19:50.000000 lendsmart_autotest-1.2/lendsmart_autotest.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      754 2023-05-10 12:19:50.000000 lendsmart_autotest-1.2/lendsmart_autotest.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-10 12:19:50.000000 lendsmart_autotest-1.2/lendsmart_autotest.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-10 12:19:50.000000 lendsmart_autotest-1.2/lendsmart_autotest.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2023-05-10 12:19:50.000000 lendsmart_autotest-1.2/lendsmart_autotest.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.634255 lendsmart_autotest-1.2/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.638255 lendsmart_autotest-1.2/lib/base/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/base/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    13128 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/base/commons.py
--rw-rw-r--   0 user      (1000) user      (1000)     9148 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/base/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)    13311 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/base/webActions.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.638255 lendsmart_autotest-1.2/lib/client_builder/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:18:05.000000 lendsmart_autotest-1.2/lib/client_builder/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.638255 lendsmart_autotest-1.2/lib/configurations/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:17:57.000000 lendsmart_autotest-1.2/lib/configurations/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6714 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/configurations/common_config.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.642255 lendsmart_autotest-1.2/lib/generator/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:17:35.000000 lendsmart_autotest-1.2/lib/generator/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2595 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/generator/generate_test_data.py
--rw-rw-r--   0 user      (1000) user      (1000)    10788 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/generator/graph.py
--rw-rw-r--   0 user      (1000) user      (1000)     9425 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/generator/initialize.py
--rw-rw-r--   0 user      (1000) user      (1000)    13581 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/generator/question_type.py
--rw-rw-r--   0 user      (1000) user      (1000)     4274 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/generator/test_data.py
--rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/generator/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.646255 lendsmart_autotest-1.2/lib/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 12:17:47.000000 lendsmart_autotest-1.2/lib/lib/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      162 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/lib/lend_event.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.646255 lendsmart_autotest-1.2/lib/runner/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/runner/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1444 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/runner/initializer.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 12:19:50.646255 lendsmart_autotest-1.2/lib/utilities/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/utilities/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      440 2023-05-10 10:48:50.000000 lendsmart_autotest-1.2/lib/utilities/random_email.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-10 12:19:50.650255 lendsmart_autotest-1.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-10 12:19:11.000000 lendsmart_autotest-1.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:16:32.596703 lendsmart_autotest-1.3/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 13:16:32.596703 lendsmart_autotest-1.3/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-10 13:16:32.596703 lendsmart_autotest-1.3/lendsmart_autotest.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      414 2023-05-10 13:16:32.000000 lendsmart_autotest-1.3/lendsmart_autotest.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-10 13:16:32.000000 lendsmart_autotest-1.3/lendsmart_autotest.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-10 13:16:32.000000 lendsmart_autotest-1.3/lendsmart_autotest.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      200 2023-05-10 13:16:32.000000 lendsmart_autotest-1.3/lendsmart_autotest.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-10 13:16:32.000000 lendsmart_autotest-1.3/lendsmart_autotest.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-10 13:16:32.596703 lendsmart_autotest-1.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1193 2023-05-10 13:16:03.000000 lendsmart_autotest-1.3/setup.py
```

### Comparing `lendsmart_autotest-1.2/setup.py` & `lendsmart_autotest-1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
 setup(
     name="lendsmart_autotest",
-    version="1.2",
+    version="1.3",
     description="The internal SDK for lendsmart autotest",
     url="https://bitbucket.org/lendsmartlabs/lendsmart_py/",
     # Author details
     author="Lendsmart",
     author_email="infos@lendsmart.ai",
     license="MIT",
     classifiers=[
```

