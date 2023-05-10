# Comparing `tmp/funcdesc-0.1.2.tar.gz` & `tmp/funcdesc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcdesc-0.1.2.tar", last modified: Mon Mar 13 03:00:31 2023, max compression
+gzip compressed data, was "funcdesc-0.1.3.tar", last modified: Wed May 10 14:39:51 2023, max compression
```

## Comparing `funcdesc-0.1.2.tar` & `funcdesc-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 03:00:31.566745 funcdesc-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-13 03:00:22.000000 funcdesc-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-13 03:00:22.000000 funcdesc-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-13 03:00:22.000000 funcdesc-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-13 03:00:31.566745 funcdesc-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-03-13 03:00:22.000000 funcdesc-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 03:00:31.566745 funcdesc-0.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 03:00:31.566745 funcdesc-0.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    36401 2023-03-13 03:00:22.000000 funcdesc-0.1.2/docs/images/concept.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 03:00:31.566745 funcdesc-0.1.2/funcdesc/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/mark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 03:00:31.566745 funcdesc-0.1.2/funcdesc/types/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/types/side_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/types/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 03:00:31.566745 funcdesc-0.1.2/funcdesc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-13 03:00:22.000000 funcdesc-0.1.2/funcdesc/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 03:00:31.566745 funcdesc-0.1.2/funcdesc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-13 03:00:31.000000 funcdesc-0.1.2/funcdesc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-13 03:00:31.000000 funcdesc-0.1.2/funcdesc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 03:00:31.000000 funcdesc-0.1.2/funcdesc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 03:00:31.000000 funcdesc-0.1.2/funcdesc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-13 03:00:31.000000 funcdesc-0.1.2/funcdesc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-13 03:00:31.000000 funcdesc-0.1.2/funcdesc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 03:00:31.566745 funcdesc-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-13 03:00:22.000000 funcdesc-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.619053 funcdesc-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-10 14:39:42.000000 funcdesc-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-10 14:39:42.000000 funcdesc-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 14:39:42.000000 funcdesc-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-10 14:39:51.619053 funcdesc-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-10 14:39:42.000000 funcdesc-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.615053 funcdesc-0.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.615053 funcdesc-0.1.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    36401 2023-05-10 14:39:42.000000 funcdesc-0.1.3/docs/images/concept.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.615053 funcdesc-0.1.3/funcdesc/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/mark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.615053 funcdesc-0.1.3/funcdesc/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/types/side_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/types/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.615053 funcdesc-0.1.3/funcdesc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-10 14:39:42.000000 funcdesc-0.1.3/funcdesc/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:39:51.615053 funcdesc-0.1.3/funcdesc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-10 14:39:51.000000 funcdesc-0.1.3/funcdesc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 14:39:51.000000 funcdesc-0.1.3/funcdesc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:39:51.000000 funcdesc-0.1.3/funcdesc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:39:51.000000 funcdesc-0.1.3/funcdesc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 14:39:51.000000 funcdesc-0.1.3/funcdesc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 14:39:51.000000 funcdesc-0.1.3/funcdesc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:39:51.619053 funcdesc-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-10 14:39:42.000000 funcdesc-0.1.3/setup.py
```

### Comparing `funcdesc-0.1.2/CONTRIBUTING.md` & `funcdesc-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/LICENSE` & `funcdesc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/PKG-INFO` & `funcdesc-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcdesc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Establish a general function description protocol, which can realize a comprehensive description of the input, output and side effects of an target function through an Python object. Provide a unified abstraction for parameter checking, interface generation and other functions in applications such as oneFace.
 Home-page: https://github.com/Nanguage/funcdesc
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT license
 Keywords: funcdesc
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `funcdesc-0.1.2/README.md` & `funcdesc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/docs/images/concept.png` & `funcdesc-0.1.3/docs/images/concept.png`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/funcdesc/desc.py` & `funcdesc-0.1.3/funcdesc/desc.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 TypeChecker = T.Callable[[T.Any, type], bool]
 RangeChecker = T.Callable[[T.Any, T.Any], bool]
 
 
 class Value(metaclass=CreateByGetItem):
+    """The description of a value."""
     type_to_range_checker: T.Dict[type, TypeChecker] = {}
     type_to_type_checker: T.Dict[type, RangeChecker] = {}
 
     def __init__(
             self,
             type_: T.Optional[T.Type[T1]] = None,
             range_: T.Optional[T.Any] = None,
@@ -109,14 +110,15 @@
         return True
 
     def __repr__(self):
         return f"<{self.__class__.__name__} description={self.description}>"
 
 
 class Description():
+    """The description of a function."""
     def __init__(
             self,
             inputs: T.Optional[T.List[Value]] = None,
             outputs: T.Optional[T.List[Value]] = None,
             side_effects: T.Optional[T.List[SideEffect]] = None,
             ):
         self.inputs = [] if inputs is None else inputs
```

### Comparing `funcdesc-0.1.2/funcdesc/guard.py` & `funcdesc-0.1.3/funcdesc/guard.py`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/funcdesc/mark.py` & `funcdesc-0.1.3/funcdesc/mark.py`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/funcdesc/types/side_effects.py` & `funcdesc-0.1.3/funcdesc/types/side_effects.py`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/funcdesc/types/value.py` & `funcdesc-0.1.3/funcdesc/types/value.py`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/funcdesc/utils/json.py` & `funcdesc-0.1.3/funcdesc/utils/json.py`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/funcdesc.egg-info/PKG-INFO` & `funcdesc-0.1.3/funcdesc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcdesc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Establish a general function description protocol, which can realize a comprehensive description of the input, output and side effects of an target function through an Python object. Provide a unified abstraction for parameter checking, interface generation and other functions in applications such as oneFace.
 Home-page: https://github.com/Nanguage/funcdesc
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT license
 Keywords: funcdesc
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `funcdesc-0.1.2/funcdesc.egg-info/SOURCES.txt` & `funcdesc-0.1.3/funcdesc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcdesc-0.1.2/setup.py` & `funcdesc-0.1.3/setup.py`

 * *Files identical despite different names*

