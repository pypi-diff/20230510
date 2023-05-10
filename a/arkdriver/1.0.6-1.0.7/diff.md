# Comparing `tmp/arkdriver-1.0.6.tar.gz` & `tmp/arkdriver-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdriver-1.0.6.tar", last modified: Mon May  1 02:17:20 2023, max compression
+gzip compressed data, was "arkdriver-1.0.7.tar", last modified: Wed May 10 05:11:03 2023, max compression
```

## Comparing `arkdriver-1.0.6.tar` & `arkdriver-1.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 02:17:20.023619 arkdriver-1.0.6/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     1935 2023-05-01 02:17:20.023619 arkdriver-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.6/README.md
--rw-rw-rw-   0        0        0      669 2023-04-27 02:55:08.000000 arkdriver-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2023-05-01 02:17:20.025618 arkdriver-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 02:17:19.982940 arkdriver-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 02:17:19.990945 arkdriver-1.0.6/src/arkdriver/
--rw-rw-rw-   0        0        0      102 2023-04-27 01:08:24.000000 arkdriver-1.0.6/src/arkdriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:17:20.011620 arkdriver-1.0.6/src/arkdriver/driver/
--rw-rw-rw-   0        0        0      182 2023-04-21 03:31:49.000000 arkdriver-1.0.6/src/arkdriver/driver/__init__.py
--rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.6/src/arkdriver/driver/application.py
--rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.6/src/arkdriver/driver/driver.py
--rw-rw-rw-   0        0        0     4303 2023-05-01 02:13:56.000000 arkdriver-1.0.6/src/arkdriver/driver/run.py
--rw-rw-rw-   0        0        0     4657 2023-04-30 23:44:23.000000 arkdriver-1.0.6/src/arkdriver/main.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:17:20.013620 arkdriver-1.0.6/src/arkdriver/presentation/
--rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.6/src/arkdriver/presentation/__init__.py
--rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.6/src/arkdriver/presentation/presentation.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.6/src/arkdriver/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-01 02:17:20.015620 arkdriver-1.0.6/src/arkdriver/session/
--rw-rw-rw-   0        0        0        0 2023-04-30 23:29:41.000000 arkdriver-1.0.6/src/arkdriver/session/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-30 23:48:48.000000 arkdriver-1.0.6/src/arkdriver/session/session.py
-drwxrwxrwx   0        0        0        0 2023-05-01 02:17:20.007617 arkdriver-1.0.6/src/arkdriver.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-05-01 02:17:19.000000 arkdriver-1.0.6/src/arkdriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-01 02:17:19.000000 arkdriver-1.0.6/src/arkdriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 02:17:19.000000 arkdriver-1.0.6/src/arkdriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-05-01 02:17:19.000000 arkdriver-1.0.6/src/arkdriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 02:17:19.000000 arkdriver-1.0.6/src/arkdriver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 02:17:20.022619 arkdriver-1.0.6/tests/
--rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.6/tests/test_lib.py
--rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.6/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.327039 arkdriver-1.0.7/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-05-10 05:11:03.327039 arkdriver-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.7/README.md
+-rw-rw-rw-   0        0        0      669 2023-04-27 02:55:08.000000 arkdriver-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1186 2023-05-10 05:11:03.333493 arkdriver-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.253450 arkdriver-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.264454 arkdriver-1.0.7/src/arkdriver/
+-rw-rw-rw-   0        0        0      102 2023-04-27 01:08:24.000000 arkdriver-1.0.7/src/arkdriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.299043 arkdriver-1.0.7/src/arkdriver/driver/
+-rw-rw-rw-   0        0        0      182 2023-04-21 03:31:49.000000 arkdriver-1.0.7/src/arkdriver/driver/__init__.py
+-rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.7/src/arkdriver/driver/application.py
+-rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.7/src/arkdriver/driver/driver.py
+-rw-rw-rw-   0        0        0     4177 2023-05-10 05:06:47.000000 arkdriver-1.0.7/src/arkdriver/driver/run.py
+-rw-rw-rw-   0        0        0     4657 2023-04-30 23:44:23.000000 arkdriver-1.0.7/src/arkdriver/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.307038 arkdriver-1.0.7/src/arkdriver/presentation/
+-rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.7/src/arkdriver/presentation/__init__.py
+-rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.7/src/arkdriver/presentation/presentation.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.7/src/arkdriver/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.316040 arkdriver-1.0.7/src/arkdriver/session/
+-rw-rw-rw-   0        0        0        0 2023-04-30 23:29:41.000000 arkdriver-1.0.7/src/arkdriver/session/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-30 23:48:48.000000 arkdriver-1.0.7/src/arkdriver/session/session.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.281453 arkdriver-1.0.7/src/arkdriver.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.326037 arkdriver-1.0.7/tests/
+-rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.7/tests/test_lib.py
+-rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.7/tests/test_main.py
```

### Comparing `arkdriver-1.0.6/LICENSE` & `arkdriver-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/PKG-INFO` & `arkdriver-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.6
+Version: 1.0.7
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdriver-1.0.6/README.md` & `arkdriver-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/pyproject.toml` & `arkdriver-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/setup.cfg` & `arkdriver-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6472 6976 6572 0d0a 7665   = arkdriver..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 360d 0a74  rsion = 1.0.6..t
+00000020: 7273 696f 6e20 3d20 312e 302e 370d 0a74  rsion = 1.0.7..t
 00000030: 6573 745f 7665 7273 696f 6e20 3d20 312e  est_version = 1.
 00000040: 302e 370d 0a70 726f 6475 6374 696f 6e5f  0.7..production_
-00000050: 7665 7273 696f 6e20 3d20 312e 302e 360d  version = 1.0.6.
+00000050: 7665 7273 696f 6e20 3d20 312e 302e 370d  version = 1.0.7.
 00000060: 0a61 7574 686f 7220 3d20 4d61 7572 6963  .author = Mauric
 00000070: 696f 0d0a 6175 7468 6f72 5f65 6d61 696c  io..author_email
 00000080: 203d 2064 6576 2e6d 6175 7269 6369 6f2e   = dev.mauricio.
 00000090: 6c6f 6d65 6c69 4067 6d61 696c 2e63 6f6d  lomeli@gmail.com
 000000a0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000b0: 5468 6973 2061 7070 6c69 6361 7469 6f6e  This application
 000000c0: 2061 6363 6573 7365 7320 7468 6520 4172   accesses the Ar
```

### Comparing `arkdriver-1.0.6/src/arkdriver/driver/application.py` & `arkdriver-1.0.7/src/arkdriver/driver/application.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/src/arkdriver/driver/driver.py` & `arkdriver-1.0.7/src/arkdriver/driver/driver.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/src/arkdriver/driver/run.py` & `arkdriver-1.0.7/src/arkdriver/driver/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 
 
 def get_new_commands(domain: str, server: ArkServer, driver_token: str) -> list:
     count = 0
     while count < 10:
         try:
             server_name = server.query.server_name.replace("\r", "").replace("\n", "")
-            service_id = str(server.service_id)
             json = {'driver_token': driver_token}
-            if service_id:
-                json['service_id'] = service_id
             if server_name:
                 json['server_name'] = server_name
             headers = {'mime': 'application/json'}
             data = requests.get(f"{domain}/command_control/queued", json=json, headers=headers).json()
             return data["commands"]
         except Exception as e:
             print(f"[Error]: {str(e)}")
```

### Comparing `arkdriver-1.0.6/src/arkdriver/main.py` & `arkdriver-1.0.7/src/arkdriver/main.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/src/arkdriver/presentation/presentation.py` & `arkdriver-1.0.7/src/arkdriver/presentation/presentation.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/src/arkdriver/session/session.py` & `arkdriver-1.0.7/src/arkdriver/session/session.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/src/arkdriver.egg-info/PKG-INFO` & `arkdriver-1.0.7/src/arkdriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.6
+Version: 1.0.7
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdriver-1.0.6/src/arkdriver.egg-info/SOURCES.txt` & `arkdriver-1.0.7/src/arkdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.6/tests/test_main.py` & `arkdriver-1.0.7/tests/test_main.py`

 * *Files identical despite different names*

