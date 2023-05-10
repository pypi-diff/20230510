# Comparing `tmp/dettectinator-1.1.1.tar.gz` & `tmp/dettectinator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dettectinator-1.1.1.tar", last modified: Mon Apr 17 10:00:19 2023, max compression
+gzip compressed data, was "dettectinator-1.2.0.tar", last modified: Wed May 10 15:15:15 2023, max compression
```

## Comparing `dettectinator-1.1.1.tar` & `dettectinator-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.336272 dettectinator-1.1.1/
--rw-r--r--   0 ruben      (501) staff       (20)    35149 2022-11-02 21:36:33.000000 dettectinator-1.1.1/LICENSE
--rw-r--r--   0 ruben      (501) staff       (20)       11 2022-11-02 21:36:33.000000 dettectinator-1.1.1/MANIFEST.in
--rw-r--r--   0 ruben      (501) staff       (20)     1560 2023-04-17 10:00:19.336006 dettectinator-1.1.1/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)     2379 2023-01-25 07:09:52.000000 dettectinator-1.1.1/README.md
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.327377 dettectinator-1.1.1/dettectinator/
--rw-r--r--   0 ruben      (501) staff       (20)      107 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)     8959 2023-01-25 07:09:52.000000 dettectinator-1.1.1/dettectinator/cli.py
--rw-r--r--   0 ruben      (501) staff       (20)     3844 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/constants.py
--rw-r--r--   0 ruben      (501) staff       (20)    41570 2023-04-17 09:54:28.000000 dettectinator-1.1.1/dettectinator/dettectinator.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.333423 dettectinator-1.1.1/dettectinator/plugins/
--rw-r--r--   0 ruben      (501) staff       (20)        0 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/plugins/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)    14192 2023-03-15 09:27:23.000000 dettectinator-1.1.1/dettectinator/plugins/datasources_import.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.335571 dettectinator-1.1.1/dettectinator/plugins/support/
--rw-r--r--   0 ruben      (501) staff       (20)        0 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/plugins/support/__init__.py
--rw-r--r--   0 ruben      (501) staff       (20)     3481 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/plugins/support/authentication.py
--rw-r--r--   0 ruben      (501) staff       (20)     5333 2022-11-02 21:36:33.000000 dettectinator-1.1.1/dettectinator/plugins/support/msal_patch.py
--rw-r--r--   0 ruben      (501) staff       (20)    32798 2023-01-25 07:09:52.000000 dettectinator-1.1.1/dettectinator/plugins/technique_import.py
-drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-04-17 10:00:19.330592 dettectinator-1.1.1/dettectinator.egg-info/
--rw-r--r--   0 ruben      (501) staff       (20)     1560 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/PKG-INFO
--rw-r--r--   0 ruben      (501) staff       (20)      581 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/SOURCES.txt
--rw-r--r--   0 ruben      (501) staff       (20)        1 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/dependency_links.txt
--rw-r--r--   0 ruben      (501) staff       (20)      134 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/requires.txt
--rw-r--r--   0 ruben      (501) staff       (20)       14 2023-04-17 10:00:19.000000 dettectinator-1.1.1/dettectinator.egg-info/top_level.txt
--rw-r--r--   0 ruben      (501) staff       (20)       38 2023-04-17 10:00:19.336348 dettectinator-1.1.1/setup.cfg
--rw-r--r--   0 ruben      (501) staff       (20)     1997 2023-04-17 09:56:17.000000 dettectinator-1.1.1/setup.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-05-10 15:15:15.353054 dettectinator-1.2.0/
+-rw-r--r--   0 ruben      (501) staff       (20)    35149 2022-11-02 21:36:33.000000 dettectinator-1.2.0/LICENSE
+-rw-r--r--   0 ruben      (501) staff       (20)       11 2022-11-02 21:36:33.000000 dettectinator-1.2.0/MANIFEST.in
+-rw-r--r--   0 ruben      (501) staff       (20)     1560 2023-05-10 15:15:15.352774 dettectinator-1.2.0/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)     2869 2023-05-10 14:24:28.000000 dettectinator-1.2.0/README.md
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-05-10 15:15:15.335060 dettectinator-1.2.0/dettectinator/
+-rw-r--r--   0 ruben      (501) staff       (20)      136 2023-05-10 14:14:27.000000 dettectinator-1.2.0/dettectinator/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)    11024 2023-05-10 14:24:28.000000 dettectinator-1.2.0/dettectinator/cli.py
+-rw-r--r--   0 ruben      (501) staff       (20)     4087 2023-05-10 14:14:27.000000 dettectinator-1.2.0/dettectinator/constants.py
+-rw-r--r--   0 ruben      (501) staff       (20)    47242 2023-05-10 14:24:28.000000 dettectinator-1.2.0/dettectinator/dettectinator.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-05-10 15:15:15.348482 dettectinator-1.2.0/dettectinator/plugins/
+-rw-r--r--   0 ruben      (501) staff       (20)        0 2022-11-02 21:36:33.000000 dettectinator-1.2.0/dettectinator/plugins/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)    14192 2023-05-10 14:24:28.000000 dettectinator-1.2.0/dettectinator/plugins/datasources_import.py
+-rw-r--r--   0 ruben      (501) staff       (20)     5250 2023-05-10 14:14:27.000000 dettectinator-1.2.0/dettectinator/plugins/groups_import.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-05-10 15:15:15.352305 dettectinator-1.2.0/dettectinator/plugins/support/
+-rw-r--r--   0 ruben      (501) staff       (20)        0 2022-11-02 21:36:33.000000 dettectinator-1.2.0/dettectinator/plugins/support/__init__.py
+-rw-r--r--   0 ruben      (501) staff       (20)     3481 2022-11-02 21:36:33.000000 dettectinator-1.2.0/dettectinator/plugins/support/authentication.py
+-rw-r--r--   0 ruben      (501) staff       (20)     5333 2022-11-02 21:36:33.000000 dettectinator-1.2.0/dettectinator/plugins/support/msal_patch.py
+-rw-r--r--   0 ruben      (501) staff       (20)    33583 2023-05-10 14:14:27.000000 dettectinator-1.2.0/dettectinator/plugins/technique_import.py
+drwxr-xr-x   0 ruben      (501) staff       (20)        0 2023-05-10 15:15:15.338598 dettectinator-1.2.0/dettectinator.egg-info/
+-rw-r--r--   0 ruben      (501) staff       (20)     1560 2023-05-10 15:15:15.000000 dettectinator-1.2.0/dettectinator.egg-info/PKG-INFO
+-rw-r--r--   0 ruben      (501) staff       (20)      620 2023-05-10 15:15:15.000000 dettectinator-1.2.0/dettectinator.egg-info/SOURCES.txt
+-rw-r--r--   0 ruben      (501) staff       (20)        1 2023-05-10 15:15:15.000000 dettectinator-1.2.0/dettectinator.egg-info/dependency_links.txt
+-rw-r--r--   0 ruben      (501) staff       (20)      140 2023-05-10 15:15:15.000000 dettectinator-1.2.0/dettectinator.egg-info/requires.txt
+-rw-r--r--   0 ruben      (501) staff       (20)       14 2023-05-10 15:15:15.000000 dettectinator-1.2.0/dettectinator.egg-info/top_level.txt
+-rw-r--r--   0 ruben      (501) staff       (20)       38 2023-05-10 15:15:15.353142 dettectinator-1.2.0/setup.cfg
+-rw-r--r--   0 ruben      (501) staff       (20)     2028 2023-05-10 14:26:28.000000 dettectinator-1.2.0/setup.py
```

### Comparing `dettectinator-1.1.1/LICENSE` & `dettectinator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.1/PKG-INFO` & `dettectinator-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dettectinator
-Version: 1.1.1
+Version: 1.2.0
 Summary: Dettectinator - The Python library to your DeTT&CT YAML files.
 Home-page: https://github.com/siriussecurity/dettectinator
 Author: Sirius Security
 License: GPL3
 Project-URL: Documentation, https://github.com/siriussecurity/dettectinator/wiki
 Project-URL: Code, https://github.com/siriussecurity/dettectinator
 Project-URL: Issue tracker, https://github.com/siriussecurity/dettectinator/issues
```

### Comparing `dettectinator-1.1.1/README.md` & `dettectinator-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,10 +24,14 @@
 For data sources, you can use the following plugins:
 - Defender for Endpoints: tables available in Advanced Hunting (based on OSSEM)
 - Windows Sysmon: event logging based on Sysmon (based on OSSEM and your Sysmon config file)
 - Sentinel Window Security Auditing: event logging (based on OSSEM and EventID's found in your logging)
 - CSV: any csv with ATT&CK data sources and products (file)
 - Excel: any Excel file with ATT&CK data sources and products (file)
 
-It's easy to create your own Dettectinator plugins or edit the ones we've provided to cover additional scenarios.
+In the latest version we have also added support for importing attack groups data. The way that you import that data will depend on how you get your CTI data delivered. We added 2 sample plugins that you can use to create your own tailored plugins:
+- Excel: import techniques for groups from Excel. In this Excel (which can be found in the examples) each group has its own tab that lists the techniques.
+- PDF: import techniques and software based on regular expressions from a PDF file.
+
+It's easy to create your own Dettectinator plugins or edit the ones we've provided to cover additional scenario's.
 
 More information on how to use Dettectinator and how to use and create plugins can be found in the [wiki](https://github.com/siriussecurity/dettectinator/wiki).
```

### Comparing `dettectinator-1.1.1/dettectinator/cli.py` & `dettectinator-1.2.0/dettectinator/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Dettectinator - The Python library to your DeTT&CT YAML files.
 Authors:
     Martijn Veken, Sirius Security
     Ruben Bouman, Sirius Security
 License: GPL-3.0 License
 """
-
+import datetime
 import json
 import sys
 import os
 import importlib
 import inspect
 
-from dettectinator import DettectTechniquesAdministration, DettectDataSourcesAdministration
+from collections import OrderedDict
+from dettectinator import DettectTechniquesAdministration, DettectDataSourcesAdministration, DettectGroupsAdministration
 from plugins.technique_import import TechniqueBase
 from plugins.datasources_import import DatasourceBase
+from plugins.groups_import import GroupBase
 from argparse import ArgumentParser, Namespace
 
 
 class CommandLine:
 
     @staticmethod
     def _get_raw_commandline(argument_names: list) -> str:
@@ -53,39 +55,40 @@
         :return: dict containing plugins and modules
         """
         import_plugins = {}
         path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'plugins')
         for module in [x for x in os.listdir(path) if x[-3:] == '.py']:
             plugin_mod = importlib.import_module('plugins.' + module[:-3])
             for name, cls in inspect.getmembers(plugin_mod, inspect.isclass):
-                if ('Technique' in name or 'Datasource' in name) and 'Base' not in name:
+                if ('Technique' in name or 'Datasource' in name or 'Group' in name) and 'Base' not in name:
                     import_plugins[name] = plugin_mod
         return import_plugins
 
     @staticmethod
     def _set_default_params(parser: ArgumentParser):
         """
         Set the default command line arguments
         """
         required = parser.add_argument_group('required arguments')
         parser.add_argument('-c', '--config', help='Configuration file location.')
         required.add_argument('-p', '--plugin', help='Data import plugin name.', required=True)
-        required.add_argument('-a', '--applicable_to',
-                              help='Systems that the detections are applicable to (comma seperated list).',
-                              required=True)
+        parser.add_argument('-a', '--applicable_to',
+                            help='Systems that the detections are applicable to (comma seperated list).')
         parser.add_argument('-d', '--domain',
                             help='The ATT&CK domain (default = enterprise). This argument is ignored if a domain is specified in the YAML file.',
                             required=False, choices=['enterprise', 'ics', 'mobile'])
         parser.add_argument('-i', '--input_file', help='YAML filename for input.', default=None)
         parser.add_argument('-o', '--output_file', help='YAML filename for output.', default=None)
         parser.add_argument('-n', '--name', help='Value for the name attribute in the YAML file.', default=None)
         parser.add_argument('-s', '--stix_location', help='Local STIX repository location.', default=None)
-
+        parser.add_argument('-lf', '--log_file', help='Log to write results and warnings to.', default=None)
+        parser.add_argument('-lp', '--log_parameters', action='store_true', help='Add the configuration parameters to the log.')
         parser.add_argument('-ch', '--check_unused', action='store_true', help='Check unused detections.')
-        parser.add_argument('-cl', '--clean_unused', action='store_true', help='Clean unused detections.')
+        parser.add_argument('-cl', '--clean_unused', action='store_true',
+                            help='Clean unused detections. When using this option, including the check_unused option is necessary.')
 
     def _get_argument_values_from_config_file(self) -> dict:
         """
         Read the command line arguments from the config file if applicable
         """
         config_file_name = self._get_raw_commandline(['-c', '--config'])
         if config_file_name:
@@ -93,14 +96,29 @@
             with open(config_file_name, 'r') as f:
                 config_file_arguments = json.load(f)
         else:
             config_file_arguments = {}
         return config_file_arguments
 
     @staticmethod
+    def _create_log_file(arguments: Namespace, output: list, plugin_name: str) -> None:
+        sep_single = '-' * 100 + '\n'
+        sep_double = "=" * 100 + '\n'
+        with open(arguments.log_file, 'a') as log_file:
+            log_file.write(sep_double)
+            log_file.write(f'Result from plugin {plugin_name} at {datetime.datetime.now()}:\n')
+            log_file.write(sep_single)
+            if arguments.log_parameters:
+                log_file.writelines([f'{k}: {v}\n' for k, v in OrderedDict(sorted(vars(arguments).items())).items()])
+                log_file.write(sep_single)
+            log_file.writelines([f'{o}\n' for o in output])
+            log_file.write(sep_double)
+            log_file.write('\n')
+
+    @staticmethod
     def process_techniques(applicable_to: list, arguments: Namespace, plugin: TechniqueBase) -> tuple:
         """
         Process all techniques from the source system
         """
         # Get the technique data
         techniques = plugin.get_attack_techniques(applicable_to)
         # Convert data to yaml
@@ -126,14 +144,28 @@
         print('Generating datasources YAML file.')
         dettect = DettectDataSourcesAdministration(arguments.input_file, domain=arguments.domain,
                                                    local_stix_path=arguments.stix_location)
         warnings, results = dettect.update_data_sources(datasources, check_unused_data_sources=arguments.check_unused,
                                                         clean_unused_data_sources=arguments.clean_unused)
         return dettect, results, warnings
 
+    @staticmethod
+    def process_groups(arguments: Namespace, plugin: GroupBase) -> tuple:
+        """
+        Process all groups from the source
+        """
+        # Get the group data
+        groups = plugin.get_attack_groups()
+        # Convert data to yaml
+        print('Generating groups YAML file.')
+        dettect = DettectGroupsAdministration(arguments.input_file, domain=arguments.domain,
+                                              local_stix_path=arguments.stix_location)
+        warnings, results = dettect.add_groups(groups)
+        return dettect, results, warnings
+
     def start(self) -> None:
         """
         Dettectinator has been started from the commandline.
         Process the command line arguments and launch the appropriate plugin.
         """
 
         # Load default argument values from the config file
@@ -168,32 +200,38 @@
             parser.set_defaults(**config_file_arguments)
             for action in parser._actions:
                 if action.dest in config_file_arguments.keys():
                     action.required = False
 
             # Evaluate command line arguments
             arguments = parser.parse_args()
-            applicable_to = [at.strip() for at in arguments.applicable_to.split(',')]
+            applicable_to = [at.strip() for at in arguments.applicable_to.split(',')] if arguments.applicable_to else []
             output_file = arguments.output_file or arguments.input_file
 
             # Read the data from the source
             print(f'Using "{plugin_name}" to collect data.')
             plugin = plugin_class(vars(arguments))
 
             if plugin_name.startswith('Technique'):
                 dettect, results, warnings = self.process_techniques(applicable_to, arguments, plugin)
-            else:
+            elif plugin_name.startswith('Datasource'):
                 dettect, results, warnings = self.process_datasource(applicable_to, arguments, plugin)
+            else:
+                dettect, results, warnings = self.process_groups(arguments, plugin)
 
             if arguments.name:
                 dettect.set_name(arguments.name)
 
             dettect.save_yaml_file(output_file)
             print(f'DeTT&CT YAML file written: {dettect.get_filename()}')
 
-            output = warnings + results
+            output = sorted(list(set(warnings + results)))
+
+            if arguments.log_file:
+                self._create_log_file(arguments, output, plugin_name)
+
             if len(output) > 0:
                 print('\nPlease review the following items:')
                 print(' - ' + '\n - '.join(output))
         else:
             print('Please specify a valid data import plugin using the "-p" argument:')
             self._print_plugins(plugins)
```

### Comparing `dettectinator-1.1.1/dettectinator/constants.py` & `dettectinator-1.2.0/dettectinator/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,11 +71,19 @@
                                   'domain': 'enterprise-attack',
                                   'systems': [{ 'applicable_to': 'default', 'platform': ['all'] }],
                                   'data_sources': []
                                  }
 
 YAML_OBJ_NEW_GROUPS_FILE = {'version': 1.0,
                             'file_type': 'group-administration',
+                            'name': 'new',
                             'domain': 'enterprise-attack',
                             'platform': ['all'],
                             'groups': []
-                           }
+                           }
+
+YAML_OBJ_GROUP = {'group_name': '',
+                  'campaign': '',
+                  'technique_id': [],
+                  'software_id': [],
+                  'enabled': True
+                  }
```

### Comparing `dettectinator-1.1.1/dettectinator/dettectinator.py` & `dettectinator-1.2.0/dettectinator/dettectinator.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,14 +104,18 @@
 
             if self.domain == 'mobile-attack':
                 raise Exception(f'{self.__class__.__name__}: Data sources for ATT&CK Mobile not yet implemented by MITRE.')
         elif isinstance(self, DettectTechniquesAdministration):
             self._yaml_content = deepcopy(YAML_OBJ_NEW_TECHNIQUES_FILE)
             self.filename = f"techniques_{self._yaml_content['name']}.yaml"
             self._yaml_content['domain'] = self.domain
+        elif isinstance(self, DettectGroupsAdministration):
+            self._yaml_content = deepcopy(YAML_OBJ_NEW_GROUPS_FILE)
+            self.filename = f"groups_{self._yaml_content['name']}.yaml"
+            self._yaml_content['domain'] = self.domain
 
     def save_yaml_file(self, filename=None) -> None:
         """
         Saves the YAML file back to disk using the given filename or the same filename when the file was read.
         """
         with open(filename if filename else self.filename, 'w') as yaml_file:
             string_io = StringIO()
@@ -222,32 +226,63 @@
         Return the technique object for the given technique_id.
         """
         for tech in self.attack_techniques:
             if tech['technique_id'] == technique_id:
                 return tech
         return None
 
+    def _load_attack_software(self) -> None:
+        """
+        Load the ATT&CK STIX data from the MITRE TAXII server.
+        :return: MITRE ATT&CK data object (STIX)
+        """
+        self._attack_software = self._convert_stix_software_to_dict(self.mitre.get_software(skip_revoked_deprecated=True))
+
+    def _get_software_from_attack(self, software_id: str) -> dict:
+        """
+        Return the technique object for the given technique_id.
+        """
+        for software in self._attack_software:
+            if software['software_id'] == software_id:
+                return software
+
+        return None
+
+    @staticmethod
+    def _convert_stix_software_to_dict(stix_attack_data: list) -> list:
+        """
+        Convert the STIX list with AttackPatterns to a dictionary for easier use in python and also include the technique_id and DeTT&CT data sources.
+        :param stix_attack_data: the MITRE ATT&CK STIX dataset with techniques
+        :return: list with dictionaries containing all software from the input stix_attack_data
+        """
+        attack_data = []
+        for stix_software in stix_attack_data:
+            software = json.loads(stix_software.serialize(), object_hook=DettectBase._date_hook)
+
+            # Add software_id as key, because it's hard to get from STIX:
+            software['software_id'] = DettectBase._get_attack_id(stix_software)
+
+            attack_data.append(software)
+
+        return attack_data
+
     @staticmethod
     def _convert_stix_techniques_to_dict(stix_attack_data: list) -> list:
         """
         Convert the STIX list with AttackPatterns to a dictionary for easier use in python and also include the technique_id and DeTT&CT data sources.
         :param stix_attack_data: the MITRE ATT&CK STIX dataset with techniques
         :return: list with dictionaries containing all techniques from the input stix_attack_data
         """
         attack_data = []
         for stix_tech in stix_attack_data:
             tech = json.loads(stix_tech.serialize(), object_hook=DettectBase._date_hook)
 
             # Add technique_id as key, because it's hard to get from STIX:
             tech['technique_id'] = DettectBase._get_attack_id(stix_tech)
 
-            # Create empty x_mitre_data_sources key for techniques without data sources:
-            if 'x_mitre_data_sources' not in tech.keys():
-                tech['x_mitre_data_sources'] = []
-
             attack_data.append(tech)
 
         return attack_data
 
     @staticmethod
     def _date_hook(json_dict: dict) -> dict:
         """
@@ -286,135 +321,157 @@
         self._load_techniques()
 
     def update_detections(self, detection_rules: dict, check_unused_detections: bool = False, clean_unused_detections: bool = False, location_prefix_unused_detections: str = '', check_unused_applicable_to: bool = False, clean_unused_applicable_to: bool = False) -> list:
         """
         Updates the techniques YAML file with the given detections.
         :param  detection_rules: a dictionary of dictionaries containing detection name as key with the following data: applicable_to, location prefix and list with ATT&CK (sub) techniques
                 {
-                    {'Detection A': {'applicable_to': ['all'], 'location_prefix': 'SIEM', 'techniques': ['T1055']}}
+                    {'Detection A': {'applicable_to': ['all'],
+                                     'location_prefix': 'SIEM',
+                                     'techniques': ['T1055']
+                                    }
+                    }
+                }
+
+                Or a dictionary of dictionaries containing multiple applicable_to items in a list:
+
+                {
+                    {'Detection A': [{'applicable_to': ['all'],
+                                     'location_prefix': 'SIEM',
+                                     'techniques': ['T1055']
+                                     }]
+                    }
                 }
         :param  check_unused_detections: boolean. When True, all detections in YAML file will be checked against given detection_rules list. It's using
                                          the location field as list for detection rules including location_prefix as prefix: "Splunk: Detection A"
         :param  clean_unused_detections: boolean. When True, all detections in YAML file that don't exist in the given detection_rules list will be removed.
         :param clean_unused_applicable_to: boolean. When True, all detection objects with a applicable_to value that doesn't exist in the given detection_rules list will be removed.
         :return a list with results containing warnings or errors during the update process.
         """
         date_today = datetime.utcnow().replace(hour=0, minute=0, second=0, microsecond=0)
 
+        # If detection_rules contains just one applicable to (as dictionary), convert the applicable_to data to a list to make it compatible:
+        for rule_name, rule_data_values in detection_rules.items():
+            if type(rule_data_values) == dict:
+                detection_rules[rule_name] = [rule_data_values]
+
         warnings, results = self._add_rules(detection_rules, date_today)
         w, r = self._delete_rules(detection_rules, check_unused_detections, clean_unused_detections,
                                   location_prefix_unused_detections, check_unused_applicable_to, clean_unused_applicable_to, date_today)
+        self._sort_locations()
         warnings += w
         results += r
 
         return warnings, results
 
     def _add_rules(self, detection_rules: dict, date_today: datetime) -> list:
         """
         Adds new detection rules to the techniques YAML file. A score_logbook entry is added for every change.
         """
         warnings, results = [], []
 
         # Loop through all detection rules:
-        for rule_name, rule_data in detection_rules.items():
-            # Loop through every technique per rule:
-            for technique_id in rule_data['techniques']:
-                attack_technique = self._get_technique_from_attack(technique_id)
-                if attack_technique is None:
-                    warnings.append(
-                        f'Technique "{technique_id}" listed in detection rule "{rule_name}" does not exist in ATT&CK ({self.domain}). Skipping.')
-                    continue
-
-                location = rule_name if rule_data['location_prefix'] == '' else rule_data['location_prefix'] + ': ' + rule_name
-                yaml_technique = self._get_technique_from_yaml(technique_id)
-                if yaml_technique is not None:
-                    # Check is applicable_to is already there:
-                    applicable_to_list = [d['applicable_to'] for d in yaml_technique['detection']]
-                    if rule_data['applicable_to'] in applicable_to_list:
-                        # applicable_to already present, go to the right applicable_to:
-                        for d in yaml_technique['detection']:
-                            if d['applicable_to'] == rule_data['applicable_to']:
-                                # Check if detection rule is in location field:
-                                rule_exist = False
-                                for loc in d['location']:
-                                    if rule_name in loc:
-                                        rule_exist = True
-                                        break
+        for rule_name, rule_applicable_to in detection_rules.items():
+            # Look through all given applicable_to values:
+            for rule_data in rule_applicable_to:
+
+                # Loop through every technique per rule:
+                for technique_id in rule_data['techniques']:
+                    attack_technique = self._get_technique_from_attack(technique_id)
+                    if attack_technique is None:
+                        warnings.append(
+                            f'Technique "{technique_id}" listed in detection rule "{rule_name}" does not exist in ATT&CK ({self.domain}). Skipping.')
+                        continue
 
-                                # If detection rule is not yet in location field, add detection rule to location field:
-                                if not rule_exist:
-                                    d['location'].append(location)
-
-                                    if len(d['score_logbook']) == 1 and d['score_logbook'][0]['date'] is None and d['score_logbook'][0]['score'] == -1:
-                                        d['score_logbook'] = []
-
-                                    # Check if score_logbook already has entry for today:
-                                    today_found = False
-                                    for logbook_entry in d['score_logbook']:
-                                        if logbook_entry['date'] == date_today:
-                                            logbook_entry['comment'] += f'. Detection rule added: {rule_name}'
-                                            today_found = True
+                    location = rule_name if rule_data['location_prefix'] == '' else rule_data['location_prefix'] + ': ' + rule_name
+                    yaml_technique = self._get_technique_from_yaml(technique_id)
+                    if yaml_technique is not None:
+                        # Check is applicable_to is already there:
+                        applicable_to_list = [d['applicable_to'] for d in yaml_technique['detection']]
+                        if rule_data['applicable_to'] in applicable_to_list:
+                            # applicable_to already present, go to the right applicable_to:
+                            for d in yaml_technique['detection']:
+                                if d['applicable_to'] == rule_data['applicable_to']:
+                                    # Check if detection rule is in location field:
+                                    rule_exist = False
+                                    for loc in d['location']:
+                                        if rule_name in loc:
+                                            rule_exist = True
                                             break
 
-                                    if not today_found:
-                                        score = self._get_latest_score(d)
-                                        score = 1 if score == -1 or score is None else score
-                                        d['score_logbook'].append({
-                                            'date': date_today,
-                                            'score': score,
-                                            'comment': f'Auto added by Dettectinator. TODO: Check score. Detection rule added: {rule_name}'
-                                        })
-                                        results.append(
-                                            f'Check score for technique {technique_id}. Detection rule(s) added for applicable_to {d["applicable_to"]}.')
-
-                                break
+                                    # If detection rule is not yet in location field, add detection rule to location field:
+                                    if not rule_exist:
+                                        d['location'].append(location)
+
+                                        # Check if score_logbook already has entry for today:
+                                        today_found = False
+                                        for logbook_entry in d['score_logbook']:
+                                            if logbook_entry['date'] == date_today:
+                                                logbook_entry['comment'] += f'. Detection rule added: {rule_name}'
+                                                results.append(
+                                                    f'Check score for technique {technique_id}. Detection rule(s) added for applicable_to {d["applicable_to"]}.')
+                                                today_found = True
+                                                break
+
+                                        if not today_found:
+                                            d['score_logbook'].append({
+                                                'date': date_today,
+                                                'score': self._get_latest_score(d),
+                                                'comment': f'Auto added by Dettectinator. TODO: Check score. Detection rule added: {rule_name}'
+                                            })
+                                            results.append(
+                                                f'Check score for technique {technique_id}. Detection rule(s) added for applicable_to {d["applicable_to"]}.')
+
+                                    break
+                        else:
+                            # applicable_to not present, add new detection object:
+                            new_detection = deepcopy(YAML_OBJ_DETECTION)
+                            new_detection['applicable_to'] = rule_data['applicable_to']
+                            new_detection['location'] = [location]
+                            new_detection['score_logbook'][0]['date'] = date_today
+                            new_detection['score_logbook'][0]['score'] = 1
+                            new_detection['score_logbook'][0][
+                                'comment'] = f'Auto added by Dettectinator. TODO: Check score. applicable_to with detection rule added: {rule_name}'
+                            yaml_technique['detection'].append(new_detection)
+                            results.append(f'Check score for technique {technique_id}. applicable_to is new: {str(rule_data["applicable_to"])}.')
                     else:
-                        # applicable_to not present, add new detection object:
+                        # Technique not present in YAML, add:
+                        new_technique = deepcopy(YAML_OBJ_TECHNIQUE)
+                        new_technique['technique_id'] = technique_id
+                        new_technique['technique_name'] = attack_technique['name']
+                        new_technique['detection'] = []
+                        new_technique['visibility'] = []
                         new_detection = deepcopy(YAML_OBJ_DETECTION)
                         new_detection['applicable_to'] = rule_data['applicable_to']
                         new_detection['location'] = [location]
                         new_detection['score_logbook'][0]['date'] = date_today
                         new_detection['score_logbook'][0]['score'] = 1
                         new_detection['score_logbook'][0][
-                            'comment'] = f'Auto added by Dettectinator. TODO: Check score. applicable_to with detection rule added: {rule_name}'
-                        yaml_technique['detection'].append(new_detection)
-                        results.append(f'Check score for technique {technique_id}. applicable_to is new: {str(rule_data["applicable_to"])}.')
-                else:
-                    # Technique not present in YAML, add:
-                    new_technique = deepcopy(YAML_OBJ_TECHNIQUE)
-                    new_technique['technique_id'] = technique_id
-                    new_technique['technique_name'] = attack_technique['name']
-                    new_technique['detection'] = []
-                    new_technique['visibility'] = []
-                    new_detection = deepcopy(YAML_OBJ_DETECTION)
-                    new_detection['applicable_to'] = rule_data['applicable_to']
-                    new_detection['location'] = [location]
-                    new_detection['score_logbook'][0]['date'] = date_today
-                    new_detection['score_logbook'][0]['score'] = 1
-                    new_detection['score_logbook'][0][
-                        'comment'] = f'Auto added by Dettectinator. TODO: Check score. Technique with detection rule added: {rule_name}'
-                    new_technique['detection'].append(new_detection)
-                    new_visibility = deepcopy(YAML_OBJ_VISIBILITY)
-                    new_technique['visibility'].append(new_visibility)
-                    self._yaml_content['techniques'].append(new_technique)
-                    results.append(f'Check score for technique {technique_id}. Technique is new.')
+                            'comment'] = f'Auto added by Dettectinator. TODO: Check score. Technique with detection rule added: {rule_name}'
+                        new_technique['detection'].append(new_detection)
+                        new_visibility = deepcopy(YAML_OBJ_VISIBILITY)
+                        new_technique['visibility'].append(new_visibility)
+                        self._yaml_content['techniques'].append(new_technique)
+                        results.append(f'Check score for technique {technique_id}. Technique is new.')
 
         return warnings, results
 
     def _delete_rules(self, detection_rules: dict, check_unused_detections: bool, clean_unused_detections: bool, location_prefix_unused_detections: str, check_unused_applicable_to: bool, clean_unused_applicable_to: bool, date_today: datetime) -> list:
         """
         Removes detection rules from the techniques YAML file which are not in the given list of detection_rules. A score_logbook entry is added for every change.
         """
         # First categorize all detection rules per applicable_to:
         warnings, results = [], []
         applicable_to_rules = {}
-        for rule_name, rule_data in detection_rules.items():
-            if str(rule_data['applicable_to']) not in applicable_to_rules.keys():
-                applicable_to_rules[str(rule_data['applicable_to'])] = {}  # cast key to string because a list cannot be a dictionary index name
-            applicable_to_rules[str(rule_data['applicable_to'])][rule_name] = rule_data
+        for rule_name, rule_applicable_to in detection_rules.items():
+            # Look through all given applicable_to values:
+            for rule_data in rule_applicable_to:
+                if str(rule_data['applicable_to']) not in applicable_to_rules.keys():
+                    applicable_to_rules[str(rule_data['applicable_to'])] = {}  # cast key to string because a list cannot be a dictionary index name
+                applicable_to_rules[str(rule_data['applicable_to'])][rule_name] = rule_data
 
         # Loop through all techniques in techniques YAML file:
         for yaml_technique in self._yaml_content['techniques']:
             # Look through all detection objects:
             to_remove = []
             for detection in yaml_technique['detection']:
                 # Proceed if applicable to from YAML file exists in detection rules list:
@@ -462,14 +519,22 @@
             for item in to_remove:
                 warnings.append(
                     f'YAML applicable_to for technique "{yaml_technique["technique_id"]}" not in rules list, so removed: {str(detection["applicable_to"])}.')
                 yaml_technique['detection'].remove(item)
 
         return warnings, results
 
+    def _sort_locations(self):
+        """
+        Sorts the location field for every technique in the YAML content.
+        """
+        for technique in self._yaml_content['techniques']:
+            for applicable_to in technique['detection']:
+                applicable_to['location'] = sorted(applicable_to['location'])
+
     def _load_techniques(self) -> None:
         """
         Loads the normalized techniques (including detection and visibility properties) from the techniques YAML file.
         """
         my_techniques = {}
 
         for d in self._yaml_content['techniques']:
@@ -764,12 +829,73 @@
             data_components = self.mitre.TC_MOBILE_SOURCE.query(Filter("type", "=", "x-mitre-data-component"))
 
         self.data_components = {}
         for data_component in data_components:
             self.data_components[data_component['name'].lower()] = data_component['name']
 
 
+class DettectGroupsAdministration(DettectBase):
+    """
+    Create or modify a DeTT&CT techniques administration YAML file.
+    """
+
+    def __init__(self, filename: str = None, domain: str = None, local_stix_path: str = None) -> None:
+        super(DettectGroupsAdministration, self).__init__(filename, domain, local_stix_path)
+        self._load_attack_software()
+
+    def add_groups(self, groups: dict) -> tuple:
+        """
+        Adds the groups to the YAML file.
+        :param groups: a dictionary containing the group name as key with the following data: campaign, a list with ATT&CK (sub)
+                       techniques and a list with ATT&CK software
+                {'APT1': {'campaign': 'P0wn them all'
+                          'techniques': ['T1566.002','T1059.001', 'T1053.005'],
+                          'software': ['S0002']
+                         }
+                }
+        :return a list with results containing warnings or errors during the update process.
+        """
+        warnings, results = self._add_groups(groups)
+
+        return warnings, results
+
+    def _add_groups(self, groups: dict) -> tuple:
+        """
+        Adds new groups to the groups YAML file.
+        """
+        warnings, results = [], []
+
+        # Loop through all groups:
+        for group_name, group in groups.items():
+            techniques = []
+            software = []
+            for technique_id in group['techniques']:
+                attack_technique = self._get_technique_from_attack(technique_id)
+                if attack_technique is None:
+                    warnings.append(
+                        f'Technique "{technique_id}" listed in group "{group_name}" does not exist in ATT&CK ({self.domain}). Skipping.')
+                else:
+                    techniques.append(technique_id)
+
+            for software_id in group['software']:
+                attack_software = self._get_software_from_attack(software_id)
+                if attack_software is None:
+                    warnings.append(
+                        f'Software "{software_id}" listed in group "{group_name}" does not exist in ATT&CK ({self.domain}). Skipping.')
+                else:
+                    software.append(software_id)
+
+            new_group = deepcopy(YAML_OBJ_GROUP)
+            new_group['group_name'] = group_name
+            new_group['campaign'] = group['campaign']
+            new_group['technique_id'] = techniques
+            new_group['software_id'] = software
+            self._yaml_content['groups'].append(new_group)
+
+        return warnings, results
+
+
 if __name__ == '__main__':
     # Where being run from the command line here, start CLI logic
     cli_mod = importlib.import_module('cli')
     cli = getattr(cli_mod, 'CommandLine')()
     cli.start()
```

### Comparing `dettectinator-1.1.1/dettectinator/plugins/datasources_import.py` & `dettectinator-1.2.0/dettectinator/plugins/datasources_import.py`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.1/dettectinator/plugins/support/authentication.py` & `dettectinator-1.2.0/dettectinator/plugins/support/authentication.py`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.1/dettectinator/plugins/support/msal_patch.py` & `dettectinator-1.2.0/dettectinator/plugins/support/msal_patch.py`

 * *Files identical despite different names*

### Comparing `dettectinator-1.1.1/dettectinator/plugins/technique_import.py` & `dettectinator-1.2.0/dettectinator/plugins/technique_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         parser.add_argument('-clp', '--clean_unused_location_prefix', action='store_true',
                             help='Clean unused detections based on location_prefix.')
 
     def get_attack_techniques(self, default_applicable_to: list) -> dict:
         """
         Retrieves use-case/technique data from a data source
         :param default_applicable_to: Default value for systems that the detections are applicable to (can be overrule from source)
-        :return: Dictionary, example: {'Detection A': {'applicable_to': ['all'], 'location_prefix': 'SIEM', 'techniques': ['T1055']}}
+        :return: Dictionary, example: {'Detection A': [{'applicable_to': ['all'], 'location_prefix': 'SIEM', 'techniques': ['T1055']}]}
         """
 
         use_cases = {}
 
         for technique, use_case, applicable_to in self.get_data_from_source():
             # Exclude all detections that match the exclude-pattern
             if self._re_exclude and not re.match(self._re_exclude, use_case) is None:
@@ -72,19 +72,30 @@
             # Include all detections that match the include-pattern
             if self._re_include and re.match(self._re_include, use_case) is None:
                 continue
 
             applicable_to = applicable_to or default_applicable_to
 
             if use_case in use_cases.keys():
-                use_cases[use_case]['techniques'].append(technique)
+                updated = False
+
+                for item in use_cases[use_case]:
+                    if sorted(applicable_to) == sorted(item['applicable_to']):
+                        item['techniques'].append(technique)
+                        updated = True
+                        break
+
+                if not updated:
+                    use_cases[use_case].append({'applicable_to': applicable_to,
+                                                'location_prefix': self._location_prefix,
+                                                'techniques': [technique]})
             else:
-                use_cases[use_case] = {'applicable_to': applicable_to,
-                                       'location_prefix': self._location_prefix,
-                                       'techniques': [technique]}
+                use_cases[use_case] = [{'applicable_to': applicable_to,
+                                        'location_prefix': self._location_prefix,
+                                        'techniques': [technique]}]
 
         return use_cases
 
     def get_data_from_source(self) -> Iterable:
         """
         Gets the use-case/technique data from the source.
         :return: Iterable, yields technique, detection, applicable_to
@@ -299,19 +310,19 @@
     More info:
     https://learn.microsoft.com/en-us/defender-for-identity/alerts-overview
     """
 
     def __init__(self, parameters: dict) -> None:
         super().__init__(parameters)
 
-        self.ATP_DOCS = ['https://raw.githubusercontent.com/MicrosoftDocs/ATADocs/master/ATPDocs/compromised-credentials-alerts.md',
-                         'https://raw.githubusercontent.com/MicrosoftDocs/ATADocs/master/ATPDocs/domain-dominance-alerts.md',
-                         'https://raw.githubusercontent.com/MicrosoftDocs/ATADocs/master/ATPDocs/exfiltration-alerts.md',
+        self.ATP_DOCS = ['https://github.com/MicrosoftDocs/ATADocs/blob/master/ATPDocs/credential-access-alerts.md',
                          'https://raw.githubusercontent.com/MicrosoftDocs/ATADocs/master/ATPDocs/lateral-movement-alerts.md',
-                         'https://raw.githubusercontent.com/MicrosoftDocs/ATADocs/master/ATPDocs/reconnaissance-alerts.md']
+                         'https://raw.githubusercontent.com/MicrosoftDocs/ATADocs/master/ATPDocs/reconnaissance-discovery-alerts.md',
+                         'https://raw.githubusercontent.com/MicrosoftDocs/ATADocs/master/ATPDocs/persistence-privilege-escalation-alerts.md',
+                         'https://raw.githubusercontent.com/MicrosoftDocs/ATADocs/master/ATPDocs/other-alerts.md']
 
     @staticmethod
     def set_plugin_params(parser: ArgumentParser) -> None:
         """
         Set command line arguments specific for the plugin
         :param parser: Argument parser
         """
@@ -320,47 +331,50 @@
     def get_data_from_source(self) -> Iterable:
         """
         Gets the use-case/technique data from the source.
         :return: Iterable, yields technique, detection, applicable_to
         """
         for source_url in self.ATP_DOCS:
             resp = requests.get(source_url)
-            body = resp.text
+            if resp.status_code == 200:
+                body = resp.text
 
-            # Remove comments from file, because it may contain commented detection rules.
-            while '<!--' in body:
-                body = body[0:body.find('<!--')] + body[body.find('-->')+3:]
-
-            regex_title = re.compile('##\s(.*\s\(external\sID\s\d{4}\))')
-            regex_tech = re.compile('\((T\d{4})\)')
-            regex_subtech = re.compile('(T\d{4}\.\d{3})')
-
-            current_detection = None
-            for line in body.splitlines():
-                title_match = regex_title.match(line)
-                if title_match or current_detection is None:
-                    if title_match:
-                        current_detection = title_match.group(1)
-                        continue
-                else:
-                    if 'MITRE attack technique' in line and 'N/A' in line:
-                        current_detection = None
-                    elif 'MITRE attack technique' in line:
-                        tech_match = regex_tech.findall(line)
-                        if tech_match:
-                            for t in tech_match:
-                                yield t, current_detection, None
-                    elif 'MITRE attack sub-technique' in line and 'N/A' in line:
-                        current_detection = None
-                    elif 'MITRE attack sub-technique' in line:
-                        subtech_match = regex_subtech.findall(line)
-                        if subtech_match:
-                            for t in subtech_match:
-                                yield t, current_detection, None
+                # Remove comments from file, because it may contain commented detection rules.
+                while '<!--' in body:
+                    body = body[0:body.find('<!--')] + body[body.find('-->')+3:]
+
+                regex_title = re.compile('##\s(.*\s\(external\sID\s\d{4}\))')
+                regex_tech = re.compile('\((T\d{4})\)')
+                regex_subtech = re.compile('(T\d{4}\.\d{3})')
+
+                current_detection = None
+                for line in body.splitlines():
+                    title_match = regex_title.match(line)
+                    if title_match or current_detection is None:
+                        if title_match:
+                            current_detection = title_match.group(1)
+                            continue
+                    else:
+                        if 'MITRE attack technique' in line and 'N/A' in line:
+                            current_detection = None
+                        elif 'MITRE attack technique' in line:
+                            tech_match = regex_tech.findall(line)
+                            if tech_match:
+                                for t in tech_match:
+                                    yield t, current_detection, None
+                        elif 'MITRE attack sub-technique' in line and 'N/A' in line:
                             current_detection = None
+                        elif 'MITRE attack sub-technique' in line:
+                            subtech_match = regex_subtech.findall(line)
+                            if subtech_match:
+                                for t in subtech_match:
+                                    yield t, current_detection, None
+                                current_detection = None
+            else:
+                print(f'Received HTTP status code "{resp.status_code}" on URL "{source_url}".')
 
 
 class TechniqueDefenderAlerts(TechniqueAzureAuthBase):
     """
     Import alerts and techniques from the Microsoft Defender API.
     """
     def __init__(self, parameters: dict) -> None:
```

### Comparing `dettectinator-1.1.1/dettectinator.egg-info/PKG-INFO` & `dettectinator-1.2.0/dettectinator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dettectinator
-Version: 1.1.1
+Version: 1.2.0
 Summary: Dettectinator - The Python library to your DeTT&CT YAML files.
 Home-page: https://github.com/siriussecurity/dettectinator
 Author: Sirius Security
 License: GPL3
 Project-URL: Documentation, https://github.com/siriussecurity/dettectinator/wiki
 Project-URL: Code, https://github.com/siriussecurity/dettectinator
 Project-URL: Issue tracker, https://github.com/siriussecurity/dettectinator/issues
```

### Comparing `dettectinator-1.1.1/dettectinator.egg-info/SOURCES.txt` & `dettectinator-1.2.0/dettectinator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,11 +9,12 @@
 dettectinator.egg-info/PKG-INFO
 dettectinator.egg-info/SOURCES.txt
 dettectinator.egg-info/dependency_links.txt
 dettectinator.egg-info/requires.txt
 dettectinator.egg-info/top_level.txt
 dettectinator/plugins/__init__.py
 dettectinator/plugins/datasources_import.py
+dettectinator/plugins/groups_import.py
 dettectinator/plugins/technique_import.py
 dettectinator/plugins/support/__init__.py
 dettectinator/plugins/support/authentication.py
 dettectinator/plugins/support/msal_patch.py
```

### Comparing `dettectinator-1.1.1/setup.py` & `dettectinator-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 
 Currently de CLI is limited to processing detections through these plugins, the library can also be used for processing data sources.
 
 See the [documentation](https://github.com/siriussecurity/dettectinator) for more information on how to use it."""
 
 setuptools.setup(
     name="dettectinator",
-    version="1.1.1",
+    version="1.2.0",
     author="Sirius Security",
     description="Dettectinator - The Python library to your DeTT&CT YAML files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/siriussecurity/dettectinator",
     project_urls={
         "Documentation": "https://github.com/siriussecurity/dettectinator/wiki",
         "Code": "https://github.com/siriussecurity/dettectinator",
         "Issue tracker": "https://github.com/siriussecurity/dettectinator/issues",
     },
     keywords="mitre attack dettect soc threat hunting",
     packages=setuptools.find_packages(exclude=["examples", "tests"]),
     install_requires=["requests", "ruamel.yaml", "attackcti", "python-dateutil", "msal", "stix2",
-                      "openpyxl", "suricataparser", "addonfactory-splunk-conf-parser-lib", "pandas", "anyascii"],
+                      "openpyxl", "suricataparser", "addonfactory-splunk-conf-parser-lib", "pandas",
+                      "anyascii", "pypdf"],
     license='GPL3',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Operating System :: OS Independent',
         'Topic :: Security',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.9'
```

