# Comparing `tmp/csrfvalidators-0.1.8.tar.gz` & `tmp/csrfvalidators-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csrfvalidators-0.1.8.tar", last modified: Wed May 10 08:34:37 2023, max compression
+gzip compressed data, was "csrfvalidators-0.1.9.tar", last modified: Wed May 10 08:38:38 2023, max compression
```

## Comparing `csrfvalidators-0.1.8.tar` & `csrfvalidators-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:34:37.199492 csrfvalidators-0.1.8/
--rw-rw-rw-   0        0        0      132 2023-05-10 08:34:37.198492 csrfvalidators-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 08:34:37.187493 csrfvalidators-0.1.8/csrfvalidators/
--rw-rw-rw-   0        0        0        0 2023-05-08 05:18:53.000000 csrfvalidators-0.1.8/csrfvalidators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:34:37.196495 csrfvalidators-0.1.8/csrfvalidators/src/
--rw-rw-rw-   0        0        0       31 2023-04-20 06:17:06.000000 csrfvalidators-0.1.8/csrfvalidators/src/__init__.py
--rw-rw-rw-   0        0        0     3219 2023-05-10 08:24:43.000000 csrfvalidators-0.1.8/csrfvalidators/src/validator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:34:37.193492 csrfvalidators-0.1.8/csrfvalidators.egg-info/
--rw-rw-rw-   0        0        0      132 2023-05-10 08:34:37.000000 csrfvalidators-0.1.8/csrfvalidators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-10 08:34:37.000000 csrfvalidators-0.1.8/csrfvalidators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:34:37.000000 csrfvalidators-0.1.8/csrfvalidators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 08:34:37.000000 csrfvalidators-0.1.8/csrfvalidators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 08:34:37.000000 csrfvalidators-0.1.8/csrfvalidators.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 08:34:37.199492 csrfvalidators-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      283 2023-05-10 08:34:35.000000 csrfvalidators-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:38:38.448736 csrfvalidators-0.1.9/
+-rw-rw-rw-   0        0        0      132 2023-05-10 08:38:38.447737 csrfvalidators-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 08:38:38.404256 csrfvalidators-0.1.9/csrfvalidators/
+-rw-rw-rw-   0        0        0       18 2023-05-10 08:38:21.000000 csrfvalidators-0.1.9/csrfvalidators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:38:38.445825 csrfvalidators-0.1.9/csrfvalidators/src/
+-rw-rw-rw-   0        0        0       31 2023-04-20 06:17:06.000000 csrfvalidators-0.1.9/csrfvalidators/src/__init__.py
+-rw-rw-rw-   0        0        0     3219 2023-05-10 08:24:43.000000 csrfvalidators-0.1.9/csrfvalidators/src/validator.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:38:38.442218 csrfvalidators-0.1.9/csrfvalidators.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-05-10 08:38:38.000000 csrfvalidators-0.1.9/csrfvalidators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-10 08:38:38.000000 csrfvalidators-0.1.9/csrfvalidators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:38:38.000000 csrfvalidators-0.1.9/csrfvalidators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 08:38:38.000000 csrfvalidators-0.1.9/csrfvalidators.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 08:38:38.000000 csrfvalidators-0.1.9/csrfvalidators.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:38:38.448736 csrfvalidators-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      283 2023-05-10 08:38:35.000000 csrfvalidators-0.1.9/setup.py
```

### Comparing `csrfvalidators-0.1.8/csrfvalidators/src/validator.py` & `csrfvalidators-0.1.9/csrfvalidators/src/validator.py`

 * *Files identical despite different names*

