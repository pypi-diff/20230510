# Comparing `tmp/globus-compute-common-0.1.0.tar.gz` & `tmp/globus-compute-common-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-common-0.1.0.tar", last modified: Thu Mar  9 15:53:52 2023, max compression
+gzip compressed data, was "globus-compute-common-0.2.0.tar", last modified: Wed May 10 20:14:55 2023, max compression
```

## Comparing `globus-compute-common-0.1.0.tar` & `globus-compute-common-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.969737 globus-compute-common-0.1.0/
--rw-r--r--   0 lei        (501) staff       (20)      996 2023-03-09 15:53:52.969807 globus-compute-common-0.1.0/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      426 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/README.md
--rw-r--r--   0 lei        (501) staff       (20)     1362 2023-03-09 15:53:52.970205 globus-compute-common-0.1.0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)       38 2022-06-21 19:08:30.000000 globus-compute-common-0.1.0/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.963230 globus-compute-common-0.1.0/src/
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.964865 globus-compute-common-0.1.0/src/globus_compute_common/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     3652 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/globus_compute_flake8.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.966424 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/
--rw-r--r--   0 lei        (501) staff       (20)      501 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      523 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.967629 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/
--rw-r--r--   0 lei        (501) staff       (20)      771 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1830 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/base.py
--rw-r--r--   0 lei        (501) staff       (20)      545 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/container.py
--rw-r--r--   0 lei        (501) staff       (20)      599 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/ep_status_report.py
--rw-r--r--   0 lei        (501) staff       (20)      376 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/manager_status_report.py
--rw-r--r--   0 lei        (501) staff       (20)      631 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/result.py
--rw-r--r--   0 lei        (501) staff       (20)      363 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/task.py
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/task_cancel.py
--rw-r--r--   0 lei        (501) staff       (20)      428 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/task_transition.py
--rw-r--r--   0 lei        (501) staff       (20)     1568 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/packer.py
--rw-r--r--   0 lei        (501) staff       (20)      519 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/protocol.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.967876 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/protocol_versions/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/protocol_versions/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     4210 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/messagepack/protocol_versions/proto1.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.968622 globus-compute-common-0.1.0/src/globus_compute_common/redis/
--rw-r--r--   0 lei        (501) staff       (20)      898 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/redis/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1672 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/redis/connection.py
--rw-r--r--   0 lei        (501) staff       (20)     2163 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/redis/fields.py
--rw-r--r--   0 lei        (501) staff       (20)     7499 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/redis/pubsub.py
--rw-r--r--   0 lei        (501) staff       (20)     1654 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/redis/serde.py
--rw-r--r--   0 lei        (501) staff       (20)     1198 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/redis/task_queue.py
--rw-r--r--   0 lei        (501) staff       (20)     3676 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/redis_endpoint_lock.py
--rw-r--r--   0 lei        (501) staff       (20)     8212 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/redis_task.py
--rw-r--r--   0 lei        (501) staff       (20)      666 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/sdk_version_sharing.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.969247 globus-compute-common-0.1.0/src/globus_compute_common/task_storage/
--rw-r--r--   0 lei        (501) staff       (20)      313 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/task_storage/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1513 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/task_storage/base.py
--rw-r--r--   0 lei        (501) staff       (20)     1048 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/task_storage/default_storage.py
--rw-r--r--   0 lei        (501) staff       (20)     1036 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/task_storage/redis.py
--rw-r--r--   0 lei        (501) staff       (20)     6640 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/task_storage/s3.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.969622 globus-compute-common-0.1.0/src/globus_compute_common/tasks/
--rw-r--r--   0 lei        (501) staff       (20)      192 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/tasks/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1256 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/tasks/constants.py
--rw-r--r--   0 lei        (501) staff       (20)      592 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/tasks/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)      520 2023-03-09 15:52:23.000000 globus-compute-common-0.1.0/src/globus_compute_common/testing.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-03-09 15:53:52.965853 globus-compute-common-0.1.0/src/globus_compute_common.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)      996 2023-03-09 15:53:52.000000 globus-compute-common-0.1.0/src/globus_compute_common.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     2111 2023-03-09 15:53:52.000000 globus-compute-common-0.1.0/src/globus_compute_common.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-03-09 15:53:52.000000 globus-compute-common-0.1.0/src/globus_compute_common.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      138 2023-03-09 15:53:52.000000 globus-compute-common-0.1.0/src/globus_compute_common.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       22 2023-03-09 15:53:52.000000 globus-compute-common-0.1.0/src/globus_compute_common.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.566807 globus-compute-common-0.2.0/
+-rw-r--r--   0 chris      (501) staff       (20)      996 2023-05-10 20:14:55.566916 globus-compute-common-0.2.0/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      426 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/README.md
+-rw-r--r--   0 chris      (501) staff       (20)     1362 2023-05-10 20:14:55.567547 globus-compute-common-0.2.0/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)       38 2022-05-26 18:40:18.000000 globus-compute-common-0.2.0/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.556995 globus-compute-common-0.2.0/src/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.559657 globus-compute-common-0.2.0/src/globus_compute_common/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     3652 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/globus_compute_flake8.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.561339 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/
+-rw-r--r--   0 chris      (501) staff       (20)      501 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      523 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/exceptions.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.563481 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/
+-rw-r--r--   0 chris      (501) staff       (20)      771 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1830 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/base.py
+-rw-r--r--   0 chris      (501) staff       (20)      545 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/container.py
+-rw-r--r--   0 chris      (501) staff       (20)      599 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/ep_status_report.py
+-rw-r--r--   0 chris      (501) staff       (20)      376 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/manager_status_report.py
+-rw-r--r--   0 chris      (501) staff       (20)      631 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/result.py
+-rw-r--r--   0 chris      (501) staff       (20)      363 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/task.py
+-rw-r--r--   0 chris      (501) staff       (20)      131 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/task_cancel.py
+-rw-r--r--   0 chris      (501) staff       (20)      428 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/task_transition.py
+-rw-r--r--   0 chris      (501) staff       (20)     1568 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/packer.py
+-rw-r--r--   0 chris      (501) staff       (20)      519 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.563841 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol_versions/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol_versions/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     4305 2023-05-10 18:57:48.000000 globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol_versions/proto1.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.565147 globus-compute-common-0.2.0/src/globus_compute_common/redis/
+-rw-r--r--   0 chris      (501) staff       (20)      898 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1672 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/connection.py
+-rw-r--r--   0 chris      (501) staff       (20)     2163 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/fields.py
+-rw-r--r--   0 chris      (501) staff       (20)     7499 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/pubsub.py
+-rw-r--r--   0 chris      (501) staff       (20)     1654 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/serde.py
+-rw-r--r--   0 chris      (501) staff       (20)     1198 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis/task_queue.py
+-rw-r--r--   0 chris      (501) staff       (20)     3676 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis_endpoint_lock.py
+-rw-r--r--   0 chris      (501) staff       (20)     8212 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/redis_task.py
+-rw-r--r--   0 chris      (501) staff       (20)      666 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/sdk_version_sharing.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.566107 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/
+-rw-r--r--   0 chris      (501) staff       (20)      313 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1513 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/base.py
+-rw-r--r--   0 chris      (501) staff       (20)     1048 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/default_storage.py
+-rw-r--r--   0 chris      (501) staff       (20)     1036 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/redis.py
+-rw-r--r--   0 chris      (501) staff       (20)     6640 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/task_storage/s3.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.566664 globus-compute-common-0.2.0/src/globus_compute_common/tasks/
+-rw-r--r--   0 chris      (501) staff       (20)      192 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/tasks/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1256 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/tasks/constants.py
+-rw-r--r--   0 chris      (501) staff       (20)      592 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/tasks/protocol.py
+-rw-r--r--   0 chris      (501) staff       (20)      520 2023-03-09 16:59:27.000000 globus-compute-common-0.2.0/src/globus_compute_common/testing.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-05-10 20:14:55.560558 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      996 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     2111 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      138 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       22 2023-05-10 20:14:55.000000 globus-compute-common-0.2.0/src/globus_compute_common.egg-info/top_level.txt
```

### Comparing `globus-compute-common-0.1.0/PKG-INFO` & `globus-compute-common-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-common
-Version: 0.1.0
+Version: 0.2.0
 Summary: Common tools for Globus Compute projects
 Home-page: https://github.com/funcX-faas/funcx-common
 Author: Globus Team
 Author-email: support@globus.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `globus-compute-common-0.1.0/setup.cfg` & `globus-compute-common-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = globus-compute-common
-version = 0.1.0
+version = 0.2.0
 description = Common tools for Globus Compute projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/funcX-faas/funcx-common
 author = Globus Team
 author_email = support@globus.org
 classifiers =
```

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/globus_compute_flake8.py` & `globus-compute-common-0.2.0/src/globus_compute_common/globus_compute_flake8.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/exceptions.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/exceptions.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/__init__.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/base.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/container.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/container.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/ep_status_report.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/ep_status_report.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/message_types/result.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/message_types/result.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/packer.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/packer.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/protocol.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/messagepack/protocol_versions/proto1.py` & `globus-compute-common-0.2.0/src/globus_compute_common/messagepack/protocol_versions/proto1.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,15 +84,20 @@
     elif issubclass(model, Message):
         outer_type = "data"
         message_type = model.Meta.message_type
     else:
         raise NotImplementedError
 
     model_ = t.cast("type[pydantic.BaseModel]", model)
-    unknown_fields = {x for x in data if x not in model_.__fields__}
+
+    unknown_fields = set(data)
+    for name, field in model_.__fields__.items():
+        unknown_fields.discard(name)
+        unknown_fields.discard(field.alias)
+
     if unknown_fields:
         log.warning(
             "encountered unknown %s fields while reading a %s message: %s",
             outer_type,
             message_type,
             unknown_fields,
         )
```

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/redis/__init__.py` & `globus-compute-common-0.2.0/src/globus_compute_common/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/redis/connection.py` & `globus-compute-common-0.2.0/src/globus_compute_common/redis/connection.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/redis/fields.py` & `globus-compute-common-0.2.0/src/globus_compute_common/redis/fields.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/redis/pubsub.py` & `globus-compute-common-0.2.0/src/globus_compute_common/redis/pubsub.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/redis/serde.py` & `globus-compute-common-0.2.0/src/globus_compute_common/redis/serde.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/redis/task_queue.py` & `globus-compute-common-0.2.0/src/globus_compute_common/redis/task_queue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/redis_endpoint_lock.py` & `globus-compute-common-0.2.0/src/globus_compute_common/redis_endpoint_lock.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/redis_task.py` & `globus-compute-common-0.2.0/src/globus_compute_common/redis_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/sdk_version_sharing.py` & `globus-compute-common-0.2.0/src/globus_compute_common/sdk_version_sharing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/task_storage/base.py` & `globus-compute-common-0.2.0/src/globus_compute_common/task_storage/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/task_storage/default_storage.py` & `globus-compute-common-0.2.0/src/globus_compute_common/task_storage/default_storage.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/task_storage/redis.py` & `globus-compute-common-0.2.0/src/globus_compute_common/task_storage/redis.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/task_storage/s3.py` & `globus-compute-common-0.2.0/src/globus_compute_common/task_storage/s3.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/tasks/constants.py` & `globus-compute-common-0.2.0/src/globus_compute_common/tasks/constants.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/tasks/protocol.py` & `globus-compute-common-0.2.0/src/globus_compute_common/tasks/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common/testing.py` & `globus-compute-common-0.2.0/src/globus_compute_common/testing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common.egg-info/PKG-INFO` & `globus-compute-common-0.2.0/src/globus_compute_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-common
-Version: 0.1.0
+Version: 0.2.0
 Summary: Common tools for Globus Compute projects
 Home-page: https://github.com/funcX-faas/funcx-common
 Author: Globus Team
 Author-email: support@globus.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `globus-compute-common-0.1.0/src/globus_compute_common.egg-info/SOURCES.txt` & `globus-compute-common-0.2.0/src/globus_compute_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

