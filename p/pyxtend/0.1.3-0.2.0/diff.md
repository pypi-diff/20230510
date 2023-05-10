# Comparing `tmp/pyxtend-0.1.3.tar.gz` & `tmp/pyxtend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxtend-0.1.3.tar", last modified: Thu Jan  6 02:30:54 2022, max compression
+gzip compressed data, was "pyxtend-0.2.0.tar", last modified: Wed May 10 01:18:27 2023, max compression
```

## Comparing `pyxtend-0.1.3.tar` & `pyxtend-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-01-06 02:30:54.124086 pyxtend-0.1.3/
--rw-rw-rw-   0        0        0     1094 2021-12-22 03:22:01.000000 pyxtend-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      603 2022-01-06 02:30:54.125071 pyxtend-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       61 2022-01-06 02:29:45.000000 pyxtend-0.1.3/README.md
--rw-rw-rw-   0        0        0      110 2021-12-22 03:22:03.000000 pyxtend-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      640 2022-01-06 02:30:54.131072 pyxtend-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-01-06 02:30:54.086077 pyxtend-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2022-01-06 02:30:54.103074 pyxtend-0.1.3/src/pyxtend/
--rw-rw-rw-   0        0        0       32 2022-01-02 19:51:01.000000 pyxtend-0.1.3/src/pyxtend/__init__.py
--rw-rw-rw-   0        0        0      699 2022-01-02 19:51:01.000000 pyxtend-0.1.3/src/pyxtend/pyxtend.py
-drwxrwxrwx   0        0        0        0 2022-01-06 02:30:54.123072 pyxtend-0.1.3/src/pyxtend.egg-info/
--rw-rw-rw-   0        0        0      603 2022-01-06 02:30:54.000000 pyxtend-0.1.3/src/pyxtend.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2022-01-06 02:30:54.000000 pyxtend-0.1.3/src/pyxtend.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-06 02:30:54.000000 pyxtend-0.1.3/src/pyxtend.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-01-06 02:30:54.000000 pyxtend-0.1.3/src/pyxtend.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 01:18:27.222142 pyxtend-0.2.0/
+-rw-rw-rw-   0        0        0     1094 2021-12-22 03:22:01.000000 pyxtend-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      562 2023-05-10 01:18:27.222142 pyxtend-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2022-01-06 02:29:45.000000 pyxtend-0.2.0/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-22 03:22:03.000000 pyxtend-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      640 2023-05-10 01:18:27.224176 pyxtend-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 01:18:27.196150 pyxtend-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 01:18:27.206144 pyxtend-0.2.0/src/pyxtend/
+-rw-rw-rw-   0        0        0       32 2022-01-02 19:51:01.000000 pyxtend-0.2.0/src/pyxtend/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-05-10 01:12:35.000000 pyxtend-0.2.0/src/pyxtend/pyxtend.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:18:27.220174 pyxtend-0.2.0/src/pyxtend.egg-info/
+-rw-rw-rw-   0        0        0      562 2023-05-10 01:18:27.000000 pyxtend-0.2.0/src/pyxtend.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-05-10 01:18:27.000000 pyxtend-0.2.0/src/pyxtend.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:18:27.000000 pyxtend-0.2.0/src/pyxtend.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 01:18:27.000000 pyxtend-0.2.0/src/pyxtend.egg-info/top_level.txt
```

### Comparing `pyxtend-0.1.3/LICENSE` & `pyxtend-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxtend-0.1.3/PKG-INFO` & `pyxtend-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: pyxtend
-Version: 0.1.3
+Version: 0.2.0
 Summary: Some functions for Python
 Home-page: https://github.com/jss367/pyxtend
 Author: Julius
 Author-email: julius.simonelli@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jss367/pyxtend/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyxtend
 
 Some functions to make Python more productive.
-
-
```

### Comparing `pyxtend-0.1.3/setup.cfg` & `pyxtend-0.2.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7978 7465 6e64 0d0a 7665 7273   = pyxtend..vers
-00000020: 696f 6e20 3d20 302e 312e 330d 0a61 7574  ion = 0.1.3..aut
+00000020: 696f 6e20 3d20 302e 322e 300d 0a61 7574  ion = 0.2.0..aut
 00000030: 686f 7220 3d20 4a75 6c69 7573 0d0a 6175  hor = Julius..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206a 756c  thor_email = jul
 00000050: 6975 732e 7369 6d6f 6e65 6c6c 6940 676d  ius.simonelli@gm
 00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000070: 7469 6f6e 203d 2053 6f6d 6520 6675 6e63  tion = Some func
 00000080: 7469 6f6e 7320 666f 7220 5079 7468 6f6e  tions for Python
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
@@ -28,13 +28,13 @@
 000001b0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
 000001c0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
 000001d0: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
 000001e0: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
 000001f0: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
 00000200: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
 00000210: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-00000220: 6573 203d 203e 3d33 2e36 0d0a 0d0a 5b6f  es = >=3.6....[o
+00000220: 6573 203d 203e 3d33 2e38 0d0a 0d0a 5b6f  es = >=3.8....[o
 00000230: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
 00000240: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
 00000250: 7263 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  rc....[egg_info]
 00000260: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
 00000270: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

### Comparing `pyxtend-0.1.3/src/pyxtend.egg-info/PKG-INFO` & `pyxtend-0.2.0/src/pyxtend.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: pyxtend
-Version: 0.1.3
+Version: 0.2.0
 Summary: Some functions for Python
 Home-page: https://github.com/jss367/pyxtend
 Author: Julius
 Author-email: julius.simonelli@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jss367/pyxtend/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyxtend
 
 Some functions to make Python more productive.
-
-
```

