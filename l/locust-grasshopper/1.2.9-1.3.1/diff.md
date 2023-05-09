# Comparing `tmp/locust-grasshopper-1.2.9.tar.gz` & `tmp/locust-grasshopper-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-grasshopper-1.2.9.tar", last modified: Mon May  1 21:35:37 2023, max compression
+gzip compressed data, was "locust-grasshopper-1.3.1.tar", last modified: Tue May  9 22:40:47 2023, max compression
```

## Comparing `locust-grasshopper-1.2.9.tar` & `locust-grasshopper-1.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20359 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-05-01 21:35:20.000000 locust-grasshopper-1.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/configuration/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/configuration/gh_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)    18919 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/grasshopper_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/grasshopper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/journeys/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/journeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6252 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/journeys/base_journey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.156842 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/er_basic_console_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/iextendedreporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/reporter_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/shared_reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/src/grasshopper/lib/util/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      330 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/check_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/launch.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/listeners.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/shapes.py
--rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-05-01 21:35:14.000000 locust-grasshopper-1.2.9/src/grasshopper/lib/util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 21:35:37.160843 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    34308 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-01 21:35:37.000000 locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.375533 locust-grasshopper-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35142 2023-05-09 22:40:47.375533 locust-grasshopper-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21193 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-05-09 22:40:33.000000 locust-grasshopper-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 22:40:47.375533 locust-grasshopper-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.371533 locust-grasshopper-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.371533 locust-grasshopper-1.3.1/src/grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.371533 locust-grasshopper-1.3.1/src/grasshopper/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.371533 locust-grasshopper-1.3.1/src/grasshopper/lib/configuration/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9663 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/configuration/gh_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.371533 locust-grasshopper-1.3.1/src/grasshopper/lib/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)    18919 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/fixtures/grasshopper_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/grasshopper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.371533 locust-grasshopper-1.3.1/src/grasshopper/lib/journeys/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/journeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7769 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/journeys/base_journey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.371533 locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/er_basic_console_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/iextendedreporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/reporter_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/shared_reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.371533 locust-grasshopper-1.3.1/src/grasshopper/lib/util/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      330 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/util/check_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/util/launch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/util/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/util/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/util/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-05-09 22:40:30.000000 locust-grasshopper-1.3.1/src/grasshopper/lib/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 22:40:47.375533 locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    35142 2023-05-09 22:40:47.000000 locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-05-09 22:40:47.000000 locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 22:40:47.000000 locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-09 22:40:47.000000 locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-05-09 22:40:47.000000 locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 22:40:47.000000 locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/top_level.txt
```

### Comparing `locust-grasshopper-1.2.9/LICENSE` & `locust-grasshopper-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/PKG-INFO` & `locust-grasshopper-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.2.9
+Version: 1.3.1
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,15 +235,138 @@
 - [timing thresholds](#thresholds)
 - [streamlined metric reporting/tagging system](#db-reporting)
   (only influxDB is supported right now)
 
 ## Installation
 This package can be installed via pip: `pip install locust-grasshopper`
 
+## Example Load Test
+- You can refer to the test `test_example.py` in the `example` directory for a basic 
+  skeleton of how to get a load test running. In the same directory, there is also an 
+  example `conftest.py` that will show you how to get basic parameterization working.
+- This test can be invoked by running `pytest example/test_example.py` in the root of 
+  this project.
+- This test can also be invoked via a YAML scenario file:
+```shell
+cd example
+pytest example_scenarios.YAML --tags=example1
+```
+ In this example scenario file, you can see how grasshopper_args, 
+ grasshopper_scenario_args, and tags are being set.
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Creating a load test
+When creating a new load test, the primary grasshopper function you will be using 
+is called `Grasshopper.launch_test`. This function can be imported like so: `from grasshopper.lib.grasshopper import Grasshopper`
+`launch_test` takes in a wide variety of args:
+- `user_classes`: User classes that the runner will run. These user classes must 
+  extend BaseJourney, which is a grasshopper class 
+  (`from grasshopper.lib.journeys.base_journey import BaseJourney`). This can be a 
+  single class, a list of classes, or a dictionary where the key is the class and 
+  the value is the locust weight to assign to that class.
+- `**complete_configuration`: In order for the test to have the correct configuration, you 
+  must pass in the kwargs provided by the `complete_configuration` fixture. See example 
+  load test on how to do this properly.
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Scenario Args   
+
+- If you want to parameterize your journey class, you should use the `scenario_args` 
+  dict. This is the proper way to pass in values from outside of 
+  the journey for access by the journey code. Note that each journey gets a 
+  ***copy*** on start, so the journey itself can safely modify its own dictionary 
+  once the test is running.
+  `scenario_args` exists for any journey that extends the grasshopper `base_journey` 
+  class. 
+  `scenario_args` also grabs from `self.defaults` on initialization. For example:
+```python
+from locust import between, task
+from grasshopper.lib.journeys.base_journey import BaseJourney
+from grasshopper.lib.grasshopper import Grasshopper
+
+# a journey class with an example task
+class ExampleJourney(BaseJourney):
+    # number of seconds to wait between each task
+    wait_time = between(min_wait=20, max_wait=30)
+    
+    # this defaults dictionary will be merged into scenario_args with lower precedence 
+    # when the journey is initialized
+    defaults = {
+        "foo": "bar",
+    }
+    
+    @task
+    def example_task:
+        logging.info(f'foo is `{self.scenario_args.get("foo")}`.')
+        
+        # aggregate all metrics for the below request under the name "get google"
+        # if name is not specified, then the full url will be the name of the metric
+        response = self.client.get('https://google.com', name='get google')
+
+# the pytest test which launches the journey class
+def test_run_example_journey(complete_configuration):
+    # update scenario args before initialization
+    ExampleJourney.update_incoming_scenario_args(complete_configuration)
+    
+    # launch the journey
+    locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
+    return locust_env
+```
+<p align="right">(<a href="#top">back to top</a>)</p>
 
+## Commonly used grasshopper pytest arguments
+- `--runtime`: Number of seconds to run each test. Set to 120 by default.
+- `--users`: Max number of users that are spawned. Set to 1 by default.
+- `--spawn_rate` : Number of users to spawn per second. Set to 1 by default.
+- `--shape`: The name of a shape to run for the test. 
+If you don't specify a shape or shape instance, then the shape `Default` will be used, 
+  which just runs with the users, runtime & spawn_rate specified on the command line (or picks up defaults 
+of 1, 1, 120s). See `utils/shapes.py` for available shapes and information on how to add
+your own shapes.
+- `--scenario_file` If you want a yaml file where you pre-define some args, this is how 
+you specify that file path. For example, 
+  `scenario_file=example/scenario_example.YAML`. 
+- `--scenario_name` If `--scenario_file` was specified, this is the scenario name that is 
+within that YAML file that corresponds to the scenario you wish to run. Defaults to None.
+- `--tags` See below example: `Loop through a collection of scenarios that match some 
+  tag`.
+- `--scenario_delay` Adds a delay in seconds between scenarios. Defaults to 0.
+- `--influx_host` If you want to report your performance test metrics to some influxdb, 
+you must specify a host.
+    E.g. `1.1.1.1`. Defaults to None.
+- `--influx_port`: Port for your `influx_host` in the case where it is non-default.
+- `--influx_user`: Username for your `influx_host`, if you have one.
+- `--influx_pwd`: Password for your `influx_host`, if you have one.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Launching tests with a configuration
+All in all, there are a few ways you can actually collect and pass params to a test:
+
+### Run a test with its defaults
+`cd example`
+`pytest test_example.py ...`
+
+### Run a test with a specific scenario
+`cd example`
+`pytest test_example.py --scenario_file=example_scenarios.YAML --scenario_name=example_scenario_1 ...`
+
+### Loop through a collection of scenarios that match some tag
+`cd example`
+`pytest example_scenarios.YAML --tags=smoke ...`
+
+- As shown above, this case involves passing a `.YAML` scenario file into pytest instead of a `.py` file.
+- The `--scenario_file` and `--scenario_name` args will be ignored in this case
+- The `--tags` arg supports AND/OR operators according to the opensource `tag-matcher` package. More info on these operators can be found [here](https://pypi.org/project/tag-matcher/).
+- If no `--tags` arg is specified, then ALL the scenarios in the `.yaml` file will be run.
+- If a value is given for `--scenario_delay`, the test will wait that many seconds between collected scenarios.
+- All scenarios are implicitly tagged with the scenario name to support easily selecting one single
+scenario
+
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Configuring Grasshopper
 <a id="creating"></a>
 
 Grasshopper adds a variety of parameters relating to performance testing along with a
 variety of ways to set these values.
 
@@ -254,27 +377,29 @@
 meaning all existing grasshopper tests should still run without modification. The 
 original fixtures and sources for configuration are deprecated, but still produce the 
 same behavior.
 
 All of the usual [pytest arguments](https://docs.pytest.org/en/6.2.x/usage.html) also remain available.
 
 The rest of the sections on configuration assume you are using `locust-grasshopper>=1.1.1`.
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Sources
 Currently, there are 5 different sources for configuration values and they are, in 
 precedence order 
 
 + command line arguments
 + environment variables
 + scenario values from a scenario yaml file
 + grasshopper configuration file
 + global defaults (currently stored in code, not configurable by consumers)
 
 Obviously, the global defaults defined by Grasshopper are not really a source for
 consumers to modify, but we mention it so values don't seem to appear "out of thin air".
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Categories
 The argument list is getting lengthy, so we've broken it down into categories. These
 categories are entirely for humans: better readability, understanding and ease of use. 
 Once they are all fully loaded by Grasshopper, they will be stored in a single 
 `GHConfiguration` object (`dict`). By definition, every argument is in only one category
 and there is no overlap of keys between the categories. If the same key is supplied in
@@ -288,14 +413,15 @@
 | Scenario    | Session            | Variables that may change per scenario and are often<br/>scenario specific; Includes user defined variables that are<br/>not declared as command line arguments by Grasshopper.<br/>However, you may use pytest's addoptions hook in your <br/>conftest to define them. |
 
 At least one of the sections must be present in the global configuration file and
 eventually this will be the same in the configuration section of a scenario in a scenario 
 yaml file. Categories are not used when specifying environment variables or command line
 options. We recommend that you use these categories in file sources, but if a variable 
 is in the wrong section, it won't actually affect the configuration loading process.
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Using Configuration Values 
 Your test(s) may access the complete merged set of key-value pairs via the session scoped 
 fixture `complete_configuration`. This returns a `GHConfiguration` object (dict) which
 is unique to the current scenario. This value will be re-calculated for each new scenario
 executed.
 
@@ -328,14 +454,16 @@
   users: 1.0
   spawn_rate: 1.0
   runtime: 600
 scenario:
   key1 : 'value1'
   key2: 0
 ```
+<p align="right">(<a href="#top">back to top</a>)</p>
+
 ### Additional Extensions to the configuration loading process
 
 If you would like to include other environment variables that might be present in the
 system, you can define a fixture called `extra_env_var_keys` which returns a list of key
 names to load from the `os.environ`. Keys that are missing in the environment will not 
 be included in the `GHConfiguration` object.
 
@@ -344,131 +472,14 @@
 become zero length after the strip will be discarded. This is a mechanism to include any
 scenario arguments you might like to pass via an environment variable.
 
 In the unlikely case that you need to use a different prefix to designate scenario
 variables, you can define a fixture called `env_var_prefix_key` which returns a prefix
 string. The same rules apply about which values are included in the configuration.
 
-### Commonly used arguments
-- `--runtime`: Number of seconds to run each test. Set to 120 by default.
-- `--users`: Max number of users that are spawned. Set to 1 by default.
-- `--spawn_rate` : Number of users to spawn per second. Set to 1 by default.
-- `--shape`: The name of a shape to run for the test. 
-If you don't specify a shape or shape instance, then the shape `Default` will be used, 
-  which just runs with the users, runtime & spawn_rate specified on the command line (or picks up defaults 
-of 1, 1, 120s). See `utils/shapes.py` for available shapes and information on how to add
-your own shapes.
-- `--scenario_file` If you want a yaml file where you pre-define some args, this is how 
-you specify that file path. For example, 
-  `scenario_file=example/scenario_example.YAML`. 
-- `--scenario_name` If `--scenario_file` was specified, this is the scenario name that is 
-within that YAML file that corresponds to the scenario you wish to run. Defaults to None.
-- `--tags` See below example: `Loop through a collection of scenarios that match some 
-  tag`.
-- `--scenario_delay` Adds a delay in seconds between scenarios. Defaults to 0.
-- `--influx_host` If you want to report your performance test metrics to some influxdb, 
-you must specify a host.
-    E.g. `1.1.1.1`. Defaults to None.
-- `--influx_port`: Port for your `influx_host` in the case where it is non-default.
-- `--influx_user`: Username for your `influx_host`, if you have one.
-- `--influx_pwd`: Password for your `influx_host`, if you have one.
-
-## Launching tests with a configuration
-All in all, there are a few ways you can actually collect and pass params to a test:
-
-### Run a test with its defaults
-`cd example`
-`pytest test_example.py ...`
-
-### Run a test with a specific scenario
-`cd example`
-`pytest test_example.py --scenario_file=example_scenarios.YAML --scenario_name=example_scenario_1 ...`
-
-### Loop through a collection of scenarios that match some tag
-`cd example`
-`pytest example_scenarios.YAML --tags=smoke ...`
-
-- As shown above, this case involves passing a `.YAML` scenario file into pytest instead of a `.py` file.
-- The `--scenario_file` and `--scenario_name` args will be ignored in this case
-- The `--tags` arg supports AND/OR operators according to the opensource `tag-matcher` package. More info on these operators can be found [here](https://pypi.org/project/tag-matcher/).
-- If no `--tags` arg is specified, then ALL the scenarios in the `.yaml` file will be run.
-- If a value is given for `--scenario_delay`, the test will wait that many seconds between collected scenarios.
-- All scenarios are implicitly tagged with the scenario name to support easily selecting one single
-scenario
-
-**Creating a load test **
-When creating a new load test, the primary grasshopper function you will be using 
-is called `Grasshopper.launch_test`. This function can be imported like so: `from grasshopper.lib.grasshopper import Grasshopper`
-`launch_test` takes in a wide variety of args:
-- `user_classes`: User classes that the runner will run. These user classes must 
-  extend BaseJourney, which is a grasshopper class 
-  (`from grasshopper.lib.journeys.base_journey import BaseJourney`). This can be a 
-  list of classes or just a single class.
-- `**complete_configuration`: In order for the test to have the correct configuration, you 
-  must pass in the kwargs provided by the `complete_configuration` fixture. See example 
-  load test on how to do this properly.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-## Example Load Test  
-
-- You can refer to the test `test_example.py` in the `example` directory for a basic 
-  skeleton of how to get a load test running. In the same directory, there is also an 
-  example `conftest.py` that will show you how to get basic parameterization working.
-- This test can be invoked by running `pytest example/test_example.py` in the root of 
-  this project.
-- This test can also be invoked via a YAML scenario file: (`cd example`, `pytest 
-  example_scenarios.YAML --tags=example1`). In this example scenario file, you can 
-  see how grasshopper_args, grasshopper_scenario_args, and tags are being set.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-## Scenario Args   
-
-- If you want to parameterize your journey class, you should use the `scenario_args` 
-  dict. This is the proper way to pass in values from outside of 
-  the journey for access by the journey code. Note that each journey gets a 
-  ***copy*** on start, so the journey itself can safely modify its own dictionary 
-  once the test is running.
-  `scenario_args` exists for any journey that extends the grasshopper `base_journey` 
-  class. 
-  `scenario_args` also grabs from `self.defaults` on initialization. For example:
-```python
-from locust import between, task
-from grasshopper.lib.journeys.base_journey import BaseJourney
-from grasshopper.lib.grasshopper import Grasshopper
-
-# a journey class with an example task
-class ExampleJourney(BaseJourney):
-    # number of seconds to wait between each task
-    wait_time = between(min_wait=20, max_wait=30)
-    
-    # this defaults dictionary will be merged into scenario_args with lower precedence 
-    # when the journey is initialized
-    defaults = {
-        "foo": "bar",
-    }
-    
-    @task
-    def example_task:
-        logging.info(f'foo is `{self.scenario_args.get("foo")}`.')
-        
-        # aggregate all metrics for the below request under the name "get google"
-        # if name is not specified, then the full url will be the name of the metric
-        response = self.client.get('https://google.com', name='get google')
-
-# the pytest test which launches the journey class
-def test_run_example_journey(complete_configuration):
-    # update scenario args before initialization
-    ExampleJourney.update_incoming_scenario_args(complete_configuration)
-    
-    # launch the journey
-    locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
-    return locust_env
-```
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Checks
 <a id="checks"></a>
 Checks are an assertion that is recorded as a metric. 
 They are useful both to ensure your test is working correctly 
 (e.g. are you getting a valid id back from some post that you sent) 
@@ -515,16 +526,16 @@
         )
 ```
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Thresholds
 <a id="thresholds"></a>
 Thresholds are time-based, and can be added to any trend, whether it be a custom 
-trend or a request response time. Thresholds are currently based off of the 90th 
-percentile of timings. Here is an example of using a threshold: 
+trend or a request response time. Thresholds default to the 0.9 percentile of timings. 
+Here is an example of using a threshold: 
 
 ```python
 # a journey class with an example threshold
 from locust import between, task
 from grasshopper.lib.journeys.base_journey import BaseJourney
 from grasshopper.lib.grasshopper import Grasshopper
 
@@ -543,23 +554,34 @@
 
 # the pytest test which launches the journey class, thresholds could be 
 # parameterized here as well.
 def test_run_example_journey(complete_configuration):
     ExampleJourney.update_incoming_scenario_args(complete_configuration)
     ExampleJourney.update_incoming_scenario_args({
         "thresholds": {
-            "{GET}get google": 4000, # 4 second HTTP response threshold
-            "{CUSTOM}my custom trend": 11000 # 11 second custom trend threshold
-            }
-        }) 
+            "get google":
+                {
+                    "type": "get",
+                    "limit": 4000  # 4 second HTTP response threshold
+                },
+            "my custom trend":
+                {
+                    "type": "custom",
+                    "limit": 11000  # 11 second custom trend threshold
+                }
+        }
+    })
     
     locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
     return locust_env
 ```
 
+Thresholds can also be defined for individual YAML scenarios. Refer to the `thresholds` 
+key in `example/example_scenarios.YAML` for how to use thresholds for YAML scenarios.
+
 After a test has concluded, trend/threshold data can be found in 
 `locust_env.stats.trends`. 
 This data is also reported to the console at the end of each test.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Time Series DB Reporting and Tagging
```

### Comparing `locust-grasshopper-1.2.9/README.md` & `locust-grasshopper-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,138 @@
 - [timing thresholds](#thresholds)
 - [streamlined metric reporting/tagging system](#db-reporting)
   (only influxDB is supported right now)
 
 ## Installation
 This package can be installed via pip: `pip install locust-grasshopper`
 
+## Example Load Test
+- You can refer to the test `test_example.py` in the `example` directory for a basic 
+  skeleton of how to get a load test running. In the same directory, there is also an 
+  example `conftest.py` that will show you how to get basic parameterization working.
+- This test can be invoked by running `pytest example/test_example.py` in the root of 
+  this project.
+- This test can also be invoked via a YAML scenario file:
+```shell
+cd example
+pytest example_scenarios.YAML --tags=example1
+```
+ In this example scenario file, you can see how grasshopper_args, 
+ grasshopper_scenario_args, and tags are being set.
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Creating a load test
+When creating a new load test, the primary grasshopper function you will be using 
+is called `Grasshopper.launch_test`. This function can be imported like so: `from grasshopper.lib.grasshopper import Grasshopper`
+`launch_test` takes in a wide variety of args:
+- `user_classes`: User classes that the runner will run. These user classes must 
+  extend BaseJourney, which is a grasshopper class 
+  (`from grasshopper.lib.journeys.base_journey import BaseJourney`). This can be a 
+  single class, a list of classes, or a dictionary where the key is the class and 
+  the value is the locust weight to assign to that class.
+- `**complete_configuration`: In order for the test to have the correct configuration, you 
+  must pass in the kwargs provided by the `complete_configuration` fixture. See example 
+  load test on how to do this properly.
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Scenario Args   
+
+- If you want to parameterize your journey class, you should use the `scenario_args` 
+  dict. This is the proper way to pass in values from outside of 
+  the journey for access by the journey code. Note that each journey gets a 
+  ***copy*** on start, so the journey itself can safely modify its own dictionary 
+  once the test is running.
+  `scenario_args` exists for any journey that extends the grasshopper `base_journey` 
+  class. 
+  `scenario_args` also grabs from `self.defaults` on initialization. For example:
+```python
+from locust import between, task
+from grasshopper.lib.journeys.base_journey import BaseJourney
+from grasshopper.lib.grasshopper import Grasshopper
+
+# a journey class with an example task
+class ExampleJourney(BaseJourney):
+    # number of seconds to wait between each task
+    wait_time = between(min_wait=20, max_wait=30)
+    
+    # this defaults dictionary will be merged into scenario_args with lower precedence 
+    # when the journey is initialized
+    defaults = {
+        "foo": "bar",
+    }
+    
+    @task
+    def example_task:
+        logging.info(f'foo is `{self.scenario_args.get("foo")}`.')
+        
+        # aggregate all metrics for the below request under the name "get google"
+        # if name is not specified, then the full url will be the name of the metric
+        response = self.client.get('https://google.com', name='get google')
+
+# the pytest test which launches the journey class
+def test_run_example_journey(complete_configuration):
+    # update scenario args before initialization
+    ExampleJourney.update_incoming_scenario_args(complete_configuration)
+    
+    # launch the journey
+    locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
+    return locust_env
+```
+<p align="right">(<a href="#top">back to top</a>)</p>
 
+## Commonly used grasshopper pytest arguments
+- `--runtime`: Number of seconds to run each test. Set to 120 by default.
+- `--users`: Max number of users that are spawned. Set to 1 by default.
+- `--spawn_rate` : Number of users to spawn per second. Set to 1 by default.
+- `--shape`: The name of a shape to run for the test. 
+If you don't specify a shape or shape instance, then the shape `Default` will be used, 
+  which just runs with the users, runtime & spawn_rate specified on the command line (or picks up defaults 
+of 1, 1, 120s). See `utils/shapes.py` for available shapes and information on how to add
+your own shapes.
+- `--scenario_file` If you want a yaml file where you pre-define some args, this is how 
+you specify that file path. For example, 
+  `scenario_file=example/scenario_example.YAML`. 
+- `--scenario_name` If `--scenario_file` was specified, this is the scenario name that is 
+within that YAML file that corresponds to the scenario you wish to run. Defaults to None.
+- `--tags` See below example: `Loop through a collection of scenarios that match some 
+  tag`.
+- `--scenario_delay` Adds a delay in seconds between scenarios. Defaults to 0.
+- `--influx_host` If you want to report your performance test metrics to some influxdb, 
+you must specify a host.
+    E.g. `1.1.1.1`. Defaults to None.
+- `--influx_port`: Port for your `influx_host` in the case where it is non-default.
+- `--influx_user`: Username for your `influx_host`, if you have one.
+- `--influx_pwd`: Password for your `influx_host`, if you have one.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Launching tests with a configuration
+All in all, there are a few ways you can actually collect and pass params to a test:
+
+### Run a test with its defaults
+`cd example`
+`pytest test_example.py ...`
+
+### Run a test with a specific scenario
+`cd example`
+`pytest test_example.py --scenario_file=example_scenarios.YAML --scenario_name=example_scenario_1 ...`
+
+### Loop through a collection of scenarios that match some tag
+`cd example`
+`pytest example_scenarios.YAML --tags=smoke ...`
+
+- As shown above, this case involves passing a `.YAML` scenario file into pytest instead of a `.py` file.
+- The `--scenario_file` and `--scenario_name` args will be ignored in this case
+- The `--tags` arg supports AND/OR operators according to the opensource `tag-matcher` package. More info on these operators can be found [here](https://pypi.org/project/tag-matcher/).
+- If no `--tags` arg is specified, then ALL the scenarios in the `.yaml` file will be run.
+- If a value is given for `--scenario_delay`, the test will wait that many seconds between collected scenarios.
+- All scenarios are implicitly tagged with the scenario name to support easily selecting one single
+scenario
+
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Configuring Grasshopper
 <a id="creating"></a>
 
 Grasshopper adds a variety of parameters relating to performance testing along with a
 variety of ways to set these values.
 
@@ -31,27 +154,29 @@
 meaning all existing grasshopper tests should still run without modification. The 
 original fixtures and sources for configuration are deprecated, but still produce the 
 same behavior.
 
 All of the usual [pytest arguments](https://docs.pytest.org/en/6.2.x/usage.html) also remain available.
 
 The rest of the sections on configuration assume you are using `locust-grasshopper>=1.1.1`.
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Sources
 Currently, there are 5 different sources for configuration values and they are, in 
 precedence order 
 
 + command line arguments
 + environment variables
 + scenario values from a scenario yaml file
 + grasshopper configuration file
 + global defaults (currently stored in code, not configurable by consumers)
 
 Obviously, the global defaults defined by Grasshopper are not really a source for
 consumers to modify, but we mention it so values don't seem to appear "out of thin air".
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Categories
 The argument list is getting lengthy, so we've broken it down into categories. These
 categories are entirely for humans: better readability, understanding and ease of use. 
 Once they are all fully loaded by Grasshopper, they will be stored in a single 
 `GHConfiguration` object (`dict`). By definition, every argument is in only one category
 and there is no overlap of keys between the categories. If the same key is supplied in
@@ -65,14 +190,15 @@
 | Scenario    | Session            | Variables that may change per scenario and are often<br/>scenario specific; Includes user defined variables that are<br/>not declared as command line arguments by Grasshopper.<br/>However, you may use pytest's addoptions hook in your <br/>conftest to define them. |
 
 At least one of the sections must be present in the global configuration file and
 eventually this will be the same in the configuration section of a scenario in a scenario 
 yaml file. Categories are not used when specifying environment variables or command line
 options. We recommend that you use these categories in file sources, but if a variable 
 is in the wrong section, it won't actually affect the configuration loading process.
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Using Configuration Values 
 Your test(s) may access the complete merged set of key-value pairs via the session scoped 
 fixture `complete_configuration`. This returns a `GHConfiguration` object (dict) which
 is unique to the current scenario. This value will be re-calculated for each new scenario
 executed.
 
@@ -105,14 +231,16 @@
   users: 1.0
   spawn_rate: 1.0
   runtime: 600
 scenario:
   key1 : 'value1'
   key2: 0
 ```
+<p align="right">(<a href="#top">back to top</a>)</p>
+
 ### Additional Extensions to the configuration loading process
 
 If you would like to include other environment variables that might be present in the
 system, you can define a fixture called `extra_env_var_keys` which returns a list of key
 names to load from the `os.environ`. Keys that are missing in the environment will not 
 be included in the `GHConfiguration` object.
 
@@ -121,131 +249,14 @@
 become zero length after the strip will be discarded. This is a mechanism to include any
 scenario arguments you might like to pass via an environment variable.
 
 In the unlikely case that you need to use a different prefix to designate scenario
 variables, you can define a fixture called `env_var_prefix_key` which returns a prefix
 string. The same rules apply about which values are included in the configuration.
 
-### Commonly used arguments
-- `--runtime`: Number of seconds to run each test. Set to 120 by default.
-- `--users`: Max number of users that are spawned. Set to 1 by default.
-- `--spawn_rate` : Number of users to spawn per second. Set to 1 by default.
-- `--shape`: The name of a shape to run for the test. 
-If you don't specify a shape or shape instance, then the shape `Default` will be used, 
-  which just runs with the users, runtime & spawn_rate specified on the command line (or picks up defaults 
-of 1, 1, 120s). See `utils/shapes.py` for available shapes and information on how to add
-your own shapes.
-- `--scenario_file` If you want a yaml file where you pre-define some args, this is how 
-you specify that file path. For example, 
-  `scenario_file=example/scenario_example.YAML`. 
-- `--scenario_name` If `--scenario_file` was specified, this is the scenario name that is 
-within that YAML file that corresponds to the scenario you wish to run. Defaults to None.
-- `--tags` See below example: `Loop through a collection of scenarios that match some 
-  tag`.
-- `--scenario_delay` Adds a delay in seconds between scenarios. Defaults to 0.
-- `--influx_host` If you want to report your performance test metrics to some influxdb, 
-you must specify a host.
-    E.g. `1.1.1.1`. Defaults to None.
-- `--influx_port`: Port for your `influx_host` in the case where it is non-default.
-- `--influx_user`: Username for your `influx_host`, if you have one.
-- `--influx_pwd`: Password for your `influx_host`, if you have one.
-
-## Launching tests with a configuration
-All in all, there are a few ways you can actually collect and pass params to a test:
-
-### Run a test with its defaults
-`cd example`
-`pytest test_example.py ...`
-
-### Run a test with a specific scenario
-`cd example`
-`pytest test_example.py --scenario_file=example_scenarios.YAML --scenario_name=example_scenario_1 ...`
-
-### Loop through a collection of scenarios that match some tag
-`cd example`
-`pytest example_scenarios.YAML --tags=smoke ...`
-
-- As shown above, this case involves passing a `.YAML` scenario file into pytest instead of a `.py` file.
-- The `--scenario_file` and `--scenario_name` args will be ignored in this case
-- The `--tags` arg supports AND/OR operators according to the opensource `tag-matcher` package. More info on these operators can be found [here](https://pypi.org/project/tag-matcher/).
-- If no `--tags` arg is specified, then ALL the scenarios in the `.yaml` file will be run.
-- If a value is given for `--scenario_delay`, the test will wait that many seconds between collected scenarios.
-- All scenarios are implicitly tagged with the scenario name to support easily selecting one single
-scenario
-
-**Creating a load test **
-When creating a new load test, the primary grasshopper function you will be using 
-is called `Grasshopper.launch_test`. This function can be imported like so: `from grasshopper.lib.grasshopper import Grasshopper`
-`launch_test` takes in a wide variety of args:
-- `user_classes`: User classes that the runner will run. These user classes must 
-  extend BaseJourney, which is a grasshopper class 
-  (`from grasshopper.lib.journeys.base_journey import BaseJourney`). This can be a 
-  list of classes or just a single class.
-- `**complete_configuration`: In order for the test to have the correct configuration, you 
-  must pass in the kwargs provided by the `complete_configuration` fixture. See example 
-  load test on how to do this properly.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-## Example Load Test  
-
-- You can refer to the test `test_example.py` in the `example` directory for a basic 
-  skeleton of how to get a load test running. In the same directory, there is also an 
-  example `conftest.py` that will show you how to get basic parameterization working.
-- This test can be invoked by running `pytest example/test_example.py` in the root of 
-  this project.
-- This test can also be invoked via a YAML scenario file: (`cd example`, `pytest 
-  example_scenarios.YAML --tags=example1`). In this example scenario file, you can 
-  see how grasshopper_args, grasshopper_scenario_args, and tags are being set.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-## Scenario Args   
-
-- If you want to parameterize your journey class, you should use the `scenario_args` 
-  dict. This is the proper way to pass in values from outside of 
-  the journey for access by the journey code. Note that each journey gets a 
-  ***copy*** on start, so the journey itself can safely modify its own dictionary 
-  once the test is running.
-  `scenario_args` exists for any journey that extends the grasshopper `base_journey` 
-  class. 
-  `scenario_args` also grabs from `self.defaults` on initialization. For example:
-```python
-from locust import between, task
-from grasshopper.lib.journeys.base_journey import BaseJourney
-from grasshopper.lib.grasshopper import Grasshopper
-
-# a journey class with an example task
-class ExampleJourney(BaseJourney):
-    # number of seconds to wait between each task
-    wait_time = between(min_wait=20, max_wait=30)
-    
-    # this defaults dictionary will be merged into scenario_args with lower precedence 
-    # when the journey is initialized
-    defaults = {
-        "foo": "bar",
-    }
-    
-    @task
-    def example_task:
-        logging.info(f'foo is `{self.scenario_args.get("foo")}`.')
-        
-        # aggregate all metrics for the below request under the name "get google"
-        # if name is not specified, then the full url will be the name of the metric
-        response = self.client.get('https://google.com', name='get google')
-
-# the pytest test which launches the journey class
-def test_run_example_journey(complete_configuration):
-    # update scenario args before initialization
-    ExampleJourney.update_incoming_scenario_args(complete_configuration)
-    
-    # launch the journey
-    locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
-    return locust_env
-```
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Checks
 <a id="checks"></a>
 Checks are an assertion that is recorded as a metric. 
 They are useful both to ensure your test is working correctly 
 (e.g. are you getting a valid id back from some post that you sent) 
@@ -292,16 +303,16 @@
         )
 ```
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Thresholds
 <a id="thresholds"></a>
 Thresholds are time-based, and can be added to any trend, whether it be a custom 
-trend or a request response time. Thresholds are currently based off of the 90th 
-percentile of timings. Here is an example of using a threshold: 
+trend or a request response time. Thresholds default to the 0.9 percentile of timings. 
+Here is an example of using a threshold: 
 
 ```python
 # a journey class with an example threshold
 from locust import between, task
 from grasshopper.lib.journeys.base_journey import BaseJourney
 from grasshopper.lib.grasshopper import Grasshopper
 
@@ -320,23 +331,34 @@
 
 # the pytest test which launches the journey class, thresholds could be 
 # parameterized here as well.
 def test_run_example_journey(complete_configuration):
     ExampleJourney.update_incoming_scenario_args(complete_configuration)
     ExampleJourney.update_incoming_scenario_args({
         "thresholds": {
-            "{GET}get google": 4000, # 4 second HTTP response threshold
-            "{CUSTOM}my custom trend": 11000 # 11 second custom trend threshold
-            }
-        }) 
+            "get google":
+                {
+                    "type": "get",
+                    "limit": 4000  # 4 second HTTP response threshold
+                },
+            "my custom trend":
+                {
+                    "type": "custom",
+                    "limit": 11000  # 11 second custom trend threshold
+                }
+        }
+    })
     
     locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
     return locust_env
 ```
 
+Thresholds can also be defined for individual YAML scenarios. Refer to the `thresholds` 
+key in `example/example_scenarios.YAML` for how to use thresholds for YAML scenarios.
+
 After a test has concluded, trend/threshold data can be found in 
 `locust_env.stats.trends`. 
 This data is also reported to the console at the end of each test.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Time Series DB Reporting and Tagging
```

### Comparing `locust-grasshopper-1.2.9/pyproject.toml` & `locust-grasshopper-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "cmake>=3.11.0,<4.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "locust-grasshopper"
-version = "1.2.9" # Managed by bump2version
+version = "1.3.1" # Managed by bump2version
 readme = {file = "README.md", content-type = "text/markdown"}
 description = "a load testing tool extended from locust"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
```

### Comparing `locust-grasshopper-1.2.9/setup.py` & `locust-grasshopper-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/configuration/gh_configuration.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/configuration/gh_configuration.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/__init__.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/fixtures/grasshopper_constants.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/fixtures/grasshopper_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,7 +28,8 @@
         "rp_endpoint",
     ]
     RUNTIME_DEFAULT = 120.0
     USERS_DEFAULT = 1
     SPAWN_RATE_DEFAULT = 1.0
     SHAPE_DEFAULT = "Default"
     SCENARIO_DELAY_DEFAULT = 0.0
+    THRESHOLD_PERCENTILE_DEFAULT = 0.9
```

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/grasshopper.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/grasshopper.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/journeys/base_journey.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/journeys/base_journey.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Module: BaseJourney.
 
 Class to hold all the common functionality that we added on top of Locust's HttpUser
 class.
 """
+import logging
 import signal
+from collections import abc
 from uuid import uuid4
 
 import gevent
 from locust import HttpUser
 
 import grasshopper.lib.util.listeners  # noqa: F401
+from grasshopper.lib.fixtures.grasshopper_constants import GrasshopperConstants
 
 
 class BaseJourney(HttpUser):
     """The base journey class for all other journey classes."""
 
     VUS_DICT = {}
     host = ""
@@ -98,55 +101,85 @@
     def _merge_incoming_defaults_and_params(self):
         self.merge_incoming_scenario_args(self.defaults)
 
     def _set_thresholds(self):
         self.environment.stats.trends = {}
 
         # If parameters are not passed in that need to be set, set them to the defaults
-        for key, value in self.scenario_args.items():
-            self._check_for_threshold_parameters_and_set_thresholds(
-                parameter_key=key,
-                parameter_value=value,
-            )
-
-    def _check_for_threshold_parameters_and_set_thresholds(
-        self, parameter_key, parameter_value
-    ):
-        if parameter_key == "thresholds":
-            for raw_trend_name, threshold_less_than_in_ms in parameter_value.items():
-                trend_name, request_type = self._extract_trend_name(raw_trend_name)
+        self._check_for_threshold_parameters_and_set_thresholds(
+            scenario_args=self.scenario_args
+        )
+
+    def _check_for_threshold_parameters_and_set_thresholds(self, scenario_args):
+        thresholds_collection = scenario_args.get("thresholds")
+        if thresholds_collection is None:
+            return
+        elif self._verify_thresholds_collection_shape(thresholds_collection):
+            for trend_name, threshold_values in thresholds_collection.items():
+                trend_name = str(trend_name)
                 thresh_object = {
-                    "less_than_in_ms": threshold_less_than_in_ms,
+                    "less_than_in_ms": int(threshold_values.get("limit")),
                     "actual_value_in_ms": None,
-                    "percentile": 0.8,
+                    "percentile": float(
+                        threshold_values.get(
+                            "percentile",
+                            GrasshopperConstants.THRESHOLD_PERCENTILE_DEFAULT,
+                        )
+                    ),
                     "succeeded": None,
-                    "http_method": request_type,
+                    "http_method": str(threshold_values.get("type")).upper(),
                 }
                 if trend_name in self.environment.stats.trends:
                     self.environment.stats.trends[trend_name]["thresholds"].append(
                         thresh_object
                     )
                 else:
                     self.environment.stats.trends[trend_name] = {
                         "tags": self.scenario_args.get("tags", {}),
                         "thresholds": [thresh_object],
                     }
+        else:
+            logging.warning(
+                "Skipping registering thresholds due to invalid " "thresholds shape..."
+            )
 
     @staticmethod
-    def _extract_trend_name(raw_trend_name: str):
-        if "{" in raw_trend_name and "}" in raw_trend_name:
-            trend_name = raw_trend_name.split("}")[1]
-            request_type = raw_trend_name.split("}")[0].split("{")[1].upper()
-            return trend_name, request_type
-        else:
-            raise ValueError(
-                "Invalid Trend Name! Please include the request type in curly "
-                + "brackets. E.G: `{POST}post_job_group`, "
-                + "`{CUSTOM}PX_TREND_photon_flow_run`, etc.."
+    def _verify_thresholds_collection_shape(thresholds_collection):
+        valid_types = ["GET", "POST", "PUT", "DELETE", "HEAD", "PATCH", "CUSTOM"]
+        if not isinstance(thresholds_collection, abc.Mapping):
+            logging.warning(
+                f"Thresholds object is of type {type(thresholds_collection)} "
+                f"but must be a mapping!"
             )
+            return False
+        for trend_name, threshold_values in thresholds_collection.items():
+            if (
+                threshold_values.get("type") is None
+                or threshold_values.get("limit") is None
+            ):
+                logging.warning(
+                    f"Singular threshold object `{trend_name}` must have `type`"
+                    f"and `limit` fields defined."
+                )
+                return False
+            elif str(threshold_values.get("type")).upper() not in valid_types:
+                logging.warning(
+                    f"For threshold object {trend_name}, type "
+                    f"`{str(threshold_values.get('type')).upper()}` is "
+                    f"invalid. Must be one of {valid_types}."
+                )
+                return False
+            elif not str(threshold_values.get("limit")).isnumeric():
+                logging.warning(
+                    f"For threshold object {trend_name}, threshold limit of "
+                    f"`{threshold_values.get('limit')}` is invalid. "
+                    f"Must be numeric."
+                )
+                return False
+        return True
 
     def teardown(self, *args, **kwargs):
         """
         Tear down the journey and quit.
 
         The proper way to do your own tear down when extending this class is like so:
             def teardown(self, *args, **kwargs):
```

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/er_basic_console_reporter.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/er_basic_console_reporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/iextendedreporter.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/iextendedreporter.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/reporter_extensions.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/reporter_extensions.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/reporting/shared_reporting.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/reporting/shared_reporting.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/util/decorators.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/util/decorators.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/util/launch.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/util/launch.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/util/listeners.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/util/listeners.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/util/metrics.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/util/metrics.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/util/shapes.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/util/shapes.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/grasshopper/lib/util/utils.py` & `locust-grasshopper-1.3.1/src/grasshopper/lib/util/utils.py`

 * *Files identical despite different names*

### Comparing `locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/PKG-INFO` & `locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-grasshopper
-Version: 1.2.9
+Version: 1.3.1
 Summary: a load testing tool extended from locust
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -235,15 +235,138 @@
 - [timing thresholds](#thresholds)
 - [streamlined metric reporting/tagging system](#db-reporting)
   (only influxDB is supported right now)
 
 ## Installation
 This package can be installed via pip: `pip install locust-grasshopper`
 
+## Example Load Test
+- You can refer to the test `test_example.py` in the `example` directory for a basic 
+  skeleton of how to get a load test running. In the same directory, there is also an 
+  example `conftest.py` that will show you how to get basic parameterization working.
+- This test can be invoked by running `pytest example/test_example.py` in the root of 
+  this project.
+- This test can also be invoked via a YAML scenario file:
+```shell
+cd example
+pytest example_scenarios.YAML --tags=example1
+```
+ In this example scenario file, you can see how grasshopper_args, 
+ grasshopper_scenario_args, and tags are being set.
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Creating a load test
+When creating a new load test, the primary grasshopper function you will be using 
+is called `Grasshopper.launch_test`. This function can be imported like so: `from grasshopper.lib.grasshopper import Grasshopper`
+`launch_test` takes in a wide variety of args:
+- `user_classes`: User classes that the runner will run. These user classes must 
+  extend BaseJourney, which is a grasshopper class 
+  (`from grasshopper.lib.journeys.base_journey import BaseJourney`). This can be a 
+  single class, a list of classes, or a dictionary where the key is the class and 
+  the value is the locust weight to assign to that class.
+- `**complete_configuration`: In order for the test to have the correct configuration, you 
+  must pass in the kwargs provided by the `complete_configuration` fixture. See example 
+  load test on how to do this properly.
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Scenario Args   
+
+- If you want to parameterize your journey class, you should use the `scenario_args` 
+  dict. This is the proper way to pass in values from outside of 
+  the journey for access by the journey code. Note that each journey gets a 
+  ***copy*** on start, so the journey itself can safely modify its own dictionary 
+  once the test is running.
+  `scenario_args` exists for any journey that extends the grasshopper `base_journey` 
+  class. 
+  `scenario_args` also grabs from `self.defaults` on initialization. For example:
+```python
+from locust import between, task
+from grasshopper.lib.journeys.base_journey import BaseJourney
+from grasshopper.lib.grasshopper import Grasshopper
+
+# a journey class with an example task
+class ExampleJourney(BaseJourney):
+    # number of seconds to wait between each task
+    wait_time = between(min_wait=20, max_wait=30)
+    
+    # this defaults dictionary will be merged into scenario_args with lower precedence 
+    # when the journey is initialized
+    defaults = {
+        "foo": "bar",
+    }
+    
+    @task
+    def example_task:
+        logging.info(f'foo is `{self.scenario_args.get("foo")}`.')
+        
+        # aggregate all metrics for the below request under the name "get google"
+        # if name is not specified, then the full url will be the name of the metric
+        response = self.client.get('https://google.com', name='get google')
+
+# the pytest test which launches the journey class
+def test_run_example_journey(complete_configuration):
+    # update scenario args before initialization
+    ExampleJourney.update_incoming_scenario_args(complete_configuration)
+    
+    # launch the journey
+    locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
+    return locust_env
+```
+<p align="right">(<a href="#top">back to top</a>)</p>
 
+## Commonly used grasshopper pytest arguments
+- `--runtime`: Number of seconds to run each test. Set to 120 by default.
+- `--users`: Max number of users that are spawned. Set to 1 by default.
+- `--spawn_rate` : Number of users to spawn per second. Set to 1 by default.
+- `--shape`: The name of a shape to run for the test. 
+If you don't specify a shape or shape instance, then the shape `Default` will be used, 
+  which just runs with the users, runtime & spawn_rate specified on the command line (or picks up defaults 
+of 1, 1, 120s). See `utils/shapes.py` for available shapes and information on how to add
+your own shapes.
+- `--scenario_file` If you want a yaml file where you pre-define some args, this is how 
+you specify that file path. For example, 
+  `scenario_file=example/scenario_example.YAML`. 
+- `--scenario_name` If `--scenario_file` was specified, this is the scenario name that is 
+within that YAML file that corresponds to the scenario you wish to run. Defaults to None.
+- `--tags` See below example: `Loop through a collection of scenarios that match some 
+  tag`.
+- `--scenario_delay` Adds a delay in seconds between scenarios. Defaults to 0.
+- `--influx_host` If you want to report your performance test metrics to some influxdb, 
+you must specify a host.
+    E.g. `1.1.1.1`. Defaults to None.
+- `--influx_port`: Port for your `influx_host` in the case where it is non-default.
+- `--influx_user`: Username for your `influx_host`, if you have one.
+- `--influx_pwd`: Password for your `influx_host`, if you have one.
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+## Launching tests with a configuration
+All in all, there are a few ways you can actually collect and pass params to a test:
+
+### Run a test with its defaults
+`cd example`
+`pytest test_example.py ...`
+
+### Run a test with a specific scenario
+`cd example`
+`pytest test_example.py --scenario_file=example_scenarios.YAML --scenario_name=example_scenario_1 ...`
+
+### Loop through a collection of scenarios that match some tag
+`cd example`
+`pytest example_scenarios.YAML --tags=smoke ...`
+
+- As shown above, this case involves passing a `.YAML` scenario file into pytest instead of a `.py` file.
+- The `--scenario_file` and `--scenario_name` args will be ignored in this case
+- The `--tags` arg supports AND/OR operators according to the opensource `tag-matcher` package. More info on these operators can be found [here](https://pypi.org/project/tag-matcher/).
+- If no `--tags` arg is specified, then ALL the scenarios in the `.yaml` file will be run.
+- If a value is given for `--scenario_delay`, the test will wait that many seconds between collected scenarios.
+- All scenarios are implicitly tagged with the scenario name to support easily selecting one single
+scenario
+
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Configuring Grasshopper
 <a id="creating"></a>
 
 Grasshopper adds a variety of parameters relating to performance testing along with a
 variety of ways to set these values.
 
@@ -254,27 +377,29 @@
 meaning all existing grasshopper tests should still run without modification. The 
 original fixtures and sources for configuration are deprecated, but still produce the 
 same behavior.
 
 All of the usual [pytest arguments](https://docs.pytest.org/en/6.2.x/usage.html) also remain available.
 
 The rest of the sections on configuration assume you are using `locust-grasshopper>=1.1.1`.
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Sources
 Currently, there are 5 different sources for configuration values and they are, in 
 precedence order 
 
 + command line arguments
 + environment variables
 + scenario values from a scenario yaml file
 + grasshopper configuration file
 + global defaults (currently stored in code, not configurable by consumers)
 
 Obviously, the global defaults defined by Grasshopper are not really a source for
 consumers to modify, but we mention it so values don't seem to appear "out of thin air".
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Categories
 The argument list is getting lengthy, so we've broken it down into categories. These
 categories are entirely for humans: better readability, understanding and ease of use. 
 Once they are all fully loaded by Grasshopper, they will be stored in a single 
 `GHConfiguration` object (`dict`). By definition, every argument is in only one category
 and there is no overlap of keys between the categories. If the same key is supplied in
@@ -288,14 +413,15 @@
 | Scenario    | Session            | Variables that may change per scenario and are often<br/>scenario specific; Includes user defined variables that are<br/>not declared as command line arguments by Grasshopper.<br/>However, you may use pytest's addoptions hook in your <br/>conftest to define them. |
 
 At least one of the sections must be present in the global configuration file and
 eventually this will be the same in the configuration section of a scenario in a scenario 
 yaml file. Categories are not used when specifying environment variables or command line
 options. We recommend that you use these categories in file sources, but if a variable 
 is in the wrong section, it won't actually affect the configuration loading process.
+<p align="right">(<a href="#top">back to top</a>)</p>
 
 ### Using Configuration Values 
 Your test(s) may access the complete merged set of key-value pairs via the session scoped 
 fixture `complete_configuration`. This returns a `GHConfiguration` object (dict) which
 is unique to the current scenario. This value will be re-calculated for each new scenario
 executed.
 
@@ -328,14 +454,16 @@
   users: 1.0
   spawn_rate: 1.0
   runtime: 600
 scenario:
   key1 : 'value1'
   key2: 0
 ```
+<p align="right">(<a href="#top">back to top</a>)</p>
+
 ### Additional Extensions to the configuration loading process
 
 If you would like to include other environment variables that might be present in the
 system, you can define a fixture called `extra_env_var_keys` which returns a list of key
 names to load from the `os.environ`. Keys that are missing in the environment will not 
 be included in the `GHConfiguration` object.
 
@@ -344,131 +472,14 @@
 become zero length after the strip will be discarded. This is a mechanism to include any
 scenario arguments you might like to pass via an environment variable.
 
 In the unlikely case that you need to use a different prefix to designate scenario
 variables, you can define a fixture called `env_var_prefix_key` which returns a prefix
 string. The same rules apply about which values are included in the configuration.
 
-### Commonly used arguments
-- `--runtime`: Number of seconds to run each test. Set to 120 by default.
-- `--users`: Max number of users that are spawned. Set to 1 by default.
-- `--spawn_rate` : Number of users to spawn per second. Set to 1 by default.
-- `--shape`: The name of a shape to run for the test. 
-If you don't specify a shape or shape instance, then the shape `Default` will be used, 
-  which just runs with the users, runtime & spawn_rate specified on the command line (or picks up defaults 
-of 1, 1, 120s). See `utils/shapes.py` for available shapes and information on how to add
-your own shapes.
-- `--scenario_file` If you want a yaml file where you pre-define some args, this is how 
-you specify that file path. For example, 
-  `scenario_file=example/scenario_example.YAML`. 
-- `--scenario_name` If `--scenario_file` was specified, this is the scenario name that is 
-within that YAML file that corresponds to the scenario you wish to run. Defaults to None.
-- `--tags` See below example: `Loop through a collection of scenarios that match some 
-  tag`.
-- `--scenario_delay` Adds a delay in seconds between scenarios. Defaults to 0.
-- `--influx_host` If you want to report your performance test metrics to some influxdb, 
-you must specify a host.
-    E.g. `1.1.1.1`. Defaults to None.
-- `--influx_port`: Port for your `influx_host` in the case where it is non-default.
-- `--influx_user`: Username for your `influx_host`, if you have one.
-- `--influx_pwd`: Password for your `influx_host`, if you have one.
-
-## Launching tests with a configuration
-All in all, there are a few ways you can actually collect and pass params to a test:
-
-### Run a test with its defaults
-`cd example`
-`pytest test_example.py ...`
-
-### Run a test with a specific scenario
-`cd example`
-`pytest test_example.py --scenario_file=example_scenarios.YAML --scenario_name=example_scenario_1 ...`
-
-### Loop through a collection of scenarios that match some tag
-`cd example`
-`pytest example_scenarios.YAML --tags=smoke ...`
-
-- As shown above, this case involves passing a `.YAML` scenario file into pytest instead of a `.py` file.
-- The `--scenario_file` and `--scenario_name` args will be ignored in this case
-- The `--tags` arg supports AND/OR operators according to the opensource `tag-matcher` package. More info on these operators can be found [here](https://pypi.org/project/tag-matcher/).
-- If no `--tags` arg is specified, then ALL the scenarios in the `.yaml` file will be run.
-- If a value is given for `--scenario_delay`, the test will wait that many seconds between collected scenarios.
-- All scenarios are implicitly tagged with the scenario name to support easily selecting one single
-scenario
-
-**Creating a load test **
-When creating a new load test, the primary grasshopper function you will be using 
-is called `Grasshopper.launch_test`. This function can be imported like so: `from grasshopper.lib.grasshopper import Grasshopper`
-`launch_test` takes in a wide variety of args:
-- `user_classes`: User classes that the runner will run. These user classes must 
-  extend BaseJourney, which is a grasshopper class 
-  (`from grasshopper.lib.journeys.base_journey import BaseJourney`). This can be a 
-  list of classes or just a single class.
-- `**complete_configuration`: In order for the test to have the correct configuration, you 
-  must pass in the kwargs provided by the `complete_configuration` fixture. See example 
-  load test on how to do this properly.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-## Example Load Test  
-
-- You can refer to the test `test_example.py` in the `example` directory for a basic 
-  skeleton of how to get a load test running. In the same directory, there is also an 
-  example `conftest.py` that will show you how to get basic parameterization working.
-- This test can be invoked by running `pytest example/test_example.py` in the root of 
-  this project.
-- This test can also be invoked via a YAML scenario file: (`cd example`, `pytest 
-  example_scenarios.YAML --tags=example1`). In this example scenario file, you can 
-  see how grasshopper_args, grasshopper_scenario_args, and tags are being set.
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-## Scenario Args   
-
-- If you want to parameterize your journey class, you should use the `scenario_args` 
-  dict. This is the proper way to pass in values from outside of 
-  the journey for access by the journey code. Note that each journey gets a 
-  ***copy*** on start, so the journey itself can safely modify its own dictionary 
-  once the test is running.
-  `scenario_args` exists for any journey that extends the grasshopper `base_journey` 
-  class. 
-  `scenario_args` also grabs from `self.defaults` on initialization. For example:
-```python
-from locust import between, task
-from grasshopper.lib.journeys.base_journey import BaseJourney
-from grasshopper.lib.grasshopper import Grasshopper
-
-# a journey class with an example task
-class ExampleJourney(BaseJourney):
-    # number of seconds to wait between each task
-    wait_time = between(min_wait=20, max_wait=30)
-    
-    # this defaults dictionary will be merged into scenario_args with lower precedence 
-    # when the journey is initialized
-    defaults = {
-        "foo": "bar",
-    }
-    
-    @task
-    def example_task:
-        logging.info(f'foo is `{self.scenario_args.get("foo")}`.')
-        
-        # aggregate all metrics for the below request under the name "get google"
-        # if name is not specified, then the full url will be the name of the metric
-        response = self.client.get('https://google.com', name='get google')
-
-# the pytest test which launches the journey class
-def test_run_example_journey(complete_configuration):
-    # update scenario args before initialization
-    ExampleJourney.update_incoming_scenario_args(complete_configuration)
-    
-    # launch the journey
-    locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
-    return locust_env
-```
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Checks
 <a id="checks"></a>
 Checks are an assertion that is recorded as a metric. 
 They are useful both to ensure your test is working correctly 
 (e.g. are you getting a valid id back from some post that you sent) 
@@ -515,16 +526,16 @@
         )
 ```
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Thresholds
 <a id="thresholds"></a>
 Thresholds are time-based, and can be added to any trend, whether it be a custom 
-trend or a request response time. Thresholds are currently based off of the 90th 
-percentile of timings. Here is an example of using a threshold: 
+trend or a request response time. Thresholds default to the 0.9 percentile of timings. 
+Here is an example of using a threshold: 
 
 ```python
 # a journey class with an example threshold
 from locust import between, task
 from grasshopper.lib.journeys.base_journey import BaseJourney
 from grasshopper.lib.grasshopper import Grasshopper
 
@@ -543,23 +554,34 @@
 
 # the pytest test which launches the journey class, thresholds could be 
 # parameterized here as well.
 def test_run_example_journey(complete_configuration):
     ExampleJourney.update_incoming_scenario_args(complete_configuration)
     ExampleJourney.update_incoming_scenario_args({
         "thresholds": {
-            "{GET}get google": 4000, # 4 second HTTP response threshold
-            "{CUSTOM}my custom trend": 11000 # 11 second custom trend threshold
-            }
-        }) 
+            "get google":
+                {
+                    "type": "get",
+                    "limit": 4000  # 4 second HTTP response threshold
+                },
+            "my custom trend":
+                {
+                    "type": "custom",
+                    "limit": 11000  # 11 second custom trend threshold
+                }
+        }
+    })
     
     locust_env = Grasshopper.launch_test(ExampleJourney, **complete_configuration)
     return locust_env
 ```
 
+Thresholds can also be defined for individual YAML scenarios. Refer to the `thresholds` 
+key in `example/example_scenarios.YAML` for how to use thresholds for YAML scenarios.
+
 After a test has concluded, trend/threshold data can be found in 
 `locust_env.stats.trends`. 
 This data is also reported to the console at the end of each test.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Time Series DB Reporting and Tagging
```

### Comparing `locust-grasshopper-1.2.9/src/locust_grasshopper.egg-info/SOURCES.txt` & `locust-grasshopper-1.3.1/src/locust_grasshopper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

