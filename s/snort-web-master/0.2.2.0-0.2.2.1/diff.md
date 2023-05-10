# Comparing `tmp/snort_web_master-0.2.2.0.tar.gz` & `tmp/snort_web_master-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\snort_web_master-0.2.2.0.tar", last modified: Tue May  2 16:53:06 2023, max compression
+gzip compressed data, was "dist\snort_web_master-0.2.2.1.tar", last modified: Wed May 10 06:37:53 2023, max compression
```

## Comparing `snort_web_master-0.2.2.0.tar` & `snort_web_master-0.2.2.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.805821 snort_web_master-0.2.2.0/
--rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-0.2.2.0/LICENSE.rst
--rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-0.2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      251 2023-05-02 16:53:06.805821 snort_web_master-0.2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-0.2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.857864 snort_web_master-0.2.2.0/data/
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.894852 snort_web_master-0.2.2.0/data/admin/
--rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.2.0/data/admin/0004_keyword_delete_keywords.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.912848 snort_web_master-0.2.2.0/data/admin/image/
--rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-0.2.2.0/data/admin/image/images.png
--rw-rw-rw-   0        0        0   241664 2023-01-07 17:05:37.000000 snort_web_master-0.2.2.0/data/db.sqlite3
--rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-0.2.2.0/data/dicts.py
--rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-0.2.2.0/data/dockercompose
--rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-0.2.2.0/data/favicon.ico
--rw-rw-rw-   0        0        0    25803 2023-05-02 11:59:42.000000 snort_web_master-0.2.2.0/data/http.cap
--rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-0.2.2.0/data/migrate sqllite to postgresql
--rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-0.2.2.0/data/my-snort-rule.tmp
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.930860 snort_web_master-0.2.2.0/data/nginx/
--rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-0.2.2.0/data/nginx/nginx
--rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-0.2.2.0/data/nginx/nginx.conf
--rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-0.2.2.0/data/requirements.txt
--rw-rw-rw-   0        0        0      889 2023-05-02 14:51:31.000000 snort_web_master-0.2.2.0/data/snortFile
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.641309 snort_web_master-0.2.2.0/data/templates/
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.064855 snort_web_master-0.2.2.0/data/templates/html/
--rw-rw-rw-   0        0        0     4867 2023-05-02 12:07:14.000000 snort_web_master-0.2.2.0/data/templates/html/full_rule.html
--rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-0.2.2.0/data/templates/html/import.html
--rw-rw-rw-   0        0        0    26921 2023-05-02 05:50:19.000000 snort_web_master-0.2.2.0/data/templates/html/snortBuilder.html
--rw-rw-rw-   0        0        0      140 2023-05-02 16:53:06.807822 snort_web_master-0.2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-05-02 10:13:09.000000 snort_web_master-0.2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:05.646307 snort_web_master-0.2.2.0/snort_web_master/
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.109849 snort_web_master-0.2.2.0/snort_web_master/pcaps/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.225077 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/
--rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0002_initial.py
--rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
--rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/__init__.py
--rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/models.py
--rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/tests.py
--rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.0/snort_web_master/pcaps/views.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.277084 snort_web_master-0.2.2.0/snort_web_master/settings/
--rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.0/snort_web_master/settings/__init__.py
--rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-0.2.2.0/snort_web_master/settings/admin.py
--rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.0/snort_web_master/settings/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.389279 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/
--rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
--rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0003_keywords_avalable.py
--rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
--rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.0/snort_web_master/settings/migrations/__init__.py
--rw-rw-rw-   0        0        0     1444 2023-04-19 07:32:10.000000 snort_web_master-0.2.2.0/snort_web_master/settings/models.py
--rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.0/snort_web_master/settings/tests.py
--rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.0/snort_web_master/settings/views.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.518443 snort_web_master-0.2.2.0/snort_web_master/snort/
--rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-0.2.2.0/snort_web_master/snort/__init__.py
--rw-rw-rw-   0        0        0    31989 2023-05-02 16:50:50.000000 snort_web_master-0.2.2.0/snort_web_master/snort/admin.py
--rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-0.2.2.0/snort_web_master/snort/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.628425 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/
--rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0002_snortruleviewarray.py
--rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
--rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0004_snortrule_deleted.py
--rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
--rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
--rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0007_snortrule_tag.py
--rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.0/snort_web_master/snort/migrations/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-0.2.2.0/snort_web_master/snort/models.py
--rw-rw-rw-   0        0        0    19362 2023-01-12 18:25:18.000000 snort_web_master-0.2.2.0/snort_web_master/snort/parser.py
--rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-0.2.2.0/snort_web_master/snort/snort_templates.py
--rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-0.2.2.0/snort_web_master/snort/tests.py
--rw-rw-rw-   0        0        0     5578 2023-05-02 16:32:07.000000 snort_web_master-0.2.2.0/snort_web_master/snort/views.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.748006 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/
--rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/__init__.py
--rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/asgi.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.803848 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/middleware/
--rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/middleware/__init__.py
--rw-rw-rw-   0        0        0      537 2023-01-09 14:10:56.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/middleware/no_cache.py
--rw-rw-rw-   0        0        0     5515 2023-05-02 07:51:40.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/settings.py
--rw-rw-rw-   0        0        0     1959 2023-04-19 08:14:20.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/urls.py
--rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-05-02 16:53:06.778850 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/
--rw-rw-rw-   0        0        0      251 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3038 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-05-02 16:53:05.000000 snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/
+-rw-rw-rw-   0        0        0       54 2022-11-21 06:29:02.000000 snort_web_master-0.2.2.1/LICENSE.rst
+-rw-rw-rw-   0        0        0       24 2022-11-24 17:54:23.000000 snort_web_master-0.2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      251 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2022-11-21 06:20:44.000000 snort_web_master-0.2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.454203 snort_web_master-0.2.2.1/data/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.470030 snort_web_master-0.2.2.1/data/admin/
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.2.1/data/admin/0004_keyword_delete_keywords.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.485548 snort_web_master-0.2.2.1/data/admin/image/
+-rw-rw-rw-   0        0        0     7972 2023-01-16 16:49:34.000000 snort_web_master-0.2.2.1/data/admin/image/images.png
+-rw-rw-rw-   0        0        0   241664 2023-01-07 17:05:37.000000 snort_web_master-0.2.2.1/data/db.sqlite3
+-rw-rw-rw-   0        0        0    39363 2022-10-13 12:31:39.000000 snort_web_master-0.2.2.1/data/dicts.py
+-rw-rw-rw-   0        0        0      690 2023-01-23 09:10:03.000000 snort_web_master-0.2.2.1/data/dockercompose
+-rw-rw-rw-   0        0        0   139272 2023-01-16 16:50:11.000000 snort_web_master-0.2.2.1/data/favicon.ico
+-rw-rw-rw-   0        0        0    25803 2023-05-02 11:59:42.000000 snort_web_master-0.2.2.1/data/http.cap
+-rw-rw-rw-   0        0        0      898 2023-01-23 08:40:15.000000 snort_web_master-0.2.2.1/data/migrate sqllite to postgresql
+-rw-rw-rw-   0        0        0      402 2022-11-14 09:05:52.000000 snort_web_master-0.2.2.1/data/my-snort-rule.tmp
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.485548 snort_web_master-0.2.2.1/data/nginx/
+-rw-rw-rw-   0        0        0       96 2023-01-23 09:09:18.000000 snort_web_master-0.2.2.1/data/nginx/nginx
+-rw-rw-rw-   0        0        0      296 2023-01-23 09:04:00.000000 snort_web_master-0.2.2.1/data/nginx/nginx.conf
+-rw-rw-rw-   0        0        0      162 2023-01-23 08:44:15.000000 snort_web_master-0.2.2.1/data/requirements.txt
+-rw-rw-rw-   0        0        0      889 2023-05-02 14:51:31.000000 snort_web_master-0.2.2.1/data/snortFile
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.321570 snort_web_master-0.2.2.1/data/templates/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.516693 snort_web_master-0.2.2.1/data/templates/html/
+-rw-rw-rw-   0        0        0     4866 2023-05-10 05:18:00.000000 snort_web_master-0.2.2.1/data/templates/html/full_rule.html
+-rw-rw-rw-   0        0        0      420 2023-01-23 09:19:00.000000 snort_web_master-0.2.2.1/data/templates/html/import.html
+-rw-rw-rw-   0        0        0    27092 2023-05-10 05:24:02.000000 snort_web_master-0.2.2.1/data/templates/html/snortBuilder.html
+-rw-rw-rw-   0        0        0      140 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-05-10 06:33:18.000000 snort_web_master-0.2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.321570 snort_web_master-0.2.2.1/snort_web_master/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.563545 snort_web_master-0.2.2.1/snort_web_master/pcaps/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/__init__.py
+-rw-rw-rw-   0        0        0     2689 2023-01-08 17:50:03.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.610432 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/
+-rw-rw-rw-   0        0        0     1385 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      813 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0      555 2022-12-19 18:24:58.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py
+-rw-rw-rw-   0        0        0      603 2022-12-19 18:25:24.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1060 2022-12-19 18:25:20.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/models.py
+-rw-rw-rw-   0        0        0       63 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/tests.py
+-rw-rw-rw-   0        0        0       66 2022-10-31 09:04:45.000000 snort_web_master-0.2.2.1/snort_web_master/pcaps/views.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.641933 snort_web_master-0.2.2.1/snort_web_master/settings/
+-rw-rw-rw-   0        0        0        0 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.1/snort_web_master/settings/__init__.py
+-rw-rw-rw-   0        0        0      546 2023-04-19 09:25:30.000000 snort_web_master-0.2.2.1/snort_web_master/settings/admin.py
+-rw-rw-rw-   0        0        0      154 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.1/snort_web_master/settings/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.704383 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/
+-rw-rw-rw-   0        0        0     1595 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1350 2022-12-26 06:21:16.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py
+-rw-rw-rw-   0        0        0      530 2022-12-26 06:23:11.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0003_keywords_avalable.py
+-rw-rw-rw-   0        0        0      698 2023-04-19 07:30:34.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py
+-rw-rw-rw-   0        0        0     1268 2023-04-19 09:28:30.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.1/snort_web_master/settings/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-19 07:32:10.000000 snort_web_master-0.2.2.1/snort_web_master/settings/models.py
+-rw-rw-rw-   0        0        0       63 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.1/snort_web_master/settings/tests.py
+-rw-rw-rw-   0        0        0       66 2022-12-19 07:00:41.000000 snort_web_master-0.2.2.1/snort_web_master/settings/views.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.774916 snort_web_master-0.2.2.1/snort_web_master/snort/
+-rw-rw-rw-   0        0        0        0 2022-10-31 09:04:41.000000 snort_web_master-0.2.2.1/snort_web_master/snort/__init__.py
+-rw-rw-rw-   0        0        0    31989 2023-05-02 16:50:50.000000 snort_web_master-0.2.2.1/snort_web_master/snort/admin.py
+-rw-rw-rw-   0        0        0      148 2022-10-31 09:04:41.000000 snort_web_master-0.2.2.1/snort_web_master/snort/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.871046 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/
+-rw-rw-rw-   0        0        0     1974 2022-12-19 18:20:00.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      870 2023-01-05 14:35:56.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0002_snortruleviewarray.py
+-rw-rw-rw-   0        0        0      610 2023-01-06 06:03:56.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py
+-rw-rw-rw-   0        0        0      423 2023-01-06 13:23:29.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0004_snortrule_deleted.py
+-rw-rw-rw-   0        0        0      522 2023-01-08 17:24:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py
+-rw-rw-rw-   0        0        0      759 2023-02-21 08:33:21.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py
+-rw-rw-rw-   0        0        0      477 2023-04-19 09:28:30.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0007_snortrule_tag.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 18:19:43.000000 snort_web_master-0.2.2.1/snort_web_master/snort/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-04-19 09:28:26.000000 snort_web_master-0.2.2.1/snort_web_master/snort/models.py
+-rw-rw-rw-   0        0        0    19362 2023-01-12 18:25:18.000000 snort_web_master-0.2.2.1/snort_web_master/snort/parser.py
+-rw-rw-rw-   0        0        0     2271 2022-12-19 09:13:39.000000 snort_web_master-0.2.2.1/snort_web_master/snort/snort_templates.py
+-rw-rw-rw-   0        0        0     4016 2023-02-21 08:27:30.000000 snort_web_master-0.2.2.1/snort_web_master/snort/tests.py
+-rw-rw-rw-   0        0        0     5996 2023-05-10 05:29:35.000000 snort_web_master-0.2.2.1/snort_web_master/snort/views.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:52.980213 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/
+-rw-rw-rw-   0        0        0        0 2022-11-21 06:23:37.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/__init__.py
+-rw-rw-rw-   0        0        0      425 2022-10-31 09:02:02.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/asgi.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/middleware/
+-rw-rw-rw-   0        0        0        0 2023-01-09 07:35:12.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/middleware/__init__.py
+-rw-rw-rw-   0        0        0      537 2023-01-09 14:10:56.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/middleware/no_cache.py
+-rw-rw-rw-   0        0        0     5515 2023-05-02 07:51:40.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/settings.py
+-rw-rw-rw-   0        0        0     1959 2023-04-19 08:14:20.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/urls.py
+-rw-rw-rw-   0        0        0      425 2023-04-19 08:13:33.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:37:53.011461 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3038 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-05-10 06:37:52.000000 snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/top_level.txt
```

### Comparing `snort_web_master-0.2.2.0/README.md` & `snort_web_master-0.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/admin/0004_keyword_delete_keywords.py` & `snort_web_master-0.2.2.1/data/admin/0004_keyword_delete_keywords.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/admin/image/images.png` & `snort_web_master-0.2.2.1/data/admin/image/images.png`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/db.sqlite3` & `snort_web_master-0.2.2.1/data/db.sqlite3`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/dicts.py` & `snort_web_master-0.2.2.1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/dockercompose` & `snort_web_master-0.2.2.1/data/dockercompose`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/favicon.ico` & `snort_web_master-0.2.2.1/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/http.cap` & `snort_web_master-0.2.2.1/data/http.cap`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/migrate sqllite to postgresql` & `snort_web_master-0.2.2.1/data/migrate sqllite to postgresql`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/snortFile` & `snort_web_master-0.2.2.1/data/snortFile`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/data/templates/html/full_rule.html` & `snort_web_master-0.2.2.1/data/templates/html/full_rule.html`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             {
                 content = content.substring(0, content.length-1) + ': !"' +elem.value + '"';
             }
             else if (elem.id.startsWith("keyword_selection") && elem.id.endsWith("data")){
                  content = content + ': "' +elem.value +'"';
            }
            else{
-               content = content + ': ' +elem.value +'';
+               content = content + ' ' +elem.value +'';
            }
             current_content = content;
         }
         prev = elem;
     }
   if (document.getElementById("id_group")[document.getElementById("id_group").value]!==undefined)
   {
@@ -101,12 +101,12 @@
   else
   {
   group = "";
   }
 
     id_content.value = id_content.textContent=action + ' ' + protocol + ' ' + srcipallow + srcip +' ' +srcportallow+
     srcport + ' ' + direction + ' ' + dstipallow + dstip + ' ' + dstportallow + dstport
-     + '(msg:"' + group + '" ' + name+ ';' + content+ '; sid:' +sigid +'; metadata: employee "'+
+     + '(msg:"' + group + ' ' + name+ '";' + content+ '; sid:' +sigid +'; metadata: employee "'+
      user_name + '", group "' + group + '", name "' + name + '", treatment "' + id_treatment +
       '", keywords "None", date "'+date_now+'", document "' + id_document + '",description "'+id_description+'"; '+id_tag+')';
 };
 </script>
```

### Comparing `snort_web_master-0.2.2.0/data/templates/html/snortBuilder.html` & `snort_web_master-0.2.2.1/data/templates/html/snortBuilder.html`

 * *Files 2% similar despite different names*

```diff
@@ -548,16 +548,20 @@
     var b = document.getElementById(field).onblur
     document.getElementById(field).onchange = undefined
     document.getElementById(field).onblur = undefined
     document.getElementById(field).value = value.trim('"')
     document.getElementById(field).onchange = c
     document.getElementById(field).onblur = b
 }
-
+var first_load = true;
 function content_change(){
+    if (first_load){
+    set_up();
+    first_load = false;
+    }
    var id_content = document.getElementById("id_content");
     postData("/build_rule/keyword_to_rule", {"fule_rule": id_content.value})
     .then((data) =>
     {
         var res_data_post = data
         for (const els of data.data){
             selectElementManual(els.htmlId, els.value.trim('"'), els.typeOfItem, els.locationX, els.locationY);
@@ -614,30 +618,30 @@
 function get_clone_rule(){
     id_content.value = sessionStorage.getItem("snort_content")
     set_content_change()
     while (document.getElementById("id_description")== undefined){
         setTimeout(() => { get_clone_rule();}, 100)
         return;
     }
-    document.getElementById("id_description").value = sessionStorage.getItem("snort_description").trim('"').trim('"');
+    document.getElementById("id_description").value = sessionStorage.getItem("snort_description").replace(/^[\x22\x27]|[\x22\x27]$/g, '');
     while (document.getElementById("id_name")== undefined){
         setTimeout(() => { get_clone_rule();}, 100)
         return;
     }
-    document.getElementById("id_name").value = sessionStorage.getItem("snort_name").trim('"').trim('"');
+    document.getElementById("id_name").value = sessionStorage.getItem("snort_name").replace(/^[\x22\x27]|[\x22\x27]$/g, '');
     while (document.getElementById("id_treatment")== undefined){
         setTimeout(() => { get_clone_rule();}, 100)
         return;
     }
-    document.getElementById("id_treatment").value = sessionStorage.getItem("snort_treatment").trim('"').trim('"');
+    document.getElementById("id_treatment").value = sessionStorage.getItem("snort_treatment").replace(/^[\x22\x27]|[\x22\x27]$/g, '');
     while (document.getElementById("id_document")== undefined){
         setTimeout(() => { get_clone_rule();}, 100)
         return;
     }
-    document.getElementById("id_document").value = sessionStorage.getItem("snort_document").trim('"').trim('"');
+    document.getElementById("id_document").value = sessionStorage.getItem("snort_document").replace(/^[\x22\x27]|[\x22\x27]$/g, '');
 
     sessionStorage.removeItem("snort_content");
     sessionStorage.removeItem("snort_name");
     sessionStorage.removeItem("snort_treatment");
     sessionStorage.removeItem("snort_document");
 }
```

### Comparing `snort_web_master-0.2.2.0/setup.py` & `snort_web_master-0.2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='snort_web_master',
-    version='0.2.2.0',
+    version='0.2.2.1',
     license='MoCorp',
     readme="README.md",
     author="meir dahan",
     author_email='1dahanmeir1@gmail.com',
     packages=find_packages('snort_web_master'),
     package_dir={'': 'snort_web_master'},
     url='https://github.com/mosheovadi1/snort-web-master',
```

### Comparing `snort_web_master-0.2.2.0/snort_web_master/pcaps/admin.py` & `snort_web_master-0.2.2.1/snort_web_master/pcaps/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0001_initial.py` & `snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0002_initial.py` & `snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py` & `snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0003_rename_rule_to_validate_pcap_rule_to_validate2_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py` & `snort_web_master-0.2.2.1/snort_web_master/pcaps/migrations/0004_rename_rule_to_validate2_pcap_rule_to_validate_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/pcaps/models.py` & `snort_web_master-0.2.2.1/snort_web_master/pcaps/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/settings/admin.py` & `snort_web_master-0.2.2.1/snort_web_master/settings/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0001_initial.py` & `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py` & `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0002_remove_keywords_type_keywords_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0003_keywords_avalable.py` & `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0003_keywords_avalable.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py` & `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0004_keyword_delete_keywords.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py` & `snort_web_master-0.2.2.1/snort_web_master/settings/migrations/0005_remove_keyword_negation_alter_keyword_description_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/settings/models.py` & `snort_web_master-0.2.2.1/snort_web_master/settings/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/admin.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/admin.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0001_initial.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0002_snortruleviewarray.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0002_snortruleviewarray.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0003_snortruleviewarray_htmlid_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0005_remove_snortrule_template_snortrule_is_template.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/migrations/0006_rename_main_ref_snortrule_document_and_more.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/models.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/models.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/parser.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/parser.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/snort_templates.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/snort_templates.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/tests.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/tests.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort/views.py` & `snort_web_master-0.2.2.1/snort_web_master/snort/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     return HttpResponse(full_rule)
 
 
 def build_rule_keyword_to_rule(request, full_rule=""):
     if not full_rule:
         full_rule = json.loads(request.body.decode()).get("fule_rule")
     resppnse = {"data": []}
+    if not full_rule:
+        return JsonResponse(resppnse)
     rule_parsed = Parser(full_rule.replace("sid:-;", ""))
     build_keyword_dict(resppnse, rule_parsed)
     return JsonResponse(resppnse)
 
 
 def get_current_user_name(request):
     return JsonResponse({"user": getattr(request.user, request.user.USERNAME_FIELD)})
@@ -78,16 +80,22 @@
             i=0
             if isinstance(op[1], str):
                 op = (op[0], [op[1]])
             for value in op[1]:
                 name = f"keyword_selection{str(op_num)}"
                 if i > 0:
                     name = f"keyword{op_num}-{i-1}"
-                    rule_keywordss.append(build_keyword_item(name, value.split(":")[0].strip().strip('"').strip("'"), x=op_num, y=i-1))
-                    value = value.split(":")[1]
+                    if ":" in value:
+                        rule_keywordss.append(build_keyword_item(name, value.split(":")[0].strip().strip('"').strip("'"), x=op_num, y=i-1))
+                        value = value.split(":")[1]
+                    else:
+                        rule_keywordss.append(
+                            build_keyword_item(name, value.strip().split(" ")[0].strip().strip('"').strip("'"), x=op_num,
+                                               y=i - 1))
+                        value = value.split(" ")[-1]
                     i += 1
                 if value.strip().startswith("!"):
                     rule_keywordss.append(
                         build_keyword_item(f"keyword{str(op_num)}" + "-not", "!", x=op_num, y=0,
                                            item_type="input"))
                     value = value.strip()[1:]
```

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort_web_master/middleware/no_cache.py` & `snort_web_master-0.2.2.1/snort_web_master/snort_web_master/middleware/no_cache.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort_web_master/settings.py` & `snort_web_master-0.2.2.1/snort_web_master/snort_web_master/settings.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort_web_master/urls.py` & `snort_web_master-0.2.2.1/snort_web_master/snort_web_master/urls.py`

 * *Files identical despite different names*

### Comparing `snort_web_master-0.2.2.0/snort_web_master/snort_web_master.egg-info/SOURCES.txt` & `snort_web_master-0.2.2.1/snort_web_master/snort_web_master.egg-info/SOURCES.txt`

 * *Files identical despite different names*

