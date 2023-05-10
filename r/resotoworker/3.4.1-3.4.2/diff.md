# Comparing `tmp/resotoworker-3.4.1.tar.gz` & `tmp/resotoworker-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.4.1.tar", last modified: Fri Apr 28 15:17:01 2023, max compression
+gzip compressed data, was "resotoworker-3.4.2.tar", last modified: Wed May 10 12:26:22 2023, max compression
```

## Comparing `resotoworker-3.4.1.tar` & `resotoworker-3.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:01.656600 resotoworker-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:14:50.000000 resotoworker-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-28 15:17:01.656600 resotoworker-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-28 15:14:50.000000 resotoworker-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 15:14:50.000000 resotoworker-3.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:01.656600 resotoworker-3.4.1/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 15:14:50.000000 resotoworker-3.4.1/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:01.656600 resotoworker-3.4.1/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 15:17:01.000000 resotoworker-3.4.1/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:17:01.656600 resotoworker-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-28 15:14:50.000000 resotoworker-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:17:01.656600 resotoworker-3.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-28 15:14:50.000000 resotoworker-3.4.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:26:22.425737 resotoworker-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:23:05.000000 resotoworker-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-10 12:26:22.425737 resotoworker-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-10 12:23:05.000000 resotoworker-3.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-10 12:23:05.000000 resotoworker-3.4.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:26:22.421737 resotoworker-3.4.2/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-10 12:23:05.000000 resotoworker-3.4.2/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:26:22.421737 resotoworker-3.4.2/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-10 12:26:22.000000 resotoworker-3.4.2/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-10 12:26:22.000000 resotoworker-3.4.2/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:26:22.000000 resotoworker-3.4.2/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 12:26:22.000000 resotoworker-3.4.2/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:26:22.000000 resotoworker-3.4.2/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 12:26:22.000000 resotoworker-3.4.2/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 12:26:22.000000 resotoworker-3.4.2/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:26:22.425737 resotoworker-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-10 12:23:05.000000 resotoworker-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:26:22.425737 resotoworker-3.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:05.000000 resotoworker-3.4.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 12:23:05.000000 resotoworker-3.4.2/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-10 12:23:05.000000 resotoworker-3.4.2/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-10 12:23:05.000000 resotoworker-3.4.2/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 12:23:05.000000 resotoworker-3.4.2/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-10 12:23:05.000000 resotoworker-3.4.2/test/test_utils.py
```

### Comparing `resotoworker-3.4.1/PKG-INFO` & `resotoworker-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.4.1
+Version: 3.4.2
 Summary: Runs collector plugins and sends the result to resotocore.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoworker
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoworker-3.4.1/README.md` & `resotoworker-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker/__main__.py` & `resotoworker-3.4.2/resotoworker/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker/cleanup.py` & `resotoworker-3.4.2/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker/collect.py` & `resotoworker-3.4.2/resotoworker/collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker/config.py` & `resotoworker-3.4.2/resotoworker/config.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker/pluginloader.py` & `resotoworker-3.4.2/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker/resotocore.py` & `resotoworker-3.4.2/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker/tag.py` & `resotoworker-3.4.2/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker/utils.py` & `resotoworker-3.4.2/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.4.2/resotoworker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.4.1
+Version: 3.4.2
 Summary: Runs collector plugins and sends the result to resotocore.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoworker
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoworker-3.4.1/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.4.2/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/setup.py` & `resotoworker-3.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/test/test_collect.py` & `resotoworker-3.4.2/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/test/test_resotocore.py` & `resotoworker-3.4.2/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.4.1/test/test_utils.py` & `resotoworker-3.4.2/test/test_utils.py`

 * *Files identical despite different names*

