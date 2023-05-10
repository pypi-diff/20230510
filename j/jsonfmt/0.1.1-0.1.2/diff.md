# Comparing `tmp/jsonfmt-0.1.1.tar.gz` & `tmp/jsonfmt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonfmt-0.1.1.tar", last modified: Thu Apr 27 13:14:26 2023, max compression
+gzip compressed data, was "jsonfmt-0.1.2.tar", last modified: Wed May 10 03:03:14 2023, max compression
```

## Comparing `jsonfmt-0.1.1.tar` & `jsonfmt-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 xu         (501) staff       (20)        0 2023-04-27 13:14:26.297214 jsonfmt-0.1.1/
--rw-r--r--   0 xu         (501) staff       (20)     1064 2023-04-27 13:04:25.000000 jsonfmt-0.1.1/LICENSE
--rw-r--r--   0 xu         (501) staff       (20)     4089 2023-04-27 13:14:26.297379 jsonfmt-0.1.1/PKG-INFO
--rw-r--r--   0 xu         (501) staff       (20)     3560 2023-04-27 13:04:25.000000 jsonfmt-0.1.1/README.md
-drwxr-xr-x   0 xu         (501) staff       (20)        0 2023-04-27 13:14:26.296862 jsonfmt-0.1.1/jsonfmt.egg-info/
--rw-r--r--   0 xu         (501) staff       (20)     4089 2023-04-27 13:14:26.000000 jsonfmt-0.1.1/jsonfmt.egg-info/PKG-INFO
--rw-r--r--   0 xu         (501) staff       (20)      205 2023-04-27 13:14:26.000000 jsonfmt-0.1.1/jsonfmt.egg-info/SOURCES.txt
--rw-r--r--   0 xu         (501) staff       (20)        1 2023-04-27 13:14:26.000000 jsonfmt-0.1.1/jsonfmt.egg-info/dependency_links.txt
--rw-r--r--   0 xu         (501) staff       (20)       41 2023-04-27 13:14:26.000000 jsonfmt-0.1.1/jsonfmt.egg-info/entry_points.txt
--rw-r--r--   0 xu         (501) staff       (20)        8 2023-04-27 13:14:26.000000 jsonfmt-0.1.1/jsonfmt.egg-info/top_level.txt
--rwxr-xr-x   0 xu         (501) staff       (20)     4288 2023-04-27 13:08:59.000000 jsonfmt-0.1.1/jsonfmt.py
--rw-r--r--   0 xu         (501) staff       (20)      107 2023-04-27 13:14:26.297957 jsonfmt-0.1.1/setup.cfg
--rwxr-xr-x   0 xu         (501) staff       (20)      850 2023-04-27 13:04:25.000000 jsonfmt-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:03:14.001402 jsonfmt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 03:03:02.000000 jsonfmt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-10 03:03:14.001402 jsonfmt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-10 03:03:02.000000 jsonfmt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:03:14.001402 jsonfmt-0.1.2/jsonfmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 03:03:13.000000 jsonfmt-0.1.2/jsonfmt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4472 2023-05-10 03:03:02.000000 jsonfmt-0.1.2/jsonfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 03:03:14.001402 jsonfmt-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-05-10 03:03:02.000000 jsonfmt-0.1.2/setup.py
```

### Comparing `jsonfmt-0.1.1/LICENSE` & `jsonfmt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonfmt-0.1.1/PKG-INFO` & `jsonfmt-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JSON object formatting tool.
 Home-page: https://github.com/seamile/jsonfmt
 Author: Seamile
 Author-email: lanhuermao@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,19 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Formator
 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/jsonfmt?label=Install&color=green)
+![PyPI](https://img.shields.io/pypi/v/jsonfmt?color=9cf)
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?branch=main&label=build&logo=python)
+
+
 **jsonfmt** is a json object formatting tool.
 
 ## Features
 
 1. Print the json object in pretty format from files or stdin.
 2. Compress the json object into a single line without spaces.
 3. Output part of a large json object via jsonpath.
```

### Comparing `jsonfmt-0.1.1/README.md` & `jsonfmt-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # JSON Formator
 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/jsonfmt?label=Install&color=green)
+![PyPI](https://img.shields.io/pypi/v/jsonfmt?color=9cf)
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?branch=main&label=build&logo=python)
+
+
 **jsonfmt** is a json object formatting tool.
 
 ## Features
 
 1. Print the json object in pretty format from files or stdin.
 2. Compress the json object into a single line without spaces.
 3. Output part of a large json object via jsonpath.
```

### Comparing `jsonfmt-0.1.1/jsonfmt.egg-info/PKG-INFO` & `jsonfmt-0.1.2/jsonfmt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonfmt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JSON object formatting tool.
 Home-page: https://github.com/seamile/jsonfmt
 Author: Seamile
 Author-email: lanhuermao@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,19 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JSON Formator
 
+![PyPI - Downloads](https://img.shields.io/pypi/dm/jsonfmt?label=Install&color=green)
+![PyPI](https://img.shields.io/pypi/v/jsonfmt?color=9cf)
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/seamile/jsonfmt/python-package.yml?branch=main&label=build&logo=python)
+
+
 **jsonfmt** is a json object formatting tool.
 
 ## Features
 
 1. Print the json object in pretty format from files or stdin.
 2. Compress the json object into a single line without spaces.
 3. Output part of a large json object via jsonpath.
```

### Comparing `jsonfmt-0.1.1/jsonfmt.py` & `jsonfmt-0.1.2/jsonfmt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,56 @@
 #!/usr/bin/env python
 '''JSON Format Tool'''
 
 import json
-from sys import stdin
+from sys import stdin, stdout, stderr
 from argparse import ArgumentParser
-from typing import Any, Optional, IO
+from typing import Any, List, IO, Union
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 
 def print_err(msg: str):
-    print(f'\033[0;31m{msg}\033[0m')
+    print(f'\033[0;31m{msg}\033[0m', file=stderr)
 
 
 class JSONPathError(Exception):
     pass
 
 
-def output(json_obj: Any, output_fp: Optional[IO] = None, compression: bool = False):
+def output(json_obj: Any, compression: bool, escape: bool, indent: int,
+           output_fp: IO = stdout):
     '''output formated json to file or stdout'''
-    if output_fp is None:
-        if compression:
-            j_str = json.dumps(json_obj, ensure_ascii=False,
-                               sort_keys=True, separators=(',', ':'))
-        else:
-            j_str = json.dumps(json_obj, ensure_ascii=False,
-                               sort_keys=True, indent=4)
-        print(j_str)
-    else:
+    if output_fp.fileno() > 2:
         output_fp.seek(0)
         output_fp.truncate()
-        if compression:
-            json.dump(json_obj, output_fp, ensure_ascii=False,
-                      sort_keys=True, separators=(',', ':'))
-        else:
-            json.dump(json_obj, output_fp, ensure_ascii=False,
-                      sort_keys=True, indent=4)
+    if compression:
+        json.dump(json_obj, output_fp, ensure_ascii=escape,
+                  sort_keys=True, separators=(',', ':'))
+    else:
+        json.dump(json_obj, output_fp, ensure_ascii=escape,
+                  sort_keys=True, indent=indent)
+
+    # append a blank line at the end of `fp``
+    output_fp.write('\n')
 
 
-def parse_jsonpath(jsonpath: str) -> list[str | int]:
+def parse_jsonpath(jsonpath: str) -> List[Union[str, int]]:
     jsonpath = jsonpath.strip().strip('/')
     if not jsonpath:
         return []
     else:
         components = jsonpath.split('/')
         for i, c in enumerate(components):
             if c.isdecimal():
                 components[i] = int(c)  # type: ignore
         return components  # type: ignore
 
 
-def get_element_by_components(json_obj: Any, jpath_components: list[str | int]) -> Any:
+def get_element_by_components(json_obj: Any, jpath_components: List[Union[str, int]]) -> Any:
     for i, c in enumerate(jpath_components):
         if c == '*' and isinstance(json_obj, list):
             return [get_element_by_components(sub_obj, jpath_components[i + 1:])
                     for sub_obj in json_obj]
         else:
             try:
                 json_obj = json_obj[c]
@@ -72,14 +68,18 @@
         return get_element_by_components(json_obj, jpath_components)
 
 
 def main():
     parser = ArgumentParser('jsonfmt')
     parser.add_argument('-c', dest='compression', action='store_true',
                         help='compression the json object in the files or stdin.')
+    parser.add_argument('-e', dest='escape', action='store_true',
+                        help='escape non-ASCII characters')
+    parser.add_argument('-i', dest='indent', type=int, default=4,
+                        help='number of spaces to use for indentation. (default: %(default)s)')
     parser.add_argument('-O', dest='overwrite', action='store_true',
                         help='overwrite the formated json object into the json file.')
     parser.add_argument('-p', dest='jsonpath', type=str, default='',
                         help='output part of json object via jsonpath.')
     parser.add_argument(dest='json_files', nargs='*',
                         help='the json files that will be processed')
     parser.add_argument('-v', dest='version', action='version', version=__version__,
@@ -91,34 +91,35 @@
         for j_file in args.json_files:
             try:
                 with open(j_file, 'r+') as fp:
                     try:
                         j_obj = json.load(fp)
                         matched_obj = jsonpath_match(j_obj, args.jsonpath)
                     except json.decoder.JSONDecodeError:
-                        print_err(f"File `{j_file}` does not contains JSON string")
+                        print_err(f"no json object found from file `{j_file}`")
                         continue
                     except JSONPathError as e:
                         print_err(f'{e}')
                         continue
-                    output_fp = fp if args.overwrite else None
-                    output(matched_obj, output_fp, args.compression)
+                    output_fp = fp if args.overwrite else stdout
+                    output(matched_obj, args.compression, args.escape,
+                           args.indent, output_fp)
 
             except FileNotFoundError:
                 print_err(f'No such file `{j_file}`')
     else:
         # get json from stdin
         try:
             j_obj = json.load(stdin)
             matched_obj = jsonpath_match(j_obj, args.jsonpath)
         except json.decoder.JSONDecodeError:
-            print_err('Wrong JSON format')
+            print_err("no json object found from `stdin`")
             exit(1)
         except JSONPathError as e:
             print_err(f'{e}')
             exit(2)
         else:
-            output(matched_obj, None, args.compression)
+            output(matched_obj, args.compression, args.escape, args.indent)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jsonfmt-0.1.1/setup.py` & `jsonfmt-0.1.2/setup.py`

 * *Files identical despite different names*

