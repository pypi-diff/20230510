# Comparing `tmp/pyrc-python-utils-1.0.3.tar.gz` & `tmp/pyrc-python-utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrc-python-utils-1.0.3.tar", last modified: Tue May  9 22:47:26 2023, max compression
+gzip compressed data, was "pyrc-python-utils-1.0.4.tar", last modified: Tue May  9 23:01:27 2023, max compression
```

## Comparing `pyrc-python-utils-1.0.3.tar` & `pyrc-python-utils-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 22:47:26.206203 pyrc-python-utils-1.0.3/
--rw-rw-rw-   0        0        0     1085 2023-05-08 22:51:52.000000 pyrc-python-utils-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       57 2023-05-08 23:01:23.000000 pyrc-python-utils-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      456 2023-05-09 22:47:26.206203 pyrc-python-utils-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.3/README.md
--rw-rw-rw-   0        0        0      519 2023-05-09 22:47:06.000000 pyrc-python-utils-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 22:47:26.206203 pyrc-python-utils-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 22:47:26.200203 pyrc-python-utils-1.0.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-08 20:58:19.000000 pyrc-python-utils-1.0.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 22:47:26.205202 pyrc-python-utils-1.0.3/src/pyrc_python_utils.egg-info/
--rw-rw-rw-   0        0        0      456 2023-05-09 22:47:26.000000 pyrc-python-utils-1.0.3/src/pyrc_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-05-09 22:47:26.000000 pyrc-python-utils-1.0.3/src/pyrc_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 22:47:26.000000 pyrc-python-utils-1.0.3/src/pyrc_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-09 22:47:26.000000 pyrc-python-utils-1.0.3/src/pyrc_python_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       98 2023-05-09 22:47:26.000000 pyrc-python-utils-1.0.3/src/pyrc_python_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      503 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.3/src/pyrc_util_datetime.py
--rw-rw-rw-   0        0        0     3409 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.3/src/pyrc_util_exchange.py
--rw-rw-rw-   0        0        0      229 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.3/src/pyrc_util_file.py
--rw-rw-rw-   0        0        0     9944 2023-05-09 22:46:49.000000 pyrc-python-utils-1.0.3/src/pyrc_util_sftp.py
--rw-rw-rw-   0        0        0     4408 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.3/src/pyrc_util_sharepoint.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:01:27.883490 pyrc-python-utils-1.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 22:51:52.000000 pyrc-python-utils-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-05-08 23:01:23.000000 pyrc-python-utils-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      456 2023-05-09 23:01:27.883490 pyrc-python-utils-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.4/README.md
+-rw-rw-rw-   0        0        0      519 2023-05-09 22:58:12.000000 pyrc-python-utils-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 23:01:27.883490 pyrc-python-utils-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 23:01:27.877485 pyrc-python-utils-1.0.4/src/
+-rw-rw-rw-   0        0        0        0 2023-05-08 20:58:19.000000 pyrc-python-utils-1.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:01:27.882489 pyrc-python-utils-1.0.4/src/pyrc_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      456 2023-05-09 23:01:27.000000 pyrc-python-utils-1.0.4/src/pyrc_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-05-09 23:01:27.000000 pyrc-python-utils-1.0.4/src/pyrc_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:01:27.000000 pyrc-python-utils-1.0.4/src/pyrc_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 23:01:27.000000 pyrc-python-utils-1.0.4/src/pyrc_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       98 2023-05-09 23:01:27.000000 pyrc-python-utils-1.0.4/src/pyrc_python_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      503 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.4/src/pyrc_util_datetime.py
+-rw-rw-rw-   0        0        0     3409 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.4/src/pyrc_util_exchange.py
+-rw-rw-rw-   0        0        0      229 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.4/src/pyrc_util_file.py
+-rw-rw-rw-   0        0        0     9946 2023-05-09 22:56:25.000000 pyrc-python-utils-1.0.4/src/pyrc_util_sftp.py
+-rw-rw-rw-   0        0        0     4408 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.4/src/pyrc_util_sharepoint.py
```

### Comparing `pyrc-python-utils-1.0.3/LICENSE` & `pyrc-python-utils-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.3/pyproject.toml` & `pyrc-python-utils-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrc-python-utils"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "Paul Vienneau", email = "paul.vienneau@payroc.com" },
 ]
 dependencies = [
     "paramiko>=3.1.0"
 ]
 description = "A small example package"
```

### Comparing `pyrc-python-utils-1.0.3/src/pyrc_util_exchange.py` & `pyrc-python-utils-1.0.4/src/pyrc_util_exchange.py`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.3/src/pyrc_util_sftp.py` & `pyrc-python-utils-1.0.4/src/pyrc_util_sftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import re
 import stat
 from io import BytesIO
 
 import paramiko
 
-from . import pyrc_util_file as util_file
+from src import pyrc_util_file as util_file
 
 
 def create_client(host: str, username: str, password: str) -> paramiko.SFTPClient:
     transport = paramiko.Transport((host, 22))
     transport.connect(None, username, password)
 
     return paramiko.SFTPClient.from_transport(transport)
```

### Comparing `pyrc-python-utils-1.0.3/src/pyrc_util_sharepoint.py` & `pyrc-python-utils-1.0.4/src/pyrc_util_sharepoint.py`

 * *Files identical despite different names*

