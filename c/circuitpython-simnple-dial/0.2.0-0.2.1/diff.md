# Comparing `tmp/circuitpython_simnple_dial-0.2.0.tar.gz` & `tmp/circuitpython_simnple_dial-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython_simnple_dial-0.2.0.tar", last modified: Fri Apr 28 03:26:17 2023, max compression
+gzip compressed data, was "circuitpython_simnple_dial-0.2.1.tar", last modified: Wed May 10 01:01:00 2023, max compression
```

## Comparing `circuitpython_simnple_dial-0.2.0.tar` & `circuitpython_simnple_dial-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.722245 circuitpython_simnple_dial-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.706245 circuitpython_simnple_dial-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.706245 circuitpython_simnple_dial-0.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.710245 circuitpython_simnple_dial-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.710245 circuitpython_simnple_dial-0.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-28 03:26:17.722245 circuitpython_simnple_dial-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.710245 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-28 03:26:17.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.710245 circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/dial_needle.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/simple_dial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.718245 circuitpython_simnple_dial-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.718245 circuitpython_simnple_dial-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/dial.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/dial.jpg.license
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/dial.png
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/dial.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)  8781743 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/watchwatch.gif
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/docs/watchwatch.gif.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:26:17.718245 circuitpython_simnple_dial-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/examples/simple_dial_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/examples/simple_dial_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/examples/simple_dial_two_needles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-28 03:26:10.000000 circuitpython_simnple_dial-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 03:26:00.000000 circuitpython_simnple_dial-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:26:17.722245 circuitpython_simnple_dial-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.281725 circuitpython_simnple_dial-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.265725 circuitpython_simnple_dial-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.269724 circuitpython_simnple_dial-0.2.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.269724 circuitpython_simnple_dial-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.269724 circuitpython_simnple_dial-0.2.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-10 01:01:00.281725 circuitpython_simnple_dial-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.269724 circuitpython_simnple_dial-0.2.1/circuitpython_simnple_dial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-10 01:01:00.000000 circuitpython_simnple_dial-0.2.1/circuitpython_simnple_dial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-10 01:01:00.000000 circuitpython_simnple_dial-0.2.1/circuitpython_simnple_dial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 01:01:00.000000 circuitpython_simnple_dial-0.2.1/circuitpython_simnple_dial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 01:01:00.000000 circuitpython_simnple_dial-0.2.1/circuitpython_simnple_dial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 01:01:00.000000 circuitpython_simnple_dial-0.2.1/circuitpython_simnple_dial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.269724 circuitpython_simnple_dial-0.2.1/circuitpython_simple_dial/
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-10 01:00:52.000000 circuitpython_simnple_dial-0.2.1/circuitpython_simple_dial/dial_needle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-05-10 01:00:52.000000 circuitpython_simnple_dial-0.2.1/circuitpython_simple_dial/simple_dial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.277725 circuitpython_simnple_dial-0.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.281725 circuitpython_simnple_dial-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/dial.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/dial.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/dial.png
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/dial.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    74034 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/watch.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/watch.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (123)  8781743 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/watchwatch.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/docs/watchwatch.gif.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:01:00.281725 circuitpython_simnple_dial-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-10 01:00:52.000000 circuitpython_simnple_dial-0.2.1/examples/simple_dial_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-10 01:00:52.000000 circuitpython_simnple_dial-0.2.1/examples/simple_dial_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-10 01:00:52.000000 circuitpython_simnple_dial-0.2.1/examples/simple_dial_two_needles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-10 01:00:52.000000 circuitpython_simnple_dial-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 01:00:42.000000 circuitpython_simnple_dial-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 01:01:00.281725 circuitpython_simnple_dial-0.2.1/setup.cfg
```

### Comparing `circuitpython_simnple_dial-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython_simnple_dial-0.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/.pre-commit-config.yaml` & `circuitpython_simnple_dial-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/.pylintrc` & `circuitpython_simnple_dial-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/CODE_OF_CONDUCT.md` & `circuitpython_simnple_dial-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/LICENSE` & `circuitpython_simnple_dial-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/LICENSES/CC-BY-4.0.txt` & `circuitpython_simnple_dial-0.2.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/LICENSES/MIT.txt` & `circuitpython_simnple_dial-0.2.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/LICENSES/Unlicense.txt` & `circuitpython_simnple_dial-0.2.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/PKG-INFO` & `circuitpython_simnple_dial-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython_simnple_dial
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple dial widget
 Author-email: "Jose D. Montoya" <simpledial@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_simple_dial.git
 Keywords: adafruit,blinka,circuitpython,displayio,circuitpython,graphics,dial,library,plotting,clock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -38,22 +38,27 @@
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha. Main Differences:
+
     * Dial is a complete circle
     * Needle is a line. This line could be full or half
     * Needle size could be shortened using the pad option
     * Can have more than one needle.
     * Minor ticks can have their own labels
 
+
+
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/dial.png
 
+.. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/watch.jpg
+
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
```

### Comparing `circuitpython_simnple_dial-0.2.0/README.rst` & `circuitpython_simnple_dial-0.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,27 @@
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha. Main Differences:
+
     * Dial is a complete circle
     * Needle is a line. This line could be full or half
     * Needle size could be shortened using the pad option
     * Can have more than one needle.
     * Minor ticks can have their own labels
 
+
+
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/dial.png
 
+.. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/watch.jpg
+
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
```

### Comparing `circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/PKG-INFO` & `circuitpython_simnple_dial-0.2.1/circuitpython_simnple_dial.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-simnple-dial
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple dial widget
 Author-email: "Jose D. Montoya" <simpledial@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_simple_dial.git
 Keywords: adafruit,blinka,circuitpython,displayio,circuitpython,graphics,dial,library,plotting,clock
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -38,22 +38,27 @@
 
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 A dial gauge widget for displaying graphical information. Derived from Dial made by Kevin Matocha. Main Differences:
+
     * Dial is a complete circle
     * Needle is a line. This line could be full or half
     * Needle size could be shortened using the pad option
     * Can have more than one needle.
     * Minor ticks can have their own labels
 
+
+
 .. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/dial.png
 
+.. image:: https://github.com/jposada202020/CircuitPython_simple_dial/blob/main/docs/watch.jpg
+
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
```

### Comparing `circuitpython_simnple_dial-0.2.0/circuitpython_simnple_dial.egg-info/SOURCES.txt` & `circuitpython_simnple_dial-0.2.1/circuitpython_simnple_dial.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 docs/dial.jpg.license
 docs/dial.png
 docs/dial.png.license
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
+docs/watch.jpg
+docs/watch.jpg.license
 docs/watchwatch.gif
 docs/watchwatch.gif.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/simple_dial_clock.py
 examples/simple_dial_test.py
 examples/simple_dial_two_needles.py
```

### Comparing `circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/dial_needle.py` & `circuitpython_simnple_dial-0.2.1/circuitpython_simple_dial/dial_needle.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/circuitpython_simple_dial/simple_dial.py` & `circuitpython_simnple_dial-0.2.1/circuitpython_simple_dial/simple_dial.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,17 @@
         # create the dial tilegrid and append to the self Widget->Group
         self.dial_tilegrid = displayio.TileGrid(
             self.dial_bitmap, pixel_shader=self.dial_palette
         )
         self.append(self.dial_tilegrid)
 
         self._draw_circle()
+        # For CP version 8.1
+        # bitmaptools.draw_circle(self.dial_bitmap, self._dial_center[0],
+        # self._dial_center[1], self._dial_radius, 1)
 
     def _draw_circle(self):
 
         x = 0
         y = self._dial_radius
         d = 3 - 2 * self._dial_radius
```

### Comparing `circuitpython_simnple_dial-0.2.0/docs/_static/favicon.ico` & `circuitpython_simnple_dial-0.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/docs/conf.py` & `circuitpython_simnple_dial-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/docs/dial.jpg` & `circuitpython_simnple_dial-0.2.1/docs/dial.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/docs/dial.png` & `circuitpython_simnple_dial-0.2.1/docs/dial.png`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/docs/examples.rst` & `circuitpython_simnple_dial-0.2.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/docs/watchwatch.gif` & `circuitpython_simnple_dial-0.2.1/docs/watchwatch.gif`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/examples/simple_dial_clock.py` & `circuitpython_simnple_dial-0.2.1/examples/simple_dial_clock.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/examples/simple_dial_test.py` & `circuitpython_simnple_dial-0.2.1/examples/simple_dial_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/examples/simple_dial_two_needles.py` & `circuitpython_simnple_dial-0.2.1/examples/simple_dial_two_needles.py`

 * *Files identical despite different names*

### Comparing `circuitpython_simnple_dial-0.2.0/pyproject.toml` & `circuitpython_simnple_dial-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython_simnple_dial"
 description = "Simple dial widget"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "simpledial@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_simple_dial.git"}
 keywords = [
     "adafruit",
```

