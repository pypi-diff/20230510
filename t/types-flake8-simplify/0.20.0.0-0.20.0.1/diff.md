# Comparing `tmp/types-flake8-simplify-0.20.0.0.tar.gz` & `tmp/types-flake8-simplify-0.20.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-simplify-0.20.0.0.tar", last modified: Fri Mar 31 01:18:03 2023, max compression
+gzip compressed data, was "types-flake8-simplify-0.20.0.1.tar", last modified: Wed May 10 15:20:10 2023, max compression
```

## Comparing `types-flake8-simplify-0.20.0.0.tar` & `types-flake8-simplify-0.20.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:18:03.418889 types-flake8-simplify-0.20.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-31 01:18:02.000000 types-flake8-simplify-0.20.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 01:18:02.000000 types-flake8-simplify-0.20.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-31 01:18:03.418889 types-flake8-simplify-0.20.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:18:03.418889 types-flake8-simplify-0.20.0.0/flake8_simplify-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-31 01:18:02.000000 types-flake8-simplify-0.20.0.0/flake8_simplify-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-31 01:17:49.000000 types-flake8-simplify-0.20.0.0/flake8_simplify-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 01:18:03.418889 types-flake8-simplify-0.20.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-31 01:18:02.000000 types-flake8-simplify-0.20.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:18:03.418889 types-flake8-simplify-0.20.0.0/types_flake8_simplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-31 01:18:03.000000 types-flake8-simplify-0.20.0.0/types_flake8_simplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-31 01:18:03.000000 types-flake8-simplify-0.20.0.0/types_flake8_simplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 01:18:03.000000 types-flake8-simplify-0.20.0.0/types_flake8_simplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 01:18:03.000000 types-flake8-simplify-0.20.0.0/types_flake8_simplify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:10.749699 types-flake8-simplify-0.20.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-10 15:20:09.000000 types-flake8-simplify-0.20.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:20:09.000000 types-flake8-simplify-0.20.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-10 15:20:10.749699 types-flake8-simplify-0.20.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:10.749699 types-flake8-simplify-0.20.0.1/flake8_simplify-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:20:09.000000 types-flake8-simplify-0.20.0.1/flake8_simplify-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-10 15:19:44.000000 types-flake8-simplify-0.20.0.1/flake8_simplify-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:20:10.753699 types-flake8-simplify-0.20.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-10 15:20:09.000000 types-flake8-simplify-0.20.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:10.749699 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-10 15:20:10.000000 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-10 15:20:10.000000 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:20:10.000000 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 15:20:10.000000 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/top_level.txt
```

### Comparing `types-flake8-simplify-0.20.0.0/CHANGELOG.md` & `types-flake8-simplify-0.20.0.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.20.0.1 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 0.20.0.0 (2023-03-31)
 
 [stubsabot] Bump flake8-simplify to 0.20.* (#9993)
 
 Release: https://pypi.org/pypi/flake8-simplify/0.20.0
 Homepage: https://github.com/MartinThoma/flake8-simplify
```

### Comparing `types-flake8-simplify-0.20.0.0/setup.py` & `types-flake8-simplify-0.20.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-simplify`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-simplify. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `34018d6a2c9833de7c5718a70b5346245f583a73`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.20.0.0",
+      version="0.20.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-simplify.md",
```

