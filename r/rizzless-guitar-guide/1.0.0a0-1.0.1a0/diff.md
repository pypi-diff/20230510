# Comparing `tmp/rizzless_guitar_guide-1.0.0a0.tar.gz` & `tmp/rizzless_guitar_guide-1.0.1a0.tar.gz`

## Comparing `rizzless_guitar_guide-1.0.0a0.tar` & `rizzless_guitar_guide-1.0.1a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/src/rizzless_guitar_guide/__init__.py
--rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/src/rizzless_guitar_guide/guide.py
--rw-r--r--   0        0        0    10041 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/src/rizzless_guitar_guide/intervalstuff.py
--rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/src/rizzless_guitar_guide/modestuff.py
--rw-r--r--   0        0        0    21611 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/src/rizzless_guitar_guide/scalestuff.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/LICENSE.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/src/rizzless_guitar_guide/__init__.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/src/rizzless_guitar_guide/guide.py
+-rw-r--r--   0        0        0    10041 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/src/rizzless_guitar_guide/intervalstuff.py
+-rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/src/rizzless_guitar_guide/modestuff.py
+-rw-r--r--   0        0        0    21611 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/src/rizzless_guitar_guide/scalestuff.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/LICENSE.txt
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 rizzless_guitar_guide-1.0.1a0/PKG-INFO
```

### Comparing `rizzless_guitar_guide-1.0.0a0/src/rizzless_guitar_guide/intervalstuff.py` & `rizzless_guitar_guide-1.0.1a0/src/rizzless_guitar_guide/intervalstuff.py`

 * *Files identical despite different names*

### Comparing `rizzless_guitar_guide-1.0.0a0/src/rizzless_guitar_guide/modestuff.py` & `rizzless_guitar_guide-1.0.1a0/src/rizzless_guitar_guide/modestuff.py`

 * *Files identical despite different names*

### Comparing `rizzless_guitar_guide-1.0.0a0/src/rizzless_guitar_guide/scalestuff.py` & `rizzless_guitar_guide-1.0.1a0/src/rizzless_guitar_guide/scalestuff.py`

 * *Files identical despite different names*

### Comparing `rizzless_guitar_guide-1.0.0a0/LICENSE.txt` & `rizzless_guitar_guide-1.0.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rizzless_guitar_guide-1.0.0a0/pyproject.toml` & `rizzless_guitar_guide-1.0.1a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rizzless_guitar_guide"
-version = "1.0.0-alpha"
+version = "1.0.1-alpha"
 authors = [
   { name="Michael Lacy", email="michaellacy21419@gmail.com" },
 ]
-description = "The first, unoptimized version of the Rizzless Guitar Guide"
+description = "Reduced nesting, topics can now be searched upon launch"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

