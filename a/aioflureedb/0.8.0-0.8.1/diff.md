# Comparing `tmp/aioflureedb-0.8.0.tar.gz` & `tmp/aioflureedb-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioflureedb-0.8.0.tar", last modified: Tue Apr 18 10:23:15 2023, max compression
+gzip compressed data, was "aioflureedb-0.8.1.tar", last modified: Wed May 10 09:49:34 2023, max compression
```

## Comparing `aioflureedb-0.8.0.tar` & `aioflureedb-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/
--rw-rw-r--   0 rob       (1000) rob       (1000)      774 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)     1798 2023-03-30 05:22:33.000000 aioflureedb-0.8.0/README.md
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/aioflureedb/
--rw-r--r--   0 rob       (1000) rob       (1000)    74739 2023-04-18 07:49:10.000000 aioflureedb-0.8.0/aioflureedb/__init__.py
--rw-rw-r--   0 rob       (1000) rob       (1000)     6874 2023-04-14 14:10:59.000000 aioflureedb-0.8.0/aioflureedb/__main__.py
--rw-r--r--   0 rob       (1000) rob       (1000)    25925 2023-04-14 14:07:21.000000 aioflureedb-0.8.0/aioflureedb/domain_api.py
--rw-r--r--   0 rob       (1000) rob       (1000)     7030 2023-04-14 14:06:52.000000 aioflureedb-0.8.0/aioflureedb/signing.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/aioflureedb.egg-info/
--rw-r--r--   0 rob       (1000) rob       (1000)      774 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/PKG-INFO
--rw-r--r--   0 rob       (1000) rob       (1000)      289 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/SOURCES.txt
--rw-r--r--   0 rob       (1000) rob       (1000)        1 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/dependency_links.txt
--rw-r--r--   0 rob       (1000) rob       (1000)       66 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/requires.txt
--rw-r--r--   0 rob       (1000) rob       (1000)       12 2023-04-18 10:23:15.000000 aioflureedb-0.8.0/aioflureedb.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-04-18 10:23:15.622116 aioflureedb-0.8.0/setup.cfg
--rw-r--r--   0 rob       (1000) rob       (1000)     1148 2023-04-18 10:21:47.000000 aioflureedb-0.8.0/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      774 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1798 2023-03-30 05:22:33.000000 aioflureedb-0.8.1/README.md
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/aioflureedb/
+-rw-r--r--   0 rob       (1000) rob       (1000)    74993 2023-05-10 09:46:00.000000 aioflureedb-0.8.1/aioflureedb/__init__.py
+-rw-rw-r--   0 rob       (1000) rob       (1000)     6874 2023-04-14 14:10:59.000000 aioflureedb-0.8.1/aioflureedb/__main__.py
+-rw-r--r--   0 rob       (1000) rob       (1000)    25925 2023-04-14 14:07:21.000000 aioflureedb-0.8.1/aioflureedb/domain_api.py
+-rw-r--r--   0 rob       (1000) rob       (1000)     7030 2023-04-14 14:06:52.000000 aioflureedb-0.8.1/aioflureedb/signing.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/aioflureedb.egg-info/
+-rw-r--r--   0 rob       (1000) rob       (1000)      774 2023-05-10 09:49:33.000000 aioflureedb-0.8.1/aioflureedb.egg-info/PKG-INFO
+-rw-r--r--   0 rob       (1000) rob       (1000)      289 2023-05-10 09:49:34.000000 aioflureedb-0.8.1/aioflureedb.egg-info/SOURCES.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)        1 2023-05-10 09:49:33.000000 aioflureedb-0.8.1/aioflureedb.egg-info/dependency_links.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)       66 2023-05-10 09:49:34.000000 aioflureedb-0.8.1/aioflureedb.egg-info/requires.txt
+-rw-r--r--   0 rob       (1000) rob       (1000)       12 2023-05-10 09:49:34.000000 aioflureedb-0.8.1/aioflureedb.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-10 09:49:34.343709 aioflureedb-0.8.1/setup.cfg
+-rw-r--r--   0 rob       (1000) rob       (1000)     1148 2023-05-10 09:46:09.000000 aioflureedb-0.8.1/setup.py
```

### Comparing `aioflureedb-0.8.0/PKG-INFO` & `aioflureedb-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioflureedb
-Version: 0.8.0
+Version: 0.8.1
 Summary: Asynchonous library for usage of the FlureeDB API
 Home-page: https://github.com/pibara/aioflureedb
 Author: Rob J Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql sparql graphql
 Platform: UNKNOWN
```

### Comparing `aioflureedb-0.8.0/README.md` & `aioflureedb-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.8.0/aioflureedb/__init__.py` & `aioflureedb-0.8.1/aioflureedb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,20 @@
         if self.ready_field is None:
             print("WARNING: no ready for this endpoint", file=sys.stderr)
             return
         while True:
             try:
                 obj = await self()
                 if obj[self.ready_field]:
-                    return
+                    # nasty hack, this shouldn't be needed
+                    if "status" not in obj:
+                        return
+                    if obj["status"]:
+                        return
+                    print("NOTICE: Fluree returns ready, but status not set")
             except FlureeHttpError as ex:
                 print(ex)
             except aiohttp.client_exceptions.ClientConnectorError:
                 pass
             await asyncio.sleep(2)
```

### Comparing `aioflureedb-0.8.0/aioflureedb/__main__.py` & `aioflureedb-0.8.1/aioflureedb/__main__.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.8.0/aioflureedb/domain_api.py` & `aioflureedb-0.8.1/aioflureedb/domain_api.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.8.0/aioflureedb/signing.py` & `aioflureedb-0.8.1/aioflureedb/signing.py`

 * *Files identical despite different names*

### Comparing `aioflureedb-0.8.0/aioflureedb.egg-info/PKG-INFO` & `aioflureedb-0.8.1/aioflureedb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioflureedb
-Version: 0.8.0
+Version: 0.8.1
 Summary: Asynchonous library for usage of the FlureeDB API
 Home-page: https://github.com/pibara/aioflureedb
 Author: Rob J Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: flureedb fluree flureeql sparql graphql
 Platform: UNKNOWN
```

### Comparing `aioflureedb-0.8.0/setup.py` & `aioflureedb-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from sys import platform
 here = path.abspath(path.dirname(__file__))
 
 requirements = ["starkbank-ecdsa>=2.0.3", "aiohttp", "base58"]
 
 setup(
     name='aioflureedb',
-    version='0.8.0',
+    version='0.8.1',
     description='Asynchonous library for usage of the FlureeDB API',
     long_description="""An asynchonous client library for communicating with a FlureeDB server, making signed transactions and queries.
     """,
     url='https://github.com/pibara/aioflureedb',
     author='Rob J Meijer',
     author_email='pibara@gmail.com',
     license='BSD',
```

