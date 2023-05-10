# Comparing `tmp/glacier-0.3.5.tar.gz` & `tmp/glacier-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glacier-0.3.5.tar", max compression
+gzip compressed data, was "glacier-0.4.0.tar", max compression
```

## Comparing `glacier-0.3.5.tar` & `glacier-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-04-21 04:27:15.100552 glacier-0.3.5/LICENSE
--rw-r--r--   0        0        0       34 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/__init__.py
--rw-r--r--   0        0        0     8558 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/core.py
--rw-r--r--   0        0        0     7855 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/docstring.py
--rw-r--r--   0        0        0      493 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/misc.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/py.typed
--rw-r--r--   0        0        0      934 2023-04-21 04:27:15.104552 glacier-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 glacier-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-10 05:25:25.532935 glacier-0.4.0/LICENSE
+-rw-r--r--   0        0        0       34 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/__init__.py
+-rw-r--r--   0        0        0     8553 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/core.py
+-rw-r--r--   0        0        0     7855 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/docstring.py
+-rw-r--r--   0        0        0      493 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/misc.py
+-rw-r--r--   0        0        0        0 2023-05-10 05:25:25.532935 glacier-0.4.0/glacier/py.typed
+-rw-r--r--   0        0        0      934 2023-05-10 05:25:25.532935 glacier-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 glacier-0.4.0/PKG-INFO
```

### Comparing `glacier-0.3.5/LICENSE` & `glacier-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glacier-0.3.5/glacier/core.py` & `glacier-0.4.0/glacier/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,52 +34,52 @@
 DEFAULT_COLOR_OPTIONS = dict(
     help_headers_color='white',
     help_options_color='cyan',
 )
 
 
 GlacierFunction = Union[
-    Callable[..., None],
+    Callable[..., Any],
     Callable[..., Coroutine[Any, Any, Any]],
 ]
 
 
 GlacierUnit = Union[
     List[GlacierFunction],
     Dict[str, GlacierFunction],
 ]
 
 
-def get_enum_map(f: Callable[..., None]) -> Dict[str, Dict[str, Any]]:
+def get_enum_map(f: Callable[..., Any]) -> Dict[str, Dict[str, Any]]:
     sig = signature(f)
 
     # pick enum from signature
     enum_map: Dict[str, Dict[str, Any]] = {}
     for param in sig.parameters.values():
         if issubclass(param.annotation, Enum):
             enum_class = param.annotation
             enum_map.setdefault(param.name, {})
             for enum_entry in enum_class:
                 enum_map[param.name][enum_entry.value] = enum_entry
     return enum_map
 
 
 def glacier_wrap(
-    f: Callable[..., None],
+    f: Callable[..., Any],
     enum_map: Dict[str, Dict[str, Any]],
-) -> Callable[..., None]:
+) -> Callable[..., Any]:
     """
     Return the new function which is click-compatible
     (has no enum signature arguments) from the arbitrary glacier compatible
     function
     """
 
     # Implemented the argument convert logic
     @functools.wraps(f)
-    def wrapped(*args: Any, **kwargs: Any) -> None:
+    def wrapped(*args: Any, **kwargs: Any) -> Any:
         # convert args and kwargs
         converted_kwargs = {}
         for name, value in kwargs.items():
             if name in enum_map:
                 converted_kwargs[name] = enum_map[name][value]
             else:
                 converted_kwargs[name] = value
```

### Comparing `glacier-0.3.5/glacier/docstring.py` & `glacier-0.4.0/glacier/docstring.py`

 * *Files identical despite different names*

### Comparing `glacier-0.3.5/pyproject.toml` & `glacier-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "glacier"
-version = "0.3.5"
+version = "0.4.0"
 description = ""
 authors = ["Hiroki Konishi <relastle@gmail.com>"]
 license = "MIT"
 packages = [
   {include = "glacier"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.9"
 typing-extensions = "^4.1.1"
 click = "^8.0.4"
 click-help-colors = "^0.9.1"
 importlib-metadata = "^4.11.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "==6.0.1"
```

### Comparing `glacier-0.3.5/PKG-INFO` & `glacier-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: glacier
-Version: 0.3.5
+Version: 0.4.0
 Summary: 
 License: MIT
 Author: Hiroki Konishi
 Author-email: relastle@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: click-help-colors (>=0.9.1,<0.10.0)
 Requires-Dist: importlib-metadata (>=4.11.3,<5.0.0)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
```

