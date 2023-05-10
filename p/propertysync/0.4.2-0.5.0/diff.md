# Comparing `tmp/propertysync-0.4.2.tar.gz` & `tmp/propertysync-0.5.0.tar.gz`

## Comparing `propertysync-0.4.2.tar` & `propertysync-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 propertysync-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.4.2/propertysync/__about__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.4.2/propertysync/__init__.py
--rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 propertysync-0.4.2/propertysync/api.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 propertysync-0.4.2/propertysync/batch.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 propertysync-0.4.2/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.4.2/propertysync/search.py
--rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.4.2/propertysync/titlesearch_batch.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.4.2/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.4.2/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.4.2/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 propertysync-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 propertysync-0.5.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/__init__.py
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/api.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/batch.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/search.py
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 propertysync-0.5.0/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 propertysync-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 propertysync-0.5.0/tests/test_batch.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 propertysync-0.5.0/tests/test_document.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 propertysync-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.5.0/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.5.0/PKG-INFO
```

### Comparing `propertysync-0.4.2/CHANGELOG.md` & `propertysync-0.5.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,28 @@
 ## [Unreleased]
 
 ### Added
 ### Fixed
 ### Changed
 ### Removed
 
+
+## [0.5.0] - 2023-05-10
+
+### Added
+- Lots of work to Batch and Document classes to support find and replace
+- Tests added for Batch and Document classes
+- New API method (get_document_pdf) to retrieve document PDFs
+
+### Changed
+- Do not automatically inject indexingRecordId in TitleSearchBatch helper
+
+### Removed
+- Old batch replace method from Batch class
+
 ## [0.4.1] - 2023-04-17
 
 ### Changed
 - Minor adjustments to TitleSearchBatch helper for default naming and date format
 
 ## [0.4.0] - 2023-04-17
```

### Comparing `propertysync-0.4.2/propertysync/api.py` & `propertysync-0.5.0/propertysync/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -111,15 +111,19 @@
         elif (method == "PATCH"):
             request = requests.patch(url,params=params,headers=headers, json=body)             
         else:
             raise Exception("Invalid method: "+method)
 
         # determine if the request was successful
         if request.status_code == 200:
-            return request.json()
+            # if we are requesting a PDF, return the raw content
+            if "pdf" in request.headers["Content-Type"]:
+                return request.content
+            else:
+                return request.json()
         elif request.status_code == 401:
             # if the token is invalid, try to login again, if we receive a failure again, raise an exception
             if (tries < 2):
                 tries += 1
                 self.login()
                 return self.api_call(method=method, url=url, params=params, tries=tries)
             else:
@@ -288,14 +292,38 @@
         return self.api_call("GET", url)
     
     # get asset from a document ID
     def get_document_asset(self, document_id, asset_id):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/documents/{document_id}/assets/{asset_id}"
         return self.api_call("GET", url)
     
+    # get pdf from assets
+    def get_document_pdf(self, document_id):
+        # first, get all assets for this document
+        assets = self.get_document_assets(document_id)
+        if(len(assets) == 0):
+            raise Exception("No assets found for document ID "+document_id)
+        
+        # find the PDF asset
+        if "pdf" not in assets:
+            raise Exception("No PDF found for document ID "+document_id)
+        
+        # get the PDF asset
+        pdf_asset = self.get_document_asset(document_id, assets["pdf"]["id"])
+
+        # create a temp file name for the pdf using the document_id
+        temp_file_name = "/tmp/"+document_id+".pdf"
+
+        # download the PDF to the temp file
+        with open(temp_file_name, 'wb') as f:
+            f.write(pdf_asset)
+
+        # return the temp file name
+        return temp_file_name
+    
     # get versions from a document ID
     def get_document_versions(self, document_id):
         url = f"{self.indexing_url}/document-groups/{self.document_group_id}/documents/{document_id}/versions"
         return self.api_call("GET", url)
 
     # get orders (requires a company ID)
     def get_orders(self):
```

### Comparing `propertysync-0.4.2/propertysync/search.py` & `propertysync-0.5.0/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.2/propertysync/titlesearch_batch.py` & `propertysync-0.5.0/propertysync/titlesearch_batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.2/LICENSE` & `propertysync-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.2/README.md` & `propertysync-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.2/pyproject.toml` & `propertysync-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.2/PKG-INFO` & `propertysync-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.4.2
+Version: 0.5.0
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

