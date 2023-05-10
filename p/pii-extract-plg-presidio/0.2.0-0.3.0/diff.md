# Comparing `tmp/pii-extract-plg-presidio-0.2.0.tar.gz` & `tmp/pii-extract-plg-presidio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pii-extract-plg-presidio-0.2.0.tar", last modified: Wed Mar 22 22:29:06 2023, max compression
+gzip compressed data, was "pii-extract-plg-presidio-0.3.0.tar", last modified: Wed May 10 18:10:16 2023, max compression
```

## Comparing `pii-extract-plg-presidio-0.2.0.tar` & `pii-extract-plg-presidio-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:29:06.006428 pii-extract-plg-presidio-0.2.0/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-extract-plg-presidio-0.2.0/LICENSE
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       79 2023-01-23 13:23:53.000000 pii-extract-plg-presidio-0.2.0/MANIFEST.in
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4843 2023-03-22 22:29:06.006428 pii-extract-plg-presidio-0.2.0/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4121 2023-03-22 22:28:54.000000 pii-extract-plg-presidio-0.2.0/README.md
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      136 2023-03-22 22:28:54.000000 pii-extract-plg-presidio-0.2.0/requirements.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-03-22 22:29:06.006428 pii-extract-plg-presidio-0.2.0/setup.cfg
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2749 2023-01-23 13:23:53.000000 pii-extract-plg-presidio-0.2.0/setup.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:29:06.002428 pii-extract-plg-presidio-0.2.0/src/
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:29:06.006428 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       18 2023-03-22 22:28:54.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2342 2023-03-22 22:28:54.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/analyzer.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:29:06.006428 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/app/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 13:23:53.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/app/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     6381 2023-01-23 13:23:53.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/app/info.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      386 2023-03-22 22:28:54.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/defs.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2402 2023-03-22 22:28:54.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/plugin_loader.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:29:06.006428 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/resources/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1131 2023-03-22 22:28:54.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/resources/plugin-config.json
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     7134 2023-03-22 22:28:54.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/task.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:29:06.006428 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio.egg-info/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4843 2023-03-22 22:29:05.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio.egg-info/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      715 2023-03-22 22:29:05.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio.egg-info/SOURCES.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-03-22 22:29:05.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio.egg-info/dependency_links.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      198 2023-03-22 22:29:05.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio.egg-info/entry_points.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      152 2023-03-22 22:29:05.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio.egg-info/requires.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       25 2023-03-22 22:29:05.000000 pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio.egg-info/top_level.txt
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-extract-plg-presidio-0.3.0/LICENSE
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       79 2023-01-23 13:23:53.000000 pii-extract-plg-presidio-0.3.0/MANIFEST.in
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4227 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4298 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/README.md
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       89 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/requirements.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/setup.cfg
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2749 2023-01-23 13:23:53.000000 pii-extract-plg-presidio-0.3.0/setup.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/src/
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       18 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/app/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 13:23:53.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/app/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     6387 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/app/info.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      431 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/defs.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2391 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/plugin_loader.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/resources/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1591 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/resources/plugin-config.json
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/task/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      124 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/task/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2309 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/task/analyzer.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2968 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/task/collector.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4952 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/task/task.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      716 2023-05-10 16:29:55.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/task/utils.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:16.325338 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio.egg-info/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4227 2023-05-10 18:10:16.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio.egg-info/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      861 2023-05-10 18:10:16.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio.egg-info/SOURCES.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-05-10 18:10:16.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio.egg-info/dependency_links.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      197 2023-05-10 18:10:16.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio.egg-info/entry_points.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      109 2023-05-10 18:10:16.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio.egg-info/requires.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       25 2023-05-10 18:10:16.000000 pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio.egg-info/top_level.txt
```

### Comparing `pii-extract-plg-presidio-0.2.0/LICENSE` & `pii-extract-plg-presidio-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-presidio-0.2.0/PKG-INFO` & `pii-extract-plg-presidio-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,91 @@
-Metadata-Version: 2.1
-Name: pii-extract-plg-presidio
-Version: 0.2.0
-Summary: Presidio plugin for PII detection
-Home-page: https://github.com/piisa/pii-extract-plg-presidio
-Author: Paulo Villegas
-Author-email: paulo.vllgs@gmail.com
-License: Apache
-Download-URL: https://github.com/piisa/pii-extract-plg-presidio/tarball/v0.2.0
-Description: # Pii Extractor plugin: Presidio
-        
-        ![version(https://img.shields.io/pypi/v/pii-extract-plg-presidio)](https://pypi.org/project/pii-extract-plg-presidio)
-        ![changelog(https://img.shields.io/badge/change-log-blue)](CHANGES.md)
-        ![license(https://img.shields.io/pypi/l/pii-extract-plg-presidio)](LICENSE)
-        ![build status(https://github.com/piisa/pii-extract-plg-presidio/actions/workflows/pii-extract-plg-presidio-pr.yml/badge.svg)](https://github.com/piisa/pii-extract-plg-presidio/actions)
-        
-        This repository builds a Python package that installs a pii-extract-base
-        plugin to perform PII detection for text data using the Microsoft Presidio
-        Python library.
-        
-        The name of the plugin entry point is `piisa-detectors-presidio`
-        
-        
-        ## Requirements
-        
-        The package neads
-         * at least Python 3.8
-         * the pii-data and the pii-extract-base base packages
-         * the presidio-analyzer package
-         * an NLP engine model for the desired language
-        
-        
-        ## Installation
-        
-         * Install the package: `pip install pii-extract-plg-presidio` (it will
-           automatically install its dependencies, including `presidio-analyzer`)
-         * Download the recognition model for the desired language, as instructed by
-           the presidio-analyzer installation instructions. For instance, for
-           spaCy models:
-              - English model: `python -m spacy download en_core_web_lg`
-              - Spanish model: `python -m spacy download es_core_news_md`
-         * For additional information on model specification, see customizing NLP
-           models. If custom models are used, the `nlp_config` element in the plugin
-           configuration(#configuration) must be adjusted accordingly.
-        
-        
-        ## Usage
-        
-        The package does not have any user-facing entry points (except for one console
-        script `pii-extract-presidio-info`, which provides information about its
-        capabilities).
-        
-        Instead, upon installation it defines a plugin entry point. This plugin is
-        automatically picked up by executing scripts and classes in pii-extract-base,
-        and thus its functionality is exposed to it.
-        
-        
-        ## Configuration
-        
-        The plugin is governed by a PIISA configuration file; there is one default
-        file included in the package resources. The format tag for the configuration
-        is `"piisa:config:extract-plg-presidio:main:v1`, and it has two sections:
-         * `reuse_engine`: build the engine only once, and reuse it if another task
-           object is created (default is `True`)
-         * `nlp_config` defines Presidio initialization arguments
-             - `languages`: the languages to initialize Presidio with
-        	 - `nlp_engine_name`: the NLP engine to be used
-        	 - `models`: a list of NLP models to be loaded (each item contains 
-        	    `lang_code` and `model_name`), and the available models
-         * `pii_list` defines the PIISA instances to be detected. It contains a list
-           of standard pii task descriptors; each one has an additional `extra`
-           field that contains the Presidio PII entity to be mapped to the descriptor.
-        
-        
-        ## Building
-        
-        The provided Makefile can be used to process the package:
-         * `make pkg` will build the Python package, creating a file that can be
-           installed with `pip`
-         * `make unit` will launch all unit tests (using pytest, so pytest must be
-           available)
-         * `make install` will install the package in a Python virtualenv. The
-           virtualenv will be chosen as, in this order:
-             - the one defined in the `VENV` environment variable, if it is defined
-             - if there is a virtualenv activated in the shell, it will be used
-             - otherwise, a default is chosen as `/opt/venv/pii` (it will be
-               created if it does not exist)
-        
-        
-        
-        
-Keywords: PIISA, PII
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
+# Pii Extractor plugin: Presidio
+
+[![version](https://img.shields.io/pypi/v/pii-extract-plg-presidio)](https://pypi.org/project/pii-extract-plg-presidio)
+[![changelog](https://img.shields.io/badge/change-log-blue)](CHANGES.md)
+[![license](https://img.shields.io/pypi/l/pii-extract-plg-presidio)](LICENSE)
+[![build status](https://github.com/piisa/pii-extract-plg-presidio/actions/workflows/pii-extract-plg-presidio-pr.yml/badge.svg)](https://github.com/piisa/pii-extract-plg-presidio/actions)
+
+This repository builds a Python package that installs a [pii-extract-base]
+plugin to perform PII detection for text data using the Microsoft [Presidio]
+Python library.
+
+The name of the plugin entry point is `piisa-detectors-presidio`
+
+
+## Requirements
+
+The package neads
+ * at least Python 3.8
+ * the [pii-data] and the [pii-extract-base] base packages
+ * the [presidio-analyzer] package
+ * an NLP engine model for the desired language
+
+
+## Installation
+
+ * Install the package: `pip install pii-extract-plg-presidio` (it will
+   automatically install its dependencies, including `presidio-analyzer`)
+ * Download the recognition model for the desired language(s), as instructed by
+   the [presidio-analyzer] installation instructions. The default plugin
+   [configuration file] defines three [spaCy models]:
+      - English model: `python -m spacy download en_core_web_lg`
+      - Spanish model: `python -m spacy download es_core_news_md`
+      - Italian model: `python -m spacy download it_core_news_md`
+ * For additional information on model specification, see [customizing NLP
+   models] in the Presidio documentation. If custom models are used, the
+   `nlp_config` element in the plugin [configuration file] must be
+   adjusted accordingly.
+
+
+## Usage
+
+The package does not have any user-facing entry points (except for one console
+script `pii-extract-presidio-info`, which provides information about its
+capabilities).
+
+Instead, upon installation it defines a plugin entry point. This plugin is
+automatically picked up by executing scripts and classes in [pii-extract-base],
+and thus its functionality is exposed to it.
+
+Runtime behaviour is governed by a [configuration file], which sets up what
+recognizers from Presidio will be instantiated and used. Note that the
+configuration defines which languages are available for detection, but the
+plugin can also be initialized with a _subset_ of those languages.
+
+The task created from the plugin is a standard [PII task] object, using the
+`pii_extract.build.task.MultiPiiTask` class definition. It will be called,
+as all PII task objects, with a `DocumentChunk` object containing the data to
+analyze. The chunk **must** contain language specification in its metadata, so
+that Presidio knows which language to use (unless the plugin task has been
+built with *only one* language; in that case if the chunk does not contain
+a language specification, it will use that single language).
+
+
+## Building
+
+The provided [Makefile] can be used to process the package:
+ * `make pkg` will build the Python package, creating a file that can be
+   installed with `pip`
+ * `make unit` will launch all unit tests (using [pytest], so pytest must be
+   available)
+ * `make install` will install the package in a Python virtualenv. The
+   virtualenv will be chosen as, in this order:
+     - the one defined in the `VENV` environment variable, if it is defined
+     - if there is a virtualenv activated in the shell, it will be used
+     - otherwise, a default is chosen as `/opt/venv/pii` (it will be
+       created if it does not exist)
+
+
+
+[pii-data]: https://github.com/piisa/pii-data
+[pii-extract-base]: https://github.com/piisa/pii-extract-base
+[pii task descriptors]: https://github.com/piisa/pii-extract-base/tree/main/doc/task-descriptor.md
+[Presidio]: https://microsoft.github.io/presidio/
+[presidio-analyzer]: https://microsoft.github.io/presidio/analyzer/
+[customizing NLP models]: https://microsoft.github.io/presidio/analyzer/customizing_nlp_models/
+[spaCy models]: https://spacy.io/usage/models
+[Makefile]: Makefile
+[pytest]: https://docs.pytest.org
+[default file]: src/pii_extract_plg_presidio/resources/plugin-config.json
+[configuration file]: doc/configuration.md
+[PII task]: https://github.com/piisa/pii-extract-base/blob/main/doc/task-implementation.md
```

### Comparing `pii-extract-plg-presidio-0.2.0/README.md` & `pii-extract-plg-presidio-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,98 @@
+Metadata-Version: 2.1
+Name: pii-extract-plg-presidio
+Version: 0.3.0
+Summary: Presidio plugin for PII detection
+Home-page: https://github.com/piisa/pii-extract-plg-presidio
+Download-URL: https://github.com/piisa/pii-extract-plg-presidio/tarball/v0.3.0
+Author: Paulo Villegas
+Author-email: paulo.vllgs@gmail.com
+License: Apache
+Keywords: PIISA, PII
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # Pii Extractor plugin: Presidio
 
-[![version](https://img.shields.io/pypi/v/pii-extract-plg-presidio)](https://pypi.org/project/pii-extract-plg-presidio)
-[![changelog](https://img.shields.io/badge/change-log-blue)](CHANGES.md)
-[![license](https://img.shields.io/pypi/l/pii-extract-plg-presidio)](LICENSE)
-[![build status](https://github.com/piisa/pii-extract-plg-presidio/actions/workflows/pii-extract-plg-presidio-pr.yml/badge.svg)](https://github.com/piisa/pii-extract-plg-presidio/actions)
+![version(https://img.shields.io/pypi/v/pii-extract-plg-presidio)](https://pypi.org/project/pii-extract-plg-presidio)
+![changelog(https://img.shields.io/badge/change-log-blue)](CHANGES.md)
+![license(https://img.shields.io/pypi/l/pii-extract-plg-presidio)](LICENSE)
+![build status(https://github.com/piisa/pii-extract-plg-presidio/actions/workflows/pii-extract-plg-presidio-pr.yml/badge.svg)](https://github.com/piisa/pii-extract-plg-presidio/actions)
 
-This repository builds a Python package that installs a [pii-extract-base]
-plugin to perform PII detection for text data using the Microsoft [Presidio]
+This repository builds a Python package that installs a pii-extract-base
+plugin to perform PII detection for text data using the Microsoft Presidio
 Python library.
 
 The name of the plugin entry point is `piisa-detectors-presidio`
 
 
 ## Requirements
 
 The package neads
  * at least Python 3.8
- * the [pii-data] and the [pii-extract-base] base packages
- * the [presidio-analyzer] package
+ * the pii-data and the pii-extract-base base packages
+ * the presidio-analyzer package
  * an NLP engine model for the desired language
 
 
 ## Installation
 
  * Install the package: `pip install pii-extract-plg-presidio` (it will
    automatically install its dependencies, including `presidio-analyzer`)
- * Download the recognition model for the desired language, as instructed by
-   the [presidio-analyzer] installation instructions. For instance, for
-   [spaCy models]:
+ * Download the recognition model for the desired language(s), as instructed by
+   the presidio-analyzer installation instructions. The default plugin
+   configuration file defines three spaCy models:
       - English model: `python -m spacy download en_core_web_lg`
       - Spanish model: `python -m spacy download es_core_news_md`
- * For additional information on model specification, see [customizing NLP
-   models]. If custom models are used, the `nlp_config` element in the plugin
-   [configuration](#configuration) must be adjusted accordingly.
+      - Italian model: `python -m spacy download it_core_news_md`
+ * For additional information on model specification, see customizing NLP
+   models in the Presidio documentation. If custom models are used, the
+   `nlp_config` element in the plugin configuration file must be
+   adjusted accordingly.
 
 
 ## Usage
 
 The package does not have any user-facing entry points (except for one console
 script `pii-extract-presidio-info`, which provides information about its
 capabilities).
 
 Instead, upon installation it defines a plugin entry point. This plugin is
-automatically picked up by executing scripts and classes in [pii-extract-base],
+automatically picked up by executing scripts and classes in pii-extract-base,
 and thus its functionality is exposed to it.
 
-
-## Configuration
-
-The plugin is governed by a PIISA configuration file; there is one [default
-file] included in the package resources. The format tag for the configuration
-is `"piisa:config:extract-plg-presidio:main:v1`, and it has two sections:
- * `reuse_engine`: build the engine only once, and reuse it if another task
-   object is created (default is `True`)
- * `nlp_config` defines Presidio initialization arguments
-     - `languages`: the languages to initialize Presidio with
-	 - `nlp_engine_name`: the NLP engine to be used
-	 - `models`: a list of NLP models to be loaded (each item contains 
-	    `lang_code` and `model_name`), and the available models
- * `pii_list` defines the PIISA instances to be detected. It contains a list
-   of standard [pii task descriptors]; each one has an additional `extra`
-   field that contains the Presidio PII entity to be mapped to the descriptor.
+Runtime behaviour is governed by a configuration file, which sets up what
+recognizers from Presidio will be instantiated and used. Note that the
+configuration defines which languages are available for detection, but the
+plugin can also be initialized with a _subset_ of those languages.
+
+The task created from the plugin is a standard PII task object, using the
+`pii_extract.build.task.MultiPiiTask` class definition. It will be called,
+as all PII task objects, with a `DocumentChunk` object containing the data to
+analyze. The chunk **must** contain language specification in its metadata, so
+that Presidio knows which language to use (unless the plugin task has been
+built with *only one* language; in that case if the chunk does not contain
+a language specification, it will use that single language).
 
 
 ## Building
 
-The provided [Makefile] can be used to process the package:
+The provided Makefile can be used to process the package:
  * `make pkg` will build the Python package, creating a file that can be
    installed with `pip`
- * `make unit` will launch all unit tests (using [pytest], so pytest must be
+ * `make unit` will launch all unit tests (using pytest, so pytest must be
    available)
  * `make install` will install the package in a Python virtualenv. The
    virtualenv will be chosen as, in this order:
      - the one defined in the `VENV` environment variable, if it is defined
      - if there is a virtualenv activated in the shell, it will be used
      - otherwise, a default is chosen as `/opt/venv/pii` (it will be
        created if it does not exist)
 
 
 
-[pii-data]: https://github.com/piisa/pii-data
-[pii-extract-base]: https://github.com/piisa/pii-extract-base
-[pii task descriptors]: https://github.com/piisa/pii-extract-base/tree/main/doc/task-descriptor.md
-[Presidio]: https://microsoft.github.io/presidio/
-[presidio-analyzer]: https://microsoft.github.io/presidio/analyzer/
-[customizing NLP models]: https://microsoft.github.io/presidio/analyzer/customizing_nlp_models/
-[spaCy models]: https://spacy.io/usage/models
-[Makefile]: Makefile
-[pytest]: https://docs.pytest.org
-[default file]: src/pii_extract_plg_presidio/resources/plugin-config.json
```

### Comparing `pii-extract-plg-presidio-0.2.0/setup.py` & `pii-extract-plg-presidio-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/analyzer.py` & `pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/task/analyzer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,69 @@
 """
 Create a Presidio analyzer engine
 """
 
-from importlib.metadata import version
 
-from typing import Dict, List
+from typing import Dict
 
 from pii_extract.helper.logger import PiiLogger
 
 from presidio_analyzer.nlp_engine import NlpEngineProvider
 from presidio_analyzer import AnalyzerEngine
 
-from . import defs
+from .. import defs
+from .utils import presidio_languages
 
 
 # Cache for engine reuse
 ENGINE_CACHE = {}
 
 
-def presidio_version() -> str:
-    """
-    Return the version of the Presidio package
-    """
-    return version("presidio_analyzer")
-
-
 def presidio_analyzer(config: Dict,
                       logger: PiiLogger = None) -> AnalyzerEngine:
     """
     Create a Presidio AnalyzerEngine object.
     Will reuse an object with the same configuration if it's in the cache
     and `reuse_engine` is True (which is its default value)
     """
     # Fetch NLP engine configuration. Keep only the language models we'll use
-    eng = config.get(defs.CFG_ENGINE)
-    lang = eng.get("languages", [])
-    if isinstance(lang, str):
-        lang = [lang]
-    langset = set(lang)
+    langset = presidio_languages(config)
+    config = config.get(defs.CFG_ENGINE)
+
+    # Prepare a configuration for the Presidio Analyzer
     nlp_config = {
-        "nlp_engine_name": eng.get("nlp_engine_name"),
-        "models": [m for m in eng.get("models")
+        "nlp_engine_name": config.get("nlp_engine_name"),
+        "models": [m for m in config.get("models")
                    if not langset or m["lang_code"] in langset]
     }
 
     if logger:
         logger(".. Presidio NLP engine: %s", nlp_config.get("nlp_engine_name"))
         logger(".. Presidio NLP models: %s", nlp_config.get("models"))
 
-    # Reuse engine if it has the same parameters
+    # Reuse the engine if we have one with the same parameters
     reuse = config.get(defs.CFG_REUSE, True)
     if reuse:
-        key_l = "-".join(sorted(lang)) if lang else "-"
+        key_l = "-".join(sorted(langset)) if langset else "-"
         key_m = (m["lang_code"] + ":" + m["model_name"]
                  for m in nlp_config["models"])
         key = [key_l, nlp_config['nlp_engine_name'], '-'.join(sorted(key_m))]
         key = '/'.join(key)
         engine = ENGINE_CACHE.get(key)
         if key in ENGINE_CACHE:
-            logger(".. Reusing Presidio NLP engine")
+            if logger:
+                logger(".. Reusing Presidio NLP engine")
             return engine
 
-
     # Create an NLP engine, according to the configuration
-    logger(".. Creating Presidio NLP engine")
+    if logger:
+        logger(".. Creating Presidio NLP engine")
     provider = NlpEngineProvider(nlp_configuration=nlp_config)
     nlp_engine = provider.create_engine()
 
     # Set up the Presidio Analyzer engine
-    engine = AnalyzerEngine(supported_languages=lang or None,
-                            nlp_engine=nlp_engine, **config[defs.CFG_PARAMS])
+    extra_params = config.get(defs.CFG_PARAMS, {})
+    engine = AnalyzerEngine(supported_languages=list(langset) or None,
+                            nlp_engine=nlp_engine, **extra_params)
     if reuse:
         ENGINE_CACHE[key] = engine
     return engine
```

### Comparing `pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/app/info.py` & `pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/app/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 from pii_extract import VERSION as VERSION_EXTRACT
 from pii_extract.gather.parser import parse_task_descriptor, RawTaskDefaults
 from pii_extract.build.collection.task_collection import filter_piid
 from pii_extract.build.build import build_task
 
 from .. import VERSION
 from ..plugin_loader import load_presidio_plugin_config
-from ..task import presidio_version, presidio_analyzer, PresidioTaskCollector
+from ..analyzer import presidio_version, presidio_analyzer
+from ..task import PresidioTaskCollector
 
 
 class Processor:
 
     def __init__(self, args: argparse.Namespace, debug: bool = False):
         self.args = args
         self.debug = debug
 
 
     def _init_presidio(self):
         config = load_presidio_plugin_config(self.args.config)
         try:
-            return presidio_analyzer(config, self.args.lang)
+            return presidio_analyzer(config)
         except Exception as e:
             raise ProcException("cannot create Presidio Analyzer engine: {}",
                                 e) from e
 
 
     def proc_version(self, out: TextIO):
         """
```

### Comparing `pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/plugin_loader.py` & `pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/plugin_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pathlib import Path
 
 from typing import Dict, Iterable, Union, List
 
 from pii_data.helper.exception import ConfigException
 from pii_data.helper.config import load_single_config
-from pii_extract.build.collection.task_collection import ensure_enum
+from pii_extract.gather.collection.utils import ensure_enum
 
 from . import VERSION, defs
 from .task import PresidioTaskCollector
 
 # Elements in the PIISA presidio config to read
 CFG_ELEM = defs.CFG_REUSE, defs.CFG_ENGINE, defs.CFG_PARAMS, defs.CFG_MAP
 
@@ -51,15 +51,15 @@
 
     def __init__(self, config: Union[str, Dict] = None, debug: bool = False,
                  languages: List[str] = None, **kwargs):
         """
           :param config: either a configuration for the plugin, or a filename
             containing that configuration
           :param debug: activate debug mode
-          :param languages: languages to load in the Presidio analyzer engine
+          :param languages: restrict the Presidio config to those languages
         """
         self.cfg = load_presidio_plugin_config(config)
         self.obj = PresidioTaskCollector(self.cfg, languages=languages,
                                          debug=debug)
 
 
     def __repr__(self) -> str:
```

### Comparing `pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/resources/plugin-config.json` & `pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/resources/plugin-config.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.880026455026455%*

 * *Differences: {"'nlp_config'": "{'models': {insert: [(2, OrderedDict([('lang_code', 'it'), ('model_name', "*

 * *                 "'it_core_news_md')]))]}, delete: ['languages']}",*

 * * "'pii_list'": "{0: {'lang': {insert: [(2, 'it')]}}, 1: {'lang': {insert: [(2, 'it')]}}, 2: "*

 * *               "{'type': 'LOCATION', 'subtype': 'place', 'lang': {insert: [(2, 'it')]}}, insert: "*

 * *               "[(4, OrderedDict([('type', 'GOV_ID'), ('subtype', 'US Driver License'), ('lang', "*

 * *               "'en'), ('country', 'us'), ('method', 'weak […]*

```diff
@@ -1,76 +1,99 @@
 {
     "format": "piisa:config:pii-extract-plg-presidio:main:v1",
     "nlp_config": {
-        "languages": [
-            "en",
-            "es"
-        ],
         "models": [
             {
                 "lang_code": "en",
                 "model_name": "en_core_web_lg"
             },
             {
                 "lang_code": "es",
                 "model_name": "es_core_news_md"
+            },
+            {
+                "lang_code": "it",
+                "model_name": "it_core_news_md"
             }
         ],
         "nlp_engine_name": "spacy"
     },
     "pii_list": [
         {
             "extra": {
                 "presidio": "PERSON"
             },
             "lang": [
                 "en",
-                "es"
+                "es",
+                "it"
             ],
             "method": "model",
             "type": "PERSON"
         },
         {
             "extra": {
                 "presidio": "NRP"
             },
             "lang": [
                 "en",
-                "es"
+                "es",
+                "it"
             ],
             "method": "model",
             "type": "NORP"
         },
         {
             "extra": {
                 "presidio": "LOCATION"
             },
             "lang": [
                 "en",
-                "es"
+                "es",
+                "it"
             ],
             "method": "model",
-            "subtype": "LOCATION",
-            "type": "OTHER"
+            "subtype": "place",
+            "type": "LOCATION"
         },
         {
             "country": "us",
             "extra": {
                 "presidio": "US_PASSPORT"
             },
             "lang": "en",
             "method": "weak-regex,context",
             "subtype": "US passport",
             "type": "GOV_ID"
         },
         {
+            "country": "us",
+            "extra": {
+                "presidio": "US_DRIVER_LICENSE"
+            },
+            "lang": "en",
+            "method": "weak-regex,context",
+            "subtype": "US Driver License",
+            "type": "GOV_ID"
+        },
+        {
             "country": "it",
             "extra": {
                 "presidio": "IT_FISCAL_CODE"
             },
             "lang": "it",
             "method": "regex,checksum,context",
             "subtype": "Italian Codice Fiscale",
             "type": "GOV_ID"
+        },
+        {
+            "country": "it",
+            "extra": {
+                "presidio": "IT_IDENTITY_CARD"
+            },
+            "lang": "it",
+            "method": "weak-regex,context",
+            "subtype": "Italian identity card",
+            "type": "GOV_ID"
         }
     ]
 }
```

### Comparing `pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio/task.py` & `pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio/task/task.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,48 +6,24 @@
 from operator import attrgetter
 from collections import defaultdict
 
 from pii_data.helper.exception import ProcException, ConfigException
 from pii_data.types import PiiEntity, PiiEntityInfo
 from pii_data.types.doc import DocumentChunk
 from pii_extract.build.task import BaseMultiPiiTask
-from pii_extract.helper.utils import taskd_field, union_sets
+from pii_extract.helper.utils import taskd_field
 from pii_extract.helper.logger import PiiLogger
 
 from typing import Iterable, Dict, List
 
-from . import VERSION, defs
-from .analyzer import presidio_version, presidio_analyzer
+from .. import VERSION
+from .utils import presidio_version
+from .analyzer import presidio_analyzer
 
 
-# ---------------------------------------------------------------------
-
-
-def pii_list(config: Dict, lang: List[str]) -> Dict:
-    """
-    Restrict the Presidio entity mapping to a given set of languages
-    """
-    langset = set([lang] if isinstance(lang, str) else lang) if lang else None
-    piimap = {}
-    for p in config[defs.CFG_MAP]:
-
-        key = f"{p['type']}/{p.get('subtype')}"
-        lang = p.get("lang")
-
-        # Remove entries with language defined as None
-        if lang is None:
-            piimap.pop(key, None)
-            continue
-        elif langset and not taskd_field(p, "lang") & langset:
-            continue    # skip if we've been given a precise set of languages
-
-        piimap[key] = p
-
-    return list(piimap.values())
-
 
 def einfo(p: Dict) -> PiiEntityInfo:
     """
     Create an entity info object from a PII descriptor dict
     """
     return PiiEntityInfo(p["pii"], p.get("lang"), p.get("country"),
                          p.get("subtype"))
@@ -62,141 +38,99 @@
     """
     pii_source = "microsoft:presidio"
     pii_name = "Presidio wrapper"
     pii_version = presidio_version
 
 
     def __init__(self, task: Dict, pii: List[Dict], cfg: Dict,
-                 log: PiiLogger, all_lang: List[str] = None, **kwargs):
+                 log: PiiLogger, **kwargs):
         """
           :param task: the PII task info dict
           :param pii: the list of descriptors for the PII entities to include
           :param cfg: the plugin configuration
           :param log: a logger object
-          :param all_lang: all languages the analyzer should be initialized for
         """
+        #print("\nPresidioTask INIT", pii)
 
-        # Use the "extra" field in each PII descriptor to build the map of
-        # Presidio entities to PIISA entities (by language)
-        self.ent_map = defaultdict(dict)
+        # Use the "extra" field in the PII dict to build a map (by language)
+        # of Presidio entities to PIISA entities
+        # (before parent constructor, which will strip away "extra" fields)
+        self._ent_map = defaultdict(dict)
+        pii_lang = set()
         if isinstance(pii, dict):
             pii = [pii]
         for p in pii:
             try:
-                langlist = p["lang"]
-                if isinstance(langlist, str):
-                    langlist = [langlist]
-                for lang in langlist:
-                    self.ent_map[lang][p["extra"]["presidio"]] = einfo(p)
+                langset = taskd_field(p, "lang")
+                pii_lang.update(langset)
+                for lang in langset:
+                    self._ent_map[lang][p["extra"]["presidio"]] = einfo(p)
             except KeyError as e:
                 raise ConfigException("invalid Presidio config: missing field '{}' in: {}", e, p)
 
-        # Now call the parent constructor
+        # Initialize
         super().__init__(task=task, pii=pii)
-
         self._log = log
 
-        # Decide is the default language (if we have a single one)
-        if all_lang is None:
-            all_lang = union_sets(taskd_field(t, "lang") for t in pii)
-        self.lang = all_lang[0] if len(all_lang) == 1 else None
+        # Decide a default language for this task (possible if we have only one)
+        self.lang = pii_lang.pop() if len(pii_lang) == 1 else None
         self._log(".. PresidioTask (%s): lang=%s tasks=#%d", VERSION,
-                  self.lang or all_lang, len(pii))
+                  self.lang, len(pii))
 
         # Set up the Presidio Analyzer engine
         try:
             self.analyzer = presidio_analyzer(cfg, log)
         except Exception as e:
             raise ProcException("cannot create Presidio Analyzer engine: {}",
                                 e) from e
 
         # Check that all Presidio entities we want are actually supported
         entities = set(self.analyzer.get_supported_entities())
-        missing = {pname for edict in self.ent_map.values() for pname in edict
+        missing = {pname for edict in self._ent_map.values() for pname in edict
                    if pname not in entities}
         if missing:
             raise ProcException("recognizer for {} not found in Presidio",
                                 missing)
 
 
     def __repr__(self) -> str:
         return f"<PresidioTask #{len(self)}>"
 
 
     def __len__(self) -> int:
-        return sum(len(k) for k in self.ent_map.values())
+        return sum(len(k) for k in self._ent_map.values())
 
 
     def find(self, chunk: DocumentChunk) -> Iterable[PiiEntity]:
         """
         Perform PII detection on a document chunk
         """
         # Decide the language we'll pass to Presidio: chunk language or default
         ctx = chunk.context or {}
         lang = ctx.get("lang", self.lang)
         if lang is None:
             raise ProcException("Presidio task exception: no language defined in task or document chunk")
-        elif lang not in self.ent_map:
+        elif lang not in self._ent_map:
             raise ProcException("Presidio task exception: no tasks for lang: {}",
                                 lang)
 
         # Take the entity map for our language
-        entity_map = self.ent_map[lang]
+        entity_map = self._ent_map[lang]
 
         # Call Presidio analyzer to get results
         try:
             results = self.analyzer.analyze(text=chunk.data, language=lang,
                                             entities=list(entity_map))
         except Exception as e:
             raise ProcException("Presidio exception: {}: {}", type(e).__name__,
                                 e) from e
 
         self._log("... Presidio results: %s", results if results else "NONE",
                   level=logging.DEBUG)
-        #print("\n**** PRESIDIO", lang, list(self.ent_map), chunk.data, "=>", results, sep="\n")
+        #print("\n**** PRESIDIO", lang, list(self._ent_map), chunk.data, "=>", results, sep="\n")
 
         # Convert results into PiEntity objects
         for r in sorted(results, key=attrgetter("start")):
             v = chunk.data[r.start:r.end]
             process = {"stage": "detection", "score": r.score}
             yield PiiEntity(entity_map[r.entity_type],
                             v, chunk.id, r.start, process=process)
-
-
-# ---------------------------------------------------------------------
-
-class PresidioTaskCollector:
-    """
-    The class used by the plugin loader to produce the Presidio task
-    """
-
-    def __init__(self, cfg: Dict, languages: List[str] = None,
-                 debug: bool = True):
-        self.cfg = cfg
-        self.lang = languages
-        self._log = PiiLogger(__name__, debug)
-        self._log(".. Presidio task collector: init (lang=%s)", languages)
-
-
-    def gather_tasks(self, lang: str = None) -> Iterable[Dict]:
-        """
-        Return an iterable of available Detector tasks
-        (in this case it is a single multi-task)
-        """
-        if not lang:
-            lang = self.lang
-        self._log(".. Presidio gather tasks for lang=%s", lang)
-
-        # The configuration to pass to to the task descriptor
-        cfg = {k: self.cfg[k] for k in (defs.CFG_ENGINE, defs.CFG_PARAMS)}
-
-        # Prepare the raw task descriptor
-        task = {
-            "class": "PiiTask",
-            "source": defs.TASK_SOURCE,
-            "version": VERSION,
-            "doc": defs.TASK_DESCRIPTION,
-            "task": PresidioTask,
-            "kwargs": {"cfg": cfg, "log": self._log, "all_lang": self.lang},
-            "pii": pii_list(self.cfg, self.lang)
-        }
-        yield task
```

### Comparing `pii-extract-plg-presidio-0.2.0/src/pii_extract_plg_presidio.egg-info/SOURCES.txt` & `pii-extract-plg-presidio-0.3.0/src/pii_extract_plg_presidio.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 src/pii_extract_plg_presidio/__init__.py
-src/pii_extract_plg_presidio/analyzer.py
 src/pii_extract_plg_presidio/defs.py
 src/pii_extract_plg_presidio/plugin_loader.py
-src/pii_extract_plg_presidio/task.py
 src/pii_extract_plg_presidio.egg-info/PKG-INFO
 src/pii_extract_plg_presidio.egg-info/SOURCES.txt
 src/pii_extract_plg_presidio.egg-info/dependency_links.txt
 src/pii_extract_plg_presidio.egg-info/entry_points.txt
 src/pii_extract_plg_presidio.egg-info/requires.txt
 src/pii_extract_plg_presidio.egg-info/top_level.txt
 src/pii_extract_plg_presidio/app/__init__.py
 src/pii_extract_plg_presidio/app/info.py
-src/pii_extract_plg_presidio/resources/plugin-config.json
+src/pii_extract_plg_presidio/resources/plugin-config.json
+src/pii_extract_plg_presidio/task/__init__.py
+src/pii_extract_plg_presidio/task/analyzer.py
+src/pii_extract_plg_presidio/task/collector.py
+src/pii_extract_plg_presidio/task/task.py
+src/pii_extract_plg_presidio/task/utils.py
```

