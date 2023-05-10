# Comparing `tmp/utracto-0.0.4.tar.gz` & `tmp/utracto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utracto-0.0.4.tar", last modified: Wed May 10 12:33:38 2023, max compression
+gzip compressed data, was "utracto-0.0.5.tar", last modified: Wed May 10 12:52:29 2023, max compression
```

## Comparing `utracto-0.0.4.tar` & `utracto-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:33:37.960000 utracto-0.0.4/
--rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1893 2023-05-10 12:33:40.000000 utracto-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1392 2023-05-10 12:17:46.000000 utracto-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 12:33:40.000000 utracto-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1070 2023-05-10 12:33:10.000000 utracto-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:33:37.960000 utracto-0.0.4/utracto/
--rw-rw-rw-   0        0        0       74 2023-05-10 12:33:20.000000 utracto-0.0.4/utracto/__init__.py
--rw-rw-rw-   0        0        0     2690 2022-12-13 15:12:08.000000 utracto-0.0.4/utracto/core.py
--rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.4/utracto/example.py
--rw-rw-rw-   0        0        0     7389 2022-12-12 15:25:56.000000 utracto-0.0.4/utracto/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:33:37.970000 utracto-0.0.4/utracto.egg-info/
--rw-rw-rw-   0        0        0     1893 2023-05-10 12:33:38.000000 utracto-0.0.4/utracto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-10 12:33:38.000000 utracto-0.0.4/utracto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:33:38.000000 utracto-0.0.4/utracto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-10 12:33:38.000000 utracto-0.0.4/utracto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 12:33:38.000000 utracto-0.0.4/utracto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:52:29.600000 utracto-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1893 2023-05-10 12:52:30.000000 utracto-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1392 2023-05-10 12:17:46.000000 utracto-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:52:30.000000 utracto-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2023-05-10 12:33:10.000000 utracto-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:52:29.620000 utracto-0.0.5/utracto/
+-rw-rw-rw-   0        0        0       74 2023-05-10 12:52:22.000000 utracto-0.0.5/utracto/__init__.py
+-rw-rw-rw-   0        0        0     2690 2022-12-13 15:12:08.000000 utracto-0.0.5/utracto/core.py
+-rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.5/utracto/example.py
+-rw-rw-rw-   0        0        0     5932 2023-05-10 12:48:36.000000 utracto-0.0.5/utracto/tracking.py
+-rw-rw-rw-   0        0        0     5172 2023-05-10 12:44:16.000000 utracto-0.0.5/utracto/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:52:29.620000 utracto-0.0.5/utracto.egg-info/
+-rw-rw-rw-   0        0        0     1893 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/top_level.txt
```

### Comparing `utracto-0.0.4/LICENSE` & `utracto-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `utracto-0.0.4/PKG-INFO` & `utracto-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.4
+Version: 0.0.5
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `utracto-0.0.4/README.md` & `utracto-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `utracto-0.0.4/setup.py` & `utracto-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.4/utracto/core.py` & `utracto-0.0.5/utracto/core.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.4/utracto.egg-info/PKG-INFO` & `utracto-0.0.5/utracto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.4
+Version: 0.0.5
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

