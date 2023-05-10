# Comparing `tmp/mlex_python-0.0.4.tar.gz` & `tmp/mlex_python-0.0.5.tar.gz`

## Comparing `mlex_python-0.0.4.tar` & `mlex_python-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mlex_python-0.0.4/MLeX/__init__.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 mlex_python-0.0.4/MLeX/experiment.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 mlex_python-0.0.4/MLeX/trial.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mlex_python-0.0.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mlex_python-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mlex_python-0.0.4/README.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 mlex_python-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mlex_python-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mlex_python-0.0.5/MLeX/__init__.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 mlex_python-0.0.5/MLeX/experiment.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 mlex_python-0.0.5/MLeX/trial.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mlex_python-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mlex_python-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mlex_python-0.0.5/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 mlex_python-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 mlex_python-0.0.5/PKG-INFO
```

### Comparing `mlex_python-0.0.4/MLeX/experiment.py` & `mlex_python-0.0.5/MLeX/experiment.py`

 * *Files identical despite different names*

### Comparing `mlex_python-0.0.4/MLeX/trial.py` & `mlex_python-0.0.5/MLeX/trial.py`

 * *Files identical despite different names*

### Comparing `mlex_python-0.0.4/.gitignore` & `mlex_python-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mlex_python-0.0.4/LICENSE` & `mlex_python-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mlex_python-0.0.4/pyproject.toml` & `mlex_python-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mlex-python"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Phoenix Pagan", email="phoenix.pgn@gmail.com" },
 ]
 description = "Lightweight machine learning experiment-tracking tool."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

### Comparing `mlex_python-0.0.4/PKG-INFO` & `mlex_python-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlex-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: Lightweight machine learning experiment-tracking tool.
 Project-URL: Homepage, https://github.com/phoenixp123/MLeX
 Project-URL: Bug Tracker, https://github.com/phoenixp123/MLeX/issues
 Author-email: Phoenix Pagan <phoenix.pgn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Phoenix Pagan
```

