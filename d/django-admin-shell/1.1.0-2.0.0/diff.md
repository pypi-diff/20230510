# Comparing `tmp/django-admin-shell-1.1.0.tar.gz` & `tmp/django-admin-shell-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-shell-1.1.0.tar", last modified: Fri Jul  8 08:52:11 2022, max compression
+gzip compressed data, was "django-admin-shell-2.0.0.tar", last modified: Wed May 10 10:36:34 2023, max compression
```

## Comparing `django-admin-shell-1.1.0.tar` & `django-admin-shell-2.0.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1059 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/LICENSE
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      113 2022-07-08 08:38:23.000000 django-admin-shell-1.1.0/MANIFEST.in
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      804 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/PKG-INFO
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     7481 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/README.rst
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       68 2022-07-08 08:37:12.000000 django-admin-shell-1.1.0/django_admin_shell/__init__.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      135 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/apps.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      206 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/forms.py
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/migrations/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/migrations/__init__.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1615 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/settings.py
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/static/
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/css/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   121200 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/css/bootstrap3.min.css
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      892 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/css/shell.css
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    20127 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   108738 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    45404 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    23424 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    18028 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    86709 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/jquery.min.js
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1234 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea-license.txt
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1294 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea.css
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4133 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea.js
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2578 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/shell.js
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      793 2017-01-28 17:02:59.000000 django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/shell.min.js
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/templates/
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/templates/django_admin_shell/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      886 2017-01-26 18:31:42.000000 django-admin-shell-1.1.0/django_admin_shell/templates/django_admin_shell/base.html
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2906 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/templates/django_admin_shell/shell.html
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell/tests/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2017-01-28 17:02:59.000000 django-admin-shell-1.1.0/django_admin_shell/tests/__init__.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      188 2017-01-28 17:02:59.000000 django-admin-shell-1.1.0/django_admin_shell/tests/models.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1725 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/tests/settings.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2011 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/tests/test_importer.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     6763 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/tests/test_runner.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     7620 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/tests/test_view.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      361 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/tests/urls.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      411 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/urls.py
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     7978 2022-07-08 08:26:10.000000 django-admin-shell-1.1.0/django_admin_shell/views.py
-drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/django_admin_shell.egg-info/
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      804 2022-07-08 08:52:11.000000 django-admin-shell-1.1.0/django_admin_shell.egg-info/PKG-INFO
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1890 2022-07-08 08:52:11.000000 django-admin-shell-1.1.0/django_admin_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        1 2022-07-08 08:52:11.000000 django-admin-shell-1.1.0/django_admin_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        1 2022-07-08 08:41:27.000000 django-admin-shell-1.1.0/django_admin_shell.egg-info/not-zip-safe
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       12 2022-07-08 08:52:11.000000 django-admin-shell-1.1.0/django_admin_shell.egg-info/requires.txt
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       19 2022-07-08 08:52:11.000000 django-admin-shell-1.1.0/django_admin_shell.egg-info/top_level.txt
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      221 2022-07-08 08:52:11.714612 django-admin-shell-1.1.0/setup.cfg
--rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1550 2022-07-08 08:52:03.000000 django-admin-shell-1.1.0/setup.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1059 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/LICENSE
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      113 2022-07-08 08:38:23.000000 django-admin-shell-2.0.0/MANIFEST.in
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      843 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/PKG-INFO
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     7571 2023-05-10 10:22:51.000000 django-admin-shell-2.0.0/README.rst
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:33.998818 django-admin-shell-2.0.0/django_admin_shell/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       68 2023-05-10 10:24:25.000000 django-admin-shell-2.0.0/django_admin_shell/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      135 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/apps.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      206 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/forms.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/django_admin_shell/migrations/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/migrations/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1615 2022-07-08 08:26:10.000000 django-admin-shell-2.0.0/django_admin_shell/settings.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:33.998818 django-admin-shell-2.0.0/django_admin_shell/static/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:33.998818 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/css/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   121200 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/css/bootstrap3.min.css
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      892 2022-07-08 08:26:10.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/css/shell.css
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    20127 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)   108738 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    45404 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    23424 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    18028 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)    86709 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/jquery.min.js
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1234 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea-license.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1294 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea.css
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     4133 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2578 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/shell.js
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      793 2017-01-28 17:02:59.000000 django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/shell.min.js
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:33.998818 django-admin-shell-2.0.0/django_admin_shell/templates/
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/django_admin_shell/templates/django_admin_shell/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      886 2017-01-26 18:31:42.000000 django-admin-shell-2.0.0/django_admin_shell/templates/django_admin_shell/base.html
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2906 2022-07-08 08:26:10.000000 django-admin-shell-2.0.0/django_admin_shell/templates/django_admin_shell/shell.html
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/django_admin_shell/tests/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        0 2017-01-28 17:02:59.000000 django-admin-shell-2.0.0/django_admin_shell/tests/__init__.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      188 2017-01-28 17:02:59.000000 django-admin-shell-2.0.0/django_admin_shell/tests/models.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1776 2023-05-10 09:13:39.000000 django-admin-shell-2.0.0/django_admin_shell/tests/settings.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     2011 2022-07-08 08:26:10.000000 django-admin-shell-2.0.0/django_admin_shell/tests/test_importer.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     6763 2022-07-08 08:26:10.000000 django-admin-shell-2.0.0/django_admin_shell/tests/test_runner.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     7620 2022-07-08 08:26:10.000000 django-admin-shell-2.0.0/django_admin_shell/tests/test_view.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      361 2022-07-08 08:26:10.000000 django-admin-shell-2.0.0/django_admin_shell/tests/urls.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      411 2023-05-10 07:52:52.000000 django-admin-shell-2.0.0/django_admin_shell/urls.py
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     7978 2022-07-08 08:26:10.000000 django-admin-shell-2.0.0/django_admin_shell/views.py
+drwxrwxr-x   0 grzegorz  (1000) grzegorz  (1000)        0 2023-05-10 10:36:33.998818 django-admin-shell-2.0.0/django_admin_shell.egg-info/
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      843 2023-05-10 10:36:33.000000 django-admin-shell-2.0.0/django_admin_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1890 2023-05-10 10:36:33.000000 django-admin-shell-2.0.0/django_admin_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        1 2023-05-10 10:36:33.000000 django-admin-shell-2.0.0/django_admin_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)        1 2023-05-10 10:36:33.000000 django-admin-shell-2.0.0/django_admin_shell.egg-info/not-zip-safe
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       12 2023-05-10 10:36:33.000000 django-admin-shell-2.0.0/django_admin_shell.egg-info/requires.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)       19 2023-05-10 10:36:33.000000 django-admin-shell-2.0.0/django_admin_shell.egg-info/top_level.txt
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)      221 2023-05-10 10:36:34.002818 django-admin-shell-2.0.0/setup.cfg
+-rw-rw-r--   0 grzegorz  (1000) grzegorz  (1000)     1553 2023-05-10 10:21:48.000000 django-admin-shell-2.0.0/setup.py
```

### Comparing `django-admin-shell-1.1.0/LICENSE` & `django-admin-shell-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/README.rst` & `django-admin-shell-2.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 
 
 Django application can execute python code in your project's environment on django admin site.
 You can use similar as `python manage shell` without reloading the environment.
 
 
 * Tested by tox with:
-    - Python :2.7, 3.6, 3.8
-    - Django : 1.10, 1.11, 2.0, 2.1, 2.2, 3.0, 3.1, 3.2
+    - Python : 3.7, 3.8, 3.10
+    - Django : 2.0, 2.1, 2.2, 3.0, 3.1, 3.2, 4.0, 4.2
 
 * Require:
     - Django >= 1.10
 
 * Tested on browsers
+    - OK - Chromium  108 - Ubuntu 20.04
+    - OK - Firefox 112.0.2 - Ubuntu 20.04
     - OK - Chromium 89 - Ubuntu 18.04
     - OK - Firefox 87.0 - Ubuntu 18.04
     - OK - Chromium 79.0  - Ubuntu 18.04
     - OK - Firefox 72.0.2 - Ubuntu 18.04
     - OK - Firefox 50.1.0 - Ubuntu 14.04
     - OK - Firefox 31.1 - CentOS 6.4
     - OK - Chromium 53.0 - Ubuntu 14.04
@@ -82,17 +84,17 @@
     ]
 
 3. Add the `django_admin_shell` urls to your root url patterns (above admin/) :
 
  *urls.py* ::
 
     urlpatterns = [
-        url(r'^admin/shell/', include('django_admin_shell.urls')),
+        re_path(r'^admin/shell/', include('django_admin_shell.urls')),
         ...
-        url(r'^admin/', admin.site.urls),
+        re_path(r'^admin/', admin.site.urls),
     ]
 
 
 Usage
 ------
 * shell is available on url: **/admin/shell**
 * On default settings user must be authenticated to django admin site and
```

### Comparing `django-admin-shell-1.1.0/django_admin_shell/settings.py` & `django-admin-shell-2.0.0/django_admin_shell/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/css/bootstrap3.min.css` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/css/bootstrap3.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/css/shell.css` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/css/shell.css`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.eot` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.svg` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.ttf` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.woff` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.woff2` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/jquery.min.js` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea-license.txt` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea-license.txt`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea.css` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea.css`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea.js` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/linedtextarea/jquery-linedtextarea.js`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/shell.js` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/shell.js`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/static/django_admin_shell/js/shell.min.js` & `django-admin-shell-2.0.0/django_admin_shell/static/django_admin_shell/js/shell.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/templates/django_admin_shell/base.html` & `django-admin-shell-2.0.0/django_admin_shell/templates/django_admin_shell/base.html`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/templates/django_admin_shell/shell.html` & `django-admin-shell-2.0.0/django_admin_shell/templates/django_admin_shell/shell.html`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/tests/settings.py` & `django-admin-shell-2.0.0/django_admin_shell/tests/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,7 +55,9 @@
         'ENGINE': 'django.db.backends.sqlite3',
         'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
     }
 }
 
 LANGUAGE_CODE = 'en-us'
 STATIC_URL = '/static/'
+
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
```

### Comparing `django-admin-shell-1.1.0/django_admin_shell/tests/test_importer.py` & `django-admin-shell-2.0.0/django_admin_shell/tests/test_importer.py`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/tests/test_runner.py` & `django-admin-shell-2.0.0/django_admin_shell/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/tests/test_view.py` & `django-admin-shell-2.0.0/django_admin_shell/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell/views.py` & `django-admin-shell-2.0.0/django_admin_shell/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/django_admin_shell.egg-info/SOURCES.txt` & `django-admin-shell-2.0.0/django_admin_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-shell-1.1.0/setup.py` & `django-admin-shell-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,22 +27,22 @@
         'static/django_admin_shell/js/linedtextarea/*',
         'static/django_admin_shell/fonts/*',
         'static/django_admin_shell/css/*',
     ]},
     tests_require=['Django', 'flake8', 'mock'],
     include_package_data=True,
     zip_safe=False,
-    install_requires=['Django>=1.9'],
+    install_requires=['Django>=2.0'],
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Utilities',
     ],
     keywords='django admin shell console terminal',
 )
```

