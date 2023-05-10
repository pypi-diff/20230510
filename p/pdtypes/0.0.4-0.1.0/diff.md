# Comparing `tmp/pdtypes-0.0.4.tar.gz` & `tmp/pdtypes-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdtypes-0.0.4.tar", max compression
+gzip compressed data, was "pdtypes-0.1.0.tar", max compression
```

## Comparing `pdtypes-0.0.4.tar` & `pdtypes-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1684 2022-03-02 18:42:08.246346 pdtypes-0.0.4/LICENSE
--rw-r--r--   0        0        0     1013 2022-03-02 18:42:08.246346 pdtypes-0.0.4/README.md
--rw-r--r--   0        0        0      233 2022-03-02 18:42:08.254346 pdtypes-0.0.4/pdtypes/__init__.py
--rw-r--r--   0        0        0    15142 2022-03-02 18:42:08.254346 pdtypes-0.0.4/pdtypes/formatters.py
--rw-r--r--   0        0        0     1354 2022-03-02 18:42:08.254346 pdtypes-0.0.4/pdtypes/groupby.py
--rw-r--r--   0        0        0     1576 2022-03-02 18:42:08.254346 pdtypes-0.0.4/pdtypes/patching.py
--rw-r--r--   0        0        0     1009 2022-03-02 18:42:08.254346 pdtypes-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1726 2022-03-02 18:42:16.789703 pdtypes-0.0.4/setup.py
--rw-r--r--   0        0        0     1668 2022-03-02 18:42:16.790032 pdtypes-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1684 2023-05-10 06:51:19.331079 pdtypes-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1013 2023-05-10 06:51:19.331079 pdtypes-0.1.0/README.md
+-rw-r--r--   0        0        0      233 2023-05-10 06:51:19.331079 pdtypes-0.1.0/pdtypes/__init__.py
+-rw-r--r--   0        0        0    15142 2023-05-10 06:51:19.331079 pdtypes-0.1.0/pdtypes/formatters.py
+-rw-r--r--   0        0        0     1354 2023-05-10 06:51:19.331079 pdtypes-0.1.0/pdtypes/groupby.py
+-rw-r--r--   0        0        0     1576 2023-05-10 06:51:19.331079 pdtypes-0.1.0/pdtypes/patching.py
+-rw-r--r--   0        0        0      977 2023-05-10 06:51:19.331079 pdtypes-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1715 1970-01-01 00:00:00.000000 pdtypes-0.1.0/PKG-INFO
```

### Comparing `pdtypes-0.0.4/LICENSE` & `pdtypes-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdtypes-0.0.4/README.md` & `pdtypes-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pdtypes-0.0.4/pdtypes/formatters.py` & `pdtypes-0.1.0/pdtypes/formatters.py`

 * *Files identical despite different names*

### Comparing `pdtypes-0.0.4/pdtypes/groupby.py` & `pdtypes-0.1.0/pdtypes/groupby.py`

 * *Files identical despite different names*

### Comparing `pdtypes-0.0.4/pdtypes/patching.py` & `pdtypes-0.1.0/pdtypes/patching.py`

 * *Files identical despite different names*

### Comparing `pdtypes-0.0.4/pyproject.toml` & `pdtypes-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pdtypes"
-version = "0.0.4"
+version = "0.1.0"
 description = "Show data types for pandas data frames in terminal and notebooks"
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "BSD 3-Clause"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pdtypes"
 repository = "https://github.com/pwwang/pdtypes"
 
 [tool.poetry.dependencies]
-python = "^3.7.1" # pandas' requirement
-pandas = "^1.2"
+python = "^3.8"
+pandas = "^1.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-cov = "*"
 
 [tool.black]
 line-length = 80
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py38', 'py39']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = "-vv --cov-config=.coveragerc --cov=pdtypes --cov-report xml:cov.xml --cov-report term-missing"
 console_output_style = "progress"
 junit_family = "xunit1"
```

### Comparing `pdtypes-0.0.4/PKG-INFO` & `pdtypes-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pdtypes
-Version: 0.0.4
+Version: 0.1.0
 Summary: Show data types for pandas data frames in terminal and notebooks
 Home-page: https://github.com/pwwang/pdtypes
 License: BSD 3-Clause
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pandas (>=1.2,<2.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=1.4,<2.0)
 Project-URL: Repository, https://github.com/pwwang/pdtypes
 Description-Content-Type: text/markdown
 
 # pdtypes
 
 Show data types for pandas data frames in terminal and notebooks by monkey-patching pandas formatters
```

