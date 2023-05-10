# Comparing `tmp/spec-pilot-0.3.0.tar.gz` & `tmp/spec-pilot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec-pilot-0.3.0.tar", last modified: Wed May 10 03:57:34 2023, max compression
+gzip compressed data, was "spec-pilot-0.3.1.tar", last modified: Wed May 10 04:07:06 2023, max compression
```

## Comparing `spec-pilot-0.3.0.tar` & `spec-pilot-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:57:34.826766 spec-pilot-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 03:57:34.826766 spec-pilot-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:57:34.826766 spec-pilot-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:57:34.822765 spec-pilot-0.3.0/spec_pilot/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/language_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/prompt_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:57:34.822765 spec-pilot-0.3.0/spec_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/spec_pilot/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/language_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/prompt_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 04:06:55.000000 spec-pilot-0.3.1/spec_pilot/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:07:06.991142 spec-pilot-0.3.1/spec_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:07:06.000000 spec-pilot-0.3.1/spec_pilot.egg-info/top_level.txt
```

### Comparing `spec-pilot-0.3.0/LICENSE` & `spec-pilot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.0/PKG-INFO` & `spec-pilot-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec-pilot
-Version: 0.3.0
+Version: 0.3.1
 Summary: A command-line tool for generating and managing OpenAPI specifications
 Home-page: https://github.com/jmfwolf/spec-pilot
 Author: jmfwolf
 Author-email: jmfwolf@hacksomniac.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `spec-pilot-0.3.0/README.md` & `spec-pilot-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.0/setup.py` & `spec-pilot-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="spec-pilot",
-    version="0.3.0",
+    version="0.3.1",
     description="A command-line tool for generating and managing OpenAPI specifications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="jmfwolf",
     author_email="jmfwolf@hacksomniac.com",
     url="https://github.com/jmfwolf/spec-pilot",
     packages=find_packages(),
```

### Comparing `spec-pilot-0.3.0/spec_pilot/__main__.py` & `spec-pilot-0.3.1/spec_pilot/__main__.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.0/spec_pilot/generator.py` & `spec-pilot-0.3.1/spec_pilot/generator.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.0/spec_pilot/language_processor.py` & `spec-pilot-0.3.1/spec_pilot/language_processor.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.0/spec_pilot/prompt_builder.py` & `spec-pilot-0.3.1/spec_pilot/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.0/spec_pilot/validator.py` & `spec-pilot-0.3.1/spec_pilot/validator.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.0/spec_pilot.egg-info/PKG-INFO` & `spec-pilot-0.3.1/spec_pilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec-pilot
-Version: 0.3.0
+Version: 0.3.1
 Summary: A command-line tool for generating and managing OpenAPI specifications
 Home-page: https://github.com/jmfwolf/spec-pilot
 Author: jmfwolf
 Author-email: jmfwolf@hacksomniac.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

