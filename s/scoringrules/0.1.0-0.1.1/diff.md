# Comparing `tmp/scoringrules-0.1.0.tar.gz` & `tmp/scoringrules-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoringrules-0.1.0.tar", max compression
+gzip compressed data, was "scoringrules-0.1.1.tar", max compression
```

## Comparing `scoringrules-0.1.0.tar` & `scoringrules-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1633 2023-05-10 11:09:55.772988 scoringrules-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-09 10:34:15.261889 scoringrules-0.1.0/scoringrules/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 10:34:10.218297 scoringrules-0.1.0/scoringrules/brier.py
--rw-r--r--   0        0        0     3817 2023-05-10 10:45:53.522090 scoringrules-0.1.0/scoringrules/crps.py
--rw-r--r--   0        0        0      128 2023-05-10 10:42:11.317264 scoringrules-0.1.0/scoringrules/utils.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 scoringrules-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-10 12:48:41.343565 scoringrules-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1633 2023-05-10 12:50:44.962188 scoringrules-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-09 10:34:15.261889 scoringrules-0.1.1/scoringrules/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:34:10.218297 scoringrules-0.1.1/scoringrules/brier.py
+-rw-r--r--   0        0        0     3817 2023-05-10 10:45:53.522090 scoringrules-0.1.1/scoringrules/crps.py
+-rw-r--r--   0        0        0      128 2023-05-10 10:42:11.317264 scoringrules-0.1.1/scoringrules/utils.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 scoringrules-0.1.1/PKG-INFO
```

### Comparing `scoringrules-0.1.0/pyproject.toml` & `scoringrules-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scoringrules"
-version = "0.1.0"
+version = "0.1.1"
 description = "Scoring rules for probabilistic forecast evaluation."
 authors = ["Francesco Zanetta <zanetta.francesco@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.4"
 scipy = "^1.9.3"
```

### Comparing `scoringrules-0.1.0/scoringrules/crps.py` & `scoringrules-0.1.1/scoringrules/crps.py`

 * *Files identical despite different names*

