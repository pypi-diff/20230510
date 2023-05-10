# Comparing `tmp/resoto-plugin-github-3.4.1.tar.gz` & `tmp/resoto-plugin-github-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-github-3.4.1.tar", last modified: Fri Apr 28 15:15:24 2023, max compression
+gzip compressed data, was "resoto-plugin-github-3.4.2.tar", last modified: Wed May 10 12:22:23 2023, max compression
```

## Comparing `resoto-plugin-github-3.4.1.tar` & `resoto-plugin-github-3.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:24.340074 resoto-plugin-github-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:13:42.000000 resoto-plugin-github-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-28 15:15:24.340074 resoto-plugin-github-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 15:13:42.000000 resoto-plugin-github-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 15:13:42.000000 resoto-plugin-github-3.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:24.336074 resoto-plugin-github-3.4.1/resoto_plugin_github/
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-28 15:13:42.000000 resoto-plugin-github-3.4.1/resoto_plugin_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-28 15:13:42.000000 resoto-plugin-github-3.4.1/resoto_plugin_github/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-04-28 15:13:42.000000 resoto-plugin-github-3.4.1/resoto_plugin_github/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:24.340074 resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-28 15:15:24.000000 resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-28 15:15:24.000000 resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:15:24.000000 resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 15:15:24.000000 resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:15:24.000000 resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 15:15:24.000000 resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 15:15:24.000000 resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:15:24.340074 resoto-plugin-github-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-28 15:13:42.000000 resoto-plugin-github-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:24.340074 resoto-plugin-github-3.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-28 15:13:42.000000 resoto-plugin-github-3.4.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:23.125100 resoto-plugin-github-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 12:20:18.000000 resoto-plugin-github-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-10 12:22:23.125100 resoto-plugin-github-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 12:20:18.000000 resoto-plugin-github-3.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 12:20:18.000000 resoto-plugin-github-3.4.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:23.121100 resoto-plugin-github-3.4.2/resoto_plugin_github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-10 12:20:18.000000 resoto-plugin-github-3.4.2/resoto_plugin_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-10 12:20:18.000000 resoto-plugin-github-3.4.2/resoto_plugin_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-05-10 12:20:18.000000 resoto-plugin-github-3.4.2/resoto_plugin_github/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:23.125100 resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-10 12:22:23.000000 resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-10 12:22:23.000000 resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:23.000000 resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 12:22:23.000000 resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:23.000000 resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 12:22:23.000000 resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 12:22:23.000000 resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:22:23.125100 resoto-plugin-github-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-10 12:20:18.000000 resoto-plugin-github-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:23.125100 resoto-plugin-github-3.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 12:20:18.000000 resoto-plugin-github-3.4.2/test/test_config.py
```

### Comparing `resoto-plugin-github-3.4.1/PKG-INFO` & `resoto-plugin-github-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.4.1
+Version: 3.4.2
 Summary: Resoto Github Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/github
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-github-3.4.1/resoto_plugin_github/__init__.py` & `resoto-plugin-github-3.4.2/resoto_plugin_github/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.4.1/resoto_plugin_github/config.py` & `resoto-plugin-github-3.4.2/resoto_plugin_github/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.4.1/resoto_plugin_github/resources.py` & `resoto-plugin-github-3.4.2/resoto_plugin_github/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-github-3.4.1/resoto_plugin_github.egg-info/PKG-INFO` & `resoto-plugin-github-3.4.2/resoto_plugin_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-github
-Version: 3.4.1
+Version: 3.4.2
 Summary: Resoto Github Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/github
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-github-3.4.1/setup.py` & `resoto-plugin-github-3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-github",
-    version="3.4.1",
+    version="3.4.2",
     description="Resoto Github Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["github = resoto_plugin_github:GithubCollectorPlugin"]},
     include_package_data=True,
```

