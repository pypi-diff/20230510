# Comparing `tmp/py-module-parser-0.2.0.tar.gz` & `tmp/py-module-parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-module-parser-0.2.0.tar", max compression
+gzip compressed data, was "py-module-parser-0.3.0.tar", max compression
```

## Comparing `py-module-parser-0.2.0.tar` & `py-module-parser-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1093 2023-05-09 19:52:20.665429 py-module-parser-0.2.0/LICENSE
--rw-r--r--   0        0        0     4004 2023-05-09 19:50:56.096364 py-module-parser-0.2.0/README.md
--rw-r--r--   0        0        0      153 2023-05-09 19:35:44.746055 py-module-parser-0.2.0/py_module_parser/__init__.py
--rw-r--r--   0        0        0     1255 2023-05-09 19:42:22.221129 py-module-parser-0.2.0/py_module_parser/models.py
--rw-r--r--   0        0        0     8767 2023-05-09 19:46:22.296262 py-module-parser-0.2.0/py_module_parser/parser.py
--rw-r--r--   0        0        0      406 2023-05-09 19:23:59.461629 py-module-parser-0.2.0/py_module_parser/utils.py
--rw-r--r--   0        0        0     1104 2023-05-09 19:55:52.231761 py-module-parser-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4977 2023-05-09 19:55:55.156420 py-module-parser-0.2.0/setup.py
--rw-r--r--   0        0        0     5084 2023-05-09 19:55:55.156870 py-module-parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-09 19:52:20.665429 py-module-parser-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5696 2023-05-10 11:02:43.165961 py-module-parser-0.3.0/README.md
+-rw-r--r--   0        0        0      214 2023-05-10 07:42:51.492515 py-module-parser-0.3.0/py_module_parser/__init__.py
+-rw-r--r--   0        0        0     2457 2023-05-10 11:02:47.910450 py-module-parser-0.3.0/py_module_parser/models.py
+-rw-r--r--   0        0        0    11129 2023-05-10 11:06:14.288465 py-module-parser-0.3.0/py_module_parser/parser.py
+-rw-r--r--   0        0        0      320 2023-05-10 10:46:15.335512 py-module-parser-0.3.0/py_module_parser/utils.py
+-rw-r--r--   0        0        0     1125 2023-05-10 11:06:42.463762 py-module-parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6813 2023-05-10 11:07:30.049463 py-module-parser-0.3.0/setup.py
+-rw-r--r--   0        0        0     6818 2023-05-10 11:07:30.050001 py-module-parser-0.3.0/PKG-INFO
```

### Comparing `py-module-parser-0.2.0/LICENSE` & `py-module-parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-module-parser-0.2.0/py_module_parser/parser.py` & `py-module-parser-0.3.0/py_module_parser/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import _ast
 import ast
 from typing import Any, Dict, List, Union
 
 from py_module_parser.models import (
     ClassOutput,
     FromImportOutput,
-    FuncCallOutput,
+    CallOutput,
     ImportOutput,
     VariableOutput,
+    FunctionOutput,
+    GroupNodesByType,
+    NodesTypes,
+    NameOutput,
+    OUTPUT_TYPE,
 )
 
 
 class PyModulesParser:
     def __init__(self, input_code: str, group_by_type: bool = False) -> None:
         self.input_code = input_code
+        self.group_by_type = group_by_type
 
     def process_assign_node(
         self, node: ast.Assign, _attrs: List
     ) -> List[VariableOutput]:
-        _properties = {}
         _type = None
         if isinstance(node.value, ast.Constant):
             # like a = 'b'
             value = node.value.value
             _type = type(node.value.value).__name__
         elif isinstance(node.value, _ast.Call):
             value = self.process_call_node(node.value)
@@ -34,15 +39,14 @@
             raise
         for target in node.targets:
             name = target.id
             _attr = VariableOutput(
                 name=name,
                 default=value,
                 type_annotation=_type,
-                properties=_properties,
                 lineno_start=node.lineno,
                 lineno_end=node.end_lineno,
             )
             _attrs.append(_attr)
         return _attrs
 
     def process_annotation(
@@ -84,19 +88,19 @@
         else:
             if isinstance(node.value, ast.Attribute):
                 value = node.value.value.id
             else:
                 value = node.value.id
         return {key: value}
 
-    def process_call_node(self, node: _ast.Call) -> FuncCallOutput:
+    def process_call_node(self, node: _ast.Call) -> CallOutput:
         if isinstance(node.func, _ast.Attribute):
-            func_name = self.process_full_attr_node_name(node.func, None)
+            call_name = self.process_full_attr_node_name(node.func, None)
         elif isinstance(node.func, ast.Name):
-            func_name = node.func.id
+            call_name = node.func.id
         kwargs = {}
         for _node in node.keywords:
             kwargs.update(self.process_keyword(_node))
 
         args = []
 
         for _node in node.args:
@@ -105,16 +109,16 @@
             elif isinstance(_node, ast.Call):
                 arg = self.process_call_node(_node)
             elif isinstance(_node, ast.Constant):
                 arg = _node.value
             else:
                 arg = _node.id
             args.append(arg)
-        value = FuncCallOutput(
-            func_name=func_name,
+        value = CallOutput(
+            call_name=call_name,
             args=args,
             kwargs=kwargs,
             lineno_start=node.lineno,
             lineno_end=node.end_lineno,
         )
         return value
 
@@ -222,33 +226,94 @@
     def process_for_node(self, node: _ast.For):
         for_nodes = []
         full_nodes_list = [node.iter] + node.body + node.orelse
         for _node in full_nodes_list:
             self.parse_node(_node, for_nodes)
         return for_nodes
 
-    def parse_node(self, node, output):
+    def parse_return_node(self, node: _ast.Return):
+        returns = []
+        self.parse_node(node.value, returns)
+        return returns
+
+    def process_func_def_node(self, node: _ast.FunctionDef) -> FunctionOutput:
+        decorators = []
+        body = []
+        returns = []
+        for _node in node.body:
+            if isinstance(_node, _ast.Return):
+                returns = self.parse_return_node(_node)
+            else:
+                self.parse_node(_node, body)
+
+        for decorator in node.decorator_list:
+            if isinstance(decorator, _ast.Call):
+                decorators.append(self.process_call_node(decorator))
+            elif isinstance(decorator, _ast.Name):
+                decorators.append(NameOutput(name=decorator.id))
+        return FunctionOutput(
+            name=node.name,
+            body=body,
+            decorators=decorators,
+            returns=returns,
+            lineno_end=node.end_lineno,
+            lineno_start=node.lineno,
+        )
+
+    def parse_node(self, node: Any, output: OUTPUT_TYPE) -> OUTPUT_TYPE:
         # global scope of module
         if isinstance(node, _ast.Import):
             output.extend(self.process_import_node(node))
         elif isinstance(node, _ast.ImportFrom):
             output.append(self.process_import_from(node))
         elif isinstance(node, _ast.Expr):
             output.append(self.process_expression_node(node))
         elif isinstance(node, _ast.Try):
             output.extend(self.process_try_node(node))
+        # elif isinstance(node, _ast.Tuple):
+        # output.extend(self.process_tuple(node))
         elif isinstance(node, _ast.If):
             output.extend(self.process_if_node(node))
+        elif isinstance(node, _ast.FunctionDef):
+            output.extend(self.process_func_def_node(node))
         elif isinstance(node, _ast.For):
             output.extend(self.process_for_node(node))
         elif isinstance(node, _ast.Assign):
             output.extend(self.process_assign_node(node, []))
         elif isinstance(node, ast.ClassDef):
             output.append(self.process_class(node))
 
-    def parse(self):
+    def group_output_by_type(self, output: OUTPUT_TYPE):
+        imports = []
+        classes = []
+        functions = []
+        calls = []
+        variables = []
+        for node_out in output:
+            node_type = node_out.node_type
+            if node_type in [NodesTypes.IMPORT.value, NodesTypes.IMPORT_FROM.value]:
+                imports.append(node_out)
+            elif node_type == NodesTypes.CLASS.value:
+                classes.append(node_type)
+            elif node_type == NodesTypes.FUNCTION_DEF.value:
+                functions.append(node_out)
+            elif node_type == NodesTypes.CALL.value:
+                calls.append(node_out)
+            elif node_type == NodesTypes.VARIABLE.value:
+                variables.append(node_out)
+        return GroupNodesByType(
+            variables=variables,
+            calls=calls,
+            classes=classes,
+            functions=functions,
+            imports=imports,
+        )
+
+    def parse(self) -> Union[OUTPUT_TYPE, GroupNodesByType]:
         self.ast_tree = ast.parse(self.input_code)
         tree = self.ast_tree
         output = []
         for node in tree.body:
             self.parse_node(node, output)
+        if self.group_by_type:
+            output = self.group_output_by_type()
         return output
```

### Comparing `py-module-parser-0.2.0/pyproject.toml` & `py-module-parser-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-module-parser"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code."
 authors = ["Iuliia Volkova <xnuinside@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/xnuinside/py-module-parser"
 repository = "https://github.com/xnuinside/py-module-parser"
 classifiers = [
@@ -15,15 +15,16 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.7"
+pydantic = "^1.10.7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3"
 twine = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `py-module-parser-0.2.0/setup.py` & `py-module-parser-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,168 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# Python Module Parser
+![badge1](https://img.shields.io/pypi/v/py-module-parser) ![badge2](https://img.shields.io/pypi/l/py-module-parser) ![badge3](https://img.shields.io/pypi/pyversions/py-module-parser)![workflow](https://github.com/xnuinside/py-module-parser/actions/workflows/main.yml/badge.svg)
 
-packages = \
-['py_module_parser']
+Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.
 
-package_data = \
-{'': ['*']}
+To get more samples of output - check tests: tests/test_py_module_parser.py
 
-setup_kwargs = {
-    'name': 'py-module-parser',
-    'version': '0.2.0',
-    'description': 'Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.',
-    'long_description': '# Python Module Parser\n![badge1](https://img.shields.io/pypi/v/py-module-parser) ![badge2](https://img.shields.io/pypi/l/py-module-parser) ![badge3](https://img.shields.io/pypi/pyversions/py-module-parser)![workflow](https://github.com/xnuinside/py-module-parser/actions/workflows/main.yml/badge.svg)\n\nPython Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.\n\nTo get more samples of output - check tests: tests/test_py_module_parser.py\n\nThis project inspired by https://github.com/xnuinside/codegraph and https://github.com/xnuinside/py-models-parser and will be used as a parser inside them in the future. \n\n## Features\n\n- Parse Python modules and extract information about imports, functions, and variables\n- Identify line numbers for each import, function, and variable\n- Represent the extracted information in a structured format\n\n## Installation\n\nTo install the Python Module Parser library, use `pip`:\n\n```bash\n    pip install py-module-parser\n```\n\n\n## Usage\nHere\'s a simple example of how to use the Python Module Parser library:\n\n```python\nfrom py_module_parser import PyModulesParser\n\nsource_code = """from django.db import models\n\n\nclass Musician(models.Model):\n    first_name = models.CharField(max_length=50)\n    last_name = models.CharField(max_length=50)\n    instrument = models.CharField(max_length=100)\n\n"""\nparsed_output = PyModulesParser(source_code).parse()\nprint(parsed_output)\n```\n\nThis will output:\n\n```python\n[\n    FromImportOutput(\n        lineno_start=1,\n        lineno_end=1,\n        module=\'django.db\',\n        imports=[\n            ImportOutput(\n                lineno_start=1,\n                lineno_end=1,\n                name=\'models\',\n                alias=None,\n                node_type=\'import\'\n            )\n        ],\n        node_type=\'from_import\'\n    ),\n    ClassOutput(\n        lineno_start=4,\n        lineno_end=7,\n        name=\'Musician\',\n        parents=[\'models.Model\'],\n        attrs=[\n            VariableOutput(\n                lineno_start=5,\n                lineno_end=5,\n                name=\'first_name\',\n                type_annotation=None,\n                default=FuncCallOutput(\n                    lineno_start=5,\n                    lineno_end=5,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 50},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            ),\n            VariableOutput(\n                lineno_start=6,\n                lineno_end=6,\n                name=\'last_name\',\n                type_annotation=None,\n                default=FuncCallOutput(\n                    lineno_start=6,\n                    lineno_end=6,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 50},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            ),\n            VariableOutput(\n                lineno_start=7,\n                lineno_end=7,\n                name=\'instrument\',\n                type_annotation=None,\n                default=FuncCallOutput(\n                    lineno_start=7,\n                    lineno_end=7,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 100},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            )\n        ],\n        node_type=\'class\'\n    )\n]\n```\n\nTo parse from file, you can use method `parse_from_file`\n\n```python\nfrom py_module_parser import parse_from_file\n\nparsed_output = parse_from_file(file_path=\'path_to/python_module.py\')\nprint(parsed_output)\n```\n',
-    'author': 'Iuliia Volkova',
-    'author_email': 'xnuinside@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/xnuinside/py-module-parser',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+This project inspired by https://github.com/xnuinside/codegraph and https://github.com/xnuinside/py-models-parser and will be used as a parser inside them in the future. 
 
+## Features
 
-setup(**setup_kwargs)
+- Parse Python modules and extract information about imports, functions, and variables
+- Identify line numbers for each import, function, and variable
+- Represent the extracted information in a structured format
+
+## Installation
+
+To install the Python Module Parser library, use `pip`:
+
+```bash
+    pip install py-module-parser
+```
+
+
+## Usage
+Here's a simple example of how to use the Python Module Parser library:
+
+```python
+from py_module_parser import PyModulesParser
+
+source_code = """from django.db import models
+
+
+class Musician(models.Model):
+    first_name = models.CharField(max_length=50)
+    last_name = models.CharField(max_length=50)
+    instrument = models.CharField(max_length=100)
+
+"""
+parsed_output = PyModulesParser(source_code).parse()
+print(parsed_output)
+```
+
+This will output:
+
+```python
+[
+    FromImportOutput(
+        lineno_start=1,
+        lineno_end=1,
+        module='django.db',
+        imports=[
+            ImportOutput(
+                lineno_start=1,
+                lineno_end=1,
+                name='models',
+                alias=None,
+                node_type='import'
+            )
+        ],
+        node_type='from_import'
+    ),
+    ClassOutput(
+        lineno_start=4,
+        lineno_end=7,
+        name='Musician',
+        parents=['models.Model'],
+        attrs=[
+            VariableOutput(
+                lineno_start=5,
+                lineno_end=5,
+                name='first_name',
+                type_annotation=None,
+                default=CallOutput(
+                    lineno_start=5,
+                    lineno_end=5,
+                    func_name='models.CharField',
+                    args=[],
+                    kwargs={'max_length': 50},
+                    node_type='func_call'
+                ),
+                properties={},
+                node_type='variable'
+            ),
+            VariableOutput(
+                lineno_start=6,
+                lineno_end=6,
+                name='last_name',
+                type_annotation=None,
+                default=CallOutput(
+                    lineno_start=6,
+                    lineno_end=6,
+                    func_name='models.CharField',
+                    args=[],
+                    kwargs={'max_length': 50},
+                    node_type='func_call'
+                ),
+                properties={},
+                node_type='variable'
+            ),
+            VariableOutput(
+                lineno_start=7,
+                lineno_end=7,
+                name='instrument',
+                type_annotation=None,
+                default=CallOutput(
+                    lineno_start=7,
+                    lineno_end=7,
+                    func_name='models.CharField',
+                    args=[],
+                    kwargs={'max_length': 100},
+                    node_type='func_call'
+                ),
+                properties={},
+                node_type='variable'
+            )
+        ],
+        node_type='class'
+    )
+]
+```
+
+To parse from file, you can use method `parse_from_file`
+
+```python
+from py_module_parser import parse_from_file
+
+parsed_output = parse_from_file(file_path='path_to/python_module.py')
+print(parsed_output)
+```
+
+## Parser Output
+
+By default parser output is a list of Pydantic models with nested objects.
+
+List of possible node types exists as enum in py_modules_parser.NodesTypes:
+    
+VARIABLE = 'variable' - all variables like `a='b'`
+CALL = 'call' - all calls - function calls or class calls like `func_name(a)` or `ClassA()`
+CLASS = 'class' - classes defenitions `class SomeClass: ...`
+FUNCTION_DEF = 'func_def' - functions defenitions `def some_func(): ...`
+IMPORT = 'import' - imports like `import module`
+IMPORT_FROM = 'import_from' - imports like `from module import name`
+
+Output is a list of pydantic models specific for each node.
+Node type is always stored in argumen `node_type`
+
+Because, output models is Pydantic models - you can do anything with them that you can do with pydantic models.
+
+You can call .json() or .dict() if you prefer to have output not in Python Classes but as python dicts or json.
+
+If you are not familiar with Pydantic - check docs: https://docs.pydantic.dev/latest/usage/exporting_models/ 
+
+## TODO in next Releases
+
+
+1. Add parsing of functions arguments
+2. Add parsing of functions returns
+3. Add parsing for nested classes
+
+## Changelog
+** 0.3.0 - First stable release**
+
+1. Renamed FuncCallOutput to CallOutput to include Class calls as well as function calls.
+2. Added Enum to define available NodeTypes as py_module_parser.NodeTypes.
+3. Added parsing of function definition nodes.
+4. Implemented parsing of decorators.
+5. Added an optional group_by_type argument to PyModulesParser. If set to True, the output will be in the GroupNodesByType model, with keys such as imports, variables, classes, and functions, and all nodes will be grouped hierarchically inside them.
```

