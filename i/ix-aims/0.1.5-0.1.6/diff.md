# Comparing `tmp/ix_aims-0.1.5.tar.gz` & `tmp/ix_aims-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ix_aims-0.1.5.tar", max compression
+gzip compressed data, was "ix_aims-0.1.6.tar", max compression
```

## Comparing `ix_aims-0.1.5.tar` & `ix_aims-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.5/ix_aims/__init__.py
--rw-r--r--   0        0        0      606 2023-05-02 23:55:26.364346 ix_aims-0.1.5/ix_aims/cli.py
--rw-r--r--   0        0        0      240 2023-05-03 17:44:05.589407 ix_aims-0.1.5/ix_aims/imgs/__init__.py
--rw-r--r--   0        0        0      335 2023-05-03 17:50:50.001156 ix_aims-0.1.5/ix_aims/imgs/ellipsBtn.png
--rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.5/ix_aims/imgs/plusTab.png
--rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.5/ix_aims/imgs/processesBtn.png
--rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.5/ix_aims/imgs/yesBtn.png
--rw-r--r--   0        0        0     3635 2023-05-08 17:12:59.884461 ix_aims-0.1.5/ix_aims/lib.py
--rw-r--r--   0        0        0      627 2023-05-08 17:12:59.868461 ix_aims-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 ix_aims-0.1.5/setup.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 ix_aims-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.6/ix_aims/__init__.py
+-rw-r--r--   0        0        0      421 2023-05-10 16:14:15.001567 ix_aims-0.1.6/ix_aims/cli.py
+-rw-r--r--   0        0        0      240 2023-05-03 17:44:05.589407 ix_aims-0.1.6/ix_aims/imgs/__init__.py
+-rw-r--r--   0        0        0      335 2023-05-03 17:50:50.001156 ix_aims-0.1.6/ix_aims/imgs/ellipsBtn.png
+-rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.6/ix_aims/imgs/plusTab.png
+-rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.6/ix_aims/imgs/processesBtn.png
+-rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.6/ix_aims/imgs/yesBtn.png
+-rw-r--r--   0        0        0     3635 2023-05-08 17:12:59.884461 ix_aims-0.1.6/ix_aims/lib.py
+-rw-r--r--   0        0        0      627 2023-05-10 16:14:26.169168 ix_aims-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 ix_aims-0.1.6/setup.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 ix_aims-0.1.6/PKG-INFO
```

### Comparing `ix_aims-0.1.5/ix_aims/imgs/processesBtn.png` & `ix_aims-0.1.6/ix_aims/imgs/processesBtn.png`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.5/ix_aims/imgs/yesBtn.png` & `ix_aims-0.1.6/ix_aims/imgs/yesBtn.png`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.5/ix_aims/lib.py` & `ix_aims-0.1.6/ix_aims/lib.py`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.5/pyproject.toml` & `ix_aims-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ix-aims"
-version = "0.1.5"
+version = "0.1.6"
 description = "iX Capture automation with AIMS data"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ix_aims"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ix_aims-0.1.5/setup.py` & `ix_aims-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['autoix = ix_aims.cli:main']}
 
 setup_kwargs = {
     'name': 'ix-aims',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'iX Capture automation with AIMS data',
     'long_description': '# auto-ix-capture\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ix_aims-0.1.5/PKG-INFO` & `ix_aims-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ix-aims
-Version: 0.1.5
+Version: 0.1.6
 Summary: iX Capture automation with AIMS data
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

