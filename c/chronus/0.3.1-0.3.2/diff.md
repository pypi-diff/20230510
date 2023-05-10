# Comparing `tmp/chronus-0.3.1.tar.gz` & `tmp/chronus-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronus-0.3.1.tar", max compression
+gzip compressed data, was "chronus-0.3.2.tar", max compression
```

## Comparing `chronus-0.3.1.tar` & `chronus-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0     1072 2023-02-17 10:23:15.441448 chronus-0.3.1/LICENSE
--rw-r--r--   0        0        0    10492 2023-05-01 07:12:50.763941 chronus-0.3.1/README.md
--rw-r--r--   0        0        0        1 2023-05-01 07:12:50.775941 chronus-0.3.1/chronus/SystemIntegration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.1/chronus/SystemIntegration/application_runners/__init__.py
--rw-r--r--   0        0        0     6026 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/SystemIntegration/application_runners/hpcg.py
--rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.1/chronus/SystemIntegration/cpu_info_services/__init__.py
--rw-r--r--   0        0        0     2714 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
--rw-r--r--   0        0        0        0 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/SystemIntegration/optimizers/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
--rw-r--r--   0        0        0     3672 2023-05-10 08:30:13.617033 chronus-0.3.1/chronus/SystemIntegration/optimizers/linear_regression.py
--rw-r--r--   0        0        0     2924 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/SystemIntegration/optimizers/random_tree_forrest.py
--rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.1/chronus/SystemIntegration/repositories/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/SystemIntegration/repositories/csv_repository.py
--rw-r--r--   0        0        0    14565 2023-05-09 10:46:16.772526 chronus-0.3.1/chronus/SystemIntegration/repositories/sqlite_repository.py
--rw-r--r--   0        0        0        0 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/SystemIntegration/settings_interface/__init__.py
--rw-r--r--   0        0        0     1285 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/SystemIntegration/settings_interface/etc_storage.py
--rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.1/chronus/SystemIntegration/system_service_interfaces/__init__.py
--rw-r--r--   0        0        0     1776 2023-05-09 10:40:56.192811 chronus-0.3.1/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
--rw-r--r--   0        0        0      330 2023-05-01 07:12:50.775941 chronus-0.3.1/chronus/__init__.py
--rw-r--r--   0        0        0    11688 2023-05-10 08:30:46.776967 chronus-0.3.1/chronus/__main__.py
--rw-r--r--   0        0        0        0 2023-05-03 06:50:47.335685 chronus-0.3.1/chronus/application/__init__.py
--rw-r--r--   0        0        0     3710 2023-05-09 10:50:44.532362 chronus-0.3.1/chronus/application/benchmark_service.py
--rw-r--r--   0        0        0     2445 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/application/init_model_service.py
--rw-r--r--   0        0        0     1323 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/application/load_model_service.py
--rw-r--r--   0        0        0      602 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/application/run_model_service.py
--rw-r--r--   0        0        0        0 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/cli/__init__.py
--rw-r--r--   0        0        0      742 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/cli/setup.py
--rw-r--r--   0        0        0      197 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/domain/LocalSettings.py
--rw-r--r--   0        0        0     2195 2023-05-08 12:04:31.896346 chronus-0.3.1/chronus/domain/Run.py
--rw-r--r--   0        0        0        0 2023-05-01 07:12:50.775941 chronus-0.3.1/chronus/domain/__init__.py
--rw-r--r--   0        0        0      461 2023-05-07 22:50:34.284001 chronus-0.3.1/chronus/domain/benchmark.py
--rw-r--r--   0        0        0     1181 2023-05-08 10:54:40.239867 chronus-0.3.1/chronus/domain/configuration.py
--rw-r--r--   0        0        0      523 2023-05-08 10:51:57.287969 chronus-0.3.1/chronus/domain/cpu_info.py
--rw-r--r--   0        0        0        0 2023-05-01 07:12:50.775941 chronus-0.3.1/chronus/domain/interfaces/__init__.py
--rw-r--r--   0        0        0      520 2023-05-07 22:50:34.288001 chronus-0.3.1/chronus/domain/interfaces/application_runner_interface.py
--rw-r--r--   0        0        0      158 2023-05-07 22:50:34.288001 chronus-0.3.1/chronus/domain/interfaces/cpu_info_service_interface.py
--rw-r--r--   0        0        0      918 2023-05-07 22:50:34.288001 chronus-0.3.1/chronus/domain/interfaces/optimizer_interface.py
--rw-r--r--   0        0        0      986 2023-05-07 22:50:34.288001 chronus-0.3.1/chronus/domain/interfaces/repository_interface.py
--rw-r--r--   0        0        0      499 2023-05-07 22:50:34.288001 chronus-0.3.1/chronus/domain/interfaces/settings_interface.py
--rw-r--r--   0        0        0      160 2023-05-07 22:50:34.288001 chronus-0.3.1/chronus/domain/interfaces/system_service_interface.py
--rw-r--r--   0        0        0      274 2023-05-07 22:50:34.288001 chronus-0.3.1/chronus/domain/model.py
--rw-r--r--   0        0        0      369 2023-05-09 10:40:55.824811 chronus-0.3.1/chronus/domain/system_sample.py
--rw-r--r--   0        0        0     3712 2023-05-10 08:31:05.348930 chronus-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    12208 1970-01-01 00:00:00.000000 chronus-0.3.1/setup.py
--rw-r--r--   0        0        0    11709 1970-01-01 00:00:00.000000 chronus-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-28 08:15:27.618142 chronus-0.3.2/LICENSE
+-rw-r--r--   0        0        0    10492 2023-04-28 10:32:38.218556 chronus-0.3.2/README.md
+-rw-r--r--   0        0        0        1 2023-04-28 08:15:27.622142 chronus-0.3.2/chronus/SystemIntegration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/SystemIntegration/application_runners/__init__.py
+-rw-r--r--   0        0        0     6026 2023-05-06 16:21:47.233103 chronus-0.3.2/chronus/SystemIntegration/application_runners/hpcg.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/SystemIntegration/cpu_info_services/__init__.py
+-rw-r--r--   0        0        0     2714 2023-05-10 09:48:21.426509 chronus-0.3.2/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:33:24.644402 chronus-0.3.2/chronus/SystemIntegration/optimizers/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
+-rw-r--r--   0        0        0     3672 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/optimizers/linear_regression.py
+-rw-r--r--   0        0        0     2924 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/optimizers/random_tree_forrest.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/SystemIntegration/repositories/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-05 17:12:11.384766 chronus-0.3.2/chronus/SystemIntegration/repositories/csv_repository.py
+-rw-r--r--   0        0        0    14565 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/repositories/sqlite_repository.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/settings_interface/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/settings_interface/etc_storage.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/SystemIntegration/system_service_interfaces/__init__.py
+-rw-r--r--   0        0        0     1776 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
+-rw-r--r--   0        0        0      330 2023-04-28 08:15:27.622142 chronus-0.3.2/chronus/__init__.py
+-rw-r--r--   0        0        0    11706 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.2/chronus/application/__init__.py
+-rw-r--r--   0        0        0     3710 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/application/benchmark_service.py
+-rw-r--r--   0        0        0     2445 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/application/init_model_service.py
+-rw-r--r--   0        0        0     1323 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/application/load_model_service.py
+-rw-r--r--   0        0        0      602 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/application/run_model_service.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/cli/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/cli/setup.py
+-rw-r--r--   0        0        0      197 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/LocalSettings.py
+-rw-r--r--   0        0        0     2195 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/Run.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.2/chronus/domain/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/benchmark.py
+-rw-r--r--   0        0        0     1181 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/configuration.py
+-rw-r--r--   0        0        0      523 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/cpu_info.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.2/chronus/domain/interfaces/__init__.py
+-rw-r--r--   0        0        0      520 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/application_runner_interface.py
+-rw-r--r--   0        0        0      158 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/cpu_info_service_interface.py
+-rw-r--r--   0        0        0      918 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/optimizer_interface.py
+-rw-r--r--   0        0        0      986 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/repository_interface.py
+-rw-r--r--   0        0        0      499 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/settings_interface.py
+-rw-r--r--   0        0        0      160 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/interfaces/system_service_interface.py
+-rw-r--r--   0        0        0      274 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/model.py
+-rw-r--r--   0        0        0      369 2023-05-10 09:48:21.430509 chronus-0.3.2/chronus/domain/system_sample.py
+-rw-r--r--   0        0        0     3757 2023-05-10 09:51:42.106451 chronus-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    11796 1970-01-01 00:00:00.000000 chronus-0.3.2/PKG-INFO
```

### Comparing `chronus-0.3.1/LICENSE` & `chronus-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/README.md` & `chronus-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/application_runners/hpcg.py` & `chronus-0.3.2/chronus/SystemIntegration/application_runners/hpcg.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py` & `chronus-0.3.2/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py` & `chronus-0.3.2/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/optimizers/linear_regression.py` & `chronus-0.3.2/chronus/SystemIntegration/optimizers/linear_regression.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/optimizers/random_tree_forrest.py` & `chronus-0.3.2/chronus/SystemIntegration/optimizers/random_tree_forrest.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/repositories/csv_repository.py` & `chronus-0.3.2/chronus/SystemIntegration/repositories/csv_repository.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/repositories/sqlite_repository.py` & `chronus-0.3.2/chronus/SystemIntegration/repositories/sqlite_repository.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/settings_interface/etc_storage.py` & `chronus-0.3.2/chronus/SystemIntegration/settings_interface/etc_storage.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py` & `chronus-0.3.2/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/__main__.py` & `chronus-0.3.2/chronus/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from chronus.domain.configuration import Configuration
 from chronus.domain.interfaces.optimizer_interface import OptimizerInterface
 from chronus.domain.interfaces.repository_interface import RepositoryInterface
 from chronus.domain.interfaces.settings_interface import Permission
 from chronus.SystemIntegration.application_runners.hpcg import HpcgService
 from chronus.SystemIntegration.cpu_info_services.cpu_info_service import LsCpuInfoService
 from chronus.SystemIntegration.optimizers.bruteforce_optmizer import BruteForceOptimizer
+from chronus.SystemIntegration.optimizers.linear_regression import LinearRegressionOptimizer
+from chronus.SystemIntegration.optimizers.random_tree_forrest import RandomTreeOptimizer
 from chronus.SystemIntegration.repositories.sqlite_repository import SqliteRepository
 from chronus.SystemIntegration.settings_interface.etc_storage import EtcLocalStorage
 from chronus.SystemIntegration.system_service_interfaces.ipmi_system_service import (
     IpmiSystemService,
 )
 
 name = "chronus"
@@ -121,21 +123,19 @@
 ) -> None:
     if debug:
         logger.setLevel(logging.DEBUG)
 
 
 class Model(str, Enum):
     brute_force = BruteForceOptimizer.name()
-    linear_regression = "linear-regression"
-    random_tree = "random-tree"
+    linear_regression = LinearRegressionOptimizer.name()
+    random_tree = RandomTreeOptimizer.name()
 
 
 def _choose_optimizer(model: str) -> OptimizerInterface:
-    from chronus.SystemIntegration.optimizers.linear_regression import LinearRegressionOptimizer
-    from chronus.SystemIntegration.optimizers.random_tree_forrest import RandomTreeOptimizer
     switcher = {
         BruteForceOptimizer.name(): BruteForceOptimizer(),
         LinearRegressionOptimizer.name(): LinearRegressionOptimizer(),
         RandomTreeOptimizer.name(): RandomTreeOptimizer(),
     }
     return switcher.get(model, BruteForceOptimizer())
```

### Comparing `chronus-0.3.1/chronus/application/benchmark_service.py` & `chronus-0.3.2/chronus/application/benchmark_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/application/init_model_service.py` & `chronus-0.3.2/chronus/application/init_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/application/load_model_service.py` & `chronus-0.3.2/chronus/application/load_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/application/run_model_service.py` & `chronus-0.3.2/chronus/application/run_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/cli/setup.py` & `chronus-0.3.2/chronus/cli/setup.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/domain/Run.py` & `chronus-0.3.2/chronus/domain/Run.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/domain/configuration.py` & `chronus-0.3.2/chronus/domain/configuration.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/domain/cpu_info.py` & `chronus-0.3.2/chronus/domain/cpu_info.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/domain/interfaces/application_runner_interface.py` & `chronus-0.3.2/chronus/domain/interfaces/application_runner_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/domain/interfaces/optimizer_interface.py` & `chronus-0.3.2/chronus/domain/interfaces/optimizer_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/chronus/domain/interfaces/repository_interface.py` & `chronus-0.3.2/chronus/domain/interfaces/repository_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.1/pyproject.toml` & `chronus-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "chronus"
-version = "0.3.1"
+version = "0.3.2"
 description = "A energy scheduling model, build for HPC."
 readme = "README.md"
 authors = ["chronus <aaspringborg@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/AndersSpringborg/chronus"
 homepage = "https://github.com/AndersSpringborg/chronus"
 
@@ -37,17 +37,18 @@
 typer = {extras = ["all"], version = "^0.7.0"}
 rich = "^12.6.0"
 scikit-learn = "^1.2.1"
 matplotlib = "^3.7.1"
 dataclasses-json = "^0.5.7"
 pyghmi = "^1.5.61"
 psutil = "^5.9.5"
+pandas = { version = "^2.0.1", extras = ["model"], optional = true }
 
-[tool.poetry.group.model_create.dependencies]
-pandas = "^2.0.1"
+[tool.poetry.extras]
+model = ["pandas"]
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = {version = "^23.3.0", allow-prereleases = true}
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.12.0"}
 mypy = "^1.2.0"
```

### Comparing `chronus-0.3.1/setup.py` & `chronus-0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,389 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: chronus
+Version: 0.3.2
+Summary: A energy scheduling model, build for HPC.
+Home-page: https://github.com/AndersSpringborg/chronus
+License: MIT
+Author: chronus
+Author-email: aaspringborg@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: model
+Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: pandas[model] (>=2.0.1,<3.0.0) ; extra == "model"
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Requires-Dist: pyghmi (>=1.5.61,<2.0.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Project-URL: Repository, https://github.com/AndersSpringborg/chronus
+Description-Content-Type: text/markdown
 
-packages = \
-['chronus',
- 'chronus.SystemIntegration',
- 'chronus.SystemIntegration.application_runners',
- 'chronus.SystemIntegration.cpu_info_services',
- 'chronus.SystemIntegration.optimizers',
- 'chronus.SystemIntegration.repositories',
- 'chronus.SystemIntegration.settings_interface',
- 'chronus.SystemIntegration.system_service_interfaces',
- 'chronus.application',
- 'chronus.cli',
- 'chronus.domain',
- 'chronus.domain.interfaces']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['dataclasses-json>=0.5.7,<0.6.0',
- 'matplotlib>=3.7.1,<4.0.0',
- 'psutil>=5.9.5,<6.0.0',
- 'pyghmi>=1.5.61,<2.0.0',
- 'rich>=12.6.0,<13.0.0',
- 'scikit-learn>=1.2.1,<2.0.0',
- 'typer[all]>=0.7.0,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['chronus = chronus.__main__:app']}
-
-setup_kwargs = {
-    'name': 'chronus',
-    'version': '0.3.1',
-    'description': 'A energy scheduling model, build for HPC.',
-    'long_description': '# chronus\n\n<div style="text-align: center">\n  <img src="https://raw.githubusercontent.com/AndersSpringborg/chronus/main/assets/images/logo.png" alt="Chronus greek god head coin isometric concept, transparent background, aspect ration 1:1" width="400" height="400">\n</div>\n<p style="text-align: center"> A energy scheduling model, build for HPC.</p>\n<div style="text-align: center;">\n\n[![Build status](https://github.com/AndersSpringborg/chronus/workflows/build/badge.svg?branch=master&event=push)](https://github.com/AndersSpringborg/chronus/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/chronus.svg)](https://pypi.org/project/chronus/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/AndersSpringborg/chronus/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/AndersSpringborg/chronus/blob/master/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/AndersSpringborg/chronus/releases)\n[![License](https://img.shields.io/github/license/AndersSpringborg/chronus)](https://github.com/AndersSpringborg/chronus/blob/master/LICENSE)\n![Coverage Report](assets/images/coverage.svg)\n\n\n</div>\n\n## 📖 About\nThis is both a library and a CLI application for scheduling energy consumption. The library is build for slurm, and the CLI application is build for the end user.\n\n## 🚀 Installation\n```\npython3 -m pip install chronus\nchronus --help\n```\n\n### Poetry\n\nWant to know more about Poetry? Check [its documentation](https://python-poetry.org/docs/).\n\n<details>\n<summary>Details about Poetry</summary>\n<p>\n\nPoetry\'s [commands](https://python-poetry.org/docs/cli/#commands) are very intuitive and easy to learn, like:\n\n- `poetry add numpy@latest`\n- `poetry run pytest`\n- `poetry publish --build`\n\netc\n</p>\n</details>\n\n### Building and releasing your package\n\nBuilding a new version of the application contains steps:\n\n- Bump the version of your package `poetry version <version>`. You can pass the new version explicitly, or a rule such as `major`, `minor`, or `patch`. For more details, refer to the [Semantic Versions](https://semver.org/) standard.\n- Make a commit to `GitHub`.\n- Create a `GitHub release`.\n- And... publish 🙂 `poetry publish --build`\n\n## 🎯 What\'s next\n\nWell, that\'s up to you 💪🏻. I can only recommend the packages and articles that helped me.\n\n- [`Typer`](https://github.com/tiangolo/typer) is great for creating CLI applications.\n- [`Rich`](https://github.com/willmcgugan/rich) makes it easy to add beautiful formatting in the terminal.\n- [`Pydantic`](https://github.com/samuelcolvin/pydantic/) – data validation and settings management using Python type hinting.\n- [`Loguru`](https://github.com/Delgan/loguru) makes logging (stupidly) simple.\n- [`tqdm`](https://github.com/tqdm/tqdm) – fast, extensible progress bar for Python and CLI.\n- [`IceCream`](https://github.com/gruns/icecream) is a little library for sweet and creamy debugging.\n- [`orjson`](https://github.com/ijl/orjson) – ultra fast JSON parsing library.\n- [`Returns`](https://github.com/dry-python/returns) makes you function\'s output meaningful, typed, and safe!\n- [`Hydra`](https://github.com/facebookresearch/hydra) is a framework for elegantly configuring complex applications.\n- [`FastAPI`](https://github.com/tiangolo/fastapi) is a type-driven asynchronous web framework.\n\nArticles:\n\n- [Open Source Guides](https://opensource.guide/).\n- [A handy guide to financial support for open source](https://github.com/nayafia/lemonade-stand)\n- [GitHub Actions Documentation](https://help.github.com/en/actions).\n- Maybe you would like to add [gitmoji](https://gitmoji.carloscuesta.me/) to commit names. This is really funny. 😄\n\n## 🚀 Features\n\n### Development features\n\n- Supports for `Python 3.9` and higher.\n- [`Poetry`](https://python-poetry.org/) as the dependencies manager. See configuration in [`pyproject.toml`](https://github.com/AndersSpringborg/chronus/blob/master/pyproject.toml) and [`setup.cfg`](https://github.com/AndersSpringborg/chronus/blob/master/setup.cfg).\n- Automatic codestyle with [`black`](https://github.com/psf/black), [`isort`](https://github.com/timothycrosley/isort) and [`pyupgrade`](https://github.com/asottile/pyupgrade).\n- Ready-to-use [`pre-commit`](https://pre-commit.com/) hooks with code-formatting.\n- Type checks with [`mypy`](https://mypy.readthedocs.io); docstring checks with [`darglint`](https://github.com/terrencepreilly/darglint); security checks with [`safety`](https://github.com/pyupio/safety) and [`bandit`](https://github.com/PyCQA/bandit)\n- Testing with [`pytest`](https://docs.pytest.org/en/latest/).\n- Ready-to-use [`.editorconfig`](https://github.com/AndersSpringborg/chronus/blob/master/.editorconfig), [`.dockerignore`](https://github.com/AndersSpringborg/chronus/blob/master/.dockerignore), and [`.gitignore`](https://github.com/AndersSpringborg/chronus/blob/master/.gitignore). You don\'t have to worry about those things.\n\n## Installation\n\n```bash\npip install -U chronus\n```\n\nor install with `Poetry`\n\n```bash\npoetry add chronus\n```\n\nThen you can run\n\n```bash\nchronus --help\n```\n\nor with `Poetry`:\n\n```bash\npoetry run chronus --help\n```\n\n### Makefile usage\n\n[`Makefile`](https://github.com/AndersSpringborg/chronus/blob/master/Makefile) contains a lot of functions for faster development.\n\n<details>\n<summary>1. Download and remove Poetry</summary>\n<p>\n\nTo download and install Poetry run:\n\n```bash\nmake poetry-download\n```\n\nTo uninstall\n\n```bash\nmake poetry-remove\n```\n\n</p>\n</details>\n\n<details>\n<summary>2. Install all dependencies and pre-commit hooks</summary>\n<p>\n\nInstall requirements:\n\n```bash\nmake install\n```\n\nPre-commit hooks coulb be installed after `git init` via\n\n```bash\nmake pre-commit-install\n```\n\n</p>\n</details>\n\n<details>\n<summary>3. Codestyle</summary>\n<p>\n\nAutomatic formatting uses `pyupgrade`, `isort` and `black`.\n\n```bash\nmake codestyle\n\n# or use synonym\nmake formatting\n```\n\nCodestyle checks only, without rewriting files:\n\n```bash\nmake check-codestyle\n```\n\n> Note: `check-codestyle` uses `isort`, `black` and `darglint` library\n\nUpdate all dev libraries to the latest version using one comand\n\n```bash\nmake update-dev-deps\n```\n\n<details>\n<summary>4. Code security</summary>\n<p>\n\n```bash\nmake check-safety\n```\n\nThis command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.\n\n```bash\nmake check-safety\n```\n\n</p>\n</details>\n\n</p>\n</details>\n\n<details>\n<summary>5. Type checks</summary>\n<p>\n\nRun `mypy` static type checker\n\n```bash\nmake mypy\n```\n\n</p>\n</details>\n\n<details>\n<summary>6. Tests with coverage badges</summary>\n<p>\n\nRun `pytest`\n\n```bash\nmake test\n```\n\n</p>\n</details>\n\n<details>\n<summary>7. All linters</summary>\n<p>\n\nOf course there is a command to ~~rule~~ run all linters in one:\n\n```bash\nmake lint\n```\n\nthe same as:\n\n```bash\nmake test && make check-codestyle && make mypy && make check-safety\n```\n\n</p>\n</details>\n\n<details>\n<summary>8. Docker</summary>\n<p>\n\n```bash\nmake docker-build\n```\n\nwhich is equivalent to:\n\n```bash\nmake docker-build VERSION=latest\n```\n\nRemove docker image with\n\n```bash\nmake docker-remove\n```\n\nMore information [about docker](https://github.com/AndersSpringborg/chronus/tree/master/docker).\n\n</p>\n</details>\n\n<details>\n<summary>9. Cleanup</summary>\n<p>\nDelete pycache files\n\n```bash\nmake pycache-remove\n```\n\nRemove package build\n\n```bash\nmake build-remove\n```\n\nDelete .DS_STORE files\n\n```bash\nmake dsstore-remove\n```\n\nRemove .mypycache\n\n```bash\nmake mypycache-remove\n```\n\nOr to remove all above run:\n\n```bash\nmake cleanup\n```\n\n</p>\n</details>\n\n## 📈 Releases\n\nYou can see the list of available releases on the [GitHub Releases](https://github.com/AndersSpringborg/chronus/releases) page.\n\nWe follow [Semantic Versions](https://semver.org/) specification.\n\nWe use [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). As pull requests are merged, a draft release is kept up-to-date listing the changes, ready to publish when you’re ready. With the categories option, you can categorize pull requests in release notes using labels.\n\n### List of labels and corresponding titles\n\n|               **Label**               |  **Title in Releases**  |\n| :-----------------------------------: | :---------------------: |\n|       `enhancement`, `feature`        |       🚀 Features       |\n| `bug`, `refactoring`, `bugfix`, `fix` | 🔧 Fixes & Refactoring  |\n|       `build`, `ci`, `testing`        | 📦 Build System & CI/CD |\n|              `breaking`               |   💥 Breaking Changes   |\n|            `documentation`            |    📝 Documentation     |\n|            `dependencies`             | ⬆️ Dependencies updates |\n\nYou can update it in [`release-drafter.yml`](https://github.com/AndersSpringborg/chronus/blob/master/.github/release-drafter.yml).\n\nGitHub creates the `bug`, `enhancement`, and `documentation` labels for you. Dependabot creates the `dependencies` label. Create the remaining labels on the Issues tab of your GitHub repository, when you need them.\n\n## 🛡 License\n\n[![License](https://img.shields.io/github/license/AndersSpringborg/chronus)](https://github.com/AndersSpringborg/chronus/blob/master/LICENSE)\n\nThis project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/AndersSpringborg/chronus/blob/master/LICENSE) for more details.\n\n## 📃 Citation\n\n```bibtex\n@misc{chronus,\n  author = {chronus},\n  title = {A energy scheduling model, build for HPC.},\n  year = {2023},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/AndersSpringborg/chronus}}\n}\n```\n\n## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)\n\nThis project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)\n',
-    'author': 'chronus',
-    'author_email': 'aaspringborg@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/AndersSpringborg/chronus',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
+# chronus
+
+<div style="text-align: center">
+  <img src="https://raw.githubusercontent.com/AndersSpringborg/chronus/main/assets/images/logo.png" alt="Chronus greek god head coin isometric concept, transparent background, aspect ration 1:1" width="400" height="400">
+</div>
+<p style="text-align: center"> A energy scheduling model, build for HPC.</p>
+<div style="text-align: center;">
+
+[![Build status](https://github.com/AndersSpringborg/chronus/workflows/build/badge.svg?branch=master&event=push)](https://github.com/AndersSpringborg/chronus/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/chronus.svg)](https://pypi.org/project/chronus/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/AndersSpringborg/chronus/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/AndersSpringborg/chronus/blob/master/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/AndersSpringborg/chronus/releases)
+[![License](https://img.shields.io/github/license/AndersSpringborg/chronus)](https://github.com/AndersSpringborg/chronus/blob/master/LICENSE)
+![Coverage Report](assets/images/coverage.svg)
+
+
+</div>
+
+## 📖 About
+This is both a library and a CLI application for scheduling energy consumption. The library is build for slurm, and the CLI application is build for the end user.
+
+## 🚀 Installation
+```
+python3 -m pip install chronus
+chronus --help
+```
+
+### Poetry
+
+Want to know more about Poetry? Check [its documentation](https://python-poetry.org/docs/).
+
+<details>
+<summary>Details about Poetry</summary>
+<p>
+
+Poetry's [commands](https://python-poetry.org/docs/cli/#commands) are very intuitive and easy to learn, like:
+
+- `poetry add numpy@latest`
+- `poetry run pytest`
+- `poetry publish --build`
+
+etc
+</p>
+</details>
+
+### Building and releasing your package
+
+Building a new version of the application contains steps:
+
+- Bump the version of your package `poetry version <version>`. You can pass the new version explicitly, or a rule such as `major`, `minor`, or `patch`. For more details, refer to the [Semantic Versions](https://semver.org/) standard.
+- Make a commit to `GitHub`.
+- Create a `GitHub release`.
+- And... publish 🙂 `poetry publish --build`
+
+## 🎯 What's next
+
+Well, that's up to you 💪🏻. I can only recommend the packages and articles that helped me.
+
+- [`Typer`](https://github.com/tiangolo/typer) is great for creating CLI applications.
+- [`Rich`](https://github.com/willmcgugan/rich) makes it easy to add beautiful formatting in the terminal.
+- [`Pydantic`](https://github.com/samuelcolvin/pydantic/) – data validation and settings management using Python type hinting.
+- [`Loguru`](https://github.com/Delgan/loguru) makes logging (stupidly) simple.
+- [`tqdm`](https://github.com/tqdm/tqdm) – fast, extensible progress bar for Python and CLI.
+- [`IceCream`](https://github.com/gruns/icecream) is a little library for sweet and creamy debugging.
+- [`orjson`](https://github.com/ijl/orjson) – ultra fast JSON parsing library.
+- [`Returns`](https://github.com/dry-python/returns) makes you function's output meaningful, typed, and safe!
+- [`Hydra`](https://github.com/facebookresearch/hydra) is a framework for elegantly configuring complex applications.
+- [`FastAPI`](https://github.com/tiangolo/fastapi) is a type-driven asynchronous web framework.
+
+Articles:
+
+- [Open Source Guides](https://opensource.guide/).
+- [A handy guide to financial support for open source](https://github.com/nayafia/lemonade-stand)
+- [GitHub Actions Documentation](https://help.github.com/en/actions).
+- Maybe you would like to add [gitmoji](https://gitmoji.carloscuesta.me/) to commit names. This is really funny. 😄
+
+## 🚀 Features
+
+### Development features
+
+- Supports for `Python 3.9` and higher.
+- [`Poetry`](https://python-poetry.org/) as the dependencies manager. See configuration in [`pyproject.toml`](https://github.com/AndersSpringborg/chronus/blob/master/pyproject.toml) and [`setup.cfg`](https://github.com/AndersSpringborg/chronus/blob/master/setup.cfg).
+- Automatic codestyle with [`black`](https://github.com/psf/black), [`isort`](https://github.com/timothycrosley/isort) and [`pyupgrade`](https://github.com/asottile/pyupgrade).
+- Ready-to-use [`pre-commit`](https://pre-commit.com/) hooks with code-formatting.
+- Type checks with [`mypy`](https://mypy.readthedocs.io); docstring checks with [`darglint`](https://github.com/terrencepreilly/darglint); security checks with [`safety`](https://github.com/pyupio/safety) and [`bandit`](https://github.com/PyCQA/bandit)
+- Testing with [`pytest`](https://docs.pytest.org/en/latest/).
+- Ready-to-use [`.editorconfig`](https://github.com/AndersSpringborg/chronus/blob/master/.editorconfig), [`.dockerignore`](https://github.com/AndersSpringborg/chronus/blob/master/.dockerignore), and [`.gitignore`](https://github.com/AndersSpringborg/chronus/blob/master/.gitignore). You don't have to worry about those things.
+
+## Installation
+
+```bash
+pip install -U chronus
+```
+
+or install with `Poetry`
+
+```bash
+poetry add chronus
+```
+
+Then you can run
+
+```bash
+chronus --help
+```
+
+or with `Poetry`:
+
+```bash
+poetry run chronus --help
+```
+
+### Makefile usage
+
+[`Makefile`](https://github.com/AndersSpringborg/chronus/blob/master/Makefile) contains a lot of functions for faster development.
+
+<details>
+<summary>1. Download and remove Poetry</summary>
+<p>
+
+To download and install Poetry run:
+
+```bash
+make poetry-download
+```
+
+To uninstall
+
+```bash
+make poetry-remove
+```
+
+</p>
+</details>
+
+<details>
+<summary>2. Install all dependencies and pre-commit hooks</summary>
+<p>
+
+Install requirements:
+
+```bash
+make install
+```
+
+Pre-commit hooks coulb be installed after `git init` via
+
+```bash
+make pre-commit-install
+```
+
+</p>
+</details>
+
+<details>
+<summary>3. Codestyle</summary>
+<p>
+
+Automatic formatting uses `pyupgrade`, `isort` and `black`.
+
+```bash
+make codestyle
+
+# or use synonym
+make formatting
+```
+
+Codestyle checks only, without rewriting files:
+
+```bash
+make check-codestyle
+```
+
+> Note: `check-codestyle` uses `isort`, `black` and `darglint` library
+
+Update all dev libraries to the latest version using one comand
+
+```bash
+make update-dev-deps
+```
+
+<details>
+<summary>4. Code security</summary>
+<p>
+
+```bash
+make check-safety
+```
+
+This command launches `Poetry` integrity checks as well as identifies security issues with `Safety` and `Bandit`.
+
+```bash
+make check-safety
+```
+
+</p>
+</details>
+
+</p>
+</details>
+
+<details>
+<summary>5. Type checks</summary>
+<p>
+
+Run `mypy` static type checker
+
+```bash
+make mypy
+```
+
+</p>
+</details>
+
+<details>
+<summary>6. Tests with coverage badges</summary>
+<p>
+
+Run `pytest`
+
+```bash
+make test
+```
+
+</p>
+</details>
+
+<details>
+<summary>7. All linters</summary>
+<p>
+
+Of course there is a command to ~~rule~~ run all linters in one:
+
+```bash
+make lint
+```
+
+the same as:
+
+```bash
+make test && make check-codestyle && make mypy && make check-safety
+```
+
+</p>
+</details>
+
+<details>
+<summary>8. Docker</summary>
+<p>
+
+```bash
+make docker-build
+```
+
+which is equivalent to:
+
+```bash
+make docker-build VERSION=latest
+```
+
+Remove docker image with
+
+```bash
+make docker-remove
+```
+
+More information [about docker](https://github.com/AndersSpringborg/chronus/tree/master/docker).
+
+</p>
+</details>
+
+<details>
+<summary>9. Cleanup</summary>
+<p>
+Delete pycache files
+
+```bash
+make pycache-remove
+```
+
+Remove package build
+
+```bash
+make build-remove
+```
+
+Delete .DS_STORE files
+
+```bash
+make dsstore-remove
+```
+
+Remove .mypycache
+
+```bash
+make mypycache-remove
+```
+
+Or to remove all above run:
+
+```bash
+make cleanup
+```
+
+</p>
+</details>
+
+## 📈 Releases
+
+You can see the list of available releases on the [GitHub Releases](https://github.com/AndersSpringborg/chronus/releases) page.
+
+We follow [Semantic Versions](https://semver.org/) specification.
+
+We use [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). As pull requests are merged, a draft release is kept up-to-date listing the changes, ready to publish when you’re ready. With the categories option, you can categorize pull requests in release notes using labels.
+
+### List of labels and corresponding titles
+
+|               **Label**               |  **Title in Releases**  |
+| :-----------------------------------: | :---------------------: |
+|       `enhancement`, `feature`        |       🚀 Features       |
+| `bug`, `refactoring`, `bugfix`, `fix` | 🔧 Fixes & Refactoring  |
+|       `build`, `ci`, `testing`        | 📦 Build System & CI/CD |
+|              `breaking`               |   💥 Breaking Changes   |
+|            `documentation`            |    📝 Documentation     |
+|            `dependencies`             | ⬆️ Dependencies updates |
+
+You can update it in [`release-drafter.yml`](https://github.com/AndersSpringborg/chronus/blob/master/.github/release-drafter.yml).
+
+GitHub creates the `bug`, `enhancement`, and `documentation` labels for you. Dependabot creates the `dependencies` label. Create the remaining labels on the Issues tab of your GitHub repository, when you need them.
+
+## 🛡 License
+
+[![License](https://img.shields.io/github/license/AndersSpringborg/chronus)](https://github.com/AndersSpringborg/chronus/blob/master/LICENSE)
+
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/AndersSpringborg/chronus/blob/master/LICENSE) for more details.
+
+## 📃 Citation
+
+```bibtex
+@misc{chronus,
+  author = {chronus},
+  title = {A energy scheduling model, build for HPC.},
+  year = {2023},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/AndersSpringborg/chronus}}
 }
+```
+
+## Credits [![🚀 Your next Python package needs a bleeding-edge project structure.](https://img.shields.io/badge/python--package--template-%F0%9F%9A%80-brightgreen)](https://github.com/TezRomacH/python-package-template)
 
+This project was generated with [`python-package-template`](https://github.com/TezRomacH/python-package-template)
 
-setup(**setup_kwargs)
```

