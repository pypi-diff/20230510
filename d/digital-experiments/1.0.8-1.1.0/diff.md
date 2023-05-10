# Comparing `tmp/digital-experiments-1.0.8.tar.gz` & `tmp/digital-experiments-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-experiments-1.0.8.tar", last modified: Tue May  9 14:18:15 2023, max compression
+gzip compressed data, was "digital-experiments-1.1.0.tar", last modified: Wed May 10 08:20:46 2023, max compression
```

## Comparing `digital-experiments-1.0.8.tar` & `digital-experiments-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.408534 digital-experiments-1.0.8/
--rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.0.8/LICENSE
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-09 14:18:15.408363 digital-experiments-1.0.8/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/README.md
--rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-09 14:18:09.000000 digital-experiments-1.0.8/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-05-09 14:18:15.408584 digital-experiments-1.0.8/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.402525 digital-experiments-1.0.8/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.405534 digital-experiments-1.0.8/src/digital_experiments/
--rw-r--r--   0 john       (504) staff       (20)      139 2023-05-09 14:18:09.000000 digital-experiments-1.0.8/src/digital_experiments/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     6329 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/src/digital_experiments/backends.py
--rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/control_center.py
--rw-r--r--   0 john       (504) staff       (20)     3651 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/src/digital_experiments/experiment.py
--rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/inspection.py
--rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/metadata.py
--rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.0.8/src/digital_experiments/minimize.py
--rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/observation.py
--rw-r--r--   0 john       (504) staff       (20)      735 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/pretty.py
--rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/src/digital_experiments/querying.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.406882 digital-experiments-1.0.8/src/digital_experiments/search/
--rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/search/skopt_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/search/space.py
--rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.0.8/src/digital_experiments/search/suggest.py
--rw-r--r--   0 john       (504) staff       (20)     3971 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/src/digital_experiments/util.py
--rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/src/digital_experiments/version_control.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.406339 digital-experiments-1.0.8/src/digital_experiments.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     1049 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      160 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       32 2023-05-09 14:18:15.000000 digital-experiments-1.0.8/src/digital_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-09 14:18:15.408121 digital-experiments-1.0.8/tests/
--rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.0.8/tests/test_backends.py
--rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/tests/test_control_center.py
--rw-r--r--   0 john       (504) staff       (20)     1179 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/tests/test_experiment.py
--rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/tests/test_metadata.py
--rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/tests/test_minimize.py
--rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/tests/test_querying.py
--rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.0.8/tests/test_space.py
--rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.0.8/tests/test_suggest.py
--rw-r--r--   0 john       (504) staff       (20)     1407 2023-05-09 14:17:13.000000 digital-experiments-1.0.8/tests/test_util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.448796 digital-experiments-1.1.0/
+-rw-r--r--   0 john       (504) staff       (20)     1051 2022-11-18 07:34:19.000000 digital-experiments-1.1.0/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-10 08:20:46.448660 digital-experiments-1.1.0/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1008 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1321 2023-05-10 08:20:37.000000 digital-experiments-1.1.0/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-05-10 08:20:46.448837 digital-experiments-1.1.0/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.443009 digital-experiments-1.1.0/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.445367 digital-experiments-1.1.0/src/digital_experiments/
+-rw-r--r--   0 john       (504) staff       (20)      139 2023-05-10 08:20:37.000000 digital-experiments-1.1.0/src/digital_experiments/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     6942 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/src/digital_experiments/backends.py
+-rw-r--r--   0 john       (504) staff       (20)     1016 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     3651 2023-05-09 14:17:13.000000 digital-experiments-1.1.0/src/digital_experiments/experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      402 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/inspection.py
+-rw-r--r--   0 john       (504) staff       (20)      592 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/metadata.py
+-rw-r--r--   0 john       (504) staff       (20)     4450 2023-04-04 08:33:50.000000 digital-experiments-1.1.0/src/digital_experiments/minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      637 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/observation.py
+-rw-r--r--   0 john       (504) staff       (20)      735 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/src/digital_experiments/pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     2581 2023-05-09 14:17:13.000000 digital-experiments-1.1.0/src/digital_experiments/querying.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.446727 digital-experiments-1.1.0/src/digital_experiments/search/
+-rw-r--r--   0 john       (504) staff       (20)     2897 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/search/skopt_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     5381 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/search/space.py
+-rw-r--r--   0 john       (504) staff       (20)     4218 2023-04-03 14:30:06.000000 digital-experiments-1.1.0/src/digital_experiments/search/suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     3837 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/src/digital_experiments/util.py
+-rw-r--r--   0 john       (504) staff       (20)     3464 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/src/digital_experiments/version_control.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.446109 digital-experiments-1.1.0/src/digital_experiments.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2642 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     1070 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      160 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       32 2023-05-10 08:20:46.000000 digital-experiments-1.1.0/src/digital_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-10 08:20:46.448464 digital-experiments-1.1.0/tests/
+-rw-r--r--   0 john       (504) staff       (20)     1861 2023-03-29 16:29:55.000000 digital-experiments-1.1.0/tests/test_backends.py
+-rw-r--r--   0 john       (504) staff       (20)      377 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/tests/test_control_center.py
+-rw-r--r--   0 john       (504) staff       (20)     1179 2023-05-09 14:17:13.000000 digital-experiments-1.1.0/tests/test_experiment.py
+-rw-r--r--   0 john       (504) staff       (20)      793 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/tests/test_metadata.py
+-rw-r--r--   0 john       (504) staff       (20)      632 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/tests/test_minimize.py
+-rw-r--r--   0 john       (504) staff       (20)      613 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/tests/test_pretty.py
+-rw-r--r--   0 john       (504) staff       (20)     1580 2023-05-09 14:17:13.000000 digital-experiments-1.1.0/tests/test_querying.py
+-rw-r--r--   0 john       (504) staff       (20)     1596 2023-03-29 15:42:00.000000 digital-experiments-1.1.0/tests/test_space.py
+-rw-r--r--   0 john       (504) staff       (20)     2188 2023-04-04 09:25:29.000000 digital-experiments-1.1.0/tests/test_suggest.py
+-rw-r--r--   0 john       (504) staff       (20)     2309 2023-05-10 08:20:22.000000 digital-experiments-1.1.0/tests/test_util.py
```

### Comparing `digital-experiments-1.0.8/LICENSE` & `digital-experiments-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/PKG-INFO` & `digital-experiments-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.0.8
+Version: 1.1.0
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.0.8/README.md` & `digital-experiments-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/pyproject.toml` & `digital-experiments-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digital-experiments"
-version = "1.0.8"
+version = "1.1.0"
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
-current_version = "1.0.8"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digital-experiments-1.0.8/src/digital_experiments/backends.py` & `digital-experiments-1.1.0/src/digital_experiments/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import pickle
 import shutil
 from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass
 from functools import partial
 from pathlib import Path
 from typing import Dict, List
 
@@ -188,14 +189,32 @@
             df = pd.read_csv(self.csv_file, dtype={"id": str})
 
         return [
             Observation(**unflatten(row, self.SEPARATOR)) for _, row in df.iterrows()
         ]
 
 
+@this_is_a_backend("pickle")
+class PickleBackend(Backend):
+    def save(self, obs: Observation):
+        file = self.home / obs.id / "observation.pickle"
+        file.parent.mkdir(parents=True, exist_ok=True)
+
+        with exclusive_file_access(file, "wb") as f:
+            pickle.dump(obs, f)
+
+    def all_observations(self) -> List[Observation]:
+        files = sorted(self.home.glob("**/observation.pickle"))
+        observations = []
+        for f in files:
+            with exclusive_file_access(f, "rb") as f:
+                observations.append(pickle.load(f))
+        return observations
+
+
 class Files:
     LABEL = ".digital-experiment"
     RUNS = "runs"
 
 
 @dataclass
 class HomeLabel:
```

### Comparing `digital-experiments-1.0.8/src/digital_experiments/control_center.py` & `digital-experiments-1.1.0/src/digital_experiments/control_center.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/experiment.py` & `digital-experiments-1.1.0/src/digital_experiments/experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/metadata.py` & `digital-experiments-1.1.0/src/digital_experiments/metadata.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/minimize.py` & `digital-experiments-1.1.0/src/digital_experiments/minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/observation.py` & `digital-experiments-1.1.0/src/digital_experiments/observation.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/pretty.py` & `digital-experiments-1.1.0/src/digital_experiments/pretty.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,17 @@
 
 
 def pretty_instance(class_name, *things, **keywords) -> str:
     """
     make a pretty representation of an instance of a class
     """
 
-    all_things = list(map(str, things)) + [
-        f"{k}={v}" for k, v in keywords.items()
-    ]
+    all_things = list(map(str, things)) + [f"{k}={v}" for k, v in keywords.items()]
 
     naive_rep = f"{class_name}({', '.join(all_things)})"
     if len(naive_rep) < 80:
         return naive_rep
 
     # if the naive representation is too long, we try to make it more readable
     # by putting each argument on a new line
-    padded_things = "\n".join(pad(thing) for thing in all_things)
+    padded_things = "\n".join(pad(thing, "    ") + "," for thing in all_things)
     return f"{class_name}(\n{padded_things}\n)"
```

### Comparing `digital-experiments-1.0.8/src/digital_experiments/querying.py` & `digital-experiments-1.1.0/src/digital_experiments/querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/search/skopt_suggest.py` & `digital-experiments-1.1.0/src/digital_experiments/search/skopt_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/search/space.py` & `digital-experiments-1.1.0/src/digital_experiments/search/space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/search/suggest.py` & `digital-experiments-1.1.0/src/digital_experiments/search/suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments/util.py` & `digital-experiments-1.1.0/src/digital_experiments/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,25 +92,17 @@
     return set.union(*[set(t) for t in things])
 
 
 def intersect(things):
     return set.intersection(*[set(t) for t in things])
 
 
-def is_in(thing):
-    def _is_in(things):
-        return thing in things
-
-    return _is_in
-
-
 @contextmanager
 def exclusive_file_access(filehandle: Union[str, Path], mode: str = "r"):
-    if isinstance(filehandle, str):
-        filehandle = Path(filehandle)
+    filehandle = Path(filehandle)
 
     lock_path = filehandle.with_suffix(".lock")
     lock = FileLock(lock_path)
     with lock:
         if not filehandle.exists():
             filehandle.touch()
         with open(filehandle, mode) as f:
```

### Comparing `digital-experiments-1.0.8/src/digital_experiments/version_control.py` & `digital-experiments-1.1.0/src/digital_experiments/version_control.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/src/digital_experiments.egg-info/PKG-INFO` & `digital-experiments-1.1.0/src/digital_experiments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digital-experiments
-Version: 1.0.8
+Version: 1.1.0
 Summary: Keep track of digital experiments.
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: Copyright 2022 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `digital-experiments-1.0.8/src/digital_experiments.egg-info/SOURCES.txt` & `digital-experiments-1.1.0/src/digital_experiments.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,11 +22,12 @@
 src/digital_experiments/search/space.py
 src/digital_experiments/search/suggest.py
 tests/test_backends.py
 tests/test_control_center.py
 tests/test_experiment.py
 tests/test_metadata.py
 tests/test_minimize.py
+tests/test_pretty.py
 tests/test_querying.py
 tests/test_space.py
 tests/test_suggest.py
 tests/test_util.py
```

### Comparing `digital-experiments-1.0.8/tests/test_backends.py` & `digital-experiments-1.1.0/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/tests/test_experiment.py` & `digital-experiments-1.1.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/tests/test_metadata.py` & `digital-experiments-1.1.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/tests/test_minimize.py` & `digital-experiments-1.1.0/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/tests/test_querying.py` & `digital-experiments-1.1.0/tests/test_querying.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/tests/test_space.py` & `digital-experiments-1.1.0/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/tests/test_suggest.py` & `digital-experiments-1.1.0/tests/test_suggest.py`

 * *Files identical despite different names*

### Comparing `digital-experiments-1.0.8/tests/test_util.py` & `digital-experiments-1.1.0/tests/test_util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+import sys
+
+import pytest
+
+from digital_experiments import experiment
 from digital_experiments.util import (
     dict_equality,
     flatten,
     generate_id,
+    get_passed_kwargs,
+    get_passed_kwargs_for,
     intersect,
     unflatten,
     union,
 )
 
 nested = {"a": 1, "b": {"c": 2, "d": {"f": "hi"}}}
 flat = {"a": 1, "b_c": 2, "b_d_f": "hi"}
@@ -47,7 +54,29 @@
     nested2 = {"a": 1, "b": {"c": 2, "d": {"f": "bye"}}}
     assert not dict_equality(nested1, nested2)
 
     assert not dict_equality({"a": 1, "b": 2}, nested1)
     assert not dict_equality(nested1, {"a": 1, "b": 2})
 
     assert not dict_equality({"a": 1, "b": 2}, {"a": 1, "b": 2, "c": 3})
+
+
+def test_kwarg_parsing(tmp_path):
+    sys.argv = ["test.py", "a=1", "b=2", "c=3", "d"]
+    with pytest.raises(ValueError, match="Invalid keyword argument passed"):
+        get_passed_kwargs()
+
+    sys.argv = ["test.py", "a=1", "b=False", "c=hello"]
+
+    # get_passed_kwargs should return a dict of strings
+    assert get_passed_kwargs() == {"a": "1", "b": "False", "c": "hello"}
+
+    @experiment(absolute_root=tmp_path)
+    def test_experiment(a: int, b=False, *, c: str):
+        return a + int(b) + len(c)
+
+    # get_passed_kwargs_for should return a dict of the correct types
+    # by inferring them either from
+    #  - the defaults in a signature
+    #  - type hints
+    kwargs = get_passed_kwargs_for(test_experiment)
+    assert kwargs == {"a": 1, "b": False, "c": "hello"}
```

