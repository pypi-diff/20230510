# Comparing `tmp/fortifyapi-3.1.4.tar.gz` & `tmp/fortifyapi-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortifyapi-3.1.4.tar", last modified: Wed Apr 26 13:45:10 2023, max compression
+gzip compressed data, was "fortifyapi-3.1.5.tar", last modified: Wed May 10 17:53:03 2023, max compression
```

## Comparing `fortifyapi-3.1.4.tar` & `fortifyapi-3.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 13:45:10.799162 fortifyapi-3.1.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-04-26 13:45:10.799162 fortifyapi-3.1.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 13:45:10.795162 fortifyapi-3.1.4/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/docs/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/docs/couscous.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 13:45:10.795162 fortifyapi-3.1.4/fortifyapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39501 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/fortify.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/fortifyapi/template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-26 13:45:10.799162 fortifyapi-3.1.4/fortifyapi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-26 13:45:10.000000 fortifyapi-3.1.4/fortifyapi.egg-info/zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-04-26 13:45:10.799162 fortifyapi-3.1.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-04-26 13:45:03.000000 fortifyapi-3.1.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1046 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       29 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7460 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/docs/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/docs/couscous.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/fortifyapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6749 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27850 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39227 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/fortify.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7013 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/fortifyapi/template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/fortifyapi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-10 17:53:03.000000 fortifyapi-3.1.5/fortifyapi.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-10 17:53:03.502205 fortifyapi-3.1.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2023-05-10 17:52:55.000000 fortifyapi-3.1.5/setup.py
```

### Comparing `fortifyapi-3.1.4/LICENSE.txt` & `fortifyapi-3.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.4/PKG-INFO` & `fortifyapi-3.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.4
+Version: 3.1.5
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.4
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.5
 Description: .. image:: https://img.shields.io/pypi/v/fortifyapi.svg
         .. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
         .. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
         
         Fortify API
         ***********
```

### Comparing `fortifyapi-3.1.4/README.rst` & `fortifyapi-3.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.4/docs/README.md` & `fortifyapi-3.1.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.4/fortifyapi/api.py` & `fortifyapi-3.1.5/fortifyapi/api.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.4/fortifyapi/client.py` & `fortifyapi-3.1.5/fortifyapi/client.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.4/fortifyapi/fortify.py` & `fortifyapi-3.1.5/fortifyapi/fortify.py`

 * *Files 2% similar despite different names*

```diff
@@ -685,28 +685,23 @@
         """
         url = '/api/v1/projectVersions/' + str(version_id) + '/issues?start=0&limit=-1&' + orderby + '&' \
                                                              'showhidden=false&' \
                                                              'showremoved=false&showsuppressed=false&' \
                                                              'showshortfilenames=false'
         return self._request('GET', url)
 
-    def get_project_version_issue_details(self, instance_id, project_name, version_name, engine='SCA'):
+    def get_project_version_issue_details(self, issue_id):
         """
-        Returns trace analysis and other details of a given issue.  The issue ID can be found from the /issues or
+        Returns trace analysis and other details of a given issue. The issue ID can be found from the /issues or
         projectVersions endpoint.
-        :param instance_id:
-        :param project_name:
-        :param version_name:
-        :param engine:
+        :param issue_id:
         :return: full detail of a given issue
         """
-        url = '/api/v1/issueDetails?instanceId=' + str(instance_id) + '&projectName=' + str(project_name) + '&projectVersionName='\
-              + str(version_name) + '&engineType=' + str(engine)
-
-        return self._request('GET', url)
+        url = "/api/v1/issueDetails/" + str(issue_id)
+        return self._request("GET", url)
 
     def get_project_version_source_file(self, version_id, path):
         """
         Returns an object with information on a source file from a specific project version.
         It includes the file content.
         :param version_id: application version id
         :param path: the relative path of the file from the project root folder
```

### Comparing `fortifyapi-3.1.4/fortifyapi/query.py` & `fortifyapi-3.1.5/fortifyapi/query.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.4/fortifyapi/template.py` & `fortifyapi-3.1.5/fortifyapi/template.py`

 * *Files identical despite different names*

### Comparing `fortifyapi-3.1.4/fortifyapi.egg-info/PKG-INFO` & `fortifyapi-3.1.5/fortifyapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fortifyapi
-Version: 3.1.4
+Version: 3.1.5
 Summary: Python library for Fortify Software Security Center (SSC) RESTFul API
 Home-page: https://github.com/fortifyadmin/fortifyapi
 Author: Brandon Spruth, Matthew Gill
 Author-email: brandon@spruth.co, mgill@c0ffee.me
 License: MIT
-Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.4
+Download-URL: https://github.com/fortifyadmin/fortifyapi/tarball/3.1.5
 Description: .. image:: https://img.shields.io/pypi/v/fortifyapi.svg
         .. image:: https://img.shields.io/pypi/pyversions/fortifyapi.svg
         .. image:: https://img.shields.io/circleci/build/github/fortifyadmin/fortifyapi/master?logo=CircleCI
         
         Fortify API
         ***********
```

### Comparing `fortifyapi-3.1.4/setup.py` & `fortifyapi-3.1.5/setup.py`

 * *Files identical despite different names*

