# Comparing `tmp/treestamps-0.4.1.tar.gz` & `tmp/treestamps-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treestamps-0.4.1.tar", max compression
+gzip compressed data, was "treestamps-0.4.2.tar", max compression
```

## Comparing `treestamps-0.4.1.tar` & `treestamps-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-05-10 03:42:57.963602 treestamps-0.4.1/LICENSE
--rw-r--r--   0        0        0     1072 2023-05-10 03:42:57.963602 treestamps-0.4.1/NEWS.md
--rw-r--r--   0        0        0     1443 2023-05-10 03:42:57.963602 treestamps-0.4.1/README.md
--rw-r--r--   0        0        0     3906 2023-05-10 03:42:57.963602 treestamps-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       13 2023-05-10 03:42:57.963602 treestamps-0.4.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     1940 2023-05-10 03:42:57.963602 treestamps-0.4.1/tests/unit/test_classmethods.py
--rw-r--r--   0        0        0      703 2023-05-10 03:42:57.963602 treestamps-0.4.1/tests/unit/test_staticmethods.py
--rw-r--r--   0        0        0      172 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/__init__.py
--rw-r--r--   0        0        0     1569 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/config.py
--rw-r--r--   0        0        0     2259 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/grove.py
--rw-r--r--   0        0        0      300 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/__init__.py
--rw-r--r--   0        0        0     3273 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/common.py
--rw-r--r--   0        0        0     1217 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/dump.py
--rw-r--r--   0        0        0      977 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/get.py
--rw-r--r--   0        0        0     4766 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/load.py
--rw-r--r--   0        0        0     2364 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/set.py
--rw-r--r--   0        0        0     1276 2023-05-10 03:42:57.963602 treestamps-0.4.1/treestamps/tree/write.py
--rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 treestamps-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 05:08:17.180783 treestamps-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1217 2023-05-10 05:08:17.180783 treestamps-0.4.2/NEWS.md
+-rw-r--r--   0        0        0     1443 2023-05-10 05:08:17.180783 treestamps-0.4.2/README.md
+-rw-r--r--   0        0        0     3906 2023-05-10 05:08:17.184783 treestamps-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-05-10 05:08:17.184783 treestamps-0.4.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1920 2023-05-10 05:08:17.184783 treestamps-0.4.2/tests/unit/test_classmethods.py
+-rw-r--r--   0        0        0      693 2023-05-10 05:08:17.184783 treestamps-0.4.2/tests/unit/test_staticmethods.py
+-rw-r--r--   0        0        0      172 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/__init__.py
+-rw-r--r--   0        0        0     1569 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/config.py
+-rw-r--r--   0        0        0     1965 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/grove.py
+-rw-r--r--   0        0        0      300 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/tree/__init__.py
+-rw-r--r--   0        0        0     3213 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/tree/common.py
+-rw-r--r--   0        0        0     1217 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/tree/dump.py
+-rw-r--r--   0        0        0      977 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/tree/get.py
+-rw-r--r--   0        0        0     4883 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/tree/load.py
+-rw-r--r--   0        0        0     2364 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/tree/set.py
+-rw-r--r--   0        0        0     1276 2023-05-10 05:08:17.184783 treestamps-0.4.2/treestamps/tree/write.py
+-rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 treestamps-0.4.2/PKG-INFO
```

### Comparing `treestamps-0.4.1/LICENSE` & `treestamps-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.1/NEWS.md` & `treestamps-0.4.2/NEWS.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # 📰 Treestamps News
 
+## v0.4.2
+
+- Fix
+  - Make treestamp paths all relative again like 0.3.x for portability
+  - Keep reading WAL if individual entries are corrupt.
+
 ## v0.4.1
 
 - Fix
   - Most paths generated improperly.
   - check_config = False would crash.
 
 ## v0.4.0
```

### Comparing `treestamps-0.4.1/README.md` & `treestamps-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.1/pyproject.toml` & `treestamps-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "treestamps"
-version = "0.4.1"
+version = "0.4.2"
 description = "Create timestamp records for recursive operations on directory trees."
 authors = ["AJ Slater <aj@slater.net>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://github.com/ajslater/treestamps"
 documentation = "https://github.com/ajslater/treestamps"
 keywords = ["timestamps", "library", "recursive", "directory"]
```

### Comparing `treestamps-0.4.1/tests/unit/test_classmethods.py` & `treestamps-0.4.2/tests/unit/test_classmethods.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,22 +42,22 @@
         }
 
         cc = CommonConfig(
             "Dummy", program_config_keys=keys, program_config={"a": {"b": [2, 1, 3, 1]}}
         )
         assert cc.program_config == {"a": {"b": [1, 2, 3]}}
 
-    def test_copse(self):
+    def test_grove(self):
         """Test the factory."""
-        path_a = Path(__file__).resolve()
+        path_a = Path(__file__)
         path_b = path_a.parent
         path_c = Path("/tmp")  # noqa
 
         paths = (path_a, path_b, path_c)
 
         config = GrovestampsConfig("Dummy", paths=paths)
         cs = Grovestamps(config)
 
-        dirset = {path_b.resolve(), path_c.resolve()}
+        dirset = {path_b.resolve(), path_c}
         assert set(cs.keys()) == dirset
         dirs = {ts.root_dir for ts in cs.values()}
         assert dirs == dirset
```

### Comparing `treestamps-0.4.1/tests/unit/test_staticmethods.py` & `treestamps-0.4.2/tests/unit/test_staticmethods.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class TestStaticMethods:
     """Test static methods."""
 
     def test_get_dir(self):
         """Test dirpath."""
-        file_path = Path(__file__).resolve()
+        file_path = Path(__file__)
         dir_path = file_path.parent
         assert Treestamps.get_dir(dir_path) == dir_path
         assert Treestamps.get_dir(file_path) == dir_path
 
     def test_maxnone(self):
         """Test maxnone."""
         assert Treestamps.max_none(1, 2) == 2  # noqa PLR2004
```

### Comparing `treestamps-0.4.1/treestamps/config.py` & `treestamps-0.4.2/treestamps/config.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.1/treestamps/grove.py` & `treestamps-0.4.2/treestamps/grove.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         This order creates dir based treestamps before files so dirs get children
         recursed and files only don't.
         """
         dirs = set()
         files = set()
         for path_str in self._config.paths:
-            path = Path(path_str).resolve()
+            path = Path(path_str)
             if not self._config.symlinks and path.is_symlink():
                 continue
             if path.is_dir():
                 dirs.add(path)
             else:
                 files.add(path)
         return tuple(sorted(dirs) + sorted(files))
@@ -53,21 +53,13 @@
             if root_dir in self:
                 continue
             tree_config = TreestampsConfig(**config_dict, path=top_path)
             ts = Treestamps(tree_config)
             self[root_dir] = ts
             ts.load()
 
-    def __getitem__(self, key):
-        """Resolve the path key before getting it."""
-        return super().__getitem__(key.resolve())
-
-    def __setitem__(self, key, val):
-        """Resolve the path key before setting it."""
-        return super().__setitem__(key.resolve(), val)
-
     def dump(self) -> None:
         """Dump all treestamps."""
         for top_path, treestamps in self.items():
             if self._config.verbose:
                 cprint(f"Saving timestamps for {top_path}")
             treestamps.dump()
```

### Comparing `treestamps-0.4.1/treestamps/tree/common.py` & `treestamps-0.4.2/treestamps/tree/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     _WAL_TAG = "wal"
     _FILENAME_TEMPLATE = ".{program_name}_treestamps.yaml"
     _WAL_FILENAME_TEMPLATE = ".{program_name}_treestamps.wal.yaml"
 
     @staticmethod
     def get_dir(path: Path):
         """Return a directory for a path."""
-        path = Path(path).resolve()
+        path = Path(path)
         return path if path.is_dir() else path.parent
 
     @classmethod
     def _get_filename(cls, program_name: str) -> str:
         """Return the timestamps filename for a program."""
         return cls._FILENAME_TEMPLATE.format(program_name=program_name)
 
@@ -59,15 +59,14 @@
         for key in CONFIG_KEYS:
             config[key] = getattr(self._config, key)
         return normalize_config(config)
 
     def _to_absolute_path(self, root: Path, path: Path) -> Optional[Path]:
         """Convert paths to relevant absolute paths."""
         full_path = path if path.is_absolute() else root / path
-        full_path = full_path.resolve()
 
         if not full_path.is_relative_to(self.root_dir):
             if self.root_dir.is_relative_to(full_path):
                 full_path = self.root_dir
             else:
                 if self._config.verbose:
                     cprint(
@@ -80,15 +79,15 @@
 
     def __init__(self, config: TreestampsConfig) -> None:
         """Initialize instance variables."""
         # config
         self._config = config
 
         # init variables
-        self.root_dir = self.get_dir(Path(self._config.path)).resolve()
+        self.root_dir = self.get_dir(Path(self._config.path))
         self._YAML = YAML()
         self._YAML.allow_duplicate_keys = True
         self._filename = self._get_filename(self._config.program_name)
         self._wal_filename = self._get_wal_filename(self._config.program_name)
         self._dump_path = self.root_dir / self._filename
         self._wal_path = self.root_dir / self._wal_filename
         self._wal: Optional[TextIO] = None
```

### Comparing `treestamps-0.4.1/treestamps/tree/dump.py` & `treestamps-0.4.2/treestamps/tree/dump.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.1/treestamps/tree/get.py` & `treestamps-0.4.2/treestamps/tree/get.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.1/treestamps/tree/load.py` & `treestamps-0.4.2/treestamps/tree/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,30 +51,31 @@
             return
 
         try:
             yaml = self._YAML.load(timestamps_path)
             if not yaml:
                 return
 
+            # pops off config entries.
             if not self._load_timestamps_file_config_matches(yaml):
                 return
 
             # WAL
-            try:
-                wal = yaml.pop(self._WAL_TAG)
-            except KeyError:
-                wal = []
+            wal = yaml.pop(self._WAL_TAG, [])
 
-            # Timestamps
+            # What's left are timestamps
             entries = list(yaml.items())
 
             # Wal entries afterwards
             for entry in wal:
-                for path_str, ts in entry.items():
-                    entries += [(path_str, ts)]
+                try:
+                    for path_str, ts in entry.items():
+                        entries += [(path_str, ts)]
+                except Exception as exc:
+                    cprint(f"WAL entry read: {exc}", "yellow")
 
             for path_str, ts in entries:
                 self._load_timestamp_entry(timestamps_path.parent, path_str, ts)
         except Exception as exc:
             cprint(f"ERROR: parsing timestamps file: {timestamps_path} {exc}", "red")
 
     def _consume_child_timestamps(self, path: Path) -> None:
```

### Comparing `treestamps-0.4.1/treestamps/tree/set.py` & `treestamps-0.4.2/treestamps/tree/set.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.1/treestamps/tree/write.py` & `treestamps-0.4.2/treestamps/tree/write.py`

 * *Files identical despite different names*

### Comparing `treestamps-0.4.1/PKG-INFO` & `treestamps-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treestamps
-Version: 0.4.1
+Version: 0.4.2
 Summary: Create timestamp records for recursive operations on directory trees.
 Home-page: https://github.com/ajslater/treestamps
 License: GPL-3.0-only
 Keywords: timestamps,library,recursive,directory
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.9,<4.0
```

