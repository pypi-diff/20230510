# Comparing `tmp/property-graph-1.0.2.tar.gz` & `tmp/property-graph-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-graph-1.0.2.tar", last modified: Mon Mar 27 23:25:27 2023, max compression
+gzip compressed data, was "property-graph-1.0.3.tar", last modified: Wed May 10 19:29:48 2023, max compression
```

## Comparing `property-graph-1.0.2.tar` & `property-graph-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:25:27.491814 property-graph-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-27 23:25:18.000000 property-graph-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-03-27 23:25:27.491814 property-graph-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-27 23:25:18.000000 property-graph-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-27 23:25:18.000000 property-graph-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 23:25:27.491814 property-graph-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:25:27.487814 property-graph-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:25:27.487814 property-graph-1.0.2/src/property_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-03-27 23:25:27.000000 property-graph-1.0.2/src/property_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-27 23:25:27.000000 property-graph-1.0.2/src/property_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 23:25:27.000000 property-graph-1.0.2/src/property_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 23:25:27.000000 property-graph-1.0.2/src/property_graph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:25:27.491814 property-graph-1.0.2/src/pypg/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/property_transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:25:27.491814 property-graph-1.0.2/src/pypg/traits/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/allowed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/obligate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/observable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/overridable.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/read_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/traits/validated.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/transcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-27 23:25:18.000000 property-graph-1.0.2/src/pypg/type_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:25:27.491814 property-graph-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_allowed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_obligate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_observable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_overridable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_readonly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_type_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-27 23:25:18.000000 property-graph-1.0.2/tests/test_type_schema_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.617139 property-graph-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 19:29:39.000000 property-graph-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-05-10 19:29:48.617139 property-graph-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-10 19:29:39.000000 property-graph-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-10 19:29:39.000000 property-graph-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 19:29:48.617139 property-graph-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.613139 property-graph-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.613139 property-graph-1.0.3/src/property_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-05-10 19:29:48.000000 property-graph-1.0.3/src/property_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-10 19:29:48.000000 property-graph-1.0.3/src/property_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:29:48.000000 property-graph-1.0.3/src/property_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 19:29:48.000000 property-graph-1.0.3/src/property_graph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.613139 property-graph-1.0.3/src/pypg/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/property_transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.613139 property-graph-1.0.3/src/pypg/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/allowed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/obligate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/overridable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/traits/validated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/transcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-10 19:29:39.000000 property-graph-1.0.3/src/pypg/type_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:29:48.617139 property-graph-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_allowed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_obligate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_observable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_overridable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_readonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_type_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-10 19:29:39.000000 property-graph-1.0.3/tests/test_type_schema_encoding.py
```

### Comparing `property-graph-1.0.2/LICENSE` & `property-graph-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/PKG-INFO` & `property-graph-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-graph
-Version: 1.0.2
+Version: 1.0.3
 Summary: python library for working with objects as graphs of property data
 Author-email: Matt Fowler <mattefowler@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `property-graph-1.0.2/README.md` & `property-graph-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/pyproject.toml` & `property-graph-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/property_graph.egg-info/PKG-INFO` & `property-graph-1.0.3/src/property_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-graph
-Version: 1.0.2
+Version: 1.0.3
 Summary: python library for working with objects as graphs of property data
 Author-email: Matt Fowler <mattefowler@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `property-graph-1.0.2/src/property_graph.egg-info/SOURCES.txt` & `property-graph-1.0.3/src/property_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/locator.py` & `property-graph-1.0.3/src/pypg/locator.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/property.py` & `property-graph-1.0.3/src/pypg/property.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                 Property provided by a classmethod may be overridden by a
                 subclass of the type originally declaring the Property.
         """
         super().__init__()
         self._subclass_proxies: dict[PropertyType, _Proxy] = {}
         self._default = default
         self.name = None
-        self.__declaring_type = None
+        self.__declaring_type: PropertyType = None
         self._getter = self.default_getter if getter is None else getter
         self._setter = self.default_setter if setter is None else setter
         self.__traits = tuple(
             filter(None, traits if isinstance(traits, Iterable) else [traits])
         )
 
     @cached_property
@@ -353,28 +353,32 @@
         """
         return (
             self._default(instance)
             if isinstance(self._default, (FunctionReference, Callable))
             else self._default
         )
 
+    @cached_property
+    def attribute_key(self):
+        return f"#_{self.__declaring_type.__name__}__{self.name}"
+
     def default_getter(self, instance) -> T:
         """
         The getter method used by a Property if none is otherwise provided. It
         retrieves its data in instance.__dict__ using self as the key. If
         instance is under construction, the initialization process will
         construct it on-demand as required.
         Args:
             instance: the instance storing the data for self.
         Returns:
             the value of this property for instance.
         """
 
         try:
-            return instance.__dict__[self]
+            return instance.__dict__[self.attribute_key]
         except KeyError as k:
             init_ctx = None
             try:
                 init_ctx = _InitializationContext.for_instance(instance)
             except KeyError as k:
                 pass
             if init_ctx is None:
@@ -390,15 +394,15 @@
         """
         The setter method used by a Property if none is otherwise provided. It
         stores its data in instance.__dict__ using self as the key.
         Args:
             instance: the instance whose Property value is being set.
             value: the value to be stored for instance.
         """
-        instance.__dict__[self] = value
+        instance.__dict__[self.attribute_key] = value
 
     def __get__(self, instance: PropertyClass, owner: PropertyType):
         proxy = self._subclass_proxies[owner]
         return proxy if instance is None else proxy.get(instance)
 
     def __set__(self, instance, value):
         self._subclass_proxies[type(instance)].set(instance, value)
```

### Comparing `property-graph-1.0.2/src/pypg/property_transcoder.py` & `property-graph-1.0.3/src/pypg/property_transcoder.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/traits/allowed_range.py` & `property-graph-1.0.3/src/pypg/traits/allowed_range.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/traits/config.py` & `property-graph-1.0.3/src/pypg/traits/config.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/traits/obligate.py` & `property-graph-1.0.3/src/pypg/traits/obligate.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/traits/observable.py` & `property-graph-1.0.3/src/pypg/traits/observable.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/traits/overridable.py` & `property-graph-1.0.3/src/pypg/traits/overridable.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/traits/read_only.py` & `property-graph-1.0.3/src/pypg/traits/read_only.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,12 +8,12 @@
     def __init__(self):
         super().__init__()
 
     def _override(self, instance, value):
         return value
 
     def apply(self, instance, value) -> Any:
-        if self.subject in instance.__dict__:
+        if self.subject.attribute_key in instance.__dict__:
             raise PermissionError(
                 f"{self.subject} of {instance} is read-only and cannot be reassigned."
             )
         return value
```

### Comparing `property-graph-1.0.2/src/pypg/traits/validated.py` & `property-graph-1.0.3/src/pypg/traits/validated.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/transcode.py` & `property-graph-1.0.3/src/pypg/transcode.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/type_registry.py` & `property-graph-1.0.3/src/pypg/type_registry.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/src/pypg/type_utils.py` & `property-graph-1.0.3/src/pypg/type_utils.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_allowed_range.py` & `property-graph-1.0.3/tests/test_allowed_range.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_config.py` & `property-graph-1.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_locator.py` & `property-graph-1.0.3/tests/test_locator.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_obligate.py` & `property-graph-1.0.3/tests/test_obligate.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_observable.py` & `property-graph-1.0.3/tests/test_observable.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_overridable.py` & `property-graph-1.0.3/tests/test_overridable.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_property.py` & `property-graph-1.0.3/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_readonly.py` & `property-graph-1.0.3/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_traits.py` & `property-graph-1.0.3/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_transcoder.py` & `property-graph-1.0.3/tests/test_transcoder.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_type_registry.py` & `property-graph-1.0.3/tests/test_type_registry.py`

 * *Files identical despite different names*

### Comparing `property-graph-1.0.2/tests/test_type_schema_encoding.py` & `property-graph-1.0.3/tests/test_type_schema_encoding.py`

 * *Files identical despite different names*

