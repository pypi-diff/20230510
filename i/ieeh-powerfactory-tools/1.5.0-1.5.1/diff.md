# Comparing `tmp/ieeh-powerfactory-tools-1.5.0.tar.gz` & `tmp/ieeh-powerfactory-tools-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieeh-powerfactory-tools-1.5.0.tar", last modified: Fri May  5 12:10:37 2023, max compression
+gzip compressed data, was "ieeh-powerfactory-tools-1.5.1.tar", last modified: Wed May 10 10:44:12 2023, max compression
```

## Comparing `ieeh-powerfactory-tools-1.5.0.tar` & `ieeh-powerfactory-tools-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      272 2023-05-05 12:09:38.305164 ieeh-powerfactory-tools-1.5.0/AUTHORS.md
--rw-r--r--   0        0        0     1568 2023-05-05 12:09:38.305164 ieeh-powerfactory-tools-1.5.0/LICENSE
--rw-r--r--   0        0        0     3565 2023-05-05 12:09:38.305164 ieeh-powerfactory-tools-1.5.0/README.md
--rw-r--r--   0        0        0      316 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/__init__.py
--rw-r--r--   0        0        0     1783 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/constants.py
--rw-r--r--   0        0        0      428 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/__init__.py
--rw-r--r--   0        0        0   100878 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/exporter.py
--rw-r--r--   0        0        0    30138 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/load_power.py
--rw-r--r--   0        0        0    36084 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/interface.py
--rw-r--r--   0        0        0    26605 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/powerfactory_types.py
--rw-r--r--   0        0        0      287 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/utils/__init__.py
--rw-r--r--   0        0        0      583 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/powerfactory_tools/utils/io.py
--rw-r--r--   0        0        0     2668 2023-05-05 12:10:30.117909 ieeh-powerfactory-tools-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      452 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0      493 2023-05-05 12:09:38.313164 ieeh-powerfactory-tools-1.5.0/tests/test_interface.py
--rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 ieeh-powerfactory-tools-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      272 2023-05-10 10:43:16.911213 ieeh-powerfactory-tools-1.5.1/AUTHORS.md
+-rw-r--r--   0        0        0     1568 2023-05-10 10:43:16.911213 ieeh-powerfactory-tools-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3565 2023-05-10 10:43:16.911213 ieeh-powerfactory-tools-1.5.1/README.md
+-rw-r--r--   0        0        0      316 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/__init__.py
+-rw-r--r--   0        0        0     1783 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/constants.py
+-rw-r--r--   0        0        0      428 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/exporter/__init__.py
+-rw-r--r--   0        0        0   100890 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/exporter/exporter.py
+-rw-r--r--   0        0        0    30138 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/exporter/load_power.py
+-rw-r--r--   0        0        0    36084 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/interface.py
+-rw-r--r--   0        0        0    26605 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/powerfactory_types.py
+-rw-r--r--   0        0        0      287 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/utils/__init__.py
+-rw-r--r--   0        0        0      583 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/powerfactory_tools/utils/io.py
+-rw-r--r--   0        0        0     2668 2023-05-10 10:44:04.627164 ieeh-powerfactory-tools-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      452 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/tests/conftest.py
+-rw-r--r--   0        0        0      493 2023-05-10 10:43:16.919213 ieeh-powerfactory-tools-1.5.1/tests/test_interface.py
+-rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 ieeh-powerfactory-tools-1.5.1/PKG-INFO
```

### Comparing `ieeh-powerfactory-tools-1.5.0/LICENSE` & `ieeh-powerfactory-tools-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.5.0/README.md` & `ieeh-powerfactory-tools-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/constants.py` & `ieeh-powerfactory-tools-1.5.1/powerfactory_tools/constants.py`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/exporter.py` & `ieeh-powerfactory-tools-1.5.1/powerfactory_tools/exporter/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -742,21 +742,21 @@
             # Neutral point phase connection
             neutral_connected_h, neutral_connected_l = self.transformer_neutral_connection_hvlv(
                 transformer_2w,
                 vector_group,
             )
 
             # Neutral point earthing
-            if "N" in vector_group_h and transformer_2w.cgnd_h == TrfNeutralPointState.EARTHED:
+            if "N" in vector_group_h.value and transformer_2w.cgnd_h == TrfNeutralPointState.EARTHED:
                 re_h = transformer_2w.re0tr_h
                 xe_h = transformer_2w.xe0tr_h
             else:
                 re_h = None
                 xe_h = None
-            if "N" in vector_group_l and transformer_2w.cgnd_l == TrfNeutralPointState.EARTHED:
+            if "N" in vector_group_l.value and transformer_2w.cgnd_l == TrfNeutralPointState.EARTHED:
                 re_l = transformer_2w.re0tr_l
                 xe_l = transformer_2w.xe0tr_l
             else:
                 re_l = None
                 xe_l = None
 
             wh = Winding(
```

### Comparing `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/exporter/load_power.py` & `ieeh-powerfactory-tools-1.5.1/powerfactory_tools/exporter/load_power.py`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/interface.py` & `ieeh-powerfactory-tools-1.5.1/powerfactory_tools/interface.py`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/powerfactory_types.py` & `ieeh-powerfactory-tools-1.5.1/powerfactory_tools/powerfactory_types.py`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.5.0/powerfactory_tools/utils/io.py` & `ieeh-powerfactory-tools-1.5.1/powerfactory_tools/utils/io.py`

 * *Files identical despite different names*

### Comparing `ieeh-powerfactory-tools-1.5.0/pyproject.toml` & `ieeh-powerfactory-tools-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "loguru",
     "pydantic",
 ]
 description = "A toolbox for Python based control of DIgSILENT PowerFactory"
 name = "ieeh-powerfactory-tools"
 readme = "README.md"
 requires-python = ">=3.10,<3.11"
-version = "1.5.0"
+version = "1.5.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/ieeh-tu-dresden/powerfactory-tools"
 
@@ -100,15 +100,15 @@
 
 [tool.black]
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
-version = "1.5.0"
+version = "1.5.1"
 version_files = [
     ".zenodo.json:version",
     "CITATION.cff:cff-version",
     "pyproject.toml:version",
 ]
 
 [tool.mypy]
```

### Comparing `ieeh-powerfactory-tools-1.5.0/PKG-INFO` & `ieeh-powerfactory-tools-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieeh-powerfactory-tools
-Version: 1.5.0
+Version: 1.5.1
 Summary: A toolbox for Python based control of DIgSILENT PowerFactory
 Author-email: Sasan Jacob Rasti <sasan_jacob.rasti@tu-dresden.de>,Maximilian Schmidt <maximilian.schmidt@tu-dresden.de>,Sebastian Krahmer <sebastian.krahmer@tu-dresden.de>
 Requires-Python: >=3.10,<3.11
 Project-URL: Source, https://github.com/ieeh-tu-dresden/powerfactory-tools
 Description-Content-Type: text/markdown
 
 # IEEH PowerFactory Tools
```

