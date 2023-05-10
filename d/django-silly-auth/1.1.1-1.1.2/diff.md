# Comparing `tmp/django-silly-auth-1.1.1.tar.gz` & `tmp/django-silly-auth-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-auth-1.1.1.tar", last modified: Mon May  1 16:00:26 2023, max compression
+gzip compressed data, was "django-silly-auth-1.1.2.tar", last modified: Wed May 10 16:18:20 2023, max compression
```

## Comparing `django-silly-auth-1.1.1.tar` & `django-silly-auth-1.1.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.025481 django-silly-auth-1.1.1/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.1.1/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1691 2023-05-01 16:00:26.021481 django-silly-auth-1.1.1/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1081 2023-04-25 13:29:12.000000 django-silly-auth-1.1.1/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:25.993480 django-silly-auth-1.1.1/django_silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-05-01 15:59:59.000000 django-silly-auth-1.1.1/django_silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5786 2023-04-19 16:59:34.000000 django-silly-auth-1.1.1/django_silly_auth/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.1.1/django_silly_auth/forms.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.001480 django-silly-auth-1.1.1/django_silly_auth/locale/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10574 2023-04-14 16:42:40.000000 django-silly-auth-1.1.1/django_silly_auth/locale/django.pot
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:25.985480 django-silly-auth-1.1.1/django_silly_auth/locale/en/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.001480 django-silly-auth-1.1.1/django_silly_auth/locale/en/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.1.1/django_silly_auth/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10588 2023-04-14 16:42:40.000000 django-silly-auth-1.1.1/django_silly_auth/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:25.985480 django-silly-auth-1.1.1/django_silly_auth/locale/fr/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.005480 django-silly-auth-1.1.1/django_silly_auth/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    10088 2023-04-14 16:42:40.000000 django-silly-auth-1.1.1/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    15857 2023-04-14 16:42:40.000000 django-silly-auth-1.1.1/django_silly_auth/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6098 2023-04-19 16:40:47.000000 django-silly-auth-1.1.1/django_silly_auth/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.005480 django-silly-auth-1.1.1/django_silly_auth/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.1.1/django_silly_auth/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.005480 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/_base.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.009481 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/_try/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-14 14:46:10.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/_try/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4478 2023-04-14 14:46:10.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/_try/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-14 14:46:10.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/_try/_single_page.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-14 14:46:10.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/_try/_users.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.013481 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/account.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/change_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/change_username.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/index.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/login.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/reset_password.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/signup.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.017481 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/emails/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/emails/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.017481 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/silly/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/silly/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.017481 django-silly-auth-1.1.1/django_silly_auth/tests/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-14 14:46:10.000000 django-silly-auth-1.1.1/django_silly_auth/tests/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3790 2023-04-14 16:20:53.000000 django-silly-auth-1.1.1/django_silly_auth/tests/test_api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3971 2023-04-14 16:42:40.000000 django-silly-auth-1.1.1/django_silly_auth/tests/test_classic_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1051 2023-04-14 16:42:40.000000 django-silly-auth-1.1.1/django_silly_auth/tests/test_silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5294 2023-04-19 16:59:34.000000 django-silly-auth-1.1.1/django_silly_auth/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3254 2023-04-14 14:46:10.000000 django-silly-auth-1.1.1/django_silly_auth/utils.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.021481 django-silly-auth-1.1.1/django_silly_auth/views/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.1.1/django_silly_auth/views/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3234 2023-05-01 15:59:59.000000 django-silly-auth-1.1.1/django_silly_auth/views/api_custom_login.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      445 2023-04-14 16:42:40.000000 django-silly-auth-1.1.1/django_silly_auth/views/api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6621 2023-04-25 13:29:12.000000 django-silly-auth-1.1.1/django_silly_auth/views/api_views_if_drf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    13683 2023-04-14 16:42:40.000000 django-silly-auth-1.1.1/django_silly_auth/views/classics.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1771 2023-04-14 14:46:10.000000 django-silly-auth-1.1.1/django_silly_auth/views/silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2023-04-14 14:46:10.000000 django-silly-auth-1.1.1/django_silly_auth/views/try_views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-01 16:00:26.001480 django-silly-auth-1.1.1/django_silly_auth.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1691 2023-05-01 16:00:25.000000 django-silly-auth-1.1.1/django_silly_auth.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2464 2023-05-01 16:00:25.000000 django-silly-auth-1.1.1/django_silly_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-05-01 16:00:25.000000 django-silly-auth-1.1.1/django_silly_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-05-01 16:00:25.000000 django-silly-auth-1.1.1/django_silly_auth.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-05-01 16:00:25.000000 django-silly-auth-1.1.1/django_silly_auth.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-05-01 16:00:26.025481 django-silly-auth-1.1.1/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2227 2023-04-19 16:40:47.000000 django-silly-auth-1.1.1/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.707922 django-silly-auth-1.1.2/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.1.2/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1691 2023-05-10 16:18:20.707922 django-silly-auth-1.1.2/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1081 2023-04-25 13:29:12.000000 django-silly-auth-1.1.2/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.687922 django-silly-auth-1.1.2/django_silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-05-10 16:17:25.000000 django-silly-auth-1.1.2/django_silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5781 2023-05-10 16:17:25.000000 django-silly-auth-1.1.2/django_silly_auth/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6302 2023-04-11 19:05:08.000000 django-silly-auth-1.1.2/django_silly_auth/forms.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.691922 django-silly-auth-1.1.2/django_silly_auth/locale/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10574 2023-04-14 16:42:40.000000 django-silly-auth-1.1.2/django_silly_auth/locale/django.pot
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.683921 django-silly-auth-1.1.2/django_silly_auth/locale/en/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.691922 django-silly-auth-1.1.2/django_silly_auth/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      337 2023-04-11 19:05:08.000000 django-silly-auth-1.1.2/django_silly_auth/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10588 2023-04-14 16:42:40.000000 django-silly-auth-1.1.2/django_silly_auth/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.683921 django-silly-auth-1.1.2/django_silly_auth/locale/fr/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.695922 django-silly-auth-1.1.2/django_silly_auth/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10088 2023-04-14 16:42:40.000000 django-silly-auth-1.1.2/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    15857 2023-04-14 16:42:40.000000 django-silly-auth-1.1.2/django_silly_auth/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/mixins.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6098 2023-05-10 16:10:58.000000 django-silly-auth-1.1.2/django_silly_auth/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.695922 django-silly-auth-1.1.2/django_silly_auth/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.1.2/django_silly_auth/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.695922 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/_base.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.695922 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/_try/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-14 14:46:10.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/_try/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4478 2023-04-14 14:46:10.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/_try/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-14 14:46:10.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/_try/_single_page.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-14 14:46:10.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/_try/_users.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.699922 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/account.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/change_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/change_username.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/index.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/login.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/reset_password.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/signup.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.703922 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/emails/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/emails/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.703922 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/silly/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/silly/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      497 2023-04-11 19:05:08.000000 django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.703922 django-silly-auth-1.1.2/django_silly_auth/tests/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-14 14:46:10.000000 django-silly-auth-1.1.2/django_silly_auth/tests/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3790 2023-04-14 16:20:53.000000 django-silly-auth-1.1.2/django_silly_auth/tests/test_api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3971 2023-04-14 16:42:40.000000 django-silly-auth-1.1.2/django_silly_auth/tests/test_classic_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1051 2023-04-14 16:42:40.000000 django-silly-auth-1.1.2/django_silly_auth/tests/test_silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5294 2023-04-19 16:59:34.000000 django-silly-auth-1.1.2/django_silly_auth/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3254 2023-04-14 14:46:10.000000 django-silly-auth-1.1.2/django_silly_auth/utils.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.707922 django-silly-auth-1.1.2/django_silly_auth/views/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.1.2/django_silly_auth/views/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3454 2023-05-10 16:17:25.000000 django-silly-auth-1.1.2/django_silly_auth/views/api_custom_login.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      445 2023-04-14 16:42:40.000000 django-silly-auth-1.1.2/django_silly_auth/views/api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6621 2023-04-25 13:29:12.000000 django-silly-auth-1.1.2/django_silly_auth/views/api_views_if_drf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    13683 2023-04-14 16:42:40.000000 django-silly-auth-1.1.2/django_silly_auth/views/classics.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1771 2023-04-14 14:46:10.000000 django-silly-auth-1.1.2/django_silly_auth/views/silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2023-04-14 14:46:10.000000 django-silly-auth-1.1.2/django_silly_auth/views/try_views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-05-10 16:18:20.691922 django-silly-auth-1.1.2/django_silly_auth.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1691 2023-05-10 16:18:20.000000 django-silly-auth-1.1.2/django_silly_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2464 2023-05-10 16:18:20.000000 django-silly-auth-1.1.2/django_silly_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-05-10 16:18:20.000000 django-silly-auth-1.1.2/django_silly_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-05-10 16:18:20.000000 django-silly-auth-1.1.2/django_silly_auth.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-05-10 16:18:20.000000 django-silly-auth-1.1.2/django_silly_auth.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-05-10 16:18:20.707922 django-silly-auth-1.1.2/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2227 2023-04-19 16:40:47.000000 django-silly-auth-1.1.2/setup.py
```

### Comparing `django-silly-auth-1.1.1/LICENSE.md` & `django-silly-auth-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/PKG-INFO` & `django-silly-auth-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.1.1
+Version: 1.1.2
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
```

### Comparing `django-silly-auth-1.1.1/README.md` & `django-silly-auth-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/config.py` & `django-silly-auth-1.1.2/django_silly_auth/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     # DRF settings
     "USE_DRF": False,  # False for only classic django views
     "CONFIRMATION_METHOD": 'GET',  # 'GET' or 'POST'
     "ALLOW_CREATE_USER_ENDPOINT": True,  # activate this endpoint
     "ALLOW_MY_INFOS_ENDPOINT": True,  # activate this endpoint
     "ALLOW_DELETE_ME_ENDPOINT": True,  # activate this endpoint
-    "USER_INFOS_EXCLUDE": ['password', 'id'],  # fields to exclude from the user infos
+    "USER_INFOS_EXCLUDE": ['password',],  # fields to exclude from the user infos
 
     # pure SPA only:
     "SPA_EMAIL_LOGIN_LINK": "http://your spa address/",  # + <jwt_token>",
 
 
     # Silly settings
     "USE_SILLY": False,
```

### Comparing `django-silly-auth-1.1.1/django_silly_auth/forms.py` & `django-silly-auth-1.1.2/django_silly_auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/locale/django.pot` & `django-silly-auth-1.1.2/django_silly_auth/locale/django.pot`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/locale/en/LC_MESSAGES/django.po` & `django-silly-auth-1.1.2/django_silly_auth/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/locale/fr/LC_MESSAGES/django.mo` & `django-silly-auth-1.1.2/django_silly_auth/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/locale/fr/LC_MESSAGES/django.po` & `django-silly-auth-1.1.2/django_silly_auth/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/mixins.py` & `django-silly-auth-1.1.2/django_silly_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/serializers.py` & `django-silly-auth-1.1.2/django_silly_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/_base.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/_try/_base.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/_try/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/account.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/account.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/change_email.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/change_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/change_username.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/change_username.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/login.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/login.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/request_password_reset.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/request_password_reset.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/reset_password.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/reset_password.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/templates/silly_auth/classic/signup.html` & `django-silly-auth-1.1.2/django_silly_auth/templates/silly_auth/classic/signup.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/tests/test_api_views.py` & `django-silly-auth-1.1.2/django_silly_auth/tests/test_api_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/tests/test_classic_views.py` & `django-silly-auth-1.1.2/django_silly_auth/tests/test_classic_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/tests/test_silly_views.py` & `django-silly-auth-1.1.2/django_silly_auth/tests/test_silly_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/urls.py` & `django-silly-auth-1.1.2/django_silly_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/utils.py` & `django-silly-auth-1.1.2/django_silly_auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/views/api_custom_login.py` & `django-silly-auth-1.1.2/django_silly_auth/views/api_custom_login.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from rest_framework.authtoken.models import Token
 from rest_framework.response import Response
 from rest_framework.authtoken.views import ObtainAuthToken
 from rest_framework.serializers import ValidationError
 
 from django_silly_auth.serializers import (
     LoginSerializer,
-    CredentialJWTokenSerializer
+    CredentialJWTokenSerializer,
+    UserInfosSerializer,
     )
 from django_silly_auth.config import SILLY_AUTH_SETTINGS as conf
 
 if conf["VERBOSE"]:
     print("=== DSA IMPORT django_silly_auth.views.api_custom_login")
 
 User = get_user_model()
@@ -40,19 +41,22 @@
         if match:
             if not user.is_confirmed and not user.is_superuser:
                 msg = _(
                     'Your account has not been confirmed yet. '
                     'Please check your inbox for a confirmation link.')
                 raise ValidationError({'detail': [msg]}, code='authorization')
             token, created = Token.objects.get_or_create(user=user)
-            return Response({
+            serializer = UserInfosSerializer(user)
+            data = {
                 'auth_token': token.key,
-                'username': user.username,
-                'email': user.email,
-                })
+                'user': serializer.data
+            }
+            return Response(
+                data,
+                )
         msg = _('Incorrect credentials.')
         raise ValidationError({'detail': [msg]}, code='authorization')
 
 
 class LoginWithJWTToken(APIView):
     @transaction.atomic
     def post(self, request, *args, **kwargs):
@@ -70,14 +74,18 @@
                 user.new_email = None
                 user.save()
                 msg = _("Your new email has been confirmed.")
             else:
                 msg = _("You've been logged in via email confirmation, "
                         "please change your password if necessary.")
             token, created = Token.objects.get_or_create(user=user)
+            serializer = UserInfosSerializer(user)
+            data = {
+                'auth_token': token.key,
+                'user': serializer.data
+            }
             return Response({
+                'user': serializer.data,
                 'auth_token': token.key,
-                'username': user.username,
-                'email': user.email,
                 'message': msg
                 })
         raise ValidationError(serializer.errors, code='authorization')
```

### Comparing `django-silly-auth-1.1.1/django_silly_auth/views/api_views_if_drf.py` & `django-silly-auth-1.1.2/django_silly_auth/views/api_views_if_drf.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/views/classics.py` & `django-silly-auth-1.1.2/django_silly_auth/views/classics.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/views/silly_views.py` & `django-silly-auth-1.1.2/django_silly_auth/views/silly_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth/views/try_views.py` & `django-silly-auth-1.1.2/django_silly_auth/views/try_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/django_silly_auth.egg-info/PKG-INFO` & `django-silly-auth-1.1.2/django_silly_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.1.1
+Version: 1.1.2
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
```

### Comparing `django-silly-auth-1.1.1/django_silly_auth.egg-info/SOURCES.txt` & `django-silly-auth-1.1.2/django_silly_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.1.1/setup.py` & `django-silly-auth-1.1.2/setup.py`

 * *Files identical despite different names*

