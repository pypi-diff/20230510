# Comparing `tmp/aiofauna-0.1.6.tar.gz` & `tmp/aiofauna-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.1.6.tar", max compression
+gzip compressed data, was "aiofauna-0.1.7.tar", max compression
```

## Comparing `aiofauna-0.1.6.tar` & `aiofauna-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1126 2023-05-08 06:43:22.972944 aiofauna-0.1.6/LICENSE
--rw-r--r--   0        0        0     2678 2023-05-08 04:44:25.192212 aiofauna-0.1.6/README.md
--rw-r--r--   0        0        0     3656 2023-05-08 06:40:40.439634 aiofauna-0.1.6/aiofauna/__init__.py
--rw-r--r--   0        0        0    16481 2023-05-08 06:40:40.591631 aiofauna-0.1.6/aiofauna/api.py
--rw-r--r--   0        0        0     3304 2023-05-08 02:52:55.686757 aiofauna-0.1.6/aiofauna/asgi.py
--rw-r--r--   0        0        0     7679 2023-05-08 06:40:32.547771 aiofauna-0.1.6/aiofauna/client.py
--rw-r--r--   0        0        0     3678 2023-05-08 02:23:17.855099 aiofauna-0.1.6/aiofauna/datastructures.py
--rw-r--r--   0        0        0      493 2023-05-06 09:16:36.202849 aiofauna-0.1.6/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8153 2023-05-08 02:23:18.327095 aiofauna-0.1.6/aiofauna/errors.py
--rw-r--r--   0        0        0     4056 2023-05-08 06:40:40.455633 aiofauna-0.1.6/aiofauna/helpers.py
--rw-r--r--   0        0        0     6728 2023-05-08 03:17:10.714267 aiofauna-0.1.6/aiofauna/json.py
--rw-r--r--   0        0        0     5841 2023-05-08 02:23:18.171096 aiofauna-0.1.6/aiofauna/objects.py
--rw-r--r--   0        0        0    14644 2023-05-08 16:22:07.056807 aiofauna-0.1.6/aiofauna/odm.py
--rw-r--r--   0        0        0     2672 2023-05-08 02:26:21.521409 aiofauna-0.1.6/aiofauna/page.py
--rw-r--r--   0        0        0    41561 2023-05-08 02:26:13.437479 aiofauna-0.1.6/aiofauna/query.py
--rw-r--r--   0        0        0      661 2023-05-08 16:22:26.340854 aiofauna-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3597 2023-05-08 16:22:33.585694 aiofauna-0.1.6/setup.py
--rw-r--r--   0        0        0     3697 2023-05-08 16:22:33.585963 aiofauna-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1126 2023-05-08 06:43:22.972944 aiofauna-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2678 2023-05-08 04:44:25.192212 aiofauna-0.1.7/README.md
+-rw-r--r--   0        0        0     3656 2023-05-08 06:40:40.439634 aiofauna-0.1.7/aiofauna/__init__.py
+-rw-r--r--   0        0        0    16832 2023-05-10 08:11:24.200112 aiofauna-0.1.7/aiofauna/api.py
+-rw-r--r--   0        0        0     3304 2023-05-08 02:52:55.686757 aiofauna-0.1.7/aiofauna/asgi.py
+-rw-r--r--   0        0        0     7679 2023-05-08 06:40:32.547771 aiofauna-0.1.7/aiofauna/client.py
+-rw-r--r--   0        0        0     3678 2023-05-08 02:23:17.855099 aiofauna-0.1.7/aiofauna/datastructures.py
+-rw-r--r--   0        0        0      493 2023-05-06 09:16:36.202849 aiofauna-0.1.7/aiofauna/deprecated.py
+-rw-r--r--   0        0        0     8153 2023-05-08 02:23:18.327095 aiofauna-0.1.7/aiofauna/errors.py
+-rw-r--r--   0        0        0     4056 2023-05-08 06:40:40.455633 aiofauna-0.1.7/aiofauna/helpers.py
+-rw-r--r--   0        0        0     6728 2023-05-08 03:17:10.714267 aiofauna-0.1.7/aiofauna/json.py
+-rw-r--r--   0        0        0     5841 2023-05-08 02:23:18.171096 aiofauna-0.1.7/aiofauna/objects.py
+-rw-r--r--   0        0        0    14644 2023-05-08 16:22:07.056807 aiofauna-0.1.7/aiofauna/odm.py
+-rw-r--r--   0        0        0     2672 2023-05-08 02:26:21.521409 aiofauna-0.1.7/aiofauna/page.py
+-rw-r--r--   0        0        0    41561 2023-05-08 02:26:13.437479 aiofauna-0.1.7/aiofauna/query.py
+-rw-r--r--   0        0        0      661 2023-05-10 08:02:31.870474 aiofauna-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3597 2023-05-10 08:11:32.956275 aiofauna-0.1.7/setup.py
+-rw-r--r--   0        0        0     3697 2023-05-10 08:11:32.957198 aiofauna-0.1.7/PKG-INFO
```

### Comparing `aiofauna-0.1.6/LICENSE` & `aiofauna-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/README.md` & `aiofauna-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/__init__.py` & `aiofauna-0.1.7/aiofauna/__init__.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/api.py` & `aiofauna-0.1.7/aiofauna/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from uuid import UUID
 from datetime import datetime, date, time
 from functools import singledispatch
 from enum import Enum
 from aiohttp.web import Application, Request, Response, json_response
 from json import JSONDecoder
 from aiohttp.web_request import FileField
+from aiohttp_sse import EventSourceResponse
 from .odm import AsyncFaunaModel
 from pydantic import BaseModel  # pylint: disable=no-name-in-module
 from .json import FaunaJSONEncoder as JSONEncoder, to_json, parse_json_or_none
 
 
 def jsonable_encoder(
     obj,
@@ -348,14 +349,24 @@
 
 class Api(Application):
     """
 
     Api class to create a fastapi-like api.
 
     """
+    
+    @property
+    def state(self) -> Dict[str,EventSourceResponse]:
+        return {}
+    
+    async def set_state(self, key: str, value: EventSourceResponse) -> None:
+        if key in self.state:
+            self.state[key] = value
+        else:
+            self.state.update({key:value})
 
     title: str = "aiofauna"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.openapi = {
             "openapi": "3.0.0",
```

### Comparing `aiofauna-0.1.6/aiofauna/asgi.py` & `aiofauna-0.1.7/aiofauna/asgi.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/client.py` & `aiofauna-0.1.7/aiofauna/client.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/datastructures.py` & `aiofauna-0.1.7/aiofauna/datastructures.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/errors.py` & `aiofauna-0.1.7/aiofauna/errors.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/helpers.py` & `aiofauna-0.1.7/aiofauna/helpers.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/json.py` & `aiofauna-0.1.7/aiofauna/json.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/objects.py` & `aiofauna-0.1.7/aiofauna/objects.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/odm.py` & `aiofauna-0.1.7/aiofauna/odm.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/page.py` & `aiofauna-0.1.7/aiofauna/page.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/aiofauna/query.py` & `aiofauna-0.1.7/aiofauna/query.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.1.6/pyproject.toml` & `aiofauna-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiofauna"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Oscar Bahamonde <oscar.bahamonde.dev@gmail.com>"]
 repository = "https://github.com/obahamonde/aiofauna"
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `aiofauna-0.1.6/setup.py` & `aiofauna-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'aiohttp>=3.8.4,<4.0.0',
  'aiohttp_cors>=0.7.0,<0.8.0',
  'iso8601>=1.1.0,<2.0.0',
  'pydantic[dotenv]>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'aiofauna',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': '',
     'long_description': '---\ntitle: AioFauna\n---\n# AioFauna\n\n🚀 Introducing aiofauna: A full-stack framework built on top of Aiohttp, Pydantic and FaunaDB.\n\n🔥 Inspired by FastAPI focuses on Developer Experience, Productivity and Versatility.\n\n🌟 Features:\n\n✅ Supports Python 3.7+, comes with an opinionated ODM (Object Document Mapper) out of the box for FaunaDB that abstracts out complex FQL expressions into pythonic, fully typed asynchronous methods for all CRUD operations.\n\n✅ Performant and scalable: Built on top of Aiohttp a powerful http server and client and FaunaDB an scalable serverless database for modern applications.\n\n✅ Async/await coroutines: Leverage the power of async programming for enhanced performance and responsiveness, being ASGI compliant is compatible with most async python frameworks.\n\n✅ Automatic Swagger UI generation: Automatic generation of interactive Swagger UI documentation for instant testing of your API.\n\n✅ SSE (Server Sent Events): Built-in support for SSE (Server Sent Events) for real-time streaming of data from FaunaDB to your application.\n\n✅ Robust data validation: Built-in support for Pydantic models for robust data validation and serialization.\n\n✅ Auto-provisioning: Automatic management of indexes, unique indexes, and collections with FaunaModel ODM.\n\n✅ Full JSON communication: Custom encoder to ensure seamless data exchange between your application and FaunaDB backend.\n\n✅ Markdown and Jinja support with live reload: experiment an smooth frontend devserver experience without leaving your backend code.\n\n✅ Inspired by fastapi, you will work with almost the same syntax and features like path operations, path parameters, query parameters, request body, status codes and more.\n\n💡 With aiofauna, you can build fast, scalable, and reliable modern applications, while building seamless integrations thanks to the fastest http client aiohttp and the most versatile database FaunaDB, you will enjoy integrating with third party services such as APIs, Data Sources and Cloud Services.\n\n📚 Check out the aiofauna library, and start building your next-gen applications today! 🚀\n\n#Python #FaunaDB #Async #Pydantic #aiofauna\n\n⚙️ If you are using a synchronous framework check out [Faudantic](https://github.com/obahamonde/faudantic) for a similar experience with FaunaDB and Pydantic.\n\n📚 [Documentation](https://obahamonde-aiofauna-docs.smartpro.solutions) (Built with aiofauna)\n\n📦 [PyPi](https://pypi.org/project/aiofauna/)\n\n📦 [GitHub](https://github.com/obahamonde/aiofauna)\n\n📦 [Demo](https://aiofaunastreams-fwuw7gz7oq-uc.a.run.app/) (Real time Latency Monitoring between FaunaDB and Google Cloud Run)\n',
     'author': 'Oscar Bahamonde',
     'author_email': 'oscar.bahamonde.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/obahamonde/aiofauna',
```

### Comparing `aiofauna-0.1.6/PKG-INFO` & `aiofauna-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiofauna
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/obahamonde/aiofauna
 License: MIT
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde.dev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

