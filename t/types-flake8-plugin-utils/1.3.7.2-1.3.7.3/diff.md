# Comparing `tmp/types-flake8-plugin-utils-1.3.7.2.tar.gz` & `tmp/types-flake8-plugin-utils-1.3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-plugin-utils-1.3.7.2.tar", last modified: Mon Mar 27 18:23:26 2023, max compression
+gzip compressed data, was "types-flake8-plugin-utils-1.3.7.3.tar", last modified: Wed May 10 15:20:05 2023, max compression
```

## Comparing `types-flake8-plugin-utils-1.3.7.2.tar` & `types-flake8-plugin-utils-1.3.7.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:26.398589 types-flake8-plugin-utils-1.3.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-27 18:23:25.000000 types-flake8-plugin-utils-1.3.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:23:25.000000 types-flake8-plugin-utils-1.3.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-27 18:23:26.398589 types-flake8-plugin-utils-1.3.7.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:26.394589 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-27 18:23:25.000000 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-27 18:21:24.000000 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-27 18:21:24.000000 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/plugin.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:26.398589 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-27 18:21:24.000000 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-27 18:21:24.000000 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/utils/assertions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-27 18:21:24.000000 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/utils/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-27 18:21:24.000000 types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/utils/equiv_nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:23:26.398589 types-flake8-plugin-utils-1.3.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-27 18:23:25.000000 types-flake8-plugin-utils-1.3.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:26.398589 types-flake8-plugin-utils-1.3.7.2/types_flake8_plugin_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-27 18:23:26.000000 types-flake8-plugin-utils-1.3.7.2/types_flake8_plugin_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-27 18:23:26.000000 types-flake8-plugin-utils-1.3.7.2/types_flake8_plugin_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:23:26.000000 types-flake8-plugin-utils-1.3.7.2/types_flake8_plugin_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-27 18:23:26.000000 types-flake8-plugin-utils-1.3.7.2/types_flake8_plugin_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:05.357573 types-flake8-plugin-utils-1.3.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-10 15:20:02.000000 types-flake8-plugin-utils-1.3.7.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:20:02.000000 types-flake8-plugin-utils-1.3.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-10 15:20:05.357573 types-flake8-plugin-utils-1.3.7.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:05.353573 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:20:02.000000 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-10 15:19:44.000000 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-10 15:19:44.000000 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/plugin.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:05.357573 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-10 15:19:44.000000 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-10 15:19:44.000000 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/utils/assertions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 15:19:44.000000 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/utils/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 15:19:44.000000 types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/utils/equiv_nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:20:05.357573 types-flake8-plugin-utils-1.3.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-10 15:20:02.000000 types-flake8-plugin-utils-1.3.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:05.357573 types-flake8-plugin-utils-1.3.7.3/types_flake8_plugin_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-10 15:20:05.000000 types-flake8-plugin-utils-1.3.7.3/types_flake8_plugin_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-10 15:20:05.000000 types-flake8-plugin-utils-1.3.7.3/types_flake8_plugin_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:20:05.000000 types-flake8-plugin-utils-1.3.7.3/types_flake8_plugin_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 15:20:05.000000 types-flake8-plugin-utils-1.3.7.3/types_flake8_plugin_utils.egg-info/top_level.txt
```

### Comparing `types-flake8-plugin-utils-1.3.7.2/CHANGELOG.md` & `types-flake8-plugin-utils-1.3.7.3/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.3.7.3 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 1.3.7.2 (2023-03-27)
 
 Add defaults for third-party stubs E-H (#9954)
 
 ## 1.3.7.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-flake8-plugin-utils-1.3.7.2/PKG-INFO` & `types-flake8-plugin-utils-1.3.7.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-plugin-utils
-Version: 1.3.7.2
+Version: 1.3.7.3
 Summary: Typing stubs for flake8-plugin-utils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-plugin-utils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-plugin-utils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-plugin-utils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-flake8-plugin-utils-1.3.7.2/flake8_plugin_utils-stubs/plugin.pyi` & `types-flake8-plugin-utils-1.3.7.3/flake8_plugin_utils-stubs/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-plugin-utils-1.3.7.2/setup.py` & `types-flake8-plugin-utils-1.3.7.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-plugin-utils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-plugin-utils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.3.7.2",
+      version="1.3.7.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-plugin-utils.md",
```

### Comparing `types-flake8-plugin-utils-1.3.7.2/types_flake8_plugin_utils.egg-info/PKG-INFO` & `types-flake8-plugin-utils-1.3.7.3/types_flake8_plugin_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-plugin-utils
-Version: 1.3.7.2
+Version: 1.3.7.3
 Summary: Typing stubs for flake8-plugin-utils
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-plugin-utils.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-plugin-utils`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-plugin-utils. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-flake8-plugin-utils-1.3.7.2/types_flake8_plugin_utils.egg-info/SOURCES.txt` & `types-flake8-plugin-utils-1.3.7.3/types_flake8_plugin_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

