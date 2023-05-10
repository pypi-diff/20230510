# Comparing `tmp/django-grpc-1.0.7.tar.gz` & `tmp/django-grpc-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-grpc-1.0.7.tar", last modified: Wed Jun 10 18:50:28 2020, max compression
+gzip compressed data, was "dist/django-grpc-1.0.8.tar", last modified: Wed Jun 10 18:50:43 2020, max compression
```

## Comparing `django-grpc-1.0.7.tar` & `django-grpc-1.0.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:28.000000 django-grpc-1.0.7/
-drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc/
--rw-r--r--   0 stan      (1000) stan      (1000)       25 2019-01-18 20:56:45.000000 django-grpc-1.0.7/django_grpc/models.py
--rw-r--r--   0 stan      (1000) stan      (1000)      156 2019-01-18 21:09:30.000000 django-grpc-1.0.7/django_grpc/apps.py
--rw-r--r--   0 stan      (1000) stan      (1000)       22 2020-06-10 18:50:24.000000 django-grpc-1.0.7/django_grpc/__version__.py
--rw-r--r--   0 stan      (1000) stan      (1000)       37 2019-11-11 22:59:11.000000 django-grpc-1.0.7/django_grpc/__init__.py
-drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc/serializers/
--rw-rw-r--   0 stan      (1000) stan      (1000)      314 2019-01-17 23:01:12.000000 django-grpc-1.0.7/django_grpc/serializers/__init__.py
--rw-rw-r--   0 stan      (1000) stan      (1000)     3306 2019-01-23 16:19:19.000000 django-grpc-1.0.7/django_grpc/serializers/base.py
--rw-r--r--   0 stan      (1000) stan      (1000)     2428 2020-06-10 18:37:09.000000 django-grpc-1.0.7/django_grpc/utils.py
-drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc/signals/
--rw-r--r--   0 stan      (1000) stan      (1000)     2789 2020-02-03 21:12:25.000000 django-grpc-1.0.7/django_grpc/signals/wrapper.py
--rw-r--r--   0 stan      (1000) stan      (1000)      631 2020-02-03 21:12:25.000000 django-grpc-1.0.7/django_grpc/signals/__init__.py
-drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc/management/
--rw-rw-r--   0 stan      (1000) stan      (1000)        0 2019-01-16 14:57:31.000000 django-grpc-1.0.7/django_grpc/management/__init__.py
-drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc/management/commands/
--rw-r--r--   0 stan      (1000) stan      (1000)     1765 2020-02-03 21:12:25.000000 django-grpc-1.0.7/django_grpc/management/commands/grpcserver.py
-drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc.egg-info/
--rw-r--r--   0 stan      (1000) stan      (1000)       11 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc.egg-info/requires.txt
--rw-r--r--   0 stan      (1000) stan      (1000)        1 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 stan      (1000) stan      (1000)        1 2019-01-18 21:15:04.000000 django-grpc-1.0.7/django_grpc.egg-info/not-zip-safe
--rw-r--r--   0 stan      (1000) stan      (1000)      710 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 stan      (1000) stan      (1000)       34 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc.egg-info/top_level.txt
--rw-r--r--   0 stan      (1000) stan      (1000)     5341 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc.egg-info/PKG-INFO
-drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:28.000000 django-grpc-1.0.7/django_grpc_testtools/
--rw-r--r--   0 stan      (1000) stan      (1000)      834 2020-06-10 18:37:08.000000 django-grpc-1.0.7/django_grpc_testtools/executor.py
--rw-rw-r--   0 stan      (1000) stan      (1000)     1358 2020-02-10 16:11:02.000000 django-grpc-1.0.7/django_grpc_testtools/context.py
--rw-rw-r--   0 stan      (1000) stan      (1000)        0 2020-02-10 18:44:22.000000 django-grpc-1.0.7/django_grpc_testtools/__init__.py
--rw-r--r--   0 stan      (1000) stan      (1000)     3077 2019-12-09 18:47:30.000000 django-grpc-1.0.7/CONTRIBUTING.md
--rw-r--r--   0 stan      (1000) stan      (1000)      120 2019-12-09 18:45:45.000000 django-grpc-1.0.7/AUTHORS.md
--rwxr-xr-x   0 stan      (1000) stan      (1000)     2487 2020-02-10 18:46:28.000000 django-grpc-1.0.7/setup.py
--rw-r--r--   0 stan      (1000) stan      (1000)      323 2020-06-10 18:50:28.000000 django-grpc-1.0.7/setup.cfg
--rw-r--r--   0 stan      (1000) stan      (1000)     3715 2020-06-10 18:48:02.000000 django-grpc-1.0.7/README.md
--rw-r--r--   0 stan      (1000) stan      (1000)      174 2019-12-09 18:48:14.000000 django-grpc-1.0.7/MANIFEST.in
--rw-r--r--   0 stan      (1000) stan      (1000)     5341 2020-06-10 18:50:28.000000 django-grpc-1.0.7/PKG-INFO
--rw-r--r--   0 stan      (1000) stan      (1000)     1076 2019-01-18 20:56:45.000000 django-grpc-1.0.7/LICENSE
+drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:43.000000 django-grpc-1.0.8/
+drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc/
+-rw-r--r--   0 stan      (1000) stan      (1000)       25 2019-01-18 20:56:45.000000 django-grpc-1.0.8/django_grpc/models.py
+-rw-r--r--   0 stan      (1000) stan      (1000)      156 2019-01-18 21:09:30.000000 django-grpc-1.0.8/django_grpc/apps.py
+-rw-r--r--   0 stan      (1000) stan      (1000)       22 2020-06-10 18:50:42.000000 django-grpc-1.0.8/django_grpc/__version__.py
+-rw-r--r--   0 stan      (1000) stan      (1000)       37 2019-11-11 22:59:11.000000 django-grpc-1.0.8/django_grpc/__init__.py
+drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc/serializers/
+-rw-rw-r--   0 stan      (1000) stan      (1000)      314 2019-01-17 23:01:12.000000 django-grpc-1.0.8/django_grpc/serializers/__init__.py
+-rw-rw-r--   0 stan      (1000) stan      (1000)     3306 2019-01-23 16:19:19.000000 django-grpc-1.0.8/django_grpc/serializers/base.py
+-rw-r--r--   0 stan      (1000) stan      (1000)     2428 2020-06-10 18:37:09.000000 django-grpc-1.0.8/django_grpc/utils.py
+drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc/signals/
+-rw-r--r--   0 stan      (1000) stan      (1000)     2789 2020-02-03 21:12:25.000000 django-grpc-1.0.8/django_grpc/signals/wrapper.py
+-rw-r--r--   0 stan      (1000) stan      (1000)      631 2020-02-03 21:12:25.000000 django-grpc-1.0.8/django_grpc/signals/__init__.py
+drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc/management/
+-rw-rw-r--   0 stan      (1000) stan      (1000)        0 2019-01-16 14:57:31.000000 django-grpc-1.0.8/django_grpc/management/__init__.py
+drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc/management/commands/
+-rw-r--r--   0 stan      (1000) stan      (1000)     1765 2020-02-03 21:12:25.000000 django-grpc-1.0.8/django_grpc/management/commands/grpcserver.py
+drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc.egg-info/
+-rw-r--r--   0 stan      (1000) stan      (1000)       11 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc.egg-info/requires.txt
+-rw-r--r--   0 stan      (1000) stan      (1000)        1 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 stan      (1000) stan      (1000)        1 2019-01-18 21:15:04.000000 django-grpc-1.0.8/django_grpc.egg-info/not-zip-safe
+-rw-r--r--   0 stan      (1000) stan      (1000)      710 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 stan      (1000) stan      (1000)       34 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc.egg-info/top_level.txt
+-rw-r--r--   0 stan      (1000) stan      (1000)     5341 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc.egg-info/PKG-INFO
+drwxr-xr-x   0 stan      (1000) stan      (1000)        0 2020-06-10 18:50:43.000000 django-grpc-1.0.8/django_grpc_testtools/
+-rw-r--r--   0 stan      (1000) stan      (1000)      834 2020-06-10 18:37:08.000000 django-grpc-1.0.8/django_grpc_testtools/executor.py
+-rw-rw-r--   0 stan      (1000) stan      (1000)     1358 2020-02-10 16:11:02.000000 django-grpc-1.0.8/django_grpc_testtools/context.py
+-rw-rw-r--   0 stan      (1000) stan      (1000)        0 2020-02-10 18:44:22.000000 django-grpc-1.0.8/django_grpc_testtools/__init__.py
+-rw-r--r--   0 stan      (1000) stan      (1000)     3077 2019-12-09 18:47:30.000000 django-grpc-1.0.8/CONTRIBUTING.md
+-rw-r--r--   0 stan      (1000) stan      (1000)      120 2019-12-09 18:45:45.000000 django-grpc-1.0.8/AUTHORS.md
+-rwxr-xr-x   0 stan      (1000) stan      (1000)     2487 2020-02-10 18:46:28.000000 django-grpc-1.0.8/setup.py
+-rw-r--r--   0 stan      (1000) stan      (1000)      323 2020-06-10 18:50:43.000000 django-grpc-1.0.8/setup.cfg
+-rw-r--r--   0 stan      (1000) stan      (1000)     3715 2020-06-10 18:48:02.000000 django-grpc-1.0.8/README.md
+-rw-r--r--   0 stan      (1000) stan      (1000)      174 2019-12-09 18:48:14.000000 django-grpc-1.0.8/MANIFEST.in
+-rw-r--r--   0 stan      (1000) stan      (1000)     5341 2020-06-10 18:50:43.000000 django-grpc-1.0.8/PKG-INFO
+-rw-r--r--   0 stan      (1000) stan      (1000)     1076 2019-01-18 20:56:45.000000 django-grpc-1.0.8/LICENSE
```

### Comparing `django-grpc-1.0.7/django_grpc/serializers/base.py` & `django-grpc-1.0.8/django_grpc/serializers/base.py`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/django_grpc/utils.py` & `django-grpc-1.0.8/django_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/django_grpc/signals/wrapper.py` & `django-grpc-1.0.8/django_grpc/signals/wrapper.py`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/django_grpc/signals/__init__.py` & `django-grpc-1.0.8/django_grpc/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/django_grpc/management/commands/grpcserver.py` & `django-grpc-1.0.8/django_grpc/management/commands/grpcserver.py`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/django_grpc.egg-info/SOURCES.txt` & `django-grpc-1.0.8/django_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/django_grpc.egg-info/PKG-INFO` & `django-grpc-1.0.8/django_grpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-grpc
-Version: 1.0.7
+Version: 1.0.8
 Summary: Easy Django based gRPC service
 Home-page: https://github.com/gluk-w/django-grpc
 Author: Stan Misiurev
 Author-email: smisiurev@gmail.com
 License: MIT
 Description: # django-grpc
```

### Comparing `django-grpc-1.0.7/django_grpc_testtools/executor.py` & `django-grpc-1.0.8/django_grpc_testtools/executor.py`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/django_grpc_testtools/context.py` & `django-grpc-1.0.8/django_grpc_testtools/context.py`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/CONTRIBUTING.md` & `django-grpc-1.0.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/setup.py` & `django-grpc-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/README.md` & `django-grpc-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `django-grpc-1.0.7/PKG-INFO` & `django-grpc-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-grpc
-Version: 1.0.7
+Version: 1.0.8
 Summary: Easy Django based gRPC service
 Home-page: https://github.com/gluk-w/django-grpc
 Author: Stan Misiurev
 Author-email: smisiurev@gmail.com
 License: MIT
 Description: # django-grpc
```

### Comparing `django-grpc-1.0.7/LICENSE` & `django-grpc-1.0.8/LICENSE`

 * *Files identical despite different names*

