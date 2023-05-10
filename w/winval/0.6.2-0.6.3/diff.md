# Comparing `tmp/winval-0.6.2.tar.gz` & `tmp/winval-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winval-0.6.2.tar", max compression
+gzip compressed data, was "winval-0.6.3.tar", max compression
```

## Comparing `winval-0.6.2.tar` & `winval-0.6.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10765 2023-05-02 07:47:08.951592 winval-0.6.2/LICENSE
--rw-r--r--   0        0        0     2873 2023-05-02 07:47:08.951592 winval-0.6.2/README.md
--rw-r--r--   0        0        0      439 2023-05-02 07:47:08.951592 winval-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      572 2023-05-02 07:47:08.951592 winval-0.6.2/winval/__init__.py
--rw-r--r--   0        0        0     3703 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winval.interp
--rw-r--r--   0        0        0      611 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winval.tokens
--rw-r--r--   0        0        0     9502 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalLexer.interp
--rw-r--r--   0        0        0     9570 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalLexer.py
--rw-r--r--   0        0        0      611 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalLexer.tokens
--rw-r--r--   0        0        0     4571 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalListener.py
--rw-r--r--   0        0        0    38746 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalParser.py
--rw-r--r--   0        0        0     2876 2023-05-02 07:47:08.951592 winval-0.6.2/winval/antlr/winvalVisitor.py
--rw-r--r--   0        0        0     4606 2023-05-02 07:47:08.951592 winval-0.6.2/winval/cloud_files_validator.py
--rw-r--r--   0        0        0     5574 2023-05-02 07:47:08.951592 winval-0.6.2/winval/constraint_eval.py
--rw-r--r--   0        0        0      849 2023-05-02 07:47:08.951592 winval-0.6.2/winval/constraints_pre_processor.py
--rw-r--r--   0        0        0     1843 2023-05-02 07:47:08.951592 winval-0.6.2/winval/parsed_workflow_inputs.py
--rw-r--r--   0        0        0     1099 2023-05-02 07:47:08.955592 winval-0.6.2/winval/python_extensions.py
--rw-r--r--   0        0        0     1901 2023-05-02 07:47:08.955592 winval-0.6.2/winval/validate_wdl_constraints.py
--rw-r--r--   0        0        0     7496 2023-05-02 07:47:08.955592 winval-0.6.2/winval/wdl_parser.py
--rw-r--r--   0        0        0     1710 2023-05-02 07:47:08.955592 winval-0.6.2/winval/winval.g4
--rw-r--r--   0        0        0     3297 2023-05-02 07:47:08.955592 winval-0.6.2/winval/winval_class.py
--rw-r--r--   0        0        0     4531 2023-05-02 07:47:08.955592 winval-0.6.2/winval/workflow_var.py
--rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 winval-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-05-10 09:11:50.098046 winval-0.6.3/LICENSE
+-rw-r--r--   0        0        0     2873 2023-05-10 09:11:50.098046 winval-0.6.3/README.md
+-rw-r--r--   0        0        0      439 2023-05-10 09:11:50.098046 winval-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      572 2023-05-10 09:11:50.098046 winval-0.6.3/winval/__init__.py
+-rw-r--r--   0        0        0     3703 2023-05-10 09:11:50.098046 winval-0.6.3/winval/antlr/winval.interp
+-rw-r--r--   0        0        0      611 2023-05-10 09:11:50.098046 winval-0.6.3/winval/antlr/winval.tokens
+-rw-r--r--   0        0        0     9502 2023-05-10 09:11:50.098046 winval-0.6.3/winval/antlr/winvalLexer.interp
+-rw-r--r--   0        0        0     9570 2023-05-10 09:11:50.098046 winval-0.6.3/winval/antlr/winvalLexer.py
+-rw-r--r--   0        0        0      611 2023-05-10 09:11:50.098046 winval-0.6.3/winval/antlr/winvalLexer.tokens
+-rw-r--r--   0        0        0     4571 2023-05-10 09:11:50.098046 winval-0.6.3/winval/antlr/winvalListener.py
+-rw-r--r--   0        0        0    38746 2023-05-10 09:11:50.098046 winval-0.6.3/winval/antlr/winvalParser.py
+-rw-r--r--   0        0        0     2876 2023-05-10 09:11:50.098046 winval-0.6.3/winval/antlr/winvalVisitor.py
+-rw-r--r--   0        0        0     4606 2023-05-10 09:11:50.098046 winval-0.6.3/winval/cloud_files_validator.py
+-rw-r--r--   0        0        0     5574 2023-05-10 09:11:50.098046 winval-0.6.3/winval/constraint_eval.py
+-rw-r--r--   0        0        0      849 2023-05-10 09:11:50.098046 winval-0.6.3/winval/constraints_pre_processor.py
+-rw-r--r--   0        0        0     1843 2023-05-10 09:11:50.098046 winval-0.6.3/winval/parsed_workflow_inputs.py
+-rw-r--r--   0        0        0     1099 2023-05-10 09:11:50.098046 winval-0.6.3/winval/python_extensions.py
+-rw-r--r--   0        0        0     1901 2023-05-10 09:11:50.098046 winval-0.6.3/winval/validate_wdl_constraints.py
+-rw-r--r--   0        0        0     7496 2023-05-10 09:11:50.098046 winval-0.6.3/winval/wdl_parser.py
+-rw-r--r--   0        0        0     1710 2023-05-10 09:11:50.098046 winval-0.6.3/winval/winval.g4
+-rw-r--r--   0        0        0     3297 2023-05-10 09:11:50.098046 winval-0.6.3/winval/winval_class.py
+-rw-r--r--   0        0        0     5172 2023-05-10 09:11:50.098046 winval-0.6.3/winval/workflow_var.py
+-rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 winval-0.6.3/PKG-INFO
```

### Comparing `winval-0.6.2/LICENSE` & `winval-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/README.md` & `winval-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/__init__.py` & `winval-0.6.3/winval/__init__.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/antlr/winval.interp` & `winval-0.6.3/winval/antlr/winval.interp`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/antlr/winval.tokens` & `winval-0.6.3/winval/antlr/winval.tokens`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/antlr/winvalLexer.interp` & `winval-0.6.3/winval/antlr/winvalLexer.interp`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/antlr/winvalLexer.py` & `winval-0.6.3/winval/antlr/winvalLexer.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/antlr/winvalLexer.tokens` & `winval-0.6.3/winval/antlr/winvalLexer.tokens`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/antlr/winvalListener.py` & `winval-0.6.3/winval/antlr/winvalListener.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/antlr/winvalParser.py` & `winval-0.6.3/winval/antlr/winvalParser.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/antlr/winvalVisitor.py` & `winval-0.6.3/winval/antlr/winvalVisitor.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/cloud_files_validator.py` & `winval-0.6.3/winval/cloud_files_validator.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/constraint_eval.py` & `winval-0.6.3/winval/constraint_eval.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/constraints_pre_processor.py` & `winval-0.6.3/winval/constraints_pre_processor.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/parsed_workflow_inputs.py` & `winval-0.6.3/winval/parsed_workflow_inputs.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/python_extensions.py` & `winval-0.6.3/winval/python_extensions.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/validate_wdl_constraints.py` & `winval-0.6.3/winval/validate_wdl_constraints.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/wdl_parser.py` & `winval-0.6.3/winval/wdl_parser.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/winval.g4` & `winval-0.6.3/winval/winval.g4`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/winval_class.py` & `winval-0.6.3/winval/winval_class.py`

 * *Files identical despite different names*

### Comparing `winval-0.6.2/winval/workflow_var.py` & `winval-0.6.3/winval/workflow_var.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,19 @@
     BOOLEAN = auto()
     STRING_ARRAY = auto()
     INT_ARRAY = auto()
     FLOAT_ARRAY = auto()
     FILE_ARRAY = auto()
     BOOLEAN_ARRAY = auto()
     FILE_MATRIX = auto()
+    FLOAT_MATRIX = auto()
+    INT_MATRIX = auto()
+    STRING_MATRIX = auto()
+    FLOAT_PAIRS = auto()
+    INT_PAIRS = auto()
     STRUCT = auto()
     MAP = auto()
     PAIR = auto()
 
     @staticmethod
     def from_string(string: str):
         if string == 'String':
@@ -39,14 +44,24 @@
             return WorkflowVarType.FLOAT_ARRAY
         elif string == 'Array[File]':
             return WorkflowVarType.FILE_ARRAY
         elif string == 'Array[Boolean]':
             return WorkflowVarType.BOOLEAN_ARRAY
         elif string == 'Array[Array[File]]':
             return WorkflowVarType.FILE_MATRIX
+        elif string == 'Array[Array[Float]]':
+            return WorkflowVarType.FLOAT_MATRIX
+        elif string == 'Array[Array[Int]]':
+            return WorkflowVarType.INT_MATRIX
+        elif string == 'Array[Array[String]]':
+            return WorkflowVarType.STRING_MATRIX
+        elif string == 'Array[Pair[Float]]':
+            return WorkflowVarType.FLOAT_PAIRS
+        elif string == 'Array[Pair[Float]]':
+            return WorkflowVarType.INT_PAIRS
         elif string.startswith('Map'):
             return WorkflowVarType.MAP
         elif string.startswith('Pair'):
             return WorkflowVarType.PAIR
         else:
             raise ValueError(f'No such WorkflowVarType: {string}')
 
@@ -97,15 +112,16 @@
                 return False
             else:
                 logger.warning(f'Ignore parsing complex default bool expression {self.type} {self.name} {value}')
                 return None
         if self.type in {WorkflowVarType.STRING_ARRAY,
                          WorkflowVarType.FILE_ARRAY,
                          WorkflowVarType.INT_ARRAY,
-                         WorkflowVarType.BOOLEAN_ARRAY}:
+                         WorkflowVarType.BOOLEAN_ARRAY,
+                         WorkflowVarType.FLOAT_ARRAY}:
             if value[0] not in {'['}:
                 logger.warning(f'Ignore parsing complex default array value {self.type} {self.name} {value}')
                 return None
             if value == '[]':
                 return []
             else:
                 str_array = value.strip('][ ').split(',')
```

### Comparing `winval-0.6.2/PKG-INFO` & `winval-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winval
-Version: 0.6.2
+Version: 0.6.3
 Summary: WDL workflow inputs validation
 License: Apache-2.0
 Author: doron
 Author-email: doron.shemtov@ultimagen.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

