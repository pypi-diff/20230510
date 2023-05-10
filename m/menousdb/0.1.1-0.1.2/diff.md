# Comparing `tmp/menousdb-0.1.1.macosx-10.9-universal2.tar.gz` & `tmp/menousdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menousdb-0.1.1.macosx-10.9-universal2.tar", last modified: Wed May 10 12:33:37 2023, max compression
+gzip compressed data, was "menousdb-0.1.2.tar", last modified: Wed May 10 12:36:00 2023, max compression
```

## Comparing `menousdb-0.1.1.macosx-10.9-universal2.tar` & `menousdb-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,13 @@
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.453499 ./
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.455560 ./Users/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.455926 ./Users/sumanlaskar/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.457249 ./Users/sumanlaskar/Documents/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.457637 ./Users/sumanlaskar/Documents/Menous Technologies/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.457902 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.459997 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.460418 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.460773 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.468078 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.572119 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.490305 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb/
--rw-r--r--   0 sumanlaskar   (501) staff       (20)     8305 2023-05-10 12:22:11.000000 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb/__init__.py
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.508732 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb/__pycache__/
--rw-r--r--   0 sumanlaskar   (501) staff       (20)    10056 2023-05-10 12:33:37.508423 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:33:37.585622 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb-0.1.1-py3.11.egg-info/
--rw-r--r--   0 sumanlaskar   (501) staff       (20)     2334 2023-05-10 12:33:37.168608 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb-0.1.1-py3.11.egg-info/PKG-INFO
--rw-r--r--   0 sumanlaskar   (501) staff       (20)      198 2023-05-10 12:33:37.192008 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb-0.1.1-py3.11.egg-info/SOURCES.txt
--rw-r--r--   0 sumanlaskar   (501) staff       (20)        1 2023-05-10 12:33:37.169636 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb-0.1.1-py3.11.egg-info/dependency_links.txt
--rw-r--r--   0 sumanlaskar   (501) staff       (20)        9 2023-05-10 12:33:37.170488 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb-0.1.1-py3.11.egg-info/requires.txt
--rw-r--r--   0 sumanlaskar   (501) staff       (20)        9 2023-05-10 12:33:37.171750 ./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb-0.1.1-py3.11.egg-info/top_level.txt
+drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:36:00.866471 menousdb-0.1.2/
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     2334 2023-05-10 12:36:00.864407 menousdb-0.1.2/PKG-INFO
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)      595 2023-05-10 12:23:09.000000 menousdb-0.1.2/README.md
+drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:36:00.855256 menousdb-0.1.2/menousdb/
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     8305 2023-05-10 12:22:11.000000 menousdb-0.1.2/menousdb/__init__.py
+drwxr-xr-x   0 sumanlaskar   (501) staff       (20)        0 2023-05-10 12:36:00.863818 menousdb-0.1.2/menousdb.egg-info/
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     2334 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/PKG-INFO
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)      198 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)        1 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)        9 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/requires.txt
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)        9 2023-05-10 12:36:00.000000 menousdb-0.1.2/menousdb.egg-info/top_level.txt
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)       38 2023-05-10 12:36:00.866722 menousdb-0.1.2/setup.cfg
+-rw-r--r--   0 sumanlaskar   (501) staff       (20)     2116 2023-05-10 12:35:45.000000 menousdb-0.1.2/setup.py
```

### Comparing `./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb/__init__.py` & `menousdb-0.1.2/menousdb/__init__.py`

 * *Files identical despite different names*

### Comparing `./Users/sumanlaskar/Documents/Menous Technologies/Company Products/Menous DB/.venv/lib/python3.11/site-packages/menousdb-0.1.1-py3.11.egg-info/PKG-INFO` & `menousdb-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: menousdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A SDK for Menous DB
 Author: Snehashish Laskar
 Author-email: snehashish.laskar@gmail.com
 License: 
         MIT License
         
         Copyright (c) 2022 Snehashish Laskar
```

