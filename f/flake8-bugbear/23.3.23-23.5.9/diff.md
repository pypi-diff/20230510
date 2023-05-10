# Comparing `tmp/flake8-bugbear-23.3.23.tar.gz` & `tmp/flake8-bugbear-23.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-bugbear-23.3.23.tar", last modified: Thu Mar 23 14:46:17 2023, max compression
+gzip compressed data, was "flake8-bugbear-23.5.9.tar", last modified: Tue May  9 23:58:06 2023, max compression
```

## Comparing `flake8-bugbear-23.3.23.tar` & `flake8-bugbear-23.5.9.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:46:17.355725 flake8-bugbear-23.3.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25653 2023-03-23 14:46:17.355725 flake8-bugbear-23.3.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24333 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    63839 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/bugbear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:46:17.351724 flake8-bugbear-23.3.23/flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25653 2023-03-23 14:46:17.000000 flake8-bugbear-23.3.23/flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-23 14:46:17.000000 flake8-bugbear-23.3.23/flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:46:17.000000 flake8-bugbear-23.3.23/flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-23 14:46:17.000000 flake8-bugbear-23.3.23/flake8_bugbear.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:46:17.000000 flake8-bugbear-23.3.23/flake8_bugbear.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-23 14:46:17.000000 flake8-bugbear-23.3.23/flake8_bugbear.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-23 14:46:17.000000 flake8-bugbear-23.3.23/flake8_bugbear.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-23 14:46:17.355725 flake8-bugbear-23.3.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:46:17.355725 flake8-bugbear-23.3.23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b001.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b002.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b003.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b004.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b005.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b006_b008.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b007.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b008_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b009_b010.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b011.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b012.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b013.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b014.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b015.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b016.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b017.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b018_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b018_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b018_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b019.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b020.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b021.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b022.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b023.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b024.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b025.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b026.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b027.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b028.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b029.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b030.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b031.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b032.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b901.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b902.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b902_py38.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b903.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b904.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b905_py310.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b906.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b907.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/b950.py
--rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-03-23 14:46:07.000000 flake8-bugbear-23.3.23/tests/test_bugbear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:58:06.916914 flake8-bugbear-23.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-05-09 23:58:06.916914 flake8-bugbear-23.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25062 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    65897 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/bugbear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:58:06.912913 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 23:58:06.000000 flake8-bugbear-23.5.9/flake8_bugbear.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-09 23:58:06.916914 flake8-bugbear-23.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:58:06.916914 flake8-bugbear-23.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b001.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b002.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b003.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b005.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b006_b008.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b008_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b009_b010.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b012.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b014.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b018_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b018_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b018_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b020.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b024.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b026.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b027.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b028.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b029.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b030.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b031.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b032.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b033.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b901.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b902.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b902_py38.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b903.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b904.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b905_py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b906.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b907.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b908.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/b950.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29111 2023-05-09 23:57:52.000000 flake8-bugbear-23.5.9/tests/test_bugbear.py
```

### Comparing `flake8-bugbear-23.3.23/LICENSE` & `flake8-bugbear-23.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/PKG-INFO` & `flake8-bugbear-23.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 23.3.23
+Version: 23.5.9
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -198,27 +198,29 @@
 the unpacked sequence, and this change of ordering can surprise and mislead readers.
 There was `cpython discussion of disallowing this syntax
 <https://github.com/python/cpython/issues/82741>`_, but legacy usage and parser
 limitations make it difficult.
 
 **B027**: Empty method in abstract base class, but has no abstract decorator. Consider adding @abstractmethod.
 
-**B028**: No explicit stacklevel keyword argument found. The warn method from the warnings module uses a
+**B028**: No explicit stacklevel argument found. The warn method from the warnings module uses a
 stacklevel of 1 by default. This will only show a stack trace for the line on which the warn method is called.
 It is therefore recommended to use a stacklevel of 2 or greater to provide more information to the user.
 
 **B029**: Using ``except ():`` with an empty tuple does not handle/catch anything. Add exceptions to handle.
 
 **B030**: Except handlers should only be exception classes or tuples of exception classes.
 
 **B031**: Using the generator returned from `itertools.groupby()` more than once will do nothing on the
 second usage. Save the result to a list if the result is needed multiple times.
 
 **B032**: Possible unintentional type annotation (using ``:``). Did you mean to assign (using ``=``)?
 
+**B033**: Sets should not contain duplicate items. Duplicate items will be replaced with a single item at runtime.
+
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
 enable.
@@ -253,14 +255,16 @@
 
 **B906**: ``visit_`` function with no further call to a ``visit`` function. This is often an error, and will stop the visitor from recursing into the subnodes of a visited node. Consider adding a call ``self.generic_visit(node)`` at the end of the function.
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
 
+**B908**: Contexts with exceptions assertions like ``with self.assertRaises`` or ``with pytest.raises`` should not have multiple top-level statements. Each statement should be in its own context. That way, the test ensures that the exception is raised only in the exact statement where you expect it.
+
 **B950**: Line too long. This is a pragmatic equivalent of
 ``pycodestyle``'s ``E501``: it considers "max-line-length" but only triggers
 when the value has been exceeded by **more than 10%**. ``noqa`` and ``type: ignore`` comments are ignored. You will no
 longer be forced to reformat code due to the closing parenthesis being
 one character too far to satisfy the linter. At the same time, if you do
 significantly violate the line length, you will receive a message that
 states what the actual limit is. This is inspired by Raymond Hettinger's
@@ -350,20 +354,29 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.5.9
+~~~~~~
+
+* Add B033: Detect duplicate items in sets
+* Add B908: Detect assertRauses like contexts only has top level statements that could throw
+* Add B028: Allow stacklevel to be explicitly assigned as a positional argument
+* Remove more < 3.8 checks / assertions
+
 23.3.23
 ~~~~~~~~~~
 
 * flake8-bugbear is now >= 3.8.1 project like flake8>=6.0.0
   * This has allowed some more modern AST usage cleanup and less CI running etc.
 * B030: Fix crash on certain unusual except handlers (e.g. ``except a[0].b:``)
+* Add B033: Check for duplicate items in sets.
 
 23.3.12
 ~~~~~~~~
 
 * B950: now ignores 'noqa' and 'type: ignore' comments.
 * B005: Do not flag when using the ``strip()`` method on an imported module.
 * B030: Allow calls and starred expressions in except handlers.
```

### Comparing `flake8-bugbear-23.3.23/README.rst` & `flake8-bugbear-23.5.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -169,27 +169,29 @@
 the unpacked sequence, and this change of ordering can surprise and mislead readers.
 There was `cpython discussion of disallowing this syntax
 <https://github.com/python/cpython/issues/82741>`_, but legacy usage and parser
 limitations make it difficult.
 
 **B027**: Empty method in abstract base class, but has no abstract decorator. Consider adding @abstractmethod.
 
-**B028**: No explicit stacklevel keyword argument found. The warn method from the warnings module uses a
+**B028**: No explicit stacklevel argument found. The warn method from the warnings module uses a
 stacklevel of 1 by default. This will only show a stack trace for the line on which the warn method is called.
 It is therefore recommended to use a stacklevel of 2 or greater to provide more information to the user.
 
 **B029**: Using ``except ():`` with an empty tuple does not handle/catch anything. Add exceptions to handle.
 
 **B030**: Except handlers should only be exception classes or tuples of exception classes.
 
 **B031**: Using the generator returned from `itertools.groupby()` more than once will do nothing on the
 second usage. Save the result to a list if the result is needed multiple times.
 
 **B032**: Possible unintentional type annotation (using ``:``). Did you mean to assign (using ``=``)?
 
+**B033**: Sets should not contain duplicate items. Duplicate items will be replaced with a single item at runtime.
+
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
 enable.
@@ -224,14 +226,16 @@
 
 **B906**: ``visit_`` function with no further call to a ``visit`` function. This is often an error, and will stop the visitor from recursing into the subnodes of a visited node. Consider adding a call ``self.generic_visit(node)`` at the end of the function.
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
 
+**B908**: Contexts with exceptions assertions like ``with self.assertRaises`` or ``with pytest.raises`` should not have multiple top-level statements. Each statement should be in its own context. That way, the test ensures that the exception is raised only in the exact statement where you expect it.
+
 **B950**: Line too long. This is a pragmatic equivalent of
 ``pycodestyle``'s ``E501``: it considers "max-line-length" but only triggers
 when the value has been exceeded by **more than 10%**. ``noqa`` and ``type: ignore`` comments are ignored. You will no
 longer be forced to reformat code due to the closing parenthesis being
 one character too far to satisfy the linter. At the same time, if you do
 significantly violate the line length, you will receive a message that
 states what the actual limit is. This is inspired by Raymond Hettinger's
@@ -321,20 +325,29 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.5.9
+~~~~~~
+
+* Add B033: Detect duplicate items in sets
+* Add B908: Detect assertRauses like contexts only has top level statements that could throw
+* Add B028: Allow stacklevel to be explicitly assigned as a positional argument
+* Remove more < 3.8 checks / assertions
+
 23.3.23
 ~~~~~~~~~~
 
 * flake8-bugbear is now >= 3.8.1 project like flake8>=6.0.0
   * This has allowed some more modern AST usage cleanup and less CI running etc.
 * B030: Fix crash on certain unusual except handlers (e.g. ``except a[0].b:``)
+* Add B033: Check for duplicate items in sets.
 
 23.3.12
 ~~~~~~~~
 
 * B950: now ignores 'noqa' and 'type: ignore' comments.
 * B005: Do not flag when using the ``strip()`` method on an imported module.
 * B030: Allow calls and starred expressions in except handlers.
```

### Comparing `flake8-bugbear-23.3.23/bugbear.py` & `flake8-bugbear-23.5.9/bugbear.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,37 @@
 from contextlib import suppress
 from functools import lru_cache, partial
 from keyword import iskeyword
 
 import attr
 import pycodestyle
 
-__version__ = "23.3.23"
+__version__ = "23.5.9"
 
 LOG = logging.getLogger("flake8.bugbear")
 CONTEXTFUL_NODES = (
     ast.Module,
     ast.ClassDef,
     ast.AsyncFunctionDef,
     ast.FunctionDef,
     ast.Lambda,
     ast.ListComp,
     ast.SetComp,
     ast.DictComp,
     ast.GeneratorExp,
 )
 FUNCTION_NODES = (ast.AsyncFunctionDef, ast.FunctionDef, ast.Lambda)
+B908_pytest_functions = {"raises", "warns"}
+B908_unittest_methods = {
+    "assertRaises",
+    "assertRaisesRegex",
+    "assertRaisesRegexp",
+    "assertWarns",
+    "assertWarnsRegex",
+}
 
 Context = namedtuple("Context", ["node", "stack"])
 
 
 @attr.s(hash=False)
 class BugBearChecker:
     name = "flake8-bugbear"
@@ -500,28 +508,33 @@
         self.check_for_b016(node)
         self.check_for_b904(node)
         self.generic_visit(node)
 
     def visit_With(self, node):
         self.check_for_b017(node)
         self.check_for_b022(node)
+        self.check_for_b908(node)
         self.generic_visit(node)
 
     def visit_JoinedStr(self, node):
         self.check_for_b907(node)
         self.generic_visit(node)
 
     def visit_AnnAssign(self, node):
         self.check_for_b032(node)
         self.generic_visit(node)
 
     def visit_Import(self, node):
         self.check_for_b005(node)
         self.generic_visit(node)
 
+    def visit_Set(self, node):
+        self.check_for_b033(node)
+        self.generic_visit(node)
+
     def check_for_b005(self, node):
         if isinstance(node, ast.Import):
             for name in node.names:
                 self._b005_imports.add(name.asname or name.name)
         elif isinstance(node, ast.Call):
             if node.func.attr not in B005.methods:
                 return  # method name doesn't match
@@ -1100,14 +1113,47 @@
             and item_context.func.value.id == "contextlib"
             and hasattr(item_context.func, "attr")
             and item_context.func.attr == "suppress"
             and len(item_context.args) == 0
         ):
             self.errors.append(B022(node.lineno, node.col_offset))
 
+    @staticmethod
+    def _is_assertRaises_like(node: ast.withitem) -> bool:
+        if not (
+            isinstance(node, ast.withitem)
+            and isinstance(node.context_expr, ast.Call)
+            and isinstance(node.context_expr.func, (ast.Attribute, ast.Name))
+        ):
+            return False
+        if isinstance(node.context_expr.func, ast.Name):
+            # "with raises"
+            return node.context_expr.func.id in B908_pytest_functions
+        elif isinstance(node.context_expr.func, ast.Attribute) and isinstance(
+            node.context_expr.func.value, ast.Name
+        ):
+            return (
+                # "with pytest.raises"
+                node.context_expr.func.value.id == "pytest"
+                and node.context_expr.func.attr in B908_pytest_functions
+            ) or (
+                # "with self.assertRaises"
+                node.context_expr.func.value.id == "self"
+                and node.context_expr.func.attr in B908_unittest_methods
+            )
+        else:
+            return False
+
+    def check_for_b908(self, node: ast.With):
+        if len(node.body) < 2:
+            return
+        for node_item in node.items:
+            if self._is_assertRaises_like(node_item):
+                self.errors.append(B908(node.lineno, node.col_offset))
+
     def check_for_b025(self, node):
         seen = []
         for handler in node.handlers:
             if isinstance(handler.type, (ast.Name, ast.Attribute)):
                 name = ".".join(compose_call_path(handler.type))
                 seen.append(name)
             elif isinstance(handler.type, ast.Tuple):
@@ -1170,19 +1216,14 @@
                 or (isinstance(n.func, ast.Name) and "visit" in n.func.id)
             ):
                 break
         else:
             self.errors.append(B906(node.lineno, node.col_offset))
 
     def check_for_b907(self, node: ast.JoinedStr):  # noqa: C901
-        # AST structure of strings in f-strings in 3.7 is different enough this
-        # implementation doesn't work
-        if sys.version_info <= (3, 7):
-            return  # pragma: no cover
-
         def myunparse(node: ast.AST) -> str:  # pragma: no cover
             if sys.version_info >= (3, 9):
                 return ast.unparse(node)
             if isinstance(node, ast.Name):
                 return node.id
             if isinstance(node, ast.Attribute):
                 return myunparse(node.value) + "." + node.attr
@@ -1286,14 +1327,15 @@
     def check_for_b028(self, node):
         if (
             isinstance(node.func, ast.Attribute)
             and node.func.attr == "warn"
             and isinstance(node.func.value, ast.Name)
             and node.func.value.id == "warnings"
             and not any(kw.arg == "stacklevel" for kw in node.keywords)
+            and len(node.args) < 3
         ):
             self.errors.append(B028(node.lineno, node.col_offset))
 
     def check_for_b032(self, node):
         if (
             node.value is None
             and hasattr(node.target, "value")
@@ -1304,14 +1346,22 @@
                     isinstance(node.target, ast.Attribute)
                     and node.target.value.id != "self"
                 )
             )
         ):
             self.errors.append(B032(node.lineno, node.col_offset))
 
+    def check_for_b033(self, node):
+        constants = [
+            item.value
+            for item in filter(lambda x: isinstance(x, ast.Constant), node.elts)
+        ]
+        if len(constants) != len(set(constants)):
+            self.errors.append(B033(node.lineno, node.col_offset))
+
 
 def compose_call_path(node):
     if isinstance(node, ast.Attribute):
         yield from compose_call_path(node.value)
         yield node.attr
     elif isinstance(node, ast.Call):
         yield from compose_call_path(node.func)
@@ -1670,15 +1720,15 @@
     message=(
         "B027 {} is an empty method in an abstract base class, but has no abstract"
         " decorator. Consider adding @abstractmethod."
     )
 )
 B028 = Error(
     message=(
-        "B028 No explicit stacklevel keyword argument found. The warn method from the"
+        "B028 No explicit stacklevel argument found. The warn method from the"
         " warnings module uses a stacklevel of 1 by default. This will only show a"
         " stack trace for the line on which the warn method is called."
         " It is therefore recommended to use a stacklevel of 2 or"
         " greater to provide more information to the user."
     )
 )
 B029 = Error(
@@ -1701,14 +1751,21 @@
 B032 = Error(
     message=(
         "B032 Possible unintentional type annotation (using `:`). Did you mean to"
         " assign (using `=`)?"
     )
 )
 
+B033 = Error(
+    message=(
+        "B033 Sets should not contain duplicate items. Duplicate items will be replaced"
+        " with a single item at runtime."
+    )
+)
+
 # Warnings disabled by default.
 B901 = Error(
     message=(
         "B901 Using `yield` together with `return x`. Use native "
         "`async def` coroutines or put a `# noqa` comment on this "
         "line if this was intentional."
     )
@@ -1754,11 +1811,16 @@
 
 B907 = Error(
     message=(
         "B907 {!r} is manually surrounded by quotes, consider using the `!r` conversion"
         " flag."
     )
 )
-
+B908 = Error(
+    message=(
+        "B908 assertRaises-type context should not contains more than one top-level"
+        " statement."
+    )
+)
 B950 = Error(message="B950 line too long ({} > {} characters)")
 
-disabled_by_default = ["B901", "B902", "B903", "B904", "B905", "B906", "B950"]
+disabled_by_default = ["B901", "B902", "B903", "B904", "B905", "B906", "B908", "B950"]
```

### Comparing `flake8-bugbear-23.3.23/flake8_bugbear.egg-info/PKG-INFO` & `flake8-bugbear-23.5.9/flake8_bugbear.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-bugbear
-Version: 23.3.23
+Version: 23.5.9
 Summary: A plugin for flake8 finding likely bugs and design problems in your program. Contains warnings that don't belong in pyflakes and pycodestyle.
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 Project-URL: Homepage, https://github.com/PyCQA/flake8-bugbear
 Project-URL: Change Log, https://github.com/PyCQA/flake8-bugbear#change-log
 Keywords: flake8,bugbear,bugs,pyflakes,pylint,linter,qa
 Classifier: Development Status :: 5 - Production/Stable
@@ -198,27 +198,29 @@
 the unpacked sequence, and this change of ordering can surprise and mislead readers.
 There was `cpython discussion of disallowing this syntax
 <https://github.com/python/cpython/issues/82741>`_, but legacy usage and parser
 limitations make it difficult.
 
 **B027**: Empty method in abstract base class, but has no abstract decorator. Consider adding @abstractmethod.
 
-**B028**: No explicit stacklevel keyword argument found. The warn method from the warnings module uses a
+**B028**: No explicit stacklevel argument found. The warn method from the warnings module uses a
 stacklevel of 1 by default. This will only show a stack trace for the line on which the warn method is called.
 It is therefore recommended to use a stacklevel of 2 or greater to provide more information to the user.
 
 **B029**: Using ``except ():`` with an empty tuple does not handle/catch anything. Add exceptions to handle.
 
 **B030**: Except handlers should only be exception classes or tuples of exception classes.
 
 **B031**: Using the generator returned from `itertools.groupby()` more than once will do nothing on the
 second usage. Save the result to a list if the result is needed multiple times.
 
 **B032**: Possible unintentional type annotation (using ``:``). Did you mean to assign (using ``=``)?
 
+**B033**: Sets should not contain duplicate items. Duplicate items will be replaced with a single item at runtime.
+
 Opinionated warnings
 ~~~~~~~~~~~~~~~~~~~~
 
 The following warnings are disabled by default because they are
 controversial.  They may or may not apply to you, enable them explicitly
 in your configuration if you find them useful.  Read below on how to
 enable.
@@ -253,14 +255,16 @@
 
 **B906**: ``visit_`` function with no further call to a ``visit`` function. This is often an error, and will stop the visitor from recursing into the subnodes of a visited node. Consider adding a call ``self.generic_visit(node)`` at the end of the function.
 Will only trigger on function names where the part after ``visit_`` is a valid ``ast`` type with a non-empty ``_fields`` attribute.
 This is meant to be enabled by developers writing visitors using the ``ast`` module, such as flake8 plugin writers.
 
 **B907**: Consider replacing ``f"'{foo}'"`` with ``f"{foo!r}"`` which is both easier to read and will escape quotes inside ``foo`` if that would appear. The check tries to filter out any format specs that are invalid together with ``!r``. If you're using other conversion flags then e.g. ``f"'{foo!a}'"`` can be replaced with ``f"{ascii(foo)!r}"``. Not currently implemented for python<3.8 or ``str.format()`` calls.
 
+**B908**: Contexts with exceptions assertions like ``with self.assertRaises`` or ``with pytest.raises`` should not have multiple top-level statements. Each statement should be in its own context. That way, the test ensures that the exception is raised only in the exact statement where you expect it.
+
 **B950**: Line too long. This is a pragmatic equivalent of
 ``pycodestyle``'s ``E501``: it considers "max-line-length" but only triggers
 when the value has been exceeded by **more than 10%**. ``noqa`` and ``type: ignore`` comments are ignored. You will no
 longer be forced to reformat code due to the closing parenthesis being
 one character too far to satisfy the linter. At the same time, if you do
 significantly violate the line length, you will receive a message that
 states what the actual limit is. This is inspired by Raymond Hettinger's
@@ -350,20 +354,29 @@
 
 MIT
 
 
 Change Log
 ----------
 
+23.5.9
+~~~~~~
+
+* Add B033: Detect duplicate items in sets
+* Add B908: Detect assertRauses like contexts only has top level statements that could throw
+* Add B028: Allow stacklevel to be explicitly assigned as a positional argument
+* Remove more < 3.8 checks / assertions
+
 23.3.23
 ~~~~~~~~~~
 
 * flake8-bugbear is now >= 3.8.1 project like flake8>=6.0.0
   * This has allowed some more modern AST usage cleanup and less CI running etc.
 * B030: Fix crash on certain unusual except handlers (e.g. ``except a[0].b:``)
+* Add B033: Check for duplicate items in sets.
 
 23.3.12
 ~~~~~~~~
 
 * B950: now ignores 'noqa' and 'type: ignore' comments.
 * B005: Do not flag when using the ``strip()`` method on an imported module.
 * B030: Allow calls and starred expressions in except handlers.
```

### Comparing `flake8-bugbear-23.3.23/flake8_bugbear.egg-info/SOURCES.txt` & `flake8-bugbear-23.5.9/flake8_bugbear.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -42,17 +42,19 @@
 tests/b026.py
 tests/b027.py
 tests/b028.py
 tests/b029.py
 tests/b030.py
 tests/b031.py
 tests/b032.py
+tests/b033.py
 tests/b901.py
 tests/b902.py
 tests/b902_py38.py
 tests/b903.py
 tests/b904.py
 tests/b905_py310.py
 tests/b906.py
 tests/b907.py
+tests/b908.py
 tests/b950.py
 tests/test_bugbear.py
```

### Comparing `flake8-bugbear-23.3.23/pyproject.toml` & `flake8-bugbear-23.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b001.py` & `flake8-bugbear-23.5.9/tests/b001.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b005.py` & `flake8-bugbear-23.5.9/tests/b005.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b006_b008.py` & `flake8-bugbear-23.5.9/tests/b006_b008.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b007.py` & `flake8-bugbear-23.5.9/tests/b007.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b009_b010.py` & `flake8-bugbear-23.5.9/tests/b009_b010.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b012.py` & `flake8-bugbear-23.5.9/tests/b012.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b013.py` & `flake8-bugbear-23.5.9/tests/b013.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b014.py` & `flake8-bugbear-23.5.9/tests/b014.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b017.py` & `flake8-bugbear-23.5.9/tests/b017.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b019.py` & `flake8-bugbear-23.5.9/tests/b019.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b020.py` & `flake8-bugbear-23.5.9/tests/b020.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b021.py` & `flake8-bugbear-23.5.9/tests/b021.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b023.py` & `flake8-bugbear-23.5.9/tests/b023.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b024.py` & `flake8-bugbear-23.5.9/tests/b024.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b027.py` & `flake8-bugbear-23.5.9/tests/b027.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b030.py` & `flake8-bugbear-23.5.9/tests/b030.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b031.py` & `flake8-bugbear-23.5.9/tests/b031.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b901.py` & `flake8-bugbear-23.5.9/tests/b901.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b902.py` & `flake8-bugbear-23.5.9/tests/b902.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b902_py38.py` & `flake8-bugbear-23.5.9/tests/b902_py38.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b903.py` & `flake8-bugbear-23.5.9/tests/b903.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b904.py` & `flake8-bugbear-23.5.9/tests/b904.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b906.py` & `flake8-bugbear-23.5.9/tests/b906.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b907.py` & `flake8-bugbear-23.5.9/tests/b907.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/b950.py` & `flake8-bugbear-23.5.9/tests/b950.py`

 * *Files identical despite different names*

### Comparing `flake8-bugbear-23.3.23/tests/test_bugbear.py` & `flake8-bugbear-23.5.9/tests/test_bugbear.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,21 +40,23 @@
     B026,
     B027,
     B028,
     B029,
     B030,
     B031,
     B032,
+    B033,
     B901,
     B902,
     B903,
     B904,
     B905,
     B906,
     B907,
+    B908,
     B950,
     BugBearChecker,
     BugBearVisitor,
 )
 
 
 class BugbearTestCase(unittest.TestCase):
@@ -116,25 +118,25 @@
             self.errors(
                 B006(60, 24),
                 B006(64, 29),
                 B006(68, 19),
                 B006(72, 19),
                 B006(76, 31),
                 B006(80, 25),
-                B006(85, 45 if sys.version_info >= (3, 8) else 46),
+                B006(85, 45),
                 B008(85, 60),
                 B006(89, 45),
                 B008(89, 63),
                 B006(93, 44),
                 B008(93, 59),
                 B006(97, 32),
                 B008(109, 38),
                 B008(113, 11),
                 B008(113, 31),
-                B008(117, 29 if sys.version_info >= (3, 8) else 30),
+                B008(117, 29),
                 B008(160, 29),
                 B008(164, 44),
                 B006(170, 19),
                 B008(170, 20),
                 B008(170, 30),
                 B008(176, 21),
                 B008(181, 18),
@@ -289,28 +291,25 @@
         expected = [B018(line, 0) for line in range(9, 19)]
         self.assertEqual(errors, self.errors(*expected))
 
     def test_b019(self):
         filename = Path(__file__).absolute().parent / "b019.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
-
-        # AST Decorator column location for callable decorators changes in 3.7
-        col = 5 if sys.version_info >= (3, 7) else 4
         self.assertEqual(
             errors,
             self.errors(
                 B019(73, 5),
                 B019(77, 5),
-                B019(81, col),
-                B019(85, col),
+                B019(81, 5),
+                B019(85, 5),
                 B019(89, 5),
                 B019(93, 5),
-                B019(97, col),
-                B019(101, col),
+                B019(97, 5),
+                B019(101, 5),
             ),
         )
 
     def test_b020(self):
         filename = Path(__file__).absolute().parent / "b020.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = [e for e in bbc.run() if e[2][:4] == "B020"]
@@ -426,15 +425,15 @@
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
         expected = self.errors(
             B027(13, 4, vars=("empty_1",)),
             B027(16, 4, vars=("empty_2",)),
             B027(19, 4, vars=("empty_3",)),
             B027(23, 4, vars=("empty_4",)),
-            B027(31 if sys.version_info >= (3, 8) else 30, 4, vars=("empty_5",)),
+            B027(31, 4, vars=("empty_5",)),
         )
         self.assertEqual(errors, expected)
 
     def test_b028(self):
         filename = Path(__file__).absolute().parent / "b028.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
@@ -485,15 +484,44 @@
             B032(16, 0),
             B032(17, 0),
             B032(18, 0),
             B032(19, 0),
         )
         self.assertEqual(errors, expected)
 
-    @unittest.skipIf(sys.version_info < (3, 8), "not implemented for <3.8")
+    def test_b033(self):
+        filename = Path(__file__).absolute().parent / "b033.py"
+        bbc = BugBearChecker(filename=str(filename))
+        errors = list(bbc.run())
+        expected = self.errors(
+            B033(6, 7),
+            B033(7, 7),
+            B033(8, 7),
+            B033(9, 7),
+            B033(10, 7),
+            B033(11, 7),
+            B033(12, 7),
+        )
+        self.assertEqual(errors, expected)
+
+    def test_b908(self):
+        filename = Path(__file__).absolute().parent / "b908.py"
+        bbc = BugBearChecker(filename=str(filename))
+        errors = list(bbc.run())
+        expected = self.errors(
+            B908(7, 0),
+            B908(15, 8),
+            B908(21, 8),
+            B908(27, 8),
+            B908(37, 0),
+            B908(41, 0),
+            B908(45, 0),
+        )
+        self.assertEqual(errors, expected)
+
     def test_b907(self):
         filename = Path(__file__).absolute().parent / "b907.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
         expected = self.errors(
             B907(8, 0, vars=("var",)),
             B907(9, 0, vars=("var",)),
@@ -533,15 +561,14 @@
             B907(68, 0, vars=("var",)),
         )
         self.assertEqual(errors, expected)
 
     # manual permutations to save overhead when doing >60k permutations
     # see format spec at
     # https://docs.python.org/3/library/string.html#format-specification-mini-language
-    @unittest.skipIf(sys.version_info < (3, 8), "not implemented for <3.8")
     def test_b907_format_specifier_permutations(self):
         visitor = BugBearVisitor(filename="", lines="")
 
         for fields in itertools.product(
             (None, "x"),  # fill (any character)
             (None, *"<>=^"),  # align
             (None, *"+- "),  # sign
@@ -611,15 +638,14 @@
                 B902(51, 32, vars=("*, self", "instance", "self")),
                 B902(54, 44, vars=("*, self", "instance", "self")),
                 B902(68, 17, vars=("'self'", "metaclass instance", "cls")),
                 B902(72, 20, vars=("'cls'", "metaclass class", "metacls")),
             ),
         )
 
-    @unittest.skipIf(sys.version_info < (3, 8), "requires 3.8+")
     def test_b902_py38(self):
         filename = Path(__file__).absolute().parent / "b902_py38.py"
         bbc = BugBearChecker(filename=str(filename))
         errors = list(bbc.run())
         self.assertEqual(
             errors,
             self.errors(
```

