# Comparing `tmp/frugy-0.4.1.tar.gz` & `tmp/frugy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/frugy-0.4.1.tar", last modified: Fri Jan 13 11:28:28 2023, max compression
+gzip compressed data, was "dist/frugy-0.4.2.tar", last modified: Wed May 10 10:29:23 2023, max compression
```

## Comparing `frugy-0.4.1.tar` & `frugy-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-13 11:28:28.000000 frugy-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-01-13 11:28:25.000000 frugy-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-01-13 11:28:28.000000 frugy-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-01-13 11:28:25.000000 frugy-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-13 11:28:28.000000 frugy-0.4.1/frugy/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/areas.py
--rw-r--r--   0 runner    (1001) docker     (122)     9006 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/fru.py
--rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/fru_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     7344 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/multirecords.py
--rw-r--r--   0 runner    (1001) docker     (122)     8900 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/multirecords_fmc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/multirecords_ipmi.py
--rw-r--r--   0 runner    (1001) docker     (122)    20339 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/multirecords_picmg.py
--rw-r--r--   0 runner    (1001) docker     (122)    23120 2023-01-13 11:28:25.000000 frugy-0.4.1/frugy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-13 11:28:28.000000 frugy-0.4.1/frugy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-01-13 11:28:28.000000 frugy-0.4.1/frugy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      423 2023-01-13 11:28:28.000000 frugy-0.4.1/frugy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-13 11:28:28.000000 frugy-0.4.1/frugy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-01-13 11:28:28.000000 frugy-0.4.1/frugy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-01-13 11:28:28.000000 frugy-0.4.1/frugy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-01-13 11:28:28.000000 frugy-0.4.1/frugy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-13 11:28:28.000000 frugy-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1269 2023-01-13 11:28:25.000000 frugy-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 10:29:23.000000 frugy-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1515 2023-05-10 10:29:20.000000 frugy-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-05-10 10:29:23.000000 frugy-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-05-10 10:29:20.000000 frugy-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 10:29:23.000000 frugy-0.4.2/frugy/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/areas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9006 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/fru.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/fru_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7344 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/multirecords.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8900 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/multirecords_fmc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/multirecords_ipmi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20339 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/multirecords_picmg.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23120 2023-05-10 10:29:20.000000 frugy-0.4.2/frugy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 10:29:23.000000 frugy-0.4.2/frugy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-05-10 10:29:23.000000 frugy-0.4.2/frugy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-10 10:29:23.000000 frugy-0.4.2/frugy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 10:29:23.000000 frugy-0.4.2/frugy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-10 10:29:23.000000 frugy-0.4.2/frugy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-10 10:29:23.000000 frugy-0.4.2/frugy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-10 10:29:23.000000 frugy-0.4.2/frugy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 10:29:23.000000 frugy-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1269 2023-05-10 10:29:20.000000 frugy-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 10:29:23.000000 frugy-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3057 2023-05-10 10:29:20.000000 frugy-0.4.2/tests/test_areas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-05-10 10:29:20.000000 frugy-0.4.2/tests/test_fru.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3132 2023-05-10 10:29:20.000000 frugy-0.4.2/tests/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-10 10:29:20.000000 frugy-0.4.2/tests/test_multirecords.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3356 2023-05-10 10:29:20.000000 frugy-0.4.2/tests/test_types.py
```

### Comparing `frugy-0.4.1/LICENSE.txt` & `frugy-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/PKG-INFO` & `frugy-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frugy
-Version: 0.4.1
+Version: 0.4.2
 Summary: FRU Generator YAML
 Home-page: https://techlab.desy.de
 Author: Patrick Huesmann
 Author-email: patrick.huesmann@desy.de
 License: BSD
 Keywords: ipmi fru microtca amc fmc picmg vita
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `frugy-0.4.1/README.md` & `frugy-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy/areas.py` & `frugy-0.4.2/frugy/areas.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,16 @@
         ('custom_info_fields', CustomStringArray),
     ]
 
     _time_ref = datetime(1996, 1, 1)
 
     def _set_mfg_date_time(self, timestamp):
         if timestamp is not None:
+            if type(timestamp) == str:
+                timestamp = datetime.fromisoformat(timestamp)
             td = timestamp - BoardInfo._time_ref
             minutes = td.seconds // 60 + td.days * (60*24)
             self._set('mfg_date_time', minutes)
         else:
             self._set('mfg_date_time', 0)
 
     def _get_mfg_date_time(self):
```

### Comparing `frugy-0.4.1/frugy/cli.py` & `frugy-0.4.2/frugy/cli.py`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy/fru.py` & `frugy-0.4.2/frugy/fru.py`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy/fru_registry.py` & `frugy-0.4.2/frugy/fru_registry.py`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy/multirecords.py` & `frugy-0.4.2/frugy/multirecords.py`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy/multirecords_fmc.py` & `frugy-0.4.2/frugy/multirecords_fmc.py`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy/multirecords_ipmi.py` & `frugy-0.4.2/frugy/multirecords_ipmi.py`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy/multirecords_picmg.py` & `frugy-0.4.2/frugy/multirecords_picmg.py`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy/types.py` & `frugy-0.4.2/frugy/types.py`

 * *Files identical despite different names*

### Comparing `frugy-0.4.1/frugy.egg-info/PKG-INFO` & `frugy-0.4.2/frugy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frugy
-Version: 0.4.1
+Version: 0.4.2
 Summary: FRU Generator YAML
 Home-page: https://techlab.desy.de
 Author: Patrick Huesmann
 Author-email: patrick.huesmann@desy.de
 License: BSD
 Keywords: ipmi fru microtca amc fmc picmg vita
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `frugy-0.4.1/setup.py` & `frugy-0.4.2/setup.py`

 * *Files identical despite different names*

