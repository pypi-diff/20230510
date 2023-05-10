# Comparing `tmp/treestamps-0.3.4.tar.gz` & `tmp/treestamps-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treestamps-0.3.4.tar", max compression
+gzip compressed data, was "treestamps-0.4.0.tar", max compression
```

## Comparing `treestamps-0.3.4.tar` & `treestamps-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-04-03 08:37:59.661198 treestamps-0.3.4/LICENSE
--rw-r--r--   0        0        0      909 2023-04-03 08:37:59.661198 treestamps-0.3.4/NEWS.md
--rw-r--r--   0        0        0      311 2023-04-03 08:37:59.661198 treestamps-0.3.4/README.md
--rw-r--r--   0        0        0     3476 2023-04-03 08:37:59.665198 treestamps-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1380 2023-04-03 08:37:59.665198 treestamps-0.3.4/tests/unit/test_classmethods.py
--rw-r--r--   0        0        0      942 2023-04-03 08:37:59.665198 treestamps-0.3.4/tests/unit/test_staticmethods.py
--rw-r--r--   0        0        0    15816 2023-04-03 08:37:59.665198 treestamps-0.3.4/treestamps.py
--rw-r--r--   0        0        0     1536 1970-01-01 00:00:00.000000 treestamps-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 01:13:54.325343 treestamps-0.4.0/LICENSE
+-rw-r--r--   0        0        0      979 2023-05-10 01:13:54.325343 treestamps-0.4.0/NEWS.md
+-rw-r--r--   0        0        0     1443 2023-05-10 01:13:54.325343 treestamps-0.4.0/README.md
+-rw-r--r--   0        0        0     3906 2023-05-10 01:13:54.325343 treestamps-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-05-10 01:13:54.325343 treestamps-0.4.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1940 2023-05-10 01:13:54.325343 treestamps-0.4.0/tests/unit/test_classmethods.py
+-rw-r--r--   0        0        0      703 2023-05-10 01:13:54.325343 treestamps-0.4.0/tests/unit/test_staticmethods.py
+-rw-r--r--   0        0        0      172 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/__init__.py
+-rw-r--r--   0        0        0     1490 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/config.py
+-rw-r--r--   0        0        0     2259 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/grove.py
+-rw-r--r--   0        0        0      300 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/tree/__init__.py
+-rw-r--r--   0        0        0     3268 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/tree/common.py
+-rw-r--r--   0        0        0     1217 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/tree/dump.py
+-rw-r--r--   0        0        0      977 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/tree/get.py
+-rw-r--r--   0        0        0     4738 2023-05-10 01:13:54.329343 treestamps-0.4.0/treestamps/tree/load.py
+-rw-r--r--   0        0        0     2364 2023-05-10 01:13:54.329343 treestamps-0.4.0/treestamps/tree/set.py
+-rw-r--r--   0        0        0     1276 2023-05-10 01:13:54.329343 treestamps-0.4.0/treestamps/tree/write.py
+-rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 treestamps-0.4.0/PKG-INFO
```

### Comparing `treestamps-0.3.4/LICENSE` & `treestamps-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `treestamps-0.3.4/NEWS.md` & `treestamps-0.4.0/NEWS.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,73 @@
 # 📰 Treestamps News
 
-## v0.3.4
+## v0.4.0
 
+- Features
+  - Big API Changes see README
 - Dev
+  - Refactor into different files.
+
+## v0.3.4
 
+- Dev
   - Update dependencies.
 
 ## v0.3.3
 
 - Features
-
   - Update dependencies & poetry lockfile
 
 ## v0.3.2
 
 - Features
-
   - Update dependencies & poetry lockfile
 
 ## v0.3.1
 
 - Fix
-
-  - Fix factory passed strings instead of paths crash.
+  - Factory passed strings instead of paths crash.
 
 ## v0.3.0
 
 - Fix
 
-  - Fix factory consuming child timestamps when given files not directories.
-  - Fix loading and dumping timestamps not related to the treestamp dir.
+  - Factory consuming child timestamps when given files not directories.
+  - Loading and dumping timestamps not related to the treestamp dir.
 
 - Features
-
   - Ignore symlinks option.
 
 ## v0.2.1
 
 - Fix
-
   - Support ignore in factory
 
 ## v0.2.0
 
 - Features
-
   - Support ignore globs
 
 ## v0.1.3
 
 - Fixes
-
   - Protect final dump yaml from child cleanup task.
 
 ## v0.1.2
 
 - Features
 
-  - colored output.
+  - Colored output.
 
 - Fixes
 
   - Trap more errors when reading timestamps
 
 ## v0.1.1
 
 - Fixes
-
   - Fix strings submitted to factory instead of paths
 
 ## v0.1.0
 
-_First Release_
-
-- Picopt's new timestamper abstracted to a library
+- Features
+  - Picopt's new timestamper abstracted to a library
```

### Comparing `treestamps-0.3.4/pyproject.toml` & `treestamps-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "treestamps"
-version = "0.3.4"
+version = "0.4.0"
 description = "Create timestamp records for recursive operations on directory trees."
 authors = ["AJ Slater <aj@slater.net>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/ajslater/treestamps"
 documentation = "https://github.com/ajslater/treestamps"
 keywords = ["timestamps", "library", "recursive", "directory"]
@@ -17,15 +17,15 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-packages = [{ include = "treestamps.py" }, { include = "tests", format = "sdist" }]
+packages = [{ include = "treestamps" }, { include = "tests", format = "sdist" }]
 include = ["NEWS.md"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 "ruamel.yaml" = "^0.17.21"
 termcolor = "^2.0.1"
 
@@ -35,15 +35,15 @@
 coverage = { extras = ["toml"], version = "^7.0" }
 neovim = "^0.3.1"
 pyright = "^1.1.237"
 pytest = "^7.0.0"
 pytest-cov = "^4.0"
 pytest-gitignore = "^1.3"
 radon = { version = "^6.0.1", extras = ["toml"]}
-ruff = "^0.0.260"
+ruff = "^0.0.265"
 vulture = "^2.1"
 
 [tool.poetry.urls]
 "Source" = "https://github.com/ajslater/treestamps"
 "Issues" = "https://github.com/ajslater/treestamps/issues"
 
 [tool.black]
@@ -104,34 +104,45 @@
   ".mypy_cache",
   ".pytest_cache",
   ".venv",
   "dist",
   "package-lock.json",
   "poetry.lock",
   "test-results",
+  "treestamps/__init__.py",
   "typings",
   "vulture_whitelist.py"
 ]
 useLibraryCodeForTypes = true
 reportMissingImports = true
 reportImportCycles = true
 
 [tool.radon]
 exclude = "*~,.git/*,.mypy_cache/*,.pytest_cache/*,.venv/*,__pycache__/*,dist/*,node_modules/*,test-results/*,typings/*"
 
 [tool.ruff]
 extend-exclude = ["cache", "typings"]
 extend-ignore = ["S101", "D203", "D213"]
-extend-select = ["B", "B9", "C", "D", "I", "N", "S", "W"]
-# external = ["V101"]
+#extend-select = ["B", "B9", "C", "D", "I", "N", "S", "W"]
+extend-select = ["A", "ARG", "B", "B9", "C", "C4", "C90", "D", "DJ",
+  "DTZ", "E", "EM", "EXE", "F", "I", "ICN", "INP", "ISC", "PIE", "PL",
+  "PT", "PTH", "PYI", "Q", "N", "RET", "RSE", "RUF", "S", "SIM", "SLF",
+  "T10", "T20", "TCH", "TID", "TRY", "UP", "W", "YTT"
+  # "ANN", "ERA", "COM"
+]
+external = ["V101"]
 # format = "grouped"
 # show-source = true
 target-version = "py39"
 task-tags = ["TODO", "FIXME", "XXX", "http", "HACK"]
 
+[tool.ruff.per-file-ignores]
+"test_*" = ["SLF001"]
+"treestamps/__init__.py" = ["F401"]
+
 [tool.ruff.pycodestyle]
 ignore-overlong-task-comments = true
 
 [tool.vulture]
-exclude = [".git/", ".mypy_cache/", ".pytest_cache", ".venv", "*__pycache__*"]
+exclude = [".git/", ".mypy_cache/", ".pytest_cache", ".venv", "*__pycache__*", "treestamps/__init__.py"]
 min_confidence = 61
 sort_by_size = true
```

### Comparing `treestamps-0.3.4/tests/unit/test_staticmethods.py` & `treestamps-0.4.0/tests/unit/test_staticmethods.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 """Test static methods."""
 from pathlib import Path
 
-from treestamps import Treestamps
+from treestamps.tree import Treestamps
 
 __all__ = ()
 
 
 class TestStaticMethods:
     """Test static methods."""
 
-    def test_dirpath(self):
+    def test_get_dir(self):
         """Test dirpath."""
         file_path = Path(__file__).resolve()
         dir_path = file_path.parent
-        assert Treestamps.dirpath(dir_path) == dir_path
-        assert Treestamps.dirpath(file_path) == dir_path
+        assert Treestamps.get_dir(dir_path) == dir_path
+        assert Treestamps.get_dir(file_path) == dir_path
 
     def test_maxnone(self):
         """Test maxnone."""
-        assert Treestamps.max_none(1, 2) == 2
-        assert Treestamps.max_none(None, 2) == 2
+        assert Treestamps.max_none(1, 2) == 2  # noqa PLR2004
+        assert Treestamps.max_none(None, 2) == 2  # noqa PLR2004
         assert Treestamps.max_none(1, None) == 1
         assert Treestamps.max_none(None, None) is None
-
-    def test_prune_dict(self):
-        """Test prune dict."""
-        assert Treestamps.prune_dict(None, ["a"]) is None
-        assert Treestamps.prune_dict({"a": 1, "b": 2}, None) == {"a": 1, "b": 2}
-        assert Treestamps.prune_dict({"a": 1, "b": 2}, ["a"]) == {"a": 1}
```

### Comparing `treestamps-0.3.4/PKG-INFO` & `treestamps-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treestamps
-Version: 0.3.4
+Version: 0.4.0
 Summary: Create timestamp records for recursive operations on directory trees.
 Home-page: https://github.com/ajslater/treestamps
 License: GPL-3.0-only
 Keywords: timestamps,library,recursive,directory
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.9,<4.0
@@ -27,12 +27,59 @@
 Description-Content-Type: text/markdown
 
 # Treestamps
 
 A library to set and retrieve timestamps to speed up operations
 run recursively on directory trees.
 
-Principal methods on the Treestamps class are: init(), get(), set(), dump().
-A factory method is also provided for creating top path to Treestamp maps.
+Documentation is pretty poor. Read the code for now.
 
-Documentation is to read the code for now.
+## Usage
+
+Used in [picopt](https://github.com/ajsater/picopt) and
+[nudebomb](https://github.com/ajsater/nudebomb). You can see how it's
+used in those projects.
+
+```python
+    from treestamps import Copsestamps, CopsestampsConfig
+
+    config = GrovestampsConfig(
+        "MyProgramName",
+        paths=["/foo", "/bar"],
+        program_config={ "optionA": True, "optionB": False}
+    )
+    cs = Grovestamps(config)
+
+    timestamp = cs["/foo"].get()
+    cs["/foo"].set()
+
+    cs["/foo"].dump()
+
+    cs.dump()
+```
+
+## Breaking Changes from 0.3.x
+
+### Renamed
+
+Treestamps.dirpath() -> Treestamps.get_dir()
+Treestamps.dir -> Treestamps.root_dir
+
+### Made Private
+
+Treestamps.prune_dict() -> Treestamps.\_prune_dict()
+Treestamps.consume_all_child_timestamps() -> Treestamps.\_consume_all_child_timestamps()
+
+### Added
+
+Treestamps.add_consumed_path(), for legacy treestamps importers to remove old files.
+Copsestamps() is the ubquitous dir of rootpaths to Treestamps.
+
+### Changed
+
+Grovestamps() and Treestamps() both require a GrovestampsConfig or TreestampsConfig
+respectively as their sole param.
+
+Treestamps now record the ignored and symlinks config options in the file and if they
+change the file is not loaded.
+This is optional with the `check_config` configuration option.
```

