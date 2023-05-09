# Comparing `tmp/fsst-0.8.3.tar.gz` & `tmp/fsst-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsst-0.8.3.tar", last modified: Tue May  9 20:37:48 2023, max compression
+gzip compressed data, was "fsst-0.8.4.tar", last modified: Tue May  9 21:14:18 2023, max compression
```

## Comparing `fsst-0.8.3.tar` & `fsst-0.8.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 20:37:48.729595 fsst-0.8.3/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 20:37:48.729595 fsst-0.8.3/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.3/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 20:37:48.729595 fsst-0.8.3/fsst.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 20:37:48.000000 fsst-0.8.3/fsst.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 20:37:48.000000 fsst-0.8.3/fsst.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 20:37:48.000000 fsst-0.8.3/fsst.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 20:37:48.000000 fsst-0.8.3/fsst.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.3/fsst.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-09 20:37:48.000000 fsst-0.8.3/fsst.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 20:37:48.000000 fsst-0.8.3/fsst.egg-info/top_level.txt
--rwxrwxr-x   0 rob       (1000) rob       (1000)   116352 2023-05-09 20:37:23.000000 fsst-0.8.3/fsst.py
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 20:37:48.729595 fsst-0.8.3/setup.cfg
--rw-rw-r--   0 rob       (1000) rob       (1000)     1170 2023-05-09 20:37:33.000000 fsst-0.8.3/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 21:14:18.677457 fsst-0.8.4/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 21:14:18.677457 fsst-0.8.4/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2640 2022-10-18 12:24:55.000000 fsst-0.8.4/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-09 21:14:18.677457 fsst-0.8.4/fsst.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      804 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      223 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       36 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2022-10-18 12:49:32.000000 fsst-0.8.4/fsst.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       88 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        5 2023-05-09 21:14:18.000000 fsst-0.8.4/fsst.egg-info/top_level.txt
+-rwxrwxr-x   0 rob       (1000) rob       (1000)   116361 2023-05-09 21:14:03.000000 fsst-0.8.4/fsst.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-09 21:14:18.677457 fsst-0.8.4/setup.cfg
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1170 2023-05-09 21:14:11.000000 fsst-0.8.4/setup.py
```

### Comparing `fsst-0.8.3/PKG-INFO` & `fsst-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.3
+Version: 0.8.4
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.3/README.md` & `fsst-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `fsst-0.8.3/fsst.egg-info/PKG-INFO` & `fsst-0.8.4/fsst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsst
-Version: 0.8.3
+Version: 0.8.4
 Summary: Fluree Schema Scenario Tool
 Home-page: https://github.com/pibara/fluree-schema-scenario-tool
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql
 Platform: UNKNOWN
```

### Comparing `fsst-0.8.3/fsst.py` & `fsst-0.8.4/fsst.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         else:
             print("-terminated")
 
 class Hooks:
     """Helper class for running hooks between runs"""
     def __init__(self):
         self.hookmodule = None
-        self.hook = None
+        self.hooks = None
         is_ok = False
         hookmodpath = os.path.join("hooks", "hooks.py")
         if os.path.exists(hookmodpath):
             try:
                 hookspec = importlib.util.spec_from_file_location("hooks", hookmodpath)
                 self.hookmodule= importlib.util.module_from_spec(hookspec)
                 hookspec.loader.exec_module(self.hookmodule)
@@ -148,37 +148,37 @@
             if is_ok:
                 self.hooks = getattr(self.hookmodule, "Hooks", None)
                 if self.hooks is None:
                     print("ERROR: No Hooks in hooks file")
                     is_ok = False
             if is_ok:
                 for method in ("before", "between", "after"):
-                    if getattr(self.hook, method, None) is None:
+                    if getattr(self.hooks, method, None) is None:
                         print("ERROR: missing hook: ", method)
                         is_ok = False
             if not is_ok:
-                self.hook = None
+                self.hooks = None
                 self.hookmodule = None
         else:
             print("WARNING: No hooks file found: ", hookmodpath)
 
     def before(self):
         """Before hook"""
-        if self.hook:
-            self.hook.before()
+        if self.hooks:
+            self.hooks.before()
 
     def between(self):
         """In between hook"""
-        if self.hook:
-            self.hook.between()
+        if self.hooks:
+            self.hooks.between()
 
     def after(self):
         """After hook"""
-        if self.hook:
-            self.hook.after()
+        if self.hooks:
+            self.hooks.after()
 
 class FlushFile:
     """Helper class for file like objects to always flush on write"""
     def __init__(self, file_descriptor):
         """Constructor
          Parameters
          ----------
```

### Comparing `fsst-0.8.3/setup.py` & `fsst-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fsst',
-    version="0.8.3",
+    version="0.8.4",
     description="Fluree Schema Scenario Tool",
     long_description="Testing tool for schema and smart function unit tests for FlureeDB",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/fluree-schema-scenario-tool',
     license='BSD',
     py_modules=['fsst'],
```

