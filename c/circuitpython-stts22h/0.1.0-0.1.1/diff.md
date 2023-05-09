# Comparing `tmp/circuitpython-stts22h-0.1.0.tar.gz` & `tmp/circuitpython-stts22h-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stts22h-0.1.0.tar", last modified: Thu May  4 17:11:28 2023, max compression
+gzip compressed data, was "circuitpython-stts22h-0.1.1.tar", last modified: Tue May  9 23:19:50 2023, max compression
```

## Comparing `circuitpython-stts22h-0.1.0.tar` & `circuitpython-stts22h-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:28.454125 circuitpython-stts22h-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:28.450125 circuitpython-stts22h-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:28.454125 circuitpython-stts22h-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-04 17:11:28.454125 circuitpython-stts22h-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:28.454125 circuitpython-stts22h-0.1.0/circuitpython_stts22h.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-04 17:11:28.000000 circuitpython-stts22h-0.1.0/circuitpython_stts22h.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-04 17:11:28.000000 circuitpython-stts22h-0.1.0/circuitpython_stts22h.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 17:11:28.000000 circuitpython-stts22h-0.1.0/circuitpython_stts22h.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 17:11:28.000000 circuitpython-stts22h-0.1.0/circuitpython_stts22h.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 17:11:28.000000 circuitpython-stts22h-0.1.0/circuitpython_stts22h.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:28.454125 circuitpython-stts22h-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:28.454125 circuitpython-stts22h-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 17:11:28.454125 circuitpython-stts22h-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-04 17:11:19.000000 circuitpython-stts22h-0.1.0/examples/stts22h_output_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 17:11:19.000000 circuitpython-stts22h-0.1.0/examples/stts22h_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-04 17:11:19.000000 circuitpython-stts22h-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-04 17:11:04.000000 circuitpython-stts22h-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 17:11:28.454125 circuitpython-stts22h-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-04 17:11:19.000000 circuitpython-stts22h-0.1.0/stts22h.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:19:50.911958 circuitpython-stts22h-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:19:50.907958 circuitpython-stts22h-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:19:50.907958 circuitpython-stts22h-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-09 23:19:50.911958 circuitpython-stts22h-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:19:50.907958 circuitpython-stts22h-0.1.1/circuitpython_stts22h.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-09 23:19:50.000000 circuitpython-stts22h-0.1.1/circuitpython_stts22h.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-09 23:19:50.000000 circuitpython-stts22h-0.1.1/circuitpython_stts22h.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:19:50.000000 circuitpython-stts22h-0.1.1/circuitpython_stts22h.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 23:19:50.000000 circuitpython-stts22h-0.1.1/circuitpython_stts22h.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 23:19:50.000000 circuitpython-stts22h-0.1.1/circuitpython_stts22h.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:19:50.911958 circuitpython-stts22h-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:19:50.911958 circuitpython-stts22h-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:19:50.911958 circuitpython-stts22h-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 23:19:41.000000 circuitpython-stts22h-0.1.1/examples/stts22h_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 23:19:41.000000 circuitpython-stts22h-0.1.1/examples/stts22h_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-09 23:19:41.000000 circuitpython-stts22h-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-09 23:19:26.000000 circuitpython-stts22h-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 23:19:50.911958 circuitpython-stts22h-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-09 23:19:41.000000 circuitpython-stts22h-0.1.1/stts22h.py
```

### Comparing `circuitpython-stts22h-0.1.0/.github/workflows/build.yml` & `circuitpython-stts22h-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/.github/workflows/release_gh.yml` & `circuitpython-stts22h-0.1.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/.gitignore` & `circuitpython-stts22h-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/.pre-commit-config.yaml` & `circuitpython-stts22h-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/.pylintrc` & `circuitpython-stts22h-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/LICENSE` & `circuitpython-stts22h-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/PKG-INFO` & `circuitpython-stts22h-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-stts22h
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython Driver for the STTS22H Temperature Sensor
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_STTS22H
 Keywords: sensor,blinka,circuitpython,micropython,stts22h,temperature,sensor,STTS22H,driver
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-stts22h-0.1.0/README.rst` & `circuitpython-stts22h-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/circuitpython_stts22h.egg-info/PKG-INFO` & `circuitpython-stts22h-0.1.1/circuitpython_stts22h.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-stts22h
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython Driver for the STTS22H Temperature Sensor
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_STTS22H
 Keywords: sensor,blinka,circuitpython,micropython,stts22h,temperature,sensor,STTS22H,driver
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-stts22h-0.1.0/circuitpython_stts22h.egg-info/SOURCES.txt` & `circuitpython-stts22h-0.1.1/circuitpython_stts22h.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/docs/_static/Logo.png` & `circuitpython-stts22h-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/docs/_static/favicon.ico` & `circuitpython-stts22h-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/docs/conf.py` & `circuitpython-stts22h-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/examples/stts22h_output_data_rate.py` & `circuitpython-stts22h-0.1.1/examples/stts22h_output_data_rate.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stts22h-0.1.0/pyproject.toml` & `circuitpython-stts22h-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-stts22h"
 description = "CircuitPython Driver for the STTS22H Temperature Sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_STTS22H"}
 keywords = [
     "sensor",
```

### Comparing `circuitpython-stts22h-0.1.0/stts22h.py` & `circuitpython-stts22h-0.1.1/stts22h.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 try:
     from busio import I2C
 except ImportError:
     pass
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_STTS22H.git"
 
 _REG_WHOAMI = const(0x01)
 _CTRL = const(0x04)
 
 
 ODR_25_HZ = const(0b00)
```

