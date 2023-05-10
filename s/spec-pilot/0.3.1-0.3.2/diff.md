# Comparing `tmp/spec-pilot-0.3.1.tar.gz` & `tmp/spec-pilot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec-pilot-0.3.1.tar", last modified: Wed May 10 04:07:06 2023, max compression
+gzip compressed data, was "spec-pilot-0.3.2.tar", last modified: Wed May 10 04:12:49 2023, max compression
```

## Comparing `spec-pilot-0.3.1.tar` & `spec-pilot-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/spec_pilot/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/language_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/prompt_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/spec_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:12:49.360288 spec-pilot-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 04:12:49.360288 spec-pilot-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:12:49.360288 spec-pilot-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:12:49.356288 spec-pilot-0.3.2/spec_pilot/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/spec_pilot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/spec_pilot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/spec_pilot/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/spec_pilot/language_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/spec_pilot/prompt_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 04:12:38.000000 spec-pilot-0.3.2/spec_pilot/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:12:49.360288 spec-pilot-0.3.2/spec_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 04:12:49.000000 spec-pilot-0.3.2/spec_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 04:12:49.000000 spec-pilot-0.3.2/spec_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:12:49.000000 spec-pilot-0.3.2/spec_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 04:12:49.000000 spec-pilot-0.3.2/spec_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 04:12:49.000000 spec-pilot-0.3.2/spec_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:12:49.000000 spec-pilot-0.3.2/spec_pilot.egg-info/top_level.txt
```

### Comparing `spec-pilot-0.3.1/LICENSE` & `spec-pilot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.1/PKG-INFO` & `spec-pilot-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec-pilot
-Version: 0.3.1
+Version: 0.3.2
 Summary: A command-line tool for generating and managing OpenAPI specifications
 Home-page: https://github.com/jmfwolf/spec-pilot
 Author: jmfwolf
 Author-email: jmfwolf@hacksomniac.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `spec-pilot-0.3.1/README.md` & `spec-pilot-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.1/setup.py` & `spec-pilot-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="spec-pilot",
-    version="0.3.1",
+    version="0.3.2",
     description="A command-line tool for generating and managing OpenAPI specifications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="jmfwolf",
     author_email="jmfwolf@hacksomniac.com",
     url="https://github.com/jmfwolf/spec-pilot",
     packages=find_packages(),
```

### Comparing `spec-pilot-0.3.1/spec_pilot/__main__.py` & `spec-pilot-0.3.2/spec_pilot/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import yaml
 import os
-from prompt_builder import PromptBuilder
-from generator import Generator
-from validator import Validator
+from .prompt_builder import PromptBuilder
+from .generator import Generator
+from .validator import Validator
 
 def create_project_structure(project_name):
     # create a project directory
     os.makedirs(project_name, exist_ok=True)
 
     # create a directory in the project for: schemas, resources, responses, and parameters
     os.makedirs(os.path.join(project_name, "schemas"), exist_ok=True)
```

### Comparing `spec-pilot-0.3.1/spec_pilot/generator.py` & `spec-pilot-0.3.2/spec_pilot/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import yaml
-from language_processor import LanguageProcessor
+from .language_processor import LanguageProcessor
 
 class Generator:
     def __init__(self, description):
         self.description = description
         self.language_processor = LanguageProcessor()
 
     def _generate_openapi_component(self, component_type, component_info):
```

### Comparing `spec-pilot-0.3.1/spec_pilot/language_processor.py` & `spec-pilot-0.3.2/spec_pilot/language_processor.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.1/spec_pilot/prompt_builder.py` & `spec-pilot-0.3.2/spec_pilot/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.1/spec_pilot/validator.py` & `spec-pilot-0.3.2/spec_pilot/validator.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.1/spec_pilot.egg-info/PKG-INFO` & `spec-pilot-0.3.2/spec_pilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec-pilot
-Version: 0.3.1
+Version: 0.3.2
 Summary: A command-line tool for generating and managing OpenAPI specifications
 Home-page: https://github.com/jmfwolf/spec-pilot
 Author: jmfwolf
 Author-email: jmfwolf@hacksomniac.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

