# Comparing `tmp/comboparse-0.0.0.tar.gz` & `tmp/comboparse-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comboparse-0.0.0.tar", last modified: Tue May  9 05:31:44 2023, max compression
+gzip compressed data, was "comboparse-1.0.1.tar", last modified: Wed May 10 01:24:19 2023, max compression
```

## Comparing `comboparse-0.0.0.tar` & `comboparse-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:31:44.589951 comboparse-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:31:44.585951 comboparse-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:31:44.585951 comboparse-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-09 05:31:35.000000 comboparse-0.0.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-09 05:31:35.000000 comboparse-0.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-05-09 05:31:35.000000 comboparse-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-09 05:31:35.000000 comboparse-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-09 05:31:44.589951 comboparse-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-09 05:31:35.000000 comboparse-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:31:44.585951 comboparse-0.0.0/comboparse/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 05:31:35.000000 comboparse-0.0.0/comboparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-09 05:31:35.000000 comboparse-0.0.0/comboparse/comboparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:31:44.589951 comboparse-0.0.0/comboparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-09 05:31:44.000000 comboparse-0.0.0/comboparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 05:31:44.000000 comboparse-0.0.0/comboparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:31:44.000000 comboparse-0.0.0/comboparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 05:31:44.000000 comboparse-0.0.0/comboparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 05:31:35.000000 comboparse-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:31:44.589951 comboparse-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 05:31:35.000000 comboparse-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:31:44.589951 comboparse-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 05:31:35.000000 comboparse-0.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-09 05:31:35.000000 comboparse-0.0.0/tests/test_comboparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:24:19.373135 comboparse-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:24:19.373135 comboparse-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:24:19.373135 comboparse-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-10 01:24:10.000000 comboparse-1.0.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-10 01:24:10.000000 comboparse-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-05-10 01:24:10.000000 comboparse-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-10 01:24:10.000000 comboparse-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-10 01:24:19.373135 comboparse-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-10 01:24:10.000000 comboparse-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:24:19.373135 comboparse-1.0.1/comboparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-10 01:24:10.000000 comboparse-1.0.1/comboparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-10 01:24:10.000000 comboparse-1.0.1/comboparse/comboparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:24:19.373135 comboparse-1.0.1/comboparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-10 01:24:19.000000 comboparse-1.0.1/comboparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-10 01:24:19.000000 comboparse-1.0.1/comboparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 01:24:19.000000 comboparse-1.0.1/comboparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 01:24:19.000000 comboparse-1.0.1/comboparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-10 01:24:10.000000 comboparse-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 01:24:19.373135 comboparse-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 01:24:10.000000 comboparse-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:24:19.373135 comboparse-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 01:24:10.000000 comboparse-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-10 01:24:10.000000 comboparse-1.0.1/tests/test_comboparser.py
```

### Comparing `comboparse-0.0.0/.github/workflows/deploy.yml` & `comboparse-1.0.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `comboparse-0.0.0/.github/workflows/test.yml` & `comboparse-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `comboparse-0.0.0/.gitignore` & `comboparse-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `comboparse-0.0.0/LICENSE` & `comboparse-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `comboparse-0.0.0/PKG-INFO` & `comboparse-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: comboparse
-Version: 0.0.0
-Summary: Drop-in replacement for argparse with support for environment variables.
-Author-email: Christopher Kaster <me@atomicptr.de>
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # comboparse
 
 Drop-in replacement for argparse with support for environment variables.
 
 ## How does it work
 
 If environment variables are present that fit a certain schema they are internally appended
@@ -100,8 +88,8 @@
 
 ### Action Type: append_const
 
 This works a bit like a normal store_true/store_false you have to use 1, true etc.
 
 ## License
 
-MIT
+MIT
```

### Comparing `comboparse-0.0.0/README.md` & `comboparse-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: comboparse
+Version: 1.0.1
+Summary: Drop-in replacement for argparse with support for environment variables.
+Author-email: Christopher Kaster <me@atomicptr.de>
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # comboparse
 
 Drop-in replacement for argparse with support for environment variables.
 
 ## How does it work
 
 If environment variables are present that fit a certain schema they are internally appended
@@ -88,8 +100,8 @@
 
 ### Action Type: append_const
 
 This works a bit like a normal store_true/store_false you have to use 1, true etc.
 
 ## License
 
-MIT
+MIT
```

### Comparing `comboparse-0.0.0/comboparse/comboparser.py` & `comboparse-1.0.1/comboparse/comboparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,14 @@
         pos_index = 0
 
         # add environment variable values as args
         for action in self._actions:
             if action.dest is not SUPPRESS and action.default is not SUPPRESS:
                 value = self._env_var_by_dest(action.dest)
 
-                print(action)
-                print(self.create_env_var_name(action.dest), value)
-
                 action_name = type(action).__name__
                 is_append_const_action = action_name == "_AppendConstAction"
 
                 # append const actions doesnt use dest for names
                 if is_append_const_action:
                     value = self._env_var_by_dest(
                         strip_slashes(action.option_strings[0])
```

### Comparing `comboparse-0.0.0/comboparse.egg-info/PKG-INFO` & `comboparse-1.0.1/comboparse.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comboparse
-Version: 0.0.0
+Version: 1.0.1
 Summary: Drop-in replacement for argparse with support for environment variables.
 Author-email: Christopher Kaster <me@atomicptr.de>
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `comboparse-0.0.0/pyproject.toml` & `comboparse-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -16,11 +16,13 @@
     "Operating System :: OS Independent",
 ]
 dynamic = ["version"]
 
 [tool.setuptools]
 packages = {find = {exclude=["tests*"]}}
 
+[tool.setuptools_scm]
+
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
-]
+]
```

### Comparing `comboparse-0.0.0/tests/test_comboparser.py` & `comboparse-1.0.1/tests/test_comboparser.py`

 * *Files identical despite different names*

