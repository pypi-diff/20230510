# Comparing `tmp/chronus-0.2.3.tar.gz` & `tmp/chronus-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronus-0.2.3.tar", max compression
+gzip compressed data, was "chronus-0.3.0.tar", max compression
```

## Comparing `chronus-0.2.3.tar` & `chronus-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,45 @@
--rw-r--r--   0        0        0     1072 2023-02-28 09:33:02.453690 chronus-0.2.3/LICENSE
--rw-r--r--   0        0        0    10481 2023-04-17 11:01:17.462307 chronus-0.2.3/README.md
--rw-r--r--   0        0        0     1122 2023-04-21 06:57:23.169699 chronus-0.2.3/chronus/SystemIntegration/FileRepository.py
--rw-r--r--   0        0        0        1 2023-04-17 10:44:37.558827 chronus-0.2.3/chronus/SystemIntegration/__init__.py
--rw-r--r--   0        0        0     1781 2023-04-23 12:23:42.096207 chronus-0.2.3/chronus/SystemIntegration/cpu_info_service.py
--rw-r--r--   0        0        0     1551 2023-04-21 06:57:23.179206 chronus-0.2.3/chronus/SystemIntegration/hpcg.py
--rw-r--r--   0        0        0      200 2023-04-21 11:06:34.779261 chronus-0.2.3/chronus/SystemIntegration/repository.py
--rw-r--r--   0        0        0      330 2023-04-17 10:14:26.979910 chronus-0.2.3/chronus/__init__.py
--rw-r--r--   0        0        0     4251 2023-04-21 13:45:31.416762 chronus-0.2.3/chronus/__main__.py
--rw-r--r--   0        0        0     1497 2023-04-21 06:57:23.157333 chronus-0.2.3/chronus/cli/__init__.py
--rw-r--r--   0        0        0     1224 2023-04-21 13:37:43.015999 chronus-0.2.3/chronus/domain/Run.py
--rw-r--r--   0        0        0        0 2023-04-17 10:14:26.980936 chronus-0.2.3/chronus/domain/__init__.py
--rw-r--r--   0        0        0     2075 2023-04-21 13:37:43.018032 chronus-0.2.3/chronus/domain/benchmark_service.py
--rw-r--r--   0        0        0      975 2023-04-21 13:37:40.293638 chronus-0.2.3/chronus/domain/configuration.py
--rw-r--r--   0        0        0        0 2023-04-21 06:56:28.522159 chronus-0.2.3/chronus/domain/interfaces/__init__.py
--rw-r--r--   0        0        0      163 2023-04-21 06:53:32.150630 chronus-0.2.3/chronus/domain/interfaces/application_runner_interface.py
--rw-r--r--   0        0        0       91 2023-04-21 06:54:31.741981 chronus-0.2.3/chronus/domain/interfaces/benchmark_run_repository_interface.py
--rw-r--r--   0        0        0      300 2023-04-21 13:37:42.986739 chronus-0.2.3/chronus/domain/interfaces/cpu_info_service_interface.py
--rw-r--r--   0        0        0      137 2023-04-21 06:56:09.236466 chronus-0.2.3/chronus/domain/interfaces/system_service_interface.py
--rw-r--r--   0        0        0      146 2023-04-21 06:38:37.130694 chronus-0.2.3/chronus/domain/system_sample.py
--rw-r--r--   0        0        0      313 2023-02-28 09:33:02.456874 chronus-0.2.3/chronus/example.py
--rw-r--r--   0        0        0        0 2023-04-17 10:32:37.222095 chronus-0.2.3/chronus/model/__init__.py
--rw-r--r--   0        0        0     2092 2023-04-21 06:57:22.994327 chronus-0.2.3/chronus/model/svm.py
--rw-r--r--   0        0        0     3611 2023-04-23 12:37:07.821085 chronus-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    11620 1970-01-01 00:00:00.000000 chronus-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-17 10:23:15.441448 chronus-0.3.0/LICENSE
+-rw-r--r--   0        0        0    10492 2023-05-01 07:12:50.763941 chronus-0.3.0/README.md
+-rw-r--r--   0        0        0        1 2023-05-01 07:12:50.775941 chronus-0.3.0/chronus/SystemIntegration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.0/chronus/SystemIntegration/application_runners/__init__.py
+-rw-r--r--   0        0        0     6026 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/application_runners/hpcg.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.0/chronus/SystemIntegration/cpu_info_services/__init__.py
+-rw-r--r--   0        0        0     2714 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
+-rw-r--r--   0        0        0        0 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/optimizers/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
+-rw-r--r--   0        0        0     3672 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/optimizers/linear_regression.py
+-rw-r--r--   0        0        0     2924 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/optimizers/random_tree_forrest.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.0/chronus/SystemIntegration/repositories/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/repositories/csv_repository.py
+-rw-r--r--   0        0        0    14565 2023-05-09 10:46:16.772526 chronus-0.3.0/chronus/SystemIntegration/repositories/sqlite_repository.py
+-rw-r--r--   0        0        0        0 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/settings_interface/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/SystemIntegration/settings_interface/etc_storage.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.0/chronus/SystemIntegration/system_service_interfaces/__init__.py
+-rw-r--r--   0        0        0     1776 2023-05-09 10:40:56.192811 chronus-0.3.0/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
+-rw-r--r--   0        0        0      330 2023-05-01 07:12:50.775941 chronus-0.3.0/chronus/__init__.py
+-rw-r--r--   0        0        0    11706 2023-05-10 08:08:52.739629 chronus-0.3.0/chronus/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.0/chronus/application/__init__.py
+-rw-r--r--   0        0        0     3710 2023-05-09 10:50:44.532362 chronus-0.3.0/chronus/application/benchmark_service.py
+-rw-r--r--   0        0        0     2445 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/application/init_model_service.py
+-rw-r--r--   0        0        0     1323 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/application/load_model_service.py
+-rw-r--r--   0        0        0      602 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/application/run_model_service.py
+-rw-r--r--   0        0        0        0 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/cli/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/cli/setup.py
+-rw-r--r--   0        0        0      197 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/domain/LocalSettings.py
+-rw-r--r--   0        0        0     2195 2023-05-08 12:04:31.896346 chronus-0.3.0/chronus/domain/Run.py
+-rw-r--r--   0        0        0        0 2023-05-01 07:12:50.775941 chronus-0.3.0/chronus/domain/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-07 22:50:34.284001 chronus-0.3.0/chronus/domain/benchmark.py
+-rw-r--r--   0        0        0     1181 2023-05-08 10:54:40.239867 chronus-0.3.0/chronus/domain/configuration.py
+-rw-r--r--   0        0        0      523 2023-05-08 10:51:57.287969 chronus-0.3.0/chronus/domain/cpu_info.py
+-rw-r--r--   0        0        0        0 2023-05-01 07:12:50.775941 chronus-0.3.0/chronus/domain/interfaces/__init__.py
+-rw-r--r--   0        0        0      520 2023-05-07 22:50:34.288001 chronus-0.3.0/chronus/domain/interfaces/application_runner_interface.py
+-rw-r--r--   0        0        0      158 2023-05-07 22:50:34.288001 chronus-0.3.0/chronus/domain/interfaces/cpu_info_service_interface.py
+-rw-r--r--   0        0        0      918 2023-05-07 22:50:34.288001 chronus-0.3.0/chronus/domain/interfaces/optimizer_interface.py
+-rw-r--r--   0        0        0      986 2023-05-07 22:50:34.288001 chronus-0.3.0/chronus/domain/interfaces/repository_interface.py
+-rw-r--r--   0        0        0      499 2023-05-07 22:50:34.288001 chronus-0.3.0/chronus/domain/interfaces/settings_interface.py
+-rw-r--r--   0        0        0      160 2023-05-07 22:50:34.288001 chronus-0.3.0/chronus/domain/interfaces/system_service_interface.py
+-rw-r--r--   0        0        0      274 2023-05-07 22:50:34.288001 chronus-0.3.0/chronus/domain/model.py
+-rw-r--r--   0        0        0      369 2023-05-09 10:40:55.824811 chronus-0.3.0/chronus/domain/system_sample.py
+-rw-r--r--   0        0        0     3712 2023-05-10 08:08:54.103626 chronus-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12208 1970-01-01 00:00:00.000000 chronus-0.3.0/setup.py
+-rw-r--r--   0        0        0    11709 1970-01-01 00:00:00.000000 chronus-0.3.0/PKG-INFO
```

### Comparing `chronus-0.2.3/LICENSE` & `chronus-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chronus-0.2.3/README.md` & `chronus-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 </div>
 
 ## 📖 About
 This is both a library and a CLI application for scheduling energy consumption. The library is build for slurm, and the CLI application is build for the end user.
 
 ## 🚀 Installation
 ```
-dnf install chronus
+python3 -m pip install chronus
 chronus --help
 ```
 
 ### Poetry
 
 Want to know more about Poetry? Check [its documentation](https://python-poetry.org/docs/).
```

### Comparing `chronus-0.2.3/chronus/domain/configuration.py` & `chronus-0.3.0/chronus/domain/configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 from typing import List
 
 from dataclasses import dataclass
 
+import dataclasses_json
+
+from chronus.domain.cpu_info import SystemInfo
+
 
 @dataclass
 class Configuration:
-    cores: int
-    frequency: float
+    cores: int = 0
+    frequency: int = 0
+    threads_per_core: int = 0
 
 
 def make_core_interval(cores_number: int):
     cores = []
     counter = 1
     while counter <= cores_number:
         cores.append(counter)
         counter *= 2
 
     return cores
 
 
-def make_configurations(cores_number: int, frequencies: List[float]):
-    cores = make_core_interval(cores_number)
+def make_configurations(cpu_info: SystemInfo) -> list[Configuration]:
+    cores = make_core_interval(cpu_info.cores)
 
     configurations = []
     for core in cores:
-        for frequency in frequencies:
-            configurations.append(Configuration(core, frequency))
+        for thread in range(1, cpu_info.threads_per_core + 1):
+            for frequency in cpu_info.frequencies:
+                configurations.append(Configuration(core, frequency, thread))
     return configurations
 
 
+@dataclasses_json.dataclass_json
 class Configurations:
-    def __init__(self, cores: int, frequencies: List[float]):
-        self.__configurations = make_configurations(cores, frequencies)
+    def __init__(self, cpu_info: SystemInfo):
+        self.__configurations = make_configurations(cpu_info)
 
     def __iter__(self):
         return iter(self.__configurations)
 
     def __len__(self):
         return len(self.__configurations)
```

### Comparing `chronus-0.2.3/pyproject.toml` & `chronus-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "chronus"
-version = "0.2.3"
+version = "0.3.0"
 description = "A energy scheduling model, build for HPC."
 readme = "README.md"
 authors = ["chronus <aaspringborg@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/AndersSpringborg/chronus"
 homepage = "https://github.com/AndersSpringborg/chronus"
 
@@ -30,19 +30,24 @@
 [tool.poetry.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "chronus" = "chronus.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
-typer = {extras = ["all"], version = "^0.4.0"}
-rich = "^10.14.0"
+typer = {extras = ["all"], version = "^0.7.0"}
+rich = "^12.6.0"
 scikit-learn = "^1.2.1"
 matplotlib = "^3.7.1"
 dataclasses-json = "^0.5.7"
+pyghmi = "^1.5.61"
+psutil = "^5.9.5"
+
+[tool.poetry.group.model_create.dependencies]
+pandas = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = {version = "^23.3.0", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.12.0"}
 mypy = "^1.2.0"
```

### Comparing `chronus-0.2.3/PKG-INFO` & `chronus-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chronus
-Version: 0.2.3
+Version: 0.3.0
 Summary: A energy scheduling model, build for HPC.
 Home-page: https://github.com/AndersSpringborg/chronus
 License: MIT
 Author: chronus
 Author-email: aaspringborg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,17 +16,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: rich (>=10.14.0,<11.0.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Requires-Dist: pyghmi (>=1.5.61,<2.0.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
-Requires-Dist: typer[all] (>=0.4.0,<0.5.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/AndersSpringborg/chronus
 Description-Content-Type: text/markdown
 
 # chronus
 
 <div style="text-align: center">
   <img src="https://raw.githubusercontent.com/AndersSpringborg/chronus/main/assets/images/logo.png" alt="Chronus greek god head coin isometric concept, transparent background, aspect ration 1:1" width="400" height="400">
@@ -49,15 +51,15 @@
 </div>
 
 ## 📖 About
 This is both a library and a CLI application for scheduling energy consumption. The library is build for slurm, and the CLI application is build for the end user.
 
 ## 🚀 Installation
 ```
-dnf install chronus
+python3 -m pip install chronus
 chronus --help
 ```
 
 ### Poetry
 
 Want to know more about Poetry? Check [its documentation](https://python-poetry.org/docs/).
```

