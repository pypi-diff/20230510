# Comparing `tmp/django_querycache-0.3.0.tar.gz` & `tmp/django_querycache-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_querycache-0.3.0.tar", max compression
+gzip compressed data, was "django_querycache-0.3.0a0.tar", max compression
```

## Comparing `django_querycache-0.3.0.tar` & `django_querycache-0.3.0a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7652 2023-04-11 07:58:42.278058 django_querycache-0.3.0/LICENSE
--rw-r--r--   0        0        0     3034 2023-05-10 03:33:24.351992 django_querycache-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-10 00:54:58.840351 django_querycache-0.3.0/django_querycache/__init__.py
--rw-r--r--   0        0        0     6168 2023-05-10 03:33:24.351992 django_querycache-0.3.0/django_querycache/cacheman.py
--rw-r--r--   0        0        0     3033 2023-05-10 00:44:46.328841 django_querycache-0.3.0/django_querycache/drf_mixins.py
--rw-r--r--   0        0        0    10408 2023-04-11 07:58:42.278058 django_querycache-0.3.0/django_querycache/fingerprinting.py
--rw-r--r--   0        0        0     2056 2023-05-10 03:33:24.351992 django_querycache-0.3.0/django_querycache/hashfunctions.py
--rw-r--r--   0        0        0     1311 2023-04-11 07:58:42.282058 django_querycache-0.3.0/django_querycache/type_annotations.py
--rw-r--r--   0        0        0     3860 2023-05-10 00:45:42.755479 django_querycache-0.3.0/django_querycache/utils.py
--rw-r--r--   0        0        0      901 2023-05-10 03:33:24.351992 django_querycache-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 django_querycache-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-04-11 07:58:42.278058 django_querycache-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0     3034 2023-05-10 01:02:06.582402 django_querycache-0.3.0a0/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 00:54:58.840351 django_querycache-0.3.0a0/django_querycache/__init__.py
+-rw-r--r--   0        0        0     6158 2023-05-10 00:44:46.348844 django_querycache-0.3.0a0/django_querycache/cacheman.py
+-rw-r--r--   0        0        0     3033 2023-05-10 00:44:46.328841 django_querycache-0.3.0a0/django_querycache/drf_mixins.py
+-rw-r--r--   0        0        0    10408 2023-04-11 07:58:42.278058 django_querycache-0.3.0a0/django_querycache/fingerprinting.py
+-rw-r--r--   0        0        0     2020 2023-05-10 00:45:16.329904 django_querycache-0.3.0a0/django_querycache/hashfunctions.py
+-rw-r--r--   0        0        0     1311 2023-04-11 07:58:42.282058 django_querycache-0.3.0a0/django_querycache/type_annotations.py
+-rw-r--r--   0        0        0     3860 2023-05-10 00:45:42.755479 django_querycache-0.3.0a0/django_querycache/utils.py
+-rw-r--r--   0        0        0      903 2023-05-10 01:03:49.564186 django_querycache-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 django_querycache-0.3.0a0/PKG-INFO
```

### Comparing `django_querycache-0.3.0/LICENSE` & `django_querycache-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_querycache-0.3.0/README.md` & `django_querycache-0.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `django_querycache-0.3.0/django_querycache/cacheman.py` & `django_querycache-0.3.0a0/django_querycache/cacheman.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     """
 
     def __init__(
         self,
         query: InputModel,
         fp: Optional[Fingerprinting] = None,
-        cache_key: Optional[str] = None,
+        cache_key: str = None,
         query_values: Iterable[Union[str, F]] = (),
         **kwargs,
     ):
         self.cache = get_query_cache(kwargs.get("cache_alias", "default"))
         self._cache_is_dummy = isinstance(caches["default"], DummyCache)
 
         self.query, self.model = inputmodel_parse(query)
```

### Comparing `django_querycache-0.3.0/django_querycache/drf_mixins.py` & `django_querycache-0.3.0a0/django_querycache/drf_mixins.py`

 * *Files identical despite different names*

### Comparing `django_querycache-0.3.0/django_querycache/fingerprinting.py` & `django_querycache-0.3.0a0/django_querycache/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `django_querycache-0.3.0/django_querycache/hashfunctions.py` & `django_querycache-0.3.0a0/django_querycache/hashfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Any  # noqa:F401
 
 from django.db import models
 from django.db.models.expressions import Func
 
 logger = logging.getLogger(__name__)
```

### Comparing `django_querycache-0.3.0/django_querycache/type_annotations.py` & `django_querycache-0.3.0a0/django_querycache/type_annotations.py`

 * *Files identical despite different names*

### Comparing `django_querycache-0.3.0/django_querycache/utils.py` & `django_querycache-0.3.0a0/django_querycache/utils.py`

 * *Files identical despite different names*

### Comparing `django_querycache-0.3.0/pyproject.toml` & `django_querycache-0.3.0a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-querycache"
-version = "0.3.0"
+version = "0.3.0a0"
 description = "Cache manager for Django querysets and serialization"
 authors = ["Joshua Brooks <josh.vdbroek@gmail.com>"]
 license = "GPLv3"
 exclude = ["django_querycache/runtests.py", "django_querycache/tests/**"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `django_querycache-0.3.0/PKG-INFO` & `django_querycache-0.3.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-querycache
-Version: 0.3.0
+Version: 0.3.0a0
 Summary: Cache manager for Django querysets and serialization
 License: GPLv3
 Author: Joshua Brooks
 Author-email: josh.vdbroek@gmail.com
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

