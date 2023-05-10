# Comparing `tmp/python-bring-api-1.1.0.tar.gz` & `tmp/python-bring-api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bring-api-1.1.0.tar", last modified: Tue May  2 19:54:44 2023, max compression
+gzip compressed data, was "python-bring-api-1.1.2.tar", last modified: Wed May 10 18:33:38 2023, max compression
```

## Comparing `python-bring-api-1.1.0.tar` & `python-bring-api-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-02 19:54:44.791806 python-bring-api-1.1.0/
--rw-------   0 elias     (1000) elias     (1000)     1114 2022-01-27 12:36:43.000000 python-bring-api-1.1.0/LICENSE
--rw-r--r--   0 elias     (1000) elias     (1000)     1860 2023-05-02 19:54:44.791806 python-bring-api-1.1.0/PKG-INFO
--rw-------   0 elias     (1000) elias     (1000)     1433 2023-05-02 19:53:41.000000 python-bring-api-1.1.0/README.md
--rw-------   0 elias     (1000) elias     (1000)      108 2022-01-30 10:52:36.000000 python-bring-api-1.1.0/pyproject.toml
--rw-------   0 elias     (1000) elias     (1000)      657 2023-05-02 19:54:44.792806 python-bring-api-1.1.0/setup.cfg
-drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-02 19:54:44.789806 python-bring-api-1.1.0/src/
-drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-02 19:54:44.790806 python-bring-api-1.1.0/src/python_bring_api/
--rw-------   0 elias     (1000) elias     (1000)        0 2022-01-27 12:29:47.000000 python-bring-api-1.1.0/src/python_bring_api/__init__.py
--rw-r--r--   0 elias     (1000) elias     (1000)     5583 2023-05-02 19:46:28.000000 python-bring-api-1.1.0/src/python_bring_api/bring.py
-drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-02 19:54:44.791806 python-bring-api-1.1.0/src/python_bring_api.egg-info/
--rw-------   0 elias     (1000) elias     (1000)     1860 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/PKG-INFO
--rw-------   0 elias     (1000) elias     (1000)      324 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/SOURCES.txt
--rw-------   0 elias     (1000) elias     (1000)        1 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/dependency_links.txt
--rw-------   0 elias     (1000) elias     (1000)        9 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/requires.txt
--rw-------   0 elias     (1000) elias     (1000)       17 2023-05-02 19:54:44.000000 python-bring-api-1.1.0/src/python_bring_api.egg-info/top_level.txt
+drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-10 18:33:38.871783 python-bring-api-1.1.2/
+-rw-r--r--   0 elias     (1000) elias     (1000)     1114 2023-05-10 18:25:16.000000 python-bring-api-1.1.2/LICENSE
+-rw-r--r--   0 elias     (1000) elias     (1000)     1768 2023-05-10 18:33:38.871783 python-bring-api-1.1.2/PKG-INFO
+-rw-r--r--   0 elias     (1000) elias     (1000)     1327 2023-05-10 18:25:16.000000 python-bring-api-1.1.2/README.md
+-rw-r--r--   0 elias     (1000) elias     (1000)      108 2023-05-10 18:25:16.000000 python-bring-api-1.1.2/pyproject.toml
+-rw-r--r--   0 elias     (1000) elias     (1000)      657 2023-05-10 18:33:38.872783 python-bring-api-1.1.2/setup.cfg
+drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-10 18:33:38.869783 python-bring-api-1.1.2/src/
+drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-10 18:33:38.871783 python-bring-api-1.1.2/src/python_bring_api/
+-rw-r--r--   0 elias     (1000) elias     (1000)        0 2023-05-10 18:25:16.000000 python-bring-api-1.1.2/src/python_bring_api/__init__.py
+-rw-r--r--   0 elias     (1000) elias     (1000)     5705 2023-05-10 18:28:02.000000 python-bring-api-1.1.2/src/python_bring_api/bring.py
+drwxr-xr-x   0 elias     (1000) elias     (1000)        0 2023-05-10 18:33:38.871783 python-bring-api-1.1.2/src/python_bring_api.egg-info/
+-rw-r--r--   0 elias     (1000) elias     (1000)     1768 2023-05-10 18:33:38.000000 python-bring-api-1.1.2/src/python_bring_api.egg-info/PKG-INFO
+-rw-r--r--   0 elias     (1000) elias     (1000)      324 2023-05-10 18:33:38.000000 python-bring-api-1.1.2/src/python_bring_api.egg-info/SOURCES.txt
+-rw-r--r--   0 elias     (1000) elias     (1000)        1 2023-05-10 18:33:38.000000 python-bring-api-1.1.2/src/python_bring_api.egg-info/dependency_links.txt
+-rw-r--r--   0 elias     (1000) elias     (1000)        9 2023-05-10 18:33:38.000000 python-bring-api-1.1.2/src/python_bring_api.egg-info/requires.txt
+-rw-r--r--   0 elias     (1000) elias     (1000)       17 2023-05-10 18:33:38.000000 python-bring-api-1.1.2/src/python_bring_api.egg-info/top_level.txt
```

### Comparing `python-bring-api-1.1.0/LICENSE` & `python-bring-api-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bring-api-1.1.0/PKG-INFO` & `python-bring-api-1.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: python-bring-api
-Version: 1.1.0
+Version: 1.1.2
 Summary: Unofficial python package to access Bring! shopping lists API.
 Home-page: https://github.com/blue1stone/python-bring-api
 Author: Elias Ball
 Author-email: contact.eliasball@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Bring Shopping Lists API
-
 An unofficial python package to access the Bring! shopping lists API.
 
 > This is a **minimal** python port of the [node-bring-api](https://github.com/foxriver76/node-bring-api) by [foxriver76](https://github.com/foxriver76). All credit goes to him for making this awesome API possible!
 
 ## Disclaimer
-
 The developers of this module are in no way endorsed by or affiliated with Bring! Labs AG, or any associated subsidiaries, logos or trademarks.
 
 ## Installation
-
-`pip install python-bring-api`
+```pip install python-bring-api```
 
 ## Usage Example
-
 ```python
 from python_bring_api.bring import Bring
 
 # Create Bring instance with email and password
 bring = Bring("EMAIL", "PASSWORD")
 # Login
 bring.login()
@@ -47,24 +43,14 @@
 print(items['purchase']) # [{'specification': 'low fat', 'name': 'Milk'}]
 
 # Remove an item from a list
 bring.removeItem(lists['lists'][0]['listUuid'], 'Milk')
 ```
 
 ## Changelog
-
-### 1.1.0
-
-Add item details endpoint, thanks to [@Dielee](https://github.com/Dielee)!
-
 ### 1.0.2
-
 Fixed error handling
 Added response return to login
-
 ### 1.0.1
-
 Add github repo
-
-### 1.0.0
-
+### 1.0.0 
 Initial release
```

### Comparing `python-bring-api-1.1.0/README.md` & `python-bring-api-1.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # Bring Shopping Lists API
-
 An unofficial python package to access the Bring! shopping lists API.
 
 > This is a **minimal** python port of the [node-bring-api](https://github.com/foxriver76/node-bring-api) by [foxriver76](https://github.com/foxriver76). All credit goes to him for making this awesome API possible!
 
 ## Disclaimer
-
 The developers of this module are in no way endorsed by or affiliated with Bring! Labs AG, or any associated subsidiaries, logos or trademarks.
 
 ## Installation
-
-`pip install python-bring-api`
+```pip install python-bring-api```
 
 ## Usage Example
-
 ```python
 from python_bring_api.bring import Bring
 
 # Create Bring instance with email and password
 bring = Bring("EMAIL", "PASSWORD")
 # Login
 bring.login()
@@ -33,24 +29,14 @@
 print(items['purchase']) # [{'specification': 'low fat', 'name': 'Milk'}]
 
 # Remove an item from a list
 bring.removeItem(lists['lists'][0]['listUuid'], 'Milk')
 ```
 
 ## Changelog
-
-### 1.1.0
-
-Add item details endpoint, thanks to [@Dielee](https://github.com/Dielee)!
-
 ### 1.0.2
-
 Fixed error handling
 Added response return to login
-
 ### 1.0.1
-
 Add github repo
-
-### 1.0.0
-
+### 1.0.0 
 Initial release
```

### Comparing `python-bring-api-1.1.0/setup.cfg` & `python-bring-api-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-bring-api
-version = 1.1.0
+version = 1.1.2
 author = Elias Ball
 author_email = contact.eliasball@gmail.com
 description = Unofficial python package to access Bring! shopping lists API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/blue1stone/python-bring-api
```

### Comparing `python-bring-api-1.1.0/src/python_bring_api/bring.py` & `python-bring-api-1.1.2/src/python_bring_api/bring.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,30 +2,34 @@
 import traceback
 
 class Bring:
     """
     Unofficial Bring API interface.
     """
 
-    def __init__(self, mail, password):
+    def __init__(self, mail, password, headers = None):
         self.mail = mail
         self.password = password
         self.url = 'https://api.getbring.com/rest/v2/'
         self.uuid = ''
         self.name = ''
         self.bearerToken = ''
         self.refreshToken = ''
-        self.headers = {
-            'Authorization': '',
-            'X-BRING-API-KEY': 'cof4Nc6D8saplXjE3h3HXqHH8m7VU2i1Gs0g85Sp',
-            'X-BRING-CLIENT-SOURCE': 'webApp',
-            'X-BRING-CLIENT': 'webApp',
-            'X-BRING-COUNTRY': 'DE',
-            'X-BRING-USER-UUID': ''
-        }
+
+        if headers:
+            self.headers = headers
+        else:
+            self.headers = {
+                'Authorization': '',
+                'X-BRING-API-KEY': 'cof4Nc6D8saplXjE3h3HXqHH8m7VU2i1Gs0g85Sp',
+                'X-BRING-CLIENT-SOURCE': 'webApp',
+                'X-BRING-CLIENT': 'webApp',
+                'X-BRING-COUNTRY': 'DE',
+                'X-BRING-USER-UUID': ''
+            }
         self.putHeaders = {
             'Authorization': '',
             'X-BRING-API-KEY': '',
             'X-BRING-CLIENT-SOURCE': '',
             'X-BRING-CLIENT': '',
             'X-BRING-COUNTRY': '',
             'X-BRING-USER-UUID': '',
```

### Comparing `python-bring-api-1.1.0/src/python_bring_api.egg-info/PKG-INFO` & `python-bring-api-1.1.2/src/python_bring_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: python-bring-api
-Version: 1.1.0
+Version: 1.1.2
 Summary: Unofficial python package to access Bring! shopping lists API.
 Home-page: https://github.com/blue1stone/python-bring-api
 Author: Elias Ball
 Author-email: contact.eliasball@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Bring Shopping Lists API
-
 An unofficial python package to access the Bring! shopping lists API.
 
 > This is a **minimal** python port of the [node-bring-api](https://github.com/foxriver76/node-bring-api) by [foxriver76](https://github.com/foxriver76). All credit goes to him for making this awesome API possible!
 
 ## Disclaimer
-
 The developers of this module are in no way endorsed by or affiliated with Bring! Labs AG, or any associated subsidiaries, logos or trademarks.
 
 ## Installation
-
-`pip install python-bring-api`
+```pip install python-bring-api```
 
 ## Usage Example
-
 ```python
 from python_bring_api.bring import Bring
 
 # Create Bring instance with email and password
 bring = Bring("EMAIL", "PASSWORD")
 # Login
 bring.login()
@@ -47,24 +43,14 @@
 print(items['purchase']) # [{'specification': 'low fat', 'name': 'Milk'}]
 
 # Remove an item from a list
 bring.removeItem(lists['lists'][0]['listUuid'], 'Milk')
 ```
 
 ## Changelog
-
-### 1.1.0
-
-Add item details endpoint, thanks to [@Dielee](https://github.com/Dielee)!
-
 ### 1.0.2
-
 Fixed error handling
 Added response return to login
-
 ### 1.0.1
-
 Add github repo
-
-### 1.0.0
-
+### 1.0.0 
 Initial release
```

