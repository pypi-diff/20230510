# Comparing `tmp/tinystream-0.0.4.tar.gz` & `tmp/tinystream-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinystream-0.0.4.tar", last modified: Wed Dec 14 11:40:19 2022, max compression
+gzip compressed data, was "tinystream-0.0.5.tar", last modified: Wed May 10 10:38:20 2023, max compression
```

## Comparing `tinystream-0.0.4.tar` & `tinystream-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2022-12-14 11:40:19.531034 tinystream-0.0.4/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.4/LICENSE
--rw-r--r--   0 mikereiche   (502) staff       (20)     3217 2022-12-14 11:40:19.530933 tinystream-0.0.4/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     2946 2022-12-14 11:39:38.000000 tinystream-0.0.4/README.md
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2022-12-14 11:40:19.531074 tinystream-0.0.4/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      490 2022-12-14 11:40:14.000000 tinystream-0.0.4/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2022-12-14 11:40:19.530795 tinystream-0.0.4/tinystream.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3217 2022-12-14 11:40:19.000000 tinystream-0.0.4/tinystream.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      176 2022-12-14 11:40:19.000000 tinystream-0.0.4/tinystream.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2022-12-14 11:40:19.000000 tinystream-0.0.4/tinystream.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       11 2022-12-14 11:40:19.000000 tinystream-0.0.4/tinystream.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)     4921 2022-12-14 11:36:33.000000 tinystream-0.0.4/tinystream.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-10 10:38:20.536895 tinystream-0.0.5/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.5/LICENSE
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3847 2023-05-10 10:38:20.536757 tinystream-0.0.5/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3613 2023-05-10 10:25:32.000000 tinystream-0.0.5/README.md
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-10 10:38:20.536933 tinystream-0.0.5/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      510 2023-05-10 10:37:44.000000 tinystream-0.0.5/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-10 10:38:20.536570 tinystream-0.0.5/tinystream.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3847 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       19 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5618 2023-05-10 10:20:05.000000 tinystream-0.0.5/tinystream.py
```

### Comparing `tinystream-0.0.4/LICENSE` & `tinystream-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tinystream-0.0.4/PKG-INFO` & `tinystream-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-Metadata-Version: 2.1
-Name: tinystream
-Version: 0.0.4
-Summary: Yet another python streams library
-Home-page: https://github.com/mreiche/python-streams
-Author: Mike Reiche
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
+![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
+[![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
 
 # tinystream / python-streams
 
 This is a simple and lightweight Streams API inspired by Java Streams with support for type hinting.
 
 This package is release as `tinystream` at pypi.
 
@@ -25,16 +17,17 @@
 stream \
     .map(lambda x: x + 1) \       # flatmap(), each(), next(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
-    .sum()                        # reduce(), max(), min()
+    .sum()                        # first, reduce(), max(), min()
 ```
+
 ## Typehinting
 
 Since Python does not support typed lambdas, this library implements a workaround.
 
 ```python
 from tinystream import Stream
 
@@ -61,16 +54,14 @@
     name: str
     parent: "Node" = None
 ```
 
 for lambdas:
 
 ```python
-from tinystream import Stream
-
 parent = Node(name="B")
 child = Node(name="A", parent=parent)
 
 stream = Stream.of([child])
 assert stream.map(lambda x: x.parent, typehint=Node).next().name == "B"
 ```
 
@@ -78,30 +69,49 @@
 ```python
 def map_parent(n: Node):
     return n.parent
 
 assert stream.map(map_parent).next().name == "B"
 ```
 
+## Retrieve optional
+
+The `first` property returns a [optional.py:Optional](https://pypi.org/project/optional.py/) 
+
+```python
+stream.first.is_present()
+```
+
 ## End of stream
 
 Calling methods like `sum()`, `collect()`, `count()`... will end the stream.
 
 ## More features
 
-### Filter by key existing
+### Filter by existing key
 ```python
 items_with_name = Stream.of([child]).filter_key("name")
 ```
 
-### Map name
+### Map object name attribute
 ```python
 names = Stream.of([child]).map_key("name")
 ```
 
+### Deep mapping of name attributes
+```python
+list = [
+   {"node": Node(name="Node A")},
+   {"node": Node(name="Node B")},
+   {"node": Node(name="Node C")},
+   {"node": Node(name="Node D")},
+]
+Stream.of(list).map_keys(("node", "name"))
+```
+
 ### Collected join
 
 ```python
 all_names = Stream.of([child]).map_key("name").join(", ")
 ```
 
 ### Stream dictionaries
@@ -125,15 +135,15 @@
 - https://github.com/9seconds/streams/ (*outdated*)
 - https://github.com/tolsac/streampy (*outdated*)
 - Apache Spark
 
 ## Run the tests
 
 ```shell
-PYTHONPATH="." pytest --cov=tinystream tests/
+PYTHONPATH="." pytest --cov=tinystream -n 4 tests/
 ```
 
 ### Release update
 1. Update version in `setup.py`
 2. Package library
     ```shell
     python setup.py sdist
@@ -143,9 +153,7 @@
     twine upload dist/tinystream-[version].tar.gz
     ```
 
 ## References
 
 - https://github.com/MichaelKim0407/tutorial-pip-package
 - https://packaging.python.org/en/latest/guides/making-a-pypi-friendly-readme/
-
-
```

### Comparing `tinystream-0.0.4/tinystream.egg-info/PKG-INFO` & `tinystream-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.0.4
+Version: 0.0.5
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
+[![Code Coverage Status](https://codecov.io/github/mreiche/python-streams/branch/main/graph/badge.svg)](https://app.codecov.io/github/mreiche/python-automation-framework)
+
 # tinystream / python-streams
 
 This is a simple and lightweight Streams API inspired by Java Streams with support for type hinting.
 
 This package is release as `tinystream` at pypi.
 
 ## Basic API
@@ -25,16 +26,17 @@
 stream \
     .map(lambda x: x + 1) \       # flatmap(), each(), next(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
-    .sum()                        # reduce(), max(), min()
+    .sum()                        # first, reduce(), max(), min()
 ```
+
 ## Typehinting
 
 Since Python does not support typed lambdas, this library implements a workaround.
 
 ```python
 from tinystream import Stream
 
@@ -61,16 +63,14 @@
     name: str
     parent: "Node" = None
 ```
 
 for lambdas:
 
 ```python
-from tinystream import Stream
-
 parent = Node(name="B")
 child = Node(name="A", parent=parent)
 
 stream = Stream.of([child])
 assert stream.map(lambda x: x.parent, typehint=Node).next().name == "B"
 ```
 
@@ -78,30 +78,49 @@
 ```python
 def map_parent(n: Node):
     return n.parent
 
 assert stream.map(map_parent).next().name == "B"
 ```
 
+## Retrieve optional
+
+The `first` property returns a [optional.py:Optional](https://pypi.org/project/optional.py/) 
+
+```python
+stream.first.is_present()
+```
+
 ## End of stream
 
 Calling methods like `sum()`, `collect()`, `count()`... will end the stream.
 
 ## More features
 
-### Filter by key existing
+### Filter by existing key
 ```python
 items_with_name = Stream.of([child]).filter_key("name")
 ```
 
-### Map name
+### Map object name attribute
 ```python
 names = Stream.of([child]).map_key("name")
 ```
 
+### Deep mapping of name attributes
+```python
+list = [
+   {"node": Node(name="Node A")},
+   {"node": Node(name="Node B")},
+   {"node": Node(name="Node C")},
+   {"node": Node(name="Node D")},
+]
+Stream.of(list).map_keys(("node", "name"))
+```
+
 ### Collected join
 
 ```python
 all_names = Stream.of([child]).map_key("name").join(", ")
 ```
 
 ### Stream dictionaries
@@ -125,15 +144,15 @@
 - https://github.com/9seconds/streams/ (*outdated*)
 - https://github.com/tolsac/streampy (*outdated*)
 - Apache Spark
 
 ## Run the tests
 
 ```shell
-PYTHONPATH="." pytest --cov=tinystream tests/
+PYTHONPATH="." pytest --cov=tinystream -n 4 tests/
 ```
 
 ### Release update
 1. Update version in `setup.py`
 2. Package library
     ```shell
     python setup.py sdist
@@ -143,9 +162,7 @@
     twine upload dist/tinystream-[version].tar.gz
     ```
 
 ## References
 
 - https://github.com/MichaelKim0407/tutorial-pip-package
 - https://packaging.python.org/en/latest/guides/making-a-pypi-friendly-readme/
-
-
```

### Comparing `tinystream-0.0.4/tinystream.py` & `tinystream-0.0.5/tinystream.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 import itertools
-from typing import Iterable, Generic, TypeVar, Callable, List, Iterator, Dict, Tuple
+from typing import Iterable, Generic, TypeVar, Callable, List, Dict, Tuple
+from optional import Optional
 
 T = TypeVar("T")
 R = TypeVar("R")
 K = TypeVar("K")
 
 
 class Stream:
@@ -20,15 +21,15 @@
     @staticmethod
     def of_many(typehint: T = None, *iterables):
         return IterableStream[T]([]).concat(*iterables)
 
 
 class IterableStream(Generic[T]):
 
-    def __normalize_iterator(self, iterable: Iterable[T]):
+    def __normalize_iterator(self, iterable: Iterable[T]) -> Iterable[T]:
         #if isinstance(iterable, Iterator):
 
         if isinstance(iterable, list):
             return iter(iterable)
         elif isinstance(iterable, dict):
             return iter(iterable.items())
         elif isinstance(iterable, str):
@@ -48,14 +49,30 @@
             if isinstance(x, (list, dict, tuple)):
                 return x[key]
             else:
                 return getattr(x, key)
 
         return self.filter_key(key).map(__map_key, R)
 
+    def map_keys(self, keys: Iterable[str], typehint: R = None) -> "IterableStream[R]":
+        def _map_keys():
+            for val in self.__iterable:
+                for key in keys:
+                    if isinstance(val, (list, dict, tuple)) and key in val:
+                        val = val[key]
+                    elif hasattr(val, key):
+                        val = getattr(val, key)
+                    else:
+                        val = None
+                        break
+                if val:
+                    yield val
+
+        return IterableStream[R](_map_keys())
+
     def filter(self, cb: Callable[[T, T], bool]):
         return IterableStream[T](filter(cb, self.__iterable))
 
     def filter_key(self, key: str | int, invert: bool = False):
         def __filter_key(x):
             if isinstance(x, (list, tuple)):
                 size = len(x)
@@ -110,14 +127,18 @@
 
     def next(self) -> T | None:
         try:
             return next(self.__iterable)
         except StopIteration as e:
             return None
 
+    @property
+    def first(self):
+        return Optional.of(self.next())
+
     def collect(self):
         """Collects all items to a list and ends the stream"""
         if not self.__collected:
             self.__collected = list(self.__iterable)
         return self.__collected
 
     def join(self, separator: str) -> str:
```

