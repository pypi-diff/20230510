# Comparing `tmp/llcsciencesdk-1.2.0.tar.gz` & `tmp/llcsciencesdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llcsciencesdk-1.2.0.tar", last modified: Tue May 10 15:02:17 2022, max compression
+gzip compressed data, was "llcsciencesdk-2.0.0.tar", last modified: Wed May 10 13:15:35 2023, max compression
```

## Comparing `llcsciencesdk-1.2.0.tar` & `llcsciencesdk-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2053 2021-11-09 10:26:22.967239 llcsciencesdk-1.2.0/.gitignore
--rw-r--r--   0        0        0     1080 2021-11-09 10:26:22.967540 llcsciencesdk-1.2.0/LICENSE
--rw-r--r--   0        0        0       83 2022-05-10 14:39:03.224558 llcsciencesdk-1.2.0/llcsciencesdk/__init__.py
--rw-r--r--   0        0        0     1056 2021-11-09 10:26:22.967978 llcsciencesdk-1.2.0/llcsciencesdk/exceptions.py
--rw-r--r--   0        0        0      171 2022-05-10 14:25:37.901159 llcsciencesdk-1.2.0/llcsciencesdk/helpers.py
--rw-r--r--   0        0        0     6751 2022-05-10 14:32:50.546202 llcsciencesdk-1.2.0/llcsciencesdk/llc_api.py
--rw-r--r--   0        0        0     1016 2022-05-10 14:25:37.902109 llcsciencesdk-1.2.0/llcsciencesdk/parameter_mapping.py
--rw-r--r--   0        0        0      719 2022-05-10 14:25:37.902914 llcsciencesdk-1.2.0/llcsciencesdk/sample.py
--rw-r--r--   0        0        0     1352 2022-05-10 14:25:37.903732 llcsciencesdk-1.2.0/llcsciencesdk/tests.py
--rw-r--r--   0        0        0     1748 2022-05-10 14:32:50.547164 llcsciencesdk-1.2.0/llcsciencesdk/urls.py
--rw-r--r--   0        0        0      319 2021-11-09 10:26:22.968795 llcsciencesdk-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2910 2022-05-10 14:37:49.210017 llcsciencesdk-1.2.0/readme.md
--rw-r--r--   0        0        0     3192 1970-01-01 00:00:00.000000 llcsciencesdk-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2071 2023-05-10 11:53:51.598334 llcsciencesdk-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1080 2021-07-05 15:00:27.981056 llcsciencesdk-2.0.0/LICENSE
+-rw-r--r--   0        0        0       83 2023-05-10 11:44:15.775052 llcsciencesdk-2.0.0/llcsciencesdk/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-10 11:44:15.775770 llcsciencesdk-2.0.0/llcsciencesdk/exceptions.py
+-rw-r--r--   0        0        0      172 2023-05-10 11:44:15.776288 llcsciencesdk-2.0.0/llcsciencesdk/helpers.py
+-rw-r--r--   0        0        0    14233 2023-05-10 11:44:15.776763 llcsciencesdk-2.0.0/llcsciencesdk/llc_api.py
+-rw-r--r--   0        0        0     1017 2023-05-10 11:44:15.777187 llcsciencesdk-2.0.0/llcsciencesdk/parameter_mapping.py
+-rw-r--r--   0        0        0      719 2022-04-07 10:48:47.109982 llcsciencesdk-2.0.0/llcsciencesdk/sample.py
+-rw-r--r--   0        0        0     1440 2023-05-10 11:44:15.777603 llcsciencesdk-2.0.0/llcsciencesdk/tests.py
+-rw-r--r--   0        0        0     4905 2023-05-10 11:44:15.778006 llcsciencesdk-2.0.0/llcsciencesdk/urls.py
+-rw-r--r--   0        0        0      318 2023-05-10 11:49:19.758651 llcsciencesdk-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1197 2023-05-10 11:44:15.778699 llcsciencesdk-2.0.0/readme.md
+-rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 llcsciencesdk-2.0.0/PKG-INFO
```

### Comparing `llcsciencesdk-1.2.0/.gitignore` & `llcsciencesdk-2.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -136,8 +136,10 @@
 
 # Cython debug symbols
 cython_debug/
 
 .vscode/
 
 #
-.idea
+.idea
+.DS_Store
+.pypirc
```

### Comparing `llcsciencesdk-1.2.0/LICENSE` & `llcsciencesdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llcsciencesdk-1.2.0/llcsciencesdk/exceptions.py` & `llcsciencesdk-2.0.0/llcsciencesdk/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,29 @@
         super().__init__(self.message)
 
     def __str__(self):
         return f" {self.message} -> {self.error_message}"
 
 
 class ApiTokenError(LlcAPIClientError):
-    def __init__(self, message="There is no valid auth token available. Please login using ScienceSdk.login(username, "
-                               "password)"):
+    def __init__(
+        self,
+        message="There is no valid auth token available. Please login using ScienceSdk.login(username, "
+        "password)",
+    ):
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
         return f" {self.message}"
 
 
 class ApiAuthenticationError(LlcAPIClientError):
     def __init__(
-            self, error_message, message="There was an error with authentication."
+        self, error_message, message="There was an error with authentication."
     ):
         self.error_message = error_message
         self.message = message
         super().__init__(self.message)
 
     def __str__(self):
         return f" {self.message} -> {self.error_message}"
```

### Comparing `llcsciencesdk-1.2.0/llcsciencesdk/sample.py` & `llcsciencesdk-2.0.0/llcsciencesdk/sample.py`

 * *Files identical despite different names*

### Comparing `llcsciencesdk-1.2.0/llcsciencesdk/tests.py` & `llcsciencesdk-2.0.0/llcsciencesdk/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 
     def test_api(self):
         """
         Very basic test.
         """
         self.assertIsInstance(self.llc_api.get_model_input_fast_track_json(46), dict)
         self.assertIsInstance(self.llc_api.get_model_input_fast_track(46), dict)
-        self.assertIsInstance(self.llc_api.get_model_input_calibrate_fast_track_json(46), dict)
-        self.assertIsInstance(self.llc_api.get_model_input_calibrate_fast_track(46), dict)
-        self.assertIsInstance(self.llc_api.get_model_input_density_analyses_fast_track_json(46), dict)
-        self.assertIsInstance(self.llc_api.get_model_input_density_analyses_fast_track(46), dict)
+        self.assertIsInstance(
+            self.llc_api.get_model_input_calibrate_fast_track_json(46), dict
+        )
+        self.assertIsInstance(
+            self.llc_api.get_model_input_calibrate_fast_track(46), dict
+        )
+        self.assertIsInstance(
+            self.llc_api.get_model_input_density_analyses_fast_track_json(46), dict
+        )
+        self.assertIsInstance(
+            self.llc_api.get_model_input_density_analyses_fast_track(46), dict
+        )
         self.assertIsInstance(self.llc_api.get_model_inputs_as_df(46), tuple)
         self.assertIsInstance(self.llc_api.get_planting_design_detail(10), dict)
         self.assertIsInstance(self.llc_api.get_planting_design_list(), list)
```

