# Comparing `tmp/pywnp-1.1.1.tar.gz` & `tmp/pywnp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywnp-1.1.1.tar", last modified: Fri Apr  7 10:53:12 2023, max compression
+gzip compressed data, was "pywnp-2.0.0.tar", last modified: Wed May 10 12:50:25 2023, max compression
```

## Comparing `pywnp-1.1.1.tar` & `pywnp-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 10:53:12.688375 pywnp-1.1.1/
--rw-rw-rw-   0        0        0     1060 2023-03-20 18:31:19.000000 pywnp-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     5353 2023-04-07 10:53:12.687376 pywnp-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3627 2023-03-30 12:26:36.000000 pywnp-1.1.1/README.md
--rw-rw-rw-   0        0        0      669 2023-04-07 10:52:53.000000 pywnp-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 10:53:12.688375 pywnp-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-07 10:53:12.669345 pywnp-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 10:53:12.671860 pywnp-1.1.1/src/pywnp/
--rw-rw-rw-   0        0        0       27 2023-03-20 19:19:07.000000 pywnp-1.1.1/src/pywnp/__init__.py
--rw-rw-rw-   0        0        0    10531 2023-04-07 09:23:15.000000 pywnp-1.1.1/src/pywnp/pywnp.py
-drwxrwxrwx   0        0        0        0 2023-04-07 10:53:12.687376 pywnp-1.1.1/src/pywnp.egg-info/
--rw-rw-rw-   0        0        0     5353 2023-04-07 10:53:12.000000 pywnp-1.1.1/src/pywnp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-07 10:53:12.000000 pywnp-1.1.1/src/pywnp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 10:53:12.000000 pywnp-1.1.1/src/pywnp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-07 10:53:12.000000 pywnp-1.1.1/src/pywnp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-07 10:53:12.000000 pywnp-1.1.1/src/pywnp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:50:25.276545 pywnp-2.0.0/
+-rw-rw-rw-   0        0        0     1060 2023-04-26 13:11:28.000000 pywnp-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     6632 2023-05-10 12:50:25.276545 pywnp-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4908 2023-05-10 12:49:48.000000 pywnp-2.0.0/README.md
+-rw-rw-rw-   0        0        0      705 2023-05-10 12:48:33.000000 pywnp-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:50:25.276545 pywnp-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 12:50:25.254595 pywnp-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:50:25.257596 pywnp-2.0.0/src/pywnp/
+-rw-rw-rw-   0        0        0       27 2023-05-08 22:50:56.000000 pywnp-2.0.0/src/pywnp/__init__.py
+-rw-rw-rw-   0        0        0    30285 2023-05-09 14:32:57.000000 pywnp-2.0.0/src/pywnp/pywnp.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:50:25.275543 pywnp-2.0.0/src/pywnp.egg-info/
+-rw-rw-rw-   0        0        0     6632 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/top_level.txt
```

### Comparing `pywnp-1.1.1/LICENSE` & `pywnp-2.0.0/LICENSE`

 * *Files identical despite different names*

