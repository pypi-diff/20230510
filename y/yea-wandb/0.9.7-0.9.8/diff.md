# Comparing `tmp/yea-wandb-0.9.7.tar.gz` & `tmp/yea-wandb-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yea-wandb-0.9.7.tar", last modified: Wed Apr 26 18:34:11 2023, max compression
+gzip compressed data, was "yea-wandb-0.9.8.tar", last modified: Wed May 10 14:20:36 2023, max compression
```

## Comparing `yea-wandb-0.9.7.tar` & `yea-wandb-0.9.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-04-26 18:34:11.809271 yea-wandb-0.9.7/
--rw-r--r--   0 kpt        (501) staff       (20)     1075 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/LICENSE
--rw-r--r--   0 kpt        (501) staff       (20)       58 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/MANIFEST.in
--rw-r--r--   0 kpt        (501) staff       (20)      154 2023-04-26 18:34:11.808911 yea-wandb-0.9.7/PKG-INFO
--rw-r--r--   0 kpt        (501) staff       (20)      885 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/README.md
--rw-r--r--   0 kpt        (501) staff       (20)      112 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/pyproject.toml
--rw-r--r--   0 kpt        (501) staff       (20)       38 2023-04-26 18:34:11.809368 yea-wandb-0.9.7/setup.cfg
--rw-r--r--   0 kpt        (501) staff       (20)      543 2023-04-26 17:04:01.000000 yea-wandb-0.9.7/setup.py
-drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-04-26 18:34:11.794563 yea-wandb-0.9.7/src/
-drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-04-26 18:34:11.804062 yea-wandb-0.9.7/src/yea_wandb/
--rw-r--r--   0 kpt        (501) staff       (20)       68 2023-04-26 17:04:01.000000 yea-wandb-0.9.7/src/yea_wandb/__init__.py
--rw-r--r--   0 kpt        (501) staff       (20)     6163 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/src/yea_wandb/artifact_emu.py
--rwxr-xr-x   0 kpt        (501) staff       (20)     8703 2023-04-26 17:04:01.000000 yea-wandb-0.9.7/src/yea_wandb/backend.py
--rw-r--r--   0 kpt        (501) staff       (20)     1676 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/hook.py
--rw-r--r--   0 kpt        (501) staff       (20)     3486 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/mitm.py
--rw-r--r--   0 kpt        (501) staff       (20)     9312 2022-08-19 03:13:13.000000 yea-wandb-0.9.7/src/yea_wandb/mock_requests.py
--rw-r--r--   0 kpt        (501) staff       (20)   105508 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/mock_server.py
--rw-r--r--   0 kpt        (501) staff       (20)    10623 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/plugin.py
--rw-r--r--   0 kpt        (501) staff       (20)     4847 2023-03-17 22:36:04.000000 yea-wandb-0.9.7/src/yea_wandb/setup.py
-drwxr-xr-x   0 kpt        (501) staff       (20)        0 2023-04-26 18:34:11.808331 yea-wandb-0.9.7/src/yea_wandb.egg-info/
--rw-r--r--   0 kpt        (501) staff       (20)      154 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/PKG-INFO
--rw-r--r--   0 kpt        (501) staff       (20)      545 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 kpt        (501) staff       (20)        1 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 kpt        (501) staff       (20)       43 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/entry_points.txt
--rw-r--r--   0 kpt        (501) staff       (20)        1 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/not-zip-safe
--rw-r--r--   0 kpt        (501) staff       (20)       43 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/requires.txt
--rw-r--r--   0 kpt        (501) staff       (20)       10 2023-04-26 18:34:11.000000 yea-wandb-0.9.7/src/yea_wandb.egg-info/top_level.txt
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-05-10 14:20:36.877453 yea-wandb-0.9.8/
+-rw-r--r--   0 jeff       (501) staff       (20)     1075 2022-05-30 23:04:24.000000 yea-wandb-0.9.8/LICENSE
+-rw-r--r--   0 jeff       (501) staff       (20)       58 2022-05-30 23:04:24.000000 yea-wandb-0.9.8/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)      154 2023-05-10 14:20:36.877152 yea-wandb-0.9.8/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      885 2022-05-30 23:04:24.000000 yea-wandb-0.9.8/README.md
+-rw-r--r--   0 jeff       (501) staff       (20)      112 2022-05-30 23:04:24.000000 yea-wandb-0.9.8/pyproject.toml
+-rw-r--r--   0 jeff       (501) staff       (20)       38 2023-05-10 14:20:36.877647 yea-wandb-0.9.8/setup.cfg
+-rw-r--r--   0 jeff       (501) staff       (20)      543 2023-05-10 14:19:45.000000 yea-wandb-0.9.8/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-05-10 14:20:36.855986 yea-wandb-0.9.8/src/
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-05-10 14:20:36.869980 yea-wandb-0.9.8/src/yea_wandb/
+-rw-r--r--   0 jeff       (501) staff       (20)       68 2023-05-10 14:19:45.000000 yea-wandb-0.9.8/src/yea_wandb/__init__.py
+-rw-r--r--   0 jeff       (501) staff       (20)     6163 2022-06-21 16:50:06.000000 yea-wandb-0.9.8/src/yea_wandb/artifact_emu.py
+-rwxr-xr-x   0 jeff       (501) staff       (20)     8703 2023-05-10 14:18:59.000000 yea-wandb-0.9.8/src/yea_wandb/backend.py
+-rw-r--r--   0 jeff       (501) staff       (20)     1676 2023-01-05 23:53:31.000000 yea-wandb-0.9.8/src/yea_wandb/hook.py
+-rw-r--r--   0 jeff       (501) staff       (20)     3486 2023-01-05 23:53:31.000000 yea-wandb-0.9.8/src/yea_wandb/mitm.py
+-rw-r--r--   0 jeff       (501) staff       (20)     9312 2022-07-08 02:01:53.000000 yea-wandb-0.9.8/src/yea_wandb/mock_requests.py
+-rw-r--r--   0 jeff       (501) staff       (20)   106220 2023-05-10 14:19:45.000000 yea-wandb-0.9.8/src/yea_wandb/mock_server.py
+-rw-r--r--   0 jeff       (501) staff       (20)    10623 2023-01-05 23:53:31.000000 yea-wandb-0.9.8/src/yea_wandb/plugin.py
+-rw-r--r--   0 jeff       (501) staff       (20)     4847 2023-01-05 23:53:31.000000 yea-wandb-0.9.8/src/yea_wandb/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-05-10 14:20:36.876194 yea-wandb-0.9.8/src/yea_wandb.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)      154 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      545 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       43 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/entry_points.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 jeff       (501) staff       (20)       43 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/requires.txt
+-rw-r--r--   0 jeff       (501) staff       (20)       10 2023-05-10 14:20:36.000000 yea-wandb-0.9.8/src/yea_wandb.egg-info/top_level.txt
```

### Comparing `yea-wandb-0.9.7/LICENSE` & `yea-wandb-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/README.md` & `yea-wandb-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/setup.py` & `yea-wandb-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """yea setup."""
 
 from setuptools import setup
 
 
 setup(
     name="yea-wandb",
-    version="0.9.7",
+    version="0.9.8",
     description="Test harness wandb plugin",
     packages=["yea_wandb"],
     install_requires=[
         "Flask",
         "requests",
         "responses",
         "pandas",
```

### Comparing `yea-wandb-0.9.7/src/yea_wandb/artifact_emu.py` & `yea-wandb-0.9.8/src/yea_wandb/artifact_emu.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/src/yea_wandb/backend.py` & `yea-wandb-0.9.8/src/yea_wandb/backend.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/src/yea_wandb/hook.py` & `yea-wandb-0.9.8/src/yea_wandb/hook.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/src/yea_wandb/mitm.py` & `yea-wandb-0.9.8/src/yea_wandb/mitm.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/src/yea_wandb/mock_requests.py` & `yea-wandb-0.9.8/src/yea_wandb/mock_requests.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/src/yea_wandb/mock_server.py` & `yea-wandb-0.9.8/src/yea_wandb/mock_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1206,14 +1206,32 @@
             return {
                 "data": {
                     "updateArtifactManifest": {
                         "artifactManifest": manifest,
                     }
                 }
             }
+        if "query ProbeServerCreateArtifactFileSpecInput" in body["query"]:
+            return json.dumps(
+                {
+                    "data": {
+                        "CreateArtifactFileSpecInputInfoType": {
+                            "inputFields": [
+                                {"name": "artifactID"},
+                                {"name": "name"},
+                                {"name": "md5"},
+                                {"name": "mimetype"},
+                                {"name": "artifactManifestID"},
+                                {"name": "uploadPartsInput"},
+                            ]
+                        },
+                    }
+                }
+            )
+
         if "mutation CreateArtifactFiles" in body["query"]:
             if ART_EMU:
                 return ART_EMU.create_files(variables=body["variables"])
             return {
                 "data": {
                     "files": [
                         {
```

### Comparing `yea-wandb-0.9.7/src/yea_wandb/plugin.py` & `yea-wandb-0.9.8/src/yea_wandb/plugin.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/src/yea_wandb/setup.py` & `yea-wandb-0.9.8/src/yea_wandb/setup.py`

 * *Files identical despite different names*

### Comparing `yea-wandb-0.9.7/src/yea_wandb.egg-info/SOURCES.txt` & `yea-wandb-0.9.8/src/yea_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

