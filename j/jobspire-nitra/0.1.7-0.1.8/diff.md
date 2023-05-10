# Comparing `tmp/jobspire_nitra-0.1.7.tar.gz` & `tmp/jobspire_nitra-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobspire_nitra-0.1.7.tar", last modified: Thu May  4 14:03:53 2023, max compression
+gzip compressed data, was "jobspire_nitra-0.1.8.tar", last modified: Wed May 10 12:11:12 2023, max compression
```

## Comparing `jobspire_nitra-0.1.7.tar` & `jobspire_nitra-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-04 14:03:53.913815 jobspire_nitra-0.1.7/
--rw-r--r--   0 niko      (1000) niko      (1000)     1055 2023-05-04 13:55:48.000000 jobspire_nitra-0.1.7/LICENSE
--rw-r--r--   0 niko      (1000) niko      (1000)     1344 2023-05-04 14:03:53.913815 jobspire_nitra-0.1.7/PKG-INFO
--rw-r--r--   0 niko      (1000) niko      (1000)     1047 2023-05-04 13:59:23.000000 jobspire_nitra-0.1.7/README.rst
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-04 14:03:53.911815 jobspire_nitra-0.1.7/jobspire_nitra/
--rw-r--r--   0 niko      (1000) niko      (1000)       39 2023-05-04 13:55:48.000000 jobspire_nitra-0.1.7/jobspire_nitra/__init__.py
--rw-r--r--   0 niko      (1000) niko      (1000)     6273 2023-05-04 13:59:06.000000 jobspire_nitra-0.1.7/jobspire_nitra/main.py
-drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-04 14:03:53.912815 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/
--rw-r--r--   0 niko      (1000) niko      (1000)     1344 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/PKG-INFO
--rw-r--r--   0 niko      (1000) niko      (1000)      266 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/SOURCES.txt
--rw-r--r--   0 niko      (1000) niko      (1000)        1 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/dependency_links.txt
--rw-r--r--   0 niko      (1000) niko      (1000)        9 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/requires.txt
--rw-r--r--   0 niko      (1000) niko      (1000)       15 2023-05-04 14:03:53.000000 jobspire_nitra-0.1.7/jobspire_nitra.egg-info/top_level.txt
--rw-r--r--   0 niko      (1000) niko      (1000)       38 2023-05-04 14:03:53.913815 jobspire_nitra-0.1.7/setup.cfg
--rw-r--r--   0 niko      (1000) niko      (1000)      763 2023-05-04 14:00:01.000000 jobspire_nitra-0.1.7/setup.py
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-10 12:11:12.862036 jobspire_nitra-0.1.8/
+-rw-r--r--   0 niko      (1000) niko      (1000)     1055 2023-05-04 13:55:48.000000 jobspire_nitra-0.1.8/LICENSE
+-rw-r--r--   0 niko      (1000) niko      (1000)     1369 2023-05-10 12:11:12.861036 jobspire_nitra-0.1.8/PKG-INFO
+-rw-r--r--   0 niko      (1000) niko      (1000)     1072 2023-05-10 12:10:29.000000 jobspire_nitra-0.1.8/README.rst
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-10 12:11:12.860036 jobspire_nitra-0.1.8/jobspire_nitra/
+-rw-r--r--   0 niko      (1000) niko      (1000)       39 2023-05-04 13:55:48.000000 jobspire_nitra-0.1.8/jobspire_nitra/__init__.py
+-rw-r--r--   0 niko      (1000) niko      (1000)     6396 2023-05-10 12:10:09.000000 jobspire_nitra-0.1.8/jobspire_nitra/main.py
+drwxr-xr-x   0 niko      (1000) niko      (1000)        0 2023-05-10 12:11:12.861036 jobspire_nitra-0.1.8/jobspire_nitra.egg-info/
+-rw-r--r--   0 niko      (1000) niko      (1000)     1369 2023-05-10 12:11:12.000000 jobspire_nitra-0.1.8/jobspire_nitra.egg-info/PKG-INFO
+-rw-r--r--   0 niko      (1000) niko      (1000)      266 2023-05-10 12:11:12.000000 jobspire_nitra-0.1.8/jobspire_nitra.egg-info/SOURCES.txt
+-rw-r--r--   0 niko      (1000) niko      (1000)        1 2023-05-10 12:11:12.000000 jobspire_nitra-0.1.8/jobspire_nitra.egg-info/dependency_links.txt
+-rw-r--r--   0 niko      (1000) niko      (1000)        9 2023-05-10 12:11:12.000000 jobspire_nitra-0.1.8/jobspire_nitra.egg-info/requires.txt
+-rw-r--r--   0 niko      (1000) niko      (1000)       15 2023-05-10 12:11:12.000000 jobspire_nitra-0.1.8/jobspire_nitra.egg-info/top_level.txt
+-rw-r--r--   0 niko      (1000) niko      (1000)       38 2023-05-10 12:11:12.862036 jobspire_nitra-0.1.8/setup.cfg
+-rw-r--r--   0 niko      (1000) niko      (1000)      763 2023-05-10 12:10:37.000000 jobspire_nitra-0.1.8/setup.py
```

### Comparing `jobspire_nitra-0.1.7/LICENSE` & `jobspire_nitra-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jobspire_nitra-0.1.7/PKG-INFO` & `jobspire_nitra-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobspire_nitra
-Version: 0.1.7
+Version: 0.1.8
 Summary: Nitra
 Home-page: https://github.com/HBS-Economics/nitra.git
 Author: JobSpire team
 Author-email: <info@jobspire.com>
 Keywords: python,nitra package
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
@@ -36,14 +36,15 @@
   nitra.delete_job_postings_by_uuid(ids: List[str])
   nitra.update_job_postings(patches_with_id: List[dict])
   nitra.get_job_postings_with_no_word_embs()
   nitra.delete_job_posting_skills(job_posting_ids: List[str])
   nitra.ping()
   nitra.get_statistics()
   nitra.get_contract_types()
+  nitra.get_esco_codes()
   nitra.add_company_esco_matches(company_esco_matches: List[dict])
 
 
 -----------
 Development
 -----------
```

### Comparing `jobspire_nitra-0.1.7/README.rst` & `jobspire_nitra-0.1.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   nitra.delete_job_postings_by_uuid(ids: List[str])
   nitra.update_job_postings(patches_with_id: List[dict])
   nitra.get_job_postings_with_no_word_embs()
   nitra.delete_job_posting_skills(job_posting_ids: List[str])
   nitra.ping()
   nitra.get_statistics()
   nitra.get_contract_types()
+  nitra.get_esco_codes()
   nitra.add_company_esco_matches(company_esco_matches: List[dict])
 
 
 -----------
 Development
 -----------
```

### Comparing `jobspire_nitra-0.1.7/jobspire_nitra/main.py` & `jobspire_nitra-0.1.8/jobspire_nitra/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,20 @@
 
     def get_contract_types(self) -> Response:
         return self.req(
             '/contract_types',
             'GET'
         )
 
+    def get_esco_codes(self) -> Response:
+        return self.req(
+            '/esco_codes',
+            'GET'
+        )
+
     def add_company_esco_matches(
         self,
         company_esco_matches: List[dict]
     ) -> Response:
 
         body = {'esco_matches': company_esco_matches}
```

### Comparing `jobspire_nitra-0.1.7/jobspire_nitra.egg-info/PKG-INFO` & `jobspire_nitra-0.1.8/jobspire_nitra.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobspire-nitra
-Version: 0.1.7
+Version: 0.1.8
 Summary: Nitra
 Home-page: https://github.com/HBS-Economics/nitra.git
 Author: JobSpire team
 Author-email: <info@jobspire.com>
 Keywords: python,nitra package
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
@@ -36,14 +36,15 @@
   nitra.delete_job_postings_by_uuid(ids: List[str])
   nitra.update_job_postings(patches_with_id: List[dict])
   nitra.get_job_postings_with_no_word_embs()
   nitra.delete_job_posting_skills(job_posting_ids: List[str])
   nitra.ping()
   nitra.get_statistics()
   nitra.get_contract_types()
+  nitra.get_esco_codes()
   nitra.add_company_esco_matches(company_esco_matches: List[dict])
 
 
 -----------
 Development
 -----------
```

### Comparing `jobspire_nitra-0.1.7/setup.py` & `jobspire_nitra-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Nitra'
 
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 # Setting up
```

