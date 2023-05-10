# Comparing `tmp/moddagudu-1.1.tar.gz` & `tmp/moddagudu-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moddagudu-1.1.tar", last modified: Wed May 10 16:51:22 2023, max compression
+gzip compressed data, was "moddagudu-1.2.tar", last modified: Wed May 10 16:55:54 2023, max compression
```

## Comparing `moddagudu-1.1.tar` & `moddagudu-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 16:51:22.644483 moddagudu-1.1/
--rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.1/LICENSE.md
--rw-rw-rw-   0        0        0      129 2023-05-10 16:51:22.644483 moddagudu-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 16:51:22.628853 moddagudu-1.1/moddagudu/
--rw-rw-rw-   0        0        0       31 2023-05-10 16:50:09.000000 moddagudu-1.1/moddagudu/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-10 16:34:06.000000 moddagudu-1.1/moddagudu/moddagudu.py
-drwxrwxrwx   0        0        0        0 2023-05-10 16:51:22.644483 moddagudu-1.1/moddagudu.egg-info/
--rw-rw-rw-   0        0        0      129 2023-05-10 16:51:22.000000 moddagudu-1.1/moddagudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-10 16:51:22.000000 moddagudu-1.1/moddagudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 16:51:22.000000 moddagudu-1.1/moddagudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 16:51:22.000000 moddagudu-1.1/moddagudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 16:51:22.644483 moddagudu-1.1/setup.cfg
--rw-rw-rw-   0        0        0      174 2023-05-10 16:50:50.000000 moddagudu-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:54.817840 moddagudu-1.2/
+-rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.2/LICENSE.md
+-rw-rw-rw-   0        0        0      129 2023-05-10 16:55:54.817840 moddagudu-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:54.802218 moddagudu-1.2/moddagudu/
+-rw-rw-rw-   0        0        0       24 2023-05-10 16:55:10.000000 moddagudu-1.2/moddagudu/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-10 16:34:06.000000 moddagudu-1.2/moddagudu/mg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:55:54.817840 moddagudu-1.2/moddagudu.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-05-10 16:55:54.000000 moddagudu-1.2/moddagudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-10 16:55:54.000000 moddagudu-1.2/moddagudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:55:54.000000 moddagudu-1.2/moddagudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 16:55:54.000000 moddagudu-1.2/moddagudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 16:55:54.817840 moddagudu-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      174 2023-05-10 16:55:29.000000 moddagudu-1.2/setup.py
```

### Comparing `moddagudu-1.1/LICENSE.md` & `moddagudu-1.2/LICENSE.md`

 * *Files identical despite different names*

