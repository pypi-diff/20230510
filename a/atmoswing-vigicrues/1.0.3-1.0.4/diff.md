# Comparing `tmp/atmoswing-vigicrues-1.0.3.tar.gz` & `tmp/atmoswing-vigicrues-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.0.3.tar", last modified: Mon May  8 19:16:50 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.0.4.tar", last modified: Wed May 10 12:17:38 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.0.3.tar` & `atmoswing-vigicrues-1.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:50.906946 atmoswing-vigicrues-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 19:16:50.906946 atmoswing-vigicrues-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 19:16:50.906946 atmoswing-vigicrues-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:50.902946 atmoswing-vigicrues-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:50.902946 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:50.906946 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:50.906946 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:50.906946 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:50.906946 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 19:16:50.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-08 19:16:50.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:16:50.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 19:16:50.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 19:16:50.000000 atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:16:50.906946 atmoswing-vigicrues-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-08 19:16:32.000000 atmoswing-vigicrues-1.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.822834 atmoswing-vigicrues-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.822834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.822834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.0.3/LICENSE` & `atmoswing-vigicrues-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/pyproject.toml` & `atmoswing-vigicrues-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/__init__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/__main__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/controller.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,35 +13,28 @@
     Attributes
     ----------
     options : object
         Options de la prévision combinant les arguments passés lors de l'utilisation en
         lignes de commandes et les options du fichier de configuration.
     verbose : bool
         Affichage verbose des messages d'erreurs (pas beaucoup utilisé)
-    max_attempts : int
-        Nombre de tentatives de téléchargement en adaptant l'heure d'échéance
-        (soustrayant 6 h). Valeur par défaut : 8
-    time_increment : int
-        Pas de temps (h) auquel émettre la prévision (p. ex. toutes les 6h)
     date : datetime
         Date de la prévision.
     """
 
     def __init__(self, cli_options):
         """
         Initialisation de l'instance Controller
 
         Parameters
         ----------
         cli_options : object
             Options passées en lignes de commandes à la fonction main()
         """
         self.options = asv.Options(cli_options)
-        self.verbose = True
-        self.max_attempts = 8
         self.time_increment = 6
         self.date = datetime.datetime.utcnow()
         self.pre_actions = []
         self.post_actions = []
         self.disseminations = []
         self._register_pre_actions()
         self._register_post_actions()
@@ -89,120 +82,132 @@
         """
         if self.options.has('pre_actions'):
             for action in self.options.get('pre_actions'):
                 if 'active' in action and not action['active']:
                     continue
                 name = action['name']
                 module = action['uses']
-                self._display_message(f"Chargement de la pre-action '{name}'")
+                print(f"Chargement de la pre-action '{name}'")
                 if not hasattr(importlib.import_module('atmoswing_vigicrues'), module):
                     raise asv.Error(f"L'action {module} est inconnue.")
                 fct = getattr(importlib.import_module('atmoswing_vigicrues'), module)
-                self.pre_actions.append(fct(action['with']))
+                self.pre_actions.append(fct(name, action['with']))
 
     def _register_post_actions(self):
         """
         Enregistre les actions postérieures à la prévision
         """
         if self.options.has('post_actions'):
             for action in self.options.get('post_actions'):
                 if 'active' in action and not action['active']:
                     continue
                 name = action['name']
                 module = action['uses']
-                self._display_message(f"Chargement de la post-action '{name}'")
+                print(f"Chargement de la post-action '{name}'")
                 if not hasattr(importlib.import_module('atmoswing_vigicrues'), module):
                     raise asv.Error(f"L'action {module} est inconnue.")
                 fct = getattr(importlib.import_module('atmoswing_vigicrues'), module)
-                self.post_actions.append(fct(action['with']))
+                self.post_actions.append(fct(name, action['with']))
 
     def _register_disseminations(self):
         """
         Enregistre les actions préalables à la prévision
         """
         if self.options.has('disseminations'):
             for action in self.options.get('disseminations'):
                 if 'active' in action and not action['active']:
                     continue
                 name = action['name']
                 module = action['uses']
-                self._display_message(f"Chargement de la disseminations '{name}'")
+                print(f"Chargement de la disseminations '{name}'")
                 if not hasattr(importlib.import_module('atmoswing_vigicrues'), module):
                     raise asv.Error(f"L'action {module} est inconnue.")
                 fct = getattr(importlib.import_module('atmoswing_vigicrues'), module)
-                self.disseminations.append(fct(action['with']))
+                self.disseminations.append(fct(name, action['with']))
 
     def _run_pre_actions(self):
         """
         Exécute les opérations préalables à la prévision par AtmoSwing.
         """
-        if not self.pre_actions:
+        if not self.pre_actions or len(self.pre_actions) == 0:
             return
 
-        attempts = 0
-        while attempts < self.max_attempts:
+        attempts_max_hours = 7 * 24
+        attempts_step_hours = 6
+        for action in self.pre_actions:
+            attempts_max_hours = min(attempts_max_hours, action.attempts_max_hours)
+            attempts_step_hours = max(attempts_step_hours, action.attempts_step_hours)
+
+        attempts_hours = 0
+        while attempts_hours < attempts_max_hours:
             success = True
             for action in self.pre_actions:
-                self._display_message(f"Exécution de : '{action.name}'")
+                print(f"Exécution de : '{action.type_name}' [{action.name}]")
                 if not action.run(self.date):
-                    attempts += 1
+                    attempts_hours += attempts_step_hours
                     success = False
                     break
             if success:
+                print("  -> Exécution correcte")
                 break
             else:
-                self._back_in_time()
+                print("  -> Recul de l'heure de la prévision")
+                self._back_in_time(attempts_step_hours)
+        else:
+            print("  -> Échec de l'exécution")
+            raise asv.Error("Nombre maximum de tentatives atteint pour la pré-action.")
 
     def _run_atmoswing(self):
         """
         Exécution d'AtmoSwing.
         """
         run = self.options.get('atmoswing')
         name = run['name']
         options = run['with']
         cmd = self._build_atmoswing_cmd(options)
-        self._display_message(f"Exécution de : '{name}'")
+        print(f"Exécution de : '{name}'")
+        print(f"Prévision pour la date : {self.date.strftime('%Y-%m-%d %H')}")
         print("Commande: " + ' '.join(cmd))
 
         try:
             ret = subprocess.run(cmd, capture_output=True, check=True)
 
             if ret.returncode != 0:
-                print("L'exécution d'AtmoSwing Forecaster a échoué.")
-                raise asv.Error("L'exécution d'AtmoSwing Forecaster a échoué.")
+                print("  -> Échec de l'exécution")
             else:
-                print("AtmoSwing Forecaster a été exécuté avec succès.")
+                print("  -> Exécution correcte")
         except Exception as e:
+            print("  -> Échec de l'exécution")
             print(f"Exception lors de l'exécution d'AtmoSwing Forecaster: {e}")
 
     def _build_atmoswing_cmd(self, options):
         now_str = self.date.strftime("%Y%m%d%H")
         cmd = []
 
         if 'atmoswing_path' not in options or not options['atmoswing_path']:
             cmd.append("atmoswing-forecaster")
         else:
             cmd.append(options['atmoswing_path'])
 
         if 'batch_file' not in options or not options['batch_file']:
-            raise asv.Error(f"Option 'batch_file' non fournie.")
+            raise asv.Error("Option 'batch_file' non fournie.")
         cmd.append("-f")
         cmd.append(options['batch_file'])
 
         if 'target' in options:
             if options['target'] == 'now':
                 cmd.append(f"--forecast-date={now_str}")
             elif options['target'] == 'past':
                 if 'target_nb_days' not in options or not options['target_nb_days']:
-                    raise asv.Error(f"Option 'target_nb_days' non fournie.")
+                    raise asv.Error("Option 'target_nb_days' non fournie.")
                 nb_days = options['target_nb_days']
                 cmd.append(f"--forecast-past={nb_days}")
             elif options['target'] == 'date':
                 if 'target_date' not in options or not options['target_date']:
-                    raise asv.Error(f"Option 'target_date' non fournie.")
+                    raise asv.Error("Option 'target_date' non fournie.")
                 date = options['target_date']
                 cmd.append(f"--forecast-date={date}")
         else:
             cmd.append(f"--forecast-date={now_str}")
 
         if 'proxy' in options and options['proxy']:
             cmd.append(f"--proxy={options['proxy']}")
@@ -211,52 +216,54 @@
 
         return cmd
 
     def _run_post_actions(self):
         """
         Exécute les opérations postérieures à la prévision par AtmoSwing.
         """
-        if not self.post_actions:
+        if not self.post_actions or len(self.post_actions) == 0:
             return
 
         files = self._list_atmoswing_output_files()
         for action in self.post_actions:
-            self._display_message(f"Exécution de : '{action.name}'")
+            print(f"Exécution de : '{action.type_name}' [{action.name}]")
             action.feed(files, {'forecast_date': self.date})
-            action.run()
+            if action.run():
+                print("  -> Exécution correcte")
+            else:
+                print("  -> Échec de l'exécution")
 
     def _run_disseminations(self):
         """
         Exécute les opérations de diffusion.
         """
-        if not self.disseminations:
+        if not self.disseminations or len(self.disseminations) == 0:
             return
 
         for action in self.disseminations:
-            self._display_message(f"Exécution de : '{action.name}'")
+            print(f"Exécution de : '{action.type_name}' [{action.name}]")
             local_dir = action.local_dir
             extension = action.extension
             files = self._list_files(local_dir, extension)
             action.feed(files)
-            action.run(self.date)
-
-    def _display_message(self, message):
-        if self.verbose:
-            print(message)
+            if action.run(self.date):
+                print("  -> Exécution correcte")
+            else:
+                print("  -> Échec de l'exécution")
 
     def _fix_date(self):
         date = self.date
         if isinstance(date, str):
             date = datetime.datetime.strptime(date, "%Y-%m-%d %H")
         hour = date.hour
         hour = self.time_increment * (hour // self.time_increment)
         self.date = datetime.datetime(date.year, date.month, date.day, hour)
 
-    def _back_in_time(self):
-        self.date = self.date - datetime.timedelta(hours=self.time_increment)
+    def _back_in_time(self, time_increment):
+        self.date = self.date - datetime.timedelta(hours=time_increment)
 
     def _list_atmoswing_output_files(self):
         output_dir = self.options.get('atmoswing')['with']['output_dir']
         return self._list_files(output_dir, '.nc', '%Y-%m-%d_%H')
 
     def _list_files(self, local_dir, ext, pattern='%Y-%m-%d_%H'):
         local_dir = asv.utils.build_date_dir_structure(local_dir, self.date)
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         Parameters
         ----------
         file_paths : list
             Chemins des fichiers à diffuser.
         """
         self._file_paths = file_paths
 
-    def run(self, date):
+    def run(self, date) -> bool:
         """
         Exécution de la diffusion.
 
         Parameters
         ----------
         date : datetime
             Date de la prévision.
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import os
 
-import paramiko, socks
+import paramiko
+import socks
 
 import atmoswing_vigicrues as asv
 
 from .dissemination import Dissemination
 
 
 class TransferSftpOut(Dissemination):
     """
     Transfer des résultats par SFTP.
 
     Parameters
     ----------
+    name: str
+        Le nom de l'action
     options: objet
         L'instance contenant les options de l'action. Les champs possibles sont:
 
         * local_dir : str
             Répertoire local contenant les fichiers à exporter.
         * extension : str
             Extension des fichiers à exporter.
@@ -32,19 +35,20 @@
             Adresse du proxy, si nécessaire.
         * proxy_port : int
             Port du proxy si nécessaire (par défaut: 1080).
         * remote_dir : str
             Chemin sur le serveur distant où enregistrer les fichiers.
     """
 
-    def __init__(self, options):
+    def __init__(self, name, options):
         """
         Initialisation de l'instance TransferSftp
         """
-        self.name = "Transfert SFTP"
+        self.type_name = "Transfert SFTP"
+        self.name = name
         self.local_dir = options['local_dir']
         self.extension = options['extension']
         self.hostname = options['hostname']
         self.port = options['port']
         self.username = options['username']
         self.password = options['password']
         self.remote_dir = options['remote_dir']
@@ -56,23 +60,31 @@
             else:
                 self.proxy_port = 1080
         else:
             self.proxy_host = None
 
         super().__init__()
 
-    def run(self, date):
+    def run(self, date) -> bool:
         """
         Exécution de la diffusion par SFTP.
 
         Parameters
         ----------
         date : datetime
             Date de la prévision.
+
+        Returns
+        -------
+        Vrai (True) en cas de succès, faux (False) autrement.
         """
+        if not self._file_paths:
+            print("Aucun fichier à traiter")
+            return False
+
         try:
             if self.proxy_host:
                 sock = socks.socksocket()
                 sock.set_proxy(
                     proxy_type=socks.SOCKS5,
                     addr=self.proxy_host,
                     port=self.proxy_port
@@ -97,28 +109,38 @@
             if sftp:
                 sftp.close()
             if transport:
                 transport.close()
 
         except paramiko.ssh_exception.PasswordRequiredException as e:
             print(f"SFTP PasswordRequiredException {e}")
+            return False
         except paramiko.ssh_exception.BadAuthenticationType as e:
             print(f"SFTP BadAuthenticationType {e}")
+            return False
         except paramiko.ssh_exception.AuthenticationException as e:
             print(f"SFTP AuthenticationException {e}")
+            return False
         except paramiko.ssh_exception.ChannelException as e:
             print(f"SFTP ChannelException {e}")
+            return False
         except paramiko.ssh_exception.ProxyCommandFailure as e:
             print(f"SFTP ProxyCommandFailure {e}")
+            return False
         except paramiko.ssh_exception.SSHException as e:
             print(f"SFTP SSHException {e}")
+            return False
         except FileNotFoundError as e:
             print(f"SFTP FileNotFoundError {e}")
+            return False
         except Exception as e:
             print(f"La diffusion SFTP a échoué ({e}).")
+            return False
+
+        return True
 
     @staticmethod
     def _chdir_or_mkdir(dir_path, sftp):
         try:
             sftp.chdir(dir_path)
         except IOError:
             sftp.mkdir(dir_path)
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,36 @@
 
 class ExportBdApBp(PostAction):
     """
     Export des prévisions au format Json de la BdApBp.
 
     Parameters
     ----------
+    name: str
+        Le nom de l'action
     options: objet
         L'instance contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Chemin cible pour l'enregistrement des fichiers.
         * number_analogs : int
             Nombre d'analogues maximal à conserver (valeurs les plus élevées).
             -1 pour toutes les analogues.
         * only_relevant_stations : bool
             Exporter uniquement les stations pour lesquelles la méthode a été calibrée.
         * use_indentation : bool
             Ajouter une indentation aux fichiers produits.
     """
 
-    def __init__(self, options):
+    def __init__(self, name, options):
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
 
-        self.name = "Export BdApBp"
+        self.type_name = "Export BdApBp"
+        self.name = name
         self.status = 100
         self.message = ""
 
         self.output_dir = options['output_dir']
         asv.check_dir_exists(self.output_dir, True)
 
         if 'number_analogs' in options:
@@ -54,24 +57,32 @@
         else:
             self.use_indentation = False
 
         self._reset_status()
 
         super().__init__()
 
-    def run(self):
+    def run(self) -> bool:
         """
         Exécution de la post-action.
 
         Erreurs possibles:
 
         * 100 : Absence du fichier netcdf.
         * 110 : Fichier netcdf corrompu.
         * 200 : Erreur lors du traitement fichier netcdf.
+
+        Returns
+        -------
+        Vrai (True) en cas de succès, faux (False) autrement.
         """
+        if not self._file_paths:
+            print("Aucun fichier à traiter")
+            return False
+
         for file in self._file_paths:
             file = Path(file)
             self._reset_status()
             nc_file = None
 
             if not asv.file_exists(file):
                 self.status = 100
@@ -119,14 +130,16 @@
                     json.dump(data, outfile, indent=4, ensure_ascii=False)
                 else:
                     json.dump(data, outfile, ensure_ascii=False)
 
             if nc_file:
                 nc_file.close()
 
+        return True
+
     def _create_metadata_block(self, nc_file):
         block = {
             'atmoswing': {
                 'creation_date': nc_file.creation_date,
                 'origin': nc_file.origin
             },
             'predictand': {
@@ -318,8 +331,7 @@
             original_file_name = now.strftime("%Y-%m-%d_%H%M%S") + '_missing'
         file_name = f'{original_file_name}.json'
         if '.nc' in original_file_name:
             file_name = original_file_name.replace('.nc', '.json')
         output_dir = self._get_output_path(self._get_metadata('forecast_date'))
         file_path = output_dir / file_name
         return file_path
-
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,34 @@
 
 class ExportPrv(PostAction):
     """
     Export des prévisions au format PRV du logiciel Scores.
 
     Parameters
     ----------
+    name: str
+        Le nom de l'action
     options: objet
         L'instance contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Chemin cible pour l'enregistrement des fichiers.
         * frequencies : list
             Les fréquences à extraire.
             Par défaut : [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 0.95]
         * combine_stations_in_one_file : bool
             Combinaison des différentes stations (entités) dans un seul fichier.
     """
 
-    def __init__(self, options):
+    def __init__(self, name, options):
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
 
-        self.name = "Export PRV"
+        self.type_name = "Export PRV"
+        self.name = name
         self.output_dir = options['output_dir']
         asv.check_dir_exists(self.output_dir, True)
 
         if 'frequencies' in options:
             self.frequencies = options['frequencies']
         else:
             self.frequencies = [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 0.95]
@@ -41,18 +44,26 @@
         if 'combine_stations_in_one_file' in options:
             self.combine_stations_in_one_file = options['combine_stations_in_one_file']
         else:
             self.combine_stations_in_one_file = True
 
         super().__init__()
 
-    def run(self):
+    def run(self) -> bool:
         """
         Exécution de la post-action.
+
+        Returns
+        -------
+        Vrai (True) en cas de succès, faux (False) autrement.
         """
+        if not self._file_paths:
+            print("Aucun fichier à traiter")
+            return False
+
         for file in self._file_paths:
             nc_file = asv.Dataset(file, 'r', format='NETCDF4')
             station_ids = self._extract_station_ids(nc_file)
             header_comments = self._create_header_comments(nc_file)
             if self.combine_stations_in_one_file:
                 header_data = self._create_header_data(nc_file, station_ids)
                 content = self._create_content(nc_file, station_ids)
@@ -68,19 +79,22 @@
                     header_data = self._create_header_data(nc_file, station_id)
                     content = self._create_content(nc_file, station_id)
                     full_content = f"{header_comments}{header_data}{content}"
 
                     # File name
                     file_path = self._build_file_path(file, station_id)
 
-                    with open(file_path, 'w', encoding="utf-8", newline='\r\n') as outfile:
+                    with open(file_path, 'w', encoding="utf-8", newline='\r\n') \
+                            as outfile:
                         outfile.write(full_content)
 
             nc_file.close()
 
+        return True
+
     def _create_header_comments(self, nc_file):
         list_frequencies = [str(int(100 * i)) for i in self.frequencies]
 
         header = \
             f"# Sortie du module ExportPrv de AtmoSwing-Vigicrues\n" \
             f"# origin;{nc_file.origin}\n" \
             f"# creation_date;{nc_file.creation_date}\n" \
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import atmoswing_vigicrues as asv
-
 
 class PostAction:
     """
     Classe de base pour les opérations de traitement des résultats d'AtmoSwing.
     """
 
     def __init__(self):
@@ -21,15 +19,15 @@
             Chemins des fichiers de prévision émis par AtmoSwing.
         metadata : dict
             Méta-données issues de la prévision.
         """
         self._file_paths = file_paths
         self._metadata = metadata
 
-    def run(self):
+    def run(self) -> bool:
         raise NotImplementedError
 
     def _get_metadata(self, key):
         if key in self._metadata:
             return self._metadata[key]
         return None
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 class DownloadGfsData(PreAction):
     """
     Téléchargement des prévisions émises par GFS.
 
     Parameters
     ----------
+    name: str
+        Le nom de l'action
     options: objet
         L'instance contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Répertoire cible pour l'enregistrement des fichiers.
         * lead_time_max : int
             Échéance maximale de la prévision en heures.
@@ -32,21 +34,28 @@
             Résolution spatiale des données.
             Options: 0.25, 0.50, 1
             Valeur par défaut : 0.25
         * proxy_host : str
             L'adresse du proxy (si nécessaire). Format : proxy_ip:proxy_port
         * proxy_user : str
             L'utilisateur et le mot de passe pour le proxy. Format : username:password
+        * attempts_max_hours : int
+            Décalage temporel autorisé pour rechercher d'anciens fichiers
+        * attempts_step_hours : int
+            Pas de temps auquel décrémenter la date pour rechercher d'anciens fichiers
     """
 
-    def __init__(self, options):
-        self.name = "Téléchargement GFS"
+    def __init__(self, name, options):
+        self.type_name = "Téléchargement GFS"
+        self.name = name
         self.output_dir = options['output_dir']
         asv.check_dir_exists(self.output_dir, True)
 
+        self._set_attempts_attributes(options)
+
         if 'lead_time_max' in options:
             self.lead_time_max = options['lead_time_max']
         else:
             self.lead_time_max = 168
 
         if 'variables' in options:
             self.variables = options['variables']
@@ -183,15 +192,15 @@
         local_path.mkdir(parents=True, exist_ok=True)
         return local_path
 
     def _build_levels_request(self):
         levels = []
         for level in self.levels:
             if isinstance(level, str) and level == 'surface':
-                levels.append(f'lev_surface=on&')
+                levels.append('lev_surface=on&')
             if isinstance(level, str) and level == 'entire_atmosphere':
                 levels.append('lev_entire_atmosphere_%5C%28considered'
                               '_as_a_single_layer%5C%29=on&')
             if isinstance(level, int) or isinstance(level, float):
                 levels.append(f'lev_{int(level)}_mb=on&')
         levels = ''.join(levels)
         return levels
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import os
 import fnmatch
 from pathlib import Path
 import tarfile
 
-import paramiko, socks
+import paramiko
+import socks
 
 import atmoswing_vigicrues as asv
 
 from .preaction import PreAction
 
 
 class TransferSftpIn(PreAction):
     """
     Récupération des prévisions des modèles météo par SFTP.
 
     Parameters
     ----------
+    name: str
+        Le nom de l'action
     options: objet
         L'instance contenant les options de l'action. Les champs possibles sont:
 
         * local_dir : str
             Répertoire cible pour l'enregistrement des fichiers.
         * prefix : str
             Prefix des fichiers à importer.
@@ -33,29 +36,36 @@
             Mot de passe de l'utilisateur sur le serveur.
         * proxy_host : str
             Adresse du proxy, si nécessaire.
         * proxy_port : int
             Port du proxy si nécessaire (par défaut: 1080).
         * remote_dir : str
             Chemin sur le serveur distant où se trouvent les fichiers.
+        * attempts_max_hours : int
+            Décalage temporel autorisé pour rechercher d'anciens fichiers
+        * attempts_step_hours : int
+            Pas de temps auquel décrémenter la date pour rechercher d'anciens fichiers
     """
 
-    def __init__(self, options):
+    def __init__(self, name, options):
         """
         Initialisation de l'instance TransferSftp
         """
-        self.name = "Transfert SFTP"
+        self.type_name = "Transfert SFTP"
+        self.name = name
         self.local_dir = options['local_dir']
         self.prefix = options['prefix']
         self.hostname = options['hostname']
         self.port = options['port']
         self.username = options['username']
         self.password = options['password']
         self.remote_dir = options['remote_dir']
 
+        self._set_attempts_attributes(options)
+
         if 'proxy_host' in options:
             self.proxy_host = options['proxy_host']
             if 'proxy_port' in options:
                 self.proxy_port = options['proxy_port']
             else:
                 self.proxy_port = 1080
         else:
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 
 class TransformEcmwfData(PreAction):
     """
     Transforme les prévisions émises par l'ECMWF en fichier netcdf.
     """
 
-    def __init__(self, options):
+    def __init__(self, name, options):
         """
         Initialisation de l'instance TransformEcmwfData
 
         Parameters
         ----------
+        name: str
+            Le nom de l'action
         options
             L'instance contenant les options de l'action. Les champs possibles sont:
             * transform_ecmwf_input_dir: str
                 Répertoire contenant les fichiers originaux (grib2).
             * transform_ecmwf_output_dir: str
                 Répertoire cible pour l'enregistrement des fichiers.
             * ecmwf_variables: list
@@ -29,19 +31,22 @@
                 Valeur par défaut: ['hgt']
         """
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
         if not asv.has_eccodes:
             raise ImportError("Le paquet eccodes est requis pour cette action.")
 
-        self.name = "Transformation données ECMWF"
+        self.type_name = "Transformation données ECMWF"
+        self.name = name
         self.input_dir = options.get('transform_ecmwf_input_dir')
         self.output_dir = options.get('transform_ecmwf_output_dir')
         asv.check_dir_exists(self.output_dir, True)
 
+        self._set_attempts_attributes(options)
+
         if options.has('ecmwf_variables'):
             self.variables = options.get('ecmwf_variables')
         else:
             self.variables = ['z']
 
         super().__init__()
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import atmoswing_vigicrues as asv
-from datetime import datetime
 #if asv.has_eccodes and asv.has_netcdf:
 #    from atmoswing_toolbox.datasets import generic, grib_dataset
 
 
 from .preaction import PreAction
 
 
 class TransformGfsData(PreAction):
     """
     Transforme les prévisions émises par GFS en fichier netcdf.
     """
 
-    def __init__(self, options):
+    def __init__(self, name, options):
         """
         Initialisation de l'instance TransformGfsData
 
         Parameters
         ----------
+        name: str
+            Le nom de l'action
         options
             L'instance contenant les options de l'action. Les champs possibles sont:
             * transform_gfs_input_dir: str
                 Répertoire contenant les fichiers originaux (grib2).
             * transform_gfs_output_dir: str
                 Répertoire cible pour l'enregistrement des fichiers.
             * gfs_variables: list
@@ -29,19 +30,22 @@
                 Valeur par défaut: ['hgt']
         """
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
         if not asv.has_eccodes:
             raise ImportError("Le paquet eccodes est requis pour cette action.")
 
-        self.name = "Transformation données GFS"
+        self.type_name = "Transformation données GFS"
+        self.name = name
         self.input_dir = options.get('transform_gfs_input_dir')
         self.output_dir = options.get('transform_gfs_output_dir')
         asv.check_dir_exists(self.output_dir, True)
 
+        self._set_attempts_attributes(options)
+
         if options.has('gfs_variables'):
             self.variables = options.get('gfs_variables')
         else:
             self.variables = ['hgt']
 
         super().__init__()
 
@@ -106,8 +110,8 @@
         return output_dir
 
     @staticmethod
     def _format_forecast_date(date):
         forecast_date = date.strftime("%Y%m%d")
         hour = 6 * (date.hour // 6)
         forecast_hour = f'{hour:02d}'
-        return forecast_date, forecast_hour
+        return forecast_date, forecast_hour
```

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/utils.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/tests/test_controller.py` & `atmoswing-vigicrues-1.0.4/tests/test_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     assert hasattr(importlib.import_module('atmoswing_vigicrues'), 'DownloadGfsData')
     with tempfile.TemporaryDirectory() as tmp_dir:
         options = asv.Options(
             types.SimpleNamespace(
                 config_file=DIR_PATH + '/files/config_gfs_download.yaml'))
         fct = getattr(importlib.import_module('atmoswing_vigicrues'), 'DownloadGfsData')
         action = options.config['pre_actions'][0]
-        fct(action['with'])
+        fct('Download GFS data', action['with'])
 
 
 def test_run_atmoswing_now():
     options = types.SimpleNamespace(
         config_file=DIR_PATH + '/files/config_atmoswing_now.yaml',
         batch_file=DIR_PATH + '/files/batch_file.xml'
     )
@@ -103,7 +103,26 @@
         config_file=DIR_PATH + '/files/config_with_special_characters.yaml',
         batch_file=DIR_PATH + '/files/batch_file.xml'
     )
     controller = asv.Controller(options)
     decoded_password = controller.options.config['pre_actions'][0]['with']['password']
     assert decoded_password == '@#°§&£¢$*[]{}()+'
 
+
+def test_catches_atmoswing_when_failing():
+    options = types.SimpleNamespace(
+        config_file=DIR_PATH + '/files/config_atmoswing_now_full.yaml',
+        batch_file=DIR_PATH + '/files/batch_file_fail.xml'
+    )
+    controller = asv.Controller(options)
+    if RUN_ATMOSWING:
+        controller.run()
+
+
+def test_flux_stops_when_preprocess_failing():
+    options = types.SimpleNamespace(
+        config_file=DIR_PATH + '/files/config_atmoswing_now_failing_preaction.yaml',
+        batch_file=DIR_PATH + '/files/batch_file_fail.xml'
+    )
+    controller = asv.Controller(options)
+    if RUN_ATMOSWING:
+        controller.run()
```

### Comparing `atmoswing-vigicrues-1.0.3/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.0.4/tests/test_download_gfs.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,66 +27,66 @@
 
 def count_files_recursively(options):
     nb_files = sum([len(files) for r, d, files in os.walk(options['output_dir'])])
     return nb_files
 
 
 def test_download_gfs_fails_if_files_not_found(options):
-    action = asv.DownloadGfsData(options)
+    action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow()
     date = date.replace(date.year + 1)
     assert action.download(date) is False
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_025_succeeds(options):
     options['resolution'] = 0.25
-    action = asv.DownloadGfsData(options)
+    action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.download(date)
     assert count_files_recursively(options) == 3 * 4
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_050_succeeds(options):
     options['resolution'] = 0.50
-    action = asv.DownloadGfsData(options)
+    action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.download(date)
     assert count_files_recursively(options) == 3 * 4
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_100_succeeds(options):
     options['resolution'] = 1
-    action = asv.DownloadGfsData(options)
+    action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.download(date)
     assert count_files_recursively(options) == 3 * 4
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_default_succeeds(options):
-    action = asv.DownloadGfsData(options)
+    action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.download(date)
     assert count_files_recursively(options) == 3 * 4
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_with_surface_var(options):
     options['levels'] = [500, 1000, 'surface']
-    action = asv.DownloadGfsData(options)
+    action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.run(date)
     assert count_files_recursively(options) == 3 * 4
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_entire_atmosphere_var(options):
     options['levels'] = ['entire_atmosphere']
     options['variables'] = ['pwat']
-    action = asv.DownloadGfsData(options)
+    action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.run(date)
     assert count_files_recursively(options) == 3 * 4
     shutil.rmtree(options['output_dir'])
```

### Comparing `atmoswing-vigicrues-1.0.3/tests/test_exceptions.py` & `atmoswing-vigicrues-1.0.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.0.4/tests/test_export_bdapbp.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 def count_files_recursively(options):
     nb_files = sum([len(files) for r, d, files in os.walk(options['output_dir'])])
     return nb_files
 
 
 def test_export_bdapbp_reports_if_files_not_found(options, metadata):
-    export = asv.ExportBdApBp(options)
+    export = asv.ExportBdApBp('Export BdApBp', options)
     export.feed(['/wrong/path'], metadata)
     export.run()
     assert count_files_recursively(options) == 1
     file_path = options['output_dir'] + '/2022/10/01/path.json'
     with open(file_path) as f:
         data = json.load(f)
         assert data['status'] == 200
@@ -53,15 +53,15 @@
 
 @pytest.fixture
 def forecast_files():
     return glob.glob(DIR_PATH + "/files/atmoswing-forecasts-v2.1/2022/10/01/*.nc")
 
 
 def test_export_bdapbp_runs(options, forecast_files, metadata):
-    export = asv.ExportBdApBp(options)
+    export = asv.ExportBdApBp('Export BdApBp', options)
     export.feed(forecast_files, metadata)
     export.run()
     assert count_files_recursively(options) == 3
 
     created_files = [
         '2022-10-01_00.PC-AZ4o.Alpes_bernoises_est.json',
         '2022-10-01_00.PC-AZ4o.Chablais.json',
@@ -75,15 +75,15 @@
     shutil.rmtree(options['output_dir'])
 
 
 def test_export_bdapbp_with_no_limit(options, forecast_files, metadata):
     forecast_files.sort()
     forecast_files = [forecast_files[0]]
     options['number_analogs'] = -1
-    export = asv.ExportBdApBp(options)
+    export = asv.ExportBdApBp('Export BdApBp', options)
     export.feed(forecast_files, metadata)
     export.run()
     assert count_files_recursively(options) == 1
 
     created_files = [
         '2022-10-01_00.PC-AZ4o.Alpes_bernoises_est.json'
     ]
@@ -95,15 +95,15 @@
     shutil.rmtree(options['output_dir'])
 
 
 def test_export_bdapbp_with_all_stations(options, forecast_files, metadata):
     forecast_files.sort()
     forecast_files = [forecast_files[0]]
     options['only_relevant_stations'] = False
-    export = asv.ExportBdApBp(options)
+    export = asv.ExportBdApBp('Export BdApBp', options)
     export.feed(forecast_files, metadata)
     export.run()
     assert count_files_recursively(options) == 1
 
     created_files = [
         '2022-10-01_00.PC-AZ4o.Alpes_bernoises_est.json'
     ]
```

### Comparing `atmoswing-vigicrues-1.0.3/tests/test_export_prv.py` & `atmoswing-vigicrues-1.0.4/tests/test_export_prv.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,33 +40,33 @@
 
 @pytest.fixture
 def forecast_files():
     return glob.glob(DIR_PATH + "/files/atmoswing-forecasts-v2.1/2022/10/01/*.nc")
 
 
 def test_export_prv_runs(options, forecast_files, metadata):
-    export = asv.ExportPrv(options)
+    export = asv.ExportPrv('Export PRV', options)
     export.feed(forecast_files, metadata)
     export.run()
     assert count_files_recursively(options) == 3
     shutil.rmtree(options['output_dir'])
 
 
 def test_export_prv_runs_separate_files(options, forecast_files, metadata):
     options['combine_stations_in_one_file'] = False
-    export = asv.ExportPrv(options)
+    export = asv.ExportPrv('Export PRV', options)
     export.feed(forecast_files, metadata)
     export.run()
     assert count_files_recursively(options) == 21
     shutil.rmtree(options['output_dir'])
 
 
 def test_export_prv_runs_multi_time_steps(options):
     files = glob.glob(DIR_PATH + "/files/atmoswing-forecasts-v2.1/2022/12/16/*.nc")
     metadata = {
         "forecast_date": "2022-12-16 00:00:00",
     }
-    export = asv.ExportPrv(options)
+    export = asv.ExportPrv('Export PRV', options)
     export.feed(files, metadata)
     export.run()
     assert count_files_recursively(options) == 4
     shutil.rmtree(options['output_dir'])
```

### Comparing `atmoswing-vigicrues-1.0.3/tests/test_options.py` & `atmoswing-vigicrues-1.0.4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.3/tests/test_utils.py` & `atmoswing-vigicrues-1.0.4/tests/test_utils.py`

 * *Files identical despite different names*

