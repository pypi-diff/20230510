# Comparing `tmp/mwgencode-1.3.8.tar.gz` & `tmp/mwgencode-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwgencode-1.3.8.tar", last modified: Wed Mar 22 07:42:32 2023, max compression
+gzip compressed data, was "mwgencode-1.3.9.tar", last modified: Wed May 10 06:49:37 2023, max compression
```

## Comparing `mwgencode-1.3.8.tar` & `mwgencode-1.3.9.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:32.488001 mwgencode-1.3.8/
--rw-rw-rw-   0        0        0     1939 2023-02-21 08:03:13.000000 mwgencode-1.3.8/CHANGES.txt
--rw-rw-rw-   0        0        0     1100 2018-05-07 02:11:24.000000 mwgencode-1.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0      212 2019-09-19 08:10:15.000000 mwgencode-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8084 2023-03-22 07:42:32.484999 mwgencode-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     5229 2020-07-30 10:05:23.000000 mwgencode-1.3.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:31.463001 mwgencode-1.3.8/gencode/
--rw-rw-rw-   0        0        0     5604 2021-01-28 09:01:34.000000 mwgencode-1.3.8/gencode/__init__.py
--rw-rw-rw-   0        0        0     9965 2022-04-27 09:18:21.000000 mwgencode-1.3.8/gencode/dd_models.py
--rw-rw-rw-   0        0        0      657 2018-01-05 11:11:44.000000 mwgencode-1.3.8/gencode/ext.py
--rw-rw-rw-   0        0        0    18399 2023-03-10 06:56:37.000000 mwgencode-1.3.8/gencode/gen_code.py
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:31.527999 mwgencode-1.3.8/gencode/gencode/
--rw-rw-rw-   0        0        0        0 2016-08-19 09:03:33.000000 mwgencode-1.3.8/gencode/gencode/__init__.py
--rw-rw-rw-   0        0        0    10557 2021-01-28 09:01:34.000000 mwgencode-1.3.8/gencode/gencode/export_class2swgclass.py
--rw-rw-rw-   0        0        0    34838 2023-03-17 04:47:36.000000 mwgencode-1.3.8/gencode/gencode/gen_bo_models_code.py
--rw-rw-rw-   0        0        0     8269 2018-01-05 06:32:44.000000 mwgencode-1.3.8/gencode/gencode/gen_state_code.py
--rw-rw-rw-   0        0        0     3739 2022-02-10 09:38:04.000000 mwgencode-1.3.8/gencode/gencode/gen_swagger_code.py
--rw-rw-rw-   0        0        0     4326 2021-01-28 09:48:37.000000 mwgencode-1.3.8/gencode/gencode/gen_tests_code.py
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:31.718003 mwgencode-1.3.8/gencode/gencode/sample/
--rw-rw-rw-   0        0        0        4 2019-08-23 10:00:15.000000 mwgencode-1.3.8/gencode/gencode/sample/__init__.py
--rw-rw-rw-   0        0        0       98 2018-04-13 04:16:45.000000 mwgencode-1.3.8/gencode/gencode/sample/babel.cfg
--rw-rw-rw-   0        0        0      172 2017-08-11 09:14:49.000000 mwgencode-1.3.8/gencode/gencode/sample/config-sample.ini
--rw-rw-rw-   0        0        0      267 2017-12-08 09:02:11.000000 mwgencode-1.3.8/gencode/gencode/sample/config.ini
--rw-rw-rw-   0        0        0      565 2019-09-25 01:00:42.000000 mwgencode-1.3.8/gencode/gencode/sample/create_new_table_run.pys
--rw-rw-rw-   0        0        0      652 2017-08-15 03:32:44.000000 mwgencode-1.3.8/gencode/gencode/sample/dockerignore.dock
--rw-rw-rw-   0        0        0    16379 2023-03-15 08:26:28.000000 mwgencode-1.3.8/gencode/gencode/sample/file_utils.pys
--rw-rw-rw-   0        0        0     2674 2017-06-12 15:42:44.000000 mwgencode-1.3.8/gencode/gencode/sample/gencode.xmi
--rw-rw-rw-   0        0        0      163 2018-11-29 09:33:31.000000 mwgencode-1.3.8/gencode/gencode/sample/gitignore.git
--rwxrwxrwx   0        0        0      100 2018-01-25 07:41:04.000000 mwgencode-1.3.8/gencode/gencode/sample/migrate_run.bat
--rw-rw-rw-   0        0        0      228 2018-01-24 06:10:37.000000 mwgencode-1.3.8/gencode/gencode/sample/migrate_run.pys
--rw-rw-rw-   0        0        0      369 2023-03-08 07:28:57.000000 mwgencode-1.3.8/gencode/gencode/sample/requirements.txt
--rw-rw-rw-   0        0        0     1157 2021-07-22 06:53:29.000000 mwgencode-1.3.8/gencode/gencode/sample/run.sh
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:31.846002 mwgencode-1.3.8/gencode/gencode/sample/seeds/
--rw-rw-rw-   0        0        0        0 2018-03-22 04:04:35.000000 mwgencode-1.3.8/gencode/gencode/sample/seeds/__init__.py
--rw-rw-rw-   0        0        0     7390 2018-04-10 04:26:22.000000 mwgencode-1.3.8/gencode/gencode/sample/seeds/models_rm.pys
--rw-rw-rw-   0        0        0      819 2018-11-06 01:48:16.000000 mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_dev_data.pys
--rw-rw-rw-   0        0        0      530 2018-03-06 16:20:58.000000 mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_init.pys
--rw-rw-rw-   0        0        0     1542 2021-02-02 09:36:29.000000 mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_rm.pys
--rw-rw-rw-   0        0        0      370 2020-06-03 07:25:15.000000 mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_run.pys
--rw-rw-rw-   0        0        0      659 2018-04-13 10:07:34.000000 mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_utils.pys
--rw-rw-rw-   0        0        0      167 2018-01-29 08:16:35.000000 mwgencode-1.3.8/gencode/gencode/sample/test__init__.pys
--rw-rw-rw-   0        0        0       60 2018-01-29 06:49:42.000000 mwgencode-1.3.8/gencode/gencode/sample/test_run.pys
--rw-rw-rw-   0        0        0     2744 2022-02-18 07:16:55.000000 mwgencode-1.3.8/gencode/gencode/sample/utils.pys
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:32.287999 mwgencode-1.3.8/gencode/gencode/template/
--rw-rw-rw-   0        0        0     2414 2022-03-04 07:07:27.000000 mwgencode-1.3.8/gencode/gencode/template/Dockerfile.tmp
--rw-rw-rw-   0        0        0     2008 2022-03-01 02:17:39.000000 mwgencode-1.3.8/gencode/gencode/template/README.md
--rw-rw-rw-   0        0        0        0 2018-03-22 04:04:08.000000 mwgencode-1.3.8/gencode/gencode/template/__init__.py
--rw-rw-rw-   0        0        0     3160 2023-03-06 02:10:35.000000 mwgencode-1.3.8/gencode/gencode/template/__init__.pys
--rw-rw-rw-   0        0        0     5824 2023-03-10 07:06:07.000000 mwgencode-1.3.8/gencode/gencode/template/config.pys
--rw-rw-rw-   0        0        0      484 2021-02-08 02:30:27.000000 mwgencode-1.3.8/gencode/gencode/template/default.conf
--rw-rw-rw-   0        0        0     1945 2021-07-22 06:53:29.000000 mwgencode-1.3.8/gencode/gencode/template/docker-compose-dev.yaml
--rw-rw-rw-   0        0        0     2088 2021-07-22 06:53:29.000000 mwgencode-1.3.8/gencode/gencode/template/docker-compose.yaml
--rw-rw-rw-   0        0        0      964 2023-03-22 03:46:56.000000 mwgencode-1.3.8/gencode/gencode/template/drone.tmp
--rw-rw-rw-   0        0        0     3913 2019-12-18 08:04:03.000000 mwgencode-1.3.8/gencode/gencode/template/flask_models.pys
--rw-rw-rw-   0        0        0     5672 2023-03-17 05:04:56.000000 mwgencode-1.3.8/gencode/gencode/template/flask_models_base.pys
--rw-rw-rw-   0        0        0      304 2020-04-05 10:26:33.000000 mwgencode-1.3.8/gencode/gencode/template/gen_code_flask.yaml
--rw-rw-rw-   0        0        0      593 2019-10-08 07:41:53.000000 mwgencode-1.3.8/gencode/gencode/template/gen_code_run.pys
--rw-rw-rw-   0        0        0     3923 2023-03-10 06:44:52.000000 mwgencode-1.3.8/gencode/gencode/template/k8s-tmp.yml
--rw-rw-rw-   0        0        0     2314 2023-02-21 08:22:49.000000 mwgencode-1.3.8/gencode/gencode/template/run.pys
--rw-rw-rw-   0        0        0    31823 2022-01-10 06:28:08.000000 mwgencode-1.3.8/gencode/gencode/template/sample.mdj
--rw-rw-rw-   0        0        0     2569 2022-03-10 08:33:17.000000 mwgencode-1.3.8/gencode/gencode/template/setup.tmp
--rw-rw-rw-   0        0        0      486 2018-03-15 02:34:00.000000 mwgencode-1.3.8/gencode/gencode/template/supervisord.conf
--rw-rw-rw-   0        0        0     5767 2022-02-10 09:38:04.000000 mwgencode-1.3.8/gencode/gencode/template/swagger_file.yaml
--rw-rw-rw-   0        0        0     1146 2018-01-28 09:39:34.000000 mwgencode-1.3.8/gencode/gencode/template/swg_class.tmp
--rw-rw-rw-   0        0        0     5904 2023-03-08 07:03:38.000000 mwgencode-1.3.8/gencode/gencode/template/swg_ctrl_code.pys
--rw-rw-rw-   0        0        0   140927 2023-03-15 06:27:21.000000 mwgencode-1.3.8/gencode/gencode/template/swg_package_mng.tmp
--rw-rw-rw-   0        0        0     1109 2020-09-16 08:07:21.000000 mwgencode-1.3.8/gencode/gencode/template/test_test_base.tmp
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:32.343000 mwgencode-1.3.8/gencode/gencode/template/tests/
--rw-rw-rw-   0        0        0        0 2018-03-22 04:05:06.000000 mwgencode-1.3.8/gencode/gencode/template/tests/__init__.py
--rw-rw-rw-   0        0        0      151 2018-03-20 06:41:59.000000 mwgencode-1.3.8/gencode/gencode/template/tests/__init__.pys
--rw-rw-rw-   0        0        0     3648 2020-09-16 08:25:02.000000 mwgencode-1.3.8/gencode/gencode/template/tests/init_test_data.pys
--rw-rw-rw-   0        0        0       58 2018-03-20 06:41:59.000000 mwgencode-1.3.8/gencode/gencode/template/tests/run.pys
--rw-rw-rw-   0        0        0     4043 2020-09-16 08:23:15.000000 mwgencode-1.3.8/gencode/gencode/template/tests/test_base.pys
--rw-rw-rw-   0        0        0     2983 2020-09-16 03:09:44.000000 mwgencode-1.3.8/gencode/gencode/template/tests/test_classmng.pys
--rw-rw-rw-   0        0        0      470 2018-11-29 10:13:23.000000 mwgencode-1.3.8/gencode/gencode/template/uwsgi.ini
--rw-rw-rw-   0        0        0     2028 2023-02-21 08:22:49.000000 mwgencode-1.3.8/gencode/gencode/template/uwsgi_run.pys
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:32.378001 mwgencode-1.3.8/gencode/importmdj/
--rw-rw-rw-   0        0        0        0 2018-01-04 03:29:42.000000 mwgencode-1.3.8/gencode/importmdj/__init__.py
--rw-rw-rw-   0        0        0    15530 2022-04-27 09:35:18.000000 mwgencode-1.3.8/gencode/importmdj/import_dd_classes.py
--rw-rw-rw-   0        0        0    16441 2022-02-10 07:59:39.000000 mwgencode-1.3.8/gencode/importmdj/import_swagger2_class.py
--rw-rw-rw-   0        0        0    21223 2021-04-25 09:25:07.000000 mwgencode-1.3.8/gencode/importmdj/import_uml_models.py
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:32.422002 mwgencode-1.3.8/gencode/importxmi/
--rw-rw-rw-   0        0        0       40 2017-05-05 06:37:35.000000 mwgencode-1.3.8/gencode/importxmi/__init__.py
--rw-rw-rw-   0        0        0    14658 2018-01-07 08:37:09.000000 mwgencode-1.3.8/gencode/importxmi/import_classes.py
--rw-rw-rw-   0        0        0     8941 2016-10-27 12:10:06.000000 mwgencode-1.3.8/gencode/importxmi/import_sequences.py
--rw-rw-rw-   0        0        0     5322 2016-09-29 03:48:12.000000 mwgencode-1.3.8/gencode/importxmi/import_states.py
--rw-rw-rw-   0        0        0     6867 2017-12-16 09:27:25.000000 mwgencode-1.3.8/gencode/importxmi/import_swagger.py
--rw-rw-rw-   0        0        0     7723 2022-02-10 05:20:51.000000 mwgencode-1.3.8/gencode/swg2_class_models.py
--rw-rw-rw-   0        0        0    14384 2020-03-23 12:28:49.000000 mwgencode-1.3.8/gencode/uml_class_models.py
--rw-rw-rw-   0        0        0     4423 2023-02-21 09:51:23.000000 mwgencode-1.3.8/gencode/upgrade.py
--rw-rw-rw-   0        0        0     6959 2021-04-26 08:23:54.000000 mwgencode-1.3.8/gencode/utils.py
--rw-rw-rw-   0        0        0     3729 2018-10-30 10:50:17.000000 mwgencode-1.3.8/help.md
--rw-rw-rw-   0        0        0     8707 2023-03-02 04:10:57.000000 mwgencode-1.3.8/manage.py
-drwxrwxrwx   0        0        0        0 2023-03-22 07:42:32.475998 mwgencode-1.3.8/mwgencode.egg-info/
--rw-rw-rw-   0        0        0     8084 2023-03-22 07:42:29.000000 mwgencode-1.3.8/mwgencode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3149 2023-03-22 07:42:30.000000 mwgencode-1.3.8/mwgencode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 07:42:29.000000 mwgencode-1.3.8/mwgencode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-03-22 07:42:29.000000 mwgencode-1.3.8/mwgencode.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      389 2023-03-22 07:42:30.000000 mwgencode-1.3.8/mwgencode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-22 07:42:30.000000 mwgencode-1.3.8/mwgencode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 07:42:32.489000 mwgencode-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2599 2023-03-08 07:09:57.000000 mwgencode-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:37.014849 mwgencode-1.3.9/
+-rw-rw-rw-   0        0        0     1939 2023-02-21 08:03:13.000000 mwgencode-1.3.9/CHANGES.txt
+-rw-rw-rw-   0        0        0     1100 2018-05-07 02:11:24.000000 mwgencode-1.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      212 2019-09-19 08:10:15.000000 mwgencode-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8084 2023-05-10 06:49:37.014849 mwgencode-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5229 2020-07-30 10:05:23.000000 mwgencode-1.3.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:36.469440 mwgencode-1.3.9/gencode/
+-rw-rw-rw-   0        0        0     5604 2021-01-28 09:01:34.000000 mwgencode-1.3.9/gencode/__init__.py
+-rw-rw-rw-   0        0        0     9965 2022-04-27 09:18:21.000000 mwgencode-1.3.9/gencode/dd_models.py
+-rw-rw-rw-   0        0        0      657 2018-01-05 11:11:44.000000 mwgencode-1.3.9/gencode/ext.py
+-rw-rw-rw-   0        0        0    18399 2023-03-10 06:56:37.000000 mwgencode-1.3.9/gencode/gen_code.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:36.503637 mwgencode-1.3.9/gencode/gencode/
+-rw-rw-rw-   0        0        0        0 2016-08-19 09:03:33.000000 mwgencode-1.3.9/gencode/gencode/__init__.py
+-rw-rw-rw-   0        0        0    10557 2021-01-28 09:01:34.000000 mwgencode-1.3.9/gencode/gencode/export_class2swgclass.py
+-rw-rw-rw-   0        0        0    34838 2023-03-17 04:47:36.000000 mwgencode-1.3.9/gencode/gencode/gen_bo_models_code.py
+-rw-rw-rw-   0        0        0     8269 2018-01-05 06:32:44.000000 mwgencode-1.3.9/gencode/gencode/gen_state_code.py
+-rw-rw-rw-   0        0        0     3739 2022-02-10 09:38:04.000000 mwgencode-1.3.9/gencode/gencode/gen_swagger_code.py
+-rw-rw-rw-   0        0        0     4326 2021-01-28 09:48:37.000000 mwgencode-1.3.9/gencode/gencode/gen_tests_code.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:36.632103 mwgencode-1.3.9/gencode/gencode/sample/
+-rw-rw-rw-   0        0        0        4 2019-08-23 10:00:15.000000 mwgencode-1.3.9/gencode/gencode/sample/__init__.py
+-rw-rw-rw-   0        0        0       98 2018-04-13 04:16:45.000000 mwgencode-1.3.9/gencode/gencode/sample/babel.cfg
+-rw-rw-rw-   0        0        0      172 2017-08-11 09:14:49.000000 mwgencode-1.3.9/gencode/gencode/sample/config-sample.ini
+-rw-rw-rw-   0        0        0      267 2017-12-08 09:02:11.000000 mwgencode-1.3.9/gencode/gencode/sample/config.ini
+-rw-rw-rw-   0        0        0      565 2019-09-25 01:00:42.000000 mwgencode-1.3.9/gencode/gencode/sample/create_new_table_run.pys
+-rw-rw-rw-   0        0        0      652 2017-08-15 03:32:44.000000 mwgencode-1.3.9/gencode/gencode/sample/dockerignore.dock
+-rw-rw-rw-   0        0        0    16379 2023-03-15 08:26:28.000000 mwgencode-1.3.9/gencode/gencode/sample/file_utils.pys
+-rw-rw-rw-   0        0        0     2674 2017-06-12 15:42:44.000000 mwgencode-1.3.9/gencode/gencode/sample/gencode.xmi
+-rw-rw-rw-   0        0        0      163 2018-11-29 09:33:31.000000 mwgencode-1.3.9/gencode/gencode/sample/gitignore.git
+-rwxrwxrwx   0        0        0      100 2018-01-25 07:41:04.000000 mwgencode-1.3.9/gencode/gencode/sample/migrate_run.bat
+-rw-rw-rw-   0        0        0      228 2018-01-24 06:10:37.000000 mwgencode-1.3.9/gencode/gencode/sample/migrate_run.pys
+-rw-rw-rw-   0        0        0      368 2023-04-18 07:14:53.000000 mwgencode-1.3.9/gencode/gencode/sample/requirements.txt
+-rw-rw-rw-   0        0        0     1157 2021-07-22 06:53:29.000000 mwgencode-1.3.9/gencode/gencode/sample/run.sh
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:36.678981 mwgencode-1.3.9/gencode/gencode/sample/seeds/
+-rw-rw-rw-   0        0        0        0 2018-03-22 04:04:35.000000 mwgencode-1.3.9/gencode/gencode/sample/seeds/__init__.py
+-rw-rw-rw-   0        0        0     7390 2018-04-10 04:26:22.000000 mwgencode-1.3.9/gencode/gencode/sample/seeds/models_rm.pys
+-rw-rw-rw-   0        0        0      819 2018-11-06 01:48:16.000000 mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_dev_data.pys
+-rw-rw-rw-   0        0        0      530 2018-03-06 16:20:58.000000 mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_init.pys
+-rw-rw-rw-   0        0        0     1542 2021-02-02 09:36:29.000000 mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_rm.pys
+-rw-rw-rw-   0        0        0      370 2020-06-03 07:25:15.000000 mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_run.pys
+-rw-rw-rw-   0        0        0      659 2018-04-13 10:07:34.000000 mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_utils.pys
+-rw-rw-rw-   0        0        0      167 2018-01-29 08:16:35.000000 mwgencode-1.3.9/gencode/gencode/sample/test__init__.pys
+-rw-rw-rw-   0        0        0       60 2018-01-29 06:49:42.000000 mwgencode-1.3.9/gencode/gencode/sample/test_run.pys
+-rw-rw-rw-   0        0        0     2744 2022-02-18 07:16:55.000000 mwgencode-1.3.9/gencode/gencode/sample/utils.pys
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:36.854595 mwgencode-1.3.9/gencode/gencode/template/
+-rw-rw-rw-   0        0        0     2414 2022-03-04 07:07:27.000000 mwgencode-1.3.9/gencode/gencode/template/Dockerfile.tmp
+-rw-rw-rw-   0        0        0     2008 2022-03-01 02:17:39.000000 mwgencode-1.3.9/gencode/gencode/template/README.md
+-rw-rw-rw-   0        0        0        0 2018-03-22 04:04:08.000000 mwgencode-1.3.9/gencode/gencode/template/__init__.py
+-rw-rw-rw-   0        0        0     3160 2023-03-06 02:10:35.000000 mwgencode-1.3.9/gencode/gencode/template/__init__.pys
+-rw-rw-rw-   0        0        0     5824 2023-03-10 07:06:07.000000 mwgencode-1.3.9/gencode/gencode/template/config.pys
+-rw-rw-rw-   0        0        0      484 2021-02-08 02:30:27.000000 mwgencode-1.3.9/gencode/gencode/template/default.conf
+-rw-rw-rw-   0        0        0     1945 2021-07-22 06:53:29.000000 mwgencode-1.3.9/gencode/gencode/template/docker-compose-dev.yaml
+-rw-rw-rw-   0        0        0     2088 2021-07-22 06:53:29.000000 mwgencode-1.3.9/gencode/gencode/template/docker-compose.yaml
+-rw-rw-rw-   0        0        0      964 2023-03-22 03:46:56.000000 mwgencode-1.3.9/gencode/gencode/template/drone.tmp
+-rw-rw-rw-   0        0        0     3913 2019-12-18 08:04:03.000000 mwgencode-1.3.9/gencode/gencode/template/flask_models.pys
+-rw-rw-rw-   0        0        0     5672 2023-03-17 05:04:56.000000 mwgencode-1.3.9/gencode/gencode/template/flask_models_base.pys
+-rw-rw-rw-   0        0        0      304 2020-04-05 10:26:33.000000 mwgencode-1.3.9/gencode/gencode/template/gen_code_flask.yaml
+-rw-rw-rw-   0        0        0      593 2019-10-08 07:41:53.000000 mwgencode-1.3.9/gencode/gencode/template/gen_code_run.pys
+-rw-rw-rw-   0        0        0     3923 2023-03-10 06:44:52.000000 mwgencode-1.3.9/gencode/gencode/template/k8s-tmp.yml
+-rw-rw-rw-   0        0        0     2318 2023-04-17 03:54:24.000000 mwgencode-1.3.9/gencode/gencode/template/run.pys
+-rw-rw-rw-   0        0        0    31823 2022-01-10 06:28:08.000000 mwgencode-1.3.9/gencode/gencode/template/sample.mdj
+-rw-rw-rw-   0        0        0     2569 2022-03-10 08:33:17.000000 mwgencode-1.3.9/gencode/gencode/template/setup.tmp
+-rw-rw-rw-   0        0        0      486 2018-03-15 02:34:00.000000 mwgencode-1.3.9/gencode/gencode/template/supervisord.conf
+-rw-rw-rw-   0        0        0     5767 2022-02-10 09:38:04.000000 mwgencode-1.3.9/gencode/gencode/template/swagger_file.yaml
+-rw-rw-rw-   0        0        0     1146 2018-01-28 09:39:34.000000 mwgencode-1.3.9/gencode/gencode/template/swg_class.tmp
+-rw-rw-rw-   0        0        0     5904 2023-03-08 07:03:38.000000 mwgencode-1.3.9/gencode/gencode/template/swg_ctrl_code.pys
+-rw-rw-rw-   0        0        0   140927 2023-03-15 06:27:21.000000 mwgencode-1.3.9/gencode/gencode/template/swg_package_mng.tmp
+-rw-rw-rw-   0        0        0     1109 2020-09-16 08:07:21.000000 mwgencode-1.3.9/gencode/gencode/template/test_test_base.tmp
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:36.903274 mwgencode-1.3.9/gencode/gencode/template/tests/
+-rw-rw-rw-   0        0        0        0 2018-03-22 04:05:06.000000 mwgencode-1.3.9/gencode/gencode/template/tests/__init__.py
+-rw-rw-rw-   0        0        0      151 2018-03-20 06:41:59.000000 mwgencode-1.3.9/gencode/gencode/template/tests/__init__.pys
+-rw-rw-rw-   0        0        0     3648 2020-09-16 08:25:02.000000 mwgencode-1.3.9/gencode/gencode/template/tests/init_test_data.pys
+-rw-rw-rw-   0        0        0       58 2018-03-20 06:41:59.000000 mwgencode-1.3.9/gencode/gencode/template/tests/run.pys
+-rw-rw-rw-   0        0        0     4043 2020-09-16 08:23:15.000000 mwgencode-1.3.9/gencode/gencode/template/tests/test_base.pys
+-rw-rw-rw-   0        0        0     2983 2020-09-16 03:09:44.000000 mwgencode-1.3.9/gencode/gencode/template/tests/test_classmng.pys
+-rw-rw-rw-   0        0        0      470 2018-11-29 10:13:23.000000 mwgencode-1.3.9/gencode/gencode/template/uwsgi.ini
+-rw-rw-rw-   0        0        0     2028 2023-02-21 08:22:49.000000 mwgencode-1.3.9/gencode/gencode/template/uwsgi_run.pys
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:36.934525 mwgencode-1.3.9/gencode/importmdj/
+-rw-rw-rw-   0        0        0        0 2018-01-04 03:29:42.000000 mwgencode-1.3.9/gencode/importmdj/__init__.py
+-rw-rw-rw-   0        0        0    15530 2022-04-27 09:35:18.000000 mwgencode-1.3.9/gencode/importmdj/import_dd_classes.py
+-rw-rw-rw-   0        0        0    16451 2023-04-13 08:06:03.000000 mwgencode-1.3.9/gencode/importmdj/import_swagger2_class.py
+-rw-rw-rw-   0        0        0    21223 2021-04-25 09:25:07.000000 mwgencode-1.3.9/gencode/importmdj/import_uml_models.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:36.976444 mwgencode-1.3.9/gencode/importxmi/
+-rw-rw-rw-   0        0        0       40 2017-05-05 06:37:35.000000 mwgencode-1.3.9/gencode/importxmi/__init__.py
+-rw-rw-rw-   0        0        0    14658 2018-01-07 08:37:09.000000 mwgencode-1.3.9/gencode/importxmi/import_classes.py
+-rw-rw-rw-   0        0        0     8941 2016-10-27 12:10:06.000000 mwgencode-1.3.9/gencode/importxmi/import_sequences.py
+-rw-rw-rw-   0        0        0     5322 2016-09-29 03:48:12.000000 mwgencode-1.3.9/gencode/importxmi/import_states.py
+-rw-rw-rw-   0        0        0     6867 2017-12-16 09:27:25.000000 mwgencode-1.3.9/gencode/importxmi/import_swagger.py
+-rw-rw-rw-   0        0        0     7723 2022-02-10 05:20:51.000000 mwgencode-1.3.9/gencode/swg2_class_models.py
+-rw-rw-rw-   0        0        0    14384 2020-03-23 12:28:49.000000 mwgencode-1.3.9/gencode/uml_class_models.py
+-rw-rw-rw-   0        0        0     4423 2023-02-21 09:51:23.000000 mwgencode-1.3.9/gencode/upgrade.py
+-rw-rw-rw-   0        0        0     6959 2021-04-26 08:23:54.000000 mwgencode-1.3.9/gencode/utils.py
+-rw-rw-rw-   0        0        0     3729 2018-10-30 10:50:17.000000 mwgencode-1.3.9/help.md
+-rw-rw-rw-   0        0        0     8707 2023-03-02 04:10:57.000000 mwgencode-1.3.9/manage.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:49:37.014849 mwgencode-1.3.9/mwgencode.egg-info/
+-rw-rw-rw-   0        0        0     8084 2023-05-10 06:49:34.000000 mwgencode-1.3.9/mwgencode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3149 2023-05-10 06:49:35.000000 mwgencode-1.3.9/mwgencode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:49:34.000000 mwgencode-1.3.9/mwgencode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-05-10 06:49:34.000000 mwgencode-1.3.9/mwgencode.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      389 2023-05-10 06:49:35.000000 mwgencode-1.3.9/mwgencode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 06:49:35.000000 mwgencode-1.3.9/mwgencode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 06:49:37.014849 mwgencode-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2599 2023-04-13 08:06:43.000000 mwgencode-1.3.9/setup.py
```

### Comparing `mwgencode-1.3.8/CHANGES.txt` & `mwgencode-1.3.9/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/LICENSE.txt` & `mwgencode-1.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/PKG-INFO` & `mwgencode-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwgencode
-Version: 1.3.8
+Version: 1.3.9
 Summary: 根据starUML文档产生flask专案的代码
 Home-page: https://bitbucket.org/maxwin-inc/gencode/src/
 Author: cxhjet
 Author-email: cxhjet@qq.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwgencode-1.3.8/README.rst` & `mwgencode-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/__init__.py` & `mwgencode-1.3.9/gencode/__init__.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/dd_models.py` & `mwgencode-1.3.9/gencode/dd_models.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/ext.py` & `mwgencode-1.3.9/gencode/ext.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gen_code.py` & `mwgencode-1.3.9/gencode/gen_code.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/export_class2swgclass.py` & `mwgencode-1.3.9/gencode/gencode/export_class2swgclass.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/gen_bo_models_code.py` & `mwgencode-1.3.9/gencode/gencode/gen_bo_models_code.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/gen_state_code.py` & `mwgencode-1.3.9/gencode/gencode/gen_state_code.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/gen_swagger_code.py` & `mwgencode-1.3.9/gencode/gencode/gen_swagger_code.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/gen_tests_code.py` & `mwgencode-1.3.9/gencode/gencode/gen_tests_code.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/create_new_table_run.pys` & `mwgencode-1.3.9/gencode/gencode/sample/create_new_table_run.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/dockerignore.dock` & `mwgencode-1.3.9/gencode/gencode/sample/dockerignore.dock`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/file_utils.pys` & `mwgencode-1.3.9/gencode/gencode/sample/file_utils.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/gencode.xmi` & `mwgencode-1.3.9/gencode/gencode/sample/gencode.xmi`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/run.sh` & `mwgencode-1.3.9/gencode/gencode/sample/run.sh`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/seeds/models_rm.pys` & `mwgencode-1.3.9/gencode/gencode/sample/seeds/models_rm.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_dev_data.pys` & `mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_dev_data.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_init.pys` & `mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_init.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_rm.pys` & `mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_rm.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/seeds/seed_utils.pys` & `mwgencode-1.3.9/gencode/gencode/sample/seeds/seed_utils.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/sample/utils.pys` & `mwgencode-1.3.9/gencode/gencode/sample/utils.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/Dockerfile.tmp` & `mwgencode-1.3.9/gencode/gencode/template/Dockerfile.tmp`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/README.md` & `mwgencode-1.3.9/gencode/gencode/template/README.md`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/__init__.pys` & `mwgencode-1.3.9/gencode/gencode/template/__init__.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/config.pys` & `mwgencode-1.3.9/gencode/gencode/template/config.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/docker-compose-dev.yaml` & `mwgencode-1.3.9/gencode/gencode/template/docker-compose-dev.yaml`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/docker-compose.yaml` & `mwgencode-1.3.9/gencode/gencode/template/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/drone.tmp` & `mwgencode-1.3.9/gencode/gencode/template/drone.tmp`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/flask_models.pys` & `mwgencode-1.3.9/gencode/gencode/template/flask_models.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/flask_models_base.pys` & `mwgencode-1.3.9/gencode/gencode/template/flask_models_base.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/gen_code_run.pys` & `mwgencode-1.3.9/gencode/gencode/template/gen_code_run.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/k8s-tmp.yml` & `mwgencode-1.3.9/gencode/gencode/template/k8s-tmp.yml`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/run.pys` & `mwgencode-1.3.9/gencode/gencode/template/run.pys`

 * *Files 0% similar despite different names*

```diff
@@ -40,13 +40,13 @@
                     check=check)
         app.logger.info('注册consul成功')
 
 if __name__ == '__main__':
     app = create_app_swagger('default')
     register_service('default',app.app)
     app.run(host='0.0.0.0')
-    if app.config.get('CONSUL_AUTO_REGISTER'):
+    if app.app.config.get('CONSUL_AUTO_REGISTER'):
         from mwsdk import Kong, dereg_service
         dereg_service('{{swagger.name}}', Kong().port)
```

### Comparing `mwgencode-1.3.8/gencode/gencode/template/sample.mdj` & `mwgencode-1.3.9/gencode/gencode/template/sample.mdj`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/setup.tmp` & `mwgencode-1.3.9/gencode/gencode/template/setup.tmp`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/swagger_file.yaml` & `mwgencode-1.3.9/gencode/gencode/template/swagger_file.yaml`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/swg_class.tmp` & `mwgencode-1.3.9/gencode/gencode/template/swg_class.tmp`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/swg_ctrl_code.pys` & `mwgencode-1.3.9/gencode/gencode/template/swg_ctrl_code.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/swg_package_mng.tmp` & `mwgencode-1.3.9/gencode/gencode/template/swg_package_mng.tmp`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/test_test_base.tmp` & `mwgencode-1.3.9/gencode/gencode/template/test_test_base.tmp`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/tests/init_test_data.pys` & `mwgencode-1.3.9/gencode/gencode/template/tests/init_test_data.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/tests/test_base.pys` & `mwgencode-1.3.9/gencode/gencode/template/tests/test_base.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/tests/test_classmng.pys` & `mwgencode-1.3.9/gencode/gencode/template/tests/test_classmng.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/gencode/template/uwsgi_run.pys` & `mwgencode-1.3.9/gencode/gencode/template/uwsgi_run.pys`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/importmdj/import_dd_classes.py` & `mwgencode-1.3.9/gencode/importmdj/import_dd_classes.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/importmdj/import_swagger2_class.py` & `mwgencode-1.3.9/gencode/importmdj/import_swagger2_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             return 'integer', 'int32'
         elif type == 'long':
             return 'integer', 'int64'
         elif type == 'float':
             return 'number', 'float'
         elif type == 'double':
             return 'number', 'double'
-        elif type == 'string':
+        elif type in ('string','text') :
             return 'string', ''
         elif type == 'byte':
             return 'string', 'byte'
         elif type == 'binary':
             return 'string', 'binary'
         elif type == 'boolean':
             return 'boolean', ''
```

### Comparing `mwgencode-1.3.8/gencode/importmdj/import_uml_models.py` & `mwgencode-1.3.9/gencode/importmdj/import_uml_models.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/importxmi/import_classes.py` & `mwgencode-1.3.9/gencode/importxmi/import_classes.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/importxmi/import_sequences.py` & `mwgencode-1.3.9/gencode/importxmi/import_sequences.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/importxmi/import_states.py` & `mwgencode-1.3.9/gencode/importxmi/import_states.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/importxmi/import_swagger.py` & `mwgencode-1.3.9/gencode/importxmi/import_swagger.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/swg2_class_models.py` & `mwgencode-1.3.9/gencode/swg2_class_models.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/uml_class_models.py` & `mwgencode-1.3.9/gencode/uml_class_models.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/upgrade.py` & `mwgencode-1.3.9/gencode/upgrade.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/gencode/utils.py` & `mwgencode-1.3.9/gencode/utils.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/help.md` & `mwgencode-1.3.9/help.md`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/manage.py` & `mwgencode-1.3.9/manage.py`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/mwgencode.egg-info/PKG-INFO` & `mwgencode-1.3.9/mwgencode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwgencode
-Version: 1.3.8
+Version: 1.3.9
 Summary: 根据starUML文档产生flask专案的代码
 Home-page: https://bitbucket.org/maxwin-inc/gencode/src/
 Author: cxhjet
 Author-email: cxhjet@qq.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwgencode-1.3.8/mwgencode.egg-info/SOURCES.txt` & `mwgencode-1.3.9/mwgencode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwgencode-1.3.8/setup.py` & `mwgencode-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 def read(f):
     return open(os.path.join(os.path.dirname(__file__), f),encoding='utf8').read()
 
 setup(
     name='mwgencode',
-    version='1.3.8',
+    version='1.3.9',
     author='cxhjet',
     author_email='cxhjet@qq.com',
     description="根据starUML文档产生flask专案的代码",
     long_description='\n\n'.join((read('README.rst'), read('CHANGES.txt'))),
     url='https://bitbucket.org/maxwin-inc/gencode/src/',  # Optional
 
     py_modules=['manage'],
```

