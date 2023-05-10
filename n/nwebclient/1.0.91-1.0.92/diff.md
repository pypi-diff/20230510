# Comparing `tmp/nwebclient-1.0.91.tar.gz` & `tmp/nwebclient-1.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.91.tar", last modified: Wed May 10 08:34:02 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.92.tar", last modified: Wed May 10 08:35:48 2023, max compression
```

## Comparing `nwebclient-1.0.91.tar` & `nwebclient-1.0.92.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:34:02.440755 nwebclient-1.0.91/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.91/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-10 08:34:02.440755 nwebclient-1.0.91/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.91/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:34:02.440755 nwebclient-1.0.91/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6457 2023-05-09 14:11:24.000000 nwebclient-1.0.91/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.91/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.91/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    13279 2023-05-10 08:33:49.000000 nwebclient-1.0.91/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.91/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.91/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:34:02.440755 nwebclient-1.0.91/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-10 08:34:02.000000 nwebclient-1.0.91/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-10 08:34:02.000000 nwebclient-1.0.91/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-10 08:34:02.000000 nwebclient-1.0.91/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-10 08:34:02.000000 nwebclient-1.0.91/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-10 08:34:02.000000 nwebclient-1.0.91/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-10 08:34:02.000000 nwebclient-1.0.91/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-10 08:34:02.440755 nwebclient-1.0.91/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-10 08:33:59.000000 nwebclient-1.0.91/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:35:48.409059 nwebclient-1.0.92/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.92/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-10 08:35:48.409059 nwebclient-1.0.92/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.92/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:35:48.409059 nwebclient-1.0.92/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6457 2023-05-09 14:11:24.000000 nwebclient-1.0.92/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.92/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-09 12:58:28.000000 nwebclient-1.0.92/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    13279 2023-05-10 08:35:36.000000 nwebclient-1.0.92/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.92/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.92/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-10 08:35:48.409059 nwebclient-1.0.92/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-10 08:35:48.000000 nwebclient-1.0.92/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-10 08:35:48.409059 nwebclient-1.0.92/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-10 08:35:46.000000 nwebclient-1.0.92/setup.py
```

### Comparing `nwebclient-1.0.91/LICENSE` & `nwebclient-1.0.92/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.91/PKG-INFO` & `nwebclient-1.0.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.91
+Version: 1.0.92
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.91/README.md` & `nwebclient-1.0.92/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.91/nwebclient/__init__.py` & `nwebclient-1.0.92/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.91/nwebclient/__main__.py` & `nwebclient-1.0.92/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.91/nwebclient/crypt.py` & `nwebclient-1.0.92/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.91/nwebclient/sd.py` & `nwebclient-1.0.92/nwebclient/sd.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -241,26 +241,26 @@
       JobFetch(NWebClient(...), 42)  
       
       npy-ticker nwebclient.sd.JobFetch:42
     """
     key = None
     def __init__(self, nwebclient=None, group=None):
         super().__init__("jobfetch",60*60*23) 
-        from cryptography.fernet import Fernet
-        from nwebclient import NWebClient
         self.nweb = nwebclient
         self.group = group
     def configure(self, arg):
+        from nwebclient import NWebClient
         self.nweb = NWebClient()
         self.group = arg
     def execute(self):
         docs = self.nweb.docs('group_id='+str(self.group))
         for doc in docs:
             self.download(doc)
     def decrypt(self, file):
+        from cryptography.fernet import Fernet
         fernet = Fernet(self.key)
         with open(file, 'rb') as f:
             original = f.read()
         encrypted = fernet.decrypt(original)
         with open(file, 'wb') as encrypted_file:
             encrypted_file.write(encrypted)
     def download(self, doc):
```

### Comparing `nwebclient-1.0.91/nwebclient/sdb.py` & `nwebclient-1.0.92/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.91/nwebclient/ticker.py` & `nwebclient-1.0.92/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.91/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.92/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.91
+Version: 1.0.92
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.91/setup.py` & `nwebclient-1.0.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.91",
+    version="1.0.92",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

