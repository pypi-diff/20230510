# Comparing `tmp/log_distance_measures-1.0.1.tar.gz` & `tmp/log_distance_measures-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log_distance_measures-1.0.1.tar", max compression
+gzip compressed data, was "log_distance_measures-1.0.2.tar", max compression
```

## Comparing `log_distance_measures-1.0.1.tar` & `log_distance_measures-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11349 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/LICENSE
--rw-r--r--   0        0        0    12826 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/README.md
--rw-r--r--   0        0        0      598 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      296 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/__init__.py
--rw-r--r--   0        0        0     5861 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/absolute_event_distribution.py
--rw-r--r--   0        0        0     8852 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/active_cases_over_time.py
--rw-r--r--   0        0        0     7352 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/case_arrival_distribution.py
--rw-r--r--   0        0        0     4623 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/circadian_event_distribution.py
--rw-r--r--   0        0        0     1034 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/config.py
--rw-r--r--   0        0        0     7185 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/control_flow_log_distance.py
--rw-r--r--   0        0        0     3080 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/cycle_time_distribution.py
--rw-r--r--   0        0        0     4372 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/earth_movers_distance.py
--rw-r--r--   0        0        0     3454 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/n_gram_distribution.py
--rw-r--r--   0        0        0     5220 2023-05-10 11:05:41.706588 log_distance_measures-1.0.1/src/log_distance_measures/relative_event_distribution.py
--rw-r--r--   0        0        0    13565 1970-01-01 00:00:00.000000 log_distance_measures-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/LICENSE
+-rw-r--r--   0        0        0    12826 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/README.md
+-rw-r--r--   0        0        0      598 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      296 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/__init__.py
+-rw-r--r--   0        0        0     5861 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/absolute_event_distribution.py
+-rw-r--r--   0        0        0     8852 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/active_cases_over_time.py
+-rw-r--r--   0        0        0     7352 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/case_arrival_distribution.py
+-rw-r--r--   0        0        0     4623 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/circadian_event_distribution.py
+-rw-r--r--   0        0        0     1034 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/config.py
+-rw-r--r--   0        0        0     7185 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/control_flow_log_distance.py
+-rw-r--r--   0        0        0     3080 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/cycle_time_distribution.py
+-rw-r--r--   0        0        0     4372 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/earth_movers_distance.py
+-rw-r--r--   0        0        0     3454 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/n_gram_distribution.py
+-rw-r--r--   0        0        0     5220 2023-05-10 11:09:21.048396 log_distance_measures-1.0.2/src/log_distance_measures/relative_event_distribution.py
+-rw-r--r--   0        0        0    13565 1970-01-01 00:00:00.000000 log_distance_measures-1.0.2/PKG-INFO
```

### Comparing `log_distance_measures-1.0.1/LICENSE` & `log_distance_measures-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/README.md` & `log_distance_measures-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/pyproject.toml` & `log_distance_measures-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "log-distance-measures"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python package with the implementation of different distance measures between two event logs, from the control-flow, temporal, and queuing perspectives."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pandas = "^2.0.0"
```

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/absolute_event_distribution.py` & `log_distance_measures-1.0.2/src/log_distance_measures/absolute_event_distribution.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/active_cases_over_time.py` & `log_distance_measures-1.0.2/src/log_distance_measures/active_cases_over_time.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/case_arrival_distribution.py` & `log_distance_measures-1.0.2/src/log_distance_measures/case_arrival_distribution.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/circadian_event_distribution.py` & `log_distance_measures-1.0.2/src/log_distance_measures/circadian_event_distribution.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/config.py` & `log_distance_measures-1.0.2/src/log_distance_measures/config.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/control_flow_log_distance.py` & `log_distance_measures-1.0.2/src/log_distance_measures/control_flow_log_distance.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/cycle_time_distribution.py` & `log_distance_measures-1.0.2/src/log_distance_measures/cycle_time_distribution.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/earth_movers_distance.py` & `log_distance_measures-1.0.2/src/log_distance_measures/earth_movers_distance.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/n_gram_distribution.py` & `log_distance_measures-1.0.2/src/log_distance_measures/n_gram_distribution.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/src/log_distance_measures/relative_event_distribution.py` & `log_distance_measures-1.0.2/src/log_distance_measures/relative_event_distribution.py`

 * *Files identical despite different names*

### Comparing `log_distance_measures-1.0.1/PKG-INFO` & `log_distance_measures-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log-distance-measures
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package with the implementation of different distance measures between two event logs, from the control-flow, temporal, and queuing perspectives.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

