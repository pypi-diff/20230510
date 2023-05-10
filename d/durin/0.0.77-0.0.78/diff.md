# Comparing `tmp/durin-0.0.77.tar.gz` & `tmp/durin-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durin-0.0.77.tar", last modified: Mon May  8 11:25:23 2023, max compression
+gzip compressed data, was "durin-0.0.78.tar", last modified: Wed May 10 12:16:41 2023, max compression
```

## Comparing `durin-0.0.77.tar` & `durin-0.0.78.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.354399 durin-0.0.77/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 11:25:11.000000 durin-0.0.77/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-08 11:25:23.354399 durin-0.0.77/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-05-08 11:25:11.000000 durin-0.0.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.346399 durin-0.0.77/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-05-08 11:25:11.000000 durin-0.0.77/bin/durin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.350399 durin-0.0.77/durin/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 11:25:11.000000 durin-0.0.77/durin/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 11:25:11.000000 durin-0.0.77/durin/Read_profilers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-05-08 11:25:11.000000 durin-0.0.77/durin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-08 11:25:11.000000 durin-0.0.77/durin/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-08 11:25:11.000000 durin-0.0.77/durin/actuator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-05-08 11:25:11.000000 durin-0.0.77/durin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.350399 durin-0.0.77/durin/controller/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/dvs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.350399 durin-0.0.77/durin/controller/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/test/test_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-08 11:25:11.000000 durin-0.0.77/durin/durin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-05-08 11:25:11.000000 durin-0.0.77/durin/durin_birdseye.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-05-08 11:25:11.000000 durin-0.0.77/durin/dvs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.354399 durin-0.0.77/durin/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/CPU_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/braitenberg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/dashboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.354399 durin-0.0.77/durin/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/gamepad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/ringbuffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/schema.capnp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-05-08 11:25:11.000000 durin-0.0.77/durin/sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14646 2023-05-08 11:25:11.000000 durin-0.0.77/durin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.350399 durin-0.0.77/durin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:25:23.354399 durin-0.0.77/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-05-08 11:25:11.000000 durin-0.0.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:41.795519 durin-0.0.78/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 12:16:32.000000 durin-0.0.78/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-10 12:16:41.791519 durin-0.0.78/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-05-10 12:16:32.000000 durin-0.0.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:41.779519 durin-0.0.78/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-05-10 12:16:32.000000 durin-0.0.78/bin/durin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:41.783519 durin-0.0.78/durin/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 12:16:32.000000 durin-0.0.78/durin/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-10 12:16:32.000000 durin-0.0.78/durin/Read_profilers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-05-10 12:16:32.000000 durin-0.0.78/durin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-10 12:16:32.000000 durin-0.0.78/durin/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-10 12:16:32.000000 durin-0.0.78/durin/actuator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-05-10 12:16:32.000000 durin-0.0.78/durin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:41.787519 durin-0.0.78/durin/controller/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-10 12:16:32.000000 durin-0.0.78/durin/controller/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-10 12:16:32.000000 durin-0.0.78/durin/controller/dvs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-05-10 12:16:32.000000 durin-0.0.78/durin/controller/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:41.787519 durin-0.0.78/durin/controller/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:32.000000 durin-0.0.78/durin/controller/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-05-10 12:16:32.000000 durin-0.0.78/durin/controller/test/test_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-10 12:16:32.000000 durin-0.0.78/durin/durin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-05-10 12:16:32.000000 durin-0.0.78/durin/durin_birdseye.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-05-10 12:16:32.000000 durin-0.0.78/durin/dvs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:41.791519 durin-0.0.78/durin/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/CPU_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/braitenberg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/dashboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-10 12:16:32.000000 durin-0.0.78/durin/examples/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:41.791519 durin-0.0.78/durin/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-10 12:16:32.000000 durin-0.0.78/durin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-10 12:16:32.000000 durin-0.0.78/durin/io/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-10 12:16:32.000000 durin-0.0.78/durin/io/gamepad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-05-10 12:16:32.000000 durin-0.0.78/durin/io/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-10 12:16:32.000000 durin-0.0.78/durin/io/ringbuffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-05-10 12:16:32.000000 durin-0.0.78/durin/io/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-10 12:16:32.000000 durin-0.0.78/durin/io/schema.capnp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-05-10 12:16:32.000000 durin-0.0.78/durin/sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14646 2023-05-10 12:16:32.000000 durin-0.0.78/durin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:16:41.783519 durin-0.0.78/durin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-10 12:16:41.000000 durin-0.0.78/durin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-10 12:16:41.000000 durin-0.0.78/durin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:16:41.000000 durin-0.0.78/durin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 12:16:41.000000 durin-0.0.78/durin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 12:16:41.000000 durin-0.0.78/durin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:16:41.795519 durin-0.0.78/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-05-10 12:16:32.000000 durin-0.0.78/setup.py
```

### Comparing `durin-0.0.77/PKG-INFO` & `durin-0.0.78/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.77
+Version: 0.0.78
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.77/README.md` & `durin-0.0.78/README.md`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/actuator.py` & `durin-0.0.78/durin/actuator.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/cli.py` & `durin-0.0.78/durin/cli.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/controller/server.py` & `durin-0.0.78/durin/controller/server.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/controller/test/test_stream.py` & `durin-0.0.78/durin/controller/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/durin.py` & `durin-0.0.78/durin/durin.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/durin_birdseye.jpg` & `durin-0.0.78/durin/durin_birdseye.jpg`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/examples/braitenberg.py` & `durin-0.0.78/durin/examples/braitenberg.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/examples/commands.py` & `durin-0.0.78/durin/examples/commands.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/examples/dashboard.py` & `durin-0.0.78/durin/examples/dashboard.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/examples/main.py` & `durin-0.0.78/durin/examples/main.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/examples/plot.py` & `durin-0.0.78/durin/examples/plot.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/examples/record.py` & `durin-0.0.78/durin/examples/record.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/examples/stats.py` & `durin-0.0.78/durin/examples/stats.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/io/__init__.py` & `durin-0.0.78/durin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/io/command.py` & `durin-0.0.78/durin/io/command.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/io/gamepad.py` & `durin-0.0.78/durin/io/gamepad.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/io/network.py` & `durin-0.0.78/durin/io/network.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/io/ringbuffer.py` & `durin-0.0.78/durin/io/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/io/runnable.py` & `durin-0.0.78/durin/io/runnable.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/io/schema.capnp` & `durin-0.0.78/durin/io/schema.capnp`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/sensor.py` & `durin-0.0.78/durin/sensor.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin/ui.py` & `durin-0.0.78/durin/ui.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/durin.egg-info/PKG-INFO` & `durin-0.0.78/durin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.77
+Version: 0.0.78
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.77/durin.egg-info/SOURCES.txt` & `durin-0.0.78/durin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `durin-0.0.77/setup.py` & `durin-0.0.78/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = fp.read().split("\n")
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="durin",
-    version="0.0.77",
+    version="0.0.78",
     install_requires=requirements,
     packages=find_packages(),
     license="LGPLv3",
     maintainer="Jens E. Pedersen",
     maintainer_email="jeped@kth.se",
     extras_require={"aestream": ["aestream"]},
     scripts=["bin/durin"],
```

