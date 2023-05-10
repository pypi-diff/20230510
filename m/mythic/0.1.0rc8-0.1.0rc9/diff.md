# Comparing `tmp/mythic-0.1.0rc8.tar.gz` & `tmp/mythic-0.1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic-0.1.0rc8.tar", last modified: Tue Apr 25 16:39:04 2023, max compression
+gzip compressed data, was "mythic-0.1.0rc9.tar", last modified: Mon May  1 17:50:40 2023, max compression
```

## Comparing `mythic-0.1.0rc8.tar` & `mythic-0.1.0rc9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 16:39:04.413421 mythic-0.1.0rc8/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-25 16:39:04.413068 mythic-0.1.0rc8/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc8/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 16:39:04.410702 mythic-0.1.0rc8/mythic/
--rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc8/mythic/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc8/mythic/graphql_queries.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    97649 2023-04-25 15:11:39.000000 mythic-0.1.0rc8/mythic/mythic.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3376 2023-04-25 16:38:38.000000 mythic-0.1.0rc8/mythic/mythic_classes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc8/mythic/mythic_exceptions.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc8/mythic/mythic_utilities.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 16:39:04.412605 mythic-0.1.0rc8/mythic.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-25 16:39:04.413520 mythic-0.1.0rc8/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-25 16:38:15.000000 mythic-0.1.0rc8/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-01 17:50:40.115728 mythic-0.1.0rc9/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-05-01 17:50:40.115341 mythic-0.1.0rc9/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc9/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-01 17:50:40.112937 mythic-0.1.0rc9/mythic/
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc9/mythic/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc9/mythic/graphql_queries.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    97649 2023-05-01 17:49:45.000000 mythic-0.1.0rc9/mythic/mythic.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3376 2023-04-25 16:38:38.000000 mythic-0.1.0rc9/mythic/mythic_classes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc9/mythic/mythic_exceptions.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc9/mythic/mythic_utilities.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-01 17:50:40.114907 mythic-0.1.0rc9/mythic.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-05-01 17:50:40.000000 mythic-0.1.0rc9/mythic.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-01 17:50:40.115831 mythic-0.1.0rc9/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-05-01 17:50:32.000000 mythic-0.1.0rc9/setup.py
```

### Comparing `mythic-0.1.0rc8/PKG-INFO` & `mythic-0.1.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc8
+Version: 0.1.0rc9
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc8/README.md` & `mythic-0.1.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc8/mythic/graphql_queries.py` & `mythic-0.1.0rc9/mythic/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc8/mythic/mythic.py` & `mythic-0.1.0rc9/mythic/mythic.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 async def update_callback(
         mythic: mythic_classes.Mythic,
         callback_display_id: int,
         active: bool = None,
         sleep_info: str = None,
         locked: bool = None,
         description: str = None,
-        ips: list[str] = None,
+        ips: List[str] = None,
         user: str = None,
         host: str = None,
         os: str = None,
         architecture: str = None,
         extra_info: str = None,
         pid: int = None,
         process_name: str = None,
@@ -2262,21 +2262,21 @@
 
 
 async def create_tag(mythic: mythic_classes.Mythic,
                      tag_type_id: int,
                      source: str = "",
                      url: str = "",
                      data: str = "",
-                     credential_ids: list[int] = None,
-                     filemeta_ids: list[int] = None,
-                     keylog_ids: list[int] = None,
-                     mythictree_ids: list[int] = None,
-                     response_ids: list[int] = None,
-                     task_ids: list[int] = None,
-                     taskartifact_ids: list[int] = None) -> list[dict]:
+                     credential_ids: List[int] = None,
+                     filemeta_ids: List[int] = None,
+                     keylog_ids: List[int] = None,
+                     mythictree_ids: List[int] = None,
+                     response_ids: List[int] = None,
+                     task_ids: List[int] = None,
+                     taskartifact_ids: List[int] = None) -> List[dict]:
     def get_mutation(target_object: str) -> str:
         return f"""
             mutation createTag($tagtype_id: Int!, $source: String!, $url: String!, $data: jsonb!, ${target_object}: Int!) {{
               insert_tag_one(object: {{data: $data, source: $source, tagtype_id: $tagtype_id, url: $url, {target_object}:${target_object}}}) {{
                 id
                 {target_object}
               }}
```

### Comparing `mythic-0.1.0rc8/mythic/mythic_classes.py` & `mythic-0.1.0rc9/mythic/mythic_classes.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc8/mythic/mythic_utilities.py` & `mythic-0.1.0rc9/mythic/mythic_utilities.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc8/mythic.egg-info/PKG-INFO` & `mythic-0.1.0rc9/mythic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc8
+Version: 0.1.0rc9
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc8/setup.py` & `mythic-0.1.0rc9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic",
-    version="0.1.0rc8",
+    version="0.1.0rc9",
     description="Interact with Mythic C2 Framework Instances",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/scripting",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

