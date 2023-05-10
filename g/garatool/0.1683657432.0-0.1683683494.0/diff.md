# Comparing `tmp/garatool-0.1683657432.0.tar.gz` & `tmp/garatool-0.1683683494.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683657432.0.tar", last modified: Tue May  9 18:37:12 2023, max compression
+gzip compressed data, was "garatool-0.1683683494.0.tar", last modified: Wed May 10 01:51:35 2023, max compression
```

## Comparing `garatool-0.1683657432.0.tar` & `garatool-0.1683683494.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 18:37:12.385780 garatool-0.1683657432.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 18:37:12.385486 garatool-0.1683657432.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683657432.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 18:37:12.382584 garatool-0.1683657432.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     6005 2023-05-09 18:22:07.000000 garatool-0.1683657432.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683657432.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 18:37:12.384972 garatool-0.1683657432.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 18:37:12.000000 garatool-0.1683657432.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 18:37:12.385873 garatool-0.1683657432.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683657432.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 01:51:35.092817 garatool-0.1683683494.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-10 01:51:35.092444 garatool-0.1683683494.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683683494.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 01:51:35.086882 garatool-0.1683683494.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     6123 2023-05-10 01:45:20.000000 garatool-0.1683683494.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683683494.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-10 01:51:35.091619 garatool-0.1683683494.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-10 01:51:34.000000 garatool-0.1683683494.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-10 01:51:35.000000 garatool-0.1683683494.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-10 01:51:34.000000 garatool-0.1683683494.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-10 01:51:34.000000 garatool-0.1683683494.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-10 01:51:34.000000 garatool-0.1683683494.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-10 01:51:35.092918 garatool-0.1683683494.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683683494.0/setup.py
```

### Comparing `garatool-0.1683657432.0/garatool/__init__.py` & `garatool-0.1683683494.0/garatool/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,16 +206,18 @@
             , 'rb').read()
             fws[file] = content
         br.files = fws
 
 
 
 
-
+    print(step('Downloading firmware ...'))
     br = request_firmware_build(br)
     # Start burning firmware
+    print(step('Programming device ...'))
     program_device(br)
 
     if parsed.serial:
-        if platform.system() == 'Darwin':
+        print(platform.system())
+        if platform.system() == 'darwin':
             os.system('say start')
             os.system(f'screen {parsed.port} 115200')
```

### Comparing `garatool-0.1683657432.0/setup.py` & `garatool-0.1683683494.0/setup.py`

 * *Files identical despite different names*

