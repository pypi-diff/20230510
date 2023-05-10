# Comparing `tmp/pysmali-0.1.1.tar.gz` & `tmp/pysmali-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmali-0.1.1.tar", last modified: Wed Mar 22 13:14:16 2023, max compression
+gzip compressed data, was "pysmali-0.1.2.tar", last modified: Wed May 10 07:59:36 2023, max compression
```

## Comparing `pysmali-0.1.1.tar` & `pysmali-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 13:14:16.256974 pysmali-0.1.1/
--rw-rw-rw-   0        0        0    35802 2023-03-15 06:06:42.000000 pysmali-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6108 2023-03-22 13:14:16.251958 pysmali-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5177 2023-03-22 12:45:31.000000 pysmali-0.1.1/README.md
--rw-rw-rw-   0        0        0      950 2023-03-22 12:45:31.000000 pysmali-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-22 13:14:15.816162 pysmali-0.1.1/pysmali.egg-info/
--rw-rw-rw-   0        0        0     6108 2023-03-22 13:14:15.000000 pysmali-0.1.1/pysmali.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-03-22 13:14:15.000000 pysmali-0.1.1/pysmali.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 13:14:15.000000 pysmali-0.1.1/pysmali.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-03-22 13:14:15.000000 pysmali-0.1.1/pysmali.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-03-22 13:14:15.000000 pysmali-0.1.1/pysmali.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 13:14:16.259962 pysmali-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-22 13:14:15.936962 pysmali-0.1.1/smali/
--rw-rw-rw-   0        0        0     1012 2023-03-18 09:43:56.000000 pysmali-0.1.1/smali/__init__.py
--rw-rw-rw-   0        0        0    20853 2023-03-22 13:05:26.000000 pysmali-0.1.1/smali/base.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:14:16.126962 pysmali-0.1.1/smali/bridge/
--rw-rw-rw-   0        0        0      909 2023-03-16 06:04:01.000000 pysmali-0.1.1/smali/bridge/__init__.py
--rw-rw-rw-   0        0        0     1937 2023-03-18 17:34:08.000000 pysmali-0.1.1/smali/bridge/errors.py
--rw-rw-rw-   0        0        0    23589 2023-03-22 12:23:53.000000 pysmali-0.1.1/smali/bridge/executor.py
--rw-rw-rw-   0        0        0     3616 2023-03-18 17:34:15.000000 pysmali-0.1.1/smali/bridge/frame.py
--rw-rw-rw-   0        0        0    27708 2023-03-19 18:12:23.000000 pysmali-0.1.1/smali/bridge/lang.py
--rw-rw-rw-   0        0        0     1133 2023-03-22 12:37:08.000000 pysmali-0.1.1/smali/bridge/objects.py
--rw-rw-rw-   0        0        0    16857 2023-03-18 17:33:09.000000 pysmali-0.1.1/smali/bridge/vm.py
--rw-rw-rw-   0        0        0     8936 2023-03-16 06:04:01.000000 pysmali-0.1.1/smali/opcode.py
--rw-rw-rw-   0        0        0    34209 2023-03-22 12:46:18.000000 pysmali-0.1.1/smali/reader.py
-drwxrwxrwx   0        0        0        0 2023-03-22 13:14:16.218958 pysmali-0.1.1/smali/shell/
--rw-rw-rw-   0        0        0     1356 2023-03-18 17:29:22.000000 pysmali-0.1.1/smali/shell/__init__.py
--rw-rw-rw-   0        0        0      854 2023-03-18 17:25:00.000000 pysmali-0.1.1/smali/shell/__main__.py
--rw-rw-rw-   0        0        0     2101 2023-03-22 11:34:16.000000 pysmali-0.1.1/smali/shell/cli.py
--rw-rw-rw-   0        0        0    10070 2023-03-22 12:43:45.000000 pysmali-0.1.1/smali/shell/model.py
--rw-rw-rw-   0        0        0    15957 2023-03-18 17:35:14.000000 pysmali-0.1.1/smali/visitor.py
--rw-rw-rw-   0        0        0    21881 2023-03-18 17:35:19.000000 pysmali-0.1.1/smali/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:59:36.529793 pysmali-0.1.2/
+-rw-rw-rw-   0        0        0    35802 2023-03-15 06:06:42.000000 pysmali-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6104 2023-05-10 07:59:36.530793 pysmali-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5327 2023-05-10 07:42:34.000000 pysmali-0.1.2/README.md
+-rw-rw-rw-   0        0        0      948 2023-05-10 07:42:34.000000 pysmali-0.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-10 07:59:35.750539 pysmali-0.1.2/pysmali.egg-info/
+-rw-rw-rw-   0        0        0     6104 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 07:59:35.000000 pysmali-0.1.2/pysmali.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 07:59:36.538794 pysmali-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 07:59:36.017443 pysmali-0.1.2/smali/
+-rw-rw-rw-   0        0        0     1012 2023-03-18 09:43:56.000000 pysmali-0.1.2/smali/__init__.py
+-rw-rw-rw-   0        0        0    20973 2023-05-10 07:03:11.000000 pysmali-0.1.2/smali/base.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:59:36.262279 pysmali-0.1.2/smali/bridge/
+-rw-rw-rw-   0        0        0      909 2023-03-16 06:04:01.000000 pysmali-0.1.2/smali/bridge/__init__.py
+-rw-rw-rw-   0        0        0     1972 2023-05-10 06:59:41.000000 pysmali-0.1.2/smali/bridge/errors.py
+-rw-rw-rw-   0        0        0    24171 2023-05-10 07:53:40.000000 pysmali-0.1.2/smali/bridge/executor.py
+-rw-rw-rw-   0        0        0     3608 2023-05-10 06:58:48.000000 pysmali-0.1.2/smali/bridge/frame.py
+-rw-rw-rw-   0        0        0    28077 2023-05-10 07:56:30.000000 pysmali-0.1.2/smali/bridge/lang.py
+-rw-rw-rw-   0        0        0     1133 2023-03-22 12:37:08.000000 pysmali-0.1.2/smali/bridge/objects.py
+-rw-rw-rw-   0        0        0    18379 2023-05-10 07:58:29.000000 pysmali-0.1.2/smali/bridge/vm.py
+-rw-rw-rw-   0        0        0     8936 2023-03-16 06:04:01.000000 pysmali-0.1.2/smali/opcode.py
+-rw-rw-rw-   0        0        0    34770 2023-05-10 07:04:22.000000 pysmali-0.1.2/smali/reader.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:59:36.367277 pysmali-0.1.2/smali/shell/
+-rw-rw-rw-   0        0        0     1356 2023-03-18 17:29:22.000000 pysmali-0.1.2/smali/shell/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-03-18 17:25:00.000000 pysmali-0.1.2/smali/shell/__main__.py
+-rw-rw-rw-   0        0        0     2274 2023-05-10 06:59:52.000000 pysmali-0.1.2/smali/shell/cli.py
+-rw-rw-rw-   0        0        0    10014 2023-05-10 06:57:18.000000 pysmali-0.1.2/smali/shell/model.py
+-rw-rw-rw-   0        0        0    16049 2023-05-10 07:04:38.000000 pysmali-0.1.2/smali/visitor.py
+-rw-rw-rw-   0        0        0    22486 2023-05-10 07:36:02.000000 pysmali-0.1.2/smali/writer.py
```

### Comparing `pysmali-0.1.1/LICENSE` & `pysmali-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.1/PKG-INFO` & `pysmali-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmali
-Version: 0.1.1
+Version: 0.1.2
 Summary: Smali Visitor-API and Smali emulator
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/pysmali
 Project-URL: API-Docs, https://pysmali.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,19 +19,18 @@
 # PySmali
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=03/18/2023&color=9cf)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=lightgreen)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
 [![Documentation Status](https://readthedocs.org/projects/pysmali/badge/?version=latest)](https://pysmali.readthedocs.io/en/latest/?badge=latest)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.1&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.2&color=lightblue)
 
 
-The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interace interpreter provided that
-acts as a Python-CLI.
+The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
 
 
 ## Installation
 
 By now, the only way to install the python module in this repository is by cloning it and running the following command:
 
 ```bash
@@ -42,15 +41,15 @@
 
 ## Usage
 
 For a more detailed explanation of the Smali Visitor-API use the [docs](https://pysmali.readthedocs.io/).
 
 ### ISmali (Interactive Smali Interpreter)
 
-As of version `0.1.1` the interactive interpreter can be used to execute Smali code directly:
+As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
 
 ```bash
 $ ismali example.ssf
 # or start interactive mode
 $ ismali
 >>> vars
 {'p0': <SmaliObject@195f5c0da90>}
@@ -92,15 +91,15 @@
 Actually, the code above does nothing as the `ClassVisitor` class does not handle any notification by the reader. For instance, to print out the class name of a parsed code, the following implementation could be used:
 
 ```python
 from smali import SmaliReader, ClassVisitor, Type
 
 class NamePrinterVisitor(ClassVisitor):
     def visit_class(self, name: str, access_flags: int) -> None:
-        # The provided name is the type descriptor, so we have to 
+        # The provided name is the type descriptor, so we have to
         # convert it:
         cls_type = Type(name)
         print('ClassName:', cls_type.class_name)
 
 reader = SmaliReader()
 reader.visit(".class public final Lcom/example/Hello;", NamePrinterVisitor())
 ```
@@ -136,36 +135,36 @@
 # create the finished source code, BUT don't forget visit_end()
 writer.visit_end()
 text = writer.code
 ```
 
 ### Importing classes and execute methods
 
-As of version `0.1.1` you can import Smali files and execute defined methods:
+As of version `0.1.2` you can import Smali files and execute defined methods:
 
 ```python
 from smali.bridge import SmaliVM, SmaliObject
 
 with open('example.smali', 'r', encoding='utf-8') as fp:
     source = fp.read()
-    
+
 vm = SmaliVM()
 # Import class definition
 smali_class = vm.classloader.load_class(source, init=False)
 # Call <clinit> method
 smali_class.clinit()
 
 # Create a new instance of the imported class
 instance = SmaliObject(smali_class)
 # Call the object's constructor
 instance.init()
 
 # Execute the method 'toString'
 toString = instance.smali_class.method("toString")
-# The instance must be always the first element (on 
+# The instance must be always the first element (on
 # static methods this argument must be None)
 value = toString(instance)
 print(value)
 ```
 
 ## License
```

### Comparing `pysmali-0.1.1/README.md` & `pysmali-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,154 +1,153 @@
-# PySmali
-
-[![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
-![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=03/18/2023&color=9cf)
-![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=lightgreen)
-![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
-[![Documentation Status](https://readthedocs.org/projects/pysmali/badge/?version=latest)](https://pysmali.readthedocs.io/en/latest/?badge=latest)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.1&color=lightblue)
-
-
-The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interace interpreter provided that
-acts as a Python-CLI.
-
-
-## Installation
-
-By now, the only way to install the python module in this repository is by cloning it and running the following command:
-
-```bash
-$ cd ./pysmali && pip install .
-# Or with pip
-$ pip install pysmali
-```
-
-## Usage
-
-For a more detailed explanation of the Smali Visitor-API use the [docs](https://pysmali.readthedocs.io/).
-
-### ISmali (Interactive Smali Interpreter)
-
-As of version `0.1.1` the interactive interpreter can be used to execute Smali code directly:
-
-```bash
-$ ismali example.ssf
-# or start interactive mode
-$ ismali
->>> vars
-{'p0': <SmaliObject@195f5c0da90>}
-```
-
-Some notes:
-
-* ``p0``: This register always stores the root-instance where defined fields and methods will be stored.
-* ``vars``: This command can be used to print all registers together with their values
-* `L<Root>;`: The name of the root-context class
-
-The API [documentation](https://pysmali.readthedocs.io/) provides some usage examples and usage hints.
-
-### Parsing Smali-Files
-
-The simplest way to parse code is to use a `SmaliReader` together with a visitor:
-
-```python
-from smali import SmaliReader, ClassVisitor
-
-code = """
-.class public final Lcom/example/Hello;
-.super Ljava/lang/Object;
-# One line comment
-.source "SourceFile" # EOL comment
-"""
-
-reader = SmaliReader()
-reader.visit(code, ClassVisitor())
-```
-
-There are a few options to have in mind when parsing with a `SmaliReader`:
-
-* `comments`: To explicitly parse comments, set this variable to True (in constructor or directly)
-* `snippet`: To parse simple code snippets without a .class definition, use the 'snippet' variable (or within the constructor). Use this property only if you don't have a '.class' definition at the start of the source code
-* `validate`: Validates the parsed code
-* `errors`: With values `"strict"` or `"ignore"` this attribute will cause the reader to raise or ignore exceptions
-
-Actually, the code above does nothing as the `ClassVisitor` class does not handle any notification by the reader. For instance, to print out the class name of a parsed code, the following implementation could be used:
-
-```python
-from smali import SmaliReader, ClassVisitor, Type
-
-class NamePrinterVisitor(ClassVisitor):
-    def visit_class(self, name: str, access_flags: int) -> None:
-        # The provided name is the type descriptor, so we have to 
-        # convert it:
-        cls_type = Type(name)
-        print('ClassName:', cls_type.class_name)
-
-reader = SmaliReader()
-reader.visit(".class public final Lcom/example/Hello;", NamePrinterVisitor())
-```
-
-### Writing Smali-Files
-
-Writing is as simple as parsing files. To write the exact same document the has been parsed, the `SmaliWriter` class can be used as the visitor:
-
-```python
-from smali import SmaliReader, SmaliWriter
-
-reader = SmaliReader()
-writer = SmaliWriter()
-
-reader.visit(".class public final Lcom/example/Hello;", writer)
-# The source code can be retrieved via a property
-text = writer.code
-```
-
-To create own Smali files, the pre-defined `SmaliWriter` can be used again:
-
-```python
-from smali import SmaliWriter, AccessType
-
-writer = SmaliWriter()
-# create the class definition
-writer.visit_class("Lcom/example/Hello;", AccessType.PUBLIC + AccessType.FINAL)
-writer.visit_super("Ljava/lang/Object;")
-
-# create a field
-field_writer = writer.visit_field("foo", AccessType.PRIVATE, "Ljava/lang/String")
-
-# create the finished source code, BUT don't forget visit_end()
-writer.visit_end()
-text = writer.code
-```
-
-### Importing classes and execute methods
-
-As of version `0.1.1` you can import Smali files and execute defined methods:
-
-```python
-from smali.bridge import SmaliVM, SmaliObject
-
-with open('example.smali', 'r', encoding='utf-8') as fp:
-    source = fp.read()
-    
-vm = SmaliVM()
-# Import class definition
-smali_class = vm.classloader.load_class(source, init=False)
-# Call <clinit> method
-smali_class.clinit()
-
-# Create a new instance of the imported class
-instance = SmaliObject(smali_class)
-# Call the object's constructor
-instance.init()
-
-# Execute the method 'toString'
-toString = instance.smali_class.method("toString")
-# The instance must be always the first element (on 
-# static methods this argument must be None)
-value = toString(instance)
-print(value)
-```
-
-## License
-
-Distributed under the GNU GPLv3. See `LICENSE` for more information.
+# PySmali
+
+[![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
+![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=03/18/2023&color=9cf)
+![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=lightgreen)
+![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
+[![Documentation Status](https://readthedocs.org/projects/pysmali/badge/?version=latest)](https://pysmali.readthedocs.io/en/latest/?badge=latest)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.2&color=lightblue)
+
+
+The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
+
+
+## Installation
+
+By now, the only way to install the python module in this repository is by cloning it and running the following command:
+
+```bash
+$ cd ./pysmali && pip install .
+# Or with pip
+$ pip install pysmali
+```
+
+## Usage
+
+For a more detailed explanation of the Smali Visitor-API use the [docs](https://pysmali.readthedocs.io/).
+
+### ISmali (Interactive Smali Interpreter)
+
+As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
+
+```bash
+$ ismali example.ssf
+# or start interactive mode
+$ ismali
+>>> vars
+{'p0': <SmaliObject@195f5c0da90>}
+```
+
+Some notes:
+
+* ``p0``: This register always stores the root-instance where defined fields and methods will be stored.
+* ``vars``: This command can be used to print all registers together with their values
+* `L<Root>;`: The name of the root-context class
+
+The API [documentation](https://pysmali.readthedocs.io/) provides some usage examples and usage hints.
+
+### Parsing Smali-Files
+
+The simplest way to parse code is to use a `SmaliReader` together with a visitor:
+
+```python
+from smali import SmaliReader, ClassVisitor
+
+code = """
+.class public final Lcom/example/Hello;
+.super Ljava/lang/Object;
+# One line comment
+.source "SourceFile" # EOL comment
+"""
+
+reader = SmaliReader()
+reader.visit(code, ClassVisitor())
+```
+
+There are a few options to have in mind when parsing with a `SmaliReader`:
+
+* `comments`: To explicitly parse comments, set this variable to True (in constructor or directly)
+* `snippet`: To parse simple code snippets without a .class definition, use the 'snippet' variable (or within the constructor). Use this property only if you don't have a '.class' definition at the start of the source code
+* `validate`: Validates the parsed code
+* `errors`: With values `"strict"` or `"ignore"` this attribute will cause the reader to raise or ignore exceptions
+
+Actually, the code above does nothing as the `ClassVisitor` class does not handle any notification by the reader. For instance, to print out the class name of a parsed code, the following implementation could be used:
+
+```python
+from smali import SmaliReader, ClassVisitor, Type
+
+class NamePrinterVisitor(ClassVisitor):
+    def visit_class(self, name: str, access_flags: int) -> None:
+        # The provided name is the type descriptor, so we have to
+        # convert it:
+        cls_type = Type(name)
+        print('ClassName:', cls_type.class_name)
+
+reader = SmaliReader()
+reader.visit(".class public final Lcom/example/Hello;", NamePrinterVisitor())
+```
+
+### Writing Smali-Files
+
+Writing is as simple as parsing files. To write the exact same document the has been parsed, the `SmaliWriter` class can be used as the visitor:
+
+```python
+from smali import SmaliReader, SmaliWriter
+
+reader = SmaliReader()
+writer = SmaliWriter()
+
+reader.visit(".class public final Lcom/example/Hello;", writer)
+# The source code can be retrieved via a property
+text = writer.code
+```
+
+To create own Smali files, the pre-defined `SmaliWriter` can be used again:
+
+```python
+from smali import SmaliWriter, AccessType
+
+writer = SmaliWriter()
+# create the class definition
+writer.visit_class("Lcom/example/Hello;", AccessType.PUBLIC + AccessType.FINAL)
+writer.visit_super("Ljava/lang/Object;")
+
+# create a field
+field_writer = writer.visit_field("foo", AccessType.PRIVATE, "Ljava/lang/String")
+
+# create the finished source code, BUT don't forget visit_end()
+writer.visit_end()
+text = writer.code
+```
+
+### Importing classes and execute methods
+
+As of version `0.1.2` you can import Smali files and execute defined methods:
+
+```python
+from smali.bridge import SmaliVM, SmaliObject
+
+with open('example.smali', 'r', encoding='utf-8') as fp:
+    source = fp.read()
+
+vm = SmaliVM()
+# Import class definition
+smali_class = vm.classloader.load_class(source, init=False)
+# Call <clinit> method
+smali_class.clinit()
+
+# Create a new instance of the imported class
+instance = SmaliObject(smali_class)
+# Call the object's constructor
+instance.init()
+
+# Execute the method 'toString'
+toString = instance.smali_class.method("toString")
+# The instance must be always the first element (on
+# static methods this argument must be None)
+value = toString(instance)
+print(value)
+```
+
+## License
+
+Distributed under the GNU GPLv3. See `LICENSE` for more information.
```

### Comparing `pysmali-0.1.1/pyproject.toml` & `pysmali-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "pysmali"
-version = "0.1.1"
+version = "0.1.2"
 description="Smali Visitor-API and Smali emulator"
 authors = [
   { name="MatrixEditor", email="not@supported.com" },
 ]
 readme = "README.md"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Science/Research',
-    'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',  
+    'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 ]
```

### Comparing `pysmali-0.1.1/pysmali.egg-info/PKG-INFO` & `pysmali-0.1.2/pysmali.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysmali
-Version: 0.1.1
+Version: 0.1.2
 Summary: Smali Visitor-API and Smali emulator
 Author-email: MatrixEditor <not@supported.com>
 Project-URL: Homepage, https://github.com/MatrixEditor/pysmali
 Project-URL: API-Docs, https://pysmali.readthedocs.io/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,19 +19,18 @@
 # PySmali
 
 [![python](https://img.shields.io/badge/python-3.8+-blue.svg?logo=python&labelColor=lightgrey)](https://www.python.org/downloads/)
 ![LastEdit](https://img.shields.io:/static/v1?label=LastEdit&message=03/18/2023&color=9cf)
 ![Status](https://img.shields.io:/static/v1?label=Status&message=Pre-Release&color=lightgreen)
 ![Platform](https://img.shields.io:/static/v1?label=Platforms&message=Linux|Windows&color=yellowgreen)
 [![Documentation Status](https://readthedocs.org/projects/pysmali/badge/?version=latest)](https://pysmali.readthedocs.io/en/latest/?badge=latest)
-![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.1&color=lightblue)
+![PyPi](https://img.shields.io:/static/v1?label=PyPi&message=0.1.2&color=lightblue)
 
 
-The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interace interpreter provided that
-acts as a Python-CLI.
+The main functionalities of this repository cover creating and parsing Smali files with Python3 as well as interpret Smali source code files. There is also an interactive interpreter provided that acts as a Python-CLI.
 
 
 ## Installation
 
 By now, the only way to install the python module in this repository is by cloning it and running the following command:
 
 ```bash
@@ -42,15 +41,15 @@
 
 ## Usage
 
 For a more detailed explanation of the Smali Visitor-API use the [docs](https://pysmali.readthedocs.io/).
 
 ### ISmali (Interactive Smali Interpreter)
 
-As of version `0.1.1` the interactive interpreter can be used to execute Smali code directly:
+As of version `0.1.2` the interactive interpreter can be used to execute Smali code directly:
 
 ```bash
 $ ismali example.ssf
 # or start interactive mode
 $ ismali
 >>> vars
 {'p0': <SmaliObject@195f5c0da90>}
@@ -92,15 +91,15 @@
 Actually, the code above does nothing as the `ClassVisitor` class does not handle any notification by the reader. For instance, to print out the class name of a parsed code, the following implementation could be used:
 
 ```python
 from smali import SmaliReader, ClassVisitor, Type
 
 class NamePrinterVisitor(ClassVisitor):
     def visit_class(self, name: str, access_flags: int) -> None:
-        # The provided name is the type descriptor, so we have to 
+        # The provided name is the type descriptor, so we have to
         # convert it:
         cls_type = Type(name)
         print('ClassName:', cls_type.class_name)
 
 reader = SmaliReader()
 reader.visit(".class public final Lcom/example/Hello;", NamePrinterVisitor())
 ```
@@ -136,36 +135,36 @@
 # create the finished source code, BUT don't forget visit_end()
 writer.visit_end()
 text = writer.code
 ```
 
 ### Importing classes and execute methods
 
-As of version `0.1.1` you can import Smali files and execute defined methods:
+As of version `0.1.2` you can import Smali files and execute defined methods:
 
 ```python
 from smali.bridge import SmaliVM, SmaliObject
 
 with open('example.smali', 'r', encoding='utf-8') as fp:
     source = fp.read()
-    
+
 vm = SmaliVM()
 # Import class definition
 smali_class = vm.classloader.load_class(source, init=False)
 # Call <clinit> method
 smali_class.clinit()
 
 # Create a new instance of the imported class
 instance = SmaliObject(smali_class)
 # Call the object's constructor
 instance.init()
 
 # Execute the method 'toString'
 toString = instance.smali_class.method("toString")
-# The instance must be always the first element (on 
+# The instance must be always the first element (on
 # static methods this argument must be None)
 value = toString(instance)
 print(value)
 ```
 
 ## License
```

### Comparing `pysmali-0.1.1/pysmali.egg-info/SOURCES.txt` & `pysmali-0.1.2/pysmali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.1/smali/__init__.py` & `pysmali-0.1.2/smali/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.1/smali/base.py` & `pysmali-0.1.2/smali/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,16 @@
 Basic component classes when working with the Smali language.
 """
 
 import re
 
 from enum import Enum, IntFlag
 
-__all__ = [
-    'AccessType', 'Token', 'Line', 'Type',
-    'smali_value', 'SmaliValueProxy'
-]
+__all__ = ["AccessType", "Token", "Line", "Type", "smali_value", "SmaliValueProxy"]
+
 
 class AccessType(IntFlag):
     """Contains all access modifiers for classes, fields, methods and annotations.
 
     There is also a possibility to use values of this class with an ``in``
     statement:
 
@@ -74,15 +72,15 @@
         result = 0
         for element in values:
             if not element:
                 continue
 
             element = str(element).lower()
             for val in AccessType:
-                if val.name.lower().replace('_', '-') == element:
+                if val.name.lower().replace("_", "-") == element:
                     result |= val.value
         return result
 
     @staticmethod
     def get_names(flags: int) -> list:
         """Converts the given access modifiers to a human readable representation.
 
@@ -90,39 +88,40 @@
         :type flags: int
         :return: a list of keywords
         :rtype: list
         """
         result = []
         for val in AccessType:
             if flags in val:
-                result.append(val.name.lower().replace('_', '-'))
+                result.append(val.name.lower().replace("_", "-"))
         return result
 
     @staticmethod
     def find(value: str) -> bool:
         """Returns whether the given keyword is a valid modifier.
 
         :param value: the value to check
         :type value: str
         :return: True, if the given value represents an access modifier
         :rtype: bool
         """
         for val in AccessType:
-            name = val.name.lower().replace('_', '-')
+            name = val.name.lower().replace("_", "-")
             if name == value:
                 return True
         return False
 
     def __contains__(self, other: int) -> bool:
         if isinstance(other, self.__class__):
             return super().__contains__(other)
         if isinstance(other, int):
             return self.value & other != 0
         raise TypeError(f"Unsupported type: {type(other)}")
 
+
 class Token(Enum):
     """Defines all common token in a Smali file.
 
     There are some special methods implemented to use constants of this
     class in the following situations:
 
     >>> "annotation" == Token.ANNOTATION
@@ -131,37 +130,37 @@
     True
     >>> len(Token.ENUM)
     4
     >>> str(Token.ARRAYDATA)
     'array-data'
     """
 
-    ANNOTATION = 'annotation'
-    ARRAYDATA = 'array-data'
-    CATCH = 'catch'
-    CATCHALL = 'catchall'
-    CLASS = 'class'
-    END = 'end'
-    ENUM = 'enum'
-    FIELD = 'field'
-    IMPLEMENTS = 'implements'
-    LINE = 'line'
-    LOCAL = 'local'
-    LOCALS = 'locals'
-    METHOD = 'method'
-    PACKEDSWITCH = 'packed-switch'
-    PARAM = 'param'
-    PROLOGUE = 'prologue'
-    REGISTERS = 'registers'
-    RESTART = 'restart'
-    SOURCE = 'source'
-    SPARSESWITCH = 'sparse-switch'
-    SUBANNOTATION = 'subannotation'
-    SUPER = 'super'
-    DEBUG = 'debug'
+    ANNOTATION = "annotation"
+    ARRAYDATA = "array-data"
+    CATCH = "catch"
+    CATCHALL = "catchall"
+    CLASS = "class"
+    END = "end"
+    ENUM = "enum"
+    FIELD = "field"
+    IMPLEMENTS = "implements"
+    LINE = "line"
+    LOCAL = "local"
+    LOCALS = "locals"
+    METHOD = "method"
+    PACKEDSWITCH = "packed-switch"
+    PARAM = "param"
+    PROLOGUE = "prologue"
+    REGISTERS = "registers"
+    RESTART = "restart"
+    SOURCE = "source"
+    SPARSESWITCH = "sparse-switch"
+    SUBANNOTATION = "subannotation"
+    SUPER = "super"
+    DEBUG = "debug"
 
     def __eq__(self, other: str) -> bool:
         if isinstance(other, self.__class__):
             return super().__eq__(other)
         return self.value == other
 
     def __ne__(self, other: str) -> bool:
@@ -171,14 +170,15 @@
 
     def __len__(self) -> int:
         return len(str(self.value))
 
     def __str__(self) -> str:
         return self.value
 
+
 class Line:
     """Simple peekable Iterator implementation."""
 
     RE_EOL_COMMENT = re.compile(r"\s*#.*")
     """Pattern for EOL (end of line) comments"""
 
     _default = object()
@@ -233,15 +233,15 @@
         self.cleaned = self.raw.lstrip()
         eol_match = Line.RE_EOL_COMMENT.search(self.cleaned)
         if eol_match is not None:
             start, end = eol_match.span()
             # Remove the EOL comment and save it in a variable. Note
             # that the visitor will be notified when StopIteration is
             # raised.
-            self.eol_comment = eol_match.group(0).lstrip('# ')
+            self.eol_comment = eol_match.group(0).lstrip("# ")
             self.cleaned = self.cleaned[:start] + self.cleaned[end:]
 
         self._elements = Line.split_line(self.cleaned)
         self._it = iter(self._elements)
         self._head = self._get_next()
 
     def peek(self, default: str = _default) -> str:
@@ -288,15 +288,15 @@
         """
         return self.__bool__()
 
     def __len__(self) -> int:
         return len(self.cleaned)
 
     @staticmethod
-    def split_line(cleaned: str, sep: str = ' ') -> list:
+    def split_line(cleaned: str, sep: str = " ") -> list:
         """Splits the line by the given delimiter and ignores values in strings
 
         :param cleaned: the input string
         :type cleaned: str
         :param sep: the delimiter, defaults to ' '
         :type sep: str, optional
         :return: the splitted values
@@ -304,38 +304,38 @@
         """
         end = cleaned.find(sep)
         start = 0
         in_literal = False
         elements = []
 
         while end != -1:
-            if end-1 > 0 and cleaned[end-1] == '"':
+            if end - 1 > 0 and cleaned[end - 1] == '"':
                 in_literal = False
                 elements.append(cleaned[start:end])
-                start = end+1
+                start = end + 1
 
             elif cleaned[start] == '"':
                 in_literal = True
 
             elif not in_literal:
                 elements.append(cleaned[start:end])
                 start = end + 1
 
-            end = cleaned.find(sep, end+1)
+            end = cleaned.find(sep, end + 1)
         elements.append(cleaned[start:])
         return elements
 
+
 class Type:
-    """Basic type definition that can handle both class and method types.
-    """
+    """Basic type definition that can handle both class and method types."""
 
-    CLINIT = '<clinit>'
+    CLINIT = "<clinit>"
     """Static block initializer"""
 
-    INIT = '<init>'
+    INIT = "<init>"
     """Constructor method"""
 
     def __init__(self, signature: str) -> None:
         self.__signature = signature
         if isinstance(signature, type):
             self.__signature = f"{signature.__module__}.{signature.__name__}"
 
@@ -346,96 +346,97 @@
         :return: the type descriptor used in the DVM (e.g. "Lcom/example/ABC;")
         :rtype: str
         """
         name = self.__signature
         if SmaliValueProxy.RE_TYPE_VALUE.match(name):
             return name
 
-        if name.startswith('['):
-            idx = name.rfind('[')
-            prefix = name[ :idx]
-            if not name.endswith(';') and name not in "ZCBSIFVJD":
+        if name.startswith("["):
+            idx = name.rfind("[")
+            prefix = name[:idx]
+            if not name.endswith(";") and name not in "ZCBSIFVJD":
                 return prefix + f"L{name[idx+1:].replace('.', '/')};"
 
             return prefix + f"{name[idx+1:].replace('.', '/')}"
 
         name = f"{name.replace('.', '/')}"
-        if name[-1] != ';' and name not in "ZCBSIFVJD":
+        if name[-1] != ";" and name not in "ZCBSIFVJD":
             name = f"L{name};"
         return name
 
     @property
     def type_name(self) -> str:
         """Returns the type name without 'L' and ';'
 
         :return: the type name
         :rtype: str
         """
         if not SmaliValueProxy.RE_TYPE_VALUE.match(self.__signature):
             return self.__signature
-        name = self.__signature.lstrip('[').replace('.', '/')
-        return name.lstrip('L').rstrip(';')
+        name = self.__signature.lstrip("[").replace(".", "/")
+        return name.lstrip("L").rstrip(";")
 
     @property
     def class_name(self) -> str:
         """Returns the Smali class name equivalent to Smali class names.
 
         :return: the class name (e.g. "com.example.ABC")
         :rtype: str
         """
-        return self.type_name.replace('/', '.').replace('[', '')
+        return self.type_name.replace("/", ".").replace("[", "")
 
     def get_method_name(self) -> str:
         """Returns the method name
 
         :return: the absolute method name
         :rtype: str
         """
-        idx = self.__signature.find('(')
+        idx = self.__signature.find("(")
         if idx == -1:
             raise TypeError(
-                f'Invalid method signature: could not find name ({self.__signature})')
+                f"Invalid method signature: could not find name ({self.__signature})"
+            )
 
         # Handle bracket names if not <clinit> or <init>
         name = self.__signature[:idx]
         if name in (Type.INIT, Type.CLINIT):
             return name
-        return name.rstrip('>').lstrip('<')
+        return name.rstrip(">").lstrip("<")
 
     def get_method_params(self) -> list:
         """Returns the method parameter internal names.
 
         :return: the method parameters
         :rtype: list
         """
-        start = self.__signature.find('(')
-        end = self.__signature.find(')')
+        start = self.__signature.find("(")
+        end = self.__signature.find(")")
         if start == -1 or end == -1:
-            raise TypeError('Invalid method signature')
+            raise TypeError("Invalid method signature")
 
-        params = self.__signature[start+1:end]
+        params = self.__signature[start + 1 : end]
         if not params:
             return []
 
         param_list = []
         idx = 0
         is_type = False
         current = ""
         while idx < len(params):
-            if params[idx] == 'L':
+            if params[idx] == "L":
                 is_type = True
-            elif params[idx] == ';':
+            elif params[idx] == ";":
                 is_type = False
-                current += ';'
+                current += ";"
                 param_list.append(current)
                 current = ""
                 idx += 1
                 continue
-            elif params[idx] == '[':
-                current += '['
+            elif params[idx] == "[":
+                current += "["
                 idx += 1
                 continue
 
             if is_type:
                 current += params[idx]
             else:
                 param_list.append(params[idx])
@@ -446,60 +447,61 @@
     def get_method_return_type(self) -> str:
         """Retrieves the method's return type
 
         :raises TypeError: if there is no valid return type
         :return: the return type's descriptor
         :rtype: str
         """
-        end = self.__signature.find(')')
+        end = self.__signature.find(")")
         if end == -1:
-            raise TypeError('Invalid method signature')
-        return self.__signature[end+1:]
+            raise TypeError("Invalid method signature")
+        return self.__signature[end + 1 :]
 
     def __str__(self) -> str:
         return self.__signature
 
-def smali_value(value: str) -> 'SmaliValueProxy':
+
+def smali_value(value: str) -> "SmaliValueProxy":
     """Parses the given string and returns its Smali value representation.
 
     :param value: the value as a string
     :type value: str
     :raises ValueError: if it has no valid Smali type
     :return: the Smali value representation
     :rtype: SmaliValueProxy
     """
     sm_value = SmaliValueProxy()
     sm_value.value = value
     sm_value.actual_value = None
     for i, entry in enumerate(SmaliValueProxy.TYPE_MAP):
         matcher, wrapper = entry
         if matcher.match(sm_value.value):
-            if i <= 3: # hex value possible
+            if i <= 3:  # hex value possible
                 hex_val = SmaliValueProxy.RE_HEX_VALUE.match(value) is not None
                 if not hex_val:
                     sm_value.actual_value = wrapper(value)
                 else:
                     sm_value.actual_value = wrapper(value, base=16)
             else:
                 sm_value.actual_value = wrapper(value)
             break
 
-
     # Handling of null values is not implemented yet
     if sm_value.actual_value is None:
         raise ValueError(f"Could not find any matching primitive type for {value}")
 
     sm_locals = {}
     for key in __smali_builtins__:
         if hasattr(sm_value.actual_value, key):
             sm_locals[key] = getattr(sm_value.actual_value, key)
 
     vars(sm_value).update(sm_locals)
     return sm_value
 
+
 class SmaliValueProxy:
     """Wrapper class for primitives in Smali.
 
     Use this class to retrieve the actual primitiva value for a parsed
     source code snippet. As this class overrides most of the internal
     special functions, objects of this class can be used as regualar
     strings or numeric values:
@@ -538,34 +540,34 @@
 
     RE_CHAR_VALUE = re.compile(r"^'.*'$")
     """Pattern for ``char`` values."""
 
     RE_STRING_VALUE = re.compile(r'^".*"$')
     """Pattern for ``String`` values."""
 
-    RE_TYPE_VALUE = re.compile(r"\[*((L\S*;$)|([ZCBSIFVJD])$)") # NOQA
+    RE_TYPE_VALUE = re.compile(r"\[*((L\S*;$)|([ZCBSIFVJD])$)")  # NOQA
     """Pattern for type descriptors."""
 
     RE_BOOL_VALUE = re.compile(r"true|false")
     """Pattern for ``boolean`` values."""
 
     RE_HEX_VALUE = re.compile(r"0x[\dabcdefABCDEF]+")
     """Pattern for integer values."""
 
     TYPE_MAP: list = [
         (RE_SHORT_VALUE, int),
         (RE_LONG_VALUE, int),
         (RE_BYTE_VALUE, int),
         (RE_INT_VALUE, int),
-        (RE_BOOL_VALUE, lambda x: x == 'true'),
+        (RE_BOOL_VALUE, lambda x: x == "true"),
         (RE_FLOAT_VALUE, float),
         (RE_DOUBLE_VALUE, float),
         (RE_CHAR_VALUE, lambda x: str(x[1:-1])),
         (RE_STRING_VALUE, lambda x: str(x[1:-1])),
-        (RE_TYPE_VALUE, Type)
+        (RE_TYPE_VALUE, Type),
     ]
     """Defines custom handlers for actual value defintions
 
     :meta private:
     """
 
     value: str
@@ -581,47 +583,47 @@
         :param value: the value to check
         :type value: str
         :return: True, if the value is a valid type descriptor
         :rtype: bool
         """
         return SmaliValueProxy.RE_TYPE_VALUE.match(value) is not None
 
+
 ####################################################################################
 # INTERNAL
 ####################################################################################
 
 __smali_builtins__ = [
-    "__contains__", "__eq__", "__ne__", "__len__", "__str__",
-    "__next__", "__bool__", "__repr__", "__str__", "__bytes__",
-    "__format__", "__lt__", "__le__", "__eq__", "__ne__", "__gt__", "__ge__",
-    "__hash__", "__bool__", "__len__", "__length_hint__", "__getitem__",
-    "__setitem__", "__delitem__", "__missing__", "__iter__", "__reversed__",
-    "__contains__", "__add__", "__sub__", "__mul__", "__truediv__",
-    "__floordiv__", "__mod__", "__divmod__", "__lshift__", "__rshift__",
-    "__and__", "__xor__", "__or__", "__radd__", "__rsub__", "__rmul__",
-    "__rtruediv__", "__rfloordiv__", "__rmod__", "__rdivmod__", "__rlshift__",
-    "__rrshift__", "__rand__", "__rxor__", "__ror__", "__neg__", "__pos__",
-    "__abs__", "__invert__", "__complex__", "__int__", "__float__", "__index__",
-    "__trunc__", "__floor__", "__ceil__",
+    "__contains__", "__eq__", "__ne__", "__len__", "__str__", "__next__", "__bool__",
+    "__repr__", "__str__", "__bytes__", "__format__", "__lt__", "__le__", "__eq__",
+    "__ne__", "__gt__", "__ge__", "__hash__", "__bool__", "__len__", "__length_hint__",
+    "__getitem__", "__setitem__", "__delitem__", "__missing__", "__iter__", "__reversed__",
+    "__contains__", "__add__", "__sub__", "__mul__", "__truediv__", "__floordiv__",
+    "__mod__", "__divmod__", "__lshift__", "__rshift__", "__and__", "__xor__", "__or__",
+    "__radd__", "__rsub__", "__rmul__", "__rtruediv__", "__rfloordiv__", "__rmod__",
+    "__rdivmod__", "__rlshift__", "__rrshift__", "__rand__", "__rxor__", "__ror__",
+    "__neg__", "__pos__", "__abs__", "__invert__", "__complex__", "__int__", "__float__",
+    "__index__", "__trunc__", "__floor__", "__ceil__",
 ]
 
 __smali_specials__ = [
-    ("__iadd__", lambda x,y: x.actual_value+y.actual_value),
-    ("__isub__", lambda x,y: x.actual_value-y.actual_value),
-    ("__imul__", lambda x,y: x.actual_value*y.actual_value),
-    ("__itruediv__", lambda x,y: x.actual_value/y.actual_value),
-    ("__ifloordiv__", lambda x,y: x.actual_value//y.actual_value),
-    ("__imod__", lambda x,y: x.actual_value%y.actual_value),
-    ("__ilshift__", lambda x,y: x.actual_value<<y.actual_value),
-    ("__irshift__", lambda x,y: x.actual_value>>y.actual_value),
-    ("__iand__", lambda x,y: x.actual_value&y.actual_value),
-    ("__ixor__", lambda x,y: x.actual_value^y.actual_value),
-    ("__ior__", lambda x,y: x.actual_value|y.actual_value)
+    ("__iadd__", lambda x, y: x.actual_value + y.actual_value),
+    ("__isub__", lambda x, y: x.actual_value - y.actual_value),
+    ("__imul__", lambda x, y: x.actual_value * y.actual_value),
+    ("__itruediv__", lambda x, y: x.actual_value / y.actual_value),
+    ("__ifloordiv__", lambda x, y: x.actual_value // y.actual_value),
+    ("__imod__", lambda x, y: x.actual_value % y.actual_value),
+    ("__ilshift__", lambda x, y: x.actual_value << y.actual_value),
+    ("__irshift__", lambda x, y: x.actual_value >> y.actual_value),
+    ("__iand__", lambda x, y: x.actual_value & y.actual_value),
+    ("__ixor__", lambda x, y: x.actual_value ^ y.actual_value),
+    ("__ior__", lambda x, y: x.actual_value | y.actual_value),
 ]
 
+
 def __wrap_args__(self, target: str, *args):
     """Tries to wrap ``SmalivalueProxy`` objects before calling the special method.
 
     :param target: the method to call
     :type target: str
     """
     if len(args) == 0:
@@ -635,23 +637,32 @@
         if isinstance(val, SmaliValueProxy):
             new_args.append(val.actual_value)
         else:
             new_args.append(val)
 
     return self.__dict__[target](*new_args)
 
+
 for method in __smali_builtins__:
-    setattr(SmaliValueProxy, method,
-        lambda self, *args, method=method: __wrap_args__(self, method, *args)
+    setattr(
+        SmaliValueProxy,
+        method,
+        lambda self, *args, method=method: __wrap_args__(self, method, *args),
     )
 
+
 def __wrap_special__(instance, actual_val, val, funct):
     funct(actual_val, val)
     return instance
 
+
 for method, func in __smali_specials__:
-    setattr(SmaliValueProxy, method,
-        lambda self, val, func=func: __wrap_special__(self, self.actual_value, val, func)
+    setattr(
+        SmaliValueProxy,
+        method,
+        lambda self, val, func=func: __wrap_special__(
+            self, self.actual_value, val, func
+        ),
     )
 
 del method
 del func
```

### Comparing `pysmali-0.1.1/smali/bridge/__init__.py` & `pysmali-0.1.2/smali/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.1/smali/bridge/errors.py` & `pysmali-0.1.2/smali/bridge/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,45 +14,56 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 __doc__ = """
 Common exceptions of the Smali-Python-Bridge
 """
 
 __all__ = [
-    'NoSuchClassError', 'NoSuchMethodError', 'NoSuchFieldError',
-    'NoSuchRegisterError', 'NoSuchOpcodeError', 'InvalidOpcodeError',
-    'ExecutionError'
+    "NoSuchClassError",
+    "NoSuchMethodError",
+    "NoSuchFieldError",
+    "NoSuchRegisterError",
+    "NoSuchOpcodeError",
+    "InvalidOpcodeError",
+    "ExecutionError",
 ]
 
+
 class NoSuchClassError(Exception):
     """The class is not defined or wasn't found"""
 
+
 class NoSuchMethodError(Exception):
     """The method is not defined"""
 
+
 class NoSuchFieldError(Exception):
     """The requested field is not defined"""
 
+
 class NoSuchRegisterError(Exception):
     """Unknown register was requested to be read"""
 
+
 class NoSuchOpcodeError(Exception):
     """The opcode does not exists or no implementation is present"""
 
+
 class InvalidOpcodeError(Exception):
     """The opcode is invalid"""
 
+
 class ExecutionError(Exception):
     """Wrapper class for runtime exceptions."""
 
     name: str
     """The exception class name"""
 
     def __init__(self, name: str, *args: object) -> None:
         super().__init__(*args)
         self.name = name
 
     def __repr__(self) -> str:
         return f"<{self.name} at {id(self)}"
 
     def __str__(self) -> str:
-        return super().__str__().replace('ExecutionError', self.name)
+        return super().__str__().replace("ExecutionError", self.name)
```

### Comparing `pysmali-0.1.1/smali/bridge/executor.py` & `pysmali-0.1.2/smali/bridge/executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 import struct
 
 from smali import SmaliValue, Type
-from smali.opcode import *
+from smali.opcode import * # noqa
 from smali.bridge.frame import Frame
 from smali.bridge.errors import ExecutionError
 from smali.bridge.lang import SmaliObject
 from smali.bridge.objects import Object, Class
 
-__executors__ = {}
+cache = {}
 """Sepcial dict tat stores all opcodes with their executors"""
 
-class Executor:
 
+class Executor:
     opcode: str
     """The linked opcode"""
 
     action = None
     """Optional action if this class is not subclassed."""
 
     frame: Frame
@@ -24,30 +24,27 @@
 
     args: tuple
     """THe current execution arguments"""
 
     kwargs: dict
     """The current execution"""
 
-    def __init__(self, action, name=None,
-                 map_to: list = None) -> None:
+    def __init__(self, action, name=None, map_to: list = None) -> None:
         self.opcode = name
         self.action = action
         self.frame = None
         if self.action:
-            self.opcode = (str(action.__name__)
-                .replace('__', '/')
-                .replace('_', '-'))
+            self.opcode = str(action.__name__).replace("__", "/").replace("_", "-")
 
         if not self.opcode:
-            raise ValueError('Opcode name must be non-null!')
-        __executors__[self.opcode] = self
+            raise ValueError("Opcode name must be non-null!")
+        cache[self.opcode] = self
         if map_to:
             for op_name in map_to:
-                __executors__[op_name] = self
+                cache[op_name] = self
 
     def __call__(self, frame: Frame):
         self.frame = frame
         self.args = self.args or ()
         if self.action:
             self.action(self, *self.args)
 
@@ -55,294 +52,361 @@
         return f"<{self.opcode} at {id(self):#x}>"
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def cast(self, value, classes):
         if not isinstance(value, classes):
-            raise ExecutionError('ClassCastError',
-                f"Could not cast '{type(value)}' to {classes}")
+            raise ExecutionError(
+                "ClassCastError", f"Could not cast '{type(value)}' to {classes}"
+            )
 
         return value
 
-def OpcodeExecutor(map_to: list = None):
+
+def opcode_executor(map_to: list = None):
     def wrapper(func):
         return Executor(func, map_to=map_to if map_to else [])
+
     return wrapper
 
-def executor(name: str) -> Executor:
-    if name not in __executors__:
-        raise KeyError(f'Could not find executor for opcode: {name}')
 
-    return __executors__[name]
+def get_executor(name: str) -> Executor:
+    if name not in cache:
+        raise KeyError(f"Could not find executor for opcode: {name}")
+
+    return cache[name]
 
 
-@OpcodeExecutor()
-def nop(self):
+@opcode_executor()
+def nop(self, *Args):
     pass
 
+
 ################################################################################
 # RETURN
 ################################################################################
 
-@OpcodeExecutor(map_to=[RETURN_VOID_BARRIER, RETURN_VOID_NO_BARRIER])
+
+@opcode_executor(map_to=[RETURN_VOID_BARRIER, RETURN_VOID_NO_BARRIER])
 def return_void(self: Executor):
     self.frame.return_value = None
     self.frame.finished = True
 
 
-@OpcodeExecutor(map_to=[RETURN, RETURN_WIDE])
+@opcode_executor(map_to=[RETURN, RETURN_WIDE])
 def return_object(self: Executor, register: str):
     self.frame.return_value = self.frame[register]
     self.frame.finished = True
 
+
 ################################################################################
 # GOTO
 ################################################################################
 
-@OpcodeExecutor(map_to=[GOTO_16, GOTO_32])
+
+@opcode_executor(map_to=[GOTO_16, GOTO_32])
 def goto(self: Executor, label: str):
     if label not in self.frame.labels:
         raise ExecutionError("NoSuchLabelError", label)
 
     self.frame.label = label
     self.frame.pos = self.frame.labels[label]
 
+
 ################################################################################
 # INVOKE
 ################################################################################
 
-@OpcodeExecutor(map_to=[
-    INVOKE_DIRECT, INVOKE_STATIC, INVOKE_VIRTUAL
-])
+
+@opcode_executor(map_to=[INVOKE_DIRECT, INVOKE_STATIC, INVOKE_VIRTUAL])
 def invoke(self: Executor, inv_type, args, owner, method):
     # TODO: add direct calls to int or str objects
-    if inv_type in ('direct', 'virtual', 'static'):
+    if inv_type in ("direct", "virtual", "static"):
         vm_class = None
-        if owner == 'Ljava/lang/Class;':
+        if owner == "Ljava/lang/Class;":
             # If class methods should be invoked, just use the
             # previously moved class object
             vm_class = self.frame[args[0]]
             if method not in Class:
-                raise ExecutionError('NoSuchMethodError', f"method '{method}' not defined!")
+                raise ExecutionError(
+                    "NoSuchMethodError", f"method '{method}' not defined!"
+                )
 
             self.frame.method_return = Class[method](vm_class)
             return
 
-        if owner == 'Ljava/lang/Object;':
+        if owner == "Ljava/lang/Object;":
             if method not in Object:
-                raise ExecutionError('NoSuchMethodError', f"method '{method}' not defined!")
+                raise ExecutionError(
+                    "NoSuchMethodError", f"method '{method}' not defined!"
+                )
 
             target = Object[method]
             self.frame.method_return = target(self.frame[args[0]])
             return
 
-
         values = [self.frame[register] for register in args]
         instance = None
-        if inv_type != 'static':
+        if inv_type != "static":
             instance = values[0]
             super_cls = instance.smali_class.super_cls
             if super_cls == owner:
                 vm_class = self.frame.vm.get_class(super_cls)
             # Remove the first argument
             values = values[1:]
 
         if not vm_class:
             vm_class = self.frame.vm.get_class(owner)
 
         target = vm_class.method(method)
         self.frame.method_return = self.frame.vm.call(target, instance, *values)
 
-@OpcodeExecutor()
+
+@opcode_executor()
 def throw(self: Executor, register: str):
-    self.frame.error = ExecutionError('RuntimeError', self.frame[register])
+    self.frame.error = ExecutionError("RuntimeError", self.frame[register])
+
 
 ################################################################################
 # INT-2-OBJECT, LONG-2-OBJECT
 ################################################################################
 
-@OpcodeExecutor()
+
+@opcode_executor()
 def int_to_long(self: Executor, dest: str, src: str):
     self.frame[dest] = self.frame[src] & 0xFFFFFFFFFFFFFFFF
 
 
-@OpcodeExecutor(map_to=[LONG_TO_INT])
+@opcode_executor(map_to=[LONG_TO_INT])
 def int_to_int(self: Executor, dest: str, src: str):
     self.frame[dest] = self.frame[src] & 0xFFFFFFFF
 
 
-@OpcodeExecutor(map_to=[INT_TO_SHORT])
+@opcode_executor(map_to=[INT_TO_SHORT])
 def int_to_char(self: Executor, dest: str, src: str):
     self.frame[dest] = self.frame[src] & 0xFFFF
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def int_to_byte(self: Executor, dest: str, src: str):
-    self.frame[dest],  = struct.unpack('>i', self.frame[src])
+    (self.frame[dest],) = struct.unpack(">i", self.frame[src])
 
 
-@OpcodeExecutor(map_to=[INT_TO_DOUBLE])
+@opcode_executor(map_to=[INT_TO_DOUBLE])
 def int_to_float(self: Executor, dest: str, src: str):
     self.frame[dest] = float(self.frame[src])
 
+
 ################################################################################
 # GET, PUT
 ################################################################################
 
-@OpcodeExecutor(map_to=[
-    SPUT, SPUT_BOOLEAN, SPUT_SHORT, SPUT_CHAR, SPUT_BYTE,
-    SPUT_OBJECT_VOLATILE, SPUT_WIDE,SPUT_WIDE_VOLATILE
-])
+
+@opcode_executor(
+    map_to=[
+        SPUT,
+        SPUT_BOOLEAN,
+        SPUT_SHORT,
+        SPUT_CHAR,
+        SPUT_BYTE,
+        SPUT_OBJECT_VOLATILE,
+        SPUT_WIDE,
+        SPUT_WIDE_VOLATILE,
+    ]
+)
 def sput_object(self: Executor, register: str, dest: str):
     # The destination string contains the owner class name, field name and
     # field type.
     value = self.frame[register]
 
-    owner, name_type = dest.split('->')
-    name, _ = name_type.split(':')
+    owner, name_type = dest.split("->")
+    name, _ = name_type.split(":")
 
     cls = self.frame.vm.get_class(owner)
     field = cls.field(name)
     field.value = value
 
 
-@OpcodeExecutor(map_to=[
-    SGET, SGET_BOOLEAN, SGET_BYTE, SGET_OBJECT_VOLATILE, SGET_VOLATILE,
-    SGET_WIDE, SGET_WIDE_VOLATILE, SGET_CHAR
-])
+@opcode_executor(
+    map_to=[
+        SGET,
+        SGET_BOOLEAN,
+        SGET_BYTE,
+        SGET_OBJECT_VOLATILE,
+        SGET_VOLATILE,
+        SGET_WIDE,
+        SGET_WIDE_VOLATILE,
+        SGET_CHAR,
+    ]
+)
 def sget_object(self: Executor, register: str, dest: str):
     # The destination string contains the owner class name, field name and
     # field type.
-    owner, name_type = dest.split('->')
-    name, _ = name_type.split(':')
+    owner, name_type = dest.split("->")
+    name, _ = name_type.split(":")
 
     cls = self.frame.vm.get_class(owner)
     field = cls.field(name)
     self.frame[register] = field.value
 
 
-@OpcodeExecutor(map_to=[
-    IGET_BOOLEAN, IGET_BYTE, IGET_CHAR, IGET_SHORT,
-    IGET_VOLATILE, IGET_WIDE, IGET, IGET_OBJECT_VOLATILE
-])
+@opcode_executor(
+    map_to=[
+        IGET_BOOLEAN,
+        IGET_BYTE,
+        IGET_CHAR,
+        IGET_SHORT,
+        IGET_VOLATILE,
+        IGET_WIDE,
+        IGET,
+        IGET_OBJECT_VOLATILE,
+    ]
+)
 def iget_object(self: Executor, dest: str, src: str, info: str):
     smali_object = self.cast(self.frame[src], SmaliObject)
-    _, field = info.split('->')
-    field_name, _ = field.split(':')
+    _, field = info.split("->")
+    field_name, _ = field.split(":")
 
     self.frame[dest] = smali_object[field_name]
 
 
-@OpcodeExecutor(map_to=[
-    IPUT, IPUT_BOOLEAN, IPUT_BYTE, IPUT_CHAR,
-    IPUT_SHORT, IPUT_OBJECT_VOLATILE, IPUT_VOLATILE,
-    IPUT_WIDE
-])
+@opcode_executor(
+    map_to=[
+        IPUT,
+        IPUT_BOOLEAN,
+        IPUT_BYTE,
+        IPUT_CHAR,
+        IPUT_SHORT,
+        IPUT_OBJECT_VOLATILE,
+        IPUT_VOLATILE,
+        IPUT_WIDE,
+    ]
+)
 def iput_object(self: Executor, src: str, obj: str, info: str):
     smali_object = self.cast(self.frame[obj], SmaliObject)
-    _, field = info.split('->')
-    field_name, _ = field.split(':')
+    _, field = info.split("->")
+    field_name, _ = field.split(":")
 
     smali_object[field_name] = self.frame[src]
 
+
 ################################################################################
 # CONST
 ################################################################################
 
-@OpcodeExecutor(map_to=[
-    CONST_STRING, CONST_STRING_JUMBO, CONST_16, CONST_4,
-    CONST_WIDE, CONST_WIDE_HIGH16, CONST_WIDE_32, 
-    CONST_STRING_JUMBO
-])
+
+@opcode_executor(
+    map_to=[
+        CONST_STRING,
+        CONST_STRING_JUMBO,
+        CONST_16,
+        CONST_4,
+        CONST_WIDE,
+        CONST_WIDE_HIGH16,
+        CONST_WIDE_32,
+        CONST_STRING_JUMBO,
+    ]
+)
 def const(self: Executor, register: str, value: str):
     self.frame[register] = SmaliValue(value)
 
 
-@OpcodeExecutor(map_to=[CONST_CLASS])
+@opcode_executor(map_to=[CONST_CLASS])
 def const_class(self: Executor, register: str, name: str):
     self.frame[register] = self.frame.vm.get_class(name)
 
+
 ################################################################################
 # MOVE
 ################################################################################
 
-@OpcodeExecutor(map_to=[MOVE_RESULT_OBJECT])
+
+@opcode_executor(map_to=[MOVE_RESULT_OBJECT])
 def move_result(self: Executor, register: str):
     self.frame[register] = self.frame.method_return
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def move(self: Executor, dest: str, src: str):
     self.frame[dest] = self.frame[src]
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def move_exception(self: Executor, dest: str):
     self.frame[dest] = self.frame.error
 
+
 ################################################################################
 # NEW-INSTANCE
 ################################################################################
 
-@OpcodeExecutor()
+
+@opcode_executor()
 def new_instance(self: Executor, register: str, descriptor: str):
     # Filter out primitive values
     if descriptor in "ISBJ":
         self.frame[register] = 0
     elif descriptor in "FD":
         self.frame[register] = 0.0
-    elif descriptor in ('Ljava/lang/String;', 'C', 'Ljava/lang/Character;'):
+    elif descriptor in ("Ljava/lang/String;", "C", "Ljava/lang/Character;"):
         self.frame[register] = ""
-    elif descriptor in ("Ljava/lang/Integer;", "Ljava/lang/Byte;",
-                        "Ljava/lang/Long", "Ljava/lang/Short;"):
+    elif descriptor in (
+        "Ljava/lang/Integer;",
+        "Ljava/lang/Byte;",
+        "Ljava/lang/Long",
+        "Ljava/lang/Short;",
+    ):
         self.frame[register] = 0
     elif descriptor in ("Ljava/lang/Boolean", "Z"):
         self.frame[register] = False
-    elif descriptor in ('Ljava/util/ArrayList;', 'Ljava/util/LinkedList;'):
+    elif descriptor in ("Ljava/util/ArrayList;", "Ljava/util/LinkedList;"):
         self.frame[register] = []
     else:
         smali_class = self.frame.vm.get_class(descriptor)
         instance = SmaliObject(smali_class)
         instance.init()
 
         self.frame[register] = instance
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def new_array(self: Executor, dest: str, count_register: str, descriptor: str):
     cls = Type(descriptor).class_name
     values = [None] * self.frame[count_register]
-    if cls in "BSIJ": # number
+    if cls in "BSIJ":  # number
         values = [0] * self.frame[count_register]
 
-    elif cls in "FD": # floating point
+    elif cls in "FD":  # floating point
         values = [0.0] * self.frame[count_register]
 
     self.frame[dest] = values
 
 
-@OpcodeExecutor(map_to=[INSTANCE_OF])
+@opcode_executor(map_to=[INSTANCE_OF])
 def check_cast(self: Executor, dest: str, descriptor: str):
     src_class = self.frame[dest]
     if not isinstance(src_class, SmaliObject):
         return
 
     src_class = src_class.smali_class
     dest_class = self.frame.vm.get_class(descriptor)
 
     if not src_class.is_assignable(dest_class):
-        raise ExecutionError('ClassCastError', f"Could not cast {dest_class} to {src_class}")
+        raise ExecutionError(
+            "ClassCastError", f"Could not cast {dest_class} to {src_class}"
+        )
 
 
 ################################################################################
 # SWITCH
 ################################################################################
 
-@OpcodeExecutor()
+
+@opcode_executor()
 def packed_switch(self: Executor, register: str, data: str):
     switch_value, cases = self.frame.switch_data[data]
     value = self.frame[register]
 
     # We must convert the switch_value into a SmaliValue object
     # as it is of type string and we need an integer
     idx = value - SmaliValue(switch_value)
@@ -351,365 +415,377 @@
         # Default branch does nothing
         return
 
     # Call GOTO-instruction directly
     goto.action(self, cases[idx])
 
 
-@OpcodeExecutor
+@opcode_executor
 def sparse_switch(self: Executor, register: str, label_name: str):
     branches = self.frame.switch_data[label_name]
     value = self.frame[register]
 
     # The iteration is needed as the branch values are strings
     for key, label in branches.items():
         if SmaliValue(key) == value:
             goto.action(self, label)
             break
 
+
 ################################################################################
 # IF
 ################################################################################
 
-@OpcodeExecutor()
+
+@opcode_executor()
 def if_le(self: Executor, left: str, right: str, label: str):
     if self.frame[left] <= self.frame[right]:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_ge(self: Executor, left: str, right: str, label: str):
     if self.frame[left] >= self.frame[right]:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_gez(self: Executor, left: str, label: str):
     if self.frame[left] >= 0:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_ltz(self: Executor, left: str, label: str):
     if self.frame[left] < 0:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_gt(self: Executor, left: str, right: str, label: str):
     if self.frame[left] > self.frame[right]:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_lt(self: Executor, left: str, right: str, label: str):
     if self.frame[left] < self.frame[right]:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_gtz(self: Executor, left: str, label: str):
     if self.frame[left] > 0:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_ne(self: Executor, left: str, right: str, label: str):
     if self.frame[left] != self.frame[right]:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_lez(self: Executor, left: str, label: str):
     if self.frame[left] <= 0:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_nez(self: Executor, left: str, label: str):
     if self.frame[left] != 0:
         goto.action(self, label)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def if_eqz(self: Executor, left: str, label: str):
     if self.frame[left] == 0:
         goto.action(self, label)
 
+
 ################################################################################
 # ARRAY
 ################################################################################
 
-@OpcodeExecutor()
+
+@opcode_executor()
 def array_length(self: Executor, dest: str, array: str):
     self.frame[dest] = len(self.frame[array])
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def fill_array_data(self: Executor, dest: str, label: str):
     self.frame[dest] = self.frame.array_data[label]
 
 
-@OpcodeExecutor(map_to=[
-    AGET_BOOLEAN, AGET_BYTE, AGET_CHAR,
-    AGET_OBJECT, AGET_SHORT, AGET_WIDE
-])
+@opcode_executor(
+    map_to=[AGET_BOOLEAN, AGET_BYTE, AGET_CHAR, AGET_OBJECT, AGET_SHORT, AGET_WIDE]
+)
 def aget(self: Executor, dest: str, array: str, index: str):
     idx_value = self.frame[index]
     array_data = self.frame[array]
     if idx_value < 0 or idx_value >= len(array):
         raise ExecutionError(
-            'IndexOutOfBoundsError',
-            f"Index {idx_value} is out of bounds for length {len(array_data)}")
+            "IndexOutOfBoundsError",
+            f"Index {idx_value} is out of bounds for length {len(array_data)}",
+        )
 
     self.frame[dest] = array_data[idx_value]
 
 
-@OpcodeExecutor(map_to=[
-    APUT_BOOLEAN, APUT_BYTE, APUT_CHAR,
-    APUT_OBJECT, APUT_SHORT, APUT_WIDE
-])
+@opcode_executor(
+    map_to=[APUT_BOOLEAN, APUT_BYTE, APUT_CHAR, APUT_OBJECT, APUT_SHORT, APUT_WIDE]
+)
 def aput(self: Executor, src: str, array: str, index: str):
     idx_value = self.frame[index]
     array_data = self.frame[array]
     if idx_value < 0 or idx_value > len(array):
         raise ExecutionError(
-            'IndexOutOfBoundsError',
-            f"Index {idx_value} is out of bounds for length {len(array_data)}")
+            "IndexOutOfBoundsError",
+            f"Index {idx_value} is out of bounds for length {len(array_data)}",
+        )
 
     if len(array) == idx_value:
         array_data.append(self.frame[src])
     else:
         array_data[idx_value] = self.frame[src]
 
+
 ################################################################################
 # Int operations (2addr)
 ################################################################################
 
-@OpcodeExecutor(map_to=[NEG_DOUBLE, NEG_FLOAT, NEG_LONG])
+
+@opcode_executor(map_to=[NEG_DOUBLE, NEG_FLOAT, NEG_LONG])
 def neg_int(self: Executor, dest: str, src: str):
     self.frame[dest] = -self.frame[src]
 
-@OpcodeExecutor(map_to=[NOT_LONG])
+
+@opcode_executor(map_to=[NOT_LONG])
 def not_int(self: Executor, dest: str, src: str):
     self.frame[dest] = ~self.frame[src]
 
-@OpcodeExecutor(map_to=[OR_LONG_2ADDR])
+
+@opcode_executor(map_to=[OR_LONG_2ADDR])
 def or_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] |= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[AND_LONG_2ADDR])
+@opcode_executor(map_to=[AND_LONG_2ADDR])
 def and_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] &= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[SUB_DOUBLE_2ADDR, SUB_FLOAT_2ADDR, SUB_LONG_2ADDR])
+@opcode_executor(map_to=[SUB_DOUBLE_2ADDR, SUB_FLOAT_2ADDR, SUB_LONG_2ADDR])
 def sub_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] -= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[XOR_LONG_2ADDR])
+@opcode_executor(map_to=[XOR_LONG_2ADDR])
 def xor_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] ^= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[ADD_DOUBLE_2ADDR, ADD_FLOAT_2ADDR, ADD_LONG_2ADDR])
+@opcode_executor(map_to=[ADD_DOUBLE_2ADDR, ADD_FLOAT_2ADDR, ADD_LONG_2ADDR])
 def add_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] += self.frame[src]
 
 
-@OpcodeExecutor(map_to=[DIV_LONG_2ADDR])
+@opcode_executor(map_to=[DIV_LONG_2ADDR])
 def div_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] //= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[DIV_DOUBLE_2ADDR])
+@opcode_executor(map_to=[DIV_DOUBLE_2ADDR])
 def div_float__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] /= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[SHL_LONG_2ADDR])
+@opcode_executor(map_to=[SHL_LONG_2ADDR])
 def shl_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] <<= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[SHR_LONG_2ADDR, USHR_INT_2ADDR, USHR_LONG_2ADDR])
+@opcode_executor(map_to=[SHR_LONG_2ADDR, USHR_INT_2ADDR, USHR_LONG_2ADDR])
 def shr_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] >>= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[REM_DOUBLE_2ADDR, REM_FLOAT_2ADDR, REM_LONG_2ADDR])
+@opcode_executor(map_to=[REM_DOUBLE_2ADDR, REM_FLOAT_2ADDR, REM_LONG_2ADDR])
 def rem_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] %= self.frame[src]
 
 
-@OpcodeExecutor(map_to=[MUL_DOUBLE_2ADDR, MUL_FLOAT_2ADDR, MUL_LONG_2ADDR])
+@opcode_executor(map_to=[MUL_DOUBLE_2ADDR, MUL_FLOAT_2ADDR, MUL_LONG_2ADDR])
 def mul_int__2addr(self: Executor, dest: str, src: str):
     self.frame[dest] *= self.frame[src]
 
+
 ################################################################################
 # Int operations (lit8 and lit16)
 # div, add, sub, rem, and, or, xor, shl, shr, rsub(lit8)
 ################################################################################
 
-@OpcodeExecutor()
+
+@opcode_executor()
 def div_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] // (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def div_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] // (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def add_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] + (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def add_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] + (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def sub_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] - (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def sub_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] - (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def mul_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] * (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def mul_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] * (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def rem_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] % (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def rem_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] % (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def and_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] & (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def and_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] & (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def or_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] | (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def or_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] | (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def xor_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] ^ (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def xor_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] ^ (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def shl_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] << (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def shl_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] << (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def shr_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] >> (SmaliValue(right) & 0xFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def shr_int__lit16(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] >> (SmaliValue(right) & 0xFFFF)
 
 
-@OpcodeExecutor()
+@opcode_executor()
 def rsub_int__lit8(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = (SmaliValue(right) & 0xFF) - self.frame[left]
 
+
 ################################################################################
 # Int operations
 ################################################################################
 
-@OpcodeExecutor()
+
+@opcode_executor()
 def div_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] // self.frame[right]
 
 
-@OpcodeExecutor(map_to=[DIV_DOUBLE])
+@opcode_executor(map_to=[DIV_DOUBLE])
 def div_float(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] / self.frame[right]
 
 
-@OpcodeExecutor(map_to=[ADD_DOUBLE, ADD_FLOAT, ADD_LONG])
+@opcode_executor(map_to=[ADD_DOUBLE, ADD_FLOAT, ADD_LONG])
 def add_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] + self.frame[right]
 
 
-@OpcodeExecutor(map_to=[SUB_DOUBLE, SUB_FLOAT, SUB_LONG])
+@opcode_executor(map_to=[SUB_DOUBLE, SUB_FLOAT, SUB_LONG])
 def sub_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] - self.frame[right]
 
 
-@OpcodeExecutor(map_to=[REM_DOUBLE, REM_FLOAT, REM_LONG])
+@opcode_executor(map_to=[REM_DOUBLE, REM_FLOAT, REM_LONG])
 def rem_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] % self.frame[right]
 
 
-@OpcodeExecutor(map_to=[MUL_DOUBLE, MUL_FLOAT, MUL_LONG])
+@opcode_executor(map_to=[MUL_DOUBLE, MUL_FLOAT, MUL_LONG])
 def mul_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] * self.frame[right]
 
 
-@OpcodeExecutor(map_to=[OR_LONG])
+@opcode_executor(map_to=[OR_LONG])
 def or_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] | self.frame[right]
 
 
-@OpcodeExecutor(map_to=[AND_LONG])
+@opcode_executor(map_to=[AND_LONG])
 def and_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] & self.frame[right]
 
 
-@OpcodeExecutor(map_to=[XOR_LONG])
+@opcode_executor(map_to=[XOR_LONG])
 def xor_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] ^ self.frame[right]
 
 
-@OpcodeExecutor(map_to=[SHL_LONG])
+@opcode_executor(map_to=[SHL_LONG])
 def shl_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] << self.frame[right]
 
 
-@OpcodeExecutor(map_to=[SHR_LONG, USHR_LONG, USHR_INT])
+@opcode_executor(map_to=[SHR_LONG, USHR_LONG, USHR_INT])
 def shr_int(self: Executor, dest: str, left: str, right: str):
     self.frame[dest] = self.frame[left] >> self.frame[right]
```

### Comparing `pysmali-0.1.1/smali/bridge/frame.py` & `pysmali-0.1.2/smali/bridge/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 of all registers in the current context.
 
 On top of that, ``Frame`` objects store method return values (sub-
 calls) as well as the final return value. If any errors occur, they
 will be stored in a separate variable.
 """
 
-from smali.bridge.errors import (
-    ExecutionError, NoSuchRegisterError
-)
+from smali.bridge.errors import ExecutionError, NoSuchRegisterError
+
 
 class Frame:
     """Class to represent execution frames.
 
     There are different special functions implemented to simplify
     the process of getting and setting register values:
```

### Comparing `pysmali-0.1.1/smali/bridge/lang.py` & `pysmali-0.1.2/smali/bridge/lang.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,55 +11,53 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 __doc__ = """
 The module ``lang`` of the provided Smali bridge defines classes that
-can be used to mimic Java's reflection at runtime of the ``SmaliVM``.
+can be used to mimic Java's reflection at runtime of the :class:`SmaliVM`.
 
 All members of a Smali class inherit functionalities of ``__eq__``,
 ``__ne__``, as well as hash value calculation and string representation
 of objects.
 
 .. hint::
 
     Some properties are modifiable like ``SmaliField.value`` or the name
-    of a ``SmaliClass`` object. It is recommended to leave them how they
+    of a :class:`SmaliClass` object. It is recommended to leave them how they
     are and let the VM make chenges to them.
 
 """
 
 import re
 
 from io import UnsupportedOperation
 
-from smali.base import (
-    AccessType,
-    SmaliValueProxy,
-    Type
-)
-from smali.bridge.errors import (
-    NoSuchMethodError,
-    NoSuchFieldError,
-    NoSuchClassError
-)
+from smali.base import AccessType, SmaliValueProxy, Type
+from smali.bridge.errors import NoSuchMethodError, NoSuchFieldError, NoSuchClassError
 
 __all__ = [
-    'SmaliMember', 'SmaliAnnotation', 'SmaliField', 'SmaliMethod',
-    'SmaliMethodBroker', 'SmaliClass', 'SmaliObject'
+    "SmaliMember",
+    "SmaliAnnotation",
+    "SmaliField",
+    "SmaliMethod",
+    "SmaliMethodBroker",
+    "SmaliClass",
+    "SmaliObject",
 ]
 
+
 class SmaliMember:
     """Base class for Python classes of the Smali language.
 
     All members must provide a signature to be identified with.
     """
 
-    __parent: 'SmaliMember'
+    __parent: "SmaliMember"
     """The parent of this member."""
 
     __signature: str
     """The qualified signature of this member"""
 
     __modifiers: int
     """The member's visibility modifiers."""
@@ -68,21 +66,27 @@
     """All annotations of this member. The will be stored in
     a type-2-object mapping.
 
     >>> member.annotations
     { 'Ljava/lang/Deprecated;': [<SmaliAnnotation at 0x...>, ...] }
     """
 
-    def __init__(self, parent: 'SmaliMember', signature: str, modifiers: int,
-                 base_class: type, annotations: list = None) -> None:
+    def __init__(
+        self,
+        parent: "SmaliMember",
+        signature: str,
+        modifiers: int,
+        base_class: type,
+        annotations: list = None,
+    ) -> None:
         self.__signature = signature
         self.__modifiers = modifiers
         self.__annotations = annotations or []
         if self.__class__ != base_class:
-            raise TypeError(f'{base_class.__name__} cannot be sub-classed!')
+            raise TypeError(f"{base_class.__name__} cannot be sub-classed!")
 
         self.__parent = parent
         if not isinstance(self.parent, SmaliMember) and parent:
             raise TypeError("Parent of this memeber must be an instance of SmaliMember")
 
     def is_annotation_present(self, a_type: str) -> bool:
         """Returns whether the given annotation is present.
@@ -111,15 +115,15 @@
         if not isinstance(a_type, str):
             # to prevent errors, the output is non-null
             return []
 
         return self.__annotations.get(a_type, [])
 
     @property
-    def parent(self) -> 'SmaliMember':
+    def parent(self) -> "SmaliMember":
         """Returns the declaring class or annotation member.
 
         :return: the parent of this member
         :rtype: SmaliMember
         """
         return self.__parent
 
@@ -190,74 +194,87 @@
     :param attr: the annotation's attributes, defaults to None
     :type attr: dict, optional
     """
 
     attr: dict
     """The attributes of this annotation (key-value map)."""
 
-    def __init__(self, parent, signature: str, modifiers: int,
-                 annotations: list = None, attr: dict = None) -> None:
+    def __init__(
+        self,
+        parent,
+        signature: str,
+        modifiers: int,
+        annotations: list = None,
+        attr: dict = None,
+    ) -> None:
         super().__init__(parent, signature, modifiers, SmaliAnnotation, annotations)
         self.attr = attr or {}
 
     def __getitem__(self, key: str) -> object:
         return self.attr.get(key, None)
 
     def __setitem__(self, key: str, value):
         self.attr[key] = value
 
     def __contains__(self, key: str) -> bool:
         return key in self.attr
 
 
 class SmaliField(SmaliMember):
-    """Pypthon class that represents fields in Smali.
+    """Python class that represents fields in Smali.
 
     :param signature: the field's signature (``name:type``)
     :type signature: str
     :param modifiers: the field's access modifiers
     :type modifiers: int
     :param annotations: the field's annotations, defaults to None
     :type annotations: list, optional
     :param value: the field's value, defaults to None
-    :type value: SmaliValueProxy, optional
+    :type value: :class:`SmaliValueProxy`, optional
     """
 
     __name: str
     """The field's name"""
 
     __smali_type: Type
     """The field's type (Smali type descriptor)"""
 
     __value: SmaliValueProxy
     """Stores the actual value of this field"""
 
-    def __init__(self, parent, signature: str, modifiers: int, name: str,
-                 smali_type: Type, annotations: list = None,
-                 value: SmaliValueProxy = None) -> None:
+    def __init__(
+        self,
+        parent,
+        signature: str,
+        modifiers: int,
+        name: str,
+        smali_type: Type,
+        annotations: list = None,
+        value: SmaliValueProxy = None,
+    ) -> None:
         super().__init__(parent, signature, modifiers, SmaliField, annotations)
         self.__value = value
         self.__smali_type = smali_type
         self.__name = name
 
     @property
     def value(self) -> SmaliValueProxy:
         """Returns the value of this field.
 
-        :return: the value as a ``SmaliValue``
-        :rtype: SmaliValueProxy
+        :return: the value as a :class:`SmaliValue`
+        :rtype: :class:`SmaliValueProxy`
         """
         return self.__value
 
     @value.setter
     def value(self, new_value: SmaliValueProxy):
         """Setter for ``self.value``.
 
         :param new_value: the new value to apply
-        :type new_value: SmaliValueProxy
+        :type new_value: :class:`SmaliValueProxy`
         :raises UnsupportedOperation: if this field can not be modified
         """
         self.__value = new_value
 
     @property
     def smali_type(self) -> Type:
         """Returns the type of this field
@@ -308,17 +325,22 @@
 
     __vm = None
     """The VM that delegates the execution of this method."""
 
     __locals: int
     """Stores the amount of locals"""
 
-
-    def __init__(self, vm, parent: 'SmaliMember', signature: str,
-                 modifiers: int, annotations: list = None) -> None:
+    def __init__(
+        self,
+        vm,
+        parent: "SmaliMember",
+        signature: str,
+        modifiers: int,
+        annotations: list = None,
+    ) -> None:
         super().__init__(parent, signature, modifiers, SmaliMethod, annotations)
         self.__vm = vm
         sig_type = Type(signature)
         self.name = sig_type.get_method_name()
         self.smali_params = sig_type.get_method_params()
         self.smali_return = sig_type.get_method_return_type()
 
@@ -367,15 +389,15 @@
     def locals(self) -> int:
         """Returns the amount of local variables."""
         return self.__locals
 
     @locals.setter
     def locals(self, value: int):
         if not isinstance(value, int):
-            raise TypeError('Invalid locals argument type')
+            raise TypeError("Invalid locals argument type")
         self.__locals = value
 
 
 RE_REGISTER = re.compile(r"p\d+")
 
 
 class _MethodBroker:
@@ -389,29 +411,29 @@
     >>> broker = SmaliMethodBroker(methods)
     >>> broker += SmaliMethod(...)
     >>> broker(object_instance, p0=1, p1=2)
     <result> # in case we defined a method with two parameters
     >>> for method in broker:
     ...     print(str(method))
 
-    There is a pre-defined alias for this class named ``SmaliMethodBroker`` in the .
+    There is a pre-defined alias for this class named :class:`SmaliMethodBroker` in the .
     same module.
     """
 
     __name: str
     """The method's name"""
 
     __methods: list
     """The methods that can be called."""
 
     def __init__(self, name: str, methods: list) -> None:
         self.__methods = methods or []
         self.__name = name
 
-    def __iadd__(self, method: SmaliMethod) -> '_MethodBroker':
+    def __iadd__(self, method: SmaliMethod) -> "_MethodBroker":
         self.__methods.append(method)
 
     def __call__(self, instance, *args, **kwds) -> object:
         if len(self.__methods) == 1:
             method = self.__methods[0]
             return method(instance, *args, **kwds)
 
@@ -435,29 +457,33 @@
             else:
                 if returns is None:
                     raise NoSuchMethodError(
                         f"Attempted to call {self.__name}() with invalid arguments"
                     )
                 # Filter by return type
                 if not returns:
-                    targets = list(filter(lambda x: (
-                        x.return_type.descriptor != 'V'), targets))
+                    targets = list(
+                        filter(lambda x: (x.return_type.descriptor != "V"), targets)
+                    )
                 else:
-                    targets = list(filter(lambda x: (
-                        x.return_type.descriptor == 'V'), targets))
+                    targets = list(
+                        filter(lambda x: (x.return_type.descriptor == "V"), targets)
+                    )
 
                 # We found one method, call it!
                 if len(targets) == 1:
                     method = targets[0]
                     return method(instance, *args, **kwds)
 
         # 2. If registers are present, filter by amount
         # of defined parameters
         elif reg_count > 0:
-            targets = list(filter(lambda x: len(x.parameters) == reg_count, self.__methods))
+            targets = list(
+                filter(lambda x: len(x.parameters) == reg_count, self.__methods)
+            )
             # Again, we find the right method if only one result is present
             if len(targets) == 1:
                 method = targets[0]
                 return method(instance, *args, **kwds)
 
         raise NoSuchMethodError(
             f"Attempted to call {self.__name}() - multiple variants present"
@@ -472,14 +498,15 @@
     def __iter__(self):
         return iter(self.__methods)
 
 
 SmaliMethodBroker = _MethodBroker
 """Public alias for method broker objects"""
 
+
 class SmaliClass(SmaliMember):
     """Internal class for storing imported class data.
 
     Annotations of a class
     ----------------------
 
     **All** declared annotations are stored within the ``annotations`` field
@@ -495,21 +522,21 @@
     ...     annotation: SmaliAnnotation
 
     Fields of a class
     -----------------
 
     Field definitions are stored in a dict to enable quick access to all of
     them. Static fields contain values at class level and the values of normal
-    fields will be stored in separate ``SmaliObject`` instances. A field that
+    fields will be stored in separate :class:`SmaliObject` instances. A field that
     belongs to a class should be retrieved via the following method:
 
     >>> field = smali_class.field("foo")
     <SmaliField 'foo:Ljava/lang/String;'>
 
-    It is also possible to retrieve the ``SmaliField`` via a dict-like access:
+    It is also possible to retrieve the :class:`SmaliField` via a dict-like access:
 
     >>> field = smali_class["foo"]
 
     .. important::
 
         Only fields are accessable via subcription, annotations, methods and
         implemented interfaces must e queried with other methods.
@@ -525,33 +552,33 @@
     their name or signature directly:
 
     >>> method = smali_class.method("<init>")
     <SmaliMethod '<init> at ...>
 
     In this example we queried the method named ``<init>``, which is the constructor
     method of this class. If there is more than one definition, a so-called
-    ``SmaliMethodBroker`` is returned:
+    :class:`SmaliMethodBroker` is returned:
 
     >>> method = smali_class.method("getString")
     <_MethodBroker of 'getString' at ...>
 
     These objects store all methods with the same name and will choose the
     best method according to the given arguments when trying to execute one
     method.
 
-    Like ``SmaliField`` objects, methods can be added via dic-set as well:
+    Like :class:`SmaliField` objects, methods can be added via dic-set as well:
 
     >>> smali_class["getString"] = SmaliMethod(...)
 
     Interfaces of a class
     ---------------------
 
     The implemented interfaces and super class will be stored as simple string
     objects. As the option ``lookup_missing`` can be set to false, these values
-    won't be initialized with ``SmaliClass`` instances to enable import of
+    won't be initialized with :class:`SmaliClass` instances to enable import of
     whole class files wihtout having all classes defined.
 
     Inner classes defined inside a SmaliClass
     -----------------------------------------
 
     Inner classes are stored like fields or methods - in a dict. They can't be
     queried directly, but the dictionary storing all classes is accessable:
@@ -579,20 +606,25 @@
 
     __super: str
     """The class descriptor of the super class"""
 
     __implements: list
     """The list of implemented interfaces."""
 
-    def __init__(self, parent: 'SmaliMember', signature: str,
-                 modifiers: int,  annotations: list = None) -> None:
+    def __init__(
+        self,
+        parent: "SmaliMember",
+        signature: str,
+        modifiers: int,
+        annotations: list = None,
+    ) -> None:
         super().__init__(parent, signature, modifiers, SmaliClass, annotations)
         sig_type = Type(signature)
         self.__name = sig_type.class_name
-        self.__simple_name = self.__name.split('.')[-1]
+        self.__simple_name = self.__name.split(".")[-1]
         self.__fields = {}
         self.__methods = {}
         self.__super = None
         self.__implements = []
 
     @property
     def simple_name(self) -> str:
@@ -677,39 +709,39 @@
 
     def field(self, name: str) -> SmaliField:
         """Returns the field with the given name.
 
         :param name: the field's name
         :type name: str
         :raises NoSuchFieldError: if no field with the goven name is defined
-        :return: the ``SmaliField`` instance
+        :return: the :class:`SmaliField` instance
         :rtype: SmaliField
         """
         if name in self.__fields:
             return self.__fields[name]
 
         raise NoSuchFieldError(f"Field with name '{name}' not found")
 
-    def inner_class(self, name: str) -> 'SmaliClass':
+    def inner_class(self, name: str) -> "SmaliClass":
         """Returns an inner class by its name.
 
         :param name: the name (type descrptor)
         :type name: str
         :raises NoSuchClassError: if no inner class with the given name is defined
-        :return: the ``SmaliClass`` instance of the inner class
+        :return: the :class:`SmaliClass` instance of the inner class
         :rtype: SmaliClass
         """
         if name not in self.__classes:
             raise NoSuchClassError(f'Class with name "{name}" not found!')
 
         return self.__classes[name]
 
     def __setitem__(self, key: str, value) -> None:
         if not key or not isinstance(key, str):
-            raise KeyError('Invalid key')
+            raise KeyError("Invalid key")
 
         if isinstance(value, SmaliMethod):
             if key not in self.__methods:
                 self.__methods[key] = SmaliMethodBroker(key, [value])
             else:
                 self.__methods[key] += value
 
@@ -717,29 +749,30 @@
             self.__fields[key] = value
 
         elif isinstance(value, SmaliClass):
             self.__classes[key] = value
 
     def __getitem__(self, key: str) -> SmaliField:
         if not key or not isinstance(key, str):
-            raise KeyError('Invalid Key')
+            raise KeyError("Invalid Key")
 
         return self.field(key)
 
     def __contains__(self, field_name: str) -> bool:
         return field_name in self.__fields
 
     def fields(self, access_type: AccessType = None):
         """Returns all fields that match the given access type.
 
         If no access type is given, all fields will be returned.
 
         :param access_type: the access type to filter, defaults to None
         :type access_type: AccessType, optional
         """
+
         def field_filter(field: SmaliField):
             if not access_type:
                 return True
             return field.modifiers in access_type
 
         return filter(field_filter, self.__fields)
 
@@ -756,25 +789,26 @@
             # we should skip the execution
             return
 
         # The first argument represents an instance of the
         # current class - for static context it is always null
         method(None)
 
-    def is_assignable(self, other: 'SmaliClass') -> bool:
+    def is_assignable(self, other: "SmaliClass") -> bool:
         if not other or not other.super_cls:
             return False
-        
+
         super_class = other.super_cls
-        while super_class and super_class != 'Ljava/lang/Object;':
+        while super_class and super_class != "Ljava/lang/Object;":
             if super_class == self or super_class == self.super_cls:
                 return True
-        
+
         return False
 
+
 class SmaliObject:
     """Python objects that store data of a Smali object.
 
     This class implements dict-like access to all fields' values and
     static fields will be directly references if possible.
 
     .. caution::
@@ -790,31 +824,30 @@
 
     __class: SmaliClass
     """The prototype class.
 
     :meta public:
     """
 
-
     def __init__(self, clazz: SmaliClass) -> None:
         self.__class = clazz
         if clazz.modifiers in (AccessType.ABSTRACT, AccessType.INTERFACE):
             raise UnsupportedOperation(
-                'Class is abstract and cannot be instantiated directly!')
+                "Class is abstract and cannot be instantiated directly!"
+            )
 
         self.__field_values = {}
         for name in clazz.fields():
             field = clazz.field(name)
             if field.modifiers not in AccessType.STATIC:
                 self.__field_values[field.name] = None
 
-
     def init(self, *args):
         """Calls the constructor of this object."""
-        ctor = self.smali_class.method('<init>')
+        ctor = self.smali_class.method("<init>")
         ctor(self, *args)
 
     @property
     def smali_class(self) -> SmaliClass:
         """Returns the prototype SmaliClass object
 
         :return: the smali class this object is an instance of
@@ -824,23 +857,24 @@
 
     def __getitem__(self, name: str):
         field = self.smali_class.field(name)
         if field.modifiers in AccessType.STATIC:
             return field.value
 
         if name not in self.__field_values:
-            raise NoSuchFieldError(f'Field not found: {name}')
+            raise NoSuchFieldError(f"Field not found: {name}")
 
         return self.__field_values[name]
 
     def __setitem__(self, name: str, value):
         field = self.smali_class.field(name)
         if field.modifiers in AccessType.FINAL:
             raise UnsupportedOperation(
-                f'Attempt to write in read-only field "{self.smali_class.name}{name}"')
+                f'Attempt to write in read-only field "{self.smali_class.name}{name}"'
+            )
 
         if field.modifiers in AccessType.STATIC:
             field.value = value
 
         # Rather don't use a check whether the field is present
         # as new members could be defined at runtime
         self.__field_values[name] = value
@@ -860,8 +894,8 @@
         :return: _description_
         :rtype: str
         :meta public:
         """
         return f"<SmaliObject@{id(self):x}>"
 
     def __str__(self) -> str:
-        return f"<SmaliObject@{id(self):x} fields={len(self.__field_values)} type={self.smali_class}"
+        return f"<SmaliObject@{id(self):x} fields={len(self.__field_values)} type={self.smali_class}"
```

### Comparing `pysmali-0.1.1/smali/bridge/objects.py` & `pysmali-0.1.2/smali/bridge/objects.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.1/smali/bridge/vm.py` & `pysmali-0.1.2/smali/bridge/vm.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,54 +14,55 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 __doc__ = """
 Implementation of a simple Smali emulator named *SmaliVM*. It supports
 execution of small code snippets as well as the execution of whole
 class files.
 
-Debugging can be done by providing a ``DebugHandler`` and enabling the
+Debugging can be done by providing a :class:`DebugHandler` and enabling the
 debug-option wihtin the VM object. It is also possible to use a custom
 ``ClassLoader`` to load or define new classes.
 """
 
 from abc import ABCMeta, abstractmethod
 
 from smali import SmaliValue, opcode
 from smali.base import Type, AccessType
 from smali.reader import SmaliReader
-from smali.visitor import (
-    ClassVisitor,
-    MethodVisitor,
-    FieldVisitor,
-    AnnotationVisitor
-)
+from smali.visitor import ClassVisitor, MethodVisitor, FieldVisitor, AnnotationVisitor
 from smali.bridge.lang import (
     SmaliClass,
     SmaliMethod,
     SmaliField,
     SmaliAnnotation,
-    RE_REGISTER
+    RE_REGISTER,
 )
 from smali.bridge.frame import Frame
 from smali.bridge.errors import (
     ExecutionError,
     NoSuchMethodError,
     InvalidOpcodeError,
-    NoSuchClassError
+    NoSuchClassError,
 )
 from smali.bridge import executor
 
 __all__ = [
-    'ClassLoader', 'DebugHandler', 'SmaliVM', 'SmaliVMAnnotationReader',
-    'SmaliVMFieldReader', 'SmaliVMMethodReader', 'SmaliVMClassReader',
-    'SmaliClassLoader'
+    "ClassLoader",
+    "DebugHandler",
+    "SmaliVM",
+    "SmaliVMAnnotationReader",
+    "SmaliVMFieldReader",
+    "SmaliVMMethodReader",
+    "SmaliVMClassReader",
+    "SmaliClassLoader",
 ]
 
+
 class ClassLoader(metaclass=ABCMeta):
-    """Abstract base class for SmaliClassLoaders"""
+    """Abstract base class for SmaliClassLoader"""
 
     @abstractmethod
     def define_class(self, source: bytes) -> SmaliClass:
         """Defines a new SmaliClass by parsing the given source file.
 
         :param source: the source code
         :type source: bytes | str
@@ -86,30 +87,40 @@
         :rtype: SmaliClass
         """
 
 
 class DebugHandler:
     """Basic adapter class used for debugging purposes"""
 
-    def precall(self, vm: 'SmaliVM', method: SmaliMethod, opc: executor.Executor) -> None:
+    def precall(
+        self, vm: "SmaliVM", method: SmaliMethod, opc: executor.Executor
+    ) -> None:
         """Called before an opcode executor is processed"""
 
-    def postcall(self, vm: 'SmaliVM', method: SmaliMethod, opc: executor.Executor) -> None:
+    def postcall(
+        self, vm: "SmaliVM", method: SmaliMethod, opc: executor.Executor
+    ) -> None:
         """Called after the opcode has been executed"""
 
 
 class SmaliVM:
     """Basic implementation of a Smali emulator in Python."""
 
     classloader: ClassLoader
     """The class loader used to define classes."""
 
     debug_handler: DebugHandler
     """The debug handler to use."""
 
+    executors: dict
+    """External executors used to operate on a single opcode."""
+
+    use_strict: bool = False
+    """Tells the VM to throw exceptions on unkown opcodes."""
+
     __classes: dict = {}
     """All classes are stored in a dict
 
     :meta public:
     """
 
     __frames: dict = {}
@@ -117,32 +128,47 @@
 
     :meta public:
     """
 
     # This map is used to determine which parameters are applied to the right
     # values.
     __type_map: dict = {
-        int: ("B", "S", "I", "J", "Ljava/lang/Byte;", "Ljava/lang/Short;",
-              "Ljava/lang/Integer;", "Ljava/lang/Long;"),
+        int: (
+            "B",
+            "S",
+            "I",
+            "J",
+            "Ljava/lang/Byte;",
+            "Ljava/lang/Short;",
+            "Ljava/lang/Integer;",
+            "Ljava/lang/Long;",
+        ),
         float: ("F", "D", "Ljava/lang/Double;", "Ljava/lang/Float;"),
         str: ("Ljava/lang/String;", "C", "Ljava/lang/Character;"),
-        bool: ('Z', 'Ljava/lang/Boolean;')
+        bool: ("Z", "Ljava/lang/Boolean;"),
     }
 
-    def __init__(self, class_loader: ClassLoader = None) -> None:
+    def __init__(
+        self,
+        class_loader: ClassLoader = None,
+        executors: dict = executor.cache,
+        use_strict: bool = False
+    ) -> None:
         self.classloader = _SmaliClassLoader(self) or class_loader
+        self.executors = executors or {}
+        self.use_strict = use_strict
 
     def new_class(self, cls: SmaliClass):
         """Defines a new class that can be accessed globally.
 
         :param cls: the class to be defined
         :type cls: SmaliClass
         """
         if not cls:
-            raise ValueError('SmaliClass object is null!')
+            raise ValueError("SmaliClass object is null!")
 
         self.__classes[cls.signature] = cls
 
     def new_frame(self, method: SmaliMethod, frame: Frame):
         """Creates a new method frame that will be mapped to the method's signature-
 
         :param method: the target method
@@ -172,39 +198,41 @@
     def call(self, method, instance, *args, **kwargs) -> object:
         """Executes the given method in the given object instance.
 
         Before the method will be executed, there is an input parameter
         check to validate all passed arguments. The required registers
         will be filled automatically.
 
-        Debugging is done via the ``DebugHandler`` that must be set globally
+        Debugging is done via the :class:`DebugHandler` that must be set globally
         in this object.
 
         :param method: the method to execute
-        :type method: SmaliMethod
+        :type method: :class:`SmaliMethod`
         :param instance: the smali object
-        :type instance: SmaliObject
+        :type instance: :class:`SmaliObject`
         :raises NoSuchMethodError: if no frame is registered to the given method
         :raises ExecutionError: if an error occurs while execution
         :return: the return value of the executed method
         :rtype: object
         """
         mhash = hash(method)
         if mhash not in self.__frames:
-            raise NoSuchMethodError(f'Method not registered! {method}')
+            raise NoSuchMethodError(f"Method not registered! {method}")
 
         frame: Frame = self.__frames[mhash]
         frame.reset()
         for i in range(method.locals):
             frame.registers[f"v{i}"] = None
 
         if method.modifiers not in AccessType.STATIC:
             if not instance:
                 raise ExecutionError(
-                    'NullPtrError', f"Expected instance of '{instance.smali_class.name}'")
+                    "NullPtrError",
+                    f"Expected instance of '{instance.smali_class.name}'",
+                )
             frame.registers["p0"] = instance
 
         # validate method and set parameter values
         self._validate_call(method, frame, args, kwargs)
         while not frame.finished:
             opcode_exec, args = frame.opcodes[frame.pos]
             opcode_exec.args = args
@@ -236,59 +264,62 @@
                 registers[key] = value
 
         start = 1 if method.modifiers not in AccessType.STATIC else 0
         for i, value in enumerate(args, start=start):
             registers[f"p{i}"] = value
 
         if len(parameters) != len(registers):
-            raise ValueError('Invalid argument count! - expected %s, got %d' % (
-                len(parameters), len(registers)
-            ))
+            raise ValueError(
+                "Invalid argument count! - expected %s, got %d"
+                % (len(parameters), len(registers))
+            )
 
         for param, register in zip(parameters, registers):
             param_type = Type(param)
             # Lookup primitive types
             for primitive, ptypes in self.__type_map.items():
                 if param_type.class_name in ptypes:
                     if not isinstance(registers[register], primitive):
-                        raise TypeError('Invalid type for parameter, expected %s - got %s' % (
-                            param, type(registers[register])
-                        ))
+                        raise TypeError(
+                            "Invalid type for parameter, expected %s - got %s"
+                            % (param, type(registers[register]))
+                        )
 
             if param_type.descriptor not in self.__classes:
                 raise NoSuchClassError(f'Class "{param_type.descriptor}" not defined!')
 
         frame.registers.update(registers)
 
+
 ####################################################################################################
 # INTERNAL
 ####################################################################################################
 
-class _SourceAnnotationVisitor(AnnotationVisitor):
 
+class _SourceAnnotationVisitor(AnnotationVisitor):
     annotation: SmaliAnnotation
     """The final annotation"""
 
     def __init__(self, annotation: SmaliAnnotation) -> None:
         super().__init__(None)
         self.annotation = annotation
 
     def visit_value(self, name: str, value) -> None:
         self.annotation[name] = SmaliValue(value)
 
     def visit_array(self, name: str, values: list) -> None:
-        self.annotation[name] = [
-            SmaliValue(x) for x in values
-        ]
+        self.annotation[name] = [SmaliValue(x) for x in values]
 
     def visit_enum(self, name: str, owner: str, const: str, value_type: str) -> None:
         # TODO: handle enum values
         return super().visit_enum(name, owner, const, value_type)
 
-    def visit_subannotation(self, name: str, access_flags: int, signature: str) -> 'AnnotationVisitor':
+    def visit_subannotation(
+        self, name: str, access_flags: int, signature: str
+    ) -> "AnnotationVisitor":
         sub = SmaliAnnotation(self.annotation, signature, access_flags)
         self.annotation[name] = sub
         return _SourceAnnotationVisitor(sub)
 
 
 class _SourceFieldVisitor(FieldVisitor):
     field: SmaliField
@@ -331,16 +362,15 @@
         self.method.locals = registers - len(self.method.parameters)
 
     def visit_catch(self, exc_name: str, blocks: tuple) -> None:
         start, _, handler = blocks
         self.frame.catch[start] = (exc_name, handler)
 
     def visit_catchall(self, exc_name: str, blocks: tuple) -> None:
-        start, _, handler = blocks
-        self.frame.catch[start] = (exc_name, handler)
+        self.visit_catch(exc_name, blocks)
 
     def visit_goto(self, block_name: str) -> None:
         self.frame.opcodes.append((executor.goto, block_name))
         self.pos += 1
 
     def visit_array_data(self, length: str, value_list: list) -> None:
         self.frame.array_data[self._last_label] = value_list
@@ -352,34 +382,47 @@
     def visit_return(self, ret_type: str, args: list) -> None:
         if ret_type:
             self.visit_instruction(f"return-{ret_type}", args)
         else:
             self.visit_instruction("return", args)
 
     def visit_instruction(self, ins_name: str, args: list) -> None:
+        cache: dict = self.frame.vm.executors
         for _, value in opcode.__dict__.items():
+             # If the value of an attribute is equal to the given instruction
+             # name,
             if value == ins_name:
-                self.frame.opcodes.append((executor.executor(ins_name), args))
+                # Check if the instruction name is not in the list of executors
+                # in the current frame's virtual machine
+                if ins_name not in cache and not self.frame.vm.use_strict:
+                    # If not, add a tuple of the "nop" opcode function and the
+                    # instruction arguments to the frame's opcodes list.
+                    func = cache["nop"] if "nop" in cache else executor.nop
+                    self.frame.opcodes.append((func, args))
+                else:
+                    # If yes, add a tuple of the executor function for the instruction
+                    # name and the instruction arguments to the frame's opcodes list.
+                    self.frame.opcodes.append((self.frame.vm.executors[ins_name], args))
                 self.pos += 1
                 return
 
-        raise InvalidOpcodeError(f'Invalid OpCode: {ins_name}')
+        raise InvalidOpcodeError(f"Invalid OpCode: {ins_name}")
 
     def visit_packed_switch(self, value: str, blocks: list) -> None:
         self.frame.switch_data[self._last_label] = (value, blocks)
 
     def visit_sparse_switch(self, branches: dict) -> None:
         self.frame.switch_data[self._last_label] = branches
 
-class _SourceClassVisitor(ClassVisitor):
 
+class _SourceClassVisitor(ClassVisitor):
     smali_class: SmaliClass
     """The result class object"""
 
-    vm : SmaliVM
+    vm: SmaliVM
     """The vm used wihtin method visitor objects"""
 
     def __init__(self, vm: SmaliVM, smali_class: SmaliClass = None) -> None:
         super().__init__()
         self.vm = vm
         self.smali_class = smali_class
 
@@ -387,26 +430,36 @@
         annotation = SmaliAnnotation(self.smali_class, signature, access_flags)
         self.smali_class.annotations.append(annotation)
         return _SourceAnnotationVisitor(annotation)
 
     def visit_class(self, name: str, access_flags: int) -> None:
         self.smali_class = SmaliClass(None, name, access_flags)
 
-    def visit_inner_class(self, name: str, access_flags: int) -> 'ClassVisitor':
+    def visit_inner_class(self, name: str, access_flags: int) -> "ClassVisitor":
         inner = SmaliClass(self.smali_class, name, access_flags)
         self.smali_class[name] = inner
         return _SourceClassVisitor(self.vm, inner)
 
-    def visit_field(self, name: str, access_flags: int, field_type: str, value=None) -> FieldVisitor:
-        field = SmaliField(self.smali_class, f"{name}:{field_type}", access_flags,
-                           name, Type(field_type), value=SmaliValue(value) if value else None)
+    def visit_field(
+        self, name: str, access_flags: int, field_type: str, value=None
+    ) -> FieldVisitor:
+        field = SmaliField(
+            self.smali_class,
+            f"{name}:{field_type}",
+            access_flags,
+            name,
+            Type(field_type),
+            value=SmaliValue(value) if value else None,
+        )
         self.smali_class[name] = field
         return _SourceFieldVisitor(field)
 
-    def visit_method(self, name: str, access_flags: int, parameters: list, return_type: str) -> MethodVisitor:
+    def visit_method(
+        self, name: str, access_flags: int, parameters: list, return_type: str
+    ) -> MethodVisitor:
         signature = f"{name}({''.join(parameters)}){return_type}"
         method = SmaliMethod(self.vm, self.smali_class, signature, access_flags)
         visitor = _SourceMethodVisitor(method)
         self.vm.new_frame(method, visitor.frame)
         self.smali_class[name] = method
         return visitor
 
@@ -414,39 +467,39 @@
         self.smali_class.interfaces.append(interface)
 
     def visit_super(self, super_class: str) -> None:
         self.smali_class.super_cls = super_class
 
 
 class _SmaliClassLoader(ClassLoader):
-
     vm: SmaliVM
     """The vm storing all defined classes."""
 
     def __init__(self, vm: SmaliVM) -> None:
         self.vm = vm
 
     def define_class(self, source: bytes) -> SmaliClass:
         reader = SmaliReader(validate=True, comments=False)
 
         visitor = _SourceClassVisitor(self.vm)
         reader.visit(source, visitor)
         smali_class = visitor.smali_class
         if not smali_class:
-            raise ValueError('Could not parse class!')
+            raise ValueError("Could not parse class!")
 
         self.vm.new_class(smali_class)
         return smali_class
 
     def load_class(self, source: str, init=True, lookup_missing=False) -> SmaliClass:
         smali_class = self.define_class(source)
         if init:
             smali_class.clinit()
         return smali_class
 
+
 ####################################################################################################
 # EXTERNAL
 ####################################################################################################
 SmaliVMAnnotationReader = _SourceAnnotationVisitor
 SmaliVMFieldReader = _SourceFieldVisitor
 SmaliVMMethodReader = _SourceMethodVisitor
 SmaliVMClassReader = _SourceClassVisitor
```

### Comparing `pysmali-0.1.1/smali/opcode.py` & `pysmali-0.1.2/smali/opcode.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.1/smali/reader.py` & `pysmali-0.1.2/smali/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,42 +22,39 @@
 import io
 
 from smali.visitor import (
     VisitorBase,
     ClassVisitor,
     FieldVisitor,
     AnnotationVisitor,
-    MethodVisitor
-)
-from smali.base import (
-    AccessType,
-    Line,
-    Token,
-    Type,
-    SmaliValueProxy
+    MethodVisitor,
 )
+from smali.base import AccessType, Line, Token, Type, SmaliValueProxy
 from smali.opcode import RETURN, GOTO
 
+
 class SupportsCopy:
     """Interface for classes that can react as a copy handler for a SmaliReader.
 
     Note that the context is used to distinguish the current visitor.
     """
 
     def copy(self, line: str, context: type = ClassVisitor) -> None:
         """Copies the given line.
 
         :param line: the line to copy
         :type line: str
         """
 
+
 EMPTY_ANNOV = AnnotationVisitor()
 EMPTY_METHV = MethodVisitor()
 EMPTY_FIELDV = FieldVisitor()
 
+
 class SmaliReader:
     """Basic implementation of a line-base Smali-SourceCode parser.
 
     :param validate: Indicates the reader should validate the input code, defaults to True
     :type validate: bool, optional
     :param comments: With this option enabled, the parser will also notify about
                         comments in the source file, defaults to False
@@ -89,61 +86,66 @@
     stack: list = []
     """Stores the current visitors (index 0 stores the initial visitor)
 
     A null value indicates that no visitors are registered for the current parsing
     context.
     """
 
-    errors: str = 'strict'
+    errors: str = "strict"
     """Indicates whether this reader should throw errors (values: 'strict', 'ignore')"""
 
     copy_handler: SupportsCopy
 
-    def __init__(self, validate: bool = True, comments: bool = False,
-                 snippet: bool = False, errors: str = 'strict') -> None:
+    def __init__(
+        self,
+        validate: bool = True,
+        comments: bool = False,
+        snippet: bool = False,
+        errors: str = "strict",
+    ) -> None:
         self.validate = validate
         self.comments = comments
         self.snippet = snippet
         self.errors = errors
         self.copy_handler = None
         # check valid values
-        if self.errors not in ('ignore', 'strict'):
-            raise ValueError(f'Invalid error handler: {errors}')
+        if self.errors not in ("ignore", "strict"):
+            raise ValueError(f"Invalid error handler: {errors}")
 
     def visit(self, source: io.IOBase, visitor: ClassVisitor) -> None:
         """Parses the given input which can be any readable source.
 
         :param source: the Smali source code
         :type source: io.IOBase | str | bytes
         :param visitor: the visitor to use, defaults to None
         :type visitor: ClassVisitor, optional
         :raises ValueError: If the provided values are null
         :raises TypeError: if the source type is not accepted
         :raises ValueError: if the source is not readable
         """
         if not visitor or not source:
-            raise ValueError('Invalid source or visitor (nullptr)')
+            raise ValueError("Invalid source or visitor (nullptr)")
 
         # Wrap string and bytes instances automatically.
         if isinstance(source, str):
             source = io.StringIO(source)
 
         elif isinstance(source, bytes):
             source = io.BytesIO(source)
 
         # The TypeError is needed to provide information about
         # types we don't accept
         elif not isinstance(source, io.IOBase):
             raise TypeError(f"Invalid source type: {source.__class__}")
 
         if not source.readable():
-            raise ValueError('Source object is not readable!')
+            raise ValueError("Source object is not readable!")
 
-        if self.errors not in ('ignore', 'strict'):
-            raise ValueError(f'Invalid error handling type: {self.errors}')
+        if self.errors not in ("ignore", "strict"):
+            raise ValueError(f"Invalid error handling type: {self.errors}")
 
         self.source = source
         self.stack.append(visitor)
 
         # We need to parse the class definition first if needed
         if not self.snippet:
             self._class_def()
@@ -184,15 +186,15 @@
 
             # Sort out blank lines without anything
             if not raw_line:
                 continue
 
             self.line.reset(raw_line)
             # Comments will be returned immediately
-            if raw_line.strip().startswith('#'):
+            if raw_line.strip().startswith("#"):
                 if self._visitor and self.comments:
                     self._visitor.visit_comment(self.line.eol_comment)
                 elif not self._visitor and self.comments:
                     self._copy_line()
                 continue
 
             # return nothing as the line object is defined globally
@@ -211,15 +213,15 @@
         :type expected: str
         :raises SyntaxError: if validation failed
         :meta public:
         """
         if not self.validate:
             return
 
-        if token[0] != '.':
+        if token[0] != ".":
             raise SyntaxError(f"Expected '.' before token - got '{token[0]}'")
 
         if token[1:] != expected:
             raise SyntaxError(f"Expected '{expected}' - got '{token[1:]}'")
 
     def _validate_descriptor(self, name: str) -> None:
         """Validates the given name if validation is enabled.
@@ -261,15 +263,15 @@
                 break
 
             flags.append(self.line.peek())
             next(self.line)
         return flags
 
     def _throw_eol(self, err):
-        if self.errors == 'strict':
+        if self.errors == "strict":
             raise SyntaxError("Unexpected EOL (end of line)") from err
 
     def _collect_values(self, strip_chars=None) -> list:
         """Collects all values stored in the rest of the current line.
 
         Note that values will be splitted if ',' is in a value, for instance:
         >>> line = "const/16 b,0xB"
@@ -283,16 +285,20 @@
         :meta public:
         """
         i_values = []
         while self.line.has_next():
             value = next(self.line).rstrip(strip_chars)
             # As the Line object splits all values by ' ', strings can
             # be marked by their '"' at the start or end.
-            if value[0] not in  ('"', "'") and value[-1] not in ('"', "'") and ',' in value:
-                i_values.extend(value.split(','))
+            if (
+                value[0] not in ('"', "'")
+                and value[-1] not in ('"', "'")
+                and "," in value
+            ):
+                i_values.extend(value.split(","))
             else:
                 i_values.append(value)
         return i_values
 
     def _do_visit(self) -> None:
         """Performs the source code visit.
 
@@ -311,18 +317,18 @@
                     # These are just blank lines used in the original
                     # source file.
                     self._copy_line()
                     continue
 
                 statement = self.line.peek()
                 # Tokens start with a leading dot
-                if statement[0] == '.':
+                if statement[0] == ".":
                     self._handle_token()
                 # The same with blocks and a ':'
-                elif statement[0] == ':':
+                elif statement[0] == ":":
                     self._handle_block()
 
                 elif isinstance(self._visitor, AnnotationVisitor):
                     self._handle_value()
 
                 elif isinstance(self._visitor, MethodVisitor):
                     self._handle_instruction()
@@ -390,15 +396,15 @@
             # Only parse the next line if we have to
             try:
                 self._next_line()
             except EOFError as eof:
                 # It should be possible to parse small code snippets.
                 if not self.validate:
                     return
-                raise SyntaxError('Expected a class defintion - got EOF') from eof
+                raise SyntaxError("Expected a class defintion - got EOF") from eof
 
         try:
             # If validation is enabled, the '.class' token is verified
             token = next(self.line)
             self._validate_token(token, Token.CLASS)
 
             flags = self._read_access_flags()
@@ -417,27 +423,29 @@
 
             # Don't forget the comment
             self._publish_comment()
             return c_visitor
         except StopIteration as err:
             self._throw_eol(err)
 
-###########################################################################################
-# TOKEN IMPLEMENTATION
-###########################################################################################
+    ###########################################################################################
+    # TOKEN IMPLEMENTATION
+    ###########################################################################################
 
     def _handle_super(self) -> None:
         try:
             # If validation is enabled, the '.super' token is verified
             token = next(self.line)
             self._validate_token(token, Token.SUPER)
 
             super_class = self.line.peek()
             if not SmaliValueProxy.is_type_descriptor(super_class):
-                raise SyntaxError(f"Expected super-class type descriptor - got '{super_class}'")
+                raise SyntaxError(
+                    f"Expected super-class type descriptor - got '{super_class}'"
+                )
 
             if self._visitor:
                 # Visit the class afterwards
                 self._visitor.visit_super(super_class)
             else:
                 self._copy_line()
             self._publish_comment()
@@ -451,15 +459,15 @@
         :type visitor: ClassVisitor
         :meta public:
         """
         try:
             token = next(self.line)
             self._validate_token(token, Token.SOURCE)
 
-            source = self.line.peek().replace('"', '')
+            source = self.line.peek().replace('"', "")
             if self._visitor:
                 self._visitor.visit_source(source)
             else:
                 self._copy_line()
             self._publish_comment()
         except StopIteration as err:
             self._throw_eol(err)
@@ -471,27 +479,29 @@
             self._validate_token(token, Token.FIELD)
 
             flags = self._read_access_flags()
             access_flags = AccessType.get_flags(flags)
 
             # The structure of a field's name is the following:
             #   - <name>:<descriptor>
-            name, descriptor = next(self.line).split(':')
+            name, descriptor = next(self.line).split(":")
             self._validate_descriptor(descriptor)
 
             # Handle bracket names
-            name = name.rstrip('>').lstrip('<')
+            name = name.rstrip(">").lstrip("<")
 
             # If we have a direct assignment, we should parse the value
             value = None
             if self.line.has_next():
                 value = self.line.last()
 
             if self._visitor:
-                f_visitor = self._visitor.visit_field(name, access_flags, descriptor, value)
+                f_visitor = self._visitor.visit_field(
+                    name, access_flags, descriptor, value
+                )
                 self._publish_comment()
             else:
                 f_visitor = EMPTY_FIELDV
 
             self.stack.append(f_visitor if f_visitor else EMPTY_FIELDV)
             if not f_visitor or f_visitor == EMPTY_FIELDV:
                 self._copy_line()
@@ -525,16 +535,18 @@
 
             # We don't need to verify the signature as this is done
             # in the Type class
             signature = Type(self.line.peek())
             m_visitor = EMPTY_METHV
             if self._visitor:
                 m_visitor = self._visitor.visit_method(
-                    signature.get_method_name(), access_flags,
-                    signature.get_method_params(), signature.get_method_return_type()
+                    signature.get_method_name(),
+                    access_flags,
+                    signature.get_method_params(),
+                    signature.get_method_return_type(),
                 )
 
             # Add the visitor first before publishing the comment
             self.stack.append(m_visitor if m_visitor else EMPTY_METHV)
             self._publish_comment()
             # The line will be copied if no visitor has been set
             if not m_visitor or m_visitor == EMPTY_METHV:
@@ -573,50 +585,52 @@
             self._throw_eol(err)
 
     def _handle_subannotation(self) -> None:
         """Handles .subannotation definitions."""
         try:
             # As we need the annotation value's name, we have to
             # use the cleaned line buffer in the current line object.
-            name = self.line.cleaned[self.line.cleaned.find(' '):]
+            name = self.line.cleaned[self.line.cleaned.find(" ") :]
             flags = self._read_access_flags()
             access_flags = AccessType.get_flags(flags)
 
             descriptor = self.line.peek()
             self._validate_descriptor(descriptor)
 
             a_visitor = EMPTY_ANNOV
             if self._visitor and self._visitor != EMPTY_ANNOV:
-                a_visitor = self._visitor.visit_subannotation(name, access_flags, descriptor)
+                a_visitor = self._visitor.visit_subannotation(
+                    name, access_flags, descriptor
+                )
 
             self.stack.append(a_visitor)
             self._publish_comment()
             if not a_visitor or a_visitor == EMPTY_ANNOV:
                 self._copy_line()
         except StopIteration as err:
             self._throw_eol(err)
 
     def _handle_enum(self) -> None:
         """Handles .enum definitions in Annotations or SubAnnotations."""
         try:
             # As we need the annotation value's name, we have to
             # use the cleaned line buffer in the current line object.
-            name = self.line.cleaned[self.line.cleaned.find(' '):]
+            name = self.line.cleaned[self.line.cleaned.find(" ") :]
 
             token = next(self.line)
             self._validate_token(token, Token.ENUM)
 
             # UNSAFE
-            descriptor, value = self.line.peek().split('->')
+            descriptor, value = self.line.peek().split("->")
             self._validate_descriptor(descriptor)
 
-            val_name, val_descriptor = value.split(':')
+            val_name, val_descriptor = value.split(":")
             self._validate_descriptor(val_descriptor)
 
-            val_name = val_name.rstrip('>').lstrip('<')
+            val_name = val_name.rstrip(">").lstrip("<")
             if self._visitor and self._visitor != EMPTY_ANNOV:
                 self._visitor.visit_enum(name, descriptor, val_name, val_descriptor)
             else:
                 self._copy_line()
 
         except StopIteration as err:
             self._throw_eol(err)
@@ -630,48 +644,51 @@
         if self._visitor:
             # Visit the class afterwards
             self._visitor.visit_super(int(enbaled))
         else:
             self._copy_line()
         self._publish_comment()
 
-###########################################################################################
-# ANNOTATION VALUE IMPLEMENTATION
-###########################################################################################
+    ###########################################################################################
+    # ANNOTATION VALUE IMPLEMENTATION
+    ###########################################################################################
 
     def _handle_value(self) -> None:
         val_name = next(self.line)
         # Skip the assignment operator ('=')
         next(self.line)
 
         statement = self.line.peek()
 
-        if statement[0] == '.':
+        if statement[0] == ".":
             self._handle_token()
 
         # We either have a normal value or an array of values
         else:
             do_copy = not self._visitor or self._visitor == EMPTY_ANNOV
             cleaned = self.line.cleaned
             if do_copy:
                 self._copy_line()
 
-            if '{' in cleaned:
-                if '}' in cleaned:
+            if "{" in cleaned:
+                if "}" in cleaned:
                     a_values = [
-                        x.strip() for x in cleaned[cleaned.find('{')+1 : cleaned.find('}')].split(',')
+                        x.strip()
+                        for x in cleaned[
+                            cleaned.find("{") + 1 : cleaned.find("}")
+                        ].split(",")
                     ]
                 else:
                     # Read lines until '}' is at line's end, but publish
                     # an EOL comment before
                     self._publish_comment()
                     a_values = []
                     self._next_line()
-                    while self.line.cleaned[-1] != '}' and self.line.cleaned[0] != '}':
-                        value = self.line.peek().rstrip(',')
+                    while self.line.cleaned[-1] != "}" and self.line.cleaned[0] != "}":
+                        value = self.line.peek().rstrip(",")
 
                         # Don't forget to publish a line comment
                         self._publish_comment()
                         a_values.append(value)
                         if do_copy:
                             self._copy_line()
                         self._next_line()
@@ -680,17 +697,17 @@
                 if self._visitor and self._visitor != EMPTY_ANNOV:
                     self._visitor.visit_array(val_name, a_values)
 
             # Parse a simple value
             elif self._visitor and self._visitor != EMPTY_ANNOV:
                 self._visitor.visit_value(val_name, self.line.peek())
 
-###########################################################################################
-# METHOD SPECIFIC IMPLEMENTATION
-###########################################################################################
+    ###########################################################################################
+    # METHOD SPECIFIC IMPLEMENTATION
+    ###########################################################################################
 
     def _handle_param(self) -> None:
         if not self._visitor or self._visitor == EMPTY_METHV:
             self._copy_line()
             return
 
         # Skip '.param' instruction
@@ -709,30 +726,39 @@
         if func:
             func(int(number))
             self._publish_comment()
         else:
             self._copy_line()
 
     def _handle_line(self) -> None:
-        self._handle_method_int(Token.LINE,
-            self._visitor.visit_line if self._visitor not in (None, EMPTY_METHV) else None
+        self._handle_method_int(
+            Token.LINE,
+            self._visitor.visit_line
+            if self._visitor not in (None, EMPTY_METHV)
+            else None,
         )
 
     def _handle_registers(self) -> None:
-        self._handle_method_int(Token.REGISTERS,
-            self._visitor.visit_registers if self._visitor  not in (None, EMPTY_METHV) else None
+        self._handle_method_int(
+            Token.REGISTERS,
+            self._visitor.visit_registers
+            if self._visitor not in (None, EMPTY_METHV)
+            else None,
         )
 
     def _handle_locals(self) -> None:
-        self._handle_method_int(Token.LOCALS,
-            self._visitor.visit_locals if self._visitor  not in (None, EMPTY_METHV) else None
+        self._handle_method_int(
+            Token.LOCALS,
+            self._visitor.visit_locals
+            if self._visitor not in (None, EMPTY_METHV)
+            else None,
         )
 
     def _handle_block(self) -> None:
-        block_id = self.line.peek().lstrip(':')
+        block_id = self.line.peek().lstrip(":")
         if self._visitor and self._visitor not in (None, EMPTY_METHV):
             self._visitor.visit_block(block_id)
             self._publish_comment()
         else:
             self._copy_line()
 
     def _handle_catch(self, is_catchall=False) -> None:
@@ -744,20 +770,20 @@
         next(self.line)
         # 1. Handle the exception descriptor
         descriptor = self.line.peek()
         self._validate_descriptor(descriptor)
 
         # 2. Collect try_start and try_end blocks
         cleaned = self.line.cleaned
-        try_start, _, try_end = (cleaned[cleaned.find('{')+1 : cleaned.find('}')]
-            .strip()
-            .split(' '))
+        try_start, _, try_end = (
+            cleaned[cleaned.find("{") + 1 : cleaned.find("}")].strip().split(" ")
+        )
         catch_block = self.line.last()
 
-        values = (try_start.lstrip(':'), try_end.lstrip(':'), catch_block.lstrip(':'))
+        values = (try_start.lstrip(":"), try_end.lstrip(":"), catch_block.lstrip(":"))
         if is_catchall:
             self._visitor.visit_catchall(descriptor, values)
         else:
             self._visitor.visit_catch(descriptor, values)
         self._publish_comment()
 
     def _handle_instruction(self) -> None:
@@ -771,42 +797,45 @@
         :meta public:
         """
         if not self._visitor or self._visitor == EMPTY_METHV:
             self._copy_line()
             return
 
         instruction = next(self.line)
-        sub_ins = "" if '-' not in instruction else instruction[instruction.find('-')+1 :]
-        if instruction.startswith('invoke'):
+        sub_ins = (
+            "" if "-" not in instruction else instruction[instruction.find("-") + 1 :]
+        )
+        if instruction.startswith("invoke"):
             # Invoke instructions will be handles separately as they have
             # as special structure
             cleaned = self.line.cleaned
             args = [
-                x.strip() for x in cleaned[cleaned.find('{')+1 : cleaned.find('}')].split(',')
+                x.strip()
+                for x in cleaned[cleaned.find("{") + 1 : cleaned.find("}")].split(",")
             ]
 
             # Maybe replace this with a method call in Line
             method_sig = self.line.last()
 
-            descriptor, signature = method_sig.split('->')
+            descriptor, signature = method_sig.split("->")
             self._validate_descriptor(descriptor)
 
             self._visitor.visit_invoke(sub_ins, args, descriptor, signature)
         elif instruction.startswith(RETURN):
             # Return statements are handled separately to make building
             # Smali files easier
-            i_values = self._collect_values(',')
+            i_values = self._collect_values(",")
             self._visitor.visit_return(sub_ins, i_values)
 
         elif instruction == GOTO:
             # Goto instructions are handled directly
-            block = self.line.peek().lstrip(':')
+            block = self.line.peek().lstrip(":")
             self._visitor.visit_goto(block)
         else:
-            i_values = self._collect_values(',')
+            i_values = self._collect_values(",")
             if self._visitor and self._visitor != EMPTY_METHV:
                 self._visitor.visit_instruction(instruction, i_values)
         # Don't forget the EOL comment
         self._publish_comment()
 
     def _handle_packed_switch(self) -> None:
         do_copy = not self._visitor or self._visitor == EMPTY_METHV
@@ -820,16 +849,16 @@
 
         blocks = []
         while True:
             next_value = next(self.line)
             self._publish_comment()
             if do_copy:
                 self._copy_line()
-            if next_value[0] == ':':
-                blocks.append(next_value.lstrip(':'))
+            if next_value[0] == ":":
+                blocks.append(next_value.lstrip(":"))
             elif Token.END.value in next_value:
                 # Use this method to prevent looping forever
                 break
             self._next_line()
 
         if self._visitor and self._visitor != EMPTY_METHV:
             self._visitor.visit_packed_switch(value, blocks)
@@ -854,15 +883,15 @@
         self._publish_comment()
         self._next_line()
         while True:
             value = self.line.peek()
             self._publish_comment()
             if do_copy:
                 self._copy_line()
-            if value[0] == '.' and value[1:] == Token.END.value:
+            if value[0] == "." and value[1:] == Token.END.value:
                 break
             values.append(value)
 
         if self._visitor and self._visitor != EMPTY_METHV:
             self._visitor.visit_array_data(length, values)
 
     def _handle_local(self) -> None:
@@ -872,18 +901,20 @@
             return
 
         # Skip the instruction
         next(self.line)
 
         values = self._collect_values()
         if len(values) != 3 and self.validate:
-            raise SyntaxError(f'Expected 3 values in ".local" statement - got {len(values)}')
+            raise SyntaxError(
+                f'Expected 3 values in ".local" statement - got {len(values)}'
+            )
 
         register = values[0]
-        name, descriptor = values[1].split(':')
+        name, descriptor = values[1].split(":")
         full_desc = values[2]
         self._validate_descriptor(descriptor)
         self._validate_descriptor(full_desc)
 
         self._visitor.visit_local(register, name.strip('"'), descriptor, full_desc)
         self._publish_comment()
 
@@ -900,18 +931,18 @@
         self._publish_comment()
         self._next_line()
         while True:
             key = self.line.peek()
             self._publish_comment()
             if do_copy:
                 self._copy_line()
-            if key[0] == '.' and key[1:] == Token.END.value:
+            if key[0] == "." and key[1:] == Token.END.value:
                 break
             # Add the block id without leading ':'
-            values[key] = self.line.last().lstrip(':')
+            values[key] = self.line.last().lstrip(":")
 
         if self._visitor and self._visitor != EMPTY_METHV:
             self._visitor.visit_sparse_switch(values)
             self._publish_comment()
 
     def _handle_prologue(self) -> None:
         if self._visitor and self._visitor != EMPTY_METHV:
```

### Comparing `pysmali-0.1.1/smali/shell/__init__.py` & `pysmali-0.1.2/smali/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.1/smali/shell/__main__.py` & `pysmali-0.1.2/smali/shell/__main__.py`

 * *Files identical despite different names*

### Comparing `pysmali-0.1.1/smali/shell/cli.py` & `pysmali-0.1.2/smali/shell/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,38 +16,55 @@
 import sys
 
 from argparse import ArgumentParser
 
 from smali import VERSION
 from smali.shell import ISmaliShell
 
+
 def start_cli():
     """Starts the Smali interpreter."""
-    
-    parser = ArgumentParser(description=(
-        "ISmali (Interactive Smali interpreter) can execute Smali-Code snippets"
-        "on the fly as well as import *.smali files and use them later on."
-    ))
-    parser.add_argument('file', nargs='*',
-        help=("The Smali-Script files ('.ssf') to be interpreted. Note that"
-              " files as input won't result in interactive mode. Use the '-i'"
-              " flag to run the interactive mode afterwards."))
-    parser.add_argument('-i', '--interactive', action='store_true',
-        help=("Runs the interactive mode after executing/ importing input files."))
-    parser.add_argument('--version', action='store_true', 
-        help="Stores the current interpreter version")
+
+    parser = ArgumentParser(
+        description=(
+            "ISmali (Interactive Smali interpreter) can execute Smali-Code snippets"
+            "on the fly as well as import *.smali files and use them later on."
+        )
+    )
+    parser.add_argument(
+        "file",
+        nargs="*",
+        help=(
+            "The Smali-Script files ('.ssf') to be interpreted. Note that"
+            " files as input won't result in interactive mode. Use the '-i'"
+            " flag to run the interactive mode afterwards."
+        ),
+    )
+    parser.add_argument(
+        "-i",
+        "--interactive",
+        action="store_true",
+        help=("Runs the interactive mode after executing/ importing input files."),
+    )
+    parser.add_argument(
+        "--version", action="store_true", help="Stores the current interpreter version"
+    )
 
     args = parser.parse_args().__dict__
-    if args['version']:
+    if args["version"]:
         print(VERSION)
         sys.exit(0)
 
     shell = ISmaliShell()
-    files = args['file']
+    files = args["file"]
 
     if len(files) > 0:
-        for path in args['file']:
+        for path in args["file"]:
             shell.do_import(path)
 
-    if len(files) == 0 or args['interactive']:
-        shell.cmdloop((f"ISmali {VERSION} on {sys.platform}\nType"
-            " 'help' or 'copyright' for more information."))
+    if len(files) == 0 or args["interactive"]:
+        shell.cmdloop(
+            (
+                f"ISmali {VERSION} on {sys.platform}\nType"
+                " 'help' or 'copyright' for more information."
+            )
+        )
```

### Comparing `pysmali-0.1.1/smali/shell/model.py` & `pysmali-0.1.2/smali/shell/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """The root class"""
 
     shell: 'ISmaliShell'
     """The shell reference"""
 
     last_label: str
     """Stores the last label that has been typed"""
-    
+
     importing: bool = False
 
     def __init__(self, shell: 'ISmaliShell') -> None:
         super().__init__(None)
         self.shell = shell
         self.frame = Frame()
         self.last_label = None
@@ -105,15 +105,15 @@
 
     def visit_catchall(self, exc_name: str, blocks: tuple) -> None:
         self.visit_catch(exc_name, blocks)
 
     def visit_instruction(self, ins_name: str, args: list) -> None:
         for _, value in opcode.__dict__.items():
             if value == ins_name:
-                exc = executor.executor(ins_name)
+                exc = executor.get_executor(ins_name)
                 exc.args = args
                 exc(self.frame)
                 self.pos += 1
 
                 if 'return' in value:
                     print(self.frame.return_value)
                 return
@@ -126,15 +126,15 @@
     def visit_field(self, name: str, access_flags: int, field_type: str,
                     value=None) -> FieldVisitor:
         field = SmaliField(self.shell.root.smali_class, f"{name}:{field_type}", access_flags,
                            name, Type(field_type), value=SmaliValue(value) if value else None)
         self.shell.root.smali_class[name] = field
         if access_flags not in AccessType.STATIC and value is not None:
             self.shell.root[name] = value
-        
+
         return SmaliVMFieldReader(field)
 
     def visit_return(self, ret_type: str, args: list) -> None:
         if ret_type:
             self.visit_instruction(f"return-{ret_type}", args)
         else:
             self.visit_instruction("return", args)
@@ -151,20 +151,20 @@
         smali_class = self.shell.root.smali_class
 
         method = SmaliMethod(self.shell.emulator, smali_class, signature, access_flags)
         visitor = SmaliVMMethodReader(method)
         self.shell.emulator.new_frame(method, visitor.frame)
         smali_class[name] = method
         return visitor
-    
+
     def visit_inner_class(self, name: str, access_flags: int) -> 'ClassVisitor':
         if self.importing:
             smali_class = self.shell.root.smali_class
             inner = SmaliClass(smali_class, name, access_flags)
-            
+
             smali_class[name] = inner
             return SmaliVMClassReader(self.shell.emulator, inner)
 
 
 class ISmaliShell(Cmd):
     """Implementation of an interactive Smali-Interpreter."""
 
@@ -184,18 +184,18 @@
     """The actual VM reference that will execute each method"""
 
     root: SmaliObject
     """The base context used to define fields and methods."""
 
     prompt: str = '>>> '
     """The prompt used by ``cmd.Cmd``"""
-    
+
     check_import: bool = True
     """Used to indicate whether this shell should verify each import"""
-    
+
     __imported_files: list = []
     """Internal file list"""
 
     def __init__(self) -> None:
         super().__init__()
         self.stack = []
         self.reader = SmaliReader(comments=False, snippet=True)
@@ -212,15 +212,15 @@
         This command will try to import the given smali file or
         Smali-Script file (.ssf). Note that files with wrong suffixes
         will be ignored.
         """
         if not os.path.exists(path):
             print(f'! Could not find file at "{path}"')
             return
-            
+
         if path in self.__imported_files and self.check_import:
             return
 
         if not path.endswith(('.smali', f".{SMALI_SCRIPT_SUFFIX}")):
             print(f"! Unknown file format (unknown suffix) at '{path}'")
             return
 
@@ -229,15 +229,15 @@
             self.__imported_files.append(path)
             if path.endswith(f".{SMALI_SCRIPT_SUFFIX}"):
                 self.visitor.importing = True
                 self.reader.visit(source, self.visitor)
                 self.visitor.importing = False
             else:
                 cls = self.emulator.classloader.load_class(source, init=False)
-            
+
 
         try:
             if cls is not None:
                 cls.clinit()
         except Exception: # :noqa
             print(traceback.format_exc())
```

### Comparing `pysmali-0.1.1/smali/visitor.py` & `pysmali-0.1.2/smali/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+
 class VisitorBase:
     """Base class for Smali-Class visitor classes.
 
     :param delegate: A delegate visitor, defaults to None
     :type delegate: BaseVisitor subclass, optional
     """
-    def __init__(self, delegate: 'VisitorBase' = None) -> None:
+
+    def __init__(self, delegate: "VisitorBase" = None) -> None:
         self.delegate = delegate
         # does not apply to muliple inheritance
         if delegate and not isinstance(delegate, self.__class__.__base__):
             raise TypeError(
-                f'Invalid Visitor type - expected subclass of {self.__class__}')
+                f"Invalid Visitor type - expected subclass of {self.__class__}"
+            )
 
     def visit_comment(self, text: str) -> None:
         """Visits a comment string.
 
         Important: if you want to visit inline comments (EOL comments)
         use `#visit_eol_comment()` instead.
 
@@ -75,15 +78,17 @@
         :type name: str
         :param values: the array's values
         :type values: list
         """
         if self.delegate:
             self.visit_array(name, values)
 
-    def visit_subannotation(self, name: str, access_flags: int, signature: str) -> 'AnnotationVisitor':
+    def visit_subannotation(
+        self, name: str, access_flags: int, signature: str
+    ) -> "AnnotationVisitor":
         """Prepares to visit an internal annotation.
 
         :param name: the annotation value name
         :type name: str
         :param access_flags: the annotations access flags (zero on most cases)
         :type access_flags: int
         :param signature: the class signature
@@ -107,15 +112,15 @@
         if self.delegate:
             self.delegate.visit_enum(name, owner, const, value_type)
 
 
 class MethodVisitor(VisitorBase):
     """Base class for method visitors."""
 
-    def __init__(self, delegate: 'MethodVisitor' = None) -> None:
+    def __init__(self, delegate: "MethodVisitor" = None) -> None:
         super().__init__(delegate)
 
     def visit_catch(self, exc_name: str, blocks: tuple) -> None:
         """Called on a ``.catch`` statement.
 
         The blocks contain the two enclosing goto blocks and the returning
         definition:
@@ -284,15 +289,17 @@
         :type length: str
         :param value_list: the array's values
         :type value_list: list
         """
         if self.delegate:
             self.delegate.visit_array_data(length, value_list)
 
-    def visit_local(self, register: str, name: str, descriptor: str, full_descriptor: str) -> None:
+    def visit_local(
+        self, register: str, name: str, descriptor: str, full_descriptor: str
+    ) -> None:
         """Handles debug information packed into .local statements.
 
         :param register: the variable register
         :type register: str
         :param name: the variable name
         :type name: str
         :param descriptor: the type descriptor
@@ -376,48 +383,53 @@
 
         :param interface: the class name (internal name)
         :type interface: str
         """
         if self.delegate:
             self.delegate.visit_implements(interface)
 
-    def visit_field(self, name: str, access_flags: int, field_type: str, value=None) -> FieldVisitor:
+    def visit_field(
+        self, name: str, access_flags: int, field_type: str, value=None
+    ) -> FieldVisitor:
         """Called when a global field definition has been parsed.
 
         :param name: the field's name
         :type name: str
         :param access_flags: the access flags like PUBLIC, FINAL, ...
         :type access_flags: str
         :param field_type: the field's type (can be primitive)
         :type field_type: str
         :param value: the field's   value
         :type value: _type_
         """
         if self.delegate:
             return self.delegate.visit_field(name, access_flags, field_type, value)
 
-    def visit_method(self, name: str, access_flags: int, parameters: list,
-                     return_type: str) -> MethodVisitor:
+    def visit_method(
+        self, name: str, access_flags: int, parameters: list, return_type: str
+    ) -> MethodVisitor:
         """Called when a method definition has been parsed.
 
         :param name: the method's name
         :type name: str
         :param access_flags: the access flags (PUBLIC, PRIVATE, ...)
         :type access_flags: int
         :param parameters: the parameter list (internal names)
         :type parameters: list
         :param return_type: the return type (internal name)
         :type return_type: str
         :return: a MethodVisitor that handles method parsing events
         :rtype: MethodVisitor
         """
         if self.delegate:
-            return self.delegate.visit_method(name, access_flags, parameters, return_type)
+            return self.delegate.visit_method(
+                name, access_flags, parameters, return_type
+            )
 
-    def visit_inner_class(self, name: str, access_flags: int) -> 'ClassVisitor':
+    def visit_inner_class(self, name: str, access_flags: int) -> "ClassVisitor":
         """Called when the class definition has been parsed.
 
         :param name: the class name (type descriptor, e.g. "Lcom/example/A;")
         :type name: str
         :param access_flags: different access flags (PUBLIC, FINAL, ...)
         :type access_flags: int
         """
```

### Comparing `pysmali-0.1.1/smali/writer.py` & `pysmali-0.1.2/smali/writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,36 +14,26 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 __doc__ = """
 Contains standard implementations for Smali writers that are able
 to procude classes, method, fields and annotations.
 """
 
-from smali.visitor import (
-    ClassVisitor,
-    MethodVisitor,
-    FieldVisitor,
-    AnnotationVisitor
-)
-from smali.base import (
-    AccessType,
-    Token
-)
+from smali.visitor import ClassVisitor, MethodVisitor, FieldVisitor, AnnotationVisitor
+from smali.base import AccessType, Token
 from smali.reader import SupportsCopy, SmaliReader
 from smali import opcode
 
-__all__ = [
-    'SmaliWriter', 'FieldWriter', 'MethodWriter', 'AnnotationWriter'
-]
+__all__ = ["SmaliWriter", "FieldWriter", "MethodWriter", "AnnotationWriter"]
 
 
 class _ContainsCodeCache(SupportsCopy):
     """Interface to make sure the code cache is returned via a method."""
 
-    def get_cache(self) -> '_CodeCache':
+    def get_cache(self) -> "_CodeCache":
         """Returns the current code cache.
 
         :return: the code cache
         :rtype: _CodeCache
         """
 
     def copy(self, line: str, context: type = ClassVisitor) -> None:
@@ -57,14 +47,15 @@
 
             elif isinstance(last_writer, SupportsCopy):
                 last_writer.copy(line, context)
 
             elif isinstance(last_writer, context):
                 last_writer.get_cache().add(line)
 
+
 class _CodeCache:
     """Simple container class for a code cache.
 
     :param indent: the indentation level of this code, defaults to 0
     :type indent: int, optional
     """
 
@@ -81,29 +72,32 @@
         """Returns the indentation level
 
         :return: the indent amount
         :rtype: int
         """
         return self.__indent
 
-    def add(self, line: str, start: str = "", end: str = "",
-            custom_indent: int = -1) -> None:
+    def add(
+        self, line: str, start: str = "", end: str = "", custom_indent: int = -1
+    ) -> None:
         """Appends the given line of code at the end of this cache.
 
         :param line: the line to add
         :type line: str
         :param start: additional prefix, defaults to ""
         :type start: str, optional
         :param end: additional suffix, defaults to ""
         :type end: str, optional
         """
-        indent = self.default_indent * (self.indent if custom_indent == -1 else custom_indent)
+        indent = self.default_indent * (
+            self.indent if custom_indent == -1 else custom_indent
+        )
         self.__code.append(start + indent + line + end)
 
-    def add_to_cache(self, cache: '_ContainsCodeCache') -> None:
+    def add_to_cache(self, cache: "_ContainsCodeCache") -> None:
         """Appends the given code cache to the end of this cache.
 
         :param cache: the cache to append
         :type cache: _CodeCache
         """
         if cache:
             self.__cache.append(cache)
@@ -111,18 +105,18 @@
     def add_comment(self, comment: str) -> None:
         """Adds the given comment to the last line
 
         :param comment: the comment to add
         :type comment: str
         """
         line = self.__code[-1]
-        new_line = line[:-1] if line[-1] == '\n' else str(line)
+        new_line = line[:-1] if line[-1] == "\n" else str(line)
         new_line += f" # {comment}"
-        if line[-1] == '\n':
-            new_line += '\n'
+        if line[-1] == "\n":
+            new_line += "\n"
         self.__code[-1] = new_line
 
     def pop_comments(self) -> list:
         """Clears the comment cache and returns all elements.
 
         :return: the comments that have been stored.
         :rtype: list
@@ -137,15 +131,19 @@
         The stored caches will be cleared and removed afterwards.
 
         :param clear_caches: whether sub-caches should be applied, defaults to False
         :type clear_caches: bool, optional
         """
         for element in self.__cache:
             cache = element.get_cache()
-            end = '\n' if isinstance(element, (_SmaliFieldWriter, _SmaliMethodWriter)) else ""
+            end = (
+                "\n"
+                if isinstance(element, (_SmaliFieldWriter, _SmaliMethodWriter))
+                else ""
+            )
             if cache:
                 self.add(cache.get_code(clear_cache=clear_caches), end=end)
                 cache.clear()
         self.__cache.clear()
 
     def get_code(self, clear_cache=False) -> str:
         """Returns the Smali-Code
@@ -153,15 +151,15 @@
         :param clear_cache: whether cached objects should be applied first, defaults to False
         :type clear_cache: bool, optional
         :return: the source code as utf-8 string
         :rtype: str
         """
         if clear_cache:
             self.apply_code_cache(True)
-        return '\n'.join(self.__code)
+        return "\n".join(self.__code)
 
     def clear(self) -> None:
         """Clears this cache."""
         self.__cache.clear()
         self.__comment_cache.clear()
         self.__code.clear()
 
@@ -170,62 +168,75 @@
 
         :return: the last element that contains itself a ``_CodeCache``
         :rtype: _ContainsCodeCache
         """
         if len(self.__cache) > 0:
             return self.__cache[-1]
 
+
 ##########################################################################################
 # ANNOTATION IMPLEMENTATION
 ##########################################################################################
 class _SmaliAnnotationWriter(AnnotationVisitor, _ContainsCodeCache):
     cache: _CodeCache
 
-    def __init__(self, delegate: 'AnnotationVisitor' = None, indent=0,
-                 name=Token.ANNOTATION) -> None:
+    def __init__(
+        self, delegate: "AnnotationVisitor" = None, indent=0, name=Token.ANNOTATION
+    ) -> None:
         super().__init__(delegate)
         self.cache = _CodeCache(indent)
         self._name = name
 
-    def get_cache(self) -> '_CodeCache':
+    def get_cache(self) -> "_CodeCache":
         return self.cache
 
     def visit_value(self, name: str, value) -> None:
         super().visit_value(name, value)
         indent = self.cache.indent + 1
         self.cache.add(f"{name} = {value}", custom_indent=indent)
 
     def visit_enum(self, name: str, owner: str, const: str, value_type: str) -> None:
         super().visit_enum(name, owner, const, value_type)
         indent = self.cache.indent + 1
-        self.cache.add(f"{name} = .{Token.ENUM} {owner}->{const}:{value_type}",
-                       custom_indent=indent)
+        self.cache.add(
+            f"{name} = .{Token.ENUM} {owner}->{const}:{value_type}",
+            custom_indent=indent,
+        )
 
-    def visit_subannotation(self, name: str, access_flags: int,
-                            signature: str) -> 'AnnotationVisitor':
+    def visit_subannotation(
+        self, name: str, access_flags: int, signature: str
+    ) -> "AnnotationVisitor":
         delegate = super().visit_subannotation(name, access_flags, signature)
         desc = f"{name} = .{Token.SUBANNOTATION} {signature}"
-        a_visitor = _SmaliAnnotationWriter(delegate, self.cache.indent+1, Token.SUBANNOTATION)
+        a_visitor = _SmaliAnnotationWriter(
+            delegate, self.cache.indent + 1, Token.SUBANNOTATION
+        )
 
         a_visitor.cache.add(desc)
         self.cache.add_to_cache(a_visitor)
         return a_visitor
 
     def visit_array(self, name: str, values: list) -> None:
         indent_value = self.cache.default_indent
         indent = self.cache.indent
 
         if len(values) == 0:
-            self.cache.add("%s = {}" % name, custom_indent=indent+1) # noqa
+            self.cache.add("%s = {}" % name, custom_indent=indent + 1)  # noqa
         else:
-            sep_value = ',\n' + indent_value*(indent+2)
-            self.cache.add("%s = {\n%s%s\n%s}" % (
-                name, indent_value*(indent+2),
-                sep_value.join(values), indent_value*(indent+1)
-            ), custom_indent=indent+1)
+            sep_value = ",\n" + indent_value * (indent + 2)
+            self.cache.add(
+                "%s = {\n%s%s\n%s}"
+                % (
+                    name,
+                    indent_value * (indent + 2),
+                    sep_value.join(values),
+                    indent_value * (indent + 1),
+                ),
+                custom_indent=indent + 1,
+            )
         return super().visit_array(name, values)
 
     def visit_comment(self, text: str) -> None:
         super().visit_comment(text)
         self.cache.add(f"# {text}")
 
     def visit_eol_comment(self, text: str) -> None:
@@ -240,28 +251,28 @@
 
 ##########################################################################################
 # FIELD IMPLEMENTATION
 ##########################################################################################
 class _SmaliFieldWriter(FieldVisitor, _ContainsCodeCache):
     cache: _CodeCache
 
-    def __init__(self, delegate: 'FieldVisitor' = None, indent=0) -> None:
+    def __init__(self, delegate: "FieldVisitor" = None, indent=0) -> None:
         super().__init__(delegate)
         self.cache = _CodeCache(indent)
 
     def visit_annotation(self, access_flags: int, signature: str) -> AnnotationVisitor:
         delegate = super().visit_annotation(access_flags, signature)
         desc = f".{Token.ANNOTATION} {' '.join(AccessType.get_names(access_flags))} {signature}"
-        a_visitor = _SmaliAnnotationWriter(delegate, self.cache.indent+1)
+        a_visitor = _SmaliAnnotationWriter(delegate, self.cache.indent + 1)
 
         a_visitor.cache.add(desc)
         self.cache.add_to_cache(a_visitor)
         return a_visitor
 
-    def get_cache(self) -> '_CodeCache':
+    def get_cache(self) -> "_CodeCache":
         return self.cache
 
     def visit_comment(self, text: str) -> None:
         super().visit_comment(text)
         self.cache.add(f"# {text}")
 
     def visit_eol_comment(self, text: str) -> None:
@@ -269,157 +280,185 @@
         self.cache.add_comment(text)
 
     def visit_end(self) -> None:
         super().visit_end()
         self.cache.apply_code_cache(True)
         self.cache.add(f".{Token.END} {Token.FIELD}")
 
+
 ##########################################################################################
 # METHOD IMPLEMENTATION
 ##########################################################################################
 class _SmaliMethodWriter(MethodVisitor, _ContainsCodeCache):
     cache: _CodeCache
 
-    def __init__(self, delegate: 'MethodVisitor' = None, indent=0) -> None:
+    def __init__(self, delegate: "MethodVisitor" = None, indent=0) -> None:
         super().__init__(delegate)
         self.cache = _CodeCache(indent)
 
     def visit_annotation(self, access_flags: int, signature: str) -> AnnotationVisitor:
         delegate = super().visit_annotation(access_flags, signature)
         desc = f".{Token.ANNOTATION} {' '.join(AccessType.get_names(access_flags))} {signature}"
-        a_visitor = _SmaliAnnotationWriter(delegate, self.cache.indent+1)
+        a_visitor = _SmaliAnnotationWriter(delegate, self.cache.indent + 1)
 
         a_visitor.cache.add(desc)
         self.cache.add_to_cache(a_visitor)
         return a_visitor
 
     def visit_block(self, name: str) -> None:
         self.cache.apply_code_cache(True)
         super().visit_block(name)
-        self.cache.add(f":{name}", custom_indent=self.cache.indent+1)
+        self.cache.add(f":{name}", custom_indent=self.cache.indent + 1)
 
     def visit_line(self, number: int) -> None:
         self.cache.apply_code_cache(True)
         super().visit_line(number)
-        self.cache.add(f".{Token.LINE} {number}", custom_indent=self.cache.indent+1)
+        self.cache.add(f".{Token.LINE} {number}", custom_indent=self.cache.indent + 1)
 
     def visit_goto(self, block_name: str) -> None:
         self.cache.apply_code_cache(True)
         super().visit_goto(block_name)
-        self.cache.add(f"{opcode.GOTO} :{block_name}", custom_indent=self.cache.indent+1)
+        self.cache.add(
+            f"{opcode.GOTO} :{block_name}", custom_indent=self.cache.indent + 1
+        )
 
     def visit_instruction(self, ins_name: str, args: list) -> None:
         self.cache.apply_code_cache(True)
         super().visit_instruction(ins_name, args)
         self.cache.add(
-            f"{ins_name} {', '.join(args)}", custom_indent=self.cache.indent+1, end='\n'
+            f"{ins_name} {', '.join(args)}",
+            custom_indent=self.cache.indent + 1,
+            end="\n",
         )
 
     def visit_param(self, register: str, name: str) -> None:
         self.cache.apply_code_cache(True)
         super().visit_param(register, name)
-        self.cache.add(f'.{Token.PARAM} {register} "{name}"', custom_indent=self.cache.indent+1)
+        self.cache.add(
+            f'.{Token.PARAM} {register} "{name}"', custom_indent=self.cache.indent + 1
+        )
 
     def visit_comment(self, text: str) -> None:
         super().visit_comment(text)
-        self.cache.add(f"# {text}", custom_indent=self.cache.indent+1)
+        self.cache.add(f"# {text}", custom_indent=self.cache.indent + 1)
 
     def visit_restart(self, register: str) -> None:
         self.cache.apply_code_cache(True)
         super().visit_restart(register)
-        self.cache.add(f".{Token.RESTART} {register}", custom_indent=self.cache.indent+1)
+        self.cache.add(
+            f".{Token.RESTART} {register}", custom_indent=self.cache.indent + 1
+        )
 
     def visit_locals(self, local_count: int) -> None:
         self.cache.apply_code_cache(True)
         super().visit_locals(local_count)
-        self.cache.add(f".{Token.LOCALS} {local_count}", custom_indent=self.cache.indent+1)
+        self.cache.add(
+            f".{Token.LOCALS} {local_count}", custom_indent=self.cache.indent + 1
+        )
 
-    def visit_local(self, register: str, name: str, descriptor: str, full_descriptor: str) -> None:
+    def visit_local(
+        self, register: str, name: str, descriptor: str, full_descriptor: str
+    ) -> None:
         self.cache.apply_code_cache(True)
         super().visit_local(register, name, descriptor, full_descriptor)
-        self.cache.add(f'.{Token.LOCAL} {register}, "{name}":{descriptor}, "{full_descriptor}"',
-                       custom_indent=self.cache.indent+1)
+        self.cache.add(
+            f'.{Token.LOCAL} {register}, "{name}":{descriptor}, "{full_descriptor}"',
+            custom_indent=self.cache.indent + 1,
+        )
 
     def visit_prologue(self) -> None:
         self.cache.apply_code_cache(True)
         super().visit_prologue()
-        self.cache.add(f".{Token.PROLOGUE}", custom_indent=self.cache.indent+1)
+        self.cache.add(f".{Token.PROLOGUE}", custom_indent=self.cache.indent + 1)
 
     def visit_catch(self, exc_name: str, blocks: tuple) -> None:
         self.cache.apply_code_cache(True)
         super().visit_catch(exc_name, blocks)
         start, end, catch = blocks
-        self.cache.add(".%s %s { :%s .. :%s } :%s" % (
-            Token.CATCH, exc_name, start, end, catch
-        ), custom_indent=self.cache.indent+1)
+        self.cache.add(
+            ".%s %s { :%s .. :%s } :%s" % (Token.CATCH, exc_name, start, end, catch),
+            custom_indent=self.cache.indent + 1,
+        )
 
     def visit_catchall(self, exc_name: str, blocks: tuple) -> None:
         self.cache.apply_code_cache(True)
         super().visit_catchall(exc_name, blocks)
         start, end, catch = blocks
-        self.cache.add(".%s %s { :%s .. :%s } :%s" % (
-            Token.CATCHALL, exc_name, start, end, catch
-        ), custom_indent=self.cache.indent+1, end='\n')
+        self.cache.add(
+            ".%s %s { :%s .. :%s } :%s" % (Token.CATCHALL, exc_name, start, end, catch),
+            custom_indent=self.cache.indent + 1,
+            end="\n",
+        )
 
     def visit_registers(self, registers: int) -> None:
         self.cache.apply_code_cache(True)
         super().visit_registers(registers)
-        self.cache.add(f".{Token.REGISTERS} {registers}", custom_indent=self.cache.indent+1,
-                       end='\n')
+        self.cache.add(
+            f".{Token.REGISTERS} {registers}",
+            custom_indent=self.cache.indent + 1,
+            end="\n",
+        )
 
     def visit_return(self, ret_type: str, args: list) -> None:
         self.cache.apply_code_cache(True)
         super().visit_return(ret_type, args)
         if ret_type:
             ret_type = f"-{ret_type}"
 
-        self.cache.add(f"return{ret_type} {' '.join(args)}",
-                       custom_indent=self.cache.indent+1)
+        self.cache.add(
+            f"return{ret_type} {' '.join(args)}", custom_indent=self.cache.indent + 1
+        )
 
     def visit_invoke(self, inv_type: str, args: list, owner: str, method: str) -> None:
         self.cache.apply_code_cache(True)
         super().visit_invoke(inv_type, args, owner, method)
-        self.cache.add("invoke-%s { %s }, %s->%s" % (
-            inv_type, ', '.join(args), owner, method
-        ), custom_indent=self.cache.indent+1, end='\n')
+        self.cache.add(
+            "invoke-%s { %s }, %s->%s" % (inv_type, ", ".join(args), owner, method),
+            custom_indent=self.cache.indent + 1,
+            end="\n",
+        )
 
     def visit_array_data(self, length: str, value_list: list) -> None:
         self.cache.apply_code_cache(True)
         super().visit_array_data(length, value_list)
-        indent_value = self.cache.default_indent * (self.cache.indent+2)
-        sep_value = '\n' + indent_value
-        self.cache.add(f".{Token.ARRAYDATA} {length}\n{indent_value}{sep_value.join(value_list)}",
-                       end='\n')
+        indent_value = self.cache.default_indent * (self.cache.indent + 2)
+        sep_value = "\n" + indent_value
+        self.cache.add(
+            f".{Token.ARRAYDATA} {length}\n{indent_value}{sep_value.join(value_list)}",
+            end="\n",
+        )
 
     def visit_packed_switch(self, value: str, blocks: list) -> None:
         self.cache.apply_code_cache(True)
         super().visit_packed_switch(value, blocks)
-        indent_value = self.cache.default_indent * (self.cache.indent+2)
-        sep_value = '\n' + indent_value + ':'
-        self.cache.add(f".{Token.PACKEDSWITCH} {value}\n{indent_value}{sep_value.join(blocks)}",
-                       end='\n')
+        indent_value = self.cache.default_indent * (self.cache.indent + 2)
+        sep_value = "\n" + indent_value + ":"
+        self.cache.add(
+            f".{Token.PACKEDSWITCH} {value}\n{indent_value}{sep_value.join(blocks)}",
+            end="\n",
+        )
 
     def visit_sparse_switch(self, branches: dict) -> None:
         self.cache.apply_code_cache(True)
         super().visit_sparse_switch(branches)
-        indent_value = self.cache.default_indent * (self.cache.indent+2)
-        values = [f"{x} -> :{y}" for x,y in branches.items()]
-        sep_value = '\n' + indent_value
+        indent_value = self.cache.default_indent * (self.cache.indent + 2)
+        values = [f"{x} -> :{y}" for x, y in branches.items()]
+        sep_value = "\n" + indent_value
         self.cache.add(f".{Token.SPARSESWITCH}\n{indent_value}{sep_value.join(values)}")
 
     def visit_eol_comment(self, text: str) -> None:
         super().visit_eol_comment(text)
         self.cache.add_comment(text)
 
     def visit_end(self) -> None:
         self.cache.apply_code_cache(True)
         super().visit_end()
         self.cache.add(f".{Token.END} {Token.METHOD}")
 
-    def get_cache(self) -> '_CodeCache':
+    def get_cache(self) -> "_CodeCache":
         return self.cache
 
 
 ##########################################################################################
 # CLASS IMPLEMENTATION
 ##########################################################################################
 class _SmaliClassWriter(ClassVisitor, _ContainsCodeCache):
@@ -430,14 +469,17 @@
 
     def __init__(self, reader: SmaliReader = None, indent=0) -> None:
         super().__init__()
         self.cache = _CodeCache(indent)
         if reader:
             reader.copy_handler = self
 
+    def __str__(self) -> str:
+        return self.code
+
     @property
     def code(self) -> str:
         """Returns the source code as an utf-8 string
 
         :return: the complete source code
         :rtype: str
         """
@@ -447,53 +489,55 @@
         """Resets the writer.
 
         Use this method before calling #visit() to ensure the internal
         buffer is cleared.
         """
         self.cache.clear()
 
-    def get_cache(self) -> '_CodeCache':
+    def get_cache(self) -> "_CodeCache":
         return self.cache
 
     ######################################################################################
     # INTERNAL
     ######################################################################################
     def visit_class(self, name: str, access_flags: int) -> None:
         super().visit_class(name, access_flags)
-        flags = ' '.join(AccessType.get_names(access_flags))
+        flags = " ".join(AccessType.get_names(access_flags))
         self.cache.add(f".{Token.CLASS} {flags} {name}")
 
     def visit_super(self, super_class: str) -> None:
         super().visit_super(super_class)
         self.cache.add(f".{Token.SUPER} {super_class}\n")
 
     def visit_implements(self, interface: str) -> None:
         super().visit_implements(interface)
         self.cache.add(f".{Token.IMPLEMENTS} {interface}")
 
     def visit_source(self, source: str) -> None:
         super().visit_source(source)
         self.cache.add(f'.{Token.SOURCE} "{source}"\n')
 
-    def visit_field(self, name: str, access_flags: int, field_type: str, value=None) -> FieldVisitor:
+    def visit_field(
+        self, name: str, access_flags: int, field_type: str, value=None
+    ) -> FieldVisitor:
         delegate = super().visit_field(name, access_flags, field_type, value)
-        flags = ' '.join(AccessType.get_names(access_flags))
+        flags = " ".join(AccessType.get_names(access_flags))
         desc = f".{Token.FIELD} {flags} {name}:{field_type}"
         if value:
             # String values come with their '"' characters
             desc = f"{desc} = {value}"
 
         f_visitor = _SmaliFieldWriter(delegate, self.cache.indent)
         f_visitor.cache.add(desc)
         self.cache.add_to_cache(f_visitor)
         return f_visitor
 
     def visit_annotation(self, access_flags: int, signature: str) -> AnnotationVisitor:
         delegate = super().visit_annotation(access_flags, signature)
-        flags = ' '.join(AccessType.get_names(access_flags))
+        flags = " ".join(AccessType.get_names(access_flags))
         desc = f".{Token.ANNOTATION} {flags} {signature}"
         a_visitor = _SmaliAnnotationWriter(delegate, self.cache.indent)
 
         a_visitor.cache.add(desc)
         self.cache.add_to_cache(a_visitor)
         return a_visitor
 
@@ -503,30 +547,31 @@
         desc = f".{Token.CLASS} {flags} {name}"
 
         c_visitor = _SmaliClassWriter(delegate)
         c_visitor.cache.add(desc)
         self.cache.add_to_cache(c_visitor)
         return c_visitor
 
-    def visit_method(self, name: str, access_flags: int, parameters: list,
-                     return_type: str) -> MethodVisitor:
+    def visit_method(
+        self, name: str, access_flags: int, parameters: list, return_type: str
+    ) -> MethodVisitor:
         delegate = super().visit_method(name, access_flags, parameters, return_type)
-        flags = ' '.join(AccessType.get_names(access_flags))
-        params = ''.join(parameters)
+        flags = " ".join(AccessType.get_names(access_flags))
+        params = "".join(parameters)
         desc = f".{Token.METHOD} {flags} {name}({params}){return_type}"
 
         m_visitor = _SmaliMethodWriter(delegate, self.cache.indent)
         m_visitor.cache.add(desc)
         self.cache.add_to_cache(m_visitor)
         return m_visitor
 
     def visit_comment(self, text: str) -> None:
         self.cache.apply_code_cache(True)
         super().visit_comment(text)
-        self.cache.add(f'# {text}')
+        self.cache.add(f"# {text}")
 
     def visit_eol_comment(self, text: str) -> None:
         super().visit_eol_comment(text)
         self.cache.add_comment(text)
 
     def visit_debug(self, enabled: int) -> None:
         super().visit_debug(enabled)
@@ -548,15 +593,16 @@
             elif isinstance(last_writer, SupportsCopy):
                 last_writer.copy(line, context)
 
             elif isinstance(last_writer, (context, _ContainsCodeCache)):
                 last_writer.get_cache().add(line)
 
             else:
-                print('Line excluded:', line, '<context> =', context)
+                print("Line excluded:", line, "<context> =", context)
+
 
 ##########################################################################################
 # EXPORTS
 ##########################################################################################
 SmaliWriter = _SmaliClassWriter
 FieldWriter = _SmaliFieldWriter
 MethodWriter = _SmaliMethodWriter
```

