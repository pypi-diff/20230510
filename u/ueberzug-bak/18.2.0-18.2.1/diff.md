# Comparing `tmp/ueberzug-bak-18.2.0.tar.gz` & `tmp/ueberzug-bak-18.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ueberzug-bak-18.2.0.tar", last modified: Wed Jan 11 05:22:09 2023, max compression
+gzip compressed data, was "ueberzug-bak-18.2.1.tar", last modified: Wed May 10 06:13:17 2023, max compression
```

## Comparing `ueberzug-bak-18.2.0.tar` & `ueberzug-bak-18.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-01-11 05:22:09.623593 ueberzug-bak-18.2.0/
--rw-r--r--   0 vesche    (1000) vesche    (1000)    35147 2023-01-11 05:19:13.000000 ueberzug-bak-18.2.0/LICENSE
--rw-r--r--   0 vesche    (1000) vesche    (1000)       74 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/MANIFEST.in
--rw-r--r--   0 vesche    (1000) vesche    (1000)      711 2023-01-11 05:22:09.623593 ueberzug-bak-18.2.0/PKG-INFO
--rw-r--r--   0 vesche    (1000) vesche    (1000)    14320 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/README.md
--rw-r--r--   0 vesche    (1000) vesche    (1000)       38 2023-01-11 05:22:09.623593 ueberzug-bak-18.2.0/setup.cfg
--rwxr-xr-x   0 vesche    (1000) vesche    (1000)     4508 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/setup.py
-drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-01-11 05:22:09.623593 ueberzug-bak-18.2.0/ueberzug/
-drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-01-11 05:22:09.623593 ueberzug-bak-18.2.0/ueberzug/X/
--rw-r--r--   0 vesche    (1000) vesche    (1000)     1397 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/X.c
--rw-r--r--   0 vesche    (1000) vesche    (1000)       81 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/X.h
--rw-r--r--   0 vesche    (1000) vesche    (1000)     9939 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/Xshm.c
--rw-r--r--   0 vesche    (1000) vesche    (1000)       98 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/Xshm.h
--rw-r--r--   0 vesche    (1000) vesche    (1000)     8846 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/display.c
--rw-r--r--   0 vesche    (1000) vesche    (1000)      544 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/display.h
--rw-r--r--   0 vesche    (1000) vesche    (1000)      133 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/math.h
--rw-r--r--   0 vesche    (1000) vesche    (1000)      190 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/python.h
--rw-r--r--   0 vesche    (1000) vesche    (1000)      785 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/util.h
--rw-r--r--   0 vesche    (1000) vesche    (1000)     9190 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/window.c
--rw-r--r--   0 vesche    (1000) vesche    (1000)      103 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/X/window.h
--rw-r--r--   0 vesche    (1000) vesche    (1000)      343 2023-01-11 05:21:01.000000 ueberzug-bak-18.2.0/ueberzug/__init__.py
--rwxr-xr-x   0 vesche    (1000) vesche    (1000)     1839 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/__main__.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)    10872 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/action.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     8083 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/batch.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)      331 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/conversion.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     1226 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/files.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)      520 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/geometry.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     7885 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/layer.py
-drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-01-11 05:22:09.623593 ueberzug-bak-18.2.0/ueberzug/lib/
--rw-r--r--   0 vesche    (1000) vesche    (1000)        0 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/lib/__init__.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     1726 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/lib/lib.sh
-drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-01-11 05:22:09.623593 ueberzug-bak-18.2.0/ueberzug/lib/v0/
--rw-r--r--   0 vesche    (1000) vesche    (1000)    12951 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/lib/v0/__init__.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)      187 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/library.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)    16502 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/loading.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     3613 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/parser.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)      345 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/pattern.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     4567 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/process.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     2908 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/query_windows.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     8479 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/scaling.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     4381 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/terminal.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     1715 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/thread.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     2563 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/tmux_util.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     6510 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/ui.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)       63 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/version.py
--rw-r--r--   0 vesche    (1000) vesche    (1000)     3997 2023-01-11 05:19:26.000000 ueberzug-bak-18.2.0/ueberzug/xutil.py
-drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-01-11 05:22:09.623593 ueberzug-bak-18.2.0/ueberzug_bak.egg-info/
--rw-r--r--   0 vesche    (1000) vesche    (1000)      711 2023-01-11 05:22:08.000000 ueberzug-bak-18.2.0/ueberzug_bak.egg-info/PKG-INFO
--rw-r--r--   0 vesche    (1000) vesche    (1000)      952 2023-01-11 05:22:08.000000 ueberzug-bak-18.2.0/ueberzug_bak.egg-info/SOURCES.txt
--rw-r--r--   0 vesche    (1000) vesche    (1000)        1 2023-01-11 05:22:08.000000 ueberzug-bak-18.2.0/ueberzug_bak.egg-info/dependency_links.txt
--rw-r--r--   0 vesche    (1000) vesche    (1000)       52 2023-01-11 05:22:08.000000 ueberzug-bak-18.2.0/ueberzug_bak.egg-info/entry_points.txt
--rw-r--r--   0 vesche    (1000) vesche    (1000)       28 2023-01-11 05:22:08.000000 ueberzug-bak-18.2.0/ueberzug_bak.egg-info/requires.txt
--rw-r--r--   0 vesche    (1000) vesche    (1000)        9 2023-01-11 05:22:08.000000 ueberzug-bak-18.2.0/ueberzug_bak.egg-info/top_level.txt
+drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-05-10 06:13:17.934229 ueberzug-bak-18.2.1/
+-rw-r--r--   0 vesche    (1000) vesche    (1000)    35147 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/LICENSE
+-rw-r--r--   0 vesche    (1000) vesche    (1000)       74 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/MANIFEST.in
+-rw-r--r--   0 vesche    (1000) vesche    (1000)    15072 2023-05-10 06:13:17.934229 ueberzug-bak-18.2.1/PKG-INFO
+-rw-r--r--   0 vesche    (1000) vesche    (1000)    14320 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/README.md
+-rw-r--r--   0 vesche    (1000) vesche    (1000)       38 2023-05-10 06:13:17.934229 ueberzug-bak-18.2.1/setup.cfg
+-rwxr-xr-x   0 vesche    (1000) vesche    (1000)     4768 2023-05-10 06:12:31.000000 ueberzug-bak-18.2.1/setup.py
+drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-05-10 06:13:17.930895 ueberzug-bak-18.2.1/ueberzug/
+drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-05-10 06:13:17.934229 ueberzug-bak-18.2.1/ueberzug/X/
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     1397 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/X.c
+-rw-r--r--   0 vesche    (1000) vesche    (1000)       81 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/X.h
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     9939 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/Xshm.c
+-rw-r--r--   0 vesche    (1000) vesche    (1000)       98 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/Xshm.h
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     8846 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/display.c
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      544 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/display.h
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      133 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/math.h
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      190 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/python.h
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      785 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/util.h
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     9190 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/window.c
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      103 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/X/window.h
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      343 2023-05-10 06:12:40.000000 ueberzug-bak-18.2.1/ueberzug/__init__.py
+-rwxr-xr-x   0 vesche    (1000) vesche    (1000)     1839 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/__main__.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)    10872 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/action.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     8083 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/batch.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      331 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/conversion.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     1226 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/files.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      520 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/geometry.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     7885 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/layer.py
+drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-05-10 06:13:17.934229 ueberzug-bak-18.2.1/ueberzug/lib/
+-rw-r--r--   0 vesche    (1000) vesche    (1000)        0 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/lib/__init__.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     1726 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/lib/lib.sh
+drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-05-10 06:13:17.934229 ueberzug-bak-18.2.1/ueberzug/lib/v0/
+-rw-r--r--   0 vesche    (1000) vesche    (1000)    12951 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/lib/v0/__init__.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      187 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/library.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)    16502 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/loading.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     3613 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/parser.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      345 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/pattern.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     4567 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/process.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     2908 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/query_windows.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     8479 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/scaling.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     4381 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/terminal.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     1715 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/thread.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     2563 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/tmux_util.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     6510 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/ui.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)       63 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/version.py
+-rw-r--r--   0 vesche    (1000) vesche    (1000)     3997 2023-05-10 06:07:10.000000 ueberzug-bak-18.2.1/ueberzug/xutil.py
+drwxr-xr-x   0 vesche    (1000) vesche    (1000)        0 2023-05-10 06:13:17.934229 ueberzug-bak-18.2.1/ueberzug_bak.egg-info/
+-rw-r--r--   0 vesche    (1000) vesche    (1000)    15072 2023-05-10 06:13:17.000000 ueberzug-bak-18.2.1/ueberzug_bak.egg-info/PKG-INFO
+-rw-r--r--   0 vesche    (1000) vesche    (1000)      952 2023-05-10 06:13:17.000000 ueberzug-bak-18.2.1/ueberzug_bak.egg-info/SOURCES.txt
+-rw-r--r--   0 vesche    (1000) vesche    (1000)        1 2023-05-10 06:13:17.000000 ueberzug-bak-18.2.1/ueberzug_bak.egg-info/dependency_links.txt
+-rw-r--r--   0 vesche    (1000) vesche    (1000)       52 2023-05-10 06:13:17.000000 ueberzug-bak-18.2.1/ueberzug_bak.egg-info/entry_points.txt
+-rw-r--r--   0 vesche    (1000) vesche    (1000)       28 2023-05-10 06:13:17.000000 ueberzug-bak-18.2.1/ueberzug_bak.egg-info/requires.txt
+-rw-r--r--   0 vesche    (1000) vesche    (1000)        9 2023-05-10 06:13:17.000000 ueberzug-bak-18.2.1/ueberzug_bak.egg-info/top_level.txt
```

### Comparing `ueberzug-bak-18.2.0/LICENSE` & `ueberzug-bak-18.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/README.md` & `ueberzug-bak-18.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/setup.py` & `ueberzug-bak-18.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 #!/usr/bin/env python3
+
+import os
 import distutils.core
 import setuptools
 import glob
 
 import ueberzug
 # To use a consistent encoding
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
+directory = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(directory, "README.md"), encoding="utf-8") as f:
+    long_description = f.read()
+
 setuptools.setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
     #
     # $ pip install sampleproject
     #
     # And where it will live on PyPI: https://pypi.org/project/sampleproject/
     #
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='ueberzug-bak',  # Required
     license=ueberzug.__license__,
-
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     include_package_data=True,
     package_data={
         '': ['*.sh'],
     },
     entry_points={
         'console_scripts': [
             'ueberzug=ueberzug.__main__:main'
@@ -96,15 +103,15 @@
 
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['pillow', 'docopt', 'attrs>=18.2.0'],  # Optional
+    install_requires=['pillow', 'docopt', 'attrs>=18.2.1'],  # Optional
     python_requires='>=3.6',
 
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
```

### Comparing `ueberzug-bak-18.2.0/ueberzug/X/X.c` & `ueberzug-bak-18.2.1/ueberzug/X/X.c`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/X/Xshm.c` & `ueberzug-bak-18.2.1/ueberzug/X/Xshm.c`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/X/display.c` & `ueberzug-bak-18.2.1/ueberzug/X/display.c`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/X/display.h` & `ueberzug-bak-18.2.1/ueberzug/X/display.h`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/X/util.h` & `ueberzug-bak-18.2.1/ueberzug/X/util.h`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/X/window.c` & `ueberzug-bak-18.2.1/ueberzug/X/window.c`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/__main__.py` & `ueberzug-bak-18.2.1/ueberzug/__main__.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/action.py` & `ueberzug-bak-18.2.1/ueberzug/action.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/batch.py` & `ueberzug-bak-18.2.1/ueberzug/batch.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/files.py` & `ueberzug-bak-18.2.1/ueberzug/files.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/geometry.py` & `ueberzug-bak-18.2.1/ueberzug/geometry.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/layer.py` & `ueberzug-bak-18.2.1/ueberzug/layer.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/lib/lib.sh` & `ueberzug-bak-18.2.1/ueberzug/lib/lib.sh`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/lib/v0/__init__.py` & `ueberzug-bak-18.2.1/ueberzug/lib/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/loading.py` & `ueberzug-bak-18.2.1/ueberzug/loading.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/parser.py` & `ueberzug-bak-18.2.1/ueberzug/parser.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/process.py` & `ueberzug-bak-18.2.1/ueberzug/process.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/query_windows.py` & `ueberzug-bak-18.2.1/ueberzug/query_windows.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/scaling.py` & `ueberzug-bak-18.2.1/ueberzug/scaling.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/terminal.py` & `ueberzug-bak-18.2.1/ueberzug/terminal.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/thread.py` & `ueberzug-bak-18.2.1/ueberzug/thread.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/tmux_util.py` & `ueberzug-bak-18.2.1/ueberzug/tmux_util.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/ui.py` & `ueberzug-bak-18.2.1/ueberzug/ui.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug/xutil.py` & `ueberzug-bak-18.2.1/ueberzug/xutil.py`

 * *Files identical despite different names*

### Comparing `ueberzug-bak-18.2.0/ueberzug_bak.egg-info/SOURCES.txt` & `ueberzug-bak-18.2.1/ueberzug_bak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

