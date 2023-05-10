# Comparing `tmp/types-bleach-6.0.0.2.tar.gz` & `tmp/types-bleach-6.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-bleach-6.0.0.2.tar", last modified: Mon Mar 27 18:23:22 2023, max compression
+gzip compressed data, was "types-bleach-6.0.0.3.tar", last modified: Wed May 10 15:21:33 2023, max compression
```

## Comparing `types-bleach-6.0.0.2.tar` & `types-bleach-6.0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:22.666548 types-bleach-6.0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:23:22.000000 types-bleach-6.0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:23:22.000000 types-bleach-6.0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:23:22.666548 types-bleach-6.0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:22.666548 types-bleach-6.0.0.2/bleach-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-27 18:23:22.000000 types-bleach-6.0.0.2/bleach-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-27 18:21:24.000000 types-bleach-6.0.0.2/bleach-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-27 18:21:24.000000 types-bleach-6.0.0.2/bleach-stubs/callbacks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-27 18:21:24.000000 types-bleach-6.0.0.2/bleach-stubs/css_sanitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-27 18:21:24.000000 types-bleach-6.0.0.2/bleach-stubs/html5lib_shim.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-27 18:21:24.000000 types-bleach-6.0.0.2/bleach-stubs/linkifier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-27 18:21:24.000000 types-bleach-6.0.0.2/bleach-stubs/sanitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:23:22.666548 types-bleach-6.0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-27 18:23:22.000000 types-bleach-6.0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:22.666548 types-bleach-6.0.0.2/types_bleach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:23:22.000000 types-bleach-6.0.0.2/types_bleach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-27 18:23:22.000000 types-bleach-6.0.0.2/types_bleach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:23:22.000000 types-bleach-6.0.0.2/types_bleach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 18:23:22.000000 types-bleach-6.0.0.2/types_bleach.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-10 15:21:32.000000 types-bleach-6.0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:21:32.000000 types-bleach-6.0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/bleach-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:21:32.000000 types-bleach-6.0.0.3/bleach-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/callbacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/css_sanitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/html5lib_shim.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/linkifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/sanitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-10 15:21:32.000000 types-bleach-6.0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/types_bleach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:21:33.000000 types-bleach-6.0.0.3/types_bleach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 15:21:33.000000 types-bleach-6.0.0.3/types_bleach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:21:33.000000 types-bleach-6.0.0.3/types_bleach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:21:33.000000 types-bleach-6.0.0.3/types_bleach.egg-info/top_level.txt
```

### Comparing `types-bleach-6.0.0.2/CHANGELOG.md` & `types-bleach-6.0.0.3/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 6.0.0.3 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 6.0.0.2 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
 
 ## 6.0.0.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-bleach-6.0.0.2/PKG-INFO` & `types-bleach-6.0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-bleach
-Version: 6.0.0.2
+Version: 6.0.0.3
 Summary: Typing stubs for bleach
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/bleach.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `bleach`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/bleach. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-bleach-6.0.0.2/bleach-stubs/__init__.pyi` & `types-bleach-6.0.0.3/bleach-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-bleach-6.0.0.2/bleach-stubs/html5lib_shim.pyi` & `types-bleach-6.0.0.3/bleach-stubs/html5lib_shim.pyi`

 * *Files identical despite different names*

### Comparing `types-bleach-6.0.0.2/bleach-stubs/linkifier.pyi` & `types-bleach-6.0.0.3/bleach-stubs/linkifier.pyi`

 * *Files identical despite different names*

### Comparing `types-bleach-6.0.0.2/bleach-stubs/sanitizer.pyi` & `types-bleach-6.0.0.3/bleach-stubs/sanitizer.pyi`

 * *Files identical despite different names*

### Comparing `types-bleach-6.0.0.2/setup.py` & `types-bleach-6.0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `bleach`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/bleach. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="6.0.0.2",
+      version="6.0.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/bleach.md",
```

### Comparing `types-bleach-6.0.0.2/types_bleach.egg-info/PKG-INFO` & `types-bleach-6.0.0.3/types_bleach.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-bleach
-Version: 6.0.0.2
+Version: 6.0.0.3
 Summary: Typing stubs for bleach
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/bleach.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `bleach`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/bleach. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

