# Comparing `tmp/types-python-datemath-1.5.0.2.tar.gz` & `tmp/types-python-datemath-1.5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-datemath-1.5.0.2.tar", last modified: Mon Mar 27 18:25:24 2023, max compression
+gzip compressed data, was "types-python-datemath-1.5.0.3.tar", last modified: Wed May 10 15:23:44 2023, max compression
```

## Comparing `types-python-datemath-1.5.0.2.tar` & `types-python-datemath-1.5.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:24.911816 types-python-datemath-1.5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-27 18:25:24.911816 types-python-datemath-1.5.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:24.911816 types-python-datemath-1.5.0.2/datemath-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/datemath-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-27 18:21:24.000000 types-python-datemath-1.5.0.2/datemath-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-27 18:21:24.000000 types-python-datemath-1.5.0.2/datemath-stubs/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:25:24.911816 types-python-datemath-1.5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:24.911816 types-python-datemath-1.5.0.2/types_python_datemath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/types_python_datemath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/types_python_datemath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/types_python_datemath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/types_python_datemath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 18:25:24.000000 types-python-datemath-1.5.0.2/types_python_datemath.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/datemath-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/datemath-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-10 15:19:44.000000 types-python-datemath-1.5.0.3/datemath-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-10 15:19:44.000000 types-python-datemath-1.5.0.3/datemath-stubs/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/top_level.txt
```

### Comparing `types-python-datemath-1.5.0.2/CHANGELOG.md` & `types-python-datemath-1.5.0.3/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.5.0.3 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 1.5.0.2 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 1.5.0.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-python-datemath-1.5.0.2/PKG-INFO` & `types-python-datemath-1.5.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-datemath
-Version: 1.5.0.2
+Version: 1.5.0.3
 Summary: Typing stubs for python-datemath
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-datemath.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-datemath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-datemath. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-python-datemath-1.5.0.2/setup.py` & `types-python-datemath-1.5.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-datemath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-datemath. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.5.0.2",
+      version="1.5.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-datemath.md",
```

### Comparing `types-python-datemath-1.5.0.2/types_python_datemath.egg-info/PKG-INFO` & `types-python-datemath-1.5.0.3/types_python_datemath.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-datemath
-Version: 1.5.0.2
+Version: 1.5.0.3
 Summary: Typing stubs for python-datemath
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-datemath.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-datemath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-datemath. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

