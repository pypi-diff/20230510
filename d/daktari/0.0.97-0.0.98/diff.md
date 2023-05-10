# Comparing `tmp/daktari-0.0.97.tar.gz` & `tmp/daktari-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daktari-0.0.97.tar", last modified: Tue May  9 09:15:10 2023, max compression
+gzip compressed data, was "daktari-0.0.98.tar", last modified: Wed May 10 09:24:12 2023, max compression
```

## Comparing `daktari-0.0.97.tar` & `daktari-0.0.98.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.584625 daktari-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 09:14:59.000000 daktari-0.0.97/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 09:14:59.000000 daktari-0.0.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-09 09:15:10.584625 daktari-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-09 09:15:01.000000 daktari-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.580625 daktari-0.0.97/daktari/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 09:15:01.000000 daktari-0.0.97/daktari/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1427 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/check_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/check_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/check_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.584625 daktari-0.0.97/daktari/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/direnv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/flutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/intellij_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/onepassword.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/test_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/test_java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/test_yarn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/checks/yarn.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/command_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/os.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/resource_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.584625 daktari-0.0.97/daktari/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/resources/daktari-local-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/resources/mock_cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/result_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_check_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_check_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_check_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_result_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/test_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-09 09:14:59.000000 daktari-0.0.97/daktari/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:15:10.580625 daktari-0.0.97/daktari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 09:15:10.000000 daktari-0.0.97/daktari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-09 09:14:59.000000 daktari-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-09 09:14:59.000000 daktari-0.0.97/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:15:10.584625 daktari-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-09 09:15:01.000000 daktari-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:24:12.930615 daktari-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-10 09:24:00.000000 daktari-0.0.98/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 09:24:00.000000 daktari-0.0.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-10 09:24:12.930615 daktari-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-10 09:24:02.000000 daktari-0.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:24:12.930615 daktari-0.0.98/daktari/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 09:24:02.000000 daktari-0.0.98/daktari/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1463 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/check_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/check_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/check_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:24:12.930615 daktari-0.0.98/daktari/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/direnv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/flutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/intellij_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/onepassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/test_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/test_yarn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/checks/yarn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/command_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/resource_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:24:12.930615 daktari-0.0.98/daktari/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/resources/daktari-local-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/resources/mock_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/result_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_check_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_check_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_check_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_check_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_result_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/test_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-10 09:24:00.000000 daktari-0.0.98/daktari/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:24:12.930615 daktari-0.0.98/daktari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-10 09:24:12.000000 daktari-0.0.98/daktari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-10 09:24:12.000000 daktari-0.0.98/daktari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:24:12.000000 daktari-0.0.98/daktari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 09:24:12.000000 daktari-0.0.98/daktari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-10 09:24:12.000000 daktari-0.0.98/daktari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 09:24:12.000000 daktari-0.0.98/daktari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 09:24:00.000000 daktari-0.0.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-10 09:24:00.000000 daktari-0.0.98/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:24:12.930615 daktari-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-10 09:24:02.000000 daktari-0.0.98/setup.py
```

### Comparing `daktari-0.0.97/LICENSE.txt` & `daktari-0.0.98/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/PKG-INFO` & `daktari-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daktari
-Version: 0.0.97
+Version: 0.0.98
 Summary: Assist in setting up and maintaining developer environments
 Home-page: https://github.com/sonocent/daktari
 Author: Matt Russell
 Author-email: matthew.russell@sonocent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.97"
+version = "0.0.98"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.97/README.md` & `daktari-0.0.98/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.97"
+version = "0.0.98"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.97/daktari/__main__.py` & `daktari-0.0.98/daktari/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     config = read_config(args.config_path)
     if config is None:
         return 1
 
     os.chdir(args.config_path.parent.absolute())
     print_config_messages(config, args)
 
-    all_passed = run_checks(config.checks, args.quiet_mode or config.quiet_mode)
+    all_passed = run_checks(config.checks, args.quiet_mode or config.quiet_mode, args.fail_fast)
     print("")
     return 0 if all_passed else 1
 
 
 def print_config_messages(config: Config, args):
     if config.title:
         print_logo(config.title)
@@ -42,13 +42,13 @@
     ignored_count = len(config.ignored_checks)
     if ignored_count > 0:
         if args.show_ignored:
             print("ⓘ  The following checks have been ignored:\n")
             for check in config.ignored_checks:
                 print(f"[{check.name}]")
             print("")
-        else:
+        elif not args.quiet_mode:
             print(f"ⓘ  {ignored_count} check(s) have been marked as ignored. Run with --show-ignored to list them.\n")
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `daktari-0.0.97/daktari/check.py` & `daktari-0.0.98/daktari/check.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/check_runner.py` & `daktari-0.0.98/daktari/check_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,37 @@
 
 from daktari.check import Check, CheckStatus, CheckResult
 from daktari.check_sorter import sort_checks
 from daktari.os import detect_os
 from daktari.result_printer import print_check_result
 
 
-def run_checks(checks: List[Check], hide_passing_checks: bool) -> bool:
-    return CheckRunner(checks, hide_passing_checks).run()
+def run_checks(checks: List[Check], quiet_mode: bool, fail_fast: bool) -> bool:
+    return CheckRunner(checks, quiet_mode, fail_fast).run()
 
 
 class CheckRunner:
-    def __init__(self, checks: List[Check], quiet_mode: bool):
+    def __init__(self, checks: List[Check], quiet_mode: bool, fail_fast: bool):
         self.checks = [check for check in checks if check.run_on is None or check.run_on == detect_os()]
         self.all_passed = True
         self.checks_passed: Set[str] = set()
         self.quiet_mode = quiet_mode
+        self.fail_fast = fail_fast
 
     def run(self) -> bool:
         for idx, check in enumerate(sort_checks(self.checks)):
             self.try_run_check(idx, check)
+            if self.early_exit():
+                break
+
         return self.all_passed
 
+    def early_exit(self) -> bool:
+        return self.fail_fast and not self.all_passed
+
     def try_run_check(self, idx: int, check: Check):
         dependencies_met = all([dependency.name in self.checks_passed for dependency in check.depends_on])
         if dependencies_met:
             self.run_check(idx, check)
         else:
             self.diagnose_missing_dependency(check)
 
@@ -36,15 +43,15 @@
         logging.info(f"Running check {check.name}")
         result = self.run_check_in_try(check)
         if result.status in (CheckStatus.PASS, CheckStatus.PASS_WITH_WARNING):
             self.checks_passed.add(check.name)
         else:
             self.all_passed = False
 
-        print_check_result(result, self.quiet_mode, idx, len(self.checks))
+        print_check_result(result, self.early_exit(), self.quiet_mode, idx, len(self.checks))
 
     def run_check_in_try(self, check: Check) -> CheckResult:
         try:
             return check.check()
         except Exception as err:
             logging.debug(f"Exception running check {check.name}", exc_info=True)
             return CheckResult(check.name, CheckStatus.ERROR, f"Check failed with unhandled {type(err).__name__}", {})
```

### Comparing `daktari-0.0.97/daktari/check_sorter.py` & `daktari-0.0.98/daktari/check_sorter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/check_utils.py` & `daktari-0.0.98/daktari/check_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/certs.py` & `daktari-0.0.98/daktari/checks/certs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/direnv.py` & `daktari-0.0.98/daktari/checks/direnv.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/docker.py` & `daktari-0.0.98/daktari/checks/docker.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/files.py` & `daktari-0.0.98/daktari/checks/files.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/flutter.py` & `daktari-0.0.98/daktari/checks/flutter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/git.py` & `daktari-0.0.98/daktari/checks/git.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/google.py` & `daktari-0.0.98/daktari/checks/google.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/intellij_idea.py` & `daktari-0.0.98/daktari/checks/intellij_idea.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/java.py` & `daktari-0.0.98/daktari/checks/java.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/kubernetes.py` & `daktari-0.0.98/daktari/checks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/misc.py` & `daktari-0.0.98/daktari/checks/misc.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/nodejs.py` & `daktari-0.0.98/daktari/checks/nodejs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/onepassword.py` & `daktari-0.0.98/daktari/checks/onepassword.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/python.py` & `daktari-0.0.98/daktari/checks/python.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/ssh.py` & `daktari-0.0.98/daktari/checks/ssh.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/terraform.py` & `daktari-0.0.98/daktari/checks/terraform.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/test_certs.py` & `daktari-0.0.98/daktari/checks/test_certs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/test_java.py` & `daktari-0.0.98/daktari/checks/test_java.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/test_ssh.py` & `daktari-0.0.98/daktari/checks/test_ssh.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/test_yarn.py` & `daktari-0.0.98/daktari/checks/test_yarn.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/xml.py` & `daktari-0.0.98/daktari/checks/xml.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/checks/yarn.py` & `daktari-0.0.98/daktari/checks/yarn.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/command_utils.py` & `daktari-0.0.98/daktari/command_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/config.py` & `daktari-0.0.98/daktari/config.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/file_utils.py` & `daktari-0.0.98/daktari/file_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/options.py` & `daktari-0.0.98/daktari/options.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 argument_parser.add_argument(
     "-i", "--show-ignored", action="store_true", help="show checks affected by ignoredChecks local setting"
 )
 argument_parser.add_argument(
     "-q", "--quiet", action="store_true", dest="quiet_mode", help="only show failed checks and overall progress"
 )
 argument_parser.add_argument(
+    "-f", "--fail-fast", action="store_true", dest="fail_fast", help="stop running checks after the first failure"
+)
+argument_parser.add_argument(
     "-c",
     "--config",
     default=".daktari.py",
     dest="config_path",
     required=False,
     help="Python configuration file",
     metavar="FILE",
```

### Comparing `daktari-0.0.97/daktari/os.py` & `daktari-0.0.98/daktari/os.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/result_printer.py` & `daktari-0.0.98/daktari/result_printer.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,36 +50,39 @@
         if len(raw_lines) > 1:
             print(f"  {line}")
         else:
             print(f"│ {line}{padding} │")
     print("└" + "─" * (max_width + 2) + "┘")
 
 
-def print_check_result(result: CheckResult, quiet_mode: bool, idx: int, total_checks: int):
+def print_check_result(result: CheckResult, early_exit: bool, quiet_mode: bool, idx: int, total_checks: int):
     this_os = detect_os()
     status_symbol = check_status_symbol(result.status)
     colour = check_status_colour(result.status)
     if result.status != CheckStatus.PASS or not quiet_mode:
         print(f"{status_symbol} [{colour(result.name)}] {result.summary}")
         if result.status in (CheckStatus.FAIL, CheckStatus.PASS_WITH_WARNING):
             suggestion = get_most_specific_suggestion(this_os, result.suggestions)
             if suggestion:
                 print_suggestion_text(suggestion)
         if quiet_mode:
             print("")
 
     if quiet_mode:
-        print_progress_bar(idx + 1, total_checks)
+        print_progress_bar(early_exit, idx + 1, total_checks)
+    elif early_exit:
+        print("ⓘ  Exited early due to --fail-fast flag")
 
 
-def print_progress_bar(current: int, total: int):
-    end_char = "\r" if current < total else "\n"
-    print(progress_bar(current, total), end=end_char)
+def print_progress_bar(early_exit: bool, current: int, total: int):
+    end_char = "\n" if current == total or early_exit else "\r"
+    print(progress_bar(current, total, early_exit), end=end_char)
 
 
-def progress_bar(current: int, total: int) -> str:
+def progress_bar(current: int, total: int, early_exit: bool) -> str:
     fraction = current / total
 
-    arrow = int(fraction * 25 - 1) * "-" + ">"
+    arrow_head = "x" if early_exit else ">"
+    arrow = int(fraction * 25 - 1) * "-" + arrow_head
     padding = int(25 - len(arrow)) * " "
 
     return f"Progress: [{arrow}{padding}] {int(fraction*100)}%  ({current}/{total})"
```

### Comparing `daktari-0.0.97/daktari/test_check.py` & `daktari-0.0.98/daktari/test_check.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/test_check_factory.py` & `daktari-0.0.98/daktari/test_check_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from daktari.check import Check, CheckResult
 
 
 class DummyCheck(Check):
-    def __init__(self, name: str = "check.name", depends_on=None):
+    def __init__(self, name: str = "check.name", depends_on=None, succeed: bool = True):
         if depends_on is None:
             depends_on = []
         self.name = name
         self.depends_on = depends_on
+        self.was_run = False
+        self.succeed = succeed
+
+    def check(self) -> CheckResult:
+        self.was_run = True
+        return self.verify(self.succeed, "dummy check")
+
+
+class ExplodingCheck(Check):
+    name = "exploding.check"
 
     def check(self) -> CheckResult:
-        return self.passed("no check")
+        raise Exception("boom")
 
 
 class DummyCheck2(Check):
     def __init__(self, name: str = "check.name", depends_on=None):
         if depends_on is None:
             depends_on = []
         self.name = name
```

### Comparing `daktari-0.0.97/daktari/test_check_sorter.py` & `daktari-0.0.98/daktari/test_check_sorter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/test_check_utils.py` & `daktari-0.0.98/daktari/test_check_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/test_config.py` & `daktari-0.0.98/daktari/test_config.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/test_version_utils.py` & `daktari-0.0.98/daktari/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari/version_utils.py` & `daktari-0.0.98/daktari/version_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/daktari.egg-info/PKG-INFO` & `daktari-0.0.98/daktari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daktari
-Version: 0.0.97
+Version: 0.0.98
 Summary: Assist in setting up and maintaining developer environments
 Home-page: https://github.com/sonocent/daktari
 Author: Matt Russell
 Author-email: matthew.russell@sonocent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.97"
+version = "0.0.98"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.97/daktari.egg-info/SOURCES.txt` & `daktari-0.0.98/daktari.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 daktari/file_utils.py
 daktari/options.py
 daktari/os.py
 daktari/resource_utils.py
 daktari/result_printer.py
 daktari/test_check.py
 daktari/test_check_factory.py
+daktari/test_check_runner.py
 daktari/test_check_sorter.py
 daktari/test_check_utils.py
 daktari/test_collection_utils.py
 daktari/test_config.py
 daktari/test_result_printer.py
 daktari/test_version_utils.py
 daktari/version_utils.py
```

### Comparing `daktari-0.0.97/requirements.txt` & `daktari-0.0.98/requirements.txt`

 * *Files identical despite different names*

### Comparing `daktari-0.0.97/setup.py` & `daktari-0.0.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="daktari",
-    version="0.0.97",
+    version="0.0.98",
     description="Assist in setting up and maintaining developer environments",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Matt Russell",
     author_email="matthew.russell@sonocent.com",
     url="https://github.com/sonocent/daktari",
```

