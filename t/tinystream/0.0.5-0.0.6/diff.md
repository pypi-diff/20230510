# Comparing `tmp/tinystream-0.0.5.tar.gz` & `tmp/tinystream-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinystream-0.0.5.tar", last modified: Wed May 10 10:38:20 2023, max compression
+gzip compressed data, was "tinystream-0.0.6.tar", last modified: Wed May 10 12:29:50 2023, max compression
```

## Comparing `tinystream-0.0.5.tar` & `tinystream-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-10 10:38:20.536895 tinystream-0.0.5/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.5/LICENSE
--rw-r--r--   0 mikereiche   (502) staff       (20)     3847 2023-05-10 10:38:20.536757 tinystream-0.0.5/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     3613 2023-05-10 10:25:32.000000 tinystream-0.0.5/README.md
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-10 10:38:20.536933 tinystream-0.0.5/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      510 2023-05-10 10:37:44.000000 tinystream-0.0.5/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-10 10:38:20.536570 tinystream-0.0.5/tinystream.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     3847 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       19 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/requires.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-10 10:38:20.000000 tinystream-0.0.5/tinystream.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)     5618 2023-05-10 10:20:05.000000 tinystream-0.0.5/tinystream.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-10 12:29:50.024924 tinystream-0.0.6/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.6/LICENSE
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3829 2023-05-10 12:29:50.024795 tinystream-0.0.6/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3595 2023-05-10 11:02:57.000000 tinystream-0.0.6/README.md
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-10 12:29:50.024965 tinystream-0.0.6/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      510 2023-05-10 12:17:31.000000 tinystream-0.0.6/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-10 12:29:50.024608 tinystream-0.0.6/tinystream.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3829 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      209 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       19 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/requires.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-10 12:29:50.000000 tinystream-0.0.6/tinystream.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)     5950 2023-05-10 10:59:00.000000 tinystream-0.0.6/tinystream.py
```

### Comparing `tinystream-0.0.5/LICENSE` & `tinystream-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tinystream-0.0.5/PKG-INFO` & `tinystream-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.0.5
+Version: 0.0.6
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
@@ -20,15 +20,15 @@
 
 ```python
 from tinystream import Stream
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
-    .map(lambda x: x + 1) \       # flatmap(), each(), next(), peek(), map_key()
+    .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
     .sum()                        # first, reduce(), max(), min()
 ```
@@ -67,23 +67,23 @@
 for lambdas:
 
 ```python
 parent = Node(name="B")
 child = Node(name="A", parent=parent)
 
 stream = Stream.of([child])
-assert stream.map(lambda x: x.parent, typehint=Node).next().name == "B"
+assert next(stream.map(lambda x: x.parent, typehint=Node)).name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
-assert stream.map(map_parent).next().name == "B"
+assert next(stream.map(map_parent)).name == "B"
 ```
 
 ## Retrieve optional
 
 The `first` property returns a [optional.py:Optional](https://pypi.org/project/optional.py/) 
 
 ```python
```

### Comparing `tinystream-0.0.5/README.md` & `tinystream-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ```python
 from tinystream import Stream
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
-    .map(lambda x: x + 1) \       # flatmap(), each(), next(), peek(), map_key()
+    .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
     .sum()                        # first, reduce(), max(), min()
 ```
@@ -58,23 +58,23 @@
 for lambdas:
 
 ```python
 parent = Node(name="B")
 child = Node(name="A", parent=parent)
 
 stream = Stream.of([child])
-assert stream.map(lambda x: x.parent, typehint=Node).next().name == "B"
+assert next(stream.map(lambda x: x.parent, typehint=Node)).name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
-assert stream.map(map_parent).next().name == "B"
+assert next(stream.map(map_parent)).name == "B"
 ```
 
 ## Retrieve optional
 
 The `first` property returns a [optional.py:Optional](https://pypi.org/project/optional.py/) 
 
 ```python
```

### Comparing `tinystream-0.0.5/tinystream.egg-info/PKG-INFO` & `tinystream-0.0.6/tinystream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.0.5
+Version: 0.0.6
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
@@ -20,15 +20,15 @@
 
 ```python
 from tinystream import Stream
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
-    .map(lambda x: x + 1) \       # flatmap(), each(), next(), peek(), map_key()
+    .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
     .reverse() \                  # collect(), count()
     .limit(2) \
     .concat([4]) \
     .sum()                        # first, reduce(), max(), min()
 ```
@@ -67,23 +67,23 @@
 for lambdas:
 
 ```python
 parent = Node(name="B")
 child = Node(name="A", parent=parent)
 
 stream = Stream.of([child])
-assert stream.map(lambda x: x.parent, typehint=Node).next().name == "B"
+assert next(stream.map(lambda x: x.parent, typehint=Node)).name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
-assert stream.map(map_parent).next().name == "B"
+assert next(stream.map(map_parent)).name == "B"
 ```
 
 ## Retrieve optional
 
 The `first` property returns a [optional.py:Optional](https://pypi.org/project/optional.py/) 
 
 ```python
```

### Comparing `tinystream-0.0.5/tinystream.py` & `tinystream-0.0.6/tinystream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import functools
 import itertools
-from typing import Iterable, Generic, TypeVar, Callable, List, Dict, Tuple
+import logging
+from typing import Iterable, TypeVar, Callable, List, Dict, Tuple, Iterator
+import warnings
 from optional import Optional
 
 T = TypeVar("T")
 R = TypeVar("R")
 K = TypeVar("K")
 
 
@@ -19,15 +21,25 @@
         return IterableStream[Tuple[K, T]](source_dict)
 
     @staticmethod
     def of_many(typehint: T = None, *iterables):
         return IterableStream[T]([]).concat(*iterables)
 
 
-class IterableStream(Generic[T]):
+
+class IterableStream(Iterator[T]):
+
+    def __next__(self) -> T|None:
+        try:
+            return next(self.__iterable)
+        except StopIteration as e:
+            return None
+
+    def __iter__(self) -> Iterator[T]:
+        return self.__iterable.__iter__()
 
     def __normalize_iterator(self, iterable: Iterable[T]) -> Iterable[T]:
         #if isinstance(iterable, Iterator):
 
         if isinstance(iterable, list):
             return iter(iterable)
         elif isinstance(iterable, dict):
@@ -119,21 +131,20 @@
         return IterableStream[T](sort)
 
     def sorted(self, key, reverse: bool = False):
         sort = sorted(self.__iterable, key=key, reverse=reverse)
         return IterableStream[T](sort)
 
     def each(self) -> Iterable[T]:
+        warnings.warn("Use the stream as iterator instead", DeprecationWarning)
         return self.__iterable
 
     def next(self) -> T | None:
-        try:
-            return next(self.__iterable)
-        except StopIteration as e:
-            return None
+        warnings.warn("Use next(stream) instead", DeprecationWarning)
+        return self.__next__()
 
     @property
     def first(self):
         return Optional.of(self.next())
 
     def collect(self):
         """Collects all items to a list and ends the stream"""
```

