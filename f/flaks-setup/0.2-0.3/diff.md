# Comparing `tmp/flaks_setup-0.2.tar.gz` & `tmp/flaks_setup-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-0.2.tar", last modified: Wed May 10 11:14:56 2023, max compression
+gzip compressed data, was "flaks_setup-0.3.tar", last modified: Wed May 10 11:16:32 2023, max compression
```

## Comparing `flaks_setup-0.2.tar` & `flaks_setup-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:14:56.537273 flaks_setup-0.2/
--rw-rw-rw-   0        0        0      218 2023-05-10 11:14:56.538274 flaks_setup-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.2/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 11:14:56.538274 flaks_setup-0.2/setup.cfg
--rw-rw-rw-   0        0        0      390 2023-05-10 11:14:54.000000 flaks_setup-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:14:56.525027 flaks_setup-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:14:56.530242 flaks_setup-0.2/src/flaks_setup/
--rw-rw-rw-   0        0        0     1674 2023-05-10 11:13:48.000000 flaks_setup-0.2/src/flaks_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:14:56.536328 flaks_setup-0.2/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      218 2023-05-10 11:14:56.000000 flaks_setup-0.2/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-10 11:14:56.000000 flaks_setup-0.2/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:14:56.000000 flaks_setup-0.2/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 11:14:56.000000 flaks_setup-0.2/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 11:14:56.000000 flaks_setup-0.2/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:16:32.269617 flaks_setup-0.3/
+-rw-rw-rw-   0        0        0      218 2023-05-10 11:16:32.270617 flaks_setup-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.3/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 11:16:32.271615 flaks_setup-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      390 2023-05-10 11:16:28.000000 flaks_setup-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:16:32.255954 flaks_setup-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:16:32.261098 flaks_setup-0.3/src/flaks_setup/
+-rw-rw-rw-   0        0        0     1674 2023-05-10 11:13:48.000000 flaks_setup-0.3/src/flaks_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:16:32.268613 flaks_setup-0.3/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-05-10 11:16:32.000000 flaks_setup-0.3/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-10 11:16:32.000000 flaks_setup-0.3/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:16:32.000000 flaks_setup-0.3/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 11:16:32.000000 flaks_setup-0.3/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 11:16:32.000000 flaks_setup-0.3/src/flaks_setup.egg-info/top_level.txt
```

### Comparing `flaks_setup-0.2/src/flaks_setup/__init__.py` & `flaks_setup-0.3/src/flaks_setup/__init__.py`

 * *Files identical despite different names*

