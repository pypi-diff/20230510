# Comparing `tmp/chronus-0.3.2.tar.gz` & `tmp/chronus-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronus-0.3.2.tar", max compression
+gzip compressed data, was "chronus-0.3.3.tar", max compression
```

## Comparing `chronus-0.3.2.tar` & `chronus-0.3.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1072 2023-04-28 08:15:27.618142 chronus-0.3.2/LICENSE
--rw-r--r--   0        0        0    10492 2023-04-28 10:32:38.218556 chronus-0.3.2/README.md
--rw-r--r--   0        0        0        1 2023-04-28 08:15:27.622142 chronus-0.3.2/chronus/SystemIntegration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/SystemIntegration/application_runners/__init__.py
--rw-r--r--   0        0        0     6026 2023-05-06 16:21:47.233103 chronus-0.3.2/chronus/SystemIntegration/application_runners/hpcg.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/SystemIntegration/cpu_info_services/__init__.py
--rw-r--r--   0        0        0     2714 2023-05-10 09:48:21.426509 chronus-0.3.2/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
--rw-r--r--   0        0        0        0 2023-05-05 13:33:24.644402 chronus-0.3.2/chronus/SystemIntegration/optimizers/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
--rw-r--r--   0        0        0     3672 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/optimizers/linear_regression.py
--rw-r--r--   0        0        0     2924 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/optimizers/random_tree_forrest.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/SystemIntegration/repositories/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-05 17:12:11.384766 chronus-0.3.2/chronus/SystemIntegration/repositories/csv_repository.py
--rw-r--r--   0        0        0    14565 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/repositories/sqlite_repository.py
--rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/settings_interface/__init__.py
--rw-r--r--   0        0        0     1285 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/settings_interface/etc_storage.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/SystemIntegration/system_service_interfaces/__init__.py
--rw-r--r--   0        0        0     1776 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
--rw-r--r--   0        0        0      330 2023-04-28 08:15:27.622142 chronus-0.3.2/chronus/__init__.py
--rw-r--r--   0        0        0    11706 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/__main__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/application/__init__.py
--rw-r--r--   0        0        0     3710 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/application/benchmark_service.py
--rw-r--r--   0        0        0     2445 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/application/init_model_service.py
--rw-r--r--   0        0        0     1323 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/application/load_model_service.py
--rw-r--r--   0        0        0      602 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/application/run_model_service.py
--rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/cli/__init__.py
--rw-r--r--   0        0        0      742 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/cli/setup.py
--rw-r--r--   0        0        0      197 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/LocalSettings.py
--rw-r--r--   0        0        0     2195 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/Run.py
--rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.2/chronus/domain/__init__.py
--rw-r--r--   0        0        0      461 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/benchmark.py
--rw-r--r--   0        0        0     1181 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/configuration.py
--rw-r--r--   0        0        0      523 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/cpu_info.py
--rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.2/chronus/domain/interfaces/__init__.py
--rw-r--r--   0        0        0      520 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/application_runner_interface.py
--rw-r--r--   0        0        0      158 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/cpu_info_service_interface.py
--rw-r--r--   0        0        0      918 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/optimizer_interface.py
--rw-r--r--   0        0        0      986 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/repository_interface.py
--rw-r--r--   0        0        0      499 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/settings_interface.py
--rw-r--r--   0        0        0      160 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/system_service_interface.py
--rw-r--r--   0        0        0      274 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/model.py
--rw-r--r--   0        0        0      369 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/system_sample.py
--rw-r--r--   0        0        0     3757 2023-05-10 09:51:42.106451 chronus-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    11796 1970-01-01 00:00:00.000000 chronus-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-28 08:15:27.618142 chronus-0.3.3/LICENSE
+-rw-r--r--   0        0        0    10584 2023-05-10 09:58:34.046336 chronus-0.3.3/README.md
+-rw-r--r--   0        0        0        1 2023-04-28 08:15:27.622142 chronus-0.3.3/chronus/SystemIntegration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.3/chronus/SystemIntegration/application_runners/__init__.py
+-rw-r--r--   0        0        0     6026 2023-05-06 16:21:47.233103 chronus-0.3.3/chronus/SystemIntegration/application_runners/hpcg.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.3/chronus/SystemIntegration/cpu_info_services/__init__.py
+-rw-r--r--   0        0        0     2714 2023-05-10 09:48:21.426509 chronus-0.3.3/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:33:24.644402 chronus-0.3.3/chronus/SystemIntegration/optimizers/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
+-rw-r--r--   0        0        0     3672 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/SystemIntegration/optimizers/linear_regression.py
+-rw-r--r--   0        0        0     2924 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/SystemIntegration/optimizers/random_tree_forrest.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.3/chronus/SystemIntegration/repositories/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-05 17:12:11.384766 chronus-0.3.3/chronus/SystemIntegration/repositories/csv_repository.py
+-rw-r--r--   0        0        0    14565 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/SystemIntegration/repositories/sqlite_repository.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/SystemIntegration/settings_interface/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/SystemIntegration/settings_interface/etc_storage.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.3/chronus/SystemIntegration/system_service_interfaces/__init__.py
+-rw-r--r--   0        0        0     1776 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
+-rw-r--r--   0        0        0      330 2023-04-28 08:15:27.622142 chronus-0.3.3/chronus/__init__.py
+-rw-r--r--   0        0        0    11726 2023-05-10 10:06:00.337846 chronus-0.3.3/chronus/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.3/chronus/application/__init__.py
+-rw-r--r--   0        0        0     3710 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/application/benchmark_service.py
+-rw-r--r--   0        0        0     2445 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/application/init_model_service.py
+-rw-r--r--   0        0        0     1323 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/application/load_model_service.py
+-rw-r--r--   0        0        0      602 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/application/run_model_service.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/cli/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/cli/setup.py
+-rw-r--r--   0        0        0      197 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/LocalSettings.py
+-rw-r--r--   0        0        0     2195 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/Run.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.3/chronus/domain/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/benchmark.py
+-rw-r--r--   0        0        0     1181 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/configuration.py
+-rw-r--r--   0        0        0      523 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/cpu_info.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.3/chronus/domain/interfaces/__init__.py
+-rw-r--r--   0        0        0      520 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/interfaces/application_runner_interface.py
+-rw-r--r--   0        0        0      158 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/interfaces/cpu_info_service_interface.py
+-rw-r--r--   0        0        0      918 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/interfaces/optimizer_interface.py
+-rw-r--r--   0        0        0      986 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/interfaces/repository_interface.py
+-rw-r--r--   0        0        0      499 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/interfaces/settings_interface.py
+-rw-r--r--   0        0        0      160 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/interfaces/system_service_interface.py
+-rw-r--r--   0        0        0      274 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/model.py
+-rw-r--r--   0        0        0      369 2023-05-10 09:48:21.430509 chronus-0.3.3/chronus/domain/system_sample.py
+-rw-r--r--   0        0        0     3757 2023-05-10 10:06:00.329846 chronus-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    11888 1970-01-01 00:00:00.000000 chronus-0.3.3/PKG-INFO
```

### Comparing `chronus-0.3.2/LICENSE` & `chronus-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/README.md` & `chronus-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,23 @@
 
 </div>
 
 ## 📖 About
 This is both a library and a CLI application for scheduling energy consumption. The library is build for slurm, and the CLI application is build for the end user.
 
 ## 🚀 Installation
-```
+```shell
 python3 -m pip install chronus
 chronus --help
+
+# To install it with support for making models
+python3 -m pip install chronus[model]
 ```
 
+
 ### Poetry
 
 Want to know more about Poetry? Check [its documentation](https://python-poetry.org/docs/).
 
 <details>
 <summary>Details about Poetry</summary>
 <p>
```

### Comparing `chronus-0.3.2/chronus/SystemIntegration/application_runners/hpcg.py` & `chronus-0.3.3/chronus/SystemIntegration/application_runners/hpcg.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py` & `chronus-0.3.3/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py` & `chronus-0.3.3/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/SystemIntegration/optimizers/linear_regression.py` & `chronus-0.3.3/chronus/SystemIntegration/optimizers/linear_regression.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/SystemIntegration/optimizers/random_tree_forrest.py` & `chronus-0.3.3/chronus/SystemIntegration/optimizers/random_tree_forrest.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/SystemIntegration/repositories/csv_repository.py` & `chronus-0.3.3/chronus/SystemIntegration/repositories/csv_repository.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/SystemIntegration/repositories/sqlite_repository.py` & `chronus-0.3.3/chronus/SystemIntegration/repositories/sqlite_repository.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/SystemIntegration/settings_interface/etc_storage.py` & `chronus-0.3.3/chronus/SystemIntegration/settings_interface/etc_storage.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py` & `chronus-0.3.3/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/__main__.py` & `chronus-0.3.3/chronus/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     if system_id == -1:
         console.print("[yellow]You need to choose a system to train a model.[/yellow]")
         console.print("[green]Here are the available systems:[/green]")
         present_systems(repo)
 
         raise typer.Exit()
 
-    logger.info("Initializing model of type %s", model.name)
+    logger.info("Initializing model of type '%s'", model.name)
     making_model = InitModelService(
         system_id=system_id,
         repository=repo,
         optimizer=_choose_optimizer(model),
     )
 
     with console.status("training model", spinner="dots12"):
@@ -222,21 +222,21 @@
 
         console.print("[yellow]Specify the model id with --model <id>[/yellow]")
 
         raise typer.Exit()
 
     model = repo.get_model(model_id)
 
-    load_model = LoadModelService(
+    _load_model = LoadModelService(
         model_id=model_id,
         repository=repo,
         optimizer=_choose_optimizer(model.type),
-        local_storage=EtcLocalStorage(),
+        local_storage=EtcLocalStorage(Permission.WRITE),
     )
-    load_model.run()
+    _load_model.run()
 
 
 @dataclasses.dataclass
 class ConfigDto:
     cores: int
     frequency: int
     threads_per_core: int
```

### Comparing `chronus-0.3.2/chronus/application/benchmark_service.py` & `chronus-0.3.3/chronus/application/benchmark_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/application/init_model_service.py` & `chronus-0.3.3/chronus/application/init_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/application/load_model_service.py` & `chronus-0.3.3/chronus/application/load_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/application/run_model_service.py` & `chronus-0.3.3/chronus/application/run_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/cli/setup.py` & `chronus-0.3.3/chronus/cli/setup.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/domain/Run.py` & `chronus-0.3.3/chronus/domain/Run.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/domain/configuration.py` & `chronus-0.3.3/chronus/domain/configuration.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/domain/cpu_info.py` & `chronus-0.3.3/chronus/domain/cpu_info.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/domain/interfaces/application_runner_interface.py` & `chronus-0.3.3/chronus/domain/interfaces/application_runner_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/domain/interfaces/optimizer_interface.py` & `chronus-0.3.3/chronus/domain/interfaces/optimizer_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/chronus/domain/interfaces/repository_interface.py` & `chronus-0.3.3/chronus/domain/interfaces/repository_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.2/pyproject.toml` & `chronus-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "chronus"
-version = "0.3.2"
+version = "0.3.3"
 description = "A energy scheduling model, build for HPC."
 readme = "README.md"
 authors = ["chronus <aaspringborg@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/AndersSpringborg/chronus"
 homepage = "https://github.com/AndersSpringborg/chronus"
```

### Comparing `chronus-0.3.2/PKG-INFO` & `chronus-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chronus
-Version: 0.3.2
+Version: 0.3.3
 Summary: A energy scheduling model, build for HPC.
 Home-page: https://github.com/AndersSpringborg/chronus
 License: MIT
 Author: chronus
 Author-email: aaspringborg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -52,19 +52,23 @@
 
 </div>
 
 ## 📖 About
 This is both a library and a CLI application for scheduling energy consumption. The library is build for slurm, and the CLI application is build for the end user.
 
 ## 🚀 Installation
-```
+```shell
 python3 -m pip install chronus
 chronus --help
+
+# To install it with support for making models
+python3 -m pip install chronus[model]
 ```
 
+
 ### Poetry
 
 Want to know more about Poetry? Check [its documentation](https://python-poetry.org/docs/).
 
 <details>
 <summary>Details about Poetry</summary>
 <p>
```

