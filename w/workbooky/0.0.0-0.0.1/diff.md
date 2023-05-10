# Comparing `tmp/workbooky-0.0.0.tar.gz` & `tmp/workbooky-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workbooky-0.0.0.tar", last modified: Wed May 10 06:30:30 2023, max compression
+gzip compressed data, was "workbooky-0.0.1.tar", last modified: Wed May 10 06:41:39 2023, max compression
```

## Comparing `workbooky-0.0.0.tar` & `workbooky-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 06:30:30.414359 workbooky-0.0.0/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 workbooky-0.0.0/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      610 2023-05-10 06:30:30.414359 workbooky-0.0.0/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      131 2023-05-10 06:26:57.000000 workbooky-0.0.0/README.md
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-10 06:30:30.414359 workbooky-0.0.0/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1173 2023-05-10 06:29:32.000000 workbooky-0.0.0/setup.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 06:30:30.411026 workbooky-0.0.0/workbooky/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      130 2023-05-10 06:29:45.000000 workbooky-0.0.0/workbooky/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-10 06:30:07.000000 workbooky-0.0.0/workbooky/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 06:30:30.414359 workbooky-0.0.0/workbooky/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 workbooky-0.0.0/workbooky/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1420 2023-05-10 06:27:45.000000 workbooky-0.0.0/workbooky/src/workbook.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 06:30:30.414359 workbooky-0.0.0/workbooky.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      610 2023-05-10 06:30:30.000000 workbooky-0.0.0/workbooky.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      268 2023-05-10 06:30:30.000000 workbooky-0.0.0/workbooky.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-10 06:30:30.000000 workbooky-0.0.0/workbooky.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-05-10 06:30:30.000000 workbooky-0.0.0/workbooky.egg-info/top_level.txt
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 06:41:39.407703 workbooky-0.0.1/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 workbooky-0.0.1/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      669 2023-05-10 06:41:39.407703 workbooky-0.0.1/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      131 2023-05-10 06:26:57.000000 workbooky-0.0.1/README.md
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-10 06:41:39.407703 workbooky-0.0.1/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1173 2023-05-10 06:29:32.000000 workbooky-0.0.1/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 06:41:39.407703 workbooky-0.0.1/workbooky/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      130 2023-05-10 06:29:45.000000 workbooky-0.0.1/workbooky/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-10 06:40:53.000000 workbooky-0.0.1/workbooky/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 06:41:39.407703 workbooky-0.0.1/workbooky/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 workbooky-0.0.1/workbooky/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1499 2023-05-10 06:40:05.000000 workbooky-0.0.1/workbooky/src/workbook.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 06:41:39.407703 workbooky-0.0.1/workbooky.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      669 2023-05-10 06:41:39.000000 workbooky-0.0.1/workbooky.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      268 2023-05-10 06:41:39.000000 workbooky-0.0.1/workbooky.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-10 06:41:39.000000 workbooky-0.0.1/workbooky.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-05-10 06:41:39.000000 workbooky-0.0.1/workbooky.egg-info/top_level.txt
```

### Comparing `workbooky-0.0.0/LICENSE.txt` & `workbooky-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `workbooky-0.0.0/setup.py` & `workbooky-0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `workbooky-0.0.0/workbooky/src/workbook.py` & `workbooky-0.0.1/workbooky/src/workbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,8 +33,12 @@
     def get_worksheet(self, sheet_name: str) -> object:
         # Return the worksheet if it exists, otherwise quit.
         try:
             worksheet = self.workbook[sheet_name]
             return worksheet
         except KeyError:
             cprint(f"There is no {sheet_name} sheet in the workbook {self.path}", ERROR_COLOUR)
-            quit()
+            quit()
+
+    def save(self):
+        # Save the workbook
+        self.workbook.save()
```

