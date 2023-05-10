# Comparing `tmp/nanolab-0.0.3.tar.gz` & `tmp/nanolab-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanolab-0.0.3.tar", last modified: Tue May  9 20:58:11 2023, max compression
+gzip compressed data, was "nanolab-0.0.4.tar", last modified: Wed May 10 19:38:38 2023, max compression
```

## Comparing `nanolab-0.0.3.tar` & `nanolab-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:58:11.171582 nanolab-0.0.3/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-09 20:58:11.171582 nanolab-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:58:11.167581 nanolab-0.0.3/nanolab/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 15:42:44.000000 nanolab-0.0.3/nanolab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:58:11.171582 nanolab-0.0.3/nanolab/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.3/nanolab/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-05-08 13:34:13.000000 nanolab-0.0.3/nanolab/command/command.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-07 13:42:34.000000 nanolab-0.0.3/nanolab/command/command_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:58:11.171582 nanolab-0.0.3/nanolab/command/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.3/nanolab/command/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-07 19:39:25.000000 nanolab-0.0.3/nanolab/command/mixins/base_mixin.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-05-09 15:37:47.000000 nanolab-0.0.3/nanolab/command/mixins/bash_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-07 19:31:15.000000 nanolab-0.0.3/nanolab/command/mixins/python_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-05-07 21:09:14.000000 nanolab-0.0.3/nanolab/command/mixins/snippet_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-08 09:49:17.000000 nanolab-0.0.3/nanolab/command/mixins/threaded_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-04-26 22:11:20.000000 nanolab-0.0.3/nanolab/decorators.py
--rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.3/nanolab/main.py
--rw-r--r--   0 root         (0) root         (0)    11028 2023-05-08 09:50:05.000000 nanolab-0.0.3/nanolab/node_interaction.py
--rw-r--r--   0 root         (0) root         (0)     6715 2023-05-09 20:51:58.000000 nanolab-0.0.3/nanolab/node_tools.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-05-04 21:39:19.000000 nanolab-0.0.3/nanolab/pycmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:58:11.171582 nanolab-0.0.3/nanolab/snippets/
--rw-r--r--   0 root         (0) root         (0)     2318 2023-05-09 15:33:56.000000 nanolab-0.0.3/nanolab/snippets/default_snips.json
--rw-r--r--   0 root         (0) root         (0)      984 2023-05-08 13:34:23.000000 nanolab-0.0.3/nanolab/snippets/test_snippets.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:58:11.171582 nanolab-0.0.3/nanolab/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.3/nanolab/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4489 2023-05-09 15:19:18.000000 nanolab-0.0.3/nanolab/src/argparse_commands.py
--rw-r--r--   0 root         (0) root         (0)     4998 2023-05-09 20:46:41.000000 nanolab-0.0.3/nanolab/src/config_handler.py
--rw-r--r--   0 root         (0) root         (0)     3891 2023-05-09 20:37:50.000000 nanolab-0.0.3/nanolab/src/config_loader.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-05-08 12:45:36.000000 nanolab-0.0.3/nanolab/src/github.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.3/nanolab/src/resolver.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-09 13:01:49.000000 nanolab-0.0.3/nanolab/src/snippet_manager.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-05-09 19:35:34.000000 nanolab-0.0.3/nanolab/src/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:58:11.171582 nanolab-0.0.3/nanolab/xnomin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.3/nanolab/xnomin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.3/nanolab/xnomin/acctools.py
--rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 22:16:30.000000 nanolab-0.0.3/nanolab/xnomin/handshake.py
--rw-r--r--   0 root         (0) root         (0)    18867 2023-05-04 22:16:30.000000 nanolab-0.0.3/nanolab/xnomin/peers.py
--rwxr-xr-x   0 root         (0) root         (0)     2438 2023-05-04 22:16:30.000000 nanolab-0.0.3/nanolab/xnomin/telemetry_req.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 20:58:11.171582 nanolab-0.0.3/nanolab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-09 20:58:11.000000 nanolab-0.0.3/nanolab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1120 2023-05-09 20:58:11.000000 nanolab-0.0.3/nanolab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 20:58:11.000000 nanolab-0.0.3/nanolab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-09 20:58:11.000000 nanolab-0.0.3/nanolab.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-09 20:58:11.000000 nanolab-0.0.3/nanolab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 20:58:11.000000 nanolab-0.0.3/nanolab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 20:58:11.171582 nanolab-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-09 20:47:41.000000 nanolab-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.279958 nanolab-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-10 19:38:38.279958 nanolab-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-09 20:58:11.000000 nanolab-0.0.4/nanolab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.4/nanolab/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/command/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/command/mixins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.4/nanolab/command/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-07 19:39:25.000000 nanolab-0.0.4/nanolab/command/mixins/base_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-05-09 15:37:47.000000 nanolab-0.0.4/nanolab/command/mixins/bash_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-07 19:31:15.000000 nanolab-0.0.4/nanolab/command/mixins/python_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/command/mixins/threaded_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-26 22:11:20.000000 nanolab-0.0.4/nanolab/decorators.py
+-rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.4/nanolab/main.py
+-rw-r--r--   0 root         (0) root         (0)    11028 2023-05-08 09:50:05.000000 nanolab-0.0.4/nanolab/node_interaction.py
+-rw-r--r--   0 root         (0) root         (0)     6715 2023-05-09 20:51:58.000000 nanolab-0.0.4/nanolab/node_tools.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-05-10 19:34:06.000000 nanolab-0.0.4/nanolab/pycmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/snippets/
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-05-09 15:33:56.000000 nanolab-0.0.4/nanolab/snippets/default_snips.json
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/snippets/test_snippets.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.4/nanolab/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/src/argparse_commands.py
+-rw-r--r--   0 root         (0) root         (0)     4899 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/src/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/src/config_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-05-08 12:45:36.000000 nanolab-0.0.4/nanolab/src/github.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.4/nanolab/src/resolver.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-10 13:22:47.000000 nanolab-0.0.4/nanolab/src/snippet_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.279958 nanolab-0.0.4/nanolab/xnomin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.4/nanolab/xnomin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.4/nanolab/xnomin/acctools.py
+-rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 22:16:30.000000 nanolab-0.0.4/nanolab/xnomin/handshake.py
+-rw-r--r--   0 root         (0) root         (0)    18867 2023-05-04 22:16:30.000000 nanolab-0.0.4/nanolab/xnomin/peers.py
+-rwxr-xr-x   0 root         (0) root         (0)     2424 2023-05-10 19:36:27.000000 nanolab-0.0.4/nanolab/xnomin/telemetry_req.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 19:38:38.275958 nanolab-0.0.4/nanolab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-10 19:38:38.000000 nanolab-0.0.4/nanolab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 19:38:38.279958 nanolab-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-10 19:38:31.000000 nanolab-0.0.4/setup.py
```

### Comparing `nanolab-0.0.3/PKG-INFO` & `nanolab-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: nanolab
-Version: 0.0.3
-Summary: testing tool using nanomock
-Home-page: https://github.com/gr0vity-dev/nanolab
-Author: gr0vity
-Description-Content-Type: text/markdown
-
 ##NanoLab
 
 NanoLab is an easy-to-use testing tool designed to run test cases against a local network of nano-nodes. It utilizes [NanoMock](https://github.com/gr0vity-dev/nanomock), a highly customizable tool for creating dockerized nano networks, to facilitate quick and efficient testing of various configurations. Simply provide a config file for the test case and watch NanoLab streamline your testing process.
 
 ###Features:
 
 - Run test cases against a local network of nano-nodes
@@ -32,8 +24,8 @@
 |Command| flag | 
 |----|----|
 | `-t --test-case`  | Use one of the available testcases (`nanolab list`)
 |                   | Can be a `/path/to/config.json` on your disk
 | `--gh-user --gh-repo --gh-path` | Default : [gr0vity-dev nanolab-configs default](https://github.com/gr0vity-dev/nanolab-configs/tree/main/default)
 |                   | Used in `nanolab list` to show available testcases
 |                   | Used in `nanolab run` to download the selected testcase 
-| `-i --image`      | List of docker images used per testrun
+| `-i --image`      | List of docker images used per testrun
```

### Comparing `nanolab-0.0.3/README.md` & `nanolab-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: nanolab
+Version: 0.0.4
+Summary: testing tool using nanomock
+Home-page: https://github.com/gr0vity-dev/nanolab
+Author: gr0vity
+Description-Content-Type: text/markdown
+
 ##NanoLab
 
 NanoLab is an easy-to-use testing tool designed to run test cases against a local network of nano-nodes. It utilizes [NanoMock](https://github.com/gr0vity-dev/nanomock), a highly customizable tool for creating dockerized nano networks, to facilitate quick and efficient testing of various configurations. Simply provide a config file for the test case and watch NanoLab streamline your testing process.
 
 ###Features:
 
 - Run test cases against a local network of nano-nodes
@@ -24,8 +32,8 @@
 |Command| flag | 
 |----|----|
 | `-t --test-case`  | Use one of the available testcases (`nanolab list`)
 |                   | Can be a `/path/to/config.json` on your disk
 | `--gh-user --gh-repo --gh-path` | Default : [gr0vity-dev nanolab-configs default](https://github.com/gr0vity-dev/nanolab-configs/tree/main/default)
 |                   | Used in `nanolab list` to show available testcases
 |                   | Used in `nanolab run` to download the selected testcase 
-| `-i --image`      | List of docker images used per testrun
+| `-i --image`      | List of docker images used per testrun
```

### Comparing `nanolab-0.0.3/nanolab/command/command.py` & `nanolab-0.0.4/nanolab/command/command.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from abc import ABC, abstractmethod
 from .mixins.bash_command_mixin import BashCommandMixin
-from .mixins.snippet_command_mixin import SnippetCommandMixin
 from .mixins.python_command_mixin import PythonCommandMixin
 from .mixins.threaded_command_mixin import ThreadedCommandMixin
-from nanolab.src.snippet_manager import SnippetManager
 
 
 class ICommand(ABC):
 
     @abstractmethod
     def validate(self):
         pass
@@ -15,24 +13,21 @@
     @abstractmethod
     def execute(self):
         pass
 
 
 class Command:
 
-    def __init__(self, command_config: dict, snippet_manager: SnippetManager):
+    def __init__(self, command_config: dict):
         self.command_config = command_config
-        self.snippet_manager = snippet_manager
         self.mixins = {
             'bash': BashCommandMixin,
-            'snippet': SnippetCommandMixin,
             'python': PythonCommandMixin,
             'threaded': ThreadedCommandMixin
         }
-
         command_type = self.command_config['type']
 
         if command_type not in self.mixins:
             raise ValueError(f"Unsupported command type '{command_type}'")
 
         mixin = self.mixins[command_type](self)
         self.mixin = mixin
@@ -41,10 +36,10 @@
         self.mixin.validate()
 
     def execute(self):
         if self.command_config.get("skip"): return
         self.mixin.execute()
 
     def execute_another_command(self, command_config):
-        another_command = Command(command_config, self.snippet_manager)
+        another_command = Command(command_config)
         another_command.validate()
         another_command.execute()
```

### Comparing `nanolab-0.0.3/nanolab/command/mixins/base_mixin.py` & `nanolab-0.0.4/nanolab/command/mixins/base_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/command/mixins/bash_command_mixin.py` & `nanolab-0.0.4/nanolab/command/mixins/bash_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/command/mixins/python_command_mixin.py` & `nanolab-0.0.4/nanolab/command/mixins/python_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/command/mixins/threaded_command_mixin.py` & `nanolab-0.0.4/nanolab/command/mixins/threaded_command_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import threading
-from nanolab.src.snippet_manager import SnippetManager
 from nanolab import pycmd
 from .base_mixin import CommandMixinBase
 from collections import defaultdict
 
 
 class ThreadedCommandMixin(CommandMixinBase):
 
     def _execute_command_sequence(self, commands):
         for command_config in commands:
             self.command_instance.execute_another_command(command_config)
 
     def validate(self):
+
         for python_command in self.command_instance.command_config["commands"]:
             if "method" not in python_command:
                 raise ValueError(f"Python command: 'method' is required.")
 
             method_name = python_command["method"]
 
             if "class" in python_command:
```

### Comparing `nanolab-0.0.3/nanolab/decorators.py` & `nanolab-0.0.4/nanolab/decorators.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/node_interaction.py` & `nanolab-0.0.4/nanolab/node_interaction.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/node_tools.py` & `nanolab-0.0.4/nanolab/node_tools.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/pycmd.py` & `nanolab-0.0.4/nanolab/pycmd.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/snippets/default_snips.json` & `nanolab-0.0.4/nanolab/snippets/default_snips.json`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/snippets/test_snippets.json` & `nanolab-0.0.4/nanolab/snippets/test_snippets.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5714285714285714%*

 * *Differences: {"'circular_in_snippet'": "OrderedDict([('commands', [OrderedDict([('type', 'snippet'), ('key', "*

 * *                          "'circular_in_snippet'), ('variables', OrderedDict([('file_name', "*

 * *                          "'test.txt')]))])])])",*

 * * "'nested_circular_in_snippet_p1'": "OrderedDict([('commands', [OrderedDict([('type', 'snippet'), "*

 * *                                    "('key', 'nested_circular_in_snippet_p2'), ('variables', "*

 * *                                    "OrderedDict([('file_name', 'test.txt') […]*

```diff
@@ -1,8 +1,41 @@
 {
+    "circular_in_snippet": {
+        "commands": [
+            {
+                "key": "circular_in_snippet",
+                "type": "snippet",
+                "variables": {
+                    "file_name": "test.txt"
+                }
+            }
+        ]
+    },
+    "nested_circular_in_snippet_p1": {
+        "commands": [
+            {
+                "key": "nested_circular_in_snippet_p2",
+                "type": "snippet",
+                "variables": {
+                    "file_name": "test.txt"
+                }
+            }
+        ]
+    },
+    "nested_circular_in_snippet_p2": {
+        "commands": [
+            {
+                "key": "nested_circular_in_snippet_p1",
+                "type": "snippet",
+                "variables": {
+                    "file_name": "test.txt"
+                }
+            }
+        ]
+    },
     "snippet_in_snippet": {
         "commands": [
             {
                 "key": "test_snippet",
                 "type": "snippet",
                 "variables": {
                     "file_name": "test.txt"
```

### Comparing `nanolab-0.0.3/nanolab/src/argparse_commands.py` & `nanolab-0.0.4/nanolab/src/argparse_commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 from os import environ
 from .github import GitHubAPI
 import argparse
 from nanolab.src.config_handler import ConfigPathHandler, ConfigResourceHandler
 from nanomock.modules.nl_parse_config import ConfigReadWrite
 from nanolab.src.utils import extract_packaged_data_to_disk
-from nanolab.src.config_loader import TestcaseConfig
+from nanolab.src.config_loader import ConfigLoader, ConfigValidator, ConfigCommandExecutor
 from nanolab.src.snippet_manager import SnippetManager
-from nanolab.command.command import Command
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description="Load configuration and snippets files")
 
     subparsers = parser.add_subparsers(dest="command")
@@ -52,43 +51,14 @@
         type=str,
         default='default',
         help='Path to testcases within the repository (default: default)')
 
     return parser.parse_args()
 
 
-def _load_and_validate_configs(snippet_path, config_path):
-
-    sinppet_manager = SnippetManager(snippet_path)
-    config_loader = TestcaseConfig(sinppet_manager, config_path=config_path)
-
-    config_loader.apply_globals()
-    config_loader.complete_config()
-    config_loader.validate_config()
-
-    return config_loader
-
-
-def _execute_command(command_config, snippet_manager: SnippetManager):
-    if command_config.get('skip', False):
-        return
-
-    command = Command(command_config, snippet_manager)
-    command.validate()
-    command.execute()
-
-
-def _execute_commands(config_loader: TestcaseConfig):
-
-    for docker_tag in config_loader.config["docker_tags"]:
-        environ["docker_tag"] = docker_tag
-        for command_config in config_loader.config["commands"]:
-            _execute_command(command_config, config_loader.snippet_manager)
-
-
 class ArgParseHandler:
 
     def __init__(self, args=None):
         self.args = args or parse_args()
         self.conf_rw = ConfigReadWrite()
         self.github_api = GitHubAPI(self.args.gh_user, self.args.gh_repo,
                                     self.args.gh_path)
@@ -106,21 +76,23 @@
 
         #resolve and downlaod resources defiend in the config
         resolved_config = resource_handler.download_and_replace_resources(
             config_path, path_handler.downloads_path)
         #replace docker_tags with commandline
         if self.args.image: resolved_config["docker_tags"] = self.args.image
 
-        self.conf_rw.write_json(path_handler.resolved_config_file_path,
-                                resolved_config)
+        resolved_path = path_handler.get_resolved_config_path()
+        snippet_path = path_handler.get_snippets_path()
 
-        config_loader = _load_and_validate_configs(
-            path_handler.get_snippets_path(),
-            path_handler.get_resolved_config_path())
-        _execute_commands(config_loader)
+        snippet_manager = SnippetManager(snippet_path)
+        config_loader = ConfigLoader(snippet_manager)
+        final_config = config_loader.load_config(resolved_config)
+        self.conf_rw.write_json(resolved_path, final_config)
+        ConfigValidator.validate_config(final_config)
+        ConfigCommandExecutor.execute_commands(final_config)
 
     def list_testcases(self):
         files = self.github_api.get_files()
 
         if files:
             for file in files:
                 if file["name"].endswith(".json"):
```

### Comparing `nanolab-0.0.3/nanolab/src/config_handler.py` & `nanolab-0.0.4/nanolab/src/config_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import shutil
-import requests
 from pathlib import Path
 from os import environ
 from nanomock.modules.nl_parse_config import ConfigReadWrite
 from nanolab.src.utils import download_data
 from nanolab.src.github import GitHubAPI
 
 
@@ -36,17 +35,14 @@
         else:
             testcase_name = testcase_alias
         return testcase_name
 
     def get_testcase_name(self):
         return self.testcase_name
 
-    def get_config_path(self):
-        return self.resources_path / "config.json"
-
     def get_resources_path(self):
         return self.resources_path
 
     def get_snippets_path(self):
         return self.snippets_path
 
     def get_resolved_config_path(self):
```

### Comparing `nanolab-0.0.3/nanolab/src/config_loader.py` & `nanolab-0.0.4/nanolab/src/config_loader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,94 @@
 import os
-import shutil
-import requests
 from nanomock.modules.nl_parse_config import ConfigReadWrite
 from .snippet_manager import SnippetManager
-from nanolab.command.command_validator import CommandValidator
+from nanolab.command.command import Command
 
 
-class TestcaseConfig:
+class ConfigLoader:
 
-    def __init__(self,
-                 snippet_manager: SnippetManager,
-                 config_path: str = None):
-        self.default_command_executor = "NodeInteraction"
-        self.conf_rw = ConfigReadWrite()
-        self.config = self._load_config(config_path)
+    def __init__(self, snippet_manager: SnippetManager):
         self.snippet_manager = snippet_manager
+        self.conf_rw = ConfigReadWrite()
+        self.default_command_executor = "NodeInteraction"
+
+    def read_config(self, config_path: str):
+        self.conf_rw.read_json(config_path)
 
-    def _load_resolved_path(self, config_path, env_var, default_path) -> dict:
-        config_path = config_path if config_path else os.environ.get(
-            env_var, default_path)
-
-        return self.conf_rw.read_json(config_path)
-
-    def _load_config(self, config_path: str) -> dict:
-        return self._load_resolved_path(config_path, "CONFIG_FILE",
-                                        'config.example.json')
-
-    def apply_globals(self):
-        testcase_name = self.config["testcase"]
-        global_variables = self.config.get("global", {})
+    def load_config(self, config: dict):
+        config = self._resolve_snippets(config, [])
+        config = self._apply_globals(config)
+        config = self._complete_config(config)
 
-        # Replace global variables in the commands section
-        for command in self.config["commands"]:
+        return config
+
+    def _apply_globals(self, config):
+        global_variables = config.get("global", {})
+
+        for command in config["commands"]:
             self._apply_variables_to_command(global_variables, command)
 
+        return config
+
     def _set_default_class(self, command):
         if command.get("type") in ["python"]:
             command.setdefault("class", self.default_command_executor)
 
-    def complete_config(self):
-        for command in self.config["commands"]:
+    def _complete_config(self, config):
+        for command in config["commands"]:
             self._set_default_class(command)
 
             if command.get("type") == "threaded":
                 for python_command in command["commands"]:
                     self._set_default_class(python_command)
 
-            if command.get("type") == "snippet":
-                snippet = self.snippet_manager.get_snippet_by_key(
-                    command["key"])
-                for python_command in snippet["commands"]:
-                    self._set_default_class(python_command)
-
-    # Add your existing _set_default_class and _load_snippet_by_key methods here
-
-    def validate_config(self):
-        if "commands" not in self.config:
-            raise ValueError(
-                "The 'commands' key is missing in the config file.")
+        return config
 
-        for idx, command in enumerate(self.config["commands"]):
-            command_type = command.get("type")
-            if command_type not in ["bash", "snippet", "python", "threaded"]:
-                raise ValueError(
-                    f"Invalid command type '{command_type}' at index {idx} in 'commands'"
+    def _resolve_snippets(self, config, breadcrumb=[]):
+        config["commands"] = self._resolve_commands(config["commands"],
+                                                    breadcrumb)
+        return config
+
+    def _resolve_commands(self, commands, breadcrumb):
+        resolved_commands = []
+        for command in commands:
+            if command.get("type") == "snippet":
+                resolved_commands.extend(
+                    self._resolve_snippet_command(command, breadcrumb))
+            else:
+                resolved_commands.append(command)
+        return resolved_commands
+
+    def _resolve_snippet_command(self, command, breadcrumb):
+        key = command["key"]
+        if key in breadcrumb:
+            raise ValueError(f"Circular snippet reference detected: {key}")
+
+        snippet = self.snippet_manager.get_snippet_by_key(key)
+        variables = command.get("variables", {})
+        self._check_mandatory_vars(snippet, variables, key)
+        resolved_snippet = self._resolve_snippets(snippet, breadcrumb + [key])
+        return self._replace_vars_in_commands(resolved_snippet["commands"],
+                                              variables)
+
+    def _check_mandatory_vars(self, snippet, variables, key):
+        mandatory_vars = snippet.get("mandatory_vars", [])
+        for var in mandatory_vars:
+            if var not in variables:
+                raise KeyError(
+                    f"Mandatory variable '{var}' is missing in '{key}'. Variables defined: {list(variables.keys())}"
                 )
-            if command_type in ("python", "threaded"):
-                CommandValidator.validate_command(
-                    command, self.snippet_manager.get_snippets())
-            elif command_type == "snippet":
-                if "key" not in command:
-                    raise ValueError(
-                        f"Missing 'key' for snippet command at index {idx} in 'commands'"
-                    )
+
+    def _replace_vars_in_commands(self, commands, variables):
+        for command in commands:
+            if "command" in command:
+                for var, value in variables.items():
+                    command["command"] = command["command"].replace(
+                        f'{{{var}}}', value)
+        return commands
 
     def _apply_variables_to_command(self, global_variables: dict,
                                     command: dict):
         if isinstance(command, dict):
             for key, value in command.items():
                 if isinstance(value, str):
                     command[key] = self._replace_global_variables(
@@ -87,8 +99,40 @@
             for item in command:
                 self._apply_variables_to_command(global_variables, item)
 
     def _replace_global_variables(self, global_variables: dict,
                                   value: str) -> str:
         for global_key, global_value in global_variables.items():
             value = value.replace(f"{{{global_key}}}", global_value)
-        return value
+        return value
+
+
+class ConfigValidator:
+
+    @staticmethod
+    def validate_config(config):
+        if "commands" not in config:
+            raise ValueError(
+                "The 'commands' key is missing in the config file.")
+
+        for idx, command in enumerate(config["commands"]):
+            command_type = command.get("type")
+            if command_type not in ["bash", "snippet", "python", "threaded"]:
+                raise ValueError(
+                    f"Invalid command type '{command_type}' at index {idx} in 'commands'"
+                )
+
+
+class ConfigCommandExecutor:
+
+    @staticmethod
+    def execute_commands(config):
+        for docker_tag in config["docker_tags"]:
+            os.environ["docker_tag"] = docker_tag
+            for command_config in config["commands"]:
+                ConfigCommandExecutor.execute_command(command_config)
+
+    @staticmethod
+    def execute_command(command_config):
+        command = Command(command_config)
+        command.validate()
+        command.execute()
```

### Comparing `nanolab-0.0.3/nanolab/src/github.py` & `nanolab-0.0.4/nanolab/src/github.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/src/resolver.py` & `nanolab-0.0.4/nanolab/src/resolver.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/src/snippet_manager.py` & `nanolab-0.0.4/nanolab/src/snippet_manager.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/src/utils.py` & `nanolab-0.0.4/nanolab/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from os import environ, path, walk
-import time
 import shutil
 from importlib import resources
 from pathlib import Path
 import logging
 import requests
 from nanomock.modules.nl_parse_config import ConfigParser
 import filecmp
```

### Comparing `nanolab-0.0.3/nanolab/xnomin/acctools.py` & `nanolab-0.0.4/nanolab/xnomin/acctools.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/xnomin/handshake.py` & `nanolab-0.0.4/nanolab/xnomin/handshake.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/xnomin/peers.py` & `nanolab-0.0.4/nanolab/xnomin/peers.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.3/nanolab/xnomin/telemetry_req.py` & `nanolab-0.0.4/nanolab/xnomin/telemetry_req.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/bin/env python3
 
-import struct
 import binascii
 
 from nanolab.xnomin.peers import message_header, message_type, message_type_enum
 
 
 class telemetry_req:
```

### Comparing `nanolab-0.0.3/nanolab.egg-info/PKG-INFO` & `nanolab-0.0.4/nanolab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolab
-Version: 0.0.3
+Version: 0.0.4
 Summary: testing tool using nanomock
 Home-page: https://github.com/gr0vity-dev/nanolab
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 ##NanoLab
```

### Comparing `nanolab-0.0.3/setup.py` & `nanolab-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanolab",
-      version="0.0.3",
+      version="0.0.4",
       author="gr0vity",
       description="testing tool using nanomock",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanolab",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
```

