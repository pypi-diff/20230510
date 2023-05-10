# Comparing `tmp/dask-bigquery-2022.5.0.tar.gz` & `tmp/dask-bigquery-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-bigquery-2022.5.0.tar", last modified: Mon May  2 18:33:28 2022, max compression
+gzip compressed data, was "dask-bigquery-2023.5.0.tar", last modified: Wed May 10 18:11:30 2023, max compression
```

## Comparing `dask-bigquery-2022.5.0.tar` & `dask-bigquery-2023.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ncclementi   (501) staff       (20)        0 2022-05-02 18:33:28.102209 dask-bigquery-2022.5.0/
--rw-r--r--   0 ncclementi   (501) staff       (20)     1514 2021-08-05 20:57:06.000000 dask-bigquery-2022.5.0/LICENSE
--rw-r--r--   0 ncclementi   (501) staff       (20)      133 2021-10-28 22:11:06.000000 dask-bigquery-2022.5.0/MANIFEST.in
--rw-r--r--   0 ncclementi   (501) staff       (20)     2174 2022-05-02 18:33:28.102260 dask-bigquery-2022.5.0/PKG-INFO
--rw-r--r--   0 ncclementi   (501) staff       (20)     1936 2021-12-13 18:36:57.000000 dask-bigquery-2022.5.0/README.md
-drwxr-xr-x   0 ncclementi   (501) staff       (20)        0 2022-05-02 18:33:28.101066 dask-bigquery-2022.5.0/dask_bigquery/
--rw-r--r--   0 ncclementi   (501) staff       (20)       54 2022-05-02 18:27:23.000000 dask-bigquery-2022.5.0/dask_bigquery/__init__.py
--rw-r--r--   0 ncclementi   (501) staff       (20)     6352 2022-04-20 16:23:10.000000 dask-bigquery-2022.5.0/dask_bigquery/core.py
-drwxr-xr-x   0 ncclementi   (501) staff       (20)        0 2022-05-02 18:33:28.101990 dask-bigquery-2022.5.0/dask_bigquery/tests/
--rw-r--r--   0 ncclementi   (501) staff       (20)     3588 2022-04-20 16:23:10.000000 dask-bigquery-2022.5.0/dask_bigquery/tests/test_core.py
-drwxr-xr-x   0 ncclementi   (501) staff       (20)        0 2022-05-02 18:33:28.101886 dask-bigquery-2022.5.0/dask_bigquery.egg-info/
--rw-r--r--   0 ncclementi   (501) staff       (20)     2174 2022-05-02 18:33:27.000000 dask-bigquery-2022.5.0/dask_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 ncclementi   (501) staff       (20)      366 2022-05-02 18:33:28.000000 dask-bigquery-2022.5.0/dask_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 ncclementi   (501) staff       (20)        1 2022-05-02 18:33:27.000000 dask-bigquery-2022.5.0/dask_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 ncclementi   (501) staff       (20)        1 2022-05-02 18:33:27.000000 dask-bigquery-2022.5.0/dask_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 ncclementi   (501) staff       (20)      144 2022-05-02 18:33:28.000000 dask-bigquery-2022.5.0/dask_bigquery.egg-info/requires.txt
--rw-r--r--   0 ncclementi   (501) staff       (20)       14 2022-05-02 18:33:28.000000 dask-bigquery-2022.5.0/dask_bigquery.egg-info/top_level.txt
--rw-r--r--   0 ncclementi   (501) staff       (20)       82 2021-10-28 22:11:06.000000 dask-bigquery-2022.5.0/requirements.txt
--rw-r--r--   0 ncclementi   (501) staff       (20)      106 2022-05-02 18:33:28.102446 dask-bigquery-2022.5.0/setup.cfg
--rw-r--r--   0 ncclementi   (501) staff       (20)      654 2022-05-02 18:27:06.000000 dask-bigquery-2022.5.0/setup.py
+drwxr-xr-x   0 ncclementi   (501) staff       (20)        0 2023-05-10 18:11:30.538303 dask-bigquery-2023.5.0/
+-rw-r--r--   0 ncclementi   (501) staff       (20)     1514 2021-08-05 20:57:06.000000 dask-bigquery-2023.5.0/LICENSE
+-rw-r--r--   0 ncclementi   (501) staff       (20)      133 2021-10-28 22:11:06.000000 dask-bigquery-2023.5.0/MANIFEST.in
+-rw-r--r--   0 ncclementi   (501) staff       (20)     3683 2023-05-10 18:11:30.538367 dask-bigquery-2023.5.0/PKG-INFO
+-rw-r--r--   0 ncclementi   (501) staff       (20)     3446 2023-05-10 16:54:19.000000 dask-bigquery-2023.5.0/README.md
+drwxr-xr-x   0 ncclementi   (501) staff       (20)        0 2023-05-10 18:11:30.537287 dask-bigquery-2023.5.0/dask_bigquery/
+-rw-r--r--   0 ncclementi   (501) staff       (20)       62 2023-05-10 18:03:32.000000 dask-bigquery-2023.5.0/dask_bigquery/__init__.py
+-rw-r--r--   0 ncclementi   (501) staff       (20)    12446 2023-05-09 17:54:09.000000 dask-bigquery-2023.5.0/dask_bigquery/core.py
+drwxr-xr-x   0 ncclementi   (501) staff       (20)        0 2023-05-10 18:11:30.538187 dask-bigquery-2023.5.0/dask_bigquery/tests/
+-rw-r--r--   0 ncclementi   (501) staff       (20)     8275 2023-05-09 17:54:09.000000 dask-bigquery-2023.5.0/dask_bigquery/tests/test_core.py
+drwxr-xr-x   0 ncclementi   (501) staff       (20)        0 2023-05-10 18:11:30.538061 dask-bigquery-2023.5.0/dask_bigquery.egg-info/
+-rw-r--r--   0 ncclementi   (501) staff       (20)     3683 2023-05-10 18:11:30.000000 dask-bigquery-2023.5.0/dask_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 ncclementi   (501) staff       (20)      366 2023-05-10 18:11:30.000000 dask-bigquery-2023.5.0/dask_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 ncclementi   (501) staff       (20)        1 2023-05-10 18:11:30.000000 dask-bigquery-2023.5.0/dask_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 ncclementi   (501) staff       (20)        1 2022-05-02 18:33:27.000000 dask-bigquery-2023.5.0/dask_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 ncclementi   (501) staff       (20)      133 2023-05-10 18:11:30.000000 dask-bigquery-2023.5.0/dask_bigquery.egg-info/requires.txt
+-rw-r--r--   0 ncclementi   (501) staff       (20)       14 2023-05-10 18:11:30.000000 dask-bigquery-2023.5.0/dask_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 ncclementi   (501) staff       (20)       88 2023-05-09 17:54:09.000000 dask-bigquery-2023.5.0/requirements.txt
+-rw-r--r--   0 ncclementi   (501) staff       (20)      106 2023-05-10 18:11:30.538592 dask-bigquery-2023.5.0/setup.cfg
+-rw-r--r--   0 ncclementi   (501) staff       (20)      619 2023-05-10 18:03:32.000000 dask-bigquery-2023.5.0/setup.py
```

### Comparing `dask-bigquery-2022.5.0/LICENSE` & `dask-bigquery-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-bigquery-2022.5.0/setup.py` & `dask-bigquery-2023.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dask-bigquery",
-    version="2022.05.0",
-    description="Dask + BigQuery intergration",
+    version="2023.05.0",
+    description="Dask + BigQuery integration",
     license="BSD",
     packages=["dask_bigquery"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     install_requires=open("requirements.txt").read().strip().split("\n"),
-    extras_require={
-        "test": ["pytest", "pandas-gbq<=0.15", "distributed", "google-auth>=1.30.0"]
-    },
+    extras_require={"test": ["pytest", "distributed", "google-auth>=1.30.0"]},
     include_package_data=True,
     zip_safe=False,
 )
```

