# Comparing `tmp/garpix_user-3.5.0rc8.tar.gz` & `tmp/garpix_user-3.5.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_user-3.5.0rc8.tar", last modified: Wed Apr 19 13:52:47 2023, max compression
+gzip compressed data, was "garpix_user-3.5.0rc9.tar", last modified: Wed May 10 13:10:11 2023, max compression
```

## Comparing `garpix_user-3.5.0rc8.tar` & `garpix_user-3.5.0rc9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.527492 garpix_user-3.5.0rc8/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-19 13:52:47.527192 garpix_user-3.5.0rc8/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.519347 garpix_user-3.5.0rc8/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4658 2023-04-18 20:25:50.000000 garpix_user-3.5.0rc8/garpix_user/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc8/garpix_user/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9155 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc8/garpix_user/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc8/garpix_user/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.520429 garpix_user-3.5.0rc8/garpix_user/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/admin/referral_type.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.5.0rc8/garpix_user/admin/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/admin/user_session.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc8/garpix_user/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.5.0rc8/garpix_user/exceptions.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.520640 garpix_user-3.5.0rc8/garpix_user/forms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/forms/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      869 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/forms/login.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.516691 garpix_user-3.5.0rc8/garpix_user/locale/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.516744 garpix_user-3.5.0rc8/garpix_user/locale/ru/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.520862 garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6866 2023-04-14 08:29:08.000000 garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9277 2023-04-07 10:32:34.000000 garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.520970 garpix_user-3.5.0rc8/garpix_user/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.521171 garpix_user-3.5.0rc8/garpix_user/mixins/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.521606 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/code_length_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5263 2023-04-19 13:51:11.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/email_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3242 2023-03-07 13:31:03.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/phone_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5436 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc8/garpix_user/mixins/models/restore_password.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.521924 garpix_user-3.5.0rc8/garpix_user/mixins/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/mixins/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc8/garpix_user/mixins/serializers/password_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.5.0rc8/garpix_user/mixins/serializers/to_lower.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.522544 garpix_user-3.5.0rc8/garpix_user/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc8/garpix_user/models/access_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/models/refferal.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc8/garpix_user/models/refresh_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.5.0rc8/garpix_user/models/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4894 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc8/garpix_user/models/user_session.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.522727 garpix_user-3.5.0rc8/garpix_user/rest/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/rest/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-01 07:20:35.000000 garpix_user-3.5.0rc8/garpix_user/rest/authentication.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.523596 garpix_user-3.5.0rc8/garpix_user/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      769 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.5.0rc8/garpix_user/serializers/auth_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/serializers/email_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1418 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc8/garpix_user/serializers/passwrod_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/serializers/phone_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/serializers/refresh_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.5.0rc8/garpix_user/serializers/registration_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.5.0rc8/garpix_user/serializers/user_session_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-19 13:52:41.000000 garpix_user-3.5.0rc8/garpix_user/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.523808 garpix_user-3.5.0rc8/garpix_user/tasks/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc8/garpix_user/tasks/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.5.0rc8/garpix_user/tasks/delete_unconfirmed_users.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.517488 garpix_user-3.5.0rc8/garpix_user/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.523921 garpix_user-3.5.0rc8/garpix_user/templates/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/templates/garpix_user/send_confirm.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.524129 garpix_user-3.5.0rc8/garpix_user/tests/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.524570 garpix_user-3.5.0rc8/garpix_user/tests/test_api/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.524771 garpix_user-3.5.0rc8/garpix_user/tests/test_api/_trial_temp/
--rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/_trial_temp/_trial_marker
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/_trial_temp/test.log
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_login.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_registration.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_user_session_restore_password.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/tests/test_views.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.525072 garpix_user-3.5.0rc8/garpix_user/tests/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/utils/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/tests/utils/test_case_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2581 2023-03-07 13:05:56.000000 garpix_user-3.5.0rc8/garpix_user/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.525710 garpix_user-3.5.0rc8/garpix_user/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc8/garpix_user/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-03-20 15:00:08.000000 garpix_user-3.5.0rc8/garpix_user/utils/backends.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/utils/current_date.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.5.0rc8/garpix_user/utils/drf_spectacular.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/utils/get_token_from_request.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc8/garpix_user/utils/repluralize.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.527016 garpix_user-3.5.0rc8/garpix_user/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/change_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.5.0rc8/garpix_user/views/email_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1401 2023-02-27 12:35:42.000000 garpix_user-3.5.0rc8/garpix_user/views/login_views.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc8/garpix_user/views/logout_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1610 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/obtain_auth_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc8/garpix_user/views/phone_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/referral_links_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.5.0rc8/garpix_user/views/refresh_token_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/registration_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3210 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc8/garpix_user/views/restore_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc8/garpix_user/views/user_session_view.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-19 13:52:47.519997 garpix_user-3.5.0rc8/garpix_user.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3140 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      283 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/garpix_user.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-04-19 13:52:47.527535 garpix_user-3.5.0rc8/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-19 13:52:47.000000 garpix_user-3.5.0rc8/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.329592 garpix_user-3.5.0rc9/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-05-10 13:10:11.000000 garpix_user-3.5.0rc9/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10065 2023-05-10 13:10:11.329245 garpix_user-3.5.0rc9/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.314407 garpix_user-3.5.0rc9/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5007 2023-05-10 13:08:48.000000 garpix_user-3.5.0rc9/garpix_user/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc9/garpix_user/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9398 2023-05-10 13:05:51.000000 garpix_user-3.5.0rc9/garpix_user/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc9/garpix_user/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.316345 garpix_user-3.5.0rc9/garpix_user/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/admin/referral_type.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.5.0rc9/garpix_user/admin/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/admin/user_session.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc9/garpix_user/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.5.0rc9/garpix_user/exceptions.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.316714 garpix_user-3.5.0rc9/garpix_user/forms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/forms/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1009 2023-05-10 09:48:06.000000 garpix_user-3.5.0rc9/garpix_user/forms/login.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.309757 garpix_user-3.5.0rc9/garpix_user/locale/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.309841 garpix_user-3.5.0rc9/garpix_user/locale/ru/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.317119 garpix_user-3.5.0rc9/garpix_user/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6866 2023-04-14 08:29:08.000000 garpix_user-3.5.0rc9/garpix_user/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9277 2023-04-07 10:32:34.000000 garpix_user-3.5.0rc9/garpix_user/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.317316 garpix_user-3.5.0rc9/garpix_user/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.317685 garpix_user-3.5.0rc9/garpix_user/mixins/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/mixins/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.318514 garpix_user-3.5.0rc9/garpix_user/mixins/models/confirm/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/mixins/models/confirm/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.5.0rc9/garpix_user/mixins/models/confirm/code_length_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5477 2023-05-10 13:07:30.000000 garpix_user-3.5.0rc9/garpix_user/mixins/models/confirm/email_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3562 2023-05-10 13:07:30.000000 garpix_user-3.5.0rc9/garpix_user/mixins/models/confirm/phone_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5436 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc9/garpix_user/mixins/models/restore_password.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.319119 garpix_user-3.5.0rc9/garpix_user/mixins/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/mixins/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc9/garpix_user/mixins/serializers/password_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.5.0rc9/garpix_user/mixins/serializers/to_lower.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.320258 garpix_user-3.5.0rc9/garpix_user/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc9/garpix_user/models/access_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/models/refferal.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc9/garpix_user/models/refresh_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.5.0rc9/garpix_user/models/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4986 2023-04-24 07:29:27.000000 garpix_user-3.5.0rc9/garpix_user/models/user_session.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.320605 garpix_user-3.5.0rc9/garpix_user/rest/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/rest/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-01 07:20:35.000000 garpix_user-3.5.0rc9/garpix_user/rest/authentication.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.322338 garpix_user-3.5.0rc9/garpix_user/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      769 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.5.0rc9/garpix_user/serializers/auth_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/serializers/email_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1418 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc9/garpix_user/serializers/passwrod_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/serializers/phone_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/serializers/refresh_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.5.0rc9/garpix_user/serializers/registration_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.5.0rc9/garpix_user/serializers/user_session_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1561 2023-05-10 12:30:22.000000 garpix_user-3.5.0rc9/garpix_user/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.322784 garpix_user-3.5.0rc9/garpix_user/tasks/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc9/garpix_user/tasks/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.5.0rc9/garpix_user/tasks/delete_unconfirmed_users.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.311062 garpix_user-3.5.0rc9/garpix_user/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.322991 garpix_user-3.5.0rc9/garpix_user/templates/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/templates/garpix_user/send_confirm.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.323387 garpix_user-3.5.0rc9/garpix_user/tests/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/tests/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.324183 garpix_user-3.5.0rc9/garpix_user/tests/test_api/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/tests/test_api/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.324545 garpix_user-3.5.0rc9/garpix_user/tests/test_api/_trial_temp/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/tests/test_api/_trial_temp/_trial_marker
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.5.0rc9/garpix_user/tests/test_api/_trial_temp/test.log
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/tests/test_api/api_login.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/tests/test_api/api_registration.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc9/garpix_user/tests/test_api/api_user_session_restore_password.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/tests/test_views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.325076 garpix_user-3.5.0rc9/garpix_user/tests/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/tests/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/tests/utils/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/tests/utils/test_case_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2581 2023-03-07 13:05:56.000000 garpix_user-3.5.0rc9/garpix_user/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.326594 garpix_user-3.5.0rc9/garpix_user/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc9/garpix_user/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-03-20 15:00:08.000000 garpix_user-3.5.0rc9/garpix_user/utils/backends.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/utils/current_date.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.5.0rc9/garpix_user/utils/drf_spectacular.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/utils/get_token_from_request.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc9/garpix_user/utils/repluralize.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.328917 garpix_user-3.5.0rc9/garpix_user/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/views/change_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.5.0rc9/garpix_user/views/email_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1622 2023-05-10 09:48:06.000000 garpix_user-3.5.0rc9/garpix_user/views/login_views.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc9/garpix_user/views/logout_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1610 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/views/obtain_auth_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc9/garpix_user/views/phone_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/views/referral_links_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.5.0rc9/garpix_user/views/refresh_token_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/views/registration_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3326 2023-05-10 09:48:06.000000 garpix_user-3.5.0rc9/garpix_user/views/restore_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc9/garpix_user/views/user_session_view.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 13:10:11.315582 garpix_user-3.5.0rc9/garpix_user.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10065 2023-05-10 13:10:11.000000 garpix_user-3.5.0rc9/garpix_user.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3140 2023-05-10 13:10:11.000000 garpix_user-3.5.0rc9/garpix_user.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-10 13:10:11.000000 garpix_user-3.5.0rc9/garpix_user.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-10 13:10:11.000000 garpix_user-3.5.0rc9/garpix_user.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      279 2023-05-10 13:10:11.000000 garpix_user-3.5.0rc9/garpix_user.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-05-10 13:10:11.000000 garpix_user-3.5.0rc9/garpix_user.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-10 13:10:11.329655 garpix_user-3.5.0rc9/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1561 2023-05-10 13:10:11.000000 garpix_user-3.5.0rc9/setup.py
```

### Comparing `garpix_user-3.5.0rc8/PKG-INFO` & `garpix_user-3.5.0rc9/garpix_user.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: garpix_user
-Version: 3.5.0rc8
+Name: garpix-user
+Version: 3.5.0rc9
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -275,24 +275,26 @@
 ```python
 # settings.py
 
 NOTIFY_EVENTS.update(GARPIX_USER_NOTIFY_EVENTS)
 
 ```
 
-You can specify email and phone code length, lifetime and time delay before next attempt:
+You can specify email and phone code length, lifetime, confirmation lifetime and time delay before next attempt:
 ```python
 #settings.py 
 
 GARPIX_USER = {
     'CONFIRM_PHONE_CODE_LENGTH': 6,
     'CONFIRM_EMAIL_CODE_LENGTH': 6,
     'TIME_LAST_REQUEST': 1,
     'CONFIRM_PHONE_CODE_LIFE_TIME': 5,  # in minutes
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
+    'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
+    'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
 }
 
 # Hint: see all available settings in the end of this document.
 
 ```
 
 Notice: the minimum and maximum values for `CONFIRM_CODE_LENGTH` are 4 and 255. These values will be hard used in case your settings are not in this interval.
@@ -313,31 +315,33 @@
 
 If you need to use email confirmation by link, you need to set corresponding variable:
 ```python
 
 # settings.py
 
 GARPIX_USER = {
-    'USE_EMAIL_LINK_CONFIRMATION': True,
-    'EMAIL_CONFIRMATION_LINK_REDIRECT': '',  # link to the page user needs to see after email confirmation
+    'USE_EMAIL_LINK_CONFIRMATION': True
 }
 
 # Hint: see all available settings in the end of this document.
 
 ```
 
+You can also override `confirm_link_redirect_url` method of `User` model to form confirmation link as you need.
+
 By default, users with unconfirmed email/phone number will be deleted in 10 days. You can set up it using `CONFIRMATION_DELAY`:
 
 ```python
 # settings.py
 
 GARPIX_USER = {
 # ...
     'CONFIRMATION_DELAY': 10,  # in days
 }
+# Hint: see all available settings in the end of this document.
 
 ```
 
 ## Referral links
 
 You can also use referral links in your project with garpix_user. To add this functionality, just add the corresponding settings:
 
@@ -376,20 +380,21 @@
     'REFERRAL_REDIRECT_URL': '/',
     # email/phone confirmation
     'USE_EMAIL_CONFIRMATION': True,
     'USE_PHONE_CONFIRMATION': True,
     'USE_PREREGISTRATION_EMAIL_CONFIRMATION': True,
     'USE_PREREGISTRATION_PHONE_CONFIRMATION': True,
     'USE_EMAIL_LINK_CONFIRMATION': True,
-    'EMAIL_CONFIRMATION_LINK_REDIRECT': '/',
     'CONFIRM_PHONE_CODE_LENGTH': 6,
     'CONFIRM_EMAIL_CODE_LENGTH': 6,
     'TIME_LAST_REQUEST': 1,
     'CONFIRM_PHONE_CODE_LIFE_TIME': 5,  # in minutes
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
+    'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
+    'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
     'CONFIRMATION_DELAY': 10,  # in days
     # restore password
     'USE_RESTORE_PASSWORD': True,
     # registration
     'REGISTRATION_SERIALIZER': 'app.serializers.RegistrationCustSerializer',
     'MIN_LENGTH_PASSWORD': 8,
     'MIN_DIGITS_PASSWORD': 2,
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/CHANGELOG.md` & `garpix_user-3.5.0rc9/garpix_user/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+### 3.5.0 (10.05.2023)
+
+- `delete_unconfirmed_users` celery task added (see `Readme.md`)
+- Authentication errors fixed
+- Localization errors fixed
+- `confirm_link_redirect_url` method added (see `Readme.md`)
+- email/phone confirmation logic fixed
+- `EMAIL_CONFIRMATION_LIFE_TIME` and `PHONE_CONFIRMATION_LIFE_TIME` settings added (see `Readme.md`)
+
 ### 3.4.0 (07.03.2023)
 
 - Release fixes to pypi.org.
 
 ### 3.4.0-rc1-3.4.0-rc4 (01.03.2023)
 
 - Bugs fixed
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/CONTRIBUTING.md` & `garpix_user-3.5.0rc9/garpix_user/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/README.md` & `garpix_user-3.5.0rc9/garpix_user/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -256,24 +256,26 @@
 ```python
 # settings.py
 
 NOTIFY_EVENTS.update(GARPIX_USER_NOTIFY_EVENTS)
 
 ```
 
-You can specify email and phone code length, lifetime and time delay before next attempt:
+You can specify email and phone code length, lifetime, confirmation lifetime and time delay before next attempt:
 ```python
 #settings.py 
 
 GARPIX_USER = {
     'CONFIRM_PHONE_CODE_LENGTH': 6,
     'CONFIRM_EMAIL_CODE_LENGTH': 6,
     'TIME_LAST_REQUEST': 1,
     'CONFIRM_PHONE_CODE_LIFE_TIME': 5,  # in minutes
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
+    'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
+    'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
 }
 
 # Hint: see all available settings in the end of this document.
 
 ```
 
 Notice: the minimum and maximum values for `CONFIRM_CODE_LENGTH` are 4 and 255. These values will be hard used in case your settings are not in this interval.
@@ -294,31 +296,33 @@
 
 If you need to use email confirmation by link, you need to set corresponding variable:
 ```python
 
 # settings.py
 
 GARPIX_USER = {
-    'USE_EMAIL_LINK_CONFIRMATION': True,
-    'EMAIL_CONFIRMATION_LINK_REDIRECT': '',  # link to the page user needs to see after email confirmation
+    'USE_EMAIL_LINK_CONFIRMATION': True
 }
 
 # Hint: see all available settings in the end of this document.
 
 ```
 
+You can also override `confirm_link_redirect_url` method of `User` model to form confirmation link as you need.
+
 By default, users with unconfirmed email/phone number will be deleted in 10 days. You can set up it using `CONFIRMATION_DELAY`:
 
 ```python
 # settings.py
 
 GARPIX_USER = {
 # ...
     'CONFIRMATION_DELAY': 10,  # in days
 }
+# Hint: see all available settings in the end of this document.
 
 ```
 
 ## Referral links
 
 You can also use referral links in your project with garpix_user. To add this functionality, just add the corresponding settings:
 
@@ -357,20 +361,21 @@
     'REFERRAL_REDIRECT_URL': '/',
     # email/phone confirmation
     'USE_EMAIL_CONFIRMATION': True,
     'USE_PHONE_CONFIRMATION': True,
     'USE_PREREGISTRATION_EMAIL_CONFIRMATION': True,
     'USE_PREREGISTRATION_PHONE_CONFIRMATION': True,
     'USE_EMAIL_LINK_CONFIRMATION': True,
-    'EMAIL_CONFIRMATION_LINK_REDIRECT': '/',
     'CONFIRM_PHONE_CODE_LENGTH': 6,
     'CONFIRM_EMAIL_CODE_LENGTH': 6,
     'TIME_LAST_REQUEST': 1,
     'CONFIRM_PHONE_CODE_LIFE_TIME': 5,  # in minutes
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
+    'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
+    'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
     'CONFIRMATION_DELAY': 10,  # in days
     # restore password
     'USE_RESTORE_PASSWORD': True,
     # registration
     'REGISTRATION_SERIALIZER': 'app.serializers.RegistrationCustSerializer',
     'MIN_LENGTH_PASSWORD': 8,
     'MIN_DIGITS_PASSWORD': 2,
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/README.rst` & `garpix_user-3.5.0rc9/garpix_user/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/admin/user.py` & `garpix_user-3.5.0rc9/garpix_user/admin/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/exceptions.py` & `garpix_user-3.5.0rc9/garpix_user/exceptions.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/django.mo` & `garpix_user-3.5.0rc9/garpix_user/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/locale/ru/LC_MESSAGES/django.po` & `garpix_user-3.5.0rc9/garpix_user/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/code_length_mixin.py` & `garpix_user-3.5.0rc9/garpix_user/mixins/models/confirm/code_length_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/email_confirm.py` & `garpix_user-3.5.0rc9/garpix_user/mixins/models/confirm/email_confirm.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     """
     Миксин для подтверждения email
     """
 
     email_confirmation_code = models.CharField(_("Email confirmation code"), max_length=255, blank=True,
                                                null=True)
     email_code_send_date = models.DateTimeField(_("Code sent date"), blank=True, null=True)
+    email_confirmed_date = models.DateTimeField(_("Date email was confirmed"), blank=True, null=True)
     new_email = models.EmailField(_("New email"), blank=True, null=True)
 
     def send_email_confirmation_link(self):
         from garpix_notify.models import Notify
         from garpix_user.models import UserSession
         from django.contrib.auth import get_user_model
 
@@ -88,24 +89,23 @@
 
         if time_is_up:
             return NoTimeLeftException(field='email_confirmation_code')
 
         self.is_email_confirmed = True
         self.email = self.new_email
         self.email_confirmation_code = None
+        self.email_confirmed_date = set_current_date()
         self.save()
         return True
 
     @classmethod
     def confirm_email_by_link(cls, hash):
         from garpix_user.exceptions import IncorrectCodeException, NoTimeLeftException
-        from garpix_user.models import UserSession
 
-        _filter_data = {'is_email_confirmed': False} if isinstance(cls, UserSession) else {}
-        users_list = cls.objects.filter(**_filter_data)
+        users_list = cls.objects.all()
 
         for user in users_list:
             if str(hashlib.sha512(
                     f'{user.email}+{user.email_confirmation_code}'.encode("utf-8")).hexdigest()).lower() == hash:
                 time_is_up = (datetime.now(
                     user.email_code_send_date.tzinfo) - user.email_code_send_date).days > settings.GARPIX_USER.get(
                     'CONFIRM_EMAIL_CODE_LIFE_TIME', 6)
@@ -116,15 +116,17 @@
                 user.email_confirmation_code = None
                 user.save()
                 return True, user
 
         return False, IncorrectCodeException(field='email_confirmation_code')
 
     def check_email_confirmation(self):
-        return self.is_email_confirmed
+        return self.is_email_confirmed and self.email_confirmed_date and self.email_confirmed_date + timedelta(
+                days=settings.GARPIX_USER.get('EMAIL_CONFIRMATION_LIFE_TIME', 2)) >= datetime.now(
+            self.email_confirmed_date.tzinfo)
 
     @classmethod
-    def confirm_link_redirect_url(cls, hash, model_type):
+    def confirm_link_redirect_url(cls, model_type, hash):
         return reverse('garpix_user:email_confirmation_link', args=[model_type, hash])
 
     class Meta:
         abstract = True
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/mixins/models/confirm/phone_confirm.py` & `garpix_user-3.5.0rc9/garpix_user/mixins/models/confirm/phone_confirm.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     """
     Миксин для подтверждения номера телефона
     """
 
     phone_confirmation_code = models.CharField(_('Phone confirmation code'), max_length=15,
                                                blank=True, null=True)
     phone_code_send_date = models.DateTimeField(_("Code sent date"), blank=True, null=True)
+    phone_confirmed_date = models.DateTimeField(_("Date phone was confirmed"), blank=True, null=True)
     new_phone = PhoneNumberField(_("New phone number"), unique=True, blank=True, null=True)
 
     def send_phone_confirmation_code(self, phone=None):
         from garpix_user.exceptions import UserRegisteredException, WaitException
         from garpix_notify.models import Notify
 
         User = get_user_model()
@@ -73,11 +74,13 @@
         self.is_phone_confirmed = True
         self.phone_confirmation_code = None
         self.phone = self.new_phone
         self.save()
         return True
 
     def check_phone_confirmation(self):
-        return self.is_phone_confirmed
+        return self.is_phone_confirmed and self.phone_confirmed_date and self.phone_confirmed_date + timedelta(
+                days=settings.GARPIX_USER.get('PHONE_CONFIRMATION_LIFE_TIME', 2)) >= datetime.now(
+            self.phone_confirmed_date.tzinfo)
 
     class Meta:
         abstract = True
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/mixins/models/restore_password.py` & `garpix_user-3.5.0rc9/garpix_user/mixins/models/restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/mixins/serializers/password_mixin.py` & `garpix_user-3.5.0rc9/garpix_user/mixins/serializers/password_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/models/access_token.py` & `garpix_user-3.5.0rc9/garpix_user/models/access_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/models/refferal.py` & `garpix_user-3.5.0rc9/garpix_user/models/refferal.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/models/refresh_token.py` & `garpix_user-3.5.0rc9/garpix_user/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/models/user.py` & `garpix_user-3.5.0rc9/garpix_user/models/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/models/user_session.py` & `garpix_user-3.5.0rc9/garpix_user/models/user_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,16 @@
             return UserSession.objects.create(
                 user=user,
                 token_number=uuid.uuid4(),
                 recognized=UserSession.UserState.REGISTERED
             )
 
         if session is True:
+            if not request.session.session_key:
+                request.session.cycle_key()
             token = request.session.session_key
             return UserSession.objects.create(
                 token_number=token,
                 recognized=UserSession.UserState.GUEST
             )
 
         if username is not None:
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/rest/authentication.py` & `garpix_user-3.5.0rc9/garpix_user/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/serializers/__init__.py` & `garpix_user-3.5.0rc9/garpix_user/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/serializers/auth_token_serializer.py` & `garpix_user-3.5.0rc9/garpix_user/serializers/auth_token_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/serializers/passwrod_serializer.py` & `garpix_user-3.5.0rc9/garpix_user/serializers/passwrod_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/serializers/registration_serializer.py` & `garpix_user-3.5.0rc9/garpix_user/serializers/registration_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/settings.py` & `garpix_user-3.5.0rc9/garpix_user/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/setup.py` & `garpix_user-3.5.0rc9/garpix_user/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.5.0-rc8',
+    version='3.5.0-rc9',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -34,13 +34,13 @@
     install_requires=[
         'Django >= 3.1, < 4',
         'djangorestframework >= 3.8',
         'django-oauth-toolkit >= 1.1.2',
         'social-auth-app-django >= 2.1.0',
         'social-auth-core == 4.3.0',
         'django-rest-framework-social-oauth2 >= 1.1.0',
-        'django-phonenumber-field-for-garpix_user >= 8.0.0-rc2',
+        'django-phonenumber-field-for-garpix_user >= 8.0.0',
         'garpix-notify >= 5.12.5',
         'garpix-utils >= 1.5.1',
         'drf-spectacular >= 0.24.2'
     ]
 )
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/tasks/delete_unconfirmed_users.py` & `garpix_user-3.5.0rc9/garpix_user/tasks/delete_unconfirmed_users.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_login.py` & `garpix_user-3.5.0rc9/garpix_user/tests/test_api/api_login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_registration.py` & `garpix_user-3.5.0rc9/garpix_user/tests/test_api/api_registration.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/tests/test_api/api_user_session_restore_password.py` & `garpix_user-3.5.0rc9/garpix_user/tests/test_api/api_user_session_restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/tests/test_views.py` & `garpix_user-3.5.0rc9/garpix_user/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/tests/utils/settings.py` & `garpix_user-3.5.0rc9/garpix_user/tests/utils/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/tests/utils/test_case_mixin.py` & `garpix_user-3.5.0rc9/garpix_user/tests/utils/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/urls.py` & `garpix_user-3.5.0rc9/garpix_user/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/utils/backends.py` & `garpix_user-3.5.0rc9/garpix_user/utils/backends.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/utils/repluralize.py` & `garpix_user-3.5.0rc9/garpix_user/utils/repluralize.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/__init__.py` & `garpix_user-3.5.0rc9/garpix_user/views/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/change_password_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/change_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/email_confirmation_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/email_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/login_views.py` & `garpix_user-3.5.0rc9/garpix_user/views/login_views.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,28 +11,35 @@
 class LogoutView(RedirectView):
     def get_redirect_url(self):
         logout(self.request)
         return self.url
 
 
 class LoginView(FormView):
+
+    def get_form_kwargs(self):
+        kwargs = super().get_form_kwargs()
+        if not kwargs.get('data'):
+            kwargs['data'] = json.loads(getattr(self.request, 'body') or b'{}')
+        return kwargs
+
     @staticmethod
     def get_form_class(**kwargs):
         return LoginForm
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         return context
 
     def form_valid(self, form):
         request = self.request
         data = form.data
         username = data.get('username')
         password = data.get('password')
-        user = authenticate(request, username=username, password=password)
+        user = authenticate(request, username=username.lower(), password=password)
         if user:
             user.set_user_session(request)
         login(request, user)
         if self.request.accepts('text/html'):
             return redirect(request.GET.get('next', '/'))
         return JsonResponse({'success': True})
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/logout_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/logout_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/obtain_auth_token.py` & `garpix_user-3.5.0rc9/garpix_user/views/obtain_auth_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/phone_confirmation_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/phone_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/referral_links_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/referral_links_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/refresh_token_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/refresh_token_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/registration_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/registration_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/restore_password_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/restore_password_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from drf_spectacular.utils import extend_schema
-from rest_framework import viewsets
+from rest_framework import viewsets, status
 from rest_framework.decorators import action
 from rest_framework.exceptions import ValidationError
 from rest_framework.response import Response
 from django.utils.translation import ugettext as _
 
 from garpix_user.models import UserSession
 from garpix_user.serializers import RestorePasswordSerializer, RestoreCheckCodeSerializer, RestoreSetPasswordSerializer
@@ -29,30 +29,30 @@
     def send_code(self, request, *args, **kwargs):
         serializer = self.get_serializer_class()(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         user = UserSession.get_from_request(request)
 
         if not user:
-            return Response({"non_field_errors": [_("user-session-token not set")]})
+            return Response({"non_field_errors": [_("user-session-token not set")]}, status=status.HTTP_400_BAD_REQUEST)
 
         result, error = user.send_restore_code(username=serializer.data['username'])
 
         if not result:
             error.raise_exception(exception_class=ValidationError)
         return Response({"result": "success"})
 
     @extend_schema(summary=_('Restore password. Step 2'))
     @action(methods=['POST'], detail=False)
     def check_code(self, request, *args, **kwargs):
 
         user = UserSession.get_from_request(request)
 
         if not user:
-            return Response({"non_field_errors": [_("user-session-token not set")]})
+            return Response({"non_field_errors": [_("user-session-token not set")]}, status=status.HTTP_400_BAD_REQUEST)
 
         serializer = self.get_serializer_class()(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         result, error = user.check_restore_code(
             restore_password_confirm_code=serializer.data['restore_password_confirm_code'])
         if not result:
@@ -62,15 +62,15 @@
     @extend_schema(summary=_('Restore password. Step 3'))
     @action(methods=['POST'], detail=False)
     def set_password(self, request, *args, **kwargs):
 
         user = UserSession.get_from_request(request)
 
         if not user:
-            return Response({"non_field_errors": [_("user-session-token not set")]})
+            return Response({"non_field_errors": [_("user-session-token not set")]}, status=status.HTTP_400_BAD_REQUEST)
 
         serializer = self.get_serializer_class()(data=request.data)
         serializer.is_valid(raise_exception=True)
 
         result, error = user.restore_password(new_password=serializer.data['new_password'],
                                               username=serializer.data['username'],
                                               restore_password_confirm_code=serializer.data[
```

### Comparing `garpix_user-3.5.0rc8/garpix_user/views/user_session_view.py` & `garpix_user-3.5.0rc9/garpix_user/views/user_session_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/garpix_user.egg-info/PKG-INFO` & `garpix_user-3.5.0rc9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: garpix-user
-Version: 3.5.0rc8
+Name: garpix_user
+Version: 3.5.0rc9
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -275,24 +275,26 @@
 ```python
 # settings.py
 
 NOTIFY_EVENTS.update(GARPIX_USER_NOTIFY_EVENTS)
 
 ```
 
-You can specify email and phone code length, lifetime and time delay before next attempt:
+You can specify email and phone code length, lifetime, confirmation lifetime and time delay before next attempt:
 ```python
 #settings.py 
 
 GARPIX_USER = {
     'CONFIRM_PHONE_CODE_LENGTH': 6,
     'CONFIRM_EMAIL_CODE_LENGTH': 6,
     'TIME_LAST_REQUEST': 1,
     'CONFIRM_PHONE_CODE_LIFE_TIME': 5,  # in minutes
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
+    'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
+    'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
 }
 
 # Hint: see all available settings in the end of this document.
 
 ```
 
 Notice: the minimum and maximum values for `CONFIRM_CODE_LENGTH` are 4 and 255. These values will be hard used in case your settings are not in this interval.
@@ -313,31 +315,33 @@
 
 If you need to use email confirmation by link, you need to set corresponding variable:
 ```python
 
 # settings.py
 
 GARPIX_USER = {
-    'USE_EMAIL_LINK_CONFIRMATION': True,
-    'EMAIL_CONFIRMATION_LINK_REDIRECT': '',  # link to the page user needs to see after email confirmation
+    'USE_EMAIL_LINK_CONFIRMATION': True
 }
 
 # Hint: see all available settings in the end of this document.
 
 ```
 
+You can also override `confirm_link_redirect_url` method of `User` model to form confirmation link as you need.
+
 By default, users with unconfirmed email/phone number will be deleted in 10 days. You can set up it using `CONFIRMATION_DELAY`:
 
 ```python
 # settings.py
 
 GARPIX_USER = {
 # ...
     'CONFIRMATION_DELAY': 10,  # in days
 }
+# Hint: see all available settings in the end of this document.
 
 ```
 
 ## Referral links
 
 You can also use referral links in your project with garpix_user. To add this functionality, just add the corresponding settings:
 
@@ -376,20 +380,21 @@
     'REFERRAL_REDIRECT_URL': '/',
     # email/phone confirmation
     'USE_EMAIL_CONFIRMATION': True,
     'USE_PHONE_CONFIRMATION': True,
     'USE_PREREGISTRATION_EMAIL_CONFIRMATION': True,
     'USE_PREREGISTRATION_PHONE_CONFIRMATION': True,
     'USE_EMAIL_LINK_CONFIRMATION': True,
-    'EMAIL_CONFIRMATION_LINK_REDIRECT': '/',
     'CONFIRM_PHONE_CODE_LENGTH': 6,
     'CONFIRM_EMAIL_CODE_LENGTH': 6,
     'TIME_LAST_REQUEST': 1,
     'CONFIRM_PHONE_CODE_LIFE_TIME': 5,  # in minutes
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
+    'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
+    'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
     'CONFIRMATION_DELAY': 10,  # in days
     # restore password
     'USE_RESTORE_PASSWORD': True,
     # registration
     'REGISTRATION_SERIALIZER': 'app.serializers.RegistrationCustSerializer',
     'MIN_LENGTH_PASSWORD': 8,
     'MIN_DIGITS_PASSWORD': 2,
```

### Comparing `garpix_user-3.5.0rc8/garpix_user.egg-info/SOURCES.txt` & `garpix_user-3.5.0rc9/garpix_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc8/setup.py` & `garpix_user-3.5.0rc9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.5.0-rc8',
+    version='3.5.0-rc9',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
@@ -34,13 +34,13 @@
     install_requires=[
         'Django >= 3.1, < 4',
         'djangorestframework >= 3.8',
         'django-oauth-toolkit >= 1.1.2',
         'social-auth-app-django >= 2.1.0',
         'social-auth-core == 4.3.0',
         'django-rest-framework-social-oauth2 >= 1.1.0',
-        'django-phonenumber-field-for-garpix_user >= 8.0.0-rc2',
+        'django-phonenumber-field-for-garpix_user >= 8.0.0',
         'garpix-notify >= 5.12.5',
         'garpix-utils >= 1.5.1',
         'drf-spectacular >= 0.24.2'
     ]
 )
```

