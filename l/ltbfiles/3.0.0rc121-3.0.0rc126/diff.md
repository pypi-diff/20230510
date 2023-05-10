# Comparing `tmp/ltbfiles-3.0.0rc121.tar.gz` & `tmp/ltbfiles-3.0.0rc126.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltbfiles-3.0.0rc121.tar", last modified: Wed May 10 12:02:25 2023, max compression
+gzip compressed data, was "ltbfiles-3.0.0rc126.tar", last modified: Wed May 10 12:29:13 2023, max compression
```

## Comparing `ltbfiles-3.0.0rc121.tar` & `ltbfiles-3.0.0rc126.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:02:25.977824 ltbfiles-3.0.0rc121/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/LICENSE_GPL_v3.txt
--rw-r--r--   0 root         (0) root         (0)     1120 2023-05-10 12:02:25.975990 ltbfiles-3.0.0rc121/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/README.md
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:02:25.972323 ltbfiles-3.0.0rc121/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:02:25.974157 ltbfiles-3.0.0rc121/python/ltbfiles/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/python/ltbfiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16202 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/python/ltbfiles/ltbfiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:02:25.975990 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1120 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      293 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 12:02:25.977824 ltbfiles-3.0.0rc121/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:29:13.717951 ltbfiles-3.0.0rc126/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-10 12:29:00.000000 ltbfiles-3.0.0rc126/LICENSE_GPL_v3.txt
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-05-10 12:29:13.717951 ltbfiles-3.0.0rc126/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-05-10 12:29:00.000000 ltbfiles-3.0.0rc126/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-05-10 12:29:00.000000 ltbfiles-3.0.0rc126/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:29:13.713950 ltbfiles-3.0.0rc126/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:29:13.715951 ltbfiles-3.0.0rc126/python/ltbfiles/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-10 12:29:00.000000 ltbfiles-3.0.0rc126/python/ltbfiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16202 2023-05-10 12:29:00.000000 ltbfiles-3.0.0rc126/python/ltbfiles/ltbfiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:29:13.717951 ltbfiles-3.0.0rc126/python/ltbfiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-05-10 12:29:13.000000 ltbfiles-3.0.0rc126/python/ltbfiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-10 12:29:13.000000 ltbfiles-3.0.0rc126/python/ltbfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:29:13.000000 ltbfiles-3.0.0rc126/python/ltbfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-10 12:29:13.000000 ltbfiles-3.0.0rc126/python/ltbfiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-10 12:29:13.000000 ltbfiles-3.0.0rc126/python/ltbfiles.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 12:29:13.718951 ltbfiles-3.0.0rc126/setup.cfg
```

### Comparing `ltbfiles-3.0.0rc121/LICENSE_GPL_v3.txt` & `ltbfiles-3.0.0rc126/LICENSE_GPL_v3.txt`

 * *Files identical despite different names*

### Comparing `ltbfiles-3.0.0rc121/PKG-INFO` & `ltbfiles-3.0.0rc126/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 3.0.0rc121
+Version: 3.0.0rc126
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ltbfiles-3.0.0rc121/README.md` & `ltbfiles-3.0.0rc126/README.md`

 * *Files identical despite different names*

### Comparing `ltbfiles-3.0.0rc121/pyproject.toml` & `ltbfiles-3.0.0rc126/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ltbfiles-3.0.0rc121/python/ltbfiles/ltbfiles.py` & `ltbfiles-3.0.0rc126/python/ltbfiles/ltbfiles.py`

 * *Files identical despite different names*

### Comparing `ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/PKG-INFO` & `ltbfiles-3.0.0rc126/python/ltbfiles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 3.0.0rc121
+Version: 3.0.0rc126
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

