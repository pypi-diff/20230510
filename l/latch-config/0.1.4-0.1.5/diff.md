# Comparing `tmp/latch_config-0.1.4.tar.gz` & `tmp/latch_config-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_config-0.1.4.tar", max compression
+gzip compressed data, was "latch_config-0.1.5.tar", max compression
```

## Comparing `latch_config-0.1.4.tar` & `latch_config-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.4/LICENSE
--rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.4/README.md
--rw-r--r--   0        0        0     2207 2023-05-09 17:07:12.285092 latch_config-0.1.4/latch_config/config.py
--rw-r--r--   0        0        0        0 2023-05-09 16:28:54.229755 latch_config-0.1.4/latch_config/py.typed
--rw-r--r--   0        0        0     1086 2023-05-09 17:08:35.939075 latch_config-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.4/setup.py
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.5/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:25:16.083190 latch_config-0.1.5/latch_config/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-09 17:07:12.285092 latch_config-0.1.5/latch_config/config.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:28:54.229755 latch_config-0.1.5/latch_config/py.typed
+-rw-r--r--   0        0        0     1086 2023-05-10 15:26:47.132443 latch_config-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.5/setup.py
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.5/PKG-INFO
```

### Comparing `latch_config-0.1.4/LICENSE` & `latch_config-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_config-0.1.4/latch_config/config.py` & `latch_config-0.1.5/latch_config/config.py`

 * *Files identical despite different names*

### Comparing `latch_config-0.1.4/pyproject.toml` & `latch_config-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-config"
-version = "0.1.4"
+version = "0.1.5"
 description = "Shared config for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_config"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_config-0.1.4/setup.py` & `latch_config-0.1.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['latch_config']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'latch-config',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Shared config for latch python backend services',
     'long_description': '# python-config\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

