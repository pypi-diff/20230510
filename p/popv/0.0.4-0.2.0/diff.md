# Comparing `tmp/popv-0.0.4.tar.gz` & `tmp/popv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/popv-0.0.4.tar", last modified: Tue Jul 27 00:19:06 2021, max compression
+gzip compressed data, was "popv-0.2.0.tar", max compression
```

## Comparing `popv-0.0.4.tar` & `popv-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxr-xr-x   0 alec      (5204) czb       (5000)        0 2021-07-27 00:19:06.000000 popv-0.0.4/
--rw-r--r--   0 alec      (5204) czb       (5000)      403 2021-07-27 00:19:06.000000 popv-0.0.4/PKG-INFO
--rw-r--r--   0 alec      (5204) czb       (5000)      237 2021-07-26 23:32:17.000000 popv-0.0.4/README.md
-drwxr-xr-x   0 alec      (5204) czb       (5000)        0 2021-07-27 00:19:06.000000 popv-0.0.4/popv/
--rw-r--r--   0 alec      (5204) czb       (5000)    32096 2021-07-26 17:28:46.000000 popv-0.0.4/popv/__init__.py
-drwxr-xr-x   0 alec      (5204) czb       (5000)        0 2021-07-27 00:19:06.000000 popv-0.0.4/popv.egg-info/
--rw-r--r--   0 alec      (5204) czb       (5000)      403 2021-07-27 00:19:06.000000 popv-0.0.4/popv.egg-info/PKG-INFO
--rw-r--r--   0 alec      (5204) czb       (5000)      201 2021-07-27 00:19:06.000000 popv-0.0.4/popv.egg-info/SOURCES.txt
--rw-r--r--   0 alec      (5204) czb       (5000)        1 2021-07-27 00:19:06.000000 popv-0.0.4/popv.egg-info/dependency_links.txt
--rw-r--r--   0 alec      (5204) czb       (5000)        1 2021-07-26 19:31:44.000000 popv-0.0.4/popv.egg-info/not-zip-safe
--rw-r--r--   0 alec      (5204) czb       (5000)      281 2021-07-27 00:19:06.000000 popv-0.0.4/popv.egg-info/requires.txt
--rw-r--r--   0 alec      (5204) czb       (5000)        5 2021-07-27 00:19:06.000000 popv-0.0.4/popv.egg-info/top_level.txt
--rw-r--r--   0 alec      (5204) czb       (5000)       38 2021-07-27 00:19:06.000000 popv-0.0.4/setup.cfg
--rw-r--r--   0 alec      (5204) czb       (5000)     1078 2021-07-27 00:18:49.000000 popv-0.0.4/setup.py
+-rw-r--r--   0        0        0     1067 2023-01-27 08:23:56.770098 popv-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5919 2023-02-04 09:31:21.059876 popv-0.2.0/README.md
+-rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.2.0/popv/__init__.py
+-rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.2.0/popv/_settings.py
+-rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.2.0/popv/_utils.py
+-rw-r--r--   0        0        0      475 2023-02-04 09:31:22.143889 popv-0.2.0/popv/algorithms/__init__.py
+-rw-r--r--   0        0        0     3876 2023-03-23 00:04:43.169426 popv-0.2.0/popv/algorithms/_bbknn.py
+-rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.2.0/popv/algorithms/_celltypist.py
+-rw-r--r--   0        0        0     7453 2023-05-09 13:10:44.713840 popv-0.2.0/popv/algorithms/_onclass.py
+-rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.2.0/popv/algorithms/_rf.py
+-rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.2.0/popv/algorithms/_scaffold_algorithm.py
+-rw-r--r--   0        0        0     3525 2023-02-17 07:50:33.768775 popv-0.2.0/popv/algorithms/_scanorama.py
+-rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.2.0/popv/algorithms/_scanvi.py
+-rw-r--r--   0        0        0     6697 2023-03-23 00:17:40.248214 popv-0.2.0/popv/algorithms/_scvi.py
+-rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.2.0/popv/algorithms/_svm.py
+-rw-r--r--   0        0        0    10981 2023-03-11 22:16:34.706423 popv-0.2.0/popv/annotation.py
+-rw-r--r--   0        0        0    16724 2023-03-29 19:07:11.783969 popv-0.2.0/popv/preprocessing.py
+-rw-r--r--   0        0        0     2643 2023-02-24 22:34:31.417602 popv-0.2.0/popv/reproducibility/_accuracy.py
+-rw-r--r--   0        0        0    12874 2023-03-08 22:06:43.264685 popv-0.2.0/popv/reproducibility/_alluvial.py
+-rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.2.0/popv/visualization.py
+-rw-r--r--   0        0        0     2376 2023-05-09 13:13:02.619397 popv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7615 2023-05-09 13:13:10.227956 popv-0.2.0/setup.py
+-rw-r--r--   0        0        0     8125 2023-05-09 13:13:10.228447 popv-0.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

