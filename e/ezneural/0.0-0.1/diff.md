# Comparing `tmp/ezneural-0.0.tar.gz` & `tmp/ezneural-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezneural-0.0.tar", last modified: Tue May  9 15:43:32 2023, max compression
+gzip compressed data, was "ezneural-0.1.tar", last modified: Tue May  9 15:57:23 2023, max compression
```

## Comparing `ezneural-0.0.tar` & `ezneural-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 15:43:32.864691 ezneural-0.0/
--rw-rw-rw-   0        0        0      206 2023-05-09 15:43:32.864691 ezneural-0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 15:43:32.855040 ezneural-0.0/ezneural/
--rw-rw-rw-   0        0        0      855 2023-05-09 15:26:35.000000 ezneural-0.0/ezneural/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:43:32.863678 ezneural-0.0/ezneural.egg-info/
--rw-rw-rw-   0        0        0      206 2023-05-09 15:43:32.000000 ezneural-0.0/ezneural.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-05-09 15:43:32.000000 ezneural-0.0/ezneural.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 15:43:32.000000 ezneural-0.0/ezneural.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-09 15:43:32.000000 ezneural-0.0/ezneural.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-05-09 15:43:32.000000 ezneural-0.0/ezneural.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 15:43:32.865678 ezneural-0.0/setup.cfg
--rw-rw-rw-   0        0        0      232 2023-05-09 14:32:03.000000 ezneural-0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:57:23.142593 ezneural-0.1/
+-rw-rw-rw-   0        0        0      320 2023-05-09 15:57:23.142593 ezneural-0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 15:57:23.139577 ezneural-0.1/ezneural/
+-rw-rw-rw-   0        0        0      855 2023-05-09 15:26:35.000000 ezneural-0.1/ezneural/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:57:23.142593 ezneural-0.1/ezneural.egg-info/
+-rw-rw-rw-   0        0        0      320 2023-05-09 15:57:23.000000 ezneural-0.1/ezneural.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-05-09 15:57:23.000000 ezneural-0.1/ezneural.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 15:57:23.000000 ezneural-0.1/ezneural.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 15:57:23.000000 ezneural-0.1/ezneural.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-09 15:57:23.000000 ezneural-0.1/ezneural.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 15:57:23.146168 ezneural-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      346 2023-05-09 15:57:07.000000 ezneural-0.1/setup.py
```

### Comparing `ezneural-0.0/ezneural/__init__.py` & `ezneural-0.1/ezneural/__init__.py`

 * *Files identical despite different names*

