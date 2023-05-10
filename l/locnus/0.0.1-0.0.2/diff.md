# Comparing `tmp/locnus-0.0.1.tar.gz` & `tmp/locnus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locnus-0.0.1.tar", last modified: Wed May 10 14:12:52 2023, max compression
+gzip compressed data, was "locnus-0.0.2.tar", last modified: Wed May 10 14:21:35 2023, max compression
```

## Comparing `locnus-0.0.1.tar` & `locnus-0.0.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0      167 2023-05-08 08:08:31.714047 locnus-0.0.1/.flake8
--rw-r--r--   0        0        0     3124 2023-05-09 08:52:54.607400 locnus-0.0.1/.gitignore
--rw-r--r--   0        0        0     1262 2023-05-08 08:33:20.081956 locnus-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      628 2023-05-08 08:08:31.714426 locnus-0.0.1/README.md
--rw-r--r--   0        0        0       33 2023-05-10 13:33:27.461993 locnus-0.0.1/additional/tests/test_foo.py
--rw-r--r--   0        0        0      235 2023-05-08 08:08:31.714575 locnus-0.0.1/example/.gitignore
--rw-r--r--   0        0        0      216 2023-05-08 08:08:31.714674 locnus-0.0.1/example/Procfile
--rw-r--r--   0        0        0     5128 2023-05-08 08:08:31.714810 locnus-0.0.1/example/commands.py
--rw-r--r--   0        0        0        0 2023-05-08 08:08:31.714903 locnus-0.0.1/example/config/__init__.py
--rw-r--r--   0        0        0      400 2023-05-08 08:08:31.715021 locnus-0.0.1/example/config/asgi.py
--rw-r--r--   0        0        0        0 2023-05-08 08:08:31.715119 locnus-0.0.1/example/config/settings/__init__.py
--rw-r--r--   0        0        0     4267 2023-05-10 14:04:23.553704 locnus-0.0.1/example/config/settings/base.py
--rw-r--r--   0        0        0      404 2023-05-08 08:08:31.715362 locnus-0.0.1/example/config/settings/development.py
--rw-r--r--   0        0        0      844 2023-05-10 14:04:48.562483 locnus-0.0.1/example/config/settings/production.py
--rw-r--r--   0        0        0      819 2023-05-08 08:08:31.715566 locnus-0.0.1/example/config/settings/test.py
--rw-r--r--   0        0        0      185 2023-05-08 08:08:31.715667 locnus-0.0.1/example/config/urls.py
--rw-r--r--   0        0        0      400 2023-05-08 08:08:31.715753 locnus-0.0.1/example/config/wsgi.py
--rw-r--r--   0        0        0      109 2023-05-08 08:08:31.715898 locnus-0.0.1/example/deploy/ansible.cfg
--rw-r--r--   0        0        0     3572 2023-05-08 08:08:31.716026 locnus-0.0.1/example/deploy/deploy.yml
--rwxr-xr-x   0        0        0      293 2023-05-08 08:08:31.716137 locnus-0.0.1/example/deploy/gunicorn.sh.j2
--rw-r--r--   0        0        0      262 2023-05-10 13:56:29.517913 locnus-0.0.1/example/deploy/inventory/hosts.yml
--rw-r--r--   0        0        0     1123 2023-05-08 08:08:31.716569 locnus-0.0.1/example/deploy/remove.yml
--rw-r--r--   0        0        0      679 2023-05-10 13:56:57.904050 locnus-0.0.1/example/deploy/secrets.yml
--rw-r--r--   0        0        0       31 2023-05-08 08:08:31.716736 locnus-0.0.1/example/deploy/templates/config.fish.template.j2
--rw-r--r--   0        0        0      149 2023-05-10 13:57:23.987855 locnus-0.0.1/example/deploy/templates/env.template.j2
--rwxr-xr-x   0        0        0      195 2023-05-08 08:08:31.716961 locnus-0.0.1/example/deploy/templates/gunicorn.sh.j2
--rw-r--r--   0        0        0      385 2023-05-08 08:08:31.717204 locnus-0.0.1/example/deploy/templates/systemd.service.j2
--rw-r--r--   0        0        0      888 2023-05-08 08:08:31.717321 locnus-0.0.1/example/deploy/templates/traefik.template.j2
--rw-r--r--   0        0        0      214 2023-05-08 08:08:31.717444 locnus-0.0.1/example/deploy/templates/user_config.fish.template.j2
--rw-r--r--   0        0        0      772 2023-05-10 13:55:08.876268 locnus-0.0.1/example/deploy/vars.yml
--rwxr-xr-x   0        0        0      737 2023-05-08 13:32:06.657820 locnus-0.0.1/example/manage.py
--rw-r--r--   0        0        0    46033 2023-05-10 11:35:59.406813 locnus-0.0.1/example/notebooks/create_toots.ipynb
--rw-r--r--   0        0        0     2543 2023-05-10 12:29:27.689622 locnus-0.0.1/example/notebooks/dot_dict.ipynb
--rw-r--r--   0        0        0    18716 2023-05-10 08:35:46.979360 locnus-0.0.1/example/notebooks/login_tests.ipynb
--rw-r--r--   0        0        0     3956 2023-05-09 13:10:57.903067 locnus-0.0.1/example/notebooks/magic_mocks.ipynb
--rw-r--r--   0        0        0     3901 2023-05-09 09:34:55.531505 locnus-0.0.1/example/notebooks/many_to_many.ipynb
--rw-r--r--   0        0        0    12908 2023-05-09 04:05:56.145620 locnus-0.0.1/example/notebooks/save_toots_in_db.ipynb
--rw-r--r--   0        0        0    16383 2023-05-09 09:14:21.217830 locnus-0.0.1/example/notebooks/scratch.ipynb
--rw-r--r--   0        0        0    24588 2023-05-10 10:59:23.572934 locnus-0.0.1/example/notebooks/timelines.ipynb
--rw-r--r--   0        0        0      622 2023-05-08 08:08:31.718924 locnus-0.0.1/example/pyproject.toml
--rw-r--r--   0        0        0      169 2023-05-08 08:08:31.719066 locnus-0.0.1/example/requirements/develop.in
--rw-r--r--   0        0        0    86363 2023-05-08 08:08:31.719725 locnus-0.0.1/example/requirements/develop.txt
--rw-r--r--   0        0        0      138 2023-05-08 08:08:31.720078 locnus-0.0.1/example/requirements/production.in
--rw-r--r--   0        0        0    17937 2023-05-08 08:08:31.720253 locnus-0.0.1/example/requirements/production.txt
--rw-r--r--   0        0        0       71 2023-05-08 08:08:31.720404 locnus-0.0.1/example/static/.gitignore
--rw-r--r--   0        0        0       71 2023-05-08 08:08:31.720567 locnus-0.0.1/example/templates/.gitignore
--rw-r--r--   0        0        0       42 2023-05-10 14:06:22.340179 locnus-0.0.1/locnus/__init__.py
--rw-r--r--   0        0        0      936 2023-05-10 08:55:31.123615 locnus-0.0.1/locnus/admin.py
--rw-r--r--   0        0        0      144 2023-05-08 08:08:31.720866 locnus-0.0.1/locnus/apps.py
--rw-r--r--   0        0        0     1485 2023-05-09 14:23:46.843585 locnus-0.0.1/locnus/forms.py
--rw-r--r--   0        0        0      667 2023-05-10 08:34:37.373575 locnus-0.0.1/locnus/management/commands/import_server_urls.py
--rw-r--r--   0        0        0     3459 2023-05-09 10:33:58.201125 locnus-0.0.1/locnus/migrations/0001_initial.py
--rw-r--r--   0        0        0      412 2023-05-09 12:26:29.335233 locnus-0.0.1/locnus/migrations/0002_alter_timeline_tag.py
--rw-r--r--   0        0        0        0 2023-05-09 09:18:25.046633 locnus-0.0.1/locnus/migrations/__init__.py
--rw-r--r--   0        0        0     4034 2023-05-10 12:43:32.255296 locnus-0.0.1/locnus/models.py
--rw-r--r--   0        0        0       71 2023-05-08 08:08:31.721477 locnus-0.0.1/locnus/static/.gitignore
--rw-r--r--   0        0        0    12551 2023-05-10 13:29:16.335143 locnus-0.0.1/locnus/templates/_base.html
--rw-r--r--   0        0        0     1463 2023-05-08 08:08:31.721822 locnus-0.0.1/locnus/templates/account_detail.html
--rw-r--r--   0        0        0     1646 2023-05-08 08:08:31.721904 locnus-0.0.1/locnus/templates/account_list.html
--rw-r--r--   0        0        0      365 2023-05-08 08:08:31.722003 locnus-0.0.1/locnus/templates/create_account.html
--rw-r--r--   0        0        0      364 2023-05-08 08:08:31.722097 locnus-0.0.1/locnus/templates/create_server.html
--rw-r--r--   0        0        0      362 2023-05-09 14:14:58.673982 locnus-0.0.1/locnus/templates/create_toot.html
--rw-r--r--   0        0        0      292 2023-05-08 08:08:31.722189 locnus-0.0.1/locnus/templates/home.html
--rw-r--r--   0        0        0     2385 2023-05-10 13:29:02.774602 locnus-0.0.1/locnus/templates/server_list.html
--rw-r--r--   0        0        0      886 2023-05-08 08:08:31.722387 locnus-0.0.1/locnus/templates/timeline.html
--rw-r--r--   0        0        0     1417 2023-05-10 12:43:32.721387 locnus-0.0.1/locnus/templates/timeline_partial.html
--rw-r--r--   0        0        0     1123 2023-05-10 13:09:04.919355 locnus-0.0.1/locnus/urls.py
--rw-r--r--   0        0        0     3848 2023-05-10 14:04:23.556064 locnus-0.0.1/locnus/views.py
--rw-r--r--   0        0        0      248 2023-05-08 08:08:31.722756 locnus-0.0.1/manage.py
--rw-r--r--   0        0        0     2442 2023-05-10 13:33:56.698306 locnus-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 08:08:31.723048 locnus-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2434 2023-05-10 12:43:32.384152 locnus-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-09 15:37:34.600769 locnus-0.0.1/tests/examples/__init__.py
--rw-r--r--   0        0        0      481 2023-05-08 10:48:13.066893 locnus-0.0.1/tests/examples/animals.py
--rw-r--r--   0        0        0     1432 2023-05-08 13:56:06.235877 locnus-0.0.1/tests/examples/animals_test.py
--rw-r--r--   0        0        0      619 2023-05-09 15:33:48.739842 locnus-0.0.1/tests/examples/class_test.py
--rw-r--r--   0        0        0      254 2023-05-09 10:29:21.412285 locnus-0.0.1/tests/examples/fixture_test.py
--rw-r--r--   0        0        0      175 2023-05-08 08:55:28.986422 locnus-0.0.1/tests/examples/math_functions.py
--rw-r--r--   0        0        0      742 2023-05-08 13:58:29.554360 locnus-0.0.1/tests/examples/math_functions_test.py
--rw-r--r--   0        0        0      132 2023-05-09 08:51:09.710993 locnus-0.0.1/tests/examples/misc.py
--rw-r--r--   0        0        0      699 2023-05-09 15:43:37.411262 locnus-0.0.1/tests/examples/misc_test.py
--rw-r--r--   0        0        0      649 2023-05-09 10:28:41.750572 locnus-0.0.1/tests/examples/test_file_fixture.py
--rw-r--r--   0        0        0       71 2023-05-08 08:08:31.723298 locnus-0.0.1/tests/files/locnus/static/.gitignore
--rw-r--r--   0        0        0      664 2023-05-09 15:39:50.025796 locnus-0.0.1/tests/forms_test.py
--rw-r--r--   0        0        0      673 2023-05-10 08:34:37.775860 locnus-0.0.1/tests/management_command_test.py
--rw-r--r--   0        0        0     1433 2023-05-09 15:38:37.810402 locnus-0.0.1/tests/mock_test.py
--rw-r--r--   0        0        0     3554 2023-05-10 12:51:51.302853 locnus-0.0.1/tests/models_test.py
--rw-r--r--   0        0        0     4966 2023-05-08 08:08:31.723412 locnus-0.0.1/tests/settings.py
--rw-r--r--   0        0        0      297 2023-05-09 15:29:33.980338 locnus-0.0.1/tests/skipif_test.py
--rw-r--r--   0        0        0     1179 2023-05-09 15:29:33.994371 locnus-0.0.1/tests/tdd_test.py
--rw-r--r--   0        0        0      122 2023-05-08 08:08:31.723490 locnus-0.0.1/tests/urls.py
--rw-r--r--   0        0        0     2816 2023-05-10 14:04:23.557102 locnus-0.0.1/tests/views_test.py
--rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 locnus-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      167 2023-05-08 08:08:31.714047 locnus-0.0.2/.flake8
+-rw-r--r--   0        0        0     3124 2023-05-09 08:52:54.607400 locnus-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1262 2023-05-08 08:33:20.081956 locnus-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      628 2023-05-08 08:08:31.714426 locnus-0.0.2/README.md
+-rw-r--r--   0        0        0       33 2023-05-10 13:33:27.461993 locnus-0.0.2/additional/tests/test_foo.py
+-rw-r--r--   0        0        0      235 2023-05-08 08:08:31.714575 locnus-0.0.2/example/.gitignore
+-rw-r--r--   0        0        0      216 2023-05-08 08:08:31.714674 locnus-0.0.2/example/Procfile
+-rw-r--r--   0        0        0     5128 2023-05-08 08:08:31.714810 locnus-0.0.2/example/commands.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:08:31.714903 locnus-0.0.2/example/config/__init__.py
+-rw-r--r--   0        0        0      400 2023-05-08 08:08:31.715021 locnus-0.0.2/example/config/asgi.py
+-rw-r--r--   0        0        0        0 2023-05-08 08:08:31.715119 locnus-0.0.2/example/config/settings/__init__.py
+-rw-r--r--   0        0        0     4267 2023-05-10 14:04:23.553704 locnus-0.0.2/example/config/settings/base.py
+-rw-r--r--   0        0        0      404 2023-05-08 08:08:31.715362 locnus-0.0.2/example/config/settings/development.py
+-rw-r--r--   0        0        0      844 2023-05-10 14:04:48.562483 locnus-0.0.2/example/config/settings/production.py
+-rw-r--r--   0        0        0      819 2023-05-08 08:08:31.715566 locnus-0.0.2/example/config/settings/test.py
+-rw-r--r--   0        0        0      185 2023-05-08 08:08:31.715667 locnus-0.0.2/example/config/urls.py
+-rw-r--r--   0        0        0      400 2023-05-08 08:08:31.715753 locnus-0.0.2/example/config/wsgi.py
+-rw-r--r--   0        0        0      109 2023-05-08 08:08:31.715898 locnus-0.0.2/example/deploy/ansible.cfg
+-rw-r--r--   0        0        0     3705 2023-05-10 14:17:06.453281 locnus-0.0.2/example/deploy/deploy.yml
+-rwxr-xr-x   0        0        0      293 2023-05-08 08:08:31.716137 locnus-0.0.2/example/deploy/gunicorn.sh.j2
+-rw-r--r--   0        0        0      262 2023-05-10 13:56:29.517913 locnus-0.0.2/example/deploy/inventory/hosts.yml
+-rw-r--r--   0        0        0     1123 2023-05-08 08:08:31.716569 locnus-0.0.2/example/deploy/remove.yml
+-rw-r--r--   0        0        0      679 2023-05-10 13:56:57.904050 locnus-0.0.2/example/deploy/secrets.yml
+-rw-r--r--   0        0        0       31 2023-05-08 08:08:31.716736 locnus-0.0.2/example/deploy/templates/config.fish.template.j2
+-rw-r--r--   0        0        0      149 2023-05-10 13:57:23.987855 locnus-0.0.2/example/deploy/templates/env.template.j2
+-rwxr-xr-x   0        0        0      195 2023-05-08 08:08:31.716961 locnus-0.0.2/example/deploy/templates/gunicorn.sh.j2
+-rw-r--r--   0        0        0      385 2023-05-08 08:08:31.717204 locnus-0.0.2/example/deploy/templates/systemd.service.j2
+-rw-r--r--   0        0        0      888 2023-05-08 08:08:31.717321 locnus-0.0.2/example/deploy/templates/traefik.template.j2
+-rw-r--r--   0        0        0      214 2023-05-08 08:08:31.717444 locnus-0.0.2/example/deploy/templates/user_config.fish.template.j2
+-rw-r--r--   0        0        0      772 2023-05-10 13:55:08.876268 locnus-0.0.2/example/deploy/vars.yml
+-rwxr-xr-x   0        0        0      737 2023-05-08 13:32:06.657820 locnus-0.0.2/example/manage.py
+-rw-r--r--   0        0        0    46033 2023-05-10 11:35:59.406813 locnus-0.0.2/example/notebooks/create_toots.ipynb
+-rw-r--r--   0        0        0     2543 2023-05-10 12:29:27.689622 locnus-0.0.2/example/notebooks/dot_dict.ipynb
+-rw-r--r--   0        0        0    18716 2023-05-10 08:35:46.979360 locnus-0.0.2/example/notebooks/login_tests.ipynb
+-rw-r--r--   0        0        0     3956 2023-05-09 13:10:57.903067 locnus-0.0.2/example/notebooks/magic_mocks.ipynb
+-rw-r--r--   0        0        0     3901 2023-05-09 09:34:55.531505 locnus-0.0.2/example/notebooks/many_to_many.ipynb
+-rw-r--r--   0        0        0    12908 2023-05-09 04:05:56.145620 locnus-0.0.2/example/notebooks/save_toots_in_db.ipynb
+-rw-r--r--   0        0        0    16383 2023-05-09 09:14:21.217830 locnus-0.0.2/example/notebooks/scratch.ipynb
+-rw-r--r--   0        0        0    24588 2023-05-10 10:59:23.572934 locnus-0.0.2/example/notebooks/timelines.ipynb
+-rw-r--r--   0        0        0      622 2023-05-08 08:08:31.718924 locnus-0.0.2/example/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-05-08 08:08:31.719066 locnus-0.0.2/example/requirements/develop.in
+-rw-r--r--   0        0        0    86362 2023-05-10 14:17:36.079786 locnus-0.0.2/example/requirements/develop.txt
+-rw-r--r--   0        0        0      138 2023-05-10 14:17:19.277357 locnus-0.0.2/example/requirements/production.in
+-rw-r--r--   0        0        0    17936 2023-05-10 14:17:38.785623 locnus-0.0.2/example/requirements/production.txt
+-rw-r--r--   0        0        0       71 2023-05-08 08:08:31.720404 locnus-0.0.2/example/static/.gitignore
+-rw-r--r--   0        0        0       71 2023-05-08 08:08:31.720567 locnus-0.0.2/example/templates/.gitignore
+-rw-r--r--   0        0        0       42 2023-05-10 14:20:31.453941 locnus-0.0.2/locnus/__init__.py
+-rw-r--r--   0        0        0      936 2023-05-10 14:14:28.131967 locnus-0.0.2/locnus/admin.py
+-rw-r--r--   0        0        0      144 2023-05-10 14:14:28.132109 locnus-0.0.2/locnus/apps.py
+-rw-r--r--   0        0        0     1485 2023-05-10 14:14:28.132642 locnus-0.0.2/locnus/forms.py
+-rw-r--r--   0        0        0      667 2023-05-10 14:14:28.133416 locnus-0.0.2/locnus/management/commands/import_server_urls.py
+-rw-r--r--   0        0        0     3459 2023-05-10 14:14:28.133880 locnus-0.0.2/locnus/migrations/0001_initial.py
+-rw-r--r--   0        0        0      412 2023-05-10 14:14:28.134111 locnus-0.0.2/locnus/migrations/0002_alter_timeline_tag.py
+-rw-r--r--   0        0        0        0 2023-05-10 14:14:28.134300 locnus-0.0.2/locnus/migrations/__init__.py
+-rw-r--r--   0        0        0     4034 2023-05-10 14:14:28.132814 locnus-0.0.2/locnus/models.py
+-rw-r--r--   0        0        0       71 2023-05-10 14:14:28.134442 locnus-0.0.2/locnus/static/.gitignore
+-rw-r--r--   0        0        0    12551 2023-05-10 14:14:28.134865 locnus-0.0.2/locnus/templates/_base.html
+-rw-r--r--   0        0        0     1463 2023-05-10 14:14:28.134993 locnus-0.0.2/locnus/templates/account_detail.html
+-rw-r--r--   0        0        0     1646 2023-05-10 14:14:28.135115 locnus-0.0.2/locnus/templates/account_list.html
+-rw-r--r--   0        0        0      365 2023-05-10 14:14:28.135235 locnus-0.0.2/locnus/templates/create_account.html
+-rw-r--r--   0        0        0      364 2023-05-10 14:14:28.135566 locnus-0.0.2/locnus/templates/create_server.html
+-rw-r--r--   0        0        0      362 2023-05-10 14:14:28.136007 locnus-0.0.2/locnus/templates/create_toot.html
+-rw-r--r--   0        0        0      292 2023-05-10 14:14:28.136137 locnus-0.0.2/locnus/templates/home.html
+-rw-r--r--   0        0        0     2385 2023-05-10 14:14:28.136304 locnus-0.0.2/locnus/templates/server_list.html
+-rw-r--r--   0        0        0      886 2023-05-10 14:14:28.136431 locnus-0.0.2/locnus/templates/timeline.html
+-rw-r--r--   0        0        0     1417 2023-05-10 14:14:28.136579 locnus-0.0.2/locnus/templates/timeline_partial.html
+-rw-r--r--   0        0        0     1123 2023-05-10 14:14:28.132982 locnus-0.0.2/locnus/urls.py
+-rw-r--r--   0        0        0     3848 2023-05-10 14:14:28.133132 locnus-0.0.2/locnus/views.py
+-rw-r--r--   0        0        0      248 2023-05-08 08:08:31.722756 locnus-0.0.2/manage.py
+-rw-r--r--   0        0        0     2442 2023-05-10 14:20:21.954077 locnus-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 08:08:31.723048 locnus-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     2434 2023-05-10 12:43:32.384152 locnus-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:37:34.600769 locnus-0.0.2/tests/examples/__init__.py
+-rw-r--r--   0        0        0      481 2023-05-08 10:48:13.066893 locnus-0.0.2/tests/examples/animals.py
+-rw-r--r--   0        0        0     1432 2023-05-08 13:56:06.235877 locnus-0.0.2/tests/examples/animals_test.py
+-rw-r--r--   0        0        0      619 2023-05-09 15:33:48.739842 locnus-0.0.2/tests/examples/class_test.py
+-rw-r--r--   0        0        0      254 2023-05-09 10:29:21.412285 locnus-0.0.2/tests/examples/fixture_test.py
+-rw-r--r--   0        0        0      175 2023-05-08 08:55:28.986422 locnus-0.0.2/tests/examples/math_functions.py
+-rw-r--r--   0        0        0      742 2023-05-08 13:58:29.554360 locnus-0.0.2/tests/examples/math_functions_test.py
+-rw-r--r--   0        0        0      132 2023-05-09 08:51:09.710993 locnus-0.0.2/tests/examples/misc.py
+-rw-r--r--   0        0        0      699 2023-05-09 15:43:37.411262 locnus-0.0.2/tests/examples/misc_test.py
+-rw-r--r--   0        0        0      649 2023-05-09 10:28:41.750572 locnus-0.0.2/tests/examples/test_file_fixture.py
+-rw-r--r--   0        0        0       71 2023-05-08 08:08:31.723298 locnus-0.0.2/tests/files/locnus/static/.gitignore
+-rw-r--r--   0        0        0      664 2023-05-09 15:39:50.025796 locnus-0.0.2/tests/forms_test.py
+-rw-r--r--   0        0        0      673 2023-05-10 08:34:37.775860 locnus-0.0.2/tests/management_command_test.py
+-rw-r--r--   0        0        0     1433 2023-05-09 15:38:37.810402 locnus-0.0.2/tests/mock_test.py
+-rw-r--r--   0        0        0     3554 2023-05-10 12:51:51.302853 locnus-0.0.2/tests/models_test.py
+-rw-r--r--   0        0        0     4966 2023-05-08 08:08:31.723412 locnus-0.0.2/tests/settings.py
+-rw-r--r--   0        0        0      297 2023-05-09 15:29:33.980338 locnus-0.0.2/tests/skipif_test.py
+-rw-r--r--   0        0        0     1179 2023-05-09 15:29:33.994371 locnus-0.0.2/tests/tdd_test.py
+-rw-r--r--   0        0        0      122 2023-05-08 08:08:31.723490 locnus-0.0.2/tests/urls.py
+-rw-r--r--   0        0        0     2816 2023-05-10 14:04:23.557102 locnus-0.0.2/tests/views_test.py
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 locnus-0.0.2/PKG-INFO
```

### Comparing `locnus-0.0.1/.gitignore` & `locnus-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/.pre-commit-config.yaml` & `locnus-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/README.md` & `locnus-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/commands.py` & `locnus-0.0.2/example/commands.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/config/settings/base.py` & `locnus-0.0.2/example/config/settings/base.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/config/settings/production.py` & `locnus-0.0.2/example/config/settings/production.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/config/settings/test.py` & `locnus-0.0.2/example/config/settings/test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/deploy/deploy.yml` & `locnus-0.0.2/example/deploy/deploy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,19 @@
     - name: Install app production requirements
       shell: "{{ pip_sync }} requirements/production.txt"
       args:
         chdir: "{{ site_path }}"
       become: true
       become_user: "{{ username }}"
 
+    - name: Install locnus
+      shell: "{{ python }} -m pip install locnus"
+      become: true
+      become_user: "{{ username }}"
+
     - name: Create gunicorn start script
       template:
         src: gunicorn.sh.j2
         dest: "{{ site_path }}/gunicorn.sh"
         owner: "{{ username }}"
         mode: "0755"
```

### Comparing `locnus-0.0.1/example/deploy/remove.yml` & `locnus-0.0.2/example/deploy/remove.yml`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/deploy/secrets.yml` & `locnus-0.0.2/example/deploy/secrets.yml`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/deploy/templates/traefik.template.j2` & `locnus-0.0.2/example/deploy/templates/traefik.template.j2`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/deploy/vars.yml` & `locnus-0.0.2/example/deploy/vars.yml`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/manage.py` & `locnus-0.0.2/example/manage.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/notebooks/create_toots.ipynb` & `locnus-0.0.2/example/notebooks/create_toots.ipynb`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/notebooks/dot_dict.ipynb` & `locnus-0.0.2/example/notebooks/dot_dict.ipynb`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/notebooks/login_tests.ipynb` & `locnus-0.0.2/example/notebooks/login_tests.ipynb`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/notebooks/magic_mocks.ipynb` & `locnus-0.0.2/example/notebooks/magic_mocks.ipynb`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/notebooks/many_to_many.ipynb` & `locnus-0.0.2/example/notebooks/many_to_many.ipynb`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/notebooks/save_toots_in_db.ipynb` & `locnus-0.0.2/example/notebooks/save_toots_in_db.ipynb`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/notebooks/scratch.ipynb` & `locnus-0.0.2/example/notebooks/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/notebooks/timelines.ipynb` & `locnus-0.0.2/example/notebooks/timelines.ipynb`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/pyproject.toml` & `locnus-0.0.2/example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/example/requirements/develop.txt` & `locnus-0.0.2/example/requirements/develop.txt`

 * *Files 0% similar despite different names*

```diff
@@ -123,17 +123,17 @@
     --hash=sha256:7611c1bc41383d2349b6129208587b5d61e8792ce953893cb49c38beeb400d1d \
     --hash=sha256:da56b163e5a816e4ad07172f5639287698e09d7f3dc38d18d9726d9c1dbc4cee
     # via mastodon-py
 build==0.10.0 \
     --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
     --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
     # via pip-tools
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.5.7 \
+    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
+    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
     # via
     #   httpcore
     #   httpx
     #   requests
 cffi==1.15.1 \
     --hash=sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5 \
     --hash=sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef \
@@ -467,17 +467,17 @@
     --hash=sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b \
     --hash=sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a
     # via sphinx
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
-ipykernel==6.22.0 \
-    --hash=sha256:1ae6047c1277508933078163721bbb479c3e7292778a04b4bacf0874550977d6 \
-    --hash=sha256:302558b81f1bc22dc259fb2a0c5c7cf2f4c0bdb21b50484348f7bafe7fb71421
+ipykernel==6.23.0 \
+    --hash=sha256:bd6f487d9e2744c84f6e667d46462d7647a4c862e70e08282f05a52b9d4b705f \
+    --hash=sha256:fc886f1dcdc0ec17f277e4d21fd071c857d381adcb04f3f3735d25325ca323c6
     # via
     #   nbclassic
     #   notebook
 ipython==8.13.2 \
     --hash=sha256:7dff3fad32b97f6488e02f87b970f309d082f758d7b7fc252e3b19ee0e432dbb \
     --hash=sha256:ffca270240fbd21b06b2974e14a86494d6d29290184e788275f55e0b55914926
     # via
@@ -707,17 +707,17 @@
     # via
     #   jupyterlab
     #   notebook
 nbclient==0.7.4 \
     --hash=sha256:c817c0768c5ff0d60e468e017613e6eae27b6fa31e43f905addd2d24df60c125 \
     --hash=sha256:d447f0e5a4cfe79d462459aec1b3dc5c2e9152597262be8ee27f7d4c02566a0d
     # via nbconvert
-nbconvert==7.3.1 \
-    --hash=sha256:78685362b11d2e8058e70196fe83b09abed8df22d3e599cf271f4d39fdc48b9e \
-    --hash=sha256:d2e95904666f1ff77d36105b9de4e0801726f93b862d5b28f69e93d99ad3b19c
+nbconvert==7.4.0 \
+    --hash=sha256:51b6c77b507b177b73f6729dba15676e42c4e92bcb00edc8cc982ee72e7d89d7 \
+    --hash=sha256:af5064a9db524f9f12f4e8be7f0799524bd5b14c1adea37e34e83c95127cc818
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 nbformat==5.8.0 \
     --hash=sha256:46dac64c781f1c34dfd8acba16547024110348f9fc7eab0f31981c2a3dc48d1f \
     --hash=sha256:d910082bd3e0bffcf07eabf3683ed7dda0727a326c446eeb2922abe102e65162
```

### Comparing `locnus-0.0.1/example/requirements/production.txt` & `locnus-0.0.2/example/requirements/production.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     --hash=sha256:71e68008da809b957b7ee4b43dbccff33d1b23519fb8344e33f049897077afac \
     --hash=sha256:9567dfe7bd8d3c8c892227827c41cce860b368104c3431da67a0c5a65a949506
     # via django
 blurhash==1.1.4 \
     --hash=sha256:7611c1bc41383d2349b6129208587b5d61e8792ce953893cb49c38beeb400d1d \
     --hash=sha256:da56b163e5a816e4ad07172f5639287698e09d7f3dc38d18d9726d9c1dbc4cee
     # via mastodon-py
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.5.7 \
+    --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
+    --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0 \
     --hash=sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6 \
     --hash=sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1 \
```

### Comparing `locnus-0.0.1/locnus/admin.py` & `locnus-0.0.2/locnus/admin.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/forms.py` & `locnus-0.0.2/locnus/forms.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/management/commands/import_server_urls.py` & `locnus-0.0.2/locnus/management/commands/import_server_urls.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/migrations/0001_initial.py` & `locnus-0.0.2/locnus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/models.py` & `locnus-0.0.2/locnus/models.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/templates/_base.html` & `locnus-0.0.2/locnus/templates/_base.html`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/templates/account_detail.html` & `locnus-0.0.2/locnus/templates/account_detail.html`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/templates/account_list.html` & `locnus-0.0.2/locnus/templates/account_list.html`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/templates/server_list.html` & `locnus-0.0.2/locnus/templates/server_list.html`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/templates/timeline.html` & `locnus-0.0.2/locnus/templates/timeline.html`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/templates/timeline_partial.html` & `locnus-0.0.2/locnus/templates/timeline_partial.html`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/urls.py` & `locnus-0.0.2/locnus/urls.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/locnus/views.py` & `locnus-0.0.2/locnus/views.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/pyproject.toml` & `locnus-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "locnus"
 authors = [
     {name = "Jochen Wersdörfer", email = "jochen@wersdoerfer.de"},
 ]
 dynamic = ["version", "description"]
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 keywords = [
     "Django",
     "Mastodon",
     "ActivityPub",
     "Fediverse",
 ]
 classifiers = [
```

### Comparing `locnus-0.0.1/tests/conftest.py` & `locnus-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/examples/animals_test.py` & `locnus-0.0.2/tests/examples/animals_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/examples/class_test.py` & `locnus-0.0.2/tests/examples/class_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/examples/math_functions_test.py` & `locnus-0.0.2/tests/examples/math_functions_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/examples/misc_test.py` & `locnus-0.0.2/tests/examples/misc_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/examples/test_file_fixture.py` & `locnus-0.0.2/tests/examples/test_file_fixture.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/forms_test.py` & `locnus-0.0.2/tests/forms_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/management_command_test.py` & `locnus-0.0.2/tests/management_command_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/mock_test.py` & `locnus-0.0.2/tests/mock_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/models_test.py` & `locnus-0.0.2/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/settings.py` & `locnus-0.0.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/tdd_test.py` & `locnus-0.0.2/tests/tdd_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/tests/views_test.py` & `locnus-0.0.2/tests/views_test.py`

 * *Files identical despite different names*

### Comparing `locnus-0.0.1/PKG-INFO` & `locnus-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: locnus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Giant sloth
 Keywords: Django,Mastodon,ActivityPub,Fediverse
 Author-email: Jochen Wersdörfer <jochen@wersdoerfer.de>
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Internet
 Classifier: Development Status :: 3 - Alpha
```

