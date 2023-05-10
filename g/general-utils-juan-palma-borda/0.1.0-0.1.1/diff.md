# Comparing `tmp/general-utils-juan-palma-borda-0.1.0.tar.gz` & `tmp/general-utils-juan-palma-borda-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general-utils-juan-palma-borda-0.1.0.tar", last modified: Wed May 10 09:37:14 2023, max compression
+gzip compressed data, was "general-utils-juan-palma-borda-0.1.1.tar", last modified: Wed May 10 09:48:08 2023, max compression
```

## Comparing `general-utils-juan-palma-borda-0.1.0.tar` & `general-utils-juan-palma-borda-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:14.949352 general-utils-juan-palma-borda-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-10 09:37:14.949352 general-utils-juan-palma-borda-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-10 09:37:14.953352 general-utils-juan-palma-borda-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:14.949352 general-utils-juan-palma-borda-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:14.949352 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:14.949352 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/clases_auxiliares/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/clases_auxiliares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/clases_auxiliares/punto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:14.949352 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/patrones/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/patrones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/patrones/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/prints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-10 09:37:03.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_j/umaths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:37:14.949352 general-utils-juan-palma-borda-0.1.0/src/general_utils_juan_palma_borda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-10 09:37:14.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_juan_palma_borda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-10 09:37:14.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_juan_palma_borda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:37:14.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_juan_palma_borda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 09:37:14.000000 general-utils-juan-palma-borda-0.1.0/src/general_utils_juan_palma_borda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:48:08.850890 general-utils-juan-palma-borda-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-10 09:48:08.850890 general-utils-juan-palma-borda-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-10 09:48:08.850890 general-utils-juan-palma-borda-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:48:08.850890 general-utils-juan-palma-borda-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:48:08.850890 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:48:08.850890 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/clases_auxiliares/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/clases_auxiliares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/clases_auxiliares/punto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:48:08.850890 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/patrones/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/patrones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/patrones/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/prints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-10 09:47:55.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_j/umaths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:48:08.850890 general-utils-juan-palma-borda-0.1.1/src/general_utils_juan_palma_borda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-10 09:48:08.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_juan_palma_borda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-10 09:48:08.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_juan_palma_borda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:48:08.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_juan_palma_borda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 09:48:08.000000 general-utils-juan-palma-borda-0.1.1/src/general_utils_juan_palma_borda.egg-info/top_level.txt
```

### Comparing `general-utils-juan-palma-borda-0.1.0/LICENSE` & `general-utils-juan-palma-borda-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `general-utils-juan-palma-borda-0.1.0/LICENSE.txt` & `general-utils-juan-palma-borda-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `general-utils-juan-palma-borda-0.1.0/PKG-INFO` & `general-utils-juan-palma-borda-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: general-utils-juan-palma-borda
-Version: 0.1.0
+Version: 0.1.1
 Summary: Group of general utils from different projects
 Home-page: https://github.com/muerterauda/general-utils
 Author: Juan Palma Borda
 Author-email: juanpalmaborda@hotmail.com
 Project-URL: Bug Tracker, https://github.com/muerterauda/general-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
-# General Utils (0.1.0)
+# General Utils (0.1.1)
 
 Group of general utils from different projects.
 
 Included classes:
 
 - Point class
 - Singleton pattern
```

### Comparing `general-utils-juan-palma-borda-0.1.0/setup.cfg` & `general-utils-juan-palma-borda-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = general-utils-juan-palma-borda
-version = 0.1.0
+version = 0.1.1
 author = Juan Palma Borda
 author_email = juanpalmaborda@hotmail.com
 description = Group of general utils from different projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/muerterauda/general-utils
 project_urls =
```

### Comparing `general-utils-juan-palma-borda-0.1.0/setup.py` & `general-utils-juan-palma-borda-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="general-utils-juan-palma-borda",
-    version="0.1.0",
+    version="0.1.1",
     author='Juan Palma Borda',
     author_email='juanpalmaborda@hotmail.com',
     description='Group of general utils from different projects',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/muerterauda/general-utils",
     project_urls={
```

### Comparing `general-utils-juan-palma-borda-0.1.0/src/general_utils_j/clases_auxiliares/punto.py` & `general-utils-juan-palma-borda-0.1.1/src/general_utils_j/clases_auxiliares/punto.py`

 * *Files identical despite different names*

### Comparing `general-utils-juan-palma-borda-0.1.0/src/general_utils_j/colors.py` & `general-utils-juan-palma-borda-0.1.1/src/general_utils_j/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     HIGHLIGHTS_LIGHT_BLUE = '\033[104m'
     HIGHLIGHTS_LIGHT_MAGENTA = '\033[105m'
     HIGHLIGHTS_LIGHT_CYAN = '\033[106m'
 
     @staticmethod
     def format_text(text, color, highlights=None, attributes: list = None, end: bool = False):
         return f'{color}{highlights if highlights is not None else ""}' \
-               f'{"".join(attributes) if len(attributes) > 0 else ""}' \
-               f'{text}{end if end is not None else ""}'
+               f'{"".join(attributes) if attributes is not None and len(attributes) > 0 else ""}' \
+               f'{text}{bcolors.ENDC if end is not None else ""}'
 
 
 class wcolors:
     BLACK = (0, 0, 0)
     GRAY = (128, 128, 128)
     WHITE = (255, 255, 255)
```

### Comparing `general-utils-juan-palma-borda-0.1.0/src/general_utils_j/prints.py` & `general-utils-juan-palma-borda-0.1.1/src/general_utils_j/prints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 class Prints:
 
     @staticmethod
     def print_list(list_print: list, end_attribute='\n'):
         if list_print is not None:
-            print(f'{end_attribute.join(list_print)}')
+            print(f'{end_attribute.join(str(list_print))}')
         if end_attribute == '':
             print()
 
     @staticmethod
     def print_dict_line(dictionary: dict, end_attribute='\n'):
         for x, y in dictionary.items():
             print(f'{x} : {y}', end=end_attribute)
```

### Comparing `general-utils-juan-palma-borda-0.1.0/src/general_utils_j/umaths.py` & `general-utils-juan-palma-borda-0.1.1/src/general_utils_j/umaths.py`

 * *Files identical despite different names*

### Comparing `general-utils-juan-palma-borda-0.1.0/src/general_utils_juan_palma_borda.egg-info/PKG-INFO` & `general-utils-juan-palma-borda-0.1.1/src/general_utils_juan_palma_borda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: general-utils-juan-palma-borda
-Version: 0.1.0
+Version: 0.1.1
 Summary: Group of general utils from different projects
 Home-page: https://github.com/muerterauda/general-utils
 Author: Juan Palma Borda
 Author-email: juanpalmaborda@hotmail.com
 Project-URL: Bug Tracker, https://github.com/muerterauda/general-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
-# General Utils (0.1.0)
+# General Utils (0.1.1)
 
 Group of general utils from different projects.
 
 Included classes:
 
 - Point class
 - Singleton pattern
```

### Comparing `general-utils-juan-palma-borda-0.1.0/src/general_utils_juan_palma_borda.egg-info/SOURCES.txt` & `general-utils-juan-palma-borda-0.1.1/src/general_utils_juan_palma_borda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

