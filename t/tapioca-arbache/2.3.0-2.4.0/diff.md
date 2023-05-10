# Comparing `tmp/tapioca_arbache-2.3.0.tar.gz` & `tmp/tapioca_arbache-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapioca_arbache-2.3.0.tar", max compression
+gzip compressed data, was "tapioca_arbache-2.4.0.tar", max compression
```

## Comparing `tapioca_arbache-2.3.0.tar` & `tapioca_arbache-2.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2023-03-09 18:58:47.071625 tapioca_arbache-2.3.0/LICENSE
--rw-r--r--   0        0        0      506 2023-03-09 18:58:47.071625 tapioca_arbache-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-03-09 18:58:47.071625 tapioca_arbache-2.3.0/tapioca_arbache/__init__.py
--rw-r--r--   0        0        0     2319 2023-03-09 18:58:47.071625 tapioca_arbache-2.3.0/tapioca_arbache/resource_mapping.py
--rw-r--r--   0        0        0     6016 2023-03-09 18:58:47.071625 tapioca_arbache-2.3.0/tapioca_arbache/tapioca_arbache.py
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 tapioca_arbache-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/LICENSE
+-rw-r--r--   0        0        0      506 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/tapioca_arbache/__init__.py
+-rw-r--r--   0        0        0     2327 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/tapioca_arbache/resource_mapping.py
+-rw-r--r--   0        0        0     6016 2023-05-10 00:54:45.318021 tapioca_arbache-2.4.0/tapioca_arbache/tapioca_arbache.py
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 tapioca_arbache-2.4.0/PKG-INFO
```

### Comparing `tapioca_arbache-2.3.0/LICENSE` & `tapioca_arbache-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tapioca_arbache-2.3.0/tapioca_arbache/resource_mapping.py` & `tapioca_arbache-2.4.0/tapioca_arbache/resource_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 PLAY_SUBDOMINIO_ENDPOINT = {
     "subdominios": {
         "resource": "/subdominios/",
         "methods": ["POST"],
     },
     "subdominio": {
         "resource": "/subdominios/{codigo}/",
-        "methods": ["PATCH"],
-    }
+        "methods": ["PATCH", "GET"],
+    },
 }
 
 PLAY_JOGO_SUBDOMINIO_ENDPOINT = {
     "jogos": {
         "resource": "/jogos-subdominios/",
         "methods": ["POST"],
     },
```

### Comparing `tapioca_arbache-2.3.0/tapioca_arbache/tapioca_arbache.py` & `tapioca_arbache-2.4.0/tapioca_arbache/tapioca_arbache.py`

 * *Files identical despite different names*

