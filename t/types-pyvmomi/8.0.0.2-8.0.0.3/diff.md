# Comparing `tmp/types-pyvmomi-8.0.0.2.tar.gz` & `tmp/types-pyvmomi-8.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyvmomi-8.0.0.2.tar", last modified: Sat May  6 01:10:02 2023, max compression
+gzip compressed data, was "types-pyvmomi-8.0.0.3.tar", last modified: Wed May 10 15:21:37 2023, max compression
```

## Comparing `types-pyvmomi-8.0.0.2.tar` & `types-pyvmomi-8.0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:02.458128 types-pyvmomi-8.0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-06 01:09:59.000000 types-pyvmomi-8.0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 01:09:59.000000 types-pyvmomi-8.0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-06 01:10:02.458128 types-pyvmomi-8.0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:02.458128 types-pyvmomi-8.0.0.2/pyVmomi-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-06 01:09:59.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:02.458128 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vim/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vim/event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vim/fault.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vim/option.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vim/view.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:02.458128 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vmodl/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vmodl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vmodl/fault.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-06 01:09:41.000000 types-pyvmomi-8.0.0.2/pyVmomi-stubs/vmodl/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 01:10:02.458128 types-pyvmomi-8.0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-06 01:09:59.000000 types-pyvmomi-8.0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 01:10:02.458128 types-pyvmomi-8.0.0.2/types_pyvmomi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-06 01:10:02.000000 types-pyvmomi-8.0.0.2/types_pyvmomi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-06 01:10:02.000000 types-pyvmomi-8.0.0.2/types_pyvmomi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 01:10:02.000000 types-pyvmomi-8.0.0.2/types_pyvmomi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 01:10:02.000000 types-pyvmomi-8.0.0.2/types_pyvmomi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:37.463720 types-pyvmomi-8.0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-10 15:21:36.000000 types-pyvmomi-8.0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:21:36.000000 types-pyvmomi-8.0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-10 15:21:37.463720 types-pyvmomi-8.0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:37.463720 types-pyvmomi-8.0.0.3/pyVmomi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-10 15:21:36.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:37.463720 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vim/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vim/fault.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vim/option.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vim/view.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:37.463720 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vmodl/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vmodl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vmodl/fault.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-10 15:19:44.000000 types-pyvmomi-8.0.0.3/pyVmomi-stubs/vmodl/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:21:37.463720 types-pyvmomi-8.0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-10 15:21:36.000000 types-pyvmomi-8.0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:37.463720 types-pyvmomi-8.0.0.3/types_pyvmomi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-10 15:21:37.000000 types-pyvmomi-8.0.0.3/types_pyvmomi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-10 15:21:37.000000 types-pyvmomi-8.0.0.3/types_pyvmomi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:21:37.000000 types-pyvmomi-8.0.0.3/types_pyvmomi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 15:21:37.000000 types-pyvmomi-8.0.0.3/types_pyvmomi.egg-info/top_level.txt
```

### Comparing `types-pyvmomi-8.0.0.2/CHANGELOG.md` & `types-pyvmomi-8.0.0.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 8.0.0.3 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 8.0.0.2 (2023-05-06)
 
 [stubsabot] Mark pyvmomi as obsolete since 8.0.1.0 (#10148)
 
 Release: https://pypi.org/pypi/pyvmomi/8.0.1.0
 Homepage: https://github.com/vmware/pyvmomi
 Diff: https://github.com/vmware/pyvmomi/compare/v8.0.0.1.2...v8.0.1.0
```

### Comparing `types-pyvmomi-8.0.0.2/PKG-INFO` & `types-pyvmomi-8.0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyvmomi
-Version: 8.0.0.2
+Version: 8.0.0.3
 Summary: Typing stubs for pyvmomi
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,8 @@
 
 *Note:* The `pyvmomi` package includes type annotations or type stubs
 since version 8.0.1.0. Please uninstall the `types-pyvmomi`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `853d01d55ef5b5c7f0733e62c2e214be1d472657`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-pyvmomi-8.0.0.2/pyVmomi-stubs/vim/__init__.pyi` & `types-pyvmomi-8.0.0.3/pyVmomi-stubs/vim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.2/pyVmomi-stubs/vim/view.pyi` & `types-pyvmomi-8.0.0.3/pyVmomi-stubs/vim/view.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.2/pyVmomi-stubs/vmodl/__init__.pyi` & `types-pyvmomi-8.0.0.3/pyVmomi-stubs/vmodl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.2/pyVmomi-stubs/vmodl/query.pyi` & `types-pyvmomi-8.0.0.3/pyVmomi-stubs/vmodl/query.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.2/setup.py` & `types-pyvmomi-8.0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 *Note:* The `pyvmomi` package includes type annotations or type stubs
 since version 8.0.1.0. Please uninstall the `types-pyvmomi`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `853d01d55ef5b5c7f0733e62c2e214be1d472657`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="8.0.0.2",
+      version="8.0.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md",
```

### Comparing `types-pyvmomi-8.0.0.2/types_pyvmomi.egg-info/PKG-INFO` & `types-pyvmomi-8.0.0.3/types_pyvmomi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyvmomi
-Version: 8.0.0.2
+Version: 8.0.0.3
 Summary: Typing stubs for pyvmomi
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,8 @@
 
 *Note:* The `pyvmomi` package includes type annotations or type stubs
 since version 8.0.1.0. Please uninstall the `types-pyvmomi`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `853d01d55ef5b5c7f0733e62c2e214be1d472657`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

