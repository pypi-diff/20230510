# Comparing `tmp/phenotype2phenopacket-0.1.1.tar.gz` & `tmp/phenotype2phenopacket-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenotype2phenopacket-0.1.1.tar", max compression
+gzip compressed data, was "phenotype2phenopacket-0.2.0.tar", max compression
```

## Comparing `phenotype2phenopacket-0.1.1.tar` & `phenotype2phenopacket-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1320 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/README.md
--rw-r--r--   0        0        0      913 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/add/__init__.py
--rw-r--r--   0        0        0     2361 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/add/add_genes.py
--rw-r--r--   0        0        0      478 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/cli.py
--rw-r--r--   0        0        0     1092 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/cli_add.py
--rw-r--r--   0        0        0     1085 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/cli_convert.py
--rw-r--r--   0        0        0     1087 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/cli_create.py
--rw-r--r--   0        0        0        0 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/convert/__init__.py
--rw-r--r--   0        0        0     1123 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/convert/convert.py
--rw-r--r--   0        0        0        0 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/create/__init__.py
--rw-r--r--   0        0        0     1897 2023-05-10 13:49:27.609352 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/create/create.py
--rw-r--r--   0        0        0 16425815 2023-05-10 13:49:27.701354 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt
--rw-r--r--   0        0        0        0 2023-05-10 13:49:27.701354 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/utils/__init__.py
--rw-r--r--   0        0        0     2405 2023-05-10 13:49:27.701354 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/utils/gene_map_utils.py
--rw-r--r--   0        0        0    22255 2023-05-10 13:49:27.701354 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/utils/phenopacket_utils.py
--rw-r--r--   0        0        0     1925 2023-05-10 13:49:27.701354 phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/utils/utils.py
--rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 phenotype2phenopacket-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1320 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/README.md
+-rw-r--r--   0        0        0      913 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/add/__init__.py
+-rw-r--r--   0        0        0     2361 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/add/add_genes.py
+-rw-r--r--   0        0        0      478 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli.py
+-rw-r--r--   0        0        0     1092 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_add.py
+-rw-r--r--   0        0        0     1085 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_convert.py
+-rw-r--r--   0        0        0     1087 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_create.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/convert/__init__.py
+-rw-r--r--   0        0        0     1123 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/convert/convert.py
+-rw-r--r--   0        0        0        0 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/create/__init__.py
+-rw-r--r--   0        0        0     1897 2023-05-10 13:55:12.725255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/create/create.py
+-rw-r--r--   0        0        0 16425815 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt
+-rw-r--r--   0        0        0        0 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/__init__.py
+-rw-r--r--   0        0        0     2405 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/gene_map_utils.py
+-rw-r--r--   0        0        0    22255 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/phenopacket_utils.py
+-rw-r--r--   0        0        0     1925 2023-05-10 13:55:12.821255 phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/utils.py
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 phenotype2phenopacket-0.2.0/PKG-INFO
```

### Comparing `phenotype2phenopacket-0.1.1/README.md` & `phenotype2phenopacket-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/pyproject.toml` & `phenotype2phenopacket-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phenotype2phenopacket"
-version = "0.1.1"
+version = "0.2.0"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>"]
 readme = "README.md"
 packages = [{ include = "phenotype2phenopacket", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/add/add_genes.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/add/add_genes.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/cli_add.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_add.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/cli_convert.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_convert.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/cli_create.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/cli_create.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/convert/convert.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/convert/convert.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/create/create.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/create/create.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/utils/gene_map_utils.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/gene_map_utils.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/utils/phenopacket_utils.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/phenopacket_utils.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/src/phenotype2phenopacket/utils/utils.py` & `phenotype2phenopacket-0.2.0/src/phenotype2phenopacket/utils/utils.py`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.1.1/PKG-INFO` & `phenotype2phenopacket-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenotype2phenopacket
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

