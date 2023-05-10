# Comparing `tmp/fastapi_querysets-0.1.1.tar.gz` & `tmp/fastapi_querysets-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_querysets-0.1.1.tar", max compression
+gzip compressed data, was "fastapi_querysets-0.1.2.tar", max compression
```

## Comparing `fastapi_querysets-0.1.1.tar` & `fastapi_querysets-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0        0 2023-01-04 14:32:42.964508 fastapi_querysets-0.1.1/fastapi_querysets/__init__.py
--rw-r--r--   0        0        0      704 2023-01-04 14:39:24.760485 fastapi_querysets-0.1.1/fastapi_querysets/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-04 14:32:42.973791 fastapi_querysets-0.1.1/fastapi_querysets/mixins/__init__.py
--rw-r--r--   0        0        0     2614 2023-02-04 13:22:58.000652 fastapi_querysets-0.1.1/fastapi_querysets/mixins/filters.py
--rw-r--r--   0        0        0     1605 2023-02-04 11:52:14.760085 fastapi_querysets-0.1.1/fastapi_querysets/mixins/ordering.py
--rw-r--r--   0        0        0     2066 2023-02-04 11:52:14.760085 fastapi_querysets-0.1.1/fastapi_querysets/mixins/pagination.py
--rw-r--r--   0        0        0     1759 2023-02-04 11:52:14.760085 fastapi_querysets-0.1.1/fastapi_querysets/queryset.py
--rw-r--r--   0        0        0     1085 2022-12-25 08:20:56.625775 fastapi_querysets-0.1.1/LICENSE
--rw-r--r--   0        0        0     1501 2023-02-04 14:06:38.792771 fastapi_querysets-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6871 2023-02-04 13:55:58.597025 fastapi_querysets-0.1.1/README.md
--rw-r--r--   0        0        0     7586 1970-01-01 00:00:00.000000 fastapi_querysets-0.1.1/setup.py
--rw-r--r--   0        0        0     7518 1970-01-01 00:00:00.000000 fastapi_querysets-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-10 15:11:47.299610 fastapi_querysets-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6610 2023-05-10 15:11:47.299610 fastapi_querysets-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:11:47.303610 fastapi_querysets-0.1.2/fastapi_querysets/__init__.py
+-rw-r--r--   0        0        0      678 2023-05-10 15:11:47.303610 fastapi_querysets-0.1.2/fastapi_querysets/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-10 15:11:47.303610 fastapi_querysets-0.1.2/fastapi_querysets/mixins/__init__.py
+-rw-r--r--   0        0        0     2543 2023-05-10 15:11:47.303610 fastapi_querysets-0.1.2/fastapi_querysets/mixins/filters.py
+-rw-r--r--   0        0        0     1559 2023-05-10 15:11:47.303610 fastapi_querysets-0.1.2/fastapi_querysets/mixins/ordering.py
+-rw-r--r--   0        0        0     2014 2023-05-10 15:11:47.303610 fastapi_querysets-0.1.2/fastapi_querysets/mixins/pagination.py
+-rw-r--r--   0        0        0     1703 2023-05-10 15:15:26.073901 fastapi_querysets-0.1.2/fastapi_querysets/queryset.py
+-rw-r--r--   0        0        0     1437 2023-05-10 15:22:56.078842 fastapi_querysets-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7516 1970-01-01 00:00:00.000000 fastapi_querysets-0.1.2/PKG-INFO
```

### Comparing `fastapi_querysets-0.1.1/fastapi_querysets/exceptions.py` & `fastapi_querysets-0.1.2/fastapi_querysets/exceptions.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Final
-from typing import List
-
-from fastapi import HTTPException
-
-ERROR_INTEGER: Final = "type_error.integer"
-ERROR_DOES_NOT_EXIST: Final = "does_not_exist"
-ERROR_PERMISSION_DENIED: Final = "permission_denied"
-ERROR_UNIQUE: Final = "not_unique"
-
-
-def create_validation_detail(msg: str, loc: List[str], _type: str = "type_error.integer"):
-    return {
-        "loc": loc,
-        "msg": msg,
-        "type": _type,
-    }
-
-
-def create_validation_exception(
-    msg: str,
-    loc: List[str],
-    status_code: int = 422,
-    _type: str = ERROR_INTEGER,
-) -> HTTPException:
-    return HTTPException(status_code, detail=[create_validation_detail(msg, loc, _type)])
+from typing import Final
+from typing import List
+
+from fastapi import HTTPException
+
+ERROR_INTEGER: Final = "type_error.integer"
+ERROR_DOES_NOT_EXIST: Final = "does_not_exist"
+ERROR_PERMISSION_DENIED: Final = "permission_denied"
+ERROR_UNIQUE: Final = "not_unique"
+
+
+def create_validation_detail(msg: str, loc: List[str], _type: str = "type_error.integer"):
+    return {
+        "loc": loc,
+        "msg": msg,
+        "type": _type,
+    }
+
+
+def create_validation_exception(
+    msg: str,
+    loc: List[str],
+    status_code: int = 422,
+    _type: str = ERROR_INTEGER,
+) -> HTTPException:
+    return HTTPException(status_code, detail=[create_validation_detail(msg, loc, _type)])
```

### Comparing `fastapi_querysets-0.1.1/fastapi_querysets/mixins/filters.py` & `fastapi_querysets-0.1.2/fastapi_querysets/mixins/filters.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import copy
-import dataclasses
-from typing import Any
-from typing import Callable
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Protocol
-from typing import Tuple
-
-from fastapi_depends_ext import DependsAttr
-from pydantic.fields import FieldInfo
-from starlette.requests import Request
-from tortoise.queryset import QuerySet
-
-
-class DataclassProtocol(Protocol):
-    __dataclass_fields__: Dict
-    __dataclass_params__: Dict
-    __post_init__: Optional[Callable]
-
-
-class BaseFilterMixin:
-    def _get_model_filters(self, request: Request, filters: DataclassProtocol) -> Dict[str, Any]:
-        fields_map = {field.default.alias or field.name: field.name for field in dataclasses.fields(filters)}
-        _fields = set(request.query_params) & set(fields_map)
-        return {fields_map[field]: getattr(filters, fields_map[field]) for field in _fields}
-
-
-class FilterNegationMixin(BaseFilterMixin):
-    # todo: allow to configure exclude_class directly
-    filter_class: DataclassProtocol
-
-    @property
-    def exclude_class(self) -> type:
-        # todo: dedicate method to create NegationClass from dataclass
-        fields: List[Tuple[str, type, dataclasses.Field]] = []
-        for field in dataclasses.fields(self.filter_class):
-            _field = copy.copy(field)
-            if isinstance(_field.default, FieldInfo):
-                _field.default = copy.copy(_field.default)
-                _field.default.alias = f"{_field.default.alias or _field.name}!"
-
-            fields.append((_field.name, _field.type, _field))
-
-        return dataclasses.make_dataclass(f"{self.filter_class.__name__}Negation", fields=fields, frozen=True)
-
-    def get_request_queryset(
-        self,
-        request: Request,
-        exclude: DataclassProtocol = DependsAttr("exclude_class"),
-        queryset: QuerySet = DependsAttr("get_request_queryset", from_super=True),
-    ) -> QuerySet:
-        if model_exclude := self._get_model_filters(request, exclude):
-            queryset = queryset.exclude(**model_exclude)
-        return queryset
-
-
-class FilterMixin(BaseFilterMixin):
-    filter_class: DataclassProtocol
-
-    def get_request_queryset(
-        self,
-        request: Request,
-        filters: DataclassProtocol = DependsAttr("filter_class"),
-        queryset: QuerySet = DependsAttr("get_request_queryset", from_super=True),
-    ) -> QuerySet:
-
-        if model_filters := self._get_model_filters(request, filters):
-            queryset = queryset.filter(**model_filters)
-        return queryset
+import copy
+import dataclasses
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Protocol
+from typing import Tuple
+
+from fastapi_depends_ext import DependsAttr
+from pydantic.fields import FieldInfo
+from starlette.requests import Request
+from tortoise.queryset import QuerySet
+
+
+class DataclassProtocol(Protocol):
+    __dataclass_fields__: Dict
+    __dataclass_params__: Dict
+    __post_init__: Optional[Callable]
+
+
+class BaseFilterMixin:
+    def _get_model_filters(self, request: Request, filters: DataclassProtocol) -> Dict[str, Any]:
+        fields_map = {field.default.alias or field.name: field.name for field in dataclasses.fields(filters)}
+        _fields = set(request.query_params) & set(fields_map)
+        return {fields_map[field]: getattr(filters, fields_map[field]) for field in _fields}
+
+
+class FilterNegationMixin(BaseFilterMixin):
+    # todo: allow to configure exclude_class directly
+    filter_class: DataclassProtocol
+
+    @property
+    def exclude_class(self) -> type:
+        # todo: dedicate method to create NegationClass from dataclass
+        fields: List[Tuple[str, type, dataclasses.Field]] = []
+        for field in dataclasses.fields(self.filter_class):
+            _field = copy.copy(field)
+            if isinstance(_field.default, FieldInfo):
+                _field.default = copy.copy(_field.default)
+                _field.default.alias = f"{_field.default.alias or _field.name}!"
+
+            fields.append((_field.name, _field.type, _field))
+
+        return dataclasses.make_dataclass(f"{self.filter_class.__name__}Negation", fields=fields, frozen=True)
+
+    def get_request_queryset(
+        self,
+        request: Request,
+        exclude: DataclassProtocol = DependsAttr("exclude_class"),
+        queryset: QuerySet = DependsAttr("get_request_queryset", from_super=True),
+    ) -> QuerySet:
+        if model_exclude := self._get_model_filters(request, exclude):
+            queryset = queryset.exclude(**model_exclude)
+        return queryset
+
+
+class FilterMixin(BaseFilterMixin):
+    filter_class: DataclassProtocol
+
+    def get_request_queryset(
+        self,
+        request: Request,
+        filters: DataclassProtocol = DependsAttr("filter_class"),
+        queryset: QuerySet = DependsAttr("get_request_queryset", from_super=True),
+    ) -> QuerySet:
+
+        if model_filters := self._get_model_filters(request, filters):
+            queryset = queryset.filter(**model_filters)
+        return queryset
```

### Comparing `fastapi_querysets-0.1.1/fastapi_querysets/mixins/ordering.py` & `fastapi_querysets-0.1.2/fastapi_querysets/mixins/ordering.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import List
-from typing import Optional
-from typing import Sequence
-from typing import Union
-
-from fastapi import Query
-from fastapi_depends_ext import DependsAttr
-from starlette import status
-from tortoise.queryset import QuerySet
-
-from fastapi_querysets.exceptions import create_validation_exception
-
-
-QUERY_ORDERING = List[str]
-
-
-class OrderingMixin:
-    ordering_default: Union[Sequence[str], str] = None
-    ordering_fields: Sequence[str] = tuple()
-
-    def get_request_queryset(
-        self,
-        ordering: Optional[QUERY_ORDERING] = Query(None, alias="ordering[]"),
-        queryset: QuerySet = DependsAttr("get_request_queryset", from_super=True),
-    ) -> QuerySet:
-        if ordering:
-            # todo: allow to patch method typing to remove custom error
-            for index, field in enumerate(ordering):
-                if field.replace("-", "") not in self.ordering_fields:
-                    raise create_validation_exception(
-                        status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-                        loc=["query", "ordering[]", index],
-                        msg="Invalid value",
-                        _type="value_error",
-                    )
-
-            queryset = queryset.order_by(*ordering)
-            return queryset
-
-        elif isinstance(self.ordering_default, str):
-            return queryset.order_by(self.ordering_default)
-
-        elif isinstance(self.ordering_default, (list, tuple, set)):
-            return queryset.order_by(*self.ordering_default)
-
-        return queryset
+from typing import List
+from typing import Optional
+from typing import Sequence
+from typing import Union
+
+from fastapi import Query
+from fastapi_depends_ext import DependsAttr
+from starlette import status
+from tortoise.queryset import QuerySet
+
+from fastapi_querysets.exceptions import create_validation_exception
+
+
+QUERY_ORDERING = List[str]
+
+
+class OrderingMixin:
+    ordering_default: Union[Sequence[str], str] = None
+    ordering_fields: Sequence[str] = tuple()
+
+    def get_request_queryset(
+        self,
+        ordering: Optional[QUERY_ORDERING] = Query(None, alias="ordering[]"),
+        queryset: QuerySet = DependsAttr("get_request_queryset", from_super=True),
+    ) -> QuerySet:
+        if ordering:
+            # todo: allow to patch method typing to remove custom error
+            for index, field in enumerate(ordering):
+                if field.replace("-", "") not in self.ordering_fields:
+                    raise create_validation_exception(
+                        status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                        loc=["query", "ordering[]", index],
+                        msg="Invalid value",
+                        _type="value_error",
+                    )
+
+            queryset = queryset.order_by(*ordering)
+            return queryset
+
+        elif isinstance(self.ordering_default, str):
+            return queryset.order_by(self.ordering_default)
+
+        elif isinstance(self.ordering_default, (list, tuple, set)):
+            return queryset.order_by(*self.ordering_default)
+
+        return queryset
```

### Comparing `fastapi_querysets-0.1.1/fastapi_querysets/mixins/pagination.py` & `fastapi_querysets-0.1.2/fastapi_querysets/mixins/pagination.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import math
-from collections import namedtuple
-from typing import Type
-from typing import cast
-
-from fastapi import Depends
-from fastapi import Query
-from fastapi_depends_ext import DependsAttr
-from starlette.responses import Response
-from tortoise.queryset import QuerySet
-
-
-Pagination = namedtuple("SkipLimit", "skip limit")
-
-
-class RouterPagination:
-    per_page_max: int = 25
-    per_page: int = 25
-
-    def __init__(self, per_page_max: int = None, per_page: int = None):
-        self.per_page_max = per_page_max or self.per_page_max
-        self.per_page = per_page or self.per_page
-
-    def __call__(self, page: int = Query(1, ge=1), per_page: int = Query(None, ge=1)) -> Pagination:
-        """Return value is tuple of (skip, limit)"""
-        per_page = min(self.per_page_max, per_page or self.per_page)
-        return Pagination(skip=(page - 1) * per_page, limit=per_page)
-
-
-class PaginationMixin:
-    # todo: add per_page_min
-    pagination_class: Type[RouterPagination]
-
-    def __init__(self, *args, per_page_max: int = None, per_page: int = None, **kwargs):
-        self._pagination = self.pagination_class(per_page_max=per_page_max, per_page=per_page)
-        super(PaginationMixin, self).__init__(*args, **kwargs)
-        self.paginated = Depends(self.get_request_queryset_paginated)
-
-    async def get_request_queryset_paginated(
-        self,
-        response: Response,
-        queryset: QuerySet = DependsAttr("get_request_queryset"),
-        pagination: Pagination = DependsAttr("_pagination"),
-    ) -> QuerySet:
-        total = await queryset.count()
-        response.headers["x-page"] = str(math.ceil(pagination.skip / pagination.limit) + 1)
-        response.headers["x-pages"] = str(math.ceil(total / pagination.limit))
-        response.headers["x-per-page"] = str(pagination.limit)
-        response.headers["x-total"] = str(total)
-
-        # todo: refactor to yield queryset and the adding pagination info
-        return queryset.offset(cast(int, pagination.skip)).limit(pagination.limit)
+import math
+from collections import namedtuple
+from typing import Type
+from typing import cast
+
+from fastapi import Depends
+from fastapi import Query
+from fastapi_depends_ext import DependsAttr
+from starlette.responses import Response
+from tortoise.queryset import QuerySet
+
+
+Pagination = namedtuple("SkipLimit", "skip limit")
+
+
+class RouterPagination:
+    per_page_max: int = 25
+    per_page: int = 25
+
+    def __init__(self, per_page_max: int = None, per_page: int = None):
+        self.per_page_max = per_page_max or self.per_page_max
+        self.per_page = per_page or self.per_page
+
+    def __call__(self, page: int = Query(1, ge=1), per_page: int = Query(None, ge=1)) -> Pagination:
+        """Return value is tuple of (skip, limit)"""
+        per_page = min(self.per_page_max, per_page or self.per_page)
+        return Pagination(skip=(page - 1) * per_page, limit=per_page)
+
+
+class PaginationMixin:
+    # todo: add per_page_min
+    pagination_class: Type[RouterPagination]
+
+    def __init__(self, *args, per_page_max: int = None, per_page: int = None, **kwargs):
+        self._pagination = self.pagination_class(per_page_max=per_page_max, per_page=per_page)
+        super(PaginationMixin, self).__init__(*args, **kwargs)
+        self.paginated = Depends(self.get_request_queryset_paginated)
+
+    async def get_request_queryset_paginated(
+        self,
+        response: Response,
+        queryset: QuerySet = DependsAttr("get_request_queryset"),
+        pagination: Pagination = DependsAttr("_pagination"),
+    ) -> QuerySet:
+        total = await queryset.count()
+        response.headers["x-page"] = str(math.ceil(pagination.skip / pagination.limit) + 1)
+        response.headers["x-pages"] = str(math.ceil(total / pagination.limit))
+        response.headers["x-per-page"] = str(pagination.limit)
+        response.headers["x-total"] = str(total)
+
+        # todo: refactor to yield queryset and the adding pagination info
+        return queryset.offset(cast(int, pagination.skip)).limit(pagination.limit)
```

### Comparing `fastapi_querysets-0.1.1/LICENSE` & `fastapi_querysets-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Nikakto
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Nikakto
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `fastapi_querysets-0.1.1/pyproject.toml` & `fastapi_querysets-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-[tool.poetry]
-name = "fastapi-querysets"
-version = "0.1.1"
-description = ""
-authors = ["Nikakto <black-z@bk.ru>"]
-license = "MIT"
-readme = "README.md"
-repository = "https://github.com/Nikakto/fastapi-querysets"
-documentation = "https://fastapi-querysets.readthedocs.io"
-keywords = ["fastapi", "filters", "filtering", "pagination", "order", "ordering", "queryset", "Tortoise", "orm", "database", "db"]
-
-[tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-fastapi = ">=0.70.0"
-tortoise-orm = ">=0.18.1"
-fastapi-depends-ext = ">=0.2.2"
-
-[tool.poetry.dev-dependencies]
-httpx = "^0.23.1"
-black = "^22.12.0"
-pytest = "^7.2.0"
-pytest-asyncio = "^0.20.3"
-pytest-mock = "^3.10.0"
-nest-asyncio = "^1.5.6"
-ipython = "^8.7.0"
-pytest-cov = "^4.0.0"
-
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
-Jinja2 = "3.0.*"
-mkdocs-material = "^9.0.5"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-asyncio_mode = "auto"
-
-[tool.black]
-line-length = 120
-target-version = ['py39']
-include = '\.pyi?$'
-exclude = '''
-
-(
-  /(
-      \.eggs         # exclude a few common directories in the
-    | \.git          # root of the project
-    | \.hg
-    | \.mypy_cache
-    | \.tox
-    | \.venv
-    | _build
-    | buck-out
-    | build
-    | dist
-  )/
-  | foo.py           # also separately exclude a file named foo.py in
-                     # the root of the project
-)
-'''
+[tool.poetry]
+name = "fastapi-querysets"
+version = "0.1.2"
+description = ""
+authors = ["Nikakto <black-z@bk.ru>"]
+license = "MIT"
+readme = "README.md"
+repository = "https://github.com/Nikakto/fastapi-querysets"
+documentation = "https://fastapi-querysets.readthedocs.io"
+keywords = ["fastapi", "filters", "filtering", "pagination", "order", "ordering", "queryset", "Tortoise", "orm", "database", "db"]
+
+[tool.poetry.dependencies]
+python = ">=3.8,<4.0"
+fastapi = ">=0.78"
+tortoise-orm = ">=0.18.1"
+fastapi-depends-ext = ">=0.2.2"
+
+[tool.poetry.dev-dependencies]
+httpx = "^0.23.1"
+black = "^22.12.0"
+pytest = "^7.2.0"
+pytest-asyncio = "^0.20.3"
+pytest-mock = "^3.10.0"
+nest-asyncio = "^1.5.6"
+ipython = "^8.7.0"
+pytest-cov = "^4.0.0"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Jinja2 = "3.0.*"
+mkdocs-material = "^9.0.5"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
+[tool.black]
+line-length = 120
+target-version = ['py39']
+include = '\.pyi?$'
+exclude = '''
+
+(
+  /(
+      \.eggs         # exclude a few common directories in the
+    | \.git          # root of the project
+    | \.hg
+    | \.mypy_cache
+    | \.tox
+    | \.venv
+    | _build
+    | buck-out
+    | build
+    | dist
+  )/
+  | foo.py           # also separately exclude a file named foo.py in
+                     # the root of the project
+)
+'''
```

### Comparing `fastapi_querysets-0.1.1/README.md` & `fastapi_querysets-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,430 +1,414 @@
 00000000: 2320 4661 7374 4150 4920 5175 6572 7973  # FastAPI Querys
-00000010: 6574 730d 0a21 5b43 444e 4a53 5d28 6874  ets..![CDNJS](ht
-00000020: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000030: 732e 696f 2f62 6164 6765 2f50 7974 686f  s.io/badge/Pytho
-00000040: 6e2d 332e 3825 3230 2537 4325 3230 332e  n-3.8%20%7C%203.
-00000050: 3925 3230 2537 4325 3230 332e 3130 2532  9%20%7C%203.10%2
-00000060: 3025 3743 2532 3033 2e31 312d 3233 3334  0%7C%203.11-2334
-00000070: 4430 3538 290d 0a21 5b43 444e 4a53 5d28  D058)..![CDNJS](
-00000080: 6874 7470 733a 2f2f 7368 6965 6c64 732e  https://shields.
-00000090: 696f 2f62 6164 6765 2f46 6173 7441 5049  io/badge/FastAPI
-000000a0: 2d25 3345 3d30 2e37 2e30 2d30 3039 3438  -%3E=0.7.0-00948
-000000b0: 3529 0d0a 0d0a 2d2d 2d0d 0a2a 2a44 6f63  5)....---..**Doc
-000000c0: 756d 656e 7461 7469 6f6e 2a2a 3a20 3c61  umentation**: <a
-000000d0: 2068 7265 663d 2268 7474 7073 3a2f 2f66   href="https://f
-000000e0: 6173 7461 7069 2d71 7565 7279 7365 7473  astapi-querysets
-000000f0: 2e72 6561 6474 6865 646f 6373 2e69 6f22  .readthedocs.io"
-00000100: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00000110: 3e68 7474 7073 3a2f 2f66 6173 7461 7069  >https://fastapi
-00000120: 2d71 7565 7279 7365 7473 2e72 6561 6474  -querysets.readt
-00000130: 6865 646f 6373 2e69 6f3c 2f61 3e0d 0a0d  hedocs.io</a>...
-00000140: 0a2a 2a53 6f75 7263 6520 436f 6465 2a2a  .**Source Code**
-00000150: 3a20 3c61 2068 7265 663d 2268 7474 7073  : <a href="https
-00000160: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e69  ://github.com/Ni
-00000170: 6b61 6b74 6f2f 6661 7374 6170 692d 7175  kakto/fastapi-qu
-00000180: 6572 7973 6574 7322 2074 6172 6765 743d  erysets" target=
-00000190: 225f 626c 616e 6b22 3e68 7474 7073 3a2f  "_blank">https:/
-000001a0: 2f67 6974 6875 622e 636f 6d2f 4e69 6b61  /github.com/Nika
-000001b0: 6b74 6f2f 6661 7374 6170 692d 7175 6572  kto/fastapi-quer
-000001c0: 7973 6574 733c 2f61 3e0d 0a0d 0a2d 2d2d  ysets</a>....---
-000001d0: 0d0a 0d0a 2323 2057 6879 2074 6f20 7573  ....## Why to us
-000001e0: 653f 0d0a 0d0a 5768 696c 6520 796f 7520  e?....While you 
-000001f0: 6172 6520 6465 7665 6c6f 7069 6e67 2046  are developing F
-00000200: 6173 7441 5049 2061 7070 6c69 6361 7469  astAPI applicati
-00000210: 6f6e 7320 796f 7520 6172 6520 7573 696e  ons you are usin
-00000220: 6720 6461 7461 6261 7365 7320 7769 7468  g databases with
-00000230: 204f 524d 2e20 4d6f 7374 206f 6620 7468   ORM. Most of th
-00000240: 6520 656e 6470 6f69 6e74 7320 6172 6520  e endpoints are 
-00000250: 7669 6577 206f 6620 6461 7461 6261 7365  view of database
-00000260: 2074 6162 6c65 7320 616e 6420 7265 7175   tables and requ
-00000270: 6972 6520 7265 7374 7269 6374 2071 7565  ire restrict que
-00000280: 7279 7365 7420 6279 2066 696c 7465 7269  ryset by filteri
-00000290: 6e67 2c20 7061 6769 6e61 7469 6f6e 2c20  ng, pagination, 
-000002a0: 6f72 6465 7269 6e67 2e20 5468 6973 2070  ordering. This p
-000002b0: 726f 6a65 6374 2069 7320 6765 6e65 7269  roject is generi
-000002c0: 6320 616e 6420 7265 7573 6162 6c65 2077  c and reusable w
-000002d0: 6179 2074 6f20 6372 6561 7465 2072 6573  ay to create res
-000002e0: 7472 6963 7465 6420 7175 6572 7973 6574  tricted queryset
-000002f0: 7320 666f 7220 796f 7572 2065 6e64 706f  s for your endpo
-00000300: 696e 7473 2e0d 0a0d 0a23 2320 5375 7070  ints.....## Supp
-00000310: 6f72 7465 6420 4f52 4d0d 0a2d 203c 6120  orted ORM..- <a 
-00000320: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000330: 7468 7562 2e63 6f6d 2f74 6f72 746f 6973  thub.com/tortois
-00000340: 652f 746f 7274 6f69 7365 2d6f 726d 2220  e/tortoise-orm" 
-00000350: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000360: 546f 7274 6f69 7365 204f 524d 3c2f 613e  Tortoise ORM</a>
-00000370: 0d0a 0d0a 2323 2052 6571 7569 7265 6d65  ....## Requireme
-00000380: 6e74 730d 0a2d 2070 7974 686f 6e20 3e3d  nts..- python >=
-00000390: 332e 382c 3c34 2e30 0d0a 2d20 6661 7374  3.8,<4.0..- fast
-000003a0: 4150 4920 3e3d 2030 2e37 2e30 0d0a 2d20  API >= 0.7.0..- 
-000003b0: 746f 7274 6f69 7365 2d6f 726d 203e 3d20  tortoise-orm >= 
-000003c0: 302e 3138 2e31 0d0a 0d0a 2323 2049 6e73  0.18.1....## Ins
-000003d0: 7461 6c6c 6174 696f 6e0d 0a0d 0a60 6060  tallation....```
-000003e0: 0d0a 7069 7020 696e 7374 616c 6c20 6661  ..pip install fa
-000003f0: 7374 6170 692d 7175 6572 7973 6574 730d  stapi-querysets.
-00000400: 0a60 6060 0d0a 0d0a 2320 5175 6963 6b20  .```....# Quick 
-00000410: 7475 746f 7269 616c 0d0a 0d0a 2d2d 2d0d  tutorial....---.
-00000420: 0a0d 0a2d 2d2d 0d0a 0d0a 2323 2054 6f72  ...---....## Tor
-00000430: 746f 6973 6520 6d6f 6465 6c0d 0a0d 0a4c  toise model....L
-00000440: 6574 e280 9973 2073 7461 7274 2077 6974  et...s start wit
-00000450: 6820 6f75 7220 6d6f 6465 6c0d 0a0d 0a60  h our model....`
-00000460: 6060 7079 7468 6f6e 0d0a 2320 6d6f 6465  ``python..# mode
-00000470: 6c73 2f74 6f72 746f 6973 652e 7079 0d0a  ls/tortoise.py..
-00000480: 0d0a 696d 706f 7274 2064 6174 6574 696d  ..import datetim
-00000490: 650d 0a66 726f 6d20 7479 7069 6e67 2069  e..from typing i
-000004a0: 6d70 6f72 7420 4f70 7469 6f6e 616c 0d0a  mport Optional..
-000004b0: 0d0a 6672 6f6d 2074 6f72 746f 6973 6520  ..from tortoise 
-000004c0: 696d 706f 7274 204d 6f64 656c 0d0a 6672  import Model..fr
-000004d0: 6f6d 2074 6f72 746f 6973 6520 696d 706f  om tortoise impo
-000004e0: 7274 2066 6965 6c64 730d 0a0d 0a0d 0a63  rt fields......c
-000004f0: 6c61 7373 2054 6173 6b28 4d6f 6465 6c29  lass Task(Model)
-00000500: 3a0d 0a20 2020 2069 643a 2069 6e74 203d  :..    id: int =
-00000510: 2066 6965 6c64 732e 496e 7446 6965 6c64   fields.IntField
-00000520: 2870 6b3d 5472 7565 290d 0a20 2020 2061  (pk=True)..    a
-00000530: 7070 726f 7665 643a 204f 7074 696f 6e61  pproved: Optiona
-00000540: 6c5b 626f 6f6c 5d20 3d20 6669 656c 6473  l[bool] = fields
-00000550: 2e42 6f6f 6c65 616e 4669 656c 6428 6465  .BooleanField(de
-00000560: 6661 756c 743d 4661 6c73 652c 206e 756c  fault=False, nul
-00000570: 6c3d 5472 7565 290d 0a20 2020 2063 6f64  l=True)..    cod
-00000580: 653a 2073 7472 203d 2066 6965 6c64 732e  e: str = fields.
-00000590: 4368 6172 4669 656c 6428 6d61 785f 6c65  CharField(max_le
-000005a0: 6e67 7468 3d36 290d 0a20 2020 2063 7265  ngth=6)..    cre
-000005b0: 6174 6564 5f61 743a 2064 6174 6574 696d  ated_at: datetim
-000005c0: 652e 6461 7465 7469 6d65 203d 2066 6965  e.datetime = fie
-000005d0: 6c64 732e 4461 7465 7469 6d65 4669 656c  lds.DatetimeFiel
-000005e0: 6428 6465 6661 756c 743d 6461 7465 7469  d(default=dateti
-000005f0: 6d65 2e64 6174 6574 696d 652e 6e6f 7729  me.datetime.now)
-00000600: 0d0a 6060 600d 0a2d 2d2d 0d0a 0d0a 2323  ..```..---....##
-00000610: 2050 7964 616e 7469 6320 6d6f 6465 6c0d   Pydantic model.
-00000620: 0a0d 0a43 7265 6174 6520 6461 7461 6261  ...Create databa
-00000630: 7365 2072 6570 7265 7365 6e74 6174 696f  se representatio
-00000640: 6e20 6d6f 6465 6c0d 0a0d 0a60 6060 7079  n model....```py
-00000650: 7468 6f6e 0d0a 2320 6d6f 6465 6c73 2f70  thon..# models/p
-00000660: 7964 616e 7469 632e 7079 0d0a 0d0a 6672  ydantic.py....fr
-00000670: 6f6d 2074 6f72 746f 6973 652e 636f 6e74  om tortoise.cont
-00000680: 7269 622e 7079 6461 6e74 6963 2069 6d70  rib.pydantic imp
-00000690: 6f72 7420 7079 6461 6e74 6963 5f6d 6f64  ort pydantic_mod
-000006a0: 656c 5f63 7265 6174 6f72 0d0a 0d0a 6672  el_creator....fr
-000006b0: 6f6d 206d 7970 726f 6a65 6374 2e6d 6f64  om myproject.mod
-000006c0: 656c 732e 746f 7274 6f69 7365 2069 6d70  els.tortoise imp
-000006d0: 6f72 7420 5461 736b 0d0a 0d0a 0d0a 5461  ort Task......Ta
-000006e0: 736b 4d6f 6465 6c4f 7574 203d 2070 7964  skModelOut = pyd
-000006f0: 616e 7469 635f 6d6f 6465 6c5f 6372 6561  antic_model_crea
-00000700: 746f 7228 0d0a 2020 2020 5461 736b 2c0d  tor(..    Task,.
-00000710: 0a20 2020 206e 616d 653d 2254 6173 6b4d  .    name="TaskM
-00000720: 6f64 656c 4f75 7422 2c0d 0a20 2020 2069  odelOut",..    i
-00000730: 6e63 6c75 6465 3d28 0d0a 2020 2020 2020  nclude=(..      
-00000740: 2020 2269 6422 2c0d 0a20 2020 2020 2020    "id",..       
-00000750: 2022 6170 7072 6f76 6564 222c 0d0a 2020   "approved",..  
-00000760: 2020 2020 2020 2263 6f64 6522 2c0d 0a20        "code",.. 
-00000770: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
-00000780: 6174 220d 0a20 2020 2029 2c0d 0a29 0d0a  at"..    ),..)..
-00000790: 6060 600d 0a0d 0a2d 2d2d 0d0a 0d0a 2323  ```....---....##
-000007a0: 2052 6f75 7465 7251 7565 7279 5365 740d   RouterQuerySet.
-000007b0: 0a0d 0a23 2323 2046 696c 7465 7273 0d0a  ...### Filters..
-000007c0: 0d0a 5765 2068 6176 6520 6120 6e75 6d62  ..We have a numb
-000007d0: 6572 206f 6620 6669 656c 6473 2077 6520  er of fields we 
-000007e0: 7761 6e74 2074 6f20 6c65 7420 6f75 7220  want to let our 
-000007f0: 7573 6572 7320 6669 6c74 6572 2062 6173  users filter bas
-00000800: 6564 206f 6e20 7468 656d 2e20 5765 2063  ed on them. We c
-00000810: 7265 6174 6520 6120 526f 7574 6572 5175  reate a RouterQu
-00000820: 6572 7953 6574 4669 6c74 6572 2066 6f72  erySetFilter for
-00000830: 2074 6869 732e 2046 696c 7465 7220 636c   this. Filter cl
-00000840: 6173 7320 6973 2061 7267 756d 656e 7420  ass is argument 
-00000850: 666f 7220 6046 6173 7441 5049 2e44 6570  for `FastAPI.Dep
-00000860: 656e 6473 6020 6174 2065 6e64 706f 696e  ends` at endpoin
-00000870: 742e 2020 0d0a 0d0a 596f 7520 7265 7175  t.  ....You requ
-00000880: 6972 6520 746f 2064 6566 696e 6520 4f52  ire to define OR
-00000890: 4d20 6669 6c74 6572 206b 6579 776f 7264  M filter keyword
-000008a0: 2c20 7479 7065 206f 6620 6461 7461 2061  , type of data a
-000008b0: 6e64 2073 6574 7570 2073 6f75 7263 6520  nd setup source 
-000008c0: 6f66 2064 6174 6120 2860 5175 6572 7960  of data (`Query`
-000008d0: 2c20 6050 6174 6860 2c20 6042 6f64 7960  , `Path`, `Body`
-000008e0: 2c20 6574 6329 2e0d 0a0d 0a60 6060 7079  , etc).....```py
-000008f0: 7468 6f6e 0d0a 2320 7175 6572 7973 6574  thon..# queryset
-00000900: 735f 6669 6c74 6572 732e 7079 0d0a 0d0a  s_filters.py....
-00000910: 696d 706f 7274 2064 6174 6163 6c61 7373  import dataclass
-00000920: 6573 0d0a 696d 706f 7274 2064 6174 6574  es..import datet
-00000930: 696d 650d 0a66 726f 6d20 7479 7069 6e67  ime..from typing
-00000940: 2069 6d70 6f72 7420 4f70 7469 6f6e 616c   import Optional
-00000950: 0d0a 0d0a 6672 6f6d 2066 6173 7461 7069  ....from fastapi
-00000960: 2069 6d70 6f72 7420 5175 6572 790d 0a0d   import Query...
-00000970: 0a0d 0a40 6461 7461 636c 6173 7365 732e  ...@dataclasses.
-00000980: 6461 7461 636c 6173 730d 0a63 6c61 7373  dataclass..class
-00000990: 2052 6f75 7465 7251 7565 7279 5365 7446   RouterQuerySetF
-000009a0: 696c 7465 723a 0d0a 2020 2020 6964 5f5f  ilter:..    id__
-000009b0: 696e 3a20 4f70 7469 6f6e 616c 5b6c 6973  in: Optional[lis
-000009c0: 745b 696e 745d 5d20 3d20 5175 6572 7928  t[int]] = Query(
-000009d0: 4e6f 6e65 2c20 616c 6961 733d 2769 645b  None, alias='id[
-000009e0: 5d27 290d 0a20 2020 2061 7070 726f 7665  ]')..    approve
-000009f0: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
-00000a00: 5d20 3d20 5175 6572 7928 4e6f 6e65 290d  ] = Query(None).
-00000a10: 0a20 2020 2061 7070 726f 7665 645f 5f69  .    approved__i
-00000a20: 736e 756c 6c3a 204f 7074 696f 6e61 6c5b  snull: Optional[
-00000a30: 626f 6f6c 5d20 3d20 5175 6572 7928 4e6f  bool] = Query(No
-00000a40: 6e65 290d 0a20 2020 2063 6f64 653a 204f  ne)..    code: O
-00000a50: 7074 696f 6e61 6c5b 7374 725d 203d 2051  ptional[str] = Q
-00000a60: 7565 7279 284e 6f6e 6529 0d0a 2020 2020  uery(None)..    
-00000a70: 6372 6561 7465 645f 6174 5f5f 6c74 653a  created_at__lte:
-00000a80: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
-00000a90: 6d65 2e64 6174 6574 696d 655d 203d 2051  me.datetime] = Q
-00000aa0: 7565 7279 284e 6f6e 6529 0d0a 2020 2020  uery(None)..    
-00000ab0: 6372 6561 7465 645f 6174 5f5f 6774 653a  created_at__gte:
-00000ac0: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
-00000ad0: 6d65 2e64 6174 6574 696d 655d 203d 2051  me.datetime] = Q
-00000ae0: 7565 7279 284e 6f6e 6529 0d0a 6060 600d  uery(None)..```.
-00000af0: 0a0d 0a23 2323 204d 6f64 656c 2051 7565  ...### Model Que
-00000b00: 7279 7365 740d 0a0d 0a43 6f6e 6669 6775  ryset....Configu
-00000b10: 7265 2060 526f 7574 6572 5175 6572 7973  re `RouterQuerys
-00000b20: 6574 6020 7072 6f70 6572 7469 6573 0d0a  et` properties..
-00000b30: 0d0a 6060 6070 7974 686f 6e0d 0a23 2071  ..```python..# q
-00000b40: 7565 7279 7365 7473 2e70 790d 0a0d 0a66  uerysets.py....f
-00000b50: 726f 6d20 6661 7374 6170 695f 7175 6572  rom fastapi_quer
-00000b60: 7973 6574 732e 6d69 7869 6e73 2e66 696c  ysets.mixins.fil
-00000b70: 7465 7273 2069 6d70 6f72 7420 4669 6c74  ters import Filt
-00000b80: 6572 4d69 7869 6e0d 0a66 726f 6d20 6661  erMixin..from fa
-00000b90: 7374 6170 695f 7175 6572 7973 6574 732e  stapi_querysets.
-00000ba0: 6d69 7869 6e73 2e66 696c 7465 7273 2069  mixins.filters i
-00000bb0: 6d70 6f72 7420 4669 6c74 6572 4e65 6761  mport FilterNega
-00000bc0: 7469 6f6e 4d69 7869 6e0d 0a66 726f 6d20  tionMixin..from 
-00000bd0: 6661 7374 6170 695f 7175 6572 7973 6574  fastapi_queryset
-00000be0: 732e 6d69 7869 6e73 2e6f 7264 6572 696e  s.mixins.orderin
-00000bf0: 6720 696d 706f 7274 204f 7264 6572 696e  g import Orderin
-00000c00: 674d 6978 696e 0d0a 6672 6f6d 2066 6173  gMixin..from fas
-00000c10: 7461 7069 5f71 7565 7279 7365 7473 2e6d  tapi_querysets.m
-00000c20: 6978 696e 732e 7061 6769 6e61 7469 6f6e  ixins.pagination
-00000c30: 2069 6d70 6f72 7420 5061 6769 6e61 7469   import Paginati
-00000c40: 6f6e 4d69 7869 6e0d 0a66 726f 6d20 6661  onMixin..from fa
-00000c50: 7374 6170 695f 7175 6572 7973 6574 732e  stapi_querysets.
-00000c60: 6d69 7869 6e73 2e70 6167 696e 6174 696f  mixins.paginatio
-00000c70: 6e20 696d 706f 7274 2052 6f75 7465 7250  n import RouterP
-00000c80: 6167 696e 6174 696f 6e0d 0a66 726f 6d20  agination..from 
-00000c90: 6661 7374 6170 695f 7175 6572 7973 6574  fastapi_queryset
-00000ca0: 732e 7175 6572 7973 6574 2069 6d70 6f72  s.queryset impor
-00000cb0: 7420 526f 7574 6572 5175 6572 7953 6574  t RouterQuerySet
-00000cc0: 0d0a 0d0a 6672 6f6d 206d 7970 726f 6a65  ....from myproje
-00000cd0: 6374 2e6d 6f64 656c 732e 746f 7274 6f69  ct.models.tortoi
-00000ce0: 7365 2069 6d70 6f72 7420 5461 736b 0d0a  se import Task..
-00000cf0: 6672 6f6d 206d 7970 726f 6a65 6374 2e71  from myproject.q
-00000d00: 7565 7279 7365 7473 5f66 696c 7465 7273  uerysets_filters
-00000d10: 2069 6d70 6f72 7420 526f 7574 6572 5175   import RouterQu
-00000d20: 6572 7953 6574 4669 6c74 6572 0d0a 0d0a  erySetFilter....
-00000d30: 0d0a 636c 6173 7320 5461 736b 7352 6f75  ..class TasksRou
-00000d40: 7465 7251 7565 7279 5365 7428 4669 6c74  terQuerySet(Filt
-00000d50: 6572 4d69 7869 6e2c 2046 696c 7465 724e  erMixin, FilterN
-00000d60: 6567 6174 696f 6e4d 6978 696e 2c20 4f72  egationMixin, Or
-00000d70: 6465 7269 6e67 4d69 7869 6e2c 2050 6167  deringMixin, Pag
-00000d80: 696e 6174 696f 6e4d 6978 696e 2c20 526f  inationMixin, Ro
-00000d90: 7574 6572 5175 6572 7953 6574 293a 0d0a  uterQuerySet):..
-00000da0: 2020 2020 6669 6c74 6572 5f63 6c61 7373      filter_class
-00000db0: 203d 2052 6f75 7465 7251 7565 7279 5365   = RouterQuerySe
-00000dc0: 7446 696c 7465 720d 0a20 2020 206f 7264  tFilter..    ord
-00000dd0: 6572 696e 675f 6465 6661 756c 7420 3d20  ering_default = 
-00000de0: 2269 6422 0d0a 2020 2020 6f72 6465 7269  "id"..    orderi
-00000df0: 6e67 5f66 6965 6c64 7320 3d20 280d 0a20  ng_fields = (.. 
-00000e00: 2020 2020 2020 2022 6964 222c 0d0a 2020         "id",..  
-00000e10: 2020 2020 2020 2261 7070 726f 7665 6422        "approved"
-00000e20: 2c0d 0a20 2020 2020 2020 2022 636f 6465  ,..        "code
-00000e30: 222c 0d0a 2020 2020 2020 2020 2263 7265  ",..        "cre
-00000e40: 6174 6564 5f61 7422 2c0d 0a20 2020 2029  ated_at",..    )
-00000e50: 0d0a 2020 2020 7061 6769 6e61 7469 6f6e  ..    pagination
-00000e60: 5f63 6c61 7373 203d 2052 6f75 7465 7250  _class = RouterP
-00000e70: 6167 696e 6174 696f 6e0d 0a20 2020 206d  agination..    m
-00000e80: 6f64 656c 203d 2054 6173 6b0d 0a60 6060  odel = Task..```
-00000e90: 0d0a 0d0a 2d2d 2d0d 0a0d 0a23 2320 4170  ....---....## Ap
-00000ea0: 706c 6963 6174 696f 6e0d 0a0d 0a43 7265  plication....Cre
-00000eb0: 6174 6520 6170 706c 6963 6174 696f 6e2c  ate application,
-00000ec0: 2072 6567 6973 7465 7220 6c69 7374 2c20   register list, 
-00000ed0: 6c69 7374 2077 6974 6820 7061 6769 6e61  list with pagina
-00000ee0: 7469 6f6e 2061 6e64 2072 6574 7269 6576  tion and retriev
-00000ef0: 6520 656e 6470 6f69 6e74 732e 0d0a 6060  e endpoints...``
-00000f00: 6070 7974 686f 6e0d 0a23 2061 7070 2e70  `python..# app.p
-00000f10: 790d 0a0d 0a66 726f 6d20 6661 7374 6170  y....from fastap
-00000f20: 6920 696d 706f 7274 2046 6173 7441 5049  i import FastAPI
-00000f30: 0d0a 6672 6f6d 2074 6f72 746f 6973 652e  ..from tortoise.
-00000f40: 636f 6e74 7269 622e 6661 7374 6170 6920  contrib.fastapi 
-00000f50: 696d 706f 7274 2072 6567 6973 7465 725f  import register_
-00000f60: 746f 7274 6f69 7365 0d0a 6672 6f6d 2074  tortoise..from t
-00000f70: 6f72 746f 6973 652e 7175 6572 7973 6574  ortoise.queryset
-00000f80: 2069 6d70 6f72 7420 5175 6572 7953 6574   import QuerySet
-00000f90: 0d0a 0d0a 6672 6f6d 206d 7970 726f 6a65  ....from myproje
-00000fa0: 6374 2e6d 6f64 656c 732e 7079 6461 6e74  ct.models.pydant
-00000fb0: 6963 2069 6d70 6f72 7420 5461 736b 4d6f  ic import TaskMo
-00000fc0: 6465 6c4f 7574 0d0a 6672 6f6d 206d 7970  delOut..from myp
-00000fd0: 726f 6a65 6374 2e6d 6f64 656c 732e 746f  roject.models.to
-00000fe0: 7274 6f69 7365 2069 6d70 6f72 7420 5461  rtoise import Ta
-00000ff0: 736b 0d0a 6672 6f6d 206d 7970 726f 6a65  sk..from myproje
-00001000: 6374 2e71 7565 7279 7365 7473 2069 6d70  ct.querysets imp
-00001010: 6f72 7420 5461 736b 7352 6f75 7465 7251  ort TasksRouterQ
-00001020: 7565 7279 5365 740d 0a0d 0a0d 0a61 7070  uerySet......app
-00001030: 203d 2046 6173 7441 5049 2829 0d0a 0d0a   = FastAPI()....
-00001040: 0d0a 7265 6769 7374 6572 5f74 6f72 746f  ..register_torto
-00001050: 6973 6528 0d0a 2020 2020 6170 702c 0d0a  ise(..    app,..
-00001060: 2020 2020 6462 5f75 726c 3d22 7371 6c69      db_url="sqli
-00001070: 7465 3a2f 2f3a 6d65 6d6f 7279 3a22 2c0d  te://:memory:",.
-00001080: 0a20 2020 206d 6f64 756c 6573 3d7b 226d  .    modules={"m
-00001090: 6f64 656c 7322 3a20 5b22 6d79 7072 6f6a  odels": ["myproj
-000010a0: 6563 742e 6d6f 6465 6c73 2e74 6f72 746f  ect.models.torto
-000010b0: 6973 6522 5d7d 2c0d 0a20 2020 2067 656e  ise"]},..    gen
-000010c0: 6572 6174 655f 7363 6865 6d61 733d 5472  erate_schemas=Tr
-000010d0: 7565 2c0d 0a20 2020 2061 6464 5f65 7863  ue,..    add_exc
-000010e0: 6570 7469 6f6e 5f68 616e 646c 6572 733d  eption_handlers=
-000010f0: 5472 7565 2c0d 0a29 0d0a 0d0a 0d0a 4061  True,..)......@a
-00001100: 7070 2e67 6574 2822 7461 736b 732f 222c  pp.get("tasks/",
-00001110: 2072 6573 706f 6e73 655f 6d6f 6465 6c3d   response_model=
-00001120: 6c69 7374 5b54 6173 6b4d 6f64 656c 4f75  list[TaskModelOu
-00001130: 745d 290d 0a61 7379 6e63 2064 6566 2074  t])..async def t
-00001140: 6173 6b73 5f6c 6973 745f 7061 6769 6e61  asks_list_pagina
-00001150: 7465 6428 7175 6572 7973 6574 3a20 5175  ted(queryset: Qu
-00001160: 6572 7953 6574 5b54 6173 6b5d 203d 2054  erySet[Task] = T
-00001170: 6173 6b73 526f 7574 6572 5175 6572 7953  asksRouterQueryS
-00001180: 6574 2829 2920 2d3e 206c 6973 745b 5461  et()) -> list[Ta
-00001190: 736b 4d6f 6465 6c4f 7574 5d3a 0d0a 2020  skModelOut]:..  
-000011a0: 2020 7265 7475 726e 2061 7761 6974 2054    return await T
-000011b0: 6173 6b4d 6f64 656c 4f75 742e 6672 6f6d  askModelOut.from
-000011c0: 5f71 7565 7279 7365 7428 7175 6572 7973  _queryset(querys
-000011d0: 6574 290d 0a0d 0a0d 0a40 6170 702e 6765  et)......@app.ge
-000011e0: 7428 2274 6173 6b73 2f70 6167 696e 6174  t("tasks/paginat
-000011f0: 6564 222c 2072 6573 706f 6e73 655f 6d6f  ed", response_mo
-00001200: 6465 6c3d 6c69 7374 5b54 6173 6b4d 6f64  del=list[TaskMod
-00001210: 656c 4f75 745d 290d 0a61 7379 6e63 2064  elOut])..async d
-00001220: 6566 2074 6173 6b73 5f6c 6973 745f 7061  ef tasks_list_pa
-00001230: 6769 6e61 7465 6428 7175 6572 7973 6574  ginated(queryset
-00001240: 3a20 5175 6572 7953 6574 5b54 6173 6b5d  : QuerySet[Task]
-00001250: 203d 2054 6173 6b73 526f 7574 6572 5175   = TasksRouterQu
-00001260: 6572 7953 6574 2829 2e70 6167 696e 6174  erySet().paginat
-00001270: 6564 2920 2d3e 206c 6973 745b 5461 736b  ed) -> list[Task
-00001280: 4d6f 6465 6c4f 7574 5d3a 0d0a 2020 2020  ModelOut]:..    
-00001290: 7265 7475 726e 2061 7761 6974 2054 6173  return await Tas
-000012a0: 6b4d 6f64 656c 4f75 742e 6672 6f6d 5f71  kModelOut.from_q
-000012b0: 7565 7279 7365 7428 7175 6572 7973 6574  ueryset(queryset
-000012c0: 290d 0a0d 0a0d 0a40 6170 702e 6765 7428  )......@app.get(
-000012d0: 2274 6173 6b73 2f7b 696e 7374 616e 6365  "tasks/{instance
-000012e0: 5f69 647d 222c 2072 6573 706f 6e73 655f  _id}", response_
-000012f0: 6d6f 6465 6c3d 6c69 7374 5b54 6173 6b4d  model=list[TaskM
-00001300: 6f64 656c 4f75 745d 290d 0a61 7379 6e63  odelOut])..async
-00001310: 2064 6566 2074 6173 6b73 5f72 6574 7269   def tasks_retri
-00001320: 6576 6528 7461 736b 3a20 5175 6572 7953  eve(task: QueryS
-00001330: 6574 5b54 6173 6b5d 203d 2054 6173 6b73  et[Task] = Tasks
-00001340: 526f 7574 6572 5175 6572 7953 6574 2829  RouterQuerySet()
-00001350: 2e69 6e73 7461 6e63 6529 202d 3e20 6c69  .instance) -> li
-00001360: 7374 5b54 6173 6b4d 6f64 656c 4f75 745d  st[TaskModelOut]
-00001370: 3a0d 0a20 2020 2072 6574 7572 6e20 5461  :..    return Ta
-00001380: 736b 4d6f 6465 6c4f 7574 2e66 726f 6d5f  skModelOut.from_
-00001390: 6f72 6d28 7461 736b 290d 0a60 6060 0d0a  orm(task)..```..
-000013a0: 0d0a 2d2d 2d0d 0a0d 0a23 2320 5265 7175  ..---....## Requ
-000013b0: 6573 7473 0d0a 0d0a 2323 2320 4c69 7374  ests....### List
-000013c0: 0d0a 0d0a 4f6e 2072 6571 7565 7374 2065  ....On request e
-000013d0: 6666 6563 7469 7665 2071 7565 7279 7365  ffective queryse
-000013e0: 7420 7769 6c6c 2062 6520 6669 6c74 6572  t will be filter
-000013f0: 6564 2061 6e64 206f 7264 6572 6564 2062  ed and ordered b
-00001400: 7920 7175 6572 7920 7061 7261 6d73 2e0d  y query params..
-00001410: 0a0d 0a46 6f72 2065 7861 6d70 6c65 2c20  ...For example, 
-00001420: 7573 6572 2068 6173 2072 6571 7565 7374  user has request
-00001430: 6564 2065 6e64 706f 696e 7420 7769 7468  ed endpoint with
-00001440: 2073 6f6d 6520 7175 6572 7920 7061 7261   some query para
-00001450: 6d73 0d0a 6060 606a 736f 6e0d 0a7b 0d0a  ms..```json..{..
-00001460: 2020 2020 2263 7265 6174 6564 5f61 745f      "created_at_
-00001470: 5f6c 7465 223a 2022 3230 3233 2d30 312d  _lte": "2023-01-
-00001480: 3031 5430 303a 3030 3a30 3022 2c0d 0a20  01T00:00:00",.. 
-00001490: 2020 2022 6170 7072 6f76 6564 223a 2066     "approved": f
-000014a0: 616c 7365 2c0d 0a20 2020 2022 6f72 6465  alse,..    "orde
-000014b0: 7269 6e67 5b5d 223a 2022 6372 6561 7465  ring[]": "create
-000014c0: 645f 6174 222c 0d0a 7d0d 0a60 6060 0d0a  d_at",..}..```..
-000014d0: 0d0a 5265 7175 6573 7420 5552 4c20 6c6f  ..Request URL lo
-000014e0: 6f6b 7320 6c69 6b65 2020 0d0a 6060 6068  oks like  ..```h
-000014f0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00001500: 3830 3030 2f74 6173 6b73 2f3f 6372 6561  8000/tasks/?crea
-00001510: 7465 645f 6174 5f5f 6c74 653d 3230 3233  ted_at__lte=2023
-00001520: 2d30 312d 3031 5430 303a 3030 3a30 3026  -01-01T00:00:00&
-00001530: 6170 7072 6f76 6564 3d66 616c 7365 266f  approved=false&o
-00001540: 7264 6572 696e 675b 5d3d 6372 6561 7465  rdering[]=create
-00001550: 645f 6174 6060 600d 0a0d 0a45 6666 6563  d_at```....Effec
-00001560: 7469 7665 2071 7565 7279 7365 7420 6174  tive queryset at
-00001570: 2074 6865 2065 6e64 706f 696e 7420 6d65   the endpoint me
-00001580: 7468 6f64 2077 696c 6c20 6265 0d0a 6060  thod will be..``
-00001590: 6070 7974 686f 6e0d 0a28 0d0a 2020 2020  `python..(..    
-000015a0: 5461 736b 0d0a 2020 2020 2e66 696c 7465  Task..    .filte
-000015b0: 7228 6372 6561 7465 645f 6174 5f5f 6c74  r(created_at__lt
-000015c0: 653d 6461 7465 7469 6d65 2e64 6174 6574  e=datetime.datet
-000015d0: 696d 6528 3230 3233 2c20 312c 2031 2c20  ime(2023, 1, 1, 
-000015e0: 302c 2030 2c20 3029 2c20 6170 7072 6f76  0, 0, 0), approv
-000015f0: 6564 3d46 616c 7365 290d 0a20 2020 202e  ed=False)..    .
-00001600: 6f72 6465 725f 6279 2822 6372 6561 7465  order_by("create
-00001610: 645f 6174 2229 0d0a 290d 0a60 6060 0d0a  d_at")..)..```..
-00001620: 0d0a 2323 2320 4c69 7374 2070 6167 696e  ..### List pagin
-00001630: 6174 6564 0d0a 0d0a 4c69 6b65 206e 6f74  ated....Like not
-00001640: 2070 6167 696e 6174 6564 2065 6e64 706f   paginated endpo
-00001650: 696e 7420 6174 2074 6869 7320 7175 6572  int at this quer
-00001660: 7973 6574 2077 696c 6c20 6265 2066 696c  yset will be fil
-00001670: 7465 7265 642c 206f 7264 6572 696e 6720  tered, ordering 
-00001680: 616e 6420 6164 6469 7469 6f6e 616c 2070  and additional p
-00001690: 6167 696e 6174 6564 2e0d 0a0d 0a46 6f72  aginated.....For
-000016a0: 2065 7861 6d70 6c65 2c20 7573 6572 2068   example, user h
-000016b0: 6173 2072 6571 7565 7374 6564 2065 6e64  as requested end
-000016c0: 706f 696e 7420 7769 7468 2073 6f6d 6520  point with some 
-000016d0: 7175 6572 7920 7061 7261 6d73 0d0a 6060  query params..``
-000016e0: 606a 736f 6e0d 0a7b 0d0a 2020 2020 2270  `json..{..    "p
-000016f0: 6167 6522 3a20 322c 0d0a 2020 2020 2270  age": 2,..    "p
-00001700: 6572 5f70 6167 6522 3a20 3130 2c0d 0a20  er_page": 10,.. 
-00001710: 2020 2022 6372 6561 7465 645f 6174 5f5f     "created_at__
-00001720: 6c74 6522 3a20 2232 3032 332d 3031 2d30  lte": "2023-01-0
-00001730: 3154 3030 3a30 303a 3030 222c 0d0a 2020  1T00:00:00",..  
-00001740: 2020 2261 7070 726f 7665 6422 3a20 6661    "approved": fa
-00001750: 6c73 652c 0d0a 2020 2020 226f 7264 6572  lse,..    "order
-00001760: 696e 675b 5d22 3a20 2263 7265 6174 6564  ing[]": "created
-00001770: 5f61 7422 2c0d 0a7d 0d0a 6060 600d 0a0d  _at",..}..```...
-00001780: 0a52 6571 7565 7374 2055 524c 206c 6f6f  .Request URL loo
-00001790: 6b73 206c 696b 6520 2020 0d0a 6060 6068  ks like   ..```h
-000017a0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-000017b0: 3830 3030 2f74 6173 6b73 2f3f 7061 6765  8000/tasks/?page
-000017c0: 3d32 2670 6572 5f70 6167 653d 3130 2663  =2&per_page=10&c
-000017d0: 7265 6174 6564 5f61 745f 5f6c 7465 3d32  reated_at__lte=2
-000017e0: 3032 332d 3031 2d30 3154 3030 3a30 303a  023-01-01T00:00:
-000017f0: 3030 2661 7070 726f 7665 643d 6661 6c73  00&approved=fals
-00001800: 6526 6f72 6465 7269 6e67 5b5d 3d63 7265  e&ordering[]=cre
-00001810: 6174 6564 5f61 7460 6060 0d0a 0d0a 0d0a  ated_at```......
-00001820: 4566 6665 6374 6976 6520 7175 6572 7973  Effective querys
-00001830: 6574 2061 7420 656e 6470 6f69 6e74 206d  et at endpoint m
-00001840: 6574 686f 6420 7769 6c6c 2062 650d 0a60  ethod will be..`
-00001850: 6060 7079 7468 6f6e 0d0a 280d 0a20 2020  ``python..(..   
-00001860: 2054 6173 6b0d 0a20 2020 202e 6669 6c74   Task..    .filt
-00001870: 6572 2863 7265 6174 6564 5f61 745f 5f6c  er(created_at__l
-00001880: 7465 3d64 6174 6574 696d 652e 6461 7465  te=datetime.date
-00001890: 7469 6d65 2832 3032 332c 2031 2c20 312c  time(2023, 1, 1,
-000018a0: 2030 2c20 302c 2030 292c 2061 7070 726f   0, 0, 0), appro
-000018b0: 7665 643d 4661 6c73 6529 0d0a 2020 2020  ved=False)..    
-000018c0: 2e6f 7264 6572 5f62 7928 2263 7265 6174  .order_by("creat
-000018d0: 6564 5f61 7422 290d 0a20 2020 202e 6f66  ed_at")..    .of
-000018e0: 6673 6574 2831 3029 0d0a 2020 2020 2e6c  fset(10)..    .l
-000018f0: 696d 6974 2831 3029 0d0a 290d 0a60 6060  imit(10)..)..```
-00001900: 0d0a 0d0a 4173 2077 656c 6c20 6173 2074  ....As well as t
-00001910: 6f20 6052 6573 706f 6e73 6560 2077 696c  o `Response` wil
-00001920: 6c20 6265 2061 6464 6564 2070 6167 696e  l be added pagin
-00001930: 6174 696f 6e20 696e 666f 726d 6174 696f  ation informatio
-00001940: 6e2e 2050 6167 696e 6174 696f 6e20 696e  n. Pagination in
-00001950: 666f 726d 6174 696f 6e20 616c 7761 7973  formation always
-00001960: 206d 6174 6368 6573 2065 6666 6563 7469   matches effecti
-00001970: 7665 2071 7565 7279 7365 740d 0a60 6060  ve queryset..```
-00001980: 6a73 6f6e 0d0a 7b0d 0a20 2020 2022 782d  json..{..    "x-
-00001990: 7061 6765 223a 2022 3222 2c0d 0a20 2020  page": "2",..   
-000019a0: 2022 782d 7061 6765 7322 3a20 2234 222c   "x-pages": "4",
-000019b0: 0d0a 2020 2020 2278 2d70 6572 2d70 6167  ..    "x-per-pag
-000019c0: 6522 3a20 2231 3022 2c0d 0a20 2020 2022  e": "10",..    "
-000019d0: 782d 746f 7461 6c22 3a20 2233 3222 0d0a  x-total": "32"..
-000019e0: 7d0d 0a60 6060 0d0a 0d0a 2323 2320 5265  }..```....### Re
-000019f0: 7472 6965 7665 0d0a 0d0a 5265 7175 6573  trieve....Reques
-00001a00: 7420 5552 4c20 6c6f 6f6b 7320 6c69 6b65  t URL looks like
-00001a10: 2020 200d 0a60 6060 6874 7470 3a2f 2f6c     ..```http://l
-00001a20: 6f63 616c 686f 7374 3a38 3030 302f 7461  ocalhost:8000/ta
-00001a30: 736b 732f 3130 2f60 6060 0d0a 0d0a 456e  sks/10/```....En
-00001a40: 6470 6f69 6e74 206d 6574 686f 6420 7769  dpoint method wi
-00001a50: 6c6c 2067 6574 2060 5461 736b 6020 7769  ll get `Task` wi
-00001a60: 7468 2060 6964 203d 3d20 3130 6020 6173  th `id == 10` as
-00001a70: 2061 7267 756d 656e 7420 6074 6173 6b60   argument `task`
-00001a80: 2e20 2020 2020 0d0a 4966 2060 5461 736b  .     ..If `Task
-00001a90: 6020 7769 7468 2060 6964 203d 3d20 3130  ` with `id == 10
-00001aa0: 6020 646f 6573 206e 6f74 2065 7869 7374  ` does not exist
-00001ab0: 2074 6865 6e20 656e 6470 6f69 6e74 2072   then endpoint r
-00001ac0: 6574 7572 6e20 6052 6573 706f 6e73 6528  eturn `Response(
-00001ad0: 3430 3429 6020 20                        404)`  
+00000010: 6574 730a 215b 4344 4e4a 535d 2868 7474  ets.![CDNJS](htt
+00000020: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000030: 2e69 6f2f 6261 6467 652f 5079 7468 6f6e  .io/badge/Python
+00000040: 2d33 2e38 2532 3025 3743 2532 3033 2e39  -3.8%20%7C%203.9
+00000050: 2532 3025 3743 2532 3033 2e31 3025 3230  %20%7C%203.10%20
+00000060: 2537 4325 3230 332e 3131 2d32 3333 3444  %7C%203.11-2334D
+00000070: 3035 3829 0a21 5b43 444e 4a53 5d28 6874  058).![CDNJS](ht
+00000080: 7470 733a 2f2f 7368 6965 6c64 732e 696f  tps://shields.io
+00000090: 2f62 6164 6765 2f46 6173 7441 5049 2d25  /badge/FastAPI-%
+000000a0: 3345 3d30 2e37 2e30 2d30 3039 3438 3529  3E=0.7.0-009485)
+000000b0: 0a0a 2d2d 2d0a 2a2a 446f 6375 6d65 6e74  ..---.**Document
+000000c0: 6174 696f 6e2a 2a3a 203c 6120 6872 6566  ation**: <a href
+000000d0: 3d22 6874 7470 733a 2f2f 6661 7374 6170  ="https://fastap
+000000e0: 692d 7175 6572 7973 6574 732e 7265 6164  i-querysets.read
+000000f0: 7468 6564 6f63 732e 696f 2220 7461 7267  thedocs.io" targ
+00000100: 6574 3d22 5f62 6c61 6e6b 223e 6874 7470  et="_blank">http
+00000110: 733a 2f2f 6661 7374 6170 692d 7175 6572  s://fastapi-quer
+00000120: 7973 6574 732e 7265 6164 7468 6564 6f63  ysets.readthedoc
+00000130: 732e 696f 3c2f 613e 0a0a 2a2a 536f 7572  s.io</a>..**Sour
+00000140: 6365 2043 6f64 652a 2a3a 203c 6120 6872  ce Code**: <a hr
+00000150: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000160: 7562 2e63 6f6d 2f4e 696b 616b 746f 2f66  ub.com/Nikakto/f
+00000170: 6173 7461 7069 2d71 7565 7279 7365 7473  astapi-querysets
+00000180: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000190: 223e 6874 7470 733a 2f2f 6769 7468 7562  ">https://github
+000001a0: 2e63 6f6d 2f4e 696b 616b 746f 2f66 6173  .com/Nikakto/fas
+000001b0: 7461 7069 2d71 7565 7279 7365 7473 3c2f  tapi-querysets</
+000001c0: 613e 0a0a 2d2d 2d0a 0a23 2320 5768 7920  a>..---..## Why 
+000001d0: 746f 2075 7365 3f0a 0a57 6869 6c65 2079  to use?..While y
+000001e0: 6f75 2061 7265 2064 6576 656c 6f70 696e  ou are developin
+000001f0: 6720 4661 7374 4150 4920 6170 706c 6963  g FastAPI applic
+00000200: 6174 696f 6e73 2079 6f75 2061 7265 2075  ations you are u
+00000210: 7369 6e67 2064 6174 6162 6173 6573 2077  sing databases w
+00000220: 6974 6820 4f52 4d2e 204d 6f73 7420 6f66  ith ORM. Most of
+00000230: 2074 6865 2065 6e64 706f 696e 7473 2061   the endpoints a
+00000240: 7265 2076 6965 7720 6f66 2064 6174 6162  re view of datab
+00000250: 6173 6520 7461 626c 6573 2061 6e64 2072  ase tables and r
+00000260: 6571 7569 7265 2072 6573 7472 6963 7420  equire restrict 
+00000270: 7175 6572 7973 6574 2062 7920 6669 6c74  queryset by filt
+00000280: 6572 696e 672c 2070 6167 696e 6174 696f  ering, paginatio
+00000290: 6e2c 206f 7264 6572 696e 672e 2054 6869  n, ordering. Thi
+000002a0: 7320 7072 6f6a 6563 7420 6973 2067 656e  s project is gen
+000002b0: 6572 6963 2061 6e64 2072 6575 7361 626c  eric and reusabl
+000002c0: 6520 7761 7920 746f 2063 7265 6174 6520  e way to create 
+000002d0: 7265 7374 7269 6374 6564 2071 7565 7279  restricted query
+000002e0: 7365 7473 2066 6f72 2079 6f75 7220 656e  sets for your en
+000002f0: 6470 6f69 6e74 732e 0a0a 2323 2053 7570  dpoints...## Sup
+00000300: 706f 7274 6564 204f 524d 0a2d 203c 6120  ported ORM.- <a 
+00000310: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000320: 7468 7562 2e63 6f6d 2f74 6f72 746f 6973  thub.com/tortois
+00000330: 652f 746f 7274 6f69 7365 2d6f 726d 2220  e/tortoise-orm" 
+00000340: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000350: 546f 7274 6f69 7365 204f 524d 3c2f 613e  Tortoise ORM</a>
+00000360: 0a0a 2323 2052 6571 7569 7265 6d65 6e74  ..## Requirement
+00000370: 730a 2d20 7079 7468 6f6e 203e 3d33 2e38  s.- python >=3.8
+00000380: 2c3c 342e 300a 2d20 6661 7374 4150 4920  ,<4.0.- fastAPI 
+00000390: 3e3d 2030 2e37 2e30 0a2d 2074 6f72 746f  >= 0.7.0.- torto
+000003a0: 6973 652d 6f72 6d20 3e3d 2030 2e31 382e  ise-orm >= 0.18.
+000003b0: 310a 0a23 2320 496e 7374 616c 6c61 7469  1..## Installati
+000003c0: 6f6e 0a0a 6060 600a 7069 7020 696e 7374  on..```.pip inst
+000003d0: 616c 6c20 6661 7374 6170 692d 7175 6572  all fastapi-quer
+000003e0: 7973 6574 730a 6060 600a 0a23 2051 7569  ysets.```..# Qui
+000003f0: 636b 2074 7574 6f72 6961 6c0a 0a2d 2d2d  ck tutorial..---
+00000400: 0a0a 2d2d 2d0a 0a23 2320 546f 7274 6f69  ..---..## Tortoi
+00000410: 7365 206d 6f64 656c 0a0a 4c65 74e2 8099  se model..Let...
+00000420: 7320 7374 6172 7420 7769 7468 206f 7572  s start with our
+00000430: 206d 6f64 656c 0a0a 6060 6070 7974 686f   model..```pytho
+00000440: 6e0a 2320 6d6f 6465 6c73 2f74 6f72 746f  n.# models/torto
+00000450: 6973 652e 7079 0a0a 696d 706f 7274 2064  ise.py..import d
+00000460: 6174 6574 696d 650a 6672 6f6d 2074 7970  atetime.from typ
+00000470: 696e 6720 696d 706f 7274 204f 7074 696f  ing import Optio
+00000480: 6e61 6c0a 0a66 726f 6d20 746f 7274 6f69  nal..from tortoi
+00000490: 7365 2069 6d70 6f72 7420 4d6f 6465 6c0a  se import Model.
+000004a0: 6672 6f6d 2074 6f72 746f 6973 6520 696d  from tortoise im
+000004b0: 706f 7274 2066 6965 6c64 730a 0a0a 636c  port fields...cl
+000004c0: 6173 7320 5461 736b 284d 6f64 656c 293a  ass Task(Model):
+000004d0: 0a20 2020 2069 643a 2069 6e74 203d 2066  .    id: int = f
+000004e0: 6965 6c64 732e 496e 7446 6965 6c64 2870  ields.IntField(p
+000004f0: 6b3d 5472 7565 290a 2020 2020 6170 7072  k=True).    appr
+00000500: 6f76 6564 3a20 4f70 7469 6f6e 616c 5b62  oved: Optional[b
+00000510: 6f6f 6c5d 203d 2066 6965 6c64 732e 426f  ool] = fields.Bo
+00000520: 6f6c 6561 6e46 6965 6c64 2864 6566 6175  oleanField(defau
+00000530: 6c74 3d46 616c 7365 2c20 6e75 6c6c 3d54  lt=False, null=T
+00000540: 7275 6529 0a20 2020 2063 6f64 653a 2073  rue).    code: s
+00000550: 7472 203d 2066 6965 6c64 732e 4368 6172  tr = fields.Char
+00000560: 4669 656c 6428 6d61 785f 6c65 6e67 7468  Field(max_length
+00000570: 3d36 290a 2020 2020 6372 6561 7465 645f  =6).    created_
+00000580: 6174 3a20 6461 7465 7469 6d65 2e64 6174  at: datetime.dat
+00000590: 6574 696d 6520 3d20 6669 656c 6473 2e44  etime = fields.D
+000005a0: 6174 6574 696d 6546 6965 6c64 2864 6566  atetimeField(def
+000005b0: 6175 6c74 3d64 6174 6574 696d 652e 6461  ault=datetime.da
+000005c0: 7465 7469 6d65 2e6e 6f77 290a 6060 600a  tetime.now).```.
+000005d0: 2d2d 2d0a 0a23 2320 5079 6461 6e74 6963  ---..## Pydantic
+000005e0: 206d 6f64 656c 0a0a 4372 6561 7465 2064   model..Create d
+000005f0: 6174 6162 6173 6520 7265 7072 6573 656e  atabase represen
+00000600: 7461 7469 6f6e 206d 6f64 656c 0a0a 6060  tation model..``
+00000610: 6070 7974 686f 6e0a 2320 6d6f 6465 6c73  `python.# models
+00000620: 2f70 7964 616e 7469 632e 7079 0a0a 6672  /pydantic.py..fr
+00000630: 6f6d 2074 6f72 746f 6973 652e 636f 6e74  om tortoise.cont
+00000640: 7269 622e 7079 6461 6e74 6963 2069 6d70  rib.pydantic imp
+00000650: 6f72 7420 7079 6461 6e74 6963 5f6d 6f64  ort pydantic_mod
+00000660: 656c 5f63 7265 6174 6f72 0a0a 6672 6f6d  el_creator..from
+00000670: 206d 7970 726f 6a65 6374 2e6d 6f64 656c   myproject.model
+00000680: 732e 746f 7274 6f69 7365 2069 6d70 6f72  s.tortoise impor
+00000690: 7420 5461 736b 0a0a 0a54 6173 6b4d 6f64  t Task...TaskMod
+000006a0: 656c 4f75 7420 3d20 7079 6461 6e74 6963  elOut = pydantic
+000006b0: 5f6d 6f64 656c 5f63 7265 6174 6f72 280a  _model_creator(.
+000006c0: 2020 2020 5461 736b 2c0a 2020 2020 6e61      Task,.    na
+000006d0: 6d65 3d22 5461 736b 4d6f 6465 6c4f 7574  me="TaskModelOut
+000006e0: 222c 0a20 2020 2069 6e63 6c75 6465 3d28  ",.    include=(
+000006f0: 0a20 2020 2020 2020 2022 6964 222c 0a20  .        "id",. 
+00000700: 2020 2020 2020 2022 6170 7072 6f76 6564         "approved
+00000710: 222c 0a20 2020 2020 2020 2022 636f 6465  ",.        "code
+00000720: 222c 0a20 2020 2020 2020 2022 6372 6561  ",.        "crea
+00000730: 7465 645f 6174 220a 2020 2020 292c 0a29  ted_at".    ),.)
+00000740: 0a60 6060 0a0a 2d2d 2d0a 0a23 2320 526f  .```..---..## Ro
+00000750: 7574 6572 5175 6572 7953 6574 0a0a 2323  uterQuerySet..##
+00000760: 2320 4669 6c74 6572 730a 0a57 6520 6861  # Filters..We ha
+00000770: 7665 2061 206e 756d 6265 7220 6f66 2066  ve a number of f
+00000780: 6965 6c64 7320 7765 2077 616e 7420 746f  ields we want to
+00000790: 206c 6574 206f 7572 2075 7365 7273 2066   let our users f
+000007a0: 696c 7465 7220 6261 7365 6420 6f6e 2074  ilter based on t
+000007b0: 6865 6d2e 2057 6520 6372 6561 7465 2061  hem. We create a
+000007c0: 2052 6f75 7465 7251 7565 7279 5365 7446   RouterQuerySetF
+000007d0: 696c 7465 7220 666f 7220 7468 6973 2e20  ilter for this. 
+000007e0: 4669 6c74 6572 2063 6c61 7373 2069 7320  Filter class is 
+000007f0: 6172 6775 6d65 6e74 2066 6f72 2060 4661  argument for `Fa
+00000800: 7374 4150 492e 4465 7065 6e64 7360 2061  stAPI.Depends` a
+00000810: 7420 656e 6470 6f69 6e74 2e20 200a 0a59  t endpoint.  ..Y
+00000820: 6f75 2072 6571 7569 7265 2074 6f20 6465  ou require to de
+00000830: 6669 6e65 204f 524d 2066 696c 7465 7220  fine ORM filter 
+00000840: 6b65 7977 6f72 642c 2074 7970 6520 6f66  keyword, type of
+00000850: 2064 6174 6120 616e 6420 7365 7475 7020   data and setup 
+00000860: 736f 7572 6365 206f 6620 6461 7461 2028  source of data (
+00000870: 6051 7565 7279 602c 2060 5061 7468 602c  `Query`, `Path`,
+00000880: 2060 426f 6479 602c 2065 7463 292e 0a0a   `Body`, etc)...
+00000890: 6060 6070 7974 686f 6e0a 2320 7175 6572  ```python.# quer
+000008a0: 7973 6574 735f 6669 6c74 6572 732e 7079  ysets_filters.py
+000008b0: 0a0a 696d 706f 7274 2064 6174 6163 6c61  ..import datacla
+000008c0: 7373 6573 0a69 6d70 6f72 7420 6461 7465  sses.import date
+000008d0: 7469 6d65 0a66 726f 6d20 7479 7069 6e67  time.from typing
+000008e0: 2069 6d70 6f72 7420 4f70 7469 6f6e 616c   import Optional
+000008f0: 0a0a 6672 6f6d 2066 6173 7461 7069 2069  ..from fastapi i
+00000900: 6d70 6f72 7420 5175 6572 790a 0a0a 4064  mport Query...@d
+00000910: 6174 6163 6c61 7373 6573 2e64 6174 6163  ataclasses.datac
+00000920: 6c61 7373 0a63 6c61 7373 2052 6f75 7465  lass.class Route
+00000930: 7251 7565 7279 5365 7446 696c 7465 723a  rQuerySetFilter:
+00000940: 0a20 2020 2069 645f 5f69 6e3a 204f 7074  .    id__in: Opt
+00000950: 696f 6e61 6c5b 6c69 7374 5b69 6e74 5d5d  ional[list[int]]
+00000960: 203d 2051 7565 7279 284e 6f6e 652c 2061   = Query(None, a
+00000970: 6c69 6173 3d27 6964 5b5d 2729 0a20 2020  lias='id[]').   
+00000980: 2061 7070 726f 7665 643a 204f 7074 696f   approved: Optio
+00000990: 6e61 6c5b 626f 6f6c 5d20 3d20 5175 6572  nal[bool] = Quer
+000009a0: 7928 4e6f 6e65 290a 2020 2020 6170 7072  y(None).    appr
+000009b0: 6f76 6564 5f5f 6973 6e75 6c6c 3a20 4f70  oved__isnull: Op
+000009c0: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 2051  tional[bool] = Q
+000009d0: 7565 7279 284e 6f6e 6529 0a20 2020 2063  uery(None).    c
+000009e0: 6f64 653a 204f 7074 696f 6e61 6c5b 7374  ode: Optional[st
+000009f0: 725d 203d 2051 7565 7279 284e 6f6e 6529  r] = Query(None)
+00000a00: 0a20 2020 2063 7265 6174 6564 5f61 745f  .    created_at_
+00000a10: 5f6c 7465 3a20 4f70 7469 6f6e 616c 5b64  _lte: Optional[d
+00000a20: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+00000a30: 5d20 3d20 5175 6572 7928 4e6f 6e65 290a  ] = Query(None).
+00000a40: 2020 2020 6372 6561 7465 645f 6174 5f5f      created_at__
+00000a50: 6774 653a 204f 7074 696f 6e61 6c5b 6461  gte: Optional[da
+00000a60: 7465 7469 6d65 2e64 6174 6574 696d 655d  tetime.datetime]
+00000a70: 203d 2051 7565 7279 284e 6f6e 6529 0a60   = Query(None).`
+00000a80: 6060 0a0a 2323 2320 4d6f 6465 6c20 5175  ``..### Model Qu
+00000a90: 6572 7973 6574 0a0a 436f 6e66 6967 7572  eryset..Configur
+00000aa0: 6520 6052 6f75 7465 7251 7565 7279 7365  e `RouterQueryse
+00000ab0: 7460 2070 726f 7065 7274 6965 730a 0a60  t` properties..`
+00000ac0: 6060 7079 7468 6f6e 0a23 2071 7565 7279  ``python.# query
+00000ad0: 7365 7473 2e70 790a 0a66 726f 6d20 6661  sets.py..from fa
+00000ae0: 7374 6170 695f 7175 6572 7973 6574 732e  stapi_querysets.
+00000af0: 6d69 7869 6e73 2e66 696c 7465 7273 2069  mixins.filters i
+00000b00: 6d70 6f72 7420 4669 6c74 6572 4d69 7869  mport FilterMixi
+00000b10: 6e0a 6672 6f6d 2066 6173 7461 7069 5f71  n.from fastapi_q
+00000b20: 7565 7279 7365 7473 2e6d 6978 696e 732e  uerysets.mixins.
+00000b30: 6669 6c74 6572 7320 696d 706f 7274 2046  filters import F
+00000b40: 696c 7465 724e 6567 6174 696f 6e4d 6978  ilterNegationMix
+00000b50: 696e 0a66 726f 6d20 6661 7374 6170 695f  in.from fastapi_
+00000b60: 7175 6572 7973 6574 732e 6d69 7869 6e73  querysets.mixins
+00000b70: 2e6f 7264 6572 696e 6720 696d 706f 7274  .ordering import
+00000b80: 204f 7264 6572 696e 674d 6978 696e 0a66   OrderingMixin.f
+00000b90: 726f 6d20 6661 7374 6170 695f 7175 6572  rom fastapi_quer
+00000ba0: 7973 6574 732e 6d69 7869 6e73 2e70 6167  ysets.mixins.pag
+00000bb0: 696e 6174 696f 6e20 696d 706f 7274 2050  ination import P
+00000bc0: 6167 696e 6174 696f 6e4d 6978 696e 0a66  aginationMixin.f
+00000bd0: 726f 6d20 6661 7374 6170 695f 7175 6572  rom fastapi_quer
+00000be0: 7973 6574 732e 6d69 7869 6e73 2e70 6167  ysets.mixins.pag
+00000bf0: 696e 6174 696f 6e20 696d 706f 7274 2052  ination import R
+00000c00: 6f75 7465 7250 6167 696e 6174 696f 6e0a  outerPagination.
+00000c10: 6672 6f6d 2066 6173 7461 7069 5f71 7565  from fastapi_que
+00000c20: 7279 7365 7473 2e71 7565 7279 7365 7420  rysets.queryset 
+00000c30: 696d 706f 7274 2052 6f75 7465 7251 7565  import RouterQue
+00000c40: 7279 5365 740a 0a66 726f 6d20 6d79 7072  rySet..from mypr
+00000c50: 6f6a 6563 742e 6d6f 6465 6c73 2e74 6f72  oject.models.tor
+00000c60: 746f 6973 6520 696d 706f 7274 2054 6173  toise import Tas
+00000c70: 6b0a 6672 6f6d 206d 7970 726f 6a65 6374  k.from myproject
+00000c80: 2e71 7565 7279 7365 7473 5f66 696c 7465  .querysets_filte
+00000c90: 7273 2069 6d70 6f72 7420 526f 7574 6572  rs import Router
+00000ca0: 5175 6572 7953 6574 4669 6c74 6572 0a0a  QuerySetFilter..
+00000cb0: 0a63 6c61 7373 2054 6173 6b73 526f 7574  .class TasksRout
+00000cc0: 6572 5175 6572 7953 6574 2846 696c 7465  erQuerySet(Filte
+00000cd0: 724d 6978 696e 2c20 4669 6c74 6572 4e65  rMixin, FilterNe
+00000ce0: 6761 7469 6f6e 4d69 7869 6e2c 204f 7264  gationMixin, Ord
+00000cf0: 6572 696e 674d 6978 696e 2c20 5061 6769  eringMixin, Pagi
+00000d00: 6e61 7469 6f6e 4d69 7869 6e2c 2052 6f75  nationMixin, Rou
+00000d10: 7465 7251 7565 7279 5365 7429 3a0a 2020  terQuerySet):.  
+00000d20: 2020 6669 6c74 6572 5f63 6c61 7373 203d    filter_class =
+00000d30: 2052 6f75 7465 7251 7565 7279 5365 7446   RouterQuerySetF
+00000d40: 696c 7465 720a 2020 2020 6f72 6465 7269  ilter.    orderi
+00000d50: 6e67 5f64 6566 6175 6c74 203d 2022 6964  ng_default = "id
+00000d60: 220a 2020 2020 6f72 6465 7269 6e67 5f66  ".    ordering_f
+00000d70: 6965 6c64 7320 3d20 280a 2020 2020 2020  ields = (.      
+00000d80: 2020 2269 6422 2c0a 2020 2020 2020 2020    "id",.        
+00000d90: 2261 7070 726f 7665 6422 2c0a 2020 2020  "approved",.    
+00000da0: 2020 2020 2263 6f64 6522 2c0a 2020 2020      "code",.    
+00000db0: 2020 2020 2263 7265 6174 6564 5f61 7422      "created_at"
+00000dc0: 2c0a 2020 2020 290a 2020 2020 7061 6769  ,.    ).    pagi
+00000dd0: 6e61 7469 6f6e 5f63 6c61 7373 203d 2052  nation_class = R
+00000de0: 6f75 7465 7250 6167 696e 6174 696f 6e0a  outerPagination.
+00000df0: 2020 2020 6d6f 6465 6c20 3d20 5461 736b      model = Task
+00000e00: 0a60 6060 0a0a 2d2d 2d0a 0a23 2320 4170  .```..---..## Ap
+00000e10: 706c 6963 6174 696f 6e0a 0a43 7265 6174  plication..Creat
+00000e20: 6520 6170 706c 6963 6174 696f 6e2c 2072  e application, r
+00000e30: 6567 6973 7465 7220 6c69 7374 2c20 6c69  egister list, li
+00000e40: 7374 2077 6974 6820 7061 6769 6e61 7469  st with paginati
+00000e50: 6f6e 2061 6e64 2072 6574 7269 6576 6520  on and retrieve 
+00000e60: 656e 6470 6f69 6e74 732e 0a60 6060 7079  endpoints..```py
+00000e70: 7468 6f6e 0a23 2061 7070 2e70 790a 0a66  thon.# app.py..f
+00000e80: 726f 6d20 6661 7374 6170 6920 696d 706f  rom fastapi impo
+00000e90: 7274 2046 6173 7441 5049 0a66 726f 6d20  rt FastAPI.from 
+00000ea0: 746f 7274 6f69 7365 2e63 6f6e 7472 6962  tortoise.contrib
+00000eb0: 2e66 6173 7461 7069 2069 6d70 6f72 7420  .fastapi import 
+00000ec0: 7265 6769 7374 6572 5f74 6f72 746f 6973  register_tortois
+00000ed0: 650a 6672 6f6d 2074 6f72 746f 6973 652e  e.from tortoise.
+00000ee0: 7175 6572 7973 6574 2069 6d70 6f72 7420  queryset import 
+00000ef0: 5175 6572 7953 6574 0a0a 6672 6f6d 206d  QuerySet..from m
+00000f00: 7970 726f 6a65 6374 2e6d 6f64 656c 732e  yproject.models.
+00000f10: 7079 6461 6e74 6963 2069 6d70 6f72 7420  pydantic import 
+00000f20: 5461 736b 4d6f 6465 6c4f 7574 0a66 726f  TaskModelOut.fro
+00000f30: 6d20 6d79 7072 6f6a 6563 742e 6d6f 6465  m myproject.mode
+00000f40: 6c73 2e74 6f72 746f 6973 6520 696d 706f  ls.tortoise impo
+00000f50: 7274 2054 6173 6b0a 6672 6f6d 206d 7970  rt Task.from myp
+00000f60: 726f 6a65 6374 2e71 7565 7279 7365 7473  roject.querysets
+00000f70: 2069 6d70 6f72 7420 5461 736b 7352 6f75   import TasksRou
+00000f80: 7465 7251 7565 7279 5365 740a 0a0a 6170  terQuerySet...ap
+00000f90: 7020 3d20 4661 7374 4150 4928 290a 0a0a  p = FastAPI()...
+00000fa0: 7265 6769 7374 6572 5f74 6f72 746f 6973  register_tortois
+00000fb0: 6528 0a20 2020 2061 7070 2c0a 2020 2020  e(.    app,.    
+00000fc0: 6462 5f75 726c 3d22 7371 6c69 7465 3a2f  db_url="sqlite:/
+00000fd0: 2f3a 6d65 6d6f 7279 3a22 2c0a 2020 2020  /:memory:",.    
+00000fe0: 6d6f 6475 6c65 733d 7b22 6d6f 6465 6c73  modules={"models
+00000ff0: 223a 205b 226d 7970 726f 6a65 6374 2e6d  ": ["myproject.m
+00001000: 6f64 656c 732e 746f 7274 6f69 7365 225d  odels.tortoise"]
+00001010: 7d2c 0a20 2020 2067 656e 6572 6174 655f  },.    generate_
+00001020: 7363 6865 6d61 733d 5472 7565 2c0a 2020  schemas=True,.  
+00001030: 2020 6164 645f 6578 6365 7074 696f 6e5f    add_exception_
+00001040: 6861 6e64 6c65 7273 3d54 7275 652c 0a29  handlers=True,.)
+00001050: 0a0a 0a40 6170 702e 6765 7428 2274 6173  ...@app.get("tas
+00001060: 6b73 2f22 2c20 7265 7370 6f6e 7365 5f6d  ks/", response_m
+00001070: 6f64 656c 3d6c 6973 745b 5461 736b 4d6f  odel=list[TaskMo
+00001080: 6465 6c4f 7574 5d29 0a61 7379 6e63 2064  delOut]).async d
+00001090: 6566 2074 6173 6b73 5f6c 6973 745f 7061  ef tasks_list_pa
+000010a0: 6769 6e61 7465 6428 7175 6572 7973 6574  ginated(queryset
+000010b0: 3a20 5175 6572 7953 6574 5b54 6173 6b5d  : QuerySet[Task]
+000010c0: 203d 2054 6173 6b73 526f 7574 6572 5175   = TasksRouterQu
+000010d0: 6572 7953 6574 2829 2920 2d3e 206c 6973  erySet()) -> lis
+000010e0: 745b 5461 736b 4d6f 6465 6c4f 7574 5d3a  t[TaskModelOut]:
+000010f0: 0a20 2020 2072 6574 7572 6e20 6177 6169  .    return awai
+00001100: 7420 5461 736b 4d6f 6465 6c4f 7574 2e66  t TaskModelOut.f
+00001110: 726f 6d5f 7175 6572 7973 6574 2871 7565  rom_queryset(que
+00001120: 7279 7365 7429 0a0a 0a40 6170 702e 6765  ryset)...@app.ge
+00001130: 7428 2274 6173 6b73 2f70 6167 696e 6174  t("tasks/paginat
+00001140: 6564 222c 2072 6573 706f 6e73 655f 6d6f  ed", response_mo
+00001150: 6465 6c3d 6c69 7374 5b54 6173 6b4d 6f64  del=list[TaskMod
+00001160: 656c 4f75 745d 290a 6173 796e 6320 6465  elOut]).async de
+00001170: 6620 7461 736b 735f 6c69 7374 5f70 6167  f tasks_list_pag
+00001180: 696e 6174 6564 2871 7565 7279 7365 743a  inated(queryset:
+00001190: 2051 7565 7279 5365 745b 5461 736b 5d20   QuerySet[Task] 
+000011a0: 3d20 5461 736b 7352 6f75 7465 7251 7565  = TasksRouterQue
+000011b0: 7279 5365 7428 292e 7061 6769 6e61 7465  rySet().paginate
+000011c0: 6429 202d 3e20 6c69 7374 5b54 6173 6b4d  d) -> list[TaskM
+000011d0: 6f64 656c 4f75 745d 3a0a 2020 2020 7265  odelOut]:.    re
+000011e0: 7475 726e 2061 7761 6974 2054 6173 6b4d  turn await TaskM
+000011f0: 6f64 656c 4f75 742e 6672 6f6d 5f71 7565  odelOut.from_que
+00001200: 7279 7365 7428 7175 6572 7973 6574 290a  ryset(queryset).
+00001210: 0a0a 4061 7070 2e67 6574 2822 7461 736b  ..@app.get("task
+00001220: 732f 7b69 6e73 7461 6e63 655f 6964 7d22  s/{instance_id}"
+00001230: 2c20 7265 7370 6f6e 7365 5f6d 6f64 656c  , response_model
+00001240: 3d6c 6973 745b 5461 736b 4d6f 6465 6c4f  =list[TaskModelO
+00001250: 7574 5d29 0a61 7379 6e63 2064 6566 2074  ut]).async def t
+00001260: 6173 6b73 5f72 6574 7269 6576 6528 7461  asks_retrieve(ta
+00001270: 736b 3a20 5175 6572 7953 6574 5b54 6173  sk: QuerySet[Tas
+00001280: 6b5d 203d 2054 6173 6b73 526f 7574 6572  k] = TasksRouter
+00001290: 5175 6572 7953 6574 2829 2e69 6e73 7461  QuerySet().insta
+000012a0: 6e63 6529 202d 3e20 6c69 7374 5b54 6173  nce) -> list[Tas
+000012b0: 6b4d 6f64 656c 4f75 745d 3a0a 2020 2020  kModelOut]:.    
+000012c0: 7265 7475 726e 2054 6173 6b4d 6f64 656c  return TaskModel
+000012d0: 4f75 742e 6672 6f6d 5f6f 726d 2874 6173  Out.from_orm(tas
+000012e0: 6b29 0a60 6060 0a0a 2d2d 2d0a 0a23 2320  k).```..---..## 
+000012f0: 5265 7175 6573 7473 0a0a 2323 2320 4c69  Requests..### Li
+00001300: 7374 0a0a 4f6e 2072 6571 7565 7374 2065  st..On request e
+00001310: 6666 6563 7469 7665 2071 7565 7279 7365  ffective queryse
+00001320: 7420 7769 6c6c 2062 6520 6669 6c74 6572  t will be filter
+00001330: 6564 2061 6e64 206f 7264 6572 6564 2062  ed and ordered b
+00001340: 7920 7175 6572 7920 7061 7261 6d73 2e0a  y query params..
+00001350: 0a46 6f72 2065 7861 6d70 6c65 2c20 7573  .For example, us
+00001360: 6572 2068 6173 2072 6571 7565 7374 6564  er has requested
+00001370: 2065 6e64 706f 696e 7420 7769 7468 2073   endpoint with s
+00001380: 6f6d 6520 7175 6572 7920 7061 7261 6d73  ome query params
+00001390: 0a60 6060 6a73 6f6e 0a7b 0a20 2020 2022  .```json.{.    "
+000013a0: 6372 6561 7465 645f 6174 5f5f 6c74 6522  created_at__lte"
+000013b0: 3a20 2232 3032 332d 3031 2d30 3154 3030  : "2023-01-01T00
+000013c0: 3a30 303a 3030 222c 0a20 2020 2022 6170  :00:00",.    "ap
+000013d0: 7072 6f76 6564 223a 2066 616c 7365 2c0a  proved": false,.
+000013e0: 2020 2020 226f 7264 6572 696e 675b 5d22      "ordering[]"
+000013f0: 3a20 2263 7265 6174 6564 5f61 7422 2c0a  : "created_at",.
+00001400: 7d0a 6060 600a 0a52 6571 7565 7374 2055  }.```..Request U
+00001410: 524c 206c 6f6f 6b73 206c 696b 6520 200a  RL looks like  .
+00001420: 6060 6068 7474 703a 2f2f 6c6f 6361 6c68  ```http://localh
+00001430: 6f73 743a 3830 3030 2f74 6173 6b73 2f3f  ost:8000/tasks/?
+00001440: 6372 6561 7465 645f 6174 5f5f 6c74 653d  created_at__lte=
+00001450: 3230 3233 2d30 312d 3031 5430 303a 3030  2023-01-01T00:00
+00001460: 3a30 3026 6170 7072 6f76 6564 3d66 616c  :00&approved=fal
+00001470: 7365 266f 7264 6572 696e 675b 5d3d 6372  se&ordering[]=cr
+00001480: 6561 7465 645f 6174 6060 600a 0a45 6666  eated_at```..Eff
+00001490: 6563 7469 7665 2071 7565 7279 7365 7420  ective queryset 
+000014a0: 6174 2074 6865 2065 6e64 706f 696e 7420  at the endpoint 
+000014b0: 6d65 7468 6f64 2077 696c 6c20 6265 0a60  method will be.`
+000014c0: 6060 7079 7468 6f6e 0a28 0a20 2020 2054  ``python.(.    T
+000014d0: 6173 6b0a 2020 2020 2e66 696c 7465 7228  ask.    .filter(
+000014e0: 6372 6561 7465 645f 6174 5f5f 6c74 653d  created_at__lte=
+000014f0: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
+00001500: 6528 3230 3233 2c20 312c 2031 2c20 302c  e(2023, 1, 1, 0,
+00001510: 2030 2c20 3029 2c20 6170 7072 6f76 6564   0, 0), approved
+00001520: 3d46 616c 7365 290a 2020 2020 2e6f 7264  =False).    .ord
+00001530: 6572 5f62 7928 2263 7265 6174 6564 5f61  er_by("created_a
+00001540: 7422 290a 290a 6060 600a 0a23 2323 204c  t").).```..### L
+00001550: 6973 7420 7061 6769 6e61 7465 640a 0a4c  ist paginated..L
+00001560: 696b 6520 6e6f 7420 7061 6769 6e61 7465  ike not paginate
+00001570: 6420 656e 6470 6f69 6e74 2061 7420 7468  d endpoint at th
+00001580: 6973 2071 7565 7279 7365 7420 7769 6c6c  is queryset will
+00001590: 2062 6520 6669 6c74 6572 6564 2c20 6f72   be filtered, or
+000015a0: 6465 7269 6e67 2061 6e64 2061 6464 6974  dering and addit
+000015b0: 696f 6e61 6c20 7061 6769 6e61 7465 642e  ional paginated.
+000015c0: 0a0a 466f 7220 6578 616d 706c 652c 2075  ..For example, u
+000015d0: 7365 7220 6861 7320 7265 7175 6573 7465  ser has requeste
+000015e0: 6420 656e 6470 6f69 6e74 2077 6974 6820  d endpoint with 
+000015f0: 736f 6d65 2071 7565 7279 2070 6172 616d  some query param
+00001600: 730a 6060 606a 736f 6e0a 7b0a 2020 2020  s.```json.{.    
+00001610: 2270 6167 6522 3a20 322c 0a20 2020 2022  "page": 2,.    "
+00001620: 7065 725f 7061 6765 223a 2031 302c 0a20  per_page": 10,. 
+00001630: 2020 2022 6372 6561 7465 645f 6174 5f5f     "created_at__
+00001640: 6c74 6522 3a20 2232 3032 332d 3031 2d30  lte": "2023-01-0
+00001650: 3154 3030 3a30 303a 3030 222c 0a20 2020  1T00:00:00",.   
+00001660: 2022 6170 7072 6f76 6564 223a 2066 616c   "approved": fal
+00001670: 7365 2c0a 2020 2020 226f 7264 6572 696e  se,.    "orderin
+00001680: 675b 5d22 3a20 2263 7265 6174 6564 5f61  g[]": "created_a
+00001690: 7422 2c0a 7d0a 6060 600a 0a52 6571 7565  t",.}.```..Reque
+000016a0: 7374 2055 524c 206c 6f6f 6b73 206c 696b  st URL looks lik
+000016b0: 6520 2020 0a60 6060 6874 7470 3a2f 2f6c  e   .```http://l
+000016c0: 6f63 616c 686f 7374 3a38 3030 302f 7461  ocalhost:8000/ta
+000016d0: 736b 732f 3f70 6167 653d 3226 7065 725f  sks/?page=2&per_
+000016e0: 7061 6765 3d31 3026 6372 6561 7465 645f  page=10&created_
+000016f0: 6174 5f5f 6c74 653d 3230 3233 2d30 312d  at__lte=2023-01-
+00001700: 3031 5430 303a 3030 3a30 3026 6170 7072  01T00:00:00&appr
+00001710: 6f76 6564 3d66 616c 7365 266f 7264 6572  oved=false&order
+00001720: 696e 675b 5d3d 6372 6561 7465 645f 6174  ing[]=created_at
+00001730: 6060 600a 0a0a 4566 6665 6374 6976 6520  ```...Effective 
+00001740: 7175 6572 7973 6574 2061 7420 656e 6470  queryset at endp
+00001750: 6f69 6e74 206d 6574 686f 6420 7769 6c6c  oint method will
+00001760: 2062 650a 6060 6070 7974 686f 6e0a 280a   be.```python.(.
+00001770: 2020 2020 5461 736b 0a20 2020 202e 6669      Task.    .fi
+00001780: 6c74 6572 2863 7265 6174 6564 5f61 745f  lter(created_at_
+00001790: 5f6c 7465 3d64 6174 6574 696d 652e 6461  _lte=datetime.da
+000017a0: 7465 7469 6d65 2832 3032 332c 2031 2c20  tetime(2023, 1, 
+000017b0: 312c 2030 2c20 302c 2030 292c 2061 7070  1, 0, 0, 0), app
+000017c0: 726f 7665 643d 4661 6c73 6529 0a20 2020  roved=False).   
+000017d0: 202e 6f72 6465 725f 6279 2822 6372 6561   .order_by("crea
+000017e0: 7465 645f 6174 2229 0a20 2020 202e 6f66  ted_at").    .of
+000017f0: 6673 6574 2831 3029 0a20 2020 202e 6c69  fset(10).    .li
+00001800: 6d69 7428 3130 290a 290a 6060 600a 0a41  mit(10).).```..A
+00001810: 7320 7765 6c6c 2061 7320 746f 2060 5265  s well as to `Re
+00001820: 7370 6f6e 7365 6020 7769 6c6c 2062 6520  sponse` will be 
+00001830: 6164 6465 6420 7061 6769 6e61 7469 6f6e  added pagination
+00001840: 2069 6e66 6f72 6d61 7469 6f6e 2e20 5061   information. Pa
+00001850: 6769 6e61 7469 6f6e 2069 6e66 6f72 6d61  gination informa
+00001860: 7469 6f6e 2061 6c77 6179 7320 6d61 7463  tion always matc
+00001870: 6865 7320 6566 6665 6374 6976 6520 7175  hes effective qu
+00001880: 6572 7973 6574 0a60 6060 6a73 6f6e 0a7b  eryset.```json.{
+00001890: 0a20 2020 2022 782d 7061 6765 223a 2022  .    "x-page": "
+000018a0: 3222 2c0a 2020 2020 2278 2d70 6167 6573  2",.    "x-pages
+000018b0: 223a 2022 3422 2c0a 2020 2020 2278 2d70  ": "4",.    "x-p
+000018c0: 6572 2d70 6167 6522 3a20 2231 3022 2c0a  er-page": "10",.
+000018d0: 2020 2020 2278 2d74 6f74 616c 223a 2022      "x-total": "
+000018e0: 3332 220a 7d0a 6060 600a 0a23 2323 2052  32".}.```..### R
+000018f0: 6574 7269 6576 650a 0a52 6571 7565 7374  etrieve..Request
+00001900: 2055 524c 206c 6f6f 6b73 206c 696b 6520   URL looks like 
+00001910: 2020 0a60 6060 6874 7470 3a2f 2f6c 6f63    .```http://loc
+00001920: 616c 686f 7374 3a38 3030 302f 7461 736b  alhost:8000/task
+00001930: 732f 3130 2f60 6060 0a0a 456e 6470 6f69  s/10/```..Endpoi
+00001940: 6e74 206d 6574 686f 6420 7769 6c6c 2067  nt method will g
+00001950: 6574 2060 5461 736b 6020 7769 7468 2060  et `Task` with `
+00001960: 6964 203d 3d20 3130 6020 6173 2061 7267  id == 10` as arg
+00001970: 756d 656e 7420 6074 6173 6b60 2e20 2020  ument `task`.   
+00001980: 2020 0a49 6620 6054 6173 6b60 2077 6974    .If `Task` wit
+00001990: 6820 6069 6420 3d3d 2031 3060 2064 6f65  h `id == 10` doe
+000019a0: 7320 6e6f 7420 6578 6973 7420 7468 656e  s not exist then
+000019b0: 2065 6e64 706f 696e 7420 7265 7475 726e   endpoint return
+000019c0: 2060 5265 7370 6f6e 7365 2834 3034 2960   `Response(404)`
+000019d0: 2020
```

### Comparing `fastapi_querysets-0.1.1/setup.py` & `fastapi_querysets-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,475 +1,470 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2766 6173 7461 7069 5f71 7565   \.['fastapi_que
-00000050: 7279 7365 7473 272c 2027 6661 7374 6170  rysets', 'fastap
-00000060: 695f 7175 6572 7973 6574 732e 6d69 7869  i_querysets.mixi
-00000070: 6e73 275d 0a0a 7061 636b 6167 655f 6461  ns']..package_da
-00000080: 7461 203d 205c 0a7b 2727 3a20 5b27 2a27  ta = \.{'': ['*'
-00000090: 5d7d 0a0a 696e 7374 616c 6c5f 7265 7175  ]}..install_requ
-000000a0: 6972 6573 203d 205c 0a5b 2766 6173 7461  ires = \.['fasta
-000000b0: 7069 2d64 6570 656e 6473 2d65 7874 3e3d  pi-depends-ext>=
-000000c0: 302e 322e 3227 2c20 2766 6173 7461 7069  0.2.2', 'fastapi
-000000d0: 3e3d 302e 3730 2e30 272c 2027 746f 7274  >=0.70.0', 'tort
-000000e0: 6f69 7365 2d6f 726d 3e3d 302e 3138 2e31  oise-orm>=0.18.1
-000000f0: 275d 0a0a 7365 7475 705f 6b77 6172 6773  ']..setup_kwargs
-00000100: 203d 207b 0a20 2020 2027 6e61 6d65 273a   = {.    'name':
-00000110: 2027 6661 7374 6170 692d 7175 6572 7973   'fastapi-querys
-00000120: 6574 7327 2c0a 2020 2020 2776 6572 7369  ets',.    'versi
-00000130: 6f6e 273a 2027 302e 312e 3127 2c0a 2020  on': '0.1.1',.  
-00000140: 2020 2764 6573 6372 6970 7469 6f6e 273a    'description':
-00000150: 2027 272c 0a20 2020 2027 6c6f 6e67 5f64   '',.    'long_d
-00000160: 6573 6372 6970 7469 6f6e 273a 2027 2320  escription': '# 
-00000170: 4661 7374 4150 4920 5175 6572 7973 6574  FastAPI Queryset
-00000180: 735c 6e21 5b43 444e 4a53 5d28 6874 7470  s\n![CDNJS](http
-00000190: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000001a0: 696f 2f62 6164 6765 2f50 7974 686f 6e2d  io/badge/Python-
-000001b0: 332e 3825 3230 2537 4325 3230 332e 3925  3.8%20%7C%203.9%
-000001c0: 3230 2537 4325 3230 332e 3130 2532 3025  20%7C%203.10%20%
-000001d0: 3743 2532 3033 2e31 312d 3233 3334 4430  7C%203.11-2334D0
-000001e0: 3538 295c 6e21 5b43 444e 4a53 5d28 6874  58)\n![CDNJS](ht
-000001f0: 7470 733a 2f2f 7368 6965 6c64 732e 696f  tps://shields.io
-00000200: 2f62 6164 6765 2f46 6173 7441 5049 2d25  /badge/FastAPI-%
-00000210: 3345 3d30 2e37 2e30 2d30 3039 3438 3529  3E=0.7.0-009485)
-00000220: 5c6e 5c6e 2d2d 2d5c 6e2a 2a44 6f63 756d  \n\n---\n**Docum
-00000230: 656e 7461 7469 6f6e 2a2a 3a20 3c61 2068  entation**: <a h
-00000240: 7265 663d 2268 7474 7073 3a2f 2f66 6173  ref="https://fas
-00000250: 7461 7069 2d71 7565 7279 7365 7473 2e72  tapi-querysets.r
-00000260: 6561 6474 6865 646f 6373 2e69 6f22 2074  eadthedocs.io" t
-00000270: 6172 6765 743d 225f 626c 616e 6b22 3e68  arget="_blank">h
-00000280: 7474 7073 3a2f 2f66 6173 7461 7069 2d71  ttps://fastapi-q
-00000290: 7565 7279 7365 7473 2e72 6561 6474 6865  uerysets.readthe
-000002a0: 646f 6373 2e69 6f3c 2f61 3e5c 6e5c 6e2a  docs.io</a>\n\n*
-000002b0: 2a53 6f75 7263 6520 436f 6465 2a2a 3a20  *Source Code**: 
-000002c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000002d0: 2f67 6974 6875 622e 636f 6d2f 4e69 6b61  /github.com/Nika
-000002e0: 6b74 6f2f 6661 7374 6170 692d 7175 6572  kto/fastapi-quer
-000002f0: 7973 6574 7322 2074 6172 6765 743d 225f  ysets" target="_
-00000300: 626c 616e 6b22 3e68 7474 7073 3a2f 2f67  blank">https://g
-00000310: 6974 6875 622e 636f 6d2f 4e69 6b61 6b74  ithub.com/Nikakt
-00000320: 6f2f 6661 7374 6170 692d 7175 6572 7973  o/fastapi-querys
-00000330: 6574 733c 2f61 3e5c 6e5c 6e2d 2d2d 5c6e  ets</a>\n\n---\n
-00000340: 5c6e 2323 2057 6879 2074 6f20 7573 653f  \n## Why to use?
-00000350: 5c6e 5c6e 5768 696c 6520 796f 7520 6172  \n\nWhile you ar
-00000360: 6520 6465 7665 6c6f 7069 6e67 2046 6173  e developing Fas
-00000370: 7441 5049 2061 7070 6c69 6361 7469 6f6e  tAPI application
-00000380: 7320 796f 7520 6172 6520 7573 696e 6720  s you are using 
-00000390: 6461 7461 6261 7365 7320 7769 7468 204f  databases with O
-000003a0: 524d 2e20 4d6f 7374 206f 6620 7468 6520  RM. Most of the 
-000003b0: 656e 6470 6f69 6e74 7320 6172 6520 7669  endpoints are vi
-000003c0: 6577 206f 6620 6461 7461 6261 7365 2074  ew of database t
-000003d0: 6162 6c65 7320 616e 6420 7265 7175 6972  ables and requir
-000003e0: 6520 7265 7374 7269 6374 2071 7565 7279  e restrict query
-000003f0: 7365 7420 6279 2066 696c 7465 7269 6e67  set by filtering
-00000400: 2c20 7061 6769 6e61 7469 6f6e 2c20 6f72  , pagination, or
-00000410: 6465 7269 6e67 2e20 5468 6973 2070 726f  dering. This pro
-00000420: 6a65 6374 2069 7320 6765 6e65 7269 6320  ject is generic 
-00000430: 616e 6420 7265 7573 6162 6c65 2077 6179  and reusable way
-00000440: 2074 6f20 6372 6561 7465 2072 6573 7472   to create restr
-00000450: 6963 7465 6420 7175 6572 7973 6574 7320  icted querysets 
-00000460: 666f 7220 796f 7572 2065 6e64 706f 696e  for your endpoin
-00000470: 7473 2e5c 6e5c 6e23 2320 5375 7070 6f72  ts.\n\n## Suppor
-00000480: 7465 6420 4f52 4d5c 6e2d 203c 6120 6872  ted ORM\n- <a hr
-00000490: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000004a0: 7562 2e63 6f6d 2f74 6f72 746f 6973 652f  ub.com/tortoise/
-000004b0: 746f 7274 6f69 7365 2d6f 726d 2220 7461  tortoise-orm" ta
-000004c0: 7267 6574 3d22 5f62 6c61 6e6b 223e 546f  rget="_blank">To
-000004d0: 7274 6f69 7365 204f 524d 3c2f 613e 5c6e  rtoise ORM</a>\n
-000004e0: 5c6e 2323 2052 6571 7569 7265 6d65 6e74  \n## Requirement
-000004f0: 735c 6e2d 2070 7974 686f 6e20 3e3d 332e  s\n- python >=3.
-00000500: 382c 3c34 2e30 5c6e 2d20 6661 7374 4150  8,<4.0\n- fastAP
-00000510: 4920 3e3d 2030 2e37 2e30 5c6e 2d20 746f  I >= 0.7.0\n- to
-00000520: 7274 6f69 7365 2d6f 726d 203e 3d20 302e  rtoise-orm >= 0.
-00000530: 3138 2e31 5c6e 5c6e 2323 2049 6e73 7461  18.1\n\n## Insta
-00000540: 6c6c 6174 696f 6e5c 6e5c 6e60 6060 5c6e  llation\n\n```\n
-00000550: 7069 7020 696e 7374 616c 6c20 6661 7374  pip install fast
-00000560: 6170 692d 7175 6572 7973 6574 735c 6e60  api-querysets\n`
-00000570: 6060 5c6e 5c6e 2320 5175 6963 6b20 7475  ``\n\n# Quick tu
-00000580: 746f 7269 616c 5c6e 5c6e 2d2d 2d5c 6e5c  torial\n\n---\n\
-00000590: 6e2d 2d2d 5c6e 5c6e 2323 2054 6f72 746f  n---\n\n## Torto
-000005a0: 6973 6520 6d6f 6465 6c5c 6e5c 6e4c 6574  ise model\n\nLet
-000005b0: e280 9973 2073 7461 7274 2077 6974 6820  ...s start with 
-000005c0: 6f75 7220 6d6f 6465 6c5c 6e5c 6e60 6060  our model\n\n```
-000005d0: 7079 7468 6f6e 5c6e 2320 6d6f 6465 6c73  python\n# models
-000005e0: 2f74 6f72 746f 6973 652e 7079 5c6e 5c6e  /tortoise.py\n\n
-000005f0: 696d 706f 7274 2064 6174 6574 696d 655c  import datetime\
-00000600: 6e66 726f 6d20 7479 7069 6e67 2069 6d70  nfrom typing imp
-00000610: 6f72 7420 4f70 7469 6f6e 616c 5c6e 5c6e  ort Optional\n\n
-00000620: 6672 6f6d 2074 6f72 746f 6973 6520 696d  from tortoise im
-00000630: 706f 7274 204d 6f64 656c 5c6e 6672 6f6d  port Model\nfrom
-00000640: 2074 6f72 746f 6973 6520 696d 706f 7274   tortoise import
-00000650: 2066 6965 6c64 735c 6e5c 6e5c 6e63 6c61   fields\n\n\ncla
-00000660: 7373 2054 6173 6b28 4d6f 6465 6c29 3a5c  ss Task(Model):\
-00000670: 6e20 2020 2069 643a 2069 6e74 203d 2066  n    id: int = f
-00000680: 6965 6c64 732e 496e 7446 6965 6c64 2870  ields.IntField(p
-00000690: 6b3d 5472 7565 295c 6e20 2020 2061 7070  k=True)\n    app
-000006a0: 726f 7665 643a 204f 7074 696f 6e61 6c5b  roved: Optional[
-000006b0: 626f 6f6c 5d20 3d20 6669 656c 6473 2e42  bool] = fields.B
-000006c0: 6f6f 6c65 616e 4669 656c 6428 6465 6661  ooleanField(defa
-000006d0: 756c 743d 4661 6c73 652c 206e 756c 6c3d  ult=False, null=
-000006e0: 5472 7565 295c 6e20 2020 2063 6f64 653a  True)\n    code:
-000006f0: 2073 7472 203d 2066 6965 6c64 732e 4368   str = fields.Ch
-00000700: 6172 4669 656c 6428 6d61 785f 6c65 6e67  arField(max_leng
-00000710: 7468 3d36 295c 6e20 2020 2063 7265 6174  th=6)\n    creat
-00000720: 6564 5f61 743a 2064 6174 6574 696d 652e  ed_at: datetime.
-00000730: 6461 7465 7469 6d65 203d 2066 6965 6c64  datetime = field
-00000740: 732e 4461 7465 7469 6d65 4669 656c 6428  s.DatetimeField(
-00000750: 6465 6661 756c 743d 6461 7465 7469 6d65  default=datetime
-00000760: 2e64 6174 6574 696d 652e 6e6f 7729 5c6e  .datetime.now)\n
-00000770: 6060 605c 6e2d 2d2d 5c6e 5c6e 2323 2050  ```\n---\n\n## P
-00000780: 7964 616e 7469 6320 6d6f 6465 6c5c 6e5c  ydantic model\n\
-00000790: 6e43 7265 6174 6520 6461 7461 6261 7365  nCreate database
-000007a0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-000007b0: 6d6f 6465 6c5c 6e5c 6e60 6060 7079 7468  model\n\n```pyth
-000007c0: 6f6e 5c6e 2320 6d6f 6465 6c73 2f70 7964  on\n# models/pyd
-000007d0: 616e 7469 632e 7079 5c6e 5c6e 6672 6f6d  antic.py\n\nfrom
-000007e0: 2074 6f72 746f 6973 652e 636f 6e74 7269   tortoise.contri
-000007f0: 622e 7079 6461 6e74 6963 2069 6d70 6f72  b.pydantic impor
-00000800: 7420 7079 6461 6e74 6963 5f6d 6f64 656c  t pydantic_model
-00000810: 5f63 7265 6174 6f72 5c6e 5c6e 6672 6f6d  _creator\n\nfrom
-00000820: 206d 7970 726f 6a65 6374 2e6d 6f64 656c   myproject.model
-00000830: 732e 746f 7274 6f69 7365 2069 6d70 6f72  s.tortoise impor
-00000840: 7420 5461 736b 5c6e 5c6e 5c6e 5461 736b  t Task\n\n\nTask
-00000850: 4d6f 6465 6c4f 7574 203d 2070 7964 616e  ModelOut = pydan
-00000860: 7469 635f 6d6f 6465 6c5f 6372 6561 746f  tic_model_creato
-00000870: 7228 5c6e 2020 2020 5461 736b 2c5c 6e20  r(\n    Task,\n 
-00000880: 2020 206e 616d 653d 2254 6173 6b4d 6f64     name="TaskMod
-00000890: 656c 4f75 7422 2c5c 6e20 2020 2069 6e63  elOut",\n    inc
-000008a0: 6c75 6465 3d28 5c6e 2020 2020 2020 2020  lude=(\n        
-000008b0: 2269 6422 2c5c 6e20 2020 2020 2020 2022  "id",\n        "
-000008c0: 6170 7072 6f76 6564 222c 5c6e 2020 2020  approved",\n    
-000008d0: 2020 2020 2263 6f64 6522 2c5c 6e20 2020      "code",\n   
-000008e0: 2020 2020 2022 6372 6561 7465 645f 6174       "created_at
-000008f0: 225c 6e20 2020 2029 2c5c 6e29 5c6e 6060  "\n    ),\n)\n``
-00000900: 605c 6e5c 6e2d 2d2d 5c6e 5c6e 2323 2052  `\n\n---\n\n## R
-00000910: 6f75 7465 7251 7565 7279 5365 745c 6e5c  outerQuerySet\n\
-00000920: 6e23 2323 2046 696c 7465 7273 5c6e 5c6e  n### Filters\n\n
-00000930: 5765 2068 6176 6520 6120 6e75 6d62 6572  We have a number
-00000940: 206f 6620 6669 656c 6473 2077 6520 7761   of fields we wa
-00000950: 6e74 2074 6f20 6c65 7420 6f75 7220 7573  nt to let our us
-00000960: 6572 7320 6669 6c74 6572 2062 6173 6564  ers filter based
-00000970: 206f 6e20 7468 656d 2e20 5765 2063 7265   on them. We cre
-00000980: 6174 6520 6120 526f 7574 6572 5175 6572  ate a RouterQuer
-00000990: 7953 6574 4669 6c74 6572 2066 6f72 2074  ySetFilter for t
-000009a0: 6869 732e 2046 696c 7465 7220 636c 6173  his. Filter clas
-000009b0: 7320 6973 2061 7267 756d 656e 7420 666f  s is argument fo
-000009c0: 7220 6046 6173 7441 5049 2e44 6570 656e  r `FastAPI.Depen
-000009d0: 6473 6020 6174 2065 6e64 706f 696e 742e  ds` at endpoint.
-000009e0: 2020 5c6e 5c6e 596f 7520 7265 7175 6972    \n\nYou requir
-000009f0: 6520 746f 2064 6566 696e 6520 4f52 4d20  e to define ORM 
-00000a00: 6669 6c74 6572 206b 6579 776f 7264 2c20  filter keyword, 
-00000a10: 7479 7065 206f 6620 6461 7461 2061 6e64  type of data and
-00000a20: 2073 6574 7570 2073 6f75 7263 6520 6f66   setup source of
-00000a30: 2064 6174 6120 2860 5175 6572 7960 2c20   data (`Query`, 
-00000a40: 6050 6174 6860 2c20 6042 6f64 7960 2c20  `Path`, `Body`, 
-00000a50: 6574 6329 2e5c 6e5c 6e60 6060 7079 7468  etc).\n\n```pyth
-00000a60: 6f6e 5c6e 2320 7175 6572 7973 6574 735f  on\n# querysets_
-00000a70: 6669 6c74 6572 732e 7079 5c6e 5c6e 696d  filters.py\n\nim
-00000a80: 706f 7274 2064 6174 6163 6c61 7373 6573  port dataclasses
-00000a90: 5c6e 696d 706f 7274 2064 6174 6574 696d  \nimport datetim
-00000aa0: 655c 6e66 726f 6d20 7479 7069 6e67 2069  e\nfrom typing i
-00000ab0: 6d70 6f72 7420 4f70 7469 6f6e 616c 5c6e  mport Optional\n
-00000ac0: 5c6e 6672 6f6d 2066 6173 7461 7069 2069  \nfrom fastapi i
-00000ad0: 6d70 6f72 7420 5175 6572 795c 6e5c 6e5c  mport Query\n\n\
-00000ae0: 6e40 6461 7461 636c 6173 7365 732e 6461  n@dataclasses.da
-00000af0: 7461 636c 6173 735c 6e63 6c61 7373 2052  taclass\nclass R
-00000b00: 6f75 7465 7251 7565 7279 5365 7446 696c  outerQuerySetFil
-00000b10: 7465 723a 5c6e 2020 2020 6964 5f5f 696e  ter:\n    id__in
-00000b20: 3a20 4f70 7469 6f6e 616c 5b6c 6973 745b  : Optional[list[
-00000b30: 696e 745d 5d20 3d20 5175 6572 7928 4e6f  int]] = Query(No
-00000b40: 6e65 2c20 616c 6961 733d 5c27 6964 5b5d  ne, alias=\'id[]
-00000b50: 5c27 295c 6e20 2020 2061 7070 726f 7665  \')\n    approve
-00000b60: 643a 204f 7074 696f 6e61 6c5b 626f 6f6c  d: Optional[bool
-00000b70: 5d20 3d20 5175 6572 7928 4e6f 6e65 295c  ] = Query(None)\
-00000b80: 6e20 2020 2061 7070 726f 7665 645f 5f69  n    approved__i
-00000b90: 736e 756c 6c3a 204f 7074 696f 6e61 6c5b  snull: Optional[
-00000ba0: 626f 6f6c 5d20 3d20 5175 6572 7928 4e6f  bool] = Query(No
-00000bb0: 6e65 295c 6e20 2020 2063 6f64 653a 204f  ne)\n    code: O
-00000bc0: 7074 696f 6e61 6c5b 7374 725d 203d 2051  ptional[str] = Q
-00000bd0: 7565 7279 284e 6f6e 6529 5c6e 2020 2020  uery(None)\n    
-00000be0: 6372 6561 7465 645f 6174 5f5f 6c74 653a  created_at__lte:
-00000bf0: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
-00000c00: 6d65 2e64 6174 6574 696d 655d 203d 2051  me.datetime] = Q
-00000c10: 7565 7279 284e 6f6e 6529 5c6e 2020 2020  uery(None)\n    
-00000c20: 6372 6561 7465 645f 6174 5f5f 6774 653a  created_at__gte:
-00000c30: 204f 7074 696f 6e61 6c5b 6461 7465 7469   Optional[dateti
-00000c40: 6d65 2e64 6174 6574 696d 655d 203d 2051  me.datetime] = Q
-00000c50: 7565 7279 284e 6f6e 6529 5c6e 6060 605c  uery(None)\n```\
-00000c60: 6e5c 6e23 2323 204d 6f64 656c 2051 7565  n\n### Model Que
-00000c70: 7279 7365 745c 6e5c 6e43 6f6e 6669 6775  ryset\n\nConfigu
-00000c80: 7265 2060 526f 7574 6572 5175 6572 7973  re `RouterQuerys
-00000c90: 6574 6020 7072 6f70 6572 7469 6573 5c6e  et` properties\n
-00000ca0: 5c6e 6060 6070 7974 686f 6e5c 6e23 2071  \n```python\n# q
-00000cb0: 7565 7279 7365 7473 2e70 795c 6e5c 6e66  uerysets.py\n\nf
-00000cc0: 726f 6d20 6661 7374 6170 695f 7175 6572  rom fastapi_quer
-00000cd0: 7973 6574 732e 6d69 7869 6e73 2e66 696c  ysets.mixins.fil
-00000ce0: 7465 7273 2069 6d70 6f72 7420 4669 6c74  ters import Filt
-00000cf0: 6572 4d69 7869 6e5c 6e66 726f 6d20 6661  erMixin\nfrom fa
-00000d00: 7374 6170 695f 7175 6572 7973 6574 732e  stapi_querysets.
-00000d10: 6d69 7869 6e73 2e66 696c 7465 7273 2069  mixins.filters i
-00000d20: 6d70 6f72 7420 4669 6c74 6572 4e65 6761  mport FilterNega
-00000d30: 7469 6f6e 4d69 7869 6e5c 6e66 726f 6d20  tionMixin\nfrom 
-00000d40: 6661 7374 6170 695f 7175 6572 7973 6574  fastapi_queryset
-00000d50: 732e 6d69 7869 6e73 2e6f 7264 6572 696e  s.mixins.orderin
-00000d60: 6720 696d 706f 7274 204f 7264 6572 696e  g import Orderin
-00000d70: 674d 6978 696e 5c6e 6672 6f6d 2066 6173  gMixin\nfrom fas
-00000d80: 7461 7069 5f71 7565 7279 7365 7473 2e6d  tapi_querysets.m
-00000d90: 6978 696e 732e 7061 6769 6e61 7469 6f6e  ixins.pagination
-00000da0: 2069 6d70 6f72 7420 5061 6769 6e61 7469   import Paginati
-00000db0: 6f6e 4d69 7869 6e5c 6e66 726f 6d20 6661  onMixin\nfrom fa
-00000dc0: 7374 6170 695f 7175 6572 7973 6574 732e  stapi_querysets.
-00000dd0: 6d69 7869 6e73 2e70 6167 696e 6174 696f  mixins.paginatio
-00000de0: 6e20 696d 706f 7274 2052 6f75 7465 7250  n import RouterP
-00000df0: 6167 696e 6174 696f 6e5c 6e66 726f 6d20  agination\nfrom 
-00000e00: 6661 7374 6170 695f 7175 6572 7973 6574  fastapi_queryset
-00000e10: 732e 7175 6572 7973 6574 2069 6d70 6f72  s.queryset impor
-00000e20: 7420 526f 7574 6572 5175 6572 7953 6574  t RouterQuerySet
-00000e30: 5c6e 5c6e 6672 6f6d 206d 7970 726f 6a65  \n\nfrom myproje
-00000e40: 6374 2e6d 6f64 656c 732e 746f 7274 6f69  ct.models.tortoi
-00000e50: 7365 2069 6d70 6f72 7420 5461 736b 5c6e  se import Task\n
-00000e60: 6672 6f6d 206d 7970 726f 6a65 6374 2e71  from myproject.q
-00000e70: 7565 7279 7365 7473 5f66 696c 7465 7273  uerysets_filters
-00000e80: 2069 6d70 6f72 7420 526f 7574 6572 5175   import RouterQu
-00000e90: 6572 7953 6574 4669 6c74 6572 5c6e 5c6e  erySetFilter\n\n
-00000ea0: 5c6e 636c 6173 7320 5461 736b 7352 6f75  \nclass TasksRou
-00000eb0: 7465 7251 7565 7279 5365 7428 4669 6c74  terQuerySet(Filt
-00000ec0: 6572 4d69 7869 6e2c 2046 696c 7465 724e  erMixin, FilterN
-00000ed0: 6567 6174 696f 6e4d 6978 696e 2c20 4f72  egationMixin, Or
-00000ee0: 6465 7269 6e67 4d69 7869 6e2c 2050 6167  deringMixin, Pag
-00000ef0: 696e 6174 696f 6e4d 6978 696e 2c20 526f  inationMixin, Ro
-00000f00: 7574 6572 5175 6572 7953 6574 293a 5c6e  uterQuerySet):\n
-00000f10: 2020 2020 6669 6c74 6572 5f63 6c61 7373      filter_class
-00000f20: 203d 2052 6f75 7465 7251 7565 7279 5365   = RouterQuerySe
-00000f30: 7446 696c 7465 725c 6e20 2020 206f 7264  tFilter\n    ord
-00000f40: 6572 696e 675f 6465 6661 756c 7420 3d20  ering_default = 
-00000f50: 2269 6422 5c6e 2020 2020 6f72 6465 7269  "id"\n    orderi
-00000f60: 6e67 5f66 6965 6c64 7320 3d20 285c 6e20  ng_fields = (\n 
-00000f70: 2020 2020 2020 2022 6964 222c 5c6e 2020         "id",\n  
-00000f80: 2020 2020 2020 2261 7070 726f 7665 6422        "approved"
-00000f90: 2c5c 6e20 2020 2020 2020 2022 636f 6465  ,\n        "code
-00000fa0: 222c 5c6e 2020 2020 2020 2020 2263 7265  ",\n        "cre
-00000fb0: 6174 6564 5f61 7422 2c5c 6e20 2020 2029  ated_at",\n    )
-00000fc0: 5c6e 2020 2020 7061 6769 6e61 7469 6f6e  \n    pagination
-00000fd0: 5f63 6c61 7373 203d 2052 6f75 7465 7250  _class = RouterP
-00000fe0: 6167 696e 6174 696f 6e5c 6e20 2020 206d  agination\n    m
-00000ff0: 6f64 656c 203d 2054 6173 6b5c 6e60 6060  odel = Task\n```
-00001000: 5c6e 5c6e 2d2d 2d5c 6e5c 6e23 2320 4170  \n\n---\n\n## Ap
-00001010: 706c 6963 6174 696f 6e5c 6e5c 6e43 7265  plication\n\nCre
-00001020: 6174 6520 6170 706c 6963 6174 696f 6e2c  ate application,
-00001030: 2072 6567 6973 7465 7220 6c69 7374 2c20   register list, 
-00001040: 6c69 7374 2077 6974 6820 7061 6769 6e61  list with pagina
-00001050: 7469 6f6e 2061 6e64 2072 6574 7269 6576  tion and retriev
-00001060: 6520 656e 6470 6f69 6e74 732e 5c6e 6060  e endpoints.\n``
-00001070: 6070 7974 686f 6e5c 6e23 2061 7070 2e70  `python\n# app.p
-00001080: 795c 6e5c 6e66 726f 6d20 6661 7374 6170  y\n\nfrom fastap
-00001090: 6920 696d 706f 7274 2046 6173 7441 5049  i import FastAPI
-000010a0: 5c6e 6672 6f6d 2074 6f72 746f 6973 652e  \nfrom tortoise.
-000010b0: 636f 6e74 7269 622e 6661 7374 6170 6920  contrib.fastapi 
-000010c0: 696d 706f 7274 2072 6567 6973 7465 725f  import register_
-000010d0: 746f 7274 6f69 7365 5c6e 6672 6f6d 2074  tortoise\nfrom t
-000010e0: 6f72 746f 6973 652e 7175 6572 7973 6574  ortoise.queryset
-000010f0: 2069 6d70 6f72 7420 5175 6572 7953 6574   import QuerySet
-00001100: 5c6e 5c6e 6672 6f6d 206d 7970 726f 6a65  \n\nfrom myproje
-00001110: 6374 2e6d 6f64 656c 732e 7079 6461 6e74  ct.models.pydant
-00001120: 6963 2069 6d70 6f72 7420 5461 736b 4d6f  ic import TaskMo
-00001130: 6465 6c4f 7574 5c6e 6672 6f6d 206d 7970  delOut\nfrom myp
-00001140: 726f 6a65 6374 2e6d 6f64 656c 732e 746f  roject.models.to
-00001150: 7274 6f69 7365 2069 6d70 6f72 7420 5461  rtoise import Ta
-00001160: 736b 5c6e 6672 6f6d 206d 7970 726f 6a65  sk\nfrom myproje
-00001170: 6374 2e71 7565 7279 7365 7473 2069 6d70  ct.querysets imp
-00001180: 6f72 7420 5461 736b 7352 6f75 7465 7251  ort TasksRouterQ
-00001190: 7565 7279 5365 745c 6e5c 6e5c 6e61 7070  uerySet\n\n\napp
-000011a0: 203d 2046 6173 7441 5049 2829 5c6e 5c6e   = FastAPI()\n\n
-000011b0: 5c6e 7265 6769 7374 6572 5f74 6f72 746f  \nregister_torto
-000011c0: 6973 6528 5c6e 2020 2020 6170 702c 5c6e  ise(\n    app,\n
-000011d0: 2020 2020 6462 5f75 726c 3d22 7371 6c69      db_url="sqli
-000011e0: 7465 3a2f 2f3a 6d65 6d6f 7279 3a22 2c5c  te://:memory:",\
-000011f0: 6e20 2020 206d 6f64 756c 6573 3d7b 226d  n    modules={"m
-00001200: 6f64 656c 7322 3a20 5b22 6d79 7072 6f6a  odels": ["myproj
-00001210: 6563 742e 6d6f 6465 6c73 2e74 6f72 746f  ect.models.torto
-00001220: 6973 6522 5d7d 2c5c 6e20 2020 2067 656e  ise"]},\n    gen
-00001230: 6572 6174 655f 7363 6865 6d61 733d 5472  erate_schemas=Tr
-00001240: 7565 2c5c 6e20 2020 2061 6464 5f65 7863  ue,\n    add_exc
-00001250: 6570 7469 6f6e 5f68 616e 646c 6572 733d  eption_handlers=
-00001260: 5472 7565 2c5c 6e29 5c6e 5c6e 5c6e 4061  True,\n)\n\n\n@a
-00001270: 7070 2e67 6574 2822 7461 736b 732f 222c  pp.get("tasks/",
-00001280: 2072 6573 706f 6e73 655f 6d6f 6465 6c3d   response_model=
-00001290: 6c69 7374 5b54 6173 6b4d 6f64 656c 4f75  list[TaskModelOu
-000012a0: 745d 295c 6e61 7379 6e63 2064 6566 2074  t])\nasync def t
-000012b0: 6173 6b73 5f6c 6973 745f 7061 6769 6e61  asks_list_pagina
-000012c0: 7465 6428 7175 6572 7973 6574 3a20 5175  ted(queryset: Qu
-000012d0: 6572 7953 6574 5b54 6173 6b5d 203d 2054  erySet[Task] = T
-000012e0: 6173 6b73 526f 7574 6572 5175 6572 7953  asksRouterQueryS
-000012f0: 6574 2829 2920 2d3e 206c 6973 745b 5461  et()) -> list[Ta
-00001300: 736b 4d6f 6465 6c4f 7574 5d3a 5c6e 2020  skModelOut]:\n  
-00001310: 2020 7265 7475 726e 2061 7761 6974 2054    return await T
-00001320: 6173 6b4d 6f64 656c 4f75 742e 6672 6f6d  askModelOut.from
-00001330: 5f71 7565 7279 7365 7428 7175 6572 7973  _queryset(querys
-00001340: 6574 295c 6e5c 6e5c 6e40 6170 702e 6765  et)\n\n\n@app.ge
-00001350: 7428 2274 6173 6b73 2f70 6167 696e 6174  t("tasks/paginat
-00001360: 6564 222c 2072 6573 706f 6e73 655f 6d6f  ed", response_mo
-00001370: 6465 6c3d 6c69 7374 5b54 6173 6b4d 6f64  del=list[TaskMod
-00001380: 656c 4f75 745d 295c 6e61 7379 6e63 2064  elOut])\nasync d
-00001390: 6566 2074 6173 6b73 5f6c 6973 745f 7061  ef tasks_list_pa
-000013a0: 6769 6e61 7465 6428 7175 6572 7973 6574  ginated(queryset
-000013b0: 3a20 5175 6572 7953 6574 5b54 6173 6b5d  : QuerySet[Task]
-000013c0: 203d 2054 6173 6b73 526f 7574 6572 5175   = TasksRouterQu
-000013d0: 6572 7953 6574 2829 2e70 6167 696e 6174  erySet().paginat
-000013e0: 6564 2920 2d3e 206c 6973 745b 5461 736b  ed) -> list[Task
-000013f0: 4d6f 6465 6c4f 7574 5d3a 5c6e 2020 2020  ModelOut]:\n    
-00001400: 7265 7475 726e 2061 7761 6974 2054 6173  return await Tas
-00001410: 6b4d 6f64 656c 4f75 742e 6672 6f6d 5f71  kModelOut.from_q
-00001420: 7565 7279 7365 7428 7175 6572 7973 6574  ueryset(queryset
-00001430: 295c 6e5c 6e5c 6e40 6170 702e 6765 7428  )\n\n\n@app.get(
-00001440: 2274 6173 6b73 2f7b 696e 7374 616e 6365  "tasks/{instance
-00001450: 5f69 647d 222c 2072 6573 706f 6e73 655f  _id}", response_
-00001460: 6d6f 6465 6c3d 6c69 7374 5b54 6173 6b4d  model=list[TaskM
-00001470: 6f64 656c 4f75 745d 295c 6e61 7379 6e63  odelOut])\nasync
-00001480: 2064 6566 2074 6173 6b73 5f72 6574 7269   def tasks_retri
-00001490: 6576 6528 7461 736b 3a20 5175 6572 7953  eve(task: QueryS
-000014a0: 6574 5b54 6173 6b5d 203d 2054 6173 6b73  et[Task] = Tasks
-000014b0: 526f 7574 6572 5175 6572 7953 6574 2829  RouterQuerySet()
-000014c0: 2e69 6e73 7461 6e63 6529 202d 3e20 6c69  .instance) -> li
-000014d0: 7374 5b54 6173 6b4d 6f64 656c 4f75 745d  st[TaskModelOut]
-000014e0: 3a5c 6e20 2020 2072 6574 7572 6e20 5461  :\n    return Ta
-000014f0: 736b 4d6f 6465 6c4f 7574 2e66 726f 6d5f  skModelOut.from_
-00001500: 6f72 6d28 7461 736b 295c 6e60 6060 5c6e  orm(task)\n```\n
-00001510: 5c6e 2d2d 2d5c 6e5c 6e23 2320 5265 7175  \n---\n\n## Requ
-00001520: 6573 7473 5c6e 5c6e 2323 2320 4c69 7374  ests\n\n### List
-00001530: 5c6e 5c6e 4f6e 2072 6571 7565 7374 2065  \n\nOn request e
-00001540: 6666 6563 7469 7665 2071 7565 7279 7365  ffective queryse
-00001550: 7420 7769 6c6c 2062 6520 6669 6c74 6572  t will be filter
-00001560: 6564 2061 6e64 206f 7264 6572 6564 2062  ed and ordered b
-00001570: 7920 7175 6572 7920 7061 7261 6d73 2e5c  y query params.\
-00001580: 6e5c 6e46 6f72 2065 7861 6d70 6c65 2c20  n\nFor example, 
-00001590: 7573 6572 2068 6173 2072 6571 7565 7374  user has request
-000015a0: 6564 2065 6e64 706f 696e 7420 7769 7468  ed endpoint with
-000015b0: 2073 6f6d 6520 7175 6572 7920 7061 7261   some query para
-000015c0: 6d73 5c6e 6060 606a 736f 6e5c 6e7b 5c6e  ms\n```json\n{\n
-000015d0: 2020 2020 2263 7265 6174 6564 5f61 745f      "created_at_
-000015e0: 5f6c 7465 223a 2022 3230 3233 2d30 312d  _lte": "2023-01-
-000015f0: 3031 5430 303a 3030 3a30 3022 2c5c 6e20  01T00:00:00",\n 
-00001600: 2020 2022 6170 7072 6f76 6564 223a 2066     "approved": f
-00001610: 616c 7365 2c5c 6e20 2020 2022 6f72 6465  alse,\n    "orde
-00001620: 7269 6e67 5b5d 223a 2022 6372 6561 7465  ring[]": "create
-00001630: 645f 6174 222c 5c6e 7d5c 6e60 6060 5c6e  d_at",\n}\n```\n
-00001640: 5c6e 5265 7175 6573 7420 5552 4c20 6c6f  \nRequest URL lo
-00001650: 6f6b 7320 6c69 6b65 2020 5c6e 6060 6068  oks like  \n```h
-00001660: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00001670: 3830 3030 2f74 6173 6b73 2f3f 6372 6561  8000/tasks/?crea
-00001680: 7465 645f 6174 5f5f 6c74 653d 3230 3233  ted_at__lte=2023
-00001690: 2d30 312d 3031 5430 303a 3030 3a30 3026  -01-01T00:00:00&
-000016a0: 6170 7072 6f76 6564 3d66 616c 7365 266f  approved=false&o
-000016b0: 7264 6572 696e 675b 5d3d 6372 6561 7465  rdering[]=create
-000016c0: 645f 6174 6060 605c 6e5c 6e45 6666 6563  d_at```\n\nEffec
-000016d0: 7469 7665 2071 7565 7279 7365 7420 6174  tive queryset at
-000016e0: 2074 6865 2065 6e64 706f 696e 7420 6d65   the endpoint me
-000016f0: 7468 6f64 2077 696c 6c20 6265 5c6e 6060  thod will be\n``
-00001700: 6070 7974 686f 6e5c 6e28 5c6e 2020 2020  `python\n(\n    
-00001710: 5461 736b 5c6e 2020 2020 2e66 696c 7465  Task\n    .filte
-00001720: 7228 6372 6561 7465 645f 6174 5f5f 6c74  r(created_at__lt
-00001730: 653d 6461 7465 7469 6d65 2e64 6174 6574  e=datetime.datet
-00001740: 696d 6528 3230 3233 2c20 312c 2031 2c20  ime(2023, 1, 1, 
-00001750: 302c 2030 2c20 3029 2c20 6170 7072 6f76  0, 0, 0), approv
-00001760: 6564 3d46 616c 7365 295c 6e20 2020 202e  ed=False)\n    .
-00001770: 6f72 6465 725f 6279 2822 6372 6561 7465  order_by("create
-00001780: 645f 6174 2229 5c6e 295c 6e60 6060 5c6e  d_at")\n)\n```\n
-00001790: 5c6e 2323 2320 4c69 7374 2070 6167 696e  \n### List pagin
-000017a0: 6174 6564 5c6e 5c6e 4c69 6b65 206e 6f74  ated\n\nLike not
-000017b0: 2070 6167 696e 6174 6564 2065 6e64 706f   paginated endpo
-000017c0: 696e 7420 6174 2074 6869 7320 7175 6572  int at this quer
-000017d0: 7973 6574 2077 696c 6c20 6265 2066 696c  yset will be fil
-000017e0: 7465 7265 642c 206f 7264 6572 696e 6720  tered, ordering 
-000017f0: 616e 6420 6164 6469 7469 6f6e 616c 2070  and additional p
-00001800: 6167 696e 6174 6564 2e5c 6e5c 6e46 6f72  aginated.\n\nFor
-00001810: 2065 7861 6d70 6c65 2c20 7573 6572 2068   example, user h
-00001820: 6173 2072 6571 7565 7374 6564 2065 6e64  as requested end
-00001830: 706f 696e 7420 7769 7468 2073 6f6d 6520  point with some 
-00001840: 7175 6572 7920 7061 7261 6d73 5c6e 6060  query params\n``
-00001850: 606a 736f 6e5c 6e7b 5c6e 2020 2020 2270  `json\n{\n    "p
-00001860: 6167 6522 3a20 322c 5c6e 2020 2020 2270  age": 2,\n    "p
-00001870: 6572 5f70 6167 6522 3a20 3130 2c5c 6e20  er_page": 10,\n 
-00001880: 2020 2022 6372 6561 7465 645f 6174 5f5f     "created_at__
-00001890: 6c74 6522 3a20 2232 3032 332d 3031 2d30  lte": "2023-01-0
-000018a0: 3154 3030 3a30 303a 3030 222c 5c6e 2020  1T00:00:00",\n  
-000018b0: 2020 2261 7070 726f 7665 6422 3a20 6661    "approved": fa
-000018c0: 6c73 652c 5c6e 2020 2020 226f 7264 6572  lse,\n    "order
-000018d0: 696e 675b 5d22 3a20 2263 7265 6174 6564  ing[]": "created
-000018e0: 5f61 7422 2c5c 6e7d 5c6e 6060 605c 6e5c  _at",\n}\n```\n\
-000018f0: 6e52 6571 7565 7374 2055 524c 206c 6f6f  nRequest URL loo
-00001900: 6b73 206c 696b 6520 2020 5c6e 6060 6068  ks like   \n```h
-00001910: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00001920: 3830 3030 2f74 6173 6b73 2f3f 7061 6765  8000/tasks/?page
-00001930: 3d32 2670 6572 5f70 6167 653d 3130 2663  =2&per_page=10&c
-00001940: 7265 6174 6564 5f61 745f 5f6c 7465 3d32  reated_at__lte=2
-00001950: 3032 332d 3031 2d30 3154 3030 3a30 303a  023-01-01T00:00:
-00001960: 3030 2661 7070 726f 7665 643d 6661 6c73  00&approved=fals
-00001970: 6526 6f72 6465 7269 6e67 5b5d 3d63 7265  e&ordering[]=cre
-00001980: 6174 6564 5f61 7460 6060 5c6e 5c6e 5c6e  ated_at```\n\n\n
-00001990: 4566 6665 6374 6976 6520 7175 6572 7973  Effective querys
-000019a0: 6574 2061 7420 656e 6470 6f69 6e74 206d  et at endpoint m
-000019b0: 6574 686f 6420 7769 6c6c 2062 655c 6e60  ethod will be\n`
-000019c0: 6060 7079 7468 6f6e 5c6e 285c 6e20 2020  ``python\n(\n   
-000019d0: 2054 6173 6b5c 6e20 2020 202e 6669 6c74   Task\n    .filt
-000019e0: 6572 2863 7265 6174 6564 5f61 745f 5f6c  er(created_at__l
-000019f0: 7465 3d64 6174 6574 696d 652e 6461 7465  te=datetime.date
-00001a00: 7469 6d65 2832 3032 332c 2031 2c20 312c  time(2023, 1, 1,
-00001a10: 2030 2c20 302c 2030 292c 2061 7070 726f   0, 0, 0), appro
-00001a20: 7665 643d 4661 6c73 6529 5c6e 2020 2020  ved=False)\n    
-00001a30: 2e6f 7264 6572 5f62 7928 2263 7265 6174  .order_by("creat
-00001a40: 6564 5f61 7422 295c 6e20 2020 202e 6f66  ed_at")\n    .of
-00001a50: 6673 6574 2831 3029 5c6e 2020 2020 2e6c  fset(10)\n    .l
-00001a60: 696d 6974 2831 3029 5c6e 295c 6e60 6060  imit(10)\n)\n```
-00001a70: 5c6e 5c6e 4173 2077 656c 6c20 6173 2074  \n\nAs well as t
-00001a80: 6f20 6052 6573 706f 6e73 6560 2077 696c  o `Response` wil
-00001a90: 6c20 6265 2061 6464 6564 2070 6167 696e  l be added pagin
-00001aa0: 6174 696f 6e20 696e 666f 726d 6174 696f  ation informatio
-00001ab0: 6e2e 2050 6167 696e 6174 696f 6e20 696e  n. Pagination in
-00001ac0: 666f 726d 6174 696f 6e20 616c 7761 7973  formation always
-00001ad0: 206d 6174 6368 6573 2065 6666 6563 7469   matches effecti
-00001ae0: 7665 2071 7565 7279 7365 745c 6e60 6060  ve queryset\n```
-00001af0: 6a73 6f6e 5c6e 7b5c 6e20 2020 2022 782d  json\n{\n    "x-
-00001b00: 7061 6765 223a 2022 3222 2c5c 6e20 2020  page": "2",\n   
-00001b10: 2022 782d 7061 6765 7322 3a20 2234 222c   "x-pages": "4",
-00001b20: 5c6e 2020 2020 2278 2d70 6572 2d70 6167  \n    "x-per-pag
-00001b30: 6522 3a20 2231 3022 2c5c 6e20 2020 2022  e": "10",\n    "
-00001b40: 782d 746f 7461 6c22 3a20 2233 3222 5c6e  x-total": "32"\n
-00001b50: 7d5c 6e60 6060 5c6e 5c6e 2323 2320 5265  }\n```\n\n### Re
-00001b60: 7472 6965 7665 5c6e 5c6e 5265 7175 6573  trieve\n\nReques
-00001b70: 7420 5552 4c20 6c6f 6f6b 7320 6c69 6b65  t URL looks like
-00001b80: 2020 205c 6e60 6060 6874 7470 3a2f 2f6c     \n```http://l
-00001b90: 6f63 616c 686f 7374 3a38 3030 302f 7461  ocalhost:8000/ta
-00001ba0: 736b 732f 3130 2f60 6060 5c6e 5c6e 456e  sks/10/```\n\nEn
-00001bb0: 6470 6f69 6e74 206d 6574 686f 6420 7769  dpoint method wi
-00001bc0: 6c6c 2067 6574 2060 5461 736b 6020 7769  ll get `Task` wi
-00001bd0: 7468 2060 6964 203d 3d20 3130 6020 6173  th `id == 10` as
-00001be0: 2061 7267 756d 656e 7420 6074 6173 6b60   argument `task`
-00001bf0: 2e20 2020 2020 5c6e 4966 2060 5461 736b  .     \nIf `Task
-00001c00: 6020 7769 7468 2060 6964 203d 3d20 3130  ` with `id == 10
-00001c10: 6020 646f 6573 206e 6f74 2065 7869 7374  ` does not exist
-00001c20: 2074 6865 6e20 656e 6470 6f69 6e74 2072   then endpoint r
-00001c30: 6574 7572 6e20 6052 6573 706f 6e73 6528  eturn `Response(
-00001c40: 3430 3429 6020 2027 2c0a 2020 2020 2761  404)`  ',.    'a
-00001c50: 7574 686f 7227 3a20 274e 696b 616b 746f  uthor': 'Nikakto
-00001c60: 272c 0a20 2020 2027 6175 7468 6f72 5f65  ',.    'author_e
-00001c70: 6d61 696c 273a 2027 626c 6163 6b2d 7a40  mail': 'black-z@
-00001c80: 626b 2e72 7527 2c0a 2020 2020 276d 6169  bk.ru',.    'mai
-00001c90: 6e74 6169 6e65 7227 3a20 274e 6f6e 6527  ntainer': 'None'
-00001ca0: 2c0a 2020 2020 276d 6169 6e74 6169 6e65  ,.    'maintaine
-00001cb0: 725f 656d 6169 6c27 3a20 274e 6f6e 6527  r_email': 'None'
-00001cc0: 2c0a 2020 2020 2775 726c 273a 2027 6874  ,.    'url': 'ht
-00001cd0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001ce0: 2f4e 696b 616b 746f 2f66 6173 7461 7069  /Nikakto/fastapi
-00001cf0: 2d71 7565 7279 7365 7473 272c 0a20 2020  -querysets',.   
-00001d00: 2027 7061 636b 6167 6573 273a 2070 6163   'packages': pac
-00001d10: 6b61 6765 732c 0a20 2020 2027 7061 636b  kages,.    'pack
-00001d20: 6167 655f 6461 7461 273a 2070 6163 6b61  age_data': packa
-00001d30: 6765 5f64 6174 612c 0a20 2020 2027 696e  ge_data,.    'in
-00001d40: 7374 616c 6c5f 7265 7175 6972 6573 273a  stall_requires':
-00001d50: 2069 6e73 7461 6c6c 5f72 6571 7569 7265   install_require
-00001d60: 732c 0a20 2020 2027 7079 7468 6f6e 5f72  s,.    'python_r
-00001d70: 6571 7569 7265 7327 3a20 273e 3d33 2e38  equires': '>=3.8
-00001d80: 2c3c 342e 3027 2c0a 7d0a 0a0a 7365 7475  ,<4.0',.}...setu
-00001d90: 7028 2a2a 7365 7475 705f 6b77 6172 6773  p(**setup_kwargs
-00001da0: 290a                                     ).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
+00000020: 6170 692d 7175 6572 7973 6574 730a 5665  api-querysets.Ve
+00000030: 7273 696f 6e3a 2030 2e31 2e32 0a53 756d  rsion: 0.1.2.Sum
+00000040: 6d61 7279 3a20 0a48 6f6d 652d 7061 6765  mary: .Home-page
+00000050: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000060: 2e63 6f6d 2f4e 696b 616b 746f 2f66 6173  .com/Nikakto/fas
+00000070: 7461 7069 2d71 7565 7279 7365 7473 0a4c  tapi-querysets.L
+00000080: 6963 656e 7365 3a20 4d49 540a 4b65 7977  icense: MIT.Keyw
+00000090: 6f72 6473 3a20 6661 7374 6170 692c 6669  ords: fastapi,fi
+000000a0: 6c74 6572 732c 6669 6c74 6572 696e 672c  lters,filtering,
+000000b0: 7061 6769 6e61 7469 6f6e 2c6f 7264 6572  pagination,order
+000000c0: 2c6f 7264 6572 696e 672c 7175 6572 7973  ,ordering,querys
+000000d0: 6574 2c54 6f72 746f 6973 652c 6f72 6d2c  et,Tortoise,orm,
+000000e0: 6461 7461 6261 7365 2c64 620a 4175 7468  database,db.Auth
+000000f0: 6f72 3a20 4e69 6b61 6b74 6f0a 4175 7468  or: Nikakto.Auth
+00000100: 6f72 2d65 6d61 696c 3a20 626c 6163 6b2d  or-email: black-
+00000110: 7a40 626b 2e72 750a 5265 7175 6972 6573  z@bk.ru.Requires
+00000120: 2d50 7974 686f 6e3a 203e 3d33 2e38 2c3c  -Python: >=3.8,<
+00000130: 342e 300a 436c 6173 7369 6669 6572 3a20  4.0.Classifier: 
+00000140: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000150: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000160: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
+00000170: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000190: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
+000001a0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000001b0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001c0: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
+000001d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001f0: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
+00000200: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000210: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000220: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
+00000230: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000240: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000250: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+00000260: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000270: 6661 7374 6170 6920 283e 3d30 2e37 3829  fastapi (>=0.78)
+00000280: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000290: 6661 7374 6170 692d 6465 7065 6e64 732d  fastapi-depends-
+000002a0: 6578 7420 283e 3d30 2e32 2e32 290a 5265  ext (>=0.2.2).Re
+000002b0: 7175 6972 6573 2d44 6973 743a 2074 6f72  quires-Dist: tor
+000002c0: 746f 6973 652d 6f72 6d20 283e 3d30 2e31  toise-orm (>=0.1
+000002d0: 382e 3129 0a50 726f 6a65 6374 2d55 524c  8.1).Project-URL
+000002e0: 3a20 446f 6375 6d65 6e74 6174 696f 6e2c  : Documentation,
+000002f0: 2068 7474 7073 3a2f 2f66 6173 7461 7069   https://fastapi
+00000300: 2d71 7565 7279 7365 7473 2e72 6561 6474  -querysets.readt
+00000310: 6865 646f 6373 2e69 6f0a 5072 6f6a 6563  hedocs.io.Projec
+00000320: 742d 5552 4c3a 2052 6570 6f73 6974 6f72  t-URL: Repositor
+00000330: 792c 2068 7474 7073 3a2f 2f67 6974 6875  y, https://githu
+00000340: 622e 636f 6d2f 4e69 6b61 6b74 6f2f 6661  b.com/Nikakto/fa
+00000350: 7374 6170 692d 7175 6572 7973 6574 730a  stapi-querysets.
+00000360: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00000370: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00000380: 6172 6b64 6f77 6e0a 0a23 2046 6173 7441  arkdown..# FastA
+00000390: 5049 2051 7565 7279 7365 7473 0a21 5b43  PI Querysets.![C
+000003a0: 444e 4a53 5d28 6874 7470 733a 2f2f 696d  DNJS](https://im
+000003b0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000003c0: 6765 2f50 7974 686f 6e2d 332e 3825 3230  ge/Python-3.8%20
+000003d0: 2537 4325 3230 332e 3925 3230 2537 4325  %7C%203.9%20%7C%
+000003e0: 3230 332e 3130 2532 3025 3743 2532 3033  203.10%20%7C%203
+000003f0: 2e31 312d 3233 3334 4430 3538 290a 215b  .11-2334D058).![
+00000400: 4344 4e4a 535d 2868 7474 7073 3a2f 2f73  CDNJS](https://s
+00000410: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000420: 4661 7374 4150 492d 2533 453d 302e 372e  FastAPI-%3E=0.7.
+00000430: 302d 3030 3934 3835 290a 0a2d 2d2d 0a2a  0-009485)..---.*
+00000440: 2a44 6f63 756d 656e 7461 7469 6f6e 2a2a  *Documentation**
+00000450: 3a20 3c61 2068 7265 663d 2268 7474 7073  : <a href="https
+00000460: 3a2f 2f66 6173 7461 7069 2d71 7565 7279  ://fastapi-query
+00000470: 7365 7473 2e72 6561 6474 6865 646f 6373  sets.readthedocs
+00000480: 2e69 6f22 2074 6172 6765 743d 225f 626c  .io" target="_bl
+00000490: 616e 6b22 3e68 7474 7073 3a2f 2f66 6173  ank">https://fas
+000004a0: 7461 7069 2d71 7565 7279 7365 7473 2e72  tapi-querysets.r
+000004b0: 6561 6474 6865 646f 6373 2e69 6f3c 2f61  eadthedocs.io</a
+000004c0: 3e0a 0a2a 2a53 6f75 7263 6520 436f 6465  >..**Source Code
+000004d0: 2a2a 3a20 3c61 2068 7265 663d 2268 7474  **: <a href="htt
+000004e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000004f0: 4e69 6b61 6b74 6f2f 6661 7374 6170 692d  Nikakto/fastapi-
+00000500: 7175 6572 7973 6574 7322 2074 6172 6765  querysets" targe
+00000510: 743d 225f 626c 616e 6b22 3e68 7474 7073  t="_blank">https
+00000520: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e69  ://github.com/Ni
+00000530: 6b61 6b74 6f2f 6661 7374 6170 692d 7175  kakto/fastapi-qu
+00000540: 6572 7973 6574 733c 2f61 3e0a 0a2d 2d2d  erysets</a>..---
+00000550: 0a0a 2323 2057 6879 2074 6f20 7573 653f  ..## Why to use?
+00000560: 0a0a 5768 696c 6520 796f 7520 6172 6520  ..While you are 
+00000570: 6465 7665 6c6f 7069 6e67 2046 6173 7441  developing FastA
+00000580: 5049 2061 7070 6c69 6361 7469 6f6e 7320  PI applications 
+00000590: 796f 7520 6172 6520 7573 696e 6720 6461  you are using da
+000005a0: 7461 6261 7365 7320 7769 7468 204f 524d  tabases with ORM
+000005b0: 2e20 4d6f 7374 206f 6620 7468 6520 656e  . Most of the en
+000005c0: 6470 6f69 6e74 7320 6172 6520 7669 6577  dpoints are view
+000005d0: 206f 6620 6461 7461 6261 7365 2074 6162   of database tab
+000005e0: 6c65 7320 616e 6420 7265 7175 6972 6520  les and require 
+000005f0: 7265 7374 7269 6374 2071 7565 7279 7365  restrict queryse
+00000600: 7420 6279 2066 696c 7465 7269 6e67 2c20  t by filtering, 
+00000610: 7061 6769 6e61 7469 6f6e 2c20 6f72 6465  pagination, orde
+00000620: 7269 6e67 2e20 5468 6973 2070 726f 6a65  ring. This proje
+00000630: 6374 2069 7320 6765 6e65 7269 6320 616e  ct is generic an
+00000640: 6420 7265 7573 6162 6c65 2077 6179 2074  d reusable way t
+00000650: 6f20 6372 6561 7465 2072 6573 7472 6963  o create restric
+00000660: 7465 6420 7175 6572 7973 6574 7320 666f  ted querysets fo
+00000670: 7220 796f 7572 2065 6e64 706f 696e 7473  r your endpoints
+00000680: 2e0a 0a23 2320 5375 7070 6f72 7465 6420  ...## Supported 
+00000690: 4f52 4d0a 2d20 3c61 2068 7265 663d 2268  ORM.- <a href="h
+000006a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006b0: 6d2f 746f 7274 6f69 7365 2f74 6f72 746f  m/tortoise/torto
+000006c0: 6973 652d 6f72 6d22 2074 6172 6765 743d  ise-orm" target=
+000006d0: 225f 626c 616e 6b22 3e54 6f72 746f 6973  "_blank">Tortois
+000006e0: 6520 4f52 4d3c 2f61 3e0a 0a23 2320 5265  e ORM</a>..## Re
+000006f0: 7175 6972 656d 656e 7473 0a2d 2070 7974  quirements.- pyt
+00000700: 686f 6e20 3e3d 332e 382c 3c34 2e30 0a2d  hon >=3.8,<4.0.-
+00000710: 2066 6173 7441 5049 203e 3d20 302e 372e   fastAPI >= 0.7.
+00000720: 300a 2d20 746f 7274 6f69 7365 2d6f 726d  0.- tortoise-orm
+00000730: 203e 3d20 302e 3138 2e31 0a0a 2323 2049   >= 0.18.1..## I
+00000740: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
+00000750: 0a70 6970 2069 6e73 7461 6c6c 2066 6173  .pip install fas
+00000760: 7461 7069 2d71 7565 7279 7365 7473 0a60  tapi-querysets.`
+00000770: 6060 0a0a 2320 5175 6963 6b20 7475 746f  ``..# Quick tuto
+00000780: 7269 616c 0a0a 2d2d 2d0a 0a2d 2d2d 0a0a  rial..---..---..
+00000790: 2323 2054 6f72 746f 6973 6520 6d6f 6465  ## Tortoise mode
+000007a0: 6c0a 0a4c 6574 e280 9973 2073 7461 7274  l..Let...s start
+000007b0: 2077 6974 6820 6f75 7220 6d6f 6465 6c0a   with our model.
+000007c0: 0a60 6060 7079 7468 6f6e 0a23 206d 6f64  .```python.# mod
+000007d0: 656c 732f 746f 7274 6f69 7365 2e70 790a  els/tortoise.py.
+000007e0: 0a69 6d70 6f72 7420 6461 7465 7469 6d65  .import datetime
+000007f0: 0a66 726f 6d20 7479 7069 6e67 2069 6d70  .from typing imp
+00000800: 6f72 7420 4f70 7469 6f6e 616c 0a0a 6672  ort Optional..fr
+00000810: 6f6d 2074 6f72 746f 6973 6520 696d 706f  om tortoise impo
+00000820: 7274 204d 6f64 656c 0a66 726f 6d20 746f  rt Model.from to
+00000830: 7274 6f69 7365 2069 6d70 6f72 7420 6669  rtoise import fi
+00000840: 656c 6473 0a0a 0a63 6c61 7373 2054 6173  elds...class Tas
+00000850: 6b28 4d6f 6465 6c29 3a0a 2020 2020 6964  k(Model):.    id
+00000860: 3a20 696e 7420 3d20 6669 656c 6473 2e49  : int = fields.I
+00000870: 6e74 4669 656c 6428 706b 3d54 7275 6529  ntField(pk=True)
+00000880: 0a20 2020 2061 7070 726f 7665 643a 204f  .    approved: O
+00000890: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
+000008a0: 6669 656c 6473 2e42 6f6f 6c65 616e 4669  fields.BooleanFi
+000008b0: 656c 6428 6465 6661 756c 743d 4661 6c73  eld(default=Fals
+000008c0: 652c 206e 756c 6c3d 5472 7565 290a 2020  e, null=True).  
+000008d0: 2020 636f 6465 3a20 7374 7220 3d20 6669    code: str = fi
+000008e0: 656c 6473 2e43 6861 7246 6965 6c64 286d  elds.CharField(m
+000008f0: 6178 5f6c 656e 6774 683d 3629 0a20 2020  ax_length=6).   
+00000900: 2063 7265 6174 6564 5f61 743a 2064 6174   created_at: dat
+00000910: 6574 696d 652e 6461 7465 7469 6d65 203d  etime.datetime =
+00000920: 2066 6965 6c64 732e 4461 7465 7469 6d65   fields.Datetime
+00000930: 4669 656c 6428 6465 6661 756c 743d 6461  Field(default=da
+00000940: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00000950: 6e6f 7729 0a60 6060 0a2d 2d2d 0a0a 2323  now).```.---..##
+00000960: 2050 7964 616e 7469 6320 6d6f 6465 6c0a   Pydantic model.
+00000970: 0a43 7265 6174 6520 6461 7461 6261 7365  .Create database
+00000980: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+00000990: 6d6f 6465 6c0a 0a60 6060 7079 7468 6f6e  model..```python
+000009a0: 0a23 206d 6f64 656c 732f 7079 6461 6e74  .# models/pydant
+000009b0: 6963 2e70 790a 0a66 726f 6d20 746f 7274  ic.py..from tort
+000009c0: 6f69 7365 2e63 6f6e 7472 6962 2e70 7964  oise.contrib.pyd
+000009d0: 616e 7469 6320 696d 706f 7274 2070 7964  antic import pyd
+000009e0: 616e 7469 635f 6d6f 6465 6c5f 6372 6561  antic_model_crea
+000009f0: 746f 720a 0a66 726f 6d20 6d79 7072 6f6a  tor..from myproj
+00000a00: 6563 742e 6d6f 6465 6c73 2e74 6f72 746f  ect.models.torto
+00000a10: 6973 6520 696d 706f 7274 2054 6173 6b0a  ise import Task.
+00000a20: 0a0a 5461 736b 4d6f 6465 6c4f 7574 203d  ..TaskModelOut =
+00000a30: 2070 7964 616e 7469 635f 6d6f 6465 6c5f   pydantic_model_
+00000a40: 6372 6561 746f 7228 0a20 2020 2054 6173  creator(.    Tas
+00000a50: 6b2c 0a20 2020 206e 616d 653d 2254 6173  k,.    name="Tas
+00000a60: 6b4d 6f64 656c 4f75 7422 2c0a 2020 2020  kModelOut",.    
+00000a70: 696e 636c 7564 653d 280a 2020 2020 2020  include=(.      
+00000a80: 2020 2269 6422 2c0a 2020 2020 2020 2020    "id",.        
+00000a90: 2261 7070 726f 7665 6422 2c0a 2020 2020  "approved",.    
+00000aa0: 2020 2020 2263 6f64 6522 2c0a 2020 2020      "code",.    
+00000ab0: 2020 2020 2263 7265 6174 6564 5f61 7422      "created_at"
+00000ac0: 0a20 2020 2029 2c0a 290a 6060 600a 0a2d  .    ),.).```..-
+00000ad0: 2d2d 0a0a 2323 2052 6f75 7465 7251 7565  --..## RouterQue
+00000ae0: 7279 5365 740a 0a23 2323 2046 696c 7465  rySet..### Filte
+00000af0: 7273 0a0a 5765 2068 6176 6520 6120 6e75  rs..We have a nu
+00000b00: 6d62 6572 206f 6620 6669 656c 6473 2077  mber of fields w
+00000b10: 6520 7761 6e74 2074 6f20 6c65 7420 6f75  e want to let ou
+00000b20: 7220 7573 6572 7320 6669 6c74 6572 2062  r users filter b
+00000b30: 6173 6564 206f 6e20 7468 656d 2e20 5765  ased on them. We
+00000b40: 2063 7265 6174 6520 6120 526f 7574 6572   create a Router
+00000b50: 5175 6572 7953 6574 4669 6c74 6572 2066  QuerySetFilter f
+00000b60: 6f72 2074 6869 732e 2046 696c 7465 7220  or this. Filter 
+00000b70: 636c 6173 7320 6973 2061 7267 756d 656e  class is argumen
+00000b80: 7420 666f 7220 6046 6173 7441 5049 2e44  t for `FastAPI.D
+00000b90: 6570 656e 6473 6020 6174 2065 6e64 706f  epends` at endpo
+00000ba0: 696e 742e 2020 0a0a 596f 7520 7265 7175  int.  ..You requ
+00000bb0: 6972 6520 746f 2064 6566 696e 6520 4f52  ire to define OR
+00000bc0: 4d20 6669 6c74 6572 206b 6579 776f 7264  M filter keyword
+00000bd0: 2c20 7479 7065 206f 6620 6461 7461 2061  , type of data a
+00000be0: 6e64 2073 6574 7570 2073 6f75 7263 6520  nd setup source 
+00000bf0: 6f66 2064 6174 6120 2860 5175 6572 7960  of data (`Query`
+00000c00: 2c20 6050 6174 6860 2c20 6042 6f64 7960  , `Path`, `Body`
+00000c10: 2c20 6574 6329 2e0a 0a60 6060 7079 7468  , etc)...```pyth
+00000c20: 6f6e 0a23 2071 7565 7279 7365 7473 5f66  on.# querysets_f
+00000c30: 696c 7465 7273 2e70 790a 0a69 6d70 6f72  ilters.py..impor
+00000c40: 7420 6461 7461 636c 6173 7365 730a 696d  t dataclasses.im
+00000c50: 706f 7274 2064 6174 6574 696d 650a 6672  port datetime.fr
+00000c60: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00000c70: 204f 7074 696f 6e61 6c0a 0a66 726f 6d20   Optional..from 
+00000c80: 6661 7374 6170 6920 696d 706f 7274 2051  fastapi import Q
+00000c90: 7565 7279 0a0a 0a40 6461 7461 636c 6173  uery...@dataclas
+00000ca0: 7365 732e 6461 7461 636c 6173 730a 636c  ses.dataclass.cl
+00000cb0: 6173 7320 526f 7574 6572 5175 6572 7953  ass RouterQueryS
+00000cc0: 6574 4669 6c74 6572 3a0a 2020 2020 6964  etFilter:.    id
+00000cd0: 5f5f 696e 3a20 4f70 7469 6f6e 616c 5b6c  __in: Optional[l
+00000ce0: 6973 745b 696e 745d 5d20 3d20 5175 6572  ist[int]] = Quer
+00000cf0: 7928 4e6f 6e65 2c20 616c 6961 733d 2769  y(None, alias='i
+00000d00: 645b 5d27 290a 2020 2020 6170 7072 6f76  d[]').    approv
+00000d10: 6564 3a20 4f70 7469 6f6e 616c 5b62 6f6f  ed: Optional[boo
+00000d20: 6c5d 203d 2051 7565 7279 284e 6f6e 6529  l] = Query(None)
+00000d30: 0a20 2020 2061 7070 726f 7665 645f 5f69  .    approved__i
+00000d40: 736e 756c 6c3a 204f 7074 696f 6e61 6c5b  snull: Optional[
+00000d50: 626f 6f6c 5d20 3d20 5175 6572 7928 4e6f  bool] = Query(No
+00000d60: 6e65 290a 2020 2020 636f 6465 3a20 4f70  ne).    code: Op
+00000d70: 7469 6f6e 616c 5b73 7472 5d20 3d20 5175  tional[str] = Qu
+00000d80: 6572 7928 4e6f 6e65 290a 2020 2020 6372  ery(None).    cr
+00000d90: 6561 7465 645f 6174 5f5f 6c74 653a 204f  eated_at__lte: O
+00000da0: 7074 696f 6e61 6c5b 6461 7465 7469 6d65  ptional[datetime
+00000db0: 2e64 6174 6574 696d 655d 203d 2051 7565  .datetime] = Que
+00000dc0: 7279 284e 6f6e 6529 0a20 2020 2063 7265  ry(None).    cre
+00000dd0: 6174 6564 5f61 745f 5f67 7465 3a20 4f70  ated_at__gte: Op
+00000de0: 7469 6f6e 616c 5b64 6174 6574 696d 652e  tional[datetime.
+00000df0: 6461 7465 7469 6d65 5d20 3d20 5175 6572  datetime] = Quer
+00000e00: 7928 4e6f 6e65 290a 6060 600a 0a23 2323  y(None).```..###
+00000e10: 204d 6f64 656c 2051 7565 7279 7365 740a   Model Queryset.
+00000e20: 0a43 6f6e 6669 6775 7265 2060 526f 7574  .Configure `Rout
+00000e30: 6572 5175 6572 7973 6574 6020 7072 6f70  erQueryset` prop
+00000e40: 6572 7469 6573 0a0a 6060 6070 7974 686f  erties..```pytho
+00000e50: 6e0a 2320 7175 6572 7973 6574 732e 7079  n.# querysets.py
+00000e60: 0a0a 6672 6f6d 2066 6173 7461 7069 5f71  ..from fastapi_q
+00000e70: 7565 7279 7365 7473 2e6d 6978 696e 732e  uerysets.mixins.
+00000e80: 6669 6c74 6572 7320 696d 706f 7274 2046  filters import F
+00000e90: 696c 7465 724d 6978 696e 0a66 726f 6d20  ilterMixin.from 
+00000ea0: 6661 7374 6170 695f 7175 6572 7973 6574  fastapi_queryset
+00000eb0: 732e 6d69 7869 6e73 2e66 696c 7465 7273  s.mixins.filters
+00000ec0: 2069 6d70 6f72 7420 4669 6c74 6572 4e65   import FilterNe
+00000ed0: 6761 7469 6f6e 4d69 7869 6e0a 6672 6f6d  gationMixin.from
+00000ee0: 2066 6173 7461 7069 5f71 7565 7279 7365   fastapi_queryse
+00000ef0: 7473 2e6d 6978 696e 732e 6f72 6465 7269  ts.mixins.orderi
+00000f00: 6e67 2069 6d70 6f72 7420 4f72 6465 7269  ng import Orderi
+00000f10: 6e67 4d69 7869 6e0a 6672 6f6d 2066 6173  ngMixin.from fas
+00000f20: 7461 7069 5f71 7565 7279 7365 7473 2e6d  tapi_querysets.m
+00000f30: 6978 696e 732e 7061 6769 6e61 7469 6f6e  ixins.pagination
+00000f40: 2069 6d70 6f72 7420 5061 6769 6e61 7469   import Paginati
+00000f50: 6f6e 4d69 7869 6e0a 6672 6f6d 2066 6173  onMixin.from fas
+00000f60: 7461 7069 5f71 7565 7279 7365 7473 2e6d  tapi_querysets.m
+00000f70: 6978 696e 732e 7061 6769 6e61 7469 6f6e  ixins.pagination
+00000f80: 2069 6d70 6f72 7420 526f 7574 6572 5061   import RouterPa
+00000f90: 6769 6e61 7469 6f6e 0a66 726f 6d20 6661  gination.from fa
+00000fa0: 7374 6170 695f 7175 6572 7973 6574 732e  stapi_querysets.
+00000fb0: 7175 6572 7973 6574 2069 6d70 6f72 7420  queryset import 
+00000fc0: 526f 7574 6572 5175 6572 7953 6574 0a0a  RouterQuerySet..
+00000fd0: 6672 6f6d 206d 7970 726f 6a65 6374 2e6d  from myproject.m
+00000fe0: 6f64 656c 732e 746f 7274 6f69 7365 2069  odels.tortoise i
+00000ff0: 6d70 6f72 7420 5461 736b 0a66 726f 6d20  mport Task.from 
+00001000: 6d79 7072 6f6a 6563 742e 7175 6572 7973  myproject.querys
+00001010: 6574 735f 6669 6c74 6572 7320 696d 706f  ets_filters impo
+00001020: 7274 2052 6f75 7465 7251 7565 7279 5365  rt RouterQuerySe
+00001030: 7446 696c 7465 720a 0a0a 636c 6173 7320  tFilter...class 
+00001040: 5461 736b 7352 6f75 7465 7251 7565 7279  TasksRouterQuery
+00001050: 5365 7428 4669 6c74 6572 4d69 7869 6e2c  Set(FilterMixin,
+00001060: 2046 696c 7465 724e 6567 6174 696f 6e4d   FilterNegationM
+00001070: 6978 696e 2c20 4f72 6465 7269 6e67 4d69  ixin, OrderingMi
+00001080: 7869 6e2c 2050 6167 696e 6174 696f 6e4d  xin, PaginationM
+00001090: 6978 696e 2c20 526f 7574 6572 5175 6572  ixin, RouterQuer
+000010a0: 7953 6574 293a 0a20 2020 2066 696c 7465  ySet):.    filte
+000010b0: 725f 636c 6173 7320 3d20 526f 7574 6572  r_class = Router
+000010c0: 5175 6572 7953 6574 4669 6c74 6572 0a20  QuerySetFilter. 
+000010d0: 2020 206f 7264 6572 696e 675f 6465 6661     ordering_defa
+000010e0: 756c 7420 3d20 2269 6422 0a20 2020 206f  ult = "id".    o
+000010f0: 7264 6572 696e 675f 6669 656c 6473 203d  rdering_fields =
+00001100: 2028 0a20 2020 2020 2020 2022 6964 222c   (.        "id",
+00001110: 0a20 2020 2020 2020 2022 6170 7072 6f76  .        "approv
+00001120: 6564 222c 0a20 2020 2020 2020 2022 636f  ed",.        "co
+00001130: 6465 222c 0a20 2020 2020 2020 2022 6372  de",.        "cr
+00001140: 6561 7465 645f 6174 222c 0a20 2020 2029  eated_at",.    )
+00001150: 0a20 2020 2070 6167 696e 6174 696f 6e5f  .    pagination_
+00001160: 636c 6173 7320 3d20 526f 7574 6572 5061  class = RouterPa
+00001170: 6769 6e61 7469 6f6e 0a20 2020 206d 6f64  gination.    mod
+00001180: 656c 203d 2054 6173 6b0a 6060 600a 0a2d  el = Task.```..-
+00001190: 2d2d 0a0a 2323 2041 7070 6c69 6361 7469  --..## Applicati
+000011a0: 6f6e 0a0a 4372 6561 7465 2061 7070 6c69  on..Create appli
+000011b0: 6361 7469 6f6e 2c20 7265 6769 7374 6572  cation, register
+000011c0: 206c 6973 742c 206c 6973 7420 7769 7468   list, list with
+000011d0: 2070 6167 696e 6174 696f 6e20 616e 6420   pagination and 
+000011e0: 7265 7472 6965 7665 2065 6e64 706f 696e  retrieve endpoin
+000011f0: 7473 2e0a 6060 6070 7974 686f 6e0a 2320  ts..```python.# 
+00001200: 6170 702e 7079 0a0a 6672 6f6d 2066 6173  app.py..from fas
+00001210: 7461 7069 2069 6d70 6f72 7420 4661 7374  tapi import Fast
+00001220: 4150 490a 6672 6f6d 2074 6f72 746f 6973  API.from tortois
+00001230: 652e 636f 6e74 7269 622e 6661 7374 6170  e.contrib.fastap
+00001240: 6920 696d 706f 7274 2072 6567 6973 7465  i import registe
+00001250: 725f 746f 7274 6f69 7365 0a66 726f 6d20  r_tortoise.from 
+00001260: 746f 7274 6f69 7365 2e71 7565 7279 7365  tortoise.queryse
+00001270: 7420 696d 706f 7274 2051 7565 7279 5365  t import QuerySe
+00001280: 740a 0a66 726f 6d20 6d79 7072 6f6a 6563  t..from myprojec
+00001290: 742e 6d6f 6465 6c73 2e70 7964 616e 7469  t.models.pydanti
+000012a0: 6320 696d 706f 7274 2054 6173 6b4d 6f64  c import TaskMod
+000012b0: 656c 4f75 740a 6672 6f6d 206d 7970 726f  elOut.from mypro
+000012c0: 6a65 6374 2e6d 6f64 656c 732e 746f 7274  ject.models.tort
+000012d0: 6f69 7365 2069 6d70 6f72 7420 5461 736b  oise import Task
+000012e0: 0a66 726f 6d20 6d79 7072 6f6a 6563 742e  .from myproject.
+000012f0: 7175 6572 7973 6574 7320 696d 706f 7274  querysets import
+00001300: 2054 6173 6b73 526f 7574 6572 5175 6572   TasksRouterQuer
+00001310: 7953 6574 0a0a 0a61 7070 203d 2046 6173  ySet...app = Fas
+00001320: 7441 5049 2829 0a0a 0a72 6567 6973 7465  tAPI()...registe
+00001330: 725f 746f 7274 6f69 7365 280a 2020 2020  r_tortoise(.    
+00001340: 6170 702c 0a20 2020 2064 625f 7572 6c3d  app,.    db_url=
+00001350: 2273 716c 6974 653a 2f2f 3a6d 656d 6f72  "sqlite://:memor
+00001360: 793a 222c 0a20 2020 206d 6f64 756c 6573  y:",.    modules
+00001370: 3d7b 226d 6f64 656c 7322 3a20 5b22 6d79  ={"models": ["my
+00001380: 7072 6f6a 6563 742e 6d6f 6465 6c73 2e74  project.models.t
+00001390: 6f72 746f 6973 6522 5d7d 2c0a 2020 2020  ortoise"]},.    
+000013a0: 6765 6e65 7261 7465 5f73 6368 656d 6173  generate_schemas
+000013b0: 3d54 7275 652c 0a20 2020 2061 6464 5f65  =True,.    add_e
+000013c0: 7863 6570 7469 6f6e 5f68 616e 646c 6572  xception_handler
+000013d0: 733d 5472 7565 2c0a 290a 0a0a 4061 7070  s=True,.)...@app
+000013e0: 2e67 6574 2822 7461 736b 732f 222c 2072  .get("tasks/", r
+000013f0: 6573 706f 6e73 655f 6d6f 6465 6c3d 6c69  esponse_model=li
+00001400: 7374 5b54 6173 6b4d 6f64 656c 4f75 745d  st[TaskModelOut]
+00001410: 290a 6173 796e 6320 6465 6620 7461 736b  ).async def task
+00001420: 735f 6c69 7374 5f70 6167 696e 6174 6564  s_list_paginated
+00001430: 2871 7565 7279 7365 743a 2051 7565 7279  (queryset: Query
+00001440: 5365 745b 5461 736b 5d20 3d20 5461 736b  Set[Task] = Task
+00001450: 7352 6f75 7465 7251 7565 7279 5365 7428  sRouterQuerySet(
+00001460: 2929 202d 3e20 6c69 7374 5b54 6173 6b4d  )) -> list[TaskM
+00001470: 6f64 656c 4f75 745d 3a0a 2020 2020 7265  odelOut]:.    re
+00001480: 7475 726e 2061 7761 6974 2054 6173 6b4d  turn await TaskM
+00001490: 6f64 656c 4f75 742e 6672 6f6d 5f71 7565  odelOut.from_que
+000014a0: 7279 7365 7428 7175 6572 7973 6574 290a  ryset(queryset).
+000014b0: 0a0a 4061 7070 2e67 6574 2822 7461 736b  ..@app.get("task
+000014c0: 732f 7061 6769 6e61 7465 6422 2c20 7265  s/paginated", re
+000014d0: 7370 6f6e 7365 5f6d 6f64 656c 3d6c 6973  sponse_model=lis
+000014e0: 745b 5461 736b 4d6f 6465 6c4f 7574 5d29  t[TaskModelOut])
+000014f0: 0a61 7379 6e63 2064 6566 2074 6173 6b73  .async def tasks
+00001500: 5f6c 6973 745f 7061 6769 6e61 7465 6428  _list_paginated(
+00001510: 7175 6572 7973 6574 3a20 5175 6572 7953  queryset: QueryS
+00001520: 6574 5b54 6173 6b5d 203d 2054 6173 6b73  et[Task] = Tasks
+00001530: 526f 7574 6572 5175 6572 7953 6574 2829  RouterQuerySet()
+00001540: 2e70 6167 696e 6174 6564 2920 2d3e 206c  .paginated) -> l
+00001550: 6973 745b 5461 736b 4d6f 6465 6c4f 7574  ist[TaskModelOut
+00001560: 5d3a 0a20 2020 2072 6574 7572 6e20 6177  ]:.    return aw
+00001570: 6169 7420 5461 736b 4d6f 6465 6c4f 7574  ait TaskModelOut
+00001580: 2e66 726f 6d5f 7175 6572 7973 6574 2871  .from_queryset(q
+00001590: 7565 7279 7365 7429 0a0a 0a40 6170 702e  ueryset)...@app.
+000015a0: 6765 7428 2274 6173 6b73 2f7b 696e 7374  get("tasks/{inst
+000015b0: 616e 6365 5f69 647d 222c 2072 6573 706f  ance_id}", respo
+000015c0: 6e73 655f 6d6f 6465 6c3d 6c69 7374 5b54  nse_model=list[T
+000015d0: 6173 6b4d 6f64 656c 4f75 745d 290a 6173  askModelOut]).as
+000015e0: 796e 6320 6465 6620 7461 736b 735f 7265  ync def tasks_re
+000015f0: 7472 6965 7665 2874 6173 6b3a 2051 7565  trieve(task: Que
+00001600: 7279 5365 745b 5461 736b 5d20 3d20 5461  rySet[Task] = Ta
+00001610: 736b 7352 6f75 7465 7251 7565 7279 5365  sksRouterQuerySe
+00001620: 7428 292e 696e 7374 616e 6365 2920 2d3e  t().instance) ->
+00001630: 206c 6973 745b 5461 736b 4d6f 6465 6c4f   list[TaskModelO
+00001640: 7574 5d3a 0a20 2020 2072 6574 7572 6e20  ut]:.    return 
+00001650: 5461 736b 4d6f 6465 6c4f 7574 2e66 726f  TaskModelOut.fro
+00001660: 6d5f 6f72 6d28 7461 736b 290a 6060 600a  m_orm(task).```.
+00001670: 0a2d 2d2d 0a0a 2323 2052 6571 7565 7374  .---..## Request
+00001680: 730a 0a23 2323 204c 6973 740a 0a4f 6e20  s..### List..On 
+00001690: 7265 7175 6573 7420 6566 6665 6374 6976  request effectiv
+000016a0: 6520 7175 6572 7973 6574 2077 696c 6c20  e queryset will 
+000016b0: 6265 2066 696c 7465 7265 6420 616e 6420  be filtered and 
+000016c0: 6f72 6465 7265 6420 6279 2071 7565 7279  ordered by query
+000016d0: 2070 6172 616d 732e 0a0a 466f 7220 6578   params...For ex
+000016e0: 616d 706c 652c 2075 7365 7220 6861 7320  ample, user has 
+000016f0: 7265 7175 6573 7465 6420 656e 6470 6f69  requested endpoi
+00001700: 6e74 2077 6974 6820 736f 6d65 2071 7565  nt with some que
+00001710: 7279 2070 6172 616d 730a 6060 606a 736f  ry params.```jso
+00001720: 6e0a 7b0a 2020 2020 2263 7265 6174 6564  n.{.    "created
+00001730: 5f61 745f 5f6c 7465 223a 2022 3230 3233  _at__lte": "2023
+00001740: 2d30 312d 3031 5430 303a 3030 3a30 3022  -01-01T00:00:00"
+00001750: 2c0a 2020 2020 2261 7070 726f 7665 6422  ,.    "approved"
+00001760: 3a20 6661 6c73 652c 0a20 2020 2022 6f72  : false,.    "or
+00001770: 6465 7269 6e67 5b5d 223a 2022 6372 6561  dering[]": "crea
+00001780: 7465 645f 6174 222c 0a7d 0a60 6060 0a0a  ted_at",.}.```..
+00001790: 5265 7175 6573 7420 5552 4c20 6c6f 6f6b  Request URL look
+000017a0: 7320 6c69 6b65 2020 0a60 6060 6874 7470  s like  .```http
+000017b0: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3030  ://localhost:800
+000017c0: 302f 7461 736b 732f 3f63 7265 6174 6564  0/tasks/?created
+000017d0: 5f61 745f 5f6c 7465 3d32 3032 332d 3031  _at__lte=2023-01
+000017e0: 2d30 3154 3030 3a30 303a 3030 2661 7070  -01T00:00:00&app
+000017f0: 726f 7665 643d 6661 6c73 6526 6f72 6465  roved=false&orde
+00001800: 7269 6e67 5b5d 3d63 7265 6174 6564 5f61  ring[]=created_a
+00001810: 7460 6060 0a0a 4566 6665 6374 6976 6520  t```..Effective 
+00001820: 7175 6572 7973 6574 2061 7420 7468 6520  queryset at the 
+00001830: 656e 6470 6f69 6e74 206d 6574 686f 6420  endpoint method 
+00001840: 7769 6c6c 2062 650a 6060 6070 7974 686f  will be.```pytho
+00001850: 6e0a 280a 2020 2020 5461 736b 0a20 2020  n.(.    Task.   
+00001860: 202e 6669 6c74 6572 2863 7265 6174 6564   .filter(created
+00001870: 5f61 745f 5f6c 7465 3d64 6174 6574 696d  _at__lte=datetim
+00001880: 652e 6461 7465 7469 6d65 2832 3032 332c  e.datetime(2023,
+00001890: 2031 2c20 312c 2030 2c20 302c 2030 292c   1, 1, 0, 0, 0),
+000018a0: 2061 7070 726f 7665 643d 4661 6c73 6529   approved=False)
+000018b0: 0a20 2020 202e 6f72 6465 725f 6279 2822  .    .order_by("
+000018c0: 6372 6561 7465 645f 6174 2229 0a29 0a60  created_at").).`
+000018d0: 6060 0a0a 2323 2320 4c69 7374 2070 6167  ``..### List pag
+000018e0: 696e 6174 6564 0a0a 4c69 6b65 206e 6f74  inated..Like not
+000018f0: 2070 6167 696e 6174 6564 2065 6e64 706f   paginated endpo
+00001900: 696e 7420 6174 2074 6869 7320 7175 6572  int at this quer
+00001910: 7973 6574 2077 696c 6c20 6265 2066 696c  yset will be fil
+00001920: 7465 7265 642c 206f 7264 6572 696e 6720  tered, ordering 
+00001930: 616e 6420 6164 6469 7469 6f6e 616c 2070  and additional p
+00001940: 6167 696e 6174 6564 2e0a 0a46 6f72 2065  aginated...For e
+00001950: 7861 6d70 6c65 2c20 7573 6572 2068 6173  xample, user has
+00001960: 2072 6571 7565 7374 6564 2065 6e64 706f   requested endpo
+00001970: 696e 7420 7769 7468 2073 6f6d 6520 7175  int with some qu
+00001980: 6572 7920 7061 7261 6d73 0a60 6060 6a73  ery params.```js
+00001990: 6f6e 0a7b 0a20 2020 2022 7061 6765 223a  on.{.    "page":
+000019a0: 2032 2c0a 2020 2020 2270 6572 5f70 6167   2,.    "per_pag
+000019b0: 6522 3a20 3130 2c0a 2020 2020 2263 7265  e": 10,.    "cre
+000019c0: 6174 6564 5f61 745f 5f6c 7465 223a 2022  ated_at__lte": "
+000019d0: 3230 3233 2d30 312d 3031 5430 303a 3030  2023-01-01T00:00
+000019e0: 3a30 3022 2c0a 2020 2020 2261 7070 726f  :00",.    "appro
+000019f0: 7665 6422 3a20 6661 6c73 652c 0a20 2020  ved": false,.   
+00001a00: 2022 6f72 6465 7269 6e67 5b5d 223a 2022   "ordering[]": "
+00001a10: 6372 6561 7465 645f 6174 222c 0a7d 0a60  created_at",.}.`
+00001a20: 6060 0a0a 5265 7175 6573 7420 5552 4c20  ``..Request URL 
+00001a30: 6c6f 6f6b 7320 6c69 6b65 2020 200a 6060  looks like   .``
+00001a40: 6068 7474 703a 2f2f 6c6f 6361 6c68 6f73  `http://localhos
+00001a50: 743a 3830 3030 2f74 6173 6b73 2f3f 7061  t:8000/tasks/?pa
+00001a60: 6765 3d32 2670 6572 5f70 6167 653d 3130  ge=2&per_page=10
+00001a70: 2663 7265 6174 6564 5f61 745f 5f6c 7465  &created_at__lte
+00001a80: 3d32 3032 332d 3031 2d30 3154 3030 3a30  =2023-01-01T00:0
+00001a90: 303a 3030 2661 7070 726f 7665 643d 6661  0:00&approved=fa
+00001aa0: 6c73 6526 6f72 6465 7269 6e67 5b5d 3d63  lse&ordering[]=c
+00001ab0: 7265 6174 6564 5f61 7460 6060 0a0a 0a45  reated_at```...E
+00001ac0: 6666 6563 7469 7665 2071 7565 7279 7365  ffective queryse
+00001ad0: 7420 6174 2065 6e64 706f 696e 7420 6d65  t at endpoint me
+00001ae0: 7468 6f64 2077 696c 6c20 6265 0a60 6060  thod will be.```
+00001af0: 7079 7468 6f6e 0a28 0a20 2020 2054 6173  python.(.    Tas
+00001b00: 6b0a 2020 2020 2e66 696c 7465 7228 6372  k.    .filter(cr
+00001b10: 6561 7465 645f 6174 5f5f 6c74 653d 6461  eated_at__lte=da
+00001b20: 7465 7469 6d65 2e64 6174 6574 696d 6528  tetime.datetime(
+00001b30: 3230 3233 2c20 312c 2031 2c20 302c 2030  2023, 1, 1, 0, 0
+00001b40: 2c20 3029 2c20 6170 7072 6f76 6564 3d46  , 0), approved=F
+00001b50: 616c 7365 290a 2020 2020 2e6f 7264 6572  alse).    .order
+00001b60: 5f62 7928 2263 7265 6174 6564 5f61 7422  _by("created_at"
+00001b70: 290a 2020 2020 2e6f 6666 7365 7428 3130  ).    .offset(10
+00001b80: 290a 2020 2020 2e6c 696d 6974 2831 3029  ).    .limit(10)
+00001b90: 0a29 0a60 6060 0a0a 4173 2077 656c 6c20  .).```..As well 
+00001ba0: 6173 2074 6f20 6052 6573 706f 6e73 6560  as to `Response`
+00001bb0: 2077 696c 6c20 6265 2061 6464 6564 2070   will be added p
+00001bc0: 6167 696e 6174 696f 6e20 696e 666f 726d  agination inform
+00001bd0: 6174 696f 6e2e 2050 6167 696e 6174 696f  ation. Paginatio
+00001be0: 6e20 696e 666f 726d 6174 696f 6e20 616c  n information al
+00001bf0: 7761 7973 206d 6174 6368 6573 2065 6666  ways matches eff
+00001c00: 6563 7469 7665 2071 7565 7279 7365 740a  ective queryset.
+00001c10: 6060 606a 736f 6e0a 7b0a 2020 2020 2278  ```json.{.    "x
+00001c20: 2d70 6167 6522 3a20 2232 222c 0a20 2020  -page": "2",.   
+00001c30: 2022 782d 7061 6765 7322 3a20 2234 222c   "x-pages": "4",
+00001c40: 0a20 2020 2022 782d 7065 722d 7061 6765  .    "x-per-page
+00001c50: 223a 2022 3130 222c 0a20 2020 2022 782d  ": "10",.    "x-
+00001c60: 746f 7461 6c22 3a20 2233 3222 0a7d 0a60  total": "32".}.`
+00001c70: 6060 0a0a 2323 2320 5265 7472 6965 7665  ``..### Retrieve
+00001c80: 0a0a 5265 7175 6573 7420 5552 4c20 6c6f  ..Request URL lo
+00001c90: 6f6b 7320 6c69 6b65 2020 200a 6060 6068  oks like   .```h
+00001ca0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+00001cb0: 3830 3030 2f74 6173 6b73 2f31 302f 6060  8000/tasks/10/``
+00001cc0: 600a 0a45 6e64 706f 696e 7420 6d65 7468  `..Endpoint meth
+00001cd0: 6f64 2077 696c 6c20 6765 7420 6054 6173  od will get `Tas
+00001ce0: 6b60 2077 6974 6820 6069 6420 3d3d 2031  k` with `id == 1
+00001cf0: 3060 2061 7320 6172 6775 6d65 6e74 2060  0` as argument `
+00001d00: 7461 736b 602e 2020 2020 200a 4966 2060  task`.     .If `
+00001d10: 5461 736b 6020 7769 7468 2060 6964 203d  Task` with `id =
+00001d20: 3d20 3130 6020 646f 6573 206e 6f74 2065  = 10` does not e
+00001d30: 7869 7374 2074 6865 6e20 656e 6470 6f69  xist then endpoi
+00001d40: 6e74 2072 6574 7572 6e20 6052 6573 706f  nt return `Respo
+00001d50: 6e73 6528 3430 3429 6020 200a            nse(404)`  .
```

