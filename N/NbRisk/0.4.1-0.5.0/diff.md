# Comparing `tmp/NbRisk-0.4.1.tar.gz` & `tmp/NbRisk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NbRisk-0.4.1.tar", last modified: Tue Apr 25 01:59:11 2023, max compression
+gzip compressed data, was "NbRisk-0.5.0.tar", last modified: Wed May 10 13:42:12 2023, max compression
```

## Comparing `NbRisk-0.4.1.tar` & `NbRisk-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-25 01:59:11.268916 NbRisk-0.4.1/
--rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-0.4.1/LICENSE
--rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-0.4.1/MANIFEST.in
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-25 01:59:11.104965 NbRisk-0.4.1/NbRisk.egg-info/
--rw-rw-r--   0 renato    (1000) renato    (1000)     3010 2023-04-25 01:59:11.000000 NbRisk-0.4.1/NbRisk.egg-info/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     1471 2023-04-25 01:59:11.000000 NbRisk-0.4.1/NbRisk.egg-info/SOURCES.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-04-25 01:59:11.000000 NbRisk-0.4.1/NbRisk.egg-info/dependency_links.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-04-25 01:59:11.000000 NbRisk-0.4.1/NbRisk.egg-info/top_level.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)     3010 2023-04-25 01:59:11.268916 NbRisk-0.4.1/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2582 2023-04-21 03:01:56.000000 NbRisk-0.4.1/README.md
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-25 01:59:11.108964 NbRisk-0.4.1/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-0.4.1/nb_risk/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-0.4.1/nb_risk/admin.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-25 01:59:11.108964 NbRisk-0.4.1/nb_risk/api/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.4.1/nb_risk/api/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-0.4.1/nb_risk/api/nested_serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5159 2023-04-21 02:18:22.000000 NbRisk-0.4.1/nb_risk/api/serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-0.4.1/nb_risk/api/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-0.4.1/nb_risk/api/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-0.4.1/nb_risk/choices.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-0.4.1/nb_risk/columns.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-0.4.1/nb_risk/cve.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-0.4.1/nb_risk/filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4277 2023-04-21 01:18:06.000000 NbRisk-0.4.1/nb_risk/forms.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.4.1/nb_risk/middleware.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-25 01:59:11.112962 NbRisk-0.4.1/nb_risk/migrations/
--rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-0.4.1/nb_risk/migrations/0001_initial.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-0.4.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-0.4.1/nb_risk/migrations/0003_control.py
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-0.4.1/nb_risk/migrations/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     8480 2023-04-21 01:12:59.000000 NbRisk-0.4.1/nb_risk/models.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3821 2023-04-21 02:14:47.000000 NbRisk-0.4.1/nb_risk/navigation.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.4.1/nb_risk/signals.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3428 2023-04-21 02:43:34.000000 NbRisk-0.4.1/nb_risk/tables.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-0.4.1/nb_risk/template_content.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-25 01:59:11.080972 NbRisk-0.4.1/nb_risk/templates/
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-04-25 01:59:11.268916 NbRisk-0.4.1/nb_risk/templates/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)     1831 2023-04-21 02:45:22.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/control.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      867 2023-04-21 02:58:51.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/control_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      867 2023-04-21 02:45:38.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/control_risks.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/generic_vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/risk.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2211 2023-01-25 20:53:20.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/threatevent.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      505 2023-01-25 20:53:31.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/threatsource.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2837 2023-04-02 19:18:33.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/vulnerability.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      609 2023-04-02 19:20:45.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-0.4.1/nb_risk/templates/nb_risk/vulnerability_search.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     5704 2023-04-21 02:56:21.000000 NbRisk-0.4.1/nb_risk/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       22 2023-04-25 01:56:31.000000 NbRisk-0.4.1/nb_risk/version.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     9823 2023-04-21 02:58:14.000000 NbRisk-0.4.1/nb_risk/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-04-25 01:59:11.268916 NbRisk-0.4.1/setup.cfg
--rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-0.4.1/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:42:12.140889 NbRisk-0.5.0/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-0.5.0/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-0.5.0/MANIFEST.in
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:42:11.876883 NbRisk-0.5.0/NbRisk.egg-info/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3010 2023-05-10 13:42:11.000000 NbRisk-0.5.0/NbRisk.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1526 2023-05-10 13:42:11.000000 NbRisk-0.5.0/NbRisk.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-05-10 13:42:11.000000 NbRisk-0.5.0/NbRisk.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-05-10 13:42:11.000000 NbRisk-0.5.0/NbRisk.egg-info/top_level.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3010 2023-05-10 13:42:12.140889 NbRisk-0.5.0/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2582 2023-04-21 03:01:56.000000 NbRisk-0.5.0/README.md
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:42:11.928884 NbRisk-0.5.0/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-0.5.0/nb_risk/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-0.5.0/nb_risk/admin.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:42:11.948884 NbRisk-0.5.0/nb_risk/api/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.5.0/nb_risk/api/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-0.5.0/nb_risk/api/nested_serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5159 2023-04-21 02:18:22.000000 NbRisk-0.5.0/nb_risk/api/serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-0.5.0/nb_risk/api/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-0.5.0/nb_risk/api/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-0.5.0/nb_risk/choices.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-0.5.0/nb_risk/columns.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-0.5.0/nb_risk/cve.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-0.5.0/nb_risk/filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5051 2023-05-10 12:58:48.000000 NbRisk-0.5.0/nb_risk/forms.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.5.0/nb_risk/middleware.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:42:11.964885 NbRisk-0.5.0/nb_risk/migrations/
+-rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-0.5.0/nb_risk/migrations/0001_initial.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-0.5.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-0.5.0/nb_risk/migrations/0003_control.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-0.5.0/nb_risk/migrations/0004_alter_vulnerability_options.py
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-0.5.0/nb_risk/migrations/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     8511 2023-05-10 12:47:27.000000 NbRisk-0.5.0/nb_risk/models.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-0.5.0/nb_risk/navigation.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-0.5.0/nb_risk/signals.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3428 2023-05-10 13:24:07.000000 NbRisk-0.5.0/nb_risk/tables.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-0.5.0/nb_risk/template_content.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:42:11.844882 NbRisk-0.5.0/nb_risk/templates/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:42:12.128888 NbRisk-0.5.0/nb_risk/templates/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1831 2023-04-21 02:45:22.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/control.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      867 2023-04-21 02:58:51.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/control_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      867 2023-04-21 02:45:38.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/control_risks.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/generic_vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/risk.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2211 2023-01-25 20:53:20.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/threatevent.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      505 2023-01-25 20:53:31.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/threatsource.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2831 2023-05-10 12:31:54.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/vulnerability.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      609 2023-04-02 19:20:45.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-0.5.0/nb_risk/templates/nb_risk/vulnerability_search.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5961 2023-05-10 13:18:51.000000 NbRisk-0.5.0/nb_risk/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       22 2023-05-10 13:39:49.000000 NbRisk-0.5.0/nb_risk/version.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10306 2023-05-10 13:24:11.000000 NbRisk-0.5.0/nb_risk/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-05-10 13:42:12.140889 NbRisk-0.5.0/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-0.5.0/setup.py
```

### Comparing `NbRisk-0.4.1/LICENSE` & `NbRisk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/NbRisk.egg-info/PKG-INFO` & `NbRisk-0.5.0/NbRisk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 0.4.1
+Version: 0.5.0
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-0.4.1/NbRisk.egg-info/SOURCES.txt` & `NbRisk-0.5.0/NbRisk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 nb_risk/api/nested_serializers.py
 nb_risk/api/serializers.py
 nb_risk/api/urls.py
 nb_risk/api/views.py
 nb_risk/migrations/0001_initial.py
 nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
 nb_risk/migrations/0003_control.py
+nb_risk/migrations/0004_alter_vulnerability_options.py
 nb_risk/migrations/__init__.py
 nb_risk/templates/nb_risk/control.html
 nb_risk/templates/nb_risk/control_assets.html
 nb_risk/templates/nb_risk/control_risks.html
 nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
 nb_risk/templates/nb_risk/generic_vulnerability_list.html
 nb_risk/templates/nb_risk/risk.html
```

### Comparing `NbRisk-0.4.1/PKG-INFO` & `NbRisk-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 0.4.1
+Version: 0.5.0
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-0.4.1/README.md` & `NbRisk-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/__init__.py` & `NbRisk-0.5.0/nb_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/api/nested_serializers.py` & `NbRisk-0.5.0/nb_risk/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/api/serializers.py` & `NbRisk-0.5.0/nb_risk/api/serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/api/views.py` & `NbRisk-0.5.0/nb_risk/api/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/choices.py` & `NbRisk-0.5.0/nb_risk/choices.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/columns.py` & `NbRisk-0.5.0/nb_risk/columns.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/cve.py` & `NbRisk-0.5.0/nb_risk/cve.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/filters.py` & `NbRisk-0.5.0/nb_risk/filters.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/forms.py` & `NbRisk-0.5.0/nb_risk/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django import forms
 
-from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm
+from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelImportForm
 from dcim.models import Device, DeviceType
 from virtualization.models import VirtualMachine
 
 from utilities.forms import (
     BootstrapMixin,
     DatePicker,
     CommentField,
@@ -77,14 +77,19 @@
         ]
 
 
 # Vulnerability Forms
 
 
 class VulnerabilityForm(NetBoxModelForm):
+
+    fieldsets = (
+        ("Vulnerability", ("name", "cve", "description", "notes"),),
+        ("CVSSv2 Score", ("cvssaccessVector", "cvssaccessComplexity", "cvssauthentication", "cvssconfidentialityImpact", "cvssintegrityImpact", "cvssavailabilityImpact", "cvssbaseScore")),
+    )
     class Meta:
         model = models.Vulnerability
         fields = [
             "name",
             "cve",
             "description",
             "notes",
@@ -116,14 +121,30 @@
     version = forms.CharField(required=False)
 
     part = forms.ChoiceField(
         choices=choices.CVE_PART_CHOICES,
         required=False,
     )
 
+class VulnerabilityImportForm(NetBoxModelImportForm):
+    class Meta:
+        model = models.Vulnerability
+        fields = [
+            "name",
+            "cve",
+            "description",
+            "notes",
+            "cvssaccessVector",
+            "cvssaccessComplexity",
+            "cvssauthentication",
+            "cvssconfidentialityImpact",
+            "cvssintegrityImpact",
+            "cvssavailabilityImpact",
+            "cvssbaseScore",
+        ]
 
 # VulnerabilityAssignment Forms
 
 
 class VulnerabilityAssignmentForm(BootstrapMixin, forms.ModelForm):
 
     vulnerability = DynamicModelChoiceField(
```

### Comparing `NbRisk-0.4.1/nb_risk/migrations/0001_initial.py` & `NbRisk-0.5.0/nb_risk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py` & `NbRisk-0.5.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/migrations/0003_control.py` & `NbRisk-0.5.0/nb_risk/migrations/0003_control.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/models.py` & `NbRisk-0.5.0/nb_risk/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,44 +42,45 @@
 class Vulnerability(NetBoxModel):
 
     name = models.CharField("Name", max_length=100, unique=True)
     cve = models.CharField("CVE", max_length=100, blank=True)
     description = models.CharField("Description", max_length=100, blank=True)
     notes = models.TextField("Notes", blank=True)
     cvssaccessVector = models.CharField(
-        "CVSS Access Vector", max_length=100, blank=True
+        "Access Vector (AV)", max_length=100, blank=True
     )
     cvssaccessComplexity = models.CharField(
-        "CVSS Access Complexity", max_length=100, blank=True
+        "Access Complexity (AC)", max_length=100, blank=True
     )
     cvssauthentication = models.CharField(
-        "CVSS Authentication", max_length=100, blank=True
+        "Authentication (Au)", max_length=100, blank=True
     )
     cvssconfidentialityImpact = models.CharField(
-        "CVSS Confidentiality Impact", max_length=100, blank=True
+        "Confidentiality Impact (C)", max_length=100, blank=True
     )
     cvssintegrityImpact = models.CharField(
-        "CVSS Integrity Impact", max_length=100, blank=True
+        "Integrity Impact (I)", max_length=100, blank=True
     )
     cvssavailabilityImpact = models.CharField(
-        "CVSS Availability Impact", max_length=100, blank=True
+        "Availability Impact (A)", max_length=100, blank=True
     )
-    cvssbaseScore = models.FloatField("CVSS Base Score", max_length=100, blank=True)
+    cvssbaseScore = models.FloatField("Base Score", max_length=100, blank=True)
 
     @property
     def affected_assets(self):
         return self.vulnerability_assignments.count()
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse("plugins:nb_risk:vulnerability", args=[self.pk])
 
     class Meta:
+        verbose_name = "Vulnerability"
         verbose_name_plural = "Vulnerabilities"
 
 
 # VulnearbilityAssingment Model
 
 
 class VulnerabilityAssignment(NetBoxModel):
```

### Comparing `NbRisk-0.4.1/nb_risk/navigation.py` & `NbRisk-0.5.0/nb_risk/navigation.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,19 @@
                             "Search",
                             "mdi mdi-magnify",
                             ButtonColorChoices.BLUE,
                             permissions=["nb_risk.view_vulnerability"],
                         ),
                     ),
                 ),
+                PluginMenuItem(
+                    permissions=["nb_risk.view_vulnerabilityassignment"],
+                    link="plugins:nb_risk:vulnerabilityassignment_list",
+                    link_text="Vulnerability Assignments",
+                ),
             ),
         ),
         (
             "Risk",
             (
                 PluginMenuItem(
                     permissions=["nb_risk.view_risk"],
```

### Comparing `NbRisk-0.4.1/nb_risk/tables.py` & `NbRisk-0.5.0/nb_risk/tables.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/template_content.py` & `NbRisk-0.5.0/nb_risk/template_content.py`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/control.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/control.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/control_assets.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/control_assets.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/control_risks.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/control_risks.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/risk.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/risk.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/threatevent.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/threatevent.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/threatsource.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/threatsource.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/vulnerability.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/vulnerability.html`

 * *Files 16% similar despite different names*

```diff
@@ -38,43 +38,43 @@
           <div class="card-body">
             {{ object.notes | markdown  }}
           </div>
         </div>        
     </div>
     <div class="col col-md-6">        
       <div class="card">
-        <h5 class="card-header">CVSS Score</h5>
+        <h5 class="card-header">CVSSv2 Score</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
-              <th scope="row">CVSS Access Vector</th>
+              <th scope="row">Access Vector (AV)</th>
               <td>{{ object.cvssaccessVector }}</td>
             </tr>
             <tr>
-              <th scope="row">CVSS Access Complexity</th>
+              <th scope="row">Access Complexity (AC)</th>
               <td>{{ object.cvssaccessComplexity }}</td>
             </tr>
             <tr>
-              <th scope="row">CVSS Authentication</th>
+              <th scope="row">Authentication (Au)</th>
               <td>{{ object.cvssauthentication }}</td>
             </tr>
             <tr>
-              <th scope="row">CVSS Confidentiality Impact</th>
+              <th scope="row">Confidentiality Impact (C)</th>
               <td>{{ object.cvssconfidentialityImpact }}</td>
             </tr>
             <tr>
-              <th scope="row">CVSS Integrity Impact</th>
+              <th scope="row">Integrity Impact (I)</th>
               <td>{{ object.cvssintegrityImpact }}</td>
             </tr>
             <tr>
-              <th scope="row">CVSS Availability Impact</th>
+              <th scope="row">Availability Impact (A)</th>
               <td>{{ object.cvssavailabilityImpact }}</td>
             </tr>
             <tr>
-              <th scope="row">CVSS Base Score</th>
+              <th scope="row">Base Score</th>
               <td>{{ object.cvssbaseScore }}</td>
             </tr> 
           </table>
         </div>
       </div>
       {% include 'inc/panels/tags.html' %}
     </div>
```

#### html2text {}

```diff
@@ -5,17 +5,17 @@
 {% endblock %} {% block content %}
 ** Vulnerability **
 Name        {{ object.name }}
 CVE         {{ object.cve }}
 Description {{ object.description }}
 ** Notes **
 {{ object.notes | markdown }}
-** CVSS Score **
-CVSS Access Vector          {{ object.cvssaccessVector }}
-CVSS Access Complexity      {{ object.cvssaccessComplexity }}
-CVSS Authentication         {{ object.cvssauthentication }}
-CVSS Confidentiality Impact {{ object.cvssconfidentialityImpact }}
-CVSS Integrity Impact       {{ object.cvssintegrityImpact }}
-CVSS Availability Impact    {{ object.cvssavailabilityImpact }}
-CVSS Base Score             {{ object.cvssbaseScore }}
+** CVSSv2 Score **
+Access Vector (AV)         {{ object.cvssaccessVector }}
+Access Complexity (AC)     {{ object.cvssaccessComplexity }}
+Authentication (Au)        {{ object.cvssauthentication }}
+Confidentiality Impact (C) {{ object.cvssconfidentialityImpact }}
+Integrity Impact (I)       {{ object.cvssintegrityImpact }}
+Availability Impact (A)    {{ object.cvssavailabilityImpact }}
+Base Score                 {{ object.cvssbaseScore }}
 {% include 'inc/panels/tags.html' %}
 {% endblock %}
```

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/templates/nb_risk/vulnerability_search.html` & `NbRisk-0.5.0/nb_risk/templates/nb_risk/vulnerability_search.html`

 * *Files identical despite different names*

### Comparing `NbRisk-0.4.1/nb_risk/urls.py` & `NbRisk-0.5.0/nb_risk/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         name="vulnerability",
     ),
     path(
         "vulnerability/<int:pk>/edit/",
         views.VulnerabilityEditView.as_view(),
         name="vulnerability_edit",
     ),
+    path('vulnerability/import/', views.VulnerabilityBulkImportView.as_view(), name='vulnerability_import'),
     path(
         "vulnerability/<int:pk>/delete/",
         views.VulnerabilityDeleteView.as_view(),
         name="vulnerability_delete",
     ),
     path(
         "vulnerability/delete/",
@@ -113,14 +114,18 @@
     ),
     # VulnerabilityAssignment URLs
     path(
         "vulnerability-assignments/add/",
         views.VulnerabilityAssignmentEditView.as_view(),
         name="vulnerabilityassignment_add",
     ),
+    path("vulnerability-assignments/",
+        views.VulnerabilityAssignmentListView.as_view(),
+        name="vulnerabilityassignment_list",
+    ),
     path(
         "vulnerability-assignments/<int:pk>/delete/",
         views.VulnerabilityAssignmentDeleteView.as_view(),
         name="vulnerabilityassignment_delete",
     ),
     # Risk URLs
     path("risk/", views.RiskListView.as_view(), name="risk_list"),
```

### Comparing `NbRisk-0.4.1/nb_risk/views.py` & `NbRisk-0.5.0/nb_risk/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,17 @@
     template_name = "nb_risk/vulnerability_list.html"
 
 
 class VulnerabilityEditView(generic.ObjectEditView):
     queryset = models.Vulnerability.objects.all()
     form = forms.VulnerabilityForm
 
+class VulnerabilityBulkImportView(generic.BulkImportView):
+    queryset = models.Vulnerability.objects.all()
+    model_form = forms.VulnerabilityImportForm
 
 class VulnerabilityDeleteView(generic.ObjectDeleteView):
     queryset = models.Vulnerability.objects.all()
 
 
 class VulnerabilityBulkDeleteView(generic.BulkDeleteView):
     queryset = models.Vulnerability.objects.all()
@@ -208,14 +211,20 @@
             "asset_id": request.GET.get("asset_id"),
         }
 
 
 class VulnerabilityAssignmentDeleteView(generic.ObjectDeleteView):
     queryset = models.VulnerabilityAssignment.objects.all()
 
+class VulnerabilityAssignmentListView(generic.ObjectListView):
+    queryset = models.VulnerabilityAssignment.objects.all()
+    table = tables.VulnerabilityExploitListTable
+    filterset = filters.VulnerabilityAssignmentFilterSet
+    filterset_form = forms.VulnerabilityAssignmentFilterForm
+    actions = ('import', 'export', )
 
 # Risk Views
 
 
 class RiskListView(generic.ObjectListView):
     queryset = models.Risk.objects.all()
     table = tables.RiskTable
```

### Comparing `NbRisk-0.4.1/setup.py` & `NbRisk-0.5.0/setup.py`

 * *Files identical despite different names*

