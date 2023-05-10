# Comparing `tmp/arkdriver-1.0.7.tar.gz` & `tmp/arkdriver-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdriver-1.0.7.tar", last modified: Wed May 10 05:11:03 2023, max compression
+gzip compressed data, was "arkdriver-1.0.8.tar", last modified: Wed May 10 06:36:52 2023, max compression
```

## Comparing `arkdriver-1.0.7.tar` & `arkdriver-1.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.327039 arkdriver-1.0.7/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1935 2023-05-10 05:11:03.327039 arkdriver-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.7/README.md
--rw-rw-rw-   0        0        0      669 2023-04-27 02:55:08.000000 arkdriver-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     1186 2023-05-10 05:11:03.333493 arkdriver-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.253450 arkdriver-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.264454 arkdriver-1.0.7/src/arkdriver/
--rw-rw-rw-   0        0        0      102 2023-04-27 01:08:24.000000 arkdriver-1.0.7/src/arkdriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.299043 arkdriver-1.0.7/src/arkdriver/driver/
--rw-rw-rw-   0        0        0      182 2023-04-21 03:31:49.000000 arkdriver-1.0.7/src/arkdriver/driver/__init__.py
--rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.7/src/arkdriver/driver/application.py
--rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.7/src/arkdriver/driver/driver.py
--rw-rw-rw-   0        0        0     4177 2023-05-10 05:06:47.000000 arkdriver-1.0.7/src/arkdriver/driver/run.py
--rw-rw-rw-   0        0        0     4657 2023-04-30 23:44:23.000000 arkdriver-1.0.7/src/arkdriver/main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.307038 arkdriver-1.0.7/src/arkdriver/presentation/
--rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.7/src/arkdriver/presentation/__init__.py
--rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.7/src/arkdriver/presentation/presentation.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.7/src/arkdriver/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.316040 arkdriver-1.0.7/src/arkdriver/session/
--rw-rw-rw-   0        0        0        0 2023-04-30 23:29:41.000000 arkdriver-1.0.7/src/arkdriver/session/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-30 23:48:48.000000 arkdriver-1.0.7/src/arkdriver/session/session.py
-drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.281453 arkdriver-1.0.7/src/arkdriver.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 05:11:03.000000 arkdriver-1.0.7/src/arkdriver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 05:11:03.326037 arkdriver-1.0.7/tests/
--rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.7/tests/test_lib.py
--rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.7/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.555234 arkdriver-1.0.8/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-05-10 06:36:52.555234 arkdriver-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.8/README.md
+-rw-rw-rw-   0        0        0      690 2023-05-10 06:36:29.000000 arkdriver-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0     1201 2023-05-10 06:36:52.557234 arkdriver-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.521376 arkdriver-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.528376 arkdriver-1.0.8/src/arkdriver/
+-rw-rw-rw-   0        0        0      102 2023-04-27 01:08:24.000000 arkdriver-1.0.8/src/arkdriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.549234 arkdriver-1.0.8/src/arkdriver/driver/
+-rw-rw-rw-   0        0        0      182 2023-04-21 03:31:49.000000 arkdriver-1.0.8/src/arkdriver/driver/__init__.py
+-rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.8/src/arkdriver/driver/application.py
+-rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.8/src/arkdriver/driver/driver.py
+-rw-rw-rw-   0        0        0     4177 2023-05-10 05:06:47.000000 arkdriver-1.0.8/src/arkdriver/driver/run.py
+-rw-rw-rw-   0        0        0     4657 2023-04-30 23:44:23.000000 arkdriver-1.0.8/src/arkdriver/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.551234 arkdriver-1.0.8/src/arkdriver/presentation/
+-rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.8/src/arkdriver/presentation/__init__.py
+-rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.8/src/arkdriver/presentation/presentation.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.8/src/arkdriver/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.553234 arkdriver-1.0.8/src/arkdriver/session/
+-rw-rw-rw-   0        0        0        0 2023-04-30 23:29:41.000000 arkdriver-1.0.8/src/arkdriver/session/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-04-30 23:48:48.000000 arkdriver-1.0.8/src/arkdriver/session/session.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.546234 arkdriver-1.0.8/src/arkdriver.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      170 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.555234 arkdriver-1.0.8/tests/
+-rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.8/tests/test_lib.py
+-rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.8/tests/test_main.py
```

### Comparing `arkdriver-1.0.7/LICENSE` & `arkdriver-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/PKG-INFO` & `arkdriver-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.7
+Version: 1.0.8
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdriver-1.0.7/README.md` & `arkdriver-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/pyproject.toml` & `arkdriver-1.0.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,16 @@
     "wheel",
     "requests>=2.28.1",
     "arklibrary==1.*",
     "pywinauto",
     "pywin32",
     "six",
     "comtypes",
-    "numpy>=1.24.2"
+    "numpy>=1.24.2",
+    "nitrado==1.*"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [too.pytest.ini_options]
 addopts = "--cov=arkdriver"
 testpaths = [
```

### Comparing `arkdriver-1.0.7/setup.cfg` & `arkdriver-1.0.8/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6472 6976 6572 0d0a 7665   = arkdriver..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 370d 0a74  rsion = 1.0.7..t
+00000020: 7273 696f 6e20 3d20 312e 302e 380d 0a74  rsion = 1.0.8..t
 00000030: 6573 745f 7665 7273 696f 6e20 3d20 312e  est_version = 1.
 00000040: 302e 370d 0a70 726f 6475 6374 696f 6e5f  0.7..production_
-00000050: 7665 7273 696f 6e20 3d20 312e 302e 370d  version = 1.0.7.
+00000050: 7665 7273 696f 6e20 3d20 312e 302e 380d  version = 1.0.8.
 00000060: 0a61 7574 686f 7220 3d20 4d61 7572 6963  .author = Mauric
 00000070: 696f 0d0a 6175 7468 6f72 5f65 6d61 696c  io..author_email
 00000080: 203d 2064 6576 2e6d 6175 7269 6369 6f2e   = dev.mauricio.
 00000090: 6c6f 6d65 6c69 4067 6d61 696c 2e63 6f6d  lomeli@gmail.com
 000000a0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000b0: 5468 6973 2061 7070 6c69 6361 7469 6f6e  This application
 000000c0: 2061 6363 6573 7365 7320 7468 6520 4172   accesses the Ar
@@ -45,31 +45,32 @@
 000002c0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
 000002d0: 200d 0a09 7768 6565 6c0d 0a09 7265 7175   ...wheel...requ
 000002e0: 6573 7473 3e3d 322e 3238 2e31 0d0a 0961  ests>=2.28.1...a
 000002f0: 726b 6c69 6272 6172 793d 3d31 2e2a 0d0a  rklibrary==1.*..
 00000300: 0970 7977 696e 6175 746f 0d0a 0970 7977  .pywinauto...pyw
 00000310: 696e 3332 0d0a 0973 6978 0d0a 0963 6f6d  in32...six...com
 00000320: 7479 7065 730d 0a09 6e75 6d70 793e 3d31  types...numpy>=1
-00000330: 2e32 342e 320d 0a0d 0a5b 6f70 7469 6f6e  .24.2....[option
-00000340: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000350: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000360: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
-00000370: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
-00000380: 6e67 203d 200d 0a09 7079 7465 7374 3e3d  ng = ...pytest>=
-00000390: 362e 300d 0a09 7079 7465 7374 2d63 6f76  6.0...pytest-cov
-000003a0: 3e3d 322e 300d 0a09 6d79 7079 3e3d 302e  >=2.0...mypy>=0.
-000003b0: 3937 310d 0a09 666c 616b 6538 3e3d 332e  971...flake8>=3.
-000003c0: 390d 0a09 746f 783e 3d33 2e32 340d 0a0d  9...tox>=3.24...
-000003d0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000003e0: 655f 6461 7461 5d0d 0a61 726b 6472 6976  e_data]..arkdriv
-000003f0: 6572 203d 2070 792e 7479 7065 642c 2061  er = py.typed, a
-00000400: 726b 2e6c 6e6b 2c20 636f 6e66 6967 2e69  rk.lnk, config.i
-00000410: 6e69 2c20 7079 7769 6e33 322d 3330 342e  ni, pywin32-304.
-00000420: 7769 6e33 322d 7079 332e 392e 6578 652c  win32-py3.9.exe,
-00000430: 2070 7977 696e 3332 2d33 3034 2e77 696e   pywin32-304.win
-00000440: 2d61 6d64 3634 2d70 7933 2e31 302e 6578  -amd64-py3.10.ex
-00000450: 650d 0a0d 0a5b 666c 616b 6538 5d0d 0a6d  e....[flake8]..m
-00000460: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-00000470: 2031 3630 0d0a 0d0a 5b65 6767 5f69 6e66   160....[egg_inf
-00000480: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000490: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000004a0: 0d0a                                     ..
+00000330: 2e32 342e 320d 0a09 6e69 7472 6164 6f3d  .24.2...nitrado=
+00000340: 3d31 2e2a 0d0a 0d0a 5b6f 7074 696f 6e73  =1.*....[options
+00000350: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+00000360: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+00000370: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+00000380: 7265 7175 6972 655d 0d0a 7465 7374 696e  require]..testin
+00000390: 6720 3d20 0d0a 0970 7974 6573 743e 3d36  g = ...pytest>=6
+000003a0: 2e30 0d0a 0970 7974 6573 742d 636f 763e  .0...pytest-cov>
+000003b0: 3d32 2e30 0d0a 096d 7970 793e 3d30 2e39  =2.0...mypy>=0.9
+000003c0: 3731 0d0a 0966 6c61 6b65 383e 3d33 2e39  71...flake8>=3.9
+000003d0: 0d0a 0974 6f78 3e3d 332e 3234 0d0a 0d0a  ...tox>=3.24....
+000003e0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000003f0: 5f64 6174 615d 0d0a 6172 6b64 7269 7665  _data]..arkdrive
+00000400: 7220 3d20 7079 2e74 7970 6564 2c20 6172  r = py.typed, ar
+00000410: 6b2e 6c6e 6b2c 2063 6f6e 6669 672e 696e  k.lnk, config.in
+00000420: 692c 2070 7977 696e 3332 2d33 3034 2e77  i, pywin32-304.w
+00000430: 696e 3332 2d70 7933 2e39 2e65 7865 2c20  in32-py3.9.exe, 
+00000440: 7079 7769 6e33 322d 3330 342e 7769 6e2d  pywin32-304.win-
+00000450: 616d 6436 342d 7079 332e 3130 2e65 7865  amd64-py3.10.exe
+00000460: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 6d61  ....[flake8]..ma
+00000470: 782d 6c69 6e65 2d6c 656e 6774 6820 3d20  x-line-length = 
+00000480: 3136 300d 0a0d 0a5b 6567 675f 696e 666f  160....[egg_info
+00000490: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000004a0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000004b0: 0a                                       .
```

### Comparing `arkdriver-1.0.7/src/arkdriver/driver/application.py` & `arkdriver-1.0.8/src/arkdriver/driver/application.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/src/arkdriver/driver/driver.py` & `arkdriver-1.0.8/src/arkdriver/driver/driver.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/src/arkdriver/driver/run.py` & `arkdriver-1.0.8/src/arkdriver/driver/run.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/src/arkdriver/main.py` & `arkdriver-1.0.8/src/arkdriver/main.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/src/arkdriver/presentation/presentation.py` & `arkdriver-1.0.8/src/arkdriver/presentation/presentation.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/src/arkdriver/session/session.py` & `arkdriver-1.0.8/src/arkdriver/session/session.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/src/arkdriver.egg-info/PKG-INFO` & `arkdriver-1.0.8/src/arkdriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.7
+Version: 1.0.8
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdriver-1.0.7/src/arkdriver.egg-info/SOURCES.txt` & `arkdriver-1.0.8/src/arkdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.7/tests/test_main.py` & `arkdriver-1.0.8/tests/test_main.py`

 * *Files identical despite different names*

