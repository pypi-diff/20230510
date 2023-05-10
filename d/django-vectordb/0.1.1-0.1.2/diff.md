# Comparing `tmp/django-vectordb-0.1.1.tar.gz` & `tmp/django-vectordb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vectordb-0.1.1.tar", last modified: Sat May  6 08:32:12 2023, max compression
+gzip compressed data, was "django-vectordb-0.1.2.tar", last modified: Wed May 10 05:40:54 2023, max compression
```

## Comparing `django-vectordb-0.1.1.tar` & `django-vectordb-0.1.2.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.923607 django-vectordb-0.1.1/
--rw-r--r--   0 pride      (501) staff       (20)    11357 2023-05-04 13:28:35.000000 django-vectordb-0.1.1/LICENSE
--rw-r--r--   0 pride      (501) staff       (20)    11705 2023-05-06 08:32:12.923974 django-vectordb-0.1.1/PKG-INFO
--rw-r--r--   0 pride      (501) staff       (20)    10305 2023-05-06 08:01:40.000000 django-vectordb-0.1.1/README.md
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.782469 django-vectordb-0.1.1/django_vectordb.egg-info/
--rw-r--r--   0 pride      (501) staff       (20)    11705 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/PKG-INFO
--rw-r--r--   0 pride      (501) staff       (20)     1365 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/SOURCES.txt
--rw-r--r--   0 pride      (501) staff       (20)        1 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/dependency_links.txt
--rw-r--r--   0 pride      (501) staff       (20)      319 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/requires.txt
--rw-r--r--   0 pride      (501) staff       (20)        9 2023-05-06 08:32:12.000000 django-vectordb-0.1.1/django_vectordb.egg-info/top_level.txt
--rw-r--r--   0 pride      (501) staff       (20)       80 2023-05-04 08:19:18.000000 django-vectordb-0.1.1/pyproject.toml
--rw-r--r--   0 pride      (501) staff       (20)     1888 2023-05-06 08:32:12.928178 django-vectordb-0.1.1/setup.cfg
--rw-r--r--   0 pride      (501) staff       (20)      216 2023-05-05 07:20:09.000000 django-vectordb-0.1.1/setup.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.805388 django-vectordb-0.1.1/vectordb/
--rw-r--r--   0 pride      (501) staff       (20)      291 2023-05-04 15:04:49.000000 django-vectordb-0.1.1/vectordb/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)      527 2023-05-05 06:20:34.000000 django-vectordb-0.1.1/vectordb/admin.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.811137 django-vectordb-0.1.1/vectordb/ann/
--rw-r--r--   0 pride      (501) staff       (20)      115 2023-05-03 14:11:45.000000 django-vectordb-0.1.1/vectordb/ann/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)     1051 2023-05-03 14:11:45.000000 django-vectordb-0.1.1/vectordb/ann/abcz.py
--rw-r--r--   0 pride      (501) staff       (20)     5918 2023-05-04 15:47:14.000000 django-vectordb-0.1.1/vectordb/ann/indexes.py
--rw-r--r--   0 pride      (501) staff       (20)      603 2023-05-04 15:46:27.000000 django-vectordb-0.1.1/vectordb/ann/singleton.py
--rw-r--r--   0 pride      (501) staff       (20)      248 2023-05-03 20:04:15.000000 django-vectordb-0.1.1/vectordb/apps.py
--rw-r--r--   0 pride      (501) staff       (20)      625 2023-05-06 07:32:16.000000 django-vectordb-0.1.1/vectordb/checks.py
--rw-r--r--   0 pride      (501) staff       (20)     1827 2023-05-04 04:39:07.000000 django-vectordb-0.1.1/vectordb/embedding_functions.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.812593 django-vectordb-0.1.1/vectordb/management/
--rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:40.000000 django-vectordb-0.1.1/vectordb/management/__init__.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.817051 django-vectordb-0.1.1/vectordb/management/commands/
--rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:44.000000 django-vectordb-0.1.1/vectordb/management/commands/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)     1020 2023-05-06 07:56:41.000000 django-vectordb-0.1.1/vectordb/management/commands/vectordb_reset.py
--rw-r--r--   0 pride      (501) staff       (20)     2276 2023-05-06 07:56:43.000000 django-vectordb-0.1.1/vectordb/management/commands/vectordb_sync.py
--rw-r--r--   0 pride      (501) staff       (20)     2813 2023-05-05 07:01:23.000000 django-vectordb-0.1.1/vectordb/manager.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.827774 django-vectordb-0.1.1/vectordb/migrations/
--rw-r--r--   0 pride      (501) staff       (20)     1892 2023-05-03 14:16:42.000000 django-vectordb-0.1.1/vectordb/migrations/0001_initial.py
--rw-r--r--   0 pride      (501) staff       (20)      887 2023-05-03 20:38:37.000000 django-vectordb-0.1.1/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py
--rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-03 14:10:09.000000 django-vectordb-0.1.1/vectordb/migrations/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)     2099 2023-05-04 20:10:03.000000 django-vectordb-0.1.1/vectordb/models.py
--rw-r--r--   0 pride      (501) staff       (20)     4464 2023-05-06 08:24:10.000000 django-vectordb-0.1.1/vectordb/queryset.py
--rw-r--r--   0 pride      (501) staff       (20)      342 2023-05-03 14:26:35.000000 django-vectordb-0.1.1/vectordb/serializers.py
--rw-r--r--   0 pride      (501) staff       (20)     3541 2023-05-06 07:26:56.000000 django-vectordb-0.1.1/vectordb/settings.py
--rw-r--r--   0 pride      (501) staff       (20)     1528 2023-05-05 06:33:16.000000 django-vectordb-0.1.1/vectordb/signals.py
--rw-r--r--   0 pride      (501) staff       (20)     1971 2023-05-04 20:13:05.000000 django-vectordb-0.1.1/vectordb/sync_signals.py
--rw-r--r--   0 pride      (501) staff       (20)     1475 2023-05-04 04:00:22.000000 django-vectordb-0.1.1/vectordb/tasks.py
-drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-06 08:32:12.922377 django-vectordb-0.1.1/vectordb/tests/
--rw-r--r--   0 pride      (501) staff       (20)       54 2023-05-04 20:37:23.000000 django-vectordb-0.1.1/vectordb/tests/__init__.py
--rw-r--r--   0 pride      (501) staff       (20)      122 2023-05-04 20:37:23.000000 django-vectordb-0.1.1/vectordb/tests/apps.py
--rw-r--r--   0 pride      (501) staff       (20)      106 2023-05-06 07:32:13.000000 django-vectordb-0.1.1/vectordb/tests/dummy_module.py
--rw-r--r--   0 pride      (501) staff       (20)      346 2023-05-04 20:37:23.000000 django-vectordb-0.1.1/vectordb/tests/models.py
--rw-r--r--   0 pride      (501) staff       (20)     1794 2023-05-04 13:22:55.000000 django-vectordb-0.1.1/vectordb/tests/settings.py
--rw-r--r--   0 pride      (501) staff       (20)     1170 2023-05-04 20:41:32.000000 django-vectordb-0.1.1/vectordb/tests/test_api_endpoint.py
--rw-r--r--   0 pride      (501) staff       (20)     2970 2023-05-04 20:41:19.000000 django-vectordb-0.1.1/vectordb/tests/test_db_indexes.py
--rw-r--r--   0 pride      (501) staff       (20)      686 2023-05-03 14:14:51.000000 django-vectordb-0.1.1/vectordb/tests/test_embedding_functions.py
--rw-r--r--   0 pride      (501) staff       (20)     2606 2023-05-06 07:32:11.000000 django-vectordb-0.1.1/vectordb/tests/test_settings.py
--rw-r--r--   0 pride      (501) staff       (20)      627 2023-05-04 20:42:47.000000 django-vectordb-0.1.1/vectordb/tests/test_singleton_meta.py
--rw-r--r--   0 pride      (501) staff       (20)     3547 2023-05-04 19:22:55.000000 django-vectordb-0.1.1/vectordb/tests/test_vectordb.py
--rw-r--r--   0 pride      (501) staff       (20)       60 2023-05-03 14:10:09.000000 django-vectordb-0.1.1/vectordb/tests.py
--rw-r--r--   0 pride      (501) staff       (20)      280 2023-05-04 20:40:02.000000 django-vectordb-0.1.1/vectordb/urls.py
--rw-r--r--   0 pride      (501) staff       (20)     3549 2023-05-06 07:28:17.000000 django-vectordb-0.1.1/vectordb/utils.py
--rw-r--r--   0 pride      (501) staff       (20)     1744 2023-05-04 18:22:43.000000 django-vectordb-0.1.1/vectordb/validators.py
--rw-r--r--   0 pride      (501) staff       (20)     1232 2023-05-05 06:34:07.000000 django-vectordb-0.1.1/vectordb/views.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.145229 django-vectordb-0.1.2/
+-rw-r--r--   0 pride      (501) staff       (20)    11357 2023-05-04 13:28:35.000000 django-vectordb-0.1.2/LICENSE
+-rw-r--r--   0 pride      (501) staff       (20)    12009 2023-05-10 05:40:54.145735 django-vectordb-0.1.2/PKG-INFO
+-rw-r--r--   0 pride      (501) staff       (20)    10609 2023-05-07 03:33:50.000000 django-vectordb-0.1.2/README.md
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.047330 django-vectordb-0.1.2/django_vectordb.egg-info/
+-rw-r--r--   0 pride      (501) staff       (20)    12009 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/PKG-INFO
+-rw-r--r--   0 pride      (501) staff       (20)     1387 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 pride      (501) staff       (20)        1 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 pride      (501) staff       (20)      319 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/requires.txt
+-rw-r--r--   0 pride      (501) staff       (20)        9 2023-05-10 05:40:54.000000 django-vectordb-0.1.2/django_vectordb.egg-info/top_level.txt
+-rw-r--r--   0 pride      (501) staff       (20)       80 2023-05-04 08:19:18.000000 django-vectordb-0.1.2/pyproject.toml
+-rw-r--r--   0 pride      (501) staff       (20)     1888 2023-05-10 05:40:54.153980 django-vectordb-0.1.2/setup.cfg
+-rw-r--r--   0 pride      (501) staff       (20)      216 2023-05-05 07:20:09.000000 django-vectordb-0.1.2/setup.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.081714 django-vectordb-0.1.2/vectordb/
+-rw-r--r--   0 pride      (501) staff       (20)      291 2023-05-04 15:04:49.000000 django-vectordb-0.1.2/vectordb/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)      527 2023-05-05 06:20:34.000000 django-vectordb-0.1.2/vectordb/admin.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.091992 django-vectordb-0.1.2/vectordb/ann/
+-rw-r--r--   0 pride      (501) staff       (20)      115 2023-05-03 14:11:45.000000 django-vectordb-0.1.2/vectordb/ann/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)     1051 2023-05-03 14:11:45.000000 django-vectordb-0.1.2/vectordb/ann/abcz.py
+-rw-r--r--   0 pride      (501) staff       (20)     5918 2023-05-04 15:47:14.000000 django-vectordb-0.1.2/vectordb/ann/indexes.py
+-rw-r--r--   0 pride      (501) staff       (20)      603 2023-05-04 15:46:27.000000 django-vectordb-0.1.2/vectordb/ann/singleton.py
+-rw-r--r--   0 pride      (501) staff       (20)      248 2023-05-03 20:04:15.000000 django-vectordb-0.1.2/vectordb/apps.py
+-rw-r--r--   0 pride      (501) staff       (20)      625 2023-05-06 07:32:16.000000 django-vectordb-0.1.2/vectordb/checks.py
+-rw-r--r--   0 pride      (501) staff       (20)     1827 2023-05-04 04:39:07.000000 django-vectordb-0.1.2/vectordb/embedding_functions.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.094206 django-vectordb-0.1.2/vectordb/management/
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:40.000000 django-vectordb-0.1.2/vectordb/management/__init__.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.104687 django-vectordb-0.1.2/vectordb/management/commands/
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-06 07:56:44.000000 django-vectordb-0.1.2/vectordb/management/commands/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)     1020 2023-05-06 07:56:41.000000 django-vectordb-0.1.2/vectordb/management/commands/vectordb_reset.py
+-rw-r--r--   0 pride      (501) staff       (20)     2276 2023-05-06 07:56:43.000000 django-vectordb-0.1.2/vectordb/management/commands/vectordb_sync.py
+-rw-r--r--   0 pride      (501) staff       (20)     2813 2023-05-05 07:01:23.000000 django-vectordb-0.1.2/vectordb/manager.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.112360 django-vectordb-0.1.2/vectordb/migrations/
+-rw-r--r--   0 pride      (501) staff       (20)     1892 2023-05-03 14:16:42.000000 django-vectordb-0.1.2/vectordb/migrations/0001_initial.py
+-rw-r--r--   0 pride      (501) staff       (20)      887 2023-05-03 20:38:37.000000 django-vectordb-0.1.2/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py
+-rw-r--r--   0 pride      (501) staff       (20)        0 2023-05-03 14:10:09.000000 django-vectordb-0.1.2/vectordb/migrations/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)     2099 2023-05-04 20:10:03.000000 django-vectordb-0.1.2/vectordb/models.py
+-rw-r--r--   0 pride      (501) staff       (20)     4464 2023-05-06 08:24:10.000000 django-vectordb-0.1.2/vectordb/queryset.py
+-rw-r--r--   0 pride      (501) staff       (20)      342 2023-05-03 14:26:35.000000 django-vectordb-0.1.2/vectordb/serializers.py
+-rw-r--r--   0 pride      (501) staff       (20)     3541 2023-05-06 07:26:56.000000 django-vectordb-0.1.2/vectordb/settings.py
+-rw-r--r--   0 pride      (501) staff       (20)     1073 2023-05-10 05:01:46.000000 django-vectordb-0.1.2/vectordb/shortcuts.py
+-rw-r--r--   0 pride      (501) staff       (20)     1528 2023-05-05 06:33:16.000000 django-vectordb-0.1.2/vectordb/signals.py
+-rw-r--r--   0 pride      (501) staff       (20)     1971 2023-05-04 20:13:05.000000 django-vectordb-0.1.2/vectordb/sync_signals.py
+-rw-r--r--   0 pride      (501) staff       (20)     1475 2023-05-04 04:00:22.000000 django-vectordb-0.1.2/vectordb/tasks.py
+drwxr-xr-x   0 pride      (501) staff       (20)        0 2023-05-10 05:40:54.143630 django-vectordb-0.1.2/vectordb/tests/
+-rw-r--r--   0 pride      (501) staff       (20)       54 2023-05-04 20:37:23.000000 django-vectordb-0.1.2/vectordb/tests/__init__.py
+-rw-r--r--   0 pride      (501) staff       (20)      122 2023-05-04 20:37:23.000000 django-vectordb-0.1.2/vectordb/tests/apps.py
+-rw-r--r--   0 pride      (501) staff       (20)      106 2023-05-06 07:32:13.000000 django-vectordb-0.1.2/vectordb/tests/dummy_module.py
+-rw-r--r--   0 pride      (501) staff       (20)      346 2023-05-04 20:37:23.000000 django-vectordb-0.1.2/vectordb/tests/models.py
+-rw-r--r--   0 pride      (501) staff       (20)     1794 2023-05-04 13:22:55.000000 django-vectordb-0.1.2/vectordb/tests/settings.py
+-rw-r--r--   0 pride      (501) staff       (20)     1170 2023-05-04 20:41:32.000000 django-vectordb-0.1.2/vectordb/tests/test_api_endpoint.py
+-rw-r--r--   0 pride      (501) staff       (20)     2970 2023-05-04 20:41:19.000000 django-vectordb-0.1.2/vectordb/tests/test_db_indexes.py
+-rw-r--r--   0 pride      (501) staff       (20)      686 2023-05-03 14:14:51.000000 django-vectordb-0.1.2/vectordb/tests/test_embedding_functions.py
+-rw-r--r--   0 pride      (501) staff       (20)     2606 2023-05-06 07:32:11.000000 django-vectordb-0.1.2/vectordb/tests/test_settings.py
+-rw-r--r--   0 pride      (501) staff       (20)      627 2023-05-04 20:42:47.000000 django-vectordb-0.1.2/vectordb/tests/test_singleton_meta.py
+-rw-r--r--   0 pride      (501) staff       (20)     3547 2023-05-04 19:22:55.000000 django-vectordb-0.1.2/vectordb/tests/test_vectordb.py
+-rw-r--r--   0 pride      (501) staff       (20)       60 2023-05-03 14:10:09.000000 django-vectordb-0.1.2/vectordb/tests.py
+-rw-r--r--   0 pride      (501) staff       (20)      280 2023-05-04 20:40:02.000000 django-vectordb-0.1.2/vectordb/urls.py
+-rw-r--r--   0 pride      (501) staff       (20)     3549 2023-05-06 07:28:17.000000 django-vectordb-0.1.2/vectordb/utils.py
+-rw-r--r--   0 pride      (501) staff       (20)     1744 2023-05-04 18:22:43.000000 django-vectordb-0.1.2/vectordb/validators.py
+-rw-r--r--   0 pride      (501) staff       (20)     1232 2023-05-05 06:34:07.000000 django-vectordb-0.1.2/vectordb/views.py
```

### Comparing `django-vectordb-0.1.1/LICENSE` & `django-vectordb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/PKG-INFO` & `django-vectordb-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vectordb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
 Home-page: https://github.com/pkavumba/django-vectordb.git
 Author: Pride Kavumba
 Author-email: pkavumba@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,20 @@
 Provides-Extra: tests
 License-File: LICENSE
 
 # Django VectorDB
 
 ---
 
+[![pypi-version]][pypi]
+
+**Adding extremely fast, low-latency, and scalable vector search to django apps.**
+
+Full documentation for the project is available at [https://pkavumba.github.io/django-vectordb/][docs].
+
 Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
@@ -73,45 +79,46 @@
 ---
 
 ## Installation
 
 Install using `pip`, it is recommended that you install the optional packages with:
 
 ```bash
-    pip install "django-vectordb[standard]" # This will install the optional dependencies above.
+# This will install the optional dependencies above.
+pip install "django-vectordb[standard]"
 ```
 
 If you dont want to install the optional packages you can run:
 
 ```bash
-    pip install django-vectordb
+pip install django-vectordb
 ```
 
 Add `'django-vectordb'` to your `INSTALLED_APPS` setting.
 
 ```python
-    INSTALLED_APPS = [
-        ...
-        'vectordb',
-    ]
+INSTALLED_APPS = [
+    ...
+    'vectordb',
+]
 ```
 
 Run the migrations to create the `vectordb` table
 
 ```bash
 $ ./manage.py migrate
 ```
 
 If you're intending to use the API, you'll probably also want to add vectordb.urls. Add the following to your root `urls.py` file.
 
 ```python
-    urlpatterns = [
-        ...
-        path('api/', include('vectordb.urls'))
-    ]
+urlpatterns = [
+    ...
+    path('api/', include('vectordb.urls'))
+]
 ```
 
 Note: that the URL path can be whatever you want.
 
 This will expose endpoints for all CRUD actions (`/api/vectordb/`) and searching (`/api/vectordb/search/`).
 
 ---
@@ -196,15 +203,15 @@
 #### Manually adding items to the vector database
 
 VectorDB provides two utility methods for adding items to the database: `vectordb.add_instance` or `vectordb.add_text`. Note that for adding the instance, you need to provide the `get_vectordb_text` and an optional `get_vectordb_metadata` methods.
 
 ##### 1. Adding Model Instances
 
 ```python
-post1 = models.create(title="post1", description="post1 description", user=user1) # provide valid user
+post1 = Post.objects.create(title="post1", description="post1 description", user=user1) # provide valid user
 
 # add to vector database
 vectordb.add_instance(post1)
 ```
 
 ##### 2. Adding Text to the Model
 
@@ -295,25 +302,25 @@
 ---
 
 ## Settings
 
 You can provide your settings in the `settings.py` file of your project. The following settings are available:
 
 ```python
-    # settings.py
-    DJANGO_VECTOR_DB = {
-        "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
-        "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
-        # Can be "cosine" or "l2"
-        "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
-        "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
-        "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
-        "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
-        "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
-    }
+# settings.py
+DJANGO_VECTOR_DB = {
+    "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
+    "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+    # Can be "cosine" or "l2"
+    "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
+    "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+    "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
+    "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
+    "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
+}
 ```
 
 ## Quickstart
 
 Can't wait to get started? The [quickstart guide][quickstart] is the fastest way to get up and running, and building APIs with REST framework.
 
 ---
@@ -350,7 +357,10 @@
 [django]: https://www.djangoproject.com
 [numpy]: https://numpy.org
 [quickstart]: tutorial/quickstart.md
 [sentence-transformers]: https://www.sbert.net
 [hnswlib]: https://github.com/nmslib/hnswlib
 [drf]: https://www.django-rest-framework.org
 [django-filters]: https://pypi.org/project/django-filter/
+[docs]: https://pkavumba.github.io/django-vectordb/
+[pypi]: https://pypi.org/project/django-vectordb/
+[pypi-version]: https://img.shields.io/pypi/v/django-vectordb.svg
```

### Comparing `django-vectordb-0.1.1/README.md` & `django-vectordb-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Django VectorDB
 
 ---
 
+[![pypi-version]][pypi]
+
+**Adding extremely fast, low-latency, and scalable vector search to django apps.**
+
+Full documentation for the project is available at [https://pkavumba.github.io/django-vectordb/][docs].
+
 Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
@@ -38,45 +44,46 @@
 ---
 
 ## Installation
 
 Install using `pip`, it is recommended that you install the optional packages with:
 
 ```bash
-    pip install "django-vectordb[standard]" # This will install the optional dependencies above.
+# This will install the optional dependencies above.
+pip install "django-vectordb[standard]"
 ```
 
 If you dont want to install the optional packages you can run:
 
 ```bash
-    pip install django-vectordb
+pip install django-vectordb
 ```
 
 Add `'django-vectordb'` to your `INSTALLED_APPS` setting.
 
 ```python
-    INSTALLED_APPS = [
-        ...
-        'vectordb',
-    ]
+INSTALLED_APPS = [
+    ...
+    'vectordb',
+]
 ```
 
 Run the migrations to create the `vectordb` table
 
 ```bash
 $ ./manage.py migrate
 ```
 
 If you're intending to use the API, you'll probably also want to add vectordb.urls. Add the following to your root `urls.py` file.
 
 ```python
-    urlpatterns = [
-        ...
-        path('api/', include('vectordb.urls'))
-    ]
+urlpatterns = [
+    ...
+    path('api/', include('vectordb.urls'))
+]
 ```
 
 Note: that the URL path can be whatever you want.
 
 This will expose endpoints for all CRUD actions (`/api/vectordb/`) and searching (`/api/vectordb/search/`).
 
 ---
@@ -161,15 +168,15 @@
 #### Manually adding items to the vector database
 
 VectorDB provides two utility methods for adding items to the database: `vectordb.add_instance` or `vectordb.add_text`. Note that for adding the instance, you need to provide the `get_vectordb_text` and an optional `get_vectordb_metadata` methods.
 
 ##### 1. Adding Model Instances
 
 ```python
-post1 = models.create(title="post1", description="post1 description", user=user1) # provide valid user
+post1 = Post.objects.create(title="post1", description="post1 description", user=user1) # provide valid user
 
 # add to vector database
 vectordb.add_instance(post1)
 ```
 
 ##### 2. Adding Text to the Model
 
@@ -260,25 +267,25 @@
 ---
 
 ## Settings
 
 You can provide your settings in the `settings.py` file of your project. The following settings are available:
 
 ```python
-    # settings.py
-    DJANGO_VECTOR_DB = {
-        "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
-        "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
-        # Can be "cosine" or "l2"
-        "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
-        "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
-        "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
-        "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
-        "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
-    }
+# settings.py
+DJANGO_VECTOR_DB = {
+    "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
+    "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+    # Can be "cosine" or "l2"
+    "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
+    "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+    "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
+    "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
+    "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
+}
 ```
 
 ## Quickstart
 
 Can't wait to get started? The [quickstart guide][quickstart] is the fastest way to get up and running, and building APIs with REST framework.
 
 ---
@@ -315,7 +322,10 @@
 [django]: https://www.djangoproject.com
 [numpy]: https://numpy.org
 [quickstart]: tutorial/quickstart.md
 [sentence-transformers]: https://www.sbert.net
 [hnswlib]: https://github.com/nmslib/hnswlib
 [drf]: https://www.django-rest-framework.org
 [django-filters]: https://pypi.org/project/django-filter/
+[docs]: https://pkavumba.github.io/django-vectordb/
+[pypi]: https://pypi.org/project/django-vectordb/
+[pypi-version]: https://img.shields.io/pypi/v/django-vectordb.svg
```

### Comparing `django-vectordb-0.1.1/django_vectordb.egg-info/PKG-INFO` & `django-vectordb-0.1.2/django_vectordb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vectordb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
 Home-page: https://github.com/pkavumba/django-vectordb.git
 Author: Pride Kavumba
 Author-email: pkavumba@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,20 @@
 Provides-Extra: tests
 License-File: LICENSE
 
 # Django VectorDB
 
 ---
 
+[![pypi-version]][pypi]
+
+**Adding extremely fast, low-latency, and scalable vector search to django apps.**
+
+Full documentation for the project is available at [https://pkavumba.github.io/django-vectordb/][docs].
+
 Django Vector DB is a powerful and flexible toolkit for adding vector search capabilities to your Django applications. It is built on top of lightening fast nearest neighbor search library: hnswlib.
 
 Some reasons you might want to use Django Vector DB:
 
 - Low latency, because you don't need to call an external API.
 - Scalable to a billion vectors with millisecond search results.
 - Fast and accurate search.
@@ -73,45 +79,46 @@
 ---
 
 ## Installation
 
 Install using `pip`, it is recommended that you install the optional packages with:
 
 ```bash
-    pip install "django-vectordb[standard]" # This will install the optional dependencies above.
+# This will install the optional dependencies above.
+pip install "django-vectordb[standard]"
 ```
 
 If you dont want to install the optional packages you can run:
 
 ```bash
-    pip install django-vectordb
+pip install django-vectordb
 ```
 
 Add `'django-vectordb'` to your `INSTALLED_APPS` setting.
 
 ```python
-    INSTALLED_APPS = [
-        ...
-        'vectordb',
-    ]
+INSTALLED_APPS = [
+    ...
+    'vectordb',
+]
 ```
 
 Run the migrations to create the `vectordb` table
 
 ```bash
 $ ./manage.py migrate
 ```
 
 If you're intending to use the API, you'll probably also want to add vectordb.urls. Add the following to your root `urls.py` file.
 
 ```python
-    urlpatterns = [
-        ...
-        path('api/', include('vectordb.urls'))
-    ]
+urlpatterns = [
+    ...
+    path('api/', include('vectordb.urls'))
+]
 ```
 
 Note: that the URL path can be whatever you want.
 
 This will expose endpoints for all CRUD actions (`/api/vectordb/`) and searching (`/api/vectordb/search/`).
 
 ---
@@ -196,15 +203,15 @@
 #### Manually adding items to the vector database
 
 VectorDB provides two utility methods for adding items to the database: `vectordb.add_instance` or `vectordb.add_text`. Note that for adding the instance, you need to provide the `get_vectordb_text` and an optional `get_vectordb_metadata` methods.
 
 ##### 1. Adding Model Instances
 
 ```python
-post1 = models.create(title="post1", description="post1 description", user=user1) # provide valid user
+post1 = Post.objects.create(title="post1", description="post1 description", user=user1) # provide valid user
 
 # add to vector database
 vectordb.add_instance(post1)
 ```
 
 ##### 2. Adding Text to the Model
 
@@ -295,25 +302,25 @@
 ---
 
 ## Settings
 
 You can provide your settings in the `settings.py` file of your project. The following settings are available:
 
 ```python
-    # settings.py
-    DJANGO_VECTOR_DB = {
-        "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
-        "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
-        # Can be "cosine" or "l2"
-        "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
-        "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
-        "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
-        "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
-        "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
-    }
+# settings.py
+DJANGO_VECTOR_DB = {
+    "DEFAULT_EMBEDDING_CLASS": ..., # Default: "vectordb.embedding_functions.SentenceTransformerEncoder",
+    "DEFAULT_EMBEDDING_MODEL": ..., # Default: "all-MiniLM-L6-v2",
+    # Can be "cosine" or "l2"
+    "DEFAULT_EMBEDDING_SPACE": ..., # Default "l2"
+    "DEFAULT_EMBEDDING_DIMENSION": ..., # Default is 384 for "all-MiniLM-L6-v2"
+    "DEFAULT_MAX_N_RESULTS": 10, # Number of results to return from search maximum is default is 10
+    "DEFAULT_MIN_SCORE": 0.0, # Minimum score to return from search default is 0.0
+    "DEFAULT_MAX_BRUTEFORCE_N": 10_000, # Maximum number of items to search using brute force default is 10_000. If the number of items is greater than this number, the search will be done using the HNSW index.
+}
 ```
 
 ## Quickstart
 
 Can't wait to get started? The [quickstart guide][quickstart] is the fastest way to get up and running, and building APIs with REST framework.
 
 ---
@@ -350,7 +357,10 @@
 [django]: https://www.djangoproject.com
 [numpy]: https://numpy.org
 [quickstart]: tutorial/quickstart.md
 [sentence-transformers]: https://www.sbert.net
 [hnswlib]: https://github.com/nmslib/hnswlib
 [drf]: https://www.django-rest-framework.org
 [django-filters]: https://pypi.org/project/django-filter/
+[docs]: https://pkavumba.github.io/django-vectordb/
+[pypi]: https://pypi.org/project/django-vectordb/
+[pypi-version]: https://img.shields.io/pypi/v/django-vectordb.svg
```

### Comparing `django-vectordb-0.1.1/django_vectordb.egg-info/SOURCES.txt` & `django-vectordb-0.1.2/django_vectordb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 vectordb/checks.py
 vectordb/embedding_functions.py
 vectordb/manager.py
 vectordb/models.py
 vectordb/queryset.py
 vectordb/serializers.py
 vectordb/settings.py
+vectordb/shortcuts.py
 vectordb/signals.py
 vectordb/sync_signals.py
 vectordb/tasks.py
 vectordb/tests.py
 vectordb/urls.py
 vectordb/utils.py
 vectordb/validators.py
```

### Comparing `django-vectordb-0.1.1/setup.cfg` & `django-vectordb-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-vectordb
-version = 0.1.1
+version = 0.1.2
 description = Add extremely fast vector search to django with support for filtering and auto-sync through signals. Scalable to a billion vectors.
 long_description = file: README.md
 url = https://github.com/pkavumba/django-vectordb.git
 author = Pride Kavumba
 author_email = pkavumba@gmail.com
 license = Apache License 2.0
 classifiers =
```

### Comparing `django-vectordb-0.1.1/vectordb/admin.py` & `django-vectordb-0.1.2/vectordb/admin.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/ann/abcz.py` & `django-vectordb-0.1.2/vectordb/ann/abcz.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/ann/indexes.py` & `django-vectordb-0.1.2/vectordb/ann/indexes.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/ann/singleton.py` & `django-vectordb-0.1.2/vectordb/ann/singleton.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/checks.py` & `django-vectordb-0.1.2/vectordb/checks.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/embedding_functions.py` & `django-vectordb-0.1.2/vectordb/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/management/commands/vectordb_reset.py` & `django-vectordb-0.1.2/vectordb/management/commands/vectordb_reset.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/management/commands/vectordb_sync.py` & `django-vectordb-0.1.2/vectordb/management/commands/vectordb_sync.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/manager.py` & `django-vectordb-0.1.2/vectordb/manager.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/migrations/0001_initial.py` & `django-vectordb-0.1.2/vectordb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py` & `django-vectordb-0.1.2/vectordb/migrations/0002_vector_created_at_vector_updated_at_and_more.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/models.py` & `django-vectordb-0.1.2/vectordb/models.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/queryset.py` & `django-vectordb-0.1.2/vectordb/queryset.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/settings.py` & `django-vectordb-0.1.2/vectordb/settings.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/signals.py` & `django-vectordb-0.1.2/vectordb/signals.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/sync_signals.py` & `django-vectordb-0.1.2/vectordb/sync_signals.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/tasks.py` & `django-vectordb-0.1.2/vectordb/tasks.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/tests/settings.py` & `django-vectordb-0.1.2/vectordb/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/tests/test_api_endpoint.py` & `django-vectordb-0.1.2/vectordb/tests/test_api_endpoint.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/tests/test_db_indexes.py` & `django-vectordb-0.1.2/vectordb/tests/test_db_indexes.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/tests/test_embedding_functions.py` & `django-vectordb-0.1.2/vectordb/tests/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/tests/test_settings.py` & `django-vectordb-0.1.2/vectordb/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/tests/test_singleton_meta.py` & `django-vectordb-0.1.2/vectordb/tests/test_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/tests/test_vectordb.py` & `django-vectordb-0.1.2/vectordb/tests/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/utils.py` & `django-vectordb-0.1.2/vectordb/utils.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/validators.py` & `django-vectordb-0.1.2/vectordb/validators.py`

 * *Files identical despite different names*

### Comparing `django-vectordb-0.1.1/vectordb/views.py` & `django-vectordb-0.1.2/vectordb/views.py`

 * *Files identical despite different names*

