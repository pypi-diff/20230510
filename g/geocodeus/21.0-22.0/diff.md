# Comparing `tmp/geocodeus-21.0.tar.gz` & `tmp/geocodeus-22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocodeus-21.0.tar", last modified: Wed May 10 04:50:33 2023, max compression
+gzip compressed data, was "geocodeus-22.0.tar", last modified: Wed May 10 05:11:37 2023, max compression
```

## Comparing `geocodeus-21.0.tar` & `geocodeus-22.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 04:50:33.289747 geocodeus-21.0/
--rw-rw-rw-   0        0        0     1063 2023-05-10 04:50:33.288746 geocodeus-21.0/PKG-INFO
--rw-rw-rw-   0        0        0      824 2023-05-10 04:32:26.000000 geocodeus-21.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 04:50:33.287747 geocodeus-21.0/geocodeus.egg-info/
--rw-rw-rw-   0        0        0     1063 2023-05-10 04:50:33.000000 geocodeus-21.0/geocodeus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-10 04:50:33.000000 geocodeus-21.0/geocodeus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 04:50:33.000000 geocodeus-21.0/geocodeus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 04:50:33.000000 geocodeus-21.0/geocodeus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0  1202674 2023-05-10 04:49:13.000000 geocodeus-21.0/geocodeus.py
--rw-rw-rw-   0        0        0       42 2023-05-10 04:50:33.289747 geocodeus-21.0/setup.cfg
--rw-rw-rw-   0        0        0      501 2023-05-10 04:50:16.000000 geocodeus-21.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:37.837896 geocodeus-22.0/
+-rw-rw-rw-   0        0        0     2185 2023-05-10 05:11:37.837896 geocodeus-22.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1946 2023-05-10 05:11:13.000000 geocodeus-22.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:37.836897 geocodeus-22.0/geocodeus.egg-info/
+-rw-rw-rw-   0        0        0     2185 2023-05-10 05:11:37.000000 geocodeus-22.0/geocodeus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-10 05:11:37.000000 geocodeus-22.0/geocodeus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 05:11:37.000000 geocodeus-22.0/geocodeus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 05:11:37.000000 geocodeus-22.0/geocodeus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0  1202674 2023-05-10 04:49:13.000000 geocodeus-22.0/geocodeus.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 05:11:37.838895 geocodeus-22.0/setup.cfg
+-rw-rw-rw-   0        0        0      501 2023-05-10 05:11:34.000000 geocodeus-22.0/setup.py
```

### Comparing `geocodeus-21.0/geocodeus.py` & `geocodeus-22.0/geocodeus.py`

 * *Files identical despite different names*

