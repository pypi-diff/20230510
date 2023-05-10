# Comparing `tmp/robocorp_browser-0.3.0.tar.gz` & `tmp/robocorp_browser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-0.3.0.tar", max compression
+gzip compressed data, was "robocorp_browser-0.4.0.tar", max compression
```

## Comparing `robocorp_browser-0.3.0.tar` & `robocorp_browser-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       94 2023-04-28 10:50:56.511915 robocorp_browser-0.3.0/README.md
--rw-r--r--   0        0        0      704 2023-05-08 12:31:25.572018 robocorp_browser-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      111 2023-05-08 08:00:17.798903 robocorp_browser-0.3.0/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0     2948 2023-05-08 10:36:59.939742 robocorp_browser-0.3.0/src/robocorp/browser/browser.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 robocorp_browser-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/README.md
+-rw-r--r--   0        0        0      640 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7225 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0     6959 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:39:41.395091 robocorp_browser-0.4.0/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 robocorp_browser-0.4.0/PKG-INFO
```

### Comparing `robocorp_browser-0.3.0/PKG-INFO` & `robocorp_browser-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: robocorp-browser
-Version: 0.3.0
+Version: 0.4.0
 Summary: Robocorp browser automation library
-Author: Ossi R.
-Author-email: ossi@robocorp.com
+Author: Fabio Z.
+Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: playwright (>=1.32.1,<2.0.0)
+Requires-Dist: robocorp-tasks (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # Robocorp browser library
 
 Provides a couple of helpers on top of Playwright python library.
```

