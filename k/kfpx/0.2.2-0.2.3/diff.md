# Comparing `tmp/kfpx-0.2.2.tar.gz` & `tmp/kfpx-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfpx-0.2.2.tar", max compression
+gzip compressed data, was "kfpx-0.2.3.tar", max compression
```

## Comparing `kfpx-0.2.2.tar` & `kfpx-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2022-05-31 04:06:19.563397 kfpx-0.2.2/LICENSE
--rw-r--r--   0        0        0       40 2022-06-14 07:54:25.417725 kfpx-0.2.2/kfpx/__init__.py
--rw-r--r--   0        0        0     2108 2022-09-08 08:53:17.783088 kfpx-0.2.2/kfpx/client.py
--rw-r--r--   0        0        0        0 2022-05-31 04:13:08.826978 kfpx-0.2.2/kfpx/compiler.py
--rw-r--r--   0        0        0      524 2022-09-08 08:51:56.590900 kfpx-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 kfpx-0.2.2/setup.py
--rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 kfpx-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-05-31 04:06:19.563397 kfpx-0.2.3/LICENSE
+-rw-r--r--   0        0        0       40 2022-06-14 07:54:25.417725 kfpx-0.2.3/kfpx/__init__.py
+-rw-r--r--   0        0        0     2108 2022-09-08 08:53:17.783088 kfpx-0.2.3/kfpx/client.py
+-rw-r--r--   0        0        0        0 2022-05-31 04:13:08.826978 kfpx-0.2.3/kfpx/compiler.py
+-rw-r--r--   0        0        0      517 2023-05-10 09:05:22.373335 kfpx-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 kfpx-0.2.3/setup.py
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 kfpx-0.2.3/PKG-INFO
```

### Comparing `kfpx-0.2.2/LICENSE` & `kfpx-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kfpx-0.2.2/kfpx/client.py` & `kfpx-0.2.3/kfpx/client.py`

 * *Files identical despite different names*

### Comparing `kfpx-0.2.2/pyproject.toml` & `kfpx-0.2.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "kfpx"
-version = "0.2.2"
+version = "0.2.3"
 description = "Extends the kfp package"
 authors = ["Hao Xin <haoxinst@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-kfp = "1.8.12"
+kfp = "1.8.21"
 
 [tool.poetry.dev-dependencies]
 black = "^22.8.0"
 isort = "^5.10.1"
 poetry-exec-plugin = "0.3.5"
 
 [tool.poetry-exec-plugin.commands]
 fmt = "poetry run isort . && poetry run black ."
 test = "poetry run pytest -s"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kfpx-0.2.2/setup.py` & `kfpx-0.2.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['kfpx']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kfp==1.8.12']
+['kfp==1.8.21']
 
 setup_kwargs = {
     'name': 'kfpx',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Extends the kfp package',
     'long_description': 'None',
     'author': 'Hao Xin',
     'author_email': 'haoxinst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

