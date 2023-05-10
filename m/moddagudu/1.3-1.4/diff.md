# Comparing `tmp/moddagudu-1.3.tar.gz` & `tmp/moddagudu-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moddagudu-1.3.tar", last modified: Wed May 10 16:58:36 2023, max compression
+gzip compressed data, was "moddagudu-1.4.tar", last modified: Wed May 10 17:21:33 2023, max compression
```

## Comparing `moddagudu-1.3.tar` & `moddagudu-1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 16:58:36.315734 moddagudu-1.3/
--rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.3/LICENSE.md
--rw-rw-rw-   0        0        0      129 2023-05-10 16:58:36.315734 moddagudu-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 16:58:36.300109 moddagudu-1.3/moddagudu/
--rw-rw-rw-   0        0        0       34 2023-05-10 16:58:15.000000 moddagudu-1.3/moddagudu/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-10 16:34:06.000000 moddagudu-1.3/moddagudu/mg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:58:36.315734 moddagudu-1.3/moddagudu.egg-info/
--rw-rw-rw-   0        0        0      129 2023-05-10 16:58:36.000000 moddagudu-1.3/moddagudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-05-10 16:58:36.000000 moddagudu-1.3/moddagudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 16:58:36.000000 moddagudu-1.3/moddagudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 16:58:36.000000 moddagudu-1.3/moddagudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 16:58:36.315734 moddagudu-1.3/setup.cfg
--rw-rw-rw-   0        0        0      174 2023-05-10 16:58:27.000000 moddagudu-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:21:33.876345 moddagudu-1.4/
+-rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.4/LICENSE.md
+-rw-rw-rw-   0        0        0      129 2023-05-10 17:21:33.874347 moddagudu-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 17:21:33.864359 moddagudu-1.4/moddagudu/
+-rw-rw-rw-   0        0        0       76 2023-05-10 17:10:53.000000 moddagudu-1.4/moddagudu/__init__.py
+-rw-rw-rw-   0        0        0     1424 2023-05-10 17:14:50.000000 moddagudu-1.4/moddagudu/mg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:21:33.873355 moddagudu-1.4/moddagudu.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 17:21:33.000000 moddagudu-1.4/moddagudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 17:21:33.877347 moddagudu-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      219 2023-05-10 17:20:08.000000 moddagudu-1.4/setup.py
```

### Comparing `moddagudu-1.3/LICENSE.md` & `moddagudu-1.4/LICENSE.md`

 * *Files identical despite different names*

