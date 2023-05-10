# Comparing `tmp/moddagudu-1.8.2.tar.gz` & `tmp/moddagudu-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moddagudu-1.8.2.tar", last modified: Wed May 10 18:24:31 2023, max compression
+gzip compressed data, was "moddagudu-1.8.3.tar", last modified: Wed May 10 18:29:05 2023, max compression
```

## Comparing `moddagudu-1.8.2.tar` & `moddagudu-1.8.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 18:24:31.593225 moddagudu-1.8.2/
--rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.8.2/LICENSE.md
--rw-rw-rw-   0        0        0      131 2023-05-10 18:24:31.591685 moddagudu-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 18:24:31.547090 moddagudu-1.8.2/moddagudu/
--rw-rw-rw-   0        0        0      196 2023-05-10 18:23:35.000000 moddagudu-1.8.2/moddagudu/__init__.py
--rw-rw-rw-   0        0        0     1314 2023-05-10 18:08:06.000000 moddagudu-1.8.2/moddagudu/ep.py
--rw-rw-rw-   0        0        0      223 2023-05-10 18:23:13.000000 moddagudu-1.8.2/moddagudu/gn.py
--rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.8.2/moddagudu/mg.py
--rw-rw-rw-   0        0        0      256 2023-05-10 18:23:17.000000 moddagudu-1.8.2/moddagudu/pn.py
--rw-rw-rw-   0        0        0      284 2023-05-10 18:20:27.000000 moddagudu-1.8.2/moddagudu/sg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 18:24:31.589146 moddagudu-1.8.2/moddagudu.egg-info/
--rw-rw-rw-   0        0        0      131 2023-05-10 18:24:31.000000 moddagudu-1.8.2/moddagudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-05-10 18:24:31.000000 moddagudu-1.8.2/moddagudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 18:24:31.000000 moddagudu-1.8.2/moddagudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-10 18:24:31.000000 moddagudu-1.8.2/moddagudu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 18:24:31.000000 moddagudu-1.8.2/moddagudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 18:24:31.593225 moddagudu-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-05-10 18:23:52.000000 moddagudu-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:29:05.044332 moddagudu-1.8.3/
+-rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.8.3/LICENSE.md
+-rw-rw-rw-   0        0        0      131 2023-05-10 18:29:05.044332 moddagudu-1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 18:29:05.015313 moddagudu-1.8.3/moddagudu/
+-rw-rw-rw-   0        0        0      196 2023-05-10 18:23:35.000000 moddagudu-1.8.3/moddagudu/__init__.py
+-rw-rw-rw-   0        0        0     1314 2023-05-10 18:28:40.000000 moddagudu-1.8.3/moddagudu/ep.py
+-rw-rw-rw-   0        0        0      206 2023-05-10 18:28:03.000000 moddagudu-1.8.3/moddagudu/gn.py
+-rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.8.3/moddagudu/mg.py
+-rw-rw-rw-   0        0        0      239 2023-05-10 18:28:07.000000 moddagudu-1.8.3/moddagudu/pn.py
+-rw-rw-rw-   0        0        0      269 2023-05-10 18:28:16.000000 moddagudu-1.8.3/moddagudu/sg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:29:05.041231 moddagudu-1.8.3/moddagudu.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-05-10 18:29:04.000000 moddagudu-1.8.3/moddagudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-10 18:29:04.000000 moddagudu-1.8.3/moddagudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:29:04.000000 moddagudu-1.8.3/moddagudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-10 18:29:04.000000 moddagudu-1.8.3/moddagudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 18:29:04.000000 moddagudu-1.8.3/moddagudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:29:05.044332 moddagudu-1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      240 2023-05-10 18:28:00.000000 moddagudu-1.8.3/setup.py
```

### Comparing `moddagudu-1.8.2/LICENSE.md` & `moddagudu-1.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `moddagudu-1.8.2/moddagudu/ep.py` & `moddagudu-1.8.3/moddagudu/ep.py`

 * *Files identical despite different names*

