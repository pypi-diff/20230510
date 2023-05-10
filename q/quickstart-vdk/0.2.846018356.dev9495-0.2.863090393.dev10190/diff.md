# Comparing `tmp/quickstart-vdk-0.2.846018356.dev9495.tar.gz` & `tmp/quickstart-vdk-0.2.863090393.dev10190.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.846018356.dev9495.tar", last modified: Mon Apr 24 04:20:29 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.863090393.dev10190.tar", last modified: Wed May 10 14:03:06 2023, max compression
```

## Comparing `quickstart-vdk-0.2.846018356.dev9495.tar` & `quickstart-vdk-0.2.863090393.dev10190.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 04:20:29.884997 quickstart-vdk-0.2.846018356.dev9495/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-24 04:20:29.884997 quickstart-vdk-0.2.846018356.dev9495/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-24 04:17:55.000000 quickstart-vdk-0.2.846018356.dev9495/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 04:20:29.884997 quickstart-vdk-0.2.846018356.dev9495/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-24 04:20:29.000000 quickstart-vdk-0.2.846018356.dev9495/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-24 04:20:29.000000 quickstart-vdk-0.2.846018356.dev9495/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 04:20:29.000000 quickstart-vdk-0.2.846018356.dev9495/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-04-24 04:20:29.000000 quickstart-vdk-0.2.846018356.dev9495/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-24 04:20:29.000000 quickstart-vdk-0.2.846018356.dev9495/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 04:20:29.884997 quickstart-vdk-0.2.846018356.dev9495/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-24 04:20:20.000000 quickstart-vdk-0.2.846018356.dev9495/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 04:20:29.884997 quickstart-vdk-0.2.846018356.dev9495/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-24 04:17:55.000000 quickstart-vdk-0.2.846018356.dev9495/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:03:06.150417 quickstart-vdk-0.2.863090393.dev10190/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-10 14:03:06.150417 quickstart-vdk-0.2.863090393.dev10190/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-10 14:02:38.000000 quickstart-vdk-0.2.863090393.dev10190/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:03:06.150417 quickstart-vdk-0.2.863090393.dev10190/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-05-10 14:03:05.000000 quickstart-vdk-0.2.863090393.dev10190/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-10 14:03:06.000000 quickstart-vdk-0.2.863090393.dev10190/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 14:03:05.000000 quickstart-vdk-0.2.863090393.dev10190/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-10 14:03:05.000000 quickstart-vdk-0.2.863090393.dev10190/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-10 14:03:06.000000 quickstart-vdk-0.2.863090393.dev10190/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 14:03:06.150417 quickstart-vdk-0.2.863090393.dev10190/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-10 14:02:43.000000 quickstart-vdk-0.2.863090393.dev10190/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:03:06.150417 quickstart-vdk-0.2.863090393.dev10190/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-10 14:02:38.000000 quickstart-vdk-0.2.863090393.dev10190/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.846018356.dev9495/PKG-INFO` & `quickstart-vdk-0.2.863090393.dev10190/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.846018356.dev9495
+Version: 0.2.863090393.dev10190
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.846018356.dev9495/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.863090393.dev10190/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.846018356.dev9495
+Version: 0.2.863090393.dev10190
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.846018356.dev9495/setup.py` & `quickstart-vdk-0.2.863090393.dev10190/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.846018356.dev9495"
+__version__ = "0.2.863090393.dev10190"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

