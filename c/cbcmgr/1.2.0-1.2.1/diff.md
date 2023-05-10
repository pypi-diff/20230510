# Comparing `tmp/cbcmgr-1.2.0.tar.gz` & `tmp/cbcmgr-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.2.0.tar", last modified: Tue May  2 21:52:44 2023, max compression
+gzip compressed data, was "cbcmgr-1.2.1.tar", last modified: Wed May 10 18:49:52 2023, max compression
```

## Comparing `cbcmgr-1.2.0.tar` & `cbcmgr-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-02 21:52:44.433478 cbcmgr-1.2.0/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.2.0/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-02 21:52:44.433359 cbcmgr-1.2.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.2.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-02 21:52:44.427026 cbcmgr-1.2.0/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.2.0/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.2.0/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.2.0/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.2.0/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     4098 2023-05-02 21:24:28.000000 cbcmgr-1.2.0/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    10675 2023-02-22 16:29:09.000000 cbcmgr-1.2.0/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.2.0/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.2.0/cbcmgr/schema.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-02 21:52:44.433157 cbcmgr-1.2.0/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      343 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       57 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-05-02 21:52:44.000000 cbcmgr-1.2.0/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-02 21:52:44.433519 cbcmgr-1.2.0/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)      705 2023-05-02 21:27:42.000000 cbcmgr-1.2.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 18:49:52.490512 cbcmgr-1.2.1/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.2.1/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-10 18:49:52.490390 cbcmgr-1.2.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.2.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 18:49:52.487526 cbcmgr-1.2.1/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.2.1/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10002 2023-04-18 18:40:46.000000 cbcmgr-1.2.1/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    19444 2023-04-18 18:36:58.000000 cbcmgr-1.2.1/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-06 18:28:18.000000 cbcmgr-1.2.1/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     4098 2023-05-02 21:24:28.000000 cbcmgr-1.2.1/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    10824 2023-05-10 18:40:42.000000 cbcmgr-1.2.1/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2841 2023-02-16 23:17:59.000000 cbcmgr-1.2.1/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.2.1/cbcmgr/schema.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-05-10 18:49:52.490205 cbcmgr-1.2.1/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1095 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      343 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       57 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-05-10 18:49:52.000000 cbcmgr-1.2.1/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-05-10 18:49:52.490555 cbcmgr-1.2.1/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)      705 2023-05-10 18:40:59.000000 cbcmgr-1.2.1/setup.py
```

### Comparing `cbcmgr-1.2.0/LICENSE.txt` & `cbcmgr-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.0/PKG-INFO` & `cbcmgr-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.2.0
+Version: 1.2.1
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.2.0/README.md` & `cbcmgr-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.0/cbcmgr/cb_connect.py` & `cbcmgr-1.2.1/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.0/cbcmgr/cb_management.py` & `cbcmgr-1.2.1/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.0/cbcmgr/cb_session.py` & `cbcmgr-1.2.1/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.0/cbcmgr/exceptions.py` & `cbcmgr-1.2.1/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.0/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.2.1/cbcmgr/httpsessionmgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     AUTH_BASIC = 0
     AUTH_CAPELLA = 1
 
     def __init__(self, username=None, password=None, auth_type=0):
         warnings.filterwarnings("ignore")
         self.username = username
         self.password = password
+        self.timeout = 30
         self.logger = logging.getLogger(self.__class__.__name__)
         self.url_prefix = "http://127.0.0.1"
         self.session = requests.Session()
         retries = Retry(total=60,
                         backoff_factor=0.2)
         self.session.mount('http://', HTTPAdapter(max_retries=retries))
         self.session.mount('https://', HTTPAdapter(max_retries=retries))
@@ -160,14 +161,17 @@
         if ssl == APISession.HTTP:
             port_num = port if port else 80
             self.url_prefix = f"http://{hostname}:{port_num}"
         else:
             port_num = port if port else 443
             self.url_prefix = f"https://{hostname}:{port_num}"
 
+    def set_timeout(self, timeout: int):
+        self.timeout = timeout
+
     def get_endpoint(self, path):
         return ':'.join(self.url_prefix.split(':')[:-1]) + path
 
     @property
     def response(self):
         return self._response
 
@@ -215,15 +219,15 @@
                     return data, None, None
         else:
             raise PaginationDataNotFound("pagination values not found")
 
     def api_get(self, endpoint, items=None):
         if items is None:
             items = []
-        response = self.session.get(self.url_prefix + endpoint, auth=self.auth_class, verify=False, timeout=15)
+        response = self.session.get(self.url_prefix + endpoint, auth=self.auth_class, verify=False, timeout=self.timeout)
 
         try:
             self.check_status_code(response.status_code)
         except Exception:
             raise
 
         try:
@@ -241,30 +245,30 @@
         return self
 
     def api_post(self, endpoint, body):
         response = self.session.post(self.url_prefix + endpoint,
                                      auth=self.auth_class,
                                      json=body,
                                      verify=False,
-                                     timeout=15)
+                                     timeout=self.timeout)
 
         try:
             self.check_status_code(response.status_code)
         except Exception:
             raise
 
         self._response = response.text
         return self
 
     def api_put(self, endpoint, body):
         response = self.session.put(self.url_prefix + endpoint,
                                     auth=self.auth_class,
                                     json=body,
                                     verify=False,
-                                    timeout=15)
+                                    timeout=self.timeout)
 
         try:
             self.check_status_code(response.status_code)
         except Exception:
             raise
 
         self._response = response.text
@@ -273,27 +277,27 @@
     def api_put_data(self, endpoint, body, content_type):
         headers = {'Content-Type': content_type}
 
         response = self.session.put(self.url_prefix + endpoint,
                                     auth=self.auth_class,
                                     data=body,
                                     verify=False,
-                                    timeout=15,
+                                    timeout=self.timeout,
                                     headers=headers)
 
         try:
             self.check_status_code(response.status_code)
         except Exception:
             raise
 
         self._response = response.text
         return self
 
     def api_delete(self, endpoint):
-        response = self.session.delete(self.url_prefix + endpoint, auth=self.auth_class, verify=False, timeout=15)
+        response = self.session.delete(self.url_prefix + endpoint, auth=self.auth_class, verify=False, timeout=self.timeout)
 
         try:
             self.check_status_code(response.status_code)
         except Exception:
             raise
 
         self._response = response.text
```

### Comparing `cbcmgr-1.2.0/cbcmgr/retry.py` & `cbcmgr-1.2.1/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.0/cbcmgr/schema.py` & `cbcmgr-1.2.1/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.2.0/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.2.1/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.2.0
+Version: 1.2.1
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cbcmgr-1.2.0/setup.py` & `cbcmgr-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.2.0',
+    version='1.2.1',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

