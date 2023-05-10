# Comparing `tmp/imaxt-multiscale-plugin-0.2.2.tar.gz` & `tmp/imaxt-multiscale-plugin-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaxt-multiscale-plugin-0.2.2.tar", last modified: Sun Dec 11 09:43:16 2022, max compression
+gzip compressed data, was "imaxt-multiscale-plugin-0.2.4.tar", last modified: Wed May 10 08:40:55 2023, max compression
```

## Comparing `imaxt-multiscale-plugin-0.2.2.tar` & `imaxt-multiscale-plugin-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 09:43:16.424937 imaxt-multiscale-plugin-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     7653 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3880 2022-12-11 09:43:16.424937 imaxt-multiscale-plugin-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      207 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1761 2022-12-11 09:43:16.425937 imaxt-multiscale-plugin-0.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 09:43:16.420937 imaxt-multiscale-plugin-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 09:43:16.422937 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/
--rw-rw-rw-   0 root         (0) root         (0)      302 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4252 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_sample_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 09:43:16.424937 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_tests/test_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      114 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_tests/test_sample_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_tests/test_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_tests/test_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     1990 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_widget.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     2449 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/napari.yaml
--rw-rw-rw-   0 root         (0) root         (0)      453 2022-12-11 09:42:37.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-11 09:43:16.423937 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3880 2022-12-11 09:43:16.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      892 2022-12-11 09:43:16.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-11 09:43:16.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2022-12-11 09:43:16.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      100 2022-12-11 09:43:16.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-12-11 09:43:16.000000 imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:40:55.062181 imaxt-multiscale-plugin-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-10 08:40:55.062181 imaxt-multiscale-plugin-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2023-05-10 08:40:55.063181 imaxt-multiscale-plugin-0.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:40:55.059181 imaxt-multiscale-plugin-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:40:55.061181 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4252 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_sample_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:40:55.062181 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_tests/test_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_tests/test_sample_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_tests/test_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_tests/test_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1990 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/napari.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-10 08:40:39.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:40:55.061181 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-10 08:40:55.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-10 08:40:55.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:40:55.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-10 08:40:55.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-10 08:40:55.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-10 08:40:55.000000 imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/top_level.txt
```

### Comparing `imaxt-multiscale-plugin-0.2.2/LICENSE` & `imaxt-multiscale-plugin-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.2/PKG-INFO` & `imaxt-multiscale-plugin-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaxt-multiscale-plugin
-Version: 0.2.2
+Version: 0.2.4
 Summary: A simple plugin to use with napari
 Home-page: https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/imaxt-multiscale-plugin
 Author: Eduardo Gonzalez Solares
 Author-email: E.GonzalezSolares@ast.cam.ac.uk
 License: LGPL-3.0-only
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `imaxt-multiscale-plugin-0.2.2/README.md` & `imaxt-multiscale-plugin-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.2/setup.cfg` & `imaxt-multiscale-plugin-0.2.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.2
+current_version = 0.2.4
 commit = True
 tag = True
 
 [metadata]
 name = imaxt-multiscale-plugin
 version = attr:imaxt_multiscale_plugin.__version__
 description = A simple plugin to use with napari
```

### Comparing `imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_reader.py` & `imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_reader.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_tests/test_reader.py` & `imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_tests/test_widget.py` & `imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_widget.py` & `imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_widget.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/_writer.py` & `imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/_writer.py`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin/napari.yaml` & `imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin/napari.yaml`

 * *Files identical despite different names*

### Comparing `imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/PKG-INFO` & `imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaxt-multiscale-plugin
-Version: 0.2.2
+Version: 0.2.4
 Summary: A simple plugin to use with napari
 Home-page: https://gitlab.developers.cam.ac.uk/astronomy/camcead/imaxt/imaxt-multiscale-plugin
 Author: Eduardo Gonzalez Solares
 Author-email: E.GonzalezSolares@ast.cam.ac.uk
 License: LGPL-3.0-only
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `imaxt-multiscale-plugin-0.2.2/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt` & `imaxt-multiscale-plugin-0.2.4/src/imaxt_multiscale_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

