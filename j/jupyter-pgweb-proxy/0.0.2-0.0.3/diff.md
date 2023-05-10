# Comparing `tmp/jupyter_pgweb_proxy-0.0.2.tar.gz` & `tmp/jupyter_pgweb_proxy-0.0.3.tar.gz`

## Comparing `jupyter_pgweb_proxy-0.0.2.tar` & `jupyter_pgweb_proxy-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/.editorconfig
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/jupyter_pgweb_proxy/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/jupyter_pgweb_proxy/jupyter_config.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/jupyter_pgweb_proxy/pgweb.svg
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/LICENSE.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/.editorconfig
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/jupyter_pgweb_proxy/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/jupyter_pgweb_proxy/jupyter_config.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/jupyter_pgweb_proxy/pgweb.svg
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/README.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 jupyter_pgweb_proxy-0.0.3/PKG-INFO
```

### Comparing `jupyter_pgweb_proxy-0.0.2/jupyter_pgweb_proxy/__init__.py` & `jupyter_pgweb_proxy-0.0.3/jupyter_pgweb_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_pgweb_proxy-0.0.2/jupyter_pgweb_proxy/pgweb.svg` & `jupyter_pgweb_proxy-0.0.3/jupyter_pgweb_proxy/pgweb.svg`

 * *Files identical despite different names*

### Comparing `jupyter_pgweb_proxy-0.0.2/.gitignore` & `jupyter_pgweb_proxy-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_pgweb_proxy-0.0.2/LICENSE.md` & `jupyter_pgweb_proxy-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jupyter_pgweb_proxy-0.0.2/pyproject.toml` & `jupyter_pgweb_proxy-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter-pgweb-proxy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Matus Kosut", email="matus.kosut@ntnu.no" },
   { name="Hans Stemshaug", email="hans.stemshaug@ntnu.no" },
 ]
 description = "Jupyter server proxy for pgweb"
 readme = "README.md"
 license = { file = "LICENSE.md" }
```

### Comparing `jupyter_pgweb_proxy-0.0.2/PKG-INFO` & `jupyter_pgweb_proxy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-pgweb-proxy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Jupyter server proxy for pgweb
 Project-URL: Homepage, https://github.com/huntdatacenter/jupyter-pgweb-proxy
 Author-email: Matus Kosut <matus.kosut@ntnu.no>, Hans Stemshaug <hans.stemshaug@ntnu.no>
 License: MIT License
         
         Copyright (c) 2023 HUNT Data Center
```

