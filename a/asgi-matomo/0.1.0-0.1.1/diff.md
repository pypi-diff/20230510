# Comparing `tmp/asgi_matomo-0.1.0.tar.gz` & `tmp/asgi_matomo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.1.0.tar", max compression
+gzip compressed data, was "asgi_matomo-0.1.1.tar", max compression
```

## Comparing `asgi_matomo-0.1.0.tar` & `asgi_matomo-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.1.0/LICENSE
--rw-r--r--   0        0        0     2502 2023-04-28 08:37:33.678107 asgi_matomo-0.1.0/README.md
--rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.1.0/asgi_matomo/__init__.py
--rw-r--r--   0        0        0     5750 2023-04-28 08:26:24.958375 asgi_matomo-0.1.0/asgi_matomo/middleware.py
--rw-r--r--   0        0        0      667 2023-04-28 08:33:05.493877 asgi_matomo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3286 1970-01-01 00:00:00.000000 asgi_matomo-0.1.0/setup.py
--rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 asgi_matomo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-27 08:08:51.206959 asgi_matomo-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2656 2023-04-28 09:27:05.974228 asgi_matomo-0.1.1/README.md
+-rw-r--r--   0        0        0       84 2023-04-27 08:57:22.265099 asgi_matomo-0.1.1/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0     6041 2023-05-09 12:28:09.880325 asgi_matomo-0.1.1/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0      667 2023-05-09 12:28:55.787635 asgi_matomo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3205 1970-01-01 00:00:00.000000 asgi_matomo-0.1.1/PKG-INFO
```

### Comparing `asgi_matomo-0.1.0/LICENSE` & `asgi_matomo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.1.0/README.md` & `asgi_matomo-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # asgi-matomo
 [![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)
 [![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)
 [![Coverage](https://github.com/spraakbanken/asgi-matomo/workflows/Coverage/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACoverage)
+[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)
 
 Tracking requests with Matomo from ASGI apps.
 
 `MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.).
 
 **Installation**
```

### Comparing `asgi_matomo-0.1.0/asgi_matomo/middleware.py` & `asgi_matomo-0.1.1/asgi_matomo/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,10 +176,17 @@
             tracking_params = urllib.parse.urlencode(tracking_dict)
             tracking_url = f"{self.matomo_url}?{tracking_params}"
             logger.debug("Making tracking call", extra={"url": tracking_url})
             try:
                 if self.client is None:
                     logger.error("self.client is not set, can't track request")
                 else:
-                    _tracking_response = await self.client.get(tracking_url)
+                    tracking_response = await self.client.get(tracking_url)
+                    logger.debug(
+                        "tracking response",
+                        extra={
+                            "status": tracking_response.status_code,
+                            "content": tracking_response.text,
+                        },
+                    )
             except httpx.HTTPError:
                 logger.exception("Error tracking view")
```

### Comparing `asgi_matomo-0.1.0/pyproject.toml` & `asgi_matomo-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.1.0"
+version = "0.1.1"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "asgi_matomo"}]
 
 [tool.poetry.dependencies]
```

### Comparing `asgi_matomo-0.1.0/setup.py` & `asgi_matomo-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,116 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: asgi-matomo
+Version: 0.1.1
+Summary: Middleware for tracking ASGI reqeusts with Matomo
+License: MIT
+Author: Kristoffer Andersson
+Author-email: kristoffer.andersson@gu.se
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: asgiref (>=3.6.0,<4.0.0)
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Description-Content-Type: text/markdown
+
+# asgi-matomo
+[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)
+[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)
+[![Coverage](https://github.com/spraakbanken/asgi-matomo/workflows/Coverage/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACoverage)
+[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)
+
+Tracking requests with Matomo from ASGI apps.
+
+`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.).
+
+**Installation**
+
+```bash
+pip install asgi-matomo
+```
+
+## Examples
+
+### Starlette
+
+```python
+from starlette.applications import Starlette
+from starlette.responses import JSONResponse
+from starlette.routing import Route
+from starlette.middleware import Middleware
+
+from asgi_matomo import MatomoMiddleware
+
+async def homepage(request):
+    return JSONResponse({"data": "a" * 4000})
+
+app = Starlette(
+  routes=[Route("/", homepage)],
+  middleware=[
+    Middleware(
+      MatomoMiddleware,
+      matomo_url="YOUR MATOMO TRACKING URL",
+      idsite=12345, # your service tracking id
+  )],
+)
+```
+
+### FastAPI
+
+```python
+from fastapi import FastAPI
+from asgi_matomo import MatomoMiddleware
+
+app = FastAPI()
+app.add_middleware(
+  BrotliMiddleware,
+  matomo_url="YOUR MATOMO TRACKING URL",
+  idsite=12345, # your service tracking id
+)
+
+@app.get("/")
+def home() -> dict:
+    return {"data": "a" * 4000}
+```
+
+## API Reference
+
+**Overview**
+
+```python
+app.add_middleware(
+  MatomoMiddleware,
+  matomo_url="YOUR MATOMO TRACKING URL",
+  idsite=12345, # your service tracking id
+  access_token="SECRETTOKEN",
+  assume_https=True,
+  minimum_size=400,
+)
+```
+
+**Parameters**:
+
+- **(Required)** `matomo_url`: The URL to make your tracking calls to.
+- **(Required)** `idsite`: The tracking id for your service.
+- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.
+- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.
+
+
+**Notes**:
+
+- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.
+
+## Ideas for further work:
+- _filtering tracked of urls_
+- _custom extraction of tracked data_
 
-packages = \
-['asgi_matomo']
 
-package_data = \
-{'': ['*']}
+# Release Notes
+## Latest Changes
 
-install_requires = \
-['asgiref>=3.6.0,<4.0.0', 'httpx>=0.24.0,<0.25.0']
-
-setup_kwargs = {
-    'name': 'asgi-matomo',
-    'version': '0.1.0',
-    'description': 'Middleware for tracking ASGI reqeusts with Matomo',
-    'long_description': '# asgi-matomo\n[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)\n[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)\n[![Coverage](https://github.com/spraakbanken/asgi-matomo/workflows/Coverage/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACoverage)\n\nTracking requests with Matomo from ASGI apps.\n\n`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.).\n\n**Installation**\n\n```bash\npip install asgi-matomo\n```\n\n## Examples\n\n### Starlette\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\n\nasync def homepage(request):\n    return JSONResponse({"data": "a" * 4000})\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n### FastAPI\n\n```python\nfrom fastapi import FastAPI\nfrom asgi_matomo import MatomoMiddleware\n\napp = FastAPI()\napp.add_middleware(\n  BrotliMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n)\n\n@app.get("/")\ndef home() -> dict:\n    return {"data": "a" * 4000}\n```\n\n## API Reference\n\n**Overview**\n\n```python\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n  access_token="SECRETTOKEN",\n  assume_https=True,\n  minimum_size=400,\n)\n```\n\n**Parameters**:\n\n- **(Required)** `matomo_url`: The URL to make your tracking calls to.\n- **(Required)** `idsite`: The tracking id for your service.\n- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.\n- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.\n\n\n**Notes**:\n\n- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.\n\n## Ideas for further work:\n- _filtering tracked of urls_\n- _custom extraction of tracked data_\n\n\n# Release Notes\n## Latest Changes\n\n## 0.1.0 - 2023-04-28\n\n- Initial release.\n\n',
-    'author': 'Kristoffer Andersson',
-    'author_email': 'kristoffer.andersson@gu.se',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+## 0.1.0 - 2023-04-28
+
+- Initial release.
 
 
-setup(**setup_kwargs)
```

