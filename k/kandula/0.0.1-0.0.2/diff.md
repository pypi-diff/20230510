# Comparing `tmp/kandula-0.0.1.tar.gz` & `tmp/kandula-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kandula-0.0.1.tar", last modified: Sat Jul  3 17:15:42 2021, max compression
+gzip compressed data, was "kandula-0.0.2.tar", max compression
```

## Comparing `kandula-0.0.1.tar` & `kandula-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
-drwxr-xr-x   0 meghdad    (501) staff       (20)        0 2021-07-03 17:15:42.396198 kandula-0.0.1/
--rw-r--r--   0 meghdad    (501) staff       (20)      247 2021-07-03 17:15:42.395909 kandula-0.0.1/PKG-INFO
-drwxr-xr-x   0 meghdad    (501) staff       (20)        0 2021-07-03 17:15:42.395566 kandula-0.0.1/kandula.egg-info/
--rw-r--r--   0 meghdad    (501) staff       (20)      247 2021-07-03 17:15:42.000000 kandula-0.0.1/kandula.egg-info/PKG-INFO
--rw-r--r--   0 meghdad    (501) staff       (20)      132 2021-07-03 17:15:42.000000 kandula-0.0.1/kandula.egg-info/SOURCES.txt
--rw-r--r--   0 meghdad    (501) staff       (20)        1 2021-07-03 17:15:42.000000 kandula-0.0.1/kandula.egg-info/dependency_links.txt
--rw-r--r--   0 meghdad    (501) staff       (20)        1 2021-07-03 17:15:42.000000 kandula-0.0.1/kandula.egg-info/top_level.txt
--rw-r--r--   0 meghdad    (501) staff       (20)       38 2021-07-03 17:15:42.396335 kandula-0.0.1/setup.cfg
--rw-r--r--   0 meghdad    (501) staff       (20)      290 2021-07-03 17:15:29.000000 kandula-0.0.1/setup.py
+-rw-r--r--   0        0        0     1074 2020-08-10 16:47:06.334488 kandula-0.0.2/LICENSE
+-rw-r--r--   0        0        0      404 2023-05-10 15:56:00.799912 kandula-0.0.2/README.rst
+-rw-r--r--   0        0        0      163 2023-05-10 12:37:45.681221 kandula-0.0.2/kandula/__init__.py
+-rw-r--r--   0        0        0     5231 2023-05-10 12:39:59.965408 kandula-0.0.2/kandula/q_learning.py
+-rw-r--r--   0        0        0     3652 2023-05-10 15:42:03.968556 kandula-0.0.2/kandula/qtable.py
+-rw-r--r--   0        0        0      600 2023-05-10 12:37:45.701938 kandula-0.0.2/kandula/steps.py
+-rw-r--r--   0        0        0      681 2023-05-10 18:47:29.716589 kandula-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 kandula-0.0.2/PKG-INFO
```

