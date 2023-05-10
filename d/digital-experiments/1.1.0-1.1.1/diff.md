# Comparing `tmp/digital-experiments-1.1.0.tar.gz` & `tmp/digital-experiments-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-experiments-1.1.0.tar", last modified: Wed May 10 08:20:46 2023, max compression
+gzip compressed data, was "digital-experiments-1.1.1.tar", last modified: Wed May 10 08:31:26 2023, max compression
```

## Comparing `digital-experiments-1.1.0.tar` & `digital-experiments-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.448796 digital-experiments-1.1.0/
--rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.1.0/LICENSE
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-10 08:20:46.448660 digital-experiments-1.1.0/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/README.md
--rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-10 08:20:37.000000 digital-experiments-1.1.0/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-05-10 08:20:46.448837 digital-experiments-1.1.0/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.443009 digital-experiments-1.1.0/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.445367 digital-experiments-1.1.0/src/digital_experiments/
--rw-r--r--   0 john       (504) staff       (20)      139 2023-05-10 08:20:37.000000 digital-experiments-1.1.0/src/digital_experiments/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     6942 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/src/digital_experiments/backends.py
--rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/control_center.py
--rw-r--r--   0 john       (504) staff       (20)     3651 2023-05-09 14:17:13.000000 digital-experiments-1.1.0/src/digital_experiments/experiment.py
--rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/inspection.py
--rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/metadata.py
--rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.1.0/src/digital_experiments/minimize.py
--rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/observation.py
--rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/src/digital_experiments/pretty.py
--rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.1.0/src/digital_experiments/querying.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.446727 digital-experiments-1.1.0/src/digital_experiments/search/
--rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/search/skopt_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/search/space.py
--rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.1.0/src/digital_experiments/search/suggest.py
--rw-r--r--   0 john       (504) staff       (20)     3837 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/src/digital_experiments/util.py
--rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/version_control.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.446109 digital-experiments-1.1.0/src/digital_experiments.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1070 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      160 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       32 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.448464 digital-experiments-1.1.0/tests/
--rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.1.0/tests/test_backends.py
--rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/tests/test_control_center.py
--rw-r--r--   0 john       (504) staff       (20)     1179 2023-05-09 14:17:13.000000 digital-experiments-1.1.0/tests/test_experiment.py
--rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/tests/test_metadata.py
--rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/tests/test_minimize.py
--rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/tests/test_pretty.py
--rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.1.0/tests/test_querying.py
--rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/tests/test_space.py
--rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.1.0/tests/test_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     2309 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/tests/test_util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:31:26.388985 digital-experiments-1.1.1/
+-rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.1.1/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-10 08:31:26.388800 digital-experiments-1.1.1/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-10 08:31:20.000000 digital-experiments-1.1.1/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-05-10 08:31:26.389042 digital-experiments-1.1.1/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:31:26.382182 digital-experiments-1.1.1/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:31:26.385403 digital-experiments-1.1.1/src/digital_experiments/
+-rw-r--r--   0 john       (504) staff       (20)      139 2023-05-10 08:31:20.000000 digital-experiments-1.1.1/src/digital_experiments/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     6951 2023-05-10 08:31:05.000000 digital-experiments-1.1.1/src/digital_experiments/backends.py
+-rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/src/digital_experiments/control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     3651 2023-05-09 14:17:13.000000 digital-experiments-1.1.1/src/digital_experiments/experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/src/digital_experiments/inspection.py
+-rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/src/digital_experiments/metadata.py
+-rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.1.1/src/digital_experiments/minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/src/digital_experiments/observation.py
+-rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.1.1/src/digital_experiments/pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.1.1/src/digital_experiments/querying.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:31:26.386757 digital-experiments-1.1.1/src/digital_experiments/search/
+-rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/src/digital_experiments/search/skopt_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/src/digital_experiments/search/space.py
+-rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.1.1/src/digital_experiments/search/suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     3837 2023-05-10 08:20:22.000000 digital-experiments-1.1.1/src/digital_experiments/util.py
+-rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/src/digital_experiments/version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:31:26.386319 digital-experiments-1.1.1/src/digital_experiments.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-10 08:31:26.000000 digital-experiments-1.1.1/src/digital_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1070 2023-05-10 08:31:26.000000 digital-experiments-1.1.1/src/digital_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-05-10 08:31:26.000000 digital-experiments-1.1.1/src/digital_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      160 2023-05-10 08:31:26.000000 digital-experiments-1.1.1/src/digital_experiments.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       32 2023-05-10 08:31:26.000000 digital-experiments-1.1.1/src/digital_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:31:26.388451 digital-experiments-1.1.1/tests/
+-rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.1.1/tests/test_backends.py
+-rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/tests/test_control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     1179 2023-05-09 14:17:13.000000 digital-experiments-1.1.1/tests/test_experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/tests/test_metadata.py
+-rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/tests/test_minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.1.1/tests/test_pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.1.1/tests/test_querying.py
+-rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.1.1/tests/test_space.py
+-rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.1.1/tests/test_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     2309 2023-05-10 08:20:22.000000 digital-experiments-1.1.1/tests/test_util.py
```

### Comparing `digital-experiments-1.1.0/LICENSE` & `digital-experiments-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/PKG-INFO` & `digital-experiments-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.1.0
+Version: 1.1.1
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.1.0/README.md` & `digital-experiments-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/pyproject.toml` & `digital-experiments-1.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digital-experiments"
-version = "1.1.0"
+version = "1.1.1"
 description = "Keep track of digital experiments."
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -41,15 +41,15 @@
     "pytest-cov",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/digital-experiments"
 
 [tool.bumpver]
-current_version = "1.1.0"
+current_version = "1.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digital-experiments-1.1.0/src/digital_experiments/backends.py` & `digital-experiments-1.1.1/src/digital_experiments/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             Observation(**unflatten(row, self.SEPARATOR)) for _, row in df.iterrows()
         ]
 
 
 @this_is_a_backend("pickle")
 class PickleBackend(Backend):
     def save(self, obs: Observation):
-        file = self.home / obs.id / "observation.pickle"
+        file = self.home / "runs" / obs.id / "observation.pickle"
         file.parent.mkdir(parents=True, exist_ok=True)
 
         with exclusive_file_access(file, "wb") as f:
             pickle.dump(obs, f)
 
     def all_observations(self) -> List[Observation]:
         files = sorted(self.home.glob("**/observation.pickle"))
```

### Comparing `digital-experiments-1.1.0/src/digital_experiments/control_center.py` & `digital-experiments-1.1.1/src/digital_experiments/control_center.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/experiment.py` & `digital-experiments-1.1.1/src/digital_experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/metadata.py` & `digital-experiments-1.1.1/src/digital_experiments/metadata.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/minimize.py` & `digital-experiments-1.1.1/src/digital_experiments/minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/observation.py` & `digital-experiments-1.1.1/src/digital_experiments/observation.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/pretty.py` & `digital-experiments-1.1.1/src/digital_experiments/pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/querying.py` & `digital-experiments-1.1.1/src/digital_experiments/querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/search/skopt_suggest.py` & `digital-experiments-1.1.1/src/digital_experiments/search/skopt_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/search/space.py` & `digital-experiments-1.1.1/src/digital_experiments/search/space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/search/suggest.py` & `digital-experiments-1.1.1/src/digital_experiments/search/suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/util.py` & `digital-experiments-1.1.1/src/digital_experiments/util.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments/version_control.py` & `digital-experiments-1.1.1/src/digital_experiments/version_control.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/src/digital_experiments.egg-info/PKG-INFO` & `digital-experiments-1.1.1/src/digital_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.1.0
+Version: 1.1.1
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.1.0/src/digital_experiments.egg-info/SOURCES.txt` & `digital-experiments-1.1.1/src/digital_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_backends.py` & `digital-experiments-1.1.1/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_experiment.py` & `digital-experiments-1.1.1/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_metadata.py` & `digital-experiments-1.1.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_minimize.py` & `digital-experiments-1.1.1/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_pretty.py` & `digital-experiments-1.1.1/tests/test_pretty.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_querying.py` & `digital-experiments-1.1.1/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_space.py` & `digital-experiments-1.1.1/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_suggest.py` & `digital-experiments-1.1.1/tests/test_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.1.0/tests/test_util.py` & `digital-experiments-1.1.1/tests/test_util.py`

 * *Files identical despite different names*

