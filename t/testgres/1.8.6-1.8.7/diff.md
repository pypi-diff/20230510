# Comparing `tmp/testgres-1.8.6.tar.gz` & `tmp/testgres-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgres-1.8.6.tar", last modified: Fri May  5 11:15:28 2023, max compression
+gzip compressed data, was "testgres-1.8.7.tar", last modified: Wed May 10 12:05:11 2023, max compression
```

## Comparing `testgres-1.8.6.tar` & `testgres-1.8.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:15:27.997087 testgres-1.8.6/
--rw-rw-r--   0 root         (0) root         (0)     1106 2022-02-22 09:57:57.000000 testgres-1.8.6/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      136 2022-02-22 09:57:57.000000 testgres-1.8.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5753 2023-05-05 11:15:27.997087 testgres-1.8.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5399 2023-05-05 04:23:08.000000 testgres-1.8.6/README.md
--rw-rw-r--   0 root         (0) root         (0)      160 2023-05-05 11:15:28.001087 testgres-1.8.6/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      975 2023-05-05 04:23:08.000000 testgres-1.8.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:15:27.997087 testgres-1.8.6/testgres/
--rw-rw-r--   0 root         (0) root         (0)     1519 2023-05-05 04:23:08.000000 testgres-1.8.6/testgres/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1524 2022-02-22 09:57:57.000000 testgres-1.8.6/testgres/api.py
--rw-rw-r--   0 root         (0) root         (0)     5187 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/backup.py
--rw-rw-r--   0 root         (0) root         (0)     2195 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/cache.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/config.py
--rw-rw-r--   0 root         (0) root         (0)     3080 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/connection.py
--rw-rw-r--   0 root         (0) root         (0)      819 2022-02-22 09:57:57.000000 testgres-1.8.6/testgres/consts.py
--rw-rw-r--   0 root         (0) root         (0)     1749 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/decorators.py
--rw-rw-r--   0 root         (0) root         (0)      932 2022-02-22 09:57:57.000000 testgres-1.8.6/testgres/defaults.py
--rw-rw-r--   0 root         (0) root         (0)     2451 2023-05-05 04:23:08.000000 testgres-1.8.6/testgres/enums.py
--rw-rw-r--   0 root         (0) root         (0)     1988 2022-02-22 09:57:57.000000 testgres-1.8.6/testgres/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     1428 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/logger.py
--rw-rw-r--   0 root         (0) root         (0)    51631 2023-05-05 10:42:56.000000 testgres-1.8.6/testgres/node.py
--rw-rw-r--   0 root         (0) root         (0)     8225 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/pubsub.py
--rw-rw-r--   0 root         (0) root         (0)     1547 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/standby.py
--rw-rw-r--   0 root         (0) root         (0)     6283 2022-11-09 15:43:39.000000 testgres-1.8.6/testgres/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:15:27.997087 testgres-1.8.6/testgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5753 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:15:27.997087 testgres-1.8.6/tests/
--rwxrwxr-x   0 root         (0) root         (0)    34618 2023-05-05 04:23:08.000000 testgres-1.8.6/tests/test_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:05:11.636103 testgres-1.8.7/
+-rw-rw-r--   0 root         (0) root         (0)     1106 2023-05-10 11:22:06.000000 testgres-1.8.7/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-02-22 09:57:57.000000 testgres-1.8.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5753 2023-05-10 12:05:11.636103 testgres-1.8.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5399 2023-05-05 04:23:08.000000 testgres-1.8.7/README.md
+-rw-rw-r--   0 root         (0) root         (0)      160 2023-05-10 12:05:11.636103 testgres-1.8.7/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1011 2023-05-10 11:40:41.000000 testgres-1.8.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:05:11.632103 testgres-1.8.7/testgres/
+-rw-rw-r--   0 root         (0) root         (0)     1519 2023-05-05 04:23:08.000000 testgres-1.8.7/testgres/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1524 2022-02-22 09:57:57.000000 testgres-1.8.7/testgres/api.py
+-rw-rw-r--   0 root         (0) root         (0)     5187 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/backup.py
+-rw-rw-r--   0 root         (0) root         (0)     2195 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/cache.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/config.py
+-rw-rw-r--   0 root         (0) root         (0)     3080 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/connection.py
+-rw-rw-r--   0 root         (0) root         (0)      819 2022-02-22 09:57:57.000000 testgres-1.8.7/testgres/consts.py
+-rw-rw-r--   0 root         (0) root         (0)     1749 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/decorators.py
+-rw-rw-r--   0 root         (0) root         (0)      932 2022-02-22 09:57:57.000000 testgres-1.8.7/testgres/defaults.py
+-rw-rw-r--   0 root         (0) root         (0)     2451 2023-05-05 04:23:08.000000 testgres-1.8.7/testgres/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     1988 2022-02-22 09:57:57.000000 testgres-1.8.7/testgres/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1428 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/logger.py
+-rw-rw-r--   0 root         (0) root         (0)    51631 2023-05-05 10:42:56.000000 testgres-1.8.7/testgres/node.py
+-rw-rw-r--   0 root         (0) root         (0)     8225 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/pubsub.py
+-rw-rw-r--   0 root         (0) root         (0)     1547 2022-05-06 11:01:56.000000 testgres-1.8.7/testgres/standby.py
+-rw-rw-r--   0 root         (0) root         (0)     6283 2022-11-09 15:43:39.000000 testgres-1.8.7/testgres/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:05:11.636103 testgres-1.8.7/testgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5753 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-10 12:05:11.000000 testgres-1.8.7/testgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:05:11.636103 testgres-1.8.7/tests/
+-rwxrwxr-x   0 root         (0) root         (0)    34618 2023-05-05 04:23:08.000000 testgres-1.8.7/tests/test_simple.py
```

### Comparing `testgres-1.8.6/LICENSE` & `testgres-1.8.7/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 testgres is released under the PostgreSQL License, a liberal Open Source license, similar to the BSD or MIT licenses.
 
-Copyright (c) 2016-2018, Postgres Professional
+Copyright (c) 2016-2023, Postgres Professional
 
 Permission to use, copy, modify, and distribute this software and its documentation for any purpose, without fee, and without a written agreement is hereby granted, provided that the above copyright notice and this paragraph and the following two paragraphs appear in all copies.
 
 IN NO EVENT SHALL POSTGRES PROFESSIONAL BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF POSTGRES PROFESSIONAL HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 POSTGRES PROFESSIONAL SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON AN "AS IS" BASIS, AND POSTGRES PROFESSIONAL HAS NO OBLIGATIONS TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
```

### Comparing `testgres-1.8.6/PKG-INFO` & `testgres-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testgres
-Version: 1.8.6
+Version: 1.8.7
 Summary: Testing utility for PostgreSQL and its extensions
 Home-page: https://github.com/postgrespro/testgres
 Author: Ildar Musin
 Author-email: zildermann@gmail.com
 License: PostgreSQL
 Keywords: test,testing,postgresql
 Platform: UNKNOWN
```

### Comparing `testgres-1.8.6/README.md` & `testgres-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/setup.py` & `testgres-1.8.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,36 @@
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 # Basic dependencies
-install_requires = ["pg8000", "port-for>=0.4", "six>=1.9.0", "psutil"]
+install_requires = [
+    "pg8000",
+    "port-for>=0.4",
+    "six>=1.9.0",
+    "psutil",
+    "packaging",
+]
 
 # Add compatibility enum class
 if sys.version_info < (3, 4):
     install_requires.append("enum34")
 
 # Add compatibility ipaddress module
 if sys.version_info < (3, 3):
     install_requires.append("ipaddress")
 
 # Get contents of README file
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
-    version='1.8.6',
+    version='1.8.7',
     name='testgres',
     packages=['testgres'],
     description='Testing utility for PostgreSQL and its extensions',
     url='https://github.com/postgrespro/testgres',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='PostgreSQL',
```

### Comparing `testgres-1.8.6/testgres/__init__.py` & `testgres-1.8.7/testgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/api.py` & `testgres-1.8.7/testgres/api.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/backup.py` & `testgres-1.8.7/testgres/backup.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/cache.py` & `testgres-1.8.7/testgres/cache.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/config.py` & `testgres-1.8.7/testgres/config.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/connection.py` & `testgres-1.8.7/testgres/connection.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/consts.py` & `testgres-1.8.7/testgres/consts.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/decorators.py` & `testgres-1.8.7/testgres/decorators.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/defaults.py` & `testgres-1.8.7/testgres/defaults.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/enums.py` & `testgres-1.8.7/testgres/enums.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/exceptions.py` & `testgres-1.8.7/testgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/logger.py` & `testgres-1.8.7/testgres/logger.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/node.py` & `testgres-1.8.7/testgres/node.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/pubsub.py` & `testgres-1.8.7/testgres/pubsub.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/standby.py` & `testgres-1.8.7/testgres/standby.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres/utils.py` & `testgres-1.8.7/testgres/utils.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/testgres.egg-info/PKG-INFO` & `testgres-1.8.7/testgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testgres
-Version: 1.8.6
+Version: 1.8.7
 Summary: Testing utility for PostgreSQL and its extensions
 Home-page: https://github.com/postgrespro/testgres
 Author: Ildar Musin
 Author-email: zildermann@gmail.com
 License: PostgreSQL
 Keywords: test,testing,postgresql
 Platform: UNKNOWN
```

### Comparing `testgres-1.8.6/testgres.egg-info/SOURCES.txt` & `testgres-1.8.7/testgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testgres-1.8.6/tests/test_simple.py` & `testgres-1.8.7/tests/test_simple.py`

 * *Files identical despite different names*

