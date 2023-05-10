# Comparing `tmp/dj-blacksmith-1.0.0.tar.gz` & `tmp/dj_blacksmith-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-blacksmith-1.0.0.tar", max compression
+gzip compressed data, was "dj_blacksmith-1.0.1.tar", max compression
```

## Comparing `dj-blacksmith-1.0.0.tar` & `dj_blacksmith-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1528 2022-01-28 20:27:00.710569 dj-blacksmith-1.0.0/LICENSE
--rw-r--r--   0        0        0      726 2022-02-04 07:53:44.233852 dj-blacksmith-1.0.0/README.rst
--rw-r--r--   0        0        0     1574 2022-02-12 15:46:40.062307 dj-blacksmith-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1430 2022-02-11 08:31:19.257375 dj-blacksmith-1.0.0/src/dj_blacksmith/__init__.py
--rw-r--r--   0        0        0      400 2022-02-07 20:58:25.337234 dj-blacksmith-1.0.0/src/dj_blacksmith/_settings.py
--rw-r--r--   0        0        0      252 2022-02-06 22:32:13.920545 dj-blacksmith-1.0.0/src/dj_blacksmith/apps.py
--rw-r--r--   0        0        0        0 2022-01-28 07:29:36.287116 dj-blacksmith-1.0.0/src/dj_blacksmith/client/__init__.py
--rw-r--r--   0        0        0        0 2022-01-28 07:25:25.423769 dj-blacksmith-1.0.0/src/dj_blacksmith/client/_async/__init__.py
--rw-r--r--   0        0        0     5041 2022-02-10 07:52:19.187503 dj-blacksmith-1.0.0/src/dj_blacksmith/client/_async/client.py
--rw-r--r--   0        0        0     2485 2022-02-06 22:32:13.927211 dj-blacksmith-1.0.0/src/dj_blacksmith/client/_async/middleware.py
--rw-r--r--   0        0        0     1207 2022-02-06 22:32:13.930545 dj-blacksmith-1.0.0/src/dj_blacksmith/client/_async/middleware_factory.py
--rw-r--r--   0        0        0        0 2022-02-12 15:45:53.175637 dj-blacksmith-1.0.0/src/dj_blacksmith/client/_sync/__init__.py
--rw-r--r--   0        0        0     4966 2022-02-12 15:45:54.198971 dj-blacksmith-1.0.0/src/dj_blacksmith/client/_sync/client.py
--rw-r--r--   0        0        0     2457 2022-02-12 15:45:53.648971 dj-blacksmith-1.0.0/src/dj_blacksmith/client/_sync/middleware.py
--rw-r--r--   0        0        0     1199 2022-02-12 15:45:53.178971 dj-blacksmith-1.0.0/src/dj_blacksmith/client/_sync/middleware_factory.py
--rw-r--r--   0        0        0        0 2022-01-27 22:55:13.494028 dj-blacksmith-1.0.0/src/dj_blacksmith/py.typed
--rw-r--r--   0        0        0     1683 2022-02-12 15:48:34.633911 dj-blacksmith-1.0.0/setup.py
--rw-r--r--   0        0        0     1822 2022-02-12 15:48:34.634190 dj-blacksmith-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1528 2022-01-28 20:27:00.710569 dj_blacksmith-1.0.1/LICENSE
+-rw-r--r--   0        0        0      726 2022-02-04 07:53:44.233852 dj_blacksmith-1.0.1/README.rst
+-rw-r--r--   0        0        0     1580 2023-05-10 07:05:25.166575 dj_blacksmith-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1430 2022-02-11 08:31:19.257375 dj_blacksmith-1.0.1/src/dj_blacksmith/__init__.py
+-rw-r--r--   0        0        0      400 2022-02-07 20:58:25.337234 dj_blacksmith-1.0.1/src/dj_blacksmith/_settings.py
+-rw-r--r--   0        0        0      252 2022-02-06 22:32:13.920545 dj_blacksmith-1.0.1/src/dj_blacksmith/apps.py
+-rw-r--r--   0        0        0        0 2022-01-28 07:29:36.287116 dj_blacksmith-1.0.1/src/dj_blacksmith/client/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-28 07:25:25.423769 dj_blacksmith-1.0.1/src/dj_blacksmith/client/_async/__init__.py
+-rw-r--r--   0        0        0     5041 2022-02-10 07:52:19.187503 dj_blacksmith-1.0.1/src/dj_blacksmith/client/_async/client.py
+-rw-r--r--   0        0        0     2506 2023-05-10 06:45:24.525491 dj_blacksmith-1.0.1/src/dj_blacksmith/client/_async/middleware.py
+-rw-r--r--   0        0        0     1207 2022-02-06 22:32:13.930545 dj_blacksmith-1.0.1/src/dj_blacksmith/client/_async/middleware_factory.py
+-rw-r--r--   0        0        0        0 2022-02-12 15:45:53.175637 dj_blacksmith-1.0.1/src/dj_blacksmith/client/_sync/__init__.py
+-rw-r--r--   0        0        0     4966 2023-05-10 06:45:24.525491 dj_blacksmith-1.0.1/src/dj_blacksmith/client/_sync/client.py
+-rw-r--r--   0        0        0     2478 2023-05-10 06:45:24.525491 dj_blacksmith-1.0.1/src/dj_blacksmith/client/_sync/middleware.py
+-rw-r--r--   0        0        0     1198 2023-05-10 06:45:24.525491 dj_blacksmith-1.0.1/src/dj_blacksmith/client/_sync/middleware_factory.py
+-rw-r--r--   0        0        0        0 2022-01-27 22:55:13.494028 dj_blacksmith-1.0.1/src/dj_blacksmith/py.typed
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 dj_blacksmith-1.0.1/PKG-INFO
```

### Comparing `dj-blacksmith-1.0.0/LICENSE` & `dj_blacksmith-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-blacksmith-1.0.0/README.rst` & `dj_blacksmith-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `dj-blacksmith-1.0.0/pyproject.toml` & `dj_blacksmith-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -9,39 +9,39 @@
   "Topic :: Internet :: WWW/HTTP",
 ]
 description = "Django Bindings for Blacksmith"
 homepage = "https://github.com/mardiros/dj-blacksmith"
 name = "dj-blacksmith"
 readme = "README.rst"
 repository = "https://github.com/mardiros/dj-blacksmith"
-version = "1.0.0"
+version = "1.0.1"
 
 [tool.poetry.dependencies]
 Django = ">=3.2, <=5"
-aioredis = "^2.0.1"
 blacksmith = {version = "^1.0.0", extras = ["prometheus"]}
 python = "^3.7"
-redis = "^4.1.2"
-types-setuptools = "^57.4.7"
+redis = "^4.2.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.3.2"
 black = "^22.1.0"
 django-stubs = "^1.9.0"
-esbonio = "^0.8.0"
+esbonio = "^0.13.0"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
-mypy = "^0.931"
-pytest = "^6.2.5"
-pytest-asyncio = "^0.17.2"
-pytest-cov = "^3.0.0"
+mypy = "^0.960"
+pytest = "^7.3.1"
+pytest-asyncio = "^0.21.0"
+pytest-cov = "^4.0.0"
 pytest-django = "^4.5.2"
 sphinx-rtd-theme = "^1.0.0"
 tomlkit = "^0.9.0"
 unasync = "^0.5.0"
+types-redis = "^4.5.5.0"
+types-setuptools = "^57.4.7"
 
 [tool.pytest.ini_options]
 norecursedirs = "docs"
 
 [tool.pyright]
 include = ["src"]
 # reportPrivateUsage = false
```

### Comparing `dj-blacksmith-1.0.0/src/dj_blacksmith/__init__.py` & `dj_blacksmith-1.0.1/src/dj_blacksmith/__init__.py`

 * *Files identical despite different names*

### Comparing `dj-blacksmith-1.0.0/src/dj_blacksmith/client/_async/client.py` & `dj_blacksmith-1.0.1/src/dj_blacksmith/client/_async/client.py`

 * *Files identical despite different names*

### Comparing `dj-blacksmith-1.0.0/src/dj_blacksmith/client/_async/middleware.py` & `dj_blacksmith-1.0.1/src/dj_blacksmith/client/_async/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Build Blacksmith middlewares from Django settings."""
 import abc
 from typing import Any, Mapping
 
-import aioredis
-from django.utils.module_loading import import_string
-
 from blacksmith import (
     AsyncCircuitBreakerMiddleware,
     AsyncHTTPAddHeadersMiddleware,
     AsyncHTTPBearerMiddleware,
     AsyncHTTPCacheMiddleware,
     AsyncHTTPMiddleware,
     AsyncPrometheusMiddleware,
     PrometheusMetrics,
 )
+from django.utils.module_loading import import_string
+from redis import asyncio as aioredis
 
 
 class AsyncHTTPMiddlewareBuilder(abc.ABC):
     """Build middleware from settings."""
 
     def __init__(
         self,
```

### Comparing `dj-blacksmith-1.0.0/src/dj_blacksmith/client/_async/middleware_factory.py` & `dj_blacksmith-1.0.1/src/dj_blacksmith/client/_async/middleware_factory.py`

 * *Files identical despite different names*

### Comparing `dj-blacksmith-1.0.0/src/dj_blacksmith/client/_sync/client.py` & `dj_blacksmith-1.0.1/src/dj_blacksmith/client/_sync/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Tuple, Type
 
-from blacksmith.typing import ClientName
-from django.http.request import HttpRequest
-from django.utils.module_loading import import_string
-
 from blacksmith import (
     AbstractCollectionParser,
     HTTPTimeout,
     PrometheusMetrics,
     SyncAbstractServiceDiscovery,
     SyncAbstractTransport,
     SyncClient,
     SyncClientFactory,
     SyncConsulDiscovery,
     SyncHTTPMiddleware,
     SyncRouterDiscovery,
     SyncStaticDiscovery,
 )
+from blacksmith.typing import ClientName
+from django.http.request import HttpRequest
+from django.utils.module_loading import import_string
+
 from dj_blacksmith._settings import get_clients, get_transport
 from dj_blacksmith.client._sync.middleware import SyncHTTPMiddlewareBuilder
 from dj_blacksmith.client._sync.middleware_factory import (
     SyncAbstractMiddlewareFactoryBuilder,
 )
```

### Comparing `dj-blacksmith-1.0.0/src/dj_blacksmith/client/_sync/middleware.py` & `dj_blacksmith-1.0.1/src/dj_blacksmith/client/_sync/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Build Blacksmith middlewares from Django settings."""
 import abc
 from typing import Any, Mapping
 
-import aioredis
-from django.utils.module_loading import import_string
-
 from blacksmith import (
     PrometheusMetrics,
     SyncCircuitBreakerMiddleware,
     SyncHTTPAddHeadersMiddleware,
     SyncHTTPBearerMiddleware,
     SyncHTTPCacheMiddleware,
     SyncHTTPMiddleware,
     SyncPrometheusMiddleware,
 )
+from django.utils.module_loading import import_string
+from redis import asyncio as aioredis
 
 
 class SyncHTTPMiddlewareBuilder(abc.ABC):
     """Build middleware from settings."""
 
     def __init__(
         self,
```

### Comparing `dj-blacksmith-1.0.0/src/dj_blacksmith/client/_sync/middleware_factory.py` & `dj_blacksmith-1.0.1/src/dj_blacksmith/client/_sync/middleware_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Middleware"""
 import abc
 from typing import Any, Dict, List, Mapping
 
-from django.http.request import HttpRequest
-
 from blacksmith import SyncHTTPAddHeadersMiddleware, SyncHTTPMiddleware
+from django.http.request import HttpRequest
 
 
 class SyncAbstractMiddlewareFactoryBuilder(abc.ABC):
     """Build the factory"""
 
     @abc.abstractmethod
     def __init__(self, settings: Mapping[str, Any]):
```

### Comparing `dj-blacksmith-1.0.0/PKG-INFO` & `dj_blacksmith-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: dj-blacksmith
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Bindings for Blacksmith
 Home-page: https://github.com/mardiros/dj-blacksmith
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Django (>=3.2,<=5)
-Requires-Dist: aioredis (>=2.0.1,<3.0.0)
 Requires-Dist: blacksmith[prometheus] (>=1.0.0,<2.0.0)
-Requires-Dist: redis (>=4.1.2,<5.0.0)
-Requires-Dist: types-setuptools (>=57.4.7,<58.0.0)
+Requires-Dist: redis (>=4.2.0,<5.0.0)
 Project-URL: Repository, https://github.com/mardiros/dj-blacksmith
 Description-Content-Type: text/x-rst
 
 dj-blacksmith
 =============
 
 .. image:: https://readthedocs.org/projects/dj-blacksmith/badge/?version=latest
```

