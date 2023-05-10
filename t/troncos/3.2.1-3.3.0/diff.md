# Comparing `tmp/troncos-3.2.1.tar.gz` & `tmp/troncos-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-3.2.1.tar", max compression
+gzip compressed data, was "troncos-3.3.0.tar", max compression
```

## Comparing `troncos-3.2.1.tar` & `troncos-3.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1077 2023-05-08 12:26:19.531825 troncos-3.2.1/LICENSE
--rw-r--r--   0        0        0    15818 2023-05-08 12:26:19.531825 troncos-3.2.1/README.md
--rw-r--r--   0        0        0     2278 2023-05-08 12:26:19.535825 troncos-3.2.1/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/__init__.py
--rw-r--r--   0        0        0     1214 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/_ddlazy/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/asgi/__init__.py
--rw-r--r--   0        0        0     3049 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/asgi/middleware.py
--rw-r--r--   0        0        0     3367 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/asgi/utils.py
--rw-r--r--   0        0        0      993 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/gunicorn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/starlette/__init__.py
--rw-r--r--   0        0        0     4488 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/starlette/uvicorn.py
--rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/structlog/__init__.py
--rw-r--r--   0        0        0     2222 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/structlog/processors.py
--rw-r--r--   0        0        0     5589 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/frameworks/structlog/setup.py
--rw-r--r--   0        0        0     4922 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/logs/__init__.py
--rw-r--r--   0        0        0     3710 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/logs/filters.py
--rw-r--r--   0        0        0     9364 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/logs/formatters.py
--rw-r--r--   0        0        0     3090 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/profiling/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/py.typed
--rw-r--r--   0        0        0    10656 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/traces/__init__.py
--rw-r--r--   0        0        0     6585 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/traces/dd_shim.py
--rw-r--r--   0        0        0     8351 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/traces/decorate.py
--rw-r--r--   0        0        0     1459 2023-05-08 12:26:19.535825 troncos-3.2.1/troncos/traces/propagation.py
--rw-r--r--   0        0        0    16888 1970-01-01 00:00:00.000000 troncos-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-10 13:08:14.285874 troncos-3.3.0/LICENSE
+-rw-r--r--   0        0        0    15818 2023-05-10 13:08:14.285874 troncos-3.3.0/README.md
+-rw-r--r--   0        0        0     2326 2023-05-10 13:08:14.289874 troncos-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/__init__.py
+-rw-r--r--   0        0        0     1214 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/_ddlazy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/asgi/__init__.py
+-rw-r--r--   0        0        0     3049 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/asgi/middleware.py
+-rw-r--r--   0        0        0     3367 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/asgi/utils.py
+-rw-r--r--   0        0        0      993 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/gunicorn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/starlette/__init__.py
+-rw-r--r--   0        0        0     4488 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/starlette/uvicorn.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/structlog/__init__.py
+-rw-r--r--   0        0        0     2222 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/structlog/processors.py
+-rw-r--r--   0        0        0     5589 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/frameworks/structlog/setup.py
+-rw-r--r--   0        0        0     4922 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/logs/__init__.py
+-rw-r--r--   0        0        0     3710 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/logs/filters.py
+-rw-r--r--   0        0        0     9364 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/logs/formatters.py
+-rw-r--r--   0        0        0     3090 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/py.typed
+-rw-r--r--   0        0        0    10949 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/traces/__init__.py
+-rw-r--r--   0        0        0     7563 2023-05-10 13:08:14.289874 troncos-3.3.0/troncos/traces/dd_shim.py
+-rw-r--r--   0        0        0     8351 2023-05-10 13:08:14.293874 troncos-3.3.0/troncos/traces/decorate.py
+-rw-r--r--   0        0        0     1459 2023-05-10 13:08:14.293874 troncos-3.3.0/troncos/traces/propagation.py
+-rw-r--r--   0        0        0    16888 1970-01-01 00:00:00.000000 troncos-3.3.0/PKG-INFO
```

### Comparing `troncos-3.2.1/LICENSE` & `troncos-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/README.md` & `troncos-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/pyproject.toml` & `troncos-3.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "troncos"
-version = "3.2.1"
+version = "3.3.0"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/troncos"
 repository = "https://github.com/kolonialno/troncos"
 documentation = "https://github.com/kolonialno/troncos"
 keywords = ["logs", "traces", "opentelemetry"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-ddtrace = "1.12.4"
+ddtrace = "1.13.0"
 opentelemetry-sdk = "1.17.0"
 opentelemetry-exporter-otlp-proto-http = {version = "1.17.0", optional = true}
 opentelemetry-exporter-otlp-proto-grpc = {version = "1.17.0", optional = true}
 structlog = {version = ">=22.3,<24.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
@@ -30,14 +30,16 @@
 pytest_codeblocks = "^0.16.1"
 fastapi = ">=0.92,<0.96"
 requests = "^2.28.2"
 pytest-cov = "^4.0.0"
 types-requests = "^2.28.11.14"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 django-environ = "^0.9.0"
+pytest-benchmark = "^4.0.0"
+snakeviz = "^2.2.0"
 
 [tool.poetry.extras]
 http = ["opentelemetry-exporter-otlp-proto-http"]
 grpc = ["opentelemetry-exporter-otlp-proto-grpc"]
 structlog = ["structlog"]
 
 [tool.black]
```

### Comparing `troncos-3.2.1/troncos/_ddlazy/__init__.py` & `troncos-3.3.0/troncos/_ddlazy/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/frameworks/asgi/middleware.py` & `troncos-3.3.0/troncos/frameworks/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/frameworks/asgi/utils.py` & `troncos-3.3.0/troncos/frameworks/asgi/utils.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/frameworks/gunicorn/__init__.py` & `troncos-3.3.0/troncos/frameworks/gunicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/frameworks/starlette/uvicorn.py` & `troncos-3.3.0/troncos/frameworks/starlette/uvicorn.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/frameworks/structlog/processors.py` & `troncos-3.3.0/troncos/frameworks/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/frameworks/structlog/setup.py` & `troncos-3.3.0/troncos/frameworks/structlog/setup.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/logs/__init__.py` & `troncos-3.3.0/troncos/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/logs/filters.py` & `troncos-3.3.0/troncos/logs/filters.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/logs/formatters.py` & `troncos-3.3.0/troncos/logs/formatters.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/profiling/__init__.py` & `troncos-3.3.0/troncos/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/traces/__init__.py` & `troncos-3.3.0/troncos/traces/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,58 @@
 def _class_index(some_list: list[Any], k: Any) -> int | None:
     for index, thing in enumerate(some_list):
         if isinstance(thing, k):
             return index
     return None
 
 
+def _patch_dd_tracer(*, dd_span_processor: DDSpanProcessor, enable_dd: bool) -> None:
+    import ddtrace
+
+    # Shutdown default tracer immediately
+    try:
+        ddtrace.tracer.shutdown()
+    except ValueError:
+        pass
+
+    class _PatchedDDTracer(ddtrace.Tracer):
+        # Since we cannot patch _default_span_processors_factory,
+        # we patch all functions that call it
+        def __init__(self, *args, **kwargs):  # type: ignore[no-untyped-def]
+            super().__init__(*args, **kwargs)
+            self._fix_span_processors()
+
+        def configure(self, *args, **kwargs):  # type: ignore[no-untyped-def]
+            super().configure(*args, **kwargs)
+            self._fix_span_processors()
+
+        def _child_after_fork(self):  # type: ignore[no-untyped-def]
+            super()._child_after_fork()  # type: ignore[no-untyped-call]
+            self._fix_span_processors()
+
+        def _fix_span_processors(self) -> None:
+            processors = self._span_processors
+
+            # Remove dd span aggregator if needed
+            dd_span_aggregator = _class_index(
+                processors, ddtrace.internal.processor.trace.SpanAggregator
+            )
+            if dd_span_aggregator and not enable_dd:
+                processors.pop(dd_span_aggregator)
+
+            # Add the custom processor
+            if not _class_index(processors, DDSpanProcessor):
+                processors.append(dd_span_processor)  # type: ignore[arg-type]
+
+    # Patch dd tracer and create new tracer
+    ddtrace.Tracer = _PatchedDDTracer  # type: ignore[misc]
+    ddtrace.tracer = ddtrace.Tracer()  # type: ignore[no-untyped-call]
+    ddlazy._dd_tracer = ddtrace.tracer  # type: ignore[assignment]
+
+
 def init_tracing_basic(
     service_name: str,
     service_env: str | None = None,
     service_version: str | None = None,
     service_attributes: dict[str, str] | None = None,
     endpoint: str | None = None,
     endpoint_dd: str | None = None,
@@ -218,54 +262,20 @@
         logger.info(f"DD traces exported to {endpoint_dd}")
     else:
         logger.info("DD traces not exported")
 
     ddtrace_already_imported = "ddtrace" in sys.modules
 
     # Initialize ddtrace
-    import ddtrace
-
-    # Shutdown default tracer immediately
-    try:
-        ddtrace.tracer.shutdown()
-    except ValueError:
-        pass
-
-    class _PatchedDDTracer(ddtrace.Tracer):
-        # Since we cannot patch _default_span_processors_factory,
-        # we patch all functions that call it
-        def __init__(self, *args, **kwargs):  # type: ignore[no-untyped-def]
-            super().__init__(*args, **kwargs)
-            self._fix_span_processors()
-
-        def configure(self, *args, **kwargs):  # type: ignore[no-untyped-def]
-            super().configure(*args, **kwargs)
-            self._fix_span_processors()
-
-        def _child_after_fork(self):  # type: ignore[no-untyped-def]
-            super()._child_after_fork()  # type: ignore[no-untyped-call]
-            self._fix_span_processors()
-
-        def _fix_span_processors(self) -> None:
-            processors = self._span_processors
-
-            # Remove dd span aggregator if needed
-            dd_span_aggregator = _class_index(
-                processors, ddtrace.internal.processor.trace.SpanAggregator
-            )
-            if dd_span_aggregator and not endpoint_dd:
-                processors.pop(dd_span_aggregator)
-
-            # Add custom processor
-            if not _class_index(processors, DDSpanProcessor):
-                processors.append(custom_dd_span_processor)  # type: ignore[arg-type]
+    _patch_dd_tracer(
+        dd_span_processor=custom_dd_span_processor,
+        enable_dd=endpoint_dd is not None,
+    )
 
-    # Patch dd tracer and create new tracer
-    ddtrace.Tracer = _PatchedDDTracer  # type: ignore[misc]
-    ddtrace.tracer = ddtrace.Tracer()  # type: ignore[no-untyped-call]
+    import ddtrace
 
     # Check if someone imported ddtrace before us. We do this by checking if the
     # variables we set above were in fact used
     if ddtrace_already_imported:
         logger.warning(
             "DETECTED THAT ddtrace WAS IMPORTED BY ANOTHER MODULE BEFORE 'init_tracing_basic' WAS CALLED. THIS IS BAD!",  # noqa: E501
         )
```

### Comparing `troncos-3.2.1/troncos/traces/dd_shim.py` & `troncos-3.3.0/troncos/traces/dd_shim.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,23 @@
-from typing import Any
+from typing import Any, Dict, Optional, Union
 
+from opentelemetry.attributes import BoundedAttributes  # type: ignore[attr-defined]
 from opentelemetry.sdk.resources import Attributes, Resource
-from opentelemetry.sdk.trace import Span, SpanContext, SpanProcessor
+from opentelemetry.sdk.trace import (
+    EventBase,
+    ReadableSpan,
+    Span,
+    SpanContext,
+    SpanProcessor,
+    _UnsetLimits,
+)
 from opentelemetry.sdk.util.instrumentation import InstrumentationScope
 from opentelemetry.trace import SpanKind, Status, StatusCode
 from opentelemetry.trace.span import TraceFlags
+from opentelemetry.util.types import AttributeValue
 
 from troncos import OTEL_LIBRARY_NAME, OTEL_LIBRARY_VERSION
 
 _instrumentation_scope = InstrumentationScope(OTEL_LIBRARY_NAME, OTEL_LIBRARY_VERSION)
 _default_trace_flags = TraceFlags(1)
 _span_kind_map = {
     "server": SpanKind.SERVER,
@@ -30,34 +39,40 @@
         self,
         dd_span: Any,
         base_resources: Attributes,
         default_resource: Resource,
         dd_traces_exported: bool,
         ignore_attrs: list[str],
     ) -> None:
-        super().__init__(
+        ReadableSpan.__init__(
+            self,
             dd_span.name,
             _internal_span_context(dd_span),
             parent=self._create_parent_context(dd_span),
-            sampler=None,
-            trace_config=None,
             resource=self._create_resource(dd_span, base_resources, default_resource),
             kind=self._create_span_kind(dd_span),
             instrumentation_scope=_instrumentation_scope,
         )
-        self.start(dd_span.start_ns)
+        self._limits = _UnsetLimits
+        self._events = self._new_events()  # type: ignore[no-untyped-call]
+        self._raw_attributes: Attributes = {}
+
+        self._start_time = dd_span.start_ns
         self._apply_translation(dd_span, ignore_attrs)
         if dd_traces_exported:
-            self.set_attributes(
-                {
-                    "dd_trace_id": str(dd_span.trace_id),
-                    "dd_span_id": str(dd_span.span_id),
-                }
-            )
-        self.end(dd_span.start_ns + dd_span.duration_ns)
+            self._raw_attributes["dd_trace_id"] = str(dd_span.trace_id)
+            self._raw_attributes["dd_span_id"] = str(dd_span.span_id)
+
+        self._end_time = dd_span.start_ns + dd_span.duration_ns
+        self._attributes = BoundedAttributes(
+            _UnsetLimits.max_span_attributes,
+            self._raw_attributes,
+            immutable=True,
+            max_value_len=_UnsetLimits.max_span_attribute_length,
+        )
 
     @staticmethod
     def _create_parent_context(dd_span: Any) -> SpanContext | None:
         if dd_span.parent_id:
             if not dd_span._parent:
                 # External trace parent
                 return SpanContext(dd_span.trace_id, dd_span.parent_id, True)
@@ -85,20 +100,18 @@
     @staticmethod
     def _create_span_kind(dd_span: Any) -> SpanKind:
         dd_kind = dd_span._meta.get("span.kind", "none")
         return _span_kind_map.get(dd_kind, SpanKind.INTERNAL)
 
     def _apply_translation(self, dd_span: Any, ignore_attrs: list[str]) -> None:
         otel_error_attr_dict = {}
-        otel_span_attr = {
-            "resource": dd_span.resource,
-        }
+        self._raw_attributes["resource"] = dd_span.resource
 
         if dd_span.span_type:
-            otel_span_attr["dd_type"] = dd_span.span_type
+            self._raw_attributes["dd_type"] = dd_span.span_type
 
         # Collect all "attributes" from the dd span
         dd_span_attr: dict[str, Any] = {
             **dd_span._meta,
             **dd_span._metrics,
         }
         dd_span_err_attr_mapping = {
@@ -111,33 +124,44 @@
         for k, v in dd_span_attr.items():
             otel_err_attr = dd_span_err_attr_mapping.get(k)
             if k.startswith("_dd"):
                 continue
             elif otel_err_attr:
                 otel_error_attr_dict[otel_err_attr] = v
             elif k not in ignore_attrs:
-                otel_span_attr[k] = v
-
-        self.set_attributes(otel_span_attr)
+                self._raw_attributes[k] = v
 
         # Map exception attributes
         if otel_error_attr_dict:
-            # self.set_attributes(otel_error_attr_dict)  # Is this needed?
             self.add_event(name="exception", attributes=otel_error_attr_dict)
 
             status_exp_type = otel_error_attr_dict.get("exception.type", None)
             status_exp_msg = otel_error_attr_dict.get("exception.message", None)
 
-            self.set_status(
-                Status(
-                    status_code=StatusCode.ERROR,
-                    description=f"{status_exp_type}: {status_exp_msg}",
-                )
+            self._status = Status(
+                status_code=StatusCode.ERROR,
+                description=f"{status_exp_type}: {status_exp_msg}",
             )
 
+    def _add_event(self, event: EventBase) -> None:
+        self._events.append(event)  # type: ignore[attr-defined]
+
+    def set_attribute(self, key: str, value: AttributeValue) -> None:
+        assert False, "Use 'self._raw_attributes[key] = value' instead"
+
+    def set_attributes(self, attributes: Dict[str, AttributeValue]) -> None:
+        assert False, "Use 'self._raw_attributes[key] = value' instead"
+
+    def set_status(
+        self,
+        status: Union[Status, StatusCode],
+        description: Optional[str] = None,
+    ) -> None:
+        assert False, "Use 'self._status = status' instead"
+
 
 class DDSpanProcessor:
     """
     A ddtrace span processor that translates dd spans into otel span and
     sends them to otel span processors
     """
```

### Comparing `troncos-3.2.1/troncos/traces/decorate.py` & `troncos-3.3.0/troncos/traces/decorate.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/troncos/traces/propagation.py` & `troncos-3.3.0/troncos/traces/propagation.py`

 * *Files identical despite different names*

### Comparing `troncos-3.2.1/PKG-INFO` & `troncos-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 3.2.1
+Version: 3.3.0
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc
 Provides-Extra: http
 Provides-Extra: structlog
-Requires-Dist: ddtrace (==1.12.4)
+Requires-Dist: ddtrace (==1.13.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.17.0) ; extra == "grpc"
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.17.0) ; extra == "http"
 Requires-Dist: opentelemetry-sdk (==1.17.0)
 Requires-Dist: structlog (>=22.3,<24.0) ; extra == "structlog"
 Project-URL: Documentation, https://github.com/kolonialno/troncos
 Project-URL: Repository, https://github.com/kolonialno/troncos
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: troncos Version: 3.2.1 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 3.3.0 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc Provides-Extra: http Provides-Extra: structlog Requires-
-Dist: ddtrace (==1.12.4) Requires-Dist: opentelemetry-exporter-otlp-proto-grpc
+Dist: ddtrace (==1.13.0) Requires-Dist: opentelemetry-exporter-otlp-proto-grpc
 (==1.17.0) ; extra == "grpc" Requires-Dist: opentelemetry-exporter-otlp-proto-
 http (==1.17.0) ; extra == "http" Requires-Dist: opentelemetry-sdk (==1.17.0)
 Requires-Dist: structlog (>=22.3,<24.0) ; extra == "structlog" Project-URL:
 Documentation, https://github.com/kolonialno/troncos Project-URL: Repository,
 https://github.com/kolonialno/troncos Description-Content-Type: text/markdown
                                   ****** ðªµ
                                    Troncos
```

