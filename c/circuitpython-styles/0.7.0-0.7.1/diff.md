# Comparing `tmp/circuitpython-styles-0.7.0.tar.gz` & `tmp/circuitpython-styles-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-styles-0.7.0.tar", last modified: Tue May  9 01:53:11 2023, max compression
+gzip compressed data, was "circuitpython-styles-0.7.1.tar", last modified: Wed May 10 00:49:34 2023, max compression
```

## Comparing `circuitpython-styles-0.7.0.tar` & `circuitpython-styles-0.7.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.451164 circuitpython-styles-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 01:53:11.000000 circuitpython-styles-0.7.0/circuitpython_styles.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.455164 circuitpython-styles-0.7.0/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4414 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/index.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (123)    12511 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/styles.gif
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/docs/styles.gif.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/examples/styles_advanced_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/examples/styles_list_select_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/examples/styles_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 01:52:54.000000 circuitpython-styles-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:53:11.459164 circuitpython-styles-0.7.0/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-09 01:53:03.000000 circuitpython-styles-0.7.0/styles/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.718309 circuitpython-styles-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.710308 circuitpython-styles-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.714309 circuitpython-styles-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.714309 circuitpython-styles-0.7.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-10 00:49:34.718309 circuitpython-styles-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.714309 circuitpython-styles-0.7.1/circuitpython_styles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-10 00:49:34.000000 circuitpython-styles-0.7.1/circuitpython_styles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-10 00:49:34.000000 circuitpython-styles-0.7.1/circuitpython_styles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:49:34.000000 circuitpython-styles-0.7.1/circuitpython_styles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 00:49:34.000000 circuitpython-styles-0.7.1/circuitpython_styles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 00:49:34.000000 circuitpython-styles-0.7.1/circuitpython_styles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.714309 circuitpython-styles-0.7.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.714309 circuitpython-styles-0.7.1/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4414 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12511 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/styles.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/docs/styles.gif.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.718309 circuitpython-styles-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-10 00:49:25.000000 circuitpython-styles-0.7.1/examples/styles_advanced_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-10 00:49:25.000000 circuitpython-styles-0.7.1/examples/styles_list_select_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-10 00:49:25.000000 circuitpython-styles-0.7.1/examples/styles_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-10 00:49:25.000000 circuitpython-styles-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 00:49:12.000000 circuitpython-styles-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 00:49:34.718309 circuitpython-styles-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-10 00:49:25.000000 circuitpython-styles-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:49:34.718309 circuitpython-styles-0.7.1/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-10 00:49:25.000000 circuitpython-styles-0.7.1/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-05-10 00:49:25.000000 circuitpython-styles-0.7.1/styles/styles.py
```

### Comparing `circuitpython-styles-0.7.0/.pre-commit-config.yaml` & `circuitpython-styles-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/.pylintrc` & `circuitpython-styles-0.7.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/CODE_OF_CONDUCT.md` & `circuitpython-styles-0.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/LICENSE` & `circuitpython-styles-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-styles-0.7.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/LICENSES/MIT.txt` & `circuitpython-styles-0.7.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/LICENSES/Unlicense.txt` & `circuitpython-styles-0.7.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/PKG-INFO` & `circuitpython-styles-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-styles
-Version: 0.7.0
+Version: 0.7.1
 Summary: Dynamic style helper for CircuitPython graphical elements
 Home-page: https://github.com/jposada202020/CircuitPython_styles.git
 Author: Jose David M.
 Author-email: "Jose D. Montoya" <styles@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_styles.git
 Keywords: hardware,micropython,circuitpython,graphic,styles,widget,displayio,color,widget,themes
@@ -52,14 +52,15 @@
 * ScrollingLabel
 * ProgressBar
 * Button
 
 Other CircuitPython Widgets in the Comunity Bundle
 
 * Annotation
+* ListSelect
 
 
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython-styles-0.7.0/README.rst` & `circuitpython-styles-0.7.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 * ScrollingLabel
 * ProgressBar
 * Button
 
 Other CircuitPython Widgets in the Comunity Bundle
 
 * Annotation
+* ListSelect
 
 
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython-styles-0.7.0/circuitpython_styles.egg-info/PKG-INFO` & `circuitpython-styles-0.7.1/circuitpython_styles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-styles
-Version: 0.7.0
+Version: 0.7.1
 Summary: Dynamic style helper for CircuitPython graphical elements
 Home-page: https://github.com/jposada202020/CircuitPython_styles.git
 Author: Jose David M.
 Author-email: "Jose D. Montoya" <styles@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_styles.git
 Keywords: hardware,micropython,circuitpython,graphic,styles,widget,displayio,color,widget,themes
@@ -52,14 +52,15 @@
 * ScrollingLabel
 * ProgressBar
 * Button
 
 Other CircuitPython Widgets in the Comunity Bundle
 
 * Annotation
+* ListSelect
 
 
 
 Dependencies
 =============
 This driver depends on:
```

### Comparing `circuitpython-styles-0.7.0/circuitpython_styles.egg-info/SOURCES.txt` & `circuitpython-styles-0.7.1/circuitpython_styles.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
+docs/requirements.txt
 docs/styles.gif
 docs/styles.gif.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/styles_advanced_example.py
 examples/styles_list_select_example.py
 examples/styles_simpletest.py
```

### Comparing `circuitpython-styles-0.7.0/docs/_static/favicon.ico` & `circuitpython-styles-0.7.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/docs/conf.py` & `circuitpython-styles-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/docs/examples.rst` & `circuitpython-styles-0.7.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/docs/styles.gif` & `circuitpython-styles-0.7.1/docs/styles.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/examples/styles_advanced_example.py` & `circuitpython-styles-0.7.1/examples/styles_advanced_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/examples/styles_list_select_example.py` & `circuitpython-styles-0.7.1/examples/styles_list_select_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/pyproject.toml` & `circuitpython-styles-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-styles"
 description = "Dynamic style helper for CircuitPython graphical elements"
-version = "0.7.0"
+version = "0.7.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "styles@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_styles.git"}
 keywords = [
     "hardware",
```

### Comparing `circuitpython-styles-0.7.0/setup.py` & `circuitpython-styles-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/styles/__init__.py` & `circuitpython-styles-0.7.1/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `circuitpython-styles-0.7.0/styles/styles.py` & `circuitpython-styles-0.7.1/styles/styles.py`

 * *Files identical despite different names*

