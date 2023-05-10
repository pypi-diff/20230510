# Comparing `tmp/merqube_client_lib-0.5.3.tar.gz` & `tmp/merqube_client_lib-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.5.3.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.5.4.tar", max compression
```

## Comparing `merqube_client_lib-0.5.3.tar` & `merqube_client_lib-0.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/LICENSE
--rw-r--r--   0        0        0      377 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/README.md
--rw-r--r--   0        0        0        0 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      367 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     3028 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/py.typed
--rw-r--r--   0        0        0        0 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0    12490 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/secapi/client.py
--rw-r--r--   0        0        0    11209 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0      677 2023-05-08 16:36:12.892175 merqube_client_lib-0.5.3/merqube_client_lib/util.py
--rw-r--r--   0        0        0     1713 2023-05-08 16:36:12.896175 merqube_client_lib-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/LICENSE
+-rw-r--r--   0        0        0      377 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      367 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     3028 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0        0 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    12490 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/secapi/client.py
+-rw-r--r--   0        0        0    11754 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-10 17:25:12.597588 merqube_client_lib-0.5.4/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1713 2023-05-10 17:25:12.601589 merqube_client_lib-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.4/PKG-INFO
```

### Comparing `merqube_client_lib-0.5.3/LICENSE` & `merqube_client_lib-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.3/merqube_client_lib/logging.py` & `merqube_client_lib-0.5.4/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.3/merqube_client_lib/mocker.py` & `merqube_client_lib-0.5.4/merqube_client_lib/mocker.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.3/merqube_client_lib/secapi/client.py` & `merqube_client_lib-0.5.4/merqube_client_lib/secapi/client.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.3/merqube_client_lib/session.py` & `merqube_client_lib-0.5.4/merqube_client_lib/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Merqube API Session - subcomponent of the client library wrapper
 """
 
 
 import json
 import os
 import uuid
-from typing import Any, Optional, Union, cast
+from typing import Any, Optional, cast
 from urllib.parse import urljoin
 
 from cachetools import LRUCache, cached
 from requests import PreparedRequest, Response, Session
 from requests.adapters import HTTPAdapter
 from requests.exceptions import HTTPError
 from urllib3.util.retry import Retry
@@ -54,24 +54,23 @@
         backoff_factor: float = 0.3,
         status_forcelist: tuple[int, ...] = (502, 504),  # status codes to retry on
         allowed_methods: list[str] = ["GET"],  # methods to retry on
         request_timeout: int | None = None,
     ):
         super().__init__()
         """
-        By default, this session only retries on GET
-
-        DELETE and POST are idempotent, and should be safe to add to the allowed methods list (note though, lost ACKs could change the status code - eg a lost ack on a 200 POST may result in a 409 DUPLICATE being eventually returned, however return codes are not a part of idempotency)
-
-        PUT is sometimes idempotent, but not in some of our APIs; for example we often have a "status" key that must be supplied - two subsequent PUTs will not work
-        in our APIs, to "update twice", you must do PUT GET PUT
-
-        see https://developer.mozilla.org/en-US/docs/Glossary/Idempotent
-        https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#urllib3.util.Retry.DEFAULT_ALLOWED_METHODS
-        https://restfulapi.net/idempotent-rest-apis/
+        By default, this session only retries on GET, but you may enable for DELETE, POST, and PUT as well. 
+        Note that when considering idempotency, only the server state is considered, not the client state.
+        See https://developer.mozilla.org/en-US/docs/Glossary/Idempotent
+
+        In our APIs, DELETE, POST, and PUT are all idempotent with respect to the server state.
+
+        However, from the client side, e.g., a lost ACK on a POST may result in a 409 DUPLICATE being returned.
+        Similarly, a lost ACK on DELETE may result in a 404 NOT FOUND being returned.
+        Finally, from the client side, for the majority of our APIs, two subsequent PUTs will not work due to the status key; you must do PUT GET PUT
         """
         for allowed in allowed_methods:
             assert allowed in HTTP_METHODS, f"Should be a valid http method: {', '.join(HTTP_METHODS)}"
 
         if allowed_methods:
             retry = Retry(
                 total=retries,
@@ -133,42 +132,61 @@
 
     def __exit__(self, exc_type: str, exc_val: Any, exc_tb: Any) -> None:
         self.close()
 
     def request(
         self,
         method: httpm,
-        url: Union[str, bytes],
+        url: str,
         params: dict[str, Any] | None = None,
         data: Any = None,
         headers: dict[str, str] | None = None,
         options: dict[str, str] | None = None,
         **kwargs: Any,
     ) -> Response:
         """
         Perform an http request with this session
         request session helpers sess.put, sess.get, etc, call this
+
+        Note: urljoin has some perhaps non obvious behavior:
+
+            In [2]: from urllib.parse import urljoin
+
+            In [3]: urljoin("https://localhost:8080", "resource")
+            Out[3]: 'https://localhost:8080/resource'
+
+            In [4]: urljoin("https://localhost:8080", "/resource")
+            Out[4]: 'https://localhost:8080/resource'
+
+            In [5]: urljoin("https://localhost:8080/", "/resource")
+            Out[5]: 'https://localhost:8080/resource'
+
+            In [6]: urljoin("https://localhost:8080", "//resource")
+            Out[6]: 'https://resource' # ??
         """
         assert params is None or options is None, "both params and options cannot be passed"
+        if url.startswith("//"):
+            logger.warning(f"URL {url} starts with //, this is probably a mistake")
 
         headers = dict(headers) if headers is not None else {}
 
         # Generate a new requestid if this call isnt being made in a chain that already has it.
         # (eg client calls dataapi, dataapi calls secapi - we dont want the second call to overwrite the original)
         # if this isnt set by a client making a call to one of our APIs, the API itself will generate one (eg customer call)
         # order is: 1) explicitly specified 2) set via chain, 3) generate new
         headers[REQUEST_ID_HEADER] = headers.get(
             REQUEST_ID_HEADER, os.getenv(MERQ_REQUEST_ID_ENV_VAR, str(uuid.uuid4()))
         )
 
         if self.token:
             headers["Authorization"] = f"{self.token_type} {self.token}"
 
-        url = urljoin(self._prefix_url, cast(str, url))
-
+        options_st = "" if not options else ("?" + "&".join([f"{k}={v}" for k, v in options.items()]))
+        url = urljoin(self._prefix_url, url)
+        logger.debug(f"Performing {method} on {url}{options_st}")
         options_dict: dict[str, str] = options or {}
         return self.http_session.request(
             method=method.value, url=url, params=options_dict or params, data=data, headers=headers, **kwargs
         )
 
     def get(self, url: str, **kwargs: Any) -> Response:
         """
@@ -227,17 +245,14 @@
         except (AttributeError, json.decoder.JSONDecodeError):
             rj = {}
         logger.debug(f"Request failed with status {res.status_code}: {rj}")
         raise APIError(code=res.status_code, response_json=rj)
 
     def request_raise(self, method: httpm, url: str, **kwargs: Any) -> Response:
         """request method that logs the status code and raises on non 2XX"""
-        options = kwargs.get("options")
-        options_st = "?" + "&".join([f"{k}={v}" for k, v in options.items()]) if options else ""
-        logger.debug(f"Performing {method} on {self._prefix_url}{url}{options_st}")
         res = self.request(method, url, **kwargs)
         try:
             res.raise_for_status()
         except HTTPError as e:
             self.handle_nonrecoverable(res, e)
 
         return res
```

### Comparing `merqube_client_lib-0.5.3/merqube_client_lib/util.py` & `merqube_client_lib-0.5.4/merqube_client_lib/util.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.5.3/pyproject.toml` & `merqube_client_lib-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.5.3"
+version = "0.5.4"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
```

### Comparing `merqube_client_lib-0.5.3/PKG-INFO` & `merqube_client_lib-0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.5.3
+Version: 0.5.4
 Summary: MerQube IndexAPI + SecAPI client library
 Home-page: https://github.com/merqube/merqube-client-lib
 License: Apache-2.0
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

