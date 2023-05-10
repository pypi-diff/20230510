# Comparing `tmp/types-Send2Trash-1.8.2.4.tar.gz` & `tmp/types-Send2Trash-1.8.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Send2Trash-1.8.2.4.tar", last modified: Tue Feb 21 01:27:40 2023, max compression
+gzip compressed data, was "types-Send2Trash-1.8.2.5.tar", last modified: Wed May 10 15:22:33 2023, max compression
```

## Comparing `types-Send2Trash-1.8.2.4.tar` & `types-Send2Trash-1.8.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:27:40.149564 types-Send2Trash-1.8.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-21 01:27:39.000000 types-Send2Trash-1.8.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:27:39.000000 types-Send2Trash-1.8.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 01:27:40.149564 types-Send2Trash-1.8.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:27:40.149564 types-Send2Trash-1.8.2.4/send2trash-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-21 01:27:39.000000 types-Send2Trash-1.8.2.4/send2trash-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-21 01:26:21.000000 types-Send2Trash-1.8.2.4/send2trash-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-21 01:26:21.000000 types-Send2Trash-1.8.2.4/send2trash-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-21 01:26:21.000000 types-Send2Trash-1.8.2.4/send2trash-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-21 01:26:21.000000 types-Send2Trash-1.8.2.4/send2trash-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:27:40.149564 types-Send2Trash-1.8.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-02-21 01:27:39.000000 types-Send2Trash-1.8.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:27:40.149564 types-Send2Trash-1.8.2.4/types_Send2Trash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 01:27:40.000000 types-Send2Trash-1.8.2.4/types_Send2Trash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-21 01:27:40.000000 types-Send2Trash-1.8.2.4/types_Send2Trash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:27:40.000000 types-Send2Trash-1.8.2.4/types_Send2Trash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-21 01:27:40.000000 types-Send2Trash-1.8.2.4/types_Send2Trash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:33.209047 types-Send2Trash-1.8.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-10 15:22:32.000000 types-Send2Trash-1.8.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:32.000000 types-Send2Trash-1.8.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-10 15:22:33.209047 types-Send2Trash-1.8.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:33.209047 types-Send2Trash-1.8.2.5/send2trash-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:22:32.000000 types-Send2Trash-1.8.2.5/send2trash-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-10 15:19:44.000000 types-Send2Trash-1.8.2.5/send2trash-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 15:19:44.000000 types-Send2Trash-1.8.2.5/send2trash-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-10 15:19:44.000000 types-Send2Trash-1.8.2.5/send2trash-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-10 15:19:44.000000 types-Send2Trash-1.8.2.5/send2trash-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:33.209047 types-Send2Trash-1.8.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-10 15:22:32.000000 types-Send2Trash-1.8.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:33.209047 types-Send2Trash-1.8.2.5/types_Send2Trash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-10 15:22:33.000000 types-Send2Trash-1.8.2.5/types_Send2Trash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-10 15:22:33.000000 types-Send2Trash-1.8.2.5/types_Send2Trash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:33.000000 types-Send2Trash-1.8.2.5/types_Send2Trash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:22:33.000000 types-Send2Trash-1.8.2.5/types_Send2Trash.egg-info/top_level.txt
```

### Comparing `types-Send2Trash-1.8.2.4/CHANGELOG.md` & `types-Send2Trash-1.8.2.5/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.8.2.5 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 1.8.2.4 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
 
 If you're reading about this commit from an autogenerated changelog entry, this should have no user-visible impact on how the stubs are interpreted by a type checker; it's just an internal change to how typeshed's tests work.
 
 ## 1.8.2.3 (2022-11-16)
```

### Comparing `types-Send2Trash-1.8.2.4/PKG-INFO` & `types-Send2Trash-1.8.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Send2Trash
-Version: 1.8.2.4
+Version: 1.8.2.5
 Summary: Typing stubs for Send2Trash
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Send2Trash.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Send2Trash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Send2Trash. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-Send2Trash-1.8.2.4/setup.py` & `types-Send2Trash-1.8.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Send2Trash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Send2Trash. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.8.2.4",
+      version="1.8.2.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Send2Trash.md",
```

### Comparing `types-Send2Trash-1.8.2.4/types_Send2Trash.egg-info/PKG-INFO` & `types-Send2Trash-1.8.2.5/types_Send2Trash.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Send2Trash
-Version: 1.8.2.4
+Version: 1.8.2.5
 Summary: Typing stubs for Send2Trash
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Send2Trash.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Send2Trash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Send2Trash. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

