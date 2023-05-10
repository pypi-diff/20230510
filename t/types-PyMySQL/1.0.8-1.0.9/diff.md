# Comparing `tmp/types-PyMySQL-1.0.8.tar.gz` & `tmp/types-PyMySQL-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyMySQL-1.0.8.tar", last modified: Tue Dec 28 12:29:31 2021, max compression
+gzip compressed data, was "types-PyMySQL-1.0.9.tar", last modified: Fri Jan  7 11:28:21 2022, max compression
```

## Comparing `types-PyMySQL-1.0.8.tar` & `types-PyMySQL-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:29:31.518363 types-PyMySQL-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1051 2021-12-28 12:29:30.000000 types-PyMySQL-1.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-28 12:29:30.000000 types-PyMySQL-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      854 2021-12-28 12:29:31.518363 types-PyMySQL-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:29:31.514363 types-PyMySQL-1.0.8/pymysql-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-28 12:29:30.000000 types-PyMySQL-1.0.8/pymysql-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      327 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/charset.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7495 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/connections.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:29:31.518363 types-PyMySQL-1.0.8/pymysql-stubs/constants/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/constants/CLIENT.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/constants/COMMAND.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11280 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/constants/ER.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/constants/FIELD_TYPE.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/constants/FLAG.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/constants/SERVER_STATUS.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/constants/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/cursors.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      600 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/err.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/times.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-12-28 12:29:14.000000 types-PyMySQL-1.0.8/pymysql-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-28 12:29:31.518363 types-PyMySQL-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-12-28 12:29:30.000000 types-PyMySQL-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 12:29:31.518363 types-PyMySQL-1.0.8/types_PyMySQL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      854 2021-12-28 12:29:31.000000 types-PyMySQL-1.0.8/types_PyMySQL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-12-28 12:29:31.000000 types-PyMySQL-1.0.8/types_PyMySQL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 12:29:31.000000 types-PyMySQL-1.0.8/types_PyMySQL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-12-28 12:29:31.000000 types-PyMySQL-1.0.8/types_PyMySQL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:28:21.770980 types-PyMySQL-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1051 2022-01-07 11:28:21.000000 types-PyMySQL-1.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-07 11:28:21.000000 types-PyMySQL-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-01-07 11:28:21.770980 types-PyMySQL-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:28:21.770980 types-PyMySQL-1.0.9/pymysql-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-07 11:28:21.000000 types-PyMySQL-1.0.9/pymysql-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      327 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/charset.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     7495 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/connections.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:28:21.770980 types-PyMySQL-1.0.9/pymysql-stubs/constants/
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/constants/CLIENT.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/constants/COMMAND.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    11280 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/constants/ER.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/constants/FIELD_TYPE.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/constants/FLAG.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/constants/SERVER_STATUS.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/constants/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/cursors.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/err.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/times.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-01-07 11:27:57.000000 types-PyMySQL-1.0.9/pymysql-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-07 11:28:21.770980 types-PyMySQL-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-01-07 11:28:21.000000 types-PyMySQL-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:28:21.770980 types-PyMySQL-1.0.9/types_PyMySQL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-01-07 11:28:21.000000 types-PyMySQL-1.0.9/types_PyMySQL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2022-01-07 11:28:21.000000 types-PyMySQL-1.0.9/types_PyMySQL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-07 11:28:21.000000 types-PyMySQL-1.0.9/types_PyMySQL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-07 11:28:21.000000 types-PyMySQL-1.0.9/types_PyMySQL.egg-info/top_level.txt
```

### Comparing `types-PyMySQL-1.0.8/CHANGELOG.md` & `types-PyMySQL-1.0.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.0.8/PKG-INFO` & `types-PyMySQL-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: types-PyMySQL
-Version: 1.0.8
+Version: 1.0.9
 Summary: Typing stubs for PyMySQL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Typing :: Typed
+Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for PyMySQL
 
 This is a PEP 561 type stub package for the `PyMySQL` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `PyMySQL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/PyMySQL. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `22bf9e8a787b38b1a0e193edd5b47119e43286ca`.
+This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
```

### Comparing `types-PyMySQL-1.0.8/pymysql-stubs/__init__.pyi` & `types-PyMySQL-1.0.9/pymysql-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.0.8/pymysql-stubs/connections.pyi` & `types-PyMySQL-1.0.9/pymysql-stubs/connections.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.0.8/pymysql-stubs/constants/ER.pyi` & `types-PyMySQL-1.0.9/pymysql-stubs/constants/ER.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.0.8/pymysql-stubs/converters.pyi` & `types-PyMySQL-1.0.9/pymysql-stubs/converters.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.0.8/pymysql-stubs/cursors.pyi` & `types-PyMySQL-1.0.9/pymysql-stubs/cursors.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.0.8/pymysql-stubs/err.pyi` & `types-PyMySQL-1.0.9/pymysql-stubs/err.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.0.8/setup.py` & `types-PyMySQL-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 This is a PEP 561 type stub package for the `PyMySQL` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `PyMySQL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/PyMySQL. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `22bf9e8a787b38b1a0e193edd5b47119e43286ca`.
+This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.0.8",
+      version="1.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       install_requires=[],
       packages=['pymysql-stubs'],
       package_data={'pymysql-stubs': ['__init__.pyi', 'charset.pyi', 'connections.pyi', 'constants/CLIENT.pyi', 'constants/COMMAND.pyi', 'constants/ER.pyi', 'constants/FIELD_TYPE.pyi', 'constants/FLAG.pyi', 'constants/SERVER_STATUS.pyi', 'constants/__init__.pyi', 'converters.pyi', 'cursors.pyi', 'err.pyi', 'times.pyi', 'util.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
-          "Typing :: Typed",
+          "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-PyMySQL-1.0.8/types_PyMySQL.egg-info/PKG-INFO` & `types-PyMySQL-1.0.9/types_PyMySQL.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: types-PyMySQL
-Version: 1.0.8
+Version: 1.0.9
 Summary: Typing stubs for PyMySQL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Typing :: Typed
+Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for PyMySQL
 
 This is a PEP 561 type stub package for the `PyMySQL` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `PyMySQL`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/PyMySQL. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `22bf9e8a787b38b1a0e193edd5b47119e43286ca`.
+This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
```

### Comparing `types-PyMySQL-1.0.8/types_PyMySQL.egg-info/SOURCES.txt` & `types-PyMySQL-1.0.9/types_PyMySQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

