# Comparing `tmp/types-flake8-bugbear-23.3.23.0.tar.gz` & `tmp/types-flake8-bugbear-23.5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-bugbear-23.3.23.0.tar", last modified: Fri Mar 24 01:15:45 2023, max compression
+gzip compressed data, was "types-flake8-bugbear-23.5.9.0.tar", last modified: Wed May 10 06:19:12 2023, max compression
```

## Comparing `types-flake8-bugbear-23.3.23.0.tar` & `types-flake8-bugbear-23.5.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:15:45.434550 types-flake8-bugbear-23.3.23.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-24 01:15:44.000000 types-flake8-bugbear-23.3.23.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-24 01:15:44.000000 types-flake8-bugbear-23.3.23.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-24 01:15:45.434550 types-flake8-bugbear-23.3.23.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:15:45.434550 types-flake8-bugbear-23.3.23.0/bugbear-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-24 01:15:44.000000 types-flake8-bugbear-23.3.23.0/bugbear-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-24 01:15:44.000000 types-flake8-bugbear-23.3.23.0/bugbear-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 01:15:45.434550 types-flake8-bugbear-23.3.23.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-24 01:15:44.000000 types-flake8-bugbear-23.3.23.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 01:15:45.434550 types-flake8-bugbear-23.3.23.0/types_flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-24 01:15:45.000000 types-flake8-bugbear-23.3.23.0/types_flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-24 01:15:45.000000 types-flake8-bugbear-23.3.23.0/types_flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 01:15:45.000000 types-flake8-bugbear-23.3.23.0/types_flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-24 01:15:45.000000 types-flake8-bugbear-23.3.23.0/types_flake8_bugbear.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:19:12.270510 types-flake8-bugbear-23.5.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-10 06:19:08.000000 types-flake8-bugbear-23.5.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 06:19:08.000000 types-flake8-bugbear-23.5.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 06:19:12.270510 types-flake8-bugbear-23.5.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:19:12.270510 types-flake8-bugbear-23.5.9.0/bugbear-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 06:19:08.000000 types-flake8-bugbear-23.5.9.0/bugbear-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-10 06:19:08.000000 types-flake8-bugbear-23.5.9.0/bugbear-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 06:19:12.270510 types-flake8-bugbear-23.5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-10 06:19:08.000000 types-flake8-bugbear-23.5.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:19:12.270510 types-flake8-bugbear-23.5.9.0/types_flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 06:19:12.000000 types-flake8-bugbear-23.5.9.0/types_flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-10 06:19:12.000000 types-flake8-bugbear-23.5.9.0/types_flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 06:19:12.000000 types-flake8-bugbear-23.5.9.0/types_flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 06:19:12.000000 types-flake8-bugbear-23.5.9.0/types_flake8_bugbear.egg-info/top_level.txt
```

### Comparing `types-flake8-bugbear-23.3.23.0/CHANGELOG.md` & `types-flake8-bugbear-23.5.9.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+## 23.5.9.0 (2023-05-10)
+
+[stubsabot] Bump flake8-bugbear to 23.5.9 (#10165)
+
+Release: https://pypi.org/pypi/flake8-bugbear/23.5.9
+Homepage: https://github.com/PyCQA/flake8-bugbear
+Changelog: https://github.com/PyCQA/flake8-bugbear#change-log
+Diff: https://github.com/PyCQA/flake8-bugbear/compare/23.3.23...23.5.9
+
+Stubsabot analysis of the diff between the two releases:
+ - 2 public Python files have been added: `tests/b033.py`, `tests/b908.py`.
+ - 0 files included in typeshed's stubs have been deleted.
+ - 1 file included in typeshed's stubs has been modified or renamed: `bugbear.py`.
+ - Total lines of Python code added: 190.
+ - Total lines of Python code deleted: 26.
+
 ## 23.3.23.0 (2023-03-24)
 
 [stubsabot] Bump flake8-bugbear to 23.3.23 (#9934)
 
 Release: https://pypi.org/pypi/flake8-bugbear/23.3.23
 Homepage: https://github.com/PyCQA/flake8-bugbear
 Changelog: https://github.com/PyCQA/flake8-bugbear#change-log
```

### Comparing `types-flake8-bugbear-23.3.23.0/PKG-INFO` & `types-flake8-bugbear-23.5.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 23.3.23.0
+Version: 23.5.9.0
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1cf2e73c32e503bed1e89b694737b2962bda0cf2`.
+This package was generated from typeshed commit `7113c35a673c503a027707a97f80091da81322a9`.
```

### Comparing `types-flake8-bugbear-23.3.23.0/bugbear-stubs/__init__.pyi` & `types-flake8-bugbear-23.5.9.0/bugbear-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-bugbear-23.3.23.0/setup.py` & `types-flake8-bugbear-23.5.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1cf2e73c32e503bed1e89b694737b2962bda0cf2`.
+This package was generated from typeshed commit `7113c35a673c503a027707a97f80091da81322a9`.
 '''.lstrip()
 
 setup(name=name,
-      version="23.3.23.0",
+      version="23.5.9.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md",
```

### Comparing `types-flake8-bugbear-23.3.23.0/types_flake8_bugbear.egg-info/PKG-INFO` & `types-flake8-bugbear-23.5.9.0/types_flake8_bugbear.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 23.3.23.0
+Version: 23.5.9.0
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-bugbear`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-bugbear. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1cf2e73c32e503bed1e89b694737b2962bda0cf2`.
+This package was generated from typeshed commit `7113c35a673c503a027707a97f80091da81322a9`.
```

