# Comparing `tmp/moddagudu-1.6.tar.gz` & `tmp/moddagudu-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moddagudu-1.6.tar", last modified: Wed May 10 17:56:32 2023, max compression
+gzip compressed data, was "moddagudu-1.7.tar", last modified: Wed May 10 18:03:15 2023, max compression
```

## Comparing `moddagudu-1.6.tar` & `moddagudu-1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:56:32.766453 moddagudu-1.6/
--rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.6/LICENSE.md
--rw-rw-rw-   0        0        0      129 2023-05-10 17:56:32.766453 moddagudu-1.6/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 17:56:32.731271 moddagudu-1.6/moddagudu/
--rw-rw-rw-   0        0        0      156 2023-05-10 17:46:18.000000 moddagudu-1.6/moddagudu/__init__.py
--rw-rw-rw-   0        0        0     1314 2023-05-10 17:25:17.000000 moddagudu-1.6/moddagudu/ep.py
--rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.6/moddagudu/mg.py
--rw-rw-rw-   0        0        0      273 2023-05-10 17:55:17.000000 moddagudu-1.6/moddagudu/pn.py
--rw-rw-rw-   0        0        0      279 2023-05-10 17:51:54.000000 moddagudu-1.6/moddagudu/sg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:56:32.766453 moddagudu-1.6/moddagudu.egg-info/
--rw-rw-rw-   0        0        0      129 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 17:56:32.000000 moddagudu-1.6/moddagudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 17:56:32.782099 moddagudu-1.6/setup.cfg
--rw-rw-rw-   0        0        0      238 2023-05-10 17:55:54.000000 moddagudu-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:03:15.233127 moddagudu-1.7/
+-rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.7/LICENSE.md
+-rw-rw-rw-   0        0        0      129 2023-05-10 18:03:15.217481 moddagudu-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 18:03:15.201538 moddagudu-1.7/moddagudu/
+-rw-rw-rw-   0        0        0      156 2023-05-10 17:57:52.000000 moddagudu-1.7/moddagudu/__init__.py
+-rw-rw-rw-   0        0        0     1314 2023-05-10 17:25:17.000000 moddagudu-1.7/moddagudu/ep.py
+-rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.7/moddagudu/mg.py
+-rw-rw-rw-   0        0        0      239 2023-05-10 18:02:38.000000 moddagudu-1.7/moddagudu/pn.py
+-rw-rw-rw-   0        0        0      265 2023-05-10 18:02:18.000000 moddagudu-1.7/moddagudu/sg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:03:15.217481 moddagudu-1.7/moddagudu.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-05-10 18:03:14.000000 moddagudu-1.7/moddagudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-10 18:03:15.000000 moddagudu-1.7/moddagudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:03:14.000000 moddagudu-1.7/moddagudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-10 18:03:14.000000 moddagudu-1.7/moddagudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 18:03:14.000000 moddagudu-1.7/moddagudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:03:15.233127 moddagudu-1.7/setup.cfg
+-rw-rw-rw-   0        0        0      238 2023-05-10 18:03:06.000000 moddagudu-1.7/setup.py
```

### Comparing `moddagudu-1.6/LICENSE.md` & `moddagudu-1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `moddagudu-1.6/moddagudu/ep.py` & `moddagudu-1.7/moddagudu/ep.py`

 * *Files identical despite different names*

