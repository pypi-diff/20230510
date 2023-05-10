# Comparing `tmp/wc-django-envoyer-0.2.1.tar.gz` & `tmp/wc-django-envoyer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-envoyer-0.2.1.tar", last modified: Tue May  9 09:46:46 2023, max compression
+gzip compressed data, was "wc-django-envoyer-0.2.2.tar", last modified: Wed May 10 13:31:31 2023, max compression
```

## Comparing `wc-django-envoyer-0.2.1.tar` & `wc-django-envoyer-0.2.2.tar`

### file list

```diff
@@ -1,75 +1,78 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      297 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/CHANGELOG.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/LICENSE
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      153 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/MANIFEST.in
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/Makefile
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7075 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/PKG-INFO
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     6224 2023-05-09 09:46:33.000000 wc-django-envoyer-0.2.1/README.md
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/setup.cfg
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1762 2023-05-08 11:10:01.000000 wc-django-envoyer-0.2.1/setup.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.804917 wc-django-envoyer-0.2.1/tests/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2192 2023-05-09 08:47:31.000000 wc-django-envoyer-0.2.1/tests/test_celery.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3981 2023-05-09 08:04:15.000000 wc-django-envoyer-0.2.1/tests/test_run.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      593 2023-05-09 08:31:54.000000 wc-django-envoyer-0.2.1/tox.ini
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.804917 wc-django-envoyer-0.2.1/wc_django_envoyer.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7075 2023-05-09 09:46:46.000000 wc-django-envoyer-0.2.1/wc_django_envoyer.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1768 2023-05-09 09:46:46.000000 wc-django-envoyer-0.2.1/wc_django_envoyer.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-05-09 09:46:46.000000 wc-django-envoyer-0.2.1/wc_django_envoyer.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      285 2023-05-09 09:46:46.000000 wc-django-envoyer-0.2.1/wc_django_envoyer.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2023-05-09 09:46:46.000000 wc-django-envoyer-0.2.1/wc_django_envoyer.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.804917 wc-django-envoyer-0.2.1/wcd_envoyer/
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      453 2023-05-09 09:46:42.000000 wc-django-envoyer-0.2.1/wcd_envoyer/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.804917 wc-django-envoyer-0.2.1/wcd_envoyer/admin/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       73 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/admin/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/admin/channels.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      376 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/admin/forms.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1156 2023-05-09 09:22:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/admin/messages.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2889 2023-05-09 09:20:35.000000 wc-django-envoyer-0.2.1/wcd_envoyer/admin/templates.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2320 2023-05-09 09:20:20.000000 wc-django-envoyer-0.2.1/wcd_envoyer/admin/utils.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)      322 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/apps.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/channels/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      102 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/channels/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5974 2023-05-08 08:50:13.000000 wc-django-envoyer-0.2.1/wcd_envoyer/channels/backend.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/channels/backends/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/channels/backends/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      952 2023-05-08 08:25:08.000000 wc-django-envoyer-0.2.1/wcd_envoyer/channels/backends/console.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4308 2023-05-08 12:08:11.000000 wc-django-envoyer-0.2.1/wcd_envoyer/channels/backends/django_sendmail.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      852 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/channels/forms.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1236 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/channels/registry_base.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/channels/renderers.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2510 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      471 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/const.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-08 12:43:08.000000 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-08 12:45:33.000000 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/services/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-08 12:45:44.000000 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1191 2023-05-09 09:14:05.000000 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/services/sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1186 2023-05-09 08:38:21.000000 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/shortcuts.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      640 2023-05-09 08:47:21.000000 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/tasks.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/pxd_actions_tracker/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:38:55.000000 wc-django-envoyer-0.2.1/wcd_envoyer/contrib/pxd_actions_tracker/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1441 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/events.py
--rwxrwxr-x   0 preusx    (1000) preusx    (1000)       40 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/exceptions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1428 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/migrations/0002_auto_20230505_0852.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/models/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/models/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      841 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/models/channels.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2651 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/models/messages.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/models/utils.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/services/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/services/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     8341 2023-05-09 09:09:38.000000 wc-django-envoyer-0.2.1/wcd_envoyer/services/sender.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      784 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/services/templates_resolver.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      935 2023-05-08 09:18:19.000000 wc-django-envoyer-0.2.1/wcd_envoyer/shortcuts.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      129 2023-05-09 09:05:12.000000 wc-django-envoyer-0.2.1/wcd_envoyer/signals.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-09 09:46:46.808917 wc-django-envoyer-0.2.1/wcd_envoyer/utils/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/utils/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1514 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/utils/functional.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1030 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/utils/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      489 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/utils/registry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      193 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.1/wcd_envoyer/utils/types.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      407 2023-05-10 13:29:01.000000 wc-django-envoyer-0.2.2/CHANGELOG.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1072 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/LICENSE
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      153 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/MANIFEST.in
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/Makefile
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7392 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/PKG-INFO
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     6431 2023-05-10 13:24:36.000000 wc-django-envoyer-0.2.2/README.md
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       79 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/setup.cfg
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)     1762 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.271869 wc-django-envoyer-0.2.2/tests/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2192 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/tests/test_celery.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3981 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/tests/test_run.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      593 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/tox.ini
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.271869 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7392 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1919 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      285 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       12 2023-05-10 13:31:31.000000 wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.271869 wc-django-envoyer-0.2.2/wcd_envoyer/
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      453 2023-05-10 13:28:56.000000 wc-django-envoyer-0.2.2/wcd_envoyer/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/admin/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       73 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/channels.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      376 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/forms.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1156 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/messages.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2889 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/templates.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2320 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/admin/utils.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      322 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/apps.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/channels/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      102 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5974 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backend.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      952 2023-05-10 13:20:17.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/console.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4478 2023-05-10 12:13:08.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/django_sendmail.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      852 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/forms.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1236 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/registry_base.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      250 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/channels/renderers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      560 2023-05-10 13:16:57.000000 wc-django-envoyer-0.2.2/wcd_envoyer/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      471 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/const.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/services/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1191 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/services/sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1186 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/shortcuts.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      640 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/tasks.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       89 2023-05-10 11:42:54.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/__init__.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)      393 2023-05-10 11:46:44.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      386 2023-05-10 13:28:21.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/handlers.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1261 2023-05-10 13:29:11.000000 wc-django-envoyer-0.2.2/wcd_envoyer/contrib/pxd_actions_tracker/tracker.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1441 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/events.py
+-rwxrwxr-x   0 preusx    (1000) preusx    (1000)       40 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/exceptions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3457 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1428 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/migrations/0002_auto_20230505_0852.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/models/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       69 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/models/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      841 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/models/channels.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2651 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/models/messages.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      415 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/models/utils.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/services/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/services/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     8672 2023-05-10 13:07:02.000000 wc-django-envoyer-0.2.2/wcd_envoyer/services/sender.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      784 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/services/templates_resolver.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      935 2023-05-08 09:18:19.000000 wc-django-envoyer-0.2.2/wcd_envoyer/shortcuts.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      129 2023-05-10 08:01:03.000000 wc-django-envoyer-0.2.2/wcd_envoyer/signals.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2023-05-10 13:31:31.275869 wc-django-envoyer-0.2.2/wcd_envoyer/utils/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1514 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/functional.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1030 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/models.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      489 2023-05-05 10:25:29.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/registry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      855 2023-05-10 13:20:23.000000 wc-django-envoyer-0.2.2/wcd_envoyer/utils/types.py
```

### Comparing `wc-django-envoyer-0.2.1/LICENSE` & `wc-django-envoyer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/Makefile` & `wc-django-envoyer-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/PKG-INFO` & `wc-django-envoyer-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-envoyer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Message sender to different channels.
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -218,17 +218,31 @@
 ```python
 from wcd_envoyer.admin import MessageAdmin
 
 # Looking hacky, but you you need - just inherit from `MessageAdmin`
 # and re-register admin for `Message` model.
 MessageAdmin.messages_sender = created_task.sender
 ```
+
+### Error tracking
+
+You can track failed messages with signals. Or there is a simple connector for `px-django-actions-tracker` lib. Just add `'wcd_envoyer.contrib.pxd_actions_tracker'` to `INSTALLED_APPS`.
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.2]
+### Added
+- Errors tracking.
+
+## [0.2.0]
+### Added
+- Celery sender.
+### Fixed
+- API improvements.
+
 ## [0.1.0]
 Initial version.
```

### Comparing `wc-django-envoyer-0.2.1/README.md` & `wc-django-envoyer-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -200,7 +200,11 @@
 ```python
 from wcd_envoyer.admin import MessageAdmin
 
 # Looking hacky, but you you need - just inherit from `MessageAdmin`
 # and re-register admin for `Message` model.
 MessageAdmin.messages_sender = created_task.sender
 ```
+
+### Error tracking
+
+You can track failed messages with signals. Or there is a simple connector for `px-django-actions-tracker` lib. Just add `'wcd_envoyer.contrib.pxd_actions_tracker'` to `INSTALLED_APPS`.
```

### Comparing `wc-django-envoyer-0.2.1/setup.py` & `wc-django-envoyer-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/tests/test_celery.py` & `wc-django-envoyer-0.2.2/tests/test_celery.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/tests/test_run.py` & `wc-django-envoyer-0.2.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/tox.ini` & `wc-django-envoyer-0.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wc_django_envoyer.egg-info/PKG-INFO` & `wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-envoyer
-Version: 0.2.1
+Version: 0.2.2
 Summary: Message sender to different channels.
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
@@ -218,17 +218,31 @@
 ```python
 from wcd_envoyer.admin import MessageAdmin
 
 # Looking hacky, but you you need - just inherit from `MessageAdmin`
 # and re-register admin for `Message` model.
 MessageAdmin.messages_sender = created_task.sender
 ```
+
+### Error tracking
+
+You can track failed messages with signals. Or there is a simple connector for `px-django-actions-tracker` lib. Just add `'wcd_envoyer.contrib.pxd_actions_tracker'` to `INSTALLED_APPS`.
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.2]
+### Added
+- Errors tracking.
+
+## [0.2.0]
+### Added
+- Celery sender.
+### Fixed
+- API improvements.
+
 ## [0.1.0]
 Initial version.
```

### Comparing `wc-django-envoyer-0.2.1/wc_django_envoyer.egg-info/SOURCES.txt` & `wc-django-envoyer-0.2.2/wc_django_envoyer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 wcd_envoyer/contrib/__init__.py
 wcd_envoyer/contrib/celery/__init__.py
 wcd_envoyer/contrib/celery/shortcuts.py
 wcd_envoyer/contrib/celery/tasks.py
 wcd_envoyer/contrib/celery/services/__init__.py
 wcd_envoyer/contrib/celery/services/sender.py
 wcd_envoyer/contrib/pxd_actions_tracker/__init__.py
+wcd_envoyer/contrib/pxd_actions_tracker/apps.py
+wcd_envoyer/contrib/pxd_actions_tracker/handlers.py
+wcd_envoyer/contrib/pxd_actions_tracker/tracker.py
 wcd_envoyer/migrations/0001_initial.py
 wcd_envoyer/migrations/0002_auto_20230505_0852.py
 wcd_envoyer/migrations/__init__.py
 wcd_envoyer/models/__init__.py
 wcd_envoyer/models/channels.py
 wcd_envoyer/models/messages.py
 wcd_envoyer/models/utils.py
```

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/admin/messages.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/admin/messages.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/admin/templates.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/admin/templates.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/admin/utils.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/admin/utils.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/channels/backend.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/channels/backend.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/channels/backends/console.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/console.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/channels/backends/django_sendmail.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/channels/backends/django_sendmail.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import *
-from django import forms
-
-from django.contrib.postgres.forms import SimpleArrayField
+import traceback
 
+from django import forms
 from django.conf import settings
 from django.core.mail import EmailMultiAlternatives, get_connection
 from django.utils.translation import pgettext_lazy
+from django.contrib.postgres.forms import SimpleArrayField
 
 from wcd_envoyer.channels.backend import (
     BaseMessagingBackend, BaseMessagesMaker, SplitRecipientsMessagesMaker,
 )
 from wcd_envoyer.channels.forms import BaseTemplateForm, BaseConfigForm
 from wcd_envoyer.utils import importable_prop
 from wcd_envoyer.models import Message, ChannelConfig
@@ -125,13 +125,16 @@
                         count = connection.send_messages([email])
 
                         if count == 1:
                             sent.append(message)
                         else:
                             failed.append((message, None))
                     except Exception as e:
-                        failed.append((message, e))
+                        failed.append((message, {
+                            'exception': e, 'message': str(e),
+                            'traceback': traceback.format_exc(),
+                        }))
 
         except Exception as e:
             return [], [(x, e) for x in messages]
 
         return sent, failed
```

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/channels/forms.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/channels/forms.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/channels/registry_base.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/channels/registry_base.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/services/sender.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/services/sender.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/shortcuts.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/shortcuts.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/contrib/celery/tasks.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/contrib/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/events.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/events.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/migrations/0001_initial.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/migrations/0002_auto_20230505_0852.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/migrations/0002_auto_20230505_0852.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/models/channels.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/models/channels.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/models/messages.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/models/messages.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/services/sender.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/services/sender.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import *
+import traceback
+import logging
 from collections import defaultdict
 
 from django.utils.translation import get_language, override
 
 
 from wcd_envoyer.events import EventRegistry, registry as events_registry
 from wcd_envoyer.channels import (
@@ -170,16 +172,20 @@
 
         for backend, config, messages in messages_groups:
             try:
                 c_succeeded, c_failed = backend.send(
                     config, messages, context=context,
                 )
             except Exception as e:
+                error = {
+                    'exception': e, 'message': str(e),
+                    'traceback': traceback.format_exc(),
+                }
                 c_succeeded = []
-                c_failed = [(x, e) for x in messages]
+                c_failed = [(x, error) for x in messages]
 
             if len(c_succeeded) > 0:
                 succeeded.append((backend, config, c_succeeded))
 
             if len(c_failed) > 0:
                 failed.append((backend, config, c_failed))
 
@@ -196,33 +202,36 @@
                     MessageStatus.FAILED, [x for x, _ in all_failed],
                     only_for_status=MessageStatus.PENDING, skip_db=True,
                 )
             ),
             only_for_status=MessageStatus.PENDING,
         )
 
-        if len(succeeded) > 0:
-            messages_sent_succeeded.send(
-                self, messages_groups=succeeded, messages=all_succeeded,
-                context=context,
-            )
+        try:
+            if len(succeeded) > 0:
+                messages_sent_succeeded.send(
+                    self, messages_groups=succeeded, messages=all_succeeded,
+                    context=context,
+                )
 
-        if len(failed) > 0:
-            messages_sent_failed.send(
-                self, messages_groups=succeeded, messages=all_succeeded,
+            if len(failed) > 0:
+                messages_sent_failed.send(
+                    self, messages_groups=failed, messages=all_failed,
+                    context=context,
+                )
+
+            messages_sent.send(
+                self,
+                succeeded_messages_groups=succeeded,
+                failed_messages_groups=failed,
+                messages=all_succeeded + all_failed,
                 context=context,
             )
-
-        messages_sent.send(
-            self,
-            succeeded_messages_groups=succeeded,
-            failed_messages_groups=failed,
-            messages=all_succeeded + all_failed,
-            context=context,
-        )
+        except Exception as e:
+            logging.exception(e)
 
         return succeeded, failed
 
     def send_messages(self, messages: Iterable[Message], context: dict = {}):
         backends = self.get_backends()
         configs = self.get_channel_configs(backends.keys())
```

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/services/templates_resolver.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/services/templates_resolver.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/shortcuts.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/shortcuts.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/utils/functional.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/utils/functional.py`

 * *Files identical despite different names*

### Comparing `wc-django-envoyer-0.2.1/wcd_envoyer/utils/models.py` & `wc-django-envoyer-0.2.2/wcd_envoyer/utils/models.py`

 * *Files identical despite different names*

