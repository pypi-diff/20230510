# Comparing `tmp/argstart-0.0.2.tar.gz` & `tmp/argstart-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argstart-0.0.2.tar", last modified: Fri Apr 22 08:45:43 2022, max compression
+gzip compressed data, was "argstart-0.0.3.tar", last modified: Wed May 10 09:59:01 2023, max compression
```

## Comparing `argstart-0.0.2.tar` & `argstart-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-04-22 08:45:43.814023 argstart-0.0.2/
--rw-rw-rw-   0        0        0     1069 2022-04-22 08:42:27.000000 argstart-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3073 2022-04-22 08:45:43.814023 argstart-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2587 2022-04-21 14:19:10.000000 argstart-0.0.2/README.md
--rw-rw-rw-   0        0        0      110 2022-04-22 08:42:15.000000 argstart-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      623 2022-04-22 08:45:43.814023 argstart-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-04-22 08:45:43.763988 argstart-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-04-22 08:45:43.783869 argstart-0.0.2/src/argstart/
--rw-rw-rw-   0        0        0       25 2022-04-22 08:38:34.000000 argstart-0.0.2/src/argstart/__init__.py
--rw-rw-rw-   0        0        0     4429 2022-04-21 15:08:23.000000 argstart-0.0.2/src/argstart/main.py
-drwxrwxrwx   0        0        0        0 2022-04-22 08:45:43.814023 argstart-0.0.2/src/argstart.egg-info/
--rw-rw-rw-   0        0        0     3073 2022-04-22 08:45:43.000000 argstart-0.0.2/src/argstart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2022-04-22 08:45:43.000000 argstart-0.0.2/src/argstart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-22 08:45:43.000000 argstart-0.0.2/src/argstart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-04-22 08:45:43.000000 argstart-0.0.2/src/argstart.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-04-22 08:45:43.000000 argstart-0.0.2/src/argstart.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 09:59:01.764968 argstart-0.0.3/
+-rw-rw-rw-   0        0        0     1069 2022-04-22 08:42:27.000000 argstart-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3032 2023-05-10 09:59:01.764968 argstart-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2587 2022-04-21 14:19:10.000000 argstart-0.0.3/README.md
+-rw-rw-rw-   0        0        0      110 2022-04-22 08:42:15.000000 argstart-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      623 2023-05-10 09:59:01.766962 argstart-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 09:59:01.729063 argstart-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:59:01.738038 argstart-0.0.3/src/argstart/
+-rw-rw-rw-   0        0        0       25 2022-04-22 08:38:34.000000 argstart-0.0.3/src/argstart/__init__.py
+-rw-rw-rw-   0        0        0     4470 2023-05-10 09:56:48.000000 argstart-0.0.3/src/argstart/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:59:01.763970 argstart-0.0.3/src/argstart.egg-info/
+-rw-rw-rw-   0        0        0     3032 2023-05-10 09:59:01.000000 argstart-0.0.3/src/argstart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-10 09:59:01.000000 argstart-0.0.3/src/argstart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:59:01.000000 argstart-0.0.3/src/argstart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-10 09:59:01.000000 argstart-0.0.3/src/argstart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 09:59:01.000000 argstart-0.0.3/src/argstart.egg-info/top_level.txt
```

### Comparing `argstart-0.0.2/LICENSE` & `argstart-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `argstart-0.0.2/PKG-INFO` & `argstart-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: argstart
-Version: 0.0.2
+Version: 0.0.3
 Summary: Run a "main" function automatically with the function's parameters as command-line arguments
 Author: 731031
 Author-email: 731031@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -94,9 +92,7 @@
 
 Finally, booleans will by default create a `--toggle-flag` which don't require any value after:
 ```python
 def main(foo=False)
 # command-line: example.py [-f]
 # (meaning foo defaults to False when -f flag is not given)
 ```
-
-
```

### Comparing `argstart-0.0.2/README.md` & `argstart-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `argstart-0.0.2/setup.cfg` & `argstart-0.0.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7267 7374 6172 740d 0a76 6572   = argstart..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6175  sion = 0.0.2..au
+00000020: 7369 6f6e 203d 2030 2e30 2e33 0d0a 6175  sion = 0.0.3..au
 00000030: 7468 6f72 203d 2037 3331 3033 310d 0a61  thor = 731031..a
 00000040: 7574 686f 725f 656d 6169 6c20 3d20 3733  uthor_email = 73
 00000050: 3130 3331 4067 6d61 696c 2e63 6f6d 0d0a  1031@gmail.com..
 00000060: 6465 7363 7269 7074 696f 6e20 3d20 5275  description = Ru
 00000070: 6e20 6120 226d 6169 6e22 2066 756e 6374  n a "main" funct
 00000080: 696f 6e20 6175 746f 6d61 7469 6361 6c6c  ion automaticall
 00000090: 7920 7769 7468 2074 6865 2066 756e 6374  y with the funct
```

### Comparing `argstart-0.0.2/src/argstart/main.py` & `argstart-0.0.3/src/argstart/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,116 @@
-import os
-import atexit
-import inspect
-import argparse
-import docstring_parser
-
-
-def start(func):
-    """"Decorator to make a main function that accepts command-line arguments"""
-    # Check that the caller is being ran as script
-    caller_name = inspect.stack()[1].frame.f_locals["__name__"]
-    if caller_name == "__main__":
-        # Run the function when the script would otherwise finish, so that a 'def main()' at the top
-        # can call functions below, like having 'if __name__ == "__main__"' at bottom allows
-        atexit.register(lambda: _run(func))
-
-    # Return the function so that it can still be called manually
-    return func
-
-
-def _run(func):
-    try:
-        # Parse arguments based on function signature
-        parser, positional_only = _construct_parser(func)
-        all_arguments = vars(parser.parse_args()).items()
-
-        # Run function with those arguments
-        args = [value for name, value in all_arguments if name in positional_only]
-        kwargs = {name: value for name, value in all_arguments if name not in positional_only}
-        func(*args, **kwargs)
-    except SystemExit as e:
-        # Escalate normal sys.exit (which doesn't work in atexit functions)
-        os._exit(e.code)
-
-
-def _construct_parser(func):
-    # Get function signature and docstring
-    signature = inspect.signature(func)
-    signature_params = signature.parameters.items()
-
-    docstring = docstring_parser.parse(func.__doc__)
-    docstring_params = docstring.params
-
-    parser = argparse.ArgumentParser(description=docstring.short_description,
-                                     epilog=docstring.long_description)
-
-    # Cycle through params, adding to arg parser
-    positional_only = []
-    for name, value in signature_params:
-        # Find param description from docstring
-        docstring_param = [param for param in docstring_params if param.arg_name == name]
-        description = docstring_param[0].description if len(docstring_param) > 0 else ""
-        name = value.name.replace("_", "-")
-
-        # Construct argument parser add_argument arguments (arg!)
-        arg_args = {"help": description}
-        if value.annotation != inspect._empty:
-            arg_args["type"] = value.annotation
-
-        kind = inspect._PARAM_NAME_MAPPING[value.kind]
-
-        # Keep track of positional-only, since they can't be passed in to function as dict
-        if kind == "positional-only":
-            positional_only.append(name)
-
-        # Variadic arguments (*args, **kwargs)
-        if kind == "variadic positional":
-            parser.add_argument(name, **arg_args, nargs="*")
-
-        elif kind == "variadic keyword":
-            parser.add_argument("-" + _acronym(name), "--" + name, **arg_args, nargs="*")
-
-        # Has no default value: Create positional argument unless it's keyword-only
-        elif value.default == inspect._empty:
-            if kind == "keyword-only":
-                parser.add_argument("-" + _acronym(name), "--" + name, **arg_args, required=True)
-            else:
-                parser.add_argument(name, **arg_args)
-
-        # Bool: Create --toggle-flag requiring no value specified after
-        elif kind == "positional or keyword" and type(value.default) == bool:
-            parser.add_argument("-" + _acronym(name), "--" + name, **arg_args,
-                                action="store_false" if value.default else "store_true")
-
-        # Has default value: Create --flag argument unless it's positional-only
-        else:
-            arg_args["default"] = value.default
-            arg_args["type"] = type(value.default)
-            if kind == "positional-only":
-                parser.add_argument(name, **arg_args, nargs="?")
-            else:
-                parser.add_argument("-" + _acronym(name), "--" + name, **arg_args)
-
-    return parser, positional_only
-
-
-def _acronym(name, already_used_cache=[]):
-    acronym = name[0]
-    prev_letter = None
-    for letter in name:
-        if letter.isupper() or prev_letter == "-":
-            acronym += letter.lower()
-        prev_letter = letter
-
-    # Append number if acronym conflicts
-    acronym_safe = acronym
-    i = 1
-    while acronym_safe in already_used_cache:
-        i += 1
-        acronym_safe = f"{acronym}{i}"
-
-    already_used_cache.append(acronym_safe)
-    return acronym_safe
+import os
+import atexit
+import inspect
+import argparse
+import docstring_parser
+
+
+def start(func):
+    """"Decorator to make a main function that accepts command-line arguments"""
+    # Check that the caller is being ran as script
+    caller_name = inspect.stack()[1].frame.f_locals["__name__"]
+    if caller_name == "__main__":
+        # Run the function when the script would otherwise finish, so that a 'def main()' at the top
+        # can call functions below, like having 'if __name__ == "__main__"' at bottom allows
+        atexit.register(lambda: _run(func))
+
+    # Return the function so that it can still be called manually
+    return func
+
+
+def _run(func):
+    try:
+        # Parse arguments based on function signature
+        parser, positional_only = _construct_parser(func)
+        all_arguments = vars(parser.parse_args()).items()
+
+        # Run function with those arguments
+        args = [value for name, value in all_arguments if name in positional_only]
+        kwargs = {name: value for name, value in all_arguments if name not in positional_only}
+        func(*args, **kwargs)
+    except SystemExit as e:
+        # Escalate normal sys.exit (which doesn't work in atexit functions)
+        os._exit(e.code)
+
+
+def _construct_parser(func):
+    # Get function signature and docstring
+    signature = inspect.signature(func)
+    signature_params = signature.parameters.items()
+
+    docstring = docstring_parser.parse(func.__doc__)
+    docstring_params = docstring.params
+
+    parser = argparse.ArgumentParser(description=docstring.short_description,
+                                     epilog=docstring.long_description)
+
+    # Cycle through params, adding to arg parser
+    positional_only = []
+    for name, value in signature_params:
+        # Find param description from docstring
+        docstring_param = [param for param in docstring_params if param.arg_name == name]
+        description = docstring_param[0].description if len(docstring_param) > 0 else ""
+        name = value.name.replace("_", "-")
+
+        # Construct argument parser add_argument arguments (arg!)
+        arg_args = {"help": description}
+        if value.annotation != inspect._empty:
+            arg_args["type"] = value.annotation
+
+        try:
+            kind = inspect._PARAM_NAME_MAPPING[value.kind]  # Works on old python versions
+        except AttributeError:
+            kind = value.kind.description  # Works on new python versions
+
+        # Keep track of positional-only, since they can't be passed in to function as dict
+        if kind == "positional-only":
+            positional_only.append(name)
+
+        # Variadic arguments (*args, **kwargs)
+        if kind == "variadic positional":
+            parser.add_argument(name, **arg_args, nargs="*")
+
+        elif kind == "variadic keyword":
+            parser.add_argument("-" + _acronym(name), "--" + name, **arg_args, nargs="*")
+
+        # Has no default value: Create positional argument unless it's keyword-only
+        elif value.default == inspect._empty:
+            if kind == "keyword-only":
+                parser.add_argument("-" + _acronym(name), "--" + name, **arg_args, required=True)
+            else:
+                parser.add_argument(name, **arg_args)
+
+        # Bool: Create --toggle-flag requiring no value specified after
+        elif kind == "positional or keyword" and type(value.default) == bool:
+            parser.add_argument("-" + _acronym(name), "--" + name, **arg_args,
+                                action="store_false" if value.default else "store_true")
+
+        # Has default value: Create --flag argument unless it's positional-only
+        else:
+            arg_args["default"] = value.default
+            arg_args["type"] = type(value.default)
+            if kind == "positional-only":
+                parser.add_argument(name, **arg_args, nargs="?")
+            else:
+                parser.add_argument("-" + _acronym(name), "--" + name, **arg_args)
+
+    return parser, positional_only
+
+
+def _acronym(name, already_used_cache=[]):
+    acronym = name[0]
+    prev_letter = None
+    for letter in name:
+        if letter.isupper() or prev_letter == "-":
+            acronym += letter.lower()
+        prev_letter = letter
+
+    # Append number if acronym conflicts
+    acronym_safe = acronym
+    i = 1
+    while acronym_safe in already_used_cache:
+        i += 1
+        acronym_safe = f"{acronym}{i}"
+
+    already_used_cache.append(acronym_safe)
+    return acronym_safe
```

### Comparing `argstart-0.0.2/src/argstart.egg-info/PKG-INFO` & `argstart-0.0.3/src/argstart.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: argstart
-Version: 0.0.2
+Version: 0.0.3
 Summary: Run a "main" function automatically with the function's parameters as command-line arguments
 Author: 731031
 Author-email: 731031@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -94,9 +92,7 @@
 
 Finally, booleans will by default create a `--toggle-flag` which don't require any value after:
 ```python
 def main(foo=False)
 # command-line: example.py [-f]
 # (meaning foo defaults to False when -f flag is not given)
 ```
-
-
```

