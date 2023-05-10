# Comparing `tmp/treestamps-0.4.0.tar.gz` & `tmp/treestamps-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treestamps-0.4.0.tar", max compression
+gzip compressed data, was "treestamps-0.4.1.tar", max compression
```

## Comparing `treestamps-0.4.0.tar` & `treestamps-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-05-10 01:13:54.325343 treestamps-0.4.0/LICENSE
--rw-r--r--   0        0        0      979 2023-05-10 01:13:54.325343 treestamps-0.4.0/NEWS.md
--rw-r--r--   0        0        0     1443 2023-05-10 01:13:54.325343 treestamps-0.4.0/README.md
--rw-r--r--   0        0        0     3906 2023-05-10 01:13:54.325343 treestamps-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-05-10 01:13:54.325343 treestamps-0.4.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     1940 2023-05-10 01:13:54.325343 treestamps-0.4.0/tests/unit/test_classmethods.py
--rw-r--r--   0        0        0      703 2023-05-10 01:13:54.325343 treestamps-0.4.0/tests/unit/test_staticmethods.py
--rw-r--r--   0        0        0      172 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/__init__.py
--rw-r--r--   0        0        0     1490 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/config.py
--rw-r--r--   0        0        0     2259 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/grove.py
--rw-r--r--   0        0        0      300 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/tree/__init__.py
--rw-r--r--   0        0        0     3268 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/tree/common.py
--rw-r--r--   0        0        0     1217 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/tree/dump.py
--rw-r--r--   0        0        0      977 2023-05-10 01:13:54.325343 treestamps-0.4.0/treestamps/tree/get.py
--rw-r--r--   0        0        0     4738 2023-05-10 01:13:54.329343 treestamps-0.4.0/treestamps/tree/load.py
--rw-r--r--   0        0        0     2364 2023-05-10 01:13:54.329343 treestamps-0.4.0/treestamps/tree/set.py
--rw-r--r--   0        0        0     1276 2023-05-10 01:13:54.329343 treestamps-0.4.0/treestamps/tree/write.py
--rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 treestamps-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 03:42:57.963602 treestamps-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1072 2023-05-10 03:42:57.963602 treestamps-0.4.1/NEWS.md
+-rw-r--r--   0        0        0     1443 2023-05-10 03:42:57.963602 treestamps-0.4.1/README.md
+-rw-r--r--   0        0        0     3906 2023-05-10 03:42:57.963602 treestamps-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-05-10 03:42:57.963602 treestamps-0.4.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1940 2023-05-10 03:42:57.963602 treestamps-0.4.1/tests/unit/test_classmethods.py
+-rw-r--r--   0        0        0      703 2023-05-10 03:42:57.963602 treestamps-0.4.1/tests/unit/test_staticmethods.py
+-rw-r--r--   0        0        0      172 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/__init__.py
+-rw-r--r--   0        0        0     1569 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/config.py
+-rw-r--r--   0        0        0     2259 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/grove.py
+-rw-r--r--   0        0        0      300 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/__init__.py
+-rw-r--r--   0        0        0     3273 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/common.py
+-rw-r--r--   0        0        0     1217 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/dump.py
+-rw-r--r--   0        0        0      977 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/get.py
+-rw-r--r--   0        0        0     4766 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/load.py
+-rw-r--r--   0        0        0     2364 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/set.py
+-rw-r--r--   0        0        0     1276 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/write.py
+-rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 treestamps-0.4.1/PKG-INFO
```

### Comparing `treestamps-0.4.0/LICENSE` & `treestamps-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/NEWS.md` & `treestamps-0.4.1/NEWS.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # 📰 Treestamps News
 
+## v0.4.1
+
+- Fix
+  - Most paths generated improperly.
+  - check_config = False would crash.
+
 ## v0.4.0
 
 - Features
   - Big API Changes see README
 - Dev
   - Refactor into different files.
```

### Comparing `treestamps-0.4.0/README.md` & `treestamps-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/pyproject.toml` & `treestamps-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "treestamps"
-version = "0.4.0"
+version = "0.4.1"
 description = "Create timestamp records for recursive operations on directory trees."
 authors = ["AJ Slater <aj@slater.net>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/ajslater/treestamps"
 documentation = "https://github.com/ajslater/treestamps"
 keywords = ["timestamps", "library", "recursive", "directory"]
```

### Comparing `treestamps-0.4.0/tests/unit/test_classmethods.py` & `treestamps-0.4.1/tests/unit/test_classmethods.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/tests/unit/test_staticmethods.py` & `treestamps-0.4.1/tests/unit/test_staticmethods.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/treestamps/config.py` & `treestamps-0.4.1/treestamps/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,17 @@
             new_config[key] = normalize_config(value)
         else:
             new_config[key] = value
 
     return new_config
 
 
+DEFAULT_CONFIG = normalize_config({"ignore": frozenset(), "symlinks": True})
+
+
 @dataclass
 class CommonConfig:
     """Common Config meant to be subclassed."""
 
     program_name: str
     verbose: int = 0
     symlinks: bool = True
```

### Comparing `treestamps-0.4.0/treestamps/grove.py` & `treestamps-0.4.1/treestamps/grove.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/treestamps/tree/common.py` & `treestamps-0.4.1/treestamps/tree/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         for key in CONFIG_KEYS:
             config[key] = getattr(self._config, key)
         return normalize_config(config)
 
     def _to_absolute_path(self, root: Path, path: Path) -> Optional[Path]:
         """Convert paths to relevant absolute paths."""
         full_path = path if path.is_absolute() else root / path
-        full_path = path.resolve()
+        full_path = full_path.resolve()
 
         if not full_path.is_relative_to(self.root_dir):
             if self.root_dir.is_relative_to(full_path):
                 full_path = self.root_dir
             else:
                 if self._config.verbose:
                     cprint(
```

### Comparing `treestamps-0.4.0/treestamps/tree/dump.py` & `treestamps-0.4.1/treestamps/tree/dump.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/treestamps/tree/get.py` & `treestamps-0.4.1/treestamps/tree/get.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/treestamps/tree/load.py` & `treestamps-0.4.1/treestamps/tree/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Load methods."""
 from pathlib import Path
 
 from termcolor import cprint
 
-from treestamps.config import normalize_config
+from treestamps.config import DEFAULT_CONFIG, normalize_config
 from treestamps.tree.get import GetMixin
 
 
 class LoadMixin(GetMixin):
     """Load methods."""
 
     def _is_path_ignored(self, path: Path) -> bool:
@@ -25,23 +25,23 @@
             if full_path not in self._timestamps or old_ts is None or ts > old_ts:
                 self._timestamps[full_path] = ts
         except Exception as exc:
             cprint(f"WARNING: Invalid timestamp for {path_str}: {ts} {exc}", "yellow")
 
     def _load_timestamps_file_config_matches(self, yaml):
         """Return if the configured and loaded configs match."""
+        yaml_ts_config = yaml.pop(self._TREESTAMPS_CONFIG_TAG, DEFAULT_CONFIG)
+        yaml_program_config = yaml.pop(self._CONFIG_TAG, None)
         if not self._config.check_config:
             return True
 
-        yaml_ts_config = yaml.pop(self._TREESTAMPS_CONFIG_TAG, {})
         ts_config = self._get_treestamps_config_dict()
         if yaml_ts_config != ts_config:
             return False
 
-        yaml_program_config = yaml.pop(self._CONFIG_TAG, None)
         yaml_program_config = normalize_config(yaml_program_config)
         if self._config.program_config != yaml_program_config:
             # Only load timestamps for comparable configs
             return False
 
         return True
```

### Comparing `treestamps-0.4.0/treestamps/tree/set.py` & `treestamps-0.4.1/treestamps/tree/set.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/treestamps/tree/write.py` & `treestamps-0.4.1/treestamps/tree/write.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.0/PKG-INFO` & `treestamps-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treestamps
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create timestamp records for recursive operations on directory trees.
 Home-page: https://github.com/ajslater/treestamps
 License: GPL-3.0-only
 Keywords: timestamps,library,recursive,directory
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.9,<4.0
```

