# Comparing `tmp/django-querycache-0.2.3.tar.gz` & `tmp/django_querycache-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-querycache-0.2.3.tar", max compression
+gzip compressed data, was "django_querycache-0.3.0a0.tar", max compression
```

## Comparing `django-querycache-0.2.3.tar` & `django_querycache-0.3.0a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7652 2022-09-20 02:02:50.962033 django-querycache-0.2.3/LICENSE
--rw-r--r--   0        0        0        0 2022-09-20 02:02:50.962033 django-querycache-0.2.3/django_querycache/__init__.py
--rw-r--r--   0        0        0     6159 2022-09-20 02:02:50.962033 django-querycache-0.2.3/django_querycache/cacheman.py
--rw-r--r--   0        0        0     2940 2022-09-22 03:07:22.820555 django-querycache-0.2.3/django_querycache/drf_mixins.py
--rw-r--r--   0        0        0    10408 2022-09-22 03:19:57.695257 django-querycache-0.2.3/django_querycache/fingerprinting.py
--rw-r--r--   0        0        0     2043 2022-09-20 02:02:50.962033 django-querycache-0.2.3/django_querycache/hashfunctions.py
--rw-r--r--   0        0        0     1311 2022-09-20 02:02:50.962033 django-querycache-0.2.3/django_querycache/type_annotations.py
--rw-r--r--   0        0        0     3868 2022-09-22 03:03:19.673207 django-querycache-0.2.3/django_querycache/utils.py
--rw-r--r--   0        0        0      917 2022-09-22 02:22:04.156389 django-querycache-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 django-querycache-0.2.3/setup.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 django-querycache-0.2.3/PKG-INFO
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

### Comparing `django-querycache-0.2.3/LICENSE` & `django_querycache-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-querycache-0.2.3/django_querycache/cacheman.py` & `django_querycache-0.3.0a0/django_querycache/cacheman.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         self,
         query: InputModel,
         fp: Optional[Fingerprinting] = None,
         cache_key: str = None,
         query_values: Iterable[Union[str, F]] = (),
         **kwargs,
     ):
-
         self.cache = get_query_cache(kwargs.get("cache_alias", "default"))
         self._cache_is_dummy = isinstance(caches["default"], DummyCache)
 
         self.query, self.model = inputmodel_parse(query)
 
         self.query_values = query_values
```

### Comparing `django-querycache-0.2.3/django_querycache/drf_mixins.py` & `django_querycache-0.3.0a0/django_querycache/drf_mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 class AddHeadersMixin:
     def _add_headers(self: ViewsetProto, object=None) -> Tuple[Tuple[str, str], ...]:
         queryset = self.filter_queryset(self.get_queryset())  # type: QuerySet
         if object:
             queryset = queryset.filter(pk=object.pk)
 
         last_modified = last_modified_queryset(queryset)
-        etag = Fingerprinting(query=queryset, hashfields=self.serializer_class.Meta.fields).query_fingerprint()
+        etag = Fingerprinting(
+            query=queryset,
+            hashfields=self.serializer_class.Meta.fields if self.serializer_class.Meta.fields != "__all__" else (),
+        ).query_fingerprint()
 
         headers = []
         if last_modified:
             headers.append(("Last-Modified", last_modified))
         if etag:
             headers.append(("ETag", etag))
```

### Comparing `django-querycache-0.2.3/django_querycache/fingerprinting.py` & `django_querycache-0.3.0a0/django_querycache/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `django-querycache-0.2.3/django_querycache/hashfunctions.py` & `django_querycache-0.3.0a0/django_querycache/hashfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Any
 
 from django.db import models
 from django.db.models.expressions import Func
 
 logger = logging.getLogger(__name__)
```

### Comparing `django-querycache-0.2.3/django_querycache/type_annotations.py` & `django_querycache-0.3.0a0/django_querycache/type_annotations.py`

 * *Files identical despite different names*

### Comparing `django-querycache-0.2.3/django_querycache/utils.py` & `django_querycache-0.3.0a0/django_querycache/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     inputmodel
         One of: model, queryset, tuple
     Returns
     -------
     A Field instance where "auto_now" is true
     """
     _, model = inputmodel_parse(inputthing)
-    fields = model._meta.fields  # type: Sequence[Field]
+    fields: Sequence[Field] = model._meta.fields
 
     for field in fields:
         if getattr(field, "auto_now", False):
             return field
     logger.warn("No timestamp column in: %s" % ([f.name for f in fields]))
     return None
```

