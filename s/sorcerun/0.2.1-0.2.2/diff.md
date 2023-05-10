# Comparing `tmp/sorcerun-0.2.1.tar.gz` & `tmp/sorcerun-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.2.1.tar", last modified: Mon May  8 19:34:05 2023, max compression
+gzip compressed data, was "sorcerun-0.2.2.tar", last modified: Wed May 10 21:19:48 2023, max compression
```

## Comparing `sorcerun-0.2.1.tar` & `sorcerun-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:05.477507 sorcerun-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-08 19:33:51.000000 sorcerun-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 19:34:05.477507 sorcerun-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 19:33:51.000000 sorcerun-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:34:05.477507 sorcerun-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-08 19:33:51.000000 sorcerun-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:05.477507 sorcerun-0.2.1/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 19:34:05.000000 sorcerun-0.2.1/sorcerun.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:34:05.477507 sorcerun-0.2.1/sorcerun_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-08 19:33:51.000000 sorcerun-0.2.1/sorcerun_package/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:19:48.158432 sorcerun-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-10 21:19:32.000000 sorcerun-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-10 21:19:48.158432 sorcerun-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-10 21:19:32.000000 sorcerun-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:19:48.158432 sorcerun-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-10 21:19:32.000000 sorcerun-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:19:48.158432 sorcerun-0.2.2/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 21:19:48.000000 sorcerun-0.2.2/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:19:48.158432 sorcerun-0.2.2/sorcerun_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-10 21:19:32.000000 sorcerun-0.2.2/sorcerun_package/sacred_utils.py
```

### Comparing `sorcerun-0.2.1/LICENSE` & `sorcerun-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.1/PKG-INFO` & `sorcerun-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.1
+Version: 0.2.2
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.1/README.md` & `sorcerun-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Sorcerun
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
 
 TODO: add simple example
 
-Regenerate response
-
 # TODO
 
 -   [ ] Utilities to forward ports via ssh
 -   [ ] Grid run utilities via CLI
 -   [ ] More template adapters and generate them via CLI
     -   Specifically something that can track STDOUT and log metrics from STDOUT?
 -   [ ] Cleaner source file and other meta info tracking
```

### Comparing `sorcerun-0.2.1/setup.py` & `sorcerun-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred==0.8.4",
         "pymongo",
         "pyyaml",
```

### Comparing `sorcerun-0.2.1/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.2.2/sorcerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.2.1
+Version: 0.2.2
 License-File: LICENSE
 
 Sorcerun is a command-line interface (CLI) designed to streamline the execution and management of computational experiments. It provides built-in support for MongoDB and Sacred, simplifying experiment setup and deployment. Users can configure experiments with a single adapter function, while Sorcerun handles running, logging, and authentication. Additionally, the CLI allows for easy management of MongoDB servers and integrates with the OmniBoard web dashboard for tracking and visualization. Sorcerun aims to facilitate a more efficient experiment lifecycle for researchers, data scientists, and engineers.
```

### Comparing `sorcerun-0.2.1/sorcerun_package/auth_mongodb_option.py` & `sorcerun-0.2.2/sorcerun_package/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.1/sorcerun_package/cli.py` & `sorcerun-0.2.2/sorcerun_package/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 def sorcerun():
     pass
 
 
 @sorcerun.command()
 @click.argument("python_file", type=click.Path(exists=True, dir_okay=False))
 @click.argument("config_file", type=click.Path(exists=True, dir_okay=False))
-def run(python_file, config_file):
+@click.option("--auth_path", default=AUTH_FILE, help="Path to sorcerun_auth.json file.")
+def run(python_file, config_file, auth_path):
     # Load the adapter function from the provided Python file
     adapter_func = load_adapter_function(python_file)
 
     # Load the config from the provided YAML file
     with open(config_file, "r") as file:
         config = yaml.safe_load(file)
 
     # Run the Sacred experiment with the provided adapter function and config
-    run_sacred_experiment(adapter_func, config)
+    run_sacred_experiment(adapter_func, config, auth_path)
 
 
 @sorcerun.group()
 def mongo():
     pass
```

### Comparing `sorcerun-0.2.1/sorcerun_package/mongodb_utils.py` & `sorcerun-0.2.2/sorcerun_package/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.2.1/sorcerun_package/sacred_utils.py` & `sorcerun-0.2.2/sorcerun_package/sacred_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     spec = importlib.util.spec_from_file_location("adapter_module", python_file)
     adapter_module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(adapter_module)
     adapter_func = adapter_module.adapter
     return adapter_func
 
 
-def run_sacred_experiment(adapter_func, config):
+def run_sacred_experiment(adapter_func, config, auth_path=AUTH_FILE):
     experiment_name = getattr(adapter_func, "experiment_name", "sorcerun_experiment")
     ex = Experiment(experiment_name)
 
-    with open(AUTH_FILE, "r") as f:
+    with open(auth_path, "r") as f:
         auth_data = json.load(f)
 
     observer = MongoObserver(
         url=f"mongodb://{auth_data['client_kwargs']['username']}:{auth_data['client_kwargs']['password']}@{auth_data['client_kwargs']['host']}:{auth_data['client_kwargs']['port']}",
         db_name=auth_data["db_name"],
     )
```

