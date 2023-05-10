# Comparing `tmp/appshwnd-0.10.tar.gz` & `tmp/appshwnd-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appshwnd-0.10.tar", last modified: Mon May  8 01:16:23 2023, max compression
+gzip compressed data, was "appshwnd-0.11.tar", last modified: Wed May 10 05:58:16 2023, max compression
```

## Comparing `appshwnd-0.10.tar` & `appshwnd-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 01:16:23.464992 appshwnd-0.10/
--rw-rw-rw-   0        0        0     1148 2023-05-08 01:16:18.000000 appshwnd-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      121 2023-05-08 01:16:16.000000 appshwnd-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     6349 2023-05-08 01:16:23.464992 appshwnd-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     5615 2023-05-08 01:14:32.000000 appshwnd-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 01:16:23.461002 appshwnd-0.10/appshwnd/
--rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 appshwnd-0.10/appshwnd/LICENSE
--rw-rw-rw-   0        0        0     5615 2023-05-08 01:14:32.000000 appshwnd-0.10/appshwnd/README.md
--rw-rw-rw-   0        0        0     5044 2023-05-08 01:16:02.000000 appshwnd-0.10/appshwnd/__init__.py
--rw-rw-rw-   0        0        0       36 2023-05-08 01:16:22.000000 appshwnd-0.10/appshwnd/requirements.txt
--rw-rw-rw-   0        0        0     2509 2023-05-08 01:16:22.000000 appshwnd-0.10/appshwnd/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-08 01:16:23.463994 appshwnd-0.10/appshwnd.egg-info/
--rw-rw-rw-   0        0        0     6349 2023-05-08 01:16:23.000000 appshwnd-0.10/appshwnd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-05-08 01:16:23.000000 appshwnd-0.10/appshwnd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 01:16:23.000000 appshwnd-0.10/appshwnd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-08 01:16:23.000000 appshwnd-0.10/appshwnd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 01:16:23.000000 appshwnd-0.10/appshwnd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-08 01:16:23.464992 appshwnd-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1474 2023-05-08 01:16:22.000000 appshwnd-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:58:16.163419 appshwnd-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-10 05:58:07.000000 appshwnd-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      121 2023-05-10 05:58:04.000000 appshwnd-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     6349 2023-05-10 05:58:16.163419 appshwnd-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     5615 2023-05-08 01:25:41.000000 appshwnd-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 05:58:16.159429 appshwnd-0.11/appshwnd/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 00:23:59.000000 appshwnd-0.11/appshwnd/LICENSE
+-rw-rw-rw-   0        0        0     5615 2023-05-08 01:25:41.000000 appshwnd-0.11/appshwnd/README.md
+-rw-rw-rw-   0        0        0     5085 2023-05-10 05:56:17.000000 appshwnd-0.11/appshwnd/__init__.py
+-rw-rw-rw-   0        0        0       36 2023-05-10 05:58:15.000000 appshwnd-0.11/appshwnd/requirements.txt
+-rw-rw-rw-   0        0        0     2509 2023-05-10 05:58:15.000000 appshwnd-0.11/appshwnd/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-10 05:58:16.162421 appshwnd-0.11/appshwnd.egg-info/
+-rw-rw-rw-   0        0        0     6349 2023-05-10 05:58:15.000000 appshwnd-0.11/appshwnd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-05-10 05:58:16.000000 appshwnd-0.11/appshwnd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 05:58:15.000000 appshwnd-0.11/appshwnd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-10 05:58:15.000000 appshwnd-0.11/appshwnd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 05:58:15.000000 appshwnd-0.11/appshwnd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-10 05:58:16.163419 appshwnd-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2023-05-10 05:58:15.000000 appshwnd-0.11/setup.py
```

### Comparing `appshwnd-0.10/LICENSE.rst` & `appshwnd-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `appshwnd-0.10/PKG-INFO` & `appshwnd-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appshwnd
-Version: 0.10
+Version: 0.11
 Summary: includes functions for finding windows based on various attributes, getting information about visible and invisible windows, and making window names unique
 Home-page: https://github.com/hansalemaos/appshwnd
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ctypes,hwnd,search,windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `appshwnd-0.10/README.md` & `appshwnd-0.11/README.md`

 * *Files identical despite different names*

### Comparing `appshwnd-0.10/appshwnd/LICENSE` & `appshwnd-0.11/appshwnd/LICENSE`

 * *Files identical despite different names*

### Comparing `appshwnd-0.10/appshwnd/README.md` & `appshwnd-0.11/appshwnd/README.md`

 * *Files identical despite different names*

### Comparing `appshwnd-0.10/appshwnd/__init__.py` & `appshwnd-0.11/appshwnd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         bestwindow,
         hwnd,
         startwindowtext,
         updatedwindowtext,
         FlexiblePartialOwnName(
             _restore_window_name,
             f"{hwnd} / {repr(startwindowtext)} / {repr(updatedwindowtext)}",
-            True,
+            True, hwnd, startwindowtext, updatedwindowtext
         ),
     )
 
 
 def _find_best_matching_window(searchdict: dict, *args, **kwargs):
     r"""
         Find the best matching window for the given criteria dictionary.
```

### Comparing `appshwnd-0.10/appshwnd/thirdparty.json` & `appshwnd-0.11/appshwnd/thirdparty.json`

 * *Files identical despite different names*

### Comparing `appshwnd-0.10/appshwnd.egg-info/PKG-INFO` & `appshwnd-0.11/appshwnd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appshwnd
-Version: 0.10
+Version: 0.11
 Summary: includes functions for finding windows based on various attributes, getting information about visible and invisible windows, and making window names unique
 Home-page: https://github.com/hansalemaos/appshwnd
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: ctypes,hwnd,search,windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `appshwnd-0.10/setup.py` & `appshwnd-0.11/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''includes functions for finding windows based on various attributes, getting information about visible and invisible windows, and making window names unique'''
 
 # Setting up
 setup(
     name="appshwnd",
     version=VERSION,
     license='MIT',
```

