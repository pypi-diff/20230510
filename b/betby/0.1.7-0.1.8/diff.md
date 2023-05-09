# Comparing `tmp/betby-0.1.7.tar.gz` & `tmp/betby-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betby-0.1.7.tar", last modified: Tue May  9 23:40:24 2023, max compression
+gzip compressed data, was "betby-0.1.8.tar", last modified: Tue May  9 23:46:52 2023, max compression
```

## Comparing `betby-0.1.7.tar` & `betby-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 23:40:24.990405 betby-0.1.7/
--rw-rw-rw-   0        0        0      539 2023-05-09 23:40:24.988409 betby-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 23:40:24.965298 betby-0.1.7/betby/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:37:29.000000 betby-0.1.7/betby/__init__.py
--rw-rw-rw-   0        0        0     1156 2023-04-30 14:03:47.000000 betby-0.1.7/betby/margin.py
-drwxrwxrwx   0        0        0        0 2023-05-09 23:40:24.984538 betby-0.1.7/betby.egg-info/
--rw-rw-rw-   0        0        0      539 2023-05-09 23:40:22.000000 betby-0.1.7/betby.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-05-09 23:40:24.000000 betby-0.1.7/betby.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 23:40:22.000000 betby-0.1.7/betby.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-09 23:40:22.000000 betby-0.1.7/betby.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 23:40:24.991402 betby-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-05-09 23:38:39.000000 betby-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:46:52.037202 betby-0.1.8/
+-rw-rw-rw-   0        0        0      539 2023-05-09 23:46:52.036207 betby-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 23:46:52.011505 betby-0.1.8/betby/
+-rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.1.8/betby/__init__.py
+-rw-rw-rw-   0        0        0     1156 2023-04-30 14:03:47.000000 betby-0.1.8/betby/margin.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:46:52.030486 betby-0.1.8/betby.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-05-09 23:46:49.000000 betby-0.1.8/betby.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-05-09 23:46:51.000000 betby-0.1.8/betby.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:46:49.000000 betby-0.1.8/betby.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 23:46:49.000000 betby-0.1.8/betby.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 23:46:52.038205 betby-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-05-09 23:45:00.000000 betby-0.1.8/setup.py
```

### Comparing `betby-0.1.7/PKG-INFO` & `betby-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.1.7
+Version: 0.1.8
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.1.7/betby/margin.py` & `betby-0.1.8/betby/margin.py`

 * *Files identical despite different names*

### Comparing `betby-0.1.7/betby.egg-info/PKG-INFO` & `betby-0.1.8/betby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.1.7
+Version: 0.1.8
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.1.7/setup.py` & `betby-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betby",
-    version="0.1.7",
+    version="0.1.8",
     author="Ayrat Badrutdinov",
     author_email="a.badrutdinov@betby.com",
     description="Betby libraries",
     packages=["betby"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

