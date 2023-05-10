# Comparing `tmp/fstflowchat-0.0.5.tar.gz` & `tmp/fstflowchat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fstflowchat-0.0.5.tar", last modified: Tue May  2 20:50:21 2023, max compression
+gzip compressed data, was "fstflowchat-0.0.6.tar", last modified: Wed May 10 01:39:55 2023, max compression
```

## Comparing `fstflowchat-0.0.5.tar` & `fstflowchat-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-02 20:50:21.629103 fstflowchat-0.0.5/
--rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.5/LICENSE
--rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.5/MANIFEST.in
--rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-05-02 20:50:21.628473 fstflowchat-0.0.5/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)     1473 2023-04-24 00:59:35.000000 fstflowchat-0.0.5/README.md
--rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-05-02 20:50:21.629299 fstflowchat-0.0.5/setup.cfg
--rwxr-xr-x   0 kaze7539   (503) staff       (20)     8199 2023-05-02 20:48:26.000000 fstflowchat-0.0.5/setup.py
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-02 20:50:21.545734 fstflowchat-0.0.5/src/
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-02 20:50:21.615668 fstflowchat-0.0.5/src/fstflowchat/
--rw-r--r--   0 kaze7539   (503) staff       (20)     4384 2023-05-02 20:40:08.000000 fstflowchat-0.0.5/src/fstflowchat/__init__.py
--rw-r--r--   0 kaze7539   (503) staff       (20)     7200 2023-04-24 01:50:56.000000 fstflowchat-0.0.5/src/fstflowchat/example.py
--rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.5/src/fstflowchat/quiz.dot
-drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-02 20:50:21.627220 fstflowchat-0.0.5/src/fstflowchat.egg-info/
--rw-r--r--   0 kaze7539   (503) staff       (20)     2614 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/PKG-INFO
--rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/SOURCES.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/dependency_links.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/entry_points.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       16 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/requires.txt
--rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-05-02 20:50:21.000000 fstflowchat-0.0.5/src/fstflowchat.egg-info/top_level.txt
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 01:39:55.355319 fstflowchat-0.0.6/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     1071 2023-04-19 21:48:08.000000 fstflowchat-0.0.6/LICENSE
+-rw-r--r--   0 kaze7539   (503) staff       (20)       28 2023-04-24 01:28:18.000000 fstflowchat-0.0.6/MANIFEST.in
+-rw-r--r--   0 kaze7539   (503) staff       (20)     3321 2023-05-10 01:39:55.354382 fstflowchat-0.0.6/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)     2180 2023-05-08 16:46:47.000000 fstflowchat-0.0.6/README.md
+-rw-r--r--   0 kaze7539   (503) staff       (20)       38 2023-05-10 01:39:55.355511 fstflowchat-0.0.6/setup.cfg
+-rwxr-xr-x   0 kaze7539   (503) staff       (20)     8199 2023-05-10 01:39:38.000000 fstflowchat-0.0.6/setup.py
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 01:39:55.322375 fstflowchat-0.0.6/src/
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 01:39:55.342918 fstflowchat-0.0.6/src/fstflowchat/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     4384 2023-05-02 20:40:08.000000 fstflowchat-0.0.6/src/fstflowchat/__init__.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)     7200 2023-04-24 01:50:56.000000 fstflowchat-0.0.6/src/fstflowchat/example.py
+-rw-r--r--   0 kaze7539   (503) staff       (20)      795 2023-04-23 23:37:09.000000 fstflowchat-0.0.6/src/fstflowchat/quiz.dot
+drwxr-xr-x   0 kaze7539   (503) staff       (20)        0 2023-05-10 01:39:55.353342 fstflowchat-0.0.6/src/fstflowchat.egg-info/
+-rw-r--r--   0 kaze7539   (503) staff       (20)     3321 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/PKG-INFO
+-rw-r--r--   0 kaze7539   (503) staff       (20)      354 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)        1 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       65 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/entry_points.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       16 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/requires.txt
+-rw-r--r--   0 kaze7539   (503) staff       (20)       12 2023-05-10 01:39:55.000000 fstflowchat-0.0.6/src/fstflowchat.egg-info/top_level.txt
```

### Comparing `fstflowchat-0.0.5/LICENSE` & `fstflowchat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.5/PKG-INFO` & `fstflowchat-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.5
+Version: 0.0.6
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
@@ -35,47 +35,73 @@
 two functions, a test function that determines if the edge is a valid
 transition, and an output fuction that determines the system's output
 as it changes state.
 
 
 ## Installation
 
-To install the development version, run 
 
-```
-pip install git+https://github.com/abecode/fstflowchat
-```
-
-Currently the development version is preferred.
-
-To run the stable version (in the future), run
+To run the stable version run
 
 ```
 pip install fstflowchat
 ```
 
-
-Currently the only dependency is the [graphviz
+You will first need to install graphviz [graphviz
 application](https://graphviz.org/download/) and the [pygraphviz
 library](https://pygraphviz.github.io/documentation/stable/install.html).
-For mac installation issues, please use the following command as
-described in this [stackoverflow
+
+
+For mac installation issues, if you receive an error, please use the
+following command after running `brew install graphviz`, as described
+in this [stackoverflow
 question](https://stackoverflow.com/questions/69970147/how-do-i-resolve-the-pygraphviz-error-on-mac-os)
 
 ```
 python -m pip install \
-    --global-option=build_ext \
-    --global-option="-I$(brew --prefix graphviz)/include/" \
-    --global-option="-L$(brew --prefix graphviz)/lib/" \
-    pygraphviz
+	--global-option=build_ext \
+	--global-option="-I$(brew --prefix graphviz)/include/" \
+	--global-option="-L$(brew --prefix graphviz)/lib/" \
+	pygraphviz
+```
+
+To install on a Colab notebook, run the following shell escaped
+commands to install graphviz and its development libraries and test
+the python pygraphviz library before installing fstflowchat:
+
 ```
+# install graphviz with development libraries
+!apt install libgraphviz-dev
+
+# test pygraphviz library (used by fstflowchat
+!pip install pygraphviz
+
+# install fstflowchat
+!pip install fstflowchat
+```
+
+
+If you are interested in contributing to fstflowchat or if you want to
+use the latest code from github (potentially with breaking changes)
+you can install fstflowchat in the following ways:
+
+```
+# clone and install as an editable pip library
+git clone git+https://github.com/abecode/fstflowchat
+cd fstflowchat
+pip install -e .
+
+# pip install directly from github
+pip install git+https://github.com/abecode/fstflowchat
+```
+
 
 ## Running a demo
 
-To see a demo, run 
+To see a demo, run
 
 ```
 fstflowchat-example
 ```
 
 ## Documentation
```

### Comparing `fstflowchat-0.0.5/README.md` & `fstflowchat-0.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,47 +9,73 @@
 two functions, a test function that determines if the edge is a valid
 transition, and an output fuction that determines the system's output
 as it changes state.
 
 
 ## Installation
 
-To install the development version, run 
 
-```
-pip install git+https://github.com/abecode/fstflowchat
-```
-
-Currently the development version is preferred.
-
-To run the stable version (in the future), run
+To run the stable version run
 
 ```
 pip install fstflowchat
 ```
 
-
-Currently the only dependency is the [graphviz
+You will first need to install graphviz [graphviz
 application](https://graphviz.org/download/) and the [pygraphviz
 library](https://pygraphviz.github.io/documentation/stable/install.html).
-For mac installation issues, please use the following command as
-described in this [stackoverflow
+
+
+For mac installation issues, if you receive an error, please use the
+following command after running `brew install graphviz`, as described
+in this [stackoverflow
 question](https://stackoverflow.com/questions/69970147/how-do-i-resolve-the-pygraphviz-error-on-mac-os)
 
 ```
 python -m pip install \
-    --global-option=build_ext \
-    --global-option="-I$(brew --prefix graphviz)/include/" \
-    --global-option="-L$(brew --prefix graphviz)/lib/" \
-    pygraphviz
+	--global-option=build_ext \
+	--global-option="-I$(brew --prefix graphviz)/include/" \
+	--global-option="-L$(brew --prefix graphviz)/lib/" \
+	pygraphviz
+```
+
+To install on a Colab notebook, run the following shell escaped
+commands to install graphviz and its development libraries and test
+the python pygraphviz library before installing fstflowchat:
+
 ```
+# install graphviz with development libraries
+!apt install libgraphviz-dev
+
+# test pygraphviz library (used by fstflowchat
+!pip install pygraphviz
+
+# install fstflowchat
+!pip install fstflowchat
+```
+
+
+If you are interested in contributing to fstflowchat or if you want to
+use the latest code from github (potentially with breaking changes)
+you can install fstflowchat in the following ways:
+
+```
+# clone and install as an editable pip library
+git clone git+https://github.com/abecode/fstflowchat
+cd fstflowchat
+pip install -e .
+
+# pip install directly from github
+pip install git+https://github.com/abecode/fstflowchat
+```
+
 
 ## Running a demo
 
-To see a demo, run 
+To see a demo, run
 
 ```
 fstflowchat-example
 ```
 
 ## Documentation
```

### Comparing `fstflowchat-0.0.5/setup.py` & `fstflowchat-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.5",  # Required
+    version="0.0.6",  # Required
     
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="a small, pedagogical, fst-based dialog toolkit.",  # Optional
     
     # This is an optional longer description of your project that represents
```

### Comparing `fstflowchat-0.0.5/src/fstflowchat/__init__.py` & `fstflowchat-0.0.6/src/fstflowchat/__init__.py`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.5/src/fstflowchat/example.py` & `fstflowchat-0.0.6/src/fstflowchat/example.py`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.5/src/fstflowchat/quiz.dot` & `fstflowchat-0.0.6/src/fstflowchat/quiz.dot`

 * *Files identical despite different names*

### Comparing `fstflowchat-0.0.5/src/fstflowchat.egg-info/PKG-INFO` & `fstflowchat-0.0.6/src/fstflowchat.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstflowchat
-Version: 0.0.5
+Version: 0.0.6
 Summary: a small, pedagogical, fst-based dialog toolkit.
 Home-page: https://fstflowchat.readthedocs.io/en/latest/
 Author: Abe Kazemzadeh
 Project-URL: Bug Reports, https://github.com/abecode/fstflowchat/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
 Project-URL: Source, https://github.com/abecode/fstflowchat/issues
@@ -35,47 +35,73 @@
 two functions, a test function that determines if the edge is a valid
 transition, and an output fuction that determines the system's output
 as it changes state.
 
 
 ## Installation
 
-To install the development version, run 
 
-```
-pip install git+https://github.com/abecode/fstflowchat
-```
-
-Currently the development version is preferred.
-
-To run the stable version (in the future), run
+To run the stable version run
 
 ```
 pip install fstflowchat
 ```
 
-
-Currently the only dependency is the [graphviz
+You will first need to install graphviz [graphviz
 application](https://graphviz.org/download/) and the [pygraphviz
 library](https://pygraphviz.github.io/documentation/stable/install.html).
-For mac installation issues, please use the following command as
-described in this [stackoverflow
+
+
+For mac installation issues, if you receive an error, please use the
+following command after running `brew install graphviz`, as described
+in this [stackoverflow
 question](https://stackoverflow.com/questions/69970147/how-do-i-resolve-the-pygraphviz-error-on-mac-os)
 
 ```
 python -m pip install \
-    --global-option=build_ext \
-    --global-option="-I$(brew --prefix graphviz)/include/" \
-    --global-option="-L$(brew --prefix graphviz)/lib/" \
-    pygraphviz
+	--global-option=build_ext \
+	--global-option="-I$(brew --prefix graphviz)/include/" \
+	--global-option="-L$(brew --prefix graphviz)/lib/" \
+	pygraphviz
+```
+
+To install on a Colab notebook, run the following shell escaped
+commands to install graphviz and its development libraries and test
+the python pygraphviz library before installing fstflowchat:
+
 ```
+# install graphviz with development libraries
+!apt install libgraphviz-dev
+
+# test pygraphviz library (used by fstflowchat
+!pip install pygraphviz
+
+# install fstflowchat
+!pip install fstflowchat
+```
+
+
+If you are interested in contributing to fstflowchat or if you want to
+use the latest code from github (potentially with breaking changes)
+you can install fstflowchat in the following ways:
+
+```
+# clone and install as an editable pip library
+git clone git+https://github.com/abecode/fstflowchat
+cd fstflowchat
+pip install -e .
+
+# pip install directly from github
+pip install git+https://github.com/abecode/fstflowchat
+```
+
 
 ## Running a demo
 
-To see a demo, run 
+To see a demo, run
 
 ```
 fstflowchat-example
 ```
 
 ## Documentation
```

