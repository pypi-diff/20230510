# Comparing `tmp/FlyHash-0.1.0.tar.gz` & `tmp/FlyHash-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlyHash-0.1.0.tar", last modified: Tue May  9 11:13:10 2023, max compression
+gzip compressed data, was "FlyHash-0.2.0.tar", last modified: Tue May  9 13:39:12 2023, max compression
```

## Comparing `FlyHash-0.1.0.tar` & `FlyHash-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.592202 FlyHash-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 11:12:24.000000 FlyHash-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.580202 FlyHash-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.584202 FlyHash-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-09 11:12:24.000000 FlyHash-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-09 11:12:24.000000 FlyHash-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 11:12:24.000000 FlyHash-0.1.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-09 11:12:24.000000 FlyHash-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-09 11:12:24.000000 FlyHash-0.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 11:12:24.000000 FlyHash-0.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 11:12:24.000000 FlyHash-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-09 11:12:24.000000 FlyHash-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 11:12:24.000000 FlyHash-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-09 11:13:10.592202 FlyHash-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-09 11:12:24.000000 FlyHash-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.588202 FlyHash-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.588202 FlyHash-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-09 11:12:24.000000 FlyHash-0.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 11:12:24.000000 FlyHash-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-09 11:13:10.592202 FlyHash-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-09 11:12:24.000000 FlyHash-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.580202 FlyHash-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.592202 FlyHash-0.1.0/src/FlyHash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-09 11:13:10.000000 FlyHash-0.1.0/src/FlyHash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-09 11:13:10.000000 FlyHash-0.1.0/src/FlyHash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:13:10.000000 FlyHash-0.1.0/src/FlyHash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:13:10.000000 FlyHash-0.1.0/src/FlyHash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 11:13:10.000000 FlyHash-0.1.0/src/FlyHash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 11:13:10.000000 FlyHash-0.1.0/src/FlyHash.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.592202 FlyHash-0.1.0/src/flyhash/
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-09 11:12:24.000000 FlyHash-0.1.0/src/flyhash/FlyHash.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-09 11:12:24.000000 FlyHash-0.1.0/src/flyhash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:13:10.592202 FlyHash-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-09 11:12:24.000000 FlyHash-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-09 11:12:24.000000 FlyHash-0.1.0/tests/test_FlyHash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-09 11:12:24.000000 FlyHash-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.666074 FlyHash-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.666074 FlyHash-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-09 13:38:05.000000 FlyHash-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 13:38:05.000000 FlyHash-0.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 13:38:05.000000 FlyHash-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-05-09 13:38:05.000000 FlyHash-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 13:38:05.000000 FlyHash-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-09 13:39:12.670074 FlyHash-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-09 13:38:05.000000 FlyHash-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-09 13:38:05.000000 FlyHash-0.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 13:38:05.000000 FlyHash-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-09 13:39:12.670074 FlyHash-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-09 13:38:05.000000 FlyHash-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.666074 FlyHash-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/src/FlyHash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 13:39:12.000000 FlyHash-0.2.0/src/FlyHash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/src/flyhash/
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-09 13:38:05.000000 FlyHash-0.2.0/src/flyhash/FlyHash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-09 13:38:05.000000 FlyHash-0.2.0/src/flyhash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:39:12.670074 FlyHash-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-09 13:38:05.000000 FlyHash-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-09 13:38:05.000000 FlyHash-0.2.0/tests/test_FlyHash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-09 13:38:05.000000 FlyHash-0.2.0/tox.ini
```

### Comparing `FlyHash-0.1.0/.coveragerc` & `FlyHash-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/.github/workflows/ci.yml` & `FlyHash-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/.gitignore` & `FlyHash-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/.pre-commit-config.yaml` & `FlyHash-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/.readthedocs.yml` & `FlyHash-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/CONTRIBUTING.md` & `FlyHash-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/LICENSE.txt` & `FlyHash-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/PKG-INFO` & `FlyHash-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyHash
-Version: 0.1.0
+Version: 0.2.0
 Summary: A novel hashing algorithm based on "A neural algorithm for a fundamental computing problem" by S. Dasgupta, C. F. Stevens, and S. Navlakha (2017)
 Home-page: https://github.com/TeddyHuang-00/FlyHash
 Author: TeddyHuang-00
 Author-email: teddyhuangnan@gmail.com
 License: MIT
 Project-URL: Documentation, https://flyhash.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/TeddyHuang-00/FlyHash/
@@ -21,7 +21,31 @@
 [![PyPI-Server](https://img.shields.io/pypi/v/FlyHash.svg)](https://pypi.org/project/FlyHash/)
 [![Monthly Downloads](https://pepy.tech/badge/FlyHash/month)](https://pepy.tech/project/FlyHash)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # FlyHash
 
 > A novel hashing algorithm based on "A neural algorithm for a fundamental computing problem" by S. Dasgupta, C. F. Stevens, and S. Navlakha (2017)
+
+FlyHash is a LSH algorithm that maps input data to a sparse hash embedding,
+where the dimension of the hash embedding is much larger than the input,
+and keeps the locality of the input data in the hash embedding.
+
+FlyHash is designed to be cheap to compute, yet not ganranteeing
+memory efficiency. It is suitable for hashing small to medium sized data
+($d$ ~ 10-1000) to a large hash embedding ($m$ ~ 100-10000).
+
+## Usage
+
+Using a large hash_dim $m=100$ for a small input_dim $d=10$:
+
+```python-repl
+>>> import numpy as np
+>>> from flyhash import FlyHash
+>>> d = 10
+>>> m = 100
+>>> flyhash = FlyHash(d, m)
+>>> data = np.random.randn(5, d)
+>>> hashed_data = flyhash(data)
+```
+
+For detailed usage, please refer to the [documentation](https://FlyHash.readthedocs.io/en/latest/).
```

### Comparing `FlyHash-0.1.0/docs/Makefile` & `FlyHash-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/docs/conf.py` & `FlyHash-0.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.ifconfig",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
 ]
 
+# Configure napoleon
+napoleon_include_init_with_doc = True
+napoleon_include_private_with_doc = True
+napoleon_include_special_with_doc = True
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 
 # Enable markdown
 extensions.append("myst_parser")
 
@@ -167,23 +172,20 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
-}
+html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
@@ -297,8 +299,8 @@
     "sklearn": ("https://scikit-learn.org/stable", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
     "setuptools": ("https://setuptools.pypa.io/en/stable/", None),
     "pyscaffold": ("https://pyscaffold.org/en/stable", None),
 }
 
-print(f"loading configurations for {project} {version} ...", file=sys.stderr)
+print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `FlyHash-0.1.0/setup.cfg` & `FlyHash-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/setup.py` & `FlyHash-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/src/FlyHash.egg-info/PKG-INFO` & `FlyHash-0.2.0/src/FlyHash.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlyHash
-Version: 0.1.0
+Version: 0.2.0
 Summary: A novel hashing algorithm based on "A neural algorithm for a fundamental computing problem" by S. Dasgupta, C. F. Stevens, and S. Navlakha (2017)
 Home-page: https://github.com/TeddyHuang-00/FlyHash
 Author: TeddyHuang-00
 Author-email: teddyhuangnan@gmail.com
 License: MIT
 Project-URL: Documentation, https://flyhash.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/TeddyHuang-00/FlyHash/
@@ -21,7 +21,31 @@
 [![PyPI-Server](https://img.shields.io/pypi/v/FlyHash.svg)](https://pypi.org/project/FlyHash/)
 [![Monthly Downloads](https://pepy.tech/badge/FlyHash/month)](https://pepy.tech/project/FlyHash)
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # FlyHash
 
 > A novel hashing algorithm based on "A neural algorithm for a fundamental computing problem" by S. Dasgupta, C. F. Stevens, and S. Navlakha (2017)
+
+FlyHash is a LSH algorithm that maps input data to a sparse hash embedding,
+where the dimension of the hash embedding is much larger than the input,
+and keeps the locality of the input data in the hash embedding.
+
+FlyHash is designed to be cheap to compute, yet not ganranteeing
+memory efficiency. It is suitable for hashing small to medium sized data
+($d$ ~ 10-1000) to a large hash embedding ($m$ ~ 100-10000).
+
+## Usage
+
+Using a large hash_dim $m=100$ for a small input_dim $d=10$:
+
+```python-repl
+>>> import numpy as np
+>>> from flyhash import FlyHash
+>>> d = 10
+>>> m = 100
+>>> flyhash = FlyHash(d, m)
+>>> data = np.random.randn(5, d)
+>>> hashed_data = flyhash(data)
+```
+
+For detailed usage, please refer to the [documentation](https://FlyHash.readthedocs.io/en/latest/).
```

### Comparing `FlyHash-0.1.0/src/FlyHash.egg-info/SOURCES.txt` & `FlyHash-0.2.0/src/FlyHash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/src/flyhash/__init__.py` & `FlyHash-0.2.0/src/flyhash/__init__.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/tests/test_FlyHash.py` & `FlyHash-0.2.0/tests/test_FlyHash.py`

 * *Files identical despite different names*

### Comparing `FlyHash-0.1.0/tox.ini` & `FlyHash-0.2.0/tox.ini`

 * *Files identical despite different names*

