# Comparing `tmp/django_hmac_authentication-1.1.0.tar.gz` & `tmp/django_hmac_authentication-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-1.1.0.tar", last modified: Tue May  9 23:20:26 2023, max compression
+gzip compressed data, was "django_hmac_authentication-1.1.1.tar", last modified: Wed May 10 01:30:26 2023, max compression
```

## Comparing `django_hmac_authentication-1.1.0.tar` & `django_hmac_authentication-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.223873 django_hmac_authentication-1.1.0/
--rw-r--r--   0 topcat    (1000) topcat    (1000)    11358 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.0/LICENSE
--rw-r--r--   0 topcat    (1000) topcat    (1000)     4440 2023-05-09 23:20:26.223873 django_hmac_authentication-1.1.0/PKG-INFO
--rw-r--r--   0 topcat    (1000) topcat    (1000)     3902 2023-05-09 23:14:39.000000 django_hmac_authentication-1.1.0/README.md
--rw-r--r--   0 topcat    (1000) topcat    (1000)      722 2023-05-09 23:19:28.000000 django_hmac_authentication-1.1.0/pyproject.toml
--rw-r--r--   0 topcat    (1000) topcat    (1000)       38 2023-05-09 23:20:26.223873 django_hmac_authentication-1.1.0/setup.cfg
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.215873 django_hmac_authentication-1.1.0/src/
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.215873 django_hmac_authentication-1.1.0/src/django_hmac_authentication/
--rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-05-09 23:19:28.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      752 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/admin.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      638 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/aes.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2858 2023-05-09 14:13:26.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/authentication.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2817 2023-05-09 23:14:39.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/client_utils.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.219873 django_hmac_authentication-1.1.0/src/django_hmac_authentication/management/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.219873 django_hmac_authentication-1.1.0/src/django_hmac_authentication/management/commands/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/management/commands/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1282 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.219873 django_hmac_authentication-1.1.0/src/django_hmac_authentication/migrations/
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1776 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/migrations/0001_initial.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/migrations/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      969 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/models.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      192 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/padding.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      298 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/serializers.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1519 2023-05-09 22:12:50.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/server_utils.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      813 2023-05-08 07:07:48.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.219873 django_hmac_authentication-1.1.0/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 topcat    (1000) topcat    (1000)     4440 2023-05-09 23:20:26.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2037 2023-05-09 23:20:26.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)        1 2023-05-09 23:20:26.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-09 23:20:26.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 topcat    (1000) topcat    (1000)       56 2023-05-09 23:20:26.000000 django_hmac_authentication-1.1.0/src/django_hmac_authentication.egg-info/top_level.txt
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.219873 django_hmac_authentication-1.1.0/src/example_django_project/
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.219873 django_hmac_authentication-1.1.0/src/example_django_project/accounts/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/example_django_project/accounts/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/example_django_project/accounts/admin.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      148 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/example_django_project/accounts/apps.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.219873 django_hmac_authentication-1.1.0/src/example_django_project/accounts/migrations/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/example_django_project/accounts/migrations/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       57 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/example_django_project/accounts/models.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)       60 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/example_django_project/accounts/tests.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      266 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/example_django_project/accounts/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      576 2023-05-09 23:14:39.000000 django_hmac_authentication-1.1.0/src/example_django_project/accounts/views.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.223873 django_hmac_authentication-1.1.0/src/example_django_project/example_django_project/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.0/src/example_django_project/example_django_project/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.0/src/example_django_project/example_django_project/asgi.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     3718 2023-05-09 13:02:58.000000 django_hmac_authentication-1.1.0/src/example_django_project/example_django_project/settings.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1025 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.0/src/example_django_project/example_django_project/urls.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.0/src/example_django_project/example_django_project/wsgi.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1834 2023-05-09 22:48:29.000000 django_hmac_authentication-1.1.0/src/example_django_project/example_python_client.py
--rwxr-xr-x   0 topcat    (1000) topcat    (1000)      678 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.0/src/example_django_project/manage.py
-drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-09 23:20:26.223873 django_hmac_authentication-1.1.0/src/tests/
--rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 05:37:24.000000 django_hmac_authentication-1.1.0/src/tests/__init__.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1427 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.0/src/tests/factories.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     7010 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.0/src/tests/test_authentication_api_key_secret.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1510 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)      563 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.0/src/tests/test_padding.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     2747 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.0/src/tests/test_utils.py
--rw-r--r--   0 topcat    (1000) topcat    (1000)     1836 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.0/src/tests/test_view_create_api_key_secret.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)    11358 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/LICENSE
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     4717 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/PKG-INFO
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     4179 2023-05-09 23:43:54.000000 django_hmac_authentication-1.1.1/README.md
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      722 2023-05-10 01:29:36.000000 django_hmac_authentication-1.1.1/pyproject.toml
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       38 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/setup.cfg
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.863941 django_hmac_authentication-1.1.1/src/
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       54 2023-05-10 01:29:36.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      752 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/admin.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      638 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/aes.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     3213 2023-05-10 01:25:49.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/authentication.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     2817 2023-05-09 23:14:39.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/client_utils.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/commands/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 13:51:47.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/commands/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1282 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication/migrations/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1776 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/migrations/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      969 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/models.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      192 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/padding.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      298 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/serializers.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1519 2023-05-09 22:12:50.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/server_utils.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      813 2023-05-08 07:07:48.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     4717 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     2089 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        1 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       56 2023-05-10 01:30:26.000000 django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.867941 django_hmac_authentication-1.1.1/src/example_django_project/
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/src/example_django_project/accounts/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       63 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/admin.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      148 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/apps.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/src/example_django_project/accounts/migrations/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/migrations/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       57 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/models.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)       60 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/tests.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      266 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/urls.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      576 2023-05-09 23:14:39.000000 django_hmac_authentication-1.1.1/src/example_django_project/accounts/views.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/asgi.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     3718 2023-05-09 13:02:58.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/settings.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1025 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/urls.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      421 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/wsgi.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1834 2023-05-10 01:27:46.000000 django_hmac_authentication-1.1.1/src/example_django_project/example_python_client.py
+-rwxr-xr-x   0 topcat    (1000) topcat    (1000)      678 2023-05-06 22:55:18.000000 django_hmac_authentication-1.1.1/src/example_django_project/manage.py
+drwxr-xr-x   0 topcat    (1000) topcat    (1000)        0 2023-05-10 01:30:26.871941 django_hmac_authentication-1.1.1/src/tests/
+-rw-r--r--   0 topcat    (1000) topcat    (1000)        0 2023-05-07 05:37:24.000000 django_hmac_authentication-1.1.1/src/tests/__init__.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1427 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/tests/factories.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     7007 2023-05-10 01:25:49.000000 django_hmac_authentication-1.1.1/src/tests/test_authentication_api_key_secret.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1502 2023-05-10 01:25:49.000000 django_hmac_authentication-1.1.1/src/tests/test_hmac_authorization_header_parsing.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1510 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/tests/test_mgmt_cmd_create_hmac_for_user.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)      563 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/tests/test_padding.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     2747 2023-05-09 04:08:40.000000 django_hmac_authentication-1.1.1/src/tests/test_utils.py
+-rw-r--r--   0 topcat    (1000) topcat    (1000)     1836 2023-05-08 02:03:56.000000 django_hmac_authentication-1.1.1/src/tests/test_view_create_api_key_secret.py
```

### Comparing `django_hmac_authentication-1.1.0/LICENSE` & `django_hmac_authentication-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/PKG-INFO` & `django_hmac_authentication-1.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,16 @@
-Metadata-Version: 2.1
-Name: django_hmac_authentication
-Version: 1.1.0
-Summary: Django HMAC authentication using shared secret
-Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
-Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # django_hmac_authentication
 Django hmac authentication with shared secret
 
 * Django model with HMAC shared encrypted secret
 * Authentication class `HMACAuthentication` 
 * Reject requests earlier than configured timeout
 * Supports `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * HMAC secret can be created with management command or obtained with a configured url
+* Supports Javascript and Python clients
 
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
@@ -105,28 +93,35 @@
 A prerequest script for generating the signature is provided (same as included in postman collection).
 
 ## 4.2 Python client
 See `example_django_project/example_python_client.py`
 
 # 5. Signature
 
+# 5.1 How is it calculated
+
 Signature is calculated on hash( request body json ) + utc 8601
 
-Fields
+Steps:
+
+1. request body (data) -> json string in utf-8 -> hash -> **base64 of body hash**
+2. **utc 8601 string**
+3. string to sign = **base64 of body hash** + ";" + **utc 8601 string**
+4. signature = hash (string to sign) -> base64
 
-* Hash of request body. Hash function is one of supported methods in Authorization header
+* Hash function is one of supported methods in Authorization header
 * UTC time now in ISO 8601 format. Example `2023-05-07T14:15:37.862560+00:00`
 
 # 6. Authorization header
 * method: One of `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * api_key: Key used to identify the hmac secret used to generate signature
 * signature: base64 signature
 * request_utc: time in ISO 8601 set in signed string
 
-`Syntax`: method api_key;signature;request_utc
+`Syntax`: METHOD api_key;signature;request_utc_8601
 
 Example
 ```python
 'HMAC-SHA512 aa733037-e4c0-4f75-a864-df6c1966481b;6k3XaUREI6dDw6thyQWASJjzjsx1M7GOZAglguv0OElpRue1+gb7CK2n3JpzJGz9VcREw2y3rIW5zoZYEUY+0w==;2023-05-07T14:15:37.862560+00:00'
 ```
 # 7. License
 Apache2 License
```

### Comparing `django_hmac_authentication-1.1.0/pyproject.toml` & `django_hmac_authentication-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_hmac_authentication"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/admin.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/admin.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/aes.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/aes.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 
 class HMACAuthentication(authentication.BaseAuthentication):
     authentication_methods = {'HMAC-SHA512', 'HMAC-SHA384', 'HMAC-SHA256'}
 
     def parse_authorization_header(self, content):
         if not content:
-            return None, None, None
+            return None, None, None, None
         try:
             auth_method, rest = content.split()
             if not auth_method or not rest:
-                return None, None
+                return None, None, None, None
 
             api_key, signature, dt = rest.split(';')
             if not api_key or not signature or not dt:
-                return None, None
+                return None, None, None, None
 
             return auth_method, api_key, signature, dt
         except (AttributeError, ValueError):
-            return None, None
+            return None, None, None, None
 
     def compute_request_signature(self, request, auth_method, date_in, hmac_key):
         enc_secret = base64.b64decode(hmac_key.secret.encode('utf-8'))
         enc_salt = base64.b64decode(hmac_key.salt.encode('utf-8'))
         secret = aes_decrypt_hmac_secret(enc_secret, enc_salt)
 
         data = getattr(request, 'data', None)
@@ -47,19 +47,29 @@
         auth_hdr = request_meta.get('HTTP_AUTHORIZATION')
 
         if not auth_hdr:
             return None
 
         auth_method, key, signature, date_in = self.parse_authorization_header(auth_hdr)
 
+        if not auth_method or not key or not signature or not date_in:
+            return None
+
+        # auth header structure is for hmac authentication
         if auth_method not in self.authentication_methods:
             raise AuthenticationFailed(f'Unsupported HMAC method {auth_method}')
 
         utcnow = datetime.datetime.now(timezone.utc)
-        delta = utcnow - datetime.datetime.fromisoformat(date_in)
+
+        try:
+            req_utc = datetime.datetime.fromisoformat(date_in)
+        except ValueError:
+            raise AuthenticationFailed('Invalid date format in Authorization header')
+
+        delta = utcnow - req_utc
         if delta.total_seconds() > auth_req_timeout:
             raise AuthenticationFailed('Request timed out')
 
         hmac_key = ApiHMACKey.objects.filter(id=key).first()
         if not hmac_key or hmac_key.revoked:
             raise AuthenticationFailed('Invalid API Key')
```

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/models.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/models.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/server_utils.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/server_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication/views.py` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication.egg-info/PKG-INFO` & `django_hmac_authentication-1.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-hmac-authentication
-Version: 1.1.0
+Name: django_hmac_authentication
+Version: 1.1.1
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
@@ -15,14 +15,15 @@
 Django hmac authentication with shared secret
 
 * Django model with HMAC shared encrypted secret
 * Authentication class `HMACAuthentication` 
 * Reject requests earlier than configured timeout
 * Supports `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * HMAC secret can be created with management command or obtained with a configured url
+* Supports Javascript and Python clients
 
 # 1. Install
 `pip install django_hmac_authentication`
 
 # 2. Configuration
 
 ## 2.1 settings.py
@@ -105,28 +106,35 @@
 A prerequest script for generating the signature is provided (same as included in postman collection).
 
 ## 4.2 Python client
 See `example_django_project/example_python_client.py`
 
 # 5. Signature
 
+# 5.1 How is it calculated
+
 Signature is calculated on hash( request body json ) + utc 8601
 
-Fields
+Steps:
+
+1. request body (data) -> json string in utf-8 -> hash -> **base64 of body hash**
+2. **utc 8601 string**
+3. string to sign = **base64 of body hash** + ";" + **utc 8601 string**
+4. signature = hash (string to sign) -> base64
 
-* Hash of request body. Hash function is one of supported methods in Authorization header
+* Hash function is one of supported methods in Authorization header
 * UTC time now in ISO 8601 format. Example `2023-05-07T14:15:37.862560+00:00`
 
 # 6. Authorization header
 * method: One of `HMAC-SHA512`, `HMAC-SHA384`, `HMAC-SHA256`
 * api_key: Key used to identify the hmac secret used to generate signature
 * signature: base64 signature
 * request_utc: time in ISO 8601 set in signed string
 
-`Syntax`: method api_key;signature;request_utc
+`Syntax`: METHOD api_key;signature;request_utc_8601
 
 Example
 ```python
 'HMAC-SHA512 aa733037-e4c0-4f75-a864-df6c1966481b;6k3XaUREI6dDw6thyQWASJjzjsx1M7GOZAglguv0OElpRue1+gb7CK2n3JpzJGz9VcREw2y3rIW5zoZYEUY+0w==;2023-05-07T14:15:37.862560+00:00'
 ```
 # 7. License
 Apache2 License
```

### Comparing `django_hmac_authentication-1.1.0/src/django_hmac_authentication.egg-info/SOURCES.txt` & `django_hmac_authentication-1.1.1/src/django_hmac_authentication.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -35,11 +35,12 @@
 src/example_django_project/example_django_project/asgi.py
 src/example_django_project/example_django_project/settings.py
 src/example_django_project/example_django_project/urls.py
 src/example_django_project/example_django_project/wsgi.py
 src/tests/__init__.py
 src/tests/factories.py
 src/tests/test_authentication_api_key_secret.py
+src/tests/test_hmac_authorization_header_parsing.py
 src/tests/test_mgmt_cmd_create_hmac_for_user.py
 src/tests/test_padding.py
 src/tests/test_utils.py
 src/tests/test_view_create_api_key_secret.py
```

### Comparing `django_hmac_authentication-1.1.0/src/example_django_project/accounts/views.py` & `django_hmac_authentication-1.1.1/src/example_django_project/accounts/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/example_django_project/example_django_project/settings.py` & `django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/example_django_project/example_django_project/urls.py` & `django_hmac_authentication-1.1.1/src/example_django_project/example_django_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/example_django_project/example_python_client.py` & `django_hmac_authentication-1.1.1/src/example_django_project/example_python_client.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/example_django_project/manage.py` & `django_hmac_authentication-1.1.1/src/example_django_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/tests/factories.py` & `django_hmac_authentication-1.1.1/src/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/tests/test_authentication_api_key_secret.py` & `django_hmac_authentication-1.1.1/src/tests/test_authentication_api_key_secret.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from rest_framework.test import APIRequestFactory, APITestCase
 from rest_framework.views import APIView
 
 from django_hmac_authentication.authentication import HMACAuthentication
 from django_hmac_authentication.client_utils import prepare_string_to_sign, sign_string
 from django_hmac_authentication.server_utils import aes_decrypt_hmac_secret
 from tests.factories import ApiHMACKeyFactory, ApiHMACKeyUserFactory
+from tests.test_hmac_authorization_header_parsing import (
+    test_data__authorization_header_parsing_invalid,
+)
 
 
 class TestView(APIView):
     authentication_classes = (HMACAuthentication,)
 
     def get(self, request):
         return Response(data={'method': 'GET'})
@@ -129,36 +132,14 @@
         response = self.view(request)
         self.assertEqual(
             response.status_code,
             HTTPStatus.OK,
             f'Authentication failed with digest {digest} http_method {http_method}',
         )
 
-    test_data__authorization_header_parsing__invalid = (
-        # invalid values for authorization header content
-        (None,),
-        ('',),
-        ('one_part',),
-        ('two parts',),
-        ('with three parts',),
-        ('with such four parts',),
-    )
-
-    @data(*test_data__authorization_header_parsing__invalid)
-    @unpack
-    def test_hmac_authentication_authorization_header_parsing__invalid(
-        self, header=None, expected_token=None
-    ):
-        header_parts = self.auth.parse_authorization_header(header)
-        for part in header_parts:
-            self.assertIsNone(
-                part,
-                f'Header parsing failed. Header part {part} when expecting None',
-            )
-
     def test_hmac_authentication__revoked(self):
         self.hmac_key.revoked = True
         self.hmac_key.save()
         self.hmac_key.refresh_from_db()
         factory = APIRequestFactory()
         req_data = ''
         signature, utc_8601 = self._request_auth_header_fields(req_data, 'HMAC-SHA512')
@@ -209,7 +190,25 @@
         request = factory.get('api/commons/languages/', data=None, **headers)
         response = self.view(request)
         self.assertEqual(
             response.status_code,
             HTTPStatus.FORBIDDEN,
             'Timed out request must fail authentication',
         )
+
+    @data(*test_data__authorization_header_parsing_invalid)
+    @unpack
+    def test_hmac_authentication__fail_malformed_header(
+        self, header=None, valid_header=False
+    ):
+        factory = APIRequestFactory()
+        headers = {
+            f'{self.auth_header}': header,
+            'Content-Type': 'application/json',
+        }
+        request = factory.get('/', data=None, **headers)
+        response = self.view(request)
+        self.assertEqual(
+            response.status_code,
+            HTTPStatus.FORBIDDEN,
+            'Authentication must fail on malformed header',
+        )
```

### Comparing `django_hmac_authentication-1.1.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py` & `django_hmac_authentication-1.1.1/src/tests/test_mgmt_cmd_create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/tests/test_padding.py` & `django_hmac_authentication-1.1.1/src/tests/test_padding.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/tests/test_utils.py` & `django_hmac_authentication-1.1.1/src/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.1.0/src/tests/test_view_create_api_key_secret.py` & `django_hmac_authentication-1.1.1/src/tests/test_view_create_api_key_secret.py`

 * *Files identical despite different names*

