# Comparing `tmp/types-commonmark-0.9.2.2.tar.gz` & `tmp/types-commonmark-0.9.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-commonmark-0.9.2.2.tar", last modified: Tue Feb 21 01:29:41 2023, max compression
+gzip compressed data, was "types-commonmark-0.9.2.3.tar", last modified: Wed May 10 15:22:05 2023, max compression
```

## Comparing `types-commonmark-0.9.2.2.tar` & `types-commonmark-0.9.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:29:41.035765 types-commonmark-0.9.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-21 01:29:40.000000 types-commonmark-0.9.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:29:40.000000 types-commonmark-0.9.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 01:29:41.035765 types-commonmark-0.9.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:29:41.031765 types-commonmark-0.9.2.2/commonmark-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-21 01:29:40.000000 types-commonmark-0.9.2.2/commonmark-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/blocks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/cmark.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/common.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/dump.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/entitytrans.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/inlines.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/main.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/node.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/normalize_reference.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:29:41.031765 types-commonmark-0.9.2.2/commonmark-stubs/render/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/render/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/render/html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/render/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-21 01:26:21.000000 types-commonmark-0.9.2.2/commonmark-stubs/render/rst.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:29:41.035765 types-commonmark-0.9.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-02-21 01:29:40.000000 types-commonmark-0.9.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:29:41.035765 types-commonmark-0.9.2.2/types_commonmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 01:29:40.000000 types-commonmark-0.9.2.2/types_commonmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-02-21 01:29:41.000000 types-commonmark-0.9.2.2/types_commonmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:29:40.000000 types-commonmark-0.9.2.2/types_commonmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-21 01:29:40.000000 types-commonmark-0.9.2.2/types_commonmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:05.640394 types-commonmark-0.9.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 15:22:04.000000 types-commonmark-0.9.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:04.000000 types-commonmark-0.9.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-10 15:22:05.640394 types-commonmark-0.9.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:05.636393 types-commonmark-0.9.2.3/commonmark-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:22:04.000000 types-commonmark-0.9.2.3/commonmark-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/blocks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/cmark.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/dump.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/entitytrans.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/inlines.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/normalize_reference.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:05.640394 types-commonmark-0.9.2.3/commonmark-stubs/render/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/render/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/render/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/render/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-10 15:19:44.000000 types-commonmark-0.9.2.3/commonmark-stubs/render/rst.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:05.640394 types-commonmark-0.9.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-10 15:22:04.000000 types-commonmark-0.9.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:05.640394 types-commonmark-0.9.2.3/types_commonmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-10 15:22:05.000000 types-commonmark-0.9.2.3/types_commonmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-10 15:22:05.000000 types-commonmark-0.9.2.3/types_commonmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:05.000000 types-commonmark-0.9.2.3/types_commonmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:22:05.000000 types-commonmark-0.9.2.3/types_commonmark.egg-info/top_level.txt
```

### Comparing `types-commonmark-0.9.2.2/PKG-INFO` & `types-commonmark-0.9.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-commonmark
-Version: 0.9.2.2
+Version: 0.9.2.3
 Summary: Typing stubs for commonmark
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/commonmark.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `commonmark`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/commonmark. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-commonmark-0.9.2.2/commonmark-stubs/blocks.pyi` & `types-commonmark-0.9.2.3/commonmark-stubs/blocks.pyi`

 * *Files identical despite different names*

### Comparing `types-commonmark-0.9.2.2/commonmark-stubs/common.pyi` & `types-commonmark-0.9.2.3/commonmark-stubs/common.pyi`

 * *Files identical despite different names*

### Comparing `types-commonmark-0.9.2.2/commonmark-stubs/inlines.pyi` & `types-commonmark-0.9.2.3/commonmark-stubs/inlines.pyi`

 * *Files identical despite different names*

### Comparing `types-commonmark-0.9.2.2/commonmark-stubs/node.pyi` & `types-commonmark-0.9.2.3/commonmark-stubs/node.pyi`

 * *Files identical despite different names*

### Comparing `types-commonmark-0.9.2.2/commonmark-stubs/render/html.pyi` & `types-commonmark-0.9.2.3/commonmark-stubs/render/html.pyi`

 * *Files identical despite different names*

### Comparing `types-commonmark-0.9.2.2/commonmark-stubs/render/rst.pyi` & `types-commonmark-0.9.2.3/commonmark-stubs/render/rst.pyi`

 * *Files identical despite different names*

### Comparing `types-commonmark-0.9.2.2/setup.py` & `types-commonmark-0.9.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `commonmark`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/commonmark. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.9.2.2",
+      version="0.9.2.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/commonmark.md",
```

### Comparing `types-commonmark-0.9.2.2/types_commonmark.egg-info/PKG-INFO` & `types-commonmark-0.9.2.3/types_commonmark.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-commonmark
-Version: 0.9.2.2
+Version: 0.9.2.3
 Summary: Typing stubs for commonmark
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/commonmark.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `commonmark`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/commonmark. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-commonmark-0.9.2.2/types_commonmark.egg-info/SOURCES.txt` & `types-commonmark-0.9.2.3/types_commonmark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

