# Comparing `tmp/spec-pilot-0.3.3.tar.gz` & `tmp/spec-pilot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec-pilot-0.3.3.tar", last modified: Wed May 10 04:33:24 2023, max compression
+gzip compressed data, was "spec-pilot-0.3.4.tar", last modified: Wed May 10 05:15:28 2023, max compression
```

## Comparing `spec-pilot-0.3.3.tar` & `spec-pilot-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:33:24.715129 spec-pilot-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 04:33:24.711130 spec-pilot-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 04:33:24.715129 spec-pilot-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:33:24.711130 spec-pilot-0.3.3/spec_pilot/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/spec_pilot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/spec_pilot/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/spec_pilot/language_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/spec_pilot/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/spec_pilot/prompt_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 04:33:13.000000 spec-pilot-0.3.3/spec_pilot/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:33:24.711130 spec-pilot-0.3.3/spec_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 04:33:24.000000 spec-pilot-0.3.3/spec_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 04:33:24.000000 spec-pilot-0.3.3/spec_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:33:24.000000 spec-pilot-0.3.3/spec_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 04:33:24.000000 spec-pilot-0.3.3/spec_pilot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 04:33:24.000000 spec-pilot-0.3.3/spec_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:33:24.000000 spec-pilot-0.3.3/spec_pilot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:15:28.567728 spec-pilot-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 05:15:28.567728 spec-pilot-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 05:15:28.567728 spec-pilot-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:15:28.567728 spec-pilot-0.3.4/spec_pilot/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/spec_pilot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/spec_pilot/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/spec_pilot/language_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/spec_pilot/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/spec_pilot/prompt_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 05:15:14.000000 spec-pilot-0.3.4/spec_pilot/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:15:28.567728 spec-pilot-0.3.4/spec_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 05:15:28.000000 spec-pilot-0.3.4/spec_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 05:15:28.000000 spec-pilot-0.3.4/spec_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:15:28.000000 spec-pilot-0.3.4/spec_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 05:15:28.000000 spec-pilot-0.3.4/spec_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 05:15:28.000000 spec-pilot-0.3.4/spec_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 05:15:28.000000 spec-pilot-0.3.4/spec_pilot.egg-info/top_level.txt
```

### Comparing `spec-pilot-0.3.3/LICENSE` & `spec-pilot-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.3/PKG-INFO` & `spec-pilot-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec-pilot
-Version: 0.3.3
+Version: 0.3.4
 Summary: A command-line tool for generating and managing OpenAPI specifications
 Home-page: https://github.com/jmfwolf/spec-pilot
 Author: jmfwolf
 Author-email: jmfwolf@hacksomniac.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `spec-pilot-0.3.3/README.md` & `spec-pilot-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.3/setup.py` & `spec-pilot-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setup(
     name="spec-pilot",
-    version="0.3.3",
+    version="0.3.4",
     description="A command-line tool for generating and managing OpenAPI specifications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="jmfwolf",
     author_email="jmfwolf@hacksomniac.com",
     url="https://github.com/jmfwolf/spec-pilot",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
-            "spec-pilo=spec_pilot.main:main",
+            "spec-pilot=spec_pilot.main:main",
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
@@ -31,8 +31,8 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     python_requires='>=3.6',
-)
+)
```

### Comparing `spec-pilot-0.3.3/spec_pilot/generator.py` & `spec-pilot-0.3.4/spec_pilot/generator.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.3/spec_pilot/language_processor.py` & `spec-pilot-0.3.4/spec_pilot/language_processor.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.3/spec_pilot/main.py` & `spec-pilot-0.3.4/spec_pilot/main.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.3/spec_pilot/prompt_builder.py` & `spec-pilot-0.3.4/spec_pilot/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.3/spec_pilot/validator.py` & `spec-pilot-0.3.4/spec_pilot/validator.py`

 * *Files identical despite different names*

### Comparing `spec-pilot-0.3.3/spec_pilot.egg-info/PKG-INFO` & `spec-pilot-0.3.4/spec_pilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spec-pilot
-Version: 0.3.3
+Version: 0.3.4
 Summary: A command-line tool for generating and managing OpenAPI specifications
 Home-page: https://github.com/jmfwolf/spec-pilot
 Author: jmfwolf
 Author-email: jmfwolf@hacksomniac.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

