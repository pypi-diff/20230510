# Comparing `tmp/odimh5-0.1.0.tar.gz` & `tmp/odimh5-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nicolas_noe/PycharmProjects/odimh5/dist/tmphcfxzon6/odimh5-0.1.0.tar", last modified: Tue Jun  8 14:30:29 2021, max compression
+gzip compressed data, was "odimh5-1.0.0.tar", last modified: Wed May 10 08:36:14 2023, max compression
```

## Comparing `odimh5-0.1.0.tar` & `odimh5-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2021-06-08 14:30:29.000000 odimh5-0.1.0/
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1056 2021-06-08 13:54:51.000000 odimh5-0.1.0/LICENSE
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1703 2021-06-08 14:30:29.000000 odimh5-0.1.0/PKG-INFO
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1077 2021-06-08 14:03:05.000000 odimh5-0.1.0/README.md
-drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2021-06-08 14:30:29.000000 odimh5-0.1.0/odimh5/
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168        0 2021-06-08 07:52:19.000000 odimh5-0.1.0/odimh5/__init__.py
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     3008 2021-06-08 12:19:53.000000 odimh5-0.1.0/odimh5/reader.py
-drwxr-xr-x   0 nicolas_noe (1863200185) 1892331168        0 2021-06-08 14:30:29.000000 odimh5-0.1.0/odimh5.egg-info/
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168     1703 2021-06-08 14:30:29.000000 odimh5-0.1.0/odimh5.egg-info/PKG-INFO
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      226 2021-06-08 14:30:29.000000 odimh5-0.1.0/odimh5.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168        1 2021-06-08 14:30:29.000000 odimh5-0.1.0/odimh5.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168       17 2021-06-08 14:30:29.000000 odimh5-0.1.0/odimh5.egg-info/requires.txt
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168        7 2021-06-08 14:30:29.000000 odimh5-0.1.0/odimh5.egg-info/top_level.txt
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      103 2021-06-08 12:30:07.000000 odimh5-0.1.0/pyproject.toml
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168       38 2021-06-08 14:30:29.000000 odimh5-0.1.0/setup.cfg
--rw-r--r--   0 nicolas_noe (1863200185) 1892331168      984 2021-06-08 13:50:43.000000 odimh5-0.1.0/setup.py
+drwxr-xr-x   0 nnoe       (501) staff       (20)        0 2023-05-10 08:36:14.195131 odimh5-1.0.0/
+-rw-r--r--   0 nnoe       (501) staff       (20)     1056 2023-05-10 08:28:45.000000 odimh5-1.0.0/LICENSE
+-rw-r--r--   0 nnoe       (501) staff       (20)       72 2023-05-10 08:36:14.195018 odimh5-1.0.0/PKG-INFO
+-rw-r--r--   0 nnoe       (501) staff       (20)     1325 2023-05-10 08:28:45.000000 odimh5-1.0.0/README.md
+drwxr-xr-x   0 nnoe       (501) staff       (20)        0 2023-05-10 08:36:14.194223 odimh5-1.0.0/odimh5/
+-rw-r--r--   0 nnoe       (501) staff       (20)        0 2023-05-10 08:28:45.000000 odimh5-1.0.0/odimh5/__init__.py
+-rw-r--r--   0 nnoe       (501) staff       (20)     3008 2023-05-10 08:28:45.000000 odimh5-1.0.0/odimh5/reader.py
+drwxr-xr-x   0 nnoe       (501) staff       (20)        0 2023-05-10 08:36:14.194726 odimh5-1.0.0/odimh5.egg-info/
+-rw-r--r--   0 nnoe       (501) staff       (20)       72 2023-05-10 08:36:14.000000 odimh5-1.0.0/odimh5.egg-info/PKG-INFO
+-rw-r--r--   0 nnoe       (501) staff       (20)      247 2023-05-10 08:36:14.000000 odimh5-1.0.0/odimh5.egg-info/SOURCES.txt
+-rw-r--r--   0 nnoe       (501) staff       (20)        1 2023-05-10 08:36:14.000000 odimh5-1.0.0/odimh5.egg-info/dependency_links.txt
+-rw-r--r--   0 nnoe       (501) staff       (20)       10 2023-05-10 08:36:14.000000 odimh5-1.0.0/odimh5.egg-info/requires.txt
+-rw-r--r--   0 nnoe       (501) staff       (20)        7 2023-05-10 08:36:14.000000 odimh5-1.0.0/odimh5.egg-info/top_level.txt
+-rw-r--r--   0 nnoe       (501) staff       (20)      103 2023-05-10 08:28:45.000000 odimh5-1.0.0/pyproject.toml
+-rw-r--r--   0 nnoe       (501) staff       (20)       38 2023-05-10 08:36:14.195161 odimh5-1.0.0/setup.cfg
+-rw-r--r--   0 nnoe       (501) staff       (20)      114 2023-05-10 08:30:20.000000 odimh5-1.0.0/setup.py
+drwxr-xr-x   0 nnoe       (501) staff       (20)        0 2023-05-10 08:36:14.194828 odimh5-1.0.0/tests/
+-rw-r--r--   0 nnoe       (501) staff       (20)     3631 2023-05-10 08:28:45.000000 odimh5-1.0.0/tests/test_reader.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `odimh5-0.1.0/LICENSE` & `odimh5-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odimh5-0.1.0/README.md` & `odimh5-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # odimh5
 
+**This package is no longer maintained. Its functionality is entirely included in [vptstools](https://github.com/enram/vptstools).**
+
+[![PyPI version](https://badge.fury.io/py/odimh5.svg)](https://badge.fury.io/py/odimh5)
 [![.github/workflows/run-tests.yaml](https://github.com/enram/odimh5/actions/workflows/run-tests.yaml/badge.svg)](https://github.com/enram/odimh5/actions/workflows/run-tests.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A simple Python package to access data in [ODIM HDF5](https://www.eumetnet.eu/wp-content/uploads/2019/01/ODIM_H5_v23.pdf) format.
 
 Limitations:
 
 - (currently) read-only
 - Python 3.7+
 
 # Tutorial
 
-## Install from PyPI
+## Install from [PyPI](https://pypi.org/project/odimh5/)
 
     $ pip install odimh5
 
 # Development instructions
 
 ## Install the local package
 
@@ -48,15 +51,12 @@
 4) Upload it to PyPI:
 
 ```
 $ python3 -m twine upload dist/*
 ```
 
 5) Tag it:
-   
+
 ```
 $ git tag v0.1.0
 $ git push origin --tags
 ```
-    
-
-
```

### Comparing `odimh5-0.1.0/odimh5/reader.py` & `odimh5-1.0.0/odimh5/reader.py`

 * *Files identical despite different names*

