# Comparing `tmp/tyro-0.5.1.tar.gz` & `tmp/tyro-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyro-0.5.1.tar", max compression
+gzip compressed data, was "tyro-0.5.2.tar", max compression
```

## Comparing `tyro-0.5.1.tar` & `tyro-0.5.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1065 2023-05-05 21:00:12.706733 tyro-0.5.1/LICENSE
--rw-r--r--   0        0        0     4445 2023-05-05 21:02:11.568767 tyro-0.5.1/README.md
--rw-r--r--   0        0        0     1866 2023-05-05 21:00:12.706733 tyro-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      406 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/__init__.py
--rw-r--r--   0        0        0    22530 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_argparse_formatter.py
--rw-r--r--   0        0        0    19510 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_arguments.py
--rw-r--r--   0        0        0     8697 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_calling.py
--rw-r--r--   0        0        0    15642 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_cli.py
--rw-r--r--   0        0        0      101 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_deprecated.py
--rw-r--r--   0        0        0    11749 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_docstrings.py
--rw-r--r--   0        0        0    30130 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_fields.py
--rw-r--r--   0        0        0    23100 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_instantiators.py
--rw-r--r--   0        0        0    21122 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_parsers.py
--rw-r--r--   0        0        0    11374 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_resolver.py
--rw-r--r--   0        0        0      383 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_singleton.py
--rw-r--r--   0        0        0     4949 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_strings.py
--rw-r--r--   0        0        0     3793 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_subcommand_matching.py
--rw-r--r--   0        0        0      764 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_typing.py
--rw-r--r--   0        0        0     1206 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/_unsafe_cache.py
--rw-r--r--   0        0        0      921 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/conf/__init__.py
--rw-r--r--   0        0        0     1998 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/conf/_confstruct.py
--rw-r--r--   0        0        0     5478 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/conf/_markers.py
--rw-r--r--   0        0        0      579 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/extras/__init__.py
--rw-r--r--   0        0        0     2055 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/extras/_base_configs.py
--rw-r--r--   0        0        0     1129 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/extras/_choices_type.py
--rw-r--r--   0        0        0     8196 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/extras/_serialization.py
--rw-r--r--   0        0        0        0 2023-05-05 21:00:12.710733 tyro-0.5.1/tyro/py.typed
--rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 tyro-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-10 07:27:30.566393 tyro-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4445 2023-05-10 07:29:30.531699 tyro-0.5.2/README.md
+-rw-r--r--   0        0        0     1866 2023-05-10 07:27:30.570393 tyro-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/__init__.py
+-rw-r--r--   0        0        0    22530 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_argparse_formatter.py
+-rw-r--r--   0        0        0    19335 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_arguments.py
+-rw-r--r--   0        0        0     8560 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_calling.py
+-rw-r--r--   0        0        0    15642 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_cli.py
+-rw-r--r--   0        0        0      101 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_deprecated.py
+-rw-r--r--   0        0        0    11749 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_docstrings.py
+-rw-r--r--   0        0        0    30130 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_fields.py
+-rw-r--r--   0        0        0    23100 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_instantiators.py
+-rw-r--r--   0        0        0    21122 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_parsers.py
+-rw-r--r--   0        0        0    11374 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_resolver.py
+-rw-r--r--   0        0        0      383 2023-05-10 07:27:30.570393 tyro-0.5.2/tyro/_singleton.py
+-rw-r--r--   0        0        0     4949 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/_strings.py
+-rw-r--r--   0        0        0     3793 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/_subcommand_matching.py
+-rw-r--r--   0        0        0      764 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/_typing.py
+-rw-r--r--   0        0        0     1206 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/_unsafe_cache.py
+-rw-r--r--   0        0        0     1083 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/conf/__init__.py
+-rw-r--r--   0        0        0     1998 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/conf/_confstruct.py
+-rw-r--r--   0        0        0     5781 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/conf/_markers.py
+-rw-r--r--   0        0        0      579 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/extras/__init__.py
+-rw-r--r--   0        0        0     2055 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/extras/_base_configs.py
+-rw-r--r--   0        0        0     1129 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/extras/_choices_type.py
+-rw-r--r--   0        0        0     8196 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/extras/_serialization.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:27:30.574393 tyro-0.5.2/tyro/py.typed
+-rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 tyro-0.5.2/PKG-INFO
```

### Comparing `tyro-0.5.1/LICENSE` & `tyro-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/README.md` & `tyro-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/pyproject.toml` & `tyro-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tyro"
-version = "0.5.1"
+version = "0.5.2"
 description = "Strongly typed, zero-effort CLI interfaces"
 authors = ["brentyi <brentyi@berkeley.edu>"]
 include = ["./tyro/**/*"]
 readme = "README.md"
 repository = "https://github.com/brentyi/tyro"
 homepage = "https://github.com/brentyi/tyro"
 documentation = "https://brentyi.github.io/tyro/"
```

### Comparing `tyro-0.5.1/tyro/_argparse_formatter.py` & `tyro-0.5.2/tyro/_argparse_formatter.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_arguments.py` & `tyro-0.5.2/tyro/_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,19 +130,16 @@
             kwargs["default"] = []
 
         # Apply overrides in our arg configuration object.
         # Note that the `name` field is applied when the field object is instantiated!
         if self.field.argconf.metavar is not None:
             kwargs["metavar"] = self.field.argconf.metavar
 
-        # Add argument! Note that the name must be passed in as a position argument.
-        try:
-            arg = parser.add_argument(name_or_flag, **kwargs)
-        except argparse.ArgumentError:
-            return
+        # Add argument!
+        arg = parser.add_argument(name_or_flag, **kwargs)
 
         # Do our best to tab complete paths.
         # There will be false positives here, but if choices is unset they should be
         # harmless.
         if "choices" not in kwargs:
             name_suggests_dir = (
                 # The conditions are intended to be conservative; if a directory path is
@@ -453,14 +450,15 @@
 def _rule_set_name_or_flag_and_dest(
     arg: ArgumentDefinition,
     lowered: LoweredArgumentDefinition,
 ) -> LoweredArgumentDefinition:
     name_or_flag = _strings.make_field_name(
         [arg.name_prefix, arg.field.name]
         if arg.field.argconf.prefix_name
+        and _markers.OmitArgPrefixes not in arg.field.markers
         else [arg.field.name]
     )
 
     # Prefix keyword arguments with --.
     if not arg.field.is_positional():
         name_or_flag = "--" + name_or_flag
 
@@ -471,19 +469,15 @@
         assert name_or_flag.startswith(strip_prefix)
         if _markers.OmitSubcommandPrefixes in arg.field.markers:
             name_or_flag = "--" + name_or_flag[len(strip_prefix) :]
 
     return dataclasses.replace(
         lowered,
         name_or_flag=name_or_flag,
-        dest=(
-            _strings.make_field_name([arg.dest_prefix, arg.field.name])
-            if arg.field.argconf.prefix_name
-            else arg.field.name
-        ),
+        dest=_strings.make_field_name([arg.dest_prefix, arg.field.name]),
     )
 
 
 def _rule_positional_special_handling(
     arg: ArgumentDefinition,
     lowered: LoweredArgumentDefinition,
 ) -> LoweredArgumentDefinition:
```

### Comparing `tyro-0.5.1/tyro/_calling.py` & `tyro-0.5.2/tyro/_calling.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,19 +61,15 @@
         field_type = field.typ
 
         if prefixed_field_name in arg_from_prefixed_field_name:
             assert prefixed_field_name not in consumed_keywords
 
             # Standard arguments.
             arg = arg_from_prefixed_field_name[prefixed_field_name]
-            name_maybe_prefixed = (
-                prefixed_field_name
-                if field.argconf.prefix_name
-                else _strings.make_field_name([field.name])
-            )
+            name_maybe_prefixed = prefixed_field_name
             consumed_keywords.add(name_maybe_prefixed)
             if not arg.lowered.is_fixed():
                 value = get_value_from_arg(name_maybe_prefixed)
 
                 if value in _fields.MISSING_SINGLETONS:
                     value = arg.field.default
                 else:
```

### Comparing `tyro-0.5.1/tyro/_cli.py` & `tyro-0.5.2/tyro/_cli.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_docstrings.py` & `tyro-0.5.2/tyro/_docstrings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_fields.py` & `tyro-0.5.2/tyro/_fields.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_instantiators.py` & `tyro-0.5.2/tyro/_instantiators.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_parsers.py` & `tyro-0.5.2/tyro/_parsers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_resolver.py` & `tyro-0.5.2/tyro/_resolver.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_strings.py` & `tyro-0.5.2/tyro/_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_subcommand_matching.py` & `tyro-0.5.2/tyro/_subcommand_matching.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_typing.py` & `tyro-0.5.2/tyro/_typing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/_unsafe_cache.py` & `tyro-0.5.2/tyro/_unsafe_cache.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/conf/_confstruct.py` & `tyro-0.5.2/tyro/conf/_confstruct.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/conf/_markers.py` & `tyro-0.5.2/tyro/conf/_markers.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,25 @@
 
     cmd: Union[NestedTypeA, NestedTypeB]
 
 By default, `--cmd.arg` may be generated as a flag for each dataclass in the union.
 If subcommand prefixes are omitted, we would instead simply have `--arg`.
 """
 
+OmitArgPrefixes = Annotated[T, None]
+"""Make flags used for keyword arguments in arguments shorter by omitting prefixes.
+
+If we have a structure with the field:
+
+    cmd: NestedType
+
+By default, `--cmd.arg` may be generated as a flag. If prefixes are omitted, we would
+instead simply have `--arg`.
+"""
+
 UseAppendAction = Annotated[T, None]
 """Use "append" actions for variable-length arguments.
 
 Given an annotation like `x: List[int]`, this means that `x = [0, 1, 2]` can be set via
 the CLI syntax `--x 0 --x 1 --x 2` instead of the default of `--x 0 1 2`.
 
 The resulting syntax may be more user-friendly; for `tyro`, it also enables support for
```

### Comparing `tyro-0.5.1/tyro/extras/__init__.py` & `tyro-0.5.2/tyro/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/extras/_base_configs.py` & `tyro-0.5.2/tyro/extras/_base_configs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/extras/_choices_type.py` & `tyro-0.5.2/tyro/extras/_choices_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/tyro/extras/_serialization.py` & `tyro-0.5.2/tyro/extras/_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.1/PKG-INFO` & `tyro-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.5.1
+Version: 0.5.2
 Summary: Strongly typed, zero-effort CLI interfaces
 Home-page: https://github.com/brentyi/tyro
 Author: brentyi
 Author-email: brentyi@berkeley.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

