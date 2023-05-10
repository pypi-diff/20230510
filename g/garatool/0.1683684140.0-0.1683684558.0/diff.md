# Comparing `tmp/garatool-0.1683684140.0.tar.gz` & `tmp/garatool-0.1683684558.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683684140.0.tar", last modified: Wed May 10 02:02:20 2023, max compression
+gzip compressed data, was "garatool-0.1683684558.0.tar", last modified: Wed May 10 02:09:20 2023, max compression
```

## Comparing `garatool-0.1683684140.0.tar` & `garatool-0.1683684558.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 02:02:20.795755 garatool-0.1683684140.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-10 02:02:20.795436 garatool-0.1683684140.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683684140.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 02:02:20.792550 garatool-0.1683684140.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     6424 2023-05-10 02:02:05.000000 garatool-0.1683684140.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683684140.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 02:02:20.794840 garatool-0.1683684140.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-10 02:02:20.000000 garatool-0.1683684140.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-10 02:02:20.000000 garatool-0.1683684140.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-10 02:02:20.000000 garatool-0.1683684140.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-10 02:02:20.000000 garatool-0.1683684140.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-10 02:02:20.000000 garatool-0.1683684140.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-10 02:02:20.795850 garatool-0.1683684140.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683684140.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 02:09:20.267911 garatool-0.1683684558.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-10 02:09:20.267367 garatool-0.1683684558.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683684558.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 02:09:20.245966 garatool-0.1683684558.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     6418 2023-05-10 02:09:06.000000 garatool-0.1683684558.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683684558.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 02:09:20.262399 garatool-0.1683684558.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-10 02:09:19.000000 garatool-0.1683684558.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-10 02:09:20.000000 garatool-0.1683684558.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-10 02:09:19.000000 garatool-0.1683684558.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-10 02:09:19.000000 garatool-0.1683684558.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-10 02:09:19.000000 garatool-0.1683684558.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-10 02:09:20.269381 garatool-0.1683684558.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683684558.0/setup.py
```

### Comparing `garatool-0.1683684140.0/garatool/__init__.py` & `garatool-0.1683684558.0/garatool/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-b', '--board', type=Board, choices=list(Board), help='Select board type')
 parser.add_argument('-p', '--port', help = 'Select the COM port')
 parser.add_argument('-t', '--tag', type=str, help="Select firmware tag", default='dev')
-parser.add_argument('-i', '--imei', type=str, help='IMEI code', default='NOIMEI')
+parser.add_argument('-i', '--imei', type=str, help='IMEI code', default='')
 parser.add_argument('-n', '--name', help='Device name', default='Creator Device')
 parser.add_argument('-s', '--serial', action='store_true', help='Enable Serial debug')
 parser.add_argument('-u', '--upload', help='(Admin) Publish firmware tag',action='store_true')
 parser.add_argument('-k', '--key', help='(Admin) With secret key', default='')
 parser.add_argument('-r', '--root', help='(Admin) Location of firmware', default='')
 parser.add_argument('-d', '--download', help="(Admin) Download tagged firmware", action='store_true')
```

### Comparing `garatool-0.1683684140.0/setup.py` & `garatool-0.1683684558.0/setup.py`

 * *Files identical despite different names*

