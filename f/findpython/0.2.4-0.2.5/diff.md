# Comparing `tmp/findpython-0.2.4.tar.gz` & `tmp/findpython-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findpython-0.2.4.tar", last modified: Tue Jan 31 04:43:09 2023, max compression
+gzip compressed data, was "findpython-0.2.5.tar", last modified: Wed May 10 08:28:07 2023, max compression
```

## Comparing `findpython-0.2.4.tar` & `findpython-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-31 04:42:55.856444 findpython-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-01-31 04:42:55.856444 findpython-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-01-31 04:42:55.856444 findpython-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/pep514tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/pep514tools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/pep514tools/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/pep514tools/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/providers/asdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/providers/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-01-31 04:42:55.856444 findpython-0.2.4/src/findpython/providers/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-01-31 04:42:55.860444 findpython-0.2.4/src/findpython/providers/pep514.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-31 04:42:55.860444 findpython-0.2.4/src/findpython/providers/pyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-01-31 04:42:55.860444 findpython-0.2.4/src/findpython/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-01-31 04:42:55.860444 findpython-0.2.4/src/findpython/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 04:42:55.860444 findpython-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-01-31 04:42:55.860444 findpython-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-31 04:42:55.860444 findpython-0.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-01-31 04:42:55.860444 findpython-0.2.4/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-01-31 04:42:55.860444 findpython-0.2.4/tests/test_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-01-31 04:42:55.860444 findpython-0.2.4/tests/test_utils.py
--rw-------   0 runner    (1001) docker     (123)     4938 2023-01-31 04:43:09.920751 findpython-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-10 08:27:49.053817 findpython-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4389 2023-05-10 08:27:49.053817 findpython-0.2.5/README.md
+-rw-r--r--   0        0        0     1291 2023-05-10 08:27:49.053817 findpython-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1474 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/__init__.py
+-rw-r--r--   0        0        0     2335 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/__version__.py
+-rw-r--r--   0        0        0     6201 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/finder.py
+-rw-r--r--   0        0        0      442 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/pep514tools/__init__.py
+-rw-r--r--   0        0        0      254 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/pep514tools/__main__.py
+-rw-r--r--   0        0        0     6631 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/pep514tools/_registry.py
+-rw-r--r--   0        0        0     4637 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/pep514tools/environment.py
+-rw-r--r--   0        0        0      724 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/__init__.py
+-rw-r--r--   0        0        0     1078 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/asdf.py
+-rw-r--r--   0        0        0     1555 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/base.py
+-rw-r--r--   0        0        0      779 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/macos.py
+-rw-r--r--   0        0        0      682 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/path.py
+-rw-r--r--   0        0        0     1269 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/pep514.py
+-rw-r--r--   0        0        0     1092 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/providers/pyenv.py
+-rw-r--r--   0        0        0     6344 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/python.py
+-rw-r--r--   0        0        0     4056 2023-05-10 08:27:49.053817 findpython-0.2.5/src/findpython/utils.py
+-rw-r--r--   0        0        0        0 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     1689 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0      613 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/test_cli.py
+-rw-r--r--   0        0        0     4814 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/test_finder.py
+-rw-r--r--   0        0        0     1489 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/test_posix.py
+-rw-r--r--   0        0        0      681 2023-05-10 08:27:49.053817 findpython-0.2.5/tests/test_utils.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 findpython-0.2.5/PKG-INFO
```

### Comparing `findpython-0.2.4/LICENSE` & `findpython-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/README.md` & `findpython-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/pyproject.toml` & `findpython-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
-version = "0.2.4"
+version = "0.2.5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/frostming/findpython"
```

### Comparing `findpython-0.2.4/src/findpython/__init__.py` & `findpython-0.2.5/src/findpython/__init__.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/__main__.py` & `findpython-0.2.5/src/findpython/__main__.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/finder.py` & `findpython-0.2.5/src/findpython/finder.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/pep514tools/_registry.py` & `findpython-0.2.5/src/findpython/pep514tools/_registry.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/pep514tools/environment.py` & `findpython-0.2.5/src/findpython/pep514tools/environment.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/providers/__init__.py` & `findpython-0.2.5/src/findpython/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/providers/asdf.py` & `findpython-0.2.5/src/findpython/providers/asdf.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/providers/macos.py` & `findpython-0.2.5/src/findpython/providers/macos.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/providers/path.py` & `findpython-0.2.5/src/findpython/providers/path.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/providers/pep514.py` & `findpython-0.2.5/src/findpython/providers/pep514.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/providers/pyenv.py` & `findpython-0.2.5/src/findpython/providers/pyenv.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/src/findpython/python.py` & `findpython-0.2.5/src/findpython/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,17 +177,22 @@
         return self._run_script(script).strip()
 
     @lru_cache(maxsize=1024)
     def _run_script(self, script: str, timeout: float | None = None) -> str:
         """Run a script and return the output."""
         command = [self.executable.as_posix(), "-c", script]
         logger.debug("Running script: %s", command)
-        return subprocess.check_output(
-            command, input=None, stderr=subprocess.DEVNULL, timeout=timeout
-        ).decode("utf-8")
+        return subprocess.run(
+            command,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.DEVNULL,
+            timeout=timeout,
+            check=True,
+            text=True,
+        ).stdout
 
     def __lt__(self, other: PythonVersion) -> bool:
         """Sort by the version, then by length of the executable path."""
         return (self.version, len(self.executable.as_posix())) < (
             other.version,
             len(other.executable.as_posix()),
         )
```

### Comparing `findpython-0.2.4/src/findpython/utils.py` & `findpython-0.2.5/src/findpython/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
+import errno
 import hashlib
 import os
 import re
 import sys
 from functools import lru_cache
 from pathlib import Path
+from typing import Generator
 
 VERSION_RE = re.compile(
     r"(?P<major>\d+)(?:\.(?P<minor>\d+)(?:\.(?P<patch>[0-9]+))?)?\.?"
     r"(?:(?P<prerel>[abc]|rc|dev)(?:(?P<prerelversion>\d+(?:\.\d+)*))?)"
     r"?(?P<postdev>(\.post(?P<post>\d+))?(\.dev(?P<dev>\d+))?)?"
     r"(?:-(?P<architecture>32|64))?"
 )
@@ -37,17 +39,26 @@
         "|".join(PYTHON_IMPLEMENTATIONS),
         "|".join(KNOWN_EXTS),
     )
 )
 RE_MATCHER = re.compile(PY_MATCH_STR)
 
 
-def path_is_readable(path: Path) -> bool:
-    """Return True if the path is readable."""
-    return os.access(str(path), os.R_OK)
+def safe_iter_dir(path: Path) -> Generator[Path, None, None]:
+    """Iterate over a directory, returning an empty iterator if the path
+    is not a directory or is not readable.
+    """
+    if not os.access(str(path), os.R_OK) or not path.is_dir():
+        return
+    try:
+        yield from path.iterdir()
+    except OSError as exc:
+        if exc.errno == errno.EACCES:
+            return
+        raise
 
 
 @lru_cache(maxsize=1024)
 def path_is_known_executable(path: Path) -> bool:
     """
     Returns whether a given path is a known executable from known executable extensions
     or has the executable bit toggled.
```

### Comparing `findpython-0.2.4/tests/conftest.py` & `findpython-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/tests/test_cli.py` & `findpython-0.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/tests/test_finder.py` & `findpython-0.2.5/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/tests/test_posix.py` & `findpython-0.2.5/tests/test_posix.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/tests/test_utils.py` & `findpython-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `findpython-0.2.4/PKG-INFO` & `findpython-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findpython
-Version: 0.2.4
+Version: 0.2.5
 Summary: A utility to find python versions on your system
 License: MIT
 Author-email: Frost Ming <mianghong@gmail.com>
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findpython Version: 0.2.4 Summary: A utility to
+Metadata-Version: 2.1 Name: findpython Version: 0.2.5 Summary: A utility to
 find python versions on your system License: MIT Author-email: Frost Ming
 gmail.com> Requires-Python: >=3.7 Classifier: Programming Language :: Python ::
 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Project-URL: Homepage, https:
 //github.com/frostming/findpython Description-Content-Type: text/markdown #
 FindPython _A utility to find python versions on your system._ [![Tests](https:
```

