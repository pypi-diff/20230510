# Comparing `tmp/types-fpdf2-2.7.4.0.tar.gz` & `tmp/types-fpdf2-2.7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-fpdf2-2.7.4.0.tar", last modified: Wed May  3 18:17:57 2023, max compression
+gzip compressed data, was "types-fpdf2-2.7.4.1.tar", last modified: Wed May 10 15:23:23 2023, max compression
```

## Comparing `types-fpdf2-2.7.4.0.tar` & `types-fpdf2-2.7.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:17:57.115836 types-fpdf2-2.7.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-03 18:17:55.000000 types-fpdf2-2.7.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 18:17:55.000000 types-fpdf2-2.7.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-03 18:17:57.115836 types-fpdf2-2.7.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:17:57.111836 types-fpdf2-2.7.4.0/fpdf-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 18:17:55.000000 types-fpdf2-2.7.4.0/fpdf-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/_fonttools_shims.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/annotations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/deprecation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/encryption.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/fpdf.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/graphics_state.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/html.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/image_parsing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/line_break.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/linearization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/outline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/output.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/prefs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/recorder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/sign.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/structure_tree.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/svg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/syntax.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/transitions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 18:17:41.000000 types-fpdf2-2.7.4.0/fpdf-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:17:57.115836 types-fpdf2-2.7.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-03 18:17:55.000000 types-fpdf2-2.7.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:17:57.111836 types-fpdf2-2.7.4.0/types_fpdf2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-03 18:17:57.000000 types-fpdf2-2.7.4.0/types_fpdf2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-03 18:17:57.000000 types-fpdf2-2.7.4.0/types_fpdf2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:17:57.000000 types-fpdf2-2.7.4.0/types_fpdf2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 18:17:57.000000 types-fpdf2-2.7.4.0/types_fpdf2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 18:17:57.000000 types-fpdf2-2.7.4.0/types_fpdf2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:23.282237 types-fpdf2-2.7.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-10 15:23:22.000000 types-fpdf2-2.7.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:22.000000 types-fpdf2-2.7.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-10 15:23:23.282237 types-fpdf2-2.7.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:23.282237 types-fpdf2-2.7.4.1/fpdf-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 15:23:22.000000 types-fpdf2-2.7.4.1/fpdf-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/_fonttools_shims.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/annotations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/deprecation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/encryption.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20289 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/fpdf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/graphics_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/image_parsing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/line_break.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/linearization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/outline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/output.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/prefs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/recorder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/sign.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/structure_tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/svg.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/syntax.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/transitions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-10 15:19:44.000000 types-fpdf2-2.7.4.1/fpdf-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:23.282237 types-fpdf2-2.7.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-10 15:23:22.000000 types-fpdf2-2.7.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:23.282237 types-fpdf2-2.7.4.1/types_fpdf2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-10 15:23:23.000000 types-fpdf2-2.7.4.1/types_fpdf2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-10 15:23:23.000000 types-fpdf2-2.7.4.1/types_fpdf2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:23.000000 types-fpdf2-2.7.4.1/types_fpdf2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 15:23:23.000000 types-fpdf2-2.7.4.1/types_fpdf2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 15:23:23.000000 types-fpdf2-2.7.4.1/types_fpdf2.egg-info/top_level.txt
```

### Comparing `types-fpdf2-2.7.4.0/CHANGELOG.md` & `types-fpdf2-2.7.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.7.4.1 (2023-05-10)
+
+Fix return type of FPDF.output() (#10166)
+
 ## 2.7.4.0 (2023-05-03)
 
 [fpdf2] Update stubs for fpdf 2.7.4 (#10136)
 
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
 
 ## 2.7.1.0 (2023-05-03)
```

### Comparing `types-fpdf2-2.7.4.0/PKG-INFO` & `types-fpdf2-2.7.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-fpdf2
-Version: 2.7.4.0
+Version: 2.7.4.1
 Summary: Typing stubs for fpdf2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f1c419e816e101dfacf8cd9cbc808f4839b32dda`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/__init__.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/_fonttools_shims.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/_fonttools_shims.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/actions.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/actions.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/annotations.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/annotations.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/drawing.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/drawing.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/encryption.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/encryption.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/enums.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/enums.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/fonts.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/fonts.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/fpdf.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/fpdf.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -544,12 +544,12 @@
     @overload
     def output(  # type: ignore[misc]
         self,
         name: Literal[""] | None = "",
         dest: Unused = "",
         linearize: bool = False,
         output_producer_class: Callable[[FPDF], OutputProducer] = ...,
-    ) -> None: ...
+    ) -> bytearray: ...
     @overload
     def output(
         self, name: str, dest: Unused = "", linearize: bool = False, output_producer_class: Callable[[FPDF], OutputProducer] = ...
-    ) -> bytearray: ...
+    ) -> None: ...
```

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/graphics_state.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/graphics_state.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/html.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/html.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/image_parsing.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/image_parsing.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/line_break.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/line_break.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/linearization.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/linearization.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/outline.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/outline.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/output.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/output.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/prefs.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/prefs.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/sign.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/sign.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/structure_tree.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/structure_tree.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/svg.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/svg.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/syntax.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/syntax.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/table.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/table.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/template.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/template.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/transitions.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/transitions.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/fpdf-stubs/util.pyi` & `types-fpdf2-2.7.4.1/fpdf-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.4.0/setup.py` & `types-fpdf2-2.7.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f1c419e816e101dfacf8cd9cbc808f4839b32dda`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.7.4.0",
+      version="2.7.4.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md",
```

### Comparing `types-fpdf2-2.7.4.0/types_fpdf2.egg-info/PKG-INFO` & `types-fpdf2-2.7.4.1/types_fpdf2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-fpdf2
-Version: 2.7.4.0
+Version: 2.7.4.1
 Summary: Typing stubs for fpdf2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f1c419e816e101dfacf8cd9cbc808f4839b32dda`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-fpdf2-2.7.4.0/types_fpdf2.egg-info/SOURCES.txt` & `types-fpdf2-2.7.4.1/types_fpdf2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

