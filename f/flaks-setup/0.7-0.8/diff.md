# Comparing `tmp/flaks_setup-0.7.tar.gz` & `tmp/flaks_setup-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-0.7.tar", last modified: Wed May 10 12:52:44 2023, max compression
+gzip compressed data, was "flaks_setup-0.8.tar", last modified: Wed May 10 13:01:42 2023, max compression
```

## Comparing `flaks_setup-0.7.tar` & `flaks_setup-0.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:52:43.998902 flaks_setup-0.7/
--rw-rw-rw-   0        0        0      218 2023-05-10 12:52:43.998902 flaks_setup-0.7/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.7/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 12:52:43.999901 flaks_setup-0.7/setup.cfg
--rw-rw-rw-   0        0        0      390 2023-05-10 12:52:35.000000 flaks_setup-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:52:43.985605 flaks_setup-0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:52:43.989628 flaks_setup-0.7/src/flaks_setup/
--rw-rw-rw-   0        0        0     1717 2023-05-10 12:52:25.000000 flaks_setup-0.7/src/flaks_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:52:43.996896 flaks_setup-0.7/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      218 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:42.239068 flaks_setup-0.8/
+-rw-rw-rw-   0        0        0      218 2023-05-10 13:01:42.239068 flaks_setup-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.8/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 13:01:42.241041 flaks_setup-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      390 2023-05-10 13:01:39.000000 flaks_setup-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:42.225865 flaks_setup-0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:42.230981 flaks_setup-0.8/src/flaks_setup/
+-rw-rw-rw-   0        0        0        0 2023-05-10 13:00:57.000000 flaks_setup-0.8/src/flaks_setup/__init__.py
+-rw-rw-rw-   0        0        0     1717 2023-05-10 13:00:59.000000 flaks_setup-0.8/src/flaks_setup/post_install.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:01:42.238035 flaks_setup-0.8/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-05-10 13:01:42.000000 flaks_setup-0.8/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-10 13:01:42.000000 flaks_setup-0.8/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:01:42.000000 flaks_setup-0.8/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 13:01:42.000000 flaks_setup-0.8/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 13:01:42.000000 flaks_setup-0.8/src/flaks_setup.egg-info/top_level.txt
```

### Comparing `flaks_setup-0.7/src/flaks_setup/__init__.py` & `flaks_setup-0.8/src/flaks_setup/post_install.py`

 * *Files identical despite different names*

