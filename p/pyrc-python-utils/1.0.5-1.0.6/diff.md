# Comparing `tmp/pyrc-python-utils-1.0.5.tar.gz` & `tmp/pyrc-python-utils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrc-python-utils-1.0.5.tar", last modified: Tue May  9 23:25:55 2023, max compression
+gzip compressed data, was "pyrc-python-utils-1.0.6.tar", last modified: Tue May  9 23:46:03 2023, max compression
```

## Comparing `pyrc-python-utils-1.0.5.tar` & `pyrc-python-utils-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 23:25:55.150832 pyrc-python-utils-1.0.5/
--rw-rw-rw-   0        0        0     1085 2023-05-08 22:51:52.000000 pyrc-python-utils-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       57 2023-05-08 23:01:23.000000 pyrc-python-utils-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      456 2023-05-09 23:25:55.150832 pyrc-python-utils-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.5/README.md
--rw-rw-rw-   0        0        0      519 2023-05-09 23:25:37.000000 pyrc-python-utils-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 23:25:55.151832 pyrc-python-utils-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 23:25:55.144833 pyrc-python-utils-1.0.5/src/
--rw-rw-rw-   0        0        0        0 2023-05-09 23:25:13.000000 pyrc-python-utils-1.0.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 23:25:55.149832 pyrc-python-utils-1.0.5/src/pyrc_python_utils.egg-info/
--rw-rw-rw-   0        0        0      456 2023-05-09 23:25:55.000000 pyrc-python-utils-1.0.5/src/pyrc_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-05-09 23:25:55.000000 pyrc-python-utils-1.0.5/src/pyrc_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 23:25:55.000000 pyrc-python-utils-1.0.5/src/pyrc_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 23:25:55.000000 pyrc-python-utils-1.0.5/src/pyrc_python_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       98 2023-05-09 23:25:55.000000 pyrc-python-utils-1.0.5/src/pyrc_python_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      503 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.5/src/pyrc_util_datetime.py
--rw-rw-rw-   0        0        0     3409 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.5/src/pyrc_util_exchange.py
--rw-rw-rw-   0        0        0      229 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.5/src/pyrc_util_file.py
--rw-rw-rw-   0        0        0     9944 2023-05-09 23:25:03.000000 pyrc-python-utils-1.0.5/src/pyrc_util_sftp.py
--rw-rw-rw-   0        0        0     4408 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.5/src/pyrc_util_sharepoint.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:46:03.367354 pyrc-python-utils-1.0.6/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 22:51:52.000000 pyrc-python-utils-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-05-08 23:01:23.000000 pyrc-python-utils-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      143 2023-05-09 23:46:03.367354 pyrc-python-utils-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.6/README.md
+-rw-rw-rw-   0        0        0      568 2023-05-09 23:45:37.000000 pyrc-python-utils-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 23:46:03.367354 pyrc-python-utils-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 23:46:03.361351 pyrc-python-utils-1.0.6/src/
+-rw-rw-rw-   0        0        0        0 2023-05-09 23:25:13.000000 pyrc-python-utils-1.0.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:46:03.366350 pyrc-python-utils-1.0.6/src/pyrc_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      143 2023-05-09 23:46:03.000000 pyrc-python-utils-1.0.6/src/pyrc_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-05-09 23:46:03.000000 pyrc-python-utils-1.0.6/src/pyrc_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:46:03.000000 pyrc-python-utils-1.0.6/src/pyrc_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 23:46:03.000000 pyrc-python-utils-1.0.6/src/pyrc_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       98 2023-05-09 23:46:03.000000 pyrc-python-utils-1.0.6/src/pyrc_python_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      503 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.6/src/pyrc_util_datetime.py
+-rw-rw-rw-   0        0        0     3409 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.6/src/pyrc_util_exchange.py
+-rw-rw-rw-   0        0        0      229 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.6/src/pyrc_util_file.py
+-rw-rw-rw-   0        0        0     9936 2023-05-09 23:45:01.000000 pyrc-python-utils-1.0.6/src/pyrc_util_sftp.py
+-rw-rw-rw-   0        0        0     4408 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.6/src/pyrc_util_sharepoint.py
```

### Comparing `pyrc-python-utils-1.0.5/LICENSE` & `pyrc-python-utils-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.5/pyproject.toml` & `pyrc-python-utils-1.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrc-python-utils"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     { name = "Paul Vienneau", email = "paul.vienneau@payroc.com" },
 ]
 dependencies = [
     "paramiko>=3.1.0"
 ]
+[build]
+package = [
+    {include = "src"},
+]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyrc-python-utils-1.0.5/src/pyrc_util_exchange.py` & `pyrc-python-utils-1.0.6/src/pyrc_util_exchange.py`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.5/src/pyrc_util_sftp.py` & `pyrc-python-utils-1.0.6/src/pyrc_util_sftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import re
 import stat
 from io import BytesIO
 
 import paramiko
 
-from . import pyrc_util_file as util_file
+from . import pyrc_util_file
 
 
 def create_client(host: str, username: str, password: str) -> paramiko.SFTPClient:
     transport = paramiko.Transport((host, 22))
     transport.connect(None, username, password)
 
     return paramiko.SFTPClient.from_transport(transport)
@@ -152,15 +152,15 @@
         full_path = os.path.join(local_path, local_file)
     else:
         # Local file name was not provided, so use the remote file name
         full_path = os.path.join(local_path, os.path.basename(remote_file))
 
     # If we're asked NOT to overwrite, get next available file name
     if not overwrite_local_file:
-        full_path = util_file.get_next_available_filename(full_path)
+        full_path = pyrc_util_file.get_next_available_filename(full_path)
 
     client.get(remote_file, full_path)
 
 
 def get_files(client: paramiko.SFTPClient, remote_path: str, local_path: str, match_exp: str = None):
     # For a remote directory, get all files or those matching the regex - match_exp
     for remote_file in client.listdir(remote_path):
```

### Comparing `pyrc-python-utils-1.0.5/src/pyrc_util_sharepoint.py` & `pyrc-python-utils-1.0.6/src/pyrc_util_sharepoint.py`

 * *Files identical despite different names*

