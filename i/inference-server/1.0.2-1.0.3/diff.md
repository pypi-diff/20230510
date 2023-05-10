# Comparing `tmp/inference-server-1.0.2.tar.gz` & `tmp/inference-server-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference-server-1.0.2.tar", last modified: Wed May 10 12:39:26 2023, max compression
+gzip compressed data, was "inference-server-1.0.3.tar", last modified: Wed May 10 17:41:25 2023, max compression
```

## Comparing `inference-server-1.0.2.tar` & `inference-server-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 12:39:11.000000 inference-server-1.0.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-10 12:39:11.000000 inference-server-1.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.048981 inference-server-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.048981 inference-server-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-10 12:39:11.000000 inference-server-1.0.2/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-10 12:39:11.000000 inference-server-1.0.2/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-10 12:39:11.000000 inference-server-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-10 12:39:11.000000 inference-server-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 12:39:11.000000 inference-server-1.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-10 12:39:11.000000 inference-server-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-10 12:39:11.000000 inference-server-1.0.2/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-10 12:39:26.052981 inference-server-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-10 12:39:11.000000 inference-server-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/inference_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/inference_server_testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-10 12:39:11.000000 inference-server-1.0.2/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-10 12:39:11.000000 inference-server-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:39:26.052981 inference-server-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.048981 inference-server-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/src/inference_server/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/default_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-10 12:39:11.000000 inference-server-1.0.2/src/inference_server/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/src/inference_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 12:39:26.000000 inference-server-1.0.2/src/inference_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:39:26.052981 inference-server-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-10 12:39:11.000000 inference-server-1.0.2/tests/test_inference_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-10 12:39:11.000000 inference-server-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:41:25.341382 inference-server-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 17:41:12.000000 inference-server-1.0.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-10 17:41:12.000000 inference-server-1.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:41:25.333381 inference-server-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:41:25.337381 inference-server-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-10 17:41:12.000000 inference-server-1.0.3/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-10 17:41:12.000000 inference-server-1.0.3/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-10 17:41:12.000000 inference-server-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-10 17:41:12.000000 inference-server-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 17:41:12.000000 inference-server-1.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-10 17:41:12.000000 inference-server-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-10 17:41:12.000000 inference-server-1.0.3/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-10 17:41:25.341382 inference-server-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-10 17:41:12.000000 inference-server-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:41:25.337381 inference-server-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/inference_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/inference_server_testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-10 17:41:12.000000 inference-server-1.0.3/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-10 17:41:12.000000 inference-server-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 17:41:25.341382 inference-server-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:41:25.337381 inference-server-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:41:25.341382 inference-server-1.0.3/src/inference_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-10 17:41:12.000000 inference-server-1.0.3/src/inference_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-10 17:41:12.000000 inference-server-1.0.3/src/inference_server/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-10 17:41:12.000000 inference-server-1.0.3/src/inference_server/default_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 17:41:12.000000 inference-server-1.0.3/src/inference_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-10 17:41:12.000000 inference-server-1.0.3/src/inference_server/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:41:25.341382 inference-server-1.0.3/src/inference_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14170 2023-05-10 17:41:25.000000 inference-server-1.0.3/src/inference_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 17:41:25.000000 inference-server-1.0.3/src/inference_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:41:25.000000 inference-server-1.0.3/src/inference_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 17:41:25.000000 inference-server-1.0.3/src/inference_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 17:41:25.000000 inference-server-1.0.3/src/inference_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:41:25.341382 inference-server-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-10 17:41:12.000000 inference-server-1.0.3/tests/test_inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-10 17:41:12.000000 inference-server-1.0.3/tox.ini
```

### Comparing `inference-server-1.0.2/.flake8` & `inference-server-1.0.3/.flake8`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/.github/workflows/release-package.yml` & `inference-server-1.0.3/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/.github/workflows/test-package.yml` & `inference-server-1.0.3/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/.gitignore` & `inference-server-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/.pre-commit-config.yaml` & `inference-server-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/.readthedocs.yaml` & `inference-server-1.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/LICENSE` & `inference-server-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/LICENSE_HEADER.txt` & `inference-server-1.0.3/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/PKG-INFO` & `inference-server-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.0.2
+Version: 1.0.3
 Summary: Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-1.0.2/README.md` & `inference-server-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/docs/conf.py` & `inference-server-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/docs/deployment.rst` & `inference-server-1.0.3/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/docs/hooks.rst` & `inference-server-1.0.3/docs/hooks.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/docs/introduction.rst` & `inference-server-1.0.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/docs/testing.rst` & `inference-server-1.0.3/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/pyproject.toml` & `inference-server-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/src/inference_server/__init__.py` & `inference-server-1.0.3/src/inference_server/__init__.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/src/inference_server/_plugin.py` & `inference-server-1.0.3/src/inference_server/_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/src/inference_server/default_plugin.py` & `inference-server-1.0.3/src/inference_server/default_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/src/inference_server/testing.py` & `inference-server-1.0.3/src/inference_server/testing.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/src/inference_server.egg-info/PKG-INFO` & `inference-server-1.0.3/src/inference_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.0.2
+Version: 1.0.3
 Summary: Deploy your AI/ML model to Amazon SageMaker for real-time inference using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-1.0.2/src/inference_server.egg-info/SOURCES.txt` & `inference-server-1.0.3/src/inference_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/tests/test_inference_server.py` & `inference-server-1.0.3/tests/test_inference_server.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.0.2/tox.ini` & `inference-server-1.0.3/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -60,16 +60,14 @@
   python -m mypy --install-types --non-interactive --package=inference_server
 
 [testenv:docs]
 # Sphinx documentation generation environment
 
 extras =
   docs
-# TODO: remove once docs written
-ignore_outcome = true
 commands =
   # Command exactly as executed on readthedocs.org. See https://readthedocs.org/projects/inference-server/builds/.
   python -m sphinx -T -E -W --keep-going -b html -d {toxinidir}{/}docs{/}_build{/}doctrees -D language=en {toxinidir}{/}docs {toxinidir}{/}docs{/}_build{/}html
 
 [testenv:py312]
 # Overrides for Python 3.12 (dev) test environment
 # TODO: remove entire section once Python 3.12 is released (October 2023)
```

