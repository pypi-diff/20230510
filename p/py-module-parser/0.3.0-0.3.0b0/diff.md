# Comparing `tmp/py-module-parser-0.3.0.tar.gz` & `tmp/py-module-parser-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-module-parser-0.3.0.tar", max compression
+gzip compressed data, was "py-module-parser-0.3.0b0.tar", max compression
```

## Comparing `py-module-parser-0.3.0.tar` & `py-module-parser-0.3.0b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1093 2023-05-09 19:52:20.665429 py-module-parser-0.3.0/LICENSE
--rw-r--r--   0        0        0     5696 2023-05-10 11:02:43.165961 py-module-parser-0.3.0/README.md
--rw-r--r--   0        0        0      214 2023-05-10 07:42:51.492515 py-module-parser-0.3.0/py_module_parser/__init__.py
--rw-r--r--   0        0        0     2457 2023-05-10 11:02:47.910450 py-module-parser-0.3.0/py_module_parser/models.py
--rw-r--r--   0        0        0    11129 2023-05-10 11:06:14.288465 py-module-parser-0.3.0/py_module_parser/parser.py
--rw-r--r--   0        0        0      320 2023-05-10 10:46:15.335512 py-module-parser-0.3.0/py_module_parser/utils.py
--rw-r--r--   0        0        0     1125 2023-05-10 11:06:42.463762 py-module-parser-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6813 2023-05-10 11:07:30.049463 py-module-parser-0.3.0/setup.py
--rw-r--r--   0        0        0     6818 2023-05-10 11:07:30.050001 py-module-parser-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-09 19:52:20.665429 py-module-parser-0.3.0b0/LICENSE
+-rw-r--r--   0        0        0     5696 2023-05-10 11:02:43.165961 py-module-parser-0.3.0b0/README.md
+-rw-r--r--   0        0        0      214 2023-05-10 07:42:51.492515 py-module-parser-0.3.0b0/py_module_parser/__init__.py
+-rw-r--r--   0        0        0     2457 2023-05-10 11:02:47.910450 py-module-parser-0.3.0b0/py_module_parser/models.py
+-rw-r--r--   0        0        0    11480 2023-05-10 11:01:46.874722 py-module-parser-0.3.0b0/py_module_parser/parser.py
+-rw-r--r--   0        0        0      320 2023-05-10 10:46:15.335512 py-module-parser-0.3.0b0/py_module_parser/utils.py
+-rw-r--r--   0        0        0     1127 2023-05-10 10:52:20.592352 py-module-parser-0.3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     6815 2023-05-10 11:04:32.685243 py-module-parser-0.3.0b0/setup.py
+-rw-r--r--   0        0        0     6820 2023-05-10 11:04:32.685853 py-module-parser-0.3.0b0/PKG-INFO
```

### Comparing `py-module-parser-0.3.0/LICENSE` & `py-module-parser-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-module-parser-0.3.0/README.md` & `py-module-parser-0.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `py-module-parser-0.3.0/py_module_parser/models.py` & `py-module-parser-0.3.0b0/py_module_parser/models.py`

 * *Files identical despite different names*

### Comparing `py-module-parser-0.3.0/py_module_parser/parser.py` & `py-module-parser-0.3.0b0/py_module_parser/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self.input_code = input_code
         self.group_by_type = group_by_type
 
     def process_assign_node(
         self, node: ast.Assign, _attrs: List
     ) -> List[VariableOutput]:
         _type = None
+        print(node.targets[0].id)
         if isinstance(node.value, ast.Constant):
             # like a = 'b'
             value = node.value.value
             _type = type(node.value.value).__name__
         elif isinstance(node.value, _ast.Call):
             value = self.process_call_node(node.value)
             _type = None
@@ -43,14 +44,15 @@
                 name=name,
                 default=value,
                 type_annotation=_type,
                 lineno_start=node.lineno,
                 lineno_end=node.end_lineno,
             )
             _attrs.append(_attr)
+        print(_attrs)
         return _attrs
 
     def process_annotation(
         self, ann: Union[ast.Name, _ast.Subscript, _ast.Attribute]
     ) -> Union[Dict, str]:
         if isinstance(ann, ast.Name):
             _type = ann.id
@@ -236,18 +238,20 @@
         return returns
 
     def process_func_def_node(self, node: _ast.FunctionDef) -> FunctionOutput:
         decorators = []
         body = []
         returns = []
         for _node in node.body:
+            print(type(_node))
             if isinstance(_node, _ast.Return):
                 returns = self.parse_return_node(_node)
             else:
                 self.parse_node(_node, body)
+                print(body)
 
         for decorator in node.decorator_list:
             if isinstance(decorator, _ast.Call):
                 decorators.append(self.process_call_node(decorator))
             elif isinstance(decorator, _ast.Name):
                 decorators.append(NameOutput(name=decorator.id))
         return FunctionOutput(
@@ -255,14 +259,23 @@
             body=body,
             decorators=decorators,
             returns=returns,
             lineno_end=node.end_lineno,
             lineno_start=node.lineno,
         )
 
+    """def process_tuple(self, node: _ast.Tuple):
+        tuple_items = []
+        for _node in node.elts:
+            print(type(_node))
+            self.parse_node(_node, tuple_items)
+        print(tuple_items)
+        raise
+    """
+
     def parse_node(self, node: Any, output: OUTPUT_TYPE) -> OUTPUT_TYPE:
         # global scope of module
         if isinstance(node, _ast.Import):
             output.extend(self.process_import_node(node))
         elif isinstance(node, _ast.ImportFrom):
             output.append(self.process_import_from(node))
         elif isinstance(node, _ast.Expr):
```

### Comparing `py-module-parser-0.3.0/pyproject.toml` & `py-module-parser-0.3.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-module-parser"
-version = "0.3.0"
+version = "0.3.0b0"
 description = "Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code."
 authors = ["Iuliia Volkova <xnuinside@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/xnuinside/py-module-parser"
 repository = "https://github.com/xnuinside/py-module-parser"
 classifiers = [
```

### Comparing `py-module-parser-0.3.0/setup.py` & `py-module-parser-0.3.0b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'py-module-parser',
-    'version': '0.3.0',
+    'version': '0.3.0b0',
     'description': 'Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.',
     'long_description': '# Python Module Parser\n![badge1](https://img.shields.io/pypi/v/py-module-parser) ![badge2](https://img.shields.io/pypi/l/py-module-parser) ![badge3](https://img.shields.io/pypi/pyversions/py-module-parser)![workflow](https://github.com/xnuinside/py-module-parser/actions/workflows/main.yml/badge.svg)\n\nPython Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.\n\nTo get more samples of output - check tests: tests/test_py_module_parser.py\n\nThis project inspired by https://github.com/xnuinside/codegraph and https://github.com/xnuinside/py-models-parser and will be used as a parser inside them in the future. \n\n## Features\n\n- Parse Python modules and extract information about imports, functions, and variables\n- Identify line numbers for each import, function, and variable\n- Represent the extracted information in a structured format\n\n## Installation\n\nTo install the Python Module Parser library, use `pip`:\n\n```bash\n    pip install py-module-parser\n```\n\n\n## Usage\nHere\'s a simple example of how to use the Python Module Parser library:\n\n```python\nfrom py_module_parser import PyModulesParser\n\nsource_code = """from django.db import models\n\n\nclass Musician(models.Model):\n    first_name = models.CharField(max_length=50)\n    last_name = models.CharField(max_length=50)\n    instrument = models.CharField(max_length=100)\n\n"""\nparsed_output = PyModulesParser(source_code).parse()\nprint(parsed_output)\n```\n\nThis will output:\n\n```python\n[\n    FromImportOutput(\n        lineno_start=1,\n        lineno_end=1,\n        module=\'django.db\',\n        imports=[\n            ImportOutput(\n                lineno_start=1,\n                lineno_end=1,\n                name=\'models\',\n                alias=None,\n                node_type=\'import\'\n            )\n        ],\n        node_type=\'from_import\'\n    ),\n    ClassOutput(\n        lineno_start=4,\n        lineno_end=7,\n        name=\'Musician\',\n        parents=[\'models.Model\'],\n        attrs=[\n            VariableOutput(\n                lineno_start=5,\n                lineno_end=5,\n                name=\'first_name\',\n                type_annotation=None,\n                default=CallOutput(\n                    lineno_start=5,\n                    lineno_end=5,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 50},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            ),\n            VariableOutput(\n                lineno_start=6,\n                lineno_end=6,\n                name=\'last_name\',\n                type_annotation=None,\n                default=CallOutput(\n                    lineno_start=6,\n                    lineno_end=6,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 50},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            ),\n            VariableOutput(\n                lineno_start=7,\n                lineno_end=7,\n                name=\'instrument\',\n                type_annotation=None,\n                default=CallOutput(\n                    lineno_start=7,\n                    lineno_end=7,\n                    func_name=\'models.CharField\',\n                    args=[],\n                    kwargs={\'max_length\': 100},\n                    node_type=\'func_call\'\n                ),\n                properties={},\n                node_type=\'variable\'\n            )\n        ],\n        node_type=\'class\'\n    )\n]\n```\n\nTo parse from file, you can use method `parse_from_file`\n\n```python\nfrom py_module_parser import parse_from_file\n\nparsed_output = parse_from_file(file_path=\'path_to/python_module.py\')\nprint(parsed_output)\n```\n\n## Parser Output\n\nBy default parser output is a list of Pydantic models with nested objects.\n\nList of possible node types exists as enum in py_modules_parser.NodesTypes:\n    \nVARIABLE = \'variable\' - all variables like `a=\'b\'`\nCALL = \'call\' - all calls - function calls or class calls like `func_name(a)` or `ClassA()`\nCLASS = \'class\' - classes defenitions `class SomeClass: ...`\nFUNCTION_DEF = \'func_def\' - functions defenitions `def some_func(): ...`\nIMPORT = \'import\' - imports like `import module`\nIMPORT_FROM = \'import_from\' - imports like `from module import name`\n\nOutput is a list of pydantic models specific for each node.\nNode type is always stored in argumen `node_type`\n\nBecause, output models is Pydantic models - you can do anything with them that you can do with pydantic models.\n\nYou can call .json() or .dict() if you prefer to have output not in Python Classes but as python dicts or json.\n\nIf you are not familiar with Pydantic - check docs: https://docs.pydantic.dev/latest/usage/exporting_models/ \n\n## TODO in next Releases\n\n\n1. Add parsing of functions arguments\n2. Add parsing of functions returns\n3. Add parsing for nested classes\n\n## Changelog\n** 0.3.0 - First stable release**\n\n1. Renamed FuncCallOutput to CallOutput to include Class calls as well as function calls.\n2. Added Enum to define available NodeTypes as py_module_parser.NodeTypes.\n3. Added parsing of function definition nodes.\n4. Implemented parsing of decorators.\n5. Added an optional group_by_type argument to PyModulesParser. If set to True, the output will be in the GroupNodesByType model, with keys such as imports, variables, classes, and functions, and all nodes will be grouped hierarchically inside them.\n',
     'author': 'Iuliia Volkova',
     'author_email': 'xnuinside@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/xnuinside/py-module-parser',
```

### Comparing `py-module-parser-0.3.0/PKG-INFO` & `py-module-parser-0.3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-module-parser
-Version: 0.3.0
+Version: 0.3.0b0
 Summary: Python Module Parser is a library that parses Python modules and outputs information about imports, functions, variables, and their corresponding line numbers. This makes it easier to analyze and understand the structure of your Python code.
 Home-page: https://github.com/xnuinside/py-module-parser
 License: MIT
 Author: Iuliia Volkova
 Author-email: xnuinside@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

