# Comparing `tmp/sosin-1.0.5.tar.gz` & `tmp/sosin-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.0.5.tar", last modified: Wed May 10 06:55:55 2023, max compression
+gzip compressed data, was "sosin-1.1.0.tar", last modified: Wed May 10 08:13:48 2023, max compression
```

## Comparing `sosin-1.0.5.tar` & `sosin-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 06:55:55.669030 sosin-1.0.5/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-05-10 06:55:55.668021 sosin-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 06:55:55.670558 sosin-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-05-10 06:51:08.000000 sosin-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:55:55.595174 sosin-1.0.5/sosin/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.5/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:55:55.637867 sosin-1.0.5/sosin/databases/
--rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.0.5/sosin/databases/fs.py
--rw-rw-rw-   0        0        0     9667 2023-04-24 02:18:48.000000 sosin-1.0.5/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:55:55.641887 sosin-1.0.5/sosin/rpa/
--rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.0.5/sosin/rpa/email_mgr.py
--rw-rw-rw-   0        0        0     3698 2023-04-24 11:58:43.000000 sosin-1.0.5/sosin/rpa/sms_mgr.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:55:55.653450 sosin-1.0.5/sosin/utils/
--rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.5/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.5/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.5/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.5/sosin/utils/secret.py
--rw-rw-rw-   0        0        0      885 2023-04-28 16:00:12.000000 sosin-1.0.5/sosin/utils/zip.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:55:55.664723 sosin-1.0.5/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.0.5/sosin/web/content.py
--rw-rw-rw-   0        0        0     5240 2023-05-10 06:52:57.000000 sosin-1.0.5/sosin/web/session.py
--rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.5/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4796 2023-04-24 07:25:27.000000 sosin-1.0.5/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:55:55.629351 sosin-1.0.5/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-05-10 06:55:54.000000 sosin-1.0.5/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-05-10 06:55:55.000000 sosin-1.0.5/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 06:55:55.000000 sosin-1.0.5/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-10 06:55:55.000000 sosin-1.0.5/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 06:55:55.000000 sosin-1.0.5/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.631873 sosin-1.1.0/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-05-10 08:13:48.630872 sosin-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:13:48.631873 sosin-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-05-10 08:13:43.000000 sosin-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.586562 sosin-1.1.0/sosin/
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.1.0/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.602434 sosin-1.1.0/sosin/databases/
+-rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.0/sosin/databases/fs.py
+-rw-rw-rw-   0        0        0     9667 2023-05-10 06:56:55.000000 sosin-1.1.0/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.605646 sosin-1.1.0/sosin/rpa/
+-rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.1.0/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.0/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.625581 sosin-1.1.0/sosin/utils/
+-rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.0/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.629873 sosin-1.1.0/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.0/sosin/web/content.py
+-rw-rw-rw-   0        0        0     5505 2023-05-10 08:13:43.000000 sosin-1.1.0/sosin/web/session.py
+-rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.1.0/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4796 2023-04-24 07:25:27.000000 sosin-1.1.0/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:13:48.599924 sosin-1.1.0/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 08:13:48.000000 sosin-1.1.0/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.0.5/LICENSE` & `sosin-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/PKG-INFO` & `sosin-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.5
+Version: 1.1.0
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sosin-1.0.5/README.md` & `sosin-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/setup.py` & `sosin-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.0.5",
+    version                             = "1.1.0",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'beautifulsoup4', 'PyMySQL',],
```

### Comparing `sosin-1.0.5/sosin/databases/fs.py` & `sosin-1.1.0/sosin/databases/fs.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/databases/rdb.py` & `sosin-1.1.0/sosin/databases/rdb.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/rpa/email_mgr.py` & `sosin-1.1.0/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/rpa/sms_mgr.py` & `sosin-1.1.0/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/utils/currency.py` & `sosin-1.1.0/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/utils/progress.py` & `sosin-1.1.0/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/utils/zip.py` & `sosin-1.1.0/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/web/content.py` & `sosin-1.1.0/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/web/session.py` & `sosin-1.1.0/sosin/web/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,25 +61,28 @@
                  method:str='post', no_parsing:bool=False, **kwargs) -> requests.Response:
         """
         request
 
         method = get, post, put
         files -> {key: file_path}
         """
+        headers = {k.lower(): headers[k] for k in headers}
+
         type_header = {}
-        if data:
+        if data and not no_parsing:
+            # charset?
             type_header['content-type'] = 'application/x-www-form-urlencoded'\
                 if type(data) == str else 'application/json;charset=UTF-8'
 
         if method.lower() == 'post':
             if files:
                 boundary = '----WebKitFormBoundary' +\
                     ''.join(random.sample(string.ascii_letters + string.digits, 16))
                 data = MultipartEncoder(fields={**data, **{k: self.get_file_form(v) for k, v in files.items()}}, boundary=boundary)
-                headers = {**headers, 'Content-Type': data.content_type, "Connection": "keep-alive"}
+                headers = {**headers, 'content-type': data.content_type, "connection": "keep-alive"}
 
             r = requests.post(url, headers={**self._headers, **type_header, **headers}, 
                               cookies={**self._cookies, **cookies}, 
                               data=data if type(data) in [str, MultipartEncoder] or no_parsing else json.dumps(data), **kwargs)
         elif method.lower() == 'get':
             r = requests.get(url, headers={**self._headers, **type_header, **headers}, 
                              cookies={**self._cookies, **cookies}, **kwargs)
@@ -88,16 +91,22 @@
                              cookies={**self._cookies, **cookies}, data=json.dumps(data), **kwargs)
         
         self._set_cookies(r)
         return r
     
     # ------------------------------------------------------------------------
     # Cookie Management
+    def add_cookies(self, cookies:dict) -> None:
+        self._cookies.update(cookies)
+
+    def get_cookie(self, k:str) -> str:
+        return self._cookies.get(k, '')
+
     def _set_cookies(self, r:requests.Response) -> None:
-        self._cookies = {**self._cookies, **dict(r.cookies)}
+        self._cookies.update(dict(r.cookies))
 
     def _reset_cookies(self, keys:list=[]) -> None:
         self._cookies = {k: self._cookies[k] for k in keys}
     
     def _save_cookies(self) -> None:
         open(self._cookie_path, 'w').write('\n'.join(['{}={}'.format(k, v) for k, v in self._cookies.items()]))
```

### Comparing `sosin-1.0.5/sosin/web/translate.py` & `sosin-1.1.0/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin/web/virtual.py` & `sosin-1.1.0/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.5/sosin.egg-info/PKG-INFO` & `sosin-1.1.0/sosin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.5
+Version: 1.1.0
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

