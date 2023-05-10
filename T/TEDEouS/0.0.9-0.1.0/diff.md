# Comparing `tmp/TEDEouS-0.0.9.tar.gz` & `tmp/TEDEouS-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TEDEouS-0.0.9.tar", last modified: Mon Mar 21 15:22:31 2022, max compression
+gzip compressed data, was "TEDEouS-0.1.0.tar", last modified: Wed May 10 20:21:07 2023, max compression
```

## Comparing `TEDEouS-0.0.9.tar` & `TEDEouS-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:22:31.471715 TEDEouS-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-03-21 15:22:31.471715 TEDEouS-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:22:31.471715 TEDEouS-0.0.9/TEDEouS/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     9355 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/finite_diffs.py
--rw-r--r--   0 runner    (1001) docker     (121)    14063 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/input_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)    16737 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3869 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/points_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    21351 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/TEDEouS/torch_rbf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:22:31.471715 TEDEouS-0.0.9/TEDEouS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-03-21 15:22:30.000000 TEDEouS-0.0.9/TEDEouS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-03-21 15:22:31.000000 TEDEouS-0.0.9/TEDEouS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 15:22:31.000000 TEDEouS-0.0.9/TEDEouS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-21 15:22:31.000000 TEDEouS-0.0.9/TEDEouS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-21 15:22:31.471715 TEDEouS-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-03-21 15:22:22.000000 TEDEouS-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:21:07.966845 TEDEouS-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-10 20:21:02.000000 TEDEouS-0.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 20:21:07.966845 TEDEouS-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-10 20:21:02.000000 TEDEouS-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:21:07.966845 TEDEouS-0.1.0/TEDEouS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 20:21:07.000000 TEDEouS-0.1.0/TEDEouS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 20:21:07.000000 TEDEouS-0.1.0/TEDEouS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:21:07.000000 TEDEouS-0.1.0/TEDEouS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:21:07.000000 TEDEouS-0.1.0/TEDEouS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:21:07.966845 TEDEouS-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-10 20:21:03.000000 TEDEouS-0.1.0/setup.py
```

### Comparing `TEDEouS-0.0.9/setup.py` & `TEDEouS-0.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-Created on Wed May 26 13:36:47 2021
 
-@author: mike_ubuntu
-"""
 
 from setuptools import setup, find_packages
 from os.path import dirname, join
 from pathlib import Path
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
-# Get the long description from the README file
-long_description = (here / 'README.md').read_text(encoding='utf-8')
 
-name = 'TEDEouS' # Add name
-version= '0.0.9' # Add version
-description = 'TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library'
-author = 'Alexander Hvatov'
-author_email = 'itmo.nss.team@gmail.com' # add email
-url = 'https://github.com/ITMO-NSS-team/torch_DE_solver'
+
 
 def read(*names, **kwargs):
     with open(
             join(dirname(__file__), *names),
             encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
@@ -36,22 +25,23 @@
 
 
 def get_requirements():
     requirements = extract_requirements('requirements.txt')
     return requirements
 
 setup(
-      name = name,
-      version = version,
-      description = description,
-      author = author,
-      author_email = author_email,
-      url = url,
-      classifiers = [      
+    name = 'TEDEouS',
+    version= '0.1.0' ,
+    description = 'TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library',
+    long_description = 'Combine power of pytorch, numerical methods and math overall to conquer and solve ALL {O,P}DEs. There are some examples to provide a little insight to an operator form',
+    author = 'Alexander Hvatov',
+    author_email = 'itmo.nss.team@gmail.com', # add email
+    classifiers = [      
               'Development Status :: 3 - Alpha',
               'Programming Language :: Python :: 3',
               'License :: OSI Approved :: MIT License',
               'Operating System :: OS Independent',
       ],
-      packages = find_packages(include = ['TEDEouS']), 
+      packages = find_packages(include = ['tedeous']), 
+      include_package_data = True,                               
       python_requires =' >=3.8'
       )
```

