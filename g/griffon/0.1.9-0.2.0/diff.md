# Comparing `tmp/griffon-0.1.9.tar.gz` & `tmp/griffon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griffon-0.1.9.tar", last modified: Fri Mar 31 11:59:25 2023, max compression
+gzip compressed data, was "griffon-0.2.0.tar", last modified: Wed May 10 08:52:14 2023, max compression
```

## Comparing `griffon-0.1.9.tar` & `griffon-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.885891 griffon-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-31 11:59:11.000000 griffon-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-31 11:59:25.885891 griffon-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-31 11:59:11.000000 griffon-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.881891 griffon-0.1.9/griffon/
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.881891 griffon-0.1.9/griffon/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.885891 griffon-0.1.9/griffon/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18280 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/plugin_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.885891 griffon-0.1.9/griffon/commands/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/plugins/cve_mitre.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/plugins/cvelib.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/plugins/fcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/plugins/go_vuln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/plugins/osv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    22098 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30001 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.885891 griffon-0.1.9/griffon/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/services/core_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    37876 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/services/core_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/services/core_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.885891 griffon-0.1.9/griffon/static/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-31 11:59:11.000000 griffon-0.1.9/griffon/static/default_griffonrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.881891 griffon-0.1.9/griffon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-31 11:59:25.000000 griffon-0.1.9/griffon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-31 11:59:25.000000 griffon-0.1.9/griffon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 11:59:25.000000 griffon-0.1.9/griffon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-31 11:59:25.000000 griffon-0.1.9/griffon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-31 11:59:25.000000 griffon-0.1.9/griffon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-31 11:59:25.000000 griffon-0.1.9/griffon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-31 11:59:11.000000 griffon-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 11:59:25.885891 griffon-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-31 11:59:11.000000 griffon-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 11:59:25.885891 griffon-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-31 11:59:11.000000 griffon-0.1.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-31 11:59:11.000000 griffon-0.1.9/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-31 11:59:11.000000 griffon-0.1.9/tests/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-31 11:59:11.000000 griffon-0.1.9/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-31 11:59:11.000000 griffon-0.1.9/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-31 11:59:11.000000 griffon-0.1.9/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-31 11:59:11.000000 griffon-0.1.9/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-31 11:59:11.000000 griffon-0.1.9/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 08:51:59.000000 griffon-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-10 08:52:14.970026 griffon-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-10 08:51:59.000000 griffon-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.966026 griffon-0.2.0/griffon/
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.966026 griffon-0.2.0/griffon/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/commands/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26909 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/community_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/corgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/entities/osidb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugin_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/commands/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/cve_mitre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/cvelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/fcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/go_vuln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/osv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/plugins/semgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24015 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38678 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/services/core_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38394 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/services/core_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20730 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/services/core_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/griffon/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-10 08:51:59.000000 griffon-0.2.0/griffon/static/default_griffonrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.966026 griffon-0.2.0/griffon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-10 08:52:14.000000 griffon-0.2.0/griffon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-10 08:51:59.000000 griffon-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:52:14.970026 griffon-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-10 08:51:59.000000 griffon-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:14.970026 griffon-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 08:51:59.000000 griffon-0.2.0/tests/test_unit.py
```

### Comparing `griffon-0.1.9/LICENSE` & `griffon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/PKG-INFO` & `griffon-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.1.9
+Version: 0.2.0
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,26 +36,25 @@
   -d, --debug                     Debug log level.
   -f, --format [json|text|table]  Result format (default is text format).
   -v                              Verbose output, more detailed search
                                   results, can be used multiple times (e.g.
                                   -vvv).
   --no-progress-bar               Disable progress bar.
   --no-color                      Disable output of color ansi esc sequences.
-  --profile [cloud|openshift|middleware|latest|all]
+  --profile [default|cloud|openshift|middleware|latest]
                                   Activate profile, defined in .griffonrc.
+  --editor / --no-editor          Allow text editor prompt.
   --help                          Show this message and exit.
 
 Commands:
   configure  Configure griffon.
   docs       Links to useful docs.
-  entities   Entity operations (UNDER DEVELOPMENT).
-  manage     Manage operations.
+  entities   Entity operations.
   plugins    3rd party plugins.
   service    Service operations.
-
 ```
 To install:
 
 ```commandline
 pip install griffon
 ```
```

### Comparing `griffon-0.1.9/README.md` & `griffon-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,26 +22,25 @@
   -d, --debug                     Debug log level.
   -f, --format [json|text|table]  Result format (default is text format).
   -v                              Verbose output, more detailed search
                                   results, can be used multiple times (e.g.
                                   -vvv).
   --no-progress-bar               Disable progress bar.
   --no-color                      Disable output of color ansi esc sequences.
-  --profile [cloud|openshift|middleware|latest|all]
+  --profile [default|cloud|openshift|middleware|latest]
                                   Activate profile, defined in .griffonrc.
+  --editor / --no-editor          Allow text editor prompt.
   --help                          Show this message and exit.
 
 Commands:
   configure  Configure griffon.
   docs       Links to useful docs.
-  entities   Entity operations (UNDER DEVELOPMENT).
-  manage     Manage operations.
+  entities   Entity operations.
   plugins    3rd party plugins.
   service    Service operations.
-
 ```
 To install:
 
 ```commandline
 pip install griffon
 ```
```

### Comparing `griffon-0.1.9/griffon/autocomplete/__init__.py` & `griffon-0.2.0/griffon/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/cli.py` & `griffon-0.2.0/griffon/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     list_config_sections,
     print_version,
 )
 
 from .commands.configure import configure_grp
 from .commands.docs import docs_grp
 from .commands.entities import entities_grp
-from .commands.manage import manage_grp
 from .commands.plugin_commands import plugin_commands
 from .commands.queries import queries_grp
 from .output import OUTPUT_FORMAT
 
 logger = logging.getLogger("griffon")
 
 click_completion.init()
@@ -42,23 +41,14 @@
 
 
 entities.add_command(entities_grp)
 
 
 @click.group()
 @click.pass_context
-def manage(ctx):
-    pass
-
-
-manage.add_command(manage_grp)
-
-
-@click.group()
-@click.pass_context
 def services_grp(ctx):
     pass
 
 
 services_grp.add_command(queries_grp)
 
 
@@ -87,15 +77,15 @@
 #
 #   A click.CommandCollection is used to aggregate up all CLI sub commands.
 #   Top level CLI options (germane to all commands) are included here.
 
 
 @click.group(
     cls=click.CommandCollection,
-    sources=(configure, entities, services_grp, manage, docs, plugins),
+    sources=(configure, entities, services_grp, docs, plugins),
 )
 @click.option(
     "--version",
     "-V",
     is_flag=True,
     callback=print_version,
     expose_value=False,
@@ -125,16 +115,17 @@
     type=click.Choice(list_config_sections()),
     default=get_config_option(
         "default",
         "profile",
     ),
     help="Activate profile, defined in .griffonrc.",
 )
+@click.option("--editor/--no-editor", default=True, help="Allow text editor prompt.")
 @click.pass_context
-def cli(ctx, debug, format, verbose, no_progress_bar, no_color, profile):
+def cli(ctx, debug, format, verbose, no_progress_bar, no_color, profile, editor):
     """Red Hat product security CLI"""
 
     if ctx.invoked_subcommand is None:
         click.echo(ctx.parent.get_help())
 
     if not debug:
         config_logging(level="INFO")
@@ -148,10 +139,11 @@
     ctx.obj["SHOW_UPSTREAM"] = False
     ctx.obj["FORMAT"] = format
     ctx.obj["VERBOSE"] = verbose
     ctx.obj["NO_PROGRESS_BAR"] = no_progress_bar
     ctx.obj["NO_COLOR"] = no_color
     ctx.obj["PROFILE"] = profile
     ctx.obj["SHORT_VERSION_VALUES"] = True
+    ctx.obj["EDITOR"] = editor
 
 
 cli.help = "Red Hat Product Security CLI"
```

### Comparing `griffon-0.1.9/griffon/commands/configure.py` & `griffon-0.2.0/griffon/commands/configure.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/commands/docs.py` & `griffon-0.2.0/griffon/commands/docs.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/commands/entities.py` & `griffon-0.2.0/griffon/commands/entities/corgi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,332 +1,175 @@
 """
-entity operations
+corgi entity operations
 
 """
 import concurrent.futures
 import logging
 
 import click
-
-from griffon import (
-    CORGI_API_URL,
-    OSIDB_API_URL,
-    CorgiService,
-    OSIDBService,
-    progress_bar,
+import requests
+from component_registry_bindings.bindings.python_client.api.v1 import (
+    v1_builds_list,
+    v1_builds_retrieve,
+    v1_channels_list,
+    v1_channels_retrieve,
+    v1_components_list,
+    v1_components_retrieve,
+    v1_product_streams_list,
+    v1_product_streams_retrieve,
+    v1_product_variants_list,
+    v1_product_variants_retrieve,
+    v1_product_versions_list,
+    v1_product_versions_retrieve,
+    v1_products_list,
+    v1_products_retrieve,
+)
+from component_registry_bindings.bindings.python_client.models import (
+    Channel,
+    Component,
+    Product,
+    ProductStream,
+    ProductVariant,
+    ProductVersion,
+    SoftwareBuild,
 )
+
+from griffon import CORGI_API_URL, CorgiService, progress_bar
 from griffon.autocomplete import (
-    get_component_names,
     get_component_purls,
-    get_cve_ids,
     get_product_stream_names,
     get_product_stream_ofuris,
+    get_product_version_ofuris,
+)
+from griffon.commands.entities.helpers import (
+    multivalue_params_to_csv,
+    query_params_options,
 )
 from griffon.output import console, cprint
 
 logger = logging.getLogger("griffon")
 
 default_conditions: dict = {}
 
 
-@click.group(name="entities", help="Entity operations (UNDER DEVELOPMENT).")
-@click.option("--open-browser", is_flag=True, help="open browser to service results.")
-@click.option("--limit", default=10, help="# of items returned by list operations.")
-@click.pass_context
-def entities_grp(ctx, open_browser, limit):
-    ctx.ensure_object(dict)
-    ctx.obj["open_browser"] = open_browser
-    ctx.obj["limit"] = limit
-
-
-# flaws
-@entities_grp.group(help=f"{OSIDB_API_URL}/osidb/api/v1/flaws")
-@click.pass_context
-def flaws(ctx):
-    """OSIDB Flaws."""
-
-
-@flaws.command(name="list")
-@click.option(
-    "--state",
-    "flaw_state",
-    type=click.Choice(OSIDBService.get_flaw_states()),
-    help="Flaw state.",
-)
-@click.option(
-    "--resolution",
-    type=click.Choice(OSIDBService.get_flaw_resolutions()),
-    help="Flaw resolution.",
-)
-@click.option(
-    "--impact",
-    type=click.Choice(OSIDBService.get_flaw_impacts()),
-    help="Flaw impact.",
-)
-@click.option(
-    "--embargoed",
-    "is_embargoed",
-    is_flag=True,
-    help="Include embargoed flaws (requires access).",
-)
-@click.option("--major-incident", "is_major_incident", is_flag=True, help="Only major incidents.")
-@click.pass_context
-@progress_bar
-def list_flaws(ctx, flaw_state, resolution, impact, is_embargoed, is_major_incident):
-    if not flaw_state and not resolution and not impact:
-        click.echo(ctx.get_help())
-        exit(0)
-    session = OSIDBService.create_session()
-    conditions = default_conditions
-    if flaw_state:
-        conditions["state"] = flaw_state
-    if resolution:
-        conditions["resolution"] = resolution
-    if impact:
-        conditions["impact"] = impact
-    data = session.flaws.retrieve_list(**conditions).results
-    return cprint(data, ctx=ctx)
-
-
-@flaws.command(name="get")
-@click.option("--cve-id", help="Flaw CVE-ID.", shell_complete=get_cve_ids)
-@click.option(
-    "--uuid",
-    "flaw_uuid",
-    help="Flaw UUID.",
-)
-@click.pass_context
-def get_flaw(ctx, cve_id, flaw_uuid):
-    if not cve_id and not flaw_uuid:
-        click.echo(ctx.get_help())
-        exit(0)
-    session = OSIDBService.create_session()
-    if flaw_uuid:
-        data = session.flaws.retrieve(flaw_uuid)
-    if cve_id:
-        data = session.flaws.retrieve(cve_id)
-    return cprint(data, ctx=ctx)
-
-
-# affects
-@entities_grp.group(help=f"{OSIDB_API_URL}/osidb/api/v1/affects")
+@click.group(name="component-registry")
 @click.pass_context
-def affects(ctx):
-    """OSIDB Affects."""
+def corgi_grp(ctx):
     pass
 
 
-@affects.command(name="list")
-@click.option("--product_version", help="ps module")
-@click.option("--component_name", help="ps component")
-@click.option("--affectedness", type=click.Choice(OSIDBService.get_affect_affectedness()))
-@click.option(
-    "--resolution",
-    type=click.Choice(OSIDBService.get_affect_resolution()),
-)
-@click.option("--impact", type=click.Choice(OSIDBService.get_affect_impact()))
-@click.pass_context
-@progress_bar
-def list_affects(ctx, product_version, component_name, affectedness, resolution, impact):
-    if (
-        not product_version
-        and not component_name
-        and not affectedness
-        and not resolution
-        and not impact
-    ):
-        click.echo(ctx.get_help())
-        exit(0)
-    session = OSIDBService.create_session()
-    conditions = default_conditions
-    if product_version:
-        conditions["ps_module"] = product_version
-    if component_name:
-        conditions["ps_component"] = component_name
-    if affectedness:
-        conditions["affectedness"] = affectedness
-    if resolution:
-        conditions["resolution"] = resolution
-    if impact:
-        conditions["impact"] = impact
-    data = session.affects.retrieve_list(**conditions).results
-    return cprint(data, ctx=ctx)
-
-
-@affects.command(name="get")
-@click.option("--uuid", "affect_uuid")
-@click.pass_context
-def get_affect(ctx, affect_uuid):
-    if not affect_uuid:
-        click.echo(ctx.get_help())
-        exit(0)
-    session = OSIDBService.create_session()
-    data = session.affects.retrieve(affect_uuid)
-    return cprint(data, ctx=ctx)
-
-
-# trackers
-@entities_grp.group(help=f"{OSIDB_API_URL}/osidb/api/v1/trackers")
-@click.pass_context
-def trackers(ctx):
-    """OSIDB Trackers."""
-    pass
+# COMPONENTS
 
 
-@trackers.command(name="list")
-@click.pass_context
-def list_trackers(ctx):
-    session = OSIDBService.create_session()
-    conditions = default_conditions
-    data = session.trackers.retrieve_list(**conditions).results
-    return cprint(data, ctx=ctx)
-
-
-@trackers.command(name="get")
-@click.option("--uuid", "tracker_uuid")
-@click.pass_context
-@progress_bar
-def get_tracker(ctx, tracker_uuid):
-    if not tracker_uuid:
-        click.echo(ctx.get_help())
-        exit(0)
-    session = OSIDBService.create_session()
-    data = session.trackers.retrieve(tracker_uuid)
-    return cprint(data, ctx=ctx)
-
-
-# components
-@entities_grp.group(help=f"{CORGI_API_URL}/api/v1/components")
+@corgi_grp.group(help=f"{CORGI_API_URL}/api/v1/components")
 @click.pass_context
 def components(ctx):
-    pass
+    """Corgi Components."""
 
 
 @components.command(name="list")
 @click.argument("component_name", required=False)
-@click.option("--namespace", type=click.Choice(CorgiService.get_component_namespaces()), help="")
-@click.option("--ofuri", shell_complete=get_product_stream_ofuris)
-@click.option("--re_purl", shell_complete=get_component_purls)
-@click.option("--re_name", shell_complete=get_component_names)
-@click.option("--version")
 @click.option(
-    "--type",
-    "component_type",
-    type=click.Choice(CorgiService.get_component_types()),
-    help="",  # noqa
+    "-s",
+    "strict_name_search",
+    is_flag=True,
+    default=False,
+    help="Strict search, exact match of component name.",
 )
-@click.option(
-    "--arch",
-    type=click.Choice(CorgiService.get_component_arches()),
+@query_params_options(
+    entity="Component",
+    endpoint_module=v1_components_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Component))},
+    },
 )
-@click.option("--product-stream-name", shell_complete=get_product_stream_names)
-@click.option("--product-stream-ofuri", shell_complete=get_product_stream_ofuris)
 @click.pass_context
 @progress_bar
-def list_components(
-    ctx,
-    component_name,
-    namespace,
-    ofuri,
-    re_purl,
-    re_name,
-    version,
-    component_type,
-    arch,
-    product_stream_name,
-    product_stream_ofuri,
-):
-    """Retrieve a list of Components."""
-
-    if (
-        not component_name
-        and not ofuri
-        and not re_purl
-        and not re_name
-        and not version
-        and not arch
-        and not namespace
-        and not component_type
-        and not product_stream_name
-        and not product_stream_ofuri
-    ):
+def list_components(ctx, strict_name_search, component_name, **params):
+    # TODO: handle pagination
+    # TODO: handle output
+    is_params_empty = [False for v in params.values() if v]
+    if not component_name and not is_params_empty:
         click.echo(ctx.get_help())
         exit(0)
-    session = CorgiService.create_session()
-
-    conditions = default_conditions
-    conditions[
-        "include_fields"
-    ] = "link,purl,nvr,version,type,name,upstreams,related_url,download_url"
-
-    # TODO- condition union could be a separate helper function
+    if strict_name_search:
+        params["name"] = component_name
+    elif component_name:
+        params["re_name"] = component_name
 
-    if component_name:
-        conditions["name"] = component_name
+    if not params["include_fields"]:
+        params[
+            "include_fields"
+        ] = "link,uuid,purl,nvr,version,type,name,upstreams,related_url,download_url"
 
-    if namespace:
-        conditions["namespace"] = namespace
-    if ofuri:
-        conditions["ofuri"] = ofuri
-    if re_purl:
-        conditions["re_purl"] = re_purl
-    if re_name:
-        conditions["re_name"] = re_name
-    if version:
-        conditions["version"] = version
-    if arch:
-        conditions["arch"] = arch
-    if component_type:
-        conditions["type"] = component_type
-    if product_stream_ofuri:
-        conditions["product_streams"] = product_stream_ofuri
+    session = CorgiService.create_session()
+    params = multivalue_params_to_csv(params)
 
-    # TODO- This kind of optimisation should probably be developed in the
-    #       service binding itself rather then here
     logger.debug("starting parallel http requests")
-    component_cnt = session.components.retrieve_list(**conditions).count
+    component_cnt = session.components.retrieve_list(**params).count
+    logger.debug(component_cnt)
     if component_cnt < 3000000:
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = []
             components = list()
             for batch in range(0, component_cnt, 1200):
+                params["offset"] = batch
+                params["limit"] = 1200
                 futures.append(
                     executor.submit(
                         session.components.retrieve_list,
-                        **conditions,
-                        offset=batch,
-                        limit=1200,  # noqa
+                        **params,
                     )
                 )
 
             for future in concurrent.futures.as_completed(futures):
                 try:
                     components.extend(future.result().results)
                 except Exception as exc:
                     logger.warning("%r generated an exception: %s" % (future, exc))
 
             data = sorted(components, key=lambda d: d.purl)
             return cprint(data, ctx=ctx)
     else:
-        console.print("downloading too many")
+        console.warning("Too many components.")
 
 
 @components.command(name="get")
-@click.option("--uuid", "component_uuid")
-@click.option("--purl", shell_complete=get_component_purls, help="Purl are URI and must be quoted.")
-@click.option("--nvr")
+@click.argument("component_id", required=False)
+@click.option("--purl", shell_complete=get_component_purls, help="purls must be quoted!")
+@query_params_options(
+    entity="Component",
+    endpoint_module=v1_components_retrieve,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Component))},
+    },
+)
 @click.pass_context
 @progress_bar
-def get_component(ctx, component_uuid, purl, nvr):
-    """Retrieve Component."""
-    if not component_uuid and not purl and not nvr:
+def get_component(ctx, component_id, purl, **params):
+    is_params_empty = [False for v in params.values() if v]
+    if not component_id and not purl and not is_params_empty:
         click.echo(ctx.get_help())
         exit(0)
+
+    if purl:
+        params["purl"] = purl
+
+    if not params["include_fields"]:
+        params[
+            "include_fields"
+        ] = "link,purl,nvr,version,type,name,upstreams,related_url,download_url"
+
+    params = multivalue_params_to_csv(params)
+
     session = CorgiService.create_session()
-    data = session.components.retrieve_list(purl=purl)
+    if component_id:
+        data = session.components.retrieve(component_id, **params)
+    else:
+        data = session.components.retrieve_list(**params)
     return cprint(data, ctx=ctx)
 
 
 @components.command(
     name="summary",
     help="Get Component summaries.",
 )
@@ -337,19 +180,27 @@
 @click.option(
     "-s",
     "strict_name_search",
     is_flag=True,
     default=False,
     help="Strict search, exact match of name.",
 )
+@query_params_options(
+    entity="Component",
+    endpoint_module=v1_components_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Component))},
+    },
+)
 @click.pass_context
 @progress_bar
-def get_component_summary(ctx, component_name, strict_name_search):
+def get_component_summary(ctx, component_name, strict_name_search, **params):
     """Get Component summary."""
-    if not component_name:
+    is_params_empty = [False for v in params.values() if v]
+    if not component_name and not is_params_empty:
         click.echo(ctx.get_help())
         exit(0)
     session = CorgiService.create_session()
 
     cond = {
         "include_fields": "name,type,download_url,purl,tags,arch,release,version,product_streams,upstreams,related_url",  # noqa
         "name": component_name,
@@ -375,27 +226,27 @@
             upstreams.append(upstream["purl"])
         for ps in component.product_streams:
             product_streams.append(ps["name"])
 
     cond = {
         "include_fields": "name,purl,version,type,tags,arch,release,product_streams",  # noqa
         "name": component_name,
-        "view": "latest",
+        "latest_components_by_streams": True,
     }
-    latest_components = session.components.retrieve_list(**cond, limit=10000)
-
+    # latest_components = session.components.retrieve_list(**cond, limit=10000)
+    #
     latest = []
 
-    for latest_component in latest_components.results:
-        latest.append(
-            {
-                "product_stream": latest_component["product_stream"],
-                "purl": latest_component.purl,
-            }
-        )
+    # for latest_component in latest_components.results:
+    #     latest.append(
+    #         {
+    #             "product_stream": latest_component["product_stream"],
+    #             "purl": latest_component.purl,
+    #         }
+    #     )
     data = {
         "link": f"{CORGI_API_URL}/api/v1/components?name={component_name}",
         "type": component_type,
         "name": component_name,
         "tags": sorted(list(set(tags))),
         "count": len(components.results),
         "product_streams": sorted(list(set(product_streams))),
@@ -409,189 +260,619 @@
     }
     cprint(data, ctx=ctx)
 
 
 @components.command(name="provides")
 @click.option("--uuid", "component_uuid")
 @click.option("--purl", shell_complete=get_component_purls, help="Purl are URI and must be quoted.")
+@query_params_options(
+    entity="Component",
+    endpoint_module=v1_components_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Component))},
+    },
+)
 @click.pass_context
 @progress_bar
-def get_component_provides(ctx, component_uuid, purl):
+def get_component_provides(ctx, component_uuid, purl, **params):
     """Retrieve all Components provided by a Component."""
-    if not component_uuid and not purl:
+    is_params_empty = [False for v in params.values() if v]
+    if not component_uuid and not purl and not is_params_empty:
         click.echo(ctx.get_help())
         exit(0)
+    if not params["include_fields"]:
+        params[
+            "include_fields"
+        ] = "link,purl,nvr,version,type,name,upstreams,related_url,download_url"
+    if purl:
+        params["sources"] = purl
+
     session = CorgiService.create_session()
     if component_uuid:
-        data = session.components.retrieve(component_uuid).provides
+        purl = session.components.retrieve(component_uuid).purl
+        params["sources"] = purl
+        data = session.components.retrieve_list(**params)
         return cprint(data, ctx=ctx)
     else:
-        c = session.components.retrieve_list(purl=purl)
-        if c:
-            data = session.components.retrieve(c["uuid"]).provides
-            return cprint(data, ctx=ctx)
+        data = session.components.retrieve_list(**params)
+        return cprint(data, ctx=ctx)
 
 
 @components.command(name="sources")
 @click.option("--uuid", "component_uuid")
 @click.option("--purl", shell_complete=get_component_purls, help="Purl are URI and must be quoted.")
+@query_params_options(
+    entity="Component",
+    endpoint_module=v1_components_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Component))},
+    },
+)
 @click.pass_context
 @progress_bar
-def get_component_sources(ctx, component_uuid, purl):
+def get_component_sources(ctx, component_uuid, purl, **params):
     """Retrieve all Components that contain Component."""
-    if not component_uuid and not purl:
+    is_params_empty = [False for v in params.values() if v]
+    if not component_uuid and not purl and not is_params_empty:
         click.echo(ctx.get_help())
         exit(0)
+    if not params["include_fields"]:
+        params[
+            "include_fields"
+        ] = "link,purl,nvr,version,type,name,upstreams,related_url,download_url"
+    if purl:
+        params["provides"] = purl
     session = CorgiService.create_session()
     if component_uuid:
-        data = session.components.retrieve(component_uuid).sources
+        purl = session.components.retrieve(component_uuid).purl
+        params["provides"] = purl
+        data = session.components.retrieve_list(**params)
         return cprint(data, ctx=ctx)
     else:
-        c = session.components.retrieve_list(purl=purl)
-        if c:
-            data = session.components.retrieve(c["uuid"]).sources
-            return cprint(data, ctx=ctx)
+        data = session.components.retrieve_list(**params)
+        return cprint(data, ctx=ctx)
 
 
 @components.command(name="manifest")
 @click.option("--uuid", "component_uuid")
 @click.option("--purl", shell_complete=get_component_purls, help="Purl are URI and must be quoted.")
+@click.option(
+    "--spdx-json",
+    "spdx_json_format",
+    is_flag=True,
+    default=False,
+    help="Generate spdx manifest (json).",
+)
 @click.pass_context
 @progress_bar
-def get_component_manifest(ctx, component_uuid, purl):
+def get_component_manifest(ctx, component_uuid, purl, spdx_json_format):
     """Retrieve Component manifest."""
     if not component_uuid and not purl:
         click.echo(ctx.get_help())
         exit(0)
+    if spdx_json_format:
+        ctx.ensure_object(dict)
+        ctx.obj["FORMAT"] = "json"  # TODO - investigate if we need yaml format.
     session = CorgiService.create_session()
     if component_uuid:
         data = session.components.retrieve_manifest(component_uuid)
         return cprint(data, ctx=ctx)
     else:
         c = session.components.retrieve_list(purl=purl)
         if c:
             data = session.components.retrieve_manifest(c["uuid"])
             return cprint(data, ctx=ctx)
 
 
-# product streams
-@entities_grp.group(help=f"{CORGI_API_URL}/api/v1/product_streams")
+@components.command(name="tree")
+@click.option("--uuid", "component_uuid")
+@click.option("--nvr", "nvr")
+@click.option("--purl", shell_complete=get_component_purls, help="Purl are URI and must be quoted.")
+@click.option(
+    "--show-purl",
+    "show_purl",
+    is_flag=True,
+    default=False,
+    help="Display purl.",
+)
+@click.pass_context
+@progress_bar
+def get_component_tree(ctx, component_uuid, nvr, purl, show_purl):
+    """Retrieve Component dependency tree."""
+    if not component_uuid and not purl and not nvr:
+        click.echo(ctx.get_help())
+        exit(0)
+    ctx.ensure_object(dict)
+    # ctx.obj["FORMAT"] = "text"
+    session = CorgiService.create_session()
+    if purl:
+        c = session.components.retrieve_list(purl=purl, include_fields="uuid")
+        component_uuid = c["uuid"]
+    elif nvr:
+        c = session.components.retrieve_list(nvr=nvr, include_fields="uuid")
+        component_uuid = c.results[0].uuid
+    c = session.components.retrieve(component_uuid, include_fields="uuid,nvr,arch")
+    if c.arch == "src" or c.arch == "noarch":
+        data = requests.get(f"{CORGI_API_URL}/api/v1/components/{component_uuid}/taxonomy")
+        return cprint(data.json(), ctx=ctx)
+    else:
+        logger.info(f"{c.nvr},{c.arch} not a root component.")
+
+
+# PRODUCT STREAM
+@corgi_grp.group(help=f"{CORGI_API_URL}/api/v1/product_streams")
 @click.pass_context
 def product_streams(ctx):
     pass
 
 
 @product_streams.command(name="list")
 @click.argument(
     "product_stream_name",
     required=False,
     type=click.STRING,
     shell_complete=get_product_stream_names,
 )
+@query_params_options(
+    entity="ProductStream",
+    endpoint_module=v1_product_streams_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(ProductStream))},
+    },
+)
 @click.pass_context
-def list_product_streams(ctx, product_stream_name):
+def list_product_streams(ctx, product_stream_name, **params):
     """Retrieve a list of Product Streams."""
+    is_params_empty = [False for v in params.values() if v]
+    if not product_stream_name and not is_params_empty:
+        click.echo(ctx.get_help())
+        exit(0)
     session = CorgiService.create_session()
-    cond = default_conditions
+    if not params["include_fields"]:
+        params["include_fields"] = "link,uuid,ofuri,name"
+
     if product_stream_name:
-        cond["re_name"] = product_stream_name
-    data = session.product_streams.retrieve_list(**cond, limit=1000).results
+        params["re_name"] = product_stream_name
+    data = session.product_streams.retrieve_list(**params).results
     return cprint(data, ctx=ctx)
 
 
 @product_streams.command(name="get")
 @click.argument(
     "product_stream_name",
     required=False,
     type=click.STRING,
     shell_complete=get_product_stream_names,
 )
 @click.option("--inactive", is_flag=True, default=False, help="Show inactive project streams")
 @click.option("--ofuri", "ofuri", type=click.STRING, shell_complete=get_product_stream_ofuris)
+@query_params_options(
+    entity="ProductStream",
+    endpoint_module=v1_product_streams_retrieve,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(ProductStream))},
+    },
+)
 @click.pass_context
 @progress_bar
-def get_product_stream(ctx, product_stream_name, inactive, ofuri):
+def get_product_stream(ctx, product_stream_name, inactive, ofuri, **params):
     """Retrieve Product Stream."""
-    if not ofuri and not product_stream_name:
+    is_params_empty = [False for v in params.values() if v]
+    if not product_stream_name and not is_params_empty:
         click.echo(ctx.get_help())
         exit(0)
     session = CorgiService.create_session()
-    cond = {}
     if ofuri:
-        cond["ofuri"] = ofuri
+        params["ofuri"] = ofuri
     if product_stream_name:
-        cond["name"] = product_stream_name
-    data = session.product_streams.retrieve_list(**cond)
+        params["name"] = product_stream_name
+    data = session.product_streams.retrieve_list(**params)
     return cprint(data, ctx=ctx)
 
 
 @product_streams.command(name="latest-components")
 @click.argument(
     "product_stream_name",
     required=False,
     type=click.STRING,
     shell_complete=get_product_stream_names,
 )
-@click.option("--namespace", type=click.Choice(CorgiService.get_component_namespaces()), help="")
 @click.option("--ofuri", "ofuri", type=click.STRING, shell_complete=get_product_stream_ofuris)
-@click.option("--view", default="summary")
+@query_params_options(
+    entity="Component",
+    endpoint_module=v1_components_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Component))},
+    },
+)
 @click.pass_context
-def get_product_stream_components(ctx, product_stream_name, namespace, ofuri, view):
+def get_product_stream_components(ctx, product_stream_name, ofuri, **params):
     """Retrieve Product Stream latest Components."""
     if not ofuri and not product_stream_name:
         click.echo(ctx.get_help())
         exit(0)
-    ctx.invoke(list_components, ofuri=ofuri)
+    if not params["include_fields"]:
+        params[
+            "include_fields"
+        ] = "link,uuid,purl,nvr,version,type,name,upstreams,related_url,download_url"
+
+    if product_stream_name:
+        session = CorgiService.create_session()
+        ps = session.product_streams.retrieve_list(name=product_stream_name)
+        params["ofuri"] = ps["ofuri"]
+    if ofuri:
+        params["ofuri"] = ofuri
+    ctx.invoke(list_components, **params)
 
 
 @product_streams.command(name="manifest")
 @click.argument(
     "product_stream_name",
     required=False,
     type=click.STRING,
     shell_complete=get_product_stream_names,
 )
 @click.option("--ofuri", "ofuri", type=click.STRING, shell_complete=get_product_stream_ofuris)
+@click.option(
+    "--spdx-json",
+    "spdx_json_format",
+    is_flag=True,
+    default=False,
+    help="Generate spdx manifest (json).",
+)
 @click.pass_context
-def get_product_stream_manifest(ctx, product_stream_name, ofuri):
+@progress_bar
+def get_product_stream_manifest(ctx, product_stream_name, ofuri, spdx_json_format):
     """Retrieve Product Stream manifest."""
     if not ofuri and not product_stream_name:
         click.echo(ctx.get_help())
         exit(0)
     session = CorgiService.create_session()
-    pv = None
+    if spdx_json_format:
+        ctx.ensure_object(dict)
+        ctx.obj["FORMAT"] = "json"  # TODO - investigate if we need yaml format.
+    ps = None
     if ofuri:
-        pv = session.product_streams.retrieve_list(ofuri=ofuri).additional_properties
+        ps = session.product_streams.retrieve_list(ofuri=ofuri).additional_properties
     if product_stream_name:
-        pv = session.product_streams.retrieve_list(name=product_stream_name).additional_properties
-    if pv:
-        data = session.product_streams.retrieve_manifest(pv["uuid"])
-        return cprint(data, ctx=ctx)
+        ps = session.product_streams.retrieve_list(name=product_stream_name).additional_properties
+    if not ps:
+        logger.warning("could not find active product stream.")
+    data = requests.get(ps["manifest"])
+    cprint(data.json(), ctx=ctx)
+
+
+# BUILDS
 
 
-@entities_grp.group(help=f"{CORGI_API_URL}/api/v1/builds")
+@corgi_grp.group(help=f"{CORGI_API_URL}/api/v1/builds")
 @click.pass_context
 def builds(ctx):
     pass
 
 
 @builds.command(name="list")
 @click.argument("software_build_name", required=False)
+@query_params_options(
+    entity="SoftwareBuild",
+    endpoint_module=v1_builds_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(SoftwareBuild))},
+    },
+)
 @click.pass_context
-def list_software_builds(ctx, software_build_name):
+def list_software_builds(ctx, software_build_name, **params):
     """Retrieve a list of Software Builds."""
     session = CorgiService.create_session()
-    cond = default_conditions
     if software_build_name:
-        cond["name"] = software_build_name
-    data = session.builds.retrieve_list(**cond, limit=1000).results
+        params["name"] = software_build_name
+    data = session.builds.retrieve_list(**params).results
     return cprint(data, ctx=ctx)
 
 
 @builds.command(name="get")
-@click.argument("build_id", required=False)
+@click.argument(
+    "software_build_name",
+    required=False,
+    type=click.STRING,
+    shell_complete=get_product_stream_names,
+)
+@query_params_options(
+    entity="SoftwareBuild",
+    endpoint_module=v1_builds_retrieve,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(SoftwareBuild))},
+    },
+)
+@click.pass_context
+@progress_bar
+def get_software_build(ctx, software_build_name, **params):
+    """Retrieve SoftwareBuild."""
+    is_params_empty = [False for v in params.values() if v]
+    if not software_build_name and not is_params_empty:
+        click.echo(ctx.get_help())
+        exit(0)
+    session = CorgiService.create_session()
+    if software_build_name:
+        params["name"] = software_build_name
+    data = session.builds.retrieve_list(**params)
+    return cprint(data, ctx=ctx)
+
+
+# Products
+
+
+@corgi_grp.group(help=f"{CORGI_API_URL}/api/v1/products")
+@click.pass_context
+def products(ctx):
+    pass
+
+
+@products.command(name="list")
+@click.argument("product_name", required=False)
+@query_params_options(
+    entity="Product",
+    endpoint_module=v1_products_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Product))},
+    },
+)
+@click.pass_context
+@progress_bar
+def list_products(ctx, product_name, **params):
+    """Retrieve a list of Software Builds."""
+    session = CorgiService.create_session()
+    if product_name:
+        params["re_name"] = product_name
+    data = session.products.retrieve_list(**params).results
+    return cprint(data, ctx=ctx)
+
+
+@products.command(name="get")
+@click.argument(
+    "product_name",
+    required=False,
+    type=click.STRING,
+    shell_complete=get_product_stream_names,
+)
+@click.option("--ofuri", "ofuri", type=click.STRING, shell_complete=get_product_stream_ofuris)
+@query_params_options(
+    entity="Product",
+    endpoint_module=v1_products_retrieve,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Product))},
+    },
+)
+@click.pass_context
+@progress_bar
+def get_product(ctx, product_name, ofuri, **params):
+    """Retrieve Product."""
+    is_params_empty = [False for v in params.values() if v]
+    if not product_name and not is_params_empty:
+        click.echo(ctx.get_help())
+        exit(0)
+    session = CorgiService.create_session()
+    if ofuri:
+        params["ofuri"] = ofuri
+    if product_name:
+        params["name"] = product_name
+    data = session.products.retrieve_list(**params)
+    return cprint(data, ctx=ctx)
+
+
+# PRODUCT VERSION
+@corgi_grp.group(help=f"{CORGI_API_URL}/api/v1/product-versions")
+@click.pass_context
+def product_versions(ctx):
+    pass
+
+
+@product_versions.command(name="list")
+@click.argument("product_version_name", required=False)
+@query_params_options(
+    entity="ProductVersion",
+    endpoint_module=v1_product_versions_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(ProductVersion))},
+    },
+)
+@click.pass_context
+@progress_bar
+def list_product_versions(ctx, product_version_name, **params):
+    """Retrieve a list of Product Versions."""
+    session = CorgiService.create_session()
+    if product_version_name:
+        params["re_name"] = product_version_name
+    data = session.product_versions.retrieve_list(**params).results
+    return cprint(data, ctx=ctx)
+
+
+@product_versions.command(name="get")
+@click.argument(
+    "product_version_name",
+    required=False,
+    type=click.STRING,
+    shell_complete=get_product_stream_names,
+)
+@click.option("--ofuri", "ofuri", type=click.STRING, shell_complete=get_product_version_ofuris)
+@query_params_options(
+    entity="ProductVersion",
+    endpoint_module=v1_product_versions_retrieve,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(ProductVersion))},
+    },
+)
+@click.pass_context
+@progress_bar
+def get_product_version(ctx, product_version_name, ofuri, **params):
+    """Retrieve ProductVersion."""
+    is_params_empty = [False for v in params.values() if v]
+    if not product_version_name and not is_params_empty:
+        click.echo(ctx.get_help())
+        exit(0)
+    session = CorgiService.create_session()
+    if ofuri:
+        params["ofuri"] = ofuri
+    if product_version_name:
+        params["name"] = product_version_name
+    data = session.product_versions.retrieve_list(**params)
+    return cprint(data, ctx=ctx)
+
+
+# PRODUCT VARIANT
+@corgi_grp.group(help=f"{CORGI_API_URL}/api/v1/product-variants")
+@click.pass_context
+def product_variants(ctx):
+    pass
+
+
+@product_variants.command(name="list")
+@click.argument("product_variant_name", required=False)
+@query_params_options(
+    entity="ProductVariant",
+    endpoint_module=v1_product_variants_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(ProductVariant))},
+    },
+)
+@click.pass_context
+@progress_bar
+def list_product_variants(ctx, product_variant_name, **params):
+    """Retrieve a list of Product Variants."""
+    session = CorgiService.create_session()
+    if product_variant_name:
+        params["re_name"] = product_variant_name
+    data = session.product_variants.retrieve_list(**params).results
+    return cprint(data, ctx=ctx)
+
+
+@product_variants.command(name="get")
+@click.argument(
+    "product_variant_name",
+    required=False,
+    type=click.STRING,
+    shell_complete=get_product_stream_names,
+)
+@click.option("--ofuri", "ofuri", type=click.STRING, shell_complete=get_product_version_ofuris)
+@query_params_options(
+    entity="ProductVariant",
+    endpoint_module=v1_product_variants_retrieve,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(ProductVariant))},
+    },
+)
 @click.pass_context
-def get_software_builds(ctx, build_id):
-    """Retrieve Software Build."""
+@progress_bar
+def get_product_variant(ctx, product_variant_name, ofuri, **params):
+    """Retrieve ProductVariant."""
+    is_params_empty = [False for v in params.values() if v]
+    if not product_variant_name and not is_params_empty:
+        click.echo(ctx.get_help())
+        exit(0)
     session = CorgiService.create_session()
-    data = session.builds.retrieve(build_id)
+    if ofuri:
+        params["ofuri"] = ofuri
+    if product_variant_name:
+        params["name"] = product_variant_name
+    data = session.product_varints.retrieve_list(**params)
     return cprint(data, ctx=ctx)
+
+
+# CHANNEL
+@corgi_grp.group(help=f"{CORGI_API_URL}/api/v1/channels")
+@click.pass_context
+def channels(ctx):
+    pass
+
+
+@channels.command(name="list")
+@click.argument("channel_name", required=False)
+@query_params_options(
+    entity="Channel",
+    endpoint_module=v1_channels_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Channel))},
+    },
+)
+@click.pass_context
+@progress_bar
+def list_channels(ctx, channel_name, **params):
+    """Retrieve a list of Channels."""
+    session = CorgiService.create_session()
+    if channel_name:
+        params["re_name"] = channel_name
+    data = session.channels.retrieve_list(**params).results
+    return cprint(data, ctx=ctx)
+
+
+@channels.command(name="get")
+@click.argument(
+    "channel_name",
+    required=False,
+    type=click.STRING,
+    shell_complete=get_product_stream_names,
+)
+@click.option("--ofuri", "ofuri", type=click.STRING, shell_complete=get_product_version_ofuris)
+@query_params_options(
+    entity="Channel",
+    endpoint_module=v1_channels_retrieve,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Channel))},
+    },
+)
+@click.pass_context
+@progress_bar
+def get_channel(ctx, channel_name, ofuri, **params):
+    """Retrieve ProductVariant."""
+    is_params_empty = [False for v in params.values() if v]
+    if not channel_name and not is_params_empty:
+        click.echo(ctx.get_help())
+        exit(0)
+    session = CorgiService.create_session()
+    if ofuri:
+        params["ofuri"] = ofuri
+    if channel_name:
+        params["name"] = channel_name
+    data = session.channels.retrieve_list(**params)
+    return cprint(data, ctx=ctx)
+
+
+# ADMIN
+@corgi_grp.group(name="admin")
+@click.pass_context
+def manage_grp(ctx):
+    """Manage component registry"""
+    pass
+
+
+@manage_grp.command(name="status")
+@click.pass_context
+def corgi_status(ctx):
+    session = CorgiService.create_session()
+    data = session.status()
+    return cprint(data.additional_properties, ctx=ctx)
+
+
+@manage_grp.command(name="health")
+@click.pass_context
+def corgi_health(ctx):
+    try:
+        session = CorgiService.create_session()
+        status = session.status()["status"]
+        if status == "ok":
+            console.log(f"{CORGI_API_URL} is operational")
+        else:
+            console.log(f"{CORGI_API_URL} is NOT operational")
+            exit(1)
+    except:  # noqa
+        console.log(f"{CORGI_API_URL} is NOT operational")
+        raise click.ClickException("Component registry health check failed.")
+
+
+@manage_grp.command(name="data")
+def corgi_data():
+    click.launch(f"{CORGI_API_URL}/data")
+
+
+@manage_grp.command(name="api_doc")
+def corgi_api_docs():
+    click.launch(f"{CORGI_API_URL}/api/v1/schema/docs")
```

### Comparing `griffon-0.1.9/griffon/commands/plugin_commands.py` & `griffon-0.2.0/griffon/commands/plugin_commands.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/commands/plugins/go_vuln.py` & `griffon-0.2.0/griffon/commands/plugins/go_vuln.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/commands/plugins/osv.py` & `griffon-0.2.0/griffon/commands/plugins/osv.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import requests
 
 from griffon.output import cprint
 
 logger = logging.getLogger("griffon")
 
 api_url = "https://api.osv.dev/v1/query"
+search_api_url = "https://osv.dev/list"
 
 
 @click.group()
 @click.pass_context
 def plugins(ctx):
     """OSV plugin"""
     pass
@@ -54,7 +55,22 @@
     data = json.dumps({"commit": commit_hash})
     res = requests.post(
         api_url,
         data=data,
         headers={"Content-type": "application/json"},
     )
     cprint(res.json(), ctx=ctx)
+
+
+@plugins.command()
+@click.argument(
+    "query_string",
+    required=True,
+    type=click.STRING,
+)
+@click.pass_context
+def search(ctx, query_string):
+    """Search osv.dev by query term"""
+    if not query_string:
+        click.echo(ctx.get_help())
+        exit(0)
+    click.launch(f"{search_api_url}?ecosystem=&q={query_string}")
```

### Comparing `griffon-0.1.9/griffon/commands/process.py` & `griffon-0.2.0/griffon/commands/process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/commands/queries.py` & `griffon-0.2.0/griffon/commands/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """
 
 """
 import copy
 import logging
 
 import click
+from component_registry_bindings.bindings.python_client.api.v1 import v1_components_list
+from component_registry_bindings.bindings.python_client.models import Component
 
-from griffon import CorgiService, OSIDBService, progress_bar
+from griffon import CorgiService, OSIDBService, get_config_option, progress_bar
 from griffon.autocomplete import (
     get_component_names,
     get_cve_ids,
+    get_product_stream_names,
+    get_product_stream_ofuris,
     get_product_version_names,
 )
-from griffon.commands.entities import (
+from griffon.commands.entities.corgi import (
     get_component_manifest,
     get_component_summary,
     get_product_stream_manifest,
-    get_product_stream_names,
-    get_product_stream_ofuris,
     list_components,
 )
+from griffon.commands.entities.helpers import query_params_options
 from griffon.commands.reports import (
     generate_affects_report,
     generate_entity_report,
     generate_license_report,
 )
 from griffon.output import console, cprint, raw_json_transform
 from griffon.services import QueryService, core_queries  # , exp
@@ -75,18 +78,27 @@
 @click.option(
     "--all",
     "all",
     is_flag=True,
     default=False,
     help="Return all Products.",
 )
+@click.option(
+    "-v",
+    "verbose",
+    count=True,
+    default=get_config_option("default", "verbosity", 0),
+    help="Verbose output, more detailed search results, can be used multiple times (e.g. -vvv).",
+)  # noqa
 @click.pass_context
 @progress_bar
-def get_product_summary(ctx, product_stream_name, strict_name_search, all):
+def get_product_summary(ctx, product_stream_name, strict_name_search, all, verbose):
     """get product stream."""
+    if verbose:
+        ctx.obj["VERBOSE"] = verbose
     if not product_stream_name and not all and not strict_name_search:
         click.echo(ctx.get_help())
         exit(0)
     q = query_service.invoke(core_queries.product_stream_summary, ctx.params)
     cprint(q, ctx=ctx)
 
 
@@ -185,37 +197,51 @@
     default=False,
     help="Search related url (\033[1menabled by default\033[0m).",
 )
 @click.option(
     "--filter-rh-naming",
     is_flag=True,
     default=False,
-    help="Filter rh naming (\033[1menabled by default\033[0m).",
+    help="Filter rh naming.",
 )
 @click.option(
     "--search-all",
     "search_all",
     is_flag=True,
     default=False,
-    help="Search root Components and dependencies.",
+    help="Search all root Components and dependencies.",
+)
+@click.option(
+    "--search-redhat",
+    "search_redhat",
+    is_flag=True,
+    default=False,
+    help="Search all Red Hat root Components and dependencies.",
 )
 @click.option(
     "--search-community",
     "search_community",
     is_flag=True,
     default=False,
-    help="Search community Components (\033[1mNot Implemented\033[0m).",
+    help="Search community Components.",
 )
 @click.option(
     "--search-upstreams",
     "search_upstreams",
     is_flag=True,
     default=False,
     help="Search for Components by upstream.",
 )
+@click.option(
+    "-v",
+    "verbose",
+    count=True,
+    default=get_config_option("default", "verbosity", 0),
+    help="Verbose output, more detailed search results, can be used multiple times (e.g. -vvv).",
+)  # noqa
 @click.pass_context
 def get_product_contain_component(
     ctx,
     component_name,
     purl,
     arch,
     namespace,
@@ -224,37 +250,41 @@
     affect_mode,
     sfm2_flaw_id,
     flaw_mode,
     search_latest,
     search_related_url,
     filter_rh_naming,
     search_all,
+    search_redhat,
     search_community,
     search_upstreams,
+    verbose,
 ):
     with console.status("griffoning", spinner="line") as operation_status:
         """List products of a latest component."""
+        if verbose:
+            ctx.obj["VERBOSE"] = verbose
         if not purl and not component_name:
             click.echo(ctx.get_help())
             click.echo("")
             click.echo("\033[1mMust supply Component name or --purl.\033[0m")
             exit(0)
 
         if (
             not search_latest
             and not search_all
             and not search_related_url
             and not search_community
             and not search_upstreams
+            and not search_redhat
         ):
             ctx.params["search_latest"] = True
-            ctx.params["search_related_url"] = True
-            # ctx.params["filter_rh_naming"] = True
 
         params = copy.deepcopy(ctx.params)
+        params.pop("verbose")
         params.pop("sfm2_flaw_id")
         params.pop("flaw_mode")
         params.pop("affect_mode")
         if component_name:
             q = query_service.invoke(core_queries.products_containing_component_query, params)
         if purl:
             q = query_service.invoke(
@@ -407,27 +437,37 @@
 @click.option(
     "-s",
     "strict_name_search",
     is_flag=True,
     default=False,
     help="Strict search, exact match of component name.",
 )
+@click.option(
+    "-v",
+    "verbose",
+    count=True,
+    default=get_config_option("default", "verbosity", 0),
+    help="Verbose output, more detailed search results, can be used multiple times (e.g. -vvv).",
+)  # noqa
 @click.pass_context
 @progress_bar
 def get_component_contain_component(
     ctx,
     component_name,
     purl,
     component_type,
     component_version,
     component_arch,
     namespace,
     strict_name_search,
+    verbose,
 ):
     """List components that contain component."""
+    if verbose:
+        ctx.obj["VERBOSE"] = verbose
     if not component_name and not purl:
         click.echo(ctx.get_help())
         exit(0)
     if component_name:
         q = query_service.invoke(core_queries.components_containing_component_query, ctx.params)
         cprint(q, ctx=ctx)
     if purl:
@@ -469,31 +509,50 @@
     ctx.invoke(get_product_stream_manifest, **cond)
 
 
 @queries_grp.command(
     name="product-components",
     help="List LATEST Root Components of Product.",
 )
-@click.pass_context
 @click.argument("product_stream_name", required=False, shell_complete=get_product_stream_names)
 @click.option("--ofuri", "ofuri", type=click.STRING, shell_complete=get_product_stream_ofuris)
-def get_product_latest_components_query(ctx, product_stream_name, ofuri):
+@query_params_options(
+    entity="Component",
+    endpoint_module=v1_components_list,
+    options_overrides={
+        "include_fields": {"type": click.Choice(CorgiService.get_fields(Component))},
+    },
+)
+@click.option(
+    "-v",
+    "verbose",
+    count=True,
+    default=get_config_option("default", "verbosity", 0),
+    help="Verbose output, more detailed search results, can be used multiple times (e.g. -vvv).",
+)  # noqa
+@click.pass_context
+def get_product_latest_components_query(ctx, product_stream_name, ofuri, verbose, **params):
     """List components of a specific product version."""
+    if verbose:
+        ctx.obj["VERBOSE"] = verbose
+        ctx.params.pop("verbose")
     if not ofuri and not product_stream_name:
         click.echo(ctx.get_help())
         exit(0)
-    cond = {}
     if ofuri:
-        cond["ofuri"] = ofuri
+        params["ofuri"] = ofuri
     if product_stream_name:
         # lookup ofuri
-        q = query_service.invoke(core_queries.product_stream_summary, ctx.params)
-        ofuri = q[0]["ofuri"]
-        cond["ofuri"] = ofuri
-    ctx.invoke(list_components, **cond)
+        session = CorgiService.create_session()
+        ps = session.product_streams.retrieve_list(
+            name=product_stream_name, include_fields="name,ofuri"
+        )
+        params["ofuri"] = ps["ofuri"]
+        params["include_fields"] = "name,nvr,related_url,purl,version,release,type,software_build"
+    ctx.invoke(list_components, **params)
 
 
 @queries_grp.command(
     name="component-manifest",
     help="Get Component manifest.",
 )
 @click.option("--uuid", "component_uuid")
@@ -704,14 +763,15 @@
     "-s",
     "strict_name_search",
     is_flag=True,
     default=False,
     help="Strict search, exact match of component name.",
 )
 @click.pass_context
+@progress_bar
 def cves_for_specific_product_query(
     ctx,
     product_version_name,
     ofuri,
     flaw_state,
     flaw_impact,
     flaw_resolution,
```

### Comparing `griffon-0.1.9/griffon/commands/reports.py` & `griffon-0.2.0/griffon/commands/reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/output.py` & `griffon-0.2.0/griffon/output.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import logging
 
 import click
 from packageurl import PackageURL
 from rich.console import Console
 from rich.text import Text
+from rich.tree import Tree
 
 console = Console(color_system="auto")
 
 logger = logging.getLogger("griffon")
 
 
 class OUTPUT_FORMAT(enum.Enum):
@@ -82,14 +83,38 @@
 def output_version(ctx, version):
     if version:
         if version.startswith("sha256") and ctx.obj["SHORT_VERSION_VALUES"]:
             return f"sha256...{version[-8:]}"
     return version
 
 
+def walk_component_tree(obj, key, tree, show_purl=False):
+    if isinstance(obj, dict):
+        for k, v in obj.items():
+            if isinstance(v, (dict, list)):
+                walk_component_tree(v, k, tree, show_purl=show_purl)
+    elif isinstance(obj, list):
+        for item in obj:
+            label = f"{item['node_type']}: {item['nvr']},{item['type']}"
+            if show_purl:
+                label = f"{item['node_type']}: {item['purl']}"
+            child = tree.add(label)
+            walk_component_tree(item, None, child, show_purl=show_purl)
+    return tree
+
+
+def text_output_tree(ctx, output):
+    tree = Tree(
+        "component dependency tree",
+        guide_style="bold magenta",
+    )
+    console.print(walk_component_tree(output, None, tree, show_purl=ctx.params["show_purl"]))
+    ctx.exit()
+
+
 def text_output_product_summary(ctx, output, format, exclude_products):
     ordered_results = sorted(output["results"], key=lambda d: d["name"])
 
     if exclude_products:
         exclude_products_results = []
         for result in ordered_results:
             if result["product_version"] not in exclude_products:
@@ -125,15 +150,17 @@
                 item["ofuri"],
                 item["manifest_link"],
                 no_wrap=False,
             )
     ctx.exit()
 
 
-def text_output_products_contain_component(ctx, output, format, exclude_products):
+def text_output_products_contain_component(
+    ctx, output, format, exclude_products, exclude_components
+):
     component_name = ctx.params["component_name"]
 
     # handle single component
     if ctx.params["purl"]:
         ordered_results = sorted(output["results"], key=lambda d: d["ofuri"])
         for item in ordered_results:
             console.print(
@@ -166,264 +193,357 @@
                 flaw_operation = "update"
             product_versions = sorted(
                 list(set([item["product_version"] for item in ordered_results]))
             )
             for pv in product_versions:
                 names = [item["name"] for item in ordered_results if pv == item["product_version"]]
                 names = list(set(names))
+                if component_name in names and f"{component_name}-container" in names:
+                    names.remove(f"{component_name}-container")
                 for name in names:
-                    dep_name = name
-                    console.print(
-                        f"{pv}/{name}={flaw_operation}",
-                        no_wrap=False,
-                    )
+                    if not any([match in name for match in exclude_components]):
+                        dep_name = name
+                        console.print(
+                            f"{pv}/{name}={flaw_operation}",
+                            no_wrap=False,
+                        )
         else:
             if ctx.obj["VERBOSE"] == 0:  # product_version X source component
                 product_versions = sorted(
                     list(set([item["product_version"] for item in ordered_results]))
                 )
                 for pv in product_versions:
                     names = [
                         item["name"] for item in ordered_results if pv == item["product_version"]
                     ]
                     names = list(set(names))
+                    if component_name in names and f"{component_name}-container" in names:
+                        names.remove(f"{component_name}-container")
                     for name in names:
-                        dep_name = name.replace(component_name, f"[b]{component_name}[/b]")
-                        dep = f"[white]({dep_name})[/white]"
-                        console.print(
-                            Text(pv, style="magenta b u"),
-                            dep,
-                            no_wrap=False,
-                        )
+                        if not any([match in name for match in exclude_components]):
+                            dep_name = name.replace(component_name, f"[b]{component_name}[/b]")
+                            dep = f"[white]({dep_name})[/white]"
+                            console.print(
+                                Text(pv, style="magenta b u"),
+                                dep,
+                                no_wrap=False,
+                            )
 
             if ctx.obj["VERBOSE"] == 1:  # product_stream X source component
                 product_streams = sorted(
                     list(set([item["product_stream"] for item in ordered_results]))
                 )
                 for ps in product_streams:
                     ps_components = [
                         item for item in ordered_results if item["product_stream"] == ps
                     ]
                     names = sorted(list(set([item["name"] for item in ps_components])))
+                    if component_name in names and f"{component_name}-container" in names:
+                        names.remove(f"{component_name}-container")
 
                     for name in names:
-                        sources = []
-                        for item in ps_components:
-                            if item["name"] == name and "sources" in item:
-                                sources.extend(item["sources"])
-
-                        root_component = "root component"
-                        if sources:
-                            source_purl = PackageURL.from_string(sources[0]["purl"])
-                            root_component = source_purl.name
-                        dep_name = name.replace(component_name, f"[b]{component_name}[/b]")
-                        dep = f"[white]({dep_name})[/white]"
-                        console.print(
-                            Text(ps, style="magenta b u"),
-                            root_component,
-                            dep,
-                            no_wrap=False,
-                        )
+                        if not any([match in name for match in exclude_components]):
+                            sources = []
+                            nvr = ""
+                            for item in ps_components:
+                                if item["name"] == name and "sources" in item:
+                                    sources.extend(item["sources"])
+                                if item["nvr"]:
+                                    nvr = item["nvr"]
+
+                            root_component = "root component"
+                            if sources:
+                                source_purl = PackageURL.from_string(sources[0]["purl"])
+                                root_component = sources[0]["name"]
+
+                            dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
+                            dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
+                            console.print(
+                                Text(ps, style="magenta b u"),
+                                root_component,
+                                dep,
+                                no_wrap=False,
+                            )
 
             if ctx.obj["VERBOSE"] == 2:  # product_stream X nvr
                 product_streams = sorted(
                     list(set([item["product_stream"] for item in ordered_results]))
                 )
                 for ps in product_streams:
                     ps_components = [
                         item for item in ordered_results if item["product_stream"] == ps
                     ]
                     names = sorted(list(set([item["name"] for item in ps_components])))
+                    if component_name in names and f"{component_name}-container" in names:
+                        names.remove(f"{component_name}-container")
 
                     for name in names:
-                        sources = []
-                        for item in ps_components:
-                            if item["name"] == name and "sources" in item:
-                                sources.extend(item["sources"])
-
-                        root_component = "root component"
-                        if sources:
-                            source_purl = PackageURL.from_string(sources[0]["purl"])
-                            root_component = (
-                                f"{source_purl.name}-{output_version(ctx,source_purl.version)}"
-                            )
+                        if not any([match in name for match in exclude_components]):
+                            sources = []
+                            nvr = ""
+                            for item in ps_components:
+                                if item["name"] == name and "sources" in item:
+                                    sources.extend(item["sources"])
+                                if item["nvr"]:
+                                    nvr = item["nvr"]
 
-                        dep_name = name.replace(component_name, f"[b]{component_name}[/b]")
-                        dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
-                        console.print(
-                            Text(ps, style="magenta b u"),
-                            root_component,
-                            dep,
-                            no_wrap=False,
-                        )
+                            root_component = "root component"
+                            if sources:
+                                source_purl = PackageURL.from_string(sources[0]["purl"])
+                                root_component = f"{sources[0]['purl']}-{output_version(ctx,source_purl.version)}"  # noqa
+
+                            dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
+                            dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
+                            console.print(
+                                Text(ps, style="magenta b u"),
+                                root_component,
+                                dep,
+                                no_wrap=False,
+                            )
 
             if ctx.obj["VERBOSE"] == 3:  # source url, upstream
                 product_streams = sorted(
                     list(set([item["product_stream"] for item in ordered_results]))
                 )
                 for ps in product_streams:
                     ps_components = [
                         item for item in ordered_results if item["product_stream"] == ps
                     ]
                     names = sorted(list(set([item["name"] for item in ps_components])))
+                    if component_name in names and f"{component_name}-container" in names:
+                        names.remove(f"{component_name}-container")
                     for name in names:
-                        sources = []
-                        related_url = ""
-                        build_source_url = ""
-                        nvr = ""
-                        for item in ps_components:
-                            if item["name"] == name:
-                                if item["nvr"]:
-                                    nvr = item["nvr"]
-                                if "sources" in item:
-                                    sources.extend(item["sources"])
-                                if item["related_url"]:
-                                    related_url = item["related_url"]
-                                if item["build_source_url"]:
-                                    build_source_url = item["build_source_url"]
-                        root_component = "root component"
-                        if sources:
-                            source_purl = PackageURL.from_string(sources[0]["purl"])
-                            root_component = (
-                                f"{source_purl.name}-{output_version(ctx,source_purl.version)}"
-                            )
-                        dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
-                        dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
-                        related_url = related_url.replace(
-                            component_name, f"[b]{component_name}[/b]"
-                        )
-                        console.print(
-                            Text(ps, style="magenta b u"),
-                            root_component,
-                            dep,
-                            related_url,
-                            no_wrap=False,
-                        )
+                        if not any([match in name for match in exclude_components]):
+                            sources = []
+                            related_url = ""
+                            build_source_url = ""
+                            nvr = ""
+                            for item in ps_components:
+                                if item["name"] == name:
+                                    if item["nvr"]:
+                                        nvr = item["nvr"]
+                                    if "sources" in item:
+                                        sources.extend(item["sources"])
+                                    if item["related_url"]:
+                                        related_url = item["related_url"]
+                                    if item["build_source_url"]:
+                                        build_source_url = item["build_source_url"]
+                            root_component = "root component"
+                            if sources:
+                                source_purl = PackageURL.from_string(sources[0]["purl"])
+                                root_component = f"{sources[0]['purl']}-{output_version(ctx,source_purl.version)}"  # noqa
+                            dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
+                            dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
+                            related_url = related_url.replace(
+                                component_name, f"[b]{component_name}[/b]"
+                            )
+                            console.print(
+                                Text(ps, style="magenta b u"),
+                                root_component,
+                                dep,
+                                related_url,
+                                no_wrap=False,
+                            )
             if ctx.obj["VERBOSE"] > 3:  # source url, upstream
                 product_streams = sorted(
                     list(set([item["product_stream"] for item in ordered_results]))
                 )
                 for ps in product_streams:
                     ps_components = [
                         item for item in ordered_results if item["product_stream"] == ps
                     ]
                     names = sorted(list(set([item["name"] for item in ps_components])))
+                    if component_name in names and f"{component_name}-container" in names:
+                        names.remove(f"{component_name}-container")
                     for name in names:
-                        sources = []
-                        related_url = ""
-                        build_source_url = ""
-                        nvr = ""
-                        for item in ps_components:
-                            if item["name"] == name:
-                                if item["nvr"]:
-                                    nvr = item["nvr"]
-                                if "sources" in item:
-                                    sources.extend(item["sources"])
-                                if item["related_url"]:
-                                    related_url = item["related_url"]
-                                if item["build_source_url"]:
-                                    build_source_url = item["build_source_url"]
-                        root_component = "root component"
-                        if sources:
-                            source_purl = PackageURL.from_string(sources[0]["purl"])
-                            root_component = (
-                                f"{source_purl.name}-{output_version(ctx,source_purl.version)}"
-                            )
-                        upstream = ""
-                        if item["upstream_purl"]:
-                            upstream = f"[cyan]{item['upstream_purl']}[/cyan]"
-                        dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
-                        dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
-                        related_url = related_url.replace(
-                            component_name, f"[b]{component_name}[/b]"
-                        )
-                        console.print(
-                            Text(ps, style="magenta b u"),
-                            root_component,
-                            dep,
-                            related_url,
-                            build_source_url,
-                            upstream,
-                            no_wrap=False,
-                        )
+                        if not any([match in name for match in exclude_components]):
+                            sources = []
+                            related_url = ""
+                            build_source_url = ""
+                            nvr = ""
+                            for item in ps_components:
+                                if item["name"] == name:
+                                    if item["nvr"]:
+                                        nvr = item["nvr"]
+                                    if "sources" in item:
+                                        sources.extend(item["sources"])
+                                    if item["related_url"]:
+                                        related_url = item["related_url"]
+                                    if item["build_source_url"]:
+                                        build_source_url = item["build_source_url"]
+                            root_component = "root component"
+                            if sources:
+                                source_purl = PackageURL.from_string(sources[0]["purl"])
+                                root_component = f"{sources[0]['purl']}-{output_version(ctx,source_purl.version)}"  # noqa
+                            upstream = ""
+                            if item["upstream_purl"]:
+                                upstream = f"[cyan]{item['upstream_purl']}[/cyan]"
+                            dep_name = nvr.replace(component_name, f"[b]{component_name}[/b]")
+                            dep = f"[white]({dep_name}, {item['type'].lower()})[/white]"
+                            related_url = related_url.replace(
+                                component_name, f"[b]{component_name}[/b]"
+                            )
+                            console.print(
+                                Text(ps, style="magenta b u"),
+                                root_component,
+                                dep,
+                                related_url,
+                                build_source_url,
+                                upstream,
+                                no_wrap=False,
+                            )
 
         ctx.exit()
 
 
-def text_output_components_contain_component(ctx, output, format):
+def text_output_components_contain_component(ctx, output, format, exclude_components):
     if "results" in output:
         for item in output["results"]:
             component_name = item["name"]
+            component_nvr = item["nvr"]
+            related_url = item["related_url"]
+            download_url = item["download_url"]
+            arch = item["arch"]
+            if not any([match in component_name for match in exclude_components]):
+                if ctx.obj["VERBOSE"] == 0:
+                    ordered_sources = sorted(item["sources"], key=lambda d: d["purl"])
+                    for source in ordered_sources:
+                        if "arch=noarch" in source["purl"] or "arch=src" in source["purl"]:
+                            source_purl = PackageURL.from_string(source["purl"])
+                            root_component = source_purl.name
+                            if source_purl.type == "oci" and "-source" not in source_purl.name:
+                                root_component = (
+                                    f"[u magenta]{source_purl.name}-container[/u magenta]"
+                                )
+                            if source_purl.type == "oci":
+                                component_ns = Text("REDHAT", style="bold magenta")
+                            elif not source_purl.namespace:
+                                component_ns = Text("UPSTREAM", style="bold magenta")
+                            else:
+                                component_ns = Text(source_purl.namespace.upper(), style="bold red")
 
-            if ctx.obj["VERBOSE"] == 0:
-                ordered_sources = sorted(item["sources"], key=lambda d: d["purl"])
-                for source in ordered_sources:
-                    if "arch=noarch" in source["purl"] or "arch=src" in source["purl"]:
-                        source_purl = PackageURL.from_string(source["purl"])
-                        root_component = source_purl.name
-                        if source_purl.type == "oci" and "-source" not in source_purl.name:
-                            root_component = f"[u magenta]{source_purl.name}-container[/u magenta]"
-                        console.print(
-                            root_component,
-                            component_name,
-                            no_wrap=False,
-                        )
+                            console.print(
+                                component_ns,
+                                source_purl.type.upper(),
+                                root_component,
+                                Text(component_name, style="bold white"),
+                                no_wrap=False,
+                            )
+                if ctx.obj["VERBOSE"] == 1:
+                    ordered_sources = sorted(item["sources"], key=lambda d: d["purl"])
+                    for source in ordered_sources:
+                        if "arch=noarch" in source["purl"] or "arch=src" in source["purl"]:
+                            source_purl = PackageURL.from_string(source["purl"])
+                            root_component = f"{source_purl.name}-{source_purl.version}"
+                            if source_purl.type == "oci" and "-source" not in source_purl.name:
+                                root_component = (
+                                    f"[u magenta]{source_purl.name}-container[/u magenta]"
+                                )
+                            if source_purl.type == "oci":
+                                component_ns = Text("REDHAT", style="bold magenta")
+                            elif not source_purl.namespace:
+                                component_ns = Text("UPSTREAM", style="bold magenta")
+                            else:
+                                component_ns = Text(source_purl.namespace.upper(), style="bold red")
+                            console.print(
+                                component_ns,
+                                source_purl.type.upper(),
+                                root_component,
+                                Text(component_nvr, style="bold white"),
+                                arch,
+                                no_wrap=False,
+                            )
+                if ctx.obj["VERBOSE"] > 1:
+                    ordered_sources = sorted(item["sources"], key=lambda d: d["purl"])
+                    for source in ordered_sources:
+                        if "arch=noarch" in source["purl"] or "arch=src" in source["purl"]:
+                            source_purl = PackageURL.from_string(source["purl"])
+                            root_component = f"{source_purl.name}-{source_purl.version}"
+                            if source_purl.type == "oci" and "-source" not in source_purl.name:
+                                root_component = (
+                                    f"[u magenta]{source_purl.name}-container[/u magenta]"
+                                )
+                            if source_purl.type == "oci":
+                                component_ns = Text("REDHAT", style="bold magenta")
+                            elif not source_purl.namespace:
+                                component_ns = Text("UPSTREAM", style="bold magenta")
+                            else:
+                                component_ns = Text(source_purl.namespace.upper(), style="bold red")
+                            console.print(
+                                component_ns,
+                                source_purl.type.upper(),
+                                root_component,
+                                Text(component_nvr, style="bold white"),
+                                arch,
+                                related_url,
+                                download_url,
+                                no_wrap=False,
+                            )
     ctx.exit()
 
 
 def text_output_components_affected_by_cve(ctx, output, format):
     console.print("Flaw Title:", output["title"])
     console.print(
         "affects:",
     )
-    ordered_affects = sorted(output["affects"], key=lambda d: d["product_version_name"])
-    for affect in ordered_affects:
-        if "components" in affect:
-            for component in affect["components"]:
-                affected_component1 = f"({component['purl']})"
-                if not ctx.obj["SHOW_PURL"]:
-                    purl = PackageURL.from_string(component["purl"])
-                    ns = "UPSTREAM"
-                    if purl.namespace:
-                        ns = purl.namespace.upper()
-                    affected_component1 = f"([bold cyan]{ns}[/bold cyan] {purl.name}-{purl.version},{purl.type.upper()})"  # noqa
-                    if ctx.obj["VERBOSE"] == 0:
-                        console.print(
-                            ns,
-                            affected_component1,
-                            no_wrap=True,
-                        )
-                    if ctx.obj["VERBOSE"] == 1:
-                        console.print(
-                            ns,
-                            affected_component1,
-                            no_wrap=True,
-                        )
+    for component in output["components"]:
+        affected_component1 = f"({component['purl']})"
+        if not ctx.obj["SHOW_PURL"]:
+            purl = PackageURL.from_string(component["purl"])
+            ns = "UPSTREAM"
+            if purl.namespace:
+                ns = purl.namespace.upper()
+            affected_component = f"([bold cyan]{ns}[/bold cyan] {purl.name}-{purl.version},{purl.type.upper()})"  # noqa
+            versions = [pv["name"] for pv in component["product_versions"]]
+            if ctx.obj["VERBOSE"] == 0:
+                console.print(
+                    Text(str(versions), style="bold magenta u"),
+                    ns,
+                    affected_component,
+                    no_wrap=False,
+                )
+            if ctx.obj["VERBOSE"] == 1:
+                console.print(
+                    Text(component["product_streams"], style="bold magenta u"),
+                    ns,
+                    affected_component1,
+                    no_wrap=False,
+                )
+            if ctx.obj["VERBOSE"] > 1:
+                console.print(
+                    Text(component["product_streams"], style="bold magenta u"),
+                    ns,
+                    affected_component1,
+                    Text(component["build_source_url"], style="i"),
+                    Text(component["related_url"], style="i"),
+                    Text(component["download_url"], style="i"),
+                    no_wrap=False,
+                )
     ctx.exit()
 
 
 def text_output_products_affected_by_cve(ctx, output, format, exclude_products):
     console.print("[white]link:[/white]", output["link"])
     console.print("[white]cve_id:[/white]", output["cve_id"])
     console.print("[white]title:[/white]", output["title"])
-    console.print(
-        "[white]product_versions:[/white]",
-    )
     if ctx.obj["VERBOSE"] == 0:
-        ordered_product_versions = sorted(output["product_versions"], key=lambda d: d["name"])
+        console.print(
+            "[white]product_versions:[/white]",
+        )
+        ordered_product_versions = sorted(output["product_versions"])
         for product_version in ordered_product_versions:
-            console.print(Text(product_version["name"], style="bold magenta u"), no_wrap=True)
+            console.print(Text(product_version, style="bold magenta u"), no_wrap=True)
     if ctx.obj["VERBOSE"] > 0:
-        ordered_affects = sorted(output["affects"], key=lambda d: d["product_version_name"])
-        for affect in ordered_affects:
-            console.print(
-                Text(affect["product_version_name"], style="bold magenta u"),
-                affect["component_name"],
-                no_wrap=True,
-            )
+        console.print(
+            "[white]product_streams:[/white]",
+        )
+        ordered_product_streams = sorted(output["product_streams"])
+        for product_stream in ordered_product_streams:
+            console.print(Text(product_stream, style="bold magenta u"), no_wrap=True)
     ctx.exit()
 
 
 def text_output_get_manifest(ctx, output, format):
     if not ctx.obj["SHOW_PURL"]:
         for component in output["packages"]:
             if "pkg:" in component["externalRefs"][0]["referenceLocator"]:
@@ -456,133 +576,139 @@
             flaw_cve_id = "Vulnerability"
             if affect["flaw_cve_id"]:
                 flaw_cve_id = affect["flaw_cve_id"]
             if ctx.obj["VERBOSE"] == 0:
                 console.print(
                     Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
+                    Text(affect["affect_product_version"], style="cyan"),
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
                     no_wrap=True,
                 )
             if ctx.obj["VERBOSE"] == 1:
                 console.print(
                     Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
-                    f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
                     Text(affect["affect_product_version"], style="cyan"),
+                    f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
                     no_wrap=True,
                 )
             if ctx.obj["VERBOSE"] > 1:
                 console.print(Text(affect["title"], style="white"))
                 console.print(
                     Text(component_name, style="magenta"),
-                    f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
                     Text(affect["affect_product_version"], style="cyan"),
+                    f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
                     no_wrap=True,
                 )
     ctx.exit()
 
 
 def text_output_product_flaws(ctx, output, format):
     for item in output["results"]:
         component_name = item["name"]
         for affect in item["affects"]:
+            flaw_cve_id = "Vulnerability"
+            if affect["flaw_cve_id"]:
+                flaw_cve_id = affect["flaw_cve_id"]
             if ctx.obj["VERBOSE"] == 0:
                 console.print(
-                    Text(affect["flaw_cve_id"], style="magenta"),
+                    Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
-                    affect["affect_name"],
+                    affect["affect_component_name"],
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
                     no_wrap=True,
                 )
             if ctx.obj["VERBOSE"] == 1:
                 console.print(
-                    Text(affect["flaw_cve_id"], style="magenta"),
+                    Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
                     f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
-                    affect["affect_name"],
+                    affect["affect_component_name"],
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
                     no_wrap=True,
                 )
             if ctx.obj["VERBOSE"] > 1:
                 console.print(affect["title"])
                 console.print(
+                    Text(flaw_cve_id, style="magenta"),
                     Text(component_name, style="white"),
                     f"(state: {affect['flaw_state']} resolution:{affect['flaw_resolution']})",
-                    affect["affect_name"],
+                    affect["affect_component_name"],
                     affect["affect_affectedness"],
                     affect["affect_impact"],
                     affect["affect_resolution"],
                     no_wrap=True,
                 )
     ctx.exit()
 
 
-def text_output_list(ctx, output, format):
+def text_output_list(ctx, output, format, exclude_components):
     if "results" in output and output["count"] > 0:
         # handle component
         if "purl" in output["results"][0]:
             ordered_components = sorted(output["results"], key=lambda d: d["name"])
             for row in ordered_components:
-                if "purl" in row:
-                    purl = PackageURL.from_string(row["purl"])
-                    if purl.type == "oci":
-                        component_ns = Text("REDHAT", style="bold magenta")
-                    elif not purl.namespace:
-                        component_ns = Text("UPSTREAM", style="bold magenta")
-                    else:
-                        component_ns = Text(purl.namespace.upper(), style="bold red")
-
-                    sha256 = ""
-                    if purl.version:
-                        if purl.version.startswith("sha256"):
-                            sha256 = output_version(ctx, purl.version)
-                    nvr = None
-                    if "nvr" in row:
-                        nvr = row["nvr"]
-
-                    if not ctx.obj["SHOW_PURL"]:
-                        if ctx.obj["VERBOSE"] == 0:
-                            console.print(
-                                component_ns,
-                                purl.type.upper(),
-                                Text(nvr, style="bold white"),
-                                sha256,
-                                row["related_url"],
-                                purl.qualifiers.get("arch"),
-                            )
-                        if ctx.obj["VERBOSE"] == 1:
-                            download_url = ""
-                            if "download_url" in row:
-                                download_url = row["download_url"]
+                if not any([match in row["purl"] for match in exclude_components]):
+                    if "purl" in row:
+                        purl = PackageURL.from_string(row["purl"])
+                        if purl.type == "oci":
+                            component_ns = Text("REDHAT", style="bold magenta")
+                        elif not purl.namespace:
+                            component_ns = Text("UPSTREAM", style="bold magenta")
+                        else:
+                            component_ns = Text(purl.namespace.upper(), style="bold red")
+
+                        sha256 = ""
+                        if purl.version:
+                            if purl.version.startswith("sha256"):
+                                sha256 = output_version(ctx, purl.version)
+                        nvr = None
+                        if "nvr" in row:
+                            nvr = row["nvr"]
+
+                        if not ctx.obj["SHOW_PURL"]:
+                            if ctx.obj["VERBOSE"] == 0:
+                                console.print(
+                                    component_ns,
+                                    purl.type.upper(),
+                                    Text(nvr, style="bold white"),
+                                    sha256,
+                                    row["related_url"],
+                                    purl.qualifiers.get("arch"),
+                                )
+                            if ctx.obj["VERBOSE"] > 0:
+                                download_url = ""
+                                if "download_url" in row:
+                                    download_url = row["download_url"]
+                                console.print(
+                                    component_ns,
+                                    purl.type.upper(),
+                                    Text(nvr, style="bold white"),
+                                    sha256,
+                                    row["related_url"],
+                                    purl.qualifiers.get("arch"),
+                                    download_url,
+                                )
+                        else:
                             console.print(
-                                component_ns,
-                                purl.type.upper(),
-                                Text(nvr, style="bold white"),
-                                sha256,
-                                row["related_url"],
-                                purl.qualifiers.get("arch"),
-                                download_url,
+                                row["purl"],
                             )
-                    else:
-                        console.print(
-                            row["purl"],
-                        )
         # handle flaw
         if "cve_id" in output["results"][0]:
             for row in output["results"]:
                 console.print(
                     row["title"],
                     row["state"],
                     row["impact"],
@@ -604,15 +730,23 @@
         if "ofuri" in output["results"][0]:
             for row in output["results"]:
                 console.print(
                     Text(row["name"], style="magenta bold u"),
                     row["ofuri"],
                     no_wrap=True,
                 )
-
+        # handle channels
+        if "relative_url" in output["results"][0]:
+            for row in output["results"]:
+                console.print(
+                    Text(row["name"], style="magenta bold u"),
+                    row["type"],
+                    row["description"],
+                    no_wrap=True,
+                )
         # handle builds
         if "build_id" in output["results"][0]:
             for row in output["results"]:
                 console.print(
                     Text(str(row["build_id"]), style="magenta bold u"),
                     row["build_type"],
                     Text(row["name"], style="white"),
@@ -671,48 +805,57 @@
     filename=None,
     ctx=None,
     show_count: bool = True,
 ):
     """handle format and output"""
     from griffon import get_config_option
 
-    exclude_products = None
-    if ctx.obj["PROFILE"] != "default":
+    exclude_products = []
+    if get_config_option(ctx.obj["PROFILE"], "exclude"):
         exclude_products = get_config_option(ctx.obj["PROFILE"], "exclude").split("\n")
+    logger.debug(f"exclude products = {exclude_products}")
+
+    exclude_components = []
+    if get_config_option(ctx.obj["PROFILE"], "exclude_components"):
+        exclude_components = get_config_option(ctx.obj["PROFILE"], "exclude_components").split("\n")
+    logger.debug(f"exclude_components = {exclude_components}")
 
     output = raw_json_transform(data, show_count)
     if ctx and ctx.obj["NO_COLOR"]:
         console.no_color = True
     format = OUTPUT_FORMAT.JSON
     if ctx and "FORMAT" in ctx.obj:
         format = OUTPUT_FORMAT(ctx.obj["FORMAT"])
-
     if format is OUTPUT_FORMAT.TEXT:
         if ctx.info_name == "product-summary":
             text_output_product_summary(ctx, output, format, exclude_products)
         if ctx.info_name == "products-contain-component":
-            text_output_products_contain_component(ctx, output, format, exclude_products)
+            text_output_products_contain_component(
+                ctx, output, format, exclude_products, exclude_components
+            )
         if ctx.info_name == "components-contain-component":
-            text_output_components_contain_component(ctx, output, format)
-        if ctx.info_name == "components-affected-by-cve":
+            text_output_components_contain_component(ctx, output, format, exclude_components)
+        if ctx.info_name == "components-affected-by-flaw":
             text_output_components_affected_by_cve(ctx, output, format)
-        if ctx.info_name == "products-affected-by-cve":
+        if ctx.info_name == "products-affected-by-flaw":
             text_output_products_affected_by_cve(ctx, output, format, exclude_products)
         if ctx.info_name == "get-manifest":
             text_output_get_manifest(ctx, output, format)
         if ctx.info_name == "list":
-            text_output_list(ctx, output, format)
+            text_output_list(ctx, output, format, exclude_components)
         if ctx.info_name == "component-flaws":
             text_output_component_flaws(ctx, output, format)
         if ctx.info_name == "product-flaws":
             text_output_product_flaws(ctx, output, format)
         if ctx.info_name == "provides":
             text_output_purls(ctx, output, format)
         if ctx.info_name == "sources":
             text_output_purls(ctx, output, format)
+        if ctx.info_name == "tree":
+            text_output_tree(ctx, output)
 
         # last chance text formatted output
         text_output_generic(ctx, output, format)
 
     if format is OUTPUT_FORMAT.JSON:
         if dest is DEST.CONSOLE:
             console.print_json(json.dumps(output))
```

### Comparing `griffon-0.1.9/griffon/services/__init__.py` & `griffon-0.2.0/griffon/services/__init__.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/services/core_process.py` & `griffon-0.2.0/griffon/services/core_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/griffon/services/core_queries.py` & `griffon-0.2.0/griffon/services/core_queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,32 @@
 import logging
 import re
 from typing import Any, Dict, List
 
 import requests
 from component_registry_bindings.bindings.python_client.models import Component
 
-from griffon import CORGI_API_URL, OSIDB_API_URL, CorgiService, OSIDBService
+from griffon import (
+    COMMUNITY_COMPONENTS_API_URL,
+    CORGI_API_URL,
+    OSIDB_API_URL,
+    CommunityComponentService,
+    CorgiService,
+    OSIDBService,
+)
 
 logger = logging.getLogger("griffon")
 
 
 class product_stream_summary:
     """retrieve product_stream summary"""
 
     name = "product_stream_summary"
     description = "retrieve product_stream summary"
-    allowed_params = ["strict_name_search", "all", "product_stream_name", "ofuri"]
+    allowed_params = ["strict_name_search", "all", "product_stream_name", "ofuri", "verbose"]
 
     def __init__(self, params: dict) -> None:
         self.corgi_session = CorgiService.create_session()
         self.params = params
         self.product_stream_name = self.params.get("product_stream_name")
         self.ofuri = self.params.get("ofuri")
         self.strict_name_search = self.params.get("strict_name_search", None)
@@ -44,23 +51,24 @@
 
         # TODO - corgi bindings need to support ofuri in product_streams
         product_streams = self.corgi_session.product_streams.retrieve_list(
             **cond,
             limit=400,
             include_fields="link,ofuri,name,products,product_versions,brew_tags,manifest",
         )
+
         results = []
         if product_streams.results:
             for ps in product_streams.results:
                 result = {
                     "link": ps.link,
                     "ofuri": ps.ofuri,
                     "name": ps.name,
                     "product": ps.products[0]["name"],
-                    "product_version": ps.product_versions[0]["name"],
+                    "product_version": str([pv["name"] for pv in ps.product_versions]),
                     "brew_tags": [brew_tag for brew_tag in ps.brew_tags.to_dict().keys()],
                     # "build_count": ps.build_count,
                     "manifest_link": ps.manifest,
                     "latest_components_link": f"{CORGI_API_URL}/api/v1/components?ofuri={ps.ofuri}&view=summary",  # noqa
                     "all_components_link": f"{CORGI_API_URL}/api/v1/components?product_streams={ps.ofuri}&include_fields=link,name,purl",  # noqa
                 }
                 results.append(result)
@@ -85,42 +93,75 @@
 
     name = "product-versions-affected-by-specific-cve"
     description = "Given a specific CVE ID, what product versions are affected?"
     allowed_params = ["cve_id"]
 
     def __init__(self, params: dict) -> None:
         self.osidb_session = OSIDBService.create_session()
+        self.corgi_session = CorgiService.create_session()
         self.params = params
+        self.cve_id = self.params.get("cve_id")
+        self.affectedness = self.params.get("affectedness")
+        self.affect_resolution = self.params.get("affect_resolution")
+        self.affect_impact = self.params.get("affect_impact")
+        self.component_type = self.params.get("component_type")
+        self.namespace = self.params.get("namespace")
 
     def execute(self) -> dict:
-        cve_id = self.params["cve_id"]
-        flaw = self.osidb_session.flaws.retrieve(cve_id)
-        affects = list()
-        pv_names = list()
-        for affect in flaw.affects:
-            pv_names.append(affect.ps_module)
-            affects.append(
-                {"component_name": affect.ps_component, "product_version_name": affect.ps_module}
-            )
-        pv_names = list(set(pv_names))
-        product_versions = list()
-        for pv_name in pv_names:
-            product_versions.append(
-                {
-                    "link": f"{CORGI_API_URL}/api/v1/product_versions?name={pv_name}",
-                    "name": pv_name,
-                }
-            )
+        cond = {}
+        if self.affectedness:
+            cond["affectedness"] = self.affectedness
+        if self.affect_resolution:
+            cond["resolution"] = self.affect_resolution
+        if self.affect_impact:
+            cond["impact"] = self.affect_impact
+
+        component_cond = {}
+        if self.namespace:
+            component_cond["namespace"] = self.namespace
+        if self.component_type:
+            component_cond["type"] = self.component_type
+
+        flaw = self.osidb_session.flaws.retrieve(self.cve_id)
+        affects = flaw.affects
+        results = list()
+        product_versions = set()
+        product_streams = set()
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            futures = []
+            for affect in affects:
+                futures.append(
+                    executor.submit(
+                        self.corgi_session.components.retrieve_list,
+                        name=affect.ps_component,
+                        latest_components_by_streams=True,
+                        include_fields="product_streams.name,product_versions.name",
+                    )
+                )
+            for future in concurrent.futures.as_completed(futures):
+                try:
+                    for c in future.result().results:
+                        results.append(c.to_dict())
+                except Exception as exc:
+                    logger.error("%r generated an exception: %s" % (future, exc))
+                    exit(0)
+
+            for c in results:
+                for ps in c["product_streams"]:
+                    product_streams.add(ps["name"])
+                for pv in c["product_versions"]:
+                    product_versions.add(ps["name"])
         return {
-            "link": f"{OSIDB_API_URL}/osidb/api/v1/flaws/{cve_id}",
-            "cve_id": cve_id,
+            "link": f"{OSIDB_API_URL}/osidb/api/v1/flaws/{flaw.cve_id}",
+            "cve_id": flaw.cve_id,
             "title": flaw.title,
             "description": flaw.description,
-            "product_versions": product_versions,
-            "affects": affects,
+            "product_versions": sorted(list(product_versions)),
+            "product_streams": sorted(list(product_streams)),
+            # "components": results,
         }
 
 
 class products_containing_specific_component_query:
     """What products contain a specific component?"""
 
     name = "products_containing_specific_component_query"
@@ -135,28 +176,91 @@
         "affect_mode",
         "search_latest",
         "search_all",
         "search_related_url",
         "search_community",
         "search_upstreams",
         "filter_rh_naming",
+        "search_redhat",
     ]
 
     def __init__(self, params: dict) -> None:
         self.corgi_session = CorgiService.create_session()
         self.params = params
         self.purl = self.params.get("purl")
 
     def execute(self) -> dict:
         c = self.corgi_session.components.retrieve_list(
             purl=self.purl,
         )
         return c["product_streams"]
 
 
+def output_component(pv, ps, c):
+    is_root = False
+    if (c.arch == "src" and c.type == "RPM") or (c.arch == "noarch" and c.type == "OCI"):
+        is_root = True
+    sources = [{"purl": source["purl"]} for source in c.sources]
+    component = {
+        "is_root": is_root,
+        "product_version": pv["name"],
+        "product_version_ofuri": pv["ofuri"],
+        "product_stream": ps["name"],
+        "product_stream_ofuri": ps["ofuri"],
+        "product_active": True,
+        "purl": c.purl,
+        "type": str(c.type),
+        "namespace": str(c.namespace),
+        "name": c.name,
+        "arch": c.arch,
+        "release": c.release,
+        "version": c.version,
+        "sources": sources,
+        "nvr": c.nvr,
+        "build_id": None,
+        "build_type": None,
+        "build_source_url": None,
+        "related_url": None,
+        "upstream_purl": None,
+    }
+    if c.software_build:
+        component["build_id"] = str(c.software_build.build_id)
+        component["build_type"] = str(c.software_build.build_type)
+        component["build_name"] = str(c.software_build.name)
+        component["build_source_url"] = str(c.software_build.source)
+    if c.upstreams:
+        component["upstream_purl"] = str(c.upstreams[0]["purl"])
+    return component
+
+
+def async_retrieve_components(corgi_session, params, components_initial, component_cnt):
+    components = list()
+    if component_cnt < 120:
+        components.extend(components_initial.results)
+    elif component_cnt > 120:
+        components.extend(components_initial.results)
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            futures = []
+            for batch in range(120, component_cnt, 120):
+                futures.append(
+                    executor.submit(
+                        corgi_session.components.retrieve_list,
+                        **params,
+                        offset=batch,
+                        limit=120,  # noqa
+                    )
+                )
+            for future in concurrent.futures.as_completed(futures):
+                try:
+                    components.extend(future.result().results)
+                except Exception as exc:
+                    logger.warning("%r generated an exception: %s" % (future, exc))
+    return components
+
+
 class products_containing_component_query:
     """What products contain a component?"""
 
     name = "products_containing_component_query"
     description = "What products contain a component?"
     allowed_params = [
         "component_name",
@@ -164,14 +268,15 @@
         "arch",
         "namespace",
         "component_type",
         "strict_name_search",
         "search_latest",
         "search_all",
         "search_related_url",
+        "search_redhat",
         "search_community",
         "search_upstreams",
         "filter_rh_naming",
     ]
 
     def __init__(self, params: dict) -> None:
         self.corgi_session = CorgiService.create_session()
@@ -180,292 +285,139 @@
         self.component_type = self.params.get("component_type")
         self.strict_name_search = self.params.get("strict_name_search")
         self.search_deps = self.params.get("search_deps")
         self.ns = self.params.get("namespace")
         self.search_latest = self.params.get("search_latest")
         self.search_all = self.params.get("search_all")
         self.search_related_url = self.params.get("search_related_url")
+        self.search_redhat = self.params.get("search_redhat")
         self.search_community = self.params.get("search_community")
         self.search_upstreams = self.params.get("search_upstreams")
         self.filter_rh_naming = self.params.get("filter_rh_naming")
 
     def execute(self) -> List[Dict[str, Any]]:
-        url: str = f"{CORGI_API_URL}/api/v1/components"
-
         results = []
+
         if self.search_latest:
-            cond = {"view": "latest"}
+            params = {
+                "latest_components_by_streams": True,
+                "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
+            }
             if not self.strict_name_search:
-                cond["re_name"] = self.component_name  # type: ignore
+                params["re_name"] = self.component_name
             else:
-                cond["name"] = self.component_name  # type: ignore
-            cond["namespace"] = "REDHAT"
-            result = self.corgi_session.components.retrieve_list(**cond, limit=1000)
-            results = result.results
-            # TODO: this should be done server side at some point
-            if self.component_type:
-                results = [result for result in results if result.type == self.component_type]
+                params["name"] = self.component_name
+            if self.ns:
+                params["namespace"] = self.ns
 
-        #  TODO: uncomment once component-registry-bindings support related_url
-        # if self.search_related_url:
-        #     # TODO - not in bindings yet
-        #     params = {
-        #         "include_fields": "name,arch,namespace,release,version,nvr,type,link,purl,software_build,product_versions,product_streams,sources,upstreams",  # noqa
-        #         "related_url": self.component_name,
-        #     }
-        #     params["namespace"] = "REDHAT"
-        #     if self.component_type:
-        #         params["type"] = self.component_type
-        #
-        #     component_cnt = self.corgi_session.components.retrieve_list(**params).count
-        #     if component_cnt < 3000000:
-        #         with concurrent.futures.ThreadPoolExecutor() as executor:
-        #             futures = []
-        #             components = list()
-        #             for batch in range(0, component_cnt, 120):
-        #                 futures.append(
-        #                     executor.submit(
-        #                         self.corgi_session.components.retrieve_list,
-        #                         **params,
-        #                         offset=batch,
-        #                         limit=120,  # noqa
-        #                     )
-        #                 )
-        #             for future in concurrent.futures.as_completed(futures):
-        #                 try:
-        #                     components.extend(future.result().results)
-        #                 except Exception as exc:
-        #                     logger.warning("%r generated an exception: %s" % (future, exc))
-        #
-        #             for c in components:
-        #                 for pv in c.product_versions:
-        #                     for ps in c.product_streams:
-        #                         is_dep = False
-        #                         if c.arch == "src" or c.arch == "noarch":
-        #                             is_dep = True
-        #                         component = {
-        #                             "is_dep": is_dep,
-        #                             "product_version": pv["name"],
-        #                             "product_version_ofuri": pv["ofuri"],
-        #                             "product_stream": ps["name"],
-        #                             "product_stream_ofuri": ps["ofuri"],
-        #                             "product_active": True,
-        #                             "purl": c.purl,
-        #                             "type": c.type,
-        #                             "namespace": c.namespace,
-        #                             "name": c.name,
-        #                             "arch": c.arch,
-        #                             "release": c.release,
-        #                             "version": c.version,
-        #                             "sources": c.sources,
-        #                             "nvr": c.nvr,
-        #                             "build_id": None,
-        #                             "build_type": None,
-        #                             "build_source_url": None,
-        #                             "related_url": None,
-        #                             "upstream_purl": None,
-        #                         }
-        #                         if c.software_build:
-        #                             component["build_id"] = c.software_build.build_id
-        #                             component["build_type"] = c.software_build.build_type
-        #                             component["build_name"] = c.software_build.name
-        #                             component["build_source_url"] = c.software_build.source
-        #                         if c.upstreams:
-        #                             component["upstream_purl"] = c.upstreams[0]["purl"]
-        #                         results.append(component)
+            component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
+            latest_components: list = async_retrieve_components(
+                self.corgi_session, params, component_initial, component_initial.count
+            )
+            for c in latest_components:
+                if self.strict_name_search:
+                    if c.name != self.component_name:
+                        continue
+                for pv in c.product_versions:
+                    for ps in c.product_streams:
+                        component = output_component(pv, ps, c)
+                        results.append(component)
 
-        # TODO: remove following search_related_url
         if self.search_related_url:
-            # TODO - not in bindings yet
+            # Note: related_url filter has no concept of strict
             params = {
-                "include_fields": "name,arch,namespace,release,version,nvr,type,link,purl,software_build,product_versions,product_streams,sources,upstreams",  # noqa
+                "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
                 "related_url": self.component_name,
-                "limit": 10000,
             }
             params["namespace"] = "REDHAT"
             if self.component_type:
                 params["type"] = self.component_type
-            related_url_search = requests.get(
-                url,
-                params=params,
-            )
 
-            for c in related_url_search.json()["results"]:
-                for pv in c["product_versions"]:
-                    for ps in c["product_streams"]:
-                        is_dep = False
-                        if c["arch"] == "src" or c["arch"] == "noarch":
-                            is_dep = True
-                        component = {
-                            "is_dep": is_dep,
-                            "product_version": pv["name"],
-                            "product_version_ofuri": pv["ofuri"],
-                            "product_stream": ps["name"],
-                            "product_stream_ofuri": ps["ofuri"],
-                            "product_active": True,
-                            "purl": c["purl"],
-                            "type": c["type"],
-                            "namespace": c["namespace"],
-                            "name": c["name"],
-                            "arch": c["arch"],
-                            "release": c["release"],
-                            "version": c["version"],
-                            "sources": c["sources"],
-                            "nvr": c["nvr"],
-                            "build_id": None,
-                            "build_type": None,
-                            "build_source_url": None,
-                            "related_url": None,
-                            "upstream_purl": None,
-                        }
-                        if c["software_build"]:
-                            component["build_id"] = c["software_build"]["build_id"]
-                            component["build_type"] = c["software_build"]["build_type"]
-                            component["build_name"] = c["software_build"]["name"]
-                            component["build_source_url"] = c["software_build"]["source"]
-                        if c["upstreams"]:
-                            component["upstream_purl"] = c["upstreams"][0]["purl"]
-                        results.append(component)
+            component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
+            related_url_components: list = async_retrieve_components(
+                self.corgi_session, params, component_initial, component_initial.count
+            )
+            for c in related_url_components:
+                if self.strict_name_search:
+                    if c.name != self.component_name:
+                        continue
+                for pv in c.product_versions:
+                    for ps in c.product_streams:
+                        results.append(output_component(pv, ps, c))
 
         if self.search_all:
-            # TODO - not in bindings yet
             params = {
-                "include_fields": "name,arch,namespace,release,version,nvr,type,link,purl,software_build,product_versions,product_streams,sources,upstreams",  # noqa
+                "type": "RPM",
+                "arch": "src",
+                "include_fields": "link,purl,type,name,related_url,namespace,software_build,nvr,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
             }
             if not self.strict_name_search:
                 params["re_name"] = self.component_name
             else:
                 params["name"] = self.component_name
 
             if self.component_type:
                 params["type"] = self.component_type
 
-            component_cnt = self.corgi_session.components.retrieve_list(**params).count
-            if component_cnt < 3000000:
-                with concurrent.futures.ThreadPoolExecutor() as executor:
-                    futures = []
-                    components = list()
-                    for batch in range(0, component_cnt, 100):
-                        futures.append(
-                            executor.submit(
-                                self.corgi_session.components.retrieve_list,
-                                **params,
-                                offset=batch,
-                                limit=100,  # noqa
-                            )
-                        )
-                    for future in concurrent.futures.as_completed(futures):
-                        try:
-                            components.extend(future.result().results)
-                        except Exception as exc:
-                            logger.warning("%r generated an exception: %s" % (future, exc))
-
-                    for c in components:
-                        for pv in c.product_versions:
-                            for ps in c.product_streams:
-                                is_dep = False
-                                if c.arch == "src" or c.arch == "noarch":
-                                    is_dep = True
-                                component = {
-                                    "is_dep": is_dep,
-                                    "product_version": pv["name"],
-                                    "product_version_ofuri": pv["ofuri"],
-                                    "product_stream": ps["name"],
-                                    "product_stream_ofuri": ps["ofuri"],
-                                    "product_active": True,
-                                    "purl": c.purl,
-                                    "type": c.type,
-                                    "namespace": c.namespace,
-                                    "name": c.name,
-                                    "arch": c.arch,
-                                    "release": c.release,
-                                    "version": c.version,
-                                    "sources": c.sources,
-                                    "nvr": c.nvr,
-                                    "build_id": None,
-                                    "build_type": None,
-                                    "build_source_url": None,
-                                    "related_url": None,
-                                    "upstream_purl": None,
-                                }
-                                if c.software_build:
-                                    component["build_id"] = c.software_build.build_id
-                                    component["build_type"] = c.software_build.build_type
-                                    component["build_name"] = c.software_build.name
-                                    component["build_source_url"] = c.software_build.source
-                                if c.upstreams:
-                                    component["upstream_purl"] = c.upstreams[0]["purl"]
-                                results.append(component)
+            all_src_component_initial = self.corgi_session.components.retrieve_list(
+                limit=120, **params
+            )
+            all_src_components: list = async_retrieve_components(
+                self.corgi_session,
+                params,
+                all_src_component_initial,
+                all_src_component_initial.count,
+            )
+            params["type"] = "OCI"
+            params["arch"] = "noarch"
+            all_noarch_component_initial = self.corgi_session.components.retrieve_list(
+                limit=120, **params
+            )
+            all_noarch_components: list = async_retrieve_components(
+                self.corgi_session,
+                params,
+                all_noarch_component_initial,
+                all_noarch_component_initial.count,
+            )
+            all_components = all_src_components + all_noarch_components
+
+            for c in all_components:
+                if self.strict_name_search:
+                    if c.name != self.component_name:
+                        continue
+                for pv in c.product_versions:
+                    for ps in c.product_streams:
+                        results.append(output_component(pv, ps, c))
 
         if self.search_upstreams:
-            # TODO - not in bindings yet
+            # Note: upstreams only takes a purl ... so we must use re_upstreams for
+            # both strict and not strict search
             params = params = {
-                "include_fields": "name,arch,namespace,release,version,nvr,type,link,purl,software_build,product_versions,product_streams,sources,upstreams",  # noqa
-                "re_upstreams": self.component_name,
-                # "limit": 10000,
+                "include_fields": "link,purl,type,name,namespace,software_build,nvr,related_url,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
+                "namespace": "UPSTREAM",
             }
+
+            if not self.strict_name_search:
+                params["re_name"] = self.component_name
+            else:
+                params["name"] = self.component_name
             if self.component_type:
                 params["type"] = self.component_type
 
-            component_cnt = self.corgi_session.components.retrieve_list(**params).count
-            if component_cnt < 3000000:
-                with concurrent.futures.ThreadPoolExecutor() as executor:
-                    futures = []
-                    components = list()
-                    for batch in range(0, component_cnt, 120):
-                        futures.append(
-                            executor.submit(
-                                self.corgi_session.components.retrieve_list,
-                                **params,
-                                offset=batch,
-                                limit=120,  # noqa
-                            )
-                        )
-                    for future in concurrent.futures.as_completed(futures):
-                        try:
-                            components.extend(future.result().results)
-                        except Exception as exc:
-                            logger.warning("%r generated an exception: %s" % (future, exc))
-
-                    for c in components:
-                        for pv in c.product_versions:
-                            for ps in c.product_streams:
-                                is_dep = False
-                                if c.arch == "src" or c.arch == "noarch":
-                                    is_dep = True
-                                component = {
-                                    "is_dep": is_dep,
-                                    "product_version": pv["name"],
-                                    "product_version_ofuri": pv["ofuri"],
-                                    "product_stream": ps["name"],
-                                    "product_stream_ofuri": ps["ofuri"],
-                                    "product_active": True,
-                                    "purl": c.purl,
-                                    "type": c.type,
-                                    "namespace": c.namespace,
-                                    "name": c.name,
-                                    "arch": c.arch,
-                                    "release": c.release,
-                                    "version": c.version,
-                                    "sources": c.sources,
-                                    "nvr": c.nvr,
-                                    "build_id": None,
-                                    "build_type": None,
-                                    "build_source_url": None,
-                                    "related_url": None,
-                                    "upstream_purl": None,
-                                }
-                                if c.software_build:
-                                    component["build_id"] = c.software_build.build_id
-                                    component["build_type"] = c.software_build.build_type
-                                    component["build_name"] = c.software_build.name
-                                    component["build_source_url"] = c.software_build.source
-                                if c.upstreams:
-                                    component["upstream_purl"] = c.upstreams[0]["purl"]
-                                results.append(component)
+            component_initial = self.corgi_session.components.retrieve_list(limit=120, **params)
+            upstream_components: list = async_retrieve_components(
+                self.corgi_session, params, component_initial, component_initial.count
+            )
+            for c in upstream_components:
+                if self.strict_name_search:
+                    if c.name != self.component_name:
+                        continue
+                for pv in c.product_versions:
+                    for ps in c.product_streams:
+                        results.append(output_component(pv, ps, c))
 
         if self.filter_rh_naming:
             flags = re.IGNORECASE
             patterns = [
                 # binutils
                 re.compile(
                     f"(devtoolset\\-[0-9]+\\-|mingw\\-|gcc\\-toolset\\-[0-9]+\\-)?{self.component_name}[0-9\\.]*$",  # noqa
@@ -498,14 +450,54 @@
                         if m:
                             filtered_results.append(result)
                             is_matched = True
                             break
 
             results = filtered_results
 
+        if self.search_community or self.search_all:
+            self.community_session = CommunityComponentService.create_session()
+
+            params = {
+                "include_fields": "link,purl,type,name,namespace,software_build,nvr,upstreams.purl,upstreams.name,release,version,arch,sources.name,sources.purl,sources.name,product_versions.name,product_versions.ofuri,product_streams.name,product_streams.ofuri",  # noqa
+                "type": "RPM",
+                "arch": "src",
+            }
+            if not self.strict_name_search:
+                params["re_name"] = self.component_name
+            else:
+                params["name"] = self.component_name
+
+            if self.component_type:
+                params["type"] = self.component_type
+
+            component_initial = self.community_session.components.retrieve_list(limit=120, **params)
+            commmunity_src_components: list = async_retrieve_components(
+                self.community_session, params, component_initial, component_initial.count
+            )
+            params["type"] = "OCI"
+            params["arch"] = "noarch"
+            component_initial_noarch = self.community_session.components.retrieve_list(
+                limit=120, **params
+            )
+            commmunity_noarch_components: list = async_retrieve_components(
+                self.community_session,
+                params,
+                component_initial_noarch,
+                component_initial_noarch.count,
+            )
+            community_components = commmunity_src_components + commmunity_noarch_components
+            for c in community_components:
+                if self.strict_name_search:
+                    if c.name != self.component_name:
+                        continue
+                for pv in c.product_versions:
+                    for ps in c.product_streams:
+                        results.append(output_component(pv, ps, c))
+
         return results
 
 
 class components_containing_specific_component_query:
     """What components contain a specific component?"""
 
     name = "components_containing_specific_component_query"
@@ -515,14 +507,15 @@
         "component_name",
         "purl",
         "component_type",
         "component_version",
         "component_arch",
         "namespace",
         "strict_name_search",
+        "verbose",
     ]
 
     def __init__(self, params: dict):
         self.corgi_session = CorgiService.create_session()
         self.params = params
         self.purl = self.params.get("purl")
 
@@ -554,14 +547,15 @@
         "component_name",
         "purl",
         "component_type",
         "component_version",
         "component_arch",
         "namespace",
         "strict_name_search",
+        "verbose",
     ]
 
     def __init__(self, params: dict) -> None:
         self.corgi_session = CorgiService.create_session()
         self.params = params
         self.component_name = self.params.get("component_name")
         self.component_type = self.params.get("component_type")
@@ -592,16 +586,16 @@
                 components = list()
                 for batch in range(0, component_cnt, 120):
                     futures.append(
                         executor.submit(
                             self.corgi_session.components.retrieve_list,
                             **cond,
                             offset=batch,
-                            include_fields="link,name,type,version,purl,sources",
-                            limit=120,  # noqa
+                            include_fields="link,name,type,arch,version,purl,nvr,sources,related_url,download_url",  # noqa
+                            limit=120,
                         )
                     )
                 for future in concurrent.futures.as_completed(futures):
                     try:
                         components.extend(future.result().results)
                     except Exception as exc:
                         logger.warning("%r generated an exception: %s" % (future, exc))
@@ -615,14 +609,18 @@
                 ]
             results.append(
                 {
                     "link": c.link,
                     "type": c.type,
                     "name": c.name,
                     "version": c.version,
+                    "nvr": c.nvr,
+                    "arch": c.arch,
+                    "download_url": c.download_url,
+                    "related_url": c.related_url,
                     "purl": c.purl,
                     "sources": sources,
                 }
             )
         return results
 
 
@@ -663,67 +661,41 @@
         component_cond = {}
         if self.namespace:
             component_cond["namespace"] = self.namespace
         if self.component_type:
             component_cond["type"] = self.component_type
 
         flaw = self.osidb_session.flaws.retrieve(self.cve_id)
-        affects = self.osidb_session.affects.retrieve_list(
-            flaw=flaw.uuid, **cond, limit=1000
-        ).results
+        affects = flaw.affects
         results = list()
-        for affect in affects:
-            try:
-                product_version = self.corgi_session.product_versions.retrieve_list(
-                    name=affect.ps_module
-                ).results[0]
-                components = []
-                with concurrent.futures.ThreadPoolExecutor() as executor:
-                    futures = []
-                    for ps in product_version.product_streams:
-                        futures.append(
-                            executor.submit(
-                                self.corgi_session.components.retrieve_list,
-                                **component_cond,
-                                ofuri=ps["ofuri"],
-                                name=affect.ps_component,
-                                include_fields="link,purl,name,type",
-                                limit=50000,
-                            )
-                        )
-                    for future in concurrent.futures.as_completed(futures):
-                        try:
-                            for c in future.result().results:
-                                components.append(c.to_dict())
-                        except Exception as exc:
-                            logger.error("%r generated an exception: %s" % (future, exc))
-                            exit(0)
-
-                results.append(
-                    {
-                        "link": f"{OSIDB_API_URL}/osidb/api/v1/affects/{affect.uuid}",
-                        "product_version_name": affect.ps_module,
-                        "component_name": affect.ps_component,
-                        "affectedness": affect.affectedness,
-                        "affect_impact": affect.impact,
-                        "affect_resolution": affect.resolution,
-                        "components": components,
-                    }
-                )
-            except IndexError:
-                logger.warning(
-                    f"{affect.ps_module} product stream not found in component-registry (may not exist or a community product)."  # noqa
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            futures = []
+            for affect in affects:
+                futures.append(
+                    executor.submit(
+                        self.corgi_session.components.retrieve_list,
+                        name=affect.ps_component,
+                        latest_components_by_streams=True,
+                        include_fields="purl,product_streams,product_versions,software_build",
+                    )
                 )
+            for future in concurrent.futures.as_completed(futures):
+                try:
+                    for c in future.result().results:
+                        results.append(c.to_dict())
+                except Exception as exc:
+                    logger.error("%r generated an exception: %s" % (future, exc))
+                    exit(0)
 
         return {
             "link": f"{OSIDB_API_URL}/osidb/api/v1/flaws/{flaw.cve_id}",
             "cve_id": flaw.cve_id,
             "title": flaw.title,
             "description": flaw.description,
-            "affects": results,
+            "components": results,
         }
 
 
 class cves_for_specific_component_query:
     """CVEs affecting a specific component?"""
 
     # include count
@@ -754,52 +726,88 @@
         self.affect_resolution = self.params.get("affect_resolution")
         self.affect_impact = self.params.get("affect_impact")
 
     def execute(self) -> List[Dict[str, Any]]:
         components = []
         if self.component_name:
             affects: list = []
-            # component = self.corgi_session.components.retrieve_list(name=self.component_name)
-            cond = {}
-            cond["ps_component"] = self.component_name
+            params = {
+                "include_fields": "cve_id,title,state,resolution,impact,affects",
+            }
+            params["affects__ps_component"] = self.component_name
+            if self.flaw_state:
+                params["state"] = self.flaw_state
+            if self.flaw_resolution:
+                params["resolution"] = self.flaw_resolution
+            if self.flaw_impact:
+                params["impact"] = self.flaw_impact
             if self.affectedness:
-                cond["affectedness"] = self.affectedness
+                params["affects__affectedness"] = self.affectedness
             if self.affect_resolution:
-                cond["resolution"] = self.affect_resolution
+                params["affects__resolution"] = self.affect_resolution
             if self.affect_impact:
-                cond["impact"] = self.affect_impact
+                params["affects__impact"] = self.affect_impact
 
-            for affect in self.osidb_session.affects.retrieve_list(
-                **cond,
-                limit=1000,
-            ).results:
-                flaw = self.osidb_session.flaws.retrieve(affect.flaw)
-                if flaw:
-                    affects.append(
-                        {
-                            "link_affect": f"{OSIDB_API_URL}/osidb/api/v1/affects/{affect.uuid}",  # noqa
-                            "link_cve": f"{OSIDB_API_URL}/osidb/api/v1/flaws/{flaw.cve_id}",
-                            "flaw_cve_id": flaw.cve_id,
-                            "title": flaw.title,
-                            "flaw_state": flaw.state,
-                            "flaw_resolution": flaw.resolution,
-                            "affect_name": affect.ps_component,
-                            "affect_product_version": affect.ps_module,
-                            "affect_affectedness": affect.affectedness,
-                            "affect_impact": affect.impact,
-                            "affect_resolution": affect.resolution,
-                        }
+            res = requests.get(f"{OSIDB_API_URL}/osidb/api/v1/flaws", params=params)
+            flaws = res.json()
+            flaws_cnt = int(flaws["count"])
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                futures = []
+                flaws = list()
+                for batch in range(0, flaws_cnt, 75):
+                    params["offset"] = batch  # type: ignore
+                    params["limit"] = 75  # type: ignore
+                    futures.append(
+                        executor.submit(
+                            requests.get,
+                            f"{OSIDB_API_URL}/osidb/api/v1/flaws",
+                            params=params,
+                        )
                     )
-            components.append(
-                {
-                    "link": f"{CORGI_API_URL}/api/v1/components?purl=",
-                    "name": self.component_name,
-                    "affects": affects,
-                }
-            )
+                for future in concurrent.futures.as_completed(futures):
+                    try:
+                        flaws.extend(future.result().json()["results"])
+                    except Exception as exc:
+                        logger.warning("%r generated an exception: %s" % (future, exc))
+
+                for flaw in flaws:
+                    for affect in flaw["affects"]:
+                        if self.affectedness:
+                            if self.affectedness != affect["affectedness"]:
+                                continue
+                        if self.affect_resolution:
+                            if self.affect_resolution != affect["resolution"]:
+                                continue
+                        if self.affect_impact:
+                            if self.affect_impact != affect["impact"]:
+                                continue
+                        affects.append(
+                            {
+                                "link_affect": f"{OSIDB_API_URL}/osidb/api/v1/affects/{affect['uuid']}",  # noqa
+                                "link_cve": f"{OSIDB_API_URL}/osidb/api/v1/flaws/{flaw['cve_id']}",  # noqa
+                                "link_component": f"{CORGI_API_URL}/api/v1/components?name={affect['ps_component']}&latest_components_by_streams=True",  # noqa
+                                "link_community_component": f"{COMMUNITY_COMPONENTS_API_URL}/api/v1/components?name={affect['ps_component']}&latest_components_by_streams=True",  # noqa
+                                "flaw_cve_id": flaw["cve_id"],
+                                "title": flaw["title"],
+                                "flaw_state": flaw["state"],
+                                "flaw_resolution": flaw["resolution"],
+                                "affect_component_name": affect["ps_component"],
+                                "affect_product_version": affect["ps_module"],
+                                "affect_affectedness": affect["affectedness"],
+                                "affect_impact": affect["impact"],
+                                "affect_resolution": affect["resolution"],
+                            }
+                        )
+                components.append(
+                    {
+                        "link": f"{CORGI_API_URL}/api/v1/components?name={self.component_name}",
+                        "name": self.component_name,
+                        "affects": affects,
+                    }
+                )
 
         if self.purl:
             pass
 
         return components
 
 
@@ -831,50 +839,83 @@
         self.affect_resolution = self.params.get("affect_resolution")
         self.affect_impact = self.params.get("affect_impact")
 
     def execute(self) -> List[Dict[str, Any]]:
         components = []
         if self.product_version_name:
             affects: list = []
-            # component = self.corgi_session.components.retrieve_list(name=self.component_name)
-            cond = {}
-            cond["ps_module"] = self.product_version_name
+            params = {
+                "include_fields": "cve_id,title,state,resolution,impact,affects",
+            }
+            params["affects__ps_module"] = self.product_version_name
+            if self.flaw_state:
+                params["state"] = self.flaw_state
+            if self.flaw_resolution:
+                params["resolution"] = self.flaw_resolution
+            if self.flaw_impact:
+                params["impact"] = self.flaw_impact
             if self.affectedness:
-                cond["affectedness"] = self.affectedness
+                params["affects__affectedness"] = self.affectedness
             if self.affect_resolution:
-                cond["resolution"] = self.affect_resolution
+                params["affects__resolution"] = self.affect_resolution
             if self.affect_impact:
-                cond["impact"] = self.affect_impact
+                params["affects__impact"] = self.affect_impact
 
-            for affect in self.osidb_session.affects.retrieve_list(
-                **cond,
-                limit=1000,
-            ).results:
-                flaw = self.osidb_session.flaws.retrieve(affect.flaw)
-                if flaw:
-                    affects.append(
-                        {
-                            "link_affect": f"{OSIDB_API_URL}/osidb/api/v1/affects/{affect.uuid}",  # noqa
-                            "link_cve": f"{OSIDB_API_URL}/osidb/api/v1/flaws/{flaw.cve_id}",
-                            "flaw_cve_id": flaw.cve_id,
-                            "title": flaw.title,
-                            "flaw_state": flaw.state,
-                            "flaw_resolution": flaw.resolution,
-                            "affect_name": affect.ps_component,
-                            "affect_product_version": affect.ps_module,
-                            "affect_affectedness": affect.affectedness,
-                            "affect_impact": affect.impact,
-                            "affect_resolution": affect.resolution,
-                        }
+            res = requests.get(f"{OSIDB_API_URL}/osidb/api/v1/flaws", params=params)
+            flaws = res.json()
+            flaws_cnt = int(flaws["count"])
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                futures = []
+                flaws = list()
+                for batch in range(0, flaws_cnt, 75):
+                    params["offset"] = batch  # type: ignore
+                    params["limit"] = 75  # type: ignore
+                    futures.append(
+                        executor.submit(
+                            requests.get,
+                            f"{OSIDB_API_URL}/osidb/api/v1/flaws",
+                            params=params,
+                        )
                     )
-            components.append(
-                {
-                    "link": f"{CORGI_API_URL}/api/v1/product_version?ofuri=",
-                    "name": self.product_version_name,
-                    "affects": affects,
-                }
-            )
+                for future in concurrent.futures.as_completed(futures):
+                    try:
+                        flaws.extend(future.result().json()["results"])
+                    except Exception as exc:
+                        logger.warning("%r generated an exception: %s" % (future, exc))
 
-        if self.ofuri:
-            pass
+                for flaw in flaws:
+                    for affect in flaw["affects"]:
+                        if self.affectedness:
+                            if self.affectedness != affect["affectedness"]:
+                                continue
+                        if self.affect_resolution:
+                            if self.affect_resolution != affect["resolution"]:
+                                continue
+                        if self.affect_impact:
+                            if self.affect_impact != affect["impact"]:
+                                continue
+                        affects.append(
+                            {
+                                "link_affect": f"{OSIDB_API_URL}/osidb/api/v1/affects/{affect['uuid']}",  # noqa
+                                "link_cve": f"{OSIDB_API_URL}/osidb/api/v1/flaws/{flaw['cve_id']}",  # noqa
+                                "link_component": f"{CORGI_API_URL}/api/v1/components?name={affect['ps_component']}&latest_components_by_streams=True",  # noqa
+                                "link_community_component": f"{COMMUNITY_COMPONENTS_API_URL}/api/v1/components?name={affect['ps_component']}&latest_components_by_streams=True",  # noqa
+                                "flaw_cve_id": flaw["cve_id"],
+                                "title": flaw["title"],
+                                "flaw_state": flaw["state"],
+                                "flaw_resolution": flaw["resolution"],
+                                "affect_component_name": affect["ps_component"],
+                                "affect_product_version": affect["ps_module"],
+                                "affect_affectedness": affect["affectedness"],
+                                "affect_impact": affect["impact"],
+                                "affect_resolution": affect["resolution"],
+                            }
+                        )
+                components.append(
+                    {
+                        "link": f"{CORGI_API_URL}/api/v1/product_versions?name={self.product_version_name}",  # noqa
+                        "name": self.product_version_name,
+                        "affects": affects,
+                    }
+                )
 
         return components
```

### Comparing `griffon-0.1.9/griffon/services/core_reports.py` & `griffon-0.2.0/griffon/services/core_reports.py`

 * *Files 3% similar despite different names*

```diff
@@ -360,40 +360,43 @@
         self.params = params
         self.product_stream_name = params.get("product_stream_name")
         self.purl = params.get("purl")
         self.exclude_children = params.get("exclude_children")
 
     def generate(self) -> dict:
         output = {}
-        filter = {
-            "include_fields": "uuid,purl,type,license_declared,related_url,software_build.build_id,provides,download_url",  # noqa
+        component_filter = {
+            "include_fields": "uuid,purl,type,"
+            "license_concluded,license_declared,"
+            "related_url,download_url,"
+            "software_build.build_id,provides",
         }
         if self.purl:
-            filter["purl"] = self.purl
+            component_filter["purl"] = self.purl
         if self.product_stream_name:
             product_stream = self.corgi_session.product_streams.retrieve_list(
                 name=self.product_stream_name
             )
             stream_ofuri = product_stream["ofuri"]
-            filter["ofuri"] = stream_ofuri
-        initial_component = self.corgi_session.components.retrieve_list(**filter)
+            component_filter["ofuri"] = stream_ofuri
+        initial_component = self.corgi_session.components.retrieve_list(**component_filter)
         component_cnt = initial_component.count
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = []
             components = list()
             if self.purl:
                 components.append(
                     self.corgi_session.components.retrieve(initial_component.to_dict()["uuid"])
                 )
             else:
                 for batch in range(0, component_cnt, 120):
                     futures.append(
                         executor.submit(
                             self.corgi_session.components.retrieve_list,
-                            **filter,
+                            **component_filter,
                             offset=batch,
                             limit=120,
                         )
                     )
                 for future in concurrent.futures.as_completed(futures):
                     try:
                         components.extend(future.result().results)
@@ -404,21 +407,32 @@
                 purl = component.purl
                 logger.debug(purl)
                 output[purl] = {
                     "license_declared": component.license_declared,
                     "related_url": component.related_url,
                     "build_id": component.software_build.build_id,
                 }
-                if str(component.type) in ["GEM", "GOLANG", "NPM", "PYPI"]:
-                    output[purl]["upstream_url"] = component.download_url
+                if component.license_concluded:
+                    # Some components can't be scanned, e.g. binary RPMs
+                    output[purl]["license_concluded"] = component.license_concluded
+                if str(component.type) not in ("RPM", "RPMMOD") and (
+                    # Report container's exact repository_url if present
+                    # Container Catalog search page is used as a fallback
+                    # Just ignore it if no specific URL is available
+                    component.download_url
+                    != "https://catalog.redhat.com/software/containers/search"
+                ):
+                    output[purl]["download_url"] = component.download_url
 
                 children = []
                 provides_filter = {
                     "sources": purl,
-                    "include_fields": "purl,type,license_declared,related_url,download_url",
+                    "include_fields": "purl,type,"
+                    "license_concluded,license_declared,"
+                    "related_url,download_url",
                 }
                 provides_cnt = self.corgi_session.components.retrieve_list(**provides_filter).count
                 logger.debug(provides_cnt)
 
                 if not self.exclude_children:
                     futures_children = []
                     for batch in range(0, provides_cnt, 120):
@@ -434,15 +448,24 @@
                         try:
                             for c in future.result().results:
                                 child = {
                                     "purl": c.purl,
                                     "license_declared": c.license_declared,
                                     "related_url": c.related_url,
                                 }
-                                if str(c.type) in ["GEM", "GOLANG", "NPM", "PYPI"]:
-                                    child["upstream_url"] = c.download_url
+                                if c.license_concluded:
+                                    # Some components can't be scanned, e.g. binary RPMs
+                                    child["license_concluded"] = c.license_concluded
+                                if str(c.type) not in ("RPM", "RPMMOD") and (
+                                    # Report container's exact repository_url if present
+                                    # Container Catalog search page is used as a fallback
+                                    # Just ignore it if no specific URL is available
+                                    c.download_url
+                                    != "https://catalog.redhat.com/software/containers/search"
+                                ):
+                                    child["download_url"] = c.download_url
                                 children.append(child)
                         except Exception as exc:
                             logger.warning("%r generated an exception: %s" % (future, exc))
 
                     output[purl]["children"] = children
         return output
```

### Comparing `griffon-0.1.9/griffon/static/default_griffonrc` & `griffon-0.2.0/griffon/static/default_griffonrc`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 [default]
 format = text
 history_log = ~/.griffon/history.log
 profile = default
 verbosity = 0
 sfm2_api_url = http://localhost:5600
 custom_plugin_dir = ~/.griffon/plugins/
+editor = vi
+exclude_components = -container-source
+    -debuginfo
+    -debugsource
+    -static
+    -common-debuginfo
+    -doc
+    -devel
 
 # profile sections (use with --profile {profile} flag)
 [cloud]
 exclude=3amp-2
     amq-.*
     ansible_automation_platform-.*
     codeready_ws-2
```

### Comparing `griffon-0.1.9/griffon.egg-info/PKG-INFO` & `griffon-0.2.0/griffon.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griffon
-Version: 0.1.9
+Version: 0.2.0
 Summary: Red Hat Product Security CLI
 Home-page: https://github.com/RedHatProductSecurity/griffon
 Author: James Fuller, Red Hat Product Security
 License: MIT
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,26 +36,25 @@
   -d, --debug                     Debug log level.
   -f, --format [json|text|table]  Result format (default is text format).
   -v                              Verbose output, more detailed search
                                   results, can be used multiple times (e.g.
                                   -vvv).
   --no-progress-bar               Disable progress bar.
   --no-color                      Disable output of color ansi esc sequences.
-  --profile [cloud|openshift|middleware|latest|all]
+  --profile [default|cloud|openshift|middleware|latest]
                                   Activate profile, defined in .griffonrc.
+  --editor / --no-editor          Allow text editor prompt.
   --help                          Show this message and exit.
 
 Commands:
   configure  Configure griffon.
   docs       Links to useful docs.
-  entities   Entity operations (UNDER DEVELOPMENT).
-  manage     Manage operations.
+  entities   Entity operations.
   plugins    3rd party plugins.
   service    Service operations.
-
 ```
 To install:
 
 ```commandline
 pip install griffon
 ```
```

### Comparing `griffon-0.1.9/griffon.egg-info/SOURCES.txt` & `griffon-0.2.0/griffon.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,25 +11,29 @@
 griffon.egg-info/dependency_links.txt
 griffon.egg-info/entry_points.txt
 griffon.egg-info/requires.txt
 griffon.egg-info/top_level.txt
 griffon/autocomplete/__init__.py
 griffon/commands/configure.py
 griffon/commands/docs.py
-griffon/commands/entities.py
-griffon/commands/manage.py
 griffon/commands/plugin_commands.py
 griffon/commands/process.py
 griffon/commands/queries.py
 griffon/commands/reports.py
+griffon/commands/entities/__init__.py
+griffon/commands/entities/community_component_registry.py
+griffon/commands/entities/corgi.py
+griffon/commands/entities/helpers.py
+griffon/commands/entities/osidb.py
 griffon/commands/plugins/cve_mitre.py
 griffon/commands/plugins/cvelib.py
 griffon/commands/plugins/fcc.py
 griffon/commands/plugins/go_vuln.py
 griffon/commands/plugins/osv.py
+griffon/commands/plugins/semgrep.py
 griffon/services/__init__.py
 griffon/services/core_process.py
 griffon/services/core_queries.py
 griffon/services/core_reports.py
 griffon/static/default_griffonrc
 tests/test_cli.py
 tests/test_entities.py
```

### Comparing `griffon-0.1.9/pyproject.toml` & `griffon-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/setup.py` & `griffon-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/RedHatProductSecurity/griffon",
     description="Red Hat Product Security CLI",
     package_data={"griffon": ["static/*"]},
     packages=[
         "griffon",
         "griffon/commands",
+        "griffon/commands/entities",
         "griffon/commands/plugins",
         "griffon/services",
         "griffon/autocomplete",
     ],
     install_requires=[
         "click",
         "click-completion",
```

### Comparing `griffon-0.1.9/tests/test_cli.py` & `griffon-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/tests/test_process.py` & `griffon-0.2.0/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/tests/test_queries.py` & `griffon-0.2.0/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/tests/test_reports.py` & `griffon-0.2.0/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `griffon-0.1.9/tests/test_unit.py` & `griffon-0.2.0/tests/test_unit.py`

 * *Files identical despite different names*

