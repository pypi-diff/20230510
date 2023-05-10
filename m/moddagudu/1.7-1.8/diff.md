# Comparing `tmp/moddagudu-1.7.tar.gz` & `tmp/moddagudu-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moddagudu-1.7.tar", last modified: Wed May 10 18:03:15 2023, max compression
+gzip compressed data, was "moddagudu-1.8.tar", last modified: Wed May 10 18:08:46 2023, max compression
```

## Comparing `moddagudu-1.7.tar` & `moddagudu-1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 18:03:15.233127 moddagudu-1.7/
--rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.7/LICENSE.md
--rw-rw-rw-   0        0        0      129 2023-05-10 18:03:15.217481 moddagudu-1.7/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 18:03:15.201538 moddagudu-1.7/moddagudu/
--rw-rw-rw-   0        0        0      156 2023-05-10 17:57:52.000000 moddagudu-1.7/moddagudu/__init__.py
--rw-rw-rw-   0        0        0     1314 2023-05-10 17:25:17.000000 moddagudu-1.7/moddagudu/ep.py
--rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.7/moddagudu/mg.py
--rw-rw-rw-   0        0        0      239 2023-05-10 18:02:38.000000 moddagudu-1.7/moddagudu/pn.py
--rw-rw-rw-   0        0        0      265 2023-05-10 18:02:18.000000 moddagudu-1.7/moddagudu/sg.py
-drwxrwxrwx   0        0        0        0 2023-05-10 18:03:15.217481 moddagudu-1.7/moddagudu.egg-info/
--rw-rw-rw-   0        0        0      129 2023-05-10 18:03:14.000000 moddagudu-1.7/moddagudu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-10 18:03:15.000000 moddagudu-1.7/moddagudu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 18:03:14.000000 moddagudu-1.7/moddagudu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-10 18:03:14.000000 moddagudu-1.7/moddagudu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 18:03:14.000000 moddagudu-1.7/moddagudu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 18:03:15.233127 moddagudu-1.7/setup.cfg
--rw-rw-rw-   0        0        0      238 2023-05-10 18:03:06.000000 moddagudu-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:08:46.143627 moddagudu-1.8/
+-rw-rw-rw-   0        0        0     1055 2023-05-10 16:33:33.000000 moddagudu-1.8/LICENSE.md
+-rw-rw-rw-   0        0        0      129 2023-05-10 18:08:46.140098 moddagudu-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-10 16:33:29.000000 moddagudu-1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 18:08:46.102494 moddagudu-1.8/moddagudu/
+-rw-rw-rw-   0        0        0      156 2023-05-10 17:57:52.000000 moddagudu-1.8/moddagudu/__init__.py
+-rw-rw-rw-   0        0        0     1314 2023-05-10 18:08:06.000000 moddagudu-1.8/moddagudu/ep.py
+-rw-rw-rw-   0        0        0      110 2023-05-10 17:25:22.000000 moddagudu-1.8/moddagudu/mg.py
+-rw-rw-rw-   0        0        0      239 2023-05-10 18:02:38.000000 moddagudu-1.8/moddagudu/pn.py
+-rw-rw-rw-   0        0        0      265 2023-05-10 18:02:18.000000 moddagudu-1.8/moddagudu/sg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:08:46.138638 moddagudu-1.8/moddagudu.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-05-10 18:08:45.000000 moddagudu-1.8/moddagudu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-10 18:08:45.000000 moddagudu-1.8/moddagudu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:08:45.000000 moddagudu-1.8/moddagudu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-10 18:08:45.000000 moddagudu-1.8/moddagudu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 18:08:45.000000 moddagudu-1.8/moddagudu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:08:46.143627 moddagudu-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      238 2023-05-10 18:08:20.000000 moddagudu-1.8/setup.py
```

### Comparing `moddagudu-1.7/LICENSE.md` & `moddagudu-1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `moddagudu-1.7/moddagudu/ep.py` & `moddagudu-1.8/moddagudu/ep.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     cov = np.cov(features)
     
     U, s, Vh = np.linalg.svd(cov)
     A = np.dot(np.dot(U, np.diag(np.sqrt(s))), U.T)
     x = np.mean(features, axis=1)
     d=np.dot(A, U.T)
     d = np.dot(np.dot(A, U.T), (x))
-    print(d)
+    return d
```

