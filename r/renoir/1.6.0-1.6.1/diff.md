# Comparing `tmp/renoir-1.6.0.tar.gz` & `tmp/renoir-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renoir-1.6.0.tar", max compression
+gzip compressed data, was "renoir-1.6.1.tar", max compression
```

## Comparing `renoir-1.6.0.tar` & `renoir-1.6.1.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     1008 2022-12-18 18:59:09.152541 renoir-1.6.0/CHANGES.md
--rw-r--r--   0        0        0     1486 2022-12-18 18:59:09.152541 renoir-1.6.0/LICENSE
--rw-r--r--   0        0        0      728 2022-12-18 18:59:09.152541 renoir-1.6.0/README.md
--rw-r--r--   0        0        0      374 2022-12-18 18:59:09.152541 renoir-1.6.0/docs/README.md
--rw-r--r--   0        0        0     5916 2022-12-18 18:59:09.152541 renoir-1.6.0/docs/extensions.md
--rw-r--r--   0        0        0     2100 2022-12-18 18:59:09.152541 renoir-1.6.0/docs/installation.md
--rw-r--r--   0        0        0     4544 2022-12-18 18:59:09.152541 renoir-1.6.0/docs/quickstart.md
--rw-r--r--   0        0        0       52 2022-12-18 18:59:09.152541 renoir-1.6.0/docs/tree.yml
--rw-r--r--   0        0        0     1450 2022-12-18 18:59:09.152541 renoir-1.6.0/pyproject.toml
--rw-r--r--   0        0        0       93 2022-12-18 18:59:09.152541 renoir-1.6.0/renoir/__init__.py
--rw-r--r--   0        0        0       22 2022-12-18 18:59:09.152541 renoir-1.6.0/renoir/__version__.py
--rw-r--r--   0        0        0      321 2022-12-18 18:59:09.152541 renoir-1.6.0/renoir/_internal.py
--rw-r--r--   0        0        0      970 2022-12-18 18:59:09.152541 renoir-1.6.0/renoir/_shortcuts.py
--rw-r--r--   0        0        0     7137 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/apis.py
--rw-r--r--   0        0        0     3204 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/cache.py
--rw-r--r--   0        0        0      371 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/constants.py
--rw-r--r--   0        0        0    10099 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/debug.py
--rw-r--r--   0        0        0     1262 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/errors.py
--rw-r--r--   0        0        0     2132 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/extensions.py
--rw-r--r--   0        0        0     1267 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/helpers.py
--rw-r--r--   0        0        0      150 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/parsing/__init__.py
--rw-r--r--   0        0        0     9982 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/parsing/contents.py
--rw-r--r--   0        0        0     6511 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/parsing/lexers.py
--rw-r--r--   0        0        0    10432 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/parsing/parsers.py
--rw-r--r--   0        0        0     8006 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/parsing/stack.py
--rw-r--r--   0        0        0      353 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/typing.py
--rw-r--r--   0        0        0     1211 2022-12-18 18:59:09.156541 renoir-1.6.0/renoir/writers.py
--rw-r--r--   0        0        0      157 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/blocks/child.txt
--rw-r--r--   0        0        0       84 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/blocks/child_multi_incl.txt
--rw-r--r--   0        0        0       48 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/blocks/parent.txt
--rw-r--r--   0        0        0      214 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/blocks/parent_incl.txt
--rw-r--r--   0        0        0      179 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/blocks/parent_multi_incl.txt
--rw-r--r--   0        0        0      200 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/blocks/parent_noincl.txt
--rw-r--r--   0        0        0       18 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/html/_footer.html
--rw-r--r--   0        0        0       19 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/html/_header.html
--rw-r--r--   0        0        0      592 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/html/layout.html
--rw-r--r--   0        0        0      225 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/html/pre.html
--rw-r--r--   0        0        0       27 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/html/pyerror.html
--rw-r--r--   0        0        0      222 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/html/test.html
--rw-r--r--   0        0        0      161 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/html/test2.html
--rw-r--r--   0        0        0     1634 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/test_cache.py
--rw-r--r--   0        0        0     1802 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/test_extensions.py
--rw-r--r--   0        0        0     3433 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/test_parsers.py
--rw-r--r--   0        0        0     8170 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/test_render.py
--rw-r--r--   0        0        0       44 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/yaml/_inclusion.1.yaml
--rw-r--r--   0        0        0       89 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/yaml/_inclusion.2.yaml
--rw-r--r--   0        0        0       53 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/yaml/_inclusion.3.yaml
--rw-r--r--   0        0        0       93 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/yaml/_inclusion.4.yaml
--rw-r--r--   0        0        0       72 2022-12-18 18:59:09.156541 renoir-1.6.0/tests/yaml/_inclusion.yaml
--rw-r--r--   0        0        0      565 2022-12-18 18:59:09.160541 renoir-1.6.0/tests/yaml/basic.yaml
--rw-r--r--   0        0        0      449 2022-12-18 18:59:09.160541 renoir-1.6.0/tests/yaml/blocks.yaml
--rw-r--r--   0        0        0      584 2022-12-18 18:59:09.160541 renoir-1.6.0/tests/yaml/nested.yaml
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 renoir-1.6.0/setup.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 renoir-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1008 2023-05-10 16:36:13.874483 renoir-1.6.1/CHANGES.md
+-rw-r--r--   0        0        0     1486 2023-05-10 16:36:13.874483 renoir-1.6.1/LICENSE
+-rw-r--r--   0        0        0      728 2023-05-10 16:36:13.874483 renoir-1.6.1/README.md
+-rw-r--r--   0        0        0      374 2023-05-10 16:36:13.874483 renoir-1.6.1/docs/README.md
+-rw-r--r--   0        0        0     5916 2023-05-10 16:36:13.874483 renoir-1.6.1/docs/extensions.md
+-rw-r--r--   0        0        0     2100 2023-05-10 16:36:13.874483 renoir-1.6.1/docs/installation.md
+-rw-r--r--   0        0        0     4544 2023-05-10 16:36:13.874483 renoir-1.6.1/docs/quickstart.md
+-rw-r--r--   0        0        0       52 2023-05-10 16:36:13.874483 renoir-1.6.1/docs/tree.yml
+-rw-r--r--   0        0        0     1432 2023-05-10 16:36:13.874483 renoir-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/__version__.py
+-rw-r--r--   0        0        0      321 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/_internal.py
+-rw-r--r--   0        0        0      970 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/_shortcuts.py
+-rw-r--r--   0        0        0     7137 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/apis.py
+-rw-r--r--   0        0        0     3287 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/cache.py
+-rw-r--r--   0        0        0      371 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/constants.py
+-rw-r--r--   0        0        0    10099 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/debug.py
+-rw-r--r--   0        0        0     1262 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/errors.py
+-rw-r--r--   0        0        0     2132 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/extensions.py
+-rw-r--r--   0        0        0     1267 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/helpers.py
+-rw-r--r--   0        0        0      150 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/parsing/__init__.py
+-rw-r--r--   0        0        0     9982 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/parsing/contents.py
+-rw-r--r--   0        0        0     6511 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/parsing/lexers.py
+-rw-r--r--   0        0        0    10491 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/parsing/parsers.py
+-rw-r--r--   0        0        0     8032 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/parsing/stack.py
+-rw-r--r--   0        0        0      353 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/typing.py
+-rw-r--r--   0        0        0     1211 2023-05-10 16:36:13.874483 renoir-1.6.1/renoir/writers.py
+-rw-r--r--   0        0        0      157 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/blocks/child.txt
+-rw-r--r--   0        0        0       84 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/blocks/child_multi_incl.txt
+-rw-r--r--   0        0        0       48 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/blocks/parent.txt
+-rw-r--r--   0        0        0      214 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/blocks/parent_incl.txt
+-rw-r--r--   0        0        0      179 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/blocks/parent_multi_incl.txt
+-rw-r--r--   0        0        0      200 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/blocks/parent_noincl.txt
+-rw-r--r--   0        0        0       18 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/html/_footer.html
+-rw-r--r--   0        0        0       19 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/html/_header.html
+-rw-r--r--   0        0        0      592 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/html/layout.html
+-rw-r--r--   0        0        0      225 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/html/pre.html
+-rw-r--r--   0        0        0       27 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/html/pyerror.html
+-rw-r--r--   0        0        0      222 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/html/test.html
+-rw-r--r--   0        0        0      161 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/html/test2.html
+-rw-r--r--   0        0        0     1634 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/test_cache.py
+-rw-r--r--   0        0        0     1802 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/test_extensions.py
+-rw-r--r--   0        0        0     3433 2023-05-10 16:36:13.874483 renoir-1.6.1/tests/test_parsers.py
+-rw-r--r--   0        0        0     8170 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/test_render.py
+-rw-r--r--   0        0        0       44 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/yaml/_inclusion.1.yaml
+-rw-r--r--   0        0        0       89 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/yaml/_inclusion.2.yaml
+-rw-r--r--   0        0        0       53 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/yaml/_inclusion.3.yaml
+-rw-r--r--   0        0        0       93 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/yaml/_inclusion.4.yaml
+-rw-r--r--   0        0        0       72 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/yaml/_inclusion.yaml
+-rw-r--r--   0        0        0      565 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/yaml/basic.yaml
+-rw-r--r--   0        0        0      449 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/yaml/blocks.yaml
+-rw-r--r--   0        0        0      584 2023-05-10 16:36:13.878483 renoir-1.6.1/tests/yaml/nested.yaml
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 renoir-1.6.1/PKG-INFO
```

### Comparing `renoir-1.6.0/CHANGES.md` & `renoir-1.6.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/LICENSE` & `renoir-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/README.md` & `renoir-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/docs/extensions.md` & `renoir-1.6.1/docs/extensions.md`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/docs/installation.md` & `renoir-1.6.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/docs/quickstart.md` & `renoir-1.6.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/pyproject.toml` & `renoir-1.6.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "Renoir"
-version = "1.6.0"
+name = "renoir"
+version = "1.6.1"
 description = "A templating engine designed with simplicity in mind"
 authors = ["Giovanni Barillari <gi0baro@d4net.org>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/renoir"
 repository = "https://github.com/emmett-framework/renoir"
@@ -40,13 +40,12 @@
 "Issue Tracker" = "https://github.com/emmett-framework/renoir/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
-pylint = "^2.4.4"
 pyyaml = "^5.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `renoir-1.6.0/renoir/_shortcuts.py` & `renoir-1.6.1/renoir/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/renoir/apis.py` & `renoir-1.6.1/renoir/apis.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/renoir/cache.py` & `renoir-1.6.1/renoir/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,27 +86,27 @@
 
 class ParserCache(HashableCache):
     def __init__(self, cache_interface):
         super().__init__(cache_interface)
         self.cdata = {}
         self.dependencies = {}
 
-    def _expired_dependency(self, name):
-        path, file_name = self.cache.templater.preload(name)
+    def _expired_dependency(self, name, preload_params):
+        path, file_name = self.cache.templater.preload(name, **preload_params)
         file_path = os.path.join(path, file_name)
         if os.stat(file_path).st_mtime != self.cache.load.mtimes[file_path]:
             return True
         return False
 
     def reloader_get(self, name, source):
         hashed = make_hash(source)
         if self.hashes.get(name) != hashed:
             return None, None
-        for dep_name in self.dependencies[name]:
-            if self._expired_dependency(dep_name):
+        for dep_name, dep_preload_params in self.dependencies[name].values():
+            if self._expired_dependency(dep_name, dep_preload_params):
                 return None, None
         return self.cached_get(name, source)
 
     def cached_get(self, name, source):
         return self.data.get(name), self.cdata.get(name)
 
     def set(self, name, source, compiled, content, dependencies):
```

### Comparing `renoir-1.6.0/renoir/debug.py` & `renoir-1.6.1/renoir/debug.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/renoir/errors.py` & `renoir-1.6.1/renoir/errors.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/renoir/extensions.py` & `renoir-1.6.1/renoir/extensions.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/renoir/helpers.py` & `renoir-1.6.1/renoir/helpers.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/renoir/parsing/contents.py` & `renoir-1.6.1/renoir/parsing/contents.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/renoir/parsing/lexers.py` & `renoir-1.6.1/renoir/parsing/lexers.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/renoir/parsing/parsers.py` & `renoir-1.6.1/renoir/parsing/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,33 +78,33 @@
         try:
             filename = eval(filename, self.scope)
         except Exception:
             raise TemplateError(
                 'Invalid template filename', ctx.state.source, ctx.state.lines
             )
         #: resolve paths
-        preload_params = {}
+        preload_name, preload_params = filename, {}
         if any(filename.startswith(relpath) for relpath in ["./", "../"]):
             full_path = (ctxpath / Path(filename)).resolve()
             preload_params["path"] = full_path.parent
-            filename = full_path.name
+            preload_name = full_path.name
         #: get the file contents
-        path, file_name = self.templater.preload(filename, **preload_params)
+        path, file_name = self.templater.preload(preload_name, **preload_params)
         file_path = os.path.join(path, file_name)
         try:
             text = self.templater.load(file_path)
         except Exception:
             raise TemplateError(
                 'Unable to open included view file',
                 ctx.state.source, ctx.state.lines
             )
         text = self.templater.prerender(text, file_path)
         if strip_ending_new_line and text.endswith("\n"):
             text = text[:-1]
-        return filename, file_path, text
+        return filename, file_path, (preload_name, preload_params), text
 
     def parse_plain_block(self, ctx, element):
         ctx.update_lines_count(element.linesn)
         ctx.plain(element)
 
     #: get rid of delimiters
     def _get_python_block_text(self, element):
@@ -172,15 +172,15 @@
             plain_node_cls=self._nodes_cls['plain']
         )
 
     def parse(self, text):
         ctx = self._build_ctx(text)
         ctx.parse()
         self.content = ctx.content
-        self.dependencies = list(set(ctx.state.dependencies))
+        self.dependencies = dict(ctx.state.dependencies)
 
     def reindent(self, text):
         lines = text.split('\n')
         new_lines = []
         indent = 0
         dedented = 0
         match_stack = []
```

### Comparing `renoir-1.6.0/renoir/parsing/stack.py` & `renoir-1.6.1/renoir/parsing/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.in_python_block = in_python_block
         self.parent = parent
         self.source = source
         self.lines = ParsedLines(line_start, line_start)
         self.settings = settings
         self.content = Content()
         self.blocks = blocks if blocks is not None else {}
-        self.dependencies = []
+        self.dependencies = {}
         self.indent = 0
         self.offset = 0
         if (
             self.elements and
             self.elements[0].is_python_block and
             not self.in_python_block
         ):
@@ -153,21 +153,21 @@
         self.stack.append(self.state)
         self.state = self.state(
             name=name, elements=elements, in_python_block=in_python_block,
             **kwargs)
         return self
 
     def load(self, name, **kwargs):
-        name, file_path, text = self.parser._get_file_text(
+        name, file_path, preload_params, text = self.parser._get_file_text(
             self,
             name,
             ctxpath=self.cwd,
             strip_ending_new_line=kwargs.pop("strip_ending_new_line", False)
         )
-        self.state.dependencies.append(name)
+        self.state.dependencies[name] = preload_params
         kwargs['source'] = file_path
         kwargs['in_python_block'] = False
         return self(
             name=name,
             elements=Elements(self.parser._tag_split_text(text)).to_list(),
             **kwargs
         )
@@ -178,29 +178,29 @@
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type:
             raise
         self.swap_block_type()
-        deps = list(self.state.dependencies)
+        deps = dict(self.state.dependencies)
         contents = self.content.contents
         name = self.name
         lines = self.state.lines
         in_python_block = self.state.in_python_block
         isolated_pyblockstate = self.state.isolated_pyblockstate
         state_id = self.state._id
         self.state = self.stack.pop()
         node = self.node_group(contents)
         if not isolated_pyblockstate:
             self.state.in_python_block = in_python_block
             self.update_lines_count(
                 lines.end - lines.start, offset=lines.end)
         self.state.blocks[name] = state_id
-        self.state.dependencies.extend(deps)
+        self.state.dependencies.update(deps)
         self.nodes_map[state_id] = node
 
     def python_node(self, value=None):
         node = Node(value, source=self.state.source, lines=self.state.lines)
         self.content.append(node)
         return node
```

### Comparing `renoir-1.6.0/renoir/writers.py` & `renoir-1.6.1/renoir/writers.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/tests/html/layout.html` & `renoir-1.6.1/tests/html/layout.html`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/tests/test_cache.py` & `renoir-1.6.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/tests/test_extensions.py` & `renoir-1.6.1/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/tests/test_parsers.py` & `renoir-1.6.1/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/tests/test_render.py` & `renoir-1.6.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/tests/yaml/basic.yaml` & `renoir-1.6.1/tests/yaml/basic.yaml`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/tests/yaml/nested.yaml` & `renoir-1.6.1/tests/yaml/nested.yaml`

 * *Files identical despite different names*

### Comparing `renoir-1.6.0/PKG-INFO` & `renoir-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renoir
-Version: 1.6.0
+Version: 1.6.1
 Summary: A templating engine designed with simplicity in mind
 Home-page: https://github.com/emmett-framework/renoir
 License: BSD-3-Clause
 Keywords: templates,html,web
 Author: Giovanni Barillari
 Author-email: gi0baro@d4net.org
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: renoir Version: 1.6.0 Summary: A templating engine
+Metadata-Version: 2.1 Name: renoir Version: 1.6.1 Summary: A templating engine
 designed with simplicity in mind Home-page: https://github.com/emmett-
 framework/renoir License: BSD-3-Clause Keywords: templates,html,web Author:
 Giovanni Barillari Author-email: gi0baro@d4net.org Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Web Environment Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

