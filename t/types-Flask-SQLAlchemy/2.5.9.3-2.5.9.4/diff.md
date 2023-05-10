# Comparing `tmp/types-Flask-SQLAlchemy-2.5.9.3.tar.gz` & `tmp/types-Flask-SQLAlchemy-2.5.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-SQLAlchemy-2.5.9.3.tar", last modified: Mon Mar 27 18:25:51 2023, max compression
+gzip compressed data, was "types-Flask-SQLAlchemy-2.5.9.4.tar", last modified: Wed May 10 15:23:27 2023, max compression
```

## Comparing `types-Flask-SQLAlchemy-2.5.9.3.tar` & `types-Flask-SQLAlchemy-2.5.9.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:51.860099 types-Flask-SQLAlchemy-2.5.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-27 18:25:51.860099 types-Flask-SQLAlchemy-2.5.9.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:51.860099 types-Flask-SQLAlchemy-2.5.9.3/flask_sqlalchemy-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/flask_sqlalchemy-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-03-27 18:21:24.000000 types-Flask-SQLAlchemy-2.5.9.3/flask_sqlalchemy-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-27 18:21:24.000000 types-Flask-SQLAlchemy-2.5.9.3/flask_sqlalchemy-stubs/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-27 18:21:24.000000 types-Flask-SQLAlchemy-2.5.9.3/flask_sqlalchemy-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:25:51.860099 types-Flask-SQLAlchemy-2.5.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:25:51.860099 types-Flask-SQLAlchemy-2.5.9.3/types_Flask_SQLAlchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/types_Flask_SQLAlchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/types_Flask_SQLAlchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/types_Flask_SQLAlchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/types_Flask_SQLAlchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-27 18:25:51.000000 types-Flask-SQLAlchemy-2.5.9.3/types_Flask_SQLAlchemy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:27.842344 types-Flask-SQLAlchemy-2.5.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-10 15:23:27.842344 types-Flask-SQLAlchemy-2.5.9.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:27.842344 types-Flask-SQLAlchemy-2.5.9.4/flask_sqlalchemy-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/flask_sqlalchemy-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-10 15:19:44.000000 types-Flask-SQLAlchemy-2.5.9.4/flask_sqlalchemy-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-10 15:19:44.000000 types-Flask-SQLAlchemy-2.5.9.4/flask_sqlalchemy-stubs/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-10 15:19:44.000000 types-Flask-SQLAlchemy-2.5.9.4/flask_sqlalchemy-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:27.842344 types-Flask-SQLAlchemy-2.5.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:27.842344 types-Flask-SQLAlchemy-2.5.9.4/types_Flask_SQLAlchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/types_Flask_SQLAlchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/types_Flask_SQLAlchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/types_Flask_SQLAlchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/types_Flask_SQLAlchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 15:23:27.000000 types-Flask-SQLAlchemy-2.5.9.4/types_Flask_SQLAlchemy.egg-info/top_level.txt
```

### Comparing `types-Flask-SQLAlchemy-2.5.9.3/CHANGELOG.md` & `types-Flask-SQLAlchemy-2.5.9.4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.5.9.4 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 2.5.9.3 (2023-03-27)
 
 Add defaults for third-party stubs E-H (#9954)
 
 ## 2.5.9.2 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-Flask-SQLAlchemy-2.5.9.3/PKG-INFO` & `types-Flask-SQLAlchemy-2.5.9.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-SQLAlchemy
-Version: 2.5.9.3
+Version: 2.5.9.4
 Summary: Typing stubs for Flask-SQLAlchemy
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-SQLAlchemy.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,8 @@
 
 *Note:* The `Flask-SQLAlchemy` package includes type annotations or type stubs
 since version 3.0.1. Please uninstall the `types-Flask-SQLAlchemy`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-Flask-SQLAlchemy-2.5.9.3/flask_sqlalchemy-stubs/__init__.pyi` & `types-Flask-SQLAlchemy-2.5.9.4/flask_sqlalchemy-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-SQLAlchemy-2.5.9.3/flask_sqlalchemy-stubs/model.pyi` & `types-Flask-SQLAlchemy-2.5.9.4/flask_sqlalchemy-stubs/model.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-SQLAlchemy-2.5.9.3/setup.py` & `types-Flask-SQLAlchemy-2.5.9.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 *Note:* The `Flask-SQLAlchemy` package includes type annotations or type stubs
 since version 3.0.1. Please uninstall the `types-Flask-SQLAlchemy`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.5.9.3",
+      version="2.5.9.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-SQLAlchemy.md",
```

### Comparing `types-Flask-SQLAlchemy-2.5.9.3/types_Flask_SQLAlchemy.egg-info/PKG-INFO` & `types-Flask-SQLAlchemy-2.5.9.4/types_Flask_SQLAlchemy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-SQLAlchemy
-Version: 2.5.9.3
+Version: 2.5.9.4
 Summary: Typing stubs for Flask-SQLAlchemy
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-SQLAlchemy.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,8 @@
 
 *Note:* The `Flask-SQLAlchemy` package includes type annotations or type stubs
 since version 3.0.1. Please uninstall the `types-Flask-SQLAlchemy`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

