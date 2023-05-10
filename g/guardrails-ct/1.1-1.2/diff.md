# Comparing `tmp/guardrails-ct-1.1.tar.gz` & `tmp/guardrails-ct-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrails-ct-1.1.tar", last modified: Wed May 10 18:56:43 2023, max compression
+gzip compressed data, was "guardrails-ct-1.2.tar", last modified: Wed May 10 19:51:32 2023, max compression
```

## Comparing `guardrails-ct-1.1.tar` & `guardrails-ct-1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:56:43.905747 guardrails-ct-1.1/
--rw-r--r--   0 root         (0) root         (0)      584 2023-05-10 18:56:43.905747 guardrails-ct-1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:56:43.901747 guardrails-ct-1.1/guardrails/
--rw-rw-r--   0 root         (0) root         (0)      629 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:56:43.902747 guardrails-ct-1.1/guardrails/applications/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/applications/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6588 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/applications/text2sql.py
--rw-rw-r--   0 root         (0) root         (0)     1613 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/cli.py
--rw-rw-r--   0 root         (0) root         (0)    16775 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/datatypes.py
--rw-rw-r--   0 root         (0) root         (0)     7361 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/document_store.py
--rw-rw-r--   0 root         (0) root         (0)     6331 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/embedding.py
--rw-rw-r--   0 root         (0) root         (0)     6486 2023-05-10 18:51:54.000000 guardrails-ct-1.1/guardrails/guard.py
--rw-rw-r--   0 root         (0) root         (0)     4794 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/llm_providers.py
--rw-rw-r--   0 root         (0) root         (0)      118 2023-05-10 17:48:36.000000 guardrails-ct-1.1/guardrails/logging_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:56:43.902747 guardrails-ct-1.1/guardrails/prompt/
--rw-rw-r--   0 root         (0) root         (0)      115 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/prompt/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3260 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/prompt/base_prompt.py
--rw-rw-r--   0 root         (0) root         (0)     1279 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/prompt/instructions.py
--rw-rw-r--   0 root         (0) root         (0)      796 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/prompt/prompt.py
--rw-rw-r--   0 root         (0) root         (0)     7373 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/rail.py
--rw-rw-r--   0 root         (0) root         (0)    10470 2023-05-10 17:47:54.000000 guardrails-ct-1.1/guardrails/run.py
--rw-rw-r--   0 root         (0) root         (0)    18806 2023-05-10 17:47:05.000000 guardrails-ct-1.1/guardrails/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:56:43.904747 guardrails-ct-1.1/guardrails/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1555 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/utils/constants.py
--rw-rw-r--   0 root         (0) root         (0)     2530 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/utils/docs_utils.py
--rw-rw-r--   0 root         (0) root         (0)     6145 2023-05-10 17:55:25.000000 guardrails-ct-1.1/guardrails/utils/logs_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2613 2023-05-10 17:54:27.000000 guardrails-ct-1.1/guardrails/utils/misc.py
--rw-rw-r--   0 root         (0) root         (0)     3349 2023-05-10 17:53:21.000000 guardrails-ct-1.1/guardrails/utils/pydantic_utils.py
--rw-rw-r--   0 root         (0) root         (0)     8944 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/utils/reask_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4030 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/utils/sql_utils.py
--rw-rw-r--   0 root         (0) root         (0)    45134 2023-05-10 17:46:41.000000 guardrails-ct-1.1/guardrails/validators.py
--rw-rw-r--   0 root         (0) root         (0)       22 2023-05-10 07:58:25.000000 guardrails-ct-1.1/guardrails/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 18:56:43.905747 guardrails-ct-1.1/guardrails_ct.egg-info/
--rw-r--r--   0 root         (0) root         (0)      584 2023-05-10 18:56:43.000000 guardrails-ct-1.1/guardrails_ct.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2023-05-10 18:56:43.000000 guardrails-ct-1.1/guardrails_ct.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 18:56:43.000000 guardrails-ct-1.1/guardrails_ct.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-10 18:56:43.000000 guardrails-ct-1.1/guardrails_ct.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-10 18:56:43.000000 guardrails-ct-1.1/guardrails_ct.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-10 18:56:43.000000 guardrails-ct-1.1/guardrails_ct.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 18:56:43.905747 guardrails-ct-1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3772 2023-05-10 18:55:43.000000 guardrails-ct-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:51:32.729969 guardrails-ct-1.2/
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-10 19:51:32.728969 guardrails-ct-1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:51:32.725969 guardrails-ct-1.2/guardrails/
+-rw-rw-r--   0 root         (0) root         (0)      629 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:51:32.725969 guardrails-ct-1.2/guardrails/applications/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/applications/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6588 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/applications/text2sql.py
+-rw-rw-r--   0 root         (0) root         (0)     1613 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/cli.py
+-rw-rw-r--   0 root         (0) root         (0)    16775 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/datatypes.py
+-rw-rw-r--   0 root         (0) root         (0)     7361 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/document_store.py
+-rw-rw-r--   0 root         (0) root         (0)     6331 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/embedding.py
+-rw-rw-r--   0 root         (0) root         (0)     6486 2023-05-10 18:51:54.000000 guardrails-ct-1.2/guardrails/guard.py
+-rw-rw-r--   0 root         (0) root         (0)     4794 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/llm_providers.py
+-rw-rw-r--   0 root         (0) root         (0)      118 2023-05-10 17:48:36.000000 guardrails-ct-1.2/guardrails/logging_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:51:32.726969 guardrails-ct-1.2/guardrails/prompt/
+-rw-rw-r--   0 root         (0) root         (0)      115 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/prompt/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3260 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/prompt/base_prompt.py
+-rw-rw-r--   0 root         (0) root         (0)     1279 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/prompt/instructions.py
+-rw-rw-r--   0 root         (0) root         (0)      796 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/prompt/prompt.py
+-rw-rw-r--   0 root         (0) root         (0)     7373 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/rail.py
+-rw-rw-r--   0 root         (0) root         (0)    10470 2023-05-10 17:47:54.000000 guardrails-ct-1.2/guardrails/run.py
+-rw-rw-r--   0 root         (0) root         (0)    18806 2023-05-10 17:47:05.000000 guardrails-ct-1.2/guardrails/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:51:32.727969 guardrails-ct-1.2/guardrails/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6103 2023-05-10 19:48:46.000000 guardrails-ct-1.2/guardrails/utils/constants.py
+-rw-rw-r--   0 root         (0) root         (0)     2530 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/utils/docs_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6145 2023-05-10 17:55:25.000000 guardrails-ct-1.2/guardrails/utils/logs_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2613 2023-05-10 17:54:27.000000 guardrails-ct-1.2/guardrails/utils/misc.py
+-rw-rw-r--   0 root         (0) root         (0)     3349 2023-05-10 17:53:21.000000 guardrails-ct-1.2/guardrails/utils/pydantic_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     8944 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/utils/reask_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4030 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/utils/sql_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    45134 2023-05-10 17:46:41.000000 guardrails-ct-1.2/guardrails/validators.py
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-05-10 07:58:25.000000 guardrails-ct-1.2/guardrails/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:51:32.728969 guardrails-ct-1.2/guardrails_ct.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-10 19:51:32.000000 guardrails-ct-1.2/guardrails_ct.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-05-10 19:51:32.000000 guardrails-ct-1.2/guardrails_ct.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 19:51:32.000000 guardrails-ct-1.2/guardrails_ct.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-10 19:51:32.000000 guardrails-ct-1.2/guardrails_ct.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-10 19:51:32.000000 guardrails-ct-1.2/guardrails_ct.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-10 19:51:32.000000 guardrails-ct-1.2/guardrails_ct.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:51:32.729969 guardrails-ct-1.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4084 2023-05-10 19:50:30.000000 guardrails-ct-1.2/setup.py
```

### Comparing `guardrails-ct-1.1/PKG-INFO` & `guardrails-ct-1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: guardrails-ct
-Version: 1.1
+Version: 1.2
 Summary: Adding guardrails to large language models.
-Home-page: UNKNOWN
+Home-page: https://github.com/shreyar/guardrails
+Author: Shreya Rajpal
+Author-email: shreya.rajpal@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
```

### Comparing `guardrails-ct-1.1/guardrails/__init__.py` & `guardrails-ct-1.2/guardrails/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/applications/text2sql.py` & `guardrails-ct-1.2/guardrails/applications/text2sql.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/cli.py` & `guardrails-ct-1.2/guardrails/cli.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/datatypes.py` & `guardrails-ct-1.2/guardrails/datatypes.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/document_store.py` & `guardrails-ct-1.2/guardrails/document_store.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/embedding.py` & `guardrails-ct-1.2/guardrails/embedding.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/guard.py` & `guardrails-ct-1.2/guardrails/guard.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/llm_providers.py` & `guardrails-ct-1.2/guardrails/llm_providers.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/prompt/base_prompt.py` & `guardrails-ct-1.2/guardrails/prompt/base_prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/prompt/instructions.py` & `guardrails-ct-1.2/guardrails/prompt/instructions.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/prompt/prompt.py` & `guardrails-ct-1.2/guardrails/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/rail.py` & `guardrails-ct-1.2/guardrails/rail.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/run.py` & `guardrails-ct-1.2/guardrails/run.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/schema.py` & `guardrails-ct-1.2/guardrails/schema.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/utils/docs_utils.py` & `guardrails-ct-1.2/guardrails/utils/docs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/utils/logs_utils.py` & `guardrails-ct-1.2/guardrails/utils/logs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/utils/misc.py` & `guardrails-ct-1.2/guardrails/utils/misc.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/utils/pydantic_utils.py` & `guardrails-ct-1.2/guardrails/utils/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/utils/reask_utils.py` & `guardrails-ct-1.2/guardrails/utils/reask_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/utils/sql_utils.py` & `guardrails-ct-1.2/guardrails/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails/validators.py` & `guardrails-ct-1.2/guardrails/validators.py`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/guardrails_ct.egg-info/PKG-INFO` & `guardrails-ct-1.2/guardrails_ct.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: guardrails-ct
-Version: 1.1
+Version: 1.2
 Summary: Adding guardrails to large language models.
-Home-page: UNKNOWN
+Home-page: https://github.com/shreyar/guardrails
+Author: Shreya Rajpal
+Author-email: shreya.rajpal@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
```

### Comparing `guardrails-ct-1.1/guardrails_ct.egg-info/SOURCES.txt` & `guardrails-ct-1.2/guardrails_ct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guardrails-ct-1.1/setup.py` & `guardrails-ct-1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,37 @@
 #   $ pipenv install twine --dev
 import sys
 from distutils.util import convert_path
 
 from setuptools import Command, find_packages, setup
 
 
+
 # Package meta-data.
 NAME = "guardrails-ct"
 DESCRIPTION = "Adding guardrails to large language models."
+URL = "https://github.com/shreyar/guardrails"
+EMAIL = "shreya.rajpal@gmail.com"
+AUTHOR = "Shreya Rajpal"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = 1.1
+VERSION = "1.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "lxml",
     "openai",
     "rich",
     "eliot",
     "eliot-tree",
     "pydantic",
     "typer",
     "griffe",
     "tenacity",
 ]
 
-
-
 # What packages are optional?
 EXTRAS = {
     "dev": [
         "black==22.12.0",
         "isort>=5.12.0",
         "flake8>=3.8.4",
         "docformatter>=1.4",
@@ -57,16 +59,19 @@
 # Except, perhaps the License and Trove Classifiers!
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-
-long_description = DESCRIPTION
+try:
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
     with open(os.path.join(here, project_slug, "__version__.py")) as f:
         exec(f.read(), about)
@@ -109,15 +114,18 @@
 # Where the magic happens:
 setup(
     name=NAME,
     version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
+    author=AUTHOR,
+    author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
+    url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
     # Add CLI for "guardrails" command, point to guardrails.cli:cli
     entry_points={
         "console_scripts": ["guardrails=guardrails.cli:cli"],
     },
@@ -133,8 +141,8 @@
         "Programming Language :: Python :: 3.6",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     # $ setup.py publish support.
     cmdclass={
         "upload": UploadCommand,
     },
-)
+)
```

