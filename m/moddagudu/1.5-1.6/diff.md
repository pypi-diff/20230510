# Comparing `tmp/moddagudu-1.5.tar.gz` & `tmp/moddagudu-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moddagudu-1.5.tar", last modified: Wed May 10 17:25:59 2023, max compression
+gzip compressed data, was "moddagudu-1.6.tar", last modified: Wed May 10 17:56:32 2023, max compression
```

## Comparing `moddagudu-1.5.tar` & `moddagudu-1.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:59.268175 moddagudu-1.5/
--rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.5/LICENSE.md
--rw-rw-rw-   0        0        0      129 2023-05-10 17:25:59.268175 moddagudu-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:59.236921 moddagudu-1.5/moddagudu/
--rw-rw-rw-   0        0        0       76 2023-05-10 17:25:29.000000 moddagudu-1.5/moddagudu/__init__.py
--rw-rw-rw-   0        0        0     1314 2023-05-10 17:25:17.000000 moddagudu-1.5/moddagudu/ep.py
--rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.5/moddagudu/mg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:59.268175 moddagudu-1.5/moddagudu.egg-info/
--rw-rw-rw-   0        0        0      129 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 17:25:59.000000 moddagudu-1.5/moddagudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 17:25:59.268175 moddagudu-1.5/setup.cfg
--rw-rw-rw-   0        0        0      219 2023-05-10 17:25:54.000000 moddagudu-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:56:32.766453 moddagudu-1.6/
+-rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.6/LICENSE.md
+-rw-rw-rw-   0        0        0      129 2023-05-10 17:56:32.766453 moddagudu-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 17:56:32.731271 moddagudu-1.6/moddagudu/
+-rw-rw-rw-   0        0        0      156 2023-05-10 17:46:18.000000 moddagudu-1.6/moddagudu/__init__.py
+-rw-rw-rw-   0        0        0     1314 2023-05-10 17:25:17.000000 moddagudu-1.6/moddagudu/ep.py
+-rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.6/moddagudu/mg.py
+-rw-rw-rw-   0        0        0      273 2023-05-10 17:55:17.000000 moddagudu-1.6/moddagudu/pn.py
+-rw-rw-rw-   0        0        0      279 2023-05-10 17:51:54.000000 moddagudu-1.6/moddagudu/sg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 17:56:32.766453 moddagudu-1.6/moddagudu.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 17:56:32.782099 moddagudu-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      238 2023-05-10 17:55:54.000000 moddagudu-1.6/setup.py
```

### Comparing `moddagudu-1.5/LICENSE.md` & `moddagudu-1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `moddagudu-1.5/moddagudu/ep.py` & `moddagudu-1.6/moddagudu/ep.py`

 * *Files identical despite different names*

