# Comparing `tmp/types-Flask-Migrate-4.0.0.3.tar.gz` & `tmp/types-Flask-Migrate-4.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-Migrate-4.0.0.3.tar", last modified: Mon Mar 27 18:26:01 2023, max compression
+gzip compressed data, was "types-Flask-Migrate-4.0.0.4.tar", last modified: Wed May 10 15:23:58 2023, max compression
```

## Comparing `types-Flask-Migrate-4.0.0.3.tar` & `types-Flask-Migrate-4.0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:01.912205 types-Flask-Migrate-4.0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-27 18:26:01.912205 types-Flask-Migrate-4.0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:01.912205 types-Flask-Migrate-4.0.0.3/flask_migrate-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/flask_migrate-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-27 18:21:24.000000 types-Flask-Migrate-4.0.0.3/flask_migrate-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:26:01.912205 types-Flask-Migrate-4.0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:26:01.912205 types-Flask-Migrate-4.0.0.3/types_Flask_Migrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/types_Flask_Migrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/types_Flask_Migrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/types_Flask_Migrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/types_Flask_Migrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 18:26:01.000000 types-Flask-Migrate-4.0.0.3/types_Flask_Migrate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 15:23:57.000000 types-Flask-Migrate-4.0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:57.000000 types-Flask-Migrate-4.0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/flask_migrate-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 15:23:57.000000 types-Flask-Migrate-4.0.0.4/flask_migrate-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 15:19:44.000000 types-Flask-Migrate-4.0.0.4/flask_migrate-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-10 15:23:57.000000 types-Flask-Migrate-4.0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:58.195036 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 15:23:58.000000 types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/top_level.txt
```

### Comparing `types-Flask-Migrate-4.0.0.3/CHANGELOG.md` & `types-Flask-Migrate-4.0.0.4/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 4.0.0.4 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 4.0.0.3 (2023-03-27)
 
 Add defaults for third-party stubs E-H (#9954)
 
 ## 4.0.0.2 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-Flask-Migrate-4.0.0.3/PKG-INFO` & `types-Flask-Migrate-4.0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Migrate
-Version: 4.0.0.3
+Version: 4.0.0.4
 Summary: Typing stubs for Flask-Migrate
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Flask-Migrate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Flask-Migrate. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-Flask-Migrate-4.0.0.3/flask_migrate-stubs/__init__.pyi` & `types-Flask-Migrate-4.0.0.4/flask_migrate-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Migrate-4.0.0.3/setup.py` & `types-Flask-Migrate-4.0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Flask-Migrate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Flask-Migrate. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="4.0.0.3",
+      version="4.0.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md",
```

### Comparing `types-Flask-Migrate-4.0.0.3/types_Flask_Migrate.egg-info/PKG-INFO` & `types-Flask-Migrate-4.0.0.4/types_Flask_Migrate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Migrate
-Version: 4.0.0.3
+Version: 4.0.0.4
 Summary: Typing stubs for Flask-Migrate
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Flask-Migrate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Flask-Migrate. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

