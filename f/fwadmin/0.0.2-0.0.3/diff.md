# Comparing `tmp/fwadmin-0.0.2.tar.gz` & `tmp/fwadmin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwadmin-0.0.2.tar", last modified: Wed May 10 10:59:51 2023, max compression
+gzip compressed data, was "fwadmin-0.0.3.tar", last modified: Wed May 10 15:56:09 2023, max compression
```

## Comparing `fwadmin-0.0.2.tar` & `fwadmin-0.0.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.395972 fwadmin-0.0.2/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-05-05 06:03:20.000000 fwadmin-0.0.2/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      248 2023-05-05 06:18:18.000000 fwadmin-0.0.2/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      477 2023-05-10 10:59:51.395972 fwadmin-0.0.2/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      614 2023-05-05 19:11:38.000000 fwadmin-0.0.2/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.379972 fwadmin-0.0.2/fwadmin/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1353 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.391972 fwadmin-0.0.2/fwadmin/api/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/api/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1911 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/api/serializers.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      604 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/api/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1215 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/api/views.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2604 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/filtersets.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4348 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/forms.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.391972 fwadmin-0.0.2/fwadmin/migrations/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7938 2023-05-10 10:59:49.000000 fwadmin-0.0.2/fwadmin/migrations/0001_initial.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      499 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/migrations/0002_remove_sessionrequest_user_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1115 2023-05-10 10:59:49.000000 fwadmin-0.0.2/fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      985 2023-05-10 10:59:49.000000 fwadmin-0.0.2/fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      612 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:49.000000 fwadmin-0.0.2/fwadmin/migrations/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7258 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/models.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2162 2023-05-10 10:59:49.000000 fwadmin-0.0.2/fwadmin/navigation.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2954 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/tables.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.371971 fwadmin-0.0.2/fwadmin/templates/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.391972 fwadmin-0.0.2/fwadmin/templates/fwadmin/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.391972 fwadmin-0.0.2/fwadmin/templates/fwadmin/buttons/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      402 2023-05-08 19:10:26.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/buttons/approve.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      399 2023-05-08 19:10:38.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/buttons/reject.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      412 2023-05-08 19:11:15.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/buttons/self_approve.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1495 2023-05-06 13:26:26.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/devicegroup.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2557 2023-05-10 10:35:53.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/dynamiclist.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1852 2023-05-06 13:21:06.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/firewall.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.391972 fwadmin-0.0.2/fwadmin/templates/fwadmin/htmx/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1250 2023-05-09 18:44:21.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/htmx/manage_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3169 2023-05-08 18:21:36.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/sessionrequest.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1381 2023-05-10 09:38:16.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1973 2023-05-10 10:43:02.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/sessionrequest_list.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      637 2023-05-08 18:50:35.000000 fwadmin-0.0.2/fwadmin/templates/fwadmin/sessionrequest_manage.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.391972 fwadmin-0.0.2/fwadmin/templatetags/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/templatetags/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.395972 fwadmin-0.0.2/fwadmin/templatetags/__pycache__/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      150 2023-05-05 15:02:55.000000 fwadmin-0.0.2/fwadmin/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1284 2023-05-10 09:28:33.000000 fwadmin-0.0.2/fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-05-05 06:16:08.000000 fwadmin-0.0.2/fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1203 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/templatetags/fwadmin_buttons.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3980 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    16276 2023-05-10 10:59:49.000000 fwadmin-0.0.2/fwadmin/views.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-05-10 10:59:50.000000 fwadmin-0.0.2/fwadmin/workflows.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 10:59:51.391972 fwadmin-0.0.2/fwadmin.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      477 2023-05-10 10:59:51.000000 fwadmin-0.0.2/fwadmin.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1629 2023-05-10 10:59:51.000000 fwadmin-0.0.2/fwadmin.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-10 10:59:51.000000 fwadmin-0.0.2/fwadmin.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-05 14:55:33.000000 fwadmin-0.0.2/fwadmin.egg-info/not-zip-safe
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       89 2023-05-10 10:59:51.000000 fwadmin-0.0.2/fwadmin.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        8 2023-05-10 10:59:51.000000 fwadmin-0.0.2/fwadmin.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-05-10 10:59:51.395972 fwadmin-0.0.2/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1182 2023-05-10 10:59:49.000000 fwadmin-0.0.2/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.291735 fwadmin-0.0.3/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-05-05 06:03:20.000000 fwadmin-0.0.3/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      248 2023-05-05 06:18:18.000000 fwadmin-0.0.3/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      477 2023-05-10 15:56:09.291735 fwadmin-0.0.3/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      614 2023-05-05 19:11:38.000000 fwadmin-0.0.3/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.275735 fwadmin-0.0.3/fwadmin/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1414 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.279735 fwadmin-0.0.3/fwadmin/api/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/api/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1911 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/api/serializers.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      604 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/api/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1215 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/api/views.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2604 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/filtersets.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4206 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/forms.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.283735 fwadmin-0.0.3/fwadmin/migrations/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7938 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0001_initial.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      499 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0002_remove_sessionrequest_user_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1115 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      985 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      612 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7231 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/models.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2162 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/navigation.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3008 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/tables.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3386 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/tasks.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.267734 fwadmin-0.0.3/fwadmin/templates/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.287735 fwadmin-0.0.3/fwadmin/templates/fwadmin/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.287735 fwadmin-0.0.3/fwadmin/templates/fwadmin/buttons/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      402 2023-05-08 19:10:26.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/buttons/approve.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      399 2023-05-08 19:10:38.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/buttons/reject.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      412 2023-05-08 19:11:15.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/buttons/self_approve.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1495 2023-05-06 13:26:26.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/devicegroup.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2557 2023-05-10 10:35:53.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/dynamiclist.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1852 2023-05-06 13:21:06.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/firewall.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.287735 fwadmin-0.0.3/fwadmin/templates/fwadmin/htmx/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1250 2023-05-09 18:44:21.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/htmx/manage_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3169 2023-05-08 18:21:36.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1381 2023-05-10 09:38:16.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1973 2023-05-10 10:43:02.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_list.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      637 2023-05-08 18:50:35.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_manage.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.291735 fwadmin-0.0.3/fwadmin/templatetags/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/templatetags/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.291735 fwadmin-0.0.3/fwadmin/templatetags/__pycache__/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      150 2023-05-05 15:02:55.000000 fwadmin-0.0.3/fwadmin/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1284 2023-05-10 09:28:33.000000 fwadmin-0.0.3/fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-05-05 06:16:08.000000 fwadmin-0.0.3/fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1203 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/templatetags/fwadmin_buttons.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3980 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    16276 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/views.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/workflows.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.279735 fwadmin-0.0.3/fwadmin.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      477 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1646 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-05 14:55:33.000000 fwadmin-0.0.3/fwadmin.egg-info/not-zip-safe
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        9 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        8 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-05-10 15:56:09.291735 fwadmin-0.0.3/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1058 2023-05-10 15:56:08.000000 fwadmin-0.0.3/setup.py
```

### Comparing `fwadmin-0.0.2/LICENSE` & `fwadmin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/README.md` & `fwadmin-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/__init__.py` & `fwadmin-0.0.3/fwadmin/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main class."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 import os
 import pkgutil
 import shutil
 
 from django.conf import settings
 
@@ -24,15 +24,16 @@
     verbose_name = "FWAdmin"
     description = "Firewall manager and viewer plugin for Netbox"
     version = __version__
     author = "Andrea Dainese"
     author_email = "andrea@adainese.it"
     base_url = "fwadmin"
     default_settings = {
-        "ALLOW_SELF_APPROVAL": True,
+        "ALLOW_SELF_APPROVAL": True,  # TODO: not implemented
+        "EDL_UPDATE_INTERVAL": 300,
     }
 
 
 config = FWAdminConfig  # pylint: disable=invalid-name
 
 # Copy scripts
 package = pkgutil.get_loader("fwadmin")
```

### Comparing `fwadmin-0.0.2/fwadmin/api/serializers.py` & `fwadmin-0.0.3/fwadmin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/api/urls.py` & `fwadmin-0.0.3/fwadmin/api/urls.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/api/views.py` & `fwadmin-0.0.3/fwadmin/api/views.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/filtersets.py` & `fwadmin-0.0.3/fwadmin/filtersets.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/forms.py` & `fwadmin-0.0.3/fwadmin/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,31 +79,28 @@
 
 class FirewallForm(NetBoxModelForm):
     """Form used to add/edit Firewall."""
 
     name = forms.CharField()
     address = forms.CharField(help_text="IP address or FQDN used to connect to")
     model = forms.ChoiceField(choices=FirewallChoices)
-    access_key = forms.CharField(
-        required=False, widget=forms.PasswordInput, help_text="Username or access key"
-    )
     secret_key = forms.CharField(
-        required=False, widget=forms.PasswordInput, help_text="Password or secret key"
+        widget=forms.PasswordInput, help_text="Password or secret key"
     )
 
     class Meta:
         """Form metadata."""
 
         model = Firewall
         fields = [
             "name",
             "address",
             "model",
-            "access_key",
             "secret_key",
+            "verify_cert",
             "tags",
         ]
 
 
 class SessionRequestForm(NetBoxModelForm):
     """Form used to add SessionRequest."""
```

### Comparing `fwadmin-0.0.2/fwadmin/migrations/0001_initial.py` & `fwadmin-0.0.3/fwadmin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py` & `fwadmin-0.0.3/fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py` & `fwadmin-0.0.3/fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py` & `fwadmin-0.0.3/fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/models.py` & `fwadmin-0.0.3/fwadmin/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,19 +162,17 @@
     name = models.CharField(max_length=100, help_text="Firewall name")
     address = models.CharField(
         max_length=100, help_text="Management FQDN or IP address"
     )
     model = models.CharField(
         max_length=100, choices=FirewallChoices, default="paloalto-panos"
     )
-    access_key = models.CharField(
-        max_length=200, blank=True, help_text="Username or access key"
-    )
-    secret_key = models.CharField(
-        max_length=200, blank=True, help_text="Password or secret token"
+    secret_key = models.CharField(max_length=200, help_text="Password or secret token")
+    verify_cert = models.BooleanField(
+        default=True, help_text="Validate firewall's certificate"
     )
 
     class Meta:
         """Database metadata."""
 
         ordering = ["name"]
         unique_together = [["name"], ["address"]]
```

### Comparing `fwadmin-0.0.2/fwadmin/navigation.py` & `fwadmin-0.0.3/fwadmin/navigation.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/tables.py` & `fwadmin-0.0.3/fwadmin/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,22 +76,24 @@
         model = models.Firewall
         fields = [
             "pk",
             "id",
             "name",
             "address",
             "model",
+            "verify_cert",
             "dynamiclist_count",
             "last_updated",
             "created",
         ]
         default_columns = [
             "name",
             "address",
             "model",
+            "verify_cert",
             "dynamiclist_count",
         ]
 
 
 class SessionRequestTable(NetBoxTable):
     """SessionRequest list table used in SessionRequestlView."""
```

### Comparing `fwadmin-0.0.2/fwadmin/templates/fwadmin/devicegroup.html` & `fwadmin-0.0.3/fwadmin/templates/fwadmin/devicegroup.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templates/fwadmin/dynamiclist.html` & `fwadmin-0.0.3/fwadmin/templates/fwadmin/dynamiclist.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templates/fwadmin/firewall.html` & `fwadmin-0.0.3/fwadmin/templates/fwadmin/firewall.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templates/fwadmin/htmx/manage_form.html` & `fwadmin-0.0.3/fwadmin/templates/fwadmin/htmx/manage_form.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templates/fwadmin/sessionrequest.html` & `fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html` & `fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templates/fwadmin/sessionrequest_list.html` & `fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_list.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templates/fwadmin/sessionrequest_manage.html` & `fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_manage.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc` & `fwadmin-0.0.3/fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc` & `fwadmin-0.0.3/fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/templatetags/fwadmin_buttons.py` & `fwadmin-0.0.3/fwadmin/templatetags/fwadmin_buttons.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/urls.py` & `fwadmin-0.0.3/fwadmin/urls.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/views.py` & `fwadmin-0.0.3/fwadmin/views.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin/workflows.py` & `fwadmin-0.0.3/fwadmin/workflows.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.2/fwadmin.egg-info/SOURCES.txt` & `fwadmin-0.0.3/fwadmin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 fwadmin/__init__.py
 fwadmin/filtersets.py
 fwadmin/forms.py
 fwadmin/models.py
 fwadmin/navigation.py
 fwadmin/tables.py
+fwadmin/tasks.py
 fwadmin/urls.py
 fwadmin/views.py
 fwadmin/workflows.py
 fwadmin.egg-info/PKG-INFO
 fwadmin.egg-info/SOURCES.txt
 fwadmin.egg-info/dependency_links.txt
 fwadmin.egg-info/not-zip-safe
```

### Comparing `fwadmin-0.0.2/setup.py` & `fwadmin-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,32 +9,28 @@
     twine upload dist/*
 """
 
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 from setuptools import find_packages, setup
 
 setup(
     name="fwadmin",
     version=__version__,
     description="Firewall manager and viewer plugin for Netbox",
     url="https://github.com/dainok/fwadmin",
     author="Andrea Dainese",
     author_email="andrea@adainese.it",
     license="GNU v3.0",
     install_requires=[
-        "django_xworkflows==1.0.0",
-        "netmiko==4.1.2",
-        "nornir==3.3.0",
-        "nornir_netmiko==0.2.0",
-        "nornir_utils",
+        "requests",
     ],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

