# Comparing `tmp/omero-user-token-0.2.1.tar.gz` & `tmp/omero-user-token-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-user-token-0.2.1.tar", last modified: Fri May  5 10:35:36 2023, max compression
+gzip compressed data, was "omero-user-token-0.3.0.tar", last modified: Wed May 10 07:26:19 2023, max compression
```

## Comparing `omero-user-token-0.2.1.tar` & `omero-user-token-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:35:36.527318 omero-user-token-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-05-05 10:35:29.000000 omero-user-token-0.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 10:35:29.000000 omero-user-token-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-05 10:35:36.527318 omero-user-token-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-05 10:35:29.000000 omero-user-token-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:35:36.527318 omero-user-token-0.2.1/omero_user_token/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2957 2023-05-05 10:35:29.000000 omero-user-token-0.2.1/omero_user_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:35:36.527318 omero-user-token-0.2.1/omero_user_token/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 10:35:29.000000 omero-user-token-0.2.1/omero_user_token/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-05 10:35:29.000000 omero-user-token-0.2.1/omero_user_token/cli/omero_user_token.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 10:35:32.000000 omero-user-token-0.2.1/omero_user_token/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:35:36.527318 omero-user-token-0.2.1/omero_user_token.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-05 10:35:36.000000 omero-user-token-0.2.1/omero_user_token.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-05 10:35:36.000000 omero-user-token-0.2.1/omero_user_token.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:35:36.000000 omero-user-token-0.2.1/omero_user_token.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 10:35:36.000000 omero-user-token-0.2.1/omero_user_token.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 10:35:36.000000 omero-user-token-0.2.1/omero_user_token.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 10:35:36.000000 omero-user-token-0.2.1/omero_user_token.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:35:36.000000 omero-user-token-0.2.1/omero_user_token.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 10:35:36.527318 omero-user-token-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-05 10:35:29.000000 omero-user-token-0.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-05 10:35:29.000000 omero-user-token-0.2.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:26:19.051280 omero-user-token-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-05-10 07:26:09.000000 omero-user-token-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 07:26:09.000000 omero-user-token-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-10 07:26:19.051280 omero-user-token-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-10 07:26:09.000000 omero-user-token-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:26:19.047280 omero-user-token-0.3.0/omero_user_token/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2023-05-10 07:26:09.000000 omero-user-token-0.3.0/omero_user_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:26:19.051280 omero-user-token-0.3.0/omero_user_token/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-10 07:26:09.000000 omero-user-token-0.3.0/omero_user_token/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-10 07:26:09.000000 omero-user-token-0.3.0/omero_user_token/cli/omero_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 07:26:14.000000 omero-user-token-0.3.0/omero_user_token/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:26:19.051280 omero-user-token-0.3.0/omero_user_token.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-10 07:26:19.000000 omero-user-token-0.3.0/omero_user_token.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 07:26:19.000000 omero-user-token-0.3.0/omero_user_token.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:26:19.000000 omero-user-token-0.3.0/omero_user_token.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 07:26:19.000000 omero-user-token-0.3.0/omero_user_token.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 07:26:19.000000 omero-user-token-0.3.0/omero_user_token.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 07:26:19.000000 omero-user-token-0.3.0/omero_user_token.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:26:19.000000 omero-user-token-0.3.0/omero_user_token.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 07:26:19.051280 omero-user-token-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-10 07:26:09.000000 omero-user-token-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-10 07:26:09.000000 omero-user-token-0.3.0/version.py
```

### Comparing `omero-user-token-0.2.1/LICENSE.txt` & `omero-user-token-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omero-user-token-0.2.1/PKG-INFO` & `omero-user-token-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-user-token
-Version: 0.2.1
+Version: 0.3.0
 Summary: OMERO user token management system
 Home-page: https://github.com/glencoesoftware/omero-user-token
 Author: Glencoe Software, Inc.
 Author-email: info@glencoesoftware.com
 License: UNKNOWN
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `omero-user-token-0.2.1/README.md` & `omero-user-token-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `omero-user-token-0.2.1/omero_user_token/__init__.py` & `omero-user-token-0.3.0/omero_user_token/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,38 +62,45 @@
         with open(assert_and_get_token_path(), 'w') as token_file:
             token_file.write(token)
         return token
     finally:
         client.closeSession()
 
 
-def login():
+def get_token():
     """
-    Returns an omero.client object from the current user token.  The
-    session the token refers to has had a join attempt made upon it.  If
-    the token file does not exist a FileNotFoundError will be raised.
+    Returns the current user token
+    Raises FileNotFoundError if the token file does not exist
     """
-    token_path = assert_and_get_token_path()
-    with open(token_path, 'r') as token_file:
-        token = token_file.read().strip()
-        omero_session_key = token[:token.find('@')]
-        host, port = token[token.find('@') + 1:].split(':')
-        client = omero.client(host, int(port))
-        try:
-            session = client.joinSession(omero_session_key)
-            session.detachOnDestroy()
-        except Exception:
-            pass
-        return client
+    with open(assert_and_get_token_path(), 'r') as token_path:
+        return token_path.read().strip()
+
+
+def login(token):
+    """
+    Returns an omero.client object from a valid token.  The
+    session the token refers to has had a join attempt made upon it.
+    """
+    omero_session_key = token[:token.find('@')]
+    host, port = token[token.find('@') + 1:].split(':')
+    client = omero.client(host, int(port))
+    try:
+        session = client.joinSession(omero_session_key)
+        session.detachOnDestroy()
+    except Exception:
+        pass
+    return client
 
 
 def getter():
     try:
-        client = login()
+        token = get_token()
+        client = login(token)
         try:
             client.getSession()
         except Exception:
             sys.exit('ERROR: Token is invalid!')
         finally:
             client.closeSession()
+        return token
     except FileNotFoundError:
         sys.exit('ERROR: No token available, `omero_user_token set` required!')
```

### Comparing `omero-user-token-0.2.1/omero_user_token/cli/omero_user_token.py` & `omero-user-token-0.3.0/omero_user_token/cli/omero_user_token.py`

 * *Files identical despite different names*

### Comparing `omero-user-token-0.2.1/omero_user_token.egg-info/PKG-INFO` & `omero-user-token-0.3.0/omero_user_token.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-user-token
-Version: 0.2.1
+Version: 0.3.0
 Summary: OMERO user token management system
 Home-page: https://github.com/glencoesoftware/omero-user-token
 Author: Glencoe Software, Inc.
 Author-email: info@glencoesoftware.com
 License: UNKNOWN
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `omero-user-token-0.2.1/setup.py` & `omero-user-token-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
       url='https://github.com/glencoesoftware/omero-user-token',
       packages=find_packages(),
       zip_safe=True,
       include_package_data=True,
       platforms='any',
       setup_requires=['flake8'],
       install_requires=[
-          'click==7.0',
+          'click>=7.0',
           'configparser==4.0.2',
           'omero-py>5.6',
       ],
       tests_require=[],
       cmdclass={'test': PyTest},
       data_files=[],
       entry_points={
```

### Comparing `omero-user-token-0.2.1/version.py` & `omero-user-token-0.3.0/version.py`

 * *Files identical despite different names*

