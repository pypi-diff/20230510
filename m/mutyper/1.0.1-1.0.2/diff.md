# Comparing `tmp/mutyper-1.0.1.tar.gz` & `tmp/mutyper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutyper-1.0.1.tar", last modified: Sat Apr 22 22:08:08 2023, max compression
+gzip compressed data, was "mutyper-1.0.2.tar", last modified: Wed May 10 18:13:17 2023, max compression
```

## Comparing `mutyper-1.0.1.tar` & `mutyper-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:08:08.203976 mutyper-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 22:07:58.000000 mutyper-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 22:07:58.000000 mutyper-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-22 22:08:08.203976 mutyper-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-22 22:07:58.000000 mutyper-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:08:08.203976 mutyper-1.0.1/mutyper/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-22 22:07:58.000000 mutyper-1.0.1/mutyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-22 22:08:08.203976 mutyper-1.0.1/mutyper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-22 22:07:58.000000 mutyper-1.0.1/mutyper/ancestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-04-22 22:07:58.000000 mutyper-1.0.1/mutyper/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:08:08.203976 mutyper-1.0.1/mutyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-22 22:08:08.000000 mutyper-1.0.1/mutyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-22 22:08:08.000000 mutyper-1.0.1/mutyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:08:08.000000 mutyper-1.0.1/mutyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 22:08:08.000000 mutyper-1.0.1/mutyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-22 22:08:08.000000 mutyper-1.0.1/mutyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 22:08:08.000000 mutyper-1.0.1/mutyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-22 22:08:08.203976 mutyper-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-22 22:07:58.000000 mutyper-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-22 22:07:58.000000 mutyper-1.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:13:17.182357 mutyper-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-10 18:12:59.000000 mutyper-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 18:12:59.000000 mutyper-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-10 18:13:17.182357 mutyper-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 18:12:59.000000 mutyper-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:13:17.182357 mutyper-1.0.2/mutyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 18:12:59.000000 mutyper-1.0.2/mutyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 18:13:17.182357 mutyper-1.0.2/mutyper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-10 18:12:59.000000 mutyper-1.0.2/mutyper/ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-05-10 18:12:59.000000 mutyper-1.0.2/mutyper/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:13:17.182357 mutyper-1.0.2/mutyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-10 18:13:17.000000 mutyper-1.0.2/mutyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 18:13:17.000000 mutyper-1.0.2/mutyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:13:17.000000 mutyper-1.0.2/mutyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 18:13:17.000000 mutyper-1.0.2/mutyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 18:13:17.000000 mutyper-1.0.2/mutyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 18:13:17.000000 mutyper-1.0.2/mutyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 18:13:17.182357 mutyper-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 18:12:59.000000 mutyper-1.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-10 18:12:59.000000 mutyper-1.0.2/versioneer.py
```

### Comparing `mutyper-1.0.1/LICENSE` & `mutyper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mutyper-1.0.1/PKG-INFO` & `mutyper-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutyper
-Version: 1.0.1
+Version: 1.0.2
 Summary: ancestral k-mer mutation types for SNP data
 Home-page: https://github.com/harrispopgen/mutyper
 Author: William DeWitt
 Author-email: wsdewitt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutyper-1.0.1/README.md` & `mutyper-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mutyper-1.0.1/mutyper/ancestor.py` & `mutyper-1.0.2/mutyper/ancestor.py`

 * *Files identical despite different names*

### Comparing `mutyper-1.0.1/mutyper/cli.py` & `mutyper-1.0.2/mutyper/cli.py`

 * *Files identical despite different names*

### Comparing `mutyper-1.0.1/mutyper.egg-info/PKG-INFO` & `mutyper-1.0.2/mutyper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutyper
-Version: 1.0.1
+Version: 1.0.2
 Summary: ancestral k-mer mutation types for SNP data
 Home-page: https://github.com/harrispopgen/mutyper
 Author: William DeWitt
 Author-email: wsdewitt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutyper-1.0.1/setup.py` & `mutyper-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `mutyper-1.0.1/versioneer.py` & `mutyper-1.0.2/versioneer.py`

 * *Files identical despite different names*

