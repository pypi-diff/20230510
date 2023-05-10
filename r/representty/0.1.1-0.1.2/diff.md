# Comparing `tmp/representty-0.1.1.tar.gz` & `tmp/representty-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "representty-0.1.1.tar", max compression
+gzip compressed data, was "representty-0.1.2.tar", max compression
```

## Comparing `representty-0.1.1.tar` & `representty-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      456 2023-03-27 20:43:54.800226 representty-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2350 2023-03-27 20:41:57.971266 representty-0.1.1/representty.py
--rw-r--r--   0        0        0      693 2023-03-27 20:44:16.098428 representty-0.1.1/setup.py
--rw-r--r--   0        0        0      412 2023-03-27 20:44:16.098558 representty-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      456 2023-05-10 21:29:19.092917 representty-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4082 2023-05-10 21:15:40.076464 representty-0.1.2/representty.py
+-rw-r--r--   0        0        0      693 2023-05-10 21:29:47.737253 representty-0.1.2/setup.py
+-rw-r--r--   0        0        0      412 2023-05-10 21:29:47.737397 representty-0.1.2/PKG-INFO
```

### Comparing `representty-0.1.1/setup.py` & `representty-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ['ipython', 'rich>=13.3.1,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['rtty = representty:just_call_the_script']}
 
 setup_kwargs = {
     'name': 'representty',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Tiny presentation tool based on rich and markdown',
     'long_description': None,
     'author': 'L3viathan',
     'author_email': 'git@l3vi.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

