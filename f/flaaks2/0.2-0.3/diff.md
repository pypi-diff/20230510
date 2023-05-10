# Comparing `tmp/flaaks2-0.2.tar.gz` & `tmp/flaaks2-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaaks2-0.2.tar", last modified: Wed May 10 08:40:06 2023, max compression
+gzip compressed data, was "flaaks2-0.3.tar", last modified: Wed May 10 08:45:52 2023, max compression
```

## Comparing `flaaks2-0.2.tar` & `flaaks2-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:40:06.822908 flaaks2-0.2/
--rw-rw-rw-   0        0        0      163 2023-05-10 08:40:06.822908 flaaks2-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 08:40:06.806909 flaaks2-0.2/flaaks/
--rw-rw-rw-   0        0        0        0 2023-04-24 12:48:40.000000 flaaks2-0.2/flaaks/__init__.py
--rw-rw-rw-   0        0        0     3834 2023-05-10 08:33:39.000000 flaaks2-0.2/flaaks/background_task.py
--rw-rw-rw-   0        0        0      265 2023-05-10 08:34:03.000000 flaaks2-0.2/flaaks/post_install.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:40:06.820909 flaaks2-0.2/flaaks2.egg-info/
--rw-rw-rw-   0        0        0      163 2023-05-10 08:40:06.000000 flaaks2-0.2/flaaks2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-05-10 08:40:06.000000 flaaks2-0.2/flaaks2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:40:06.000000 flaaks2-0.2/flaaks2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-05-10 08:40:06.000000 flaaks2-0.2/flaaks2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 08:40:06.000000 flaaks2-0.2/flaaks2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 08:40:06.000000 flaaks2-0.2/flaaks2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-05-10 08:40:06.829908 flaaks2-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-05-10 08:40:03.000000 flaaks2-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:45:52.332265 flaaks2-0.3/
+-rw-rw-rw-   0        0        0      163 2023-05-10 08:45:52.332265 flaaks2-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 08:45:52.317259 flaaks2-0.3/flaaks/
+-rw-rw-rw-   0        0        0      277 2023-05-10 08:45:14.000000 flaaks2-0.3/flaaks/__init__.py
+-rw-rw-rw-   0        0        0     3834 2023-05-10 08:33:39.000000 flaaks2-0.3/flaaks/background_task.py
+-rw-rw-rw-   0        0        0      265 2023-05-10 08:34:03.000000 flaaks2-0.3/flaaks/post_install.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:45:52.331265 flaaks2-0.3/flaaks2.egg-info/
+-rw-rw-rw-   0        0        0      163 2023-05-10 08:45:52.000000 flaaks2-0.3/flaaks2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-05-10 08:45:52.000000 flaaks2-0.3/flaaks2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:45:52.000000 flaaks2-0.3/flaaks2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-05-10 08:45:52.000000 flaaks2-0.3/flaaks2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 08:45:52.000000 flaaks2-0.3/flaaks2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 08:45:52.000000 flaaks2-0.3/flaaks2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-05-10 08:45:52.334783 flaaks2-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-05-10 08:45:50.000000 flaaks2-0.3/setup.py
```

### Comparing `flaaks2-0.2/flaaks/background_task.py` & `flaaks2-0.3/flaaks/background_task.py`

 * *Files identical despite different names*

