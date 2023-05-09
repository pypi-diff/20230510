# Comparing `tmp/grave-settings-0.1.1.tar.gz` & `tmp/grave-settings-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grave-settings-0.1.1.tar", last modified: Wed Jan 25 17:07:58 2023, max compression
+gzip compressed data, was "grave-settings-0.1.3.tar", last modified: Tue May  9 22:28:15 2023, max compression
```

## Comparing `grave-settings-0.1.1.tar` & `grave-settings-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-25 17:07:58.130479 grave-settings-0.1.1/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5100 2023-01-25 17:07:58.130479 grave-settings-0.1.1/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4664 2023-01-13 13:51:44.000000 grave-settings-0.1.1/README.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      690 2023-01-25 17:07:58.130479 grave-settings-0.1.1/setup.cfg
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       67 2023-01-03 08:24:35.000000 grave-settings-0.1.1/setup.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-25 17:07:58.126479 grave-settings-0.1.1/src/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-25 17:07:58.130479 grave-settings-0.1.1/src/grave_settings/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       18 2023-01-25 17:07:41.000000 grave-settings-0.1.1/src/grave_settings/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5250 2023-01-25 04:09:28.000000 grave-settings-0.1.1/src/grave_settings/abstract.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6871 2023-01-25 05:01:03.000000 grave-settings-0.1.1/src/grave_settings/base.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     9079 2023-01-25 15:48:28.000000 grave-settings-0.1.1/src/grave_settings/config_file.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3131 2023-01-25 16:21:09.000000 grave-settings-0.1.1/src/grave_settings/conversion_manager.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    12824 2023-01-25 01:06:29.000000 grave-settings-0.1.1/src/grave_settings/default_handlers.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    24161 2023-01-25 16:05:22.000000 grave-settings-0.1.1/src/grave_settings/formatter.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6850 2023-01-25 02:09:17.000000 grave-settings-0.1.1/src/grave_settings/formatter_settings.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-25 17:07:58.130479 grave-settings-0.1.1/src/grave_settings/formatters/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-01-10 10:00:38.000000 grave-settings-0.1.1/src/grave_settings/formatters/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1328 2023-01-22 02:38:48.000000 grave-settings-0.1.1/src/grave_settings/formatters/bson.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      668 2023-01-22 02:25:37.000000 grave-settings-0.1.1/src/grave_settings/formatters/json.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1081 2023-01-25 01:06:59.000000 grave-settings-0.1.1/src/grave_settings/formatters/toml.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      977 2023-01-22 19:34:40.000000 grave-settings-0.1.1/src/grave_settings/framestack_context.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     7924 2023-01-25 01:05:01.000000 grave-settings-0.1.1/src/grave_settings/handlers.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1548 2023-01-19 20:54:39.000000 grave-settings-0.1.1/src/grave_settings/helper_objects.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    13217 2023-01-25 02:09:17.000000 grave-settings-0.1.1/src/grave_settings/semantics.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3099 2023-01-23 06:16:10.000000 grave-settings-0.1.1/src/grave_settings/utilities.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-25 17:07:58.130479 grave-settings-0.1.1/src/grave_settings/utils/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2023-01-13 13:52:44.000000 grave-settings-0.1.1/src/grave_settings/utils/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3387 2023-01-07 14:11:28.000000 grave-settings-0.1.1/src/grave_settings/validation.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-01-25 17:07:58.130479 grave-settings-0.1.1/src/grave_settings.egg-info/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5100 2023-01-25 17:07:58.000000 grave-settings-0.1.1/src/grave_settings.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      912 2023-01-25 17:07:58.000000 grave-settings-0.1.1/src/grave_settings.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-01-25 17:07:58.000000 grave-settings-0.1.1/src/grave_settings.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       41 2023-01-25 17:07:58.000000 grave-settings-0.1.1/src/grave_settings.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       15 2023-01-25 17:07:58.000000 grave-settings-0.1.1/src/grave_settings.egg-info/top_level.txt
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.385882 grave-settings-0.1.3/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1071 2023-02-15 04:33:38.000000 grave-settings-0.1.3/LICENSE
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     5580 2023-05-09 22:28:15.385882 grave-settings-0.1.3/PKG-INFO
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     5122 2023-02-15 04:33:38.000000 grave-settings-0.1.3/README.md
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      690 2023-05-09 22:28:15.385882 grave-settings-0.1.3/setup.cfg
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       67 2023-02-15 04:33:38.000000 grave-settings-0.1.3/setup.py
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.382548 grave-settings-0.1.3/src/
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.382548 grave-settings-0.1.3/src/grave_settings/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       18 2023-05-09 22:25:55.000000 grave-settings-0.1.3/src/grave_settings/__init__.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     5229 2023-05-02 00:14:49.000000 grave-settings-0.1.3/src/grave_settings/abstract.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     6220 2023-05-02 00:57:12.000000 grave-settings-0.1.3/src/grave_settings/base.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    10636 2023-05-08 21:21:57.000000 grave-settings-0.1.3/src/grave_settings/config_file.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     3715 2023-05-01 23:21:15.000000 grave-settings-0.1.3/src/grave_settings/conversion_manager.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    13209 2023-05-02 00:14:49.000000 grave-settings-0.1.3/src/grave_settings/default_handlers.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    24288 2023-05-01 23:21:15.000000 grave-settings-0.1.3/src/grave_settings/formatter.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     6850 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatter_settings.py
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.385882 grave-settings-0.1.3/src/grave_settings/formatters/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatters/__init__.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1328 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatters/bson.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      668 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatters/json.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1081 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/formatters/toml.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      977 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/framestack_context.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     7918 2023-05-02 00:22:48.000000 grave-settings-0.1.3/src/grave_settings/handlers.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1548 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/helper_objects.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)    13217 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/semantics.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     3099 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/utilities.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     3387 2023-02-15 04:33:38.000000 grave-settings-0.1.3/src/grave_settings/validation.py
+drwxr-xr-x   0 ryan      (1000) ryan      (1000)        0 2023-05-09 22:28:15.385882 grave-settings-0.1.3/src/grave_settings.egg-info/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     5580 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/PKG-INFO
+-rw-r--r--   0 ryan      (1000) ryan      (1000)      883 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        1 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       41 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/requires.txt
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       15 2023-05-09 22:28:15.000000 grave-settings-0.1.3/src/grave_settings.egg-info/top_level.txt
```

### Comparing `grave-settings-0.1.1/PKG-INFO` & `grave-settings-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: grave-settings
-Version: 0.1.1
+Version: 0.1.3
 Summary: A library for automatic serialization of python object hierarchies to storage
 Home-page: https://github.com/ILikesCaviar/GraveSettings
 Author: Ryan McConnell
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Grave Settings
 
 A library for automatic serialization of python object hierarchies to storage. Most python objects are 
 compatible without any extra code, and there are several tools for fine-grain control.
 
 The framework uses either duck typing or strong typing to allow objects define custom behaviors and defines a Formatter 
@@ -21,39 +22,49 @@
 Pre-defined formats:
 - json (via built in json module)
 - toml (read via tomlib, write enabled when tomli-w module is installed)
 - bson (only tested experimentally)
 
 Red the [documenation](https://ilikescaviar.github.io/GraveSettings/) for examples and important considerations.
 
+## Install
+
+```
+pip install grave-settings
+```
+
 ## Features
 
 - Save / Import types to reconstruct object hierarchies
 - Preserve "is" relationships automatically by scanning object ids
 - Abstractions for object version management for easing continuous deployment
 - OrderedHandler objects allow for custom serialization / deserialization logic for types without using inheritance or duck typing
 - Detect circular references
 - Event handlers for finalizing serialization / deserialization (intended to fix circular references)
 - Semantic objects for communicating options to the formatter (ex. security options for loading of arbitrary types)
 
 <details><summary>Default standard handlers</summary>
 <p>
 Defining new handlers or adding functionality to the default handlers is easy, but some types have already been done:
 
-| Name         | Description                                                  |
-|--------------|--------------------------------------------------------------|
-| Type         | built-in python type object                                  |
-| NoneType     | None                                                         |
-| Iterable     | General catch all for Iterable defined in collections module |
-| Mapping      | General catch all for Mapping defined in collections module  |
-| FunctionType | Python user-defined function                                 |
-| date         | from datetime module                                         |
-| datetime     | from datetime module                                         |
-| timedelta    | from datetime module                                         |
-| Enum         | from enum module                                             |
+| Name               | Description                                                  |
+|--------------------|--------------------------------------------------------------|
+| Type               | built-in python type object                                  |
+| NoneType           | None                                                         |
+| Iterable           | General catch all for Iterable defined in collections module |
+| Mapping            | General catch all for Mapping defined in collections module  |
+| FunctionType       | Python user-defined function                                 |
+| date               | from datetime module                                         |
+| datetime           | from datetime module  (experimental timezone support)        |
+| timedelta          | from datetime module                                         |
+| Enum               | from enum module                                             |
+| partial            | builtin partial class                                        |
+| bytes              | builtin bytes data                                           |
+| Complex / Rational | builtin numerical classes                                    |
+| Path               | from pathlib                                                 |
 
 There is still a ways to go before most of the built in types have handlers. To see how the handlers work read:
 [default_handlers.py](src/grave_settings/default_handlers.py)
 
 </p>
 </details>
```

### Comparing `grave-settings-0.1.1/README.md` & `grave-settings-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,39 +9,49 @@
 Pre-defined formats:
 - json (via built in json module)
 - toml (read via tomlib, write enabled when tomli-w module is installed)
 - bson (only tested experimentally)
 
 Red the [documenation](https://ilikescaviar.github.io/GraveSettings/) for examples and important considerations.
 
+## Install
+
+```
+pip install grave-settings
+```
+
 ## Features
 
 - Save / Import types to reconstruct object hierarchies
 - Preserve "is" relationships automatically by scanning object ids
 - Abstractions for object version management for easing continuous deployment
 - OrderedHandler objects allow for custom serialization / deserialization logic for types without using inheritance or duck typing
 - Detect circular references
 - Event handlers for finalizing serialization / deserialization (intended to fix circular references)
 - Semantic objects for communicating options to the formatter (ex. security options for loading of arbitrary types)
 
 <details><summary>Default standard handlers</summary>
 <p>
 Defining new handlers or adding functionality to the default handlers is easy, but some types have already been done:
 
-| Name         | Description                                                  |
-|--------------|--------------------------------------------------------------|
-| Type         | built-in python type object                                  |
-| NoneType     | None                                                         |
-| Iterable     | General catch all for Iterable defined in collections module |
-| Mapping      | General catch all for Mapping defined in collections module  |
-| FunctionType | Python user-defined function                                 |
-| date         | from datetime module                                         |
-| datetime     | from datetime module                                         |
-| timedelta    | from datetime module                                         |
-| Enum         | from enum module                                             |
+| Name               | Description                                                  |
+|--------------------|--------------------------------------------------------------|
+| Type               | built-in python type object                                  |
+| NoneType           | None                                                         |
+| Iterable           | General catch all for Iterable defined in collections module |
+| Mapping            | General catch all for Mapping defined in collections module  |
+| FunctionType       | Python user-defined function                                 |
+| date               | from datetime module                                         |
+| datetime           | from datetime module  (experimental timezone support)        |
+| timedelta          | from datetime module                                         |
+| Enum               | from enum module                                             |
+| partial            | builtin partial class                                        |
+| bytes              | builtin bytes data                                           |
+| Complex / Rational | builtin numerical classes                                    |
+| Path               | from pathlib                                                 |
 
 There is still a ways to go before most of the built in types have handlers. To see how the handlers work read:
 [default_handlers.py](src/grave_settings/default_handlers.py)
 
 </p>
 </details>
```

### Comparing `grave-settings-0.1.1/setup.cfg` & `grave-settings-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/abstract.py` & `grave-settings-0.1.3/src/grave_settings/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,19 +90,19 @@
 
     @classmethod
     def get_versioning_endpoint(cls) -> Type[Self]:
         return VersionedSerializable
 
 
 def make_kill_converter(cls: Type[VersionedSerializable]) -> Callable[[dict], dict]:
-    return lambda _: cls().to_dict(explicit=True)
+    return lambda *_: cls().to_dict(None)
 
 
 class IASettings(VersionedSerializable, MutableMapping):
-    __slots__ = 'parent', '_invalidate', 'file_path'
+    __slots__ = 'parent', '_invalidate'
 
     def __init__(self, *args, initialize_settings=True, **kwargs):
         self.parent: IASettings | None = None
         if initialize_settings:
             self.init_settings(**kwargs)
 
     def init_settings(self, **kwargs) -> None:
```

### Comparing `grave-settings-0.1.1/src/grave_settings/base.py` & `grave-settings-0.1.3/src/grave_settings/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # - * -coding: utf - 8 - * -
 """
 
 
 @author: ☙ Ryan McConnell ❧
 """
 from typing import Mapping, Generator, Type
+from abc import ABCMeta
 
 from ordered_set import OrderedSet
 from grave_settings.utilities import unwrap_slots_to_base, ext_str_slots
 from grave_settings.abstract import IASettings, _KT, _VT, VersionedSerializable
 from grave_settings.formatter_settings import FormatterContext
 
 
@@ -67,78 +68,59 @@
     def generate_key_value_pairs(self, **kwargs) -> Generator[tuple[object, object], None, None]:
         yield from self.sd.items()
 
     def to_dict(self, context: FormatterContext, **kwargs) -> dict:
         return self.sd.copy()
 
 
-#rem_slot_fixed = set()
+def assemble_settings_keys_from_base(cls: Type, msub=IASettings) -> tuple:
+    try:
+        ret = object.__getattribute__(cls, 'SETTINGS_KEYS')
+        if ret is not None:  # cached
+            return ret
+    except AttributeError:
+        pass
+    keys = OrderedSet()
+    try:
+        keys.update(object.__getattribute__(cls, '__slots__'))
+    except AttributeError:
+        pass
+    for tt in cls.__bases__:
+        if tt is not msub and issubclass(tt, msub):
+            ins = OrderedSet(assemble_settings_keys_from_base(tt))
+            ins.update(keys)
+            keys = ins
+    try:
+        _slot_rems = object.__getattribute__(cls, '_slot_rems')
+        if _slot_rems is not None:
+            return tuple(k for k in keys if k not in _slot_rems)
+    except AttributeError:
+        pass
+    return tuple(keys)
+
+
+class slotsettings_meta(ABCMeta):
+    def __new__(cls, clsname, bases, attrs):
+        if '__slots__' not in attrs:
+            attrs['__slots__'] = tuple()
+        tt = super().__new__(cls, clsname, bases, attrs)
+        if hasattr(tt, 'assemble_settings_keys_from_base'):
+            settings_keys = tt.assemble_settings_keys_from_base(tt)
+        else:
+            settings_keys = assemble_settings_keys_from_base(tt)
+        setattr(tt, 'SETTINGS_KEYS', settings_keys)
+        setattr(tt, '__metaclass__', slotsettings_meta)
+        return tt
 
 
-class SlotSettings(IASettings):
+class SlotSettings(IASettings, metaclass=slotsettings_meta):
     _slot_rems = None
     __slots__ = tuple()
     SETTINGS_KEYS = None
 
-    # @classmethod
-    # def __new__(cls, *args, **kwargs):
-    #     if cls not in rem_slot_fixed:
-    #         found_slot_rems = False
-    #
-    #
-    #         slrm = set()
-    #         for tt in generate_hierarchy_to_base(SlotSettings, cls):
-    #             if hasattr(tt, '_slot_rems') and tt._slot_rems is not None:
-    #                 found_slot_rems = True
-    #                 slrm.update(tt._slot_rems)
-    #
-    #         if found_slot_rems:
-    #             cls._slot_rems = tuple(slrm)
-    #             cls.get_settings_keys = cls.get_settings_keys_rems
-    #         else:
-    #             cls.get_settings_keys = cls.get_settings_keys_base_slots
-    #         rem_slot_fixed.add(cls)
-    #
-    #    return super(SlotSettings, cls).__new__(cls)
-
-    def __init__(self):
-        cls = self.__class__
-        try:
-            object.__getattribute__(cls, 'SETTINGS_KEYS')
-        except AttributeError:
-            # this whole process is inefficient, but it only happens once so, eh
-            cls.SETTINGS_KEYS = OrderedSet(cls.assemble_settings_keys_from_base(cls))
-        super().__init__()
-
-    @staticmethod
-    def assemble_settings_keys_from_base(cls: Type) -> tuple:
-        try:
-            ret = object.__getattribute__(cls, 'SETTINGS_KEYS')
-            if ret is not None:  # cached
-                return ret
-        except AttributeError:
-            pass
-        keys = OrderedSet()
-        try:
-            keys.update(object.__getattribute__(cls, '__slots__'))
-        except AttributeError:
-            pass
-        for tt in cls.__bases__:
-            if hasattr(tt, 'assemble_settings_keys_from_base'):
-                ins = OrderedSet(tt.assemble_settings_keys_from_base(tt))
-                ins.update(keys)
-                keys = ins
-        try:
-            _slot_rems = object.__getattribute__(cls, '_slot_rems')
-            if _slot_rems is not None:
-                return tuple(k for k in keys if k not in _slot_rems)
-        except AttributeError:
-            pass
-        return tuple(keys)
-
     @classmethod
     def get_versioning_endpoint(cls) -> Type[VersionedSerializable]:
         return SlotSettings
 
     def get_settings_keys_rems(self, rems=None) -> set:
         if rems is None:
             rems = self._slot_rems
```

### Comparing `grave-settings-0.1.1/src/grave_settings/config_file.py` & `grave-settings-0.1.3/src/grave_settings/config_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 import shutil
 from datetime import datetime
 from pathlib import Path
 from typing import Self, Any, Type
 
 from observer_hooks import EventCapturer
 
-from grave_settings.utilities import format_class_str
+from grave_settings.conversion_manager import get_descendent_class_formats
+from grave_settings.utilities import format_class_str, generate_type_hierarchy_to_base
 from grave_settings.abstract import IASettings, Serializable
 from grave_settings.formatter_settings import FormatterContext
 from grave_settings.formatters.toml import TomlFormatter
 from grave_settings.formatters.json import JsonFormatter
 from grave_settings.formatter import Formatter, DeSerializer, Serializer
 from grave_settings.handlers import OrderedHandler
-from grave_settings.semantics import ClassStringPassFunction, Semantics, Semantic
+from grave_settings.semantics import ClassStringPassFunction, Semantics, Semantic, SecurityException
 
 
 class PassLogFilePath(Semantic[str]):
     pass
 
 
 class LogFileLink(Serializable):
@@ -52,31 +53,55 @@
         else:
             self.file_path = state_obj['path']
         self.config = state_obj['config']
 
 
 class ConfigFile(Serializable):
     FORMATTER_STR_DICT = {
-        'json': JsonFormatter(),
-        'toml': TomlFormatter()
+        'json': JsonFormatter,
+        'toml': TomlFormatter
     }
+    FORMATTER_PREFERRED_EXT: dict[type, str] = {
+        JsonFormatter: 'json',
+        TomlFormatter: 'toml'
+    }  # Might seem redundant but FORMATTER_STR_DICT values might not be types
 
     def __init__(self, file_path: Path, data: IASettings | Any | Type | None = None,
                  formatter: None | Formatter | str = None, auto_save=False, read_only=False):
+        if file_path is not None:
+            if formatter is None:
+                formatter = file_path.suffix.lower()
+                if formatter.startswith('.'):
+                    formatter = formatter[1:]
+            file_path = file_path.resolve().absolute()
         if type(formatter) == str:
-            formatter = self.FORMATTER_STR_DICT[formatter]
-        self.file_path = file_path.resolve().absolute()
+            formatter = self.guess_formatter_from_str(formatter)()
+        self.file_path = file_path
         self.data = data
-        self.auto_save = auto_save
+        self.save_on_invalidate = auto_save
         self.formatter = formatter
         self.changes_made = not isinstance(data, IASettings)
+        self.track_changes = self.changes_made
         self.read_only = read_only
         self.sub_configs: dict[Any, LogFileLink] = {}
         self.sub_config_paths: dict[Path, Any] = {}
 
+    def set_file_path(self, path: Path):
+        self.file_path = path
+
+    @classmethod
+    def guess_file_type(cls, formatter: Formatter):
+        for t in generate_type_hierarchy_to_base(object, formatter.__class__):
+            if t in cls.FORMATTER_PREFERRED_EXT:
+                return cls.FORMATTER_PREFERRED_EXT[t]
+
+    @classmethod
+    def guess_formatter_from_str(cls, short_name: str):
+        return cls.FORMATTER_STR_DICT[short_name]
+
     def add_config_dependency(self, other: 'ConfigFile', relative_path=True):
         if not other.is_loaded():
             raise ValueError('Only add config files after they have been loaded or set their data object properly')
         if relative_path:
             log_file_link = LogFileLink(config=other, rel_path=other.file_path.relative_to(self.file_path.parent))
         else:
             log_file_link = LogFileLink(config=other, file_path=other.file_path)
@@ -97,59 +122,61 @@
             base = self.file_path.parent
             dt_n = datetime.now().strftime('%Y_%m_%d %H%M')
             backup_path = base / f"{self.file_path.stem}_backup_{dt_n}{self.file_path.suffix}"
             shutil.copyfile(str(self.file_path), str(backup_path))
 
     def settings_invalidated(self):
         self.changes_made = True
-        if self.auto_save:
+        if self.save_on_invalidate:
             self.save()
 
-    def validate_file_path(self, path: Path, must_exist=False):
+    def validate_file_path(self, path: Path, must_exist=False, test_if_file=True):
+        if self.file_path is None:
+            raise ValueError('File path not specified')
         if must_exist:
             if not path.exists():
                 raise ValueError(f'Path does not exist: {path}')
         if path.exists() and (not os.access(path, os.R_OK)):
             raise ValueError(f'Do not have permission to write to: {path}')
         if not self.read_only:
             if path.exists() and (not os.access(path, os.W_OK)):
                 raise ValueError(f'Do not have permission to write to: {path}')
-        if path.exists() and (not path.is_file()):
+        if test_if_file and path.exists() and (not path.is_file()):
             raise ValueError(f'File path is invalid: {path}')
 
     def save(self, path: Path = None, formatter: None | Formatter = None, force=True, validate_path=True):
         if self.read_only:
             raise ValueError('Saving in read-only mode')
         if path is None:
             path = self.file_path
             vf = self.changes_made
-        elif (not force) and self.changes_made and hasattr(self.data, 'invalidate'):
+        elif (not force) and (not self.changes_made) and self.track_changes:
             return
         else:
             vf = False
         if validate_path:
             self.validate_file_path(path)
         if formatter is None:
             formatter = self.formatter
         if formatter is None:
             raise ValueError('No formatter supplied')
         serializer = self.formatter.get_serializer(self.data, self.get_serialization_context())
-        serializer.handler.type_bank[object] = self.handle_serialize_IASettings
+        serializer.handler.type_bank[object] = self.handle_serialize_object
         #serializer.handler.add_handler(IASettings, self.handle_serialize_IASettings)
         formatter.write_to_file(self.data, str(self.file_path), serializer=serializer)
         self.changes_made = vf
 
     @classmethod
     def check_in_serialization_context(cls, context: FormatterContext):
         pass
 
     def get_serialization_context(self):
         return self.formatter.get_serialization_context()
 
-    def handle_serialize_IASettings(self, serializer: Serializer, obj: IASettings, **kwargs):
+    def handle_serialize_object(self, serializer: Serializer, obj: IASettings, **kwargs):
         if obj in self.sub_configs:
             link = self.sub_configs[obj]
             link.config.save()
             return serializer.handle_default(link)
         else:
             return serializer.handle_default(obj, **kwargs)
 
@@ -167,28 +194,34 @@
         deserializer.secondary_handler.add_handler(LogFileLink, self.handle_deserialize_LogFileLink)
         if semantics is not None:
             context.semantic_context.semantics.update(semantics)
         with EventCapturer(deserializer.notify_settings_converted) as capture:
             self.data = formatter.read_from_file(str(path), deserializer=deserializer)
         if len(capture) > 0:
             self.backup_settings_file()
-        if isinstance(self.data, IASettings):
-            self.data.file_path = self.file_path
         self.changes_made = False
 
     @classmethod
     def check_in_deserialization_context(cls, context: FormatterContext):
         handler = OrderedHandler()
         handler.add_handler(ConfigFile, cls.handle_me)
         context.semantic_context.set_handler(handler, update_order=True)
 
     def get_deserialization_context(self):
         context = self.formatter.get_deserialization_context()
+        found_init = False
+        def descriptive_error(class_string: str):
+            if class_string in format_class_str(self.data):
+                return True
+            elif found_init:
+                if class_string in get_descendent_class_formats(self.data):  # TODO: This is not functional
+                    return True
+            raise SecurityException(f'{class_string} does not match correct class string {format_class_str(self.data)}')
         if isinstance(self.data, type):
-            context.add_frame_semantics(ClassStringPassFunction(lambda x: x == format_class_str(self.data)))
+            context.add_frame_semantics(ClassStringPassFunction(descriptive_error))
         return context
 
     def handle_deserialize_LogFileLink(self, deserializer: DeSerializer, obj: LogFileLink, **kwargs):
         if obj.file_path is not None:
             obj.config.file_path = obj.file_path.absolute()
         else:
             obj.config.file_path = obj.rel_path.absolute()
@@ -208,15 +241,15 @@
         if load:
             self.load(validate_path=False)
         elif isinstance(self.data, type):
             self.data = self.instantiate_data()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        if not self.read_only:
+        if self.file_path is not None and not self.read_only:
             self.save()
 
     def get_load_data_obj(self):
         if not self.is_loaded():
             self.load()
         return self.data
```

### Comparing `grave-settings-0.1.1/src/grave_settings/conversion_manager.py` & `grave-settings-0.1.3/src/grave_settings/conversion_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,29 @@
     new_json_obj = {}
     for k, v in mapping.items():
         if k in json_obj:
             new_json_obj[mapping[k]] = json_obj[k]
     return new_json_obj
 
 
+def get_object_versioning_endpoint(t_obj: Type | object):
+    if hasattr(t_obj, 'get_versioning_endpoint'):
+        return t_obj.get_versioning_endpoint()
+    else:
+        return object
+
+
+def get_descendent_class_formats(t_obj: Type | object, end_point=None) -> set[Type]:
+    if end_point is None:
+        end_point = get_object_versioning_endpoint(t_obj)
+    if not isinstance(t_obj, type):  # meta-classes force use of isinstance for Type[type] checking
+        t_obj = t_obj.__class__
+    return {format_class_str(c) for c in generate_type_hierarchy_to_base(end_point, t_obj)}
+
+
 class ConversionManager:
     __slots__ = 'converters', 'converted'
 
     def __init__(self):
         # mapping of version to tuple of conversion function and output version
         self.converters: dict[tuple[str, str], tuple[Callable, str]] = {}
         self.converted = EventHandler()
```

### Comparing `grave-settings-0.1.1/src/grave_settings/default_handlers.py` & `grave-settings-0.1.3/src/grave_settings/default_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from zoneinfo import ZoneInfo
 
 from observer_hooks import FunctionStub, EventHandler
 from grave_settings.utilities import get_type_hints, format_class_str, load_type, T
 
 from grave_settings.formatter_settings import Temporary, PreservedReference, FormatterContext, NoRef
 from grave_settings.handlers import OrderedHandler
-from grave_settings.abstract import Serializable
+from grave_settings.abstract import Serializable, IASettings
 from grave_settings.framestack_context import FrameStackContext
 from grave_settings.helper_objects import KeySerializableDict
 from grave_settings.semantics import *
 
 
-def force_instantiate(type_obj: Type[T]) -> T:
+def force_instantiate(type_obj: Type[T], *args, **kwargs) -> T:
     try:
-        return type_obj()
+        return type_obj(*args, **kwargs)
     except TypeError:
         return type_obj.__new__(type_obj)
 
 
 class NotSerializableException(Exception):
     pass
 
@@ -225,14 +225,15 @@
             NoneType: self.handle_NoneType,
             tuple: self.handle_tuple,
             set: self.handle_set,
             PreservedReference: self.handle_PreservedReference,
             FunctionType: self.handle_type,
             MethodType: self.handle_method,
             Serializable: self.handle_serializable,
+            IASettings: self.handle_iasettings,
             KeySerializableDict: self.handle_KeySerializableDict,
             date: self.handle_date,
             datetime: self.handle_datetime,
             timedelta: self.handle_timedelta,
             Enum: self.handle_Enum,
             partial: self.handle_partial,
             bytes: self.handle_bytes,
@@ -307,14 +308,20 @@
     @staticmethod
     def handle_serializable(t_object: Type[Serializable], json_obj: dict, context: FormatterContext, **kwargs) -> Serializable:
         settings_obj = force_instantiate(t_object)
         settings_obj.from_dict(json_obj, context, **kwargs)
         return settings_obj
 
     @staticmethod
+    def handle_iasettings(t_object: Type[IASettings], json_obj: dict, context: FormatterContext, **kwargs):
+        settings_obj = force_instantiate(t_object, initialize_settings=False)
+        settings_obj.from_dict(json_obj, context, **kwargs)
+        return settings_obj
+
+    @staticmethod
     def handle_datetime(t_object: Type[datetime], json_obj: dict, context: FormatterContext, **kwargs) -> datetime:
         obs = json_obj['state']
 
         tz1 = None
         total_secs = None
         if 'timezone' in json_obj:
             tz1 = ZoneInfo(json_obj['timezone'])
```

### Comparing `grave-settings-0.1.1/src/grave_settings/formatter.py` & `grave-settings-0.1.3/src/grave_settings/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,17 +456,18 @@
                 instance[k] = v
             else:
                 with self.context(k), self.semantics:
                     instance[k] = self.deserialize(v, **kwargs)
 
         if class_id is not None:
             if ducks and (version_info is not None) and hasattr(type_obj, 'check_convert_update'):
-                if ti := type_obj.check_convert_update(instance, self.context.load_type, version_info):
-                    instance = ti
-                    self.notify_settings_converted(class_id)
+                with self.semantics:  # TODO: The version info messes up SecurityException semantics (more needed)
+                    if ti := type_obj.check_convert_update(instance, self.context.load_type, version_info):
+                        instance = ti
+                        self.notify_settings_converted(class_id)
             ret = self.context.handler.handle_node(type_obj, instance, self.context, **kwargs)
             if method_name := self.semantics[NotifyFinalizedMethodName]:
                 self.context.finalize.subscribe(getattr(ret, method_name.val))
             return ret
         else:
             return instance
```

### Comparing `grave-settings-0.1.1/src/grave_settings/formatter_settings.py` & `grave-settings-0.1.3/src/grave_settings/formatter_settings.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/formatters/bson.py` & `grave-settings-0.1.3/src/grave_settings/formatters/bson.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/formatters/json.py` & `grave-settings-0.1.3/src/grave_settings/formatters/json.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/formatters/toml.py` & `grave-settings-0.1.3/src/grave_settings/formatters/toml.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/framestack_context.py` & `grave-settings-0.1.3/src/grave_settings/framestack_context.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/handlers.py` & `grave-settings-0.1.3/src/grave_settings/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,24 +155,22 @@
         f = self.get_key_func(key.__class__)
         return f(pass_self, key, *args, **kwargs)
 
     def handle(self, pass_self, instance, *args, **kwargs):
         return self.handle_node(pass_self, instance, *args, **kwargs)
 
 
-
 MHS = Callable[[object, T, ...], T]
 
 
 class MroHandler(Handler):
     def __init__(self, *args, **kwargs):
         super(MroHandler, self).__init__(*args, **kwargs)
-        self.type_bank: dict[Type, MHS] = {}
+        self.type_bank: dict[Type, MHS] = self.type_bank
         self.cache: dict[Type, tuple[MHS]] = {}
-
     def update(self, handler: Handler):
         super(MroHandler, self).update(handler)
         self.cache = {}
 
     def add_handler(self, target_type, func_format, bind_as_method=False, clear_cache=True):
         if bind_as_method:
             func_format = MethodType(func_format, self)
@@ -185,15 +183,15 @@
 
     def get_ordered_handlers(self, key):
         if key in self.cache:
             return self.cache[key]
         else:
             bs = tuple(self.type_bank[tt] for tt in reversed(key.__mro__) if tt in self.type_bank)
             if len(bs) <= 0:
-                bs = (self.default_handler,)
+                bs = tuple()
             self.cache[key] = bs
             return bs
 
     def handle(self, instance, *args, **kwargs):
         return self.handle_custom(instance.__class__, instance, None,  *args, **kwargs)
 
     def __contains__(self, item: Type):
```

### Comparing `grave-settings-0.1.1/src/grave_settings/helper_objects.py` & `grave-settings-0.1.3/src/grave_settings/helper_objects.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/semantics.py` & `grave-settings-0.1.3/src/grave_settings/semantics.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/utilities.py` & `grave-settings-0.1.3/src/grave_settings/utilities.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings/validation.py` & `grave-settings-0.1.3/src/grave_settings/validation.py`

 * *Files identical despite different names*

### Comparing `grave-settings-0.1.1/src/grave_settings.egg-info/PKG-INFO` & `grave-settings-0.1.3/src/grave_settings.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: grave-settings
-Version: 0.1.1
+Version: 0.1.3
 Summary: A library for automatic serialization of python object hierarchies to storage
 Home-page: https://github.com/ILikesCaviar/GraveSettings
 Author: Ryan McConnell
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Grave Settings
 
 A library for automatic serialization of python object hierarchies to storage. Most python objects are 
 compatible without any extra code, and there are several tools for fine-grain control.
 
 The framework uses either duck typing or strong typing to allow objects define custom behaviors and defines a Formatter 
@@ -21,39 +22,49 @@
 Pre-defined formats:
 - json (via built in json module)
 - toml (read via tomlib, write enabled when tomli-w module is installed)
 - bson (only tested experimentally)
 
 Red the [documenation](https://ilikescaviar.github.io/GraveSettings/) for examples and important considerations.
 
+## Install
+
+```
+pip install grave-settings
+```
+
 ## Features
 
 - Save / Import types to reconstruct object hierarchies
 - Preserve "is" relationships automatically by scanning object ids
 - Abstractions for object version management for easing continuous deployment
 - OrderedHandler objects allow for custom serialization / deserialization logic for types without using inheritance or duck typing
 - Detect circular references
 - Event handlers for finalizing serialization / deserialization (intended to fix circular references)
 - Semantic objects for communicating options to the formatter (ex. security options for loading of arbitrary types)
 
 <details><summary>Default standard handlers</summary>
 <p>
 Defining new handlers or adding functionality to the default handlers is easy, but some types have already been done:
 
-| Name         | Description                                                  |
-|--------------|--------------------------------------------------------------|
-| Type         | built-in python type object                                  |
-| NoneType     | None                                                         |
-| Iterable     | General catch all for Iterable defined in collections module |
-| Mapping      | General catch all for Mapping defined in collections module  |
-| FunctionType | Python user-defined function                                 |
-| date         | from datetime module                                         |
-| datetime     | from datetime module                                         |
-| timedelta    | from datetime module                                         |
-| Enum         | from enum module                                             |
+| Name               | Description                                                  |
+|--------------------|--------------------------------------------------------------|
+| Type               | built-in python type object                                  |
+| NoneType           | None                                                         |
+| Iterable           | General catch all for Iterable defined in collections module |
+| Mapping            | General catch all for Mapping defined in collections module  |
+| FunctionType       | Python user-defined function                                 |
+| date               | from datetime module                                         |
+| datetime           | from datetime module  (experimental timezone support)        |
+| timedelta          | from datetime module                                         |
+| Enum               | from enum module                                             |
+| partial            | builtin partial class                                        |
+| bytes              | builtin bytes data                                           |
+| Complex / Rational | builtin numerical classes                                    |
+| Path               | from pathlib                                                 |
 
 There is still a ways to go before most of the built in types have handlers. To see how the handlers work read:
 [default_handlers.py](src/grave_settings/default_handlers.py)
 
 </p>
 </details>
```

### Comparing `grave-settings-0.1.1/src/grave_settings.egg-info/SOURCES.txt` & `grave-settings-0.1.3/src/grave_settings.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 src/grave_settings/__init__.py
 src/grave_settings/abstract.py
 src/grave_settings/base.py
 src/grave_settings/config_file.py
@@ -19,9 +20,8 @@
 src/grave_settings.egg-info/SOURCES.txt
 src/grave_settings.egg-info/dependency_links.txt
 src/grave_settings.egg-info/requires.txt
 src/grave_settings.egg-info/top_level.txt
 src/grave_settings/formatters/__init__.py
 src/grave_settings/formatters/bson.py
 src/grave_settings/formatters/json.py
-src/grave_settings/formatters/toml.py
-src/grave_settings/utils/__init__.py
+src/grave_settings/formatters/toml.py
```

