# Comparing `tmp/flaks_setup-0.91.tar.gz` & `tmp/flaks_setup-0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-0.91.tar", last modified: Wed May 10 13:08:26 2023, max compression
+gzip compressed data, was "flaks_setup-0.92.tar", last modified: Wed May 10 13:21:48 2023, max compression
```

## Comparing `flaks_setup-0.91.tar` & `flaks_setup-0.92.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:08:26.438198 flaks_setup-0.91/
--rw-rw-rw-   0        0        0      219 2023-05-10 13:08:26.438198 flaks_setup-0.91/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.91/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 13:08:26.439937 flaks_setup-0.91/setup.cfg
--rw-rw-rw-   0        0        0      391 2023-05-10 13:08:24.000000 flaks_setup-0.91/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:08:26.425101 flaks_setup-0.91/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:08:26.430103 flaks_setup-0.91/src/flaks_setup/
--rw-rw-rw-   0        0        0     1579 2023-05-10 13:08:19.000000 flaks_setup-0.91/src/flaks_setup/__init__.py
--rw-rw-rw-   0        0        0     1717 2023-05-10 13:00:59.000000 flaks_setup-0.91/src/flaks_setup/post_install.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:08:26.437199 flaks_setup-0.91/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      219 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:21:48.756926 flaks_setup-0.92/
+-rw-rw-rw-   0        0        0      219 2023-05-10 13:21:48.757433 flaks_setup-0.92/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.92/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 13:21:48.758439 flaks_setup-0.92/setup.cfg
+-rw-rw-rw-   0        0        0      391 2023-05-10 13:10:03.000000 flaks_setup-0.92/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:21:48.742086 flaks_setup-0.92/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:21:48.747087 flaks_setup-0.92/src/flaks_setup/
+-rw-rw-rw-   0        0        0     2197 2023-05-10 13:20:13.000000 flaks_setup-0.92/src/flaks_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:21:48.755610 flaks_setup-0.92/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/top_level.txt
```

