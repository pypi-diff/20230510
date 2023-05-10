# Comparing `tmp/oopt-gnpy-libyang-0.0.5.tar.gz` & `tmp/oopt-gnpy-libyang-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oopt-gnpy-libyang-0.0.5.tar", last modified: Sat Feb  4 23:54:15 2023, max compression
+gzip compressed data, was "oopt-gnpy-libyang-0.0.6.tar", last modified: Wed May 10 09:54:35 2023, max compression
```

## Comparing `oopt-gnpy-libyang-0.0.5.tar` & `oopt-gnpy-libyang-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:54:15.679123 oopt-gnpy-libyang-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:54:15.671123 oopt-gnpy-libyang-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:54:15.675123 oopt-gnpy-libyang-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-02-04 23:54:15.675123 oopt-gnpy-libyang-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/oopt-gnpy-libyang.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:54:15.675123 oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-02-04 23:54:15.000000 oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-04 23:54:15.000000 oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 23:54:15.000000 oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 23:54:15.000000 oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-04 23:54:15.000000 oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-04 23:54:15.000000 oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 23:54:15.679123 oopt-gnpy-libyang-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:54:15.675123 oopt-gnpy-libyang-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 23:54:15.675123 oopt-gnpy-libyang-0.0.5/tests/yang/
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/tests/yang/iana-hardware@2018-03-13.yang
--rw-r--r--   0 runner    (1001) docker     (123)    37062 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/tests/yang/iana-if-type@2017-01-19.yang
--rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/tests/yang/ietf-hardware@2018-03-13.yang
--rw-r--r--   0 runner    (1001) docker     (123)    39365 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/tests/yang/ietf-interfaces@2018-02-20.yang
--rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-02-04 23:52:31.000000 oopt-gnpy-libyang-0.0.5/tests/yang/ietf-ip@2018-02-22.yang
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.080817 oopt-gnpy-libyang-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/oopt-gnpy-libyang.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:54:34.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/tests/yang/
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/iana-hardware@2018-03-13.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    37062 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/iana-if-type@2017-01-19.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/ietf-hardware@2018-03-13.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    39365 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/ietf-interfaces@2018-02-20.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/ietf-ip@2018-02-22.yang
```

### Comparing `oopt-gnpy-libyang-0.0.5/.github/workflows/ci.yaml` & `oopt-gnpy-libyang-0.0.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/CMakeLists.txt` & `oopt-gnpy-libyang-0.0.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/LICENSE` & `oopt-gnpy-libyang-0.0.6/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021-2022, Telecom Infra Project
+Copyright (c) 2021-2023, Telecom Infra Project
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `oopt-gnpy-libyang-0.0.5/PKG-INFO` & `oopt-gnpy-libyang-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oopt-gnpy-libyang
-Version: 0.0.5
+Version: 0.0.6
 Summary: Opinionated Python bindings for the libyang library
 Home-page: https://github.com/Telecominfraproject/oopt-gnpy-libyang
 Download-URL: https://pypi.org/project/oopt-gnpy-libyang/
 Author: Telecom Infra Project
 Author-email: jan.kundrat@telecominfraproject.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
@@ -152,9 +152,9 @@
 
 Unlike the wheels already bundle all the required libraries, when building from source, `libyang`, `libyang-cpp` and all their dependencies will have to be installed first.
 Also, in a from-source build these won't be bundled into the resulting package.
 For an inspiration, consult our [GitHub packaging recipes](./.github/workflows/ci.yaml).
 
 ## License
 
-Copyright © 2021-2022 Telecom Infra Project and GNPy contributors.
+Copyright © 2021-2023 Telecom Infra Project and GNPy contributors.
 Licensed under the [3-clause BSD license](LICENSE).
```

### Comparing `oopt-gnpy-libyang-0.0.5/README.md` & `oopt-gnpy-libyang-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -126,9 +126,9 @@
 
 Unlike the wheels already bundle all the required libraries, when building from source, `libyang`, `libyang-cpp` and all their dependencies will have to be installed first.
 Also, in a from-source build these won't be bundled into the resulting package.
 For an inspiration, consult our [GitHub packaging recipes](./.github/workflows/ci.yaml).
 
 ## License
 
-Copyright © 2021-2022 Telecom Infra Project and GNPy contributors.
+Copyright © 2021-2023 Telecom Infra Project and GNPy contributors.
 Licensed under the [3-clause BSD license](LICENSE).
```

### Comparing `oopt-gnpy-libyang-0.0.5/oopt-gnpy-libyang.cpp` & `oopt-gnpy-libyang-0.0.6/oopt-gnpy-libyang.cpp`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/PKG-INFO` & `oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oopt-gnpy-libyang
-Version: 0.0.5
+Version: 0.0.6
 Summary: Opinionated Python bindings for the libyang library
 Home-page: https://github.com/Telecominfraproject/oopt-gnpy-libyang
 Download-URL: https://pypi.org/project/oopt-gnpy-libyang/
 Author: Telecom Infra Project
 Author-email: jan.kundrat@telecominfraproject.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
@@ -152,9 +152,9 @@
 
 Unlike the wheels already bundle all the required libraries, when building from source, `libyang`, `libyang-cpp` and all their dependencies will have to be installed first.
 Also, in a from-source build these won't be bundled into the resulting package.
 For an inspiration, consult our [GitHub packaging recipes](./.github/workflows/ci.yaml).
 
 ## License
 
-Copyright © 2021-2022 Telecom Infra Project and GNPy contributors.
+Copyright © 2021-2023 Telecom Infra Project and GNPy contributors.
 Licensed under the [3-clause BSD license](LICENSE).
```

### Comparing `oopt-gnpy-libyang-0.0.5/oopt_gnpy_libyang.egg-info/SOURCES.txt` & `oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/pyproject.toml` & `oopt-gnpy-libyang-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/setup.py` & `oopt-gnpy-libyang-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/tests/conftest.py` & `oopt-gnpy-libyang-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/tests/test_context.py` & `oopt-gnpy-libyang-0.0.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/tests/test_validation.py` & `oopt-gnpy-libyang-0.0.6/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/tests/yang/iana-hardware@2018-03-13.yang` & `oopt-gnpy-libyang-0.0.6/tests/yang/iana-hardware@2018-03-13.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/tests/yang/iana-if-type@2017-01-19.yang` & `oopt-gnpy-libyang-0.0.6/tests/yang/iana-if-type@2017-01-19.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/tests/yang/ietf-hardware@2018-03-13.yang` & `oopt-gnpy-libyang-0.0.6/tests/yang/ietf-hardware@2018-03-13.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/tests/yang/ietf-interfaces@2018-02-20.yang` & `oopt-gnpy-libyang-0.0.6/tests/yang/ietf-interfaces@2018-02-20.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.5/tests/yang/ietf-ip@2018-02-22.yang` & `oopt-gnpy-libyang-0.0.6/tests/yang/ietf-ip@2018-02-22.yang`

 * *Files identical despite different names*

