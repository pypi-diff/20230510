# Comparing `tmp/fyers_token_manager_v2-0.0.2.tar.gz` & `tmp/fyers_token_manager_v2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.0.2.tar", last modified: Wed May 10 04:44:46 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.0.3.tar", last modified: Wed May 10 05:00:34 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.0.2.tar` & `fyers_token_manager_v2-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.2/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 04:19:57.000000 fyers_token_manager_v2-0.0.2/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4523 2023-05-10 04:19:45.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2/__init__.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      305 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 04:44:46.000000 fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      383 2023-05-10 04:19:38.000000 fyers_token_manager_v2-0.0.2/pyproject.toml
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 04:44:46.959379 fyers_token_manager_v2-0.0.2/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      690 2023-05-10 04:20:08.000000 fyers_token_manager_v2-0.0.2/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.3/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 04:19:57.000000 fyers_token_manager_v2-0.0.3/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4523 2023-05-10 04:19:45.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2/__init__.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      690 2023-05-10 04:58:29.000000 fyers_token_manager_v2-0.0.3/setup.py
```

### Comparing `fyers_token_manager_v2-0.0.2/PKG-INFO` & `fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fyers_token_manager_v2
-Version: 0.0.2
+Name: fyers-token-manager-v2
+Version: 0.0.3
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.0.2/README.md` & `fyers_token_manager_v2-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.0.2/fyers_token_manager_v2/__init__.py` & `fyers_token_manager_v2-0.0.3/fyers_token_manager_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.0.2/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fyers-token-manager-v2
-Version: 0.0.2
+Name: fyers_token_manager_v2
+Version: 0.0.3
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.0.2/setup.py` & `fyers_token_manager_v2-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.0.2",
+    version="0.0.3",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
```

