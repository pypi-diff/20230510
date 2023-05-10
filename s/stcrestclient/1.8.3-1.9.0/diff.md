# Comparing `tmp/stcrestclient-1.8.3.tar.gz` & `tmp/stcrestclient-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stcrestclient-1.8.3.tar", last modified: Wed Feb 19 14:17:55 2020, max compression
+gzip compressed data, was "dist/stcrestclient-1.9.0.tar", last modified: Tue Jun 30 16:04:32 2020, max compression
```

## Comparing `stcrestclient-1.8.3.tar` & `stcrestclient-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sdua     (1668650661) 1275193766        0 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/
--rw-r--r--   0 sdua     (1668650661) 1275193766      949 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/PKG-INFO
--rw-r--r--   0 sdua     (1668650661) 1275193766    17639 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/README.md
-drwxr-xr-x   0 sdua     (1668650661) 1275193766        0 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient.egg-info/
--rw-r--r--   0 sdua     (1668650661) 1275193766      949 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient.egg-info/PKG-INFO
--rw-r--r--   0 sdua     (1668650661) 1275193766        1 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient.egg-info/zip-safe
--rw-r--r--   0 sdua     (1668650661) 1275193766      466 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient.egg-info/SOURCES.txt
--rw-r--r--   0 sdua     (1668650661) 1275193766       92 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient.egg-info/entry_points.txt
--rw-r--r--   0 sdua     (1668650661) 1275193766       14 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient.egg-info/requires.txt
--rw-r--r--   0 sdua     (1668650661) 1275193766       14 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient.egg-info/top_level.txt
--rw-r--r--   0 sdua     (1668650661) 1275193766        1 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient.egg-info/dependency_links.txt
--rw-r--r--   0 sdua     (1668650661) 1275193766     1605 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/setup.py
--rw-r--r--   0 sdua     (1668650661) 1275193766       67 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/setup.cfg
-drwxr-xr-x   0 sdua     (1668650661) 1275193766        0 2020-02-19 14:17:55.000000 stcrestclient-1.8.3/stcrestclient/
--rw-r--r--   0 sdua     (1668650661) 1275193766    17443 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/stcrestclient/resthttp.py
--rw-r--r--   0 sdua     (1668650661) 1275193766    14185 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/stcrestclient/stcpythonrest.py
--rw-r--r--   0 sdua     (1668650661) 1275193766        0 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/stcrestclient/__init__.py
--rw-r--r--   0 sdua     (1668650661) 1275193766     1699 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/stcrestclient/systeminfo.py
--rw-r--r--   0 sdua     (1668650661) 1275193766    25135 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/stcrestclient/stchttp.py
--rw-r--r--   0 sdua     (1668650661) 1275193766    33407 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/stcrestclient/tccsh.py
--rw-r--r--   0 sdua     (1668650661) 1275193766     2294 2020-02-19 14:14:38.000000 stcrestclient-1.8.3/stcrestclient/adapt.py
+drwxr-xr-x   0 sdua     (1668650661) 1275193766        0 2020-06-30 16:04:32.000000 stcrestclient-1.9.0/
+-rw-r--r--   0 sdua     (1668650661) 1275193766      949 2020-06-30 16:04:32.000000 stcrestclient-1.9.0/PKG-INFO
+-rw-r--r--   0 sdua     (1668650661) 1275193766    17639 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/README.md
+drwxr-xr-x   0 sdua     (1668650661) 1275193766        0 2020-06-30 16:04:32.000000 stcrestclient-1.9.0/stcrestclient.egg-info/
+-rw-r--r--   0 sdua     (1668650661) 1275193766      949 2020-06-30 16:04:27.000000 stcrestclient-1.9.0/stcrestclient.egg-info/PKG-INFO
+-rw-r--r--   0 sdua     (1668650661) 1275193766        1 2020-06-30 16:04:27.000000 stcrestclient-1.9.0/stcrestclient.egg-info/zip-safe
+-rw-r--r--   0 sdua     (1668650661) 1275193766      466 2020-06-30 16:04:27.000000 stcrestclient-1.9.0/stcrestclient.egg-info/SOURCES.txt
+-rw-r--r--   0 sdua     (1668650661) 1275193766       92 2020-06-30 16:04:27.000000 stcrestclient-1.9.0/stcrestclient.egg-info/entry_points.txt
+-rw-r--r--   0 sdua     (1668650661) 1275193766       14 2020-06-30 16:04:27.000000 stcrestclient-1.9.0/stcrestclient.egg-info/requires.txt
+-rw-r--r--   0 sdua     (1668650661) 1275193766       14 2020-06-30 16:04:27.000000 stcrestclient-1.9.0/stcrestclient.egg-info/top_level.txt
+-rw-r--r--   0 sdua     (1668650661) 1275193766        1 2020-06-30 16:04:27.000000 stcrestclient-1.9.0/stcrestclient.egg-info/dependency_links.txt
+-rw-r--r--   0 sdua     (1668650661) 1275193766     1605 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/setup.py
+-rw-r--r--   0 sdua     (1668650661) 1275193766       67 2020-06-30 16:04:32.000000 stcrestclient-1.9.0/setup.cfg
+drwxr-xr-x   0 sdua     (1668650661) 1275193766        0 2020-06-30 16:04:27.000000 stcrestclient-1.9.0/stcrestclient/
+-rw-r--r--   0 sdua     (1668650661) 1275193766    19891 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/stcrestclient/resthttp.py
+-rw-r--r--   0 sdua     (1668650661) 1275193766    14185 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/stcrestclient/stcpythonrest.py
+-rw-r--r--   0 sdua     (1668650661) 1275193766        0 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/stcrestclient/__init__.py
+-rw-r--r--   0 sdua     (1668650661) 1275193766     1699 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/stcrestclient/systeminfo.py
+-rw-r--r--   0 sdua     (1668650661) 1275193766    30012 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/stcrestclient/stchttp.py
+-rw-r--r--   0 sdua     (1668650661) 1275193766    33407 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/stcrestclient/tccsh.py
+-rw-r--r--   0 sdua     (1668650661) 1275193766     2294 2020-06-30 15:46:15.000000 stcrestclient-1.9.0/stcrestclient/adapt.py
```

### Comparing `stcrestclient-1.8.3/PKG-INFO` & `stcrestclient-1.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stcrestclient
-Version: 1.8.3
+Version: 1.9.0
 Summary: stcrestclient: Client modules for STC ReST API
 Home-page: https://github.com/Spirent/py-stcrestclient
 Author: Spirent
 Author-email: support@spirent.com
 License: http://www.opensource.org/licenses/mit-license.php
 Description: See https://github.com/Spirent/py-stcrestclient#python-stc-rest-api-client-stcrestclient
 Keywords: Spirent TestCenter API
```

### Comparing `stcrestclient-1.8.3/README.md` & `stcrestclient-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `stcrestclient-1.8.3/stcrestclient.egg-info/PKG-INFO` & `stcrestclient-1.9.0/stcrestclient.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: stcrestclient
-Version: 1.8.3
+Version: 1.9.0
 Summary: stcrestclient: Client modules for STC ReST API
 Home-page: https://github.com/Spirent/py-stcrestclient
 Author: Spirent
 Author-email: support@spirent.com
 License: http://www.opensource.org/licenses/mit-license.php
 Description: See https://github.com/Spirent/py-stcrestclient#python-stc-rest-api-client-stcrestclient
 Keywords: Spirent TestCenter API
```

### Comparing `stcrestclient-1.8.3/setup.py` & `stcrestclient-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 except ImportError:
     from distutils.core import setup
 
 
 def main():
     setup(
         name='stcrestclient',
-        version= '1.8.3',
+        version= '1.9.0',
         author='Spirent',
         author_email='support@spirent.com',
         url='https://github.com/Spirent/py-stcrestclient',
         description='stcrestclient: Client modules for STC ReST API',
         long_description = 'See https://github.com/Spirent/py-stcrestclient#python-stc-rest-api-client-stcrestclient',
         license='http://www.opensource.org/licenses/mit-license.php',
         keywords='Spirent TestCenter API',
```

### Comparing `stcrestclient-1.8.3/stcrestclient/resthttp.py` & `stcrestclient-1.9.0/stcrestclient/resthttp.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 """
 from __future__ import print_function
 
 import base64
 import os
 import sys
+import copy
 
 import requests
 
 
 class RestHttpError(Exception):
 
     """
@@ -498,7 +499,67 @@
         print('===> %s %s' % (method, url))
         print('  --- Headers ---')
         for k, v in headers.items():
             print('    %s: %s' % (k, v))
         if params:
             print('  --- Params ---')
             print('   ', params)
+
+    def bulk_get_request(self, container, resource=None, query_items=None, depth=1, 
+                    accept=None, to_lower=False):
+        """Send a GET request."""
+        url = self.make_url(container, resource)
+        headers = self._make_headers(accept)
+        myheaders = copy.deepcopy(headers)
+        myheaders["X-STC-API-Children-Depth"] = str(depth)
+
+        if query_items and isinstance(query_items, (list, tuple, set)):
+            url += RestHttp._list_query_str(query_items)
+            query_items = None
+
+        try:
+            rsp = requests.get(url, query_items, headers=myheaders,
+                               verify=self._verify, timeout=self._timeout)
+        except requests.exceptions.ConnectionError as e:
+            RestHttp._raise_conn_error(e)
+
+        if self._dbg_print:
+            self.__print_req('GET', rsp.url, headers, None)
+
+        return self._handle_response(rsp, to_lower)
+
+    def bulk_put_request(self, container, resource=None, params=None, accept=None):
+        """Send a PUT request."""
+        url = self.make_url(container, resource)
+        headers = self._make_headers(accept)
+        myheaders = copy.deepcopy(headers)
+        myheaders["content-length"] = str(len(params))
+        myheaders["content-type"] = "application/json"
+        try:
+            rsp = requests.put(url, params, headers=myheaders,
+                               verify=self._verify, timeout=self._timeout)
+        except requests.exceptions.ConnectionError as e:
+            RestHttp._raise_conn_error(e)
+
+        if self._dbg_print:
+            self.__print_req('PUT', rsp.url, headers, params)
+
+        return self._handle_response(rsp)
+
+    def bulk_post_request(self, container, resource=None, params=None, accept=None):
+        """Send a POST request."""
+        url = self.make_url(container, resource)
+        headers = self._make_headers(accept)
+        myheaders = copy.deepcopy(headers)
+        myheaders["content-length"] = str(len(params))
+        myheaders["content-type"] = "application/json"
+
+        try:
+            rsp = requests.post(url, data=params, headers=myheaders,
+                                verify=self._verify, timeout=self._timeout)
+        except requests.exceptions.ConnectionError as e:
+            RestHttp._raise_conn_error(e)
+
+        if self._dbg_print:
+            self.__print_req('POST', rsp.url, headers, params)
+
+        return self._handle_response(rsp)
```

### Comparing `stcrestclient-1.8.3/stcrestclient/stcpythonrest.py` & `stcrestclient-1.9.0/stcrestclient/stcpythonrest.py`

 * *Files identical despite different names*

### Comparing `stcrestclient-1.8.3/stcrestclient/systeminfo.py` & `stcrestclient-1.9.0/stcrestclient/systeminfo.py`

 * *Files identical despite different names*

### Comparing `stcrestclient-1.8.3/stcrestclient/stchttp.py` & `stcrestclient-1.9.0/stcrestclient/stchttp.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 """
 from __future__ import absolute_import
 from __future__ import print_function
 
 import time
 import os
 import socket
+import json
+from requests.utils import quote
 
 try:
     from . import resthttp
 except ValueError:
     import resthttp
 
 # Use this port if it is not specified when creating StcHttp, or by the
@@ -707,7 +709,144 @@
                     raise RuntimeError('failed to get stcapi_version')
             except Exception as e:
                 if self._dbg_print:
                     print('===>', e)
                 return (0, 0, 0)
 
         return self._api_ver
+
+    def has_bulk_ops(self):
+        status, data = self._rest.get_request('system')
+        if 'features' in data:
+            features = data['features']
+            if str(features).find('bulk-api') != -1:
+                return True
+        return False
+
+
+    def bulkconfig(self, locations, attributes=None, **kwattrs):
+        """Sets or modifies one or more object attributes or relations.
+
+        Arguments can be supplied either as a dictionary or as keyword
+        arguments.  Examples:
+            stc.bulkconfig('emulateddevice[@name="mydev"]/bgprouterconfig/bgpipv4routeconfig[0]',  {'NextHopIncrement': '0.0.1.0'})
+            stc.bulkconfig('emulateddevice[@name="mydev"]/bgprouterconfig/bgpipv4routeconfig[1]',  NextHopIncrement='0.0.1.0')
+
+        Arguments:
+        locations     -- the locations of object to modify.
+        attributes -- Dictionary of attributes (name-value pairs).
+        kwattrs    -- Optional keyword attributes (name=value pairs).
+
+        """
+        self._check_session()
+        if kwattrs:
+            if attributes:
+                if isinstance(attributes, dict):
+                    attributes.update(kwattrs)
+                elif isinstance(attributes, list):
+                    for attr in attributes:
+                        attr.update(kwattrs)
+            else:
+                attributes = kwattrs
+        
+        attributes = json.dumps(attributes)
+        status, data = self._rest.bulk_put_request('bulk/objects', quote(locations), attributes)
+        return data
+
+    def bulkcreate(self, object_type, attributes=None, **kwattrs):
+        """Create a new automation object.
+
+        Arguments:
+        object_type -- Type of object to create.
+        attributes  -- Dictionary of attributes (name-value pairs).
+        kwattrs     -- Optional keyword attributes (name=value pairs).
+
+        """
+        data = self._bulkcreateex(object_type, None, attributes, **kwattrs)
+        return data
+
+    def bulkcreateex(self, under, attributes=None, **kwattrs):
+        data = self._bulkcreateex(None, under, attributes, **kwattrs)
+        return data
+
+    def _bulkcreateex(self, object_type, under=None, attributes=None, **kwattrs):
+        """Create a new automation object.
+
+        Arguments:
+        object_type -- Type of object to create.
+        under       -- Handle of the parent of the new object.
+        attributes  -- Dictionary of attributes (name-value pairs).
+        kwattrs     -- Optional keyword attributes (name=value pairs).
+
+        """
+        self._check_session()
+        params = {'object_type': object_type}
+        if under:
+            params['under'] = under
+        if attributes:
+            if isinstance(attributes, dict):
+                params.update(attributes)
+                if kwattrs:
+                    params.update(kwattrs)
+            elif isinstance(attributes, list):
+                if kwattrs:
+                    for attr in attributes:
+                        attr.update(kwattrs)
+                params['bulklist']  = attributes
+        else:
+            if kwattrs:
+                params.update(kwattrs)
+
+        myparams = json.dumps(params)
+        status, data = self._rest.bulk_post_request('bulk/objects', None, myparams)
+        return data
+
+    def bulkget(self, locations, args=None, depth=1):
+        """Returns the value(s) of one or more object attributes.
+
+        If multiple arguments, this method returns a dictionary of argument
+        names mapped to the value returned by each argument.
+
+        If a single argument is given, then the response is a list of values
+        for that argument.
+
+        Arguments:
+        handle -- Handle that identifies object to get info for.
+        args  -- Zero or more attributes or relationships.
+
+
+        """
+        self._check_session()
+        status, data = self._rest.bulk_get_request('bulk/objects', quote(locations), args, depth)
+        return data
+
+    def bulkperform(self, command, params=None, **kwargs):
+        """Execute a command.
+
+        Arguments:
+        command -- Command to execute.
+        params  -- Optional.  Dictionary of parameters (name-value pairs).
+        kwargs  -- Optional keyword arguments (name=value pairs).
+
+        Return:
+        Data from command.
+
+        """
+        self._check_session()
+        if not params:
+            params = {}
+        if kwargs:
+            params.update(kwargs)
+        params['command'] = command
+        status, data = self._rest.post_request('bulk/perform', None, params)
+        return data
+
+    def bulkdelete(self, handles):
+        """bulkDelete the specified object.
+
+        Arguments:
+        handle -- Handles of objects to delete.
+
+        """
+        self._check_session()
+        status, data = self._rest.delete_request('bulk/objects', str(handles))
+        return data
```

### Comparing `stcrestclient-1.8.3/stcrestclient/tccsh.py` & `stcrestclient-1.9.0/stcrestclient/tccsh.py`

 * *Files identical despite different names*

### Comparing `stcrestclient-1.8.3/stcrestclient/adapt.py` & `stcrestclient-1.9.0/stcrestclient/adapt.py`

 * *Files identical despite different names*

