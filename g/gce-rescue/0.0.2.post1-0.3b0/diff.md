# Comparing `tmp/gce-rescue-0.0.2.post1.tar.gz` & `tmp/gce-rescue-0.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gce-rescue-0.0.2.post1.tar", last modified: Fri Dec 16 15:25:06 2022, max compression
+gzip compressed data, was "gce-rescue-0.3b0.tar", last modified: Wed May 10 13:44:37 2023, max compression
```

## Comparing `gce-rescue-0.0.2.post1.tar` & `gce-rescue-0.3b0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 halleysouza (863006) primarygroup (89939)        0 2022-12-16 15:25:06.077341 gce-rescue-0.0.2.post1/
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)    11357 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/LICENSE
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     8343 2022-12-16 15:25:06.077170 gce-rescue-0.0.2.post1/PKG-INFO
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     7593 2022-12-16 15:00:57.000000 gce-rescue-0.0.2.post1/README.md
-drwxr-xr-x   0 halleysouza (863006) primarygroup (89939)        0 2022-12-16 15:25:06.067492 gce-rescue-0.0.2.post1/gce_rescue/
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)        0 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/__init__.py
-drwxr-xr-x   0 halleysouza (863006) primarygroup (89939)        0 2022-12-16 15:25:06.067784 gce-rescue-0.0.2.post1/gce_rescue/bin/
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)        0 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/bin/__init__.py
--rwxr-xr-x   0 halleysouza (863006) primarygroup (89939)     3128 2022-12-16 15:23:35.000000 gce-rescue-0.0.2.post1/gce_rescue/bin/rescue.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1180 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/config.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1601 2022-12-16 15:02:10.000000 gce-rescue-0.0.2.post1/gce_rescue/messages.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1292 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/messages_test.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1190 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/multitasks.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1659 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/multitasks_test.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     4477 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/rescue.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     2234 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/rescue_test.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1082 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/startup-script.txt
-drwxr-xr-x   0 halleysouza (863006) primarygroup (89939)        0 2022-12-16 15:25:06.074635 gce-rescue-0.0.2.post1/gce_rescue/tasks/
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)        0 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/__init__.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     2917 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/actions.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1881 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/backup.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1373 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/backup_test.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     6028 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/disks.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     2354 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/disks_test.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     2694 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/metadata.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1442 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/metadata_test.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1615 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/operations.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1290 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/operations_test.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1544 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/pre_validations.py
-drwxr-xr-x   0 halleysouza (863006) primarygroup (89939)        0 2022-12-16 15:25:06.075115 gce-rescue-0.0.2.post1/gce_rescue/tasks/validations/
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)        0 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/validations/__init__.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     2643 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/tasks/validations/authentication.py
-drwxr-xr-x   0 halleysouza (863006) primarygroup (89939)        0 2022-12-16 15:25:06.075464 gce-rescue-0.0.2.post1/gce_rescue/test/
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)        0 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/test/__init__.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1943 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/test/mocks.py
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     5706 2022-11-24 15:32:29.000000 gce-rescue-0.0.2.post1/gce_rescue/utils.py
-drwxr-xr-x   0 halleysouza (863006) primarygroup (89939)        0 2022-12-16 15:25:06.076935 gce-rescue-0.0.2.post1/gce_rescue.egg-info/
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     8343 2022-12-16 15:25:05.000000 gce-rescue-0.0.2.post1/gce_rescue.egg-info/PKG-INFO
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)     1098 2022-12-16 15:25:06.000000 gce-rescue-0.0.2.post1/gce_rescue.egg-info/SOURCES.txt
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)        1 2022-12-16 15:25:05.000000 gce-rescue-0.0.2.post1/gce_rescue.egg-info/dependency_links.txt
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)       58 2022-12-16 15:25:06.000000 gce-rescue-0.0.2.post1/gce_rescue.egg-info/entry_points.txt
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)        1 2022-12-16 15:25:05.000000 gce-rescue-0.0.2.post1/gce_rescue.egg-info/not-zip-safe
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)       52 2022-12-16 15:25:06.000000 gce-rescue-0.0.2.post1/gce_rescue.egg-info/requires.txt
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)       11 2022-12-16 15:25:06.000000 gce-rescue-0.0.2.post1/gce_rescue.egg-info/top_level.txt
--rw-r--r--   0 halleysouza (863006) primarygroup (89939)       38 2022-12-16 15:25:06.077391 gce-rescue-0.0.2.post1/setup.cfg
--rwxr-xr-x   0 halleysouza (863006) primarygroup (89939)     2146 2022-12-16 15:22:06.000000 gce-rescue-0.0.2.post1/setup.py
+drwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:37.425732 gce-rescue-0.3b0/
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)    11357 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/LICENSE
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     8584 2023-05-10 13:44:37.425732 gce-rescue-0.3b0/PKG-INFO
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     7629 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/README.md
+drwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:37.417731 gce-rescue-0.3b0/gce_rescue/
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/__init__.py
+drwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:37.417731 gce-rescue-0.3b0/gce_rescue/bin/
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/bin/__init__.py
+-rwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)     2359 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/bin/rescue.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     2067 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/config.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     6201 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/gce.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     2231 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/gce_test.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1614 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/messages.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1289 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/messages_test.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1082 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/startup-script.txt
+drwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:37.421731 gce-rescue-0.3b0/gce_rescue/tasks/
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/__init__.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     2905 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/actions.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1888 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/backup.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1370 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/backup_test.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     6047 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/disks.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     2351 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/disks_test.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1844 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/keeper.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     2701 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/metadata.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1414 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/metadata_test.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1619 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/operations.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1287 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/operations_test.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1716 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/pre_validations.py
+drwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:37.421731 gce-rescue-0.3b0/gce_rescue/tasks/validations/
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/validations/__init__.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1628 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/validations/api.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     2754 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/validations/authentication.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1560 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/tasks/validations/authorization.py
+drwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:37.421731 gce-rescue-0.3b0/gce_rescue/test/
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/test/__init__.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1943 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/test/mocks.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     3568 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/utils.py
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1675 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/gce_rescue/utils_test.py
+drwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)        0 2023-05-10 13:44:37.421731 gce-rescue-0.3b0/gce_rescue.egg-info/
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     8584 2023-05-10 13:44:37.000000 gce-rescue-0.3b0/gce_rescue.egg-info/PKG-INFO
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)     1175 2023-05-10 13:44:37.000000 gce-rescue-0.3b0/gce_rescue.egg-info/SOURCES.txt
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)        1 2023-05-10 13:44:37.000000 gce-rescue-0.3b0/gce_rescue.egg-info/dependency_links.txt
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)       58 2023-05-10 13:44:37.000000 gce-rescue-0.3b0/gce_rescue.egg-info/entry_points.txt
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)        1 2023-05-10 13:44:37.000000 gce-rescue-0.3b0/gce_rescue.egg-info/not-zip-safe
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)       52 2023-05-10 13:44:37.000000 gce-rescue-0.3b0/gce_rescue.egg-info/requires.txt
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)       11 2023-05-10 13:44:37.000000 gce-rescue-0.3b0/gce_rescue.egg-info/top_level.txt
+-rw-r--r--   0 halleysouza  (1000) halleysouza  (1001)       38 2023-05-10 13:44:37.425732 gce-rescue-0.3b0/setup.cfg
+-rwxr-xr-x   0 halleysouza  (1000) halleysouza  (1001)     2374 2023-05-10 13:44:21.000000 gce-rescue-0.3b0/setup.py
```

### Comparing `gce-rescue-0.0.2.post1/LICENSE` & `gce-rescue-0.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `gce-rescue-0.0.2.post1/PKG-INFO` & `gce-rescue-0.3b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: gce-rescue
-Version: 0.0.2.post1
+Version: 0.3b0
 Summary: GCE Rescue - Boot your GCE VM in rescue mode.
 Home-page: https://github.com/googlecloudplatform/gce-rescue
 Author: Halley de Souza
 Author-email: gce-rescue-dev@google.com
 License: Apache-2.0
-Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Boot
 Classifier: Topic :: System :: Boot :: Init
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: System :: Systems Administration
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -117,18 +121,18 @@
 ```shellscript
 $ gce-rescue --zone europe-central2-a --name test
 
 This option will boot the instance test in RESCUE MODE.
 If your instance is running it will be rebooted.
 Do you want to continue [y/N]: y
 Starting...
-- Configuring...
- \- Progress 6/6 [█████████████████████████████████████████████████████████████]
-- Configurations finished.
-- Your instance is READY! You can now connect your instance "test" via:
+┌── Configuring...
+│   └── Progress 6/6 [█████████████████████████████████████████████████████████████]
+├── Configurations finished.
+└── Your instance is READY! You can now connect your instance "test" via:
   1. CLI. (add --tunnel-through-iap if necessary)
     $ gcloud compute ssh test --zone=europe-central2-a --project=my-project --ssh-flag="-o StrictHostKeyChecking=no"
   OR
   2. Google Cloud Console:
     https://ssh.cloud.google.com/v2/ssh/projects/my-project/zones/europe-central2-a/instances/test?authuser=0&hl=en_US&useAdminProxy=true&troubleshoot4005Enabled=true
 
 ```
```

### Comparing `gce-rescue-0.0.2.post1/README.md` & `gce-rescue-0.3b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,18 @@
 ```shellscript
 $ gce-rescue --zone europe-central2-a --name test
 
 This option will boot the instance test in RESCUE MODE.
 If your instance is running it will be rebooted.
 Do you want to continue [y/N]: y
 Starting...
-- Configuring...
- \- Progress 6/6 [█████████████████████████████████████████████████████████████]
-- Configurations finished.
-- Your instance is READY! You can now connect your instance "test" via:
+┌── Configuring...
+│   └── Progress 6/6 [█████████████████████████████████████████████████████████████]
+├── Configurations finished.
+└── Your instance is READY! You can now connect your instance "test" via:
   1. CLI. (add --tunnel-through-iap if necessary)
     $ gcloud compute ssh test --zone=europe-central2-a --project=my-project --ssh-flag="-o StrictHostKeyChecking=no"
   OR
   2. Google Cloud Console:
     https://ssh.cloud.google.com/v2/ssh/projects/my-project/zones/europe-central2-a/instances/test?authuser=0&hl=en_US&useAdminProxy=true&troubleshoot4005Enabled=true
 
 ```
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/bin/rescue.py` & `gce-rescue-0.3b0/gce_rescue/bin/rescue.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,50 +13,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Main script to be used to set/reset rescue mode. """
 
 from datetime import datetime
-import argparse
 import logging
 
+from gce_rescue.config import process_args, set_configs
 from gce_rescue import messages
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 from gce_rescue.tasks.actions import call_tasks
 from gce_rescue.utils import read_input, set_logging
 
-def usage():
-  """ Print usage options. """
-  parser = argparse.ArgumentParser(description='GCE Rescue v0.0.2-1 - Set/Reset\
-    GCE instances to boot in rescue mode.')
-  parser.add_argument('-p', '--project',
-                      help='The project-id that has the instance.')
-  parser.add_argument('-z', '--zone', help='Zone where the instance \
-    is created.',
-                      required=True)
-  parser.add_argument('-n', '--name', help='Instance name.', required=True)
-  parser.add_argument('-d', '--debug', action='store_true',
-                      help='Print to the log file in debug leve')
-  parser.add_argument('-f', '--force', action='store_true',
-                      help='Don\'t ask for confirmation.')
-
-  return parser
-
 def main():
   """ Main script function. """
-  parser = usage()
+  parser = process_args()
   args = parser.parse_args()
+  set_configs(args)
 
-  if args.debug:
-    log_level = 'DEBUG'
-  else:
-    log_level = 'INFO'
-
-  set_logging(vm_name=args.name, level=log_level)
+  set_logging(vm_name=args.name)
 
   parse_kwargs = {
       'zone': args.zone,
       'name': args.name,
   }
 
   if args.project:
@@ -92,8 +71,8 @@
     msg = messages.tip_restore_disk(vm)
 
   call_tasks(vm=vm, action=action)
   print(msg)
 
 
 if __name__ == '__main__':
-  main()
+  main()
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/messages.py` & `gce-rescue-0.3b0/gce_rescue/messages.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ List of messages to inform and educate the user. """
 
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 
 def tip_connect_ssh(vm: Instance) -> str:
-  return (f'- Your instance is READY! You can now connect your instance '
+  return (f'└── Your instance is READY! You can now connect your instance '
     f' {vm.name} via:\n  1. CLI. (add --tunnel-through-iap if necessary)\n'
     f'    $ gcloud compute ssh {vm.name} --zone={vm.zone} '
     f'--project={vm.project} --ssh-flag="-o StrictHostKeyChecking=no"\n  OR\n'
     f'  2. Google Cloud Console:\n'
     f'    https://ssh.cloud.google.com/v2/ssh/projects/{vm.project}/zones/'
     f'{vm.zone}/instances/{vm.name}?authuser=0&hl=en_US&useAdminProxy=true&'
     f'troubleshoot4005Enabled=true\n')
 
 def tip_restore_disk(vm: Instance) -> str:
-  return (f'- The instance {vm.name} was restored! Use the snapshot below '
+  return (f'└── The instance {vm.name} was restored! Use the snapshot below '
     f'if you need to restore the modification made while the instance was '
     f'in rescue mode.\n Snapshot name: {vm.disks["disk_name"]}-{vm.ts}\n'
     f' More information: '
     f'https://cloud.google.com/compute/docs/disks/restore-snapshot\n')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/messages_test.py` & `gce-rescue-0.3b0/gce_rescue/messages_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Test code for messages.py. """
 
 from absl.testing import absltest
 from gce_rescue import messages
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 from gce_rescue.test.mocks import mock_api_object, MOCK_TEST_VM
 
 
 class MessagesTest(absltest.TestCase):
   vm: Instance
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/multitasks_test.py` & `gce-rescue-0.3b0/gce_rescue/utils_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Multitask test code """
 
 from absl.testing import absltest
-from gce_rescue.multitasks import Handler
+from gce_rescue.utils import ThreadHandler as Handler
 import time
 
 OUTPUT1 = 'task1 done'
 OUTPUT2 = 'task1 done'
 
 
 class MultitasksTest(absltest.TestCase):
@@ -27,25 +27,25 @@
 	  'task1_done': False,
 	  'task2_done': False,
 	}
 
 
   @classmethod
   def task1(cls):
-    for i in range(0, 3):
-      print(f'task 1, time {i}')
+    for _ in range(0, 3):
+      # print(f'task 1, time {i}')
       time.sleep(0.001)
     MultitasksTest.status['task1_done'] = True
     return OUTPUT1
 
 
   @classmethod
   def task2(cls):
-    for i in range(0, 3):
-      print(f'task 2, time {i}')
+    for _ in range(0, 3):
+      # print(f'task 2, time {i}')
       time.sleep(0.001)
     MultitasksTest.status['task2_done'] = True
     return OUTPUT2
 
 
   def test_multitasks(self):
     t1 = Handler(target=MultitasksTest.task1)
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/rescue_test.py` & `gce-rescue-0.3b0/gce_rescue/gce_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Test code for rescue.py."""
 
 from absl.testing import absltest
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 from gce_rescue.test.mocks import (
   mock_api_object,
   MOCK_TEST_VM,
   MOCK_TEST_DATA
 )
 
 class RescueTest(absltest.TestCase):
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/startup-script.txt` & `gce-rescue-0.3b0/gce_rescue/startup-script.txt`

 * *Files identical despite different names*

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/actions.py` & `gce-rescue-0.3b0/gce_rescue/tasks/actions.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ List of ordered tasks to be executed when set/reset VM rescue mode. """
 
-from typing import Dict
+from typing import List
 import logging
 
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 from gce_rescue.tasks.disks import (
   config_rescue_disks,
   restore_original_disk,
   attach_disk
 )
 from gce_rescue.tasks.operations import (
   start_instance,
@@ -31,15 +31,15 @@
   set_metadata,
   restore_metadata_items
 )
 from gce_rescue.utils import Tracker
 
 _logger = logging.getLogger(__name__)
 
-def _list_tasks(vm: Instance, action: str) -> Dict:
+def _list_tasks(vm: Instance, action: str) -> List:
   """ List tasks, by order, per operation
     operations (str):
       1. set_rescue_mode
       2. reset_rescue_mode
   """
   all_tasks = {
     'set_rescue_mode': [
@@ -109,15 +109,15 @@
         }]
       },
     ]
   }
 
   if action not in all_tasks:
     _logger.info(f'Unable to find "{action}".')
-    raise Exception(ValueError)
+    raise ValueError()
   return all_tasks[action]
 
 
 def call_tasks(vm: Instance, action: str) -> None:
   """ Loop tasks dict and execute """
   tasks = _list_tasks(vm = vm, action = action)
   total_tasks = len(tasks)
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/backup.py` & `gce-rescue-0.3b0/gce_rescue/tasks/backup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Different operations to guarantee VM disks backup, before performing
     any modifications."""
 
-from gce_rescue.utils import wait_for_operation
+from gce_rescue.tasks.keeper import wait_for_operation
 from typing import Dict, List
 import logging
 
 _logger = logging.getLogger(__name__)
 
 def backup_metadata_items(data: Dict) -> List:
   """ Returns the "items" content (ssh-keys, scripts, etc) to be restored
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/backup_test.py` & `gce-rescue-0.3b0/gce_rescue/tasks/backup_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Test code for backup.py."""
 
 from absl.testing import absltest
 from gce_rescue.tasks import backup
 from gce_rescue.test.mocks import mock_api_object, MOCK_TEST_VM
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 
 
 class BackupTest(absltest.TestCase):
   vm : Instance
 
 
   def setUp(self):
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/disks.py` & `gce-rescue-0.3b0/gce_rescue/tasks/disks.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 """ Compilations of all disks tasks related. """
 
 from typing import Dict
 import logging
 
 import googleapiclient.errors
 
-from gce_rescue.utils import wait_for_operation
+from gce_rescue.tasks.keeper import wait_for_operation
 from gce_rescue.tasks.backup import  backup
-from gce_rescue.multitasks import Handler
+from gce_rescue.utils import ThreadHandler as Handler
 
 _logger = logging.getLogger(__name__)
 
 def _create_rescue_disk(vm, source_disk: str) -> Dict:
   """ Create new temporary rescue disk based on source_disk.
   https://cloud.google.com/compute/docs/reference/rest/v1/disks/insert
   Returns:
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/disks_test.py` & `gce-rescue-0.3b0/gce_rescue/tasks/disks_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Test code for disks.py."""
 
 from absl.testing import absltest
 from absl import logging
 
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 from gce_rescue.tasks import disks
 from gce_rescue.test.mocks import (
   mock_api_object,
   MOCK_TEST_VM,
   MOCK_TEST_DATA,
 )
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/metadata.py` & `gce-rescue-0.3b0/gce_rescue/tasks/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Different functions to modify VM custom metadata. """
 
 from gce_rescue.config import get_config
-from gce_rescue.utils import wait_for_operation, wait_for_os_boot
+from gce_rescue.tasks.keeper import wait_for_operation, wait_for_os_boot
 from typing import Dict
 import logging
 
 _logger = logging.getLogger(__name__)
 
 def set_metadata(vm) -> Dict:
   """Configure Instance custom metadata.
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/metadata_test.py` & `gce-rescue-0.3b0/gce_rescue/tasks/metadata_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Test code for metadata.py."""
 
 from absl.testing import absltest
-from absl import logging
 
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 from gce_rescue.tasks import metadata
 from gce_rescue.test.mocks import  mock_api_object, MOCK_TEST_VM
 
 
 class MetadataTest(absltest.TestCase):
   def setUp(self):
     self.vm = Instance(test_mode=True, **MOCK_TEST_VM)
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/operations.py` & `gce-rescue-0.3b0/gce_rescue/tasks/operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Standard VM operations. """
 
-from gce_rescue.rescue import Instance
-from gce_rescue.utils import wait_for_operation
+from gce_rescue.gce import Instance
+from gce_rescue.tasks.keeper import wait_for_operation
 import logging
 
 _logger = logging.getLogger(__name__)
 
 def start_instance(vm: Instance) -> str:
   """Start instance."""
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/operations_test.py` & `gce-rescue-0.3b0/gce_rescue/tasks/operations_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Test code for operations.py."""
 
 from absl.testing import absltest
-from gce_rescue.rescue import Instance
+from gce_rescue.gce import Instance
 from gce_rescue.tasks.operations import start_instance, stop_instance
 from gce_rescue.test.mocks import mock_api_object, MOCK_TEST_VM
 
 
 class OperationsTest(absltest.TestCase):
   vm: Instance
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/pre_validations.py` & `gce-rescue-0.3b0/gce_rescue/tasks/pre_validations.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """ Validations that should be performed before continue the script execution.
     Each validations steps can be appended to the class Validations() and keep
     the file under validations/ folder."""
 
 from dataclasses import dataclass, field
 import googleapiclient.discovery
+from gce_rescue.tasks.validations.authorization import authorize_check
 from gce_rescue.tasks.validations.authentication import (
   authenticate_check,
   project_name
 )
 
 @dataclass
 class Validations:
@@ -38,14 +39,18 @@
     return authenticate_check(
       project = self.project,
       zone = self.zone,
       instance_name = self.name,
       test_mode = self.test_mode,
     )
 
+  def __post_init__(self):
+    if not self.test_mode:
+      authorize_check(project = self.project)
+
   @property
   def compute(self) -> googleapiclient.discovery.Resource:
     return self._authentication()
 
   @property
   def adc_project(self) -> str:
     return project_name()
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/tasks/validations/authentication.py` & `gce-rescue-0.3b0/gce_rescue/tasks/validations/authentication.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Authentication validation to be called from ../pre_validations.py """
-import googleapiclient.discovery
 import google.auth
 import sys
+
+from googleapiclient.discovery import Resource
+from gce_rescue.tasks.validations.api import api_service
 from gce_rescue.test.mocks import mock_api_object
 
 PROJECT = ''
 
 def _get_auth():
   global PROJECT
   try:
@@ -37,28 +39,29 @@
     sys.exit(1)
 
 def authenticate_check(
   zone: str,
   instance_name: str,
   project: str = None,
   test_mode: bool = False
-) -> googleapiclient.discovery.Resource:
+) -> Resource:
   global PROJECT
   PROJECT = project
   if test_mode:
     service = mock_api_object(['compute'])
     return service
   credentials = _get_auth()
   if not credentials:
     return False
-  service = googleapiclient.discovery.build(
-    'compute',
-    'v1',
-    credentials = credentials
-  )
+  # service = googleapiclient.discovery.build(
+  #   'compute',
+  #   'v1',
+  #   credentials = credentials
+  # )
+  service =  api_service('compute', 'v1', credentials)
   request = service.instances().get(
 		project = PROJECT,
 		zone = zone,
 		instance = instance_name)
   try:
     request.execute()
     return service
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/test/mocks.py` & `gce-rescue-0.3b0/gce_rescue/test/mocks.py`

 * *Files identical despite different names*

### Comparing `gce-rescue-0.0.2.post1/gce_rescue/utils.py` & `gce-rescue-0.3b0/gce_rescue/gce.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,90 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-""" List of classes and functions to be used across the code. """
+""" Initilization Instance() with VM information. """
 
-import googleapiclient.discovery
+from googleapiclient.discovery import Resource
 
-from time import time, sleep
-from typing import Dict
+from dataclasses import dataclass, field
+from typing import Dict, List, Union
+from time import time
+from gce_rescue.tasks.backup import backup_metadata_items
+from gce_rescue.tasks.disks import list_disk
+from gce_rescue.tasks.pre_validations import Validations
 from gce_rescue.config import get_config
-import logging
-import multiprocessing
-import sys
-import json
-
-_logger = logging.getLogger(__name__)
-
-class Tracker():
-  """ Track tasks using multiprocessing and print progress bar. """
-
-  def __init__(self, target):
-    self.target = target
-    self._pivot = multiprocessing.Value('i', 1)
-    self._proc = None
-
-  def start(self):
-    self._proc = multiprocessing.Process(target=self._run)
-    self._proc.start()
-    print('- Configuring...')
-
-  def advance(self, step=None):
-    if not step:
-      step = 1
-    self._pivot.value += step
-
-  def finish(self):
-    self._pivot.value = self.target
-    self._proc.join()
-    sleep(0.5)
-    print('- Configurations finished.')
-
-  def _loading(self):
-    chars = ['-', '|', '/', '|', '\\']
-    i = 0
-    while True:
-      yield chars[i]
-      i += 1
-      if i == len(chars):
-        i = 0
-
-  def _run(self):
-    self._gen = self._loading()
-    while self._pivot.value < self.target:
-      try:
-        sleep(0.001)
-        self._print()
-      except Exception as exc:
-        raise f'{exc}: {self._pivot.value} = {self.target}'
-
-    self._print()
-    print('\r')
-
-  def _print(self):
-    size = 60
-    loading = next(self._gen)
-    if self._pivot.value == self.target:
-      loading = '█'
-    count = self._pivot.value
-    total = self.target
-    x = int(size * self._pivot.value / self.target)
-    progress = '█' * x
-    bar = '.' * (size-x)
-    print(f' \\- Progress {count}/{total} [{progress}{loading}{bar}]',
-      end='\r',
-      file=sys.stderr,
-      flush=True)
+
 
 def get_instance_info(
-  compute: googleapiclient.discovery.Resource,
+  compute: Resource,
   name: str,
   project_data: Dict[str, str]
 ) -> Dict:
   """Set Dictionary with complete data from instances().get() from the instance.
   https://cloud.google.com/compute/docs/reference/rest/v1/instances/get
   Attributes:
     compute: obj, API Object
@@ -99,36 +38,14 @@
     project_data: dict, Dictionary containing project and zone keys to be
       unpacked when calling the API.
   """
   return compute.instances().get(
       **project_data,
       instance = name).execute()
 
-def generate_ts() -> int:
-  """Get the current timestamp to be used as unique ID
-  during this execution."""
-  return int(time())
-
-def validate_instance_mode(data: Dict) -> Dict:
-  """Validate if the instance is already configured as rescue mode."""
-
-  result = {
-      'rescue-mode': False,
-      'ts': generate_ts()
-  }
-  if 'metadata' in data and  'items' in data['metadata']:
-    metadata = data['metadata']
-    for item in metadata['items']:
-      if item['key'] == 'rescue-mode':
-        result = {
-          'rescue-mode': True,
-          'ts': item['value']
-        }
-
-  return result
 
 def guess_guest(data: Dict) -> str:
   """Determined which Guest OS Family is being used and select a
   different OS for recovery disk.
      Default: projects/debian-cloud/global/images/family/debian-11"""
 
   guests = get_config('source_guests')
@@ -142,68 +59,160 @@
       guest_name = guest_default.split('/')[-1]
       for lic in disk['licenses']:
         if guest_name in lic:
           guest_default = guests[arch][1]
   return guest_default
 
 
-def wait_for_operation(
-  instance_obj: googleapiclient.discovery.Resource,
-  oper: Dict
-) -> Dict:
-  """ Creating poll to wait the operation to finish. """
+def validate_instance_mode(data: Dict) -> Dict:
+  """Validate if the instance is already configured as rescue mode."""
+
+  result = {
+      'rescue-mode': False,
+      'ts': generate_ts()
+  }
+  if 'metadata' in data and  'items' in data['metadata']:
+    metadata = data['metadata']
+    for item in metadata['items']:
+      if item['key'] == 'rescue-mode':
+        result = {
+          'rescue-mode': True,
+          'ts': item['value']
+        }
+
+  return result
+
+def generate_ts() -> int:
+  """Get the current timestamp to be used as unique ID
+  during this execution."""
+  return int(time())
+
 
-  while True:
-    if oper['status'] == 'DONE':
-      _logger.info('done.')
-      if 'error' in oper:
-        raise Exception(oper['error'])
-      return oper
-
-    oper = instance_obj.compute.zoneOperations().get(
-      **instance_obj.project_data,
-      operation = oper['name']).execute()
-    sleep(1)
-
-def wait_for_os_boot(vm: googleapiclient.discovery.Resource) -> bool:
-  """Wait guest OS to complete the boot proccess."""
-
-  timeout = 60
-  wait_time = 2
-  end_string = f'END:{vm.ts}'
-  _logger.info('Waiting startup-script to complete.')
-  while True:
-    result = vm.compute.instances().getSerialPortOutput(
-      **vm.project_data,
-      instance = vm.name
-    ).execute()
-
-    if end_string in json.dumps(result):
-      _logger.info('startup-script has ended.')
-      return True
-
-    sleep(wait_time)
-    timeout -= wait_time
-    if not timeout:
-      return False
-
-
-def set_logging(vm_name: str, level: str ='INFO') -> None:
-  """ Set logfile and verbosity. """
-
-  log_level = getattr(logging, level.upper())
-  file_name = f'{vm_name}.log'
-  logging.basicConfig(
-    filename=file_name,
-    filemode='a',
-    format='%(asctime)s,%(msecs)03d %(levelname)-8s [%(filename)s:%(lineno)d]\
-      %(message)s',
-    datefmt='%Y-%m-%d:%H:%M:%S',
-    level=log_level)
-
-def read_input(msg: str) -> None:
-  """Read user input if --force is not provided."""
-  print(msg, end='')
-  input_answer = input()
-  if input_answer.upper() != 'Y':
-    print('Cancelled.')
-    sys.exit(1)
+@dataclass
+class Instance(Resource):
+  """Initialize instance."""
+  zone: str
+  name: str
+  project: str = None
+  test_mode: bool = field(default_factory=False)
+  compute: Resource = field(init=False)
+  data: Dict[str, Union[str, int]] = field(init=False)
+  ts: int = field(init=False)
+  _status: str = ''
+  _rescue_source_disk: str = ''
+  _rescue_mode_status: Dict[str, Union[str, int]] = field(
+    default_factory=lambda: ({})
+  )
+  _disks: Dict[str, str] = field(default_factory=lambda: ({}))
+  _backup_items: Dict[str, Union[str, int]] = field(
+    default_factory=lambda: ([])
+  )
+
+  def __post_init__(self):
+    check = Validations(
+        name=self.name,
+        test_mode=self.test_mode,
+        **self.project_data
+    )
+    self.compute = check.compute
+    self.project = check.adc_project
+    self.data = get_instance_info(
+        compute=self.compute,
+        name=self.name,
+        project_data=self.project_data)
+
+    self._rescue_mode_status = validate_instance_mode(self.data)
+    self.ts = self._rescue_mode_status['ts']
+    self._status = self.data['status']
+    self._rescue_source_disk = guess_guest(self.data)
+    self._disks = self._define_disks()
+
+    # Backup metadata items
+    self._backup_items = backup_metadata_items(
+        data=self.data
+    )
+
+  def refresh_fingerprint(self) -> None:
+    """Refresh the current metadata fingerprint value."""
+
+    project_data = get_instance_info(
+        compute=self.compute,
+        name=self.name,
+        project_data=self.project_data)
+
+    new_fingerprint = project_data['metadata']['fingerprint']
+    self.data['metadata']['fingerprint'] = new_fingerprint
+
+  def _define_disks(self) -> Dict[str, str]:
+    """Define the values of disk_name and device_name."""
+
+    rescue_on = self._rescue_mode_status['rescue-mode']
+    if not rescue_on:
+      for disk in self.data['disks']:
+        if disk['boot']:
+          device_name = disk['deviceName']
+          source = disk['source']
+          disk_name = source.split('/')[-1]
+
+    else:
+      ts = self._rescue_mode_status['ts']
+      disk_filter = f'labels.rescue={ts}'
+
+      disk = list_disk(
+        vm=self,
+        project_data=self.project_data,
+        label_filter=disk_filter
+      )
+
+      disk_name = disk[0]['name']
+      disks = self.data['disks']
+      for disk in disks:
+        full_source = disk['source']
+        source = full_source.split('/')[-1]
+        if disk_name == source:
+          device_name = disk['deviceName']
+
+    result = {
+        'device_name': device_name,
+        'disk_name': disk_name
+    }
+    return result
+
+  @property
+  def rescue_mode_status(self) -> Dict[str, Union[str, int]]:
+    return self._rescue_mode_status
+
+  @property
+  def project_data(self) -> str:
+    return {'project': self.project, 'zone': self.zone}
+
+  @property
+  def rescue_disk(self) -> str:
+    return f'linux-rescue-disk-{self.ts}'
+
+  @property
+  def status(self) -> str:
+    return self._status
+
+  @status.setter
+  def status(self, v: str) -> None:
+    self._status = v
+
+  @property
+  def rescue_source_disk(self) -> str:
+    return self._rescue_source_disk
+
+  @rescue_source_disk.setter
+  def rescue_source_disk(self, v: str) -> None:
+    self._rescue_source_disk = v
+
+  @property
+  def backup_items(self) -> List[str]:
+    return self._backup_items
+
+  @backup_items.setter
+  def backup_items(self, v: List[str]) -> None:
+    self._backup_items = v
+
+  @property
+  def disks(self) -> List[str]:
+    return self._disks
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue.egg-info/PKG-INFO` & `gce-rescue-0.3b0/gce_rescue.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: gce-rescue
-Version: 0.0.2.post1
+Version: 0.3b0
 Summary: GCE Rescue - Boot your GCE VM in rescue mode.
 Home-page: https://github.com/googlecloudplatform/gce-rescue
 Author: Halley de Souza
 Author-email: gce-rescue-dev@google.com
 License: Apache-2.0
-Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Boot
 Classifier: Topic :: System :: Boot :: Init
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: System :: Systems Administration
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -117,18 +121,18 @@
 ```shellscript
 $ gce-rescue --zone europe-central2-a --name test
 
 This option will boot the instance test in RESCUE MODE.
 If your instance is running it will be rebooted.
 Do you want to continue [y/N]: y
 Starting...
-- Configuring...
- \- Progress 6/6 [█████████████████████████████████████████████████████████████]
-- Configurations finished.
-- Your instance is READY! You can now connect your instance "test" via:
+┌── Configuring...
+│   └── Progress 6/6 [█████████████████████████████████████████████████████████████]
+├── Configurations finished.
+└── Your instance is READY! You can now connect your instance "test" via:
   1. CLI. (add --tunnel-through-iap if necessary)
     $ gcloud compute ssh test --zone=europe-central2-a --project=my-project --ssh-flag="-o StrictHostKeyChecking=no"
   OR
   2. Google Cloud Console:
     https://ssh.cloud.google.com/v2/ssh/projects/my-project/zones/europe-central2-a/instances/test?authuser=0&hl=en_US&useAdminProxy=true&troubleshoot4005Enabled=true
 
 ```
```

### Comparing `gce-rescue-0.0.2.post1/gce_rescue.egg-info/SOURCES.txt` & `gce-rescue-0.3b0/gce_rescue.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 LICENSE
 README.md
 setup.py
 ./gce_rescue/__init__.py
 ./gce_rescue/config.py
+./gce_rescue/gce.py
+./gce_rescue/gce_test.py
 ./gce_rescue/messages.py
 ./gce_rescue/messages_test.py
-./gce_rescue/multitasks.py
-./gce_rescue/multitasks_test.py
-./gce_rescue/rescue.py
-./gce_rescue/rescue_test.py
 ./gce_rescue/startup-script.txt
 ./gce_rescue/utils.py
+./gce_rescue/utils_test.py
 ./gce_rescue/bin/__init__.py
 ./gce_rescue/bin/rescue.py
 ./gce_rescue/tasks/__init__.py
 ./gce_rescue/tasks/actions.py
 ./gce_rescue/tasks/backup.py
 ./gce_rescue/tasks/backup_test.py
 ./gce_rescue/tasks/disks.py
 ./gce_rescue/tasks/disks_test.py
+./gce_rescue/tasks/keeper.py
 ./gce_rescue/tasks/metadata.py
 ./gce_rescue/tasks/metadata_test.py
 ./gce_rescue/tasks/operations.py
 ./gce_rescue/tasks/operations_test.py
 ./gce_rescue/tasks/pre_validations.py
 ./gce_rescue/tasks/validations/__init__.py
+./gce_rescue/tasks/validations/api.py
 ./gce_rescue/tasks/validations/authentication.py
+./gce_rescue/tasks/validations/authorization.py
 ./gce_rescue/test/__init__.py
 ./gce_rescue/test/mocks.py
 gce_rescue.egg-info/PKG-INFO
 gce_rescue.egg-info/SOURCES.txt
 gce_rescue.egg-info/dependency_links.txt
 gce_rescue.egg-info/entry_points.txt
 gce_rescue.egg-info/not-zip-safe
```

### Comparing `gce-rescue-0.0.2.post1/setup.py` & `gce-rescue-0.3b0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 # limitations under the License.
 
 """ Install GCE Rescue """
 
 from setuptools import setup, find_packages
 from os import path
 
+from gce_rescue.config import VERSION
+
 my_pwd = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(my_pwd, 'README.md'), encoding='utf-8') as f:
   long_description_readme = f.read()
 
 # Get requirements
 with open(path.join(my_pwd, 'requirements.txt'), encoding='utf-8') as f:
   list_requirements = f.readlines()
 
 setup(
   name = 'gce-rescue',
-  version = '0.0.2-1',
+  version = VERSION,
   description='GCE Rescue - Boot your GCE VM in rescue mode.',
   url = 'https://github.com/googlecloudplatform/gce-rescue',
   author = 'Halley de Souza',
   author_email = 'gce-rescue-dev@google.com',
   license = 'Apache-2.0',
   long_description = long_description_readme,
   long_description_content_type = 'text/markdown',
@@ -47,18 +49,22 @@
   include_package_data = True,
   entry_points={
         'console_scripts': [
             'gce-rescue = gce_rescue.bin.rescue:main',
         ],
     },
   classifiers = [
-    'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
-    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Topic :: System :: Boot',
     'Topic :: System :: Boot :: Init',
     'Topic :: System :: Recovery Tools',
     'Topic :: System :: System Shells',
     'Topic :: System :: Systems Administration',
   ]
 )
```

