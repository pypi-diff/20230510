# Comparing `tmp/fyers_token_manager_v2-0.0.5.tar.gz` & `tmp/fyers_token_manager_v2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.0.5.tar", last modified: Wed May 10 05:20:42 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.0.6.tar", last modified: Wed May 10 05:24:24 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.0.5.tar` & `fyers_token_manager_v2-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.5/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:19:02.000000 fyers_token_manager_v2-0.0.5/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:18:24.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2/__init__.py
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4523 2023-05-10 05:18:34.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2/v2.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      319 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:20:42.000000 fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:20:42.141628 fyers_token_manager_v2-0.0.5/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-10 05:20:32.000000 fyers_token_manager_v2-0.0.5/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.6/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 05:19:02.000000 fyers_token_manager_v2-0.0.6/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4523 2023-05-10 05:24:06.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2/__init__.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:24:24.000000 fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:24:24.935935 fyers_token_manager_v2-0.0.6/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-10 05:23:56.000000 fyers_token_manager_v2-0.0.6/setup.py
```

### Comparing `fyers_token_manager_v2-0.0.5/PKG-INFO` & `fyers_token_manager_v2-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_token_manager_v2
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.0.5/README.md` & `fyers_token_manager_v2-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.0.5/fyers_token_manager_v2/v2.py` & `fyers_token_manager_v2-0.0.6/fyers_token_manager_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.0.5/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.0.6/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager-v2
-Version: 0.0.5
+Version: 0.0.6
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.0.5/setup.py` & `fyers_token_manager_v2-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.0.5",
+    version="0.0.6",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

