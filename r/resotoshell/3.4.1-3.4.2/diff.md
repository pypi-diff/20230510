# Comparing `tmp/resotoshell-3.4.1.tar.gz` & `tmp/resotoshell-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.4.1.tar", last modified: Fri Apr 28 15:19:13 2023, max compression
+gzip compressed data, was "resotoshell-3.4.2.tar", last modified: Wed May 10 12:23:03 2023, max compression
```

## Comparing `resotoshell-3.4.1.tar` & `resotoshell-3.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:13.033838 resotoshell-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:16:45.000000 resotoshell-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-28 15:19:13.033838 resotoshell-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-28 15:16:45.000000 resotoshell-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 15:16:45.000000 resotoshell-3.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:13.033838 resotoshell-3.4.1/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 15:16:45.000000 resotoshell-3.4.1/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-04-28 15:16:45.000000 resotoshell-3.4.1/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-04-28 15:16:45.000000 resotoshell-3.4.1/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-28 15:16:45.000000 resotoshell-3.4.1/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-28 15:16:45.000000 resotoshell-3.4.1/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:13.033838 resotoshell-3.4.1/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-28 15:19:13.000000 resotoshell-3.4.1/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-28 15:19:13.000000 resotoshell-3.4.1/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:19:13.000000 resotoshell-3.4.1/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 15:19:13.000000 resotoshell-3.4.1/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:19:13.000000 resotoshell-3.4.1/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-28 15:19:13.000000 resotoshell-3.4.1/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 15:19:13.000000 resotoshell-3.4.1/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-28 15:19:13.033838 resotoshell-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-28 15:16:45.000000 resotoshell-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:19:13.033838 resotoshell-3.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-04-28 15:16:45.000000 resotoshell-3.4.1/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-28 15:16:45.000000 resotoshell-3.4.1/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:03.671552 resotoshell-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:20:33.000000 resotoshell-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-10 12:23:03.671552 resotoshell-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-10 12:20:33.000000 resotoshell-3.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:20:33.000000 resotoshell-3.4.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:03.667552 resotoshell-3.4.2/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-10 12:20:33.000000 resotoshell-3.4.2/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:03.671552 resotoshell-3.4.2/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 12:23:03.000000 resotoshell-3.4.2/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 12:23:03.671552 resotoshell-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-10 12:20:33.000000 resotoshell-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:23:03.671552 resotoshell-3.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-05-10 12:20:33.000000 resotoshell-3.4.2/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-10 12:20:33.000000 resotoshell-3.4.2/test/test_protected_files.py
```

### Comparing `resotoshell-3.4.1/PKG-INFO` & `resotoshell-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.4.1
+Version: 3.4.2
 Summary: Commandline interpreter to interact with Resoto.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoshell
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoshell-3.4.1/README.md` & `resotoshell-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.1/resotoshell/__main__.py` & `resotoshell-3.4.2/resotoshell/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.1/resotoshell/promptsession.py` & `resotoshell-3.4.2/resotoshell/promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.1/resotoshell/protected_files.py` & `resotoshell-3.4.2/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.1/resotoshell/shell.py` & `resotoshell-3.4.2/resotoshell/shell.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.1/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.4.2/resotoshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.4.1
+Version: 3.4.2
 Summary: Commandline interpreter to interact with Resoto.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotoshell
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotoshell-3.4.1/setup.py` & `resotoshell-3.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.1/test/test_promptsession.py` & `resotoshell-3.4.2/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.4.1/test/test_protected_files.py` & `resotoshell-3.4.2/test/test_protected_files.py`

 * *Files identical despite different names*

