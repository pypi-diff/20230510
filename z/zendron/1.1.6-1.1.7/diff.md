# Comparing `tmp/zendron-1.1.6.tar.gz` & `tmp/zendron-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zendron-1.1.6.tar", last modified: Sun Apr 30 00:31:20 2023, max compression
+gzip compressed data, was "zendron-1.1.7.tar", last modified: Wed May 10 19:13:09 2023, max compression
```

## Comparing `zendron-1.1.6.tar` & `zendron-1.1.7.tar`

### file list

```diff
@@ -1,53 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 00:30:55.000000 zendron-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-30 00:30:55.000000 zendron-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-30 00:31:20.044253 zendron-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-30 00:30:55.000000 zendron-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:30:55.000000 zendron-1.1.6/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-30 00:30:55.000000 zendron-1.1.6/conf/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/notes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/notes/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/notes/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-04-30 00:30:55.000000 zendron-1.1.6/notes/assets/images/zotero.api-key.md.zotero-api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:30:55.000000 zendron-1.1.6/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-30 00:30:55.000000 zendron-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 00:31:20.044253 zendron-1.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/src/zendron/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/cache_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/comments_deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/src/zendron/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/conf/config_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/conf/default_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/front.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.040253 zendron-1.1.6/src/zendron/pods/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/src/zendron/pods/dendron.markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/pods/dendron.markdown/config.import.yml
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/read_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-30 00:30:55.000000 zendron-1.1.6/src/zendron/user_citation_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 00:31:20.044253 zendron-1.1.6/src/zendron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 00:31:20.000000 zendron-1.1.6/src/zendron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.498339 zendron-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 19:12:58.000000 zendron-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-10 19:12:58.000000 zendron-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-10 19:13:09.498339 zendron-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-10 19:12:58.000000 zendron-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.490338 zendron-1.1.7/notes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.490338 zendron-1.1.7/notes/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.490338 zendron-1.1.7/notes/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   108556 2023-05-10 19:12:58.000000 zendron-1.1.7/notes/assets/images/zotero.api-key.md.zotero-api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.490338 zendron-1.1.7/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.494338 zendron-1.1.7/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 19:12:58.000000 zendron-1.1.7/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-10 19:12:58.000000 zendron-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 19:13:09.498339 zendron-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.490338 zendron-1.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.494338 zendron-1.1.7/src/zendron/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/cache_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/comments_deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.494338 zendron-1.1.7/src/zendron/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/conf/config_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/conf/default_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.490338 zendron-1.1.7/src/zendron/pods/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.498339 zendron-1.1.7/src/zendron/pods/dendron.markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/pods/dendron.markdown/config.import.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/read_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-10 19:12:58.000000 zendron-1.1.7/src/zendron/user_citation_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:13:09.494338 zendron-1.1.7/src/zendron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-10 19:13:09.000000 zendron-1.1.7/src/zendron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-10 19:13:09.000000 zendron-1.1.7/src/zendron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:13:09.000000 zendron-1.1.7/src/zendron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 19:13:09.000000 zendron-1.1.7/src/zendron.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-10 19:13:09.000000 zendron-1.1.7/src/zendron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 19:13:09.000000 zendron-1.1.7/src/zendron.egg-info/top_level.txt
```

### Comparing `zendron-1.1.6/LICENSE` & `zendron-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/PKG-INFO` & `zendron-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.6
+Version: 1.1.7
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zendron-1.1.6/README.md` & `zendron-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/notes/assets/images/zotero.api-key.md.zotero-api-key.png` & `zendron-1.1.7/notes/assets/images/zotero.api-key.md.zotero-api-key.png`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/pods/dendron.markdown/config.import.yml` & `zendron-1.1.7/src/zendron/pods/dendron.markdown/config.import.yml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/pyproject.toml` & `zendron-1.1.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=67.7.2", "wheel>=0.40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zendron"
-version = "1.1.6"
+version = "1.1.7"
 description = "Import Zotero annotations with Dendron integration"
 readme = "README.md"
 authors = [{ name = "Michael Volk", email = "michaeljvolk7@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `zendron-1.1.6/src/zendron/__main__.py` & `zendron-1.1.7/src/zendron/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 USER_CONFIGURE = False
 
 if init.user_configure():
     USER_CONFIGURE = True
 
 
 @hydra.main(
-    version_base=None, config_path=osp.join(os.getcwd(), "conf"), config_name="config"
+    version_base=None,
+    config_path=osp.join(os.getcwd(), "conf", "zendron"),
+    config_name="config",
 )
 def main(cfg: DictConfig) -> None:
     if USER_CONFIGURE:
         return
     elif cfg.remove:
         from zendron import remove
```

### Comparing `zendron-1.1.6/src/zendron/annotations.py` & `zendron-1.1.7/src/zendron/annotations.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/bibtex.py` & `zendron-1.1.7/src/zendron/bibtex.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/cache.py` & `zendron-1.1.7/src/zendron/cache.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/cache_deprecated.py` & `zendron-1.1.7/src/zendron/cache_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/comments.py` & `zendron-1.1.7/src/zendron/comments.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/comments_deprecated.py` & `zendron-1.1.7/src/zendron/comments_deprecated.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/conf/config_template.yaml` & `zendron-1.1.7/src/zendron/conf/config_template.yaml`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/config.py` & `zendron-1.1.7/src/zendron/config.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/front.py` & `zendron-1.1.7/src/zendron/front.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/init.py` & `zendron-1.1.7/src/zendron/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 from omegaconf import OmegaConf
 
 
 def load_default_config():
     workspace_root = os.getcwd()
-    default_config_path = osp.join(workspace_root, "conf", "default.yaml")
+    default_config_path = osp.join(workspace_root, "conf", "zendron", "default.yaml")
     if not osp.exists(default_config_path):
         return False
     return OmegaConf.load(default_config_path)
 
 
 def is_initialized() -> bool:
     try:
@@ -28,15 +28,15 @@
     return is_zendron_initialized
 
 
 def set_initialized():
     default_config = load_default_config()
     default_config.initialized = True
     workspace_root = os.getcwd()
-    default_config_path = osp.join(workspace_root, "conf", "default.yaml")
+    default_config_path = osp.join(workspace_root, "conf", "zendron", "default.yaml")
     OmegaConf.save(default_config, default_config_path)
 
     # Update config.import.yml with desired values
     config_path = osp.join(
         workspace_root, "pods", "dendron.markdown", "config.import.yml"
     )
     config = OmegaConf.load(config_path)
```

### Comparing `zendron-1.1.6/src/zendron/items.py` & `zendron-1.1.7/src/zendron/items.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/load.py` & `zendron-1.1.7/src/zendron/load.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/metadata.py` & `zendron-1.1.7/src/zendron/metadata.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/read_md.py` & `zendron-1.1.7/src/zendron/read_md.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/remove.py` & `zendron-1.1.7/src/zendron/remove.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/scratch.py` & `zendron-1.1.7/src/zendron/scratch.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/sync.py` & `zendron-1.1.7/src/zendron/sync.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron/user_citation_key.py` & `zendron-1.1.7/src/zendron/user_citation_key.py`

 * *Files identical despite different names*

### Comparing `zendron-1.1.6/src/zendron.egg-info/PKG-INFO` & `zendron-1.1.7/src/zendron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zendron
-Version: 1.1.6
+Version: 1.1.7
 Summary: Import Zotero annotations with Dendron integration
 Author-email: Michael Volk <michaeljvolk7@gmail.com>
 License: MIT License
         
         Copyright (c) [2022] [Michael Volk]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zendron-1.1.6/src/zendron.egg-info/SOURCES.txt` & `zendron-1.1.7/src/zendron.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-conf/__init__.py
-conf/default.yaml
-src/../conf/default.yaml
 src/../notes/assets/images/zotero.api-key.md.zotero-api-key.png
 src/../pods/dendron.markdown/config.import.yml
 src/zendron/__init__.py
 src/zendron/__main__.py
 src/zendron/annotations.py
 src/zendron/bibtex.py
 src/zendron/cache.py
```

