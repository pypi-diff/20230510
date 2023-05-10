# Comparing `tmp/types-pyflakes-3.0.0.3.tar.gz` & `tmp/types-pyflakes-3.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyflakes-3.0.0.3.tar", last modified: Mon Mar 27 18:24:19 2023, max compression
+gzip compressed data, was "types-pyflakes-3.0.0.4.tar", last modified: Wed May 10 15:22:14 2023, max compression
```

## Comparing `types-pyflakes-3.0.0.3.tar` & `types-pyflakes-3.0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:19.439130 types-pyflakes-3.0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-27 18:24:18.000000 types-pyflakes-3.0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:18.000000 types-pyflakes-3.0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:24:19.439130 types-pyflakes-3.0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:19.439130 types-pyflakes-3.0.0.3/pyflakes-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-27 18:24:18.000000 types-pyflakes-3.0.0.3/pyflakes-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 18:21:24.000000 types-pyflakes-3.0.0.3/pyflakes-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-27 18:21:24.000000 types-pyflakes-3.0.0.3/pyflakes-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-03-27 18:21:24.000000 types-pyflakes-3.0.0.3/pyflakes-stubs/checker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-03-27 18:21:24.000000 types-pyflakes-3.0.0.3/pyflakes-stubs/messages.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-27 18:21:24.000000 types-pyflakes-3.0.0.3/pyflakes-stubs/reporter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:19.439130 types-pyflakes-3.0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-27 18:24:18.000000 types-pyflakes-3.0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:19.439130 types-pyflakes-3.0.0.3/types_pyflakes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:24:19.000000 types-pyflakes-3.0.0.3/types_pyflakes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-27 18:24:19.000000 types-pyflakes-3.0.0.3/types_pyflakes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:19.000000 types-pyflakes-3.0.0.3/types_pyflakes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 18:24:19.000000 types-pyflakes-3.0.0.3/types_pyflakes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:14.688607 types-pyflakes-3.0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 15:22:13.000000 types-pyflakes-3.0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:13.000000 types-pyflakes-3.0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:22:14.684607 types-pyflakes-3.0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:14.684607 types-pyflakes-3.0.0.4/pyflakes-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:22:13.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/checker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/messages.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/reporter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:14.688607 types-pyflakes-3.0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-10 15:22:13.000000 types-pyflakes-3.0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:14.684607 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:22:14.000000 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 15:22:14.000000 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:14.000000 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:22:14.000000 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/top_level.txt
```

### Comparing `types-pyflakes-3.0.0.3/CHANGELOG.md` & `types-pyflakes-3.0.0.4/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.0.0.4 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 3.0.0.3 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 3.0.0.2 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-pyflakes-3.0.0.3/PKG-INFO` & `types-pyflakes-3.0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyflakes
-Version: 3.0.0.3
+Version: 3.0.0.4
 Summary: Typing stubs for pyflakes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyflakes`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyflakes. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-pyflakes-3.0.0.3/pyflakes-stubs/api.pyi` & `types-pyflakes-3.0.0.4/pyflakes-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.0.0.3/pyflakes-stubs/checker.pyi` & `types-pyflakes-3.0.0.4/pyflakes-stubs/checker.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.0.0.3/pyflakes-stubs/messages.pyi` & `types-pyflakes-3.0.0.4/pyflakes-stubs/messages.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.0.0.3/setup.py` & `types-pyflakes-3.0.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyflakes`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyflakes. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.3",
+      version="3.0.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md",
```

### Comparing `types-pyflakes-3.0.0.3/types_pyflakes.egg-info/PKG-INFO` & `types-pyflakes-3.0.0.4/types_pyflakes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyflakes
-Version: 3.0.0.3
+Version: 3.0.0.4
 Summary: Typing stubs for pyflakes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyflakes`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyflakes. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

