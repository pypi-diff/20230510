# Comparing `tmp/jcmutils-1.4.0.tar.gz` & `tmp/jcmutils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.4.0.tar", last modified: Wed May 10 03:07:24 2023, max compression
+gzip compressed data, was "jcmutils-1.4.1.tar", last modified: Wed May 10 04:18:01 2023, max compression
```

## Comparing `jcmutils-1.4.0.tar` & `jcmutils-1.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 03:07:24.555660 jcmutils-1.4.0/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.0/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-10 03:07:24.555660 jcmutils-1.4.0/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.0/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 03:07:24.555660 jcmutils-1.4.0/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.0/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2613 2023-04-19 07:20:15.000000 jcmutils-1.4.0/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.0/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.0/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8801 2023-05-10 03:03:53.000000 jcmutils-1.4.0/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 03:07:24.555660 jcmutils-1.4.0/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-10 03:07:24.555660 jcmutils-1.4.0/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-05-10 03:06:10.000000 jcmutils-1.4.0/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 04:18:01.418849 jcmutils-1.4.1/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.1/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-10 04:18:01.418849 jcmutils-1.4.1/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.1/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 04:18:01.418849 jcmutils-1.4.1/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.1/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2613 2023-04-19 07:20:15.000000 jcmutils-1.4.1/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.1/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.1/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8781 2023-05-10 04:17:24.000000 jcmutils-1.4.1/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 04:18:01.418849 jcmutils-1.4.1/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-10 04:18:01.000000 jcmutils-1.4.1/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-10 04:18:01.418849 jcmutils-1.4.1/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-05-10 04:17:38.000000 jcmutils-1.4.1/setup.py
```

### Comparing `jcmutils-1.4.0/LICENSE` & `jcmutils-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.0/README.md` & `jcmutils-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.0/jcmutils/dataset_utils.py` & `jcmutils-1.4.1/jcmutils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.0/jcmutils/gen_sources.py` & `jcmutils-1.4.1/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.0/jcmutils/logger.py` & `jcmutils-1.4.1/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.0/jcmutils/solver.py` & `jcmutils-1.4.1/jcmutils/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,8 +207,8 @@
             logger.error(f"the key is : {key}")
             raise Exception(f"get result failed! target key not find in resultbag,the key is {key}")
     
     def __start_timing(self):
         return datetime.datetime.now()
     
     def __count_time(self,last_time):
-        return datetime.timedelta(datetime.datetime.now() - last_time)
+        return datetime.datetime.now() - last_time
```

### Comparing `jcmutils-1.4.0/setup.py` & `jcmutils-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.4.0'
+VERSION = '1.4.1'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

