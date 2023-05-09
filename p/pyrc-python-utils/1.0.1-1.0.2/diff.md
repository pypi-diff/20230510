# Comparing `tmp/pyrc-python-utils-1.0.1.tar.gz` & `tmp/pyrc-python-utils-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrc-python-utils-1.0.1.tar", last modified: Tue May  9 21:11:06 2023, max compression
+gzip compressed data, was "pyrc-python-utils-1.0.2.tar", last modified: Tue May  9 21:27:59 2023, max compression
```

## Comparing `pyrc-python-utils-1.0.1.tar` & `pyrc-python-utils-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 21:11:06.877145 pyrc-python-utils-1.0.1/
--rw-rw-rw-   0        0        0     1085 2023-05-08 22:51:52.000000 pyrc-python-utils-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       57 2023-05-08 23:01:23.000000 pyrc-python-utils-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      532 2023-05-09 21:11:06.876145 pyrc-python-utils-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.1/README.md
--rw-rw-rw-   0        0        0      559 2023-05-09 21:10:54.000000 pyrc-python-utils-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 21:11:06.877145 pyrc-python-utils-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 21:11:06.872144 pyrc-python-utils-1.0.1/src/
--rw-rw-rw-   0        0        0        0 2023-05-08 20:58:19.000000 pyrc-python-utils-1.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 21:11:06.875145 pyrc-python-utils-1.0.1/src/pyrc_python_utils.egg-info/
--rw-rw-rw-   0        0        0      532 2023-05-09 21:11:06.000000 pyrc-python-utils-1.0.1/src/pyrc_python_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-05-09 21:11:06.000000 pyrc-python-utils-1.0.1/src/pyrc_python_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 21:11:06.000000 pyrc-python-utils-1.0.1/src/pyrc_python_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-09 21:11:06.000000 pyrc-python-utils-1.0.1/src/pyrc_python_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      503 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.1/src/pyrc_util_datetime.py
--rw-rw-rw-   0        0        0     3409 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.1/src/pyrc_util_exchange.py
--rw-rw-rw-   0        0        0      229 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.1/src/pyrc_util_file.py
--rw-rw-rw-   0        0        0     9941 2023-05-09 21:02:11.000000 pyrc-python-utils-1.0.1/src/pyrc_util_sftp.py
--rw-rw-rw-   0        0        0     4408 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.1/src/pyrc_util_sharepoint.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:27:59.030266 pyrc-python-utils-1.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 22:51:52.000000 pyrc-python-utils-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-05-08 23:01:23.000000 pyrc-python-utils-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      456 2023-05-09 21:27:59.030266 pyrc-python-utils-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.2/README.md
+-rw-rw-rw-   0        0        0      519 2023-05-09 21:27:40.000000 pyrc-python-utils-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 21:27:59.030266 pyrc-python-utils-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 21:27:59.024265 pyrc-python-utils-1.0.2/src/
+-rw-rw-rw-   0        0        0        0 2023-05-08 20:58:19.000000 pyrc-python-utils-1.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:27:59.029265 pyrc-python-utils-1.0.2/src/pyrc_python_utils.egg-info/
+-rw-rw-rw-   0        0        0      456 2023-05-09 21:27:59.000000 pyrc-python-utils-1.0.2/src/pyrc_python_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-05-09 21:27:59.000000 pyrc-python-utils-1.0.2/src/pyrc_python_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 21:27:59.000000 pyrc-python-utils-1.0.2/src/pyrc_python_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-09 21:27:59.000000 pyrc-python-utils-1.0.2/src/pyrc_python_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       98 2023-05-09 21:27:59.000000 pyrc-python-utils-1.0.2/src/pyrc_python_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      503 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.2/src/pyrc_util_datetime.py
+-rw-rw-rw-   0        0        0     3409 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.2/src/pyrc_util_exchange.py
+-rw-rw-rw-   0        0        0      229 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.2/src/pyrc_util_file.py
+-rw-rw-rw-   0        0        0     9941 2023-05-09 21:02:11.000000 pyrc-python-utils-1.0.2/src/pyrc_util_sftp.py
+-rw-rw-rw-   0        0        0     4408 2023-05-08 17:54:07.000000 pyrc-python-utils-1.0.2/src/pyrc_util_sharepoint.py
```

### Comparing `pyrc-python-utils-1.0.1/LICENSE` & `pyrc-python-utils-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.1/pyproject.toml` & `pyrc-python-utils-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrc-python-utils"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "Paul Vienneau", email = "paul.vienneau@payroc.com" },
 ]
+dependencies = [
+    "paramiko>=3.1.0"
+]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[project.urls]
-"Homepage" = "https://github.com/payroc/pyrc-scripts-python_utils"
```

### Comparing `pyrc-python-utils-1.0.1/src/pyrc_util_exchange.py` & `pyrc-python-utils-1.0.2/src/pyrc_util_exchange.py`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.1/src/pyrc_util_sftp.py` & `pyrc-python-utils-1.0.2/src/pyrc_util_sftp.py`

 * *Files identical despite different names*

### Comparing `pyrc-python-utils-1.0.1/src/pyrc_util_sharepoint.py` & `pyrc-python-utils-1.0.2/src/pyrc_util_sharepoint.py`

 * *Files identical despite different names*

