# Comparing `tmp/strawberry_resources-0.4.3.tar.gz` & `tmp/strawberry_resources-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_resources-0.4.3.tar", max compression
+gzip compressed data, was "strawberry_resources-0.5.0.tar", max compression
```

## Comparing `strawberry_resources-0.4.3.tar` & `strawberry_resources-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/LICENSE
--rw-r--r--   0        0        0     9125 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/README.md
--rw-r--r--   0        0        0     4057 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1174 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/__init__.py
--rw-r--r--   0        0        0       59 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/__main__.py
--rw-r--r--   0        0        0      123 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/cli/__init__.py
--rw-r--r--   0        0        0     1268 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/cli/export.py
--rw-r--r--   0        0        0     2828 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/exporter.py
--rw-r--r--   0        0        0      124 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/integrations/__init__.py
--rw-r--r--   0        0        0     1660 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/integrations/base.py
--rw-r--r--   0        0        0     9393 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/integrations/django.py
--rw-r--r--   0        0        0        0 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/py.typed
--rw-r--r--   0        0        0      628 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/queries.py
--rw-r--r--   0        0        0     7570 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/resolver.py
--rw-r--r--   0        0        0     7143 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/types.py
--rw-r--r--   0        0        0        0 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/utils/__init__.py
--rw-r--r--   0        0        0     2033 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/utils/inspect.py
--rw-r--r--   0        0        0      662 2023-04-27 21:06:09.009353 strawberry_resources-0.4.3/strawberry_resources/utils/pyutils.py
--rw-r--r--   0        0        0    10950 1970-01-01 00:00:00.000000 strawberry_resources-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-10 20:26:55.027210 strawberry_resources-0.5.0/LICENSE
+-rw-r--r--   0        0        0     9125 2023-05-10 20:26:55.027210 strawberry_resources-0.5.0/README.md
+-rw-r--r--   0        0        0     4057 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1174 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/__main__.py
+-rw-r--r--   0        0        0      123 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/cli/__init__.py
+-rw-r--r--   0        0        0     1268 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/cli/export.py
+-rw-r--r--   0        0        0     2828 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/exporter.py
+-rw-r--r--   0        0        0      124 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/integrations/__init__.py
+-rw-r--r--   0        0        0     1660 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/integrations/base.py
+-rw-r--r--   0        0        0     9742 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/integrations/django.py
+-rw-r--r--   0        0        0        0 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/py.typed
+-rw-r--r--   0        0        0      628 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/queries.py
+-rw-r--r--   0        0        0     7741 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/resolver.py
+-rw-r--r--   0        0        0     7143 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/types.py
+-rw-r--r--   0        0        0        0 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/utils/__init__.py
+-rw-r--r--   0        0        0     2033 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/utils/inspect.py
+-rw-r--r--   0        0        0      662 2023-05-10 20:26:55.031211 strawberry_resources-0.5.0/strawberry_resources/utils/pyutils.py
+-rw-r--r--   0        0        0    10950 1970-01-01 00:00:00.000000 strawberry_resources-0.5.0/PKG-INFO
```

### Comparing `strawberry_resources-0.4.3/LICENSE` & `strawberry_resources-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/README.md` & `strawberry_resources-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/pyproject.toml` & `strawberry_resources-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-resources"
-version = "0.4.3"
+version = "0.5.0"
 description = "Introspection utilities to extract data from strawberry graphql"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-resources"
 repository = "https://github.com/blb-ventures/strawberry-resources"
 documentation = "https://github.com/blb-ventures/strawberry-resources"
```

### Comparing `strawberry_resources-0.4.3/strawberry_resources/__init__.py` & `strawberry_resources-0.5.0/strawberry_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/strawberry_resources/cli/export.py` & `strawberry_resources-0.5.0/strawberry_resources/cli/export.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/strawberry_resources/exporter.py` & `strawberry_resources-0.5.0/strawberry_resources/exporter.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/strawberry_resources/integrations/base.py` & `strawberry_resources-0.5.0/strawberry_resources/integrations/base.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/strawberry_resources/integrations/django.py` & `strawberry_resources-0.5.0/strawberry_resources/integrations/django.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,56 +115,64 @@
         FieldOptionsConfig,
         HiddenField,
         HiddenFieldError,
         StringFieldValidation,
     )
 
     options: FieldOptions = {}
+    if (
+        relay is not None
+        and isinstance(resolved_type, type)
+        and issubclass(resolved_type, relay.GlobalID)
+    ):
+        options["kind"] = FieldKind.ID
 
-    if (dj_type := _get_django_type(origin)) is None:
-        return {}
-
-    model = dj_type.model
-    model_attr = getattr(model, field.name, None)
+    if (dj_type := _get_django_type(origin)) is not None:
+        model = dj_type.model
+        model_attr = getattr(model, field.name, None)
+    else:
+        model = None
+        model_attr = None
 
     # Try to populate options from the model property
     if (
         ModelProperty is not None
+        and model_attr is not None
         and isinstance(model_attr, ModelProperty)
         and (get_origin(annotation := model_attr.func.__annotations__.get("return")) is Annotated)
     ):
         for opt in get_args(annotation)[1:]:
             if isinstance(opt, HiddenField):
                 raise HiddenFieldError
 
             if not isinstance(opt, FieldOptionsConfig):
                 continue
 
             options.update(opt.options)
 
-    dj_field = _get_model_field(model, field.name)
+    dj_field = _get_model_field(model, field.name) if model is not None else None
 
     if hasattr(resolved_type, "_type_definition"):
         field_obj_options: FieldObjectOptions = {}
 
         assert isinstance(resolved_type, type)
         if ListInput is not None and issubclass(resolved_type, ListInput):
             assert isinstance(K, TypeVar)
             field_obj_options["obj_kind"] = FieldObjectKind.LIST_INPUT
 
         label = options.get("label")
-        if label is None:
+        if label is None and dj_field is not None:
             label = getattr(dj_field, "verbose_name", None)
         if label is not None:
             field_obj_options["label"] = label
 
         return field_obj_options
 
     if dj_field is None:
-        return {}
+        return options
 
     choices: Optional[List[FieldChoice]] = None
     default_value = v if (v := getattr(dj_field, "default", None)) is not NOT_PROVIDED else None
     if isinstance(resolved_type, type) and issubclass(resolved_type, models.Choices):
         if choices is None:
             choices = [
                 FieldChoice(label=lbl, value=cast(JSON, value))
@@ -195,17 +203,17 @@
 
     if (label := getattr(dj_field, "verbose_name", None) or None) is not None:
         options["label"] = label
 
     if (help_text := getattr(dj_field, "help_Text", None) or None) is not None:
         options["help_text"] = help_text
 
-    if (order := dj_type.order) and order is not UNSET:
+    if dj_type and (order := dj_type.order) and order is not UNSET:
         options["orderable"] = field.name in {f.name for f in dataclasses.fields(cast(type, order))}
-    if (filters := dj_type.filters) and filters is not UNSET:
+    if dj_type and (filters := dj_type.filters) and filters is not UNSET:
         options["filterable"] = field.name in {
             f.name for f in dataclasses.fields(cast(type, filters))
         }
 
     if isinstance(dj_field, models.ImageField):
         options["kind"] = FieldKind.IMAGE
     elif isinstance(dj_field, models.FileField):
```

### Comparing `strawberry_resources-0.4.3/strawberry_resources/queries.py` & `strawberry_resources-0.5.0/strawberry_resources/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/strawberry_resources/resolver.py` & `strawberry_resources-0.5.0/strawberry_resources/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,16 @@
             continue
 
         is_list: bool = False
         while isinstance(f_type, StrawberryContainer):
             is_list = is_list or isinstance(f_type, StrawberryList)
             f_type = f_type.of_type
 
+        options["multiple"] = is_list
+
         if isinstance(f_type, LazyType):
             f_type = f_type.resolve_type()
         if isinstance(f_type, EnumDefinition):
             if all(isinstance(v.value, int) for v in f_type.values):
                 options["kind"] = FieldKind.INT
             elif all(isinstance(v.value, str) for v in f_type.values):
                 options["kind"] = FieldKind.STRING
@@ -206,15 +208,20 @@
             if obj_kind is None:
                 obj_kind_map: Dict[Tuple[bool, bool], FieldObjectKind] = {
                     (False, False): FieldObjectKind.OBJECT,
                     (True, False): FieldObjectKind.OBJECT_LIST,
                     (True, True): FieldObjectKind.INPUT_LIST,
                     (False, True): FieldObjectKind.INPUT,
                 }
-                obj_kind = obj_kind_map[(is_list, getattr(inner_type_def, "is_input", False))]
+                obj_kind = obj_kind_map[
+                    (
+                        options.get("multiple", False),
+                        getattr(inner_type_def, "is_input", False),
+                    )
+                ]
 
             yield FieldObject(
                 name=cname,
                 label=options.get("label", field.name),
                 obj_kind=obj_kind,
                 obj_type=inner_type_def.name,
                 fields=list(resolve_fields_for_type(f_type, depth=depth + 1)),
```

### Comparing `strawberry_resources-0.4.3/strawberry_resources/types.py` & `strawberry_resources-0.5.0/strawberry_resources/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/strawberry_resources/utils/inspect.py` & `strawberry_resources-0.5.0/strawberry_resources/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/strawberry_resources/utils/pyutils.py` & `strawberry_resources-0.5.0/strawberry_resources/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.4.3/PKG-INFO` & `strawberry_resources-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-resources
-Version: 0.4.3
+Version: 0.5.0
 Summary: Introspection utilities to extract data from strawberry graphql
 Home-page: https://github.com/blb-ventures/strawberry-resources
 License: MIT
 Keywords: strawberry,django,graphql,resources,forms
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

