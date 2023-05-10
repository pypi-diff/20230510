# Comparing `tmp/pii-transform-0.4.2.tar.gz` & `tmp/pii-transform-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pii-transform-0.4.2.tar", last modified: Wed Mar 22 23:18:59 2023, max compression
+gzip compressed data, was "pii-transform-0.5.0.tar", last modified: Wed May 10 18:10:32 2023, max compression
```

## Comparing `pii-transform-0.4.2.tar` & `pii-transform-0.5.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.545236 pii-transform-0.4.2/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-transform-0.4.2/LICENSE
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       79 2023-01-22 18:11:59.000000 pii-transform-0.4.2/MANIFEST.in
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2105 2023-03-22 23:18:59.545236 pii-transform-0.4.2/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1594 2023-03-17 20:33:13.000000 pii-transform-0.4.2/README.md
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       61 2023-03-20 21:20:34.000000 pii-transform-0.4.2/requirements.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-03-22 23:18:59.545236 pii-transform-0.4.2/setup.cfg
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2701 2023-03-17 20:33:13.000000 pii-transform-0.4.2/setup.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.541236 pii-transform-0.4.2/src/
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.541236 pii-transform-0.4.2/src/pii_transform/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       18 2023-03-22 23:18:38.000000 pii-transform-0.4.2/src/pii_transform/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.541236 pii-transform-0.4.2/src/pii_transform/api/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-01-22 18:11:59.000000 pii-transform-0.4.2/src/pii_transform/api/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.541236 pii-transform-0.4.2/src/pii_transform/api/e2e/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      153 2023-03-22 22:35:17.000000 pii-transform-0.4.2/src/pii_transform/api/e2e/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4396 2023-03-20 21:20:34.000000 pii-transform-0.4.2/src/pii_transform/api/e2e/document.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4404 2023-03-22 23:18:38.000000 pii-transform-0.4.2/src/pii_transform/api/e2e/multilang.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2985 2023-03-22 22:35:17.000000 pii-transform-0.4.2/src/pii_transform/api/e2e/textchunk.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3314 2023-03-17 20:33:13.000000 pii-transform-0.4.2/src/pii_transform/api/transform.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.541236 pii-transform-0.4.2/src/pii_transform/app/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-22 18:11:59.000000 pii-transform-0.4.2/src/pii_transform/app/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      397 2023-01-25 18:43:02.000000 pii-transform-0.4.2/src/pii_transform/app/chunk.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      662 2023-03-22 22:58:31.000000 pii-transform-0.4.2/src/pii_transform/app/multi.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3119 2023-01-24 22:48:30.000000 pii-transform-0.4.2/src/pii_transform/app/process.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2859 2023-01-22 18:11:59.000000 pii-transform-0.4.2/src/pii_transform/app/transform.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      128 2023-03-17 20:33:13.000000 pii-transform-0.4.2/src/pii_transform/defs.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.541236 pii-transform-0.4.2/src/pii_transform/helper/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       47 2023-01-22 18:11:59.000000 pii-transform-0.4.2/src/pii_transform/helper/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1810 2023-01-23 19:30:15.000000 pii-transform-0.4.2/src/pii_transform/helper/logger.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3734 2023-03-17 20:33:13.000000 pii-transform-0.4.2/src/pii_transform/helper/placeholder.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     5059 2023-03-17 20:33:13.000000 pii-transform-0.4.2/src/pii_transform/helper/substitution.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     5078 2023-03-17 20:33:13.000000 pii-transform-0.4.2/src/pii_transform/helper/synthetic.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.541236 pii-transform-0.4.2/src/pii_transform/resources/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1412 2023-03-17 20:33:13.000000 pii-transform-0.4.2/src/pii_transform/resources/placeholder.json
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       73 2023-03-05 21:06:11.000000 pii-transform-0.4.2/src/pii_transform/resources/transform.json
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 23:18:59.541236 pii-transform-0.4.2/src/pii_transform.egg-info/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2105 2023-03-22 23:18:59.000000 pii-transform-0.4.2/src/pii_transform.egg-info/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1025 2023-03-22 23:18:59.000000 pii-transform-0.4.2/src/pii_transform.egg-info/SOURCES.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-03-22 23:18:59.000000 pii-transform-0.4.2/src/pii_transform.egg-info/dependency_links.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      113 2023-03-22 23:18:59.000000 pii-transform-0.4.2/src/pii_transform.egg-info/entry_points.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       82 2023-03-22 23:18:59.000000 pii-transform-0.4.2/src/pii_transform.egg-info/requires.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       14 2023-03-22 23:18:59.000000 pii-transform-0.4.2/src/pii_transform.egg-info/top_level.txt
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.893382 pii-transform-0.5.0/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-transform-0.5.0/LICENSE
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       79 2023-01-22 18:11:59.000000 pii-transform-0.5.0/MANIFEST.in
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2114 2023-05-10 18:10:32.893382 pii-transform-0.5.0/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1938 2023-05-10 18:08:53.000000 pii-transform-0.5.0/README.md
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       61 2023-05-10 18:08:53.000000 pii-transform-0.5.0/requirements.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-05-10 18:10:32.893382 pii-transform-0.5.0/setup.cfg
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2765 2023-05-10 18:08:53.000000 pii-transform-0.5.0/setup.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.889382 pii-transform-0.5.0/src/
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.889382 pii-transform-0.5.0/src/pii_transform/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       18 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.893382 pii-transform-0.5.0/src/pii_transform/api/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-01-22 18:11:59.000000 pii-transform-0.5.0/src/pii_transform/api/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.893382 pii-transform-0.5.0/src/pii_transform/api/e2e/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      243 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/api/e2e/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       90 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/api/e2e/defs.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4792 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/api/e2e/document.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     6076 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/api/e2e/multilang.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3480 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/api/e2e/textchunk.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3314 2023-03-30 21:45:31.000000 pii-transform-0.5.0/src/pii_transform/api/transform.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.893382 pii-transform-0.5.0/src/pii_transform/app/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-22 18:11:59.000000 pii-transform-0.5.0/src/pii_transform/app/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      526 2023-05-10 07:37:04.000000 pii-transform-0.5.0/src/pii_transform/app/chunk.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4569 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/app/multi.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3116 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/app/process.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2859 2023-01-22 18:11:59.000000 pii-transform-0.5.0/src/pii_transform/app/transform.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      128 2023-03-17 20:33:13.000000 pii-transform-0.5.0/src/pii_transform/defs.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.893382 pii-transform-0.5.0/src/pii_transform/helper/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       47 2023-01-22 18:11:59.000000 pii-transform-0.5.0/src/pii_transform/helper/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1810 2023-01-23 19:30:15.000000 pii-transform-0.5.0/src/pii_transform/helper/logger.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1018 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/helper/misc.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3965 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/helper/placeholder.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     5655 2023-05-10 18:08:53.000000 pii-transform-0.5.0/src/pii_transform/helper/substitution.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     5078 2023-04-22 10:24:37.000000 pii-transform-0.5.0/src/pii_transform/helper/synthetic.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.893382 pii-transform-0.5.0/src/pii_transform/resources/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1412 2023-03-17 20:33:13.000000 pii-transform-0.5.0/src/pii_transform/resources/placeholder.json
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       73 2023-03-05 21:06:11.000000 pii-transform-0.5.0/src/pii_transform/resources/transform.json
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:10:32.893382 pii-transform-0.5.0/src/pii_transform.egg-info/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2114 2023-05-10 18:10:32.000000 pii-transform-0.5.0/src/pii_transform.egg-info/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1092 2023-05-10 18:10:32.000000 pii-transform-0.5.0/src/pii_transform.egg-info/SOURCES.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-05-10 18:10:32.000000 pii-transform-0.5.0/src/pii_transform.egg-info/dependency_links.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      161 2023-05-10 18:10:32.000000 pii-transform-0.5.0/src/pii_transform.egg-info/entry_points.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       82 2023-05-10 18:10:32.000000 pii-transform-0.5.0/src/pii_transform.egg-info/requires.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       14 2023-05-10 18:10:32.000000 pii-transform-0.5.0/src/pii_transform.egg-info/top_level.txt
```

### Comparing `pii-transform-0.4.2/LICENSE` & `pii-transform-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pii-transform-0.4.2/PKG-INFO` & `pii-transform-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 Metadata-Version: 2.1
 Name: pii-transform
-Version: 0.4.2
+Version: 0.5.0
 Summary: Transform recognized PII instances in a document
 Home-page: https://github.com/piisa/pii-transform
+Download-URL: https://github.com/piisa/pii-transform/tarball/v0.5.0
 Author: Paulo Villegas
 Author-email: paulo.vllgs@gmail.com
 License: Apache
-Download-URL: https://github.com/piisa/pii-transform/tarball/v0.4.2
-Description: # pii-transform
-        
-        
-        This package takes a source document, a collection of detected PII instances,
-        and transforms the document by replacing the PII instances in the document
-        with a different representation.
-        
-        The type of substitution done is defined by transformation policies.
-        
-        
-        ## Command-line scripts
-        
-        The package provides two console scripts:
-        
-         * `pii-transform` loads a source document & a collection of detected PII, 
-           and produces a transformed document following the required policies.
-         * `pii-process` is a full end-to-end script:
-            - load a document, from among the formats supported by `pii-preprocess`
-        	- detects PII instances, according to `pii-extract` and its installed
-        	  plugins
-            - transforms the detected PII instances (according to the indicated policy)
-        	  and writes out the transformed documennt
-        	  
-        	  
-        Note that `pii-process` will need additional packages to be present:
-         * `pii-preprocess`
-         * `pii-extract-base`, together with any available detection plugins, e.g.
-           `pii-extract-plg-regex`
-        
-        
-        ## API
-        
-        The same functionality provided by the command-line scripts can also be
-        accessed via a Python API
-        
-        
-        
 Keywords: PIISA, PII
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# pii-transform
+
+
+This package takes a source document, a collection of detected PII instances,
+and transforms the document by replacing the PII instances in the document
+with a different representation.
+
+The type of substitution done is defined by transformation policies.
+
+
+## Command-line scripts
+
+The package provides three console scripts:
+
+ * `pii-transform` loads a source document & a collection of already-detected
+   PII, and produces a transformed document following the required policies.
+ * `pii-process` is a full end-to-end script:
+    - load a document, from among the formats supported by `pii-preprocess`
+	- detects PII instances, according to `pii-extract` and its installed
+	  plugins
+    - transforms the detected PII instances (according to the indicated policy)
+	  and writes out the transformed documennt
+ * `pii-process-jsonl` is also a full end-to-end script; this one reads
+   JSONL files and processes each line as a separate text buffer (possibly in
+   different languages), producing a transformed JSONL document
+	  
+	  
+Note that `pii-process` & `pii-process-jsonl` will need additional packages
+to be installed:
+ * `pii-preprocess` (only for `pii-process`)
+ * `pii-extract-base`, together with any available detection plugins, e.g.
+   `pii-extract-plg-regex` and/or `pii-extract-plg-presidio`
+
+
+## API
+
+The same functionality provided by the command-line scripts can also be
+accessed via a Python API
+
+
```

### Comparing `pii-transform-0.4.2/README.md` & `pii-transform-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -10,33 +10,38 @@
 with a different representation.
 
 The type of substitution done is defined by [transformation policies].
 
 
 ## Command-line scripts
 
-The package provides two console scripts:
+The package provides three console scripts:
 
- * `pii-transform` loads a source document & a collection of detected PII, 
-   and produces a transformed document following the required policies.
+ * `pii-transform` loads a source document & a collection of already-detected
+   PII, and produces a transformed document following the required policies.
  * `pii-process` is a full end-to-end script:
     - load a document, from among the formats supported by `pii-preprocess`
 	- detects PII instances, according to `pii-extract` and its installed
 	  plugins
     - transforms the detected PII instances (according to the indicated policy)
 	  and writes out the transformed documennt
+ * [`pii-process-jsonl`] is also a full end-to-end script; this one reads
+   JSONL files and processes each line as a separate text buffer (possibly in
+   different languages), producing a transformed JSONL document
 	  
 	  
-Note that `pii-process` will need additional packages to be present:
- * `pii-preprocess`
+Note that `pii-process` & `pii-process-jsonl` will need additional packages
+to be installed:
+ * `pii-preprocess` (only for `pii-process`)
  * `pii-extract-base`, together with any available detection plugins, e.g.
-   `pii-extract-plg-regex`
+   `pii-extract-plg-regex` and/or `pii-extract-plg-presidio`
 
 
 ## API
 
 The same functionality provided by the command-line scripts can also be
 accessed via a [Python API]
 
+
 [transformation policies]: doc/policies.md
 [Python API]: doc/api.md
-
+[`pii-process-jsonl`]: doc/jsonl.md
```

### Comparing `pii-transform-0.4.2/setup.py` & `pii-transform-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     },
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
     entry_points={
         "console_scripts": [
             "pii-transform = pii_transform.app.transform:main",
             "pii-process = pii_transform.app.process:main",
+            "pii-process-jsonl = pii_transform.app.multi:main",
         ]
     },
     include_package_data=False,
     package_data={
         'pii_transform': ['resources/*.json'],
     },
     # Post-install hooks
```

### Comparing `pii-transform-0.4.2/src/pii_transform/api/e2e/document.py` & `pii-transform-0.5.0/src/pii_transform/api/e2e/document.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 End-to-end PII processing for documents
 """
 
 import sys
 
 from typing import List, Union, Dict
 
+from packaging.version import Version
+
 from pii_data.helper.io import openfile
 from pii_data.helper.config import load_config, TYPE_CONFIG_LIST
 from pii_data.helper.exception import InvArgException, ProcException
 from ..transform import PiiTransformer
+from . import defs
 try:
     from pii_data.helper.logger import PiiLogger
 except ImportError:
     from ...helper.logger import PiiLogger
 try:
     from pii_preprocess.loader import DocumentLoader
     from pii_extract.api import PiiProcessor
     from pii_extract.api.file import piic_format, print_stats, print_tasks
-    from pii_extract.build.collection import TYPE_TASKENUM
-    MISSING_LIBS = None
+    from pii_extract.gather.collection import TYPE_TASKENUM
+    from pii_extract import VERSION as PII_EXTRACT_VERSION
+    MISSING_MOD = None
 except ImportError as e:
-    MISSING_LIBS = str(e)
+    MISSING_MOD = str(e)
+    DocumentLoader = None
+    PiiProcessor = None
     TYPE_TASKENUM = List
+    PII_EXTRACT_VERSION = None
 
 
 def format_policy(name: str, param: str = None) -> Dict:
     """
     Format a policy
       :param name: policy name
       :param param: policy parameter, for policies that require it
@@ -65,16 +72,20 @@
      :param tasks: restrict to an specific set of detection tasks
      :param chunk_context: add contexts to chunks when detecting
      :param default_policy: default transform policy
      :param verbose: verbosity level, if > 0 print out progress messages
      :param show_tasks: print out the list of built tasks
      :param show_stats: print out statistics on detected PII
     """
-    if MISSING_LIBS is not None:
-        raise ProcException("Error: missing package dependency: {}", MISSING_LIBS)
+    if MISSING_MOD is not None:
+        raise ProcException("Error: missing package dependency: {}", MISSING_MOD)
+    elif Version(PII_EXTRACT_VERSION) < Version(defs.MIN_PII_EXTRACT_VERSION):
+        raise ProcException("incompatible pii-extract-base version {}",
+                            PII_EXTRACT_VERSION)
+
     log = PiiLogger(__name__, verbose > 0)
 
     # Load a configuration, if given
     if config:
         log(". Loading config: %s", config)
         config = load_config(config)
     else:
```

### Comparing `pii-transform-0.4.2/src/pii_transform/api/e2e/multilang.py` & `pii-transform-0.5.0/src/pii_transform/api/e2e/textchunk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,119 +1,94 @@
 """
-Multi-language processor for raw text buffers
+Processor for raw text buffers.
+All buffers must be in the same language.
 """
 
 from typing import List, Tuple, Dict
 
 from packaging.version import Version
 
 from pii_data.helper.config import TYPE_CONFIG_LIST, load_config
 from pii_data.helper.exception import ProcException
-from pii_data.helper.logger import PiiLogger
 from pii_data.types import PiiCollection
 from pii_data.types.doc import DocumentChunk
 from pii_transform.api import PiiTransformer
+from . import defs
 try:
     from pii_extract.api.processor import PiiProcessor, PiiCollectionBuilder
-    from pii_extract.build.collection import TYPE_TASKENUM
+    from pii_extract.gather.collection import TYPE_TASKENUM
     from pii_extract import VERSION as PII_EXTRACT_VERSION
-    MISSING = None
+    MISSING_MOD = None
 except ImportError as e:
-    MISSING = str(e)
+    MISSING_MOD = str(e)
     PiiProcessor = None
     PiiCollectionBuilder = None
     TYPE_TASKENUM = List
     PII_EXTRACT_VERSION = None
 
 
 
-class MultiPiiTextProcessor:
+class PiiTextProcessor:
     """
-    A simple class that performs end2end PII processing on a text buffer,
-    suitable for a list of languages
+    A simple class that performs end2end PII processing on a text buffer
     """
 
-    def __init__(self, lang: List[str], default_policy: str = None,
+    def __init__(self, lang: str = "en", default_policy: str = None,
                  config: TYPE_CONFIG_LIST = None, country: List[str] = None,
-                 tasks: TYPE_TASKENUM = None, keep_piic: bool = False,
-                 debug: bool = False):
+                 tasks: TYPE_TASKENUM = None, debug: bool = False):
         """
-         :param lang: list of languages that text buffers can be in
+         :param lang: language that all text buffers will be in
          :param default_policy: default transformation policy to use
          :param config: configuration(s) to load, in addition to the defaults
          :param country: country(es) to restrict task for
          :param tasks: restrict to an specific set of detection tasks
-         :param keep_piic: store all detected PII
          :param debug: activate debug output
         """
-        if MISSING is not None:
-            raise ProcException("missing package dependency: {}", MISSING)
-        elif Version(PII_EXTRACT_VERSION) < Version("0.3.1"):
+        if MISSING_MOD is not None:
+            raise ProcException("missing package dependency: {}", MISSING_MOD)
+        elif Version(PII_EXTRACT_VERSION) < Version(defs.MIN_PII_EXTRACT_VERSION):
             raise ProcException("incompatible pii-extract-base version {}",
                                 PII_EXTRACT_VERSION)
-
-        self._log = PiiLogger(__name__, debug)
-        self._log(". start: lang=%s", lang)
         self._cid = 0
         self.config = load_config(config or [])
-        self.policy = default_policy
         self.lang = lang
-        self._proc = PiiProcessor(config=self.config, debug=debug)
-        self._piic = PiiCollectionBuilder() if keep_piic else None
-        num = 0
-        for lng in lang:
-            ctr = country[lng] if isinstance(country, dict) else country
-            self._log(". build-tasks for: %s", lng)
-            num += self._proc.build_tasks(lang=lng, country=ctr, pii=tasks)
-        self._trf = PiiTransformer(default_policy=default_policy,
-                                   config=self.config, debug=debug)
-        self.num_tasks = num
+        self.policy = default_policy
+        self.proc = PiiProcessor(config=self.config, debug=debug)
+        self.proc.build_tasks(lang=lang, country=country, pii=tasks)
+        self.trf = PiiTransformer(default_policy=default_policy,
+                                  config=self.config, debug=debug)
 
 
     def __repr__(self) -> str:
-        return f"<MultiPiiTextProcessor [#{len(self.lang)}/{self.num_tasks} {self.policy}]>"
+        return f"<PiiTextProcessor [{self.policy}]>"
 
 
     def process(self, chunk: DocumentChunk) -> Tuple[DocumentChunk, PiiCollection]:
         """
         Process a document chunk: detect PII and transform the PII instances
         found in the chunk, according to the defined policy
           :return: a tuple (output-chunk, collection-of-detected-pii)
         """
-        try:
-            lang = chunk.context["lang"]
-        except (KeyError, TypeError):
-            raise ProcException("missing chunk language")
-
-        piic = self._piic if self._piic is not None else PiiCollectionBuilder(lang=lang)
-        self._proc.detect_chunk(chunk, piic)
-        chunk = self._trf.transform_chunk(chunk, piic)
+        piic = PiiCollectionBuilder(lang=self.lang)
+        self.proc.detect_chunk(chunk, piic)
+        chunk = self.trf.transform_chunk(chunk, piic)
         return chunk, piic
 
 
-    def __call__(self, text: str, lang: str) -> str:
+    def __call__(self, text: str) -> str:
         """
         Process a text buffer: detect PII and transform the PII instances found,
         according to the defined policy
-          :param text: text buffer
-          :param lang: text language
           :return: the trasformed text buffer
         """
         self._cid += 1
         input_chunk = DocumentChunk(id=self._cid, data=text,
-                                    context={"lang": lang})
+                                    context={"lang": self.lang})
         output_chunk, piic = self.process(input_chunk)
         return output_chunk.data
 
 
-    def piic(self) -> PiiCollection:
-        """
-        Returns the object with all detected PII (if configured)
-        """
-        return self._piic
-
-
     def stats(self) -> Dict:
         """
         Returns statistics on the detected PII instances
         """
         return self._proc.get_stats()
```

### Comparing `pii-transform-0.4.2/src/pii_transform/api/e2e/textchunk.py` & `pii-transform-0.5.0/src/pii_transform/api/transform.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,93 @@
 """
-Process raw text buffers
+Transform documents by replacing PII instances according to a policy
 """
+from operator import attrgetter
 
-from typing import List, Tuple, Dict
+from typing import Dict, Union
 
-from pii_data.helper.config import TYPE_CONFIG_LIST, load_config
-from pii_data.helper.exception import ProcException
 from pii_data.types import PiiCollection
-from pii_data.types.doc import DocumentChunk
-from pii_transform.api import PiiTransformer
-try:
-    from pii_extract.api.processor import PiiProcessor, PiiCollectionBuilder
-    from pii_extract.build.collection import TYPE_TASKENUM
-    MISSING = None
-except ImportError as e:
-    MISSING = str(e)
-    TYPE_TASKENUM = List
-    PiiProcessor = None
-    PiiCollectionBuilder = None
+from pii_data.types.doc import SrcDocument, DocumentChunk, LocalSrcDocument
+from pii_data.types.piicollection import PiiChunkIterator
+from pii_data.helper.config import load_config
 
+from ..helper import PiiSubstitutionValue
+from .. import defs
 
+# Reset all assigment caches for each new document
+DEFAULT_RESET = "document"
 
-class PiiTextProcessor:
-    """
-    A simple class that performs end2end PII processing on a text buffer
-    """
-
-    def __init__(self, lang: str = "en", default_policy: str = None,
-                 config: TYPE_CONFIG_LIST = None, country: List[str] = None,
-                 tasks: TYPE_TASKENUM = None, debug: bool = False):
-        """
-         :param lang: language that text buffers will be in
-         :param default_policy: default transformation policy to use
-         :param config: configuration(s) to load, in addition to the defaults
-         :param country: country(es) to restrict task for
-         :param tasks: restrict to an specific set of detection tasks
-         :param debug: activate debug output
-        """
-        if MISSING is not None:
-            raise ProcException("missing package dependency: {}", MISSING)
-        self._cid = 0
-        self.config = load_config(config or [])
-        self.lang = lang
-        self.policy = default_policy
-        self.proc = PiiProcessor(config=self.config, debug=debug)
-        self.proc.build_tasks(lang=lang, country=country, pii=tasks)
-        self.trf = PiiTransformer(default_policy=default_policy,
-                                  config=self.config, debug=debug)
 
+# --------------------------------------------------------------------------
 
-    def __repr__(self) -> str:
-        return f"<PiiTextProcessor [{self.policy}]>"
 
+class PiiTransformer:
 
-    def process(self, chunk: DocumentChunk) -> Tuple[DocumentChunk, PiiCollection]:
+    def __init__(self, default_policy: Union[str, Dict] = None,
+                 config: Dict = None, debug: bool = False):
         """
-        Process a document chunk: detect PII and transform the PII instances
-        found in the chunk, according to the defined policy
-          :return: a tuple (output-chunk, collection-of-detected-pii)
+         :param default_policy: a default policy value to apply to all entities
+            that do not have a specific policy
+         :param config: object configuration to apply
+         :param debug: print out debug messages
         """
-        piic = PiiCollectionBuilder(lang=self.lang)
-        self.proc.detect_chunk(chunk, piic)
-        chunk = self.trf.transform_chunk(chunk, piic)
-        return chunk, piic
+        self._debug = debug
+        all_config = load_config(config, [defs.FMT_CONFIG_TRANSFORM,
+                                          defs.FMT_CONFIG_PLACEHOLDER])
+        config = all_config.get(defs.FMT_CONFIG_TRANSFORM) or {}
+        self._reset = config.get("reset", DEFAULT_RESET)
+        if default_policy is None:
+            default_policy = config.get("default_policy")
+        self.subst = PiiSubstitutionValue(default_policy, all_config)
 
 
-    def __call__(self, text: str) -> str:
-        """
-        Process a text buffer: detect PII and transform the PII instances found,
-        according to the defined policy
-          :return: the trasformed text buffer
-        """
-        self._cid += 1
-        input_chunk = DocumentChunk(id=self._cid, data=text)
-        output_chunk, piic = self.process(input_chunk)
-        return output_chunk.data
+    def __repr__(self) -> str:
+        return "<PiiTransformer>"
 
 
-    def stats(self) -> Dict:
-        """
-        Returns statistics on the detected PII instances
+    def transform_chunk(self, chunk: DocumentChunk, piic: PiiCollection):
         """
-        return self._proc.get_stats()
+        Perform a transformation on a DocumentChunk
+         :param chunk: original chunk
+         :param piic: a collection providing the piic for this chunk
+        """
+        # Construct the new content for the chunk
+        output = []
+        pos = 0
+        for pii in sorted(piic, key=attrgetter("pos")):
+            action = pii.fields.get("process", {}).get("action", "transform")
+            if action == "ignore":
+                continue
+            output += [chunk.data[pos:pii.pos], self.subst(pii)]
+            pos = pii.pos + len(pii)
+        chunk_data = "".join(output) + chunk.data[pos:]
+        return DocumentChunk(chunk.id, chunk_data, chunk.context)
+
+
+    def __call__(self, document: SrcDocument,
+                 piic: PiiCollection) -> SrcDocument:
+        """
+        Replace in a document the passed detected PII values, in accordance
+        with the policies that have been set
+         :param document: the original document
+         :param piic: the list of detected PII instances
+         :return: a local document with all replacements done
+        """
+        if self._reset == "document":
+            self.subst.reset()
+
+        pii_it = PiiChunkIterator(piic)
+
+        # Create the output document, and clone all its metadata
+        meta = document.metadata
+        dtype = meta.get("document", {}).get("type", "sequence")
+        out = LocalSrcDocument(dtype)
+        out.add_metadata(**meta)
+
+        # Substitute all PII instances in all chunks
+        for chunk in document:
+            if self._reset == "chunk":
+                self.subst.reset()
+            newchunk = self.transform_chunk(chunk, pii_it(chunk.id))
+            out.add_chunk(newchunk)
+
+        return out
```

### Comparing `pii-transform-0.4.2/src/pii_transform/app/process.py` & `pii-transform-0.5.0/src/pii_transform/app/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 
 from typing import List
 
 from .. import VERSION
 from ..helper.substitution import POLICIES
 
-from ..api.e2e import process_document, format_policy, MISSING_LIBS
+from ..api.e2e import process_document, format_policy, MISSING_MOD
 
 
 # -------------------------------------------------------------------------
 
 
 def parse_args(args: List[str]) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
@@ -56,16 +56,16 @@
     g3.add_argument("--show-stats", action="store_true", help="show statistics")
     g3.add_argument("--show-tasks", action="store_true", help="show defined tasks")
 
     return parser.parse_args(args)
 
 
 def main(args: List[str] = None):
-    if MISSING_LIBS is not None:
-        print("Error: missing package dependency:", MISSING_LIBS)
+    if MISSING_MOD is not None:
+        print("Error: missing package dependency:", MISSING_MOD)
         sys.exit(1)
     if args is None:
         args = sys.argv[1:]
 
     args = parse_args(args)
     kw = vars(args)
     reraise = kw.pop("reraise")
```

### Comparing `pii-transform-0.4.2/src/pii_transform/app/transform.py` & `pii-transform-0.5.0/src/pii_transform/app/transform.py`

 * *Files identical despite different names*

### Comparing `pii-transform-0.4.2/src/pii_transform/helper/logger.py` & `pii-transform-0.5.0/src/pii_transform/helper/logger.py`

 * *Files identical despite different names*

### Comparing `pii-transform-0.4.2/src/pii_transform/helper/placeholder.py` & `pii-transform-0.5.0/src/pii_transform/helper/placeholder.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  * values can be fixed strings or lists of choices
  * if a choice, they are assigned consecutively to PiiEntity of the same type
  * the chosen value is maintained for subsequent appearances of the same
    PiiInstance (same type & value)
  * the list is rotated as much as needed
 """
 
+import random
 from pathlib import Path
 from functools import lru_cache
 from collections import defaultdict
 
 from typing import Union, List, Tuple, Dict
 
 from pii_data.types import PiiEntity
@@ -60,15 +61,15 @@
 
     def __repr__(self) -> str:
         return f"<PlaceholderValue: #{len(self._values)}>"
 
 
     def _select_value(self, pii: PiiEntity) -> Union[str, List[str]]:
         """
-        Select the value to apply from the placeholder database
+        Select the value to apply from the placeholder data
         """
         fields = pii.fields
         pii_type = fields["type"]
         elem = self._values.get(pii_type)
 
         if not elem:
             return pii_type
@@ -88,18 +89,24 @@
     def _rotate_value(self, key: str, value: str, choices: Tuple[str]):
         """
         Rotate the value to use from the list, keeping consistency in
         assignments to the same PiiEntity values
 
         Note: "value" is used as argument only to trigger LRU cache retrieval
         """
+        # First time we use this key?
+        num_choices = len(choices)
+        if key not in self._index:
+            self._index[key] = random.randrange(num_choices)
+
+        # Select element & rotate key for next call
         try:
             return choices[self._index[key]]
         finally:
-            self._index[key] = (self._index[key] + 1) % len(choices)
+            self._index[key] = (self._index[key] + 1) % num_choices
 
 
     def __call__(self, pii: PiiEntity) -> str:
         """
         Return the appropriate placeholder value for a given PiiEntity
         """
         # Check the value we have
```

### Comparing `pii-transform-0.4.2/src/pii_transform/helper/substitution.py` & `pii-transform-0.5.0/src/pii_transform/helper/substitution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 The main object performing PII value substitution
 """
+import random
 import hashlib
 
 from typing import Union, Dict, Callable
 
-from pii_data.helper.exception import InvArgException, UnimplementedException
+from pii_data.helper.exception import InvArgException
 from pii_data.types import PiiEnum, PiiEntity
 
 from .. import defs
 from .placeholder import PlaceholderValue
-from .synthetic import SyntheticValue
+from .synthetic import SyntheticValue, PROVIDER as SYNT_PROVIDER
 
 
 DEFAULT_POLICY = "label"
 
 POLICIES = (
     "passthrough", "redact", "hash", "label", "placeholder",
     "synthetic", "annotate", "custom"
@@ -83,20 +84,25 @@
     def __init__(self, default_policy: Union[str, Dict] = None,
                  config: Dict = None):
         """
          :param default_policy: a default policy to apply to all entities that
             do not have a specific policy in the configuration
          :param config: configuration to apply
         """
+        self._cache = {}
         self._config = config or {}
-        self._ph = None
+        cfg = self._config.get(defs.FMT_CONFIG_TRANSFORM) or {}
+
+        # Set the random seed, if needed
+        self.seed = cfg.get("seed") if config else None
+        if self.seed:
+            random.seed(self.seed)
 
         # Build the policy assigner
         self._assign = {"default": self._policy(default_policy or DEFAULT_POLICY)}
-        cfg = self._config.get(defs.FMT_CONFIG_TRANSFORM) or {}
         policy = cfg.get("policy")
         if policy is not None:
             for p, v in policy.items():
                 self._assign[policy_target(p)] = self._policy(v)
 
 
     def __repr__(self) -> str:
@@ -120,49 +126,57 @@
                 raise InvArgException("invalid policy value '{}': {}",
                                       policy, e) from e
         if pname not in POLICIES:
             raise InvArgException("unsupported policy: {}", pname)
 
         # Return the transformation for this policy
         if pname == "placeholder":
-            if self._ph is None:
+            if pname not in self._cache:
                 cfg = self._config.get(defs.FMT_CONFIG_PLACEHOLDER)
-                self._ph = PlaceholderValue(cfg)
-            return self._ph
+                self._cache[pname] = PlaceholderValue(cfg)
+            return self._cache[pname]
+        elif pname == "synthetic":
+            if pname not in self._cache:
+                cfg = self._config.get(defs.FMT_CONFIG_TRANSFORM)
+                self._cache[pname] = SyntheticValue(cfg)
+            return self._cache[pname]
         elif pname == "hash":
             try:
                 key = policy["key"]
             except KeyError as e:
                 raise InvArgException("hash policy needs a key") from e
             return Hasher(key, size=policy.get("size"))
-        elif pname == "synthetic":
-            cfg = self._config.get(defs.FMT_CONFIG_TRANSFORM)
-            return SyntheticValue(cfg)
         elif pname == "custom":
             try:
                 return policy["template"]
             except (TypeError, KeyError) as e:
                 raise InvArgException("custom policy needs a supplied template") from e
         else:
             # a known policy with an available template
             return TEMPLATES[pname]
 
 
     def reset(self):
         """
-        Reset all caches (i.e. forget all previous assignments
+        Reset all caches (i.e. forget all previous substitutions)
         """
         for p in self._assign.values():
             if hasattr(p, "reset"):
                 p.reset()
 
 
     def __call__(self, pii: PiiEntity) -> str:
         """
         Find the substitution string for an entity, according to the installed
         policies
         """
-        v = self._assign.get(pii.fields["type"]) or self._assign["default"]
-        if isinstance(v, str):
-            return v.format_map(DefaultEmpty(pii.asdict()))
+        # Find the substitution processor.
+        # For Synthetic ensure we've got a provider, else use the default
+        proc = self._assign.get(pii.fields["type"]) or self._assign["default"]
+        if isinstance(proc, SyntheticValue) and pii.info.pii not in SYNT_PROVIDER:
+            proc = self._policy(DEFAULT_POLICY)
+
+        # Apply the processor
+        if isinstance(proc, str):
+            return proc.format_map(DefaultEmpty(pii.asdict()))
         else:
-            return v(pii)
+            return proc(pii)
```

### Comparing `pii-transform-0.4.2/src/pii_transform/helper/synthetic.py` & `pii-transform-0.5.0/src/pii_transform/helper/synthetic.py`

 * *Files identical despite different names*

### Comparing `pii-transform-0.4.2/src/pii_transform/resources/placeholder.json` & `pii-transform-0.5.0/src/pii_transform/resources/placeholder.json`

 * *Files identical despite different names*

### Comparing `pii-transform-0.4.2/src/pii_transform.egg-info/PKG-INFO` & `pii-transform-0.5.0/src/pii_transform.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 Metadata-Version: 2.1
 Name: pii-transform
-Version: 0.4.2
+Version: 0.5.0
 Summary: Transform recognized PII instances in a document
 Home-page: https://github.com/piisa/pii-transform
+Download-URL: https://github.com/piisa/pii-transform/tarball/v0.5.0
 Author: Paulo Villegas
 Author-email: paulo.vllgs@gmail.com
 License: Apache
-Download-URL: https://github.com/piisa/pii-transform/tarball/v0.4.2
-Description: # pii-transform
-        
-        
-        This package takes a source document, a collection of detected PII instances,
-        and transforms the document by replacing the PII instances in the document
-        with a different representation.
-        
-        The type of substitution done is defined by transformation policies.
-        
-        
-        ## Command-line scripts
-        
-        The package provides two console scripts:
-        
-         * `pii-transform` loads a source document & a collection of detected PII, 
-           and produces a transformed document following the required policies.
-         * `pii-process` is a full end-to-end script:
-            - load a document, from among the formats supported by `pii-preprocess`
-        	- detects PII instances, according to `pii-extract` and its installed
-        	  plugins
-            - transforms the detected PII instances (according to the indicated policy)
-        	  and writes out the transformed documennt
-        	  
-        	  
-        Note that `pii-process` will need additional packages to be present:
-         * `pii-preprocess`
-         * `pii-extract-base`, together with any available detection plugins, e.g.
-           `pii-extract-plg-regex`
-        
-        
-        ## API
-        
-        The same functionality provided by the command-line scripts can also be
-        accessed via a Python API
-        
-        
-        
 Keywords: PIISA, PII
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# pii-transform
+
+
+This package takes a source document, a collection of detected PII instances,
+and transforms the document by replacing the PII instances in the document
+with a different representation.
+
+The type of substitution done is defined by transformation policies.
+
+
+## Command-line scripts
+
+The package provides three console scripts:
+
+ * `pii-transform` loads a source document & a collection of already-detected
+   PII, and produces a transformed document following the required policies.
+ * `pii-process` is a full end-to-end script:
+    - load a document, from among the formats supported by `pii-preprocess`
+	- detects PII instances, according to `pii-extract` and its installed
+	  plugins
+    - transforms the detected PII instances (according to the indicated policy)
+	  and writes out the transformed documennt
+ * `pii-process-jsonl` is also a full end-to-end script; this one reads
+   JSONL files and processes each line as a separate text buffer (possibly in
+   different languages), producing a transformed JSONL document
+	  
+	  
+Note that `pii-process` & `pii-process-jsonl` will need additional packages
+to be installed:
+ * `pii-preprocess` (only for `pii-process`)
+ * `pii-extract-base`, together with any available detection plugins, e.g.
+   `pii-extract-plg-regex` and/or `pii-extract-plg-presidio`
+
+
+## API
+
+The same functionality provided by the command-line scripts can also be
+accessed via a Python API
+
+
```

### Comparing `pii-transform-0.4.2/src/pii_transform.egg-info/SOURCES.txt` & `pii-transform-0.5.0/src/pii_transform.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 src/pii_transform.egg-info/dependency_links.txt
 src/pii_transform.egg-info/entry_points.txt
 src/pii_transform.egg-info/requires.txt
 src/pii_transform.egg-info/top_level.txt
 src/pii_transform/api/__init__.py
 src/pii_transform/api/transform.py
 src/pii_transform/api/e2e/__init__.py
+src/pii_transform/api/e2e/defs.py
 src/pii_transform/api/e2e/document.py
 src/pii_transform/api/e2e/multilang.py
 src/pii_transform/api/e2e/textchunk.py
 src/pii_transform/app/__init__.py
 src/pii_transform/app/chunk.py
 src/pii_transform/app/multi.py
 src/pii_transform/app/process.py
 src/pii_transform/app/transform.py
 src/pii_transform/helper/__init__.py
 src/pii_transform/helper/logger.py
+src/pii_transform/helper/misc.py
 src/pii_transform/helper/placeholder.py
 src/pii_transform/helper/substitution.py
 src/pii_transform/helper/synthetic.py
 src/pii_transform/resources/placeholder.json
 src/pii_transform/resources/transform.json
```

