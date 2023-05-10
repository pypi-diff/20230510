# Comparing `tmp/types-caldav-1.2.0.1.tar.gz` & `tmp/types-caldav-1.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-caldav-1.2.0.1.tar", last modified: Mon Mar 27 18:25:54 2023, max compression
+gzip compressed data, was "types-caldav-1.2.0.2.tar", last modified: Wed May 10 15:23:54 2023, max compression
```

## Comparing `types-caldav-1.2.0.1.tar` & `types-caldav-1.2.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:54.868131 types-caldav-1.2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:25:54.868131 types-caldav-1.2.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:54.868131 types-caldav-1.2.0.1/caldav-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/caldav-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/davclient.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:54.868131 types-caldav-1.2.0.1/caldav-stubs/elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/elements/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/elements/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/elements/cdav.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/elements/dav.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/elements/ical.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:54.868131 types-caldav-1.2.0.1/caldav-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/lib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/lib/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/lib/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/lib/url.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/lib/vcal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/objects.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-27 18:21:24.000000 types-caldav-1.2.0.1/caldav-stubs/requests.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:25:54.868131 types-caldav-1.2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:54.868131 types-caldav-1.2.0.1/types_caldav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/types_caldav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/types_caldav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/types_caldav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/types_caldav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 18:25:54.000000 types-caldav-1.2.0.1/types_caldav.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.014937 types-caldav-1.2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:23:54.014937 types-caldav-1.2.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.010938 types-caldav-1.2.0.2/caldav-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/caldav-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/davclient.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.010938 types-caldav-1.2.0.2/caldav-stubs/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/cdav.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/dav.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/ical.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.010938 types-caldav-1.2.0.2/caldav-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/url.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/vcal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/objects.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/requests.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:54.014937 types-caldav-1.2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.010938 types-caldav-1.2.0.2/types_caldav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/top_level.txt
```

### Comparing `types-caldav-1.2.0.1/CHANGELOG.md` & `types-caldav-1.2.0.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.2.0.2 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 1.2.0.1 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
 
 ## 1.2.0.0 (2023-02-27)
 
 Update caldav to 1.2 (#9821)
```

### Comparing `types-caldav-1.2.0.1/PKG-INFO` & `types-caldav-1.2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-caldav
-Version: 1.2.0.1
+Version: 1.2.0.2
 Summary: Typing stubs for caldav
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/caldav.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `caldav`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/caldav. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-caldav-1.2.0.1/caldav-stubs/davclient.pyi` & `types-caldav-1.2.0.2/caldav-stubs/davclient.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.1/caldav-stubs/elements/base.pyi` & `types-caldav-1.2.0.2/caldav-stubs/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.1/caldav-stubs/elements/cdav.pyi` & `types-caldav-1.2.0.2/caldav-stubs/elements/cdav.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.1/caldav-stubs/elements/dav.pyi` & `types-caldav-1.2.0.2/caldav-stubs/elements/dav.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.1/caldav-stubs/lib/error.pyi` & `types-caldav-1.2.0.2/caldav-stubs/lib/error.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.1/caldav-stubs/lib/url.pyi` & `types-caldav-1.2.0.2/caldav-stubs/lib/url.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.1/caldav-stubs/objects.pyi` & `types-caldav-1.2.0.2/caldav-stubs/objects.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.1/setup.py` & `types-caldav-1.2.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `caldav`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/caldav. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.2.0.1",
+      version="1.2.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/caldav.md",
```

### Comparing `types-caldav-1.2.0.1/types_caldav.egg-info/PKG-INFO` & `types-caldav-1.2.0.2/types_caldav.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-caldav
-Version: 1.2.0.1
+Version: 1.2.0.2
 Summary: Typing stubs for caldav
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/caldav.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `caldav`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/caldav. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-caldav-1.2.0.1/types_caldav.egg-info/SOURCES.txt` & `types-caldav-1.2.0.2/types_caldav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

