# Comparing `tmp/meilisearch_python_async-1.2.0.tar.gz` & `tmp/meilisearch_python_async-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.2.0.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.2.1.tar", max compression
```

## Comparing `meilisearch_python_async-1.2.0.tar` & `meilisearch_python_async-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/LICENSE
--rw-r--r--   0        0        0     4641 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/README.md
--rw-r--r--   0        0        0       73 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2538 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0    22123 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     1886 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    86427 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     1576 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0      392 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1285 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0      769 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11610 2023-04-17 14:11:57.547336 meilisearch_python_async-1.2.0/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2138 2023-04-17 14:11:57.551337 meilisearch_python_async-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 meilisearch_python_async-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-10 14:48:00.242952 meilisearch_python_async-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4641 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/README.md
+-rw-r--r--   0        0        0      161 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2769 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0      426 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    22123 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     1886 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    86427 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0      392 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1285 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0      769 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11610 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2184 2023-05-10 14:48:00.246943 meilisearch_python_async-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 meilisearch_python_async-1.2.1/PKG-INFO
```

### Comparing `meilisearch_python_async-1.2.0/LICENSE` & `meilisearch_python_async-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/README.md` & `meilisearch_python_async-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/_http_requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
+from functools import lru_cache
 from typing import Any, Callable
 
 from httpx import (
     AsyncClient,
     ConnectError,
     ConnectTimeout,
     HTTPError,
     RemoteProtocolError,
     Response,
 )
 
+from meilisearch_python_async._version import get_version
 from meilisearch_python_async.errors import (
     MeilisearchApiError,
     MeilisearchCommunicationError,
     MeilisearchError,
 )
 
 
@@ -23,27 +25,26 @@
         self.http_client = http_client
 
     async def _send_request(
         self,
         http_method: Callable,
         path: str,
         body: Any | None = None,
-        content_type: str = "applicaiton/json",
+        content_type: str = "applicaton/json",
     ) -> Response:
+        headers = {"user-agent": user_agent()}
         try:
             if not body:
                 response = await http_method(path)
             elif content_type != "application/json":
-                response = await http_method(
-                    path, content=body, headers={"Content-Type": content_type}
-                )
+                headers["Content-Type"] = content_type
+                response = await http_method(path, content=body, headers=headers)
             else:
-                response = await http_method(
-                    path, json=body, headers={"Content-Type": content_type}
-                )
+                headers["Content-Type"] = content_type
+                response = await http_method(path, json=body, headers=headers)
 
             response.raise_for_status()
             return response
 
         except (ConnectError, ConnectTimeout, RemoteProtocolError) as err:
             raise MeilisearchCommunicationError(str(err)) from err
         except HTTPError as err:
@@ -69,7 +70,12 @@
     async def put(
         self, path: str, body: Any | None = None, content_type: str = "application/json"
     ) -> Response:
         return await self._send_request(self.http_client.put, path, body, content_type)
 
     async def delete(self, path: str, body: dict | None = None) -> Response:
         return await self._send_request(self.http_client.delete, path, body)
+
+
+@lru_cache(maxsize=1)
+def user_agent() -> str:
+    return f"Meilisearch Python Async (v{get_version()})"
```

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/client.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/index.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/models/client.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/models/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/models/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/models/task.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/models/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/meilisearch_python_async/task.py` & `meilisearch_python_async-1.2.1/meilisearch_python_async/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.2.0/pyproject.toml` & `meilisearch_python_async-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.2.0"
+version = "1.2.1"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
@@ -40,14 +40,15 @@
 tox = ">=3.26.0"
 pytest-asyncio = ">=0.19.0"
 types-aiofiles = ">=22.1.0"
 mkdocs = ">=1.2.4"
 mkdocs-material = ">=8.2.7"
 mkdocstrings = {version = ">=0.19.0", extras = ["python"]}
 ruff = ">=0.0.259"
+tomli = {version = "2.0.1", python = "<3.11"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
```

### Comparing `meilisearch_python_async-1.2.0/PKG-INFO` & `meilisearch_python_async-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
```

