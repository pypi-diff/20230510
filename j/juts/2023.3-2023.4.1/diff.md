# Comparing `tmp/juts-2023.3.tar.gz` & `tmp/juts-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juts-2023.3.tar", last modified: Thu Apr 27 14:24:04 2023, max compression
+gzip compressed data, was "juts-2023.4.1.tar", last modified: Tue May  9 22:44:35 2023, max compression
```

## Comparing `juts-2023.3.tar` & `juts-2023.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:24:04.370401 juts-2023.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-27 14:23:49.000000 juts-2023.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-27 14:24:04.370401 juts-2023.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:24:04.366401 juts-2023.3/juts/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 14:23:49.000000 juts-2023.3/juts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-04-27 14:23:49.000000 juts-2023.3/juts/container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:24:04.370401 juts-2023.3/juts/customjobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:23:49.000000 juts-2023.3/juts/customjobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:24:04.370401 juts-2023.3/juts/customplots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:23:49.000000 juts-2023.3/juts/customplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-27 14:23:49.000000 juts-2023.3/juts/customplots/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-04-27 14:23:49.000000 juts-2023.3/juts/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-04-27 14:23:49.000000 juts-2023.3/juts/plotwidgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:24:04.370401 juts-2023.3/juts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 14:23:49.000000 juts-2023.3/juts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-27 14:23:49.000000 juts-2023.3/juts/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-27 14:23:49.000000 juts-2023.3/juts/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-27 14:23:49.000000 juts-2023.3/juts/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    27135 2023-04-27 14:23:49.000000 juts-2023.3/juts/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 14:24:04.370401 juts-2023.3/juts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-27 14:24:04.000000 juts-2023.3/juts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-27 14:24:04.000000 juts-2023.3/juts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 14:24:04.000000 juts-2023.3/juts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-27 14:24:04.000000 juts-2023.3/juts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 14:24:04.000000 juts-2023.3/juts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 14:24:04.370401 juts-2023.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-27 14:23:49.000000 juts-2023.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-09 22:44:22.000000 juts-2023.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 22:44:35.115958 juts-2023.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts/customjobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/customjobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts/customplots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/customplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/customplots/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/plotwidgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27135 2023-05-09 22:44:22.000000 juts-2023.4.1/juts/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:44:35.115958 juts-2023.4.1/juts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 22:44:35.000000 juts-2023.4.1/juts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:44:35.115958 juts-2023.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-09 22:44:22.000000 juts-2023.4.1/setup.py
```

### Comparing `juts-2023.3/LICENSE` & `juts-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `juts-2023.3/juts/container.py` & `juts-2023.4.1/juts/container.py`

 * *Files identical despite different names*

### Comparing `juts-2023.3/juts/customplots/matplotlib.py` & `juts-2023.4.1/juts/customplots/matplotlib.py`

 * *Files identical despite different names*

### Comparing `juts-2023.3/juts/interface.py` & `juts-2023.4.1/juts/interface.py`

 * *Files identical despite different names*

### Comparing `juts-2023.3/juts/plotwidgets.py` & `juts-2023.4.1/juts/plotwidgets.py`

 * *Files identical despite different names*

### Comparing `juts-2023.3/juts/tests/test_container.py` & `juts-2023.4.1/juts/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `juts-2023.3/juts/tests/test_interface.py` & `juts-2023.4.1/juts/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `juts-2023.3/juts/tests/test_widgets.py` & `juts-2023.4.1/juts/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `juts-2023.3/juts/widgets.py` & `juts-2023.4.1/juts/widgets.py`

 * *Files identical despite different names*

### Comparing `juts-2023.3/setup.py` & `juts-2023.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,20 @@
         return file.read()
 
 
 description = read_file("Readme.md")
 
 setuptools.setup(
     name="juts",
-    version="2023.3",
+    version="2023.4.1",
     author="Marcus Riesmeier",
     author_email="gluehen-sierren-0c@icloud.com",
     license="BSD 3-Clause License",
-    description=description.splitlines()[0],
+    description="Jupyter widgets for scheduling processes and visualizing the resulting (live) data",
+    long_description_content_type="text/markdown",
     long_description=description,
     packages=setuptools.find_packages(),
     install_requires=read_file("requirements.txt"),
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
```

