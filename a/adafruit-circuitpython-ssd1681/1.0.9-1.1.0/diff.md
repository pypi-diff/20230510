# Comparing `tmp/adafruit-circuitpython-ssd1681-1.0.9.tar.gz` & `tmp/adafruit-circuitpython-ssd1681-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1681-1.0.9.tar", last modified: Tue Jun  7 16:41:19 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1681-1.1.0.tar", last modified: Wed May 10 18:24:34 2023, max compression
```

## Comparing `adafruit-circuitpython-ssd1681-1.0.9.tar` & `adafruit-circuitpython-ssd1681-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.559192 adafruit-circuitpython-ssd1681-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.551192 adafruit-circuitpython-ssd1681-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.555192 adafruit-circuitpython-ssd1681-1.0.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.555192 adafruit-circuitpython-ssd1681-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.555192 adafruit-circuitpython-ssd1681-1.0.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2022-06-07 16:41:19.559192 adafruit-circuitpython-ssd1681-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.555192 adafruit-circuitpython-ssd1681-1.0.9/adafruit_circuitpython_ssd1681.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2022-06-07 16:41:19.000000 adafruit-circuitpython-ssd1681-1.0.9/adafruit_circuitpython_ssd1681.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-06-07 16:41:19.000000 adafruit-circuitpython-ssd1681-1.0.9/adafruit_circuitpython_ssd1681.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 16:41:19.000000 adafruit-circuitpython-ssd1681-1.0.9/adafruit_circuitpython_ssd1681.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 16:41:19.000000 adafruit-circuitpython-ssd1681-1.0.9/adafruit_circuitpython_ssd1681.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-07 16:41:19.000000 adafruit-circuitpython-ssd1681-1.0.9/adafruit_circuitpython_ssd1681.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/adafruit_ssd1681.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.559192 adafruit-circuitpython-ssd1681-1.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.559192 adafruit-circuitpython-ssd1681-1.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:41:19.559192 adafruit-circuitpython-ssd1681-1.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)   360122 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/examples/ssd1681_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 16:41:19.559192 adafruit-circuitpython-ssd1681-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1899 2022-06-07 16:41:04.000000 adafruit-circuitpython-ssd1681-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.348829 adafruit-circuitpython-ssd1681-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.344829 adafruit-circuitpython-ssd1681-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.344829 adafruit-circuitpython-ssd1681-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.344829 adafruit-circuitpython-ssd1681-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.344829 adafruit-circuitpython-ssd1681-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-10 18:24:34.348829 adafruit-circuitpython-ssd1681-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.348829 adafruit-circuitpython-ssd1681-1.1.0/adafruit_circuitpython_ssd1681.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-10 18:24:34.000000 adafruit-circuitpython-ssd1681-1.1.0/adafruit_circuitpython_ssd1681.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-10 18:24:34.000000 adafruit-circuitpython-ssd1681-1.1.0/adafruit_circuitpython_ssd1681.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:24:34.000000 adafruit-circuitpython-ssd1681-1.1.0/adafruit_circuitpython_ssd1681.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 18:24:34.000000 adafruit-circuitpython-ssd1681-1.1.0/adafruit_circuitpython_ssd1681.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 18:24:34.000000 adafruit-circuitpython-ssd1681-1.1.0/adafruit_circuitpython_ssd1681.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-10 18:24:27.000000 adafruit-circuitpython-ssd1681-1.1.0/adafruit_ssd1681.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.348829 adafruit-circuitpython-ssd1681-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.348829 adafruit-circuitpython-ssd1681-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:34.348829 adafruit-circuitpython-ssd1681-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   360122 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-10 18:24:27.000000 adafruit-circuitpython-ssd1681-1.1.0/examples/ssd1681_four_corners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-10 18:24:27.000000 adafruit-circuitpython-ssd1681-1.1.0/examples/ssd1681_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-10 18:24:27.000000 adafruit-circuitpython-ssd1681-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 18:24:17.000000 adafruit-circuitpython-ssd1681-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:24:34.348829 adafruit-circuitpython-ssd1681-1.1.0/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1681-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/.gitignore` & `adafruit-circuitpython-ssd1681-1.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1681-1.1.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/.pylintrc` & `adafruit-circuitpython-ssd1681-1.1.0/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1681-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/LICENSE` & `adafruit-circuitpython-ssd1681-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1681-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1681-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1681-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/PKG-INFO` & `adafruit-circuitpython-ssd1681-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1681
-Version: 1.0.9
+Version: 1.1.0
 Summary: CircuitPython `displayio` drivers for SSD1681-based ePaper displays
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1681
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython ssd1681 displayio epd epaper
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1681
+Keywords: adafruit,blinka,circuitpython,micropython,ssd1681,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1681/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ssd1681/en/latest/
@@ -73,16 +72,16 @@
     sudo pip3 install adafruit-circuitpython-ssd1681
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ssd1681
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -140,9 +139,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1681/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/README.rst` & `adafruit-circuitpython-ssd1681-1.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     sudo pip3 install adafruit-circuitpython-ssd1681
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ssd1681
 
 Usage Example
 =============
 
 .. code-block:: python
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/adafruit_circuitpython_ssd1681.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1681-1.1.0/adafruit_circuitpython_ssd1681.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1681
-Version: 1.0.9
+Version: 1.1.0
 Summary: CircuitPython `displayio` drivers for SSD1681-based ePaper displays
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SSD1681
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython ssd1681 displayio epd epaper
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1681
+Keywords: adafruit,blinka,circuitpython,micropython,ssd1681,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ssd1681/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ssd1681/en/latest/
@@ -73,16 +72,16 @@
     sudo pip3 install adafruit-circuitpython-ssd1681
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ssd1681
 
 Usage Example
 =============
 
 .. code-block:: python
 
@@ -140,9 +139,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_SSD1681/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/adafruit_circuitpython_ssd1681.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1681-1.1.0/adafruit_circuitpython_ssd1681.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_ssd1681.py
+optional_requirements.txt
 pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ssd1681.egg-info/PKG-INFO
 adafruit_circuitpython_ssd1681.egg-info/SOURCES.txt
 adafruit_circuitpython_ssd1681.egg-info/dependency_links.txt
 adafruit_circuitpython_ssd1681.egg-info/requires.txt
@@ -30,8 +31,9 @@
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/display-ruler.bmp
 examples/display-ruler.bmp.license
+examples/ssd1681_four_corners.py
 examples/ssd1681_simpletest.py
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/adafruit_ssd1681.py` & `adafruit-circuitpython-ssd1681-1.1.0/adafruit_ssd1681.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * Adafruit CircuitPython firmware (version 5+) for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1681.git"
 
 _START_SEQUENCE = (
     b"\x12\x80\x14"  # soft reset and wait 20ms
     b"\x11\x01\x03"  # Ram data entry mode
     b"\x3C\x01\x05"  # border color
     b"\x18\x01\x80"  # Temp control
@@ -55,24 +55,26 @@
           Display width
         * *height* (``int``) --
           Display height
         * *rotation* (``int``) --
           Display rotation
     """
 
-    def __init__(self, bus, **kwargs):
+    def __init__(self, bus: displayio.FourWire, **kwargs) -> None:
         start_sequence = bytearray(_START_SEQUENCE)
 
         width = kwargs["width"]
         height = kwargs["height"]
         if "rotation" in kwargs and kwargs["rotation"] % 180 != 0:
             width, height = height, width
         start_sequence[21] = (width - 1) & 0xFF
         start_sequence[22] = ((width >> 8) - 1) & 0xFF
 
+        # RAM is actually only 200 bits high but we use 296 to match the 9 bits
+        # (and therefore two bytes) used to address height.
         super().__init__(
             bus,
             start_sequence,
             _STOP_SEQUENCE,
             **kwargs,
             ram_width=200,
             ram_height=296,
@@ -82,8 +84,9 @@
             black_bits_inverted=False,
             set_column_window_command=0x44,
             set_row_window_command=0x45,
             set_current_column_command=0x4E,
             set_current_row_command=0x4F,
             refresh_display_command=0x20,
             always_toggle_chip_select=True,
+            address_little_endian=True
         )
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1681-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/docs/conf.py` & `adafruit-circuitpython-ssd1681-1.1.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -41,15 +42,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit  CircuitPython SSD1681 Library"
-copyright = "2021 Melissa LeBlanc-Williams"
+creation_year = "2021"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Melissa LeBlanc-Williams"
 author = "Melissa LeBlanc-Williams"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/docs/index.rst` & `adafruit-circuitpython-ssd1681-1.1.0/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     :caption: Related Products
 
     Adafruit 1.54" Tri-Color eInk / ePaper 200x200 Display with SRAM <https://www.adafruit.com/product/4868>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_SSD1681/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_SSD1681/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/examples/display-ruler.bmp` & `adafruit-circuitpython-ssd1681-1.1.0/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1681-1.0.9/examples/ssd1681_simpletest.py` & `adafruit-circuitpython-ssd1681-1.1.0/examples/ssd1681_simpletest.py`

 * *Files identical despite different names*

