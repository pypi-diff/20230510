# Comparing `tmp/hyperfetch-1.1.0.tar.gz` & `tmp/hyperfetch-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfetch-1.1.0.tar", last modified: Mon May  8 16:02:57 2023, max compression
+gzip compressed data, was "hyperfetch-1.1.1.tar", last modified: Wed May 10 15:36:57 2023, max compression
```

## Comparing `hyperfetch-1.1.0.tar` & `hyperfetch-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 16:02:57.916342 hyperfetch-1.1.0/
--rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     7281 2023-05-08 16:02:57.916342 hyperfetch-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4916 2023-05-08 16:01:58.000000 hyperfetch-1.1.0/README.md
--rw-rw-rw-   0        0        0     1615 2023-05-08 16:02:31.000000 hyperfetch-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 16:02:57.916342 hyperfetch-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 16:02:57.879988 hyperfetch-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 16:02:57.887355 hyperfetch-1.1.0/src/hyperfetch/
--rw-rw-rw-   0        0        0        0 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/__init__.py
--rw-rw-rw-   0        0        0    10569 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/alg_samplers.py
--rw-rw-rw-   0        0        0      654 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/auth_connection.py
--rw-rw-rw-   0        0        0     1934 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/callbacks.py
--rw-rw-rw-   0        0        0    33572 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/manager.py
--rw-rw-rw-   0        0        0     4994 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/tuning.py
--rw-rw-rw-   0        0        0     1183 2023-05-08 15:20:59.000000 hyperfetch-1.1.0/src/hyperfetch/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 16:02:57.915425 hyperfetch-1.1.0/src/hyperfetch.egg-info/
--rw-rw-rw-   0        0        0     7281 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      261 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 16:02:57.000000 hyperfetch-1.1.0/src/hyperfetch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 15:36:57.914463 hyperfetch-1.1.1/
+-rw-rw-rw-   0        0        0     1317 2023-04-14 16:09:58.000000 hyperfetch-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7386 2023-05-10 15:36:57.914463 hyperfetch-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4990 2023-05-10 15:29:45.000000 hyperfetch-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1643 2023-05-10 15:36:31.000000 hyperfetch-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 15:36:57.914463 hyperfetch-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 15:36:57.868984 hyperfetch-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:36:57.876986 hyperfetch-1.1.1/src/hyperfetch/
+-rw-rw-rw-   0        0        0        0 2023-05-10 15:20:46.000000 hyperfetch-1.1.1/src/hyperfetch/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-05-10 15:20:46.000000 hyperfetch-1.1.1/src/hyperfetch/alg_samplers.py
+-rw-rw-rw-   0        0        0      654 2023-05-10 15:20:46.000000 hyperfetch-1.1.1/src/hyperfetch/auth_connection.py
+-rw-rw-rw-   0        0        0     1934 2023-05-10 15:20:46.000000 hyperfetch-1.1.1/src/hyperfetch/callbacks.py
+-rw-rw-rw-   0        0        0    33572 2023-05-10 15:20:46.000000 hyperfetch-1.1.1/src/hyperfetch/manager.py
+-rw-rw-rw-   0        0        0     4994 2023-05-10 15:20:46.000000 hyperfetch-1.1.1/src/hyperfetch/tuning.py
+-rw-rw-rw-   0        0        0     1183 2023-05-10 15:20:46.000000 hyperfetch-1.1.1/src/hyperfetch/util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:36:57.912462 hyperfetch-1.1.1/src/hyperfetch.egg-info/
+-rw-rw-rw-   0        0        0     7386 2023-05-10 15:36:57.000000 hyperfetch-1.1.1/src/hyperfetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-05-10 15:36:57.000000 hyperfetch-1.1.1/src/hyperfetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 15:36:57.000000 hyperfetch-1.1.1/src/hyperfetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-05-10 15:36:57.000000 hyperfetch-1.1.1/src/hyperfetch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      261 2023-05-10 15:36:57.000000 hyperfetch-1.1.1/src/hyperfetch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-10 15:36:57.000000 hyperfetch-1.1.1/src/hyperfetch.egg-info/top_level.txt
```

### Comparing `hyperfetch-1.1.0/LICENSE` & `hyperfetch-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.1.0/PKG-INFO` & `hyperfetch-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.1.0
-Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application. Currently only available on Linux.
+Version: 1.1.1
+Summary: A tool to optimize and post hyperparameters for your reinforcement learning application. Currently available on Linux and macOS.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, 
@@ -28,30 +28,34 @@
 Project-URL: Website, https://www.hyperfetch.online/
 Project-URL: Source, https://github.com/karolisw/hyperFetch
 Keywords: reinforcement learning,hyperparameters,replication
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: FastAPI
 Requires-Python: <3.11.0,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HyperFetch
 
 #### Prerequisistes 
-Has been tested with Linux and MacOS with these prerequisites:
+The package has been successfully tested with Linux and MacOS.\
+However, these are the prerequisites:
 - pip==22.2.2
 - setuptools==64.0.3
 - swig==4.0.2
 - box2d-py==2.3.8
 
+NB: If you are able to install box2d-py==2.3.8 on your Windows computer, then the installation will likely succeed 
+there as well.
 
 #### HyperFetch is a tool consisting of:
 - A [website](https://www.hyperfetch.online/) for fetching hyperparameters that are tuned by others
 - This pip-module for tuning and saving hyperparameters yourself 
 
 #### The intention of HyperFetch is to:
 - Make recreation of existing projects easier within the 
@@ -63,52 +67,48 @@
 By posting tuned [algorithm x environment] combinations to the website it's expected that:
 - Developers/Students can access hyperparameters that have already been optimially tuned instead of having to tune them themselves.
 - Researchers can filter by project on the website and access hyperparameters they wish to recreate/replicate for their own research.
 - Transparancy related to emissions will become more mainstream within the field.
 
 
 ## Content
-* [Links](#links)
-* 1.0 [Using the pip module](#using-the-pip-module)
-* 2.0 [Examples](#example-1--tuning--posting-using-hyperfetch)
+* 1.0 [Using this package](#using-the-pip-module)
+* 2.0 [Examples of use](#example-1--tuning--posting-using-hyperfetch)
 
 
 ## Links
 Repository: [HyperFetch Github](https://github.com/karolisw/hyperFetch)\
 Documentation: [Configuration docs](https://www.hyperfetch.online/configDocs)\
 Website: [hyperfetch.online](https://www.hyperfetch.online/)
-## Using the pip module
-To use the pip model please do the following:
+## Using this package
+To use this package please do the following:
 
 1. Create a virtual environment in your favorite IDE. 
 
    Install virtualenv if you haven't 
    
            pip install virtualenv
    
    Create a virtual environment
    
            virtualenv [some_name]
 
    Activate virtualenv this way (Linux/MacOS):
    
             source myvenv/bin/activate
-2. Install the pip-module. 
+2. Install the [prerequisites](#prerequisistes).
+3. Install the pip-module. 
 
         pip install hyperfetch
 
 
          
-## Example 1: tuning + posting using HyperFetch
+## Example 1: tuning + posting 
 Here is a quick example of how to tune and run PPO in the Pendulum-v1 environment inside your new or existing project:
 
-### Just a reminder:
-The pip package must be installed before this can be done.
-For details, see [using the pip module](#using-the-pip-module).
-
 ### 1. Create configuration file using YAML (minimal example)
 If you are unsure of which configuration values to use, see the [config docs](https://www.hyperfetch.online/configDocs)
 
 ```yaml
 # Required (example values)
 alg: ppo
 env: Pendulum-v1
@@ -118,15 +118,15 @@
 # Some other useful parameters
 sampler: tpe
 tuner: median
 n_trials: 20
 log_folder: logs
 ```
 
-### 2. Tune using python file or the command line
+### 2. Tune and post using python file or the command line
 
 ```python
 
 from hyperfetch import tuning
 
 # Path to your YAML config file 
 config_path = "../some_folder/config_name.yml"
@@ -170,23 +170,23 @@
   learning_rate: 0.0002126832542803243
   learning_starts: 10000
   net_arch: medium
   subsample_steps: 4
   target_update_interval: 1000
   train_freq: 8
   
-# Not required (but appreciated)
+# Not required (but appreciated if you have the data)
 CO2_emissions: 0.78 #kgs
 energy_consumed: 3.27 #kWh
 cpu_model: 12th Gen Intel(R) Core(TM) i5-12500H
 gpu_model: NVIDIA GeForce RTX 3070
-total_time: 0:04:16.842800 # H:M:S:MS
+total_time: 0:04:16.842800 # Format: H:M:S:MS
 ```
 
-### 2. Save/post using python file or command line
+### 2. Post using python file or command line
 
 #### Python file:
 ```python
 
 from hyperfetch import tuning
 
 # Path to your YAML config file
```

### Comparing `hyperfetch-1.1.0/README.md` & `hyperfetch-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # HyperFetch
 
 #### Prerequisistes 
-Has been tested with Linux and MacOS with these prerequisites:
+The package has been successfully tested with Linux and MacOS.\
+However, these are the prerequisites:
 - pip==22.2.2
 - setuptools==64.0.3
 - swig==4.0.2
 - box2d-py==2.3.8
 
+NB: If you are able to install box2d-py==2.3.8 on your Windows computer, then the installation will likely succeed 
+there as well.
 
 #### HyperFetch is a tool consisting of:
 - A [website](https://www.hyperfetch.online/) for fetching hyperparameters that are tuned by others
 - This pip-module for tuning and saving hyperparameters yourself 
 
 #### The intention of HyperFetch is to:
 - Make recreation of existing projects easier within the 
@@ -22,52 +25,48 @@
 By posting tuned [algorithm x environment] combinations to the website it's expected that:
 - Developers/Students can access hyperparameters that have already been optimially tuned instead of having to tune them themselves.
 - Researchers can filter by project on the website and access hyperparameters they wish to recreate/replicate for their own research.
 - Transparancy related to emissions will become more mainstream within the field.
 
 
 ## Content
-* [Links](#links)
-* 1.0 [Using the pip module](#using-the-pip-module)
-* 2.0 [Examples](#example-1--tuning--posting-using-hyperfetch)
+* 1.0 [Using this package](#using-the-pip-module)
+* 2.0 [Examples of use](#example-1--tuning--posting-using-hyperfetch)
 
 
 ## Links
 Repository: [HyperFetch Github](https://github.com/karolisw/hyperFetch)\
 Documentation: [Configuration docs](https://www.hyperfetch.online/configDocs)\
 Website: [hyperfetch.online](https://www.hyperfetch.online/)
-## Using the pip module
-To use the pip model please do the following:
+## Using this package
+To use this package please do the following:
 
 1. Create a virtual environment in your favorite IDE. 
 
    Install virtualenv if you haven't 
    
            pip install virtualenv
    
    Create a virtual environment
    
            virtualenv [some_name]
 
    Activate virtualenv this way (Linux/MacOS):
    
             source myvenv/bin/activate
-2. Install the pip-module. 
+2. Install the [prerequisites](#prerequisistes).
+3. Install the pip-module. 
 
         pip install hyperfetch
 
 
          
-## Example 1: tuning + posting using HyperFetch
+## Example 1: tuning + posting 
 Here is a quick example of how to tune and run PPO in the Pendulum-v1 environment inside your new or existing project:
 
-### Just a reminder:
-The pip package must be installed before this can be done.
-For details, see [using the pip module](#using-the-pip-module).
-
 ### 1. Create configuration file using YAML (minimal example)
 If you are unsure of which configuration values to use, see the [config docs](https://www.hyperfetch.online/configDocs)
 
 ```yaml
 # Required (example values)
 alg: ppo
 env: Pendulum-v1
@@ -77,15 +76,15 @@
 # Some other useful parameters
 sampler: tpe
 tuner: median
 n_trials: 20
 log_folder: logs
 ```
 
-### 2. Tune using python file or the command line
+### 2. Tune and post using python file or the command line
 
 ```python
 
 from hyperfetch import tuning
 
 # Path to your YAML config file 
 config_path = "../some_folder/config_name.yml"
@@ -129,23 +128,23 @@
   learning_rate: 0.0002126832542803243
   learning_starts: 10000
   net_arch: medium
   subsample_steps: 4
   target_update_interval: 1000
   train_freq: 8
   
-# Not required (but appreciated)
+# Not required (but appreciated if you have the data)
 CO2_emissions: 0.78 #kgs
 energy_consumed: 3.27 #kWh
 cpu_model: 12th Gen Intel(R) Core(TM) i5-12500H
 gpu_model: NVIDIA GeForce RTX 3070
-total_time: 0:04:16.842800 # H:M:S:MS
+total_time: 0:04:16.842800 # Format: H:M:S:MS
 ```
 
-### 2. Save/post using python file or command line
+### 2. Post using python file or command line
 
 #### Python file:
 ```python
 
 from hyperfetch import tuning
 
 # Path to your YAML config file
```

### Comparing `hyperfetch-1.1.0/pyproject.toml` & `hyperfetch-1.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["hyperfetch"]
 
 [project]
 name = "hyperfetch"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Karoline Sund Wahl", email="karolines.wahl@gmail.com" },
 ]
-description = "HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application. Currently only available on Linux."
+description = "A tool to optimize and post hyperparameters for your reinforcement learning application. Currently available on Linux and macOS."
 readme = "README.md"
 requires-python = ">=3.9, <3.11.0"
 license = {file = "LICENSE"}
 keywords = ["reinforcement learning", "hyperparameters", "replication"]
 
 classifiers = [
       'Development Status :: 3 - Alpha',
       'Intended Audience :: Developers',
       'License :: OSI Approved :: BSD License',
       'Operating System :: POSIX :: Linux',
+      'Operating System :: MacOS',
       'Programming Language :: Python :: 3.9',
       'Programming Language :: Python :: 3.10',
       'Framework :: FastAPI',
 ]
 
 dependencies = [
       'setuptools==64.0.3',
```

### Comparing `hyperfetch-1.1.0/src/hyperfetch/alg_samplers.py` & `hyperfetch-1.1.1/src/hyperfetch/alg_samplers.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.1.0/src/hyperfetch/auth_connection.py` & `hyperfetch-1.1.1/src/hyperfetch/auth_connection.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.1.0/src/hyperfetch/callbacks.py` & `hyperfetch-1.1.1/src/hyperfetch/callbacks.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.1.0/src/hyperfetch/manager.py` & `hyperfetch-1.1.1/src/hyperfetch/manager.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.1.0/src/hyperfetch/tuning.py` & `hyperfetch-1.1.1/src/hyperfetch/tuning.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.1.0/src/hyperfetch/util.py` & `hyperfetch-1.1.1/src/hyperfetch/util.py`

 * *Files identical despite different names*

### Comparing `hyperfetch-1.1.0/src/hyperfetch.egg-info/PKG-INFO` & `hyperfetch-1.1.1/src/hyperfetch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hyperfetch
-Version: 1.1.0
-Summary: HyperFetch. A tool to optimize and fetch hyperparameters for your reinforcement learning application. Currently only available on Linux.
+Version: 1.1.1
+Summary: A tool to optimize and post hyperparameters for your reinforcement learning application. Currently available on Linux and macOS.
 Author-email: Karoline Sund Wahl <karolines.wahl@gmail.com>
 License: Copyright 2023 Karoline Sund Wahl
         
         Redistribution and use in source and binary forms, with or without modification, 
         are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, 
@@ -28,30 +28,34 @@
 Project-URL: Website, https://www.hyperfetch.online/
 Project-URL: Source, https://github.com/karolisw/hyperFetch
 Keywords: reinforcement learning,hyperparameters,replication
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: FastAPI
 Requires-Python: <3.11.0,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HyperFetch
 
 #### Prerequisistes 
-Has been tested with Linux and MacOS with these prerequisites:
+The package has been successfully tested with Linux and MacOS.\
+However, these are the prerequisites:
 - pip==22.2.2
 - setuptools==64.0.3
 - swig==4.0.2
 - box2d-py==2.3.8
 
+NB: If you are able to install box2d-py==2.3.8 on your Windows computer, then the installation will likely succeed 
+there as well.
 
 #### HyperFetch is a tool consisting of:
 - A [website](https://www.hyperfetch.online/) for fetching hyperparameters that are tuned by others
 - This pip-module for tuning and saving hyperparameters yourself 
 
 #### The intention of HyperFetch is to:
 - Make recreation of existing projects easier within the 
@@ -63,52 +67,48 @@
 By posting tuned [algorithm x environment] combinations to the website it's expected that:
 - Developers/Students can access hyperparameters that have already been optimially tuned instead of having to tune them themselves.
 - Researchers can filter by project on the website and access hyperparameters they wish to recreate/replicate for their own research.
 - Transparancy related to emissions will become more mainstream within the field.
 
 
 ## Content
-* [Links](#links)
-* 1.0 [Using the pip module](#using-the-pip-module)
-* 2.0 [Examples](#example-1--tuning--posting-using-hyperfetch)
+* 1.0 [Using this package](#using-the-pip-module)
+* 2.0 [Examples of use](#example-1--tuning--posting-using-hyperfetch)
 
 
 ## Links
 Repository: [HyperFetch Github](https://github.com/karolisw/hyperFetch)\
 Documentation: [Configuration docs](https://www.hyperfetch.online/configDocs)\
 Website: [hyperfetch.online](https://www.hyperfetch.online/)
-## Using the pip module
-To use the pip model please do the following:
+## Using this package
+To use this package please do the following:
 
 1. Create a virtual environment in your favorite IDE. 
 
    Install virtualenv if you haven't 
    
            pip install virtualenv
    
    Create a virtual environment
    
            virtualenv [some_name]
 
    Activate virtualenv this way (Linux/MacOS):
    
             source myvenv/bin/activate
-2. Install the pip-module. 
+2. Install the [prerequisites](#prerequisistes).
+3. Install the pip-module. 
 
         pip install hyperfetch
 
 
          
-## Example 1: tuning + posting using HyperFetch
+## Example 1: tuning + posting 
 Here is a quick example of how to tune and run PPO in the Pendulum-v1 environment inside your new or existing project:
 
-### Just a reminder:
-The pip package must be installed before this can be done.
-For details, see [using the pip module](#using-the-pip-module).
-
 ### 1. Create configuration file using YAML (minimal example)
 If you are unsure of which configuration values to use, see the [config docs](https://www.hyperfetch.online/configDocs)
 
 ```yaml
 # Required (example values)
 alg: ppo
 env: Pendulum-v1
@@ -118,15 +118,15 @@
 # Some other useful parameters
 sampler: tpe
 tuner: median
 n_trials: 20
 log_folder: logs
 ```
 
-### 2. Tune using python file or the command line
+### 2. Tune and post using python file or the command line
 
 ```python
 
 from hyperfetch import tuning
 
 # Path to your YAML config file 
 config_path = "../some_folder/config_name.yml"
@@ -170,23 +170,23 @@
   learning_rate: 0.0002126832542803243
   learning_starts: 10000
   net_arch: medium
   subsample_steps: 4
   target_update_interval: 1000
   train_freq: 8
   
-# Not required (but appreciated)
+# Not required (but appreciated if you have the data)
 CO2_emissions: 0.78 #kgs
 energy_consumed: 3.27 #kWh
 cpu_model: 12th Gen Intel(R) Core(TM) i5-12500H
 gpu_model: NVIDIA GeForce RTX 3070
-total_time: 0:04:16.842800 # H:M:S:MS
+total_time: 0:04:16.842800 # Format: H:M:S:MS
 ```
 
-### 2. Save/post using python file or command line
+### 2. Post using python file or command line
 
 #### Python file:
 ```python
 
 from hyperfetch import tuning
 
 # Path to your YAML config file
```

