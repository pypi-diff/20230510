# Comparing `tmp/sacc-0.8.tar.gz` & `tmp/sacc-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sacc-0.8.tar", last modified: Wed May  3 09:48:18 2023, max compression
+gzip compressed data, was "sacc-0.8.1.tar", last modified: Wed May 10 16:00:52 2023, max compression
```

## Comparing `sacc-0.8.tar` & `sacc-0.8.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.278178 sacc-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 09:48:07.000000 sacc-0.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-03 09:48:07.000000 sacc-0.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.266177 sacc-0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.270177 sacc-0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-03 09:48:07.000000 sacc-0.8/.github/workflows/desc-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-03 09:48:07.000000 sacc-0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-03 09:48:07.000000 sacc-0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-03 09:48:07.000000 sacc-0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-03 09:48:07.000000 sacc-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 09:48:07.000000 sacc-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 09:48:18.274178 sacc-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-03 09:48:07.000000 sacc-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.270177 sacc-0.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-03 09:48:07.000000 sacc-0.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-03 09:48:07.000000 sacc-0.8/doc/format.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.270177 sacc-0.8/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/covariance.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/data_types.rst
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/sacc.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/tracers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 09:48:07.000000 sacc-0.8/doc/source/windows.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-03 09:48:07.000000 sacc-0.8/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)   102753 2023-05-03 09:48:07.000000 sacc-0.8/examples/CMB_LSS_read.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   120842 2023-05-03 09:48:07.000000 sacc-0.8/examples/CMB_LSS_write.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-03 09:48:07.000000 sacc-0.8/examples/Convert_DES_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-05-03 09:48:07.000000 sacc-0.8/examples/Convert_KIDS_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    50825 2023-05-03 09:48:07.000000 sacc-0.8/examples/Create_Sacc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42715 2023-05-03 09:48:07.000000 sacc-0.8/examples/Create_cluster_count_SACC.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 09:48:07.000000 sacc-0.8/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-05-03 09:48:07.000000 sacc-0.8/examples/SACC_for_clusters.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   154105 2023-05-03 09:48:07.000000 sacc-0.8/examples/SACC_read.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-03 09:48:07.000000 sacc-0.8/examples/SACC_write.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20744 2023-05-03 09:48:07.000000 sacc-0.8/examples/example-txpipe-sacc1.sacc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 09:48:07.000000 sacc-0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/sacc/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-03 09:48:07.000000 sacc-0.8/sacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-03 09:48:07.000000 sacc-0.8/sacc/covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    16583 2023-05-03 09:48:07.000000 sacc-0.8/sacc/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    49485 2023-05-03 09:48:07.000000 sacc-0.8/sacc/sacc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-03 09:48:07.000000 sacc-0.8/sacc/tracers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-03 09:48:07.000000 sacc-0.8/sacc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-03 09:48:07.000000 sacc-0.8/sacc/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/sacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 09:48:18.000000 sacc-0.8/sacc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:48:18.278178 sacc-0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-05-03 09:48:07.000000 sacc-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:48:18.274178 sacc-0.8/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 09:48:07.000000 sacc-0.8/test/data/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-03 09:48:07.000000 sacc-0.8/test/make_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    27726 2023-05-03 09:48:07.000000 sacc-0.8/test/test_sacc2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.766541 sacc-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 16:00:48.000000 sacc-0.8.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 16:00:48.000000 sacc-0.8.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.758541 sacc-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.758541 sacc-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-10 16:00:48.000000 sacc-0.8.1/.github/workflows/desc-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 16:00:48.000000 sacc-0.8.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 16:00:48.000000 sacc-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-10 16:00:48.000000 sacc-0.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-10 16:00:48.000000 sacc-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 16:00:48.000000 sacc-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-10 16:00:52.766541 sacc-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-10 16:00:48.000000 sacc-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.758541 sacc-0.8.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/format.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.762541 sacc-0.8.1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/covariance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/data_types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/sacc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/tracers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-10 16:00:48.000000 sacc-0.8.1/doc/source/windows.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.762541 sacc-0.8.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   102753 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/CMB_LSS_read.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   120842 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/CMB_LSS_write.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/Convert_DES_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/Convert_KIDS_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    50825 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/Create_Sacc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42715 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/Create_cluster_count_SACC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/SACC_for_clusters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   154105 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/SACC_read.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/SACC_write.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20744 2023-05-10 16:00:48.000000 sacc-0.8.1/examples/example-txpipe-sacc1.sacc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 16:00:48.000000 sacc-0.8.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.762541 sacc-0.8.1/sacc/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16583 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49485 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/sacc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27599 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/tracers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-10 16:00:48.000000 sacc-0.8.1/sacc/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.762541 sacc-0.8.1/sacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 16:00:52.000000 sacc-0.8.1/sacc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:00:52.766541 sacc-0.8.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      698 2023-05-10 16:00:48.000000 sacc-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.766541 sacc-0.8.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:00:52.766541 sacc-0.8.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 16:00:48.000000 sacc-0.8.1/test/data/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-10 16:00:48.000000 sacc-0.8.1/test/make_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28004 2023-05-10 16:00:48.000000 sacc-0.8.1/test/test_sacc2.py
```

### Comparing `sacc-0.8/.github/workflows/desc-ci.yml` & `sacc-0.8.1/.github/workflows/desc-ci.yml`

 * *Files identical despite different names*

### Comparing `sacc-0.8/.gitignore` & `sacc-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sacc-0.8/LICENSE` & `sacc-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sacc-0.8/PKG-INFO` & `sacc-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sacc
-Version: 0.8
+Version: 0.8.1
 Summary: SACC - the LSST/DESC summary statistic data format library
 Home-page: https://github.com/LSSTDESC/sacc
 Author: LSST DESC
 Author-email: joezuntz@googlemail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -38,17 +38,17 @@
 The [examples directory](https://github.com/LSSTDESC/sacc/tree/master/examples) on github contains ipython notebooks showing various ways of constructing and using sacc data files.
 
 If you have a problem you've not been able to debug, or a feature request/suggestion the you can [open an issue](https://github.com/LSSTDESC/sacc/issues) to discuss it.
 
 Versions
 --------
 
-The current release is [version 0.4.5](https://github.com/LSSTDESC/sacc/releases/tag/0.4.5).
+The current release is [version 0.8](https://github.com/LSSTDESC/sacc/releases/tag/0.8).
 
-You can find a list of [previous releases here](https://github.com/LSSTDESC/sacc/releases).  The releases above 0.2 are all compatible; 0.1 is a previous version of the format.
+You can find a list of [previous releases here](https://github.com/LSSTDESC/sacc/releases).  The releases above 0.2 are all backwards compatible; 0.1 is a previous version of the format.
 
 The master branch includes more recent (non-released) development changes.
 
 
 Citation
 --------
```

### Comparing `sacc-0.8/README.md` & `sacc-0.8.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 The [examples directory](https://github.com/LSSTDESC/sacc/tree/master/examples) on github contains ipython notebooks showing various ways of constructing and using sacc data files.
 
 If you have a problem you've not been able to debug, or a feature request/suggestion the you can [open an issue](https://github.com/LSSTDESC/sacc/issues) to discuss it.
 
 Versions
 --------
 
-The current release is [version 0.4.5](https://github.com/LSSTDESC/sacc/releases/tag/0.4.5).
+The current release is [version 0.8](https://github.com/LSSTDESC/sacc/releases/tag/0.8).
 
-You can find a list of [previous releases here](https://github.com/LSSTDESC/sacc/releases).  The releases above 0.2 are all compatible; 0.1 is a previous version of the format.
+You can find a list of [previous releases here](https://github.com/LSSTDESC/sacc/releases).  The releases above 0.2 are all backwards compatible; 0.1 is a previous version of the format.
 
 The master branch includes more recent (non-released) development changes.
 
 
 Citation
 --------
```

### Comparing `sacc-0.8/doc/Makefile` & `sacc-0.8.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sacc-0.8/doc/format.md` & `sacc-0.8.1/doc/format.md`

 * *Files identical despite different names*

### Comparing `sacc-0.8/doc/source/Makefile` & `sacc-0.8.1/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `sacc-0.8/doc/source/conf.py` & `sacc-0.8.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8/doc/source/intro.rst` & `sacc-0.8.1/doc/source/intro.rst`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/CMB_LSS_read.ipynb` & `sacc-0.8.1/examples/CMB_LSS_read.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/CMB_LSS_write.ipynb` & `sacc-0.8.1/examples/CMB_LSS_write.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/Convert_DES_Sacc.ipynb` & `sacc-0.8.1/examples/Convert_DES_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/Convert_KIDS_Sacc.ipynb` & `sacc-0.8.1/examples/Convert_KIDS_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/Create_Sacc.ipynb` & `sacc-0.8.1/examples/Create_Sacc.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/Create_cluster_count_SACC.ipynb` & `sacc-0.8.1/examples/Create_cluster_count_SACC.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/SACC_for_clusters.ipynb` & `sacc-0.8.1/examples/SACC_for_clusters.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/SACC_read.ipynb` & `sacc-0.8.1/examples/SACC_read.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/SACC_write.ipynb` & `sacc-0.8.1/examples/SACC_write.ipynb`

 * *Files identical despite different names*

### Comparing `sacc-0.8/examples/example-txpipe-sacc1.sacc` & `sacc-0.8.1/examples/example-txpipe-sacc1.sacc`

 * *Files identical despite different names*

### Comparing `sacc-0.8/sacc/covariance.py` & `sacc-0.8.1/sacc/covariance.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8/sacc/data_types.py` & `sacc-0.8.1/sacc/data_types.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8/sacc/sacc.py` & `sacc-0.8.1/sacc/sacc.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8/sacc/tracers.py` & `sacc-0.8.1/sacc/tracers.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                           "If possible use a pre-defined quantity, or "
                           "add to the list.")
         self.name = name
         self.quantity = quantity
         self.metadata = kwargs.pop('metadata', {})
 
     def __init_subclass__(cls, tracer_type):
-        cls._tracer_classes[tracer_type] = cls
+        cls._tracer_classes[tracer_type.lower()] = cls
         cls.tracer_type = tracer_type
 
     @classmethod
     def make(cls, tracer_type, name, *args, **kwargs):
         """
         Select a Tracer subclass based on tracer_type
         and instantiate in instance of it with the remaining
@@ -68,15 +68,15 @@
             The name for this specific tracer.
 
         Returns
         -------
         instance: Tracer object
             An instance of a Tracer subclass
         """
-        subclass = cls._tracer_classes[tracer_type]
+        subclass = cls._tracer_classes[tracer_type.lower()]
         obj = subclass(name, *args, **kwargs)
         return obj
 
     @classmethod
     def to_tables(cls, instance_list):
         """Convert a list of tracers to a list of astropy tables
 
@@ -131,26 +131,26 @@
         Returns
         -------
         tracers: dict
             Dict mapping string names to tracer objects.
         """
         tracers = {}
         # Figure out the different subclasses that are present
-        subclass_names = unique_list(table.meta['SACCCLSS']
+        subclass_names = unique_list(table.meta['SACCCLSS'].lower()
                                      for table in table_list)
         subclasses = [cls._tracer_classes[name]
                       for name in subclass_names]
 
         # For each subclass find the tables representing that subclass.
         # We do it like this because we might want to represent one tracer with
         # multiple tables, or one table can have multiple tracers -
         # it depends on the tracers class and how complicated it is.
         for name, subcls in zip(subclass_names, subclasses):
             subcls_table_list = [table for table in table_list
-                                 if table.meta['SACCCLSS'] == name]
+                                 if table.meta['SACCCLSS'].lower() == name]
             # and ask the subclass to read from those tables.
             tracers.update(subcls.from_tables(subcls_table_list))
         return tracers
 
 
 class MiscTracer(BaseTracer, tracer_type='Misc'):
     """A Tracer type for miscellaneous other data points.
```

### Comparing `sacc-0.8/sacc/utils.py` & `sacc-0.8.1/sacc/utils.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8/sacc/windows.py` & `sacc-0.8.1/sacc/windows.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8/sacc.egg-info/PKG-INFO` & `sacc-0.8.1/sacc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sacc
-Version: 0.8
+Version: 0.8.1
 Summary: SACC - the LSST/DESC summary statistic data format library
 Home-page: https://github.com/LSSTDESC/sacc
 Author: LSST DESC
 Author-email: joezuntz@googlemail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -38,17 +38,17 @@
 The [examples directory](https://github.com/LSSTDESC/sacc/tree/master/examples) on github contains ipython notebooks showing various ways of constructing and using sacc data files.
 
 If you have a problem you've not been able to debug, or a feature request/suggestion the you can [open an issue](https://github.com/LSSTDESC/sacc/issues) to discuss it.
 
 Versions
 --------
 
-The current release is [version 0.4.5](https://github.com/LSSTDESC/sacc/releases/tag/0.4.5).
+The current release is [version 0.8](https://github.com/LSSTDESC/sacc/releases/tag/0.8).
 
-You can find a list of [previous releases here](https://github.com/LSSTDESC/sacc/releases).  The releases above 0.2 are all compatible; 0.1 is a previous version of the format.
+You can find a list of [previous releases here](https://github.com/LSSTDESC/sacc/releases).  The releases above 0.2 are all backwards compatible; 0.1 is a previous version of the format.
 
 The master branch includes more recent (non-released) development changes.
 
 
 Citation
 --------
```

### Comparing `sacc-0.8/sacc.egg-info/SOURCES.txt` & `sacc-0.8.1/sacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sacc-0.8/setup.py` & `sacc-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8/test/make_test_data.py` & `sacc-0.8.1/test/make_test_data.py`

 * *Files identical despite different names*

### Comparing `sacc-0.8/test/test_sacc2.py` & `sacc-0.8.1/test/test_sacc2.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,14 +329,21 @@
     T2 = sacc.BaseTracer.make('NZ', 'tracer2', z, Nz2,
                               quantity='galaxy_shear',
                               spin=2,
                               metadata=md2)
     assert T1.metadata == md1
     assert T2.metadata == md2
 
+    # check that we can make a tracer using lower case
+    T3 = sacc.BaseTracer.make('nz', 'tracer2', z, Nz2,
+                              quantity='galaxy_shear',
+                              spin=2,
+                              metadata=md2)
+    assert T3.metadata == md2
+
     tables = sacc.BaseTracer.to_tables([T1, T2])
     D = sacc.BaseTracer.from_tables(tables)
 
     T1a = D['tracer1']
     T2a = D['tracer2']
     assert T1a.metadata == md1
     assert T2a.metadata == md2
@@ -354,15 +361,15 @@
     Nz2 = 2*z
     T1 = sacc.BaseTracer.make('NZ', 'tracer1', z, Nz1,
                               quantity='galaxy_convergence')
     T2 = sacc.BaseTracer.make('NZ', 'tracer2', z, Nz2,
                               quantity='galaxy_shear', metadata=md1)
 
     M1 = sacc.BaseTracer.make("Misc", "sample1", metadata=md2)
-    M2 = sacc.BaseTracer.make("Misc", "sample2", metadata=md3)
+    M2 = sacc.BaseTracer.make("mISC", "sample2", metadata=md3)
 
     tables = sacc.BaseTracer.to_tables([T1, M1, T2, M2])
     recovered = sacc.BaseTracer.from_tables(tables)
     assert recovered['sample1'].metadata['rank'] == 'duke'
     assert recovered['sample2'].metadata['robes'] == 78
     assert np.all(recovered['tracer1'].nz == Nz1)
     assert recovered['tracer2'].metadata['potato'] == 'never'
@@ -418,17 +425,17 @@
 def test_keep_remove():
     s = sacc.Sacc()
 
     # Tracer
     z = np.arange(0., 1.0, 0.01)
     nz = (z-0.5)**2/0.1**2
     s.add_tracer('NZ', 'source_0', z, nz)
-    s.add_tracer('NZ', 'source_1', z, nz,
+    s.add_tracer('nZ', 'source_1', z, nz,
                  quantity='galaxy_shear', spin=2)
-    s.add_tracer('NZ', 'source_2', z, nz,
+    s.add_tracer('nz', 'source_2', z, nz,
                  quantity='cluster_density')
 
     for i in range(20):
         ee = 0.1 * i
         tracers = ('source_0', 'source_0')
         s.add_data_point(sacc.standard_types.galaxy_shear_cl_ee,
                          tracers, ee, ell=10.0*i)
@@ -747,15 +754,15 @@
     bandpass = np.ones(100)
     z = np.arange(0., 1.0, 0.01)
     nz = (z-0.5)**2/0.1**2
 
     # Tracer
     s.add_tracer('NZ', 'gc', z, nz)
     s.add_tracer('NuMap', 'cmbp', 2, nu, bandpass, ell, beam)
-    s.add_tracer('Map', 'sz', 0, ell, beam)
+    s.add_tracer('maP', 'sz', 0, ell, beam)
 
     # Window
     ells_large = np.arange(n_ell_large)
     window_single = np.zeros([n_ell, n_ell_large])
     for i in range(n_ell):
         window_single[i, i * d_ell: (i + 1) * d_ell] = 1.
     wins = sacc.BandpowerWindow(ells_large, window_single.T)
@@ -848,15 +855,15 @@
     s = sacc.Sacc()
 
     # Tracer
     z = np.linspace(0., 1.0, 101)
     nz = np.expand_dims((z-0.5)**2/0.1**2, 0)
     ens = qp.Ensemble(qp.interp, data=dict(xvals=z, yvals=nz))
     ens.set_ancil(dict(modes = ens.mode(z)))
-    s.add_tracer('QPNZ', 'source_0', ens)
+    s.add_tracer('QpnZ', 'source_0', ens)
 
     for i in range(20):
         ee = 0.1 * i
         tracers = ('source_0', 'source_0')
         s.add_data_point(sacc.standard_types.galaxy_shear_cl_ee,
                          tracers, ee, ell=10.0*i)
```

