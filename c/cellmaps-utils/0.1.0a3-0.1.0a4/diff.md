# Comparing `tmp/cellmaps_utils-0.1.0a3.tar.gz` & `tmp/cellmaps_utils-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_utils-0.1.0a3.tar", last modified: Fri May  5 20:44:32 2023, max compression
+gzip compressed data, was "dist/cellmaps_utils-0.1.0a4.tar", last modified: Tue May  9 21:57:37 2023, max compression
```

## Comparing `cellmaps_utils-0.1.0a3.tar` & `cellmaps_utils-0.1.0a4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 20:44:32.386894 cellmaps_utils-0.1.0a3/
--rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a3/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a3/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     4726 2023-05-05 20:44:32.387047 cellmaps_utils-0.1.0a3/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a3/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 20:44:32.378320 cellmaps_utils-0.1.0a3/cellmaps_utils/
--rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-05 00:53:45.000000 cellmaps_utils-0.1.0a3/cellmaps_utils/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)      795 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a3/cellmaps_utils/constants.py
--rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.1.0a3/cellmaps_utils/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a3/cellmaps_utils/logutils.py
--rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a3/cellmaps_utils/music_utils.py
--rw-r--r--   0 churas     (504) staff       (20)    11676 2023-05-05 20:36:20.000000 cellmaps_utils-0.1.0a3/cellmaps_utils/provenance.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 20:44:32.380420 cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     4726 2023-05-05 20:44:32.000000 cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      979 2023-05-05 20:44:32.000000 cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-05 20:44:32.000000 cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-05 20:44:32.000000 cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       37 2023-05-05 20:44:32.000000 cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-05 20:44:32.000000 cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 20:44:32.384868 cellmaps_utils-0.1.0a3/docs/
--rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 20:44:32.373632 cellmaps_utils-0.1.0a3/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 20:44:32.373766 cellmaps_utils-0.1.0a3/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 20:44:32.385599 cellmaps_utils-0.1.0a3/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a3/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a3/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a3/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      838 2023-05-05 00:54:50.000000 cellmaps_utils-0.1.0a3/docs/cellmaps_utils.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a3/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-05 20:44:32.387692 cellmaps_utils-0.1.0a3/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1901 2023-05-01 21:40:49.000000 cellmaps_utils-0.1.0a3/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 20:44:32.386650 cellmaps_utils-0.1.0a3/tests/
--rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a3/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a3/tests/test_logutils.py
--rw-r--r--   0 churas     (504) staff       (20)    12495 2023-05-05 20:38:11.000000 cellmaps_utils-0.1.0a3/tests/test_provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-09 21:57:37.567954 cellmaps_utils-0.1.0a4/
+-rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a4/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a4/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-09 21:57:37.568114 cellmaps_utils-0.1.0a4/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a4/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-09 21:57:37.556245 cellmaps_utils-0.1.0a4/cellmaps_utils/
+-rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-09 21:51:11.000000 cellmaps_utils-0.1.0a4/cellmaps_utils/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     2139 2023-05-09 21:51:11.000000 cellmaps_utils-0.1.0a4/cellmaps_utils/constants.py
+-rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.1.0a4/cellmaps_utils/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a4/cellmaps_utils/logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a4/cellmaps_utils/music_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)    11676 2023-05-05 20:36:20.000000 cellmaps_utils-0.1.0a4/cellmaps_utils/provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-09 21:57:37.558022 cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-09 21:57:37.000000 cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)      979 2023-05-09 21:57:37.000000 cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-09 21:57:37.000000 cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-09 21:57:37.000000 cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       51 2023-05-09 21:57:37.000000 cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-09 21:57:37.000000 cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-09 21:57:37.564627 cellmaps_utils-0.1.0a4/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-09 21:57:37.549368 cellmaps_utils-0.1.0a4/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-09 21:57:37.549470 cellmaps_utils-0.1.0a4/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-09 21:57:37.566109 cellmaps_utils-0.1.0a4/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a4/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      838 2023-05-05 00:54:50.000000 cellmaps_utils-0.1.0a4/docs/cellmaps_utils.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a4/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-09 21:57:37.568619 cellmaps_utils-0.1.0a4/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1787 2023-05-05 21:20:31.000000 cellmaps_utils-0.1.0a4/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-09 21:57:37.567439 cellmaps_utils-0.1.0a4/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a4/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a4/tests/test_logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)    12542 2023-05-09 21:54:19.000000 cellmaps_utils-0.1.0a4/tests/test_provenance.py
```

### Comparing `cellmaps_utils-0.1.0a3/CONTRIBUTING.rst` & `cellmaps_utils-0.1.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/LICENSE` & `cellmaps_utils-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/PKG-INFO` & `cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cellmaps_utils
-Version: 0.1.0a3
+Name: cellmaps-utils
+Version: 0.1.0a4
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
@@ -129,15 +129,12 @@
         
 Keywords: cellmaps_utils
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
```

### Comparing `cellmaps_utils-0.1.0a3/README.rst` & `cellmaps_utils-0.1.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/cellmaps_utils/logutils.py` & `cellmaps_utils-0.1.0a4/cellmaps_utils/logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/cellmaps_utils/music_utils.py` & `cellmaps_utils-0.1.0a4/cellmaps_utils/music_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/cellmaps_utils/provenance.py` & `cellmaps_utils-0.1.0a4/cellmaps_utils/provenance.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/PKG-INFO` & `cellmaps_utils-0.1.0a4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cellmaps-utils
-Version: 0.1.0a3
+Name: cellmaps_utils
+Version: 0.1.0a4
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
@@ -129,15 +129,12 @@
         
 Keywords: cellmaps_utils
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
```

### Comparing `cellmaps_utils-0.1.0a3/cellmaps_utils.egg-info/SOURCES.txt` & `cellmaps_utils-0.1.0a4/cellmaps_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/Makefile` & `cellmaps_utils-0.1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/cellmaps_utils.rst` & `cellmaps_utils-0.1.0a4/docs/cellmaps_utils.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/conf.py` & `cellmaps_utils-0.1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/index.rst` & `cellmaps_utils-0.1.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/installation.rst` & `cellmaps_utils-0.1.0a4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/make.bat` & `cellmaps_utils-0.1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/newrelease.rst` & `cellmaps_utils-0.1.0a4/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/pypircfile.rst` & `cellmaps_utils-0.1.0a4/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/docs/versioningscheme.rst` & `cellmaps_utils-0.1.0a4/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/setup.py` & `cellmaps_utils-0.1.0a4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['scipy',
+requirements = ['fairscape-cli',
+                'scipy',
                 'scikit-learn',
                 'pandas',
                 'numpy',
                 'dill']
 
 setup_requirements = [ ]
 
@@ -32,21 +33,18 @@
     author="Clara Hu",
     author_email='mhu@health.ucsd.edu',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
     description="Utilities needed for Cell Maps for AI",
     install_requires=requirements,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     long_description_content_type = 'text/x-rst',
     include_package_data=True,
```

### Comparing `cellmaps_utils-0.1.0a3/tests/test_logutils.py` & `cellmaps_utils-0.1.0a4/tests/test_logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a3/tests/test_provenance.py` & `cellmaps_utils-0.1.0a4/tests/test_provenance.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 """Tests for `cellmaps_utils.cellmaps_io` package."""
 
 import os
 import sys
 import shutil
 import tempfile
+from datetime import date
 import unittest
 from unittest.mock import patch
 
 from cellmaps_utils.provenance import ProvenanceUtil
 from cellmaps_utils.exceptions import CellMapsProvenanceError
 
 
@@ -122,15 +123,15 @@
                                  'outstr : errstr', str(ce))
         mock_method.assert_called_once_with(['fairscape-cli',
                                              'rocrate', 'add',
                                              'computation',
                                              '--name', 'aname',
                                              '--run-by', 'user',
                                              '--date-created',
-                                             '05-05-2023',
+                                             date.today().strftime('%m-%d-%Y'),
                                              '--command', '',
                                              '--description',
                                              'desc', 'foo'], timeout=60)
 
     def test_register_computation_actual_invocation(self):
         temp_dir = tempfile.mkdtemp()
         try:
```

