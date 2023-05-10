# Comparing `tmp/django_trackings-0.6.1a0.tar.gz` & `tmp/django_trackings-0.6.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_trackings-0.6.1a0.tar", last modified: Tue Apr 18 17:37:59 2023, max compression
+gzip compressed data, was "django_trackings-0.6.2a0.tar", last modified: Wed May 10 17:38:19 2023, max compression
```

## Comparing `django_trackings-0.6.1a0.tar` & `django_trackings-0.6.2a0.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-18 17:37:59.351720 django_trackings-0.6.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.343720 django_trackings-0.6.1a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-04-18 17:37:58.000000 django_trackings-0.6.1a0/src/dj_tracker/cache_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/cache_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/cache_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    15372 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/db_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/field_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-04-18 17:37:50.000000 django_trackings-0.6.1a0/src/dj_tracker/hash_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/hash_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/pythoncapi_compat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.343720 django_trackings-0.6.1a0/src/dj_tracker/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.343720 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/css/
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/js/query_group.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.343720 django_trackings-0.6.1a0/src/dj_tracker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/listing.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/query.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/queries.html
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query.html
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/requests.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/templatetags/dj_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/dj_tracker/test/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-04-18 17:37:58.000000 django_trackings-0.6.1a0/src/dj_tracker/traceback.c
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/traceback.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-04-18 17:37:46.000000 django_trackings-0.6.1a0/src/dj_tracker/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:37:59.347720 django_trackings-0.6.1a0/src/django_trackings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-18 17:37:59.000000 django_trackings-0.6.1a0/src/django_trackings.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.529928 django_trackings-0.6.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-10 17:38:19.529928 django_trackings-0.6.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-10 17:38:19.533928 django_trackings-0.6.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.517928 django_trackings-0.6.2a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.525928 django_trackings-0.6.2a0/src/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-05-10 17:38:18.000000 django_trackings-0.6.2a0/src/dj_tracker/cache_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/cache_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/cache_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/db_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/field_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-05-10 17:38:08.000000 django_trackings-0.6.2a0/src/dj_tracker/hash_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/hash_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.525928 django_trackings-0.6.2a0/src/dj_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/pythoncapi_compat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.517928 django_trackings-0.6.2a0/src/dj_tracker/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.517928 django_trackings-0.6.2a0/src/dj_tracker/static/dj_tracker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.529928 django_trackings-0.6.2a0/src/dj_tracker/static/dj_tracker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-05-10 17:38:03.000000 django_trackings-0.6.2a0/src/dj_tracker/static/dj_tracker/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.529928 django_trackings-0.6.2a0/src/dj_tracker/static/dj_tracker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/static/dj_tracker/js/query_group.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.517928 django_trackings-0.6.2a0/src/dj_tracker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.529928 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.529928 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/includes/listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/includes/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/queries.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/query_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/query_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/requests.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.529928 django_trackings-0.6.2a0/src/dj_tracker/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/templatetags/dj_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-05-10 17:38:18.000000 django_trackings-0.6.2a0/src/dj_tracker/traceback.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/traceback.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-05-10 17:38:02.000000 django_trackings-0.6.2a0/src/dj_tracker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:19.529928 django_trackings-0.6.2a0/src/django_trackings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-10 17:38:19.000000 django_trackings-0.6.2a0/src/django_trackings.egg-info/SOURCES.txt
```

### Comparing `django_trackings-0.6.1a0/LICENSE` & `django_trackings-0.6.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/PKG-INFO` & `django_trackings-0.6.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_trackings
-Version: 0.6.1a0
+Version: 0.6.2a0
 Summary: A Django app that tracks your queries to help optimize them.
 Home-page: https://github.com/tijani-dia/dj-tracker/
 Author: Tidiane Dia
 Author-email: atdia97@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://tijani-dia.github.io/dj-tracker/
 Project-URL: Source, https://github.com/tijani-dia/dj-tracker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django_trackings Version: 0.6.1a0 Summary: A Django
+Metadata-Version: 2.1 Name: django_trackings Version: 0.6.2a0 Summary: A Django
 app that tracks your queries to help optimize them. Home-page: https://
 github.com/tijani-dia/dj-tracker/ Author: Tidiane Dia Author-email:
 atdia97@gmail.com License: BSD-3-Clause Project-URL: Documentation, https://
 tijani-dia.github.io/dj-tracker/ Project-URL: Source, https://github.com/
 tijani-dia/dj-tracker/ Project-URL: Issue tracker, https://github.com/tijani-
 dia/dj-tracker/issues/ Classifier: Development Status :: 3 - Alpha Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
```

### Comparing `django_trackings-0.6.1a0/README.md` & `django_trackings-0.6.2a0/README.md`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/setup.cfg` & `django_trackings-0.6.2a0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_trackings
-version = 0.6.1a0
+version = 0.6.2a0
 description = A Django app that tracks your queries to help optimize them.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tijani-dia/dj-tracker/
 author = Tidiane Dia
 author_email = atdia97@gmail.com
 license = BSD-3-Clause
```

### Comparing `django_trackings-0.6.1a0/setup.py` & `django_trackings-0.6.2a0/setup.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/cache_utils.c` & `django_trackings-0.6.2a0/src/dj_tracker/cache_utils.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/cache_utils.pyx` & `django_trackings-0.6.2a0/src/dj_tracker/cache_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/collector.py` & `django_trackings-0.6.2a0/src/dj_tracker/collector.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/constants.py` & `django_trackings-0.6.2a0/src/dj_tracker/constants.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/datastructures.py` & `django_trackings-0.6.2a0/src/dj_tracker/datastructures.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,7 +499,13 @@
         return len(trackers)
 
     def __hash__(self):
         return id(self)
 
     def __repr__(self):
         return f"<QueryTracker {self['sql']}>"
+
+    def __getstate__(self):
+        return dict(self.items())
+
+    def __setstate__(self, state):
+        self.update(state)
```

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/db_router.py` & `django_trackings-0.6.2a0/src/dj_tracker/db_router.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/field_descriptors.py` & `django_trackings-0.6.2a0/src/dj_tracker/field_descriptors.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/hash_utils.c` & `django_trackings-0.6.2a0/src/dj_tracker/hash_utils.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/hash_utils.pyx` & `django_trackings-0.6.2a0/src/dj_tracker/hash_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/logging.py` & `django_trackings-0.6.2a0/src/dj_tracker/logging.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/migrations/0001_initial.py` & `django_trackings-0.6.2a0/src/dj_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/models.py` & `django_trackings-0.6.2a0/src/dj_tracker/models.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/profile.py` & `django_trackings-0.6.2a0/src/dj_tracker/profile.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/promise.py` & `django_trackings-0.6.2a0/src/dj_tracker/promise.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/pythoncapi_compat.h` & `django_trackings-0.6.2a0/src/dj_tracker/pythoncapi_compat.h`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/css/main.css` & `django_trackings-0.6.2a0/src/dj_tracker/static/dj_tracker/css/main.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-/*! tailwindcss v3.3.1 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}a{--tw-text-opacity:1;color:rgb(49 46 129/var(--tw-text-opacity));display:block;font-weight:500;width:100%}li{list-style-type:none}li:hover{--tw-bg-opacity:1;background-color:rgb(241 245 249/var(--tw-bg-opacity))}table{--tw-text-opacity:1;text-align:left;width:100%}table,thead{color:rgb(51 65 85/var(--tw-text-opacity))}thead{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(248 250 252/var(--tw-bg-opacity));font-size:.875rem;line-height:1.25rem;text-transform:uppercase}th[scope=col]{padding:.75rem 1.5rem}th[scope=row]{--tw-text-opacity:1;color:rgb(15 23 42/var(--tw-text-opacity));font-weight:500;padding:1rem 1.5rem;white-space:nowrap}tr{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));border-bottom-width:1px}td{padding-bottom:1rem;padding-top:1rem}section{margin-bottom:2rem;margin-top:2rem}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.rounded-pill{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(226 232 240/var(--tw-bg-opacity));border-radius:9999px;color:rgb(71 85 105/var(--tw-text-opacity));font-size:.875rem;height:-moz-fit-content;height:fit-content;line-height:1.25rem;padding:.25rem .5rem}.text-muted{font-size:.875rem;line-height:1.25rem;opacity:.75}.listing-objects .text-muted{color:initial}.listing-form label{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity));font-weight:500;margin-bottom:.25rem;margin-top:.25rem}.listing-form>div{display:flex;flex-direction:column;margin-bottom:.5rem;margin-top:.5rem}.listing-form select{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity));border-color:rgb(209 213 219/var(--tw-border-opacity));border-radius:.5rem;border-width:1px;color:rgb(17 24 39/var(--tw-text-opacity));display:block;padding:.625rem;width:100%}.listing-form select:focus{--tw-border-opacity:1;--tw-ring-opacity:1;--tw-ring-color:rgb(99 102 241/var(--tw-ring-opacity));border-color:rgb(99 102 241/var(--tw-border-opacity))}[type=submit]{--tw-gradient-from:#4f46e5 var(--tw-gradient-from-position);--tw-gradient-from-position: ;--tw-gradient-to:#4f46e500 var(--tw-gradient-from-position);--tw-gradient-stops:var(--tw-gradient-from),var(--tw-gradient-to);--tw-gradient-via-position: ;--tw-gradient-to:#4338ca00 var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from),#4338ca var(--tw-gradient-via-position),var(--tw-gradient-to);--tw-gradient-to:#3730a3 var(--tw-gradient-to-position);--tw-gradient-to-position: ;--tw-text-opacity:1;background-image:linear-gradient(to right,var(--tw-gradient-stops));border-radius:.5rem;color:rgb(255 255 255/var(--tw-text-opacity));font-size:.875rem;font-weight:500;line-height:1.25rem;margin-bottom:.5rem;margin-right:.5rem;padding:.625rem 1.25rem;text-align:center}.section__title{--tw-text-opacity:1;color:rgb(51 65 85/var(--tw-text-opacity));font-size:1.875rem;font-weight:700;line-height:2.25rem}.section__subtitle{--tw-text-opacity:1;color:rgb(71 85 105/var(--tw-text-opacity));font-size:1.25rem;font-weight:500;line-height:1.75rem;padding-bottom:.5rem;padding-top:.5rem}.section__body{margin-top:.5rem}.static{position:static}.m-2{margin:.5rem}.m-\[12px\]{margin:12px}.m-auto{margin:auto}.mx-10{margin-left:2.5rem;margin-right:2.5rem}.my-1{margin-bottom:.25rem;margin-top:.25rem}.my-2{margin-bottom:.5rem;margin-top:.5rem}.my-3{margin-bottom:.75rem;margin-top:.75rem}.my-4{margin-bottom:1rem;margin-top:1rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mr-1{margin-right:-.25rem}.mb-12{margin-bottom:3rem}.mb-2{margin-bottom:.5rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-8{margin-bottom:2rem}.ml-1{margin-left:.25rem}.ml-1\.5{margin-left:.375rem}.ml-2{margin-left:.5rem}.mr-1{margin-right:.25rem}.mr-1\.5{margin-right:.375rem}.mr-5{margin-right:1.25rem}.mr-8{margin-right:2rem}.mt-10{margin-top:2.5rem}.mt-16{margin-top:4rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.mt-8{margin-top:2rem}.block{display:block}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.h-5{height:1.25rem}.h-px{height:1px}.min-h-screen{min-height:100vh}.w-1\/2{width:50%}.w-1\/3{width:33.333333%}.w-1\/5{width:20%}.w-11\/12{width:91.666667%}.w-2\/3{width:66.666667%}.w-3\/5{width:60%}.w-4\/5{width:80%}.w-5{width:1.25rem}.w-auto{width:auto}.w-full{width:100%}.w-max{width:-moz-max-content;width:max-content}.max-w-sm{max-width:24rem}.shrink-0{flex-shrink:0}.flex-grow,.grow{flex-grow:1}.cursor-pointer{cursor:pointer}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.items-baseline{align-items:baseline}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.divide-y>:not([hidden])~:not([hidden]){--tw-divide-y-reverse:0;border-bottom-width:calc(1px*var(--tw-divide-y-reverse));border-top-width:calc(1px*(1 - var(--tw-divide-y-reverse)))}.divide-slate-300>:not([hidden])~:not([hidden]){--tw-divide-opacity:1;border-color:rgb(203 213 225/var(--tw-divide-opacity))}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.rounded-lg{border-radius:.5rem}.rounded-t-lg{border-top-left-radius:.5rem;border-top-right-radius:.5rem}.border{border-width:1px}.border-0{border-width:0}.border-b{border-bottom-width:1px}.border-l-8{border-left-width:8px}.border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225/var(--tw-border-opacity))}.border-l-violet-100{--tw-border-opacity:1;border-left-color:rgb(237 233 254/var(--tw-border-opacity))}.bg-gray-200{--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.bg-indigo-700{--tw-bg-opacity:1;background-color:rgb(67 56 202/var(--tw-bg-opacity))}.bg-indigo-900{--tw-bg-opacity:1;background-color:rgb(49 46 129/var(--tw-bg-opacity))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-gradient-to-l{background-image:linear-gradient(to left,var(--tw-gradient-stops))}.bg-gradient-to-r{background-image:linear-gradient(to right,var(--tw-gradient-stops))}.from-indigo-800{--tw-gradient-from:#3730a3 var(--tw-gradient-from-position);--tw-gradient-from-position: ;--tw-gradient-to:#3730a300 var(--tw-gradient-from-position);--tw-gradient-to-position: ;--tw-gradient-stops:var(--tw-gradient-from),var(--tw-gradient-to)}.to-indigo-900{--tw-gradient-to:#312e81 var(--tw-gradient-to-position);--tw-gradient-to-position: }.p-2{padding:.5rem}.p-2\.5{padding:.625rem}.p-3{padding:.75rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-2\.5{padding-bottom:.625rem;padding-top:.625rem}.py-3{padding-bottom:.75rem;padding-top:.75rem}.py-4{padding-top:1rem}.pb-4,.py-4{padding-bottom:1rem}.pl-8{padding-left:2rem}.pr-20{padding-right:5rem}.text-center{text-align:center}.font-mono{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem}.text-lg,.text-xl{line-height:1.75rem}.text-xl{font-size:1.25rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-none{line-height:1}.tracking-tight{letter-spacing:-.025em}.text-gray-900{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity))}.text-indigo-800{--tw-text-opacity:1;color:rgb(55 48 163/var(--tw-text-opacity))}.text-indigo-900{--tw-text-opacity:1;color:rgb(49 46 129/var(--tw-text-opacity))}.text-inherit{color:inherit}.text-slate-50{--tw-text-opacity:1;color:rgb(248 250 252/var(--tw-text-opacity))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105/var(--tw-text-opacity))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59/var(--tw-text-opacity))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.underline{text-decoration-line:underline}.underline-offset-2{text-underline-offset:2px}.opacity-75{opacity:.75}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.first\:pt-0:first-child{padding-top:0}@media (prefers-color-scheme:dark){.dark\:bg-gray-700{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}}
+/*! tailwindcss v3.3.2 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}a{--tw-text-opacity:1;color:rgb(49 46 129/var(--tw-text-opacity));display:block;font-weight:500;width:100%}li{list-style-type:none}li:hover{--tw-bg-opacity:1;background-color:rgb(241 245 249/var(--tw-bg-opacity))}table{--tw-text-opacity:1;text-align:left;width:100%}table,thead{color:rgb(51 65 85/var(--tw-text-opacity))}thead{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(248 250 252/var(--tw-bg-opacity));font-size:.875rem;line-height:1.25rem;text-transform:uppercase}th[scope=col]{padding:.75rem 1.5rem}th[scope=row]{--tw-text-opacity:1;color:rgb(15 23 42/var(--tw-text-opacity));font-weight:500;padding:1rem 1.5rem;white-space:nowrap}tr{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));border-bottom-width:1px}td{padding-bottom:1rem;padding-top:1rem}section{margin-bottom:2rem;margin-top:2rem}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.rounded-pill{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(226 232 240/var(--tw-bg-opacity));border-radius:9999px;color:rgb(71 85 105/var(--tw-text-opacity));font-size:.875rem;height:-moz-fit-content;height:fit-content;line-height:1.25rem;padding:.25rem .5rem}.text-muted{font-size:.875rem;line-height:1.25rem;opacity:.75}.listing-objects .text-muted{color:initial}.listing-form label{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity));font-weight:500;margin-bottom:.25rem;margin-top:.25rem}.listing-form>div{display:flex;flex-direction:column;margin-bottom:.5rem;margin-top:.5rem}.listing-form select{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity));border-color:rgb(209 213 219/var(--tw-border-opacity));border-radius:.5rem;border-width:1px;color:rgb(17 24 39/var(--tw-text-opacity));display:block;padding:.625rem;width:100%}.listing-form select:focus{--tw-border-opacity:1;--tw-ring-opacity:1;--tw-ring-color:rgb(99 102 241/var(--tw-ring-opacity));border-color:rgb(99 102 241/var(--tw-border-opacity))}[type=submit]{--tw-gradient-from:#4f46e5 var(--tw-gradient-from-position);--tw-gradient-to:#4f46e500 var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from),var(--tw-gradient-to);--tw-gradient-to:#4338ca00 var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from),#4338ca var(--tw-gradient-via-position),var(--tw-gradient-to);--tw-gradient-to:#3730a3 var(--tw-gradient-to-position);--tw-text-opacity:1;background-image:linear-gradient(to right,var(--tw-gradient-stops));border-radius:.5rem;color:rgb(255 255 255/var(--tw-text-opacity));font-size:.875rem;font-weight:500;line-height:1.25rem;margin-bottom:.5rem;margin-right:.5rem;padding:.625rem 1.25rem;text-align:center}.section__title{--tw-text-opacity:1;color:rgb(51 65 85/var(--tw-text-opacity));font-size:1.875rem;font-weight:700;line-height:2.25rem}.section__subtitle{--tw-text-opacity:1;color:rgb(71 85 105/var(--tw-text-opacity));font-size:1.25rem;font-weight:500;line-height:1.75rem;padding-bottom:.5rem;padding-top:.5rem}.section__body{margin-top:.5rem}.static{position:static}.m-2{margin:.5rem}.m-\[12px\]{margin:12px}.m-auto{margin:auto}.mx-10{margin-left:2.5rem;margin-right:2.5rem}.my-1{margin-bottom:.25rem;margin-top:.25rem}.my-2{margin-bottom:.5rem;margin-top:.5rem}.my-3{margin-bottom:.75rem;margin-top:.75rem}.my-4{margin-bottom:1rem;margin-top:1rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mr-1{margin-right:-.25rem}.mb-12{margin-bottom:3rem}.mb-2{margin-bottom:.5rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-8{margin-bottom:2rem}.ml-1{margin-left:.25rem}.ml-1\.5{margin-left:.375rem}.ml-2{margin-left:.5rem}.mr-1{margin-right:.25rem}.mr-1\.5{margin-right:.375rem}.mr-5{margin-right:1.25rem}.mr-8{margin-right:2rem}.mt-10{margin-top:2.5rem}.mt-16{margin-top:4rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.mt-8{margin-top:2rem}.block{display:block}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.h-5{height:1.25rem}.h-px{height:1px}.min-h-screen{min-height:100vh}.w-1\/2{width:50%}.w-1\/3{width:33.333333%}.w-1\/5{width:20%}.w-11\/12{width:91.666667%}.w-2\/3{width:66.666667%}.w-3\/5{width:60%}.w-4\/5{width:80%}.w-5{width:1.25rem}.w-auto{width:auto}.w-full{width:100%}.w-max{width:-moz-max-content;width:max-content}.max-w-sm{max-width:24rem}.shrink-0{flex-shrink:0}.flex-grow,.grow{flex-grow:1}.cursor-pointer{cursor:pointer}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.items-baseline{align-items:baseline}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.divide-y>:not([hidden])~:not([hidden]){--tw-divide-y-reverse:0;border-bottom-width:calc(1px*var(--tw-divide-y-reverse));border-top-width:calc(1px*(1 - var(--tw-divide-y-reverse)))}.divide-slate-300>:not([hidden])~:not([hidden]){--tw-divide-opacity:1;border-color:rgb(203 213 225/var(--tw-divide-opacity))}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.rounded-lg{border-radius:.5rem}.rounded-t-lg{border-top-left-radius:.5rem;border-top-right-radius:.5rem}.border{border-width:1px}.border-0{border-width:0}.border-b{border-bottom-width:1px}.border-l-8{border-left-width:8px}.border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225/var(--tw-border-opacity))}.border-l-violet-100{--tw-border-opacity:1;border-left-color:rgb(237 233 254/var(--tw-border-opacity))}.bg-gray-200{--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.bg-indigo-700{--tw-bg-opacity:1;background-color:rgb(67 56 202/var(--tw-bg-opacity))}.bg-indigo-900{--tw-bg-opacity:1;background-color:rgb(49 46 129/var(--tw-bg-opacity))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-gradient-to-l{background-image:linear-gradient(to left,var(--tw-gradient-stops))}.bg-gradient-to-r{background-image:linear-gradient(to right,var(--tw-gradient-stops))}.from-indigo-800{--tw-gradient-from:#3730a3 var(--tw-gradient-from-position);--tw-gradient-to:#3730a300 var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from),var(--tw-gradient-to)}.to-indigo-900{--tw-gradient-to:#312e81 var(--tw-gradient-to-position)}.p-2{padding:.5rem}.p-2\.5{padding:.625rem}.p-3{padding:.75rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-2\.5{padding-bottom:.625rem;padding-top:.625rem}.py-3{padding-bottom:.75rem;padding-top:.75rem}.py-4{padding-top:1rem}.pb-4,.py-4{padding-bottom:1rem}.pl-8{padding-left:2rem}.pr-20{padding-right:5rem}.text-center{text-align:center}.font-mono{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem}.text-lg,.text-xl{line-height:1.75rem}.text-xl{font-size:1.25rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-none{line-height:1}.tracking-tight{letter-spacing:-.025em}.text-gray-900{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity))}.text-indigo-800{--tw-text-opacity:1;color:rgb(55 48 163/var(--tw-text-opacity))}.text-indigo-900{--tw-text-opacity:1;color:rgb(49 46 129/var(--tw-text-opacity))}.text-inherit{color:inherit}.text-slate-50{--tw-text-opacity:1;color:rgb(248 250 252/var(--tw-text-opacity))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105/var(--tw-text-opacity))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59/var(--tw-text-opacity))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.underline{text-decoration-line:underline}.underline-offset-2{text-underline-offset:2px}.opacity-75{opacity:.75}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.first\:pt-0:first-child{padding-top:0}@media (prefers-color-scheme:dark){.dark\:bg-gray-700{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}}
```

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/static/dj_tracker/js/query_group.js` & `django_trackings-0.6.2a0/src/dj_tracker/static/dj_tracker/js/query_group.js`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/base.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/base.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/home.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/home.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/listing.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/includes/listing.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/pagination.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/includes/query.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/includes/query.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/queries.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/queries.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/query.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query_group.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/query_group.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/query_groups.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/query_groups.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templates/dj_tracker/requests.html` & `django_trackings-0.6.2a0/src/dj_tracker/templates/dj_tracker/requests.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/templatetags/dj_tracker.py` & `django_trackings-0.6.2a0/src/dj_tracker/templatetags/dj_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 from django import VERSION as DJANGO_VERSION
 from django import template
-from django.utils.safestring import mark_safe
 
 register = template.Library()
 
 
 @register.filter
 def total_queries(queries):
     return sum(query.num_occurrences for query in queries)
 
 
 @register.tag
 def preserve_query_parameters(parser, token):
+    # https://djangosnippets.org/snippets/2428/
     params = {}
 
     for pair in token.split_contents()[1:]:
         s = pair.split("=", 1)
         params[s[0]] = parser.compile_filter(s[1])
 
     return PreserveQueryParameters(params)
 
 
 class PreserveQueryParameters(template.Node):
-    # https://djangosnippets.org/snippets/2428/
     def __init__(self, params):
         self.params = params
 
     def render(self, context):
         params = context["request"].GET.copy()
         params.update(
             (key, value.resolve(context)) for key, value in self.params.items()
         )
         return "?%s" % params.urlencode()
 
 
 if DJANGO_VERSION[0] < 4 or (DJANGO_VERSION[0] == 4 and DJANGO_VERSION[1] < 1):
+    from django.utils.safestring import mark_safe
 
     @register.filter
     def form_as_div(form):
         return mark_safe(form.as_p().replace("<p>", "<div>").replace("</p>", "</div>"))
 
 else:
```

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/test/__init__.py` & `django_trackings-0.6.2a0/src/dj_tracker/test.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/traceback.c` & `django_trackings-0.6.2a0/src/dj_tracker/traceback.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/traceback.pyx` & `django_trackings-0.6.2a0/src/dj_tracker/traceback.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/tracker.py` & `django_trackings-0.6.2a0/src/dj_tracker/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self.model = model
         # model.from_db is a classmethod, so we store the actual function.
         # This will keep inheritance rules.
         self.__func__ = model.from_db.__func__
 
     def __call__(self, db, field_names, values):
         instance = self.__func__(self.model, db, field_names, values)
+        # TODO: Consider adding the `_tracker` attribute to the instance's `_state`.
         instance._tracker = new_model_instance_tracker(field_names)
         return instance
 
 
 class ResultCacheDescriptor:
     def __get__(self, queryset, cls):
         if queryset is None:
```

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/urls.py` & `django_trackings-0.6.2a0/src/dj_tracker/urls.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/dj_tracker/views.py` & `django_trackings-0.6.2a0/src/dj_tracker/views.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.1a0/src/django_trackings.egg-info/SOURCES.txt` & `django_trackings-0.6.2a0/src/django_trackings.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 src/dj_tracker/context.py
 src/dj_tracker/datastructures.py
 src/dj_tracker/db_router.py
 src/dj_tracker/field_descriptors.py
 src/dj_tracker/hash_utils.c
 src/dj_tracker/hash_utils.pyx
 src/dj_tracker/logging.py
+src/dj_tracker/middleware.py
 src/dj_tracker/models.py
 src/dj_tracker/profile.py
 src/dj_tracker/promise.py
 src/dj_tracker/pythoncapi_compat.h
+src/dj_tracker/test.py
 src/dj_tracker/traceback.c
 src/dj_tracker/traceback.pyx
 src/dj_tracker/tracker.py
 src/dj_tracker/urls.py
 src/dj_tracker/views.py
-src/dj_tracker/middleware/__init__.py
 src/dj_tracker/migrations/0001_initial.py
 src/dj_tracker/migrations/__init__.py
 src/dj_tracker/static/dj_tracker/css/main.css
 src/dj_tracker/static/dj_tracker/js/query_group.js
 src/dj_tracker/templates/dj_tracker/base.html
 src/dj_tracker/templates/dj_tracker/home.html
 src/dj_tracker/templates/dj_tracker/list.html
@@ -39,9 +40,8 @@
 src/dj_tracker/templates/dj_tracker/query_group.html
 src/dj_tracker/templates/dj_tracker/query_groups.html
 src/dj_tracker/templates/dj_tracker/requests.html
 src/dj_tracker/templates/dj_tracker/includes/listing.html
 src/dj_tracker/templates/dj_tracker/includes/pagination.html
 src/dj_tracker/templates/dj_tracker/includes/query.html
 src/dj_tracker/templatetags/__init__.py
-src/dj_tracker/templatetags/dj_tracker.py
-src/dj_tracker/test/__init__.py
+src/dj_tracker/templatetags/dj_tracker.py
```

