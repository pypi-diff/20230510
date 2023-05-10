# Comparing `tmp/whisper2subs-0.1.0.tar.gz` & `tmp/whisper2subs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper2subs-0.1.0.tar", last modified: Tue Apr 11 23:41:09 2023, max compression
+gzip compressed data, was "whisper2subs-0.1.1.tar", last modified: Wed May 10 20:24:27 2023, max compression
```

## Comparing `whisper2subs-0.1.0.tar` & `whisper2subs-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:41:09.000152 whisper2subs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-11 23:41:09.000152 whisper2subs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:41:09.000152 whisper2subs-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:41:09.000152 whisper2subs-0.1.0/whisper2subs/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/whisper2subs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/whisper2subs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/whisper2subs/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/whisper2subs/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/whisper2subs/transcribe.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-11 23:40:58.000000 whisper2subs-0.1.0/whisper2subs/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:41:09.000152 whisper2subs-0.1.0/whisper2subs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-11 23:41:08.000000 whisper2subs-0.1.0/whisper2subs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-11 23:41:08.000000 whisper2subs-0.1.0/whisper2subs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:41:08.000000 whisper2subs-0.1.0/whisper2subs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 23:41:08.000000 whisper2subs-0.1.0/whisper2subs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-11 23:41:08.000000 whisper2subs-0.1.0/whisper2subs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 23:41:08.000000 whisper2subs-0.1.0/whisper2subs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:24:27.125236 whisper2subs-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-10 20:24:27.125236 whisper2subs-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:24:27.125236 whisper2subs-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:24:27.125236 whisper2subs-0.1.1/whisper2subs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/whisper2subs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/whisper2subs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/whisper2subs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/whisper2subs/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/whisper2subs/transcribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-10 20:24:13.000000 whisper2subs-0.1.1/whisper2subs/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:24:27.125236 whisper2subs-0.1.1/whisper2subs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-10 20:24:27.000000 whisper2subs-0.1.1/whisper2subs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 20:24:27.000000 whisper2subs-0.1.1/whisper2subs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:24:27.000000 whisper2subs-0.1.1/whisper2subs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 20:24:27.000000 whisper2subs-0.1.1/whisper2subs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 20:24:27.000000 whisper2subs-0.1.1/whisper2subs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 20:24:27.000000 whisper2subs-0.1.1/whisper2subs.egg-info/top_level.txt
```

### Comparing `whisper2subs-0.1.0/LICENSE` & `whisper2subs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper2subs-0.1.0/PKG-INFO` & `whisper2subs-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: whisper2subs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transcribes audio using Whisper and translates it using DeepL.
 Author-email: Daniel Luque <danielluque14@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/LuqueDaniel/whisper2subs
 Project-URL: Issue Tracker, https://github.com/LuqueDaniel/whisper2subs/issues
 Project-URL: Documentation, https://github.com/LuqueDaniel/whisper2subs/blob/main/README.md
 Keywords: whisper,subs,cli,translate,transcribe
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,17 +22,17 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-![PyPI](https://img.shields.io/pypi/v/whisper2subs?style=flat-square)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whisper2subs?style=flat-square)
-![GitHub](https://img.shields.io/github/license/LuqueDaniel/whisper2subs?style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/whisper2subs?style=flat-square)](https://pypi.org/project/whisper2subs/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whisper2subs?style=flat-square)](https://pypi.org/project/whisper2subs/)
+[![PyPI - License](https://img.shields.io/pypi/l/whisper2subs?style=flat-square)](https://github.com/LuqueDaniel/whisper2subs/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black?style=flat-square)
 
 # whisper2subs
 
 A CLI tool that transcribes audio using [`openai-whisper`](https://github.com/openai/whisper) and translates it using [DeepL](https://www.deepl.com/docs-api).
 
 ## Install
```

### Comparing `whisper2subs-0.1.0/README.md` & `whisper2subs-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-![PyPI](https://img.shields.io/pypi/v/whisper2subs?style=flat-square)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whisper2subs?style=flat-square)
-![GitHub](https://img.shields.io/github/license/LuqueDaniel/whisper2subs?style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/whisper2subs?style=flat-square)](https://pypi.org/project/whisper2subs/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whisper2subs?style=flat-square)](https://pypi.org/project/whisper2subs/)
+[![PyPI - License](https://img.shields.io/pypi/l/whisper2subs?style=flat-square)](https://github.com/LuqueDaniel/whisper2subs/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black?style=flat-square)
 
 # whisper2subs
 
 A CLI tool that transcribes audio using [`openai-whisper`](https://github.com/openai/whisper) and translates it using [DeepL](https://www.deepl.com/docs-api).
 
 ## Install
```

### Comparing `whisper2subs-0.1.0/pyproject.toml` & `whisper2subs-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "whisper2subs"
 description = "Transcribes audio using Whisper and translates it using DeepL."
 authors = [{name = "Daniel Luque", email = "danielluque14@gmail.com"}]
 readme = "README.md"
 license = {text = "MIT"}
 keywords = ["whisper", "subs", "cli", "translate", "transcribe"]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Environment :: GPU :: NVIDIA CUDA",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -38,15 +38,15 @@
 Documentation = "https://github.com/LuqueDaniel/whisper2subs/blob/main/README.md"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit >=3.2.2",
     "black >=23.3.0",
     "isort >=5.12.0",
-    "ruff >=0.0.261",
+    "ruff >=0.0.265",
     "mypy >=1.2.0",
 ]
 
 [project.scripts]
 whisper2subs = "whisper2subs.cli:whisper2subs"
 
 [tool.setuptools]
```

### Comparing `whisper2subs-0.1.0/whisper2subs/cli.py` & `whisper2subs-0.1.1/whisper2subs/cli.py`

 * *Files identical despite different names*

### Comparing `whisper2subs-0.1.0/whisper2subs/transcribe.py` & `whisper2subs-0.1.1/whisper2subs/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper2subs-0.1.0/whisper2subs/translate.py` & `whisper2subs-0.1.1/whisper2subs/translate.py`

 * *Files identical despite different names*

### Comparing `whisper2subs-0.1.0/whisper2subs.egg-info/PKG-INFO` & `whisper2subs-0.1.1/whisper2subs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: whisper2subs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transcribes audio using Whisper and translates it using DeepL.
 Author-email: Daniel Luque <danielluque14@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/LuqueDaniel/whisper2subs
 Project-URL: Issue Tracker, https://github.com/LuqueDaniel/whisper2subs/issues
 Project-URL: Documentation, https://github.com/LuqueDaniel/whisper2subs/blob/main/README.md
 Keywords: whisper,subs,cli,translate,transcribe
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,17 +22,17 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-![PyPI](https://img.shields.io/pypi/v/whisper2subs?style=flat-square)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whisper2subs?style=flat-square)
-![GitHub](https://img.shields.io/github/license/LuqueDaniel/whisper2subs?style=flat-square)
+[![PyPI](https://img.shields.io/pypi/v/whisper2subs?style=flat-square)](https://pypi.org/project/whisper2subs/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/whisper2subs?style=flat-square)](https://pypi.org/project/whisper2subs/)
+[![PyPI - License](https://img.shields.io/pypi/l/whisper2subs?style=flat-square)](https://github.com/LuqueDaniel/whisper2subs/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black?style=flat-square)
 
 # whisper2subs
 
 A CLI tool that transcribes audio using [`openai-whisper`](https://github.com/openai/whisper) and translates it using [DeepL](https://www.deepl.com/docs-api).
 
 ## Install
```

