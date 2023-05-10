# Comparing `tmp/flaks_setup-1.1.tar.gz` & `tmp/flaks_setup-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-1.1.tar", last modified: Wed May 10 14:11:39 2023, max compression
+gzip compressed data, was "flaks_setup-1.2.tar", last modified: Wed May 10 14:18:17 2023, max compression
```

## Comparing `flaks_setup-1.1.tar` & `flaks_setup-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:11:39.741848 flaks_setup-1.1/
--rw-rw-rw-   0        0        0      218 2023-05-10 14:11:39.741848 flaks_setup-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-1.1/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 14:11:39.742879 flaks_setup-1.1/setup.cfg
--rw-rw-rw-   0        0        0      390 2023-05-10 14:11:26.000000 flaks_setup-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:11:39.723891 flaks_setup-1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 14:11:39.732398 flaks_setup-1.1/src/flaks_setup/
--rw-rw-rw-   0        0        0     4461 2023-05-10 14:03:26.000000 flaks_setup-1.1/src/flaks_setup/__init__.py
--rw-rw-rw-   0        0        0       78 2023-05-10 13:30:09.000000 flaks_setup-1.1/src/flaks_setup/execute_install.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:11:39.739842 flaks_setup-1.1/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      218 2023-05-10 14:11:39.000000 flaks_setup-1.1/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-10 14:11:39.000000 flaks_setup-1.1/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:11:39.000000 flaks_setup-1.1/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 14:11:39.000000 flaks_setup-1.1/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 14:11:39.000000 flaks_setup-1.1/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 14:18:17.978746 flaks_setup-1.2/
+-rw-rw-rw-   0        0        0      218 2023-05-10 14:18:17.978746 flaks_setup-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-1.2/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 14:18:17.979752 flaks_setup-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      390 2023-05-10 14:18:13.000000 flaks_setup-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:18:17.964131 flaks_setup-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 14:18:17.970645 flaks_setup-1.2/src/flaks_setup/
+-rw-rw-rw-   0        0        0     2563 2023-05-10 14:18:05.000000 flaks_setup-1.2/src/flaks_setup/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-05-10 13:30:09.000000 flaks_setup-1.2/src/flaks_setup/execute_install.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:18:17.977644 flaks_setup-1.2/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-05-10 14:18:17.000000 flaks_setup-1.2/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-10 14:18:17.000000 flaks_setup-1.2/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:18:17.000000 flaks_setup-1.2/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 14:18:17.000000 flaks_setup-1.2/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 14:18:17.000000 flaks_setup-1.2/src/flaks_setup.egg-info/top_level.txt
```

