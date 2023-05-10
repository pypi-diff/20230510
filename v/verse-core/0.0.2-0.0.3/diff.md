# Comparing `tmp/verse-core-0.0.2.tar.gz` & `tmp/verse-core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verse-core-0.0.2.tar", last modified: Thu Apr 27 21:14:30 2023, max compression
+gzip compressed data, was "verse-core-0.0.3.tar", last modified: Wed May 10 21:50:29 2023, max compression
```

## Comparing `verse-core-0.0.2.tar` & `verse-core-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 21:14:30.589800 verse-core-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verse-core-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      593 2023-04-27 21:14:30.587805 verse-core-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-04-26 23:13:54.000000 verse-core-0.0.2/README.md
--rw-rw-rw-   0        0        0      667 2023-04-27 21:14:12.000000 verse-core-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 21:14:30.590798 verse-core-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 21:14:30.522453 verse-core-0.0.2/src/
--rw-rw-rw-   0        0        0      125 2023-04-27 20:54:44.000000 verse-core-0.0.2/src/__init__.py
--rw-rw-rw-   0        0        0      162 2023-04-26 23:17:00.000000 verse-core-0.0.2/src/async_helper.py
--rw-rw-rw-   0        0        0      402 2023-04-26 23:17:08.000000 verse-core-0.0.2/src/import_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-27 21:14:30.585811 verse-core-0.0.2/verse_core.egg-info/
--rw-rw-rw-   0        0        0      593 2023-04-27 21:14:30.000000 verse-core-0.0.2/verse_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-04-27 21:14:30.000000 verse-core-0.0.2/verse_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 21:14:30.000000 verse-core-0.0.2/verse_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 21:14:30.000000 verse-core-0.0.2/verse_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 21:50:29.549864 verse-core-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verse-core-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      593 2023-05-10 21:50:29.548868 verse-core-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-04-26 23:13:54.000000 verse-core-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 21:50:29.520944 verse-core-0.0.3/core/
+-rw-rw-rw-   0        0        0      125 2023-04-27 20:54:44.000000 verse-core-0.0.3/core/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-04-26 23:17:00.000000 verse-core-0.0.3/core/async_helper.py
+-rw-rw-rw-   0        0        0      402 2023-04-26 23:17:08.000000 verse-core-0.0.3/core/import_helper.py
+-rw-rw-rw-   0        0        0      463 2023-05-08 23:41:13.000000 verse-core-0.0.3/core/model.py
+-rw-rw-rw-   0        0        0      668 2023-05-10 21:45:59.000000 verse-core-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 21:50:29.549864 verse-core-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 21:50:29.546874 verse-core-0.0.3/verse_core.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-05-10 21:50:29.000000 verse-core-0.0.3/verse_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-10 21:50:29.000000 verse-core-0.0.3/verse_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 21:50:29.000000 verse-core-0.0.3/verse_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 21:50:29.000000 verse-core-0.0.3/verse_core.egg-info/top_level.txt
```

### Comparing `verse-core-0.0.2/LICENSE` & `verse-core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `verse-core-0.0.2/PKG-INFO` & `verse-core-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verse-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Core Verse package shared by all Verse packages
 Author-email: Rapidverse <admin@rapidverse.com>
 Project-URL: Homepage, https://github.com/rapidverse/verse
 Project-URL: Bug Tracker, https://github.com/rapidverse/verse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `verse-core-0.0.2/pyproject.toml` & `verse-core-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "verse-core"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "Rapidverse", email = "admin@rapidverse.com" }]
 description = "Core Verse package shared by all Verse packages"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
 [tool.setuptools]
-package-dir = { "verse.core" = "src" }
+package-dir = { "verse.core" = "core" }
 
 [project.urls]
 "Homepage" = "https://github.com/rapidverse/verse"
 "Bug Tracker" = "https://github.com/rapidverse/verse/issues"
```

### Comparing `verse-core-0.0.2/verse_core.egg-info/PKG-INFO` & `verse-core-0.0.3/verse_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verse-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Core Verse package shared by all Verse packages
 Author-email: Rapidverse <admin@rapidverse.com>
 Project-URL: Homepage, https://github.com/rapidverse/verse
 Project-URL: Bug Tracker, https://github.com/rapidverse/verse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

