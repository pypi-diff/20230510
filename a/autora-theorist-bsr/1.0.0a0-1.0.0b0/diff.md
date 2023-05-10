# Comparing `tmp/autora-theorist-bsr-1.0.0a0.tar.gz` & `tmp/autora-theorist-bsr-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-bsr-1.0.0a0.tar", last modified: Fri May  5 20:01:44 2023, max compression
+gzip compressed data, was "autora-theorist-bsr-1.0.0b0.tar", last modified: Wed May 10 11:00:54 2023, max compression
```

## Comparing `autora-theorist-bsr-1.0.0a0.tar` & `autora-theorist-bsr-1.0.0b0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.911169 autora-theorist-bsr-1.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.911169 autora-theorist-bsr-1.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    37812 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/docs/bsr.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/docs/how_it_works.md
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/docs/img.png
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/docs/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/docs/meta_parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/docs/search_space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.911169 autora-theorist-bsr-1.0.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.911169 autora-theorist-bsr-1.0.0a0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.911169 autora-theorist-bsr-1.0.0a0/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32217 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/src/autora_theorist_bsr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-05 20:01:44.000000 autora-theorist-bsr-1.0.0a0/src/autora_theorist_bsr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-05 20:01:44.000000 autora-theorist-bsr-1.0.0a0/src/autora_theorist_bsr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:01:44.000000 autora-theorist-bsr-1.0.0a0/src/autora_theorist_bsr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 20:01:44.000000 autora-theorist-bsr-1.0.0a0/src/autora_theorist_bsr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 20:01:44.000000 autora-theorist-bsr-1.0.0a0/src/autora_theorist_bsr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:44.915170 autora-theorist-bsr-1.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/tests/test_bsr_mcmc_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/tests/test_bsr_node_and_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-05 20:01:32.000000 autora-theorist-bsr-1.0.0a0/tests/test_bsr_tree_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.354676 autora-theorist-bsr-1.0.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.346676 autora-theorist-bsr-1.0.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.350676 autora-theorist-bsr-1.0.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-10 11:00:54.354676 autora-theorist-bsr-1.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.350676 autora-theorist-bsr-1.0.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    32362 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/docs/basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/docs/how-it-works.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/docs/img.png
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.350676 autora-theorist-bsr-1.0.0b0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/docs/meta-parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/docs/quick-start.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/docs/search-space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.350676 autora-theorist-bsr-1.0.0b0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:00:54.354676 autora-theorist-bsr-1.0.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.350676 autora-theorist-bsr-1.0.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.350676 autora-theorist-bsr-1.0.0b0/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.350676 autora-theorist-bsr-1.0.0b0/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.354676 autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32217 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.354676 autora-theorist-bsr-1.0.0b0/src/autora_theorist_bsr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-10 11:00:54.000000 autora-theorist-bsr-1.0.0b0/src/autora_theorist_bsr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-10 11:00:54.000000 autora-theorist-bsr-1.0.0b0/src/autora_theorist_bsr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:00:54.000000 autora-theorist-bsr-1.0.0b0/src/autora_theorist_bsr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 11:00:54.000000 autora-theorist-bsr-1.0.0b0/src/autora_theorist_bsr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 11:00:54.000000 autora-theorist-bsr-1.0.0b0/src/autora_theorist_bsr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:54.354676 autora-theorist-bsr-1.0.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/tests/test_bsr_mcmc_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/tests/test_bsr_node_and_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-10 11:00:42.000000 autora-theorist-bsr-1.0.0b0/tests/test_bsr_tree_operation.py
```

### Comparing `autora-theorist-bsr-1.0.0a0/.github/workflows/python-publish.yml` & `autora-theorist-bsr-1.0.0b0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/.gitignore` & `autora-theorist-bsr-1.0.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/.pre-commit-config.yaml` & `autora-theorist-bsr-1.0.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/PKG-INFO` & `autora-theorist-bsr-1.0.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bsr
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: Bayesian Symbolic Regression theorist for AutoRA
 Author-email: "Sida (Star) Li" <listar2000@uchicago.edu>, Ben Andrew <benwallaceandrew@gmail.com>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bsr
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-bsr-1.0.0a0/README.md` & `autora-theorist-bsr-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/docs/how_it_works.md` & `autora-theorist-bsr-1.0.0b0/docs/how-it-works.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/docs/img.png` & `autora-theorist-bsr-1.0.0b0/docs/img.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/docs/introduction.md` & `autora-theorist-bsr-1.0.0b0/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/docs/meta_parameters.md` & `autora-theorist-bsr-1.0.0b0/docs/meta-parameters.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/docs/search_space.md` & `autora-theorist-bsr-1.0.0b0/docs/search-space.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/mkdocs/base.yml` & `autora-theorist-bsr-1.0.0b0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/pyproject.toml` & `autora-theorist-bsr-1.0.0b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.8,<4"
 
 dependencies = [
     "autora-core",
     "scikit-learn",
+    "torch",
     "scipy",
 ]
 
 [project.optional-dependencies]
 dev = [
     "autora-core[dev]"
 ]
```

### Comparing `autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/funcs.py` & `autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/funcs.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/misc.py` & `autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/misc.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/node.py` & `autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/node.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/operation.py` & `autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/operation.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/prior.py` & `autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/src/autora/theorist/bsr/regressor.py` & `autora-theorist-bsr-1.0.0b0/src/autora/theorist/bsr/regressor.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/src/autora_theorist_bsr.egg-info/PKG-INFO` & `autora-theorist-bsr-1.0.0b0/src/autora_theorist_bsr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-bsr
-Version: 1.0.0a0
+Version: 1.0.0b0
 Summary: Bayesian Symbolic Regression theorist for AutoRA
 Author-email: "Sida (Star) Li" <listar2000@uchicago.edu>, Ben Andrew <benwallaceandrew@gmail.com>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-bsr
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-bsr-1.0.0a0/src/autora_theorist_bsr.egg-info/SOURCES.txt` & `autora-theorist-bsr-1.0.0b0/src/autora_theorist_bsr.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
-docs/bsr.ipynb
-docs/how_it_works.md
+docs/basic-usage.ipynb
+docs/how-it-works.md
 docs/img.png
-docs/introduction.md
-docs/meta_parameters.md
-docs/search_space.md
+docs/index.md
+docs/meta-parameters.md
+docs/quick-start.md
+docs/search-space.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/theorist/bsr/__init__.py
 src/autora/theorist/bsr/funcs.py
 src/autora/theorist/bsr/misc.py
 src/autora/theorist/bsr/node.py
 src/autora/theorist/bsr/operation.py
```

### Comparing `autora-theorist-bsr-1.0.0a0/tests/README.md` & `autora-theorist-bsr-1.0.0b0/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/tests/test_bsr_mcmc_actions.py` & `autora-theorist-bsr-1.0.0b0/tests/test_bsr_mcmc_actions.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/tests/test_bsr_node_and_operator.py` & `autora-theorist-bsr-1.0.0b0/tests/test_bsr_node_and_operator.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0a0/tests/test_bsr_tree_operation.py` & `autora-theorist-bsr-1.0.0b0/tests/test_bsr_tree_operation.py`

 * *Files identical despite different names*

