# Comparing `tmp/types-Flask-Cors-3.0.8.tar.gz` & `tmp/types-Flask-Cors-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-Cors-3.0.8.tar", last modified: Sat May  7 09:18:11 2022, max compression
+gzip compressed data, was "types-Flask-Cors-3.0.9.tar", last modified: Thu Jul  7 12:38:39 2022, max compression
```

## Comparing `types-Flask-Cors-3.0.8.tar` & `types-Flask-Cors-3.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 09:18:11.538167 types-Flask-Cors-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-05-07 09:18:11.000000 types-Flask-Cors-3.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-07 09:18:11.000000 types-Flask-Cors-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-05-07 09:18:11.538167 types-Flask-Cors-3.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 09:18:11.538167 types-Flask-Cors-3.0.8/flask_cors-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-07 09:18:11.000000 types-Flask-Cors-3.0.8/flask_cors-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-07 09:18:00.000000 types-Flask-Cors-3.0.8/flask_cors-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2022-05-07 09:18:00.000000 types-Flask-Cors-3.0.8/flask_cors-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-05-07 09:18:00.000000 types-Flask-Cors-3.0.8/flask_cors-stubs/decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-05-07 09:18:00.000000 types-Flask-Cors-3.0.8/flask_cors-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-07 09:18:00.000000 types-Flask-Cors-3.0.8/flask_cors-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-07 09:18:11.538167 types-Flask-Cors-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-05-07 09:18:11.000000 types-Flask-Cors-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-07 09:18:11.538167 types-Flask-Cors-3.0.8/types_Flask_Cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-05-07 09:18:11.000000 types-Flask-Cors-3.0.8/types_Flask_Cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-05-07 09:18:11.000000 types-Flask-Cors-3.0.8/types_Flask_Cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-07 09:18:11.000000 types-Flask-Cors-3.0.8/types_Flask_Cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-07 09:18:11.000000 types-Flask-Cors-3.0.8/types_Flask_Cors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-07-07 12:38:38.000000 types-Flask-Cors-3.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-07 12:38:38.000000 types-Flask-Cors-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/flask_cors-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-07 12:38:38.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-07 12:38:30.000000 types-Flask-Cors-3.0.9/flask_cors-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1641 2022-07-07 12:38:38.000000 types-Flask-Cors-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 12:38:39.560135 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-07-07 12:38:39.000000 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-07 12:38:39.000000 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-07 12:38:39.000000 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-07 12:38:39.000000 types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/top_level.txt
```

### Comparing `types-Flask-Cors-3.0.8/CHANGELOG.md` & `types-Flask-Cors-3.0.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.0.9 (2022-07-07)
+
+Fix various `TypeAlias` issues (#8248)
+
 ## 3.0.8 (2022-05-07)
 
 Import generics from standard modules in all third-party stubs (#7791)
 
 ## 3.0.7 (2022-05-06)
 
 `flask-cors.decorator`: allow `re.Pattern` objects to `origins` and `allow_headers` parameters (#7782)
```

### Comparing `types-Flask-Cors-3.0.8/PKG-INFO` & `types-Flask-Cors-3.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 3.0.8
+Version: 3.0.9
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `Flask-Cors` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `Flask-Cors`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/Flask-Cors. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `4e946b74bf18dc932caf41d0257957d85bbabe91`.
+This package was generated from typeshed commit `9ccf4589a0cc8f0c5a8cc2c07c485da6d7118767`.
```

### Comparing `types-Flask-Cors-3.0.8/flask_cors-stubs/core.pyi` & `types-Flask-Cors-3.0.9/flask_cors-stubs/core.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ACL_CREDENTIALS: str
 ACL_MAX_AGE: str
 ACL_REQUEST_METHOD: str
 ACL_REQUEST_HEADERS: str
 ALL_METHODS: list[str]
 CONFIG_OPTIONS: list[str]
 FLASK_CORS_EVALUATED: str
-RegexObject: TypeAlias = Pattern[str]
+RegexObject: type[Pattern[str]]
 DEFAULT_OPTIONS: _Options
 
 def parse_resources(resources: dict[str, _Options] | Iterable[str] | str | Pattern[str]) -> list[tuple[str, _Options]]: ...
 def get_regexp_pattern(regexp: str | Pattern[str]) -> str: ...
 def get_cors_origins(options: _Options, request_origin: str | None) -> list[str] | None: ...
 def get_allow_headers(options: _Options, acl_request_headers: str | None) -> str | None: ...
 def get_cors_headers(options: _Options, request_headers: dict[str, Any], request_method: str) -> _MultiDict: ...
```

### Comparing `types-Flask-Cors-3.0.8/flask_cors-stubs/decorator.pyi` & `types-Flask-Cors-3.0.9/flask_cors-stubs/decorator.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Cors-3.0.8/flask_cors-stubs/extension.pyi` & `types-Flask-Cors-3.0.9/flask_cors-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Cors-3.0.8/setup.py` & `types-Flask-Cors-3.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `Flask-Cors` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `Flask-Cors`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/Flask-Cors. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `4e946b74bf18dc932caf41d0257957d85bbabe91`.
+This package was generated from typeshed commit `9ccf4589a0cc8f0c5a8cc2c07c485da6d7118767`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.8",
+      version="3.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md",
```

### Comparing `types-Flask-Cors-3.0.8/types_Flask_Cors.egg-info/PKG-INFO` & `types-Flask-Cors-3.0.9/types_Flask_Cors.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 3.0.8
+Version: 3.0.9
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -19,10 +19,10 @@
 This is a PEP 561 type stub package for the `Flask-Cors` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `Flask-Cors`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/Flask-Cors. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `4e946b74bf18dc932caf41d0257957d85bbabe91`.
+This package was generated from typeshed commit `9ccf4589a0cc8f0c5a8cc2c07c485da6d7118767`.
```

