# Comparing `tmp/types-chardet-5.0.4.5.tar.gz` & `tmp/types-chardet-5.0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-chardet-5.0.4.5.tar", last modified: Sat Apr 29 15:14:05 2023, max compression
+gzip compressed data, was "types-chardet-5.0.4.6.tar", last modified: Wed May 10 15:22:19 2023, max compression
```

## Comparing `types-chardet-5.0.4.5.tar` & `types-chardet-5.0.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:05.828437 types-chardet-5.0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-29 15:14:05.828437 types-chardet-5.0.4.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:05.828437 types-chardet-5.0.4.5/chardet-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/chardet-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langbulgarianmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langcyrillicmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langgreekmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langhebrewmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langhungarianmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langthaimodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/langturkishmodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/universaldetector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-29 15:13:39.000000 types-chardet-5.0.4.5/chardet-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:14:05.832437 types-chardet-5.0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:14:05.828437 types-chardet-5.0.4.5/types_chardet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/types_chardet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/types_chardet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/types_chardet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-29 15:14:05.000000 types-chardet-5.0.4.5/types_chardet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:19.176713 types-chardet-5.0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-10 15:22:18.000000 types-chardet-5.0.4.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:18.000000 types-chardet-5.0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-10 15:22:19.176713 types-chardet-5.0.4.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:19.176713 types-chardet-5.0.4.6/chardet-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 15:22:18.000000 types-chardet-5.0.4.6/chardet-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/langbulgarianmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/langcyrillicmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/langgreekmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/langhebrewmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/langhungarianmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/langthaimodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/langturkishmodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/universaldetector.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 15:19:44.000000 types-chardet-5.0.4.6/chardet-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:19.176713 types-chardet-5.0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-10 15:22:18.000000 types-chardet-5.0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:19.176713 types-chardet-5.0.4.6/types_chardet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-10 15:22:19.000000 types-chardet-5.0.4.6/types_chardet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 15:22:19.000000 types-chardet-5.0.4.6/types_chardet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:19.000000 types-chardet-5.0.4.6/types_chardet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 15:22:19.000000 types-chardet-5.0.4.6/types_chardet.egg-info/top_level.txt
```

### Comparing `types-chardet-5.0.4.5/CHANGELOG.md` & `types-chardet-5.0.4.6/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 5.0.4.6 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 5.0.4.5 (2023-04-29)
 
 chardet: UniversalDetector.feed accepts bytearray (#10107)
 
 Technically it accepts any buffer, but the inline type annotations
 now say bytes | bytearray, so let's stick to that.
```

### Comparing `types-chardet-5.0.4.5/PKG-INFO` & `types-chardet-5.0.4.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-chardet
-Version: 5.0.4.5
+Version: 5.0.4.6
 Summary: Typing stubs for chardet
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chardet.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,8 @@
 
 *Note:* The `chardet` package includes type annotations or type stubs
 since version 5.1.0. Please uninstall the `types-chardet`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-chardet-5.0.4.5/chardet-stubs/__init__.pyi` & `types-chardet-5.0.4.6/chardet-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-chardet-5.0.4.5/chardet-stubs/enums.pyi` & `types-chardet-5.0.4.6/chardet-stubs/enums.pyi`

 * *Files identical despite different names*

### Comparing `types-chardet-5.0.4.5/chardet-stubs/universaldetector.pyi` & `types-chardet-5.0.4.6/chardet-stubs/universaldetector.pyi`

 * *Files identical despite different names*

### Comparing `types-chardet-5.0.4.5/setup.py` & `types-chardet-5.0.4.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 *Note:* The `chardet` package includes type annotations or type stubs
 since version 5.1.0. Please uninstall the `types-chardet`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="5.0.4.5",
+      version="5.0.4.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chardet.md",
```

### Comparing `types-chardet-5.0.4.5/types_chardet.egg-info/PKG-INFO` & `types-chardet-5.0.4.6/types_chardet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-chardet
-Version: 5.0.4.5
+Version: 5.0.4.6
 Summary: Typing stubs for chardet
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chardet.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,8 @@
 
 *Note:* The `chardet` package includes type annotations or type stubs
 since version 5.1.0. Please uninstall the `types-chardet`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0f270e61bfaa5677cecc0e3401084924fe0e04ce`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-chardet-5.0.4.5/types_chardet.egg-info/SOURCES.txt` & `types-chardet-5.0.4.6/types_chardet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

