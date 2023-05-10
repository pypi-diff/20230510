# Comparing `tmp/types-flake8-rst-docstrings-0.3.0.1.tar.gz` & `tmp/types-flake8-rst-docstrings-0.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-rst-docstrings-0.3.0.1.tar", last modified: Tue Feb 21 01:28:40 2023, max compression
+gzip compressed data, was "types-flake8-rst-docstrings-0.3.0.2.tar", last modified: Wed May 10 15:21:00 2023, max compression
```

## Comparing `types-flake8-rst-docstrings-0.3.0.1.tar` & `types-flake8-rst-docstrings-0.3.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:40.510388 types-flake8-rst-docstrings-0.3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-02-21 01:28:39.000000 types-flake8-rst-docstrings-0.3.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:28:39.000000 types-flake8-rst-docstrings-0.3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-21 01:28:40.510388 types-flake8-rst-docstrings-0.3.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:40.510388 types-flake8-rst-docstrings-0.3.0.1/flake8_rst_docstrings-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-21 01:28:39.000000 types-flake8-rst-docstrings-0.3.0.1/flake8_rst_docstrings-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-21 01:28:39.000000 types-flake8-rst-docstrings-0.3.0.1/flake8_rst_docstrings-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:28:40.510388 types-flake8-rst-docstrings-0.3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-21 01:28:39.000000 types-flake8-rst-docstrings-0.3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:28:40.510388 types-flake8-rst-docstrings-0.3.0.1/types_flake8_rst_docstrings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-21 01:28:40.000000 types-flake8-rst-docstrings-0.3.0.1/types_flake8_rst_docstrings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-21 01:28:40.000000 types-flake8-rst-docstrings-0.3.0.1/types_flake8_rst_docstrings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:28:40.000000 types-flake8-rst-docstrings-0.3.0.1/types_flake8_rst_docstrings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-21 01:28:40.000000 types-flake8-rst-docstrings-0.3.0.1/types_flake8_rst_docstrings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:00.462865 types-flake8-rst-docstrings-0.3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-10 15:20:59.000000 types-flake8-rst-docstrings-0.3.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:20:59.000000 types-flake8-rst-docstrings-0.3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-10 15:21:00.462865 types-flake8-rst-docstrings-0.3.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:00.458865 types-flake8-rst-docstrings-0.3.0.2/flake8_rst_docstrings-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:20:59.000000 types-flake8-rst-docstrings-0.3.0.2/flake8_rst_docstrings-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-10 15:20:59.000000 types-flake8-rst-docstrings-0.3.0.2/flake8_rst_docstrings-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:21:00.462865 types-flake8-rst-docstrings-0.3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-10 15:20:59.000000 types-flake8-rst-docstrings-0.3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:00.462865 types-flake8-rst-docstrings-0.3.0.2/types_flake8_rst_docstrings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-10 15:21:00.000000 types-flake8-rst-docstrings-0.3.0.2/types_flake8_rst_docstrings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-10 15:21:00.000000 types-flake8-rst-docstrings-0.3.0.2/types_flake8_rst_docstrings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:21:00.000000 types-flake8-rst-docstrings-0.3.0.2/types_flake8_rst_docstrings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 15:21:00.000000 types-flake8-rst-docstrings-0.3.0.2/types_flake8_rst_docstrings.egg-info/top_level.txt
```

### Comparing `types-flake8-rst-docstrings-0.3.0.1/CHANGELOG.md` & `types-flake8-rst-docstrings-0.3.0.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.3.0.2 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 0.3.0.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
 
 If you're reading about this commit from an autogenerated changelog entry, this should have no user-visible impact on how the stubs are interpreted by a type checker; it's just an internal change to how typeshed's tests work.
 
 ## 0.3.0.0 (2022-11-17)
```

### Comparing `types-flake8-rst-docstrings-0.3.0.1/PKG-INFO` & `types-flake8-rst-docstrings-0.3.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-rst-docstrings
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: Typing stubs for flake8-rst-docstrings
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-rst-docstrings.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-rst-docstrings`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-rst-docstrings. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-flake8-rst-docstrings-0.3.0.1/flake8_rst_docstrings-stubs/__init__.pyi` & `types-flake8-rst-docstrings-0.3.0.2/flake8_rst_docstrings-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-rst-docstrings-0.3.0.1/setup.py` & `types-flake8-rst-docstrings-0.3.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-rst-docstrings`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-rst-docstrings. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.3.0.1",
+      version="0.3.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-rst-docstrings.md",
```

### Comparing `types-flake8-rst-docstrings-0.3.0.1/types_flake8_rst_docstrings.egg-info/PKG-INFO` & `types-flake8-rst-docstrings-0.3.0.2/types_flake8_rst_docstrings.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-rst-docstrings
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: Typing stubs for flake8-rst-docstrings
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-rst-docstrings.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-rst-docstrings`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-rst-docstrings. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

