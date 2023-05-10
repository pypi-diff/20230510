# Comparing `tmp/NbRisk-34.0.0.tar.gz` & `tmp/NbRisk-35.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NbRisk-34.0.0.tar", last modified: Wed May 10 13:46:17 2023, max compression
+gzip compressed data, was "NbRisk-35.0.0.tar", last modified: Wed May 10 14:31:10 2023, max compression
```

## Comparing `NbRisk-34.0.0.tar` & `NbRisk-35.0.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:46:17.222591 NbRisk-34.0.0/
--rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-34.0.0/LICENSE
--rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-34.0.0/MANIFEST.in
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:46:17.206591 NbRisk-34.0.0/NbRisk.egg-info/
--rw-rw-r--   0 renato    (1000) renato    (1000)     3011 2023-05-10 13:46:17.000000 NbRisk-34.0.0/NbRisk.egg-info/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     1526 2023-05-10 13:46:17.000000 NbRisk-34.0.0/NbRisk.egg-info/SOURCES.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-05-10 13:46:17.000000 NbRisk-34.0.0/NbRisk.egg-info/dependency_links.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-05-10 13:46:17.000000 NbRisk-34.0.0/NbRisk.egg-info/top_level.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)     3011 2023-05-10 13:46:17.222591 NbRisk-34.0.0/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2582 2023-04-21 03:01:56.000000 NbRisk-34.0.0/README.md
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:46:17.210591 NbRisk-34.0.0/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-34.0.0/nb_risk/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-34.0.0/nb_risk/admin.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:46:17.214591 NbRisk-34.0.0/nb_risk/api/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-34.0.0/nb_risk/api/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-34.0.0/nb_risk/api/nested_serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5159 2023-04-21 02:18:22.000000 NbRisk-34.0.0/nb_risk/api/serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-34.0.0/nb_risk/api/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-34.0.0/nb_risk/api/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-34.0.0/nb_risk/choices.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-34.0.0/nb_risk/columns.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-34.0.0/nb_risk/cve.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-34.0.0/nb_risk/filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5051 2023-05-10 12:58:48.000000 NbRisk-34.0.0/nb_risk/forms.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-34.0.0/nb_risk/middleware.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:46:17.214591 NbRisk-34.0.0/nb_risk/migrations/
--rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-34.0.0/nb_risk/migrations/0001_initial.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-34.0.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-34.0.0/nb_risk/migrations/0003_control.py
--rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-34.0.0/nb_risk/migrations/0004_alter_vulnerability_options.py
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-34.0.0/nb_risk/migrations/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     8511 2023-05-10 12:47:27.000000 NbRisk-34.0.0/nb_risk/models.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-34.0.0/nb_risk/navigation.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-34.0.0/nb_risk/signals.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3428 2023-05-10 13:24:07.000000 NbRisk-34.0.0/nb_risk/tables.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-34.0.0/nb_risk/template_content.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:46:17.202591 NbRisk-34.0.0/nb_risk/templates/
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 13:46:17.222591 NbRisk-34.0.0/nb_risk/templates/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)     1831 2023-04-21 02:45:22.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/control.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      867 2023-04-21 02:58:51.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/control_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      867 2023-04-21 02:45:38.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/control_risks.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/generic_vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/risk.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2211 2023-01-25 20:53:20.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/threatevent.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      505 2023-01-25 20:53:31.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/threatsource.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2831 2023-05-10 12:31:54.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/vulnerability.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      609 2023-04-02 19:20:45.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-34.0.0/nb_risk/templates/nb_risk/vulnerability_search.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     5961 2023-05-10 13:18:51.000000 NbRisk-34.0.0/nb_risk/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       23 2023-05-10 13:45:50.000000 NbRisk-34.0.0/nb_risk/version.py
--rw-rw-r--   0 renato    (1000) renato    (1000)    10306 2023-05-10 13:24:11.000000 NbRisk-34.0.0/nb_risk/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-05-10 13:46:17.222591 NbRisk-34.0.0/setup.cfg
--rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-34.0.0/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.175196 NbRisk-35.0.0/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-35.0.0/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-35.0.0/MANIFEST.in
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.167196 NbRisk-35.0.0/NbRisk.egg-info/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3011 2023-05-10 14:31:10.000000 NbRisk-35.0.0/NbRisk.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1526 2023-05-10 14:31:10.000000 NbRisk-35.0.0/NbRisk.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-05-10 14:31:10.000000 NbRisk-35.0.0/NbRisk.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-05-10 14:31:10.000000 NbRisk-35.0.0/NbRisk.egg-info/top_level.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3011 2023-05-10 14:31:10.175196 NbRisk-35.0.0/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2582 2023-04-21 03:01:56.000000 NbRisk-35.0.0/README.md
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.171196 NbRisk-35.0.0/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-35.0.0/nb_risk/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-35.0.0/nb_risk/admin.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.171196 NbRisk-35.0.0/nb_risk/api/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.0/nb_risk/api/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-35.0.0/nb_risk/api/nested_serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5107 2023-05-10 14:09:32.000000 NbRisk-35.0.0/nb_risk/api/serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-35.0.0/nb_risk/api/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-35.0.0/nb_risk/api/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-35.0.0/nb_risk/choices.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-35.0.0/nb_risk/columns.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-35.0.0/nb_risk/cve.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-35.0.0/nb_risk/filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4997 2023-05-10 14:08:50.000000 NbRisk-35.0.0/nb_risk/forms.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.0/nb_risk/middleware.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.171196 NbRisk-35.0.0/nb_risk/migrations/
+-rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-35.0.0/nb_risk/migrations/0001_initial.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-35.0.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-35.0.0/nb_risk/migrations/0003_control.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-35.0.0/nb_risk/migrations/0004_alter_vulnerability_options.py
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-35.0.0/nb_risk/migrations/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     8511 2023-05-10 12:47:27.000000 NbRisk-35.0.0/nb_risk/models.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-35.0.0/nb_risk/navigation.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.0/nb_risk/signals.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3428 2023-05-10 13:24:07.000000 NbRisk-35.0.0/nb_risk/tables.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-35.0.0/nb_risk/template_content.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.167196 NbRisk-35.0.0/nb_risk/templates/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-10 14:31:10.175196 NbRisk-35.0.0/nb_risk/templates/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2236 2023-05-10 14:28:34.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/control.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1272 2023-05-10 14:28:23.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/control_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1272 2023-05-10 14:28:29.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/control_risks.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/generic_vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/risk.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2604 2023-05-10 14:28:43.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/threatevent.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      898 2023-05-10 14:28:39.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/threatsource.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3216 2023-05-10 14:28:51.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      996 2023-05-10 14:28:47.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_search.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5961 2023-05-10 13:18:51.000000 NbRisk-35.0.0/nb_risk/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       23 2023-05-10 13:48:53.000000 NbRisk-35.0.0/nb_risk/version.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10306 2023-05-10 14:21:42.000000 NbRisk-35.0.0/nb_risk/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-05-10 14:31:10.175196 NbRisk-35.0.0/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-35.0.0/setup.py
```

### Comparing `NbRisk-34.0.0/LICENSE` & `NbRisk-35.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/NbRisk.egg-info/PKG-INFO` & `NbRisk-35.0.0/NbRisk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 34.0.0
+Version: 35.0.0
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-34.0.0/NbRisk.egg-info/SOURCES.txt` & `NbRisk-35.0.0/NbRisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/PKG-INFO` & `NbRisk-35.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 34.0.0
+Version: 35.0.0
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-34.0.0/README.md` & `NbRisk-35.0.0/README.md`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/__init__.py` & `NbRisk-35.0.0/nb_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/api/nested_serializers.py` & `NbRisk-35.0.0/nb_risk/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/api/serializers.py` & `NbRisk-35.0.0/nb_risk/api/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from rest_framework import serializers
 from django.contrib.contenttypes.models import ContentType
 from netbox.api.fields import ChoiceField, ContentTypeField, SerializedPKRelatedField
 from netbox.api.serializers import WritableNestedSerializer
 from utilities.api import get_serializer_for_model
-from drf_yasg.utils import swagger_serializer_method
+
 
 from netbox.api.serializers import NetBoxModelSerializer
 from nb_risk.api.nested_serializers import (
     NestedThreatSourceSerializer,
     NestedRiskSerializer,
 )
 from .. import models, choices
```

### Comparing `NbRisk-34.0.0/nb_risk/api/views.py` & `NbRisk-35.0.0/nb_risk/api/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/choices.py` & `NbRisk-35.0.0/nb_risk/choices.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/columns.py` & `NbRisk-35.0.0/nb_risk/columns.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/cve.py` & `NbRisk-35.0.0/nb_risk/cve.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/filters.py` & `NbRisk-35.0.0/nb_risk/filters.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/forms.py` & `NbRisk-35.0.0/nb_risk/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from django import forms
 
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelImportForm
 from dcim.models import Device, DeviceType
-from virtualization.models import VirtualMachine
-
-from utilities.forms import (
-    BootstrapMixin,
-    DatePicker,
-    CommentField,
+from utilities.forms import BootstrapMixin
+from utilities.forms.fields import (
     DynamicModelMultipleChoiceField,
     SlugField,
     DynamicModelChoiceField,
 )
 
 from . import models, choices
```

### Comparing `NbRisk-34.0.0/nb_risk/migrations/0001_initial.py` & `NbRisk-35.0.0/nb_risk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py` & `NbRisk-35.0.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/migrations/0003_control.py` & `NbRisk-35.0.0/nb_risk/migrations/0003_control.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/models.py` & `NbRisk-35.0.0/nb_risk/models.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/navigation.py` & `NbRisk-35.0.0/nb_risk/navigation.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/tables.py` & `NbRisk-35.0.0/nb_risk/tables.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/template_content.py` & `NbRisk-35.0.0/nb_risk/template_content.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/control.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/control_assets.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,34 @@
 {% extends 'generic/object.html' %}
 {% load render_table from django_tables2 %}
+{% load tabs %}
 
-{% block extra_tabs %}
-<li role="presentation" class="nav-item">
-    <a href="{% url 'plugins:nb_risk:control_risks' pk=object.pk %}" class="nav-link{% if tab == 'risks' %} active{% endif %}">
-        Risks  {% if risks_count  %}<span class="badge bg-secondary">{{ risks_count }}</span>{% endif %}
-    </a>
-</li>
-<li role="presentation" class="nav-item">
-    <a href="{% url 'plugins:nb_risk:control_assets' pk=object.pk %}" class="nav-link{% if tab == 'assets' %} active{% endif %}">
-        Related Assets  {% if assets_count  %}<span class="badge bg-secondary">{{ assets_count }}</span>{% endif %}
-    </a>
-</li>
-{% endblock %}
+
+{% block tabs %}
+  <ul class="nav nav-tabs px-3">
+    {# Primary tab #}
+    <li class="nav-item" role="presentation">
+      <a class="nav-link{% if not tab %} active{% endif %}" href="{{ object.get_absolute_url }}">{{ object|meta:"verbose_name"|bettertitle }}</a>
+    </li>
+    <li role="presentation" class="nav-item">
+        <a href="{% url 'plugins:nb_risk:control_risks' pk=object.pk %}" class="nav-link{% if tab == 'risks' %} active{% endif %}">
+            Risks  {% if risks_count  %}<span class="badge bg-secondary">{{ risks_count }}</span>{% endif %}
+        </a>
+    </li>
+    <li role="presentation" class="nav-item">
+        <a href="{% url 'plugins:nb_risk:control_assets' pk=object.pk %}" class="nav-link{% if tab == 'assets' %} active{% endif %}">
+            Related Assets  {% if assets_count  %}<span class="badge bg-secondary">{{ assets_count }}</span>{% endif %}
+        </a>
+    </li>
+
+    {# Include tabs for registered model views #}
+    {% model_view_tabs object %}
+  </ul>
+{% endblock tabs %}
 
 {% block content %}
-<div class="row mb-3">
-    <div class="col col-md-6">
-        <div class="card">
-            <h5 class="card-header">Control</h5>
-            <div class="card-body">
-                <table class="table table-hover attr-table">
-                    <tr>
-                        <th scope="row">Name</th>
-                        <td>{{ object.name }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Category</th>
-                        <td>{{ object.category }}</td>
-                    </tr>
-                </table>
-            </div>
-        </div>
-    </div>
-    <div class="col col-md-6">
-        <div class="card">
-            <h5 class="card-header">Notes</h5>
-            <div class="card-body">
-              {{ object.notes | markdown  }}
-            </div>
-        </div> 
-    </div>
-</div>
-<div class="row mb-3">
-    <div class="col col-md-6">
-        {% include 'inc/panels/comments.html' %}
-        {% include 'inc/panels/custom_fields.html' %}
-        {% include 'inc/panels/tags.html' %}
+<div class="card">
+    <div class="card-body" id="object_list">
+      {% include 'htmx/table.html' %}
     </div>
-           
 </div>
-
-
-
-
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,11 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% block extra_tabs %}
-Risks_{%_if_risks_count_%}{{_risks_count_}}{%_endif_%}
-Related_Assets_{%_if_assets_count_%}{{_assets_count_}}{%_endif_%}
-{% endblock %} {% block content %}
-** Control **
-Name     {{ object.name }}
-Category {{ object.category }}
-** Notes **
-{{ object.notes | markdown }}
-{% include 'inc/panels/comments.html' %} {% include 'inc/panels/
-custom_fields.html' %} {% include 'inc/panels/tags.html' %}
+{% load tabs %} {% block tabs %}
+    * {# Primary tab #}
+    * {{_object|meta:"verbose_name"|bettertitle_}}
+    * Risks_{%_if_risks_count_%}{{_risks_count_}}{%_endif_%}
+    * Related_Assets_{%_if_assets_count_%}{{_assets_count_}}{%_endif_%}
+    * {# Include tabs for registered model views #} {% model_view_tabs object
+      %}
+{% endblock tabs %} {% block content %}
+{% include 'htmx/table.html' %}
 {% endblock %}
```

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/control_assets.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 {% extends 'generic/object.html' %}
 {% load render_table from django_tables2 %}
+{% load tabs %}
+
+
+{% block tabs %}
+  <ul class="nav nav-tabs px-3">
+    {# Primary tab #}
+    <li class="nav-item" role="presentation">
+      <a class="nav-link{% if not tab %} active{% endif %}" href="{{ object.get_absolute_url }}">{{ object|meta:"verbose_name"|bettertitle }}</a>
+    </li>
+    <li role="presentation" class="nav-item">
+      <a href="{% url 'plugins:nb_risk:vulnerability_affected_assets' pk=object.pk %}" class="nav-link{% if tab == 'affected_assets' %} active{% endif %}">
+        Affected Assets  {% if affected_assets_count  %}<span class="badge bg-secondary">{{ affected_assets_count }}</span>{% endif %}
+      </a>
+    </li>
+
+    {# Include tabs for registered model views #}
+    {% model_view_tabs object %}
+  </ul>
+{% endblock tabs %}
 
-{% block extra_tabs %}
-<li role="presentation" class="nav-item">
-    <a href="{% url 'plugins:nb_risk:control_risks' pk=object.pk %}" class="nav-link{% if tab == 'risks' %} active{% endif %}">
-        Risks  {% if risks_count  %}<span class="badge bg-secondary">{{ risks_count }}</span>{% endif %}
-    </a>
-</li>
-<li role="presentation" class="nav-item">
-    <a href="{% url 'plugins:nb_risk:control_assets' pk=object.pk %}" class="nav-link{% if tab == 'assets' %} active{% endif %}">
-        Related Assets  {% if assets_count  %}<span class="badge bg-secondary">{{ assets_count }}</span>{% endif %}
-    </a>
-</li>
-{% endblock %}
 
 {% block content %}
-<div class="card">
-    <div class="card-body" id="object_list">
-      {% include 'htmx/table.html' %}
-    </div>
+<div class="row mb-3">
+  <div class="card-body" id="object_list">
+    {% include 'htmx/table.html' %}
+  </div>
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% block extra_tabs %}
-Risks_{%_if_risks_count_%}{{_risks_count_}}{%_endif_%}
-Related_Assets_{%_if_assets_count_%}{{_assets_count_}}{%_endif_%}
-{% endblock %} {% block content %}
+{% load tabs %} {% block tabs %}
+    * {# Primary tab #}
+    * {{_object|meta:"verbose_name"|bettertitle_}}
+    * Affected_Assets_{%_if_affected_assets_count_%}{{_affected_assets_count_}}
+      {%_endif_%}
+    * {# Include tabs for registered model views #} {% model_view_tabs object
+      %}
+{% endblock tabs %} {% block content %}
 {% include 'htmx/table.html' %}
 {% endblock %}
```

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/control_risks.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 {% extends 'generic/object.html' %}
 {% load render_table from django_tables2 %}
+{% load tabs %}
 
-{% block extra_tabs %}
-<li role="presentation" class="nav-item">
-    <a href="{% url 'plugins:nb_risk:control_risks' pk=object.pk %}" class="nav-link{% if tab == 'risks' %} active{% endif %}">
-        Risks  {% if risks_count  %}<span class="badge bg-secondary">{{ risks_count }}</span>{% endif %}
-    </a>
-</li>
-<li role="presentation" class="nav-item">
-    <a href="{% url 'plugins:nb_risk:control_assets' pk=object.pk %}" class="nav-link{% if tab == 'assets' %} active{% endif %}">
-        Related Assets  {% if assets_count  %}<span class="badge bg-secondary">{{ assets_count }}</span>{% endif %}
-    </a>
-</li>
-{% endblock %}
+
+{% block tabs %}
+  <ul class="nav nav-tabs px-3">
+    {# Primary tab #}
+    <li class="nav-item" role="presentation">
+      <a class="nav-link{% if not tab %} active{% endif %}" href="{{ object.get_absolute_url }}">{{ object|meta:"verbose_name"|bettertitle }}</a>
+    </li>
+    <li role="presentation" class="nav-item">
+        <a href="{% url 'plugins:nb_risk:threatevent_vulnerabilities' pk=object.pk %}" class="nav-link{% if tab == 'vulnerabilities' %} active{% endif %}">
+            Exploit Vulnerabilities
+        </a>
+    </li>
+
+    {# Include tabs for registered model views #}
+    {% model_view_tabs object %}
+  </ul>
+{% endblock tabs %}
 
 {% block content %}
-<div class="card">
-    <div class="card-body" id="object_list">
-      {% include 'htmx/table.html' %}
-    </div>
+<div class="row mb-3">
+  <div class="card-body" id="object_list">
+    {% include 'htmx/table.html' %}
+  </div>
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,7 +1,10 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% block extra_tabs %}
-Risks_{%_if_risks_count_%}{{_risks_count_}}{%_endif_%}
-Related_Assets_{%_if_assets_count_%}{{_assets_count_}}{%_endif_%}
-{% endblock %} {% block content %}
+{% load tabs %} {% block tabs %}
+    * {# Primary tab #}
+    * {{_object|meta:"verbose_name"|bettertitle_}}
+    * Exploit_Vulnerabilities
+    * {# Include tabs for registered model views #} {% model_view_tabs object
+      %}
+{% endblock tabs %} {% block content %}
 {% include 'htmx/table.html' %}
 {% endblock %}
```

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/risk.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/risk.html`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/threatevent.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/threatevent.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 {% extends 'generic/object.html' %}
 {% load render_table from django_tables2 %}
+{% load tabs %}
+
+{% block tabs %}
+  <ul class="nav nav-tabs px-3">
+    {# Primary tab #}
+    <li class="nav-item" role="presentation">
+      <a class="nav-link{% if not tab %} active{% endif %}" href="{{ object.get_absolute_url }}">{{ object|meta:"verbose_name"|bettertitle }}</a>
+    </li>
+    <li role="presentation" class="nav-item">
+        <a href="{% url 'plugins:nb_risk:threatevent_vulnerabilities' pk=object.pk %}" class="nav-link{% if tab == 'vulnerabilities' %} active{% endif %}">
+            Exploit Vulnerabilities
+        </a>
+    </li>
+
+    {# Include tabs for registered model views #}
+    {% model_view_tabs object %}
+  </ul>
+{% endblock tabs %}
 
-{% block extra_tabs %}
-<li role="presentation" class="nav-item">
-  <a href="{% url 'plugins:nb_risk:threatevent_vulnerabilities' pk=object.pk %}" class="nav-link{% if tab == 'vulnerabilities' %} active{% endif %}">
-    Exploit Vulnerabilities
-  </a>
-</li>
-{% endblock %}
 
 {% block content %}
 <div class="row mb-3">
     <div class="col col-md-6">
         <div class="card">
             <h5 class="card-header">Threat Event</h5>
             <div class="card-body">
```

#### html2text {}

```diff
@@ -1,11 +1,15 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% block extra_tabs %}
-Exploit_Vulnerabilities
-{% endblock %} {% block content %}
+{% load tabs %} {% block tabs %}
+    * {# Primary tab #}
+    * {{_object|meta:"verbose_name"|bettertitle_}}
+    * Exploit_Vulnerabilities
+    * {# Include tabs for registered model views #} {% model_view_tabs object
+      %}
+{% endblock tabs %} {% block content %}
 ** Threat Event **
 Name          {{ object.name }}
               {% if object.threat_source %} {% if
 Threat Source object.threat_source.get_absolute_url %} {{_object.threat_source
               }} {% endif %} {% else %} --- {% endif %}
 Relevance     {{ object.relevance }}
 Likelihood    {{ object.likelihood }}
```

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/threatsource.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/threatsource.html`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/vulnerability.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 {% extends 'generic/object.html' %}
 {% load humanize %}
 {% load helpers %}
 {% load render_table from django_tables2 %}
+{% load tabs %}
 
-{% block extra_tabs %}
-<li role="presentation" class="nav-item">
-  <a href="{% url 'plugins:nb_risk:vulnerability_affected_assets' pk=object.pk %}" class="nav-link{% if tab == 'affected_assets' %} active{% endif %}">
-    Affected Assets  {% if affected_assets_count  %}<span class="badge bg-secondary">{{ affected_assets_count }}</span>{% endif %}
-  </a>
-</li>
-{% endblock %}
+
+{% block tabs %}
+  <ul class="nav nav-tabs px-3">
+    {# Primary tab #}
+    <li class="nav-item" role="presentation">
+      <a class="nav-link{% if not tab %} active{% endif %}" href="{{ object.get_absolute_url }}">{{ object|meta:"verbose_name"|bettertitle }}</a>
+    </li>
+    <li role="presentation" class="nav-item">
+      <a href="{% url 'plugins:nb_risk:vulnerability_affected_assets' pk=object.pk %}" class="nav-link{% if tab == 'affected_assets' %} active{% endif %}">
+        Affected Assets  {% if affected_assets_count  %}<span class="badge bg-secondary">{{ affected_assets_count }}</span>{% endif %}
+      </a>
+    </li>
+
+    {# Include tabs for registered model views #}
+    {% model_view_tabs object %}
+  </ul>
+{% endblock tabs %}
 
 {% block content %}
 <div class="row mb-3">
     <div class="col col-md-6">
         <div class="card">
             <h5 class="card-header">Vulnerability</h5>
             <div class="card-body">
```

#### html2text {}

```diff
@@ -1,12 +1,16 @@
 {% extends 'generic/object.html' %} {% load humanize %} {% load helpers %} {%
-load render_table from django_tables2 %} {% block extra_tabs %}
-Affected_Assets_{%_if_affected_assets_count_%}{{_affected_assets_count_}}{%
-endif_%}
-{% endblock %} {% block content %}
+load render_table from django_tables2 %} {% load tabs %} {% block tabs %}
+    * {# Primary tab #}
+    * {{_object|meta:"verbose_name"|bettertitle_}}
+    * Affected_Assets_{%_if_affected_assets_count_%}{{_affected_assets_count_}}
+      {%_endif_%}
+    * {# Include tabs for registered model views #} {% model_view_tabs object
+      %}
+{% endblock tabs %} {% block content %}
 ** Vulnerability **
 Name        {{ object.name }}
 CVE         {{ object.cve }}
 Description {{ object.description }}
 ** Notes **
 {{ object.notes | markdown }}
 ** CVSSv2 Score **
```

### Comparing `NbRisk-34.0.0/nb_risk/templates/nb_risk/vulnerability_search.html` & `NbRisk-35.0.0/nb_risk/templates/nb_risk/vulnerability_search.html`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/urls.py` & `NbRisk-35.0.0/nb_risk/urls.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/nb_risk/views.py` & `NbRisk-35.0.0/nb_risk/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-34.0.0/setup.py` & `NbRisk-35.0.0/setup.py`

 * *Files identical despite different names*

