# Comparing `tmp/api_session-1.3.2.tar.gz` & `tmp/api_session-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_session-1.3.2.tar", max compression
+gzip compressed data, was "api_session-1.3.3.tar", max compression
```

## Comparing `api_session-1.3.2.tar` & `api_session-1.3.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1062 2022-10-13 08:59:59.776436 api_session-1.3.2/LICENSE
--rw-r--r--   0        0        0      958 2022-10-13 08:59:59.776436 api_session-1.3.2/README.md
--rw-r--r--   0        0        0     7509 2022-10-13 08:59:59.776436 api_session-1.3.2/api_session/__init__.py
--rw-r--r--   0        0        0        0 2022-10-13 08:59:59.776436 api_session-1.3.2/api_session/py.typed
--rw-r--r--   0        0        0      712 2022-10-13 08:59:59.776436 api_session-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 api_session-1.3.2/setup.py
--rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 api_session-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 16:27:51.315090 api_session-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1048 2023-05-10 16:27:51.315090 api_session-1.3.3/README.md
+-rw-r--r--   0        0        0     7684 2023-05-10 16:27:51.315090 api_session-1.3.3/api_session/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 16:27:51.315090 api_session-1.3.3/api_session/py.typed
+-rw-r--r--   0        0        0      712 2023-05-10 16:27:51.315090 api_session-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 api_session-1.3.3/PKG-INFO
```

### Comparing `api_session-1.3.2/LICENSE` & `api_session-1.3.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2021-2022 – Bixoto.com
+Copyright © 2021-2023 – Bixoto.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `api_session-1.3.2/README.md` & `api_session-1.3.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 [PyMagento]: https://github.com/Bixoto/PyMagento
 [PyBigBuy]: https://github.com/Bixoto/PyBigBuy
 
 ## Features
 
 * base URL: the base API URL is given only once on object creation; subsequent calls use `.get("/path")`
 * read-only flag: if given, prevents the API from doing `POST` and similar calls
+* offline flag: if given, prevents the API from doing any call. This is useful for tests.
 * `requests.Session` inheritance: the class inherits from `requests.Session`, so it stays 100% compatible with it
 
 ## Install
 
     pip install api-session
 
 Dependency: Python 3.8+.
```

### Comparing `api_session-1.3.2/api_session/__init__.py` & `api_session-1.3.3/api_session/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Optional, Union, Text, Dict, Any
 
 import requests
 
-__version__ = "1.3.2"
+__version__ = "1.3.3"
 
 # We can’t really do better than Any for now.
 # See https://github.com/python/typing/issues/182.
 JSONDict = Dict[str, Any]
 
 
 class APISession(requests.Session):
     """
     HTTP Session with helpers to call a JSON-based API.
     """
     READ_METHODS = {"HEAD", "GET", "OPTIONS", "CONNECT", "TRACE"}
 
     def __init__(self, base_url: str, user_agent: Optional[str] = None, read_only=False, *,
+                 offline=False,
                  none_on_404=True,
                  none_on_empty=False):
         """
         :param base_url: Base URL of the API.
         :param user_agent: Optional user-agent header to use.
         :param read_only: if True, any POST/PUT/DELETE call will fail with an AssertError.
         :param none_on_404: set the default for the argument of the same name in ``.get_json_api`` calls. This can still
@@ -27,14 +28,15 @@
         :param none_on_empty: set the default for the argument of the same name in ``.get_json_api`` calls. This can
           still be overridden by passing it explicitly when calling the method.
         """
         super().__init__()
 
         self.base_url = base_url.rstrip("/")
         self.read_only = read_only
+        self.offline = offline
         self.none_on_404 = none_on_404
         self.none_on_empty = none_on_empty
 
         if user_agent is not None:
             self.headers['User-Agent'] = user_agent
 
     # noinspection PyMethodMayBeStatic
@@ -51,14 +53,17 @@
         :param method: method argument passed to the underlying ``.request()`` method
         :param url: URL argument passed to the underlying ``.request()`` method
         :param args: arguments passed to the underlying ``.request()`` method
         :param bypass_read_only: if True, ignore the ``.read_only`` attribute
         :param kwargs: keyword arguments passed to the underlying ``.request()`` method
         :return:
         """
+        if self.offline:
+            raise AssertionError("Can't perform %r action in offline mode!" % method)
+
         if self.read_only and not bypass_read_only and method.upper() not in self.READ_METHODS:
             raise AssertionError("Can't perform %r action in read-only mode!" % method)
         return super().request(method, url, *args, **kwargs)
 
     def request_api(self, method: str, path: str, *args, throw: Optional[bool] = None, **kwargs):
         """
         Wrapper around .request() that prefixes the path with the base API URL.
```

### Comparing `api_session-1.3.2/pyproject.toml` & `api_session-1.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "api-session"
-version = "1.3.2"
+version = "1.3.3"
 description = "requests.Session to work with JSON APIs"
 authors = ["Baptiste Fontaine <baptiste@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/api-session"
 include = ["api_session/py.typed"]
 readme = "README.md"
 classifiers = [
@@ -14,15 +14,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^0"
+mypy = "^1"
 types-requests = "^2.25.9"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `api_session-1.3.2/PKG-INFO` & `api_session-1.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-session
-Version: 1.3.2
+Version: 1.3.3
 Summary: requests.Session to work with JSON APIs
 Home-page: https://github.com/Bixoto/api-session
 License: MIT
 Author: Baptiste Fontaine
 Author-email: baptiste@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,14 +30,15 @@
 [PyMagento]: https://github.com/Bixoto/PyMagento
 [PyBigBuy]: https://github.com/Bixoto/PyBigBuy
 
 ## Features
 
 * base URL: the base API URL is given only once on object creation; subsequent calls use `.get("/path")`
 * read-only flag: if given, prevents the API from doing `POST` and similar calls
+* offline flag: if given, prevents the API from doing any call. This is useful for tests.
 * `requests.Session` inheritance: the class inherits from `requests.Session`, so it stays 100% compatible with it
 
 ## Install
 
     pip install api-session
 
 Dependency: Python 3.8+.
```

