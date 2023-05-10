# Comparing `tmp/types-google-cloud-ndb-2.1.0.6.tar.gz` & `tmp/types-google-cloud-ndb-2.1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-google-cloud-ndb-2.1.0.6.tar", last modified: Tue Apr  4 15:15:59 2023, max compression
+gzip compressed data, was "types-google-cloud-ndb-2.1.0.7.tar", last modified: Wed May 10 15:22:36 2023, max compression
```

## Comparing `types-google-cloud-ndb-2.1.0.6.tar` & `types-google-cloud-ndb-2.1.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:15:59.358097 types-google-cloud-ndb-2.1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-04 15:15:58.000000 types-google-cloud-ndb-2.1.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 15:15:58.000000 types-google-cloud-ndb-2.1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-04 15:15:59.358097 types-google-cloud-ndb-2.1.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:15:59.354097 types-google-cloud-ndb-2.1.0.6/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-04 15:15:58.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:15:59.354097 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:15:59.358097 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_batch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_datastore_api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_datastore_query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_eventloop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_options.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/blobstore.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/context.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/django_middleware.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/global_cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/msgprop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/polymodel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/stats.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/tasklets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-04 15:15:34.000000 types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 15:15:59.358097 types-google-cloud-ndb-2.1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-04 15:15:58.000000 types-google-cloud-ndb-2.1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:15:59.358097 types-google-cloud-ndb-2.1.0.6/types_google_cloud_ndb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-04 15:15:59.000000 types-google-cloud-ndb-2.1.0.6/types_google_cloud_ndb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-04 15:15:59.000000 types-google-cloud-ndb-2.1.0.6/types_google_cloud_ndb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:15:59.000000 types-google-cloud-ndb-2.1.0.6/types_google_cloud_ndb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-04 15:15:59.000000 types-google-cloud-ndb-2.1.0.6/types_google_cloud_ndb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-10 15:22:35.000000 types-google-cloud-ndb-2.1.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:35.000000 types-google-cloud-ndb-2.1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 15:22:35.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.677130 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_datastore_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_datastore_query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_eventloop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/blobstore.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/django_middleware.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/global_cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18633 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/msgprop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/polymodel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/stats.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/tasklets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-10 15:19:44.000000 types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-10 15:22:35.000000 types-google-cloud-ndb-2.1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:36.681130 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-10 15:22:36.000000 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 15:22:36.000000 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:36.000000 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:22:36.000000 types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/top_level.txt
```

### Comparing `types-google-cloud-ndb-2.1.0.6/CHANGELOG.md` & `types-google-cloud-ndb-2.1.0.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.1.0.7 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 2.1.0.6 (2023-04-04)
 
 `google-cloud-ndb`, `paramiko`, `setuptools`: remove unnecessary `= ...`s (#10011)
 
 ## 2.1.0.5 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
```

### Comparing `types-google-cloud-ndb-2.1.0.6/PKG-INFO` & `types-google-cloud-ndb-2.1.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-google-cloud-ndb
-Version: 2.1.0.6
+Version: 2.1.0.7
 Summary: Typing stubs for google-cloud-ndb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `google-cloud-ndb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/google-cloud-ndb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `60939b00afede13feeec3cee6f6dfe6eb2df1593`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/__init__.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_cache.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_cache.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_datastore_query.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_datastore_query.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_eventloop.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_eventloop.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/_transaction.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/_transaction.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/blobstore.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/blobstore.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/client.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/context.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/context.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/exceptions.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/global_cache.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/global_cache.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/key.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/key.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/metadata.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/metadata.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/model.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/model.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/query.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/query.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/stats.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/stats.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/tasklets.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/tasklets.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/google-stubs/cloud/ndb/utils.pyi` & `types-google-cloud-ndb-2.1.0.7/google-stubs/cloud/ndb/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-google-cloud-ndb-2.1.0.6/setup.py` & `types-google-cloud-ndb-2.1.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `google-cloud-ndb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/google-cloud-ndb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `60939b00afede13feeec3cee6f6dfe6eb2df1593`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.1.0.6",
+      version="2.1.0.7",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md",
```

### Comparing `types-google-cloud-ndb-2.1.0.6/types_google_cloud_ndb.egg-info/PKG-INFO` & `types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-google-cloud-ndb
-Version: 2.1.0.6
+Version: 2.1.0.7
 Summary: Typing stubs for google-cloud-ndb
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/google-cloud-ndb.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `google-cloud-ndb`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/google-cloud-ndb. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `60939b00afede13feeec3cee6f6dfe6eb2df1593`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-google-cloud-ndb-2.1.0.6/types_google_cloud_ndb.egg-info/SOURCES.txt` & `types-google-cloud-ndb-2.1.0.7/types_google_cloud_ndb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

