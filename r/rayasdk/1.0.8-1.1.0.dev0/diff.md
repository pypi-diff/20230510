# Comparing `tmp/rayasdk-1.0.8.tar.gz` & `tmp/rayasdk-1.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rayasdk-1.0.8.tar", last modified: Fri Jul 15 03:08:33 2022, max compression
+gzip compressed data, was "rayasdk-1.1.0.dev0.tar", last modified: Tue May  9 21:23:14 2023, max compression
```

## Comparing `rayasdk-1.0.8.tar` & `rayasdk-1.1.0.dev0.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2022-07-15 03:08:33.148542 rayasdk-1.0.8/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4355 2022-07-15 03:08:33.148542 rayasdk-1.0.8/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4010 2022-07-14 15:42:02.000000 rayasdk-1.0.8/README.md
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2022-07-15 03:08:33.148542 rayasdk-1.0.8/rayasdk/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      546 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/__init__.py
--rwxrwxr-x   0 camilo    (1000) camilo    (1000)     2879 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4359 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/connect.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3594 2022-07-14 15:42:02.000000 rayasdk-1.0.8/rayasdk/constants.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2022-07-15 03:08:33.148542 rayasdk-1.0.8/rayasdk/container_handlers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/container_handlers/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     9738 2022-07-15 03:06:48.000000 rayasdk-1.0.8/rayasdk/container_handlers/docker_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2870 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/initializer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      577 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/killer.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      785 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/logger.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2277 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/runner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1653 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/scanner.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      595 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/simulator.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2022-07-15 03:08:33.148542 rayasdk-1.0.8/rayasdk/template/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      244 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/template/__main__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      547 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/template/app.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      108 2022-07-11 21:44:43.000000 rayasdk-1.0.8/rayasdk/template/manifest.json
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2022-07-15 03:08:33.148542 rayasdk-1.0.8/rayasdk.egg-info/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4355 2022-07-15 03:08:33.000000 rayasdk-1.0.8/rayasdk.egg-info/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      581 2022-07-15 03:08:33.000000 rayasdk-1.0.8/rayasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2022-07-15 03:08:33.000000 rayasdk-1.0.8/rayasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       51 2022-07-15 03:08:33.000000 rayasdk-1.0.8/rayasdk.egg-info/entry_points.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       73 2022-07-15 03:08:33.000000 rayasdk-1.0.8/rayasdk.egg-info/requires.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        8 2022-07-15 03:08:33.000000 rayasdk-1.0.8/rayasdk.egg-info/top_level.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       79 2022-07-15 03:08:33.148542 rayasdk-1.0.8/setup.cfg
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      922 2022-07-15 03:06:48.000000 rayasdk-1.0.8/setup.py
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-09 21:23:14.772804 rayasdk-1.1.0.dev0/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      357 2023-05-09 21:23:14.772804 rayasdk-1.1.0.dev0/PKG-INFO
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        0 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/README.md
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-09 21:23:14.768804 rayasdk-1.1.0.dev0/rayasdk/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      546 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/__init__.py
+-rwxrwxr-x   0 santiagour  (1000) santiagour  (1000)     4569 2023-05-09 21:20:54.000000 rayasdk-1.1.0.dev0/rayasdk/__main__.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     5095 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/connect.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6161 2023-05-09 21:20:54.000000 rayasdk-1.1.0.dev0/rayasdk/constants.py
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-09 21:23:14.768804 rayasdk-1.1.0.dev0/rayasdk/container_handlers/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        0 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/container_handlers/__init__.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6326 2023-05-09 21:20:54.000000 rayasdk-1.1.0.dev0/rayasdk/container_handlers/docker_handler.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     9391 2023-05-09 21:20:54.000000 rayasdk-1.1.0.dev0/rayasdk/container_handlers/vcs.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     2398 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/initializer.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1358 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/killer.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1291 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/logger.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      822 2023-05-09 21:20:54.000000 rayasdk-1.1.0.dev0/rayasdk/messages.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     6371 2023-05-09 21:20:54.000000 rayasdk-1.1.0.dev0/rayasdk/runner.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     4187 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/scanner.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1671 2023-05-09 21:20:54.000000 rayasdk-1.1.0.dev0/rayasdk/simulator.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     2467 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/sshKeyGen.py
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-09 21:23:14.772804 rayasdk-1.1.0.dev0/rayasdk/template/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      244 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/template/__main__.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      547 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/template/app.py
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      399 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/template/launch.json
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      108 2023-05-04 20:26:47.000000 rayasdk-1.1.0.dev0/rayasdk/template/manifest.json
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     3113 2023-05-09 21:20:54.000000 rayasdk-1.1.0.dev0/rayasdk/utils.py
+drwxrwxr-x   0 santiagour  (1000) santiagour  (1000)        0 2023-05-09 21:23:14.768804 rayasdk-1.1.0.dev0/rayasdk.egg-info/
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      357 2023-05-09 21:23:14.000000 rayasdk-1.1.0.dev0/rayasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      702 2023-05-09 21:23:14.000000 rayasdk-1.1.0.dev0/rayasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        1 2023-05-09 21:23:14.000000 rayasdk-1.1.0.dev0/rayasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)       51 2023-05-09 21:23:14.000000 rayasdk-1.1.0.dev0/rayasdk.egg-info/entry_points.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)      103 2023-05-09 21:23:14.000000 rayasdk-1.1.0.dev0/rayasdk.egg-info/requires.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)        8 2023-05-09 21:23:14.000000 rayasdk-1.1.0.dev0/rayasdk.egg-info/top_level.txt
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)       79 2023-05-09 21:23:14.772804 rayasdk-1.1.0.dev0/setup.cfg
+-rw-rw-r--   0 santiagour  (1000) santiagour  (1000)     1002 2023-05-09 21:21:47.000000 rayasdk-1.1.0.dev0/setup.py
```

### Comparing `rayasdk-1.0.8/rayasdk/__init__.py` & `rayasdk-1.1.0.dev0/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.0.8/rayasdk/__main__.py` & `rayasdk-1.1.0.dev0/rayasdk/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,105 @@
-#!/usr/bin/env python
-
-# Copyright 2020 Unlimited Robotics
-
-import argparse
 import os
-import sys
-import platform
-
-from rayasdk.connect import URConnect
+import urllib
+import json 
+import tarfile
+import progressbar
+from simple_file_checksum import get_checksum
 
-from rayasdk.logger import log, LogLevels, log_error, log_verbose, set_logger_level
-from rayasdk.scanner import URScanner
-from rayasdk.initializer import URInitializer
-from rayasdk.runner import URRunner
-from rayasdk.simulator import URSimulator
-from rayasdk.killer import URKiller
+from rayasdk.messages import *
 from rayasdk.constants import *
+from rayasdk.logger import *
+from rayasdk.container_handlers.docker_handler import *
 
-from rayasdk.container_handlers.docker_handler import check_container
 
-class URSDK:
+class MyProgressBar:
     def __init__(self):
-        self.command_objects = []
-        self.command_objects.append(URInitializer())
-        self.command_objects.append(URScanner())
-        self.command_objects.append(URConnect())
-        self.command_objects.append(URRunner())
-        self.command_objects.append(URSimulator())
-        self.command_objects.append(URKiller())
-        self.init_parser()
-    
-    def init_parser(self):
-        # Init top parser
-        self.argparser = argparse.ArgumentParser(description='Unlimited Robotics SDK')
-        group = self.argparser.add_mutually_exclusive_group()
-        group.add_argument("-v", "--verbose", action="store_true", help="increase output verbosity.")
-        group.add_argument("-q", "--quiet", action="store_true", help="don't print on stdout.")
-        subparsers = self.argparser.add_subparsers(help='SDK Command', dest='command')
-        subparsers.required = True
-        # Init subparsers
-        for obj in self.command_objects:
-            obj.init_parser(subparsers)
-        # Parse arguments
-        self.args, self.unknownargs = self.argparser.parse_known_args()
-        # Setup Logger
-        set_logger_level(self.args.verbose, self.args.quiet)
-
-    def init_ursdk_folder(self):
-        if not os.path.exists(URSDK_TEMP_PATH):
-            log_verbose(f'Folder {URSDK_TEMP_PATH} does not exists, creating it.')
-            try:
-                os.mkdir(URSDK_TEMP_PATH)
-            except OSError as exc:
-                log_error(f'Folder {URSDK_TEMP_PATH} could not be created.')
-                return False
-            return True
+        self.pbar = None
+
+
+    def __call__(self, block_num, block_size, total_size):
+        if self.pbar is None:
+            self.pbar = progressbar.ProgressBar(maxval=total_size)
+            self.pbar.start()
+
+        downloaded = block_num * block_size
+        if downloaded < total_size:
+            self.pbar.update(downloaded)
         else:
-            log_verbose(f'Folder {URSDK_TEMP_PATH} found.')
-            return True
+            self.pbar.finish()           
 
-    def run(self):
-        if not self.init_ursdk_folder():
-            return False
-        if not check_container():
-            return False
-        for obj in self.command_objects:
-            if self.args.command == type(obj).COMMAND:
-                return obj.run(self.args, self.unknownargs)
-
-def main():
-    if platform.system() not in ['Linux', 'Windows']:
-        print(f'Platform \'{platform.system()}\' not supported.')
-        exit(1)
-    ursdk = URSDK()
-    ret = ursdk.run()
-    if not ret:
-        log_verbose('Finished with error.')
-        sys.exit(1)
-    else:
-        sys.exit(0)
+
+def run_simulator_bridge():
+    return launch_command()
 
 
-if __name__ == "__main__":
-    main()
+def download_simulator(response=None):
+    if response is not None:
+        # Get parameters from VCS API
+        for component in response:
+            if component['name'] == 'Unity':
+                response = component
+        sim_url = response["link"]
+        garysim_sha256 = response["checksum"]
+        version = response["versionId"]
+    else:
+        # Set parameters from local constants file 
+        sim_url = GARYSIM_URL
+        garysim_sha256 = GARYSIM_SHA256
+        version = GARYSIM_VERSION
+    log_info(f'Downloading Ra-Ya simulator v{version}...')
+    sim_tarpath = f'{SIMS_HOME}/simulator_{version}.tar.gz'
+    
+    try:
+        urllib.request.urlretrieve(sim_url, sim_tarpath, MyProgressBar())
+    except urllib.error.HTTPError:
+        log_error(f'Download error, the url {sim_url} does not exist.')
+        return False
+
+    log_info(f'Checking downloaded file...')
+    try:
+        sha256 = get_checksum(sim_tarpath, algorithm="SHA256")
+    except FileNotFoundError:
+        log_error('Download error, try again.')
+        return False
+    if garysim_sha256 != sha256:
+        log_error('Download error, try again.')
+        return False
+    
+    log_info(f'Extracting...')
+    simtar = tarfile.open(sim_tarpath)
+    simtar.extractall(SIMS_HOME)
+    os.remove(sim_tarpath)
+    return True
+
+
+def is_snake_case(s:str):
+    """
+    Returns True if s is in snake case, False otherwise.
+    """
+    if not s.islower():
+        return False
+    if '__' in s:
+        return False
+    if s.startswith('_') or s.endswith('_'):
+        return False
+    if not all(c.isalpha() or c.isdigit() or c == '_' for c in s):
+        return False
+    return True
+
+
+def validate_app_id_and_folder_name(app_id:str):
+    APP_MAIN_FOLDER_NAME = os.path.basename(os.path.normpath(CURRENT_PATH))
+    if APP_MAIN_FOLDER_NAME != app_id:
+        raise Exception('The app_id and the folder name are different')
+    if not is_snake_case(app_id):
+        raise Exception('The app_id have to be in snake case format')
+    return True
+
+
+def open_connection_file():
+    try:
+        with open(CONNECTION_SETTINGS_PATH, 'r', encoding='utf-8') as f:
+                connection_settings = json.load(f)
+        return connection_settings
+    except OSError as exc:
+            raise(f'the file "{CONNECTION_SETTINGS_FILE}" was not found, run rayasdk connect ')
```

### Comparing `rayasdk-1.0.8/rayasdk/connect.py` & `rayasdk-1.1.0.dev0/rayasdk/connect.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,125 @@
 # Copyright 2020 Unlimited Robotics
-import json
+import subprocess
 
-from rayasdk.container_handlers.docker_handler import scanner
+from rayasdk.sshKeyGen import SshKeyGen
 from rayasdk.logger import log_error, log_verbose, log_info
 from rayasdk.constants import *
 
+import json
+
+
 
 class URConnect:
 
     COMMAND = 'connect'
 
 
     def __init__(self):
         pass
 
 
     def init_parser(self, subparser):
-        self.parser = subparser.add_parser(type(self).COMMAND, help="execute current Raya project.")
+        self.parser = subparser.add_parser(
+                type(self).COMMAND, 
+                help="execute current Raya project."
+            )
         group = self.parser.add_mutually_exclusive_group(required=True)
-        group.add_argument('--robot-id', help='robot identificator (from scan list)', type=str)
-        group.add_argument('--simulator', help='connect the project to the simulator', action="store_true")
-
-
-    def robot_available(self, robot_id, domain, serial):
-        robots_info_dict = scanner(domain, domain, silent=True)
-        if robot_id not in robots_info_dict:
-            return False
-        if robots_info_dict[robot_id][JSON_SCAN_DDSCH] != domain:
-            return False
-        if robots_info_dict[robot_id][JSON_SCAN_SERIAL] != serial:
-            return False
-        return True
+        group.add_argument(
+                '--robot-id', 
+                help='robot identificator (from scan list)', 
+                type=str
+            )
+        group.add_argument(
+                '--robot-ip', 
+                help='robot ip (from scan list)', 
+                type=str
+            )
+        group.add_argument(
+                '--simulator', 
+                help='connect the project to the simulator', 
+                action="store_true"
+            )
 
 
     def run(self, args, unknownargs):
         self.args = args
         self.unknownargs = unknownargs
+
+        robot_id = self.args.robot_id
+        robot_ip = self.args.robot_ip
         try:
-            with open(EXECSETTINGS_PATH, 'r', encoding='utf-8') as f:
-                exec_settings = json.load(f)
-        except OSError as exc:
-            log_error(f'Could not open "{EXECSETTINGS_FILE}" file, no project initialized in this folder.')
-            return False
-        if self.args.simulator:
-            exec_settings[JSON_EXECINFO_SIM] = True
+            exec_settings = dict()
+            exec_settings[JSON_EXECINFO_SIM] = False
+            exec_settings[JSON_EXECINFO_ROBCONN] = dict()
             exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBID] = ''
             exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBIP] = ''
-            exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBDDSCH] = 0
-        else:
-            robot_id = self.args.robot_id
-            try:
+
+            if self.args.simulator:
+                exec_settings[JSON_EXECINFO_SIM] = True
+                log_info(f'You have successfully connected to the simulator')
+            else:
                 with open(LAST_SCANNING_PATH, 'r', encoding='utf-8') as f:
                     scanned_robots = json.load(f)
-            except OSError as exc:
-                log_error(f'Could  not get scanning info, execute "ursdk scan" before this command.')
-                return False
-            try:
-                if robot_id in scanned_robots:
-                    # check robot connected to the same serial and domain
-                    if self.robot_available(
-                                robot_id,
-                                scanned_robots[robot_id][JSON_SCAN_DDSCH],
-                                scanned_robots[robot_id][JSON_SCAN_SERIAL]
-                            ):
-                        # if robot exists, register it.
-                        exec_settings[JSON_EXECINFO_SIM] = False
-                        if JSON_EXECINFO_ROBCONN not in  exec_settings:
-                            exec_settings[JSON_EXECINFO_ROBCONN] = {}    
+                # Check if robot is in last scan
+                for robot in scanned_robots:
+                    if (robot_id and robot_id in scanned_robots[robot]["ROBOT_ID"]) or \
+                            (robot_ip and robot_ip in scanned_robots[robot]["ROBOT_IP"]):
+                        if JSON_EXECINFO_ROBCONN not in exec_settings:
+                            exec_settings[JSON_EXECINFO_ROBCONN] = {}
+
+                        if exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBID] != '':
+                            raise NameError((
+                                    f'\'{robot_id}\' was detected with '
+                                    'multiple IP addresses, connect using the'
+                                    ' \'--robot-ip\' argument instead.'
+                                ))
+
                         exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBID] = \
-                            robot_id
+                            scanned_robots[robot][JSON_SCAN_ID]
                         exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBIP] = \
-                            scanned_robots[robot_id][JSON_SCAN_IP]
-                        exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBDDSCH] = \
-                            scanned_robots[robot_id][JSON_SCAN_DDSCH]
+                            scanned_robots[robot][JSON_SCAN_IP]
                         exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBSERIAL] = \
-                            scanned_robots[robot_id][JSON_SCAN_SERIAL]
-                        log_info(f'You have successfully connected to {robot_id}')
+                            scanned_robots[robot][JSON_SCAN_SERIAL]
+
+                # If the robot was not found on the scan raise exception
+                if exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBID] == '':
+                    if robot_id:
+                        raise NameError(f'Robot ID "{robot_id}" not found in scan info, verify it or scan again.')
+                    elif robot_ip:
+                        raise NameError(f'Robot IP "{robot_ip}" not found in scan info, verify it or scan again.')
                     else:
-                        log_error(f'{exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBID]} is not longer available')
-                else:
-                    log_error(f'Robot ID "{robot_id}" not found in scan info, verify it or scan again.')
-                    return False
-            except KeyError as e:
-                print(e)
-                log_error(f'Scanning info malformed, please scan again by running "rayasdk scan".')
-                return False
-        try:
-            with open(EXECSETTINGS_PATH, 'w', encoding='utf-8') as f:
-                json.dump(exec_settings, f, ensure_ascii=False, indent=4)
+                        raise KeyError('')
+
+                # Send ssh key to robot
+                SshKeyGen(
+                    user=SSH_USER,
+                    host=exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBIP],
+                    port=SSH_PORT
+                )
+                log_info(
+                    f'You have successfully connected to '
+                    f'{exec_settings[JSON_EXECINFO_ROBCONN][JSON_EXECINFO_ROBID]}'
+                )
+
+            # Save connection globally
+            with open(CONNECTION_SETTINGS_PATH, 'w', encoding='utf-8') as f:
+                settings = dict()
+                settings[JSON_EXECINFO_SIM] = exec_settings[JSON_EXECINFO_SIM]
+                settings[JSON_EXECINFO_ROBCONN] = exec_settings[JSON_EXECINFO_ROBCONN]
+                json.dump(settings, f, ensure_ascii=False, indent=4)
+
+
         except FileNotFoundError:
-            log_error(f'Could not write file "{EXECSETTINGS_FILE}".')
-            return False
+            raise Exception(f'Could not write file "{CONNECTION_SETTINGS_FILE}".')
+        except OSError:
+            raise Exception(f'Could not get scanning info, execute "rayasdk scan" before this command.')
+        except subprocess.SubprocessError:
+            raise Exception("SSH Key not send, Check if raya_os is running")
+        except NameError as error:
+            raise Exception(str(error))
+        except KeyError as error:
+            print(error)
+            raise Exception(f'Scanning info malformed, please scan again by running "rayasdk scan".')
 
         log_verbose('\nCorrect!')
         return True
```

### Comparing `rayasdk-1.0.8/rayasdk/logger.py` & `rayasdk-1.1.0.dev0/rayasdk/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,56 @@
 from enum import Enum
 
+
 verbose = False
 quiet = False
 
+
+class bcolors:
+    HEADER = '\033[95m'
+    OKBLUE = '\033[94m'
+    OKCYAN = '\033[96m'
+    OKGREEN = '\033[92m'
+    WARNING = '\033[93m'
+    FAIL = '\033[91m'
+    ENDC = '\033[0m'
+    BOLD = '\033[1m'
+    UNDERLINE = '\033[4m'
+
+
 class LogLevels(Enum):
     VERBOSE = 1
     INFO = 2
-    ERROR = 3
+    WARNING = 3
+    ERROR = 4
+
 
 def set_logger_level(_verbose, _quiet):
     global verbose, quiet
     verbose = _verbose
     quiet = _quiet
 
+
 def log(level, msg, end='\n', flush=False):
-    if not quiet:
-        if level==LogLevels.INFO or (level==LogLevels.VERBOSE and verbose):
+    if level==LogLevels.INFO or (level==LogLevels.VERBOSE and verbose):
+        if not quiet:
             print(msg, end=end, flush=flush)
-    if level==LogLevels.ERROR:
+    elif level==LogLevels.ERROR:
         print(msg, end=end, flush=flush)
+    elif level==LogLevels.WARNING:
+        print(msg, end=end, flush=flush)
+
 
 def log_verbose(msg, end='\n', flush=False):
     log(LogLevels.VERBOSE, msg, end=end, flush=flush)
 
+
 def log_info(msg, end='\n', flush=False):
     log(LogLevels.INFO, msg, end=end, flush=flush)
 
+
+def log_warning(msg, end='\n', flush=False):
+    log(LogLevels.WARNING, f'{bcolors.WARNING}WARNING:{bcolors.ENDC} {msg}', end=end, flush=flush)
+
+
 def log_error(msg, end='\n', flush=False):
-    log(LogLevels.ERROR, 'ERROR: '+msg, end=end, flush=flush)
+    log(LogLevels.ERROR, f'{bcolors.FAIL}ERROR:{bcolors.ENDC} {msg}', end=end, flush=flush)
```

### Comparing `rayasdk-1.0.8/rayasdk/template/app.py` & `rayasdk-1.1.0.dev0/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-1.0.8/rayasdk.egg-info/SOURCES.txt` & `rayasdk-1.1.0.dev0/rayasdk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 rayasdk/__init__.py
 rayasdk/__main__.py
 rayasdk/connect.py
 rayasdk/constants.py
 rayasdk/initializer.py
 rayasdk/killer.py
 rayasdk/logger.py
+rayasdk/messages.py
 rayasdk/runner.py
 rayasdk/scanner.py
 rayasdk/simulator.py
+rayasdk/sshKeyGen.py
+rayasdk/utils.py
 rayasdk.egg-info/PKG-INFO
 rayasdk.egg-info/SOURCES.txt
 rayasdk.egg-info/dependency_links.txt
 rayasdk.egg-info/entry_points.txt
 rayasdk.egg-info/requires.txt
 rayasdk.egg-info/top_level.txt
 rayasdk/container_handlers/__init__.py
 rayasdk/container_handlers/docker_handler.py
+rayasdk/container_handlers/vcs.py
 rayasdk/template/__main__.py
 rayasdk/template/app.py
+rayasdk/template/launch.json
 rayasdk/template/manifest.json
```

### Comparing `rayasdk-1.0.8/setup.py` & `rayasdk-1.1.0.dev0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='rayasdk',
     packages=find_packages(),
-    version='1.0.8',
+    version='1.1.0.dev0',
     license='MIT',
     description='Raya SDK - Unlimited Robotics Software Development Kit',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Unlimited Robotics',
     author_email='camilo@unlimited-robotics.com',
     url='',
@@ -21,15 +21,19 @@
     keywords = ['robotics', 'unlimited-robotics', 'gary'],
     install_requires=[
         'tabulate',
         'importlib_metadata',
         'tqdm',
         'docker',
         'progressbar',
-        'simple_file_checksum'
+        'simple_file_checksum', 
+        'gsutil',
+        'zeroconf',
+        'raya',
+        'paramiko'
     ],
     entry_points={
         'console_scripts': [
             'rayasdk = rayasdk.__main__:main',
         ],
     },
 )
```

